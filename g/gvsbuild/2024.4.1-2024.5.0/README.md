# Comparing `tmp/gvsbuild-2024.4.1.tar.gz` & `tmp/gvsbuild-2024.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gvsbuild-2024.4.1.tar", max compression
+gzip compressed data, was "gvsbuild-2024.5.0.tar", max compression
```

## Comparing `gvsbuild-2024.4.1.tar` & `gvsbuild-2024.5.0.tar`

### file list

```diff
@@ -1,931 +1,901 @@
--rw-r--r--   0        0        0     2185 2024-04-08 18:08:22.040712 gvsbuild-2024.4.1/AUTHORS.md
--rw-r--r--   0        0        0    18433 2024-04-08 18:08:22.040712 gvsbuild-2024.4.1/COPYING
--rw-r--r--   0        0        0       37 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/__init__.py
--rw-r--r--   0        0        0    16410 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/build.py
--rw-r--r--   0        0        0     7322 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/deps.py
--rw-r--r--   0        0        0     2121 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/groups.py
--rw-r--r--   0        0        0      244 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/info.py
--rw-r--r--   0        0        0     5581 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/list.py
--rw-r--r--   0        0        0     1977 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/main.py
--rw-r--r--   0        0        0     2609 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/outdated.py
--rw-r--r--   0        0        0      634 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/cairo/0001-fix-alloca-unresolved.patch
--rw-r--r--   0        0        0      213 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/check_utils.c
--rw-r--r--   0        0        0      537 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/check_utils.h
--rw-r--r--   0        0        0    18437 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/COPYING
--rw-r--r--   0        0        0     9831 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/meson.build
--rw-r--r--   0        0        0      175 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/test_atk.c
--rw-r--r--   0        0        0      167 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/test_cairo.c
--rw-r--r--   0        0        0      224 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/test_freetype2.c
--rw-r--r--   0        0        0      205 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/test_gdk-pixbuf.c
--rw-r--r--   0        0        0      170 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/test_glib.c
--rw-r--r--   0        0        0      183 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/test_jasper.c
--rw-r--r--   0        0        0      204 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/test_json_glib.c
--rw-r--r--   0        0        0      201 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/test_libarchive.c
--rw-r--r--   0        0        0      191 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/test_libcurl.c
--rw-r--r--   0        0        0      125 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/test_libffi.c
--rw-r--r--   0        0        0      193 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/test_libjpeg-turbo.c
--rw-r--r--   0        0        0      194 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/test_libjpeg.c
--rw-r--r--   0        0        0      188 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/test_libpng.c
--rw-r--r--   0        0        0      187 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/test_libtiff-4.c
--rw-r--r--   0        0        0      179 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/test_libxml2.c
--rw-r--r--   0        0        0      187 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/test_libyuv.c
--rw-r--r--   0        0        0      173 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/test_pango.c
--rw-r--r--   0        0        0      180 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/test_wing.c
--rw-r--r--   0        0        0      127 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/check-libs/test_zlib.c
--rw-r--r--   0        0        0     9047 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atkcomponent-example.vcxproj
--rw-r--r--   0        0        0     1020 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atkcomponent-example.vcxproj.filters
--rw-r--r--   0        0        0     9101 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atkeditabletext-example.vcxproj
--rw-r--r--   0        0        0     1023 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atkeditabletext-example.vcxproj.filters
--rw-r--r--   0        0        0     9557 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atkevents-example.vcxproj
--rw-r--r--   0        0        0     1017 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atkevents-example.vcxproj.filters
--rw-r--r--   0        0        0     9085 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atktext-example.vcxproj
--rw-r--r--   0        0        0      958 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atktext-example.vcxproj.filters
--rw-r--r--   0        0        0     9033 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/cally-clone-example.vcxproj
--rw-r--r--   0        0        0     1013 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/cally-clone-example.vcxproj.filters
--rw-r--r--   0        0        0     4196 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/clutter-build-defines.props
--rw-r--r--   0        0        0     6817 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/clutter-gen-srcs.props
--rw-r--r--   0        0        0    16612 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/clutter-install.props
--rw-r--r--   0        0        0    10665 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/clutter-install.vcxproj
--rw-r--r--   0        0        0     2510 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/clutter-version-paths.props
--rw-r--r--   0        0        0      405 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/clutter.bld.win32.win32
--rw-r--r--   0        0        0    29220 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/clutter.sln
--rw-r--r--   0        0        0    50071 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj
--rw-r--r--   0        0        0    15822 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj.filters
--rw-r--r--   0        0        0     2515 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj.filtersin
--rw-r--r--   0        0        0    41134 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxprojin
--rw-r--r--   0        0        0     1794 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/Makefile.am
--rw-r--r--   0        0        0    19138 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/Makefile.in
--rw-r--r--   0        0        0     4749 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/README.txt
--rw-r--r--   0        0        0     8818 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-cogl-perf.vcxproj
--rw-r--r--   0        0        0      532 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-cogl-perf.vcxproj.filters
--rw-r--r--   0        0        0    13484 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxproj
--rw-r--r--   0        0        0     5987 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxproj.filters
--rw-r--r--   0        0        0      464 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxproj.filtersin
--rw-r--r--   0        0        0     9685 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxprojin
--rw-r--r--   0        0        0     8719 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-picking-performance.vcxproj
--rw-r--r--   0        0        0      866 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-picking-performance.vcxproj.filters
--rw-r--r--   0        0        0     8897 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-picking.vcxproj
--rw-r--r--   0        0        0      530 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-picking.vcxproj.filters
--rw-r--r--   0        0        0     8822 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-random-text.vcxproj
--rw-r--r--   0        0        0      534 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-random-text.vcxproj.filters
--rw-r--r--   0        0        0     8728 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-hidden-performance.vcxproj
--rw-r--r--   0        0        0      871 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-hidden-performance.vcxproj.filters
--rw-r--r--   0        0        0     8738 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-interactive-performance.vcxproj
--rw-r--r--   0        0        0      876 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-interactive-performance.vcxproj.filters
--rw-r--r--   0        0        0     8724 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-mini-performance.vcxproj
--rw-r--r--   0        0        0      869 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-mini-performance.vcxproj.filters
--rw-r--r--   0        0        0     8715 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-performance.vcxproj
--rw-r--r--   0        0        0      864 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-performance.vcxproj.filters
--rw-r--r--   0        0        0     8724 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-pick-performance.vcxproj
--rw-r--r--   0        0        0      869 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-pick-performance.vcxproj.filters
--rw-r--r--   0        0        0     8722 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf-performance.vcxproj
--rw-r--r--   0        0        0      868 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf-performance.vcxproj.filters
--rw-r--r--   0        0        0     8818 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf.vcxproj
--rw-r--r--   0        0        0      532 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf.vcxproj.filters
--rw-r--r--   0        0        0     8809 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-text.vcxproj
--rw-r--r--   0        0        0      527 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-text.vcxproj.filters
--rw-r--r--   0        0        0     9047 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atkcomponent-example.vcxproj
--rw-r--r--   0        0        0     1020 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atkcomponent-example.vcxproj.filters
--rw-r--r--   0        0        0     9101 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atkeditabletext-example.vcxproj
--rw-r--r--   0        0        0     1023 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atkeditabletext-example.vcxproj.filters
--rw-r--r--   0        0        0     9557 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atkevents-example.vcxproj
--rw-r--r--   0        0        0     1017 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atkevents-example.vcxproj.filters
--rw-r--r--   0        0        0     9085 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atktext-example.vcxproj
--rw-r--r--   0        0        0      958 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atktext-example.vcxproj.filters
--rw-r--r--   0        0        0     9033 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/cally-clone-example.vcxproj
--rw-r--r--   0        0        0     1013 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/cally-clone-example.vcxproj.filters
--rw-r--r--   0        0        0     4196 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/clutter-build-defines.props
--rw-r--r--   0        0        0     6817 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/clutter-gen-srcs.props
--rw-r--r--   0        0        0    16612 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/clutter-install.props
--rw-r--r--   0        0        0    10665 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/clutter-install.vcxproj
--rw-r--r--   0        0        0     2510 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/clutter-version-paths.props
--rw-r--r--   0        0        0      405 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/clutter.bld.win32.win32
--rw-r--r--   0        0        0    27777 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/clutter.sln
--rw-r--r--   0        0        0    50071 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj
--rw-r--r--   0        0        0    15822 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj.filters
--rw-r--r--   0        0        0     2515 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj.filtersin
--rw-r--r--   0        0        0    41134 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxprojin
--rw-r--r--   0        0        0     1794 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/Makefile.am
--rw-r--r--   0        0        0    19138 2024-04-08 18:08:22.056332 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/Makefile.in
--rw-r--r--   0        0        0     4749 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/README.txt
--rw-r--r--   0        0        0     8818 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-cogl-perf.vcxproj
--rw-r--r--   0        0        0      532 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-cogl-perf.vcxproj.filters
--rw-r--r--   0        0        0     8719 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-picking-performance.vcxproj
--rw-r--r--   0        0        0      866 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-picking-performance.vcxproj.filters
--rw-r--r--   0        0        0     8897 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-picking.vcxproj
--rw-r--r--   0        0        0      530 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-picking.vcxproj.filters
--rw-r--r--   0        0        0     8822 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-random-text.vcxproj
--rw-r--r--   0        0        0      534 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-random-text.vcxproj.filters
--rw-r--r--   0        0        0     8728 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-hidden-performance.vcxproj
--rw-r--r--   0        0        0      871 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-hidden-performance.vcxproj.filters
--rw-r--r--   0        0        0     8738 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-interactive-performance.vcxproj
--rw-r--r--   0        0        0      876 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-interactive-performance.vcxproj.filters
--rw-r--r--   0        0        0     8724 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-mini-performance.vcxproj
--rw-r--r--   0        0        0      869 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-mini-performance.vcxproj.filters
--rw-r--r--   0        0        0     8715 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-performance.vcxproj
--rw-r--r--   0        0        0      864 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-performance.vcxproj.filters
--rw-r--r--   0        0        0     8724 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-pick-performance.vcxproj
--rw-r--r--   0        0        0      869 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-pick-performance.vcxproj.filters
--rw-r--r--   0        0        0     8722 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf-performance.vcxproj
--rw-r--r--   0        0        0      868 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf-performance.vcxproj.filters
--rw-r--r--   0        0        0     8818 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf.vcxproj
--rw-r--r--   0        0        0      532 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf.vcxproj.filters
--rw-r--r--   0        0        0     8809 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-text.vcxproj
--rw-r--r--   0        0        0      527 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-text.vcxproj.filters
--rw-r--r--   0        0        0     9126 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atkcomponent-example.vcxproj
--rw-r--r--   0        0        0     1020 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atkcomponent-example.vcxproj.filters
--rw-r--r--   0        0        0     9180 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atkeditabletext-example.vcxproj
--rw-r--r--   0        0        0     1023 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atkeditabletext-example.vcxproj.filters
--rw-r--r--   0        0        0     9636 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atkevents-example.vcxproj
--rw-r--r--   0        0        0     1017 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atkevents-example.vcxproj.filters
--rw-r--r--   0        0        0     9164 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atktext-example.vcxproj
--rw-r--r--   0        0        0      958 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atktext-example.vcxproj.filters
--rw-r--r--   0        0        0     9112 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/cally-clone-example.vcxproj
--rw-r--r--   0        0        0     1013 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/cally-clone-example.vcxproj.filters
--rw-r--r--   0        0        0     4196 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/clutter-build-defines.props
--rw-r--r--   0        0        0     6817 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/clutter-gen-srcs.props
--rw-r--r--   0        0        0    16612 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/clutter-install.props
--rw-r--r--   0        0        0    10744 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/clutter-install.vcxproj
--rw-r--r--   0        0        0     2510 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/clutter-version-paths.props
--rw-r--r--   0        0        0      405 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/clutter.bld.win32.win32
--rw-r--r--   0        0        0    27909 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/clutter.sln
--rw-r--r--   0        0        0    50150 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj
--rw-r--r--   0        0        0    15822 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj.filters
--rw-r--r--   0        0        0     2515 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj.filtersin
--rw-r--r--   0        0        0    41134 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxprojin
--rw-r--r--   0        0        0     1794 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/Makefile.am
--rw-r--r--   0        0        0    19138 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/Makefile.in
--rw-r--r--   0        0        0     4749 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/README.txt
--rw-r--r--   0        0        0     8897 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-cogl-perf.vcxproj
--rw-r--r--   0        0        0      532 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-cogl-perf.vcxproj.filters
--rw-r--r--   0        0        0     8798 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-picking-performance.vcxproj
--rw-r--r--   0        0        0      866 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-picking-performance.vcxproj.filters
--rw-r--r--   0        0        0     8976 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-picking.vcxproj
--rw-r--r--   0        0        0      530 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-picking.vcxproj.filters
--rw-r--r--   0        0        0     8901 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-random-text.vcxproj
--rw-r--r--   0        0        0      534 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-random-text.vcxproj.filters
--rw-r--r--   0        0        0     8807 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-hidden-performance.vcxproj
--rw-r--r--   0        0        0      871 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-hidden-performance.vcxproj.filters
--rw-r--r--   0        0        0     8817 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-interactive-performance.vcxproj
--rw-r--r--   0        0        0      876 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-interactive-performance.vcxproj.filters
--rw-r--r--   0        0        0     8803 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-mini-performance.vcxproj
--rw-r--r--   0        0        0      869 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-mini-performance.vcxproj.filters
--rw-r--r--   0        0        0     8794 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-performance.vcxproj
--rw-r--r--   0        0        0      864 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-performance.vcxproj.filters
--rw-r--r--   0        0        0     8803 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-pick-performance.vcxproj
--rw-r--r--   0        0        0      869 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-pick-performance.vcxproj.filters
--rw-r--r--   0        0        0     8801 2024-04-08 18:08:22.071959 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf-performance.vcxproj
--rw-r--r--   0        0        0      868 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf-performance.vcxproj.filters
--rw-r--r--   0        0        0     8897 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf.vcxproj
--rw-r--r--   0        0        0      532 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf.vcxproj.filters
--rw-r--r--   0        0        0     8888 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-text.vcxproj
--rw-r--r--   0        0        0      527 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-text.vcxproj.filters
--rw-r--r--   0        0        0      316 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/001-cogl-missing-symbols.patch
--rw-r--r--   0        0        0      339 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/002-cogl-pango-missing-symbols.patch
--rw-r--r--   0        0        0     3533 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-build-defines.props
--rw-r--r--   0        0        0    10205 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-crate.vcxproj
--rw-r--r--   0        0        0      519 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-crate.vcxproj.filters
--rw-r--r--   0        0        0     5411 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-gen-srcs.props
--rw-r--r--   0        0        0     8918 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-hello.vcxproj
--rw-r--r--   0        0        0      519 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-hello.vcxproj.filters
--rw-r--r--   0        0        0     9239 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-info.vcxproj
--rw-r--r--   0        0        0      518 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-info.vcxproj.filters
--rw-r--r--   0        0        0    10887 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-install.props
--rw-r--r--   0        0        0    14290 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-install.vcxproj
--rw-r--r--   0        0        0     8788 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-msaa.vcxproj
--rw-r--r--   0        0        0      518 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-msaa.vcxproj.filters
--rw-r--r--   0        0        0    12851 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj
--rw-r--r--   0        0        0     1402 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj.filters
--rw-r--r--   0        0        0      789 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj.filtersin
--rw-r--r--   0        0        0    11992 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxprojin
--rw-r--r--   0        0        0    16347 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj
--rw-r--r--   0        0        0     2531 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj.filters
--rw-r--r--   0        0        0     1267 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj.filtersin
--rw-r--r--   0        0        0    15092 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxprojin
--rw-r--r--   0        0        0     9571 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-sdl2-hello.vcxproj
--rw-r--r--   0        0        0      522 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-sdl2-hello.vcxproj.filters
--rw-r--r--   0        0        0     2482 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-version-paths.props
--rw-r--r--   0        0        0    12059 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl.sln
--rw-r--r--   0        0        0    48250 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj
--rw-r--r--   0        0        0    14547 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj.filters
--rw-r--r--   0        0        0     3009 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj.filtersin
--rw-r--r--   0        0        0    41403 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxprojin
--rw-r--r--   0        0        0      919 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/Makefile.am
--rw-r--r--   0        0        0    19171 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/Makefile.in
--rw-r--r--   0        0        0     4783 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/README.txt
--rw-r--r--   0        0        0    13862 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj
--rw-r--r--   0        0        0     5574 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj.filters
--rw-r--r--   0        0        0      563 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj.filtersin
--rw-r--r--   0        0        0     9905 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxprojin
--rw-r--r--   0        0        0     3533 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-build-defines.props
--rw-r--r--   0        0        0    10205 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-crate.vcxproj
--rw-r--r--   0        0        0      519 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-crate.vcxproj.filters
--rw-r--r--   0        0        0     5411 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-gen-srcs.props
--rw-r--r--   0        0        0     8918 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-hello.vcxproj
--rw-r--r--   0        0        0      519 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-hello.vcxproj.filters
--rw-r--r--   0        0        0     9239 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-info.vcxproj
--rw-r--r--   0        0        0      518 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-info.vcxproj.filters
--rw-r--r--   0        0        0    10887 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-install.props
--rw-r--r--   0        0        0    14290 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-install.vcxproj
--rw-r--r--   0        0        0     8788 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-msaa.vcxproj
--rw-r--r--   0        0        0      518 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-msaa.vcxproj.filters
--rw-r--r--   0        0        0    12851 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj
--rw-r--r--   0        0        0     1402 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj.filters
--rw-r--r--   0        0        0      789 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj.filtersin
--rw-r--r--   0        0        0    11992 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxprojin
--rw-r--r--   0        0        0    16347 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj
--rw-r--r--   0        0        0     2531 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj.filters
--rw-r--r--   0        0        0     1267 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj.filtersin
--rw-r--r--   0        0        0    15092 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxprojin
--rw-r--r--   0        0        0     9571 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-sdl2-hello.vcxproj
--rw-r--r--   0        0        0      522 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-sdl2-hello.vcxproj.filters
--rw-r--r--   0        0        0     2482 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-version-paths.props
--rw-r--r--   0        0        0    12059 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl.sln
--rw-r--r--   0        0        0    48250 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj
--rw-r--r--   0        0        0    14547 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj.filters
--rw-r--r--   0        0        0     3009 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj.filtersin
--rw-r--r--   0        0        0    41403 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxprojin
--rw-r--r--   0        0        0      919 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/Makefile.am
--rw-r--r--   0        0        0    19171 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/Makefile.in
--rw-r--r--   0        0        0     4783 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/README.txt
--rw-r--r--   0        0        0    13862 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj
--rw-r--r--   0        0        0     5574 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj.filters
--rw-r--r--   0        0        0      563 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj.filtersin
--rw-r--r--   0        0        0     9905 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxprojin
--rw-r--r--   0        0        0     3533 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-build-defines.props
--rw-r--r--   0        0        0    10284 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-crate.vcxproj
--rw-r--r--   0        0        0      519 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-crate.vcxproj.filters
--rw-r--r--   0        0        0     5411 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-gen-srcs.props
--rw-r--r--   0        0        0     8997 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-hello.vcxproj
--rw-r--r--   0        0        0      519 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-hello.vcxproj.filters
--rw-r--r--   0        0        0     9318 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-info.vcxproj
--rw-r--r--   0        0        0      518 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-info.vcxproj.filters
--rw-r--r--   0        0        0    10887 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-install.props
--rw-r--r--   0        0        0    14369 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-install.vcxproj
--rw-r--r--   0        0        0     8788 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-msaa.vcxproj
--rw-r--r--   0        0        0      518 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-msaa.vcxproj.filters
--rw-r--r--   0        0        0    12930 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj
--rw-r--r--   0        0        0     1402 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj.filters
--rw-r--r--   0        0        0      789 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj.filtersin
--rw-r--r--   0        0        0    11992 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxprojin
--rw-r--r--   0        0        0    16426 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj
--rw-r--r--   0        0        0     2531 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj.filters
--rw-r--r--   0        0        0     1267 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj.filtersin
--rw-r--r--   0        0        0    15092 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxprojin
--rw-r--r--   0        0        0     9571 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-sdl2-hello.vcxproj
--rw-r--r--   0        0        0      522 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-sdl2-hello.vcxproj.filters
--rw-r--r--   0        0        0     2482 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-version-paths.props
--rw-r--r--   0        0        0    12161 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl.sln
--rw-r--r--   0        0        0    48329 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj
--rw-r--r--   0        0        0    14547 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj.filters
--rw-r--r--   0        0        0     3009 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj.filtersin
--rw-r--r--   0        0        0    41403 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxprojin
--rw-r--r--   0        0        0      919 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/Makefile.am
--rw-r--r--   0        0        0    19171 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/Makefile.in
--rw-r--r--   0        0        0     4783 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/README.txt
--rw-r--r--   0        0        0    13941 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj
--rw-r--r--   0        0        0     5574 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj.filters
--rw-r--r--   0        0        0      563 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj.filtersin
--rw-r--r--   0        0        0     9905 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxprojin
--rw-r--r--   0        0        0   244356 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/GL/glcorearb.h
--rw-r--r--   0        0        0   810011 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/GL/glext.h
--rw-r--r--   0        0        0    48113 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/GL/glxext.h
--rw-r--r--   0        0        0    44095 2024-04-08 18:08:22.087581 gvsbuild-2024.4.1/gvsbuild/patches/cogl/GL/wglext.h
--rw-r--r--   0        0        0     1121 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cyrus-sasl/0001-Add-MIT-Kerberos-as-GSSAPI-provider.patch
--rw-r--r--   0        0        0     1060 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cyrus-sasl/0001-Fix-openssl-libs-to-point-to-the-new-openssl-1.1.1-n.patch
--rw-r--r--   0        0        0      740 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cyrus-sasl/0001-fix-snprintf-macro.patch
--rw-r--r--   0        0        0     1135 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cyrus-sasl/0002-Provide-a-compile-option-for-32-64-gssapi.patch
--rw-r--r--   0        0        0     1045 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cyrus-sasl/include/md5global.h
--rw-r--r--   0        0        0      312 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/cyrus-sasl/pc-files/libsasl2.pc
--rw-r--r--   0        0        0      418 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/enchant/src/config.h
--rw-r--r--   0        0        0      660 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/enchant/src/libenchant.rc
--rw-r--r--   0        0        0    17426 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/enchant/src/makefile.mak
--rw-r--r--   0        0        0      754 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/expat/0001-CMakeLists-do-not-add-postfix-d-in-debug-builds.patch
--rw-r--r--   0        0        0     2152 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/ffmpeg/build/build.sh
--rw-r--r--   0        0        0      787 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/freetype/0001-meson-in-shared-libraries-we-need-to-export-the-meth.patch
--rw-r--r--   0        0        0     3296 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/gettext/gettext-runtime-c99.patch
--rw-r--r--   0        0        0    33686 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/gettext/gettext-tools-c99.patch
--rw-r--r--   0        0        0      367 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/gettext/gettext-tools-gnulib-memset.patch
--rw-r--r--   0        0        0     9543 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/gettext/libtextstyle-c99.patch
--rw-r--r--   0        0        0     3065 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/alloca.h
--rw-r--r--   0        0        0     7623 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/errno.h
--rw-r--r--   0        0        0    33617 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/fcntl.h
--rw-r--r--   0        0        0     2128 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/getopt-cdefs.h
--rw-r--r--   0        0        0     3334 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/getopt.h
--rw-r--r--   0        0        0    26308 2024-04-08 18:08:22.103207 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/iconv.h
--rw-r--r--   0        0        0    43681 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/inttypes.h
--rw-r--r--   0        0        0    27515 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/langinfo.h
--rw-r--r--   0        0        0     4377 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/limits.h
--rw-r--r--   0        0        0    32044 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/locale.h
--rw-r--r--   0        0        0    37498 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/signal.h
--rw-r--r--   0        0        0     4322 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/stddef.h
--rw-r--r--   0        0        0    63279 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/stdlib.h
--rw-r--r--   0        0        0    63715 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/string.h
--rw-r--r--   0        0        0    44998 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/sys/stat.h
--rw-r--r--   0        0        0     3250 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/sys/types.h
--rw-r--r--   0        0        0    35655 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/time.h
--rw-r--r--   0        0        0    81450 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unistd.h
--rw-r--r--   0        0        0    24256 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unistr.h
--rw-r--r--   0        0        0     2201 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unitypes.h
--rw-r--r--   0        0        0     2239 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/uniwidth.h
--rw-r--r--   0        0        0    62421 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/wchar.h
--rw-r--r--   0        0        0    38906 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/wctype.h
--rw-r--r--   0        0        0    20126 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/intl/libgnuintl.h
--rw-r--r--   0        0        0    19299 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/intl/libintl.h
--rw-r--r--   0        0        0     3088 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/alloca.h
--rw-r--r--   0        0        0     2708 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/autosprintf.h
--rw-r--r--   0        0        0     7648 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/errno.h
--rw-r--r--   0        0        0     3065 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/alloca.h
--rw-r--r--   0        0        0     2093 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/byteswap.h
--rw-r--r--   0        0        0    22716 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/ctype.h
--rw-r--r--   0        0        0    30933 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/dirent.h
--rw-r--r--   0        0        0     7623 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/errno.h
--rw-r--r--   0        0        0    33701 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/fcntl.h
--rw-r--r--   0        0        0    25904 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/fnmatch.h
--rw-r--r--   0        0        0     2128 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/getopt-cdefs.h
--rw-r--r--   0        0        0     3334 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/getopt.h
--rw-r--r--   0        0        0    26308 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/iconv.h
--rw-r--r--   0        0        0    43508 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/inttypes.h
--rw-r--r--   0        0        0    27538 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/langinfo.h
--rw-r--r--   0        0        0     4658 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/c14n.h
--rw-r--r--   0        0        0     6506 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/catalog.h
--rw-r--r--   0        0        0     6869 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/chvalid.h
--rw-r--r--   0        0        0     6788 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/debugXML.h
--rw-r--r--   0        0        0     3460 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/dict.h
--rw-r--r--   0        0        0     4672 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/DOCBparser.h
--rw-r--r--   0        0        0    10171 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/encoding.h
--rw-r--r--   0        0        0     6282 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/entities.h
--rw-r--r--   0        0        0    16639 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/globals.h
--rw-r--r--   0        0        0     8258 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/hash.h
--rw-r--r--   0        0        0    11135 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/HTMLparser.h
--rw-r--r--   0        0        0     5212 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/HTMLtree.h
--rw-r--r--   0        0        0     4904 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/list.h
--rw-r--r--   0        0        0     5340 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/nanoftp.h
--rw-r--r--   0        0        0     3505 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/nanohttp.h
--rw-r--r--   0        0        0    42377 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/parser.h
--rw-r--r--   0        0        0    19481 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/parserInternals.h
--rw-r--r--   0        0        0     4105 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/pattern.h
--rw-r--r--   0        0        0     7632 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/relaxng.h
--rw-r--r--   0        0        0     5931 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/SAX.h
--rw-r--r--   0        0        0     6544 2024-04-08 18:08:22.118917 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/SAX2.h
--rw-r--r--   0        0        0    28618 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/schemasInternals.h
--rw-r--r--   0        0        0     5930 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/schematron.h
--rw-r--r--   0        0        0     3466 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/threads.h
--rw-r--r--   0        0        0    40837 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/tree.h
--rw-r--r--   0        0        0     4177 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/uri.h
--rw-r--r--   0        0        0    15497 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/valid.h
--rw-r--r--   0        0        0     4515 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xinclude.h
--rw-r--r--   0        0        0     6648 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xlink.h
--rw-r--r--   0        0        0     5521 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlautomata.h
--rw-r--r--   0        0        0    39148 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlerror.h
--rw-r--r--   0        0        0     5514 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlexports.h
--rw-r--r--   0        0        0    12396 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlIO.h
--rw-r--r--   0        0        0     7586 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlmemory.h
--rw-r--r--   0        0        0     2646 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlmodule.h
--rw-r--r--   0        0        0    14454 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlreader.h
--rw-r--r--   0        0        0     7099 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlregexp.h
--rw-r--r--   0        0        0     3844 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlsave.h
--rw-r--r--   0        0        0     8732 2024-04-08 18:08:22.128941 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlschemas.h
--rw-r--r--   0        0        0     6409 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlschemastypes.h
--rw-r--r--   0        0        0     7070 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlstring.h
--rw-r--r--   0        0        0    11675 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlunicode.h
--rw-r--r--   0        0        0    10024 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlversion.h
--rw-r--r--   0        0        0    23172 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlwriter.h
--rw-r--r--   0        0        0    18374 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpath.h
--rw-r--r--   0        0        0    21404 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpathInternals.h
--rw-r--r--   0        0        0     4892 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpointer.h
--rw-r--r--   0        0        0     4377 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/limits.h
--rw-r--r--   0        0        0    32067 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/locale.h
--rw-r--r--   0        0        0     1209 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/omp.h
--rw-r--r--   0        0        0    23409 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sched.h
--rw-r--r--   0        0        0    37554 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/signal.h
--rw-r--r--   0        0        0    61302 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/spawn.h
--rw-r--r--   0        0        0     4298 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/stddef.h
--rw-r--r--   0        0        0    63335 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/stdlib.h
--rw-r--r--   0        0        0    63743 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/string.h
--rw-r--r--   0        0        0    24900 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/random.h
--rw-r--r--   0        0        0    32949 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/select.h
--rw-r--r--   0        0        0    44998 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/stat.h
--rw-r--r--   0        0        0    29890 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/time.h
--rw-r--r--   0        0        0     3250 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/types.h
--rw-r--r--   0        0        0    24835 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/wait.h
--rw-r--r--   0        0        0    35681 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/time.h
--rw-r--r--   0        0        0     7748 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniconv.h
--rw-r--r--   0        0        0    42529 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unictype.h
--rw-r--r--   0        0        0     4287 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unilbrk.h
--rw-r--r--   0        0        0     1625 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniname.h
--rw-r--r--   0        0        0    81730 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unistd.h
--rw-r--r--   0        0        0    24256 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unistr.h
--rw-r--r--   0        0        0     2201 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unitypes.h
--rw-r--r--   0        0        0     2239 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniwidth.h
--rw-r--r--   0        0        0    24592 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/utime.h
--rw-r--r--   0        0        0    62584 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/wchar.h
--rw-r--r--   0        0        0    38904 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/wctype.h
--rw-r--r--   0        0        0    27214 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/arpa/inet.h
--rw-r--r--   0        0        0     1287 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/netinet/in.h
--rw-r--r--   0        0        0    91289 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/pthread.h
--rw-r--r--   0        0        0     4873 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/stdalign.h
--rw-r--r--   0        0        0    23344 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/ioctl.h
--rw-r--r--   0        0        0    46391 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/socket.h
--rw-r--r--   0        0        0     1629 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/uio.h
--rw-r--r--   0        0        0     3065 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/alloca.h
--rw-r--r--   0        0        0     7648 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/errno.h
--rw-r--r--   0        0        0    33726 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/fcntl.h
--rw-r--r--   0        0        0    17539 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/gettext-po.h
--rw-r--r--   0        0        0    26333 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/iconv.h
--rw-r--r--   0        0        0    43508 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/inttypes.h
--rw-r--r--   0        0        0     4402 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/limits.h
--rw-r--r--   0        0        0    32092 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/locale.h
--rw-r--r--   0        0        0    37579 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/signal.h
--rw-r--r--   0        0        0     4333 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/stddef.h
--rw-r--r--   0        0        0    63360 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/stdlib.h
--rw-r--r--   0        0        0    63768 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/string.h
--rw-r--r--   0        0        0    45023 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/sys/stat.h
--rw-r--r--   0        0        0     3275 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/sys/types.h
--rw-r--r--   0        0        0    13023 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/textstyle.h
--rw-r--r--   0        0        0    35677 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/time.h
--rw-r--r--   0        0        0     7748 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/uniconv.h
--rw-r--r--   0        0        0    42529 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unictype.h
--rw-r--r--   0        0        0     4287 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unilbrk.h
--rw-r--r--   0        0        0    81764 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unistd.h
--rw-r--r--   0        0        0    24256 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unistr.h
--rw-r--r--   0        0        0     2201 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unitypes.h
--rw-r--r--   0        0        0     2239 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/uniwidth.h
--rw-r--r--   0        0        0    62609 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/wchar.h
--rw-r--r--   0        0        0    38929 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/wctype.h
--rw-r--r--   0        0        0    27563 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgrep/langinfo.h
--rw-r--r--   0        0        0     4432 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/stdbool.h
--rw-r--r--   0        0        0     1392 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/version.h
--rw-r--r--   0        0        0     1230 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/woe32dll.h
--rw-r--r--   0        0        0    23446 2024-04-08 18:08:22.134964 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle.h
--rw-r--r--   0        0        0     3065 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/alloca.h
--rw-r--r--   0        0        0     7643 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/errno.h
--rw-r--r--   0        0        0    33637 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/fcntl.h
--rw-r--r--   0        0        0     4938 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/ghash.h
--rw-r--r--   0        0        0     5545 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/glist.h
--rw-r--r--   0        0        0     9729 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gmacros.h
--rw-r--r--   0        0        0     2028 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gprimes.h
--rw-r--r--   0        0        0     2257 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gprintfint.h
--rw-r--r--   0        0        0    10124 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gstrfuncs.h
--rw-r--r--   0        0        0     6212 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gstring.h
--rw-r--r--   0        0        0    16052 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gtypes.h
--rw-r--r--   0        0        0     2765 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib.h
--rw-r--r--   0        0        0     6279 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glibconfig.h
--rw-r--r--   0        0        0    43677 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/inttypes.h
--rw-r--r--   0        0        0     4658 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/c14n.h
--rw-r--r--   0        0        0     6506 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/catalog.h
--rw-r--r--   0        0        0     6869 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/chvalid.h
--rw-r--r--   0        0        0     6788 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/debugXML.h
--rw-r--r--   0        0        0     3460 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/dict.h
--rw-r--r--   0        0        0     4672 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/DOCBparser.h
--rw-r--r--   0        0        0    10171 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/encoding.h
--rw-r--r--   0        0        0     6282 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/entities.h
--rw-r--r--   0        0        0    16639 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/globals.h
--rw-r--r--   0        0        0     8258 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/hash.h
--rw-r--r--   0        0        0    11135 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/HTMLparser.h
--rw-r--r--   0        0        0     5212 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/HTMLtree.h
--rw-r--r--   0        0        0     4904 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/list.h
--rw-r--r--   0        0        0     5340 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/nanoftp.h
--rw-r--r--   0        0        0     3505 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/nanohttp.h
--rw-r--r--   0        0        0    42377 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/parser.h
--rw-r--r--   0        0        0    19481 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/parserInternals.h
--rw-r--r--   0        0        0     4105 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/pattern.h
--rw-r--r--   0        0        0     7632 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/relaxng.h
--rw-r--r--   0        0        0     5931 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/SAX.h
--rw-r--r--   0        0        0     6544 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/SAX2.h
--rw-r--r--   0        0        0    28618 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/schemasInternals.h
--rw-r--r--   0        0        0     5930 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/schematron.h
--rw-r--r--   0        0        0     3466 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/threads.h
--rw-r--r--   0        0        0    40837 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/tree.h
--rw-r--r--   0        0        0     4177 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/uri.h
--rw-r--r--   0        0        0    15497 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/valid.h
--rw-r--r--   0        0        0     4515 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xinclude.h
--rw-r--r--   0        0        0     6648 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xlink.h
--rw-r--r--   0        0        0     5521 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlautomata.h
--rw-r--r--   0        0        0    39148 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlerror.h
--rw-r--r--   0        0        0     5514 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlexports.h
--rw-r--r--   0        0        0    12396 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlIO.h
--rw-r--r--   0        0        0     7586 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlmemory.h
--rw-r--r--   0        0        0     2646 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlmodule.h
--rw-r--r--   0        0        0    14454 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlreader.h
--rw-r--r--   0        0        0     7099 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlregexp.h
--rw-r--r--   0        0        0     3844 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlsave.h
--rw-r--r--   0        0        0     8732 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlschemas.h
--rw-r--r--   0        0        0     6409 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlschemastypes.h
--rw-r--r--   0        0        0     7070 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlstring.h
--rw-r--r--   0        0        0    11675 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlunicode.h
--rw-r--r--   0        0        0    10024 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlversion.h
--rw-r--r--   0        0        0    23172 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlwriter.h
--rw-r--r--   0        0        0    18374 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpath.h
--rw-r--r--   0        0        0    21404 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpathInternals.h
--rw-r--r--   0        0        0     4892 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpointer.h
--rw-r--r--   0        0        0     4396 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/limits.h
--rw-r--r--   0        0        0    37518 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/signal.h
--rw-r--r--   0        0        0     4873 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdalign.h
--rw-r--r--   0        0        0     4326 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stddef.h
--rw-r--r--   0        0        0    23157 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdint.h
--rw-r--r--   0        0        0    63299 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdlib.h
--rw-r--r--   0        0        0    63735 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/string.h
--rw-r--r--   0        0        0    46251 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/socket.h
--rw-r--r--   0        0        0    45018 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/stat.h
--rw-r--r--   0        0        0    29922 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/time.h
--rw-r--r--   0        0        0     3272 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/types.h
--rw-r--r--   0        0        0     1649 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/uio.h
--rw-r--r--   0        0        0     4432 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/stdbool.h
--rw-r--r--   0        0        0     1392 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/version.h
--rw-r--r--   0        0        0     1230 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/woe32dll.h
--rw-r--r--   0        0        0    35661 2024-04-08 18:08:22.150616 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/time.h
--rw-r--r--   0        0        0    81477 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unistd.h
--rw-r--r--   0        0        0    24256 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unistr.h
--rw-r--r--   0        0        0     2201 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unitypes.h
--rw-r--r--   0        0        0    62439 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/wchar.h
--rw-r--r--   0        0        0    54409 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/config.h
--rw-r--r--   0        0        0    23289 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/gnulib-lib/stdint.h
--rw-r--r--   0        0        0    75068 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/gnulib-lib/stdio.h
--rw-r--r--   0        0        0    97908 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/config.h
--rw-r--r--   0        0        0     1932 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/configmake.h
--rw-r--r--   0        0        0    93885 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/math.h
--rw-r--r--   0        0        0    23289 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/stdint.h
--rw-r--r--   0        0        0    75124 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/stdio.h
--rw-r--r--   0        0        0    22207 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/config.h
--rw-r--r--   0        0        0    23319 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/stdint.h
--rw-r--r--   0        0        0    75149 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/stdio.h
--rw-r--r--   0        0        0    49880 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/config.h
--rw-r--r--   0        0        0    78389 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/config.h
--rw-r--r--   0        0        0    93905 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/math.h
--rw-r--r--   0        0        0    75079 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/stdio.h
--rw-r--r--   0        0        0    54408 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/config.h
--rw-r--r--   0        0        0    23289 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/gnulib-lib/stdint.h
--rw-r--r--   0        0        0    75065 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/gnulib-lib/stdio.h
--rw-r--r--   0        0        0    97907 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/config.h
--rw-r--r--   0        0        0     1932 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/configmake.h
--rw-r--r--   0        0        0    93885 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/math.h
--rw-r--r--   0        0        0    23289 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/stdint.h
--rw-r--r--   0        0        0    75121 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/stdio.h
--rw-r--r--   0        0        0    22207 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/config.h
--rw-r--r--   0        0        0    23319 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/stdint.h
--rw-r--r--   0        0        0    75146 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/stdio.h
--rw-r--r--   0        0        0    49880 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/config.h
--rw-r--r--   0        0        0    78389 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/config.h
--rw-r--r--   0        0        0    93905 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/math.h
--rw-r--r--   0        0        0    75079 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/stdio.h
--rw-r--r--   0        0        0    54410 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/config.h
--rw-r--r--   0        0        0    23133 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/gnulib-lib/stdint.h
--rw-r--r--   0        0        0    74955 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/gnulib-lib/stdio.h
--rw-r--r--   0        0        0    97906 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/config.h
--rw-r--r--   0        0        0     1932 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/configmake.h
--rw-r--r--   0        0        0    93830 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/math.h
--rw-r--r--   0        0        0    23133 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/stdint.h
--rw-r--r--   0        0        0    75011 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/stdio.h
--rw-r--r--   0        0        0    21997 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/config.h
--rw-r--r--   0        0        0    23163 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/stdint.h
--rw-r--r--   0        0        0    75036 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/stdio.h
--rw-r--r--   0        0        0    49879 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/config.h
--rw-r--r--   0        0        0    78389 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/config.h
--rw-r--r--   0        0        0    93850 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/math.h
--rw-r--r--   0        0        0    74969 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/stdio.h
--rw-r--r--   0        0        0    54407 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/config.h
--rw-r--r--   0        0        0    23133 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/gnulib-lib/stdint.h
--rw-r--r--   0        0        0    74958 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/gnulib-lib/stdio.h
--rw-r--r--   0        0        0    97900 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/config.h
--rw-r--r--   0        0        0     1984 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/configmake.h
--rw-r--r--   0        0        0    93830 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/math.h
--rw-r--r--   0        0        0    23133 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/stdint.h
--rw-r--r--   0        0        0    75014 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/stdio.h
--rw-r--r--   0        0        0    22207 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/config.h
--rw-r--r--   0        0        0    23163 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/stdint.h
--rw-r--r--   0        0        0    75039 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/stdio.h
--rw-r--r--   0        0        0    49882 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/config.h
--rw-r--r--   0        0        0    78389 2024-04-08 18:08:22.166242 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/config.h
--rw-r--r--   0        0        0    93850 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/math.h
--rw-r--r--   0        0        0    74969 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/stdio.h
--rw-r--r--   0        0        0    54406 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/config.h
--rw-r--r--   0        0        0    23133 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/gnulib-lib/stdint.h
--rw-r--r--   0        0        0    74955 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/gnulib-lib/stdio.h
--rw-r--r--   0        0        0    97945 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/config.h
--rw-r--r--   0        0        0     1984 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/configmake.h
--rw-r--r--   0        0        0    93830 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/math.h
--rw-r--r--   0        0        0    23133 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/stdint.h
--rw-r--r--   0        0        0    75011 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/stdio.h
--rw-r--r--   0        0        0    22207 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/config.h
--rw-r--r--   0        0        0    23163 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/stdint.h
--rw-r--r--   0        0        0    75036 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/stdio.h
--rw-r--r--   0        0        0    49882 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/config.h
--rw-r--r--   0        0        0    78389 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/config.h
--rw-r--r--   0        0        0    93850 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/math.h
--rw-r--r--   0        0        0    74969 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/stdio.h
--rw-r--r--   0        0        0    22956 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/build-rules-msvc.mak
--rw-r--r--   0        0        0     6490 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/config-msvc.mak
--rw-r--r--   0        0        0    16869 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/create-lists-msvc.mak
--rwxr-xr-x   0        0        0      846 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/create-lists.bat
--rw-r--r--   0        0        0     5708 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/detectenv-msvc.mak
--rw-r--r--   0        0        0      772 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/generate-msvc.mak
--rw-r--r--   0        0        0     4576 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/gettext-runtime-sources.mk
--rw-r--r--   0        0        0     8982 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/gettext-tools-sources.mk
--rw-r--r--   0        0        0     2466 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/libgettextlib.def
--rw-r--r--   0        0        0     2852 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/libgettextsrc.def
--rw-r--r--   0        0        0     3788 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/libtextstyle-sources.mk
--rw-r--r--   0        0        0     2635 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/libtextstyle.def
--rw-r--r--   0        0        0     1051 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/Makefile.vc
--rw-r--r--   0        0        0     1582 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/glib/001-glib-package-installation-directory.patch
--rw-r--r--   0        0        0     3238 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/glib/002-gir-scanner-dll-not-found.patch
--rw-r--r--   0        0        0     1582 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/glib-base/001-glib-package-installation-directory.patch
--rw-r--r--   0        0        0     3238 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/glib-base/002-gir-scanner-dll-not-found.patch
--rw-r--r--   0        0        0       30 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/glib-py-wrapper/glib-genmarshal.config
--rw-r--r--   0        0        0       27 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/glib-py-wrapper/glib-mkenums.config
--rw-r--r--   0        0        0     1123 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/glib-py-wrapper/glib-py-wrapper.c
--rw-r--r--   0        0        0      394 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/glib-py-wrapper/meson.build
--rw-r--r--   0        0        0      611 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gobject-introspection/001-incorrect-giscanner-path.patch
--rw-r--r--   0        0        0     1468 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gsettings-desktop-schemas/0001-build-win32-replace.py-Fix-replacing-items-in-files-.patch
--rw-r--r--   0        0        0      759 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gsettings-desktop-schemas/0002-glib-mkenums-python.patch
--rw-r--r--   0        0        0     2083 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gst-plugins-bad/wasapisink-reduce-buffer-latency.patch
--rw-r--r--   0        0        0     1668 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gst-python/001-fix-instsoname-not-found.patch
--rw-r--r--   0        0        0     1958 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/0001-GDK-W32-Remove-WS_EX_LAYERED-from-an-opaque-window.patch
--rw-r--r--   0        0        0     1186 2024-04-08 18:08:22.181866 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/61162225f712df648f38fd12bc0817cfa9f79a64.patch
--rw-r--r--   0        0        0     1920 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/bfdac2f70e005b2504cc3f4ebbdab328974d005a.patch
--rw-r--r--   0        0        0     1956 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/introspection.body.mak
--rw-r--r--   0        0        0     2185 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs12/gtk-version-paths.props
--rw-r--r--   0        0        0     2185 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs14/gtk-version-paths.props
--rw-r--r--   0        0        0    10679 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gailutil.vcxproj
--rw-r--r--   0        0        0     1080 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gailutil.vcxproj.filters
--rw-r--r--   0        0        0    11397 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gdk-win32.vcxproj
--rw-r--r--   0        0        0     3760 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gdk-win32.vcxproj.filters
--rw-r--r--   0        0        0    13364 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gdk.vcxproj
--rw-r--r--   0        0        0     4222 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gdk.vcxproj.filters
--rw-r--r--   0        0        0     6519 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk+.sln
--rw-r--r--   0        0        0     3640 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-build-defines.props
--rw-r--r--   0        0        0    12279 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-demo.vcxproj
--rw-r--r--   0        0        0     4640 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-demo.vcxproj.filters
--rw-r--r--   0        0        0     1962 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-gen-srcs.props
--rw-r--r--   0        0        0    23804 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-install.props
--rw-r--r--   0        0        0     7938 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-install.vcxproj
--rw-r--r--   0        0        0     9247 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-update-icon-cache.vcxproj
--rw-r--r--   0        0        0      706 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-update-icon-cache.vcxproj.filters
--rw-r--r--   0        0        0     2185 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-version-paths.props
--rw-r--r--   0        0        0    26897 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk.vcxproj
--rw-r--r--   0        0        0    26470 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk.vcxproj.filters
--rw-r--r--   0        0        0     9451 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/libwimp.vcxproj
--rw-r--r--   0        0        0     1756 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/libwimp.vcxproj.filters
--rw-r--r--   0        0        0     3586 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/README.txt
--rw-r--r--   0        0        0      803 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/gtk-accel.patch
--rw-r--r--   0        0        0      599 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/gtk-bgimg.patch
--rw-r--r--   0        0        0      682 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/gtk-multimonitor.patch
--rw-r--r--   0        0        0     2154 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/gtk-revert-scrolldc-commit.patch
--rw-r--r--   0        0        0     1104 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk2/mod.md
--rw-r--r--   0        0        0     6104 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk3/gdk/win32/gdkkeys-win32.h
--rw-r--r--   0        0        0    11322 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk3/gdk/win32/winpointer.h
--rw-r--r--   0        0        0     1630 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtk3/gtk_update_icon_cache.patch
--rw-r--r--   0        0        0     1088 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/gtksourceview5/001-fix-fontconfig-availability-check.patch
--rw-r--r--   0        0        0      102 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/hello-world/hello-world.c
--rw-r--r--   0        0        0       66 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/hello-world/meson.build
--rw-r--r--   0        0        0      359 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/icu/pc-files/icu-uc.pc
--rw-r--r--   0        0        0      360 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/icu/pc-files-debug/icu-uc.pc
--rw-r--r--   0        0        0    39523 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/libadwaita/0001-remove-appstream-dependency.patch
--rw-r--r--   0        0        0      652 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/libcroco/mod.md
--rw-r--r--   0        0        0     3749 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/libcroco/win32/vs10/croco-version-paths.props
--rw-r--r--   0        0        0     3749 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/libcroco/win32/vs12/croco-version-paths.props
--rw-r--r--   0        0        0     3749 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/libcroco/win32/vs14/croco-version-paths.props
--rw-r--r--   0        0        0     3749 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/libcroco/win32/vs15/croco-version-paths.props
--rw-r--r--   0        0        0     4827 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/libffi/fficonfig.h.meson
--rw-r--r--   0        0        0      475 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/libffi/include/meson.build
--rw-r--r--   0        0        0      248 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/libffi/meson-scripts/extract-libtool-version.py
--rw-r--r--   0        0        0    13940 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/libffi/meson.build
--rw-r--r--   0        0        0     1154 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/libffi/meson_options.txt
--rw-r--r--   0        0        0     3334 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/libffi/src/meson.build
--rw-r--r--   0        0        0      936 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/libfido2/0001-Install-pkgconfig-files-also-on-msvc.patch
--rw-r--r--   0        0        0     1243 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/libfido2/0001-libfido2-update-cmake-script-to-have-sdl-flag-before.patch
--rw-r--r--   0        0        0     9777 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/libmicrohttpd/001-remove-postsample-perf-retries.patch
--rw-r--r--   0        0        0       44 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/libpng/mod.md
--rw-r--r--   0        0        0      318 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/libpng/pc-files/libpng.pc
--rw-r--r--   0        0        0      318 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/libpng/pc-files/libpng16.pc
--rw-r--r--   0        0        0     2998 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs12/rsvg-build-defines.props
--rw-r--r--   0        0        0     2133 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs12/rsvg-install.props
--rw-r--r--   0        0        0     2326 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs12/rsvg-version-paths.props
--rw-r--r--   0        0        0     2998 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs14/rsvg-build-defines.props
--rw-r--r--   0        0        0     2133 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs14/rsvg-install.props
--rw-r--r--   0        0        0     2326 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs14/rsvg-version-paths.props
--rw-r--r--   0        0        0     9178 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/libpixbufloader-svg.vcxproj
--rw-r--r--   0        0        0      937 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/libpixbufloader-svg.vcxproj.filters
--rw-r--r--   0        0        0     4286 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/librsvg.sln
--rw-r--r--   0        0        0      572 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/Makefile.am
--rw-r--r--   0        0        0    17549 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/Makefile.in
--rw-r--r--   0        0        0     3085 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/README.txt
--rw-r--r--   0        0        0     2998 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-build-defines.props
--rw-r--r--   0        0        0     8574 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-convert.vcxproj
--rw-r--r--   0        0        0     1026 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-convert.vcxproj.filters
--rw-r--r--   0        0        0      931 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-gen-srcs.props
--rw-r--r--   0        0        0     2133 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-install.props
--rw-r--r--   0        0        0     6578 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-install.vcxproj
--rw-r--r--   0        0        0     2326 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-version-paths.props
--rw-r--r--   0        0        0     8979 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-view-3.vcxproj
--rw-r--r--   0        0        0      925 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-view-3.vcxproj.filters
--rw-r--r--   0        0        0    14576 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg.vcxproj
--rw-r--r--   0        0        0     3427 2024-04-08 18:08:22.197489 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg.vcxproj.filters
--rw-r--r--   0        0        0      866 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/vs2019-support.patch
--rw-r--r--   0        0        0     5490 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs12/config.h
--rw-r--r--   0        0        0     8059 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs12/install.vcxproj
--rw-r--r--   0        0        0      834 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs12/install.vcxproj.filters
--rw-r--r--   0        0        0     3769 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs12/libssh-library.sln
--rw-r--r--   0        0        0     3074 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs12/property.props
--rw-r--r--   0        0        0    40095 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs12/ssh_shared.vcxproj
--rw-r--r--   0        0        0     5705 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs12/ssh_shared.vcxproj.filters
--rw-r--r--   0        0        0    32139 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs12/ssh_static.vcxproj
--rw-r--r--   0        0        0     5705 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs12/ssh_static.vcxproj.filters
--rw-r--r--   0        0        0     5490 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs14/config.h
--rw-r--r--   0        0        0     8059 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs14/install.vcxproj
--rw-r--r--   0        0        0      834 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs14/install.vcxproj.filters
--rw-r--r--   0        0        0     3767 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs14/libssh-library.sln
--rw-r--r--   0        0        0     3074 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs14/property.props
--rw-r--r--   0        0        0    40095 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs14/ssh_shared.vcxproj
--rw-r--r--   0        0        0     5705 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs14/ssh_shared.vcxproj.filters
--rw-r--r--   0        0        0    32139 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs14/ssh_static.vcxproj
--rw-r--r--   0        0        0     5705 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs14/ssh_static.vcxproj.filters
--rw-r--r--   0        0        0     5490 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs15/config.h
--rw-r--r--   0        0        0     8138 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs15/install.vcxproj
--rw-r--r--   0        0        0      834 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs15/install.vcxproj.filters
--rw-r--r--   0        0        0     3899 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs15/libssh-library.sln
--rw-r--r--   0        0        0     3074 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs15/property.props
--rw-r--r--   0        0        0    40174 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs15/ssh_shared.vcxproj
--rw-r--r--   0        0        0     5705 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs15/ssh_shared.vcxproj.filters
--rw-r--r--   0        0        0    32139 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs15/ssh_static.vcxproj
--rw-r--r--   0        0        0     5705 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs15/ssh_static.vcxproj.filters
--rw-r--r--   0        0        0     1079 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libssh/mod.md
--rw-r--r--   0        0        0      809 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libtiff-4/0001-cmake-remove-.d-postfix.patch
--rw-r--r--   0        0        0     2586 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libvpx/0001-Always-generate-pc-file.patch
--rw-r--r--   0        0        0     1251 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libvpx/0006-gen_msvs_vcxproj.sh-Select-current-Windows-SDK-if-av.patch
--rw-r--r--   0        0        0     1025 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libxml2/include/libxml/meson.build
--rw-r--r--   0        0        0     1089 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libxml2/LICENSE.build
--rw-r--r--   0        0        0     7284 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libxml2/meson.build
--rw-r--r--   0        0        0      323 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libxml2/pc-files/libxml-2.0.pc
--rw-r--r--   0        0        0      943 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libyuv/001-win-build.patch
--rw-r--r--   0        0        0      392 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/libyuv/pc-files/libyuv.pc
--rw-r--r--   0        0        0      352 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/luajit/pc-files/luajit.pc
--rw-r--r--   0        0        0      971 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/luajit/set-paths.patch
--rw-r--r--   0        0        0      319 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/pc-files/liblz4.pc
--rw-r--r--   0        0        0     8964 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/datagen/datagen.vcxproj
--rw-r--r--   0        0        0     9315 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/frametest/frametest.vcxproj
--rw-r--r--   0        0        0     9315 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/fullbench/fullbench.vcxproj
--rw-r--r--   0        0        0    10136 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/fullbench-dll/fullbench-dll.vcxproj
--rw-r--r--   0        0        0     9143 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/fuzzer/fuzzer.vcxproj
--rw-r--r--   0        0        0     9204 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/liblz4/liblz4.vcxproj
--rw-r--r--   0        0        0     1388 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/liblz4-dll/liblz4-dll.rc
--rw-r--r--   0        0        0     9307 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/liblz4-dll/liblz4-dll.vcxproj
--rw-r--r--   0        0        0     1388 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/lz4/lz4.rc
--rw-r--r--   0        0        0     9978 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/lz4/lz4.vcxproj
--rw-r--r--   0        0        0     6761 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/lz4.sln
--rw-r--r--   0        0        0     8964 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/datagen/datagen.vcxproj
--rw-r--r--   0        0        0     9315 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/frametest/frametest.vcxproj
--rw-r--r--   0        0        0     9315 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/fullbench/fullbench.vcxproj
--rw-r--r--   0        0        0    10136 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/fullbench-dll/fullbench-dll.vcxproj
--rw-r--r--   0        0        0     9143 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/fuzzer/fuzzer.vcxproj
--rw-r--r--   0        0        0     9204 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/liblz4/liblz4.vcxproj
--rw-r--r--   0        0        0     1388 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/liblz4-dll/liblz4-dll.rc
--rw-r--r--   0        0        0     9307 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/liblz4-dll/liblz4-dll.vcxproj
--rw-r--r--   0        0        0     1388 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/lz4/lz4.rc
--rw-r--r--   0        0        0     9978 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/lz4/lz4.vcxproj
--rw-r--r--   0        0        0     6761 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/lz4.sln
--rw-r--r--   0        0        0     8966 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/datagen/datagen.vcxproj
--rw-r--r--   0        0        0     9317 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/frametest/frametest.vcxproj
--rw-r--r--   0        0        0     9317 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/fullbench/fullbench.vcxproj
--rw-r--r--   0        0        0    10138 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/fullbench-dll/fullbench-dll.vcxproj
--rw-r--r--   0        0        0     9145 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/fuzzer/fuzzer.vcxproj
--rw-r--r--   0        0        0     9206 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/liblz4/liblz4.vcxproj
--rw-r--r--   0        0        0     1388 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/liblz4-dll/liblz4-dll.rc
--rw-r--r--   0        0        0     9309 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/liblz4-dll/liblz4-dll.vcxproj
--rw-r--r--   0        0        0     1388 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/lz4/lz4.rc
--rw-r--r--   0        0        0     9978 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/lz4/lz4.vcxproj
--rw-r--r--   0        0        0     6761 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/lz4.sln
--rw-r--r--   0        0        0     8964 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2022/datagen/datagen.vcxproj
--rw-r--r--   0        0        0     9315 2024-04-08 18:08:22.213117 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2022/frametest/frametest.vcxproj
--rw-r--r--   0        0        0     9315 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2022/fullbench/fullbench.vcxproj
--rw-r--r--   0        0        0    10136 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2022/fullbench-dll/fullbench-dll.vcxproj
--rw-r--r--   0        0        0     9143 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2022/fuzzer/fuzzer.vcxproj
--rw-r--r--   0        0        0     9204 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2022/liblz4/liblz4.vcxproj
--rw-r--r--   0        0        0     1388 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2022/liblz4-dll/liblz4-dll.rc
--rw-r--r--   0        0        0     9307 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2022/liblz4-dll/liblz4-dll.vcxproj
--rw-r--r--   0        0        0     1388 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2022/lz4/lz4.rc
--rw-r--r--   0        0        0     9976 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2022/lz4/lz4.vcxproj
--rw-r--r--   0        0        0     6761 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2022/lz4.sln
--rw-r--r--   0        0        0       93 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/mod.md
--rw-r--r--   0        0        0      733 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/nghttp2/0001-Define-ssize_t-if-not-defined.patch
--rw-r--r--   0        0        0     2184 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/openssl-base/0001-crypto-providers-config.patch
--rw-r--r--   0        0        0  1290625 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/openssl-base/certdata.txt
--rw-r--r--   0        0        0    19616 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/openssl-base/mk-ca-bundle.pl
--rw-r--r--   0        0        0      412 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/openssl-base/mod.md
--rw-r--r--   0        0        0      275 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/openssl-base/pc-files/libcrypto.pc
--rw-r--r--   0        0        0      285 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/openssl-base/pc-files/libssl.pc
--rw-r--r--   0        0        0      236 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/openssl-base/pc-files/openssl.pc
--rw-r--r--   0        0        0      383 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/opus/pc-files/opus.pc
--rw-r--r--   0        0        0    11464 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/pango/002-fix-wrong-usage-gweakref.patch
--rw-r--r--   0        0        0     1027 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/pango/003-remove-extra-hb-face-font.patch
--rw-r--r--   0        0        0     1089 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/pcre2/LICENSE.build
--rw-r--r--   0        0        0     7523 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/pcre2/meson.build
--rw-r--r--   0        0        0      473 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/pcre2/meson_options.txt
--rw-r--r--   0        0        0     1241 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/pkgconf/0001-libpkgconf-add-defines-to-unbreak-build-with-VS2013.patch
--rw-r--r--   0        0        0     1036 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/protobuf-c/0001-Declare-variables-at-the-beginning-of-the-block.patch
--rw-r--r--   0        0        0     2647 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/protobuf-c/0001-Do-not-build-tests.patch
--rw-r--r--   0        0        0      319 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/protobuf-c/pc-files/libprotobuf-c.pc
--rw-r--r--   0        0        0     1912 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/pygobject/001-pygobject-py38-load-dll.patch
--rw-r--r--   0        0        0      633 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/stack.props
--rw-r--r--   0        0        0     1565 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/win-iconv/COPYING
--rw-r--r--   0        0        0       92 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/win-iconv/mod.md
--rw-r--r--   0        0        0      671 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/x264/build/build.sh
--rw-r--r--   0        0        0     1385 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/x264/x264-0001-Prevent-mb_info_free-to-be-called-before-all-threads.patch
--rw-r--r--   0        0        0      343 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/patches/zlib/pc-files/zlib.pc
--rw-r--r--   0        0        0     4259 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/projects/__init__.py
--rw-r--r--   0        0        0     2040 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/projects/adwaita_icon_theme.py
--rw-r--r--   0        0        0     1808 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/projects/atk.py
--rw-r--r--   0        0        0     1774 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/projects/boringssl.py
--rw-r--r--   0        0        0     1598 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/projects/cairo.py
--rw-r--r--   0        0        0     1509 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/projects/cairomm.py
--rw-r--r--   0        0        0     1912 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/projects/check_libs.py
--rw-r--r--   0        0        0     1620 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/projects/clutter.py
--rw-r--r--   0        0        0     1758 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/projects/cogl.py
--rw-r--r--   0        0        0     2872 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/projects/cyrus_sasl.py
--rw-r--r--   0        0        0     2844 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/projects/dev_shell.py
--rw-r--r--   0        0        0     1648 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/projects/emeus.py
--rw-r--r--   0        0        0     2807 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/projects/enchant.py
--rw-r--r--   0        0        0     1572 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/projects/expat.py
--rw-r--r--   0        0        0     3386 2024-04-08 18:08:22.228741 gvsbuild-2024.4.1/gvsbuild/projects/ffmpeg.py
--rw-r--r--   0        0        0     1725 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/freerdp.py
--rw-r--r--   0        0        0     1638 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/freetype.py
--rw-r--r--   0        0        0     2093 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/fribidi.py
--rw-r--r--   0        0        0     2204 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/gdk_pixbuf.py
--rw-r--r--   0        0        0     4032 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/gettext.py
--rw-r--r--   0        0        0     4682 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/glib.py
--rw-r--r--   0        0        0     1704 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/glibmm.py
--rw-r--r--   0        0        0     2684 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/gobject_introspection.py
--rw-r--r--   0        0        0     1312 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/gperf.py
--rw-r--r--   0        0        0     1752 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/graphene.py
--rw-r--r--   0        0        0     1813 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/gsettings_desktop_schemas.py
--rw-r--r--   0        0        0     8797 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/gstreamer.py
--rw-r--r--   0        0        0     5848 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/gtk.py
--rw-r--r--   0        0        0     1806 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/gtkmm.py
--rw-r--r--   0        0        0     2846 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/gtksourceview.py
--rw-r--r--   0        0        0     1672 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/harfbuzz.py
--rw-r--r--   0        0        0     1184 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/hello_world.py
--rw-r--r--   0        0        0     1382 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/hicolor_icon_theme.py
--rw-r--r--   0        0        0     2276 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/icu.py
--rw-r--r--   0        0        0     1832 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/json_glib.py
--rw-r--r--   0        0        0     1392 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/jsonc.py
--rw-r--r--   0        0        0     1624 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/leveldb.py
--rw-r--r--   0        0        0     1417 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/lgi.py
--rw-r--r--   0        0        0     2027 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libadwaita.py
--rw-r--r--   0        0        0     2075 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libarchive.py
--rw-r--r--   0        0        0     1781 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libcbor.py
--rw-r--r--   0        0        0     1496 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libcroco.py
--rw-r--r--   0        0        0     1903 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libcurl.py
--rw-r--r--   0        0        0     1447 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libepoxy.py
--rw-r--r--   0        0        0     1341 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libffi.py
--rw-r--r--   0        0        0     2597 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libfido2.py
--rw-r--r--   0        0        0     1989 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libgxps.py
--rw-r--r--   0        0        0     1741 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libjpeg_turbo.py
--rw-r--r--   0        0        0     2331 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libmicrohttpd.py
--rw-r--r--   0        0        0     1704 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libpng.py
--rw-r--r--   0        0        0     1595 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libpsl.py
--rw-r--r--   0        0        0     2405 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/librsvg.py
--rw-r--r--   0        0        0     1737 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libsigcplusplus.py
--rw-r--r--   0        0        0     3368 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libsoup.py
--rw-r--r--   0        0        0     2181 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libssh.py
--rw-r--r--   0        0        0     1586 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libtiff.py
--rw-r--r--   0        0        0     1514 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libuv.py
--rw-r--r--   0        0        0     1511 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libvorbis.py
--rw-r--r--   0        0        0     3265 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libvpx.py
--rw-r--r--   0        0        0     1574 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libxml2.py
--rw-r--r--   0        0        0     1576 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libyuv.py
--rw-r--r--   0        0        0     1411 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/libzip.py
--rw-r--r--   0        0        0     1426 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/lmdb.py
--rw-r--r--   0        0        0     1761 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/luajit.py
--rw-r--r--   0        0        0     1778 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/lz4.py
--rw-r--r--   0        0        0     2279 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/mit_kerberos.py
--rw-r--r--   0        0        0     1587 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/nghttp2.py
--rw-r--r--   0        0        0     1477 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/ogg.py
--rw-r--r--   0        0        0     1521 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/openh264.py
--rw-r--r--   0        0        0     3381 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/openssl.py
--rw-r--r--   0        0        0     2056 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/opus.py
--rw-r--r--   0        0        0     2046 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/pango.py
--rw-r--r--   0        0        0     1768 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/pangomm.py
--rw-r--r--   0        0        0      712 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/pcre2.py
--rw-r--r--   0        0        0     1672 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/pixman.py
--rw-r--r--   0        0        0     1692 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/pkgconf.py
--rw-r--r--   0        0        0     2711 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/protobuf.py
--rw-r--r--   0        0        0     2102 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/pycairo.py
--rw-r--r--   0        0        0     2591 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/pygobject.py
--rw-r--r--   0        0        0     1618 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/sqlite.py
--rw-r--r--   0        0        0     1607 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/win_iconv.py
--rw-r--r--   0        0        0     1470 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/wing.py
--rw-r--r--   0        0        0     2341 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/x264.py
--rw-r--r--   0        0        0     2444 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/projects/zlib.py
--rw-r--r--   0        0        0     7545 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/tools.py
--rw-r--r--   0        0        0       30 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/utils/__init__.py
--rw-r--r--   0        0        0     8512 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/utils/base_builders.py
--rw-r--r--   0        0        0    15193 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/utils/base_expanders.py
--rw-r--r--   0        0        0     1339 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/utils/base_group.py
--rw-r--r--   0        0        0    20353 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/utils/base_project.py
--rw-r--r--   0        0        0     2749 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/utils/base_tool.py
--rw-r--r--   0        0        0    38283 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/utils/builder.py
--rw-r--r--   0        0        0     9899 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/utils/simple_ui.py
--rw-r--r--   0        0        0     3899 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/gvsbuild/utils/utils.py
--rw-r--r--   0        0        0     1708 2024-04-08 18:08:22.244366 gvsbuild-2024.4.1/pyproject.toml
--rw-r--r--   0        0        0    12300 2024-04-08 18:08:22.040712 gvsbuild-2024.4.1/README.md
--rw-r--r--   0        0        0    13098 1970-01-01 00:00:00.000000 gvsbuild-2024.4.1/PKG-INFO
+-rw-r--r--   0        0        0     2185 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/AUTHORS.md
+-rw-r--r--   0        0        0    18433 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/COPYING
+-rw-r--r--   0        0        0       37 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/__init__.py
+-rw-r--r--   0        0        0    16410 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/build.py
+-rw-r--r--   0        0        0     7322 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/deps.py
+-rw-r--r--   0        0        0     2121 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/groups.py
+-rw-r--r--   0        0        0      244 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/info.py
+-rw-r--r--   0        0        0     5583 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/list.py
+-rw-r--r--   0        0        0     1977 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/main.py
+-rw-r--r--   0        0        0     2609 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/outdated.py
+-rw-r--r--   0        0        0      634 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/cairo/0001-fix-alloca-unresolved.patch
+-rw-r--r--   0        0        0      213 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/check-libs/check_utils.c
+-rw-r--r--   0        0        0      537 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/check-libs/check_utils.h
+-rw-r--r--   0        0        0    18437 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/check-libs/COPYING
+-rw-r--r--   0        0        0     9831 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/check-libs/meson.build
+-rw-r--r--   0        0        0      175 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/check-libs/test_atk.c
+-rw-r--r--   0        0        0      167 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/check-libs/test_cairo.c
+-rw-r--r--   0        0        0      224 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/check-libs/test_freetype2.c
+-rw-r--r--   0        0        0      205 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/check-libs/test_gdk-pixbuf.c
+-rw-r--r--   0        0        0      170 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/check-libs/test_glib.c
+-rw-r--r--   0        0        0      183 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/check-libs/test_jasper.c
+-rw-r--r--   0        0        0      204 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/check-libs/test_json_glib.c
+-rw-r--r--   0        0        0      201 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/check-libs/test_libarchive.c
+-rw-r--r--   0        0        0      191 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/check-libs/test_libcurl.c
+-rw-r--r--   0        0        0      125 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/check-libs/test_libffi.c
+-rw-r--r--   0        0        0      193 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/check-libs/test_libjpeg-turbo.c
+-rw-r--r--   0        0        0      194 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/check-libs/test_libjpeg.c
+-rw-r--r--   0        0        0      188 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/check-libs/test_libpng.c
+-rw-r--r--   0        0        0      187 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/check-libs/test_libtiff-4.c
+-rw-r--r--   0        0        0      179 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/check-libs/test_libxml2.c
+-rw-r--r--   0        0        0      187 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/check-libs/test_libyuv.c
+-rw-r--r--   0        0        0      173 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/check-libs/test_pango.c
+-rw-r--r--   0        0        0      180 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/check-libs/test_wing.c
+-rw-r--r--   0        0        0      127 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/check-libs/test_zlib.c
+-rw-r--r--   0        0        0     9047 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkcomponent-example.vcxproj
+-rw-r--r--   0        0        0     1020 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkcomponent-example.vcxproj.filters
+-rw-r--r--   0        0        0     9101 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkeditabletext-example.vcxproj
+-rw-r--r--   0        0        0     1023 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkeditabletext-example.vcxproj.filters
+-rw-r--r--   0        0        0     9557 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkevents-example.vcxproj
+-rw-r--r--   0        0        0     1017 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkevents-example.vcxproj.filters
+-rw-r--r--   0        0        0     9085 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atktext-example.vcxproj
+-rw-r--r--   0        0        0      958 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atktext-example.vcxproj.filters
+-rw-r--r--   0        0        0     9033 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/cally-clone-example.vcxproj
+-rw-r--r--   0        0        0     1013 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/cally-clone-example.vcxproj.filters
+-rw-r--r--   0        0        0     4196 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-build-defines.props
+-rw-r--r--   0        0        0     6817 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-gen-srcs.props
+-rw-r--r--   0        0        0    16612 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-install.props
+-rw-r--r--   0        0        0    10665 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-install.vcxproj
+-rw-r--r--   0        0        0     2510 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-version-paths.props
+-rw-r--r--   0        0        0      405 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.bld.win32.win32
+-rw-r--r--   0        0        0    29220 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.sln
+-rw-r--r--   0        0        0    50071 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj
+-rw-r--r--   0        0        0    15822 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj.filters
+-rw-r--r--   0        0        0     2515 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj.filtersin
+-rw-r--r--   0        0        0    41134 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxprojin
+-rw-r--r--   0        0        0     1794 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/Makefile.am
+-rw-r--r--   0        0        0    19138 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/Makefile.in
+-rw-r--r--   0        0        0     4749 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/README.txt
+-rw-r--r--   0        0        0     8818 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-cogl-perf.vcxproj
+-rw-r--r--   0        0        0      532 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-cogl-perf.vcxproj.filters
+-rw-r--r--   0        0        0    13484 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxproj
+-rw-r--r--   0        0        0     5987 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxproj.filters
+-rw-r--r--   0        0        0      464 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxproj.filtersin
+-rw-r--r--   0        0        0     9685 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxprojin
+-rw-r--r--   0        0        0     8719 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-picking-performance.vcxproj
+-rw-r--r--   0        0        0      866 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-picking-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8897 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-picking.vcxproj
+-rw-r--r--   0        0        0      530 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-picking.vcxproj.filters
+-rw-r--r--   0        0        0     8822 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-random-text.vcxproj
+-rw-r--r--   0        0        0      534 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-random-text.vcxproj.filters
+-rw-r--r--   0        0        0     8728 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-hidden-performance.vcxproj
+-rw-r--r--   0        0        0      871 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-hidden-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8738 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-interactive-performance.vcxproj
+-rw-r--r--   0        0        0      876 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-interactive-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8724 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-mini-performance.vcxproj
+-rw-r--r--   0        0        0      869 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-mini-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8715 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-performance.vcxproj
+-rw-r--r--   0        0        0      864 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8724 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-pick-performance.vcxproj
+-rw-r--r--   0        0        0      869 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-pick-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8722 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf-performance.vcxproj
+-rw-r--r--   0        0        0      868 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8818 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf.vcxproj
+-rw-r--r--   0        0        0      532 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf.vcxproj.filters
+-rw-r--r--   0        0        0     8809 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-text.vcxproj
+-rw-r--r--   0        0        0      527 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-text.vcxproj.filters
+-rw-r--r--   0        0        0     9047 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkcomponent-example.vcxproj
+-rw-r--r--   0        0        0     1020 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkcomponent-example.vcxproj.filters
+-rw-r--r--   0        0        0     9101 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkeditabletext-example.vcxproj
+-rw-r--r--   0        0        0     1023 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkeditabletext-example.vcxproj.filters
+-rw-r--r--   0        0        0     9557 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkevents-example.vcxproj
+-rw-r--r--   0        0        0     1017 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkevents-example.vcxproj.filters
+-rw-r--r--   0        0        0     9085 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atktext-example.vcxproj
+-rw-r--r--   0        0        0      958 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atktext-example.vcxproj.filters
+-rw-r--r--   0        0        0     9033 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/cally-clone-example.vcxproj
+-rw-r--r--   0        0        0     1013 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/cally-clone-example.vcxproj.filters
+-rw-r--r--   0        0        0     4196 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-build-defines.props
+-rw-r--r--   0        0        0     6817 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-gen-srcs.props
+-rw-r--r--   0        0        0    16612 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-install.props
+-rw-r--r--   0        0        0    10665 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-install.vcxproj
+-rw-r--r--   0        0        0     2510 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-version-paths.props
+-rw-r--r--   0        0        0      405 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.bld.win32.win32
+-rw-r--r--   0        0        0    27777 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.sln
+-rw-r--r--   0        0        0    50071 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj
+-rw-r--r--   0        0        0    15822 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj.filters
+-rw-r--r--   0        0        0     2515 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj.filtersin
+-rw-r--r--   0        0        0    41134 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxprojin
+-rw-r--r--   0        0        0     1794 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/Makefile.am
+-rw-r--r--   0        0        0    19138 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/Makefile.in
+-rw-r--r--   0        0        0     4749 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/README.txt
+-rw-r--r--   0        0        0     8818 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-cogl-perf.vcxproj
+-rw-r--r--   0        0        0      532 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-cogl-perf.vcxproj.filters
+-rw-r--r--   0        0        0     8719 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-picking-performance.vcxproj
+-rw-r--r--   0        0        0      866 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-picking-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8897 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-picking.vcxproj
+-rw-r--r--   0        0        0      530 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-picking.vcxproj.filters
+-rw-r--r--   0        0        0     8822 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-random-text.vcxproj
+-rw-r--r--   0        0        0      534 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-random-text.vcxproj.filters
+-rw-r--r--   0        0        0     8728 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-hidden-performance.vcxproj
+-rw-r--r--   0        0        0      871 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-hidden-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8738 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-interactive-performance.vcxproj
+-rw-r--r--   0        0        0      876 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-interactive-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8724 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-mini-performance.vcxproj
+-rw-r--r--   0        0        0      869 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-mini-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8715 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-performance.vcxproj
+-rw-r--r--   0        0        0      864 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8724 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-pick-performance.vcxproj
+-rw-r--r--   0        0        0      869 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-pick-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8722 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf-performance.vcxproj
+-rw-r--r--   0        0        0      868 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8818 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf.vcxproj
+-rw-r--r--   0        0        0      532 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf.vcxproj.filters
+-rw-r--r--   0        0        0     8809 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-text.vcxproj
+-rw-r--r--   0        0        0      527 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-text.vcxproj.filters
+-rw-r--r--   0        0        0     9126 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkcomponent-example.vcxproj
+-rw-r--r--   0        0        0     1020 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkcomponent-example.vcxproj.filters
+-rw-r--r--   0        0        0     9180 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkeditabletext-example.vcxproj
+-rw-r--r--   0        0        0     1023 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkeditabletext-example.vcxproj.filters
+-rw-r--r--   0        0        0     9636 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkevents-example.vcxproj
+-rw-r--r--   0        0        0     1017 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkevents-example.vcxproj.filters
+-rw-r--r--   0        0        0     9164 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atktext-example.vcxproj
+-rw-r--r--   0        0        0      958 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atktext-example.vcxproj.filters
+-rw-r--r--   0        0        0     9112 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/cally-clone-example.vcxproj
+-rw-r--r--   0        0        0     1013 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/cally-clone-example.vcxproj.filters
+-rw-r--r--   0        0        0     4196 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-build-defines.props
+-rw-r--r--   0        0        0     6817 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-gen-srcs.props
+-rw-r--r--   0        0        0    16612 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-install.props
+-rw-r--r--   0        0        0    10744 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-install.vcxproj
+-rw-r--r--   0        0        0     2510 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-version-paths.props
+-rw-r--r--   0        0        0      405 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.bld.win32.win32
+-rw-r--r--   0        0        0    27909 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.sln
+-rw-r--r--   0        0        0    50150 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj
+-rw-r--r--   0        0        0    15822 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj.filters
+-rw-r--r--   0        0        0     2515 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj.filtersin
+-rw-r--r--   0        0        0    41134 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxprojin
+-rw-r--r--   0        0        0     1794 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/Makefile.am
+-rw-r--r--   0        0        0    19138 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/Makefile.in
+-rw-r--r--   0        0        0     4749 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/README.txt
+-rw-r--r--   0        0        0     8897 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-cogl-perf.vcxproj
+-rw-r--r--   0        0        0      532 2024-05-09 20:22:13.079142 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-cogl-perf.vcxproj.filters
+-rw-r--r--   0        0        0     8798 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-picking-performance.vcxproj
+-rw-r--r--   0        0        0      866 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-picking-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8976 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-picking.vcxproj
+-rw-r--r--   0        0        0      530 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-picking.vcxproj.filters
+-rw-r--r--   0        0        0     8901 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-random-text.vcxproj
+-rw-r--r--   0        0        0      534 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-random-text.vcxproj.filters
+-rw-r--r--   0        0        0     8807 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-hidden-performance.vcxproj
+-rw-r--r--   0        0        0      871 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-hidden-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8817 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-interactive-performance.vcxproj
+-rw-r--r--   0        0        0      876 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-interactive-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8803 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-mini-performance.vcxproj
+-rw-r--r--   0        0        0      869 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-mini-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8794 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-performance.vcxproj
+-rw-r--r--   0        0        0      864 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8803 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-pick-performance.vcxproj
+-rw-r--r--   0        0        0      869 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-pick-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8801 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf-performance.vcxproj
+-rw-r--r--   0        0        0      868 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf-performance.vcxproj.filters
+-rw-r--r--   0        0        0     8897 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf.vcxproj
+-rw-r--r--   0        0        0      532 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf.vcxproj.filters
+-rw-r--r--   0        0        0     8888 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-text.vcxproj
+-rw-r--r--   0        0        0      527 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-text.vcxproj.filters
+-rw-r--r--   0        0        0      316 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/cogl/001-cogl-missing-symbols.patch
+-rw-r--r--   0        0        0      339 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/cogl/002-cogl-pango-missing-symbols.patch
+-rw-r--r--   0        0        0     3533 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-build-defines.props
+-rw-r--r--   0        0        0    10205 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-crate.vcxproj
+-rw-r--r--   0        0        0      519 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-crate.vcxproj.filters
+-rw-r--r--   0        0        0     5411 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-gen-srcs.props
+-rw-r--r--   0        0        0     8918 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-hello.vcxproj
+-rw-r--r--   0        0        0      519 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-hello.vcxproj.filters
+-rw-r--r--   0        0        0     9239 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-info.vcxproj
+-rw-r--r--   0        0        0      518 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-info.vcxproj.filters
+-rw-r--r--   0        0        0    10887 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-install.props
+-rw-r--r--   0        0        0    14290 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-install.vcxproj
+-rw-r--r--   0        0        0     8788 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-msaa.vcxproj
+-rw-r--r--   0        0        0      518 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-msaa.vcxproj.filters
+-rw-r--r--   0        0        0    12851 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj
+-rw-r--r--   0        0        0     1402 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj.filters
+-rw-r--r--   0        0        0      789 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj.filtersin
+-rw-r--r--   0        0        0    11992 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxprojin
+-rw-r--r--   0        0        0    16347 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj
+-rw-r--r--   0        0        0     2531 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj.filters
+-rw-r--r--   0        0        0     1267 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj.filtersin
+-rw-r--r--   0        0        0    15092 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxprojin
+-rw-r--r--   0        0        0     9571 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-sdl2-hello.vcxproj
+-rw-r--r--   0        0        0      522 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-sdl2-hello.vcxproj.filters
+-rw-r--r--   0        0        0     2482 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-version-paths.props
+-rw-r--r--   0        0        0    12059 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.sln
+-rw-r--r--   0        0        0    48250 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj
+-rw-r--r--   0        0        0    14547 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj.filters
+-rw-r--r--   0        0        0     3009 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj.filtersin
+-rw-r--r--   0        0        0    41403 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxprojin
+-rw-r--r--   0        0        0      919 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/Makefile.am
+-rw-r--r--   0        0        0    19171 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/Makefile.in
+-rw-r--r--   0        0        0     4783 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/README.txt
+-rw-r--r--   0        0        0    13862 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj
+-rw-r--r--   0        0        0     5574 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj.filters
+-rw-r--r--   0        0        0      563 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj.filtersin
+-rw-r--r--   0        0        0     9905 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxprojin
+-rw-r--r--   0        0        0     3533 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-build-defines.props
+-rw-r--r--   0        0        0    10205 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-crate.vcxproj
+-rw-r--r--   0        0        0      519 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-crate.vcxproj.filters
+-rw-r--r--   0        0        0     5411 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-gen-srcs.props
+-rw-r--r--   0        0        0     8918 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-hello.vcxproj
+-rw-r--r--   0        0        0      519 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-hello.vcxproj.filters
+-rw-r--r--   0        0        0     9239 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-info.vcxproj
+-rw-r--r--   0        0        0      518 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-info.vcxproj.filters
+-rw-r--r--   0        0        0    10887 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-install.props
+-rw-r--r--   0        0        0    14290 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-install.vcxproj
+-rw-r--r--   0        0        0     8788 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-msaa.vcxproj
+-rw-r--r--   0        0        0      518 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-msaa.vcxproj.filters
+-rw-r--r--   0        0        0    12851 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj
+-rw-r--r--   0        0        0     1402 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj.filters
+-rw-r--r--   0        0        0      789 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj.filtersin
+-rw-r--r--   0        0        0    11992 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxprojin
+-rw-r--r--   0        0        0    16347 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj
+-rw-r--r--   0        0        0     2531 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj.filters
+-rw-r--r--   0        0        0     1267 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj.filtersin
+-rw-r--r--   0        0        0    15092 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxprojin
+-rw-r--r--   0        0        0     9571 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-sdl2-hello.vcxproj
+-rw-r--r--   0        0        0      522 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-sdl2-hello.vcxproj.filters
+-rw-r--r--   0        0        0     2482 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-version-paths.props
+-rw-r--r--   0        0        0    12059 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.sln
+-rw-r--r--   0        0        0    48250 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj
+-rw-r--r--   0        0        0    14547 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj.filters
+-rw-r--r--   0        0        0     3009 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj.filtersin
+-rw-r--r--   0        0        0    41403 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxprojin
+-rw-r--r--   0        0        0      919 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/Makefile.am
+-rw-r--r--   0        0        0    19171 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/Makefile.in
+-rw-r--r--   0        0        0     4783 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/README.txt
+-rw-r--r--   0        0        0    13862 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj
+-rw-r--r--   0        0        0     5574 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj.filters
+-rw-r--r--   0        0        0      563 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj.filtersin
+-rw-r--r--   0        0        0     9905 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxprojin
+-rw-r--r--   0        0        0     3533 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-build-defines.props
+-rw-r--r--   0        0        0    10284 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-crate.vcxproj
+-rw-r--r--   0        0        0      519 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-crate.vcxproj.filters
+-rw-r--r--   0        0        0     5411 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-gen-srcs.props
+-rw-r--r--   0        0        0     8997 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-hello.vcxproj
+-rw-r--r--   0        0        0      519 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-hello.vcxproj.filters
+-rw-r--r--   0        0        0     9318 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-info.vcxproj
+-rw-r--r--   0        0        0      518 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-info.vcxproj.filters
+-rw-r--r--   0        0        0    10887 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-install.props
+-rw-r--r--   0        0        0    14369 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-install.vcxproj
+-rw-r--r--   0        0        0     8788 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-msaa.vcxproj
+-rw-r--r--   0        0        0      518 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-msaa.vcxproj.filters
+-rw-r--r--   0        0        0    12930 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj
+-rw-r--r--   0        0        0     1402 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj.filters
+-rw-r--r--   0        0        0      789 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj.filtersin
+-rw-r--r--   0        0        0    11992 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxprojin
+-rw-r--r--   0        0        0    16426 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj
+-rw-r--r--   0        0        0     2531 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj.filters
+-rw-r--r--   0        0        0     1267 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj.filtersin
+-rw-r--r--   0        0        0    15092 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxprojin
+-rw-r--r--   0        0        0     9571 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-sdl2-hello.vcxproj
+-rw-r--r--   0        0        0      522 2024-05-09 20:22:13.126023 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-sdl2-hello.vcxproj.filters
+-rw-r--r--   0        0        0     2482 2024-05-09 20:22:13.126023 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-version-paths.props
+-rw-r--r--   0        0        0    12161 2024-05-09 20:22:13.126023 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.sln
+-rw-r--r--   0        0        0    48329 2024-05-09 20:22:13.126023 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj
+-rw-r--r--   0        0        0    14547 2024-05-09 20:22:13.126023 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj.filters
+-rw-r--r--   0        0        0     3009 2024-05-09 20:22:13.126023 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj.filtersin
+-rw-r--r--   0        0        0    41403 2024-05-09 20:22:13.126023 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxprojin
+-rw-r--r--   0        0        0      919 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/Makefile.am
+-rw-r--r--   0        0        0    19171 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/Makefile.in
+-rw-r--r--   0        0        0     4783 2024-05-09 20:22:13.110384 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/README.txt
+-rw-r--r--   0        0        0    13941 2024-05-09 20:22:13.126023 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj
+-rw-r--r--   0        0        0     5574 2024-05-09 20:22:13.126023 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj.filters
+-rw-r--r--   0        0        0      563 2024-05-09 20:22:13.126023 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj.filtersin
+-rw-r--r--   0        0        0     9905 2024-05-09 20:22:13.126023 gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxprojin
+-rw-r--r--   0        0        0   244356 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/cogl/GL/glcorearb.h
+-rw-r--r--   0        0        0   810011 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/cogl/GL/glext.h
+-rw-r--r--   0        0        0    48113 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/cogl/GL/glxext.h
+-rw-r--r--   0        0        0    44095 2024-05-09 20:22:13.094768 gvsbuild-2024.5.0/gvsbuild/patches/cogl/GL/wglext.h
+-rw-r--r--   0        0        0     1121 2024-05-09 20:22:13.126023 gvsbuild-2024.5.0/gvsbuild/patches/cyrus-sasl/0001-Add-MIT-Kerberos-as-GSSAPI-provider.patch
+-rw-r--r--   0        0        0     1060 2024-05-09 20:22:13.126023 gvsbuild-2024.5.0/gvsbuild/patches/cyrus-sasl/0001-Fix-openssl-libs-to-point-to-the-new-openssl-1.1.1-n.patch
+-rw-r--r--   0        0        0      740 2024-05-09 20:22:13.126023 gvsbuild-2024.5.0/gvsbuild/patches/cyrus-sasl/0001-fix-snprintf-macro.patch
+-rw-r--r--   0        0        0     1135 2024-05-09 20:22:13.126023 gvsbuild-2024.5.0/gvsbuild/patches/cyrus-sasl/0002-Provide-a-compile-option-for-32-64-gssapi.patch
+-rw-r--r--   0        0        0     1045 2024-05-09 20:22:13.126023 gvsbuild-2024.5.0/gvsbuild/patches/cyrus-sasl/include/md5global.h
+-rw-r--r--   0        0        0      312 2024-05-09 20:22:13.126023 gvsbuild-2024.5.0/gvsbuild/patches/cyrus-sasl/pc-files/libsasl2.pc
+-rw-r--r--   0        0        0      418 2024-05-09 20:22:13.126023 gvsbuild-2024.5.0/gvsbuild/patches/enchant/src/config.h
+-rw-r--r--   0        0        0      660 2024-05-09 20:22:13.126023 gvsbuild-2024.5.0/gvsbuild/patches/enchant/src/libenchant.rc
+-rw-r--r--   0        0        0    17426 2024-05-09 20:22:13.126023 gvsbuild-2024.5.0/gvsbuild/patches/enchant/src/makefile.mak
+-rw-r--r--   0        0        0      754 2024-05-09 20:22:13.126023 gvsbuild-2024.5.0/gvsbuild/patches/expat/0001-CMakeLists-do-not-add-postfix-d-in-debug-builds.patch
+-rw-r--r--   0        0        0     2152 2024-05-09 20:22:13.126023 gvsbuild-2024.5.0/gvsbuild/patches/ffmpeg/build/build.sh
+-rw-r--r--   0        0        0      787 2024-05-09 20:22:13.126023 gvsbuild-2024.5.0/gvsbuild/patches/freetype/0001-meson-in-shared-libraries-we-need-to-export-the-meth.patch
+-rw-r--r--   0        0        0     3296 2024-05-09 20:22:13.126023 gvsbuild-2024.5.0/gvsbuild/patches/gettext/gettext-runtime-c99.patch
+-rw-r--r--   0        0        0    33686 2024-05-09 20:22:13.126023 gvsbuild-2024.5.0/gvsbuild/patches/gettext/gettext-tools-c99.patch
+-rw-r--r--   0        0        0      367 2024-05-09 20:22:13.126023 gvsbuild-2024.5.0/gvsbuild/patches/gettext/gettext-tools-gnulib-memset.patch
+-rw-r--r--   0        0        0     9543 2024-05-09 20:22:13.126023 gvsbuild-2024.5.0/gvsbuild/patches/gettext/libtextstyle-c99.patch
+-rw-r--r--   0        0        0     3065 2024-05-09 20:22:13.126023 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/alloca.h
+-rw-r--r--   0        0        0     7623 2024-05-09 20:22:13.126023 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/errno.h
+-rw-r--r--   0        0        0    33617 2024-05-09 20:22:13.126023 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/fcntl.h
+-rw-r--r--   0        0        0     2128 2024-05-09 20:22:13.126023 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/getopt-cdefs.h
+-rw-r--r--   0        0        0     3334 2024-05-09 20:22:13.126023 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/getopt.h
+-rw-r--r--   0        0        0    26308 2024-05-09 20:22:13.126023 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/iconv.h
+-rw-r--r--   0        0        0    43681 2024-05-09 20:22:13.126023 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/inttypes.h
+-rw-r--r--   0        0        0    27515 2024-05-09 20:22:13.126023 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/langinfo.h
+-rw-r--r--   0        0        0     4377 2024-05-09 20:22:13.126023 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/limits.h
+-rw-r--r--   0        0        0    32044 2024-05-09 20:22:13.126023 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/locale.h
+-rw-r--r--   0        0        0    37498 2024-05-09 20:22:13.126023 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/signal.h
+-rw-r--r--   0        0        0     4322 2024-05-09 20:22:13.126023 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/stddef.h
+-rw-r--r--   0        0        0    63279 2024-05-09 20:22:13.126023 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/stdlib.h
+-rw-r--r--   0        0        0    63715 2024-05-09 20:22:13.126023 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/string.h
+-rw-r--r--   0        0        0    44998 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/sys/stat.h
+-rw-r--r--   0        0        0     3250 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/sys/types.h
+-rw-r--r--   0        0        0    35655 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/time.h
+-rw-r--r--   0        0        0    81450 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unistd.h
+-rw-r--r--   0        0        0    24256 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unistr.h
+-rw-r--r--   0        0        0     2201 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unitypes.h
+-rw-r--r--   0        0        0     2239 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/uniwidth.h
+-rw-r--r--   0        0        0    62421 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/wchar.h
+-rw-r--r--   0        0        0    38906 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/wctype.h
+-rw-r--r--   0        0        0    20126 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/intl/libgnuintl.h
+-rw-r--r--   0        0        0    19299 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/intl/libintl.h
+-rw-r--r--   0        0        0     3088 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/alloca.h
+-rw-r--r--   0        0        0     2708 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/autosprintf.h
+-rw-r--r--   0        0        0     7648 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/errno.h
+-rw-r--r--   0        0        0     3065 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/alloca.h
+-rw-r--r--   0        0        0     2093 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/byteswap.h
+-rw-r--r--   0        0        0    22716 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/ctype.h
+-rw-r--r--   0        0        0    30933 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/dirent.h
+-rw-r--r--   0        0        0     7623 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/errno.h
+-rw-r--r--   0        0        0    33701 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/fcntl.h
+-rw-r--r--   0        0        0    25904 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/fnmatch.h
+-rw-r--r--   0        0        0     2128 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/getopt-cdefs.h
+-rw-r--r--   0        0        0     3334 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/getopt.h
+-rw-r--r--   0        0        0    26308 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/iconv.h
+-rw-r--r--   0        0        0    43508 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/inttypes.h
+-rw-r--r--   0        0        0    27538 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/langinfo.h
+-rw-r--r--   0        0        0     4658 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/c14n.h
+-rw-r--r--   0        0        0     6506 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/catalog.h
+-rw-r--r--   0        0        0     6869 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/chvalid.h
+-rw-r--r--   0        0        0     6788 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/debugXML.h
+-rw-r--r--   0        0        0     3460 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/dict.h
+-rw-r--r--   0        0        0     4672 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/DOCBparser.h
+-rw-r--r--   0        0        0    10171 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/encoding.h
+-rw-r--r--   0        0        0     6282 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/entities.h
+-rw-r--r--   0        0        0    16639 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/globals.h
+-rw-r--r--   0        0        0     8258 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/hash.h
+-rw-r--r--   0        0        0    11135 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/HTMLparser.h
+-rw-r--r--   0        0        0     5212 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/HTMLtree.h
+-rw-r--r--   0        0        0     4904 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/list.h
+-rw-r--r--   0        0        0     5340 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/nanoftp.h
+-rw-r--r--   0        0        0     3505 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/nanohttp.h
+-rw-r--r--   0        0        0    42377 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/parser.h
+-rw-r--r--   0        0        0    19481 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/parserInternals.h
+-rw-r--r--   0        0        0     4105 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/pattern.h
+-rw-r--r--   0        0        0     7632 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/relaxng.h
+-rw-r--r--   0        0        0     5931 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/SAX.h
+-rw-r--r--   0        0        0     6544 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/SAX2.h
+-rw-r--r--   0        0        0    28618 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/schemasInternals.h
+-rw-r--r--   0        0        0     5930 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/schematron.h
+-rw-r--r--   0        0        0     3466 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/threads.h
+-rw-r--r--   0        0        0    40837 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/tree.h
+-rw-r--r--   0        0        0     4177 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/uri.h
+-rw-r--r--   0        0        0    15497 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/valid.h
+-rw-r--r--   0        0        0     4515 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xinclude.h
+-rw-r--r--   0        0        0     6648 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xlink.h
+-rw-r--r--   0        0        0     5521 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlautomata.h
+-rw-r--r--   0        0        0    39148 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlerror.h
+-rw-r--r--   0        0        0     5514 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlexports.h
+-rw-r--r--   0        0        0    12396 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlIO.h
+-rw-r--r--   0        0        0     7586 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlmemory.h
+-rw-r--r--   0        0        0     2646 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlmodule.h
+-rw-r--r--   0        0        0    14454 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlreader.h
+-rw-r--r--   0        0        0     7099 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlregexp.h
+-rw-r--r--   0        0        0     3844 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlsave.h
+-rw-r--r--   0        0        0     8732 2024-05-09 20:22:13.141692 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlschemas.h
+-rw-r--r--   0        0        0     6409 2024-05-09 20:22:13.157274 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlschemastypes.h
+-rw-r--r--   0        0        0     7070 2024-05-09 20:22:13.157274 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlstring.h
+-rw-r--r--   0        0        0    11675 2024-05-09 20:22:13.157274 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlunicode.h
+-rw-r--r--   0        0        0    10024 2024-05-09 20:22:13.157274 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlversion.h
+-rw-r--r--   0        0        0    23172 2024-05-09 20:22:13.157274 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlwriter.h
+-rw-r--r--   0        0        0    18374 2024-05-09 20:22:13.157274 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpath.h
+-rw-r--r--   0        0        0    21404 2024-05-09 20:22:13.157274 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpathInternals.h
+-rw-r--r--   0        0        0     4892 2024-05-09 20:22:13.157274 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpointer.h
+-rw-r--r--   0        0        0     4377 2024-05-09 20:22:13.157274 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/limits.h
+-rw-r--r--   0        0        0    32067 2024-05-09 20:22:13.157274 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/locale.h
+-rw-r--r--   0        0        0     1209 2024-05-09 20:22:13.157274 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/omp.h
+-rw-r--r--   0        0        0    23409 2024-05-09 20:22:13.157274 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sched.h
+-rw-r--r--   0        0        0    37554 2024-05-09 20:22:13.157274 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/signal.h
+-rw-r--r--   0        0        0    61302 2024-05-09 20:22:13.157274 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/spawn.h
+-rw-r--r--   0        0        0     4298 2024-05-09 20:22:13.157274 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/stddef.h
+-rw-r--r--   0        0        0    63335 2024-05-09 20:22:13.157274 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/stdlib.h
+-rw-r--r--   0        0        0    63743 2024-05-09 20:22:13.157274 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/string.h
+-rw-r--r--   0        0        0    24900 2024-05-09 20:22:13.157274 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/random.h
+-rw-r--r--   0        0        0    32949 2024-05-09 20:22:13.157274 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/select.h
+-rw-r--r--   0        0        0    44998 2024-05-09 20:22:13.157274 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/stat.h
+-rw-r--r--   0        0        0    29890 2024-05-09 20:22:13.157274 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/time.h
+-rw-r--r--   0        0        0     3250 2024-05-09 20:22:13.157274 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/types.h
+-rw-r--r--   0        0        0    24835 2024-05-09 20:22:13.157274 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/wait.h
+-rw-r--r--   0        0        0    35681 2024-05-09 20:22:13.157274 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/time.h
+-rw-r--r--   0        0        0     7748 2024-05-09 20:22:13.157274 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniconv.h
+-rw-r--r--   0        0        0    42529 2024-05-09 20:22:13.157274 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unictype.h
+-rw-r--r--   0        0        0     4287 2024-05-09 20:22:13.157274 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unilbrk.h
+-rw-r--r--   0        0        0     1625 2024-05-09 20:22:13.157274 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniname.h
+-rw-r--r--   0        0        0    81730 2024-05-09 20:22:13.157274 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unistd.h
+-rw-r--r--   0        0        0    24256 2024-05-09 20:22:13.157274 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unistr.h
+-rw-r--r--   0        0        0     2201 2024-05-09 20:22:13.157274 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unitypes.h
+-rw-r--r--   0        0        0     2239 2024-05-09 20:22:13.157274 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniwidth.h
+-rw-r--r--   0        0        0    24592 2024-05-09 20:22:13.157274 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/utime.h
+-rw-r--r--   0        0        0    62584 2024-05-09 20:22:13.157274 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/wchar.h
+-rw-r--r--   0        0        0    38904 2024-05-09 20:22:13.157274 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/wctype.h
+-rw-r--r--   0        0        0    27214 2024-05-09 20:22:13.157274 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/arpa/inet.h
+-rw-r--r--   0        0        0     1287 2024-05-09 20:22:13.157274 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/netinet/in.h
+-rw-r--r--   0        0        0    91289 2024-05-09 20:22:13.157274 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/pthread.h
+-rw-r--r--   0        0        0     4873 2024-05-09 20:22:13.157274 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/stdalign.h
+-rw-r--r--   0        0        0    23344 2024-05-09 20:22:13.157274 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/ioctl.h
+-rw-r--r--   0        0        0    46391 2024-05-09 20:22:13.157274 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/socket.h
+-rw-r--r--   0        0        0     1629 2024-05-09 20:22:13.157274 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/uio.h
+-rw-r--r--   0        0        0     3065 2024-05-09 20:22:13.172905 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/alloca.h
+-rw-r--r--   0        0        0     7648 2024-05-09 20:22:13.172905 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/errno.h
+-rw-r--r--   0        0        0    33726 2024-05-09 20:22:13.172905 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/fcntl.h
+-rw-r--r--   0        0        0    17539 2024-05-09 20:22:13.172905 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/gettext-po.h
+-rw-r--r--   0        0        0    26333 2024-05-09 20:22:13.172905 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/iconv.h
+-rw-r--r--   0        0        0    43508 2024-05-09 20:22:13.172905 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/inttypes.h
+-rw-r--r--   0        0        0     4402 2024-05-09 20:22:13.172905 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/limits.h
+-rw-r--r--   0        0        0    32092 2024-05-09 20:22:13.172905 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/locale.h
+-rw-r--r--   0        0        0    37579 2024-05-09 20:22:13.172905 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/signal.h
+-rw-r--r--   0        0        0     4333 2024-05-09 20:22:13.172905 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/stddef.h
+-rw-r--r--   0        0        0    63360 2024-05-09 20:22:13.172905 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/stdlib.h
+-rw-r--r--   0        0        0    63768 2024-05-09 20:22:13.172905 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/string.h
+-rw-r--r--   0        0        0    45023 2024-05-09 20:22:13.172905 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/sys/stat.h
+-rw-r--r--   0        0        0     3275 2024-05-09 20:22:13.172905 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/sys/types.h
+-rw-r--r--   0        0        0    13023 2024-05-09 20:22:13.172905 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/textstyle.h
+-rw-r--r--   0        0        0    35677 2024-05-09 20:22:13.172905 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/time.h
+-rw-r--r--   0        0        0     7748 2024-05-09 20:22:13.172905 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/uniconv.h
+-rw-r--r--   0        0        0    42529 2024-05-09 20:22:13.172905 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unictype.h
+-rw-r--r--   0        0        0     4287 2024-05-09 20:22:13.172905 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unilbrk.h
+-rw-r--r--   0        0        0    81764 2024-05-09 20:22:13.172905 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unistd.h
+-rw-r--r--   0        0        0    24256 2024-05-09 20:22:13.172905 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unistr.h
+-rw-r--r--   0        0        0     2201 2024-05-09 20:22:13.172905 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unitypes.h
+-rw-r--r--   0        0        0     2239 2024-05-09 20:22:13.172905 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/uniwidth.h
+-rw-r--r--   0        0        0    62609 2024-05-09 20:22:13.172905 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/wchar.h
+-rw-r--r--   0        0        0    38929 2024-05-09 20:22:13.172905 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/wctype.h
+-rw-r--r--   0        0        0    27563 2024-05-09 20:22:13.172905 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgrep/langinfo.h
+-rw-r--r--   0        0        0     4432 2024-05-09 20:22:13.172905 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/stdbool.h
+-rw-r--r--   0        0        0     1392 2024-05-09 20:22:13.172905 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/version.h
+-rw-r--r--   0        0        0     1230 2024-05-09 20:22:13.172905 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/woe32dll.h
+-rw-r--r--   0        0        0    23446 2024-05-09 20:22:13.172905 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle.h
+-rw-r--r--   0        0        0     3065 2024-05-09 20:22:13.172905 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/alloca.h
+-rw-r--r--   0        0        0     7643 2024-05-09 20:22:13.172905 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/errno.h
+-rw-r--r--   0        0        0    33637 2024-05-09 20:22:13.172905 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/fcntl.h
+-rw-r--r--   0        0        0     4938 2024-05-09 20:22:13.172905 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/ghash.h
+-rw-r--r--   0        0        0     5545 2024-05-09 20:22:13.172905 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/glist.h
+-rw-r--r--   0        0        0     9729 2024-05-09 20:22:13.172905 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gmacros.h
+-rw-r--r--   0        0        0     2028 2024-05-09 20:22:13.172905 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gprimes.h
+-rw-r--r--   0        0        0     2257 2024-05-09 20:22:13.172905 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gprintfint.h
+-rw-r--r--   0        0        0    10124 2024-05-09 20:22:13.172905 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gstrfuncs.h
+-rw-r--r--   0        0        0     6212 2024-05-09 20:22:13.172905 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gstring.h
+-rw-r--r--   0        0        0    16052 2024-05-09 20:22:13.172905 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gtypes.h
+-rw-r--r--   0        0        0     2765 2024-05-09 20:22:13.172905 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib.h
+-rw-r--r--   0        0        0     6279 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glibconfig.h
+-rw-r--r--   0        0        0    43677 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/inttypes.h
+-rw-r--r--   0        0        0     4658 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/c14n.h
+-rw-r--r--   0        0        0     6506 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/catalog.h
+-rw-r--r--   0        0        0     6869 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/chvalid.h
+-rw-r--r--   0        0        0     6788 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/debugXML.h
+-rw-r--r--   0        0        0     3460 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/dict.h
+-rw-r--r--   0        0        0     4672 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/DOCBparser.h
+-rw-r--r--   0        0        0    10171 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/encoding.h
+-rw-r--r--   0        0        0     6282 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/entities.h
+-rw-r--r--   0        0        0    16639 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/globals.h
+-rw-r--r--   0        0        0     8258 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/hash.h
+-rw-r--r--   0        0        0    11135 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/HTMLparser.h
+-rw-r--r--   0        0        0     5212 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/HTMLtree.h
+-rw-r--r--   0        0        0     4904 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/list.h
+-rw-r--r--   0        0        0     5340 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/nanoftp.h
+-rw-r--r--   0        0        0     3505 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/nanohttp.h
+-rw-r--r--   0        0        0    42377 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/parser.h
+-rw-r--r--   0        0        0    19481 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/parserInternals.h
+-rw-r--r--   0        0        0     4105 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/pattern.h
+-rw-r--r--   0        0        0     7632 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/relaxng.h
+-rw-r--r--   0        0        0     5931 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/SAX.h
+-rw-r--r--   0        0        0     6544 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/SAX2.h
+-rw-r--r--   0        0        0    28618 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/schemasInternals.h
+-rw-r--r--   0        0        0     5930 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/schematron.h
+-rw-r--r--   0        0        0     3466 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/threads.h
+-rw-r--r--   0        0        0    40837 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/tree.h
+-rw-r--r--   0        0        0     4177 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/uri.h
+-rw-r--r--   0        0        0    15497 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/valid.h
+-rw-r--r--   0        0        0     4515 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xinclude.h
+-rw-r--r--   0        0        0     6648 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xlink.h
+-rw-r--r--   0        0        0     5521 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlautomata.h
+-rw-r--r--   0        0        0    39148 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlerror.h
+-rw-r--r--   0        0        0     5514 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlexports.h
+-rw-r--r--   0        0        0    12396 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlIO.h
+-rw-r--r--   0        0        0     7586 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlmemory.h
+-rw-r--r--   0        0        0     2646 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlmodule.h
+-rw-r--r--   0        0        0    14454 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlreader.h
+-rw-r--r--   0        0        0     7099 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlregexp.h
+-rw-r--r--   0        0        0     3844 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlsave.h
+-rw-r--r--   0        0        0     8732 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlschemas.h
+-rw-r--r--   0        0        0     6409 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlschemastypes.h
+-rw-r--r--   0        0        0     7070 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlstring.h
+-rw-r--r--   0        0        0    11675 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlunicode.h
+-rw-r--r--   0        0        0    10024 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlversion.h
+-rw-r--r--   0        0        0    23172 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlwriter.h
+-rw-r--r--   0        0        0    18374 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpath.h
+-rw-r--r--   0        0        0    21404 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpathInternals.h
+-rw-r--r--   0        0        0     4892 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpointer.h
+-rw-r--r--   0        0        0     4396 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/limits.h
+-rw-r--r--   0        0        0    37518 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/signal.h
+-rw-r--r--   0        0        0     4873 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdalign.h
+-rw-r--r--   0        0        0     4326 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stddef.h
+-rw-r--r--   0        0        0    23157 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdint.h
+-rw-r--r--   0        0        0    63299 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdlib.h
+-rw-r--r--   0        0        0    63735 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/string.h
+-rw-r--r--   0        0        0    46251 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/socket.h
+-rw-r--r--   0        0        0    45018 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/stat.h
+-rw-r--r--   0        0        0    29922 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/time.h
+-rw-r--r--   0        0        0     3272 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/types.h
+-rw-r--r--   0        0        0     1649 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/uio.h
+-rw-r--r--   0        0        0     4432 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/stdbool.h
+-rw-r--r--   0        0        0     1392 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/version.h
+-rw-r--r--   0        0        0     1230 2024-05-09 20:22:13.188622 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/woe32dll.h
+-rw-r--r--   0        0        0    35661 2024-05-09 20:22:13.204147 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/time.h
+-rw-r--r--   0        0        0    81477 2024-05-09 20:22:13.204147 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unistd.h
+-rw-r--r--   0        0        0    24256 2024-05-09 20:22:13.204147 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unistr.h
+-rw-r--r--   0        0        0     2201 2024-05-09 20:22:13.204147 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unitypes.h
+-rw-r--r--   0        0        0    62439 2024-05-09 20:22:13.204147 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/wchar.h
+-rw-r--r--   0        0        0    54409 2024-05-09 20:22:13.204147 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/config.h
+-rw-r--r--   0        0        0    23289 2024-05-09 20:22:13.204147 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/gnulib-lib/stdint.h
+-rw-r--r--   0        0        0    75068 2024-05-09 20:22:13.204147 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/gnulib-lib/stdio.h
+-rw-r--r--   0        0        0    97908 2024-05-09 20:22:13.204147 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/config.h
+-rw-r--r--   0        0        0     1932 2024-05-09 20:22:13.204147 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/configmake.h
+-rw-r--r--   0        0        0    93885 2024-05-09 20:22:13.204147 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/math.h
+-rw-r--r--   0        0        0    23289 2024-05-09 20:22:13.204147 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/stdint.h
+-rw-r--r--   0        0        0    75124 2024-05-09 20:22:13.204147 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/stdio.h
+-rw-r--r--   0        0        0    22207 2024-05-09 20:22:13.204147 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/config.h
+-rw-r--r--   0        0        0    23319 2024-05-09 20:22:13.204147 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/stdint.h
+-rw-r--r--   0        0        0    75149 2024-05-09 20:22:13.204147 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/stdio.h
+-rw-r--r--   0        0        0    49880 2024-05-09 20:22:13.204147 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/config.h
+-rw-r--r--   0        0        0    78389 2024-05-09 20:22:13.204147 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/config.h
+-rw-r--r--   0        0        0    93905 2024-05-09 20:22:13.204147 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/math.h
+-rw-r--r--   0        0        0    75079 2024-05-09 20:22:13.204147 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/stdio.h
+-rw-r--r--   0        0        0    54408 2024-05-09 20:22:13.204147 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/config.h
+-rw-r--r--   0        0        0    23289 2024-05-09 20:22:13.204147 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/gnulib-lib/stdint.h
+-rw-r--r--   0        0        0    75065 2024-05-09 20:22:13.204147 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/gnulib-lib/stdio.h
+-rw-r--r--   0        0        0    97907 2024-05-09 20:22:13.204147 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/config.h
+-rw-r--r--   0        0        0     1932 2024-05-09 20:22:13.204147 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/configmake.h
+-rw-r--r--   0        0        0    93885 2024-05-09 20:22:13.204147 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/math.h
+-rw-r--r--   0        0        0    23289 2024-05-09 20:22:13.204147 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/stdint.h
+-rw-r--r--   0        0        0    75121 2024-05-09 20:22:13.204147 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/stdio.h
+-rw-r--r--   0        0        0    22207 2024-05-09 20:22:13.204147 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/config.h
+-rw-r--r--   0        0        0    23319 2024-05-09 20:22:13.204147 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/stdint.h
+-rw-r--r--   0        0        0    75146 2024-05-09 20:22:13.204147 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/stdio.h
+-rw-r--r--   0        0        0    49880 2024-05-09 20:22:13.204147 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/config.h
+-rw-r--r--   0        0        0    78389 2024-05-09 20:22:13.204147 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/config.h
+-rw-r--r--   0        0        0    93905 2024-05-09 20:22:13.204147 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/math.h
+-rw-r--r--   0        0        0    75079 2024-05-09 20:22:13.204147 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/stdio.h
+-rw-r--r--   0        0        0    54410 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/config.h
+-rw-r--r--   0        0        0    23133 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/gnulib-lib/stdint.h
+-rw-r--r--   0        0        0    74955 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/gnulib-lib/stdio.h
+-rw-r--r--   0        0        0    97906 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/config.h
+-rw-r--r--   0        0        0     1932 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/configmake.h
+-rw-r--r--   0        0        0    93830 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/math.h
+-rw-r--r--   0        0        0    23133 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/stdint.h
+-rw-r--r--   0        0        0    75011 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/stdio.h
+-rw-r--r--   0        0        0    21997 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/config.h
+-rw-r--r--   0        0        0    23163 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/stdint.h
+-rw-r--r--   0        0        0    75036 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/stdio.h
+-rw-r--r--   0        0        0    49879 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/config.h
+-rw-r--r--   0        0        0    78389 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/config.h
+-rw-r--r--   0        0        0    93850 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/math.h
+-rw-r--r--   0        0        0    74969 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/stdio.h
+-rw-r--r--   0        0        0    54407 2024-05-09 20:22:13.204147 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/config.h
+-rw-r--r--   0        0        0    23133 2024-05-09 20:22:13.204147 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/gnulib-lib/stdint.h
+-rw-r--r--   0        0        0    74958 2024-05-09 20:22:13.204147 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/gnulib-lib/stdio.h
+-rw-r--r--   0        0        0    97900 2024-05-09 20:22:13.204147 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/config.h
+-rw-r--r--   0        0        0     1984 2024-05-09 20:22:13.204147 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/configmake.h
+-rw-r--r--   0        0        0    93830 2024-05-09 20:22:13.204147 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/math.h
+-rw-r--r--   0        0        0    23133 2024-05-09 20:22:13.204147 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/stdint.h
+-rw-r--r--   0        0        0    75014 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/stdio.h
+-rw-r--r--   0        0        0    22207 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/config.h
+-rw-r--r--   0        0        0    23163 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/stdint.h
+-rw-r--r--   0        0        0    75039 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/stdio.h
+-rw-r--r--   0        0        0    49882 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/config.h
+-rw-r--r--   0        0        0    78389 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/config.h
+-rw-r--r--   0        0        0    93850 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/math.h
+-rw-r--r--   0        0        0    74969 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/stdio.h
+-rw-r--r--   0        0        0    54406 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/config.h
+-rw-r--r--   0        0        0    23133 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/gnulib-lib/stdint.h
+-rw-r--r--   0        0        0    74955 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/gnulib-lib/stdio.h
+-rw-r--r--   0        0        0    97945 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/config.h
+-rw-r--r--   0        0        0     1984 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/configmake.h
+-rw-r--r--   0        0        0    93830 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/math.h
+-rw-r--r--   0        0        0    23133 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/stdint.h
+-rw-r--r--   0        0        0    75011 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/stdio.h
+-rw-r--r--   0        0        0    22207 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/config.h
+-rw-r--r--   0        0        0    23163 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/stdint.h
+-rw-r--r--   0        0        0    75036 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/stdio.h
+-rw-r--r--   0        0        0    49882 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/config.h
+-rw-r--r--   0        0        0    78389 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/config.h
+-rw-r--r--   0        0        0    93850 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/math.h
+-rw-r--r--   0        0        0    74969 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/stdio.h
+-rw-r--r--   0        0        0    22956 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/nmake/build-rules-msvc.mak
+-rw-r--r--   0        0        0     6490 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/nmake/config-msvc.mak
+-rw-r--r--   0        0        0    16869 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/nmake/create-lists-msvc.mak
+-rwxr-xr-x   0        0        0      846 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/nmake/create-lists.bat
+-rw-r--r--   0        0        0     5708 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/nmake/detectenv-msvc.mak
+-rw-r--r--   0        0        0      772 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/nmake/generate-msvc.mak
+-rw-r--r--   0        0        0     4576 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/nmake/gettext-runtime-sources.mk
+-rw-r--r--   0        0        0     8982 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/nmake/gettext-tools-sources.mk
+-rw-r--r--   0        0        0     2466 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/nmake/libgettextlib.def
+-rw-r--r--   0        0        0     2852 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/nmake/libgettextsrc.def
+-rw-r--r--   0        0        0     3788 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/gettext/nmake/libtextstyle-sources.mk
+-rw-r--r--   0        0        0     2635 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/gettext/nmake/libtextstyle.def
+-rw-r--r--   0        0        0     1051 2024-05-09 20:22:13.219774 gvsbuild-2024.5.0/gvsbuild/patches/gettext/nmake/Makefile.vc
+-rw-r--r--   0        0        0     1582 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/glib/001-glib-package-installation-directory.patch
+-rw-r--r--   0        0        0     3238 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/glib/002-gir-scanner-dll-not-found.patch
+-rw-r--r--   0        0        0     1582 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/glib-base/001-glib-package-installation-directory.patch
+-rw-r--r--   0        0        0     3238 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/glib-base/002-gir-scanner-dll-not-found.patch
+-rw-r--r--   0        0        0     1209 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/glib-networking/add-null-check-in-complete_handshake.patch
+-rw-r--r--   0        0        0       30 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/glib-py-wrapper/glib-genmarshal.config
+-rw-r--r--   0        0        0       27 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/glib-py-wrapper/glib-mkenums.config
+-rw-r--r--   0        0        0     1123 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/glib-py-wrapper/glib-py-wrapper.c
+-rw-r--r--   0        0        0      394 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/glib-py-wrapper/meson.build
+-rw-r--r--   0        0        0      611 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/gobject-introspection/001-incorrect-giscanner-path.patch
+-rw-r--r--   0        0        0     1468 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/gsettings-desktop-schemas/0001-build-win32-replace.py-Fix-replacing-items-in-files-.patch
+-rw-r--r--   0        0        0      759 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/gsettings-desktop-schemas/0002-glib-mkenums-python.patch
+-rw-r--r--   0        0        0     2083 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/gst-plugins-bad/wasapisink-reduce-buffer-latency.patch
+-rw-r--r--   0        0        0     1958 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/gtk2/0001-GDK-W32-Remove-WS_EX_LAYERED-from-an-opaque-window.patch
+-rw-r--r--   0        0        0     1186 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/gtk2/61162225f712df648f38fd12bc0817cfa9f79a64.patch
+-rw-r--r--   0        0        0     1920 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/gtk2/bfdac2f70e005b2504cc3f4ebbdab328974d005a.patch
+-rw-r--r--   0        0        0     1956 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/introspection.body.mak
+-rw-r--r--   0        0        0     2185 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs12/gtk-version-paths.props
+-rw-r--r--   0        0        0     2185 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs14/gtk-version-paths.props
+-rw-r--r--   0        0        0    10679 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs15/gailutil.vcxproj
+-rw-r--r--   0        0        0     1080 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs15/gailutil.vcxproj.filters
+-rw-r--r--   0        0        0    11397 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs15/gdk-win32.vcxproj
+-rw-r--r--   0        0        0     3760 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs15/gdk-win32.vcxproj.filters
+-rw-r--r--   0        0        0    13364 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs15/gdk.vcxproj
+-rw-r--r--   0        0        0     4222 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs15/gdk.vcxproj.filters
+-rw-r--r--   0        0        0     6519 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk+.sln
+-rw-r--r--   0        0        0     3640 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-build-defines.props
+-rw-r--r--   0        0        0    12279 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-demo.vcxproj
+-rw-r--r--   0        0        0     4640 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-demo.vcxproj.filters
+-rw-r--r--   0        0        0     1962 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-gen-srcs.props
+-rw-r--r--   0        0        0    23804 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-install.props
+-rw-r--r--   0        0        0     7938 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-install.vcxproj
+-rw-r--r--   0        0        0     9247 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-update-icon-cache.vcxproj
+-rw-r--r--   0        0        0      706 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-update-icon-cache.vcxproj.filters
+-rw-r--r--   0        0        0     2185 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-version-paths.props
+-rw-r--r--   0        0        0    26897 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk.vcxproj
+-rw-r--r--   0        0        0    26470 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk.vcxproj.filters
+-rw-r--r--   0        0        0     9451 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs15/libwimp.vcxproj
+-rw-r--r--   0        0        0     1756 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs15/libwimp.vcxproj.filters
+-rw-r--r--   0        0        0     3586 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs15/README.txt
+-rw-r--r--   0        0        0      803 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/gtk2/gtk-accel.patch
+-rw-r--r--   0        0        0      599 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/gtk2/gtk-bgimg.patch
+-rw-r--r--   0        0        0      682 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/gtk2/gtk-multimonitor.patch
+-rw-r--r--   0        0        0     2154 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/gtk2/gtk-revert-scrolldc-commit.patch
+-rw-r--r--   0        0        0     1104 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/gtk2/mod.md
+-rw-r--r--   0        0        0     6104 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/gtk3/gdk/win32/gdkkeys-win32.h
+-rw-r--r--   0        0        0    11322 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/gtk3/gdk/win32/winpointer.h
+-rw-r--r--   0        0        0     1630 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/gtk3/gtk_update_icon_cache.patch
+-rw-r--r--   0        0        0     1088 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/gtksourceview5/001-fix-fontconfig-availability-check.patch
+-rw-r--r--   0        0        0      102 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/hello-world/hello-world.c
+-rw-r--r--   0        0        0       66 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/hello-world/meson.build
+-rw-r--r--   0        0        0      359 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/icu/pc-files/icu-uc.pc
+-rw-r--r--   0        0        0      360 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/icu/pc-files-debug/icu-uc.pc
+-rw-r--r--   0        0        0    39523 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/libadwaita/0001-remove-appstream-dependency.patch
+-rw-r--r--   0        0        0     4827 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/libffi/fficonfig.h.meson
+-rw-r--r--   0        0        0      475 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/libffi/include/meson.build
+-rw-r--r--   0        0        0      248 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/libffi/meson-scripts/extract-libtool-version.py
+-rw-r--r--   0        0        0    13940 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/libffi/meson.build
+-rw-r--r--   0        0        0     1154 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/libffi/meson_options.txt
+-rw-r--r--   0        0        0     3334 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/libffi/src/meson.build
+-rw-r--r--   0        0        0      936 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/libfido2/0001-Install-pkgconfig-files-also-on-msvc.patch
+-rw-r--r--   0        0        0     1243 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/libfido2/0001-libfido2-update-cmake-script-to-have-sdl-flag-before.patch
+-rw-r--r--   0        0        0     9777 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/libmicrohttpd/001-remove-postsample-perf-retries.patch
+-rw-r--r--   0        0        0       44 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/libpng/mod.md
+-rw-r--r--   0        0        0      318 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/libpng/pc-files/libpng.pc
+-rw-r--r--   0        0        0      318 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/libpng/pc-files/libpng16.pc
+-rw-r--r--   0        0        0     5490 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs12/config.h
+-rw-r--r--   0        0        0     8059 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs12/install.vcxproj
+-rw-r--r--   0        0        0      834 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs12/install.vcxproj.filters
+-rw-r--r--   0        0        0     3769 2024-05-09 20:22:13.235399 gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs12/libssh-library.sln
+-rw-r--r--   0        0        0     3074 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs12/property.props
+-rw-r--r--   0        0        0    40095 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs12/ssh_shared.vcxproj
+-rw-r--r--   0        0        0     5705 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs12/ssh_shared.vcxproj.filters
+-rw-r--r--   0        0        0    32139 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs12/ssh_static.vcxproj
+-rw-r--r--   0        0        0     5705 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs12/ssh_static.vcxproj.filters
+-rw-r--r--   0        0        0     5490 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs14/config.h
+-rw-r--r--   0        0        0     8059 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs14/install.vcxproj
+-rw-r--r--   0        0        0      834 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs14/install.vcxproj.filters
+-rw-r--r--   0        0        0     3767 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs14/libssh-library.sln
+-rw-r--r--   0        0        0     3074 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs14/property.props
+-rw-r--r--   0        0        0    40095 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs14/ssh_shared.vcxproj
+-rw-r--r--   0        0        0     5705 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs14/ssh_shared.vcxproj.filters
+-rw-r--r--   0        0        0    32139 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs14/ssh_static.vcxproj
+-rw-r--r--   0        0        0     5705 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs14/ssh_static.vcxproj.filters
+-rw-r--r--   0        0        0     5490 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs15/config.h
+-rw-r--r--   0        0        0     8138 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs15/install.vcxproj
+-rw-r--r--   0        0        0      834 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs15/install.vcxproj.filters
+-rw-r--r--   0        0        0     3899 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs15/libssh-library.sln
+-rw-r--r--   0        0        0     3074 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs15/property.props
+-rw-r--r--   0        0        0    40174 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs15/ssh_shared.vcxproj
+-rw-r--r--   0        0        0     5705 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs15/ssh_shared.vcxproj.filters
+-rw-r--r--   0        0        0    32139 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs15/ssh_static.vcxproj
+-rw-r--r--   0        0        0     5705 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs15/ssh_static.vcxproj.filters
+-rw-r--r--   0        0        0     1079 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/libssh/mod.md
+-rw-r--r--   0        0        0      809 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/libtiff-4/0001-cmake-remove-.d-postfix.patch
+-rw-r--r--   0        0        0     2586 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/libvpx/0001-Always-generate-pc-file.patch
+-rw-r--r--   0        0        0     1251 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/libvpx/0006-gen_msvs_vcxproj.sh-Select-current-Windows-SDK-if-av.patch
+-rw-r--r--   0        0        0     1025 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/libxml2/include/libxml/meson.build
+-rw-r--r--   0        0        0     1089 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/libxml2/LICENSE.build
+-rw-r--r--   0        0        0     7284 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/libxml2/meson.build
+-rw-r--r--   0        0        0      323 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/libxml2/pc-files/libxml-2.0.pc
+-rw-r--r--   0        0        0      943 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/libyuv/001-win-build.patch
+-rw-r--r--   0        0        0      392 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/libyuv/pc-files/libyuv.pc
+-rw-r--r--   0        0        0      352 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/luajit/pc-files/luajit.pc
+-rw-r--r--   0        0        0      971 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/luajit/set-paths.patch
+-rw-r--r--   0        0        0      319 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/lz4/pc-files/liblz4.pc
+-rw-r--r--   0        0        0     8964 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2013/datagen/datagen.vcxproj
+-rw-r--r--   0        0        0     9315 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2013/frametest/frametest.vcxproj
+-rw-r--r--   0        0        0     9315 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2013/fullbench/fullbench.vcxproj
+-rw-r--r--   0        0        0    10136 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2013/fullbench-dll/fullbench-dll.vcxproj
+-rw-r--r--   0        0        0     9143 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2013/fuzzer/fuzzer.vcxproj
+-rw-r--r--   0        0        0     9204 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2013/liblz4/liblz4.vcxproj
+-rw-r--r--   0        0        0     1388 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2013/liblz4-dll/liblz4-dll.rc
+-rw-r--r--   0        0        0     9307 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2013/liblz4-dll/liblz4-dll.vcxproj
+-rw-r--r--   0        0        0     1388 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2013/lz4/lz4.rc
+-rw-r--r--   0        0        0     9978 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2013/lz4/lz4.vcxproj
+-rw-r--r--   0        0        0     6761 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2013/lz4.sln
+-rw-r--r--   0        0        0     8964 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2015/datagen/datagen.vcxproj
+-rw-r--r--   0        0        0     9315 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2015/frametest/frametest.vcxproj
+-rw-r--r--   0        0        0     9315 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2015/fullbench/fullbench.vcxproj
+-rw-r--r--   0        0        0    10136 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2015/fullbench-dll/fullbench-dll.vcxproj
+-rw-r--r--   0        0        0     9143 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2015/fuzzer/fuzzer.vcxproj
+-rw-r--r--   0        0        0     9204 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2015/liblz4/liblz4.vcxproj
+-rw-r--r--   0        0        0     1388 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2015/liblz4-dll/liblz4-dll.rc
+-rw-r--r--   0        0        0     9307 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2015/liblz4-dll/liblz4-dll.vcxproj
+-rw-r--r--   0        0        0     1388 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2015/lz4/lz4.rc
+-rw-r--r--   0        0        0     9978 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2015/lz4/lz4.vcxproj
+-rw-r--r--   0        0        0     6761 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2015/lz4.sln
+-rw-r--r--   0        0        0     8966 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2017/datagen/datagen.vcxproj
+-rw-r--r--   0        0        0     9317 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2017/frametest/frametest.vcxproj
+-rw-r--r--   0        0        0     9317 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2017/fullbench/fullbench.vcxproj
+-rw-r--r--   0        0        0    10138 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2017/fullbench-dll/fullbench-dll.vcxproj
+-rw-r--r--   0        0        0     9145 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2017/fuzzer/fuzzer.vcxproj
+-rw-r--r--   0        0        0     9206 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2017/liblz4/liblz4.vcxproj
+-rw-r--r--   0        0        0     1388 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2017/liblz4-dll/liblz4-dll.rc
+-rw-r--r--   0        0        0     9309 2024-05-09 20:22:13.251023 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2017/liblz4-dll/liblz4-dll.vcxproj
+-rw-r--r--   0        0        0     1388 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2017/lz4/lz4.rc
+-rw-r--r--   0        0        0     9978 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2017/lz4/lz4.vcxproj
+-rw-r--r--   0        0        0     6761 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2017/lz4.sln
+-rw-r--r--   0        0        0     8964 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2022/datagen/datagen.vcxproj
+-rw-r--r--   0        0        0     9315 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2022/frametest/frametest.vcxproj
+-rw-r--r--   0        0        0     9315 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2022/fullbench/fullbench.vcxproj
+-rw-r--r--   0        0        0    10136 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2022/fullbench-dll/fullbench-dll.vcxproj
+-rw-r--r--   0        0        0     9143 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2022/fuzzer/fuzzer.vcxproj
+-rw-r--r--   0        0        0     9204 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2022/liblz4/liblz4.vcxproj
+-rw-r--r--   0        0        0     1388 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2022/liblz4-dll/liblz4-dll.rc
+-rw-r--r--   0        0        0     9307 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2022/liblz4-dll/liblz4-dll.vcxproj
+-rw-r--r--   0        0        0     1388 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2022/lz4/lz4.rc
+-rw-r--r--   0        0        0     9976 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2022/lz4/lz4.vcxproj
+-rw-r--r--   0        0        0     6761 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2022/lz4.sln
+-rw-r--r--   0        0        0       93 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/patches/mod.md
+-rw-r--r--   0        0        0      733 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/patches/nghttp2/0001-Define-ssize_t-if-not-defined.patch
+-rw-r--r--   0        0        0  1290625 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/patches/openssl-base/certdata.txt
+-rw-r--r--   0        0        0    19616 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/patches/openssl-base/mk-ca-bundle.pl
+-rw-r--r--   0        0        0      412 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/patches/openssl-base/mod.md
+-rw-r--r--   0        0        0      275 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/patches/openssl-base/pc-files/libcrypto.pc
+-rw-r--r--   0        0        0      285 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/patches/openssl-base/pc-files/libssl.pc
+-rw-r--r--   0        0        0      236 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/patches/openssl-base/pc-files/openssl.pc
+-rw-r--r--   0        0        0      403 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/patches/pango/001-disable-dwrite.patch
+-rw-r--r--   0        0        0    11464 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/patches/pango/002-fix-wrong-usage-gweakref.patch
+-rw-r--r--   0        0        0     1027 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/patches/pango/003-remove-extra-hb-face-font.patch
+-rw-r--r--   0        0        0     1089 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/patches/pcre2/LICENSE.build
+-rw-r--r--   0        0        0     7523 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/patches/pcre2/meson.build
+-rw-r--r--   0        0        0      473 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/patches/pcre2/meson_options.txt
+-rw-r--r--   0        0        0     1241 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/patches/pkgconf/0001-libpkgconf-add-defines-to-unbreak-build-with-VS2013.patch
+-rw-r--r--   0        0        0     1036 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/patches/protobuf-c/0001-Declare-variables-at-the-beginning-of-the-block.patch
+-rw-r--r--   0        0        0     2647 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/patches/protobuf-c/0001-Do-not-build-tests.patch
+-rw-r--r--   0        0        0      319 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/patches/protobuf-c/pc-files/libprotobuf-c.pc
+-rw-r--r--   0        0        0     1912 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/patches/pygobject/001-pygobject-py38-load-dll.patch
+-rw-r--r--   0        0        0      633 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/patches/stack.props
+-rw-r--r--   0        0        0     1565 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/patches/win-iconv/COPYING
+-rw-r--r--   0        0        0       92 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/patches/win-iconv/mod.md
+-rw-r--r--   0        0        0      671 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/patches/x264/build/build.sh
+-rw-r--r--   0        0        0     1385 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/patches/x264/x264-0001-Prevent-mb_info_free-to-be-called-before-all-threads.patch
+-rw-r--r--   0        0        0      343 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/patches/zlib/pc-files/zlib.pc
+-rw-r--r--   0        0        0     4259 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/projects/__init__.py
+-rw-r--r--   0        0        0     2040 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/projects/adwaita_icon_theme.py
+-rw-r--r--   0        0        0     1808 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/projects/atk.py
+-rw-r--r--   0        0        0     1774 2024-05-09 20:22:13.266649 gvsbuild-2024.5.0/gvsbuild/projects/boringssl.py
+-rw-r--r--   0        0        0     1642 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/cairo.py
+-rw-r--r--   0        0        0     1509 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/cairomm.py
+-rw-r--r--   0        0        0     1912 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/check_libs.py
+-rw-r--r--   0        0        0     1620 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/clutter.py
+-rw-r--r--   0        0        0     1758 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/cogl.py
+-rw-r--r--   0        0        0     2872 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/cyrus_sasl.py
+-rw-r--r--   0        0        0     2844 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/dev_shell.py
+-rw-r--r--   0        0        0     1648 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/emeus.py
+-rw-r--r--   0        0        0     2807 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/enchant.py
+-rw-r--r--   0        0        0     1572 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/expat.py
+-rw-r--r--   0        0        0     3386 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/ffmpeg.py
+-rw-r--r--   0        0        0     1725 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/freerdp.py
+-rw-r--r--   0        0        0     1638 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/freetype.py
+-rw-r--r--   0        0        0     2093 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/fribidi.py
+-rw-r--r--   0        0        0     2204 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/gdk_pixbuf.py
+-rw-r--r--   0        0        0     4032 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/gettext.py
+-rw-r--r--   0        0        0     4784 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/glib.py
+-rw-r--r--   0        0        0     1704 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/glibmm.py
+-rw-r--r--   0        0        0     2684 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/gobject_introspection.py
+-rw-r--r--   0        0        0     1312 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/gperf.py
+-rw-r--r--   0        0        0     1752 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/graphene.py
+-rw-r--r--   0        0        0     1813 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/gsettings_desktop_schemas.py
+-rw-r--r--   0        0        0     8703 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/gstreamer.py
+-rw-r--r--   0        0        0     5846 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/gtk.py
+-rw-r--r--   0        0        0     1806 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/gtkmm.py
+-rw-r--r--   0        0        0     2846 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/gtksourceview.py
+-rw-r--r--   0        0        0     1764 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/harfbuzz.py
+-rw-r--r--   0        0        0     1184 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/hello_world.py
+-rw-r--r--   0        0        0     1382 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/hicolor_icon_theme.py
+-rw-r--r--   0        0        0     2276 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/icu.py
+-rw-r--r--   0        0        0     1832 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/json_glib.py
+-rw-r--r--   0        0        0     1392 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/jsonc.py
+-rw-r--r--   0        0        0     1624 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/leveldb.py
+-rw-r--r--   0        0        0     1417 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/lgi.py
+-rw-r--r--   0        0        0     2027 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/libadwaita.py
+-rw-r--r--   0        0        0     2075 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/libarchive.py
+-rw-r--r--   0        0        0     1781 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/libcbor.py
+-rw-r--r--   0        0        0     1903 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/libcurl.py
+-rw-r--r--   0        0        0     1447 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/libepoxy.py
+-rw-r--r--   0        0        0     1341 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/libffi.py
+-rw-r--r--   0        0        0     2597 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/libfido2.py
+-rw-r--r--   0        0        0     1989 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/libgxps.py
+-rw-r--r--   0        0        0     1741 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/libjpeg_turbo.py
+-rw-r--r--   0        0        0     2331 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/libmicrohttpd.py
+-rw-r--r--   0        0        0     1948 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/libpanel.py
+-rw-r--r--   0        0        0     1704 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/libpng.py
+-rw-r--r--   0        0        0     1595 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/libpsl.py
+-rw-r--r--   0        0        0     2434 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/librsvg.py
+-rw-r--r--   0        0        0     1737 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/libsigcplusplus.py
+-rw-r--r--   0        0        0     3368 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/libsoup.py
+-rw-r--r--   0        0        0     2181 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/libssh.py
+-rw-r--r--   0        0        0     1586 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/libtiff.py
+-rw-r--r--   0        0        0     1514 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/libuv.py
+-rw-r--r--   0        0        0     1511 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/libvorbis.py
+-rw-r--r--   0        0        0     3265 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/libvpx.py
+-rw-r--r--   0        0        0     1574 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/libxml2.py
+-rw-r--r--   0        0        0     1576 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/libyuv.py
+-rw-r--r--   0        0        0     1411 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/libzip.py
+-rw-r--r--   0        0        0     1426 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/lmdb.py
+-rw-r--r--   0        0        0     1761 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/luajit.py
+-rw-r--r--   0        0        0     1778 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/lz4.py
+-rw-r--r--   0        0        0     2279 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/mit_kerberos.py
+-rw-r--r--   0        0        0     1587 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/nghttp2.py
+-rw-r--r--   0        0        0     1477 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/ogg.py
+-rw-r--r--   0        0        0     1521 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/openh264.py
+-rw-r--r--   0        0        0     3320 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/openssl.py
+-rw-r--r--   0        0        0     1578 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/opus.py
+-rw-r--r--   0        0        0     2091 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/pango.py
+-rw-r--r--   0        0        0     1768 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/pangomm.py
+-rw-r--r--   0        0        0      712 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/pcre2.py
+-rw-r--r--   0        0        0     1672 2024-05-09 20:22:13.282267 gvsbuild-2024.5.0/gvsbuild/projects/pixman.py
+-rw-r--r--   0        0        0     1692 2024-05-09 20:22:13.297892 gvsbuild-2024.5.0/gvsbuild/projects/pkgconf.py
+-rw-r--r--   0        0        0     2711 2024-05-09 20:22:13.297892 gvsbuild-2024.5.0/gvsbuild/projects/protobuf.py
+-rw-r--r--   0        0        0     2102 2024-05-09 20:22:13.297892 gvsbuild-2024.5.0/gvsbuild/projects/pycairo.py
+-rw-r--r--   0        0        0     2591 2024-05-09 20:22:13.297892 gvsbuild-2024.5.0/gvsbuild/projects/pygobject.py
+-rw-r--r--   0        0        0     1618 2024-05-09 20:22:13.297892 gvsbuild-2024.5.0/gvsbuild/projects/sqlite.py
+-rw-r--r--   0        0        0     1607 2024-05-09 20:22:13.297892 gvsbuild-2024.5.0/gvsbuild/projects/win_iconv.py
+-rw-r--r--   0        0        0     1470 2024-05-09 20:22:13.297892 gvsbuild-2024.5.0/gvsbuild/projects/wing.py
+-rw-r--r--   0        0        0     2341 2024-05-09 20:22:13.297892 gvsbuild-2024.5.0/gvsbuild/projects/x264.py
+-rw-r--r--   0        0        0     2444 2024-05-09 20:22:13.297892 gvsbuild-2024.5.0/gvsbuild/projects/zlib.py
+-rw-r--r--   0        0        0     7601 2024-05-09 20:22:13.297892 gvsbuild-2024.5.0/gvsbuild/tools.py
+-rw-r--r--   0        0        0       30 2024-05-09 20:22:13.297892 gvsbuild-2024.5.0/gvsbuild/utils/__init__.py
+-rw-r--r--   0        0        0     8512 2024-05-09 20:22:13.297892 gvsbuild-2024.5.0/gvsbuild/utils/base_builders.py
+-rw-r--r--   0        0        0    15193 2024-05-09 20:22:13.297892 gvsbuild-2024.5.0/gvsbuild/utils/base_expanders.py
+-rw-r--r--   0        0        0     1339 2024-05-09 20:22:13.297892 gvsbuild-2024.5.0/gvsbuild/utils/base_group.py
+-rw-r--r--   0        0        0    20353 2024-05-09 20:22:13.297892 gvsbuild-2024.5.0/gvsbuild/utils/base_project.py
+-rw-r--r--   0        0        0     2749 2024-05-09 20:22:13.297892 gvsbuild-2024.5.0/gvsbuild/utils/base_tool.py
+-rw-r--r--   0        0        0    38283 2024-05-09 20:22:13.297892 gvsbuild-2024.5.0/gvsbuild/utils/builder.py
+-rw-r--r--   0        0        0     9897 2024-05-09 20:22:13.297892 gvsbuild-2024.5.0/gvsbuild/utils/simple_ui.py
+-rw-r--r--   0        0        0     3899 2024-05-09 20:22:13.297892 gvsbuild-2024.5.0/gvsbuild/utils/utils.py
+-rw-r--r--   0        0        0     1733 2024-05-09 20:22:13.297892 gvsbuild-2024.5.0/pyproject.toml
+-rw-r--r--   0        0        0    12945 2024-05-09 20:22:13.063511 gvsbuild-2024.5.0/README.md
+-rw-r--r--   0        0        0    13732 1970-01-01 00:00:00.000000 gvsbuild-2024.5.0/PKG-INFO
```

### Comparing `gvsbuild-2024.4.1/AUTHORS.md` & `gvsbuild-2024.5.0/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/COPYING` & `gvsbuild-2024.5.0/COPYING`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/build.py` & `gvsbuild-2024.5.0/gvsbuild/build.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/deps.py` & `gvsbuild-2024.5.0/gvsbuild/deps.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/groups.py` & `gvsbuild-2024.5.0/gvsbuild/groups.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/list.py` & `gvsbuild-2024.5.0/gvsbuild/list.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
                         "version": f"{project.version:<45}",
                     }
                     if latest:
                         if (
                             hasattr(project, "latest_version")
                             and project.latest_version
                         ):
-                            params[
-                                "latest_version"
-                            ] = f"{str(project.latest_version):<45}"
+                            params["latest_version"] = (
+                                f"{str(project.latest_version):<45}"
+                            )
                         else:
                             params["latest_version"] = "undefined"
                         print("\t{name} {version} {latest_version}".format(**params))
                     else:
                         print("\t{name} {version}".format(**params))
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/main.py` & `gvsbuild-2024.5.0/gvsbuild/main.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/outdated.py` & `gvsbuild-2024.5.0/gvsbuild/outdated.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cairo/0001-fix-alloca-unresolved.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/cairo/0001-fix-alloca-unresolved.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/check-libs/check_utils.h` & `gvsbuild-2024.5.0/gvsbuild/patches/check-libs/check_utils.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/check-libs/COPYING` & `gvsbuild-2024.5.0/gvsbuild/patches/check-libs/COPYING`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/check-libs/meson.build` & `gvsbuild-2024.5.0/gvsbuild/patches/check-libs/meson.build`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atkcomponent-example.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkcomponent-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atkcomponent-example.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkcomponent-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atkeditabletext-example.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkeditabletext-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atkeditabletext-example.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkeditabletext-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atkevents-example.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkevents-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atkevents-example.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atkevents-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atktext-example.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atktext-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/cally-atktext-example.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/cally-atktext-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/cally-clone-example.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/cally-clone-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/cally-clone-example.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/cally-clone-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/clutter-build-defines.props` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-build-defines.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/clutter-gen-srcs.props` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-gen-srcs.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/clutter-install.props` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-install.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/clutter-install.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/clutter-version-paths.props` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/clutter-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/clutter.sln` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj.filtersin` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxprojin` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/clutter.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/Makefile.am` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/Makefile.am`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/Makefile.in` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/Makefile.in`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/README.txt` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/README.txt`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-cogl-perf.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-cogl-perf.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-cogl-perf.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-cogl-perf.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxprojin` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-interactive-clutter.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-picking-performance.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-picking-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-picking-performance.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-picking-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-picking.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-picking.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-picking.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-picking.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-random-text.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-random-text.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-random-text.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-random-text.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-hidden-performance.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-hidden-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-hidden-performance.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-hidden-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-interactive-performance.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-interactive-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-interactive-performance.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-interactive-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-mini-performance.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-mini-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-mini-performance.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-mini-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-performance.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-performance.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-pick-performance.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-pick-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-state-pick-performance.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-state-pick-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf-performance.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf-performance.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-text-perf.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-text.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-text.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs12/test-text.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs12/test-text.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atkcomponent-example.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkcomponent-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atkcomponent-example.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkcomponent-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atkeditabletext-example.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkeditabletext-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atkeditabletext-example.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkeditabletext-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atkevents-example.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkevents-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atkevents-example.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atkevents-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atktext-example.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atktext-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/cally-atktext-example.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/cally-atktext-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/cally-clone-example.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/cally-clone-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/cally-clone-example.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/cally-clone-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/clutter-build-defines.props` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-build-defines.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/clutter-gen-srcs.props` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-gen-srcs.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/clutter-install.props` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-install.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/clutter-install.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/clutter-version-paths.props` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/clutter-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/clutter.sln` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj.filtersin` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxprojin` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/clutter.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/Makefile.am` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/Makefile.am`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/Makefile.in` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/Makefile.in`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/README.txt` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/README.txt`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-cogl-perf.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-cogl-perf.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-cogl-perf.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-cogl-perf.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-picking-performance.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-picking-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-picking-performance.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-picking-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-picking.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-picking.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-picking.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-picking.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-random-text.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-random-text.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-random-text.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-random-text.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-hidden-performance.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-hidden-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-hidden-performance.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-hidden-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-interactive-performance.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-interactive-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-interactive-performance.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-interactive-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-mini-performance.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-mini-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-mini-performance.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-mini-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-performance.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-performance.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-pick-performance.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-pick-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-state-pick-performance.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-state-pick-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf-performance.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf-performance.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-text-perf.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-text.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-text.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs14/test-text.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs14/test-text.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atkcomponent-example.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkcomponent-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atkcomponent-example.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkcomponent-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atkeditabletext-example.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkeditabletext-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atkeditabletext-example.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkeditabletext-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atkevents-example.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkevents-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atkevents-example.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atkevents-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atktext-example.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atktext-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/cally-atktext-example.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/cally-atktext-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/cally-clone-example.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/cally-clone-example.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/cally-clone-example.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/cally-clone-example.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/clutter-build-defines.props` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-build-defines.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/clutter-gen-srcs.props` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-gen-srcs.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/clutter-install.props` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-install.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/clutter-install.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/clutter-version-paths.props` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/clutter-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/clutter.sln` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj.filtersin` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxprojin` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/clutter.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/Makefile.am` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/Makefile.am`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/Makefile.in` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/Makefile.in`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/README.txt` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/README.txt`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-cogl-perf.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-cogl-perf.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-cogl-perf.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-cogl-perf.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-picking-performance.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-picking-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-picking-performance.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-picking-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-picking.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-picking.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-picking.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-picking.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-random-text.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-random-text.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-random-text.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-random-text.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-hidden-performance.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-hidden-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-hidden-performance.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-hidden-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-interactive-performance.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-interactive-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-interactive-performance.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-interactive-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-mini-performance.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-mini-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-mini-performance.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-mini-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-performance.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-performance.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-pick-performance.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-pick-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-state-pick-performance.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-state-pick-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf-performance.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf-performance.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf-performance.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf-performance.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-text-perf.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-text.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-text.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/clutter/build/win32/vs15/test-text.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/clutter/build/win32/vs15/test-text.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-build-defines.props` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-build-defines.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-crate.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-crate.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-crate.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-crate.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-gen-srcs.props` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-gen-srcs.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-hello.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-hello.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-hello.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-hello.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-info.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-info.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-info.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-info.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-install.props` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-install.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-install.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-msaa.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-msaa.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-msaa.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-msaa.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj.filtersin` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxprojin` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-pango.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj.filtersin` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxprojin` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-path.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-sdl2-hello.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-sdl2-hello.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-sdl2-hello.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-sdl2-hello.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl-version-paths.props` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl.sln` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj.filtersin` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxprojin` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/cogl.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/Makefile.am` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/Makefile.am`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/Makefile.in` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/Makefile.in`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/README.txt` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/README.txt`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj.filtersin` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxprojin` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs12/test-conformance-cogl.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-build-defines.props` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-build-defines.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-crate.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-crate.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-crate.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-crate.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-gen-srcs.props` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-gen-srcs.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-hello.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-hello.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-hello.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-hello.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-info.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-info.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-info.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-info.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-install.props` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-install.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-install.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-msaa.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-msaa.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-msaa.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-msaa.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj.filtersin` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxprojin` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-pango.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj.filtersin` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxprojin` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-path.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-sdl2-hello.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-sdl2-hello.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-sdl2-hello.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-sdl2-hello.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl-version-paths.props` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl.sln` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj.filtersin` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxprojin` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/cogl.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/Makefile.am` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/Makefile.am`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/Makefile.in` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/Makefile.in`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/README.txt` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/README.txt`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj.filtersin` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxprojin` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs14/test-conformance-cogl.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-build-defines.props` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-build-defines.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-crate.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-crate.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-crate.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-crate.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-gen-srcs.props` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-gen-srcs.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-hello.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-hello.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-hello.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-hello.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-info.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-info.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-info.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-info.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-install.props` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-install.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-install.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-msaa.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-msaa.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-msaa.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-msaa.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj.filtersin` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxprojin` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-pango.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj.filtersin` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxprojin` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-path.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-sdl2-hello.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-sdl2-hello.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-sdl2-hello.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-sdl2-hello.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl-version-paths.props` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl.sln` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj.filtersin` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxprojin` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/cogl.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/Makefile.am` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/Makefile.am`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/Makefile.in` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/Makefile.in`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/README.txt` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/README.txt`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj.filtersin` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxproj.filtersin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxprojin` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/build/win32/vs15/test-conformance-cogl.vcxprojin`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/GL/glcorearb.h` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/GL/glcorearb.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/GL/glext.h` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/GL/glext.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/GL/glxext.h` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/GL/glxext.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cogl/GL/wglext.h` & `gvsbuild-2024.5.0/gvsbuild/patches/cogl/GL/wglext.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cyrus-sasl/0001-Add-MIT-Kerberos-as-GSSAPI-provider.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/cyrus-sasl/0001-Add-MIT-Kerberos-as-GSSAPI-provider.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cyrus-sasl/0001-Fix-openssl-libs-to-point-to-the-new-openssl-1.1.1-n.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/cyrus-sasl/0001-Fix-openssl-libs-to-point-to-the-new-openssl-1.1.1-n.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cyrus-sasl/0001-fix-snprintf-macro.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/cyrus-sasl/0001-fix-snprintf-macro.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cyrus-sasl/0002-Provide-a-compile-option-for-32-64-gssapi.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/cyrus-sasl/0002-Provide-a-compile-option-for-32-64-gssapi.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/cyrus-sasl/include/md5global.h` & `gvsbuild-2024.5.0/gvsbuild/patches/cyrus-sasl/include/md5global.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/enchant/src/libenchant.rc` & `gvsbuild-2024.5.0/gvsbuild/patches/enchant/src/libenchant.rc`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/enchant/src/makefile.mak` & `gvsbuild-2024.5.0/gvsbuild/patches/enchant/src/makefile.mak`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/expat/0001-CMakeLists-do-not-add-postfix-d-in-debug-builds.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/expat/0001-CMakeLists-do-not-add-postfix-d-in-debug-builds.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/ffmpeg/build/build.sh` & `gvsbuild-2024.5.0/gvsbuild/patches/ffmpeg/build/build.sh`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/freetype/0001-meson-in-shared-libraries-we-need-to-export-the-meth.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/freetype/0001-meson-in-shared-libraries-we-need-to-export-the-meth.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/gettext-runtime-c99.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/gettext-runtime-c99.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/gettext-tools-c99.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/gettext-tools-c99.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/libtextstyle-c99.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/libtextstyle-c99.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/alloca.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/alloca.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/errno.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/errno.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/fcntl.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/fcntl.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/getopt-cdefs.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/getopt-cdefs.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/getopt.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/getopt.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/iconv.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/iconv.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/inttypes.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/inttypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/langinfo.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/langinfo.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/limits.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/limits.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/locale.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/locale.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/signal.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/signal.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/stddef.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/stddef.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/stdlib.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/stdlib.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/string.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/string.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/sys/stat.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/sys/stat.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/sys/types.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/sys/types.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/time.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/time.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unistd.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unistd.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unistr.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unistr.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unitypes.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/unitypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/uniwidth.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/uniwidth.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/wchar.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/wchar.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/wctype.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/gnulib-lib/wctype.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/intl/libgnuintl.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/intl/libgnuintl.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/intl/libintl.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/intl/libintl.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/alloca.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/alloca.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/autosprintf.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/autosprintf.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/errno.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-runtime/libasprintf/errno.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/alloca.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/alloca.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/byteswap.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/byteswap.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/ctype.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/ctype.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/dirent.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/dirent.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/errno.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/errno.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/fcntl.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/fcntl.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/fnmatch.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/fnmatch.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/getopt-cdefs.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/getopt-cdefs.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/getopt.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/getopt.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/iconv.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/iconv.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/inttypes.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/inttypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/langinfo.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/langinfo.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/c14n.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/c14n.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/catalog.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/catalog.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/chvalid.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/chvalid.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/debugXML.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/debugXML.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/dict.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/dict.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/DOCBparser.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/DOCBparser.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/encoding.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/encoding.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/entities.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/entities.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/globals.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/globals.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/hash.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/hash.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/HTMLparser.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/HTMLparser.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/HTMLtree.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/HTMLtree.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/list.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/list.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/nanoftp.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/nanoftp.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/nanohttp.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/nanohttp.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/parser.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/parser.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/parserInternals.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/parserInternals.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/pattern.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/pattern.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/relaxng.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/relaxng.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/SAX.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/SAX.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/SAX2.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/SAX2.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/schemasInternals.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/schemasInternals.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/schematron.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/schematron.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/threads.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/threads.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/tree.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/tree.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/uri.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/uri.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/valid.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/valid.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xinclude.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xinclude.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xlink.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xlink.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlautomata.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlautomata.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlerror.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlerror.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlexports.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlexports.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlIO.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlIO.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlmemory.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlmemory.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlmodule.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlmodule.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlreader.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlreader.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlregexp.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlregexp.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlsave.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlsave.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlschemas.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlschemas.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlschemastypes.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlschemastypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlstring.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlstring.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlunicode.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlunicode.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlversion.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlversion.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlwriter.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xmlwriter.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpath.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpath.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpathInternals.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpathInternals.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpointer.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/libxml/xpointer.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/limits.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/limits.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/locale.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/locale.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/omp.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/omp.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sched.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sched.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/signal.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/signal.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/spawn.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/spawn.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/stddef.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/stddef.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/stdlib.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/stdlib.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/string.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/string.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/random.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/random.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/select.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/select.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/stat.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/stat.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/time.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/time.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/types.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/types.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/wait.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/sys/wait.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/time.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/time.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniconv.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniconv.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unictype.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unictype.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unilbrk.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unilbrk.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniname.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniname.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unistd.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unistd.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unistr.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unistr.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unitypes.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/unitypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniwidth.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/uniwidth.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/utime.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/utime.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/wchar.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/wchar.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/wctype.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-lib/wctype.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/arpa/inet.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/arpa/inet.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/netinet/in.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/netinet/in.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/pthread.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/pthread.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/stdalign.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/stdalign.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/ioctl.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/ioctl.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/socket.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/socket.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/uio.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/gnulib-tests/sys/uio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/alloca.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/alloca.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/errno.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/errno.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/fcntl.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/fcntl.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/gettext-po.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/gettext-po.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/iconv.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/iconv.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/inttypes.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/inttypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/limits.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/limits.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/locale.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/locale.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/signal.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/signal.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/stddef.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/stddef.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/stdlib.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/stdlib.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/string.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/string.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/sys/stat.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/sys/stat.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/sys/types.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/sys/types.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/textstyle.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/textstyle.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/time.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/time.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/uniconv.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/uniconv.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unictype.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unictype.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unilbrk.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unilbrk.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unistd.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unistd.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unistr.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unistr.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unitypes.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/unitypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/uniwidth.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/uniwidth.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/wchar.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/wchar.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/wctype.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgettextpo/wctype.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/libgrep/langinfo.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/libgrep/langinfo.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/stdbool.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/stdbool.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/version.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/version.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/woe32dll.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle/woe32dll.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/gettext-tools/src/textstyle.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/alloca.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/alloca.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/errno.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/errno.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/fcntl.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/fcntl.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/ghash.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/ghash.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/glist.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/glist.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gmacros.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gmacros.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gprimes.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gprimes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gprintfint.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gprintfint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gstrfuncs.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gstrfuncs.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gstring.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gstring.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gtypes.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib/gtypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glib.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glibconfig.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/glibconfig.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/inttypes.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/inttypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/c14n.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/c14n.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/catalog.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/catalog.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/chvalid.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/chvalid.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/debugXML.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/debugXML.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/dict.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/dict.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/DOCBparser.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/DOCBparser.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/encoding.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/encoding.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/entities.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/entities.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/globals.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/globals.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/hash.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/hash.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/HTMLparser.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/HTMLparser.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/HTMLtree.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/HTMLtree.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/list.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/list.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/nanoftp.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/nanoftp.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/nanohttp.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/nanohttp.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/parser.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/parser.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/parserInternals.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/parserInternals.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/pattern.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/pattern.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/relaxng.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/relaxng.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/SAX.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/SAX.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/SAX2.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/SAX2.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/schemasInternals.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/schemasInternals.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/schematron.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/schematron.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/threads.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/threads.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/tree.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/tree.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/uri.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/uri.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/valid.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/valid.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xinclude.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xinclude.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xlink.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xlink.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlautomata.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlautomata.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlerror.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlerror.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlexports.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlexports.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlIO.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlIO.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlmemory.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlmemory.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlmodule.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlmodule.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlreader.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlreader.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlregexp.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlregexp.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlsave.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlsave.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlschemas.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlschemas.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlschemastypes.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlschemastypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlstring.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlstring.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlunicode.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlunicode.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlversion.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlversion.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlwriter.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xmlwriter.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpath.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpath.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpathInternals.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpathInternals.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpointer.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/libxml/xpointer.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/limits.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/limits.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/signal.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/signal.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdalign.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdalign.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stddef.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stddef.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdint.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdlib.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/stdlib.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/string.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/string.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/socket.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/socket.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/stat.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/stat.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/time.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/time.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/types.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/types.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/uio.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/sys/uio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/stdbool.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/stdbool.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/version.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/version.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/woe32dll.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/textstyle/woe32dll.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/time.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/time.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unistd.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unistd.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unistr.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unistr.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unitypes.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/unitypes.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/libtextstyle/lib/wchar.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/libtextstyle/lib/wchar.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/config.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/gnulib-lib/stdint.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/gnulib-lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/gnulib-lib/stdio.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-runtime/gnulib-lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/config.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/configmake.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/configmake.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/math.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/math.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/stdint.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/stdio.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/gnulib-lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/config.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/stdint.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/stdio.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/Win32/gettext-tools/libgettextpo/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/config.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/config.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/math.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/math.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/stdio.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/Win32/libtextstyle/lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/config.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/gnulib-lib/stdint.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/gnulib-lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/gnulib-lib/stdio.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-runtime/gnulib-lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/config.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/configmake.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/configmake.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/math.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/math.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/stdint.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/stdio.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/gnulib-lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/config.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/stdint.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/stdio.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/x64/gettext-tools/libgettextpo/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/config.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/config.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/math.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/math.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/stdio.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs12/x64/libtextstyle/lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/config.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/gnulib-lib/stdint.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/gnulib-lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/gnulib-lib/stdio.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-runtime/gnulib-lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/config.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/configmake.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/configmake.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/math.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/math.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/stdint.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/stdio.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/gnulib-lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/config.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/stdint.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/stdio.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/arm64/gettext-tools/libgettextpo/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/config.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/config.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/math.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/math.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/stdio.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/arm64/libtextstyle/lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/config.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/gnulib-lib/stdint.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/gnulib-lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/gnulib-lib/stdio.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-runtime/gnulib-lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/config.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/configmake.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/configmake.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/math.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/math.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/stdint.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/stdio.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/gnulib-lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/config.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/stdint.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/stdio.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/Win32/gettext-tools/libgettextpo/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/config.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/config.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/math.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/math.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/stdio.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/Win32/libtextstyle/lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/config.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/gnulib-lib/stdint.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/gnulib-lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/gnulib-lib/stdio.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-runtime/gnulib-lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/config.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/configmake.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/configmake.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/math.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/math.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/stdint.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/stdio.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/gnulib-lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/config.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/stdint.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/stdint.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/stdio.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/x64/gettext-tools/libgettextpo/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/config.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/config.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/math.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/math.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/stdio.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/msvc/vs14/x64/libtextstyle/lib/stdio.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/build-rules-msvc.mak` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/nmake/build-rules-msvc.mak`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/config-msvc.mak` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/nmake/config-msvc.mak`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/create-lists-msvc.mak` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/nmake/create-lists-msvc.mak`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/create-lists.bat` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/nmake/create-lists.bat`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/detectenv-msvc.mak` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/nmake/detectenv-msvc.mak`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/generate-msvc.mak` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/nmake/generate-msvc.mak`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/gettext-runtime-sources.mk` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/nmake/gettext-runtime-sources.mk`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/gettext-tools-sources.mk` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/nmake/gettext-tools-sources.mk`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/libgettextlib.def` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/nmake/libgettextlib.def`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/libgettextsrc.def` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/nmake/libgettextsrc.def`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/libtextstyle-sources.mk` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/nmake/libtextstyle-sources.mk`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/libtextstyle.def` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/nmake/libtextstyle.def`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gettext/nmake/Makefile.vc` & `gvsbuild-2024.5.0/gvsbuild/patches/gettext/nmake/Makefile.vc`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/glib/001-glib-package-installation-directory.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/glib/001-glib-package-installation-directory.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/glib/002-gir-scanner-dll-not-found.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/glib/002-gir-scanner-dll-not-found.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/glib-base/001-glib-package-installation-directory.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/glib-base/001-glib-package-installation-directory.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/glib-base/002-gir-scanner-dll-not-found.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/glib-base/002-gir-scanner-dll-not-found.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/glib-py-wrapper/glib-py-wrapper.c` & `gvsbuild-2024.5.0/gvsbuild/patches/glib-py-wrapper/glib-py-wrapper.c`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gobject-introspection/001-incorrect-giscanner-path.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/gobject-introspection/001-incorrect-giscanner-path.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gsettings-desktop-schemas/0001-build-win32-replace.py-Fix-replacing-items-in-files-.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/gsettings-desktop-schemas/0001-build-win32-replace.py-Fix-replacing-items-in-files-.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gsettings-desktop-schemas/0002-glib-mkenums-python.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/gsettings-desktop-schemas/0002-glib-mkenums-python.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gst-plugins-bad/wasapisink-reduce-buffer-latency.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/gst-plugins-bad/wasapisink-reduce-buffer-latency.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/0001-GDK-W32-Remove-WS_EX_LAYERED-from-an-opaque-window.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/gtk2/0001-GDK-W32-Remove-WS_EX_LAYERED-from-an-opaque-window.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/61162225f712df648f38fd12bc0817cfa9f79a64.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/gtk2/61162225f712df648f38fd12bc0817cfa9f79a64.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/bfdac2f70e005b2504cc3f4ebbdab328974d005a.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/gtk2/bfdac2f70e005b2504cc3f4ebbdab328974d005a.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/introspection.body.mak` & `gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/introspection.body.mak`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs12/gtk-version-paths.props` & `gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs12/gtk-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs14/gtk-version-paths.props` & `gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs14/gtk-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gailutil.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs15/gailutil.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gailutil.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs15/gailutil.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gdk-win32.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs15/gdk-win32.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gdk-win32.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs15/gdk-win32.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gdk.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs15/gdk.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gdk.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs15/gdk.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk+.sln` & `gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk+.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-build-defines.props` & `gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-build-defines.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-demo.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-demo.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-demo.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-demo.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-gen-srcs.props` & `gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-gen-srcs.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-install.props` & `gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-install.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-install.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-update-icon-cache.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-update-icon-cache.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-update-icon-cache.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-update-icon-cache.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk-version-paths.props` & `gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk-version-paths.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/gtk.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs15/gtk.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/libwimp.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs15/libwimp.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/libwimp.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs15/libwimp.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/build/win32/vs15/README.txt` & `gvsbuild-2024.5.0/gvsbuild/patches/gtk2/build/win32/vs15/README.txt`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/gtk-accel.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/gtk2/gtk-accel.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/gtk-bgimg.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/gtk2/gtk-bgimg.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/gtk-multimonitor.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/gtk2/gtk-multimonitor.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/gtk-revert-scrolldc-commit.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/gtk2/gtk-revert-scrolldc-commit.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gtk2/mod.md` & `gvsbuild-2024.5.0/gvsbuild/patches/gtk2/mod.md`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gtk3/gdk/win32/gdkkeys-win32.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gtk3/gdk/win32/gdkkeys-win32.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gtk3/gdk/win32/winpointer.h` & `gvsbuild-2024.5.0/gvsbuild/patches/gtk3/gdk/win32/winpointer.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gtk3/gtk_update_icon_cache.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/gtk3/gtk_update_icon_cache.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/gtksourceview5/001-fix-fontconfig-availability-check.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/gtksourceview5/001-fix-fontconfig-availability-check.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/libadwaita/0001-remove-appstream-dependency.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/libadwaita/0001-remove-appstream-dependency.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/libffi/fficonfig.h.meson` & `gvsbuild-2024.5.0/gvsbuild/patches/libffi/fficonfig.h.meson`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/libffi/meson.build` & `gvsbuild-2024.5.0/gvsbuild/patches/libffi/meson.build`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/libffi/meson_options.txt` & `gvsbuild-2024.5.0/gvsbuild/patches/libffi/meson_options.txt`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/libffi/src/meson.build` & `gvsbuild-2024.5.0/gvsbuild/patches/libffi/src/meson.build`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/libfido2/0001-Install-pkgconfig-files-also-on-msvc.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/libfido2/0001-Install-pkgconfig-files-also-on-msvc.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/libfido2/0001-libfido2-update-cmake-script-to-have-sdl-flag-before.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/libfido2/0001-libfido2-update-cmake-script-to-have-sdl-flag-before.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/libmicrohttpd/001-remove-postsample-perf-retries.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/libmicrohttpd/001-remove-postsample-perf-retries.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs12/rsvg-version-paths.props` & `gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs12/property.props`

 * *Files 19% similar despite different names*

#### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs12/rsvg-version-paths.props` & `gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs12/property.props`

```diff
@@ -1,56 +1,80 @@
 <?xml version="1.0" encoding="utf-8"?>
-<Project xmlns="http://schemas.microsoft.com/developer/msbuild/2003" DefaultTargets="Build" ToolsVersion="12.0">
-  <ImportGroup Label="PropertySheets"/>
+<Project xmlns="http://schemas.microsoft.com/developer/msbuild/2003" DefaultTargets="Build" ToolsVersion="4.0">
   <PropertyGroup Label="UserMacros">
-    <ApiVersion>2.0</ApiVersion>
+    <ApiVersion>1.0</ApiVersion>
     <VSVer>12</VSVer>
-    <GlibEtcInstallRoot>$(SolutionDir)\..\..\..\..\..\..\..\gtk\$(Platform)\$(Configuration)</GlibEtcInstallRoot>
-    <CopyDir>..\..\..\..\librsvg-rel</CopyDir>
-    <DefDir>$(SolutionDir)$(Configuration)\$(Platform)\obj\$(ProjectName)</DefDir>
-    <RsvgLibtoolCompatibleDllPrefix>lib</RsvgLibtoolCompatibleDllPrefix>
-    <RsvgLibtoolCompatibleDllSuffix>-$(ApiVersion)-0</RsvgLibtoolCompatibleDllSuffix>
-    <RsvgSeparateVSDllPrefix/>
-    <RsvgSeparateVSDllSuffix>-$(ApiVersion)</RsvgSeparateVSDllSuffix>
-    <RsvgDllPrefix>$(RsvgSeparateVSDllPrefix)</RsvgDllPrefix>
-    <RsvgDllSuffix>$(RsvgSeparateVSDllSuffix)</RsvgDllSuffix>
+    <PrjInstallRoot>$(SolutionDir)..\..\..\..\..\..\gtk\$(Platform)\$(Configuration)</PrjInstallRoot>
+    <PrjIncludeDir/>
+    <CopyDir>..\..\..\libssh-rel</CopyDir>
+    <BinDir>$(SolutionDir)$(Configuration)\$(PlatformName)\bin</BinDir>
+    <ObjDir>$(SolutionDir)$(Configuration)\$(PlatformName)\obj\$(ProjectName)</ObjDir>
+    <SolDir>..\..</SolDir>
+    <PrjLibtoolCompatibleDllPrefix>lib</PrjLibtoolCompatibleDllPrefix>
+    <PrjLibtoolCompatibleDllSuffix/>
+    <PrjSeparateDllPrefix/>
+    <PrjSeparateDllSuffix/>
+    <PrjDllPrefix>$(PrjSeparateDllPrefix)</PrjDllPrefix>
+    <PrjDllSuffix>$(PrjSeparateDllSuffix)</PrjDllSuffix>
+    <PreBuildCfg/>
+    <PrjDoInstall>mkdir $(CopyDir)
+
+      mkdir $(CopyDir)\bin
+
+      copy $(BinDir)\*.exe $(CopyDir)\bin
+
+      copy $(BinDir)\*.dll $(CopyDir)\bin
+
+      copy $(BinDir)\*.pdb $(CopyDir)\bin
+
+      mkdir $(CopyDir)\lib
+
+      copy $(BinDir)\*.lib $(CopyDir)\lib
+
+      mkdir $(CopyDir)\include\libssh-$(ApiVersion)\libssh
+
+      copy $(SolDir)\include\libssh\*.h $(CopyDir)\include\libssh-$(ApiVersion)\libssh</PrjDoInstall>
   </PropertyGroup>
   <PropertyGroup>
-    <_PropertySheetDisplayName>rsvgversionpathsprops</_PropertySheetDisplayName>
+    <_PropertySheetDisplayName>Prjprops</_PropertySheetDisplayName>
+    <OutDir>$(SolutionDir)$(Configuration)\$(PlatformName)\bin\</OutDir>
+    <IntDir>$(SolutionDir)$(Configuration)\$(PlatformName)\obj\$(ProjectName)\</IntDir>
   </PropertyGroup>
-  <ItemDefinitionGroup/>
   <ItemGroup>
-    <BuildMacro Include="ApiVersion">
-      <Value>$(ApiVersion)</Value>
+    <BuildMacro Include="PrjInstallRoot">
+      <Value>$(PrjInstallRoot)</Value>
     </BuildMacro>
-    <BuildMacro Include="VSVer">
-      <Value>$(VSVer)</Value>
-    </BuildMacro>
-    <BuildMacro Include="GlibEtcInstallRoot">
-      <Value>$(GlibEtcInstallRoot)</Value>
+    <BuildMacro Include="PrjIncludeDir">
+      <Value>$(PrjIncludeDir)</Value>
     </BuildMacro>
     <BuildMacro Include="CopyDir">
       <Value>$(CopyDir)</Value>
     </BuildMacro>
-    <BuildMacro Include="DefDir">
-      <Value>$(DefDir)</Value>
+    <BuildMacro Include="PreBuildCfg">
+      <Value>$(PreBuildCfg)</Value>
+    </BuildMacro>
+    <BuildMacro Include="ApiVersion">
+      <Value>$(ApiVersion)</Value>
+    </BuildMacro>
+    <BuildMacro Include="PrjDoInstall">
+      <Value>$(PrjDoInstall)</Value>
     </BuildMacro>
-    <BuildMacro Include="RsvgLibtoolCompatibleDllPrefix">
-      <Value>$(RsvgLibtoolCompatibleDllPrefix)</Value>
+    <BuildMacro Include="PrjLibtoolCompatibleDllPrefix">
+      <Value>$(PrjLibtoolCompatibleDllPrefix)</Value>
     </BuildMacro>
-    <BuildMacro Include="RsvgLibtoolCompatibleDllSuffix">
-      <Value>$(RsvgLibtoolCompatibleDllSuffix)</Value>
+    <BuildMacro Include="PrjLibtoolCompatibleDllSuffix">
+      <Value>$(PrjLibtoolCompatibleDllSuffix)</Value>
     </BuildMacro>
-    <BuildMacro Include="RsvgSeparateVSDllPrefix">
-      <Value>$(RsvgSeparateVSDllPrefix)</Value>
+    <BuildMacro Include="PrjSeparateDllPrefix">
+      <Value>$(PrjSeparateDllPrefix)</Value>
     </BuildMacro>
-    <BuildMacro Include="RsvgSeparateVSDllSuffix">
-      <Value>$(RsvgSeparateVSDllSuffix)</Value>
+    <BuildMacro Include="PrjSeparateDllSuffix">
+      <Value>$(PrjSeparateDllSuffix)</Value>
     </BuildMacro>
-    <BuildMacro Include="RsvgDllPrefix">
-      <Value>$(RsvgDllPrefix)</Value>
+    <BuildMacro Include="PrjDllPrefix">
+      <Value>$(PrjDllPrefix)</Value>
     </BuildMacro>
-    <BuildMacro Include="RsvgDllSuffix">
-      <Value>$(RsvgDllSuffix)</Value>
+    <BuildMacro Include="PrjDllSuffix">
+      <Value>$(PrjDllSuffix)</Value>
     </BuildMacro>
   </ItemGroup>
 </Project>
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs14/rsvg-version-paths.props` & `gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs14/property.props`

 * *Files 17% similar despite different names*

#### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs14/rsvg-version-paths.props` & `gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs14/property.props`

```diff
@@ -1,56 +1,80 @@
 <?xml version="1.0" encoding="utf-8"?>
-<Project xmlns="http://schemas.microsoft.com/developer/msbuild/2003" DefaultTargets="Build" ToolsVersion="12.0">
-  <ImportGroup Label="PropertySheets"/>
+<Project xmlns="http://schemas.microsoft.com/developer/msbuild/2003" DefaultTargets="Build" ToolsVersion="4.0">
   <PropertyGroup Label="UserMacros">
-    <ApiVersion>2.0</ApiVersion>
+    <ApiVersion>1.0</ApiVersion>
     <VSVer>14</VSVer>
-    <GlibEtcInstallRoot>$(SolutionDir)\..\..\..\..\..\..\..\gtk\$(Platform)\$(Configuration)</GlibEtcInstallRoot>
-    <CopyDir>..\..\..\..\librsvg-rel</CopyDir>
-    <DefDir>$(SolutionDir)$(Configuration)\$(Platform)\obj\$(ProjectName)</DefDir>
-    <RsvgLibtoolCompatibleDllPrefix>lib</RsvgLibtoolCompatibleDllPrefix>
-    <RsvgLibtoolCompatibleDllSuffix>-$(ApiVersion)-0</RsvgLibtoolCompatibleDllSuffix>
-    <RsvgSeparateVSDllPrefix/>
-    <RsvgSeparateVSDllSuffix>-$(ApiVersion)</RsvgSeparateVSDllSuffix>
-    <RsvgDllPrefix>$(RsvgSeparateVSDllPrefix)</RsvgDllPrefix>
-    <RsvgDllSuffix>$(RsvgSeparateVSDllSuffix)</RsvgDllSuffix>
+    <PrjInstallRoot>$(SolutionDir)..\..\..\..\..\..\gtk\$(Platform)\$(Configuration)</PrjInstallRoot>
+    <PrjIncludeDir/>
+    <CopyDir>..\..\..\libssh-rel</CopyDir>
+    <BinDir>$(SolutionDir)$(Configuration)\$(PlatformName)\bin</BinDir>
+    <ObjDir>$(SolutionDir)$(Configuration)\$(PlatformName)\obj\$(ProjectName)</ObjDir>
+    <SolDir>..\..</SolDir>
+    <PrjLibtoolCompatibleDllPrefix>lib</PrjLibtoolCompatibleDllPrefix>
+    <PrjLibtoolCompatibleDllSuffix/>
+    <PrjSeparateDllPrefix/>
+    <PrjSeparateDllSuffix/>
+    <PrjDllPrefix>$(PrjSeparateDllPrefix)</PrjDllPrefix>
+    <PrjDllSuffix>$(PrjSeparateDllSuffix)</PrjDllSuffix>
+    <PreBuildCfg/>
+    <PrjDoInstall>mkdir $(CopyDir)
+
+      mkdir $(CopyDir)\bin
+
+      copy $(BinDir)\*.exe $(CopyDir)\bin
+
+      copy $(BinDir)\*.dll $(CopyDir)\bin
+
+      copy $(BinDir)\*.pdb $(CopyDir)\bin
+
+      mkdir $(CopyDir)\lib
+
+      copy $(BinDir)\*.lib $(CopyDir)\lib
+
+      mkdir $(CopyDir)\include\libssh-$(ApiVersion)\libssh
+
+      copy $(SolDir)\include\libssh\*.h $(CopyDir)\include\libssh-$(ApiVersion)\libssh</PrjDoInstall>
   </PropertyGroup>
   <PropertyGroup>
-    <_PropertySheetDisplayName>rsvgversionpathsprops</_PropertySheetDisplayName>
+    <_PropertySheetDisplayName>Prjprops</_PropertySheetDisplayName>
+    <OutDir>$(SolutionDir)$(Configuration)\$(PlatformName)\bin\</OutDir>
+    <IntDir>$(SolutionDir)$(Configuration)\$(PlatformName)\obj\$(ProjectName)\</IntDir>
   </PropertyGroup>
-  <ItemDefinitionGroup/>
   <ItemGroup>
-    <BuildMacro Include="ApiVersion">
-      <Value>$(ApiVersion)</Value>
+    <BuildMacro Include="PrjInstallRoot">
+      <Value>$(PrjInstallRoot)</Value>
     </BuildMacro>
-    <BuildMacro Include="VSVer">
-      <Value>$(VSVer)</Value>
-    </BuildMacro>
-    <BuildMacro Include="GlibEtcInstallRoot">
-      <Value>$(GlibEtcInstallRoot)</Value>
+    <BuildMacro Include="PrjIncludeDir">
+      <Value>$(PrjIncludeDir)</Value>
     </BuildMacro>
     <BuildMacro Include="CopyDir">
       <Value>$(CopyDir)</Value>
     </BuildMacro>
-    <BuildMacro Include="DefDir">
-      <Value>$(DefDir)</Value>
+    <BuildMacro Include="PreBuildCfg">
+      <Value>$(PreBuildCfg)</Value>
+    </BuildMacro>
+    <BuildMacro Include="ApiVersion">
+      <Value>$(ApiVersion)</Value>
+    </BuildMacro>
+    <BuildMacro Include="PrjDoInstall">
+      <Value>$(PrjDoInstall)</Value>
     </BuildMacro>
-    <BuildMacro Include="RsvgLibtoolCompatibleDllPrefix">
-      <Value>$(RsvgLibtoolCompatibleDllPrefix)</Value>
+    <BuildMacro Include="PrjLibtoolCompatibleDllPrefix">
+      <Value>$(PrjLibtoolCompatibleDllPrefix)</Value>
     </BuildMacro>
-    <BuildMacro Include="RsvgLibtoolCompatibleDllSuffix">
-      <Value>$(RsvgLibtoolCompatibleDllSuffix)</Value>
+    <BuildMacro Include="PrjLibtoolCompatibleDllSuffix">
+      <Value>$(PrjLibtoolCompatibleDllSuffix)</Value>
     </BuildMacro>
-    <BuildMacro Include="RsvgSeparateVSDllPrefix">
-      <Value>$(RsvgSeparateVSDllPrefix)</Value>
+    <BuildMacro Include="PrjSeparateDllPrefix">
+      <Value>$(PrjSeparateDllPrefix)</Value>
     </BuildMacro>
-    <BuildMacro Include="RsvgSeparateVSDllSuffix">
-      <Value>$(RsvgSeparateVSDllSuffix)</Value>
+    <BuildMacro Include="PrjSeparateDllSuffix">
+      <Value>$(PrjSeparateDllSuffix)</Value>
     </BuildMacro>
-    <BuildMacro Include="RsvgDllPrefix">
-      <Value>$(RsvgDllPrefix)</Value>
+    <BuildMacro Include="PrjDllPrefix">
+      <Value>$(PrjDllPrefix)</Value>
     </BuildMacro>
-    <BuildMacro Include="RsvgDllSuffix">
-      <Value>$(RsvgDllSuffix)</Value>
+    <BuildMacro Include="PrjDllSuffix">
+      <Value>$(PrjDllSuffix)</Value>
     </BuildMacro>
   </ItemGroup>
 </Project>
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/libpixbufloader-svg.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2017/fullbench-dll/fullbench-dll.vcxproj`

 * *Files 12% similar despite different names*

#### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/libpixbufloader-svg.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2017/fullbench-dll/fullbench-dll.vcxproj`

```diff
@@ -15,163 +15,160 @@
     </ProjectConfiguration>
     <ProjectConfiguration Include="Release|x64">
       <Configuration>Release</Configuration>
       <Platform>x64</Platform>
     </ProjectConfiguration>
   </ItemGroup>
   <PropertyGroup Label="Globals">
-    <ProjectGuid>{F0CCC693-1721-4DBD-9A64-591201A22740}</ProjectGuid>
-    <RootNamespace>libpixbufloadersvg</RootNamespace>
+    <ProjectGuid>{13992FD2-077E-4954-B065-A428198201A9}</ProjectGuid>
     <Keyword>Win32Proj</Keyword>
+    <RootNamespace>fullbench-dll</RootNamespace>
+    <OutDir>$(SolutionDir)bin\$(Platform)_$(Configuration)\</OutDir>
+    <IntDir>$(SolutionDir)bin\obj\$(RootNamespace)_$(Platform)_$(Configuration)\</IntDir>
   </PropertyGroup>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.Default.props"/>
-  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'" Label="Configuration">
-    <ConfigurationType>DynamicLibrary</ConfigurationType>
-    <PlatformToolset>v141</PlatformToolset>
-    <CharacterSet>MultiByte</CharacterSet>
-    <WholeProgramOptimization>true</WholeProgramOptimization>
-  </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'" Label="Configuration">
-    <ConfigurationType>DynamicLibrary</ConfigurationType>
+    <ConfigurationType>Application</ConfigurationType>
+    <UseDebugLibraries>true</UseDebugLibraries>
+    <CharacterSet>Unicode</CharacterSet>
     <PlatformToolset>v141</PlatformToolset>
-    <CharacterSet>MultiByte</CharacterSet>
   </PropertyGroup>
-  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'" Label="Configuration">
-    <ConfigurationType>DynamicLibrary</ConfigurationType>
+  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'" Label="Configuration">
+    <ConfigurationType>Application</ConfigurationType>
+    <UseDebugLibraries>true</UseDebugLibraries>
+    <CharacterSet>Unicode</CharacterSet>
     <PlatformToolset>v141</PlatformToolset>
-    <CharacterSet>MultiByte</CharacterSet>
+  </PropertyGroup>
+  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'" Label="Configuration">
+    <ConfigurationType>Application</ConfigurationType>
+    <UseDebugLibraries>false</UseDebugLibraries>
     <WholeProgramOptimization>true</WholeProgramOptimization>
+    <CharacterSet>Unicode</CharacterSet>
+    <PlatformToolset>v141</PlatformToolset>
   </PropertyGroup>
-  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'" Label="Configuration">
-    <ConfigurationType>DynamicLibrary</ConfigurationType>
+  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'" Label="Configuration">
+    <ConfigurationType>Application</ConfigurationType>
+    <UseDebugLibraries>false</UseDebugLibraries>
+    <WholeProgramOptimization>true</WholeProgramOptimization>
+    <CharacterSet>Unicode</CharacterSet>
     <PlatformToolset>v141</PlatformToolset>
-    <CharacterSet>MultiByte</CharacterSet>
   </PropertyGroup>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.props"/>
   <ImportGroup Label="ExtensionSettings"/>
-  <ImportGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'" Label="PropertySheets">
+  <ImportGroup Label="PropertySheets" Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">
     <Import Project="$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props" Condition="exists('$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props')" Label="LocalAppDataPlatform"/>
-    <Import Project="rsvg-build-defines.props"/>
   </ImportGroup>
-  <ImportGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'" Label="PropertySheets">
+  <ImportGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'" Label="PropertySheets">
     <Import Project="$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props" Condition="exists('$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props')" Label="LocalAppDataPlatform"/>
-    <Import Project="rsvg-build-defines.props"/>
   </ImportGroup>
-  <ImportGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'" Label="PropertySheets">
+  <ImportGroup Label="PropertySheets" Condition="'$(Configuration)|$(Platform)'=='Release|Win32'">
     <Import Project="$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props" Condition="exists('$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props')" Label="LocalAppDataPlatform"/>
-    <Import Project="rsvg-build-defines.props"/>
   </ImportGroup>
-  <ImportGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'" Label="PropertySheets">
+  <ImportGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'" Label="PropertySheets">
     <Import Project="$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props" Condition="exists('$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props')" Label="LocalAppDataPlatform"/>
-    <Import Project="rsvg-build-defines.props"/>
   </ImportGroup>
   <PropertyGroup Label="UserMacros"/>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">
     <LinkIncremental>true</LinkIncremental>
-  </PropertyGroup>
-  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'">
-    <LinkIncremental>false</LinkIncremental>
+    <IncludePath>$(IncludePath);$(UniversalCRT_IncludePath);$(SolutionDir)..\..\lib;$(SolutionDir)..\..\programs;$(VCInstallDir)include;$(VCInstallDir)atlmfc\include;$(WindowsSDK_IncludePath);</IncludePath>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'">
     <LinkIncremental>true</LinkIncremental>
+    <IncludePath>$(IncludePath);$(UniversalCRT_IncludePath);$(SolutionDir)..\..\lib;$(SolutionDir)..\..\programs;$(VCInstallDir)include;$(VCInstallDir)atlmfc\include;$(WindowsSDK_IncludePath);</IncludePath>
+    <RunCodeAnalysis>true</RunCodeAnalysis>
+  </PropertyGroup>
+  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'">
+    <LinkIncremental>false</LinkIncremental>
+    <IncludePath>$(IncludePath);$(UniversalCRT_IncludePath);$(SolutionDir)..\..\lib;$(SolutionDir)..\..\programs;$(VCInstallDir)include;$(VCInstallDir)atlmfc\include;$(WindowsSDK_IncludePath);</IncludePath>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'">
     <LinkIncremental>false</LinkIncremental>
+    <IncludePath>$(IncludePath);$(UniversalCRT_IncludePath);$(SolutionDir)..\..\lib;$(SolutionDir)..\..\programs;$(VCInstallDir)include;$(VCInstallDir)atlmfc\include;$(WindowsSDK_IncludePath);</IncludePath>
+    <RunCodeAnalysis>true</RunCodeAnalysis>
   </PropertyGroup>
   <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">
     <ClCompile>
-      <Optimization>Disabled</Optimization>
-      <AdditionalIncludeDirectories>%(AdditionalIncludeDirectories)</AdditionalIncludeDirectories>
-      <PreprocessorDefinitions>_DEBUG;$(RsvgPixbufLoaderCFlags);%(PreprocessorDefinitions)</PreprocessorDefinitions>
-      <MinimalRebuild>true</MinimalRebuild>
-      <BasicRuntimeChecks>EnableFastChecks</BasicRuntimeChecks>
-      <RuntimeLibrary>MultiThreadedDebugDLL</RuntimeLibrary>
       <PrecompiledHeader/>
-      <WarningLevel>Level3</WarningLevel>
-      <DebugInformationFormat>EditAndContinue</DebugInformationFormat>
+      <WarningLevel>Level4</WarningLevel>
+      <Optimization>Disabled</Optimization>
+      <PreprocessorDefinitions>WIN32;_DEBUG;_CONSOLE;LZ4_DLL_IMPORT=1;%(PreprocessorDefinitions)</PreprocessorDefinitions>
+      <TreatWarningAsError>true</TreatWarningAsError>
+      <EnablePREfast>false</EnablePREfast>
     </ClCompile>
     <Link>
-      <AdditionalDependencies>%(AdditionalDependencies)</AdditionalDependencies>
+      <SubSystem>Console</SubSystem>
       <GenerateDebugInformation>true</GenerateDebugInformation>
-      <SubSystem>Windows</SubSystem>
-      <TargetMachine>MachineX86</TargetMachine>
+      <AdditionalLibraryDirectories>$(SolutionDir)bin\$(Platform)_$(Configuration);%(AdditionalLibraryDirectories)</AdditionalLibraryDirectories>
+      <AdditionalDependencies>liblz4.lib;%(AdditionalDependencies)</AdditionalDependencies>
     </Link>
   </ItemDefinitionGroup>
-  <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'">
+  <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'">
     <ClCompile>
-      <Optimization>MaxSpeed</Optimization>
-      <IntrinsicFunctions>true</IntrinsicFunctions>
-      <AdditionalIncludeDirectories>%(AdditionalIncludeDirectories)</AdditionalIncludeDirectories>
-      <PreprocessorDefinitions>$(RsvgPixbufLoaderCFlags);%(PreprocessorDefinitions)</PreprocessorDefinitions>
-      <RuntimeLibrary>MultiThreadedDLL</RuntimeLibrary>
-      <FunctionLevelLinking>true</FunctionLevelLinking>
       <PrecompiledHeader/>
-      <WarningLevel>Level3</WarningLevel>
-      <DebugInformationFormat>ProgramDatabase</DebugInformationFormat>
+      <WarningLevel>Level4</WarningLevel>
+      <Optimization>Disabled</Optimization>
+      <PreprocessorDefinitions>WIN32;_DEBUG;_CONSOLE;LZ4_DLL_IMPORT=1;%(PreprocessorDefinitions)</PreprocessorDefinitions>
+      <TreatWarningAsError>true</TreatWarningAsError>
+      <EnablePREfast>true</EnablePREfast>
+      <AdditionalOptions>/analyze:stacksize295252 %(AdditionalOptions)</AdditionalOptions>
     </ClCompile>
     <Link>
-      <AdditionalDependencies>%(AdditionalDependencies)</AdditionalDependencies>
+      <SubSystem>Console</SubSystem>
       <GenerateDebugInformation>true</GenerateDebugInformation>
-      <SubSystem>Windows</SubSystem>
-      <OptimizeReferences>true</OptimizeReferences>
-      <EnableCOMDATFolding>true</EnableCOMDATFolding>
-      <TargetMachine>MachineX86</TargetMachine>
+      <AdditionalLibraryDirectories>$(SolutionDir)bin\$(Platform)_$(Configuration);%(AdditionalLibraryDirectories)</AdditionalLibraryDirectories>
+      <AdditionalDependencies>liblz4.lib;%(AdditionalDependencies)</AdditionalDependencies>
     </Link>
   </ItemDefinitionGroup>
-  <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'">
-    <Midl>
-      <TargetEnvironment>X64</TargetEnvironment>
-    </Midl>
+  <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'">
     <ClCompile>
-      <Optimization>Disabled</Optimization>
-      <AdditionalIncludeDirectories>%(AdditionalIncludeDirectories)</AdditionalIncludeDirectories>
-      <PreprocessorDefinitions>_DEBUG;$(RsvgPixbufLoaderCFlags);%(PreprocessorDefinitions)</PreprocessorDefinitions>
-      <MinimalRebuild>true</MinimalRebuild>
-      <BasicRuntimeChecks>EnableFastChecks</BasicRuntimeChecks>
-      <RuntimeLibrary>MultiThreadedDebugDLL</RuntimeLibrary>
+      <WarningLevel>Level4</WarningLevel>
       <PrecompiledHeader/>
-      <WarningLevel>Level3</WarningLevel>
-      <DebugInformationFormat>ProgramDatabase</DebugInformationFormat>
+      <Optimization>MaxSpeed</Optimization>
+      <FunctionLevelLinking>true</FunctionLevelLinking>
+      <IntrinsicFunctions>true</IntrinsicFunctions>
+      <PreprocessorDefinitions>WIN32;NDEBUG;_CONSOLE;LZ4_DLL_IMPORT=1;%(PreprocessorDefinitions)</PreprocessorDefinitions>
+      <TreatWarningAsError>false</TreatWarningAsError>
+      <EnablePREfast>false</EnablePREfast>
     </ClCompile>
     <Link>
-      <AdditionalDependencies>%(AdditionalDependencies)</AdditionalDependencies>
+      <SubSystem>Console</SubSystem>
       <GenerateDebugInformation>true</GenerateDebugInformation>
-      <SubSystem>Windows</SubSystem>
-      <TargetMachine>MachineX64</TargetMachine>
+      <EnableCOMDATFolding>true</EnableCOMDATFolding>
+      <OptimizeReferences>true</OptimizeReferences>
+      <AdditionalLibraryDirectories>$(SolutionDir)bin\$(Platform)_$(Configuration);%(AdditionalLibraryDirectories)</AdditionalLibraryDirectories>
+      <AdditionalDependencies>liblz4.lib;%(AdditionalDependencies)</AdditionalDependencies>
     </Link>
   </ItemDefinitionGroup>
   <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'">
-    <Midl>
-      <TargetEnvironment>X64</TargetEnvironment>
-    </Midl>
     <ClCompile>
+      <WarningLevel>Level4</WarningLevel>
+      <PrecompiledHeader/>
       <Optimization>MaxSpeed</Optimization>
-      <IntrinsicFunctions>true</IntrinsicFunctions>
-      <AdditionalIncludeDirectories>%(AdditionalIncludeDirectories)</AdditionalIncludeDirectories>
-      <PreprocessorDefinitions>$(RsvgPixbufLoaderCFlags);%(PreprocessorDefinitions)</PreprocessorDefinitions>
-      <RuntimeLibrary>MultiThreadedDLL</RuntimeLibrary>
       <FunctionLevelLinking>true</FunctionLevelLinking>
-      <PrecompiledHeader/>
-      <WarningLevel>Level3</WarningLevel>
-      <DebugInformationFormat>ProgramDatabase</DebugInformationFormat>
+      <IntrinsicFunctions>true</IntrinsicFunctions>
+      <PreprocessorDefinitions>WIN32;NDEBUG;_CONSOLE;LZ4_DLL_IMPORT=1;%(PreprocessorDefinitions)</PreprocessorDefinitions>
+      <TreatWarningAsError>false</TreatWarningAsError>
+      <EnablePREfast>true</EnablePREfast>
+      <AdditionalOptions>/analyze:stacksize295252 %(AdditionalOptions)</AdditionalOptions>
     </ClCompile>
     <Link>
-      <AdditionalDependencies>%(AdditionalDependencies)</AdditionalDependencies>
+      <SubSystem>Console</SubSystem>
       <GenerateDebugInformation>true</GenerateDebugInformation>
-      <SubSystem>Windows</SubSystem>
-      <OptimizeReferences>true</OptimizeReferences>
       <EnableCOMDATFolding>true</EnableCOMDATFolding>
-      <TargetMachine>MachineX64</TargetMachine>
+      <OptimizeReferences>true</OptimizeReferences>
+      <AdditionalLibraryDirectories>$(SolutionDir)bin\$(Platform)_$(Configuration);%(AdditionalLibraryDirectories)</AdditionalLibraryDirectories>
+      <AdditionalDependencies>liblz4.lib;%(AdditionalDependencies)</AdditionalDependencies>
     </Link>
   </ItemDefinitionGroup>
   <ItemGroup>
-    <ClCompile Include="..\..\..\gdk-pixbuf-loader\io-svg.c"/>
+    <ClCompile Include="..\..\..\lib\xxhash.c"/>
+    <ClCompile Include="..\..\..\tests\fullbench.c"/>
   </ItemGroup>
   <ItemGroup>
-    <ProjectReference Include="rsvg.vcxproj">
-      <Project>{3d7ef762-d969-4ac0-ab52-3cc86fa4620b}</Project>
-      <ReferenceOutputAssembly>false</ReferenceOutputAssembly>
-    </ProjectReference>
+    <ClInclude Include="..\..\..\lib\lz4.h"/>
+    <ClInclude Include="..\..\..\lib\lz4frame.h"/>
+    <ClInclude Include="..\..\..\lib\lz4hc.h"/>
+    <ClInclude Include="..\..\..\lib\xxhash.h"/>
   </ItemGroup>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.targets"/>
   <ImportGroup Label="ExtensionTargets"/>
 </Project>
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/libpixbufloader-svg.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs12/install.vcxproj.filters`

 * *Files 16% similar despite different names*

#### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/libpixbufloader-svg.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs12/install.vcxproj.filters`

```diff
@@ -1,22 +1,17 @@
 <?xml version="1.0" encoding="utf-8"?>
 <Project xmlns="http://schemas.microsoft.com/developer/msbuild/2003" ToolsVersion="4.0">
   <ItemGroup>
-    <Filter Include="Sources">
+    <Filter Include="Source Files">
       <UniqueIdentifier>{4FC737F1-C7A5-4376-A066-2A32D752A2FF}</UniqueIdentifier>
       <Extensions>cpp;c;cc;cxx;def;odl;idl;hpj;bat;asm;asmx</Extensions>
     </Filter>
-    <Filter Include="Headers">
+    <Filter Include="Header Files">
       <UniqueIdentifier>{93995380-89BD-4b04-88EB-625FBE52EBFB}</UniqueIdentifier>
-      <Extensions>h;hpp;hxx;hm;inl;inc;xsd</Extensions>
+      <Extensions>h;hh;hpp;hxx;hm;inl;inc;xsd</Extensions>
     </Filter>
     <Filter Include="Resource Files">
       <UniqueIdentifier>{67DA6AB6-F800-4c08-8B7A-83BB121AAD01}</UniqueIdentifier>
-      <Extensions>rc;ico;cur;bmp;dlg;rc2;rct;bin;rgs;gif;jpg;jpeg;jpe;resx;tiff;tif;png;wav</Extensions>
+      <Extensions>rc;ico;cur;bmp;dlg;rc2;rct;bin;rgs;gif;jpg;jpeg;jpe;resx;tiff;tif;png;wav;mfcribbon-ms</Extensions>
     </Filter>
   </ItemGroup>
-  <ItemGroup>
-    <ClCompile Include="..\..\..\gdk-pixbuf-loader\io-svg.c">
-      <Filter>Sources</Filter>
-    </ClCompile>
-  </ItemGroup>
 </Project>
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-convert.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs14/install.vcxproj`

 * *Files 11% similar despite different names*

#### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-convert.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs14/install.vcxproj`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<Project xmlns="http://schemas.microsoft.com/developer/msbuild/2003" DefaultTargets="Build" ToolsVersion="12.0">
+<Project xmlns="http://schemas.microsoft.com/developer/msbuild/2003" DefaultTargets="Build" ToolsVersion="14.0">
   <ItemGroup Label="ProjectConfigurations">
     <ProjectConfiguration Include="Debug|Win32">
       <Configuration>Debug</Configuration>
       <Platform>Win32</Platform>
     </ProjectConfiguration>
     <ProjectConfiguration Include="Debug|x64">
       <Configuration>Debug</Configuration>
@@ -15,158 +15,147 @@
     </ProjectConfiguration>
     <ProjectConfiguration Include="Release|x64">
       <Configuration>Release</Configuration>
       <Platform>x64</Platform>
     </ProjectConfiguration>
   </ItemGroup>
   <PropertyGroup Label="Globals">
-    <ProjectGuid>{039282C3-B73E-4D08-9B65-2034CF9EB4B7}</ProjectGuid>
-    <RootNamespace>rsvgconvert</RootNamespace>
+    <ProjectGuid>{F42026FA-B395-4D5D-9F86-A98636F69607}</ProjectGuid>
     <Keyword>Win32Proj</Keyword>
+    <RootNamespace>install</RootNamespace>
   </PropertyGroup>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.Default.props"/>
-  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'" Label="Configuration">
+  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
-    <PlatformToolset>v141</PlatformToolset>
-    <CharacterSet>MultiByte</CharacterSet>
-    <WholeProgramOptimization>true</WholeProgramOptimization>
+    <UseDebugLibraries>true</UseDebugLibraries>
+    <PlatformToolset>v140</PlatformToolset>
+    <CharacterSet>Unicode</CharacterSet>
   </PropertyGroup>
-  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'" Label="Configuration">
+  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
-    <PlatformToolset>v141</PlatformToolset>
-    <CharacterSet>MultiByte</CharacterSet>
+    <UseDebugLibraries>true</UseDebugLibraries>
+    <PlatformToolset>v140</PlatformToolset>
+    <CharacterSet>Unicode</CharacterSet>
   </PropertyGroup>
-  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'" Label="Configuration">
+  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
-    <PlatformToolset>v141</PlatformToolset>
-    <CharacterSet>MultiByte</CharacterSet>
+    <UseDebugLibraries>false</UseDebugLibraries>
+    <PlatformToolset>v140</PlatformToolset>
     <WholeProgramOptimization>true</WholeProgramOptimization>
+    <CharacterSet>Unicode</CharacterSet>
   </PropertyGroup>
-  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'" Label="Configuration">
+  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
-    <PlatformToolset>v141</PlatformToolset>
-    <CharacterSet>MultiByte</CharacterSet>
+    <UseDebugLibraries>false</UseDebugLibraries>
+    <PlatformToolset>v140</PlatformToolset>
+    <WholeProgramOptimization>true</WholeProgramOptimization>
+    <CharacterSet>Unicode</CharacterSet>
   </PropertyGroup>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.props"/>
   <ImportGroup Label="ExtensionSettings"/>
-  <ImportGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'" Label="PropertySheets">
+  <ImportGroup Label="PropertySheets" Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">
     <Import Project="$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props" Condition="exists('$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props')" Label="LocalAppDataPlatform"/>
-    <Import Project="rsvg-build-defines.props"/>
   </ImportGroup>
-  <ImportGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'" Label="PropertySheets">
+  <ImportGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'" Label="PropertySheets">
     <Import Project="$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props" Condition="exists('$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props')" Label="LocalAppDataPlatform"/>
-    <Import Project="rsvg-build-defines.props"/>
   </ImportGroup>
-  <ImportGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'" Label="PropertySheets">
+  <ImportGroup Label="PropertySheets" Condition="'$(Configuration)|$(Platform)'=='Release|Win32'">
     <Import Project="$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props" Condition="exists('$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props')" Label="LocalAppDataPlatform"/>
-    <Import Project="rsvg-build-defines.props"/>
   </ImportGroup>
-  <ImportGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'" Label="PropertySheets">
+  <ImportGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'" Label="PropertySheets">
     <Import Project="$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props" Condition="exists('$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props')" Label="LocalAppDataPlatform"/>
-    <Import Project="rsvg-build-defines.props"/>
   </ImportGroup>
+  <Import Project="property.props"/>
+  <Import Project="..\..\..\stack.props"/>
   <PropertyGroup Label="UserMacros"/>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">
     <LinkIncremental>true</LinkIncremental>
-  </PropertyGroup>
-  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'">
-    <LinkIncremental>false</LinkIncremental>
+    <OutDir>$(PrjInstallRoot)\</OutDir>
+    <IntDir>$(SolutionDir)$(Configuration)\$(PlatformName)\obj\$(ProjectName)</IntDir>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'">
     <LinkIncremental>true</LinkIncremental>
+    <OutDir>$(PrjInstallRoot)\</OutDir>
+    <IntDir>$(SolutionDir)$(Configuration)\$(PlatformName)\obj\$(ProjectName)</IntDir>
+  </PropertyGroup>
+  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'">
+    <LinkIncremental>false</LinkIncremental>
+    <OutDir>$(PrjInstallRoot)\</OutDir>
+    <IntDir>$(SolutionDir)$(Configuration)\$(PlatformName)\obj\$(ProjectName)</IntDir>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'">
     <LinkIncremental>false</LinkIncremental>
+    <OutDir>$(PrjInstallRoot)\</OutDir>
+    <IntDir>$(SolutionDir)$(Configuration)\$(PlatformName)\obj\$(ProjectName)</IntDir>
   </PropertyGroup>
   <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">
     <ClCompile>
-      <Optimization>Disabled</Optimization>
-      <PreprocessorDefinitions>_DEBUG;%(PreprocessorDefinitions)</PreprocessorDefinitions>
-      <MinimalRebuild>true</MinimalRebuild>
-      <BasicRuntimeChecks>EnableFastChecks</BasicRuntimeChecks>
-      <RuntimeLibrary>MultiThreadedDebugDLL</RuntimeLibrary>
       <PrecompiledHeader/>
       <WarningLevel>Level3</WarningLevel>
-      <DebugInformationFormat>EditAndContinue</DebugInformationFormat>
+      <Optimization>Disabled</Optimization>
+      <PreprocessorDefinitions>WIN32;_DEBUG;_CONSOLE;_LIB;%(PreprocessorDefinitions)</PreprocessorDefinitions>
     </ClCompile>
     <Link>
-      <AdditionalDependencies>$(IntlLib);%(AdditionalDependencies)</AdditionalDependencies>
-      <GenerateDebugInformation>true</GenerateDebugInformation>
       <SubSystem>Console</SubSystem>
-      <TargetMachine>MachineX86</TargetMachine>
+      <GenerateDebugInformation>true</GenerateDebugInformation>
     </Link>
+    <PreBuildEvent>
+      <Command>$(PrjDoInstall)</Command>
+    </PreBuildEvent>
   </ItemDefinitionGroup>
-  <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'">
+  <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'">
     <ClCompile>
-      <Optimization>MaxSpeed</Optimization>
-      <IntrinsicFunctions>true</IntrinsicFunctions>
-      <RuntimeLibrary>MultiThreadedDLL</RuntimeLibrary>
-      <FunctionLevelLinking>true</FunctionLevelLinking>
       <PrecompiledHeader/>
       <WarningLevel>Level3</WarningLevel>
-      <DebugInformationFormat>ProgramDatabase</DebugInformationFormat>
+      <Optimization>Disabled</Optimization>
+      <PreprocessorDefinitions>WIN32;_DEBUG;_CONSOLE;_LIB;%(PreprocessorDefinitions)</PreprocessorDefinitions>
     </ClCompile>
     <Link>
-      <AdditionalDependencies>$(IntlLib);%(AdditionalDependencies)</AdditionalDependencies>
-      <GenerateDebugInformation>true</GenerateDebugInformation>
       <SubSystem>Console</SubSystem>
-      <OptimizeReferences>true</OptimizeReferences>
-      <EnableCOMDATFolding>true</EnableCOMDATFolding>
-      <TargetMachine>MachineX86</TargetMachine>
+      <GenerateDebugInformation>true</GenerateDebugInformation>
     </Link>
+    <PreBuildEvent>
+      <Command>$(PrjDoInstall)</Command>
+    </PreBuildEvent>
   </ItemDefinitionGroup>
-  <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'">
-    <Midl>
-      <TargetEnvironment>X64</TargetEnvironment>
-    </Midl>
+  <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'">
     <ClCompile>
-      <Optimization>Disabled</Optimization>
-      <PreprocessorDefinitions>_DEBUG;%(PreprocessorDefinitions)</PreprocessorDefinitions>
-      <MinimalRebuild>true</MinimalRebuild>
-      <BasicRuntimeChecks>EnableFastChecks</BasicRuntimeChecks>
-      <RuntimeLibrary>MultiThreadedDebugDLL</RuntimeLibrary>
-      <PrecompiledHeader/>
       <WarningLevel>Level3</WarningLevel>
-      <DebugInformationFormat>ProgramDatabase</DebugInformationFormat>
+      <PrecompiledHeader/>
+      <Optimization>MaxSpeed</Optimization>
+      <FunctionLevelLinking>true</FunctionLevelLinking>
+      <IntrinsicFunctions>true</IntrinsicFunctions>
+      <PreprocessorDefinitions>WIN32;NDEBUG;_CONSOLE;_LIB;%(PreprocessorDefinitions)</PreprocessorDefinitions>
     </ClCompile>
     <Link>
-      <AdditionalDependencies>$(IntlLib);%(AdditionalDependencies)</AdditionalDependencies>
-      <GenerateDebugInformation>true</GenerateDebugInformation>
       <SubSystem>Console</SubSystem>
-      <TargetMachine>MachineX64</TargetMachine>
+      <GenerateDebugInformation>true</GenerateDebugInformation>
+      <EnableCOMDATFolding>true</EnableCOMDATFolding>
+      <OptimizeReferences>true</OptimizeReferences>
     </Link>
+    <PreBuildEvent>
+      <Command>$(PrjDoInstall)</Command>
+    </PreBuildEvent>
   </ItemDefinitionGroup>
   <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'">
-    <Midl>
-      <TargetEnvironment>X64</TargetEnvironment>
-    </Midl>
     <ClCompile>
+      <WarningLevel>Level3</WarningLevel>
+      <PrecompiledHeader/>
       <Optimization>MaxSpeed</Optimization>
-      <IntrinsicFunctions>true</IntrinsicFunctions>
-      <RuntimeLibrary>MultiThreadedDLL</RuntimeLibrary>
       <FunctionLevelLinking>true</FunctionLevelLinking>
-      <PrecompiledHeader/>
-      <WarningLevel>Level3</WarningLevel>
-      <DebugInformationFormat>ProgramDatabase</DebugInformationFormat>
+      <IntrinsicFunctions>true</IntrinsicFunctions>
+      <PreprocessorDefinitions>WIN32;NDEBUG;_CONSOLE;_LIB;%(PreprocessorDefinitions)</PreprocessorDefinitions>
     </ClCompile>
     <Link>
-      <AdditionalDependencies>$(IntlLib);%(AdditionalDependencies)</AdditionalDependencies>
-      <GenerateDebugInformation>true</GenerateDebugInformation>
       <SubSystem>Console</SubSystem>
-      <OptimizeReferences>true</OptimizeReferences>
+      <GenerateDebugInformation>true</GenerateDebugInformation>
       <EnableCOMDATFolding>true</EnableCOMDATFolding>
-      <TargetMachine>MachineX64</TargetMachine>
+      <OptimizeReferences>true</OptimizeReferences>
     </Link>
+    <PreBuildEvent>
+      <Command>$(PrjDoInstall)</Command>
+    </PreBuildEvent>
   </ItemDefinitionGroup>
-  <ItemGroup>
-    <ClCompile Include="..\..\..\rsvg-convert.c"/>
-    <ClCompile Include="..\..\..\rsvg-size-callback.c"/>
-  </ItemGroup>
-  <ItemGroup>
-    <ProjectReference Include="rsvg.vcxproj">
-      <Project>{3d7ef762-d969-4ac0-ab52-3cc86fa4620b}</Project>
-      <ReferenceOutputAssembly>false</ReferenceOutputAssembly>
-    </ProjectReference>
-  </ItemGroup>
+  <ItemGroup/>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.targets"/>
   <ImportGroup Label="ExtensionTargets"/>
 </Project>
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-convert.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs14/install.vcxproj.filters`

 * *Files 13% similar despite different names*

#### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-convert.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs14/install.vcxproj.filters`

```diff
@@ -1,25 +1,17 @@
 <?xml version="1.0" encoding="utf-8"?>
 <Project xmlns="http://schemas.microsoft.com/developer/msbuild/2003" ToolsVersion="4.0">
   <ItemGroup>
-    <Filter Include="Sources">
+    <Filter Include="Source Files">
       <UniqueIdentifier>{4FC737F1-C7A5-4376-A066-2A32D752A2FF}</UniqueIdentifier>
       <Extensions>cpp;c;cc;cxx;def;odl;idl;hpj;bat;asm;asmx</Extensions>
     </Filter>
-    <Filter Include="Headers">
+    <Filter Include="Header Files">
       <UniqueIdentifier>{93995380-89BD-4b04-88EB-625FBE52EBFB}</UniqueIdentifier>
-      <Extensions>h;hpp;hxx;hm;inl;inc;xsd</Extensions>
+      <Extensions>h;hh;hpp;hxx;hm;inl;inc;xsd</Extensions>
     </Filter>
     <Filter Include="Resource Files">
       <UniqueIdentifier>{67DA6AB6-F800-4c08-8B7A-83BB121AAD01}</UniqueIdentifier>
-      <Extensions>rc;ico;cur;bmp;dlg;rc2;rct;bin;rgs;gif;jpg;jpeg;jpe;resx;tiff;tif;png;wav</Extensions>
+      <Extensions>rc;ico;cur;bmp;dlg;rc2;rct;bin;rgs;gif;jpg;jpeg;jpe;resx;tiff;tif;png;wav;mfcribbon-ms</Extensions>
     </Filter>
   </ItemGroup>
-  <ItemGroup>
-    <ClCompile Include="..\..\..\rsvg-convert.c">
-      <Filter>Source Files</Filter>
-    </ClCompile>
-    <ClCompile Include="..\..\..\rsvg-size-callback.c">
-      <Filter>Source Files</Filter>
-    </ClCompile>
-  </ItemGroup>
 </Project>
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-version-paths.props` & `gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs15/property.props`

 * *Files 20% similar despite different names*

#### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-version-paths.props` & `gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs15/property.props`

```diff
@@ -1,56 +1,80 @@
 <?xml version="1.0" encoding="utf-8"?>
-<Project xmlns="http://schemas.microsoft.com/developer/msbuild/2003" DefaultTargets="Build" ToolsVersion="12.0">
-  <ImportGroup Label="PropertySheets"/>
+<Project xmlns="http://schemas.microsoft.com/developer/msbuild/2003" DefaultTargets="Build" ToolsVersion="4.0">
   <PropertyGroup Label="UserMacros">
-    <ApiVersion>2.0</ApiVersion>
-    <VSVer>17</VSVer>
-    <GlibEtcInstallRoot>$(SolutionDir)\..\..\..\..\..\..\..\gtk\$(Platform)\$(Configuration)</GlibEtcInstallRoot>
-    <CopyDir>..\..\..\..\librsvg-rel</CopyDir>
-    <DefDir>$(SolutionDir)$(Configuration)\$(Platform)\obj\$(ProjectName)</DefDir>
-    <RsvgLibtoolCompatibleDllPrefix>lib</RsvgLibtoolCompatibleDllPrefix>
-    <RsvgLibtoolCompatibleDllSuffix>-$(ApiVersion)-0</RsvgLibtoolCompatibleDllSuffix>
-    <RsvgSeparateVSDllPrefix/>
-    <RsvgSeparateVSDllSuffix>-$(ApiVersion)</RsvgSeparateVSDllSuffix>
-    <RsvgDllPrefix>$(RsvgSeparateVSDllPrefix)</RsvgDllPrefix>
-    <RsvgDllSuffix>$(RsvgSeparateVSDllSuffix)</RsvgDllSuffix>
+    <ApiVersion>1.0</ApiVersion>
+    <VSVer>14</VSVer>
+    <PrjInstallRoot>$(SolutionDir)..\..\..\..\..\..\gtk\$(Platform)\$(Configuration)</PrjInstallRoot>
+    <PrjIncludeDir/>
+    <CopyDir>..\..\..\libssh-rel</CopyDir>
+    <BinDir>$(SolutionDir)$(Configuration)\$(PlatformName)\bin</BinDir>
+    <ObjDir>$(SolutionDir)$(Configuration)\$(PlatformName)\obj\$(ProjectName)</ObjDir>
+    <SolDir>..\..</SolDir>
+    <PrjLibtoolCompatibleDllPrefix>lib</PrjLibtoolCompatibleDllPrefix>
+    <PrjLibtoolCompatibleDllSuffix/>
+    <PrjSeparateDllPrefix/>
+    <PrjSeparateDllSuffix/>
+    <PrjDllPrefix>$(PrjSeparateDllPrefix)</PrjDllPrefix>
+    <PrjDllSuffix>$(PrjSeparateDllSuffix)</PrjDllSuffix>
+    <PreBuildCfg/>
+    <PrjDoInstall>mkdir $(CopyDir)
+
+      mkdir $(CopyDir)\bin
+
+      copy $(BinDir)\*.exe $(CopyDir)\bin
+
+      copy $(BinDir)\*.dll $(CopyDir)\bin
+
+      copy $(BinDir)\*.pdb $(CopyDir)\bin
+
+      mkdir $(CopyDir)\lib
+
+      copy $(BinDir)\*.lib $(CopyDir)\lib
+
+      mkdir $(CopyDir)\include\libssh-$(ApiVersion)\libssh
+
+      copy $(SolDir)\include\libssh\*.h $(CopyDir)\include\libssh-$(ApiVersion)\libssh</PrjDoInstall>
   </PropertyGroup>
   <PropertyGroup>
-    <_PropertySheetDisplayName>rsvgversionpathsprops</_PropertySheetDisplayName>
+    <_PropertySheetDisplayName>Prjprops</_PropertySheetDisplayName>
+    <OutDir>$(SolutionDir)$(Configuration)\$(PlatformName)\bin\</OutDir>
+    <IntDir>$(SolutionDir)$(Configuration)\$(PlatformName)\obj\$(ProjectName)\</IntDir>
   </PropertyGroup>
-  <ItemDefinitionGroup/>
   <ItemGroup>
-    <BuildMacro Include="ApiVersion">
-      <Value>$(ApiVersion)</Value>
+    <BuildMacro Include="PrjInstallRoot">
+      <Value>$(PrjInstallRoot)</Value>
     </BuildMacro>
-    <BuildMacro Include="VSVer">
-      <Value>$(VSVer)</Value>
-    </BuildMacro>
-    <BuildMacro Include="GlibEtcInstallRoot">
-      <Value>$(GlibEtcInstallRoot)</Value>
+    <BuildMacro Include="PrjIncludeDir">
+      <Value>$(PrjIncludeDir)</Value>
     </BuildMacro>
     <BuildMacro Include="CopyDir">
       <Value>$(CopyDir)</Value>
     </BuildMacro>
-    <BuildMacro Include="DefDir">
-      <Value>$(DefDir)</Value>
+    <BuildMacro Include="PreBuildCfg">
+      <Value>$(PreBuildCfg)</Value>
+    </BuildMacro>
+    <BuildMacro Include="ApiVersion">
+      <Value>$(ApiVersion)</Value>
+    </BuildMacro>
+    <BuildMacro Include="PrjDoInstall">
+      <Value>$(PrjDoInstall)</Value>
     </BuildMacro>
-    <BuildMacro Include="RsvgLibtoolCompatibleDllPrefix">
-      <Value>$(RsvgLibtoolCompatibleDllPrefix)</Value>
+    <BuildMacro Include="PrjLibtoolCompatibleDllPrefix">
+      <Value>$(PrjLibtoolCompatibleDllPrefix)</Value>
     </BuildMacro>
-    <BuildMacro Include="RsvgLibtoolCompatibleDllSuffix">
-      <Value>$(RsvgLibtoolCompatibleDllSuffix)</Value>
+    <BuildMacro Include="PrjLibtoolCompatibleDllSuffix">
+      <Value>$(PrjLibtoolCompatibleDllSuffix)</Value>
     </BuildMacro>
-    <BuildMacro Include="RsvgSeparateVSDllPrefix">
-      <Value>$(RsvgSeparateVSDllPrefix)</Value>
+    <BuildMacro Include="PrjSeparateDllPrefix">
+      <Value>$(PrjSeparateDllPrefix)</Value>
     </BuildMacro>
-    <BuildMacro Include="RsvgSeparateVSDllSuffix">
-      <Value>$(RsvgSeparateVSDllSuffix)</Value>
+    <BuildMacro Include="PrjSeparateDllSuffix">
+      <Value>$(PrjSeparateDllSuffix)</Value>
     </BuildMacro>
-    <BuildMacro Include="RsvgDllPrefix">
-      <Value>$(RsvgDllPrefix)</Value>
+    <BuildMacro Include="PrjDllPrefix">
+      <Value>$(PrjDllPrefix)</Value>
     </BuildMacro>
-    <BuildMacro Include="RsvgDllSuffix">
-      <Value>$(RsvgDllSuffix)</Value>
+    <BuildMacro Include="PrjDllSuffix">
+      <Value>$(PrjDllSuffix)</Value>
     </BuildMacro>
   </ItemGroup>
 </Project>
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-view-3.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2013/frametest/frametest.vcxproj`

 * *Files 15% similar despite different names*

#### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-view-3.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2013/frametest/frametest.vcxproj`

```diff
@@ -15,161 +15,156 @@
     </ProjectConfiguration>
     <ProjectConfiguration Include="Release|x64">
       <Configuration>Release</Configuration>
       <Platform>x64</Platform>
     </ProjectConfiguration>
   </ItemGroup>
   <PropertyGroup Label="Globals">
-    <ProjectGuid>{2C4FC5FD-1CF0-47F9-83FC-A129EE313C1E}</ProjectGuid>
-    <RootNamespace>rsvgview3</RootNamespace>
+    <ProjectGuid>{39AD6ECC-8BAD-4368-95E4-A1AA2F077BB7}</ProjectGuid>
     <Keyword>Win32Proj</Keyword>
+    <RootNamespace>frametest</RootNamespace>
+    <OutDir>$(SolutionDir)bin\$(Platform)_$(Configuration)\</OutDir>
+    <IntDir>$(SolutionDir)bin\obj\$(RootNamespace)_$(Platform)_$(Configuration)\</IntDir>
   </PropertyGroup>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.Default.props"/>
-  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'" Label="Configuration">
+  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
-    <PlatformToolset>v141</PlatformToolset>
-    <CharacterSet>MultiByte</CharacterSet>
-    <WholeProgramOptimization>true</WholeProgramOptimization>
+    <UseDebugLibraries>true</UseDebugLibraries>
+    <CharacterSet>Unicode</CharacterSet>
+    <PlatformToolset>v120</PlatformToolset>
   </PropertyGroup>
-  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'" Label="Configuration">
+  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
-    <PlatformToolset>v141</PlatformToolset>
-    <CharacterSet>MultiByte</CharacterSet>
+    <UseDebugLibraries>true</UseDebugLibraries>
+    <CharacterSet>Unicode</CharacterSet>
+    <PlatformToolset>v120</PlatformToolset>
   </PropertyGroup>
-  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'" Label="Configuration">
+  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
-    <PlatformToolset>v141</PlatformToolset>
-    <CharacterSet>MultiByte</CharacterSet>
+    <UseDebugLibraries>false</UseDebugLibraries>
     <WholeProgramOptimization>true</WholeProgramOptimization>
+    <CharacterSet>Unicode</CharacterSet>
+    <PlatformToolset>v120</PlatformToolset>
   </PropertyGroup>
-  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'" Label="Configuration">
+  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
-    <PlatformToolset>v141</PlatformToolset>
-    <CharacterSet>MultiByte</CharacterSet>
+    <UseDebugLibraries>false</UseDebugLibraries>
+    <WholeProgramOptimization>true</WholeProgramOptimization>
+    <CharacterSet>Unicode</CharacterSet>
+    <PlatformToolset>v120</PlatformToolset>
   </PropertyGroup>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.props"/>
   <ImportGroup Label="ExtensionSettings"/>
-  <ImportGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'" Label="PropertySheets">
+  <ImportGroup Label="PropertySheets" Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">
     <Import Project="$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props" Condition="exists('$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props')" Label="LocalAppDataPlatform"/>
-    <Import Project="rsvg-build-defines.props"/>
   </ImportGroup>
-  <ImportGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'" Label="PropertySheets">
+  <ImportGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'" Label="PropertySheets">
     <Import Project="$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props" Condition="exists('$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props')" Label="LocalAppDataPlatform"/>
-    <Import Project="rsvg-build-defines.props"/>
   </ImportGroup>
-  <ImportGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'" Label="PropertySheets">
+  <ImportGroup Label="PropertySheets" Condition="'$(Configuration)|$(Platform)'=='Release|Win32'">
     <Import Project="$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props" Condition="exists('$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props')" Label="LocalAppDataPlatform"/>
-    <Import Project="rsvg-build-defines.props"/>
   </ImportGroup>
-  <ImportGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'" Label="PropertySheets">
+  <ImportGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'" Label="PropertySheets">
     <Import Project="$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props" Condition="exists('$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props')" Label="LocalAppDataPlatform"/>
-    <Import Project="rsvg-build-defines.props"/>
   </ImportGroup>
   <PropertyGroup Label="UserMacros"/>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">
     <LinkIncremental>true</LinkIncremental>
-  </PropertyGroup>
-  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'">
-    <LinkIncremental>false</LinkIncremental>
+    <IncludePath>$(IncludePath);$(UniversalCRT_IncludePath);$(SolutionDir)..\..\lib;$(SolutionDir)..\..\programs;$(VCInstallDir)include;$(VCInstallDir)atlmfc\include;$(WindowsSDK_IncludePath);</IncludePath>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'">
     <LinkIncremental>true</LinkIncremental>
+    <IncludePath>$(IncludePath);$(UniversalCRT_IncludePath);$(SolutionDir)..\..\lib;$(SolutionDir)..\..\programs;$(VCInstallDir)include;$(VCInstallDir)atlmfc\include;$(WindowsSDK_IncludePath);</IncludePath>
+    <RunCodeAnalysis>true</RunCodeAnalysis>
+  </PropertyGroup>
+  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'">
+    <LinkIncremental>false</LinkIncremental>
+    <IncludePath>$(IncludePath);$(UniversalCRT_IncludePath);$(SolutionDir)..\..\lib;$(SolutionDir)..\..\programs;$(VCInstallDir)include;$(VCInstallDir)atlmfc\include;$(WindowsSDK_IncludePath);</IncludePath>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'">
     <LinkIncremental>false</LinkIncremental>
+    <IncludePath>$(IncludePath);$(UniversalCRT_IncludePath);$(SolutionDir)..\..\lib;$(SolutionDir)..\..\programs;$(VCInstallDir)include;$(VCInstallDir)atlmfc\include;$(WindowsSDK_IncludePath);</IncludePath>
+    <RunCodeAnalysis>true</RunCodeAnalysis>
   </PropertyGroup>
   <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">
     <ClCompile>
-      <Optimization>Disabled</Optimization>
-      <AdditionalIncludeDirectories>$(Gtk3IncPath);%(AdditionalIncludeDirectories)</AdditionalIncludeDirectories>
-      <PreprocessorDefinitions>_DEBUG;%(PreprocessorDefinitions)</PreprocessorDefinitions>
-      <MinimalRebuild>true</MinimalRebuild>
-      <BasicRuntimeChecks>EnableFastChecks</BasicRuntimeChecks>
-      <RuntimeLibrary>MultiThreadedDebugDLL</RuntimeLibrary>
       <PrecompiledHeader/>
-      <WarningLevel>Level3</WarningLevel>
-      <DebugInformationFormat>EditAndContinue</DebugInformationFormat>
+      <WarningLevel>Level4</WarningLevel>
+      <Optimization>Disabled</Optimization>
+      <PreprocessorDefinitions>WIN32;_DEBUG;_CONSOLE;%(PreprocessorDefinitions)</PreprocessorDefinitions>
+      <TreatWarningAsError>true</TreatWarningAsError>
+      <EnablePREfast>false</EnablePREfast>
     </ClCompile>
     <Link>
-      <AdditionalDependencies>$(Gtk3Libs);%(AdditionalDependencies)</AdditionalDependencies>
-      <GenerateDebugInformation>true</GenerateDebugInformation>
       <SubSystem>Console</SubSystem>
-      <TargetMachine>MachineX86</TargetMachine>
+      <GenerateDebugInformation>true</GenerateDebugInformation>
     </Link>
   </ItemDefinitionGroup>
-  <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'">
+  <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'">
     <ClCompile>
-      <Optimization>MaxSpeed</Optimization>
-      <IntrinsicFunctions>true</IntrinsicFunctions>
-      <AdditionalIncludeDirectories>$(Gtk3IncPath);%(AdditionalIncludeDirectories)</AdditionalIncludeDirectories>
-      <RuntimeLibrary>MultiThreadedDLL</RuntimeLibrary>
-      <FunctionLevelLinking>true</FunctionLevelLinking>
       <PrecompiledHeader/>
-      <WarningLevel>Level3</WarningLevel>
-      <DebugInformationFormat>ProgramDatabase</DebugInformationFormat>
+      <WarningLevel>Level4</WarningLevel>
+      <Optimization>Disabled</Optimization>
+      <PreprocessorDefinitions>WIN32;_DEBUG;_CONSOLE;%(PreprocessorDefinitions)</PreprocessorDefinitions>
+      <TreatWarningAsError>true</TreatWarningAsError>
+      <EnablePREfast>true</EnablePREfast>
+      <AdditionalOptions>/analyze:stacksize295252 %(AdditionalOptions)</AdditionalOptions>
     </ClCompile>
     <Link>
-      <AdditionalDependencies>$(Gtk3Libs);%(AdditionalDependencies)</AdditionalDependencies>
-      <GenerateDebugInformation>true</GenerateDebugInformation>
       <SubSystem>Console</SubSystem>
-      <OptimizeReferences>true</OptimizeReferences>
-      <EnableCOMDATFolding>true</EnableCOMDATFolding>
-      <TargetMachine>MachineX86</TargetMachine>
+      <GenerateDebugInformation>true</GenerateDebugInformation>
     </Link>
   </ItemDefinitionGroup>
-  <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'">
-    <Midl>
-      <TargetEnvironment>X64</TargetEnvironment>
-    </Midl>
+  <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'">
     <ClCompile>
-      <Optimization>Disabled</Optimization>
-      <AdditionalIncludeDirectories>$(Gtk3IncPath);%(AdditionalIncludeDirectories)</AdditionalIncludeDirectories>
-      <PreprocessorDefinitions>_DEBUG;%(PreprocessorDefinitions)</PreprocessorDefinitions>
-      <MinimalRebuild>true</MinimalRebuild>
-      <BasicRuntimeChecks>EnableFastChecks</BasicRuntimeChecks>
-      <RuntimeLibrary>MultiThreadedDebugDLL</RuntimeLibrary>
+      <WarningLevel>Level4</WarningLevel>
       <PrecompiledHeader/>
-      <WarningLevel>Level3</WarningLevel>
-      <DebugInformationFormat>ProgramDatabase</DebugInformationFormat>
+      <Optimization>MaxSpeed</Optimization>
+      <FunctionLevelLinking>true</FunctionLevelLinking>
+      <IntrinsicFunctions>true</IntrinsicFunctions>
+      <PreprocessorDefinitions>WIN32;NDEBUG;_CONSOLE;%(PreprocessorDefinitions)</PreprocessorDefinitions>
+      <TreatWarningAsError>false</TreatWarningAsError>
+      <EnablePREfast>false</EnablePREfast>
     </ClCompile>
     <Link>
-      <AdditionalDependencies>$(Gtk3Libs);%(AdditionalDependencies)</AdditionalDependencies>
-      <GenerateDebugInformation>true</GenerateDebugInformation>
       <SubSystem>Console</SubSystem>
-      <TargetMachine>MachineX64</TargetMachine>
+      <GenerateDebugInformation>true</GenerateDebugInformation>
+      <EnableCOMDATFolding>true</EnableCOMDATFolding>
+      <OptimizeReferences>true</OptimizeReferences>
     </Link>
   </ItemDefinitionGroup>
   <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'">
-    <Midl>
-      <TargetEnvironment>X64</TargetEnvironment>
-    </Midl>
     <ClCompile>
+      <WarningLevel>Level4</WarningLevel>
+      <PrecompiledHeader/>
       <Optimization>MaxSpeed</Optimization>
-      <IntrinsicFunctions>true</IntrinsicFunctions>
-      <AdditionalIncludeDirectories>$(Gtk3IncPath);%(AdditionalIncludeDirectories)</AdditionalIncludeDirectories>
-      <RuntimeLibrary>MultiThreadedDLL</RuntimeLibrary>
       <FunctionLevelLinking>true</FunctionLevelLinking>
-      <PrecompiledHeader/>
-      <WarningLevel>Level3</WarningLevel>
-      <DebugInformationFormat>ProgramDatabase</DebugInformationFormat>
+      <IntrinsicFunctions>true</IntrinsicFunctions>
+      <PreprocessorDefinitions>WIN32;NDEBUG;_CONSOLE;%(PreprocessorDefinitions)</PreprocessorDefinitions>
+      <TreatWarningAsError>false</TreatWarningAsError>
+      <EnablePREfast>true</EnablePREfast>
+      <AdditionalOptions>/analyze:stacksize295252 %(AdditionalOptions)</AdditionalOptions>
     </ClCompile>
     <Link>
-      <AdditionalDependencies>$(Gtk3Libs);%(AdditionalDependencies)</AdditionalDependencies>
-      <GenerateDebugInformation>true</GenerateDebugInformation>
       <SubSystem>Console</SubSystem>
-      <OptimizeReferences>true</OptimizeReferences>
+      <GenerateDebugInformation>true</GenerateDebugInformation>
       <EnableCOMDATFolding>true</EnableCOMDATFolding>
-      <TargetMachine>MachineX64</TargetMachine>
+      <OptimizeReferences>true</OptimizeReferences>
     </Link>
   </ItemDefinitionGroup>
   <ItemGroup>
-    <ClCompile Include="..\..\..\test-display.c"/>
+    <ClCompile Include="..\..\..\lib\lz4.c"/>
+    <ClCompile Include="..\..\..\lib\lz4frame.c"/>
+    <ClCompile Include="..\..\..\lib\lz4hc.c"/>
+    <ClCompile Include="..\..\..\lib\xxhash.c"/>
+    <ClCompile Include="..\..\..\tests\frametest.c"/>
   </ItemGroup>
   <ItemGroup>
-    <ProjectReference Include="rsvg.vcxproj">
-      <Project>{3d7ef762-d969-4ac0-ab52-3cc86fa4620b}</Project>
-      <ReferenceOutputAssembly>false</ReferenceOutputAssembly>
-    </ProjectReference>
+    <ClInclude Include="..\..\..\lib\lz4.h"/>
+    <ClInclude Include="..\..\..\lib\lz4frame.h"/>
+    <ClInclude Include="..\..\..\lib\lz4frame_static.h"/>
+    <ClInclude Include="..\..\..\lib\lz4hc.h"/>
+    <ClInclude Include="..\..\..\lib\xxhash.h"/>
   </ItemGroup>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.targets"/>
   <ImportGroup Label="ExtensionTargets"/>
 </Project>
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-view-3.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs15/install.vcxproj.filters`

 * *Files 15% similar despite different names*

#### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg-view-3.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs15/install.vcxproj.filters`

```diff
@@ -1,22 +1,17 @@
 <?xml version="1.0" encoding="utf-8"?>
 <Project xmlns="http://schemas.microsoft.com/developer/msbuild/2003" ToolsVersion="4.0">
   <ItemGroup>
-    <Filter Include="Sources">
+    <Filter Include="Source Files">
       <UniqueIdentifier>{4FC737F1-C7A5-4376-A066-2A32D752A2FF}</UniqueIdentifier>
       <Extensions>cpp;c;cc;cxx;def;odl;idl;hpj;bat;asm;asmx</Extensions>
     </Filter>
-    <Filter Include="Headers">
+    <Filter Include="Header Files">
       <UniqueIdentifier>{93995380-89BD-4b04-88EB-625FBE52EBFB}</UniqueIdentifier>
-      <Extensions>h;hpp;hxx;hm;inl;inc;xsd</Extensions>
+      <Extensions>h;hh;hpp;hxx;hm;inl;inc;xsd</Extensions>
     </Filter>
     <Filter Include="Resource Files">
       <UniqueIdentifier>{67DA6AB6-F800-4c08-8B7A-83BB121AAD01}</UniqueIdentifier>
-      <Extensions>rc;ico;cur;bmp;dlg;rc2;rct;bin;rgs;gif;jpg;jpeg;jpe;resx;tiff;tif;png;wav</Extensions>
+      <Extensions>rc;ico;cur;bmp;dlg;rc2;rct;bin;rgs;gif;jpg;jpeg;jpe;resx;tiff;tif;png;wav;mfcribbon-ms</Extensions>
     </Filter>
   </ItemGroup>
-  <ItemGroup>
-    <ClCompile Include="..\..\..\test-display.c">
-      <Filter>Sources</Filter>
-    </ClCompile>
-  </ItemGroup>
 </Project>
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2017/lz4/lz4.vcxproj`

 * *Files 25% similar despite different names*

#### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/librsvg-legacy/build/win32/vs15/rsvg.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2017/lz4/lz4.vcxproj`

```diff
@@ -15,228 +15,169 @@
     </ProjectConfiguration>
     <ProjectConfiguration Include="Release|x64">
       <Configuration>Release</Configuration>
       <Platform>x64</Platform>
     </ProjectConfiguration>
   </ItemGroup>
   <PropertyGroup Label="Globals">
-    <ProjectGuid>{3D7EF762-D969-4AC0-AB52-3CC86FA4620B}</ProjectGuid>
-    <RootNamespace>rsvg</RootNamespace>
+    <ProjectGuid>{E30329AC-0057-4FE0-8FDA-7F650D398C4C}</ProjectGuid>
     <Keyword>Win32Proj</Keyword>
+    <RootNamespace>lz4</RootNamespace>
+    <OutDir>$(SolutionDir)bin\$(Platform)_$(Configuration)\</OutDir>
+    <IntDir>$(SolutionDir)bin\obj\$(RootNamespace)_$(Platform)_$(Configuration)\</IntDir>
   </PropertyGroup>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.Default.props"/>
-  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'" Label="Configuration">
-    <ConfigurationType>DynamicLibrary</ConfigurationType>
-    <PlatformToolset>v141</PlatformToolset>
-    <CharacterSet>MultiByte</CharacterSet>
-    <WholeProgramOptimization>true</WholeProgramOptimization>
-  </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'" Label="Configuration">
-    <ConfigurationType>DynamicLibrary</ConfigurationType>
+    <ConfigurationType>Application</ConfigurationType>
+    <UseDebugLibraries>true</UseDebugLibraries>
+    <CharacterSet>Unicode</CharacterSet>
     <PlatformToolset>v141</PlatformToolset>
-    <CharacterSet>MultiByte</CharacterSet>
   </PropertyGroup>
-  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'" Label="Configuration">
-    <ConfigurationType>DynamicLibrary</ConfigurationType>
+  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'" Label="Configuration">
+    <ConfigurationType>Application</ConfigurationType>
+    <UseDebugLibraries>true</UseDebugLibraries>
+    <CharacterSet>Unicode</CharacterSet>
     <PlatformToolset>v141</PlatformToolset>
-    <CharacterSet>MultiByte</CharacterSet>
+  </PropertyGroup>
+  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'" Label="Configuration">
+    <ConfigurationType>Application</ConfigurationType>
+    <UseDebugLibraries>false</UseDebugLibraries>
     <WholeProgramOptimization>true</WholeProgramOptimization>
+    <CharacterSet>Unicode</CharacterSet>
+    <PlatformToolset>v141</PlatformToolset>
   </PropertyGroup>
-  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'" Label="Configuration">
-    <ConfigurationType>DynamicLibrary</ConfigurationType>
+  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'" Label="Configuration">
+    <ConfigurationType>Application</ConfigurationType>
+    <UseDebugLibraries>false</UseDebugLibraries>
+    <WholeProgramOptimization>true</WholeProgramOptimization>
+    <CharacterSet>Unicode</CharacterSet>
     <PlatformToolset>v141</PlatformToolset>
-    <CharacterSet>MultiByte</CharacterSet>
   </PropertyGroup>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.props"/>
   <ImportGroup Label="ExtensionSettings"/>
-  <ImportGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'" Label="PropertySheets">
+  <ImportGroup Label="PropertySheets" Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">
     <Import Project="$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props" Condition="exists('$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props')" Label="LocalAppDataPlatform"/>
-    <Import Project="rsvg-gen-srcs.props"/>
   </ImportGroup>
-  <ImportGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'" Label="PropertySheets">
+  <ImportGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'" Label="PropertySheets">
     <Import Project="$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props" Condition="exists('$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props')" Label="LocalAppDataPlatform"/>
-    <Import Project="rsvg-gen-srcs.props"/>
   </ImportGroup>
-  <ImportGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'" Label="PropertySheets">
+  <ImportGroup Label="PropertySheets" Condition="'$(Configuration)|$(Platform)'=='Release|Win32'">
     <Import Project="$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props" Condition="exists('$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props')" Label="LocalAppDataPlatform"/>
-    <Import Project="rsvg-gen-srcs.props"/>
   </ImportGroup>
-  <ImportGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'" Label="PropertySheets">
+  <ImportGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'" Label="PropertySheets">
     <Import Project="$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props" Condition="exists('$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props')" Label="LocalAppDataPlatform"/>
-    <Import Project="rsvg-gen-srcs.props"/>
   </ImportGroup>
   <PropertyGroup Label="UserMacros"/>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">
     <LinkIncremental>true</LinkIncremental>
-  </PropertyGroup>
-  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'">
-    <LinkIncremental>false</LinkIncremental>
+    <IncludePath>$(IncludePath);$(UniversalCRT_IncludePath);$(SolutionDir)..\..\lib;$(VCInstallDir)include;$(VCInstallDir)atlmfc\include;$(WindowsSDK_IncludePath);</IncludePath>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'">
     <LinkIncremental>true</LinkIncremental>
+    <IncludePath>$(IncludePath);$(UniversalCRT_IncludePath);$(SolutionDir)..\..\lib;$(VCInstallDir)include;$(VCInstallDir)atlmfc\include;$(WindowsSDK_IncludePath);</IncludePath>
+    <RunCodeAnalysis>true</RunCodeAnalysis>
+  </PropertyGroup>
+  <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'">
+    <LinkIncremental>false</LinkIncremental>
+    <IncludePath>$(IncludePath);$(UniversalCRT_IncludePath);$(SolutionDir)..\..\lib;$(VCInstallDir)include;$(VCInstallDir)atlmfc\include;$(WindowsSDK_IncludePath);</IncludePath>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'">
     <LinkIncremental>false</LinkIncremental>
+    <IncludePath>$(IncludePath);$(UniversalCRT_IncludePath);$(SolutionDir)..\..\lib;$(VCInstallDir)include;$(VCInstallDir)atlmfc\include;$(WindowsSDK_IncludePath);</IncludePath>
+    <RunCodeAnalysis>true</RunCodeAnalysis>
   </PropertyGroup>
   <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">
     <ClCompile>
-      <Optimization>Disabled</Optimization>
-      <AdditionalIncludeDirectories>$(LibRsvgIncPath);%(AdditionalIncludeDirectories)</AdditionalIncludeDirectories>
-      <PreprocessorDefinitions>_DEBUG;$(LibRsvgCFlags);%(PreprocessorDefinitions)</PreprocessorDefinitions>
-      <MinimalRebuild>true</MinimalRebuild>
-      <BasicRuntimeChecks>EnableFastChecks</BasicRuntimeChecks>
-      <RuntimeLibrary>MultiThreadedDebugDLL</RuntimeLibrary>
       <PrecompiledHeader/>
-      <WarningLevel>Level3</WarningLevel>
-      <DebugInformationFormat>EditAndContinue</DebugInformationFormat>
+      <WarningLevel>Level4</WarningLevel>
+      <Optimization>Disabled</Optimization>
+      <PreprocessorDefinitions>WIN32;_DEBUG;_CONSOLE;%(PreprocessorDefinitions)</PreprocessorDefinitions>
+      <TreatWarningAsError>true</TreatWarningAsError>
+      <EnablePREfast>false</EnablePREfast>
     </ClCompile>
     <Link>
-      <AdditionalDependencies>$(LibRsvgLibs);%(AdditionalDependencies)</AdditionalDependencies>
-      <OutputFile>$(OutDir)$(RsvgDllPrefix)$(ProjectName)$(RsvgDllSuffix).dll</OutputFile>
-      <ModuleDefinitionFile>$(IntDir)$(ProjectName).def</ModuleDefinitionFile>
+      <SubSystem>Console</SubSystem>
       <GenerateDebugInformation>true</GenerateDebugInformation>
-      <ProgramDatabaseFile>$(TargetDir)$(RsvgDllPrefix)$(ProjectName)$(RsvgDllSuffix).pdb</ProgramDatabaseFile>
-      <SubSystem>Windows</SubSystem>
-      <ImportLibrary>$(TargetDir)$(ProjectName)-$(ApiVersion).lib</ImportLibrary>
-      <TargetMachine>MachineX86</TargetMachine>
+      <AdditionalDependencies>setargv.obj;%(AdditionalDependencies)</AdditionalDependencies>
     </Link>
   </ItemDefinitionGroup>
-  <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'">
+  <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'">
     <ClCompile>
-      <Optimization>MaxSpeed</Optimization>
-      <IntrinsicFunctions>true</IntrinsicFunctions>
-      <AdditionalIncludeDirectories>$(LibRsvgIncPath);%(AdditionalIncludeDirectories)</AdditionalIncludeDirectories>
-      <PreprocessorDefinitions>$(LibRsvgCFlags);%(PreprocessorDefinitions)</PreprocessorDefinitions>
-      <RuntimeLibrary>MultiThreadedDLL</RuntimeLibrary>
-      <FunctionLevelLinking>true</FunctionLevelLinking>
       <PrecompiledHeader/>
-      <WarningLevel>Level3</WarningLevel>
-      <DebugInformationFormat>ProgramDatabase</DebugInformationFormat>
+      <WarningLevel>Level4</WarningLevel>
+      <Optimization>Disabled</Optimization>
+      <PreprocessorDefinitions>WIN32;_DEBUG;_CONSOLE;%(PreprocessorDefinitions)</PreprocessorDefinitions>
+      <TreatWarningAsError>true</TreatWarningAsError>
+      <EnablePREfast>true</EnablePREfast>
+      <AdditionalOptions>/analyze:stacksize295252 %(AdditionalOptions)</AdditionalOptions>
     </ClCompile>
     <Link>
-      <AdditionalDependencies>$(LibRsvgLibs);%(AdditionalDependencies)</AdditionalDependencies>
-      <OutputFile>$(OutDir)$(RsvgDllPrefix)$(ProjectName)$(RsvgDllSuffix).dll</OutputFile>
-      <ModuleDefinitionFile>$(IntDir)$(ProjectName).def</ModuleDefinitionFile>
+      <SubSystem>Console</SubSystem>
       <GenerateDebugInformation>true</GenerateDebugInformation>
-      <ProgramDatabaseFile>$(TargetDir)$(RsvgDllPrefix)$(ProjectName)$(RsvgDllSuffix).pdb</ProgramDatabaseFile>
-      <SubSystem>Windows</SubSystem>
-      <OptimizeReferences>true</OptimizeReferences>
-      <EnableCOMDATFolding>true</EnableCOMDATFolding>
-      <ImportLibrary>$(TargetDir)$(ProjectName)-$(ApiVersion).lib</ImportLibrary>
-      <TargetMachine>MachineX86</TargetMachine>
+      <AdditionalDependencies>setargv.obj;%(AdditionalDependencies)</AdditionalDependencies>
     </Link>
   </ItemDefinitionGroup>
-  <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'">
-    <Midl>
-      <TargetEnvironment>X64</TargetEnvironment>
-    </Midl>
+  <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'">
     <ClCompile>
-      <Optimization>Disabled</Optimization>
-      <AdditionalIncludeDirectories>$(LibRsvgIncPath);%(AdditionalIncludeDirectories)</AdditionalIncludeDirectories>
-      <PreprocessorDefinitions>_DEBUG;$(LibRsvgCFlags);%(PreprocessorDefinitions)</PreprocessorDefinitions>
-      <MinimalRebuild>true</MinimalRebuild>
-      <BasicRuntimeChecks>EnableFastChecks</BasicRuntimeChecks>
-      <RuntimeLibrary>MultiThreadedDebugDLL</RuntimeLibrary>
+      <WarningLevel>Level4</WarningLevel>
       <PrecompiledHeader/>
-      <WarningLevel>Level3</WarningLevel>
-      <DebugInformationFormat>ProgramDatabase</DebugInformationFormat>
+      <Optimization>MaxSpeed</Optimization>
+      <FunctionLevelLinking>true</FunctionLevelLinking>
+      <IntrinsicFunctions>true</IntrinsicFunctions>
+      <PreprocessorDefinitions>WIN32;NDEBUG;_CONSOLE;%(PreprocessorDefinitions)</PreprocessorDefinitions>
+      <TreatWarningAsError>false</TreatWarningAsError>
+      <EnablePREfast>false</EnablePREfast>
     </ClCompile>
     <Link>
-      <AdditionalDependencies>$(LibRsvgLibs);%(AdditionalDependencies)</AdditionalDependencies>
-      <OutputFile>$(OutDir)$(RsvgDllPrefix)$(ProjectName)$(RsvgDllSuffix).dll</OutputFile>
-      <ModuleDefinitionFile>$(IntDir)$(ProjectName).def</ModuleDefinitionFile>
+      <SubSystem>Console</SubSystem>
       <GenerateDebugInformation>true</GenerateDebugInformation>
-      <ProgramDatabaseFile>$(TargetDir)$(RsvgDllPrefix)$(ProjectName)$(RsvgDllSuffix).pdb</ProgramDatabaseFile>
-      <SubSystem>Windows</SubSystem>
-      <ImportLibrary>$(TargetDir)$(ProjectName)-$(ApiVersion).lib</ImportLibrary>
-      <TargetMachine>MachineX64</TargetMachine>
+      <EnableCOMDATFolding>true</EnableCOMDATFolding>
+      <OptimizeReferences>true</OptimizeReferences>
+      <AdditionalDependencies>setargv.obj;%(AdditionalDependencies)</AdditionalDependencies>
     </Link>
   </ItemDefinitionGroup>
   <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'">
-    <Midl>
-      <TargetEnvironment>X64</TargetEnvironment>
-    </Midl>
     <ClCompile>
+      <WarningLevel>Level4</WarningLevel>
+      <PrecompiledHeader/>
       <Optimization>MaxSpeed</Optimization>
-      <IntrinsicFunctions>true</IntrinsicFunctions>
-      <AdditionalIncludeDirectories>$(LibRsvgIncPath);%(AdditionalIncludeDirectories)</AdditionalIncludeDirectories>
-      <PreprocessorDefinitions>$(LibRsvgCFlags);%(PreprocessorDefinitions)</PreprocessorDefinitions>
-      <RuntimeLibrary>MultiThreadedDLL</RuntimeLibrary>
       <FunctionLevelLinking>true</FunctionLevelLinking>
-      <PrecompiledHeader/>
-      <WarningLevel>Level3</WarningLevel>
-      <DebugInformationFormat>ProgramDatabase</DebugInformationFormat>
+      <IntrinsicFunctions>true</IntrinsicFunctions>
+      <PreprocessorDefinitions>WIN32;NDEBUG;_CONSOLE;%(PreprocessorDefinitions)</PreprocessorDefinitions>
+      <TreatWarningAsError>false</TreatWarningAsError>
+      <EnablePREfast>true</EnablePREfast>
+      <AdditionalOptions>/analyze:stacksize295252 %(AdditionalOptions)</AdditionalOptions>
     </ClCompile>
     <Link>
-      <AdditionalDependencies>$(LibRsvgLibs);%(AdditionalDependencies)</AdditionalDependencies>
-      <OutputFile>$(OutDir)$(RsvgDllPrefix)$(ProjectName)$(RsvgDllSuffix).dll</OutputFile>
-      <ModuleDefinitionFile>$(IntDir)$(ProjectName).def</ModuleDefinitionFile>
+      <SubSystem>Console</SubSystem>
       <GenerateDebugInformation>true</GenerateDebugInformation>
-      <ProgramDatabaseFile>$(TargetDir)$(RsvgDllPrefix)$(ProjectName)$(RsvgDllSuffix).pdb</ProgramDatabaseFile>
-      <SubSystem>Windows</SubSystem>
-      <OptimizeReferences>true</OptimizeReferences>
       <EnableCOMDATFolding>true</EnableCOMDATFolding>
-      <ImportLibrary>$(TargetDir)$(ProjectName)-$(ApiVersion).lib</ImportLibrary>
-      <TargetMachine>MachineX64</TargetMachine>
+      <OptimizeReferences>true</OptimizeReferences>
+      <AdditionalDependencies>setargv.obj;%(AdditionalDependencies)</AdditionalDependencies>
     </Link>
   </ItemDefinitionGroup>
   <ItemGroup>
-    <ClCompile Include="..\..\..\librsvg-features.c"/>
-    <ClCompile Include="..\..\..\rsvg-css.c"/>
-    <ClCompile Include="..\..\..\rsvg-defs.c"/>
-    <ClCompile Include="..\..\..\rsvg-image.c"/>
-    <ClCompile Include="..\..\..\rsvg-io.c"/>
-    <ClCompile Include="..\..\..\rsvg-paint-server.c"/>
-    <ClCompile Include="..\..\..\rsvg-path.c"/>
-    <ClCompile Include="..\..\..\rsvg-base-file-util.c"/>
-    <ClCompile Include="..\..\..\rsvg-filter.c"/>
-    <ClCompile Include="..\..\..\rsvg-marker.c"/>
-    <ClCompile Include="..\..\..\rsvg-mask.c"/>
-    <ClCompile Include="..\..\..\rsvg-shapes.c"/>
-    <ClCompile Include="..\..\..\rsvg-structure.c"/>
-    <ClCompile Include="..\..\..\rsvg-styles.c"/>
-    <ClCompile Include="..\..\..\rsvg-text.c"/>
-    <ClCompile Include="..\..\..\rsvg-cond.c"/>
-    <ClCompile Include="..\..\..\rsvg-base.c"/>
-    <ClCompile Include="..\..\..\librsvg-enum-types.c"/>
-    <ClCompile Include="..\..\..\rsvg-cairo-draw.c"/>
-    <ClCompile Include="..\..\..\rsvg-cairo-render.c"/>
-    <ClCompile Include="..\..\..\rsvg-cairo-clip.c"/>
-    <ClCompile Include="..\..\..\rsvg.c"/>
-    <ClCompile Include="..\..\..\rsvg-gobject.c"/>
-    <ClCompile Include="..\..\..\rsvg-file-util.c"/>
-    <ClCompile Include="..\..\..\rsvg-size-callback.c"/>
-    <ClCompile Include="..\..\..\rsvg-xml.c"/>
+    <ClInclude Include="..\..\..\lib\lz4.h"/>
+    <ClInclude Include="..\..\..\lib\lz4frame.h"/>
+    <ClInclude Include="..\..\..\lib\lz4frame_static.h"/>
+    <ClInclude Include="..\..\..\lib\lz4hc.h"/>
+    <ClInclude Include="..\..\..\lib\xxhash.h"/>
+    <ClInclude Include="..\..\..\programs\datagen.h"/>
+    <ClInclude Include="..\..\..\programs\bench.h"/>
+    <ClInclude Include="..\..\..\programs\lz4io.h"/>
+  </ItemGroup>
+  <ItemGroup>
+    <ClCompile Include="..\..\..\lib\lz4.c"/>
+    <ClCompile Include="..\..\..\lib\lz4frame.c"/>
+    <ClCompile Include="..\..\..\lib\lz4hc.c"/>
+    <ClCompile Include="..\..\..\lib\xxhash.c"/>
+    <ClCompile Include="..\..\..\programs\datagen.c"/>
+    <ClCompile Include="..\..\..\programs\bench.c"/>
+    <ClCompile Include="..\..\..\programs\lz4cli.c"/>
+    <ClCompile Include="..\..\..\programs\lz4io.c"/>
   </ItemGroup>
   <ItemGroup>
-    <CustomBuild Include="..\..\..\config.h.win32">
-      <Message Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">Copying config.h...</Message>
-      <Command Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">$(CopyConfigH)</Command>
-      <Outputs Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">..\..\..\config.h;%(Outputs)</Outputs>
-      <Message Condition="'$(Configuration)|$(Platform)'=='Debug|x64'">Copying config.h...</Message>
-      <Command Condition="'$(Configuration)|$(Platform)'=='Debug|x64'">$(CopyConfigH)</Command>
-      <Outputs Condition="'$(Configuration)|$(Platform)'=='Debug|x64'">..\..\..\config.h;%(Outputs)</Outputs>
-      <Message Condition="'$(Configuration)|$(Platform)'=='Release|Win32'">Copying config.h...</Message>
-      <Command Condition="'$(Configuration)|$(Platform)'=='Release|Win32'">$(CopyConfigH)</Command>
-      <Outputs Condition="'$(Configuration)|$(Platform)'=='Release|Win32'">..\..\..\config.h;%(Outputs)</Outputs>
-      <Message Condition="'$(Configuration)|$(Platform)'=='Release|x64'">Copying config.h...</Message>
-      <Command Condition="'$(Configuration)|$(Platform)'=='Release|x64'">$(CopyConfigH)</Command>
-      <Outputs Condition="'$(Configuration)|$(Platform)'=='Release|x64'">..\..\..\config.h;%(Outputs)</Outputs>
-    </CustomBuild>
-    <CustomBuild Include="..\..\..\rsvg.symbols">
-      <Message Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">Generating $(ProjectName).def...</Message>
-      <Command Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">$(GenerateRsvgDef)</Command>
-      <Outputs Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">$(IntDir)$(ProjectName).def;%(Outputs)</Outputs>
-      <Message Condition="'$(Configuration)|$(Platform)'=='Debug|x64'">Generating $(ProjectName).def...</Message>
-      <Command Condition="'$(Configuration)|$(Platform)'=='Debug|x64'">$(GenerateRsvgDef)</Command>
-      <Outputs Condition="'$(Configuration)|$(Platform)'=='Debug|x64'">$(IntDir)$(ProjectName).def;%(Outputs)</Outputs>
-      <Message Condition="'$(Configuration)|$(Platform)'=='Release|Win32'">Generating $(ProjectName).def...</Message>
-      <Command Condition="'$(Configuration)|$(Platform)'=='Release|Win32'">$(GenerateRsvgDef)</Command>
-      <Outputs Condition="'$(Configuration)|$(Platform)'=='Release|Win32'">$(IntDir)$(ProjectName).def;%(Outputs)</Outputs>
-      <Message Condition="'$(Configuration)|$(Platform)'=='Release|x64'">Generating $(ProjectName).def...</Message>
-      <Command Condition="'$(Configuration)|$(Platform)'=='Release|x64'">$(GenerateRsvgDef)</Command>
-      <Outputs Condition="'$(Configuration)|$(Platform)'=='Release|x64'">$(IntDir)$(ProjectName).def;%(Outputs)</Outputs>
-    </CustomBuild>
+    <ResourceCompile Include="lz4.rc"/>
   </ItemGroup>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.targets"/>
   <ImportGroup Label="ExtensionTargets"/>
 </Project>
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs12/config.h` & `gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs12/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs12/install.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs12/install.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs12/libssh-library.sln` & `gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs12/libssh-library.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs12/ssh_shared.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs12/ssh_shared.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs12/ssh_shared.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs12/ssh_shared.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs12/ssh_static.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs12/ssh_static.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs12/ssh_static.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs12/ssh_static.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs14/config.h` & `gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs14/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs14/install.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs15/install.vcxproj`

 * *Files 1% similar despite different names*

#### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs14/install.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs15/install.vcxproj`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<Project xmlns="http://schemas.microsoft.com/developer/msbuild/2003" DefaultTargets="Build" ToolsVersion="14.0">
+<Project xmlns="http://schemas.microsoft.com/developer/msbuild/2003" DefaultTargets="Build" ToolsVersion="15.0">
   <ItemGroup Label="ProjectConfigurations">
     <ProjectConfiguration Include="Debug|Win32">
       <Configuration>Debug</Configuration>
       <Platform>Win32</Platform>
     </ProjectConfiguration>
     <ProjectConfiguration Include="Debug|x64">
       <Configuration>Debug</Configuration>
@@ -18,39 +18,40 @@
       <Platform>x64</Platform>
     </ProjectConfiguration>
   </ItemGroup>
   <PropertyGroup Label="Globals">
     <ProjectGuid>{F42026FA-B395-4D5D-9F86-A98636F69607}</ProjectGuid>
     <Keyword>Win32Proj</Keyword>
     <RootNamespace>install</RootNamespace>
+    <WindowsTargetPlatformVersion>10.0.16299.0</WindowsTargetPlatformVersion>
   </PropertyGroup>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.Default.props"/>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
     <UseDebugLibraries>true</UseDebugLibraries>
-    <PlatformToolset>v140</PlatformToolset>
+    <PlatformToolset>v141</PlatformToolset>
     <CharacterSet>Unicode</CharacterSet>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
     <UseDebugLibraries>true</UseDebugLibraries>
-    <PlatformToolset>v140</PlatformToolset>
+    <PlatformToolset>v141</PlatformToolset>
     <CharacterSet>Unicode</CharacterSet>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
     <UseDebugLibraries>false</UseDebugLibraries>
-    <PlatformToolset>v140</PlatformToolset>
+    <PlatformToolset>v141</PlatformToolset>
     <WholeProgramOptimization>true</WholeProgramOptimization>
     <CharacterSet>Unicode</CharacterSet>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
     <UseDebugLibraries>false</UseDebugLibraries>
-    <PlatformToolset>v140</PlatformToolset>
+    <PlatformToolset>v141</PlatformToolset>
     <WholeProgramOptimization>true</WholeProgramOptimization>
     <CharacterSet>Unicode</CharacterSet>
   </PropertyGroup>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.props"/>
   <ImportGroup Label="ExtensionSettings"/>
   <ImportGroup Label="PropertySheets" Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">
     <Import Project="$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props" Condition="exists('$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props')" Label="LocalAppDataPlatform"/>
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs14/libssh-library.sln` & `gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs14/libssh-library.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs14/ssh_shared.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs14/ssh_shared.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs14/ssh_shared.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs14/ssh_shared.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs14/ssh_static.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs14/ssh_static.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs14/ssh_static.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs14/ssh_static.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs15/config.h` & `gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs15/config.h`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs15/install.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2015/datagen/datagen.vcxproj`

 * *Files 18% similar despite different names*

#### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs15/install.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2015/datagen/datagen.vcxproj`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<Project xmlns="http://schemas.microsoft.com/developer/msbuild/2003" DefaultTargets="Build" ToolsVersion="15.0">
+<Project xmlns="http://schemas.microsoft.com/developer/msbuild/2003" DefaultTargets="Build" ToolsVersion="12.0">
   <ItemGroup Label="ProjectConfigurations">
     <ProjectConfiguration Include="Debug|Win32">
       <Configuration>Debug</Configuration>
       <Platform>Win32</Platform>
     </ProjectConfiguration>
     <ProjectConfiguration Include="Debug|x64">
       <Configuration>Debug</Configuration>
@@ -15,45 +15,46 @@
     </ProjectConfiguration>
     <ProjectConfiguration Include="Release|x64">
       <Configuration>Release</Configuration>
       <Platform>x64</Platform>
     </ProjectConfiguration>
   </ItemGroup>
   <PropertyGroup Label="Globals">
-    <ProjectGuid>{F42026FA-B395-4D5D-9F86-A98636F69607}</ProjectGuid>
+    <ProjectGuid>{D745AE2F-596A-403A-9B91-81A8C6779243}</ProjectGuid>
     <Keyword>Win32Proj</Keyword>
-    <RootNamespace>install</RootNamespace>
-    <WindowsTargetPlatformVersion>10.0.16299.0</WindowsTargetPlatformVersion>
+    <RootNamespace>datagen</RootNamespace>
+    <OutDir>$(SolutionDir)bin\$(Platform)_$(Configuration)\</OutDir>
+    <IntDir>$(SolutionDir)bin\obj\$(RootNamespace)_$(Platform)_$(Configuration)\</IntDir>
   </PropertyGroup>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.Default.props"/>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
     <UseDebugLibraries>true</UseDebugLibraries>
-    <PlatformToolset>v141</PlatformToolset>
     <CharacterSet>Unicode</CharacterSet>
+    <PlatformToolset>v140</PlatformToolset>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
     <UseDebugLibraries>true</UseDebugLibraries>
-    <PlatformToolset>v141</PlatformToolset>
     <CharacterSet>Unicode</CharacterSet>
+    <PlatformToolset>v140</PlatformToolset>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
     <UseDebugLibraries>false</UseDebugLibraries>
-    <PlatformToolset>v141</PlatformToolset>
     <WholeProgramOptimization>true</WholeProgramOptimization>
     <CharacterSet>Unicode</CharacterSet>
+    <PlatformToolset>v140</PlatformToolset>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
     <UseDebugLibraries>false</UseDebugLibraries>
-    <PlatformToolset>v141</PlatformToolset>
     <WholeProgramOptimization>true</WholeProgramOptimization>
     <CharacterSet>Unicode</CharacterSet>
+    <PlatformToolset>v140</PlatformToolset>
   </PropertyGroup>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.props"/>
   <ImportGroup Label="ExtensionSettings"/>
   <ImportGroup Label="PropertySheets" Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">
     <Import Project="$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props" Condition="exists('$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props')" Label="LocalAppDataPlatform"/>
   </ImportGroup>
   <ImportGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'" Label="PropertySheets">
@@ -61,102 +62,102 @@
   </ImportGroup>
   <ImportGroup Label="PropertySheets" Condition="'$(Configuration)|$(Platform)'=='Release|Win32'">
     <Import Project="$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props" Condition="exists('$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props')" Label="LocalAppDataPlatform"/>
   </ImportGroup>
   <ImportGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'" Label="PropertySheets">
     <Import Project="$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props" Condition="exists('$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props')" Label="LocalAppDataPlatform"/>
   </ImportGroup>
-  <Import Project="property.props"/>
-  <Import Project="..\..\..\stack.props"/>
   <PropertyGroup Label="UserMacros"/>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">
     <LinkIncremental>true</LinkIncremental>
-    <OutDir>$(PrjInstallRoot)\</OutDir>
-    <IntDir>$(SolutionDir)$(Configuration)\$(PlatformName)\obj\$(ProjectName)</IntDir>
+    <IncludePath>$(IncludePath);$(UniversalCRT_IncludePath);$(SolutionDir)..\..\programs;$(SolutionDir)..\..\lib;$(VCInstallDir)include;$(VCInstallDir)atlmfc\include;$(WindowsSDK_IncludePath);</IncludePath>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'">
     <LinkIncremental>true</LinkIncremental>
-    <OutDir>$(PrjInstallRoot)\</OutDir>
-    <IntDir>$(SolutionDir)$(Configuration)\$(PlatformName)\obj\$(ProjectName)</IntDir>
+    <IncludePath>$(IncludePath);$(UniversalCRT_IncludePath);$(SolutionDir)..\..\programs;$(SolutionDir)..\..\lib;$(VCInstallDir)include;$(VCInstallDir)atlmfc\include;$(WindowsSDK_IncludePath);</IncludePath>
+    <RunCodeAnalysis>true</RunCodeAnalysis>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'">
     <LinkIncremental>false</LinkIncremental>
-    <OutDir>$(PrjInstallRoot)\</OutDir>
-    <IntDir>$(SolutionDir)$(Configuration)\$(PlatformName)\obj\$(ProjectName)</IntDir>
+    <IncludePath>$(IncludePath);$(UniversalCRT_IncludePath);$(SolutionDir)..\..\programs;$(SolutionDir)..\..\lib;$(VCInstallDir)include;$(VCInstallDir)atlmfc\include;$(WindowsSDK_IncludePath);</IncludePath>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'">
     <LinkIncremental>false</LinkIncremental>
-    <OutDir>$(PrjInstallRoot)\</OutDir>
-    <IntDir>$(SolutionDir)$(Configuration)\$(PlatformName)\obj\$(ProjectName)</IntDir>
+    <IncludePath>$(IncludePath);$(UniversalCRT_IncludePath);$(SolutionDir)..\..\programs;$(SolutionDir)..\..\lib;$(VCInstallDir)include;$(VCInstallDir)atlmfc\include;$(WindowsSDK_IncludePath);</IncludePath>
+    <RunCodeAnalysis>true</RunCodeAnalysis>
   </PropertyGroup>
   <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">
     <ClCompile>
       <PrecompiledHeader/>
-      <WarningLevel>Level3</WarningLevel>
+      <WarningLevel>Level4</WarningLevel>
       <Optimization>Disabled</Optimization>
-      <PreprocessorDefinitions>WIN32;_DEBUG;_CONSOLE;_LIB;%(PreprocessorDefinitions)</PreprocessorDefinitions>
+      <PreprocessorDefinitions>WIN32;_DEBUG;_CONSOLE;%(PreprocessorDefinitions)</PreprocessorDefinitions>
+      <TreatWarningAsError>true</TreatWarningAsError>
+      <EnablePREfast>false</EnablePREfast>
     </ClCompile>
     <Link>
       <SubSystem>Console</SubSystem>
       <GenerateDebugInformation>true</GenerateDebugInformation>
     </Link>
-    <PreBuildEvent>
-      <Command>$(PrjDoInstall)</Command>
-    </PreBuildEvent>
   </ItemDefinitionGroup>
   <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'">
     <ClCompile>
       <PrecompiledHeader/>
-      <WarningLevel>Level3</WarningLevel>
+      <WarningLevel>Level4</WarningLevel>
       <Optimization>Disabled</Optimization>
-      <PreprocessorDefinitions>WIN32;_DEBUG;_CONSOLE;_LIB;%(PreprocessorDefinitions)</PreprocessorDefinitions>
+      <PreprocessorDefinitions>WIN32;_DEBUG;_CONSOLE;%(PreprocessorDefinitions)</PreprocessorDefinitions>
+      <TreatWarningAsError>true</TreatWarningAsError>
+      <EnablePREfast>true</EnablePREfast>
+      <AdditionalOptions>/analyze:stacksize295252 %(AdditionalOptions)</AdditionalOptions>
     </ClCompile>
     <Link>
       <SubSystem>Console</SubSystem>
       <GenerateDebugInformation>true</GenerateDebugInformation>
     </Link>
-    <PreBuildEvent>
-      <Command>$(PrjDoInstall)</Command>
-    </PreBuildEvent>
   </ItemDefinitionGroup>
   <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'">
     <ClCompile>
-      <WarningLevel>Level3</WarningLevel>
+      <WarningLevel>Level4</WarningLevel>
       <PrecompiledHeader/>
       <Optimization>MaxSpeed</Optimization>
       <FunctionLevelLinking>true</FunctionLevelLinking>
       <IntrinsicFunctions>true</IntrinsicFunctions>
-      <PreprocessorDefinitions>WIN32;NDEBUG;_CONSOLE;_LIB;%(PreprocessorDefinitions)</PreprocessorDefinitions>
+      <PreprocessorDefinitions>WIN32;NDEBUG;_CONSOLE;%(PreprocessorDefinitions)</PreprocessorDefinitions>
+      <TreatWarningAsError>false</TreatWarningAsError>
+      <EnablePREfast>false</EnablePREfast>
     </ClCompile>
     <Link>
       <SubSystem>Console</SubSystem>
       <GenerateDebugInformation>true</GenerateDebugInformation>
       <EnableCOMDATFolding>true</EnableCOMDATFolding>
       <OptimizeReferences>true</OptimizeReferences>
     </Link>
-    <PreBuildEvent>
-      <Command>$(PrjDoInstall)</Command>
-    </PreBuildEvent>
   </ItemDefinitionGroup>
   <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'">
     <ClCompile>
-      <WarningLevel>Level3</WarningLevel>
+      <WarningLevel>Level4</WarningLevel>
       <PrecompiledHeader/>
       <Optimization>MaxSpeed</Optimization>
       <FunctionLevelLinking>true</FunctionLevelLinking>
       <IntrinsicFunctions>true</IntrinsicFunctions>
-      <PreprocessorDefinitions>WIN32;NDEBUG;_CONSOLE;_LIB;%(PreprocessorDefinitions)</PreprocessorDefinitions>
+      <PreprocessorDefinitions>WIN32;NDEBUG;_CONSOLE;%(PreprocessorDefinitions)</PreprocessorDefinitions>
+      <TreatWarningAsError>false</TreatWarningAsError>
+      <EnablePREfast>true</EnablePREfast>
+      <AdditionalOptions>/analyze:stacksize295252 %(AdditionalOptions)</AdditionalOptions>
     </ClCompile>
     <Link>
       <SubSystem>Console</SubSystem>
       <GenerateDebugInformation>true</GenerateDebugInformation>
       <EnableCOMDATFolding>true</EnableCOMDATFolding>
       <OptimizeReferences>true</OptimizeReferences>
     </Link>
-    <PreBuildEvent>
-      <Command>$(PrjDoInstall)</Command>
-    </PreBuildEvent>
   </ItemDefinitionGroup>
-  <ItemGroup/>
+  <ItemGroup>
+    <ClCompile Include="..\..\..\programs\datagen.c"/>
+    <ClCompile Include="..\..\..\tests\datagencli.c"/>
+  </ItemGroup>
+  <ItemGroup>
+    <ClInclude Include="..\..\..\programs\datagen.h"/>
+  </ItemGroup>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.targets"/>
   <ImportGroup Label="ExtensionTargets"/>
 </Project>
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs15/libssh-library.sln` & `gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs15/libssh-library.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs15/ssh_shared.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs15/ssh_shared.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs15/ssh_shared.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs15/ssh_shared.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs15/ssh_static.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs15/ssh_static.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/libssh/build/vs15/ssh_static.vcxproj.filters` & `gvsbuild-2024.5.0/gvsbuild/patches/libssh/build/vs15/ssh_static.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/libssh/mod.md` & `gvsbuild-2024.5.0/gvsbuild/patches/libssh/mod.md`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/libtiff-4/0001-cmake-remove-.d-postfix.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/libtiff-4/0001-cmake-remove-.d-postfix.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/libvpx/0001-Always-generate-pc-file.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/libvpx/0001-Always-generate-pc-file.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/libvpx/0006-gen_msvs_vcxproj.sh-Select-current-Windows-SDK-if-av.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/libvpx/0006-gen_msvs_vcxproj.sh-Select-current-Windows-SDK-if-av.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/libxml2/include/libxml/meson.build` & `gvsbuild-2024.5.0/gvsbuild/patches/libxml2/include/libxml/meson.build`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/libxml2/LICENSE.build` & `gvsbuild-2024.5.0/gvsbuild/patches/libxml2/LICENSE.build`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/libxml2/meson.build` & `gvsbuild-2024.5.0/gvsbuild/patches/libxml2/meson.build`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/libyuv/001-win-build.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/libyuv/001-win-build.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/luajit/set-paths.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/luajit/set-paths.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/datagen/datagen.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2013/datagen/datagen.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/frametest/frametest.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2015/frametest/frametest.vcxproj`

 * *Files 0% similar despite different names*

#### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/frametest/frametest.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2015/frametest/frametest.vcxproj`

```diff
@@ -26,35 +26,35 @@
     <IntDir>$(SolutionDir)bin\obj\$(RootNamespace)_$(Platform)_$(Configuration)\</IntDir>
   </PropertyGroup>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.Default.props"/>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
     <UseDebugLibraries>true</UseDebugLibraries>
     <CharacterSet>Unicode</CharacterSet>
-    <PlatformToolset>v120</PlatformToolset>
+    <PlatformToolset>v140</PlatformToolset>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
     <UseDebugLibraries>true</UseDebugLibraries>
     <CharacterSet>Unicode</CharacterSet>
-    <PlatformToolset>v120</PlatformToolset>
+    <PlatformToolset>v140</PlatformToolset>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
     <UseDebugLibraries>false</UseDebugLibraries>
     <WholeProgramOptimization>true</WholeProgramOptimization>
     <CharacterSet>Unicode</CharacterSet>
-    <PlatformToolset>v120</PlatformToolset>
+    <PlatformToolset>v140</PlatformToolset>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
     <UseDebugLibraries>false</UseDebugLibraries>
     <WholeProgramOptimization>true</WholeProgramOptimization>
     <CharacterSet>Unicode</CharacterSet>
-    <PlatformToolset>v120</PlatformToolset>
+    <PlatformToolset>v140</PlatformToolset>
   </PropertyGroup>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.props"/>
   <ImportGroup Label="ExtensionSettings"/>
   <ImportGroup Label="PropertySheets" Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">
     <Import Project="$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props" Condition="exists('$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props')" Label="LocalAppDataPlatform"/>
   </ImportGroup>
   <ImportGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'" Label="PropertySheets">
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/fullbench/fullbench.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2013/fullbench/fullbench.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/fullbench-dll/fullbench-dll.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2013/fullbench-dll/fullbench-dll.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/fuzzer/fuzzer.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2013/fuzzer/fuzzer.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/liblz4/liblz4.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2013/liblz4/liblz4.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/liblz4-dll/liblz4-dll.rc` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2013/liblz4-dll/liblz4-dll.rc`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/liblz4-dll/liblz4-dll.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2013/liblz4-dll/liblz4-dll.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/lz4/lz4.rc` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2013/lz4/lz4.rc`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/lz4/lz4.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2013/lz4/lz4.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2013/lz4.sln` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2013/lz4.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/datagen/datagen.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2017/datagen/datagen.vcxproj`

 * *Files 1% similar despite different names*

#### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/datagen/datagen.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2017/datagen/datagen.vcxproj`

```diff
@@ -26,35 +26,35 @@
     <IntDir>$(SolutionDir)bin\obj\$(RootNamespace)_$(Platform)_$(Configuration)\</IntDir>
   </PropertyGroup>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.Default.props"/>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
     <UseDebugLibraries>true</UseDebugLibraries>
     <CharacterSet>Unicode</CharacterSet>
-    <PlatformToolset>v140</PlatformToolset>
+    <PlatformToolset>v141</PlatformToolset>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
     <UseDebugLibraries>true</UseDebugLibraries>
     <CharacterSet>Unicode</CharacterSet>
-    <PlatformToolset>v140</PlatformToolset>
+    <PlatformToolset>v141</PlatformToolset>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
     <UseDebugLibraries>false</UseDebugLibraries>
     <WholeProgramOptimization>true</WholeProgramOptimization>
     <CharacterSet>Unicode</CharacterSet>
-    <PlatformToolset>v140</PlatformToolset>
+    <PlatformToolset>v141</PlatformToolset>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
     <UseDebugLibraries>false</UseDebugLibraries>
     <WholeProgramOptimization>true</WholeProgramOptimization>
     <CharacterSet>Unicode</CharacterSet>
-    <PlatformToolset>v140</PlatformToolset>
+    <PlatformToolset>v141</PlatformToolset>
   </PropertyGroup>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.props"/>
   <ImportGroup Label="ExtensionSettings"/>
   <ImportGroup Label="PropertySheets" Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">
     <Import Project="$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props" Condition="exists('$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props')" Label="LocalAppDataPlatform"/>
   </ImportGroup>
   <ImportGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'" Label="PropertySheets">
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/frametest/frametest.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2015/fullbench/fullbench.vcxproj`

 * *Files 1% similar despite different names*

#### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/frametest/frametest.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2015/fullbench/fullbench.vcxproj`

```diff
@@ -15,17 +15,17 @@
     </ProjectConfiguration>
     <ProjectConfiguration Include="Release|x64">
       <Configuration>Release</Configuration>
       <Platform>x64</Platform>
     </ProjectConfiguration>
   </ItemGroup>
   <PropertyGroup Label="Globals">
-    <ProjectGuid>{39AD6ECC-8BAD-4368-95E4-A1AA2F077BB7}</ProjectGuid>
+    <ProjectGuid>{6A4DF4EF-C77F-43C6-8901-DDCD20879E4E}</ProjectGuid>
     <Keyword>Win32Proj</Keyword>
-    <RootNamespace>frametest</RootNamespace>
+    <RootNamespace>fullbench</RootNamespace>
     <OutDir>$(SolutionDir)bin\$(Platform)_$(Configuration)\</OutDir>
     <IntDir>$(SolutionDir)bin\obj\$(RootNamespace)_$(Platform)_$(Configuration)\</IntDir>
   </PropertyGroup>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.Default.props"/>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
     <UseDebugLibraries>true</UseDebugLibraries>
@@ -152,15 +152,15 @@
     </Link>
   </ItemDefinitionGroup>
   <ItemGroup>
     <ClCompile Include="..\..\..\lib\lz4.c"/>
     <ClCompile Include="..\..\..\lib\lz4frame.c"/>
     <ClCompile Include="..\..\..\lib\lz4hc.c"/>
     <ClCompile Include="..\..\..\lib\xxhash.c"/>
-    <ClCompile Include="..\..\..\tests\frametest.c"/>
+    <ClCompile Include="..\..\..\tests\fullbench.c"/>
   </ItemGroup>
   <ItemGroup>
     <ClInclude Include="..\..\..\lib\lz4.h"/>
     <ClInclude Include="..\..\..\lib\lz4frame.h"/>
     <ClInclude Include="..\..\..\lib\lz4frame_static.h"/>
     <ClInclude Include="..\..\..\lib\lz4hc.h"/>
     <ClInclude Include="..\..\..\lib\xxhash.h"/>
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/fullbench/fullbench.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2017/fullbench/fullbench.vcxproj`

 * *Files 1% similar despite different names*

#### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/fullbench/fullbench.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2017/fullbench/fullbench.vcxproj`

```diff
@@ -26,35 +26,35 @@
     <IntDir>$(SolutionDir)bin\obj\$(RootNamespace)_$(Platform)_$(Configuration)\</IntDir>
   </PropertyGroup>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.Default.props"/>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
     <UseDebugLibraries>true</UseDebugLibraries>
     <CharacterSet>Unicode</CharacterSet>
-    <PlatformToolset>v140</PlatformToolset>
+    <PlatformToolset>v141</PlatformToolset>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
     <UseDebugLibraries>true</UseDebugLibraries>
     <CharacterSet>Unicode</CharacterSet>
-    <PlatformToolset>v140</PlatformToolset>
+    <PlatformToolset>v141</PlatformToolset>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
     <UseDebugLibraries>false</UseDebugLibraries>
     <WholeProgramOptimization>true</WholeProgramOptimization>
     <CharacterSet>Unicode</CharacterSet>
-    <PlatformToolset>v140</PlatformToolset>
+    <PlatformToolset>v141</PlatformToolset>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
     <UseDebugLibraries>false</UseDebugLibraries>
     <WholeProgramOptimization>true</WholeProgramOptimization>
     <CharacterSet>Unicode</CharacterSet>
-    <PlatformToolset>v140</PlatformToolset>
+    <PlatformToolset>v141</PlatformToolset>
   </PropertyGroup>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.props"/>
   <ImportGroup Label="ExtensionSettings"/>
   <ImportGroup Label="PropertySheets" Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">
     <Import Project="$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props" Condition="exists('$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props')" Label="LocalAppDataPlatform"/>
   </ImportGroup>
   <ImportGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'" Label="PropertySheets">
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/fullbench-dll/fullbench-dll.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2015/fullbench-dll/fullbench-dll.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/fuzzer/fuzzer.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2015/fuzzer/fuzzer.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/liblz4/liblz4.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2015/liblz4/liblz4.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/liblz4-dll/liblz4-dll.rc` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2015/liblz4-dll/liblz4-dll.rc`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/liblz4-dll/liblz4-dll.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2015/liblz4-dll/liblz4-dll.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/lz4/lz4.rc` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2015/lz4/lz4.rc`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/lz4/lz4.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2015/lz4/lz4.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2015/lz4.sln` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2015/lz4.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/datagen/datagen.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2022/datagen/datagen.vcxproj`

 * *Files 0% similar despite different names*

#### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/datagen/datagen.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2022/datagen/datagen.vcxproj`

```diff
@@ -26,35 +26,35 @@
     <IntDir>$(SolutionDir)bin\obj\$(RootNamespace)_$(Platform)_$(Configuration)\</IntDir>
   </PropertyGroup>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.Default.props"/>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
     <UseDebugLibraries>true</UseDebugLibraries>
     <CharacterSet>Unicode</CharacterSet>
-    <PlatformToolset>v141</PlatformToolset>
+    <PlatformToolset>v143</PlatformToolset>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
     <UseDebugLibraries>true</UseDebugLibraries>
     <CharacterSet>Unicode</CharacterSet>
-    <PlatformToolset>v141</PlatformToolset>
+    <PlatformToolset>v143</PlatformToolset>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
     <UseDebugLibraries>false</UseDebugLibraries>
     <WholeProgramOptimization>true</WholeProgramOptimization>
     <CharacterSet>Unicode</CharacterSet>
-    <PlatformToolset>v141</PlatformToolset>
+    <PlatformToolset>v143</PlatformToolset>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
     <UseDebugLibraries>false</UseDebugLibraries>
     <WholeProgramOptimization>true</WholeProgramOptimization>
     <CharacterSet>Unicode</CharacterSet>
-    <PlatformToolset>v141</PlatformToolset>
+    <PlatformToolset>v143</PlatformToolset>
   </PropertyGroup>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.props"/>
   <ImportGroup Label="ExtensionSettings"/>
   <ImportGroup Label="PropertySheets" Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">
     <Import Project="$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props" Condition="exists('$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props')" Label="LocalAppDataPlatform"/>
   </ImportGroup>
   <ImportGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'" Label="PropertySheets">
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/frametest/frametest.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2017/frametest/frametest.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/fullbench/fullbench.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2022/fullbench/fullbench.vcxproj`

 * *Files 0% similar despite different names*

#### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/fullbench/fullbench.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2022/fullbench/fullbench.vcxproj`

```diff
@@ -26,35 +26,35 @@
     <IntDir>$(SolutionDir)bin\obj\$(RootNamespace)_$(Platform)_$(Configuration)\</IntDir>
   </PropertyGroup>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.Default.props"/>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
     <UseDebugLibraries>true</UseDebugLibraries>
     <CharacterSet>Unicode</CharacterSet>
-    <PlatformToolset>v141</PlatformToolset>
+    <PlatformToolset>v143</PlatformToolset>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
     <UseDebugLibraries>true</UseDebugLibraries>
     <CharacterSet>Unicode</CharacterSet>
-    <PlatformToolset>v141</PlatformToolset>
+    <PlatformToolset>v143</PlatformToolset>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
     <UseDebugLibraries>false</UseDebugLibraries>
     <WholeProgramOptimization>true</WholeProgramOptimization>
     <CharacterSet>Unicode</CharacterSet>
-    <PlatformToolset>v141</PlatformToolset>
+    <PlatformToolset>v143</PlatformToolset>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
     <UseDebugLibraries>false</UseDebugLibraries>
     <WholeProgramOptimization>true</WholeProgramOptimization>
     <CharacterSet>Unicode</CharacterSet>
-    <PlatformToolset>v141</PlatformToolset>
+    <PlatformToolset>v143</PlatformToolset>
   </PropertyGroup>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.props"/>
   <ImportGroup Label="ExtensionSettings"/>
   <ImportGroup Label="PropertySheets" Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">
     <Import Project="$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props" Condition="exists('$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props')" Label="LocalAppDataPlatform"/>
   </ImportGroup>
   <ImportGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'" Label="PropertySheets">
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/fullbench-dll/fullbench-dll.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2022/fullbench-dll/fullbench-dll.vcxproj`

 * *Files 0% similar despite different names*

#### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/fullbench-dll/fullbench-dll.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2022/fullbench-dll/fullbench-dll.vcxproj`

```diff
@@ -26,35 +26,35 @@
     <IntDir>$(SolutionDir)bin\obj\$(RootNamespace)_$(Platform)_$(Configuration)\</IntDir>
   </PropertyGroup>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.Default.props"/>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
     <UseDebugLibraries>true</UseDebugLibraries>
     <CharacterSet>Unicode</CharacterSet>
-    <PlatformToolset>v141</PlatformToolset>
+    <PlatformToolset>v143</PlatformToolset>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
     <UseDebugLibraries>true</UseDebugLibraries>
     <CharacterSet>Unicode</CharacterSet>
-    <PlatformToolset>v141</PlatformToolset>
+    <PlatformToolset>v143</PlatformToolset>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
     <UseDebugLibraries>false</UseDebugLibraries>
     <WholeProgramOptimization>true</WholeProgramOptimization>
     <CharacterSet>Unicode</CharacterSet>
-    <PlatformToolset>v141</PlatformToolset>
+    <PlatformToolset>v143</PlatformToolset>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
     <UseDebugLibraries>false</UseDebugLibraries>
     <WholeProgramOptimization>true</WholeProgramOptimization>
     <CharacterSet>Unicode</CharacterSet>
-    <PlatformToolset>v141</PlatformToolset>
+    <PlatformToolset>v143</PlatformToolset>
   </PropertyGroup>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.props"/>
   <ImportGroup Label="ExtensionSettings"/>
   <ImportGroup Label="PropertySheets" Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">
     <Import Project="$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props" Condition="exists('$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props')" Label="LocalAppDataPlatform"/>
   </ImportGroup>
   <ImportGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'" Label="PropertySheets">
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/fuzzer/fuzzer.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2017/fuzzer/fuzzer.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/liblz4/liblz4.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2017/liblz4/liblz4.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/liblz4-dll/liblz4-dll.rc` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2017/liblz4-dll/liblz4-dll.rc`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/liblz4-dll/liblz4-dll.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2017/liblz4-dll/liblz4-dll.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/lz4/lz4.rc` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2017/lz4/lz4.rc`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/lz4/lz4.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2022/lz4/lz4.vcxproj`

 * *Files 2% similar despite different names*

#### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/lz4/lz4.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2022/lz4/lz4.vcxproj`

```diff
@@ -26,35 +26,35 @@
     <IntDir>$(SolutionDir)bin\obj\$(RootNamespace)_$(Platform)_$(Configuration)\</IntDir>
   </PropertyGroup>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.Default.props"/>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
     <UseDebugLibraries>true</UseDebugLibraries>
     <CharacterSet>Unicode</CharacterSet>
-    <PlatformToolset>v141</PlatformToolset>
+    <PlatformToolset>v143</PlatformToolset>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
     <UseDebugLibraries>true</UseDebugLibraries>
     <CharacterSet>Unicode</CharacterSet>
-    <PlatformToolset>v141</PlatformToolset>
+    <PlatformToolset>v143</PlatformToolset>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
     <UseDebugLibraries>false</UseDebugLibraries>
     <WholeProgramOptimization>true</WholeProgramOptimization>
     <CharacterSet>Unicode</CharacterSet>
-    <PlatformToolset>v141</PlatformToolset>
+    <PlatformToolset>v143</PlatformToolset>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
     <UseDebugLibraries>false</UseDebugLibraries>
     <WholeProgramOptimization>true</WholeProgramOptimization>
     <CharacterSet>Unicode</CharacterSet>
-    <PlatformToolset>v141</PlatformToolset>
+    <PlatformToolset>v143</PlatformToolset>
   </PropertyGroup>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.props"/>
   <ImportGroup Label="ExtensionSettings"/>
   <ImportGroup Label="PropertySheets" Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">
     <Import Project="$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props" Condition="exists('$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props')" Label="LocalAppDataPlatform"/>
   </ImportGroup>
   <ImportGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'" Label="PropertySheets">
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2017/lz4.sln` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2017/lz4.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2022/datagen/datagen.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2022/fuzzer/fuzzer.vcxproj`

 * *Files 3% similar despite different names*

#### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2022/datagen/datagen.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2022/fuzzer/fuzzer.vcxproj`

```diff
@@ -15,17 +15,17 @@
     </ProjectConfiguration>
     <ProjectConfiguration Include="Release|x64">
       <Configuration>Release</Configuration>
       <Platform>x64</Platform>
     </ProjectConfiguration>
   </ItemGroup>
   <PropertyGroup Label="Globals">
-    <ProjectGuid>{D745AE2F-596A-403A-9B91-81A8C6779243}</ProjectGuid>
+    <ProjectGuid>{18B9F1A7-9C66-4352-898B-30804DADE0FD}</ProjectGuid>
     <Keyword>Win32Proj</Keyword>
-    <RootNamespace>datagen</RootNamespace>
+    <RootNamespace>fuzzer</RootNamespace>
     <OutDir>$(SolutionDir)bin\$(Platform)_$(Configuration)\</OutDir>
     <IntDir>$(SolutionDir)bin\obj\$(RootNamespace)_$(Platform)_$(Configuration)\</IntDir>
   </PropertyGroup>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.Default.props"/>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'" Label="Configuration">
     <ConfigurationType>Application</ConfigurationType>
     <UseDebugLibraries>true</UseDebugLibraries>
@@ -65,28 +65,28 @@
   </ImportGroup>
   <ImportGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'" Label="PropertySheets">
     <Import Project="$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props" Condition="exists('$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props')" Label="LocalAppDataPlatform"/>
   </ImportGroup>
   <PropertyGroup Label="UserMacros"/>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">
     <LinkIncremental>true</LinkIncremental>
-    <IncludePath>$(IncludePath);$(UniversalCRT_IncludePath);$(SolutionDir)..\..\programs;$(SolutionDir)..\..\lib;$(VCInstallDir)include;$(VCInstallDir)atlmfc\include;$(WindowsSDK_IncludePath);</IncludePath>
+    <IncludePath>$(IncludePath);$(UniversalCRT_IncludePath);$(SolutionDir)..\..\lib;$(SolutionDir)..\..\programs;$(VCInstallDir)include;$(VCInstallDir)atlmfc\include;$(WindowsSDK_IncludePath);</IncludePath>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'">
     <LinkIncremental>true</LinkIncremental>
-    <IncludePath>$(IncludePath);$(UniversalCRT_IncludePath);$(SolutionDir)..\..\programs;$(SolutionDir)..\..\lib;$(VCInstallDir)include;$(VCInstallDir)atlmfc\include;$(WindowsSDK_IncludePath);</IncludePath>
+    <IncludePath>$(IncludePath);$(UniversalCRT_IncludePath);$(SolutionDir)..\..\lib;$(SolutionDir)..\..\programs;$(VCInstallDir)include;$(VCInstallDir)atlmfc\include;$(WindowsSDK_IncludePath);</IncludePath>
     <RunCodeAnalysis>true</RunCodeAnalysis>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'">
     <LinkIncremental>false</LinkIncremental>
-    <IncludePath>$(IncludePath);$(UniversalCRT_IncludePath);$(SolutionDir)..\..\programs;$(SolutionDir)..\..\lib;$(VCInstallDir)include;$(VCInstallDir)atlmfc\include;$(WindowsSDK_IncludePath);</IncludePath>
+    <IncludePath>$(IncludePath);$(UniversalCRT_IncludePath);$(SolutionDir)..\..\lib;$(SolutionDir)..\..\programs;$(VCInstallDir)include;$(VCInstallDir)atlmfc\include;$(WindowsSDK_IncludePath);</IncludePath>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'">
     <LinkIncremental>false</LinkIncremental>
-    <IncludePath>$(IncludePath);$(UniversalCRT_IncludePath);$(SolutionDir)..\..\programs;$(SolutionDir)..\..\lib;$(VCInstallDir)include;$(VCInstallDir)atlmfc\include;$(WindowsSDK_IncludePath);</IncludePath>
+    <IncludePath>$(IncludePath);$(UniversalCRT_IncludePath);$(SolutionDir)..\..\lib;$(SolutionDir)..\..\programs;$(VCInstallDir)include;$(VCInstallDir)atlmfc\include;$(WindowsSDK_IncludePath);</IncludePath>
     <RunCodeAnalysis>true</RunCodeAnalysis>
   </PropertyGroup>
   <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">
     <ClCompile>
       <PrecompiledHeader/>
       <WarningLevel>Level4</WarningLevel>
       <Optimization>Disabled</Optimization>
@@ -148,16 +148,20 @@
       <SubSystem>Console</SubSystem>
       <GenerateDebugInformation>true</GenerateDebugInformation>
       <EnableCOMDATFolding>true</EnableCOMDATFolding>
       <OptimizeReferences>true</OptimizeReferences>
     </Link>
   </ItemDefinitionGroup>
   <ItemGroup>
-    <ClCompile Include="..\..\..\programs\datagen.c"/>
-    <ClCompile Include="..\..\..\tests\datagencli.c"/>
+    <ClCompile Include="..\..\..\lib\lz4.c"/>
+    <ClCompile Include="..\..\..\lib\lz4hc.c"/>
+    <ClCompile Include="..\..\..\lib\xxhash.c"/>
+    <ClCompile Include="..\..\..\tests\fuzzer.c"/>
   </ItemGroup>
   <ItemGroup>
-    <ClInclude Include="..\..\..\programs\datagen.h"/>
+    <ClInclude Include="..\..\..\lib\lz4.h"/>
+    <ClInclude Include="..\..\..\lib\lz4hc.h"/>
+    <ClInclude Include="..\..\..\lib\xxhash.h"/>
   </ItemGroup>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.targets"/>
   <ImportGroup Label="ExtensionTargets"/>
 </Project>
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2022/frametest/frametest.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2022/frametest/frametest.vcxproj`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2022/fullbench/fullbench.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2022/liblz4-dll/liblz4-dll.vcxproj`

 * *Files 8% similar despite different names*

#### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2022/fullbench/fullbench.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2022/liblz4-dll/liblz4-dll.vcxproj`

```diff
@@ -15,42 +15,43 @@
     </ProjectConfiguration>
     <ProjectConfiguration Include="Release|x64">
       <Configuration>Release</Configuration>
       <Platform>x64</Platform>
     </ProjectConfiguration>
   </ItemGroup>
   <PropertyGroup Label="Globals">
-    <ProjectGuid>{6A4DF4EF-C77F-43C6-8901-DDCD20879E4E}</ProjectGuid>
+    <ProjectGuid>{9800039D-4AAA-43A4-BB78-FEF6F4836927}</ProjectGuid>
     <Keyword>Win32Proj</Keyword>
-    <RootNamespace>fullbench</RootNamespace>
+    <RootNamespace>liblz4-dll</RootNamespace>
     <OutDir>$(SolutionDir)bin\$(Platform)_$(Configuration)\</OutDir>
     <IntDir>$(SolutionDir)bin\obj\$(RootNamespace)_$(Platform)_$(Configuration)\</IntDir>
+    <ProjectName>liblz4-dll</ProjectName>
   </PropertyGroup>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.Default.props"/>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'" Label="Configuration">
-    <ConfigurationType>Application</ConfigurationType>
+    <ConfigurationType>DynamicLibrary</ConfigurationType>
     <UseDebugLibraries>true</UseDebugLibraries>
     <CharacterSet>Unicode</CharacterSet>
     <PlatformToolset>v143</PlatformToolset>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'" Label="Configuration">
-    <ConfigurationType>Application</ConfigurationType>
+    <ConfigurationType>DynamicLibrary</ConfigurationType>
     <UseDebugLibraries>true</UseDebugLibraries>
     <CharacterSet>Unicode</CharacterSet>
     <PlatformToolset>v143</PlatformToolset>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'" Label="Configuration">
-    <ConfigurationType>Application</ConfigurationType>
+    <ConfigurationType>DynamicLibrary</ConfigurationType>
     <UseDebugLibraries>false</UseDebugLibraries>
     <WholeProgramOptimization>true</WholeProgramOptimization>
     <CharacterSet>Unicode</CharacterSet>
     <PlatformToolset>v143</PlatformToolset>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'" Label="Configuration">
-    <ConfigurationType>Application</ConfigurationType>
+    <ConfigurationType>DynamicLibrary</ConfigurationType>
     <UseDebugLibraries>false</UseDebugLibraries>
     <WholeProgramOptimization>true</WholeProgramOptimization>
     <CharacterSet>Unicode</CharacterSet>
     <PlatformToolset>v143</PlatformToolset>
   </PropertyGroup>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.props"/>
   <ImportGroup Label="ExtensionSettings"/>
@@ -65,106 +66,108 @@
   </ImportGroup>
   <ImportGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'" Label="PropertySheets">
     <Import Project="$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props" Condition="exists('$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props')" Label="LocalAppDataPlatform"/>
   </ImportGroup>
   <PropertyGroup Label="UserMacros"/>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">
     <LinkIncremental>true</LinkIncremental>
-    <IncludePath>$(IncludePath);$(UniversalCRT_IncludePath);$(SolutionDir)..\..\lib;$(SolutionDir)..\..\programs;$(VCInstallDir)include;$(VCInstallDir)atlmfc\include;$(WindowsSDK_IncludePath);</IncludePath>
+    <TargetName>liblz4</TargetName>
+    <IncludePath>$(IncludePath);$(UniversalCRT_IncludePath);$(SolutionDir)..\..\lib;$(VCInstallDir)include;$(VCInstallDir)atlmfc\include;$(WindowsSDK_IncludePath);</IncludePath>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'">
     <LinkIncremental>true</LinkIncremental>
-    <IncludePath>$(IncludePath);$(UniversalCRT_IncludePath);$(SolutionDir)..\..\lib;$(SolutionDir)..\..\programs;$(VCInstallDir)include;$(VCInstallDir)atlmfc\include;$(WindowsSDK_IncludePath);</IncludePath>
+    <TargetName>liblz4</TargetName>
+    <IncludePath>$(IncludePath);$(UniversalCRT_IncludePath);$(SolutionDir)..\..\lib;$(VCInstallDir)include;$(VCInstallDir)atlmfc\include;$(WindowsSDK_IncludePath);</IncludePath>
     <RunCodeAnalysis>true</RunCodeAnalysis>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'">
     <LinkIncremental>false</LinkIncremental>
-    <IncludePath>$(IncludePath);$(UniversalCRT_IncludePath);$(SolutionDir)..\..\lib;$(SolutionDir)..\..\programs;$(VCInstallDir)include;$(VCInstallDir)atlmfc\include;$(WindowsSDK_IncludePath);</IncludePath>
+    <TargetName>liblz4</TargetName>
+    <IncludePath>$(IncludePath);$(UniversalCRT_IncludePath);$(SolutionDir)..\..\lib;$(VCInstallDir)include;$(VCInstallDir)atlmfc\include;$(WindowsSDK_IncludePath);</IncludePath>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'">
     <LinkIncremental>false</LinkIncremental>
-    <IncludePath>$(IncludePath);$(UniversalCRT_IncludePath);$(SolutionDir)..\..\lib;$(SolutionDir)..\..\programs;$(VCInstallDir)include;$(VCInstallDir)atlmfc\include;$(WindowsSDK_IncludePath);</IncludePath>
+    <TargetName>liblz4</TargetName>
+    <IncludePath>$(IncludePath);$(UniversalCRT_IncludePath);$(SolutionDir)..\..\lib;$(VCInstallDir)include;$(VCInstallDir)atlmfc\include;$(WindowsSDK_IncludePath);</IncludePath>
     <RunCodeAnalysis>true</RunCodeAnalysis>
   </PropertyGroup>
   <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">
     <ClCompile>
       <PrecompiledHeader/>
       <WarningLevel>Level4</WarningLevel>
       <Optimization>Disabled</Optimization>
-      <PreprocessorDefinitions>WIN32;_DEBUG;_CONSOLE;%(PreprocessorDefinitions)</PreprocessorDefinitions>
+      <PreprocessorDefinitions>WIN32;_DEBUG;LZ4_DLL_EXPORT=1;%(PreprocessorDefinitions)</PreprocessorDefinitions>
       <TreatWarningAsError>true</TreatWarningAsError>
       <EnablePREfast>false</EnablePREfast>
     </ClCompile>
     <Link>
-      <SubSystem>Console</SubSystem>
       <GenerateDebugInformation>true</GenerateDebugInformation>
     </Link>
   </ItemDefinitionGroup>
   <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'">
     <ClCompile>
       <PrecompiledHeader/>
       <WarningLevel>Level4</WarningLevel>
       <Optimization>Disabled</Optimization>
-      <PreprocessorDefinitions>WIN32;_DEBUG;_CONSOLE;%(PreprocessorDefinitions)</PreprocessorDefinitions>
+      <PreprocessorDefinitions>WIN32;_DEBUG;LZ4_DLL_EXPORT=1;%(PreprocessorDefinitions)</PreprocessorDefinitions>
       <TreatWarningAsError>true</TreatWarningAsError>
       <EnablePREfast>true</EnablePREfast>
       <AdditionalOptions>/analyze:stacksize295252 %(AdditionalOptions)</AdditionalOptions>
     </ClCompile>
     <Link>
-      <SubSystem>Console</SubSystem>
       <GenerateDebugInformation>true</GenerateDebugInformation>
     </Link>
   </ItemDefinitionGroup>
   <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'">
     <ClCompile>
       <WarningLevel>Level4</WarningLevel>
       <PrecompiledHeader/>
       <Optimization>MaxSpeed</Optimization>
       <FunctionLevelLinking>true</FunctionLevelLinking>
       <IntrinsicFunctions>true</IntrinsicFunctions>
-      <PreprocessorDefinitions>WIN32;NDEBUG;_CONSOLE;%(PreprocessorDefinitions)</PreprocessorDefinitions>
+      <PreprocessorDefinitions>WIN32;NDEBUG;LZ4_DLL_EXPORT=1;%(PreprocessorDefinitions)</PreprocessorDefinitions>
       <TreatWarningAsError>false</TreatWarningAsError>
       <EnablePREfast>false</EnablePREfast>
     </ClCompile>
     <Link>
-      <SubSystem>Console</SubSystem>
       <GenerateDebugInformation>true</GenerateDebugInformation>
       <EnableCOMDATFolding>true</EnableCOMDATFolding>
       <OptimizeReferences>true</OptimizeReferences>
     </Link>
   </ItemDefinitionGroup>
   <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'">
     <ClCompile>
       <WarningLevel>Level4</WarningLevel>
       <PrecompiledHeader/>
       <Optimization>MaxSpeed</Optimization>
       <FunctionLevelLinking>true</FunctionLevelLinking>
       <IntrinsicFunctions>true</IntrinsicFunctions>
-      <PreprocessorDefinitions>WIN32;NDEBUG;_CONSOLE;%(PreprocessorDefinitions)</PreprocessorDefinitions>
+      <PreprocessorDefinitions>WIN32;NDEBUG;LZ4_DLL_EXPORT=1;%(PreprocessorDefinitions)</PreprocessorDefinitions>
       <TreatWarningAsError>false</TreatWarningAsError>
       <EnablePREfast>true</EnablePREfast>
       <AdditionalOptions>/analyze:stacksize295252 %(AdditionalOptions)</AdditionalOptions>
     </ClCompile>
     <Link>
-      <SubSystem>Console</SubSystem>
       <GenerateDebugInformation>true</GenerateDebugInformation>
       <EnableCOMDATFolding>true</EnableCOMDATFolding>
       <OptimizeReferences>true</OptimizeReferences>
     </Link>
   </ItemDefinitionGroup>
   <ItemGroup>
+    <ClInclude Include="..\..\..\lib\lz4.h"/>
+    <ClInclude Include="..\..\..\lib\lz4frame.h"/>
+    <ClInclude Include="..\..\..\lib\lz4frame_static.h"/>
+    <ClInclude Include="..\..\..\lib\lz4hc.h"/>
+    <ClInclude Include="..\..\..\lib\xxhash.h"/>
+  </ItemGroup>
+  <ItemGroup>
     <ClCompile Include="..\..\..\lib\lz4.c"/>
     <ClCompile Include="..\..\..\lib\lz4frame.c"/>
     <ClCompile Include="..\..\..\lib\lz4hc.c"/>
     <ClCompile Include="..\..\..\lib\xxhash.c"/>
-    <ClCompile Include="..\..\..\tests\fullbench.c"/>
   </ItemGroup>
   <ItemGroup>
-    <ClInclude Include="..\..\..\lib\lz4.h"/>
-    <ClInclude Include="..\..\..\lib\lz4frame.h"/>
-    <ClInclude Include="..\..\..\lib\lz4frame_static.h"/>
-    <ClInclude Include="..\..\..\lib\lz4hc.h"/>
-    <ClInclude Include="..\..\..\lib\xxhash.h"/>
+    <ResourceCompile Include="liblz4-dll.rc"/>
   </ItemGroup>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.targets"/>
   <ImportGroup Label="ExtensionTargets"/>
 </Project>
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2022/fullbench-dll/fullbench-dll.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2022/liblz4/liblz4.vcxproj`

 * *Files 9% similar despite different names*

#### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2022/fullbench-dll/fullbench-dll.vcxproj` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2022/liblz4/liblz4.vcxproj`

```diff
@@ -15,42 +15,42 @@
     </ProjectConfiguration>
     <ProjectConfiguration Include="Release|x64">
       <Configuration>Release</Configuration>
       <Platform>x64</Platform>
     </ProjectConfiguration>
   </ItemGroup>
   <PropertyGroup Label="Globals">
-    <ProjectGuid>{13992FD2-077E-4954-B065-A428198201A9}</ProjectGuid>
+    <ProjectGuid>{9092C5CC-3E71-41B3-BF68-4A7BDD8A5476}</ProjectGuid>
     <Keyword>Win32Proj</Keyword>
-    <RootNamespace>fullbench-dll</RootNamespace>
+    <RootNamespace>liblz4</RootNamespace>
     <OutDir>$(SolutionDir)bin\$(Platform)_$(Configuration)\</OutDir>
     <IntDir>$(SolutionDir)bin\obj\$(RootNamespace)_$(Platform)_$(Configuration)\</IntDir>
   </PropertyGroup>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.Default.props"/>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'" Label="Configuration">
-    <ConfigurationType>Application</ConfigurationType>
+    <ConfigurationType>StaticLibrary</ConfigurationType>
     <UseDebugLibraries>true</UseDebugLibraries>
     <CharacterSet>Unicode</CharacterSet>
     <PlatformToolset>v143</PlatformToolset>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'" Label="Configuration">
-    <ConfigurationType>Application</ConfigurationType>
+    <ConfigurationType>StaticLibrary</ConfigurationType>
     <UseDebugLibraries>true</UseDebugLibraries>
     <CharacterSet>Unicode</CharacterSet>
     <PlatformToolset>v143</PlatformToolset>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'" Label="Configuration">
-    <ConfigurationType>Application</ConfigurationType>
+    <ConfigurationType>StaticLibrary</ConfigurationType>
     <UseDebugLibraries>false</UseDebugLibraries>
     <WholeProgramOptimization>true</WholeProgramOptimization>
     <CharacterSet>Unicode</CharacterSet>
     <PlatformToolset>v143</PlatformToolset>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'" Label="Configuration">
-    <ConfigurationType>Application</ConfigurationType>
+    <ConfigurationType>StaticLibrary</ConfigurationType>
     <UseDebugLibraries>false</UseDebugLibraries>
     <WholeProgramOptimization>true</WholeProgramOptimization>
     <CharacterSet>Unicode</CharacterSet>
     <PlatformToolset>v143</PlatformToolset>
   </PropertyGroup>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.props"/>
   <ImportGroup Label="ExtensionSettings"/>
@@ -65,110 +65,105 @@
   </ImportGroup>
   <ImportGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'" Label="PropertySheets">
     <Import Project="$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props" Condition="exists('$(UserRootDir)\Microsoft.Cpp.$(Platform).user.props')" Label="LocalAppDataPlatform"/>
   </ImportGroup>
   <PropertyGroup Label="UserMacros"/>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">
     <LinkIncremental>true</LinkIncremental>
-    <IncludePath>$(IncludePath);$(UniversalCRT_IncludePath);$(SolutionDir)..\..\lib;$(SolutionDir)..\..\programs;$(VCInstallDir)include;$(VCInstallDir)atlmfc\include;$(WindowsSDK_IncludePath);</IncludePath>
+    <TargetName>liblz4_static</TargetName>
+    <IncludePath>$(IncludePath);$(UniversalCRT_IncludePath);$(SolutionDir)..\..\lib;$(VCInstallDir)include;$(VCInstallDir)atlmfc\include;$(WindowsSDK_IncludePath);</IncludePath>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'">
     <LinkIncremental>true</LinkIncremental>
-    <IncludePath>$(IncludePath);$(UniversalCRT_IncludePath);$(SolutionDir)..\..\lib;$(SolutionDir)..\..\programs;$(VCInstallDir)include;$(VCInstallDir)atlmfc\include;$(WindowsSDK_IncludePath);</IncludePath>
+    <TargetName>liblz4_static</TargetName>
+    <IncludePath>$(IncludePath);$(UniversalCRT_IncludePath);$(SolutionDir)..\..\lib;$(VCInstallDir)include;$(VCInstallDir)atlmfc\include;$(WindowsSDK_IncludePath);</IncludePath>
     <RunCodeAnalysis>true</RunCodeAnalysis>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'">
     <LinkIncremental>false</LinkIncremental>
-    <IncludePath>$(IncludePath);$(UniversalCRT_IncludePath);$(SolutionDir)..\..\lib;$(SolutionDir)..\..\programs;$(VCInstallDir)include;$(VCInstallDir)atlmfc\include;$(WindowsSDK_IncludePath);</IncludePath>
+    <TargetName>liblz4_static</TargetName>
+    <IncludePath>$(IncludePath);$(UniversalCRT_IncludePath);$(SolutionDir)..\..\lib;$(VCInstallDir)include;$(VCInstallDir)atlmfc\include;$(WindowsSDK_IncludePath);</IncludePath>
   </PropertyGroup>
   <PropertyGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'">
     <LinkIncremental>false</LinkIncremental>
-    <IncludePath>$(IncludePath);$(UniversalCRT_IncludePath);$(SolutionDir)..\..\lib;$(SolutionDir)..\..\programs;$(VCInstallDir)include;$(VCInstallDir)atlmfc\include;$(WindowsSDK_IncludePath);</IncludePath>
+    <TargetName>liblz4_static</TargetName>
+    <IncludePath>$(IncludePath);$(UniversalCRT_IncludePath);$(SolutionDir)..\..\lib;$(VCInstallDir)include;$(VCInstallDir)atlmfc\include;$(WindowsSDK_IncludePath);</IncludePath>
     <RunCodeAnalysis>true</RunCodeAnalysis>
   </PropertyGroup>
   <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Debug|Win32'">
     <ClCompile>
       <PrecompiledHeader/>
       <WarningLevel>Level4</WarningLevel>
       <Optimization>Disabled</Optimization>
-      <PreprocessorDefinitions>WIN32;_DEBUG;_CONSOLE;LZ4_DLL_IMPORT=1;%(PreprocessorDefinitions)</PreprocessorDefinitions>
+      <PreprocessorDefinitions>WIN32;_DEBUG;LZ4_DLL_EXPORT=1;%(PreprocessorDefinitions)</PreprocessorDefinitions>
       <TreatWarningAsError>true</TreatWarningAsError>
       <EnablePREfast>false</EnablePREfast>
     </ClCompile>
     <Link>
-      <SubSystem>Console</SubSystem>
       <GenerateDebugInformation>true</GenerateDebugInformation>
-      <AdditionalLibraryDirectories>$(SolutionDir)bin\$(Platform)_$(Configuration);%(AdditionalLibraryDirectories)</AdditionalLibraryDirectories>
-      <AdditionalDependencies>liblz4.lib;%(AdditionalDependencies)</AdditionalDependencies>
     </Link>
   </ItemDefinitionGroup>
   <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Debug|x64'">
     <ClCompile>
       <PrecompiledHeader/>
       <WarningLevel>Level4</WarningLevel>
       <Optimization>Disabled</Optimization>
-      <PreprocessorDefinitions>WIN32;_DEBUG;_CONSOLE;LZ4_DLL_IMPORT=1;%(PreprocessorDefinitions)</PreprocessorDefinitions>
+      <PreprocessorDefinitions>WIN32;_DEBUG;LZ4_DLL_EXPORT=1;%(PreprocessorDefinitions)</PreprocessorDefinitions>
       <TreatWarningAsError>true</TreatWarningAsError>
       <EnablePREfast>true</EnablePREfast>
       <AdditionalOptions>/analyze:stacksize295252 %(AdditionalOptions)</AdditionalOptions>
     </ClCompile>
     <Link>
-      <SubSystem>Console</SubSystem>
       <GenerateDebugInformation>true</GenerateDebugInformation>
-      <AdditionalLibraryDirectories>$(SolutionDir)bin\$(Platform)_$(Configuration);%(AdditionalLibraryDirectories)</AdditionalLibraryDirectories>
-      <AdditionalDependencies>liblz4.lib;%(AdditionalDependencies)</AdditionalDependencies>
     </Link>
   </ItemDefinitionGroup>
   <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Release|Win32'">
     <ClCompile>
       <WarningLevel>Level4</WarningLevel>
       <PrecompiledHeader/>
       <Optimization>MaxSpeed</Optimization>
       <FunctionLevelLinking>true</FunctionLevelLinking>
       <IntrinsicFunctions>true</IntrinsicFunctions>
-      <PreprocessorDefinitions>WIN32;NDEBUG;_CONSOLE;LZ4_DLL_IMPORT=1;%(PreprocessorDefinitions)</PreprocessorDefinitions>
+      <PreprocessorDefinitions>WIN32;NDEBUG;LZ4_DLL_EXPORT=1;%(PreprocessorDefinitions)</PreprocessorDefinitions>
       <TreatWarningAsError>false</TreatWarningAsError>
       <EnablePREfast>false</EnablePREfast>
     </ClCompile>
     <Link>
-      <SubSystem>Console</SubSystem>
       <GenerateDebugInformation>true</GenerateDebugInformation>
       <EnableCOMDATFolding>true</EnableCOMDATFolding>
       <OptimizeReferences>true</OptimizeReferences>
-      <AdditionalLibraryDirectories>$(SolutionDir)bin\$(Platform)_$(Configuration);%(AdditionalLibraryDirectories)</AdditionalLibraryDirectories>
-      <AdditionalDependencies>liblz4.lib;%(AdditionalDependencies)</AdditionalDependencies>
     </Link>
   </ItemDefinitionGroup>
   <ItemDefinitionGroup Condition="'$(Configuration)|$(Platform)'=='Release|x64'">
     <ClCompile>
       <WarningLevel>Level4</WarningLevel>
       <PrecompiledHeader/>
       <Optimization>MaxSpeed</Optimization>
       <FunctionLevelLinking>true</FunctionLevelLinking>
       <IntrinsicFunctions>true</IntrinsicFunctions>
-      <PreprocessorDefinitions>WIN32;NDEBUG;_CONSOLE;LZ4_DLL_IMPORT=1;%(PreprocessorDefinitions)</PreprocessorDefinitions>
+      <PreprocessorDefinitions>WIN32;NDEBUG;LZ4_DLL_EXPORT=1;%(PreprocessorDefinitions)</PreprocessorDefinitions>
       <TreatWarningAsError>false</TreatWarningAsError>
       <EnablePREfast>true</EnablePREfast>
       <AdditionalOptions>/analyze:stacksize295252 %(AdditionalOptions)</AdditionalOptions>
     </ClCompile>
     <Link>
-      <SubSystem>Console</SubSystem>
       <GenerateDebugInformation>true</GenerateDebugInformation>
       <EnableCOMDATFolding>true</EnableCOMDATFolding>
       <OptimizeReferences>true</OptimizeReferences>
-      <AdditionalLibraryDirectories>$(SolutionDir)bin\$(Platform)_$(Configuration);%(AdditionalLibraryDirectories)</AdditionalLibraryDirectories>
-      <AdditionalDependencies>liblz4.lib;%(AdditionalDependencies)</AdditionalDependencies>
     </Link>
   </ItemDefinitionGroup>
   <ItemGroup>
-    <ClCompile Include="..\..\..\lib\xxhash.c"/>
-    <ClCompile Include="..\..\..\tests\fullbench.c"/>
-  </ItemGroup>
-  <ItemGroup>
     <ClInclude Include="..\..\..\lib\lz4.h"/>
     <ClInclude Include="..\..\..\lib\lz4frame.h"/>
+    <ClInclude Include="..\..\..\lib\lz4frame_static.h"/>
     <ClInclude Include="..\..\..\lib\lz4hc.h"/>
     <ClInclude Include="..\..\..\lib\xxhash.h"/>
   </ItemGroup>
+  <ItemGroup>
+    <ClCompile Include="..\..\..\lib\lz4.c"/>
+    <ClCompile Include="..\..\..\lib\lz4frame.c"/>
+    <ClCompile Include="..\..\..\lib\lz4hc.c"/>
+    <ClCompile Include="..\..\..\lib\xxhash.c"/>
+  </ItemGroup>
   <Import Project="$(VCTargetsPath)\Microsoft.Cpp.targets"/>
   <ImportGroup Label="ExtensionTargets"/>
 </Project>
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2022/liblz4-dll/liblz4-dll.rc` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2022/liblz4-dll/liblz4-dll.rc`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2022/lz4/lz4.rc` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2022/lz4/lz4.rc`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/lz4/visual/VS2022/lz4.sln` & `gvsbuild-2024.5.0/gvsbuild/patches/lz4/visual/VS2022/lz4.sln`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/nghttp2/0001-Define-ssize_t-if-not-defined.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/nghttp2/0001-Define-ssize_t-if-not-defined.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/openssl-base/certdata.txt` & `gvsbuild-2024.5.0/gvsbuild/patches/openssl-base/certdata.txt`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/openssl-base/mk-ca-bundle.pl` & `gvsbuild-2024.5.0/gvsbuild/patches/openssl-base/mk-ca-bundle.pl`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/pango/002-fix-wrong-usage-gweakref.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/pango/002-fix-wrong-usage-gweakref.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/pango/003-remove-extra-hb-face-font.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/pango/003-remove-extra-hb-face-font.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/pcre2/LICENSE.build` & `gvsbuild-2024.5.0/gvsbuild/patches/pcre2/LICENSE.build`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/pcre2/meson.build` & `gvsbuild-2024.5.0/gvsbuild/patches/pcre2/meson.build`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/pkgconf/0001-libpkgconf-add-defines-to-unbreak-build-with-VS2013.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/pkgconf/0001-libpkgconf-add-defines-to-unbreak-build-with-VS2013.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/protobuf-c/0001-Declare-variables-at-the-beginning-of-the-block.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/protobuf-c/0001-Declare-variables-at-the-beginning-of-the-block.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/protobuf-c/0001-Do-not-build-tests.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/protobuf-c/0001-Do-not-build-tests.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/pygobject/001-pygobject-py38-load-dll.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/pygobject/001-pygobject-py38-load-dll.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/stack.props` & `gvsbuild-2024.5.0/gvsbuild/patches/stack.props`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/win-iconv/COPYING` & `gvsbuild-2024.5.0/gvsbuild/patches/win-iconv/COPYING`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/x264/build/build.sh` & `gvsbuild-2024.5.0/gvsbuild/patches/x264/build/build.sh`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/patches/x264/x264-0001-Prevent-mb_info_free-to-be-called-before-all-threads.patch` & `gvsbuild-2024.5.0/gvsbuild/patches/x264/x264-0001-Prevent-mb_info_free-to-be-called-before-all-threads.patch`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/__init__.py` & `gvsbuild-2024.5.0/gvsbuild/projects/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,22 +45,22 @@
 from gvsbuild.projects.json_glib import JsonGLib
 from gvsbuild.projects.jsonc import Jsonc
 from gvsbuild.projects.leveldb import LevelDB
 from gvsbuild.projects.lgi import Lgi
 from gvsbuild.projects.libadwaita import Libadwaita
 from gvsbuild.projects.libarchive import Libarchive
 from gvsbuild.projects.libcbor import Libcbor
-from gvsbuild.projects.libcroco import Libcroco
 from gvsbuild.projects.libcurl import Libcurl
 from gvsbuild.projects.libepoxy import Libepoxy
 from gvsbuild.projects.libfido2 import Libfido2
 from gvsbuild.projects.libffi import Libffi
 from gvsbuild.projects.libgxps import Libgxps
 from gvsbuild.projects.libjpeg_turbo import LibjpegTurbo
 from gvsbuild.projects.libmicrohttpd import Libmicrohttpd
+from gvsbuild.projects.libpanel import Libpanel
 from gvsbuild.projects.libpng import Libpng
 from gvsbuild.projects.libpsl import Libpsl
 from gvsbuild.projects.librsvg import Librsvg
 from gvsbuild.projects.libsigcplusplus import Libsigcplusplus
 from gvsbuild.projects.libsoup import Libsoup2, Libsoup3
 from gvsbuild.projects.libssh import Libssh, Libssh2
 from gvsbuild.projects.libtiff import Libtiff4
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/adwaita_icon_theme.py` & `gvsbuild-2024.5.0/gvsbuild/projects/adwaita_icon_theme.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/atk.py` & `gvsbuild-2024.5.0/gvsbuild/projects/atk.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/boringssl.py` & `gvsbuild-2024.5.0/gvsbuild/projects/boringssl.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/cairo.py` & `gvsbuild-2024.5.0/gvsbuild/projects/cairo.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,13 +27,14 @@
             version="1.18.0",
             lastversion_even=True,
             archive_url="https://gitlab.freedesktop.org/cairo/cairo/-/archive/{version}/cairo-{version}.tar.gz",
             hash="39a78afdc33a435c0f2ab53a5ec2a693c3c9b6d2ec9783ceecb2b94d54d942b0",
             dependencies=["freetype", "glib", "pixman", "libpng"],
             patches=["0001-fix-alloca-unresolved.patch"],
         )
+        self.add_param("-Ddwrite=enabled")
         self.add_param("-Dfreetype=enabled")
         self.add_param("-Dfontconfig=disabled")
 
     def build(self):
         Meson.build(self)
         self.install(r".\COPYING share\doc\cairo")
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/cairomm.py` & `gvsbuild-2024.5.0/gvsbuild/projects/cairomm.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/check_libs.py` & `gvsbuild-2024.5.0/gvsbuild/projects/check_libs.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/clutter.py` & `gvsbuild-2024.5.0/gvsbuild/projects/clutter.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/cogl.py` & `gvsbuild-2024.5.0/gvsbuild/projects/cogl.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/cyrus_sasl.py` & `gvsbuild-2024.5.0/gvsbuild/projects/cyrus_sasl.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/dev_shell.py` & `gvsbuild-2024.5.0/gvsbuild/projects/dev_shell.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/emeus.py` & `gvsbuild-2024.5.0/gvsbuild/projects/emeus.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/enchant.py` & `gvsbuild-2024.5.0/gvsbuild/projects/enchant.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/expat.py` & `gvsbuild-2024.5.0/gvsbuild/projects/expat.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/ffmpeg.py` & `gvsbuild-2024.5.0/gvsbuild/projects/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/freerdp.py` & `gvsbuild-2024.5.0/gvsbuild/projects/freerdp.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/freetype.py` & `gvsbuild-2024.5.0/gvsbuild/projects/freetype.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/fribidi.py` & `gvsbuild-2024.5.0/gvsbuild/projects/fribidi.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,16 +33,16 @@
 
 @project_add
 class Fribidi(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
             "fribidi",
-            version="1.0.13",
+            version="1.0.14",
             archive_url="https://github.com/fribidi/fribidi/releases/download/v{version}/fribidi-{version}.tar.xz",
-            hash="7fa16c80c81bd622f7b198d31356da139cc318a63fc7761217af4130903f54a2",
+            hash="76ae204a7027652ac3981b9fa5817c083ba23114340284c58e756b259cd2259a",
             dependencies=["ninja", "meson"],
         )
 
     def build(self):
         Meson.build(self, meson_params="-Ddocs=false")
         self.install(r".\COPYING share\doc\fribidi")
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/gdk_pixbuf.py` & `gvsbuild-2024.5.0/gvsbuild/projects/gdk_pixbuf.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 
 @project_add
 class GdkPixbuf(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
             "gdk-pixbuf",
-            version="2.42.10",
+            version="2.42.11",
             repository="https://gitlab.gnome.org/GNOME/gdk-pixbuf",
             archive_url="https://download.gnome.org/sources/gdk-pixbuf/{major}.{minor}/gdk-pixbuf-{version}.tar.xz",
-            hash="ee9b6c75d13ba096907a2e3c6b27b61bcd17f5c7ebeab5a5b439d2f2e39fe44b",
+            hash="49dcb402388708647e8c321d56b6fb30f21e51e515d0c5a942268d23052a2f00",
             dependencies=[
                 "ninja",
                 "pkgconf",
                 "meson",
                 "libtiff-4",
                 "libjpeg-turbo",
                 "glib",
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/gettext.py` & `gvsbuild-2024.5.0/gvsbuild/projects/gettext.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/glib.py` & `gvsbuild-2024.5.0/gvsbuild/projects/glib.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,14 +99,17 @@
                 "pkgconf",
                 "ninja",
                 "meson",
                 "glib",
                 "openssl",
                 "gsettings-desktop-schemas",
             ],
+            patches=[
+                "add-null-check-in-complete_handshake.patch",
+            ],
         )
 
     def build(self):
         Meson.build(
             self, meson_params="-Dgnutls=disabled -Dopenssl=enabled -Dlibproxy=disabled"
         )
         self.install(r".\COPYING share\doc\glib-networking")
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/glibmm.py` & `gvsbuild-2024.5.0/gvsbuild/projects/glibmm.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/gobject_introspection.py` & `gvsbuild-2024.5.0/gvsbuild/projects/gobject_introspection.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/gperf.py` & `gvsbuild-2024.5.0/gvsbuild/projects/gperf.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/graphene.py` & `gvsbuild-2024.5.0/gvsbuild/projects/graphene.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/gsettings_desktop_schemas.py` & `gvsbuild-2024.5.0/gvsbuild/projects/gsettings_desktop_schemas.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/gstreamer.py` & `gvsbuild-2024.5.0/gvsbuild/projects/gstreamer.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,18 +36,18 @@
 @project_add
 class GStreamer(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
             "gstreamer",
             repository="https://gitlab.freedesktop.org/gstreamer/gstreamer",
-            version="1.24.1",
+            version="1.24.3",
             lastversion_even=True,
             archive_url="https://gstreamer.freedesktop.org/src/gstreamer/gstreamer-{version}.tar.xz",
-            hash="88fc3629a8cacf7955d8671b2ae867d4a52a07b6948daa25b67feed22f8055ef",
+            hash="1225ef4a329fae1cadc5ec727dab249ad567e8072879493561ceb91ed34aa414",
             dependencies=["meson", "ninja", "glib", "orc"],
         )
 
         if self.opts.enable_gi:
             self.add_dependency("gobject-introspection")
             enable_gi = "enabled"
         else:
@@ -86,18 +86,18 @@
 @project_add
 class GstPluginsBase(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
             "gst-plugins-base",
             repository="https://gitlab.freedesktop.org/gstreamer/gstreamer",
-            version="1.24.1",
+            version="1.24.3",
             lastversion_even=True,
             archive_url="https://gstreamer.freedesktop.org/src/gst-plugins-base/gst-plugins-base-{version}.tar.xz",
-            hash="884045d1d7c5d6bb8605e45c7ee0e9f1341888e81c2b7c42dff52bb98ede8ec3",
+            hash="f1094397eaa7932f06e57ebbb075aa33aa2c76e4b75630a16b02c8d4af46832e",
             dependencies=[
                 "meson",
                 "ninja",
                 "gstreamer",
                 "opus",
                 "ogg",
             ],
@@ -123,18 +123,18 @@
 @project_add
 class GstPluginsGood(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
             "gst-plugins-good",
             repository="https://gitlab.freedesktop.org/gstreamer/gstreamer",
-            version="1.24.1",
+            version="1.24.3",
             lastversion_even=True,
             archive_url="https://gstreamer.freedesktop.org/src/gst-plugins-good/gst-plugins-good-{version}.tar.xz",
-            hash="c02ba5583863e0bd9e265e5e4a27a03a3c473eb9ec1c10b07238f7176d9368a2",
+            hash="150f914e61dc05600b68b88ca103c7cc227130158e389ea9ea159f4050a2ebb0",
             dependencies=[
                 "meson",
                 "ninja",
                 "gst-plugins-base",
                 "libvpx",
             ],
         )
@@ -147,18 +147,18 @@
 @project_add
 class GstPluginsBad(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
             "gst-plugins-bad",
             repository="https://gitlab.freedesktop.org/gstreamer/gstreamer",
-            version="1.24.1",
+            version="1.24.3",
             lastversion_even=True,
             archive_url="https://gstreamer.freedesktop.org/src/gst-plugins-bad/gst-plugins-bad-{version}.tar.xz",
-            hash="f1a183966ea9136a00f159ee42db4d1d106abef022d1b49e63fba2fcbe50c8f8",
+            hash="e90f26c7dc9c76f4aa599b758cfd6d8c10d6a0b9cb265ba2c3c9bdf3888558f8",
             dependencies=["meson", "ninja", "gst-plugins-base"],
             patches=[
                 "wasapisink-reduce-buffer-latency.patch",
             ],
         )
         self.add_param("-Dcurl=disabled")
         self.add_param("-Dcurl-ssh2=disabled")
@@ -179,18 +179,18 @@
 @project_add
 class GstPluginsUgly(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
             "gst-plugins-ugly",
             repository="https://gitlab.freedesktop.org/gstreamer/gstreamer",
-            version="1.24.1",
+            version="1.24.3",
             lastversion_even=True,
             archive_url="https://gstreamer.freedesktop.org/src/gst-plugins-ugly/gst-plugins-ugly-{version}.tar.xz",
-            hash="6462d36ce64b74203a8b302c109e762b1dd404a6235dfec3c4255106b7b86976",
+            hash="4c951341c4c648630b6fe1234ec113d81dd2d248529bf2b5478e0ad077c80ed3",
             dependencies=["meson", "ninja", "gst-plugins-base"],
         )
 
     def build(self):
         Meson.build(self)
         self.install(r".\COPYING share\doc\gst-plugins-ugly")
 
@@ -198,18 +198,18 @@
 @project_add
 class GstDevTools(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
             "gst-devtools",
             repository="https://gitlab.freedesktop.org/gstreamer/gstreamer",
-            version="1.24.1",
+            version="1.24.3",
             lastversion_even=True,
             archive_url="https://gstreamer.freedesktop.org/src/gst-devtools/gst-devtools-{version}.tar.xz",
-            hash="49ae0347f463641b094ebbc63350936a29e8a063ca90cd0b44a49e0c2b2129d2",
+            hash="b91114a2fd958f42acf441186e87e2bec93538ef35a9f8248111197360ffb237",
             dependencies=["meson", "ninja", "json-glib"],
         )
 
         if self.opts.enable_gi:
             self.add_dependency("gobject-introspection")
             enable_gi = "enabled"
         else:
@@ -225,20 +225,17 @@
 @project_add
 class GstPython(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
             "gst-python",
             repository="https://gitlab.freedesktop.org/gstreamer/gstreamer",
-            version="1.24.1",
+            version="1.24.3",
             lastversion_even=True,
             archive_url="https://gstreamer.freedesktop.org/src/gst-python/gst-python-{version}.tar.xz",
-            hash="5a23732783edae03cc2164c6927c05477bbb3a7008f8939291b855473781a651",
+            hash="ecdb3e2ba94ea2c82b93a8c715d5a7e04f9726a8838c0a6b17694928fd1e8595",
             dependencies=["meson", "ninja", "pygobject", "gst-plugins-base"],
-            patches=[
-                "001-fix-instsoname-not-found.patch",
-            ],
         )
 
     def build(self):
         Meson.build(self)
         self.install(r".\COPYING share\doc\gst-python")
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/gtk.py` & `gvsbuild-2024.5.0/gvsbuild/projects/gtk.py`

 * *Files 12% similar despite different names*

```diff
@@ -118,20 +118,20 @@
 @project_add
 class Gtk4(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
             "gtk4",
             prj_dir="gtk4",
-            version="4.14.2",
+            version="4.14.4",
             lastversion_major=4,
             lastversion_even=True,
             repository="https://gitlab.gnome.org/GNOME/gtk",
             archive_url="https://download.gnome.org/sources/gtk/{major}.{minor}/gtk-{version}.tar.xz",
-            hash="22604cef2898a79e5f2143bb7aee2b7d1fa2eb946989a9d1338ecf9c8ae0e072",
+            hash="443518b97e8348f9f6430ac435b1010f9a6c5207f4dc6a7cd5d24e3820cee633",
             dependencies=[
                 "gdk-pixbuf",
                 "pango",
                 "libepoxy",
                 "graphene",
                 "cairo",
                 "harfbuzz",
@@ -150,9 +150,8 @@
         self.add_param("-Dbuild-demos=false")
         self.add_param("-Dbuild-examples=false")
         self.add_param("-Dmedia-gstreamer=disabled")
         self.add_param("-Dvulkan=disabled")
 
     def build(self):
         Meson.build(self)
-
         self.install(r".\COPYING share\doc\gtk4")
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/gtkmm.py` & `gvsbuild-2024.5.0/gvsbuild/projects/gtkmm.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/gtksourceview.py` & `gvsbuild-2024.5.0/gvsbuild/projects/gtksourceview.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/harfbuzz.py` & `gvsbuild-2024.5.0/gvsbuild/projects/harfbuzz.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,10 +32,13 @@
 
         if Project.opts.enable_gi:
             self.add_dependency("gobject-introspection")
             self.add_param("-Dintrospection=enabled")
         else:
             self.add_param("-Dintrospection=disabled")
 
+        self.add_param("-Ddirectwrite=enabled")
+        self.add_param("-Dgdi=enabled")
+
     def build(self):
         Meson.build(self)
         self.install(r".\COPYING share\doc\harfbuzz")
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/hello_world.py` & `gvsbuild-2024.5.0/gvsbuild/projects/hello_world.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/hicolor_icon_theme.py` & `gvsbuild-2024.5.0/gvsbuild/projects/hicolor_icon_theme.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/icu.py` & `gvsbuild-2024.5.0/gvsbuild/projects/icu.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/json_glib.py` & `gvsbuild-2024.5.0/gvsbuild/projects/json_glib.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/jsonc.py` & `gvsbuild-2024.5.0/gvsbuild/projects/jsonc.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/leveldb.py` & `gvsbuild-2024.5.0/gvsbuild/projects/leveldb.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/lgi.py` & `gvsbuild-2024.5.0/gvsbuild/projects/lgi.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/libadwaita.py` & `gvsbuild-2024.5.0/gvsbuild/projects/libadwaita.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/libarchive.py` & `gvsbuild-2024.5.0/gvsbuild/projects/libarchive.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 
 @project_add
 class Libarchive(Tarball, CmakeProject):
     def __init__(self):
         Project.__init__(
             self,
             "libarchive",
-            version="3.7.2",
+            version="3.7.4",
             archive_url="https://libarchive.org/downloads/libarchive-{version}.tar.xz",
-            hash="04357661e6717b6941682cde02ad741ae4819c67a260593dfb2431861b251acb",
+            hash="f887755c434a736a609cbd28d87ddbfbe9d6a3bb5b703c22c02f6af80a802735",
             dependencies=[
                 "cmake",
                 "ninja",
                 "win-iconv",
                 "zlib",
                 "lz4",
                 "openssl",
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/libcbor.py` & `gvsbuild-2024.5.0/gvsbuild/projects/libcbor.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/libcroco.py` & `gvsbuild-2024.5.0/gvsbuild/projects/lmdb.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,28 +9,32 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program; if not, see <http://www.gnu.org/licenses/>.
 
-from gvsbuild.utils.base_expanders import Tarball
+from gvsbuild.utils.base_builders import Meson
+from gvsbuild.utils.base_expanders import GitRepo
 from gvsbuild.utils.base_project import Project, project_add
 
 
 @project_add
-class Libcroco(Tarball, Project):
+class Lmdb(GitRepo, Meson):
     def __init__(self):
         Project.__init__(
             self,
-            "libcroco",
-            version="0.6.13",
-            lastversion_even=True,
-            repository="https://gitlab.gnome.org/Archive/libcroco",
-            archive_url="https://download.gnome.org/sources/libcroco/{major}.{minor}/libcroco-{version}.tar.xz",
-            hash="767ec234ae7aa684695b3a735548224888132e063f92db585759b422570621d4",
-            dependencies=["glib", "libxml2"],
+            "lmdb",
+            repo_url="https://github.com/wingtk/lmdb.git",
+            fetch_submodules=False,
+            tag="mdb.RE/0.9-meson",
+            dependencies=[
+                "ninja",
+                "meson",
+            ],
         )
 
     def build(self):
-        self.exec_msbuild_gen(r"win32", "libcroco.sln")
-        self.install(r".\COPYING share\doc\libcroco")
+        self.push_location(r".\libraries\liblmdb")
+        Meson.build(self)
+        self.install(r"LICENSE share\doc\lmdb")
+        self.pop_location()
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/libcurl.py` & `gvsbuild-2024.5.0/gvsbuild/projects/libcurl.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/libepoxy.py` & `gvsbuild-2024.5.0/gvsbuild/projects/libepoxy.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/libffi.py` & `gvsbuild-2024.5.0/gvsbuild/projects/libffi.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/libfido2.py` & `gvsbuild-2024.5.0/gvsbuild/projects/libfido2.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/libgxps.py` & `gvsbuild-2024.5.0/gvsbuild/projects/libgxps.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/libjpeg_turbo.py` & `gvsbuild-2024.5.0/gvsbuild/projects/libjpeg_turbo.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/libmicrohttpd.py` & `gvsbuild-2024.5.0/gvsbuild/projects/libmicrohttpd.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/libpng.py` & `gvsbuild-2024.5.0/gvsbuild/projects/libpng.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/libpsl.py` & `gvsbuild-2024.5.0/gvsbuild/projects/libpsl.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/librsvg.py` & `gvsbuild-2024.5.0/gvsbuild/projects/librsvg.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
             hash="d7c444a926406b59790be0deae196e18ed26059da573fa1aa9ec9ca7658a559c",
             dependencies=[
                 "cargo",
                 "cairo",
                 "pango",
                 "gdk-pixbuf",
                 "libxml2",
+                "freetype",
             ],
         )
         if Project.opts.enable_gi:
             self.add_dependency("gobject-introspection")
 
     def build(self):
         self.builder.mod_env("INCLUDE", "include\\cairo", add_gtk=True)
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/libsigcplusplus.py` & `gvsbuild-2024.5.0/gvsbuild/projects/libsigcplusplus.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/libsoup.py` & `gvsbuild-2024.5.0/gvsbuild/projects/libsoup.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/libssh.py` & `gvsbuild-2024.5.0/gvsbuild/projects/libssh.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/libtiff.py` & `gvsbuild-2024.5.0/gvsbuild/projects/libtiff.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/libuv.py` & `gvsbuild-2024.5.0/gvsbuild/projects/libuv.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/libvorbis.py` & `gvsbuild-2024.5.0/gvsbuild/projects/libvorbis.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/libvpx.py` & `gvsbuild-2024.5.0/gvsbuild/projects/libvpx.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/libxml2.py` & `gvsbuild-2024.5.0/gvsbuild/projects/libxml2.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/libyuv.py` & `gvsbuild-2024.5.0/gvsbuild/projects/libyuv.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/libzip.py` & `gvsbuild-2024.5.0/gvsbuild/projects/libzip.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/lmdb.py` & `gvsbuild-2024.5.0/gvsbuild/projects/nghttp2.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,32 +9,33 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program; if not, see <http://www.gnu.org/licenses/>.
 
-from gvsbuild.utils.base_builders import Meson
-from gvsbuild.utils.base_expanders import GitRepo
+from gvsbuild.utils.base_builders import CmakeProject
+from gvsbuild.utils.base_expanders import Tarball
 from gvsbuild.utils.base_project import Project, project_add
 
 
 @project_add
-class Lmdb(GitRepo, Meson):
+class Nghttp2(Tarball, CmakeProject):
     def __init__(self):
         Project.__init__(
             self,
-            "lmdb",
-            repo_url="https://github.com/wingtk/lmdb.git",
-            fetch_submodules=False,
-            tag="mdb.RE/0.9-meson",
+            "nghttp2",
+            version="1.59.0",
+            archive_url="https://github.com/nghttp2/nghttp2/releases/download/v{version}/nghttp2-{version}.tar.xz",
+            hash="fdc9bd71f5cf8d3fdfb63066b89364c10eb2fdeab55f3c6755cd7917b2ec4ffb",
             dependencies=[
+                "cmake",
+                "zlib",
                 "ninja",
-                "meson",
             ],
+            patches=["0001-Define-ssize_t-if-not-defined.patch"],
         )
 
     def build(self):
-        self.push_location(r".\libraries\liblmdb")
-        Meson.build(self)
-        self.install(r"LICENSE share\doc\lmdb")
-        self.pop_location()
+        CmakeProject.build(self, use_ninja=True)
+
+        self.install(r".\COPYING share\doc\nghttp2")
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/luajit.py` & `gvsbuild-2024.5.0/gvsbuild/projects/luajit.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/lz4.py` & `gvsbuild-2024.5.0/gvsbuild/projects/lz4.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/mit_kerberos.py` & `gvsbuild-2024.5.0/gvsbuild/projects/mit_kerberos.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/nghttp2.py` & `gvsbuild-2024.5.0/gvsbuild/projects/openh264.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,33 +9,32 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program; if not, see <http://www.gnu.org/licenses/>.
 
-from gvsbuild.utils.base_builders import CmakeProject
+from gvsbuild.utils.base_builders import Meson
 from gvsbuild.utils.base_expanders import Tarball
 from gvsbuild.utils.base_project import Project, project_add
 
 
 @project_add
-class Nghttp2(Tarball, CmakeProject):
+class OpenH264(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
-            "nghttp2",
-            version="1.59.0",
-            archive_url="https://github.com/nghttp2/nghttp2/releases/download/v{version}/nghttp2-{version}.tar.xz",
-            hash="fdc9bd71f5cf8d3fdfb63066b89364c10eb2fdeab55f3c6755cd7917b2ec4ffb",
+            "openh264",
+            version="2.4.1",
+            archive_url="https://github.com/cisco/openh264/archive/refs/tags/v{version}.tar.gz",
+            archive_filename="openh264-{version}.tar.gz",
+            hash="8ffbe944e74043d0d3fb53d4a2a14c94de71f58dbea6a06d0dc92369542958ea",
             dependencies=[
-                "cmake",
-                "zlib",
                 "ninja",
+                "meson",
+                "nasm",
             ],
-            patches=["0001-Define-ssize_t-if-not-defined.patch"],
         )
 
     def build(self):
-        CmakeProject.build(self, use_ninja=True)
-
-        self.install(r".\COPYING share\doc\nghttp2")
+        Meson.build(self)
+        self.install(r"LICENSE share\doc\openh264")
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/ogg.py` & `gvsbuild-2024.5.0/gvsbuild/projects/ogg.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/openh264.py` & `gvsbuild-2024.5.0/gvsbuild/projects/pixman.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,26 +15,28 @@
 
 from gvsbuild.utils.base_builders import Meson
 from gvsbuild.utils.base_expanders import Tarball
 from gvsbuild.utils.base_project import Project, project_add
 
 
 @project_add
-class OpenH264(Tarball, Meson):
+class Pixman(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
-            "openh264",
-            version="2.4.1",
-            archive_url="https://github.com/cisco/openh264/archive/refs/tags/v{version}.tar.gz",
-            archive_filename="openh264-{version}.tar.gz",
-            hash="8ffbe944e74043d0d3fb53d4a2a14c94de71f58dbea6a06d0dc92369542958ea",
-            dependencies=[
-                "ninja",
-                "meson",
-                "nasm",
-            ],
+            "pixman",
+            repository="https://gitlab.freedesktop.org/pixman/pixman",
+            version="0.42.2",
+            lastversion_even=True,
+            archive_url="http://cairographics.org/releases/pixman-{version}.tar.gz",
+            hash="ea1480efada2fd948bc75366f7c349e1c96d3297d09a3fe62626e38e234a625e",
+            dependencies=["ninja", "meson"],
         )
 
     def build(self):
-        Meson.build(self)
-        self.install(r"LICENSE share\doc\openh264")
+        enable_mmx = "disabled" if self.builder.x64 else "enabled"
+        Meson.build(
+            self,
+            meson_params=f"-Dsse2=enabled -Dssse3=enabled -Dmmx={enable_mmx} -Dtests=disabled",
+        )
+
+        self.install(r".\COPYING share\doc\pixman")
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/openssl.py` & `gvsbuild-2024.5.0/gvsbuild/projects/openssl.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,23 +21,22 @@
 
 @project_add
 class OpenSSLBase(Tarball, Project):
     def __init__(self):
         Project.__init__(
             self,
             "openssl-base",
-            version="3.2.1",
+            version="3.3.0",
             archive_url="https://www.openssl.org/source/openssl-{version}.tar.gz",
-            hash="83c7329fe52c850677d75e5d0b0ca245309b97e8ecbcfdc1dfdc4ab9fac35b39",
+            hash="53e66b043322a606abf0087e7699a0e033a37fa13feb9742df35c3a33b18fb02",
             dependencies=[
                 "perl",
                 "nasm",
                 "msys2",
             ],
-            patches=["0001-crypto-providers-config.patch"],
         )
 
     def build(self):
         common_options = r"enable-fips no-comp no-docs no-ssl3 --openssldir=%(gtk_dir)s/etc/ssl --prefix=%(gtk_dir)s"
         debug_option = "debug-" if self.builder.opts.configuration == "debug" else ""
         target_option = "VC-WIN32 " if self.builder.x86 else "VC-WIN64A "
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/pango.py` & `gvsbuild-2024.5.0/gvsbuild/projects/pango.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,15 @@
                 "meson",
                 "freetype",
                 "cairo",
                 "harfbuzz",
                 "fribidi",
             ],
             patches=[
+                "001-disable-dwrite.patch",
                 "002-fix-wrong-usage-gweakref.patch",
                 "003-remove-extra-hb-face-font.patch",
             ],
         )
         if self.opts.enable_gi:
             self.add_dependency("gobject-introspection")
             enable_gi = "enabled"
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/pangomm.py` & `gvsbuild-2024.5.0/gvsbuild/projects/pangomm.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/pcre2.py` & `gvsbuild-2024.5.0/gvsbuild/projects/pcre2.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/pixman.py` & `gvsbuild-2024.5.0/gvsbuild/projects/pkgconf.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,28 +15,29 @@
 
 from gvsbuild.utils.base_builders import Meson
 from gvsbuild.utils.base_expanders import Tarball
 from gvsbuild.utils.base_project import Project, project_add
 
 
 @project_add
-class Pixman(Tarball, Meson):
+class PkgConf(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
-            "pixman",
-            repository="https://gitlab.freedesktop.org/pixman/pixman",
-            version="0.42.2",
-            lastversion_even=True,
-            archive_url="http://cairographics.org/releases/pixman-{version}.tar.gz",
-            hash="ea1480efada2fd948bc75366f7c349e1c96d3297d09a3fe62626e38e234a625e",
+            "pkgconf",
+            prj_dir="pkgconf",
+            version="2.2.0",
+            archive_url="https://distfiles.ariadne.space/pkgconf/pkgconf-{version}.tar.gz",
+            hash="28f8dfc279a10ef66148befa3f6eb266e5f3570316600208ed50e9781c7269d8",
             dependencies=["ninja", "meson"],
+            patches=["0001-libpkgconf-add-defines-to-unbreak-build-with-VS2013.patch"],
         )
+        self.add_param("-Dtests=disabled")
 
     def build(self):
-        enable_mmx = "disabled" if self.builder.x64 else "enabled"
-        Meson.build(
-            self,
-            meson_params=f"-Dsse2=enabled -Dssse3=enabled -Dmmx={enable_mmx} -Dtests=disabled",
-        )
+        Meson.build(self)
+        self.install(r".\COPYING share\doc\pkgconf")
 
-        self.install(r".\COPYING share\doc\pixman")
+    def post_install(self):
+        self.exec_cmd(
+            r"copy %(gtk_dir)s\bin\pkgconf.exe %(gtk_dir)s\bin\pkg-config.exe"
+        )
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/pkgconf.py` & `gvsbuild-2024.5.0/gvsbuild/projects/wing.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,29 +15,22 @@
 
 from gvsbuild.utils.base_builders import Meson
 from gvsbuild.utils.base_expanders import Tarball
 from gvsbuild.utils.base_project import Project, project_add
 
 
 @project_add
-class PkgConf(Tarball, Meson):
+class Wing(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
-            "pkgconf",
-            prj_dir="pkgconf",
-            version="2.2.0",
-            archive_url="https://distfiles.ariadne.space/pkgconf/pkgconf-{version}.tar.gz",
-            hash="28f8dfc279a10ef66148befa3f6eb266e5f3570316600208ed50e9781c7269d8",
-            dependencies=["ninja", "meson"],
-            patches=["0001-libpkgconf-add-defines-to-unbreak-build-with-VS2013.patch"],
+            "wing",
+            version="0.3.18",
+            repository="https://gitlab.gnome.org/GNOME/wing",
+            archive_url="https://gitlab.gnome.org/GNOME/wing/-/archive/v{version}/wing-v{version}.tar.gz",
+            hash="6d15984c917d9bdf2c88a06072991daf39a226d2024ec5b196a1c9ed8e81e962",
+            dependencies=["ninja", "meson", "pkgconf", "glib"],
         )
-        self.add_param("-Dtests=disabled")
 
     def build(self):
         Meson.build(self)
-        self.install(r".\COPYING share\doc\pkgconf")
-
-    def post_install(self):
-        self.exec_cmd(
-            r"copy %(gtk_dir)s\bin\pkgconf.exe %(gtk_dir)s\bin\pkg-config.exe"
-        )
+        self.install(r".\COPYING share\doc\wing")
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/protobuf.py` & `gvsbuild-2024.5.0/gvsbuild/projects/protobuf.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/pycairo.py` & `gvsbuild-2024.5.0/gvsbuild/projects/pycairo.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/pygobject.py` & `gvsbuild-2024.5.0/gvsbuild/projects/pygobject.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,19 +22,19 @@
 
 @project_add
 class PyGObject(Tarball, Meson):
     def __init__(self):
         Project.__init__(
             self,
             "pygobject",
-            version="3.48.1",
+            version="3.48.2",
             lastversion_even=True,
             repository="https://gitlab.gnome.org/GNOME/pygobject",
             archive_url="https://download.gnome.org/sources/pygobject/{major}.{minor}/pygobject-{version}.tar.xz",
-            hash="3a0a2c0c0f25931b5840649c54834b9e58a63148d37fa9f6308887b7027e15c2",
+            hash="0794aeb4a9be31a092ac20621b5f54ec280f9185943d328b105cdae6298ad1a7",
             dependencies=["pycairo", "gobject-introspection", "libffi"],
             patches=[
                 "001-pygobject-py38-load-dll.patch",
             ],
         )
 
     def build(self):
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/sqlite.py` & `gvsbuild-2024.5.0/gvsbuild/projects/sqlite.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 
 @project_add
 class SQLite(Tarball, Project):
     def __init__(self):
         Project.__init__(
             self,
             "sqlite",
-            version="3.45.2",
+            version="3.45.3",
             archive_url="https://www.sqlite.org/2024/sqlite-autoconf-{major}{minor:0<3}{micro:0<3}.tar.gz",
-            hash="bc9067442eedf3dd39989b5c5cfbfff37ae66cc9c99274e0c3052dc4d4a8f6ae",
+            hash="b2809ca53124c19c60f42bf627736eae011afdcc205bb48270a5ee9a38191531",
         )
 
     def build(self):
         nmake_debug = (
             "DEBUG=2" if self.builder.opts.configuration == "debug" else "DEBUG=0"
         )
         self.exec_vs(f"nmake /f Makefile.msc sqlite3.dll DYNAMIC_SHELL=1 {nmake_debug}")
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/win_iconv.py` & `gvsbuild-2024.5.0/gvsbuild/projects/win_iconv.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/wing.py` & `gvsbuild-2024.5.0/gvsbuild/projects/opus.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,26 +11,32 @@
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program; if not, see <http://www.gnu.org/licenses/>.
 
 from gvsbuild.utils.base_builders import Meson
 from gvsbuild.utils.base_expanders import Tarball
-from gvsbuild.utils.base_project import Project, project_add
+from gvsbuild.utils.base_project import project_add
 
 
 @project_add
-class Wing(Tarball, Meson):
+class Opus(Tarball, Meson):
     def __init__(self):
-        Project.__init__(
+        Meson.__init__(
             self,
-            "wing",
-            version="0.3.18",
-            repository="https://gitlab.gnome.org/GNOME/wing",
-            archive_url="https://gitlab.gnome.org/GNOME/wing/-/archive/v{version}/wing-v{version}.tar.gz",
-            hash="6d15984c917d9bdf2c88a06072991daf39a226d2024ec5b196a1c9ed8e81e962",
-            dependencies=["ninja", "meson", "pkgconf", "glib"],
+            "opus",
+            version="1.5.2",
+            repository="https://github.com/xiph/opus",
+            archive_url="https://downloads.xiph.org/releases/opus/opus-{version}.tar.gz",
+            hash="65c1d2f78b9f2fb20082c38cbe47c951ad5839345876e46941612ee87f9a7ce1",
+            dependencies=[
+                "ninja",
+                "meson",
+                "pkgconf",
+            ],
         )
+        self.add_param("-Dtests=disabled")
+        self.add_param("-Ddocs=disabled")
 
     def build(self):
         Meson.build(self)
-        self.install(r".\COPYING share\doc\wing")
+        self.install(r"COPYING share\doc\opus")
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/x264.py` & `gvsbuild-2024.5.0/gvsbuild/projects/x264.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/projects/zlib.py` & `gvsbuild-2024.5.0/gvsbuild/projects/zlib.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/tools.py` & `gvsbuild-2024.5.0/gvsbuild/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 @tool_add
 class ToolCargo(Tool):
     def __init__(self):
         Tool.__init__(
             self,
             "cargo",
-            version="1.77.1",
+            version="1.78.0",
             repository="rust-lang/rust",
             archive_url="https://win.rustup.rs/x86_64",
             archive_filename="rustup-init.exe",
             exe_name="cargo.exe",
         )
 
     def load_defaults(self):
@@ -62,17 +62,17 @@
 
 @tool_add
 class ToolCmake(Tool):
     def __init__(self):
         Tool.__init__(
             self,
             "cmake",
-            version="3.29.1",
+            version="3.29.2",
             archive_url="https://github.com/Kitware/CMake/releases/download/v{version}/cmake-{version}-windows-x86_64.zip",
-            hash="c8cf6ed50551d00ad8cd1f3b232810cd0a8b43b4a1d4f1393f0a575d423884dc",
+            hash="86b5de51f60a0e9d62be4d8ca76ea467d154083d356fcc9af1409606be341cd8",
             dir_part="cmake-{version}-windows-x86_64",
         )
 
     def load_defaults(self):
         Tool.load_defaults(self)
         self.tool_path = os.path.join(self.build_dir, "bin")
         self.full_exe = os.path.join(self.tool_path, "cmake.exe")
@@ -131,17 +131,17 @@
 
 @tool_add
 class ToolNasm(Tool):
     def __init__(self):
         Tool.__init__(
             self,
             "nasm",
-            version="2.16.02",
+            version="2.16.03",
             archive_url="https://www.nasm.us/pub/nasm/releasebuilds/{version}/win64/nasm-{version}-win64.zip",
-            hash="3facb987f97b9fc4a485d2f95aa64219dbfa991fc5d1867f7b0f93e416074d3c",
+            hash="3ee4782247bcb874378d02f7eab4e294a84d3d15f3f6ee2de2f47a46aa7226e6",
             dir_part="nasm-{version}",
             exe_name="nasm.exe",
         )
 
     def unpack(self):
         # We download directly the exe file so we copy it on the tool directory ...
         self.mark_deps = extract_exec(
@@ -156,18 +156,18 @@
 
 @tool_add
 class ToolNinja(Tool):
     def __init__(self):
         Tool.__init__(
             self,
             "ninja",
-            version="1.11.1",
+            version="1.12.0",
             archive_url="https://github.com/ninja-build/ninja/releases/download/v{version}/ninja-win.zip",
             archive_filename="ninja-win-{version}.zip",
-            hash="524b344a1a9a55005eaf868d991e090ab8ce07fa109f1820d40e74642e289abc",
+            hash="51d99be9ceea8835edf536d52d47fa4c316aa332e57f71a08df5bd059da11417",
             dir_part="ninja-{version}",
             exe_name="ninja.exe",
         )
 
     def unpack(self):
         self.mark_deps = extract_exec(
             self.archive_file, self.build_dir, check_file=self.full_exe, check_mark=True
@@ -206,14 +206,15 @@
 @tool_add
 class ToolGo(Tool):
     def __init__(self):
         Tool.__init__(
             self,
             "go",
             version="1.22.2",
+            repository="https://github.com/golang/go",
             archive_url="https://go.dev/dl/go{version}.windows-amd64.zip",
             hash="8e581cf330f49d3266e936521a2d8263679ef7e2fc2cbbceb85659122d883596",
             dir_part="go-{version}",
         )
 
     def load_defaults(self):
         Tool.load_defaults(self)
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/utils/base_builders.py` & `gvsbuild-2024.5.0/gvsbuild/utils/base_builders.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/utils/base_expanders.py` & `gvsbuild-2024.5.0/gvsbuild/utils/base_expanders.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/utils/base_group.py` & `gvsbuild-2024.5.0/gvsbuild/utils/base_group.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/utils/base_project.py` & `gvsbuild-2024.5.0/gvsbuild/utils/base_project.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/utils/base_tool.py` & `gvsbuild-2024.5.0/gvsbuild/utils/base_tool.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/utils/builder.py` & `gvsbuild-2024.5.0/gvsbuild/utils/builder.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/gvsbuild/utils/simple_ui.py` & `gvsbuild-2024.5.0/gvsbuild/utils/simple_ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program; if not, see <http://www.gnu.org/licenses/>.
 
 """Simple user interface for info, log & debug messages."""
 
-
 import ctypes
 import datetime
 import os
 import sys
 from contextlib import contextmanager, suppress
 
 from rich import print
```

### Comparing `gvsbuild-2024.4.1/gvsbuild/utils/utils.py` & `gvsbuild-2024.5.0/gvsbuild/utils/utils.py`

 * *Files identical despite different names*

### Comparing `gvsbuild-2024.4.1/pyproject.toml` & `gvsbuild-2024.5.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gvsbuild"
-version = "2024.4.1"
+version = "2024.5.0"
 description = "GTK stack for Windows"
 authors = ["Ignacio Casal Quinteiro <qignacio@amazon.com>", "Dan Yeaw <dan@yeaw.me>"]
 license = "GPL-2.0-only"
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Topic :: Software Development :: Build Tools",
@@ -51,27 +51,29 @@
 
 [testenv]
 commands = pytest
 deps = pytest
 """
 
 [tool.ruff]
-ignore = ["E501"]
 line-length = 88
+
+[tool.ruff.lint]
+ignore = ["E501"]
 select = [
     "B",
     "B9",
     "C",
     "E",
     "F",
     "W",
 ]
 extend-select = ["I"]
 
-[tool.ruff.mccabe]
+[tool.ruff.lint.mccabe]
 max-complexity = 20
 
 [tool.ruff.lint.flake8-bugbear]
 extend-immutable-calls = ["typer.Argument", "typer.Option"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `gvsbuild-2024.4.1/README.md` & `gvsbuild-2024.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 This python script helps you build a full [GTK](https://www.gtk.org/) library
 stack for Windows using Visual Studio. Currently, GTK 3 and GTK 4 are supported.
 
 ## Install GTK Only
 
 If you want to only run GTK on Windows and not build it yourself, you can download
-a zip file from the last release and unzip it to `C:\gtk`.
+a zip file from the [latest release](https://github.com/wingtk/gvsbuild/releases/latest) and unzip it to `C:\gtk`.
 
 It comes with GTK4, Cairo, PyGObject, Pycairo, GtkSourceView5, adwaita-icon-theme, and
 all of their dependencies.
 
 Note however that these binaries are provided “AS IS”, WITHOUT WARRANTY OF ANY KIND.
 They just contain the output of our latest CI run. They are not tested, and we cannot
 commit to timely updates even for security issues. We strongly recommend to build your
@@ -314,14 +314,25 @@
  ```
 gvsbuild deps --graph --gv-file test.gv
  ```
 
 Without option a simple dependency of all the projects is printed, as usual with
 --help a summary of the options/commands is printed.
 
+## Gvsbuild Users
+
+The following projects are using Gvsbuild for Windows GTK cross-platform support:
+
+- [Deluge](https://github.com/deluge-torrent/deluge) - BitTorrent client
+- [Gaphor](https://github.com/gaphor/gaphor) - A simple SysML/UML modeling tool
+- [PothosSDR](https://github.com/pothosware/PothosSDR) - Software-Defined Radio development environment
+- [SkyTemple Randomizer](https://github.com/SkyTemple/skytemple-randomizer) - Randomizer for Pokémon Mystery Dungeon Explorers of Sky
+
+Are you using Gvsbuild? Please submit a Pull Request to add your app to the list.
+
 ## License
 
 This build script is licensed under the GPL2.0 license, see the COPYING file for
 the full text.
 
 The binaries produced by the build script are licensed under the license terms
 of the project that is built (ie glib is LGPL so you can use glib.dll built
```

### Comparing `gvsbuild-2024.4.1/PKG-INFO` & `gvsbuild-2024.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gvsbuild
-Version: 2024.4.1
+Version: 2024.5.0
 Summary: GTK stack for Windows
 License: GPL-2.0-only
 Author: Ignacio Casal Quinteiro
 Author-email: qignacio@amazon.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: X11 Applications :: GTK
@@ -31,15 +31,15 @@
 
 This python script helps you build a full [GTK](https://www.gtk.org/) library
 stack for Windows using Visual Studio. Currently, GTK 3 and GTK 4 are supported.
 
 ## Install GTK Only
 
 If you want to only run GTK on Windows and not build it yourself, you can download
-a zip file from the last release and unzip it to `C:\gtk`.
+a zip file from the [latest release](https://github.com/wingtk/gvsbuild/releases/latest) and unzip it to `C:\gtk`.
 
 It comes with GTK4, Cairo, PyGObject, Pycairo, GtkSourceView5, adwaita-icon-theme, and
 all of their dependencies.
 
 Note however that these binaries are provided “AS IS”, WITHOUT WARRANTY OF ANY KIND.
 They just contain the output of our latest CI run. They are not tested, and we cannot
 commit to timely updates even for security issues. We strongly recommend to build your
@@ -341,14 +341,25 @@
  ```
 gvsbuild deps --graph --gv-file test.gv
  ```
 
 Without option a simple dependency of all the projects is printed, as usual with
 --help a summary of the options/commands is printed.
 
+## Gvsbuild Users
+
+The following projects are using Gvsbuild for Windows GTK cross-platform support:
+
+- [Deluge](https://github.com/deluge-torrent/deluge) - BitTorrent client
+- [Gaphor](https://github.com/gaphor/gaphor) - A simple SysML/UML modeling tool
+- [PothosSDR](https://github.com/pothosware/PothosSDR) - Software-Defined Radio development environment
+- [SkyTemple Randomizer](https://github.com/SkyTemple/skytemple-randomizer) - Randomizer for Pokémon Mystery Dungeon Explorers of Sky
+
+Are you using Gvsbuild? Please submit a Pull Request to add your app to the list.
+
 ## License
 
 This build script is licensed under the GPL2.0 license, see the COPYING file for
 the full text.
 
 The binaries produced by the build script are licensed under the license terms
 of the project that is built (ie glib is LGPL so you can use glib.dll built
```

