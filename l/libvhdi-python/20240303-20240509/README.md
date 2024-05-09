# Comparing `tmp/libvhdi-python-20240303.tar.gz` & `tmp/libvhdi-python-20240509.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libvhdi-python-20240303.tar", last modified: Sun Mar  3 08:23:02 2024, max compression
+gzip compressed data, was "libvhdi-python-20240509.tar", last modified: Thu May  9 06:52:14 2024, max compression
```

## Comparing `libvhdi-python-20240303.tar` & `libvhdi-python-20240509.tar`

### file list

```diff
@@ -1,829 +1,829 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:00.000000 libvhdi-20240303/libfdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-03-03 08:06:43.000000 libvhdi-20240303/libfdata/libfdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37893 2024-03-03 08:06:43.000000 libvhdi-20240303/libfdata/libfdata_area.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9700 2024-03-03 08:06:43.000000 libvhdi-20240303/libfdata/libfdata_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2024-03-03 08:06:43.000000 libvhdi-20240303/libfdata/libfdata_cache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30931 2024-03-03 08:06:43.000000 libvhdi-20240303/libfdata/libfdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2024-03-03 08:06:43.000000 libvhdi-20240303/libfdata/libfdata_mapped_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-03-03 08:06:43.000000 libvhdi-20240303/libfdata/libfdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6533 2024-03-03 08:06:43.000000 libvhdi-20240303/libfdata/libfdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   107689 2024-03-03 08:06:43.000000 libvhdi-20240303/libfdata/libfdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-03-03 08:06:43.000000 libvhdi-20240303/libfdata/libfdata_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12090 2024-03-03 08:06:43.000000 libvhdi-20240303/libfdata/libfdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4017 2024-03-03 08:06:43.000000 libvhdi-20240303/libfdata/libfdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1291 2024-03-03 08:06:43.000000 libvhdi-20240303/libfdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-03-03 08:06:43.000000 libvhdi-20240303/libfdata/libfdata_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-03-03 08:06:43.000000 libvhdi-20240303/libfdata/libfdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-03-03 08:06:43.000000 libvhdi-20240303/libfdata/libfdata_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-03-03 08:06:43.000000 libvhdi-20240303/libfdata/libfdata_cache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66203 2024-03-03 08:06:43.000000 libvhdi-20240303/libfdata/libfdata_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-03-03 08:06:43.000000 libvhdi-20240303/libfdata/libfdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2092 2024-03-03 08:06:43.000000 libvhdi-20240303/libfdata/libfdata_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7327 2024-03-03 08:06:43.000000 libvhdi-20240303/libfdata/libfdata_area.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-03-03 08:06:43.000000 libvhdi-20240303/libfdata/libfdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-03-03 08:06:43.000000 libvhdi-20240303/libfdata/libfdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2024-03-03 08:06:43.000000 libvhdi-20240303/libfdata/libfdata_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1995 2024-03-03 08:06:43.000000 libvhdi-20240303/libfdata/libfdata_mapped_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2024-03-03 08:06:43.000000 libvhdi-20240303/libfdata/libfdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19329 2024-03-03 08:06:43.000000 libvhdi-20240303/libfdata/libfdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21271 2024-03-03 08:06:43.000000 libvhdi-20240303/libfdata/libfdata_segments_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2054 2024-03-03 08:06:43.000000 libvhdi-20240303/libfdata/libfdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-03-03 08:06:43.000000 libvhdi-20240303/libfdata/libfdata_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6013 2024-03-03 08:06:43.000000 libvhdi-20240303/libfdata/libfdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2804 2024-03-03 08:06:43.000000 libvhdi-20240303/libfdata/libfdata_segments_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32254 2024-03-03 08:07:00.000000 libvhdi-20240303/libfdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49670 2024-03-03 08:06:43.000000 libvhdi-20240303/libfdata/libfdata_vector.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-03-03 08:06:43.000000 libvhdi-20240303/libfdata/libfdata_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7810 2024-03-03 08:06:43.000000 libvhdi-20240303/libfdata/libfdata_vector.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-03-03 07:54:29.000000 libvhdi-20240303/COPYING
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-03-03 08:06:59.000000 libvhdi-20240303/install-sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 07:54:29.000000 libvhdi-20240303/NEWS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-03-03 08:07:00.000000 libvhdi-20240303/depcomp
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:00.000000 libvhdi-20240303/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-03-03 08:06:44.000000 libvhdi-20240303/libfguid/libfguid_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2024-03-03 08:06:44.000000 libvhdi-20240303/libfguid/libfguid_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2024-03-03 08:06:44.000000 libvhdi-20240303/libfguid/libfguid_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-03-03 08:06:44.000000 libvhdi-20240303/libfguid/libfguid_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      681 2024-03-03 08:06:44.000000 libvhdi-20240303/libfguid/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-03-03 08:06:44.000000 libvhdi-20240303/libfguid/libfguid_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-03-03 08:06:44.000000 libvhdi-20240303/libfguid/libfguid_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-03-03 08:06:44.000000 libvhdi-20240303/libfguid/libfguid_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2024-03-03 08:06:44.000000 libvhdi-20240303/libfguid/libfguid_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2024-03-03 08:06:44.000000 libvhdi-20240303/libfguid/libfguid_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-03-03 08:06:44.000000 libvhdi-20240303/libfguid/libfguid_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28469 2024-03-03 08:07:00.000000 libvhdi-20240303/libfguid/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-03-03 08:06:44.000000 libvhdi-20240303/libfguid/libfguid_error.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:22:59.000000 libvhdi-20240303/m4/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11498 2023-12-03 09:15:05.000000 libvhdi-20240303/m4/libcfile.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:15:05.000000 libvhdi-20240303/m4/tests.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9379 2023-12-03 09:15:05.000000 libvhdi-20240303/m4/libcpath.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:15:04.000000 libvhdi-20240303/m4/lib-prefix.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:15:05.000000 libvhdi-20240303/m4/progtest.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31269 2023-12-03 09:15:04.000000 libvhdi-20240303/m4/libuna.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:15:04.000000 libvhdi-20240303/m4/gettext.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:15:04.000000 libvhdi-20240303/m4/lib-ld.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8230 2023-12-03 09:15:04.000000 libvhdi-20240303/m4/libclocale.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17147 2023-12-03 09:15:04.000000 libvhdi-20240303/m4/libcdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7384 2023-12-03 09:15:05.000000 libvhdi-20240303/m4/libcsplit.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14115 2023-12-03 09:15:04.000000 libvhdi-20240303/m4/common.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11112 2023-12-03 09:15:04.000000 libvhdi-20240303/m4/libcthreads.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-03-03 08:06:53.000000 libvhdi-20240303/m4/ltversion.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-03-03 08:06:53.000000 libvhdi-20240303/m4/ltsugar.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15545 2023-12-03 09:15:05.000000 libvhdi-20240303/m4/libfdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:15:04.000000 libvhdi-20240303/m4/host-cpu-c-abi.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5232 2023-12-03 09:15:04.000000 libvhdi-20240303/m4/libfuse.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-03-03 08:06:52.000000 libvhdi-20240303/m4/libtool.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:15:04.000000 libvhdi-20240303/m4/po.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2023-12-03 09:15:05.000000 libvhdi-20240303/m4/libcerror.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5638 2023-12-03 09:15:04.000000 libvhdi-20240303/m4/libcnotify.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5640 2023-12-03 09:15:05.000000 libvhdi-20240303/m4/libfguid.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11692 2023-12-03 09:15:04.000000 libvhdi-20240303/m4/libbfio.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:15:04.000000 libvhdi-20240303/m4/intlmacosx.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-03-03 08:06:53.000000 libvhdi-20240303/m4/lt~obsolete.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:15:04.000000 libvhdi-20240303/m4/lib-link.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:15:04.000000 libvhdi-20240303/m4/iconv.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-03-03 08:06:52.000000 libvhdi-20240303/m4/ltoptions.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:15:04.000000 libvhdi-20240303/m4/nls.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6323 2023-12-03 09:15:05.000000 libvhdi-20240303/m4/python.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:15:04.000000 libvhdi-20240303/m4/types.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7325 2023-12-03 09:15:04.000000 libvhdi-20240303/m4/libfcache.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3852 2023-12-03 09:15:05.000000 libvhdi-20240303/m4/pthread.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:22:59.000000 libvhdi-20240303/include/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      459 2024-03-03 07:54:29.000000 libvhdi-20240303/include/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12120 2024-03-03 08:07:14.000000 libvhdi-20240303/include/libvhdi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12120 2024-03-03 07:54:31.000000 libvhdi-20240303/include/libvhdi.h.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:22:59.000000 libvhdi-20240303/include/libvhdi/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2125 2024-03-03 07:54:31.000000 libvhdi-20240303/include/libvhdi/definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2123 2024-03-03 08:07:14.000000 libvhdi-20240303/include/libvhdi/definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4933 2024-03-03 07:54:31.000000 libvhdi-20240303/include/libvhdi/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4802 2024-03-03 08:07:14.000000 libvhdi-20240303/include/libvhdi/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1539 2024-03-03 07:54:31.000000 libvhdi-20240303/include/libvhdi/features.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6689 2024-03-03 07:54:31.000000 libvhdi-20240303/include/libvhdi/error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-03-03 07:54:31.000000 libvhdi-20240303/include/libvhdi/extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1475 2024-03-03 08:07:14.000000 libvhdi-20240303/include/libvhdi/features.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5195 2024-03-03 07:54:31.000000 libvhdi-20240303/include/libvhdi/codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26996 2024-03-03 08:06:59.000000 libvhdi-20240303/include/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:22:59.000000 libvhdi-20240303/common/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-03-03 07:54:31.000000 libvhdi-20240303/common/config_borlandc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-03-03 07:54:31.000000 libvhdi-20240303/common/file_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-03-03 07:54:31.000000 libvhdi-20240303/common/memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-03-03 07:54:31.000000 libvhdi-20240303/common/byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-03-03 07:54:31.000000 libvhdi-20240303/common/common.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-03-03 07:54:31.000000 libvhdi-20240303/common/config_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-03-03 07:54:31.000000 libvhdi-20240303/common/system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      366 2024-03-03 07:54:29.000000 libvhdi-20240303/common/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-03-03 07:54:31.000000 libvhdi-20240303/common/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7373 2024-03-03 08:07:14.000000 libvhdi-20240303/common/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16174 2024-03-03 08:06:59.000000 libvhdi-20240303/common/config.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17131 2024-03-03 08:07:14.000000 libvhdi-20240303/common/config.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-03-03 07:54:31.000000 libvhdi-20240303/common/wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-03-03 07:54:31.000000 libvhdi-20240303/common/narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-03-03 07:54:31.000000 libvhdi-20240303/common/config_msc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24022 2024-03-03 08:06:59.000000 libvhdi-20240303/common/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:22:59.000000 libvhdi-20240303/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-03-03 08:06:36.000000 libvhdi-20240303/libclocale/libclocale_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-03-03 08:06:36.000000 libvhdi-20240303/libclocale/libclocale_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      779 2024-03-03 08:06:36.000000 libvhdi-20240303/libclocale/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-03-03 08:06:36.000000 libvhdi-20240303/libclocale/libclocale_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-03-03 08:06:36.000000 libvhdi-20240303/libclocale/libclocale_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-03-03 08:06:36.000000 libvhdi-20240303/libclocale/libclocale_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-03-03 08:06:36.000000 libvhdi-20240303/libclocale/libclocale_locale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-03-03 08:06:36.000000 libvhdi-20240303/libclocale/libclocale_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-03-03 08:06:36.000000 libvhdi-20240303/libclocale/libclocale_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-03-03 08:06:36.000000 libvhdi-20240303/libclocale/libclocale_locale.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29025 2024-03-03 08:07:00.000000 libvhdi-20240303/libclocale/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-03-03 08:06:36.000000 libvhdi-20240303/libclocale/libclocale_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-03-03 08:06:36.000000 libvhdi-20240303/libclocale/libclocale_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-03-03 08:06:36.000000 libvhdi-20240303/libclocale/libclocale_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3274 2024-03-03 07:54:29.000000 libvhdi-20240303/libvhdi.spec.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:00.000000 libvhdi-20240303/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-03-03 08:06:42.000000 libvhdi-20240303/libfcache/libfcache_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2024-03-03 08:06:42.000000 libvhdi-20240303/libfcache/libfcache_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2024-03-03 08:06:42.000000 libvhdi-20240303/libfcache/libfcache_cache_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-03-03 08:06:42.000000 libvhdi-20240303/libfcache/libfcache_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      880 2024-03-03 08:06:42.000000 libvhdi-20240303/libfcache/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-03-03 08:06:42.000000 libvhdi-20240303/libfcache/libfcache_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-03-03 08:06:42.000000 libvhdi-20240303/libfcache/libfcache_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2024-03-03 08:06:42.000000 libvhdi-20240303/libfcache/libfcache_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2024-03-03 08:06:42.000000 libvhdi-20240303/libfcache/libfcache_cache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-03-03 08:06:42.000000 libvhdi-20240303/libfcache/libfcache_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-03-03 08:06:42.000000 libvhdi-20240303/libfcache/libfcache_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2024-03-03 08:06:42.000000 libvhdi-20240303/libfcache/libfcache_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-03-03 08:06:42.000000 libvhdi-20240303/libfcache/libfcache_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2024-03-03 08:06:42.000000 libvhdi-20240303/libfcache/libfcache_cache_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29498 2024-03-03 08:07:00.000000 libvhdi-20240303/libfcache/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-03-03 08:06:42.000000 libvhdi-20240303/libfcache/libfcache_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-03-03 08:06:42.000000 libvhdi-20240303/libfcache/libfcache_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2024-03-03 08:06:42.000000 libvhdi-20240303/libfcache/libfcache_cache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2207 2023-12-03 09:15:01.000000 libvhdi-20240303/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:00.000000 libvhdi-20240303/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-03-03 08:06:30.000000 libvhdi-20240303/libbfio/libbfio_file_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-03-03 08:06:30.000000 libvhdi-20240303/libbfio/libbfio_file_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-03-03 08:06:30.000000 libvhdi-20240303/libbfio/libbfio_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-03-03 08:06:30.000000 libvhdi-20240303/libbfio/libbfio_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-03-03 08:06:30.000000 libvhdi-20240303/libbfio/libbfio_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-03-03 08:06:30.000000 libvhdi-20240303/libbfio/libbfio_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-03-03 08:06:30.000000 libvhdi-20240303/libbfio/libbfio_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-03-03 08:06:30.000000 libvhdi-20240303/libbfio/libbfio_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-03-03 08:06:30.000000 libvhdi-20240303/libbfio/libbfio_file_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-03-03 08:06:30.000000 libvhdi-20240303/libbfio/libbfio_file_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-03-03 08:06:30.000000 libvhdi-20240303/libbfio/libbfio_file_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-03-03 08:06:30.000000 libvhdi-20240303/libbfio/libbfio_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-03-03 08:06:30.000000 libvhdi-20240303/libbfio/libbfio_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-03-03 08:06:30.000000 libvhdi-20240303/libbfio/libbfio_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-03-03 08:06:30.000000 libvhdi-20240303/libbfio/libbfio_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-03-03 08:06:30.000000 libvhdi-20240303/libbfio/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-03-03 08:06:30.000000 libvhdi-20240303/libbfio/libbfio_libcfile.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-03-03 08:06:30.000000 libvhdi-20240303/libbfio/libbfio_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-03-03 08:06:30.000000 libvhdi-20240303/libbfio/libbfio_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-03-03 08:06:30.000000 libvhdi-20240303/libbfio/libbfio_file_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-03-03 08:06:30.000000 libvhdi-20240303/libbfio/libbfio_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-03-03 08:06:30.000000 libvhdi-20240303/libbfio/libbfio_memory_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-03-03 08:06:30.000000 libvhdi-20240303/libbfio/libbfio_file_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-03-03 08:06:30.000000 libvhdi-20240303/libbfio/libbfio_file_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-03-03 08:06:30.000000 libvhdi-20240303/libbfio/libbfio_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-03-03 08:06:30.000000 libvhdi-20240303/libbfio/libbfio_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-03-03 08:06:30.000000 libvhdi-20240303/libbfio/libbfio_memory_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-03-03 08:06:30.000000 libvhdi-20240303/libbfio/libbfio_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-03-03 08:06:30.000000 libvhdi-20240303/libbfio/libbfio_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-03-03 08:06:30.000000 libvhdi-20240303/libbfio/libbfio_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-03-03 08:06:30.000000 libvhdi-20240303/libbfio/libbfio_memory_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-03-03 08:06:30.000000 libvhdi-20240303/libbfio/libbfio_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-03-03 08:06:30.000000 libvhdi-20240303/libbfio/libbfio_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32484 2024-03-03 08:06:59.000000 libvhdi-20240303/libbfio/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-03-03 08:06:30.000000 libvhdi-20240303/libbfio/libbfio_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-03-03 08:06:30.000000 libvhdi-20240303/libbfio/libbfio_memory_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-03-03 08:06:30.000000 libvhdi-20240303/libbfio/libbfio_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-03-03 08:06:30.000000 libvhdi-20240303/libbfio/libbfio_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:15:01.000000 libvhdi-20240303/ABOUT-NLS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-03-03 08:06:59.000000 libvhdi-20240303/config.guess
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:22:59.000000 libvhdi-20240303/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1024 2024-03-03 07:54:32.000000 libvhdi-20240303/dpkg/copyright
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-03-03 07:54:29.000000 libvhdi-20240303/dpkg/libvhdi-tools.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-03-03 07:54:29.000000 libvhdi-20240303/dpkg/libvhdi.install
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:22:59.000000 libvhdi-20240303/dpkg/source/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-03-03 07:54:29.000000 libvhdi-20240303/dpkg/source/format
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2106 2024-03-03 07:54:29.000000 libvhdi-20240303/dpkg/control
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      761 2024-03-03 07:54:29.000000 libvhdi-20240303/dpkg/rules
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      120 2024-03-03 07:54:29.000000 libvhdi-20240303/dpkg/changelog.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      139 2024-03-03 08:07:14.000000 libvhdi-20240303/dpkg/changelog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-03-03 07:54:29.000000 libvhdi-20240303/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-03-03 07:54:29.000000 libvhdi-20240303/dpkg/libvhdi-dev.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-03-03 07:54:29.000000 libvhdi-20240303/dpkg/libvhdi-python3.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      479 2024-03-03 08:07:14.000000 libvhdi-20240303/setup.cfg
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-03-03 07:54:29.000000 libvhdi-20240303/COPYING.LESSER
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1705275 2024-03-03 08:06:57.000000 libvhdi-20240303/configure
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-03-03 08:06:59.000000 libvhdi-20240303/compile
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-03-03 08:06:59.000000 libvhdi-20240303/missing
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/libfdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6858 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/libfdata/libfdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/vhdi_test_dynamic_disk_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6016 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/vhdi_test_dynamic_disk_header/vhdi_test_dynamic_disk_header.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/vhdi_test_tools_info_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6008 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/vhdi_test_tools_info_handle/vhdi_test_tools_info_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/vhdi_test_region_table_entry/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5766 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/vhdi_test_region_table_entry/vhdi_test_region_table_entry.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/vhdi_test_region_table/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5748 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/vhdi_test_region_table/vhdi_test_region_table.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/vhdi_test_io_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5739 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/vhdi_test_io_handle/vhdi_test_io_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/vhdi_test_block_allocation_table/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5778 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/vhdi_test_block_allocation_table/vhdi_test_block_allocation_table.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/vhdi_test_parent_locator_entry/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5772 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/vhdi_test_parent_locator_entry/vhdi_test_parent_locator_entry.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/vhdi_test_support/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6388 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/vhdi_test_support/vhdi_test_support.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/vhdi_test_parent_locator_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5775 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/vhdi_test_parent_locator_header/vhdi_test_parent_locator_header.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/vhdi_test_metadata_table_entry/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5772 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/vhdi_test_metadata_table_entry/vhdi_test_metadata_table_entry.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/libfguid/libfguid.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/vhdi_test_tools_output/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5675 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/vhdi_test_tools_output/vhdi_test_tools_output.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/vhdi_test_image_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5995 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/vhdi_test_image_header/vhdi_test_image_header.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/vhdi_test_error/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5484 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/vhdi_test_error/vhdi_test_error.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/libclocale/libclocale.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/libfcache/libfcache.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/vhdi_test_tools_signal/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5675 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/vhdi_test_tools_signal/vhdi_test_tools_signal.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2204 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/libbfio/libbfio.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/vhdi_test_sector_range_descriptor/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5781 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/vhdi_test_sector_range_descriptor/vhdi_test_sector_range_descriptor.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/vhdi_test_parent_locator/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5754 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/vhdi_test_parent_locator/vhdi_test_parent_locator.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/vhdi_test_block_descriptor/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5760 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/vhdi_test_block_descriptor/vhdi_test_block_descriptor.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/libcfile/libcfile.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/pyvhdi/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6506 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/pyvhdi/pyvhdi.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/vhdi_test_file_footer/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5992 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/vhdi_test_file_footer/vhdi_test_file_footer.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/libcdata/libcdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/vhdi_test_metadata_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5757 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/vhdi_test_metadata_values/vhdi_test_metadata_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/vhdimount/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7556 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/vhdimount/vhdimount.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/vhdi_test_region_table_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5769 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/vhdi_test_region_table_header/vhdi_test_region_table_header.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/vhdiinfo/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6829 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/vhdiinfo/vhdiinfo.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/libcthreads/libcthreads.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/libcpath/libcpath.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/vhdi_test_file/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6461 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/vhdi_test_file/vhdi_test_file.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/vhdi_test_metadata_table/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5754 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/vhdi_test_metadata_table/vhdi_test_metadata_table.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/vhdi_test_metadata_table_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5775 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/vhdi_test_metadata_table_header/vhdi_test_metadata_table_header.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/vhdi_test_file_information/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6007 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/vhdi_test_file_information/vhdi_test_file_information.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39154 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/libvhdi.sln
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/libcsplit/libcsplit.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/libvhdi/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11785 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/libvhdi/libvhdi.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/libuna/libuna.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23194 2024-03-03 08:07:00.000000 libvhdi-20240303/msvscpp/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/libcnotify/libcnotify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/vhdi_test_checksum/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5656 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/vhdi_test_checksum/vhdi_test_checksum.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/libcerror/libcerror.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/msvscpp/vhdi_test_notify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5651 2024-03-03 07:56:41.000000 libvhdi-20240303/msvscpp/vhdi_test_notify/vhdi_test_notify.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-03-03 07:54:30.000000 libvhdi-20240303/AUTHORS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:00.000000 libvhdi-20240303/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-03-03 08:06:35.000000 libvhdi-20240303/libcfile/libcfile_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-03-03 08:06:35.000000 libvhdi-20240303/libcfile/libcfile_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-03-03 08:06:35.000000 libvhdi-20240303/libcfile/libcfile_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-03-03 08:06:35.000000 libvhdi-20240303/libcfile/libcfile_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-03-03 08:06:35.000000 libvhdi-20240303/libcfile/libcfile_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-03-03 08:06:35.000000 libvhdi-20240303/libcfile/libcfile_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      942 2024-03-03 08:06:35.000000 libvhdi-20240303/libcfile/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-03-03 08:06:35.000000 libvhdi-20240303/libcfile/libcfile_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-03-03 08:06:35.000000 libvhdi-20240303/libcfile/libcfile_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-03-03 08:06:35.000000 libvhdi-20240303/libcfile/libcfile_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-03-03 08:06:35.000000 libvhdi-20240303/libcfile/libcfile_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-03-03 08:06:35.000000 libvhdi-20240303/libcfile/libcfile_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-03-03 08:06:35.000000 libvhdi-20240303/libcfile/libcfile_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-03-03 08:06:35.000000 libvhdi-20240303/libcfile/libcfile_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-03-03 08:06:35.000000 libvhdi-20240303/libcfile/libcfile_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-03-03 08:06:35.000000 libvhdi-20240303/libcfile/libcfile_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-03-03 08:06:35.000000 libvhdi-20240303/libcfile/libcfile_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29789 2024-03-03 08:07:00.000000 libvhdi-20240303/libcfile/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-03-03 08:06:35.000000 libvhdi-20240303/libcfile/libcfile_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-03-03 08:06:35.000000 libvhdi-20240303/libcfile/libcfile_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-03-03 08:06:35.000000 libvhdi-20240303/libcfile/libcfile_winapi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-03-03 08:06:35.000000 libvhdi-20240303/libcfile/libcfile_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      613 2024-03-03 07:55:55.000000 libvhdi-20240303/README
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:00.000000 libvhdi-20240303/pyvhdi/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-03-03 07:54:32.000000 libvhdi-20240303/pyvhdi/pyvhdi_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-03-03 07:54:32.000000 libvhdi-20240303/pyvhdi/pyvhdi_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1603 2024-03-03 07:54:32.000000 libvhdi-20240303/pyvhdi/pyvhdi_disk_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33791 2024-03-03 07:54:32.000000 libvhdi-20240303/pyvhdi/pyvhdi_file_object_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1190 2023-12-03 09:15:05.000000 libvhdi-20240303/pyvhdi/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14542 2024-03-03 07:55:55.000000 libvhdi-20240303/pyvhdi/pyvhdi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1531 2024-03-03 07:54:32.000000 libvhdi-20240303/pyvhdi/pyvhdi_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-03-03 07:54:32.000000 libvhdi-20240303/pyvhdi/pyvhdi_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2030 2024-03-03 07:54:32.000000 libvhdi-20240303/pyvhdi/pyvhdi_python.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8858 2024-03-03 07:54:32.000000 libvhdi-20240303/pyvhdi/pyvhdi_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40871 2024-03-03 07:58:51.000000 libvhdi-20240303/pyvhdi/pyvhdi_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1847 2024-03-03 07:54:32.000000 libvhdi-20240303/pyvhdi/pyvhdi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1535 2024-03-03 07:54:32.000000 libvhdi-20240303/pyvhdi/pyvhdi_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-03-03 07:54:32.000000 libvhdi-20240303/pyvhdi/pyvhdi_libvhdi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-03-03 07:54:32.000000 libvhdi-20240303/pyvhdi/pyvhdi_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5797 2024-03-03 07:54:32.000000 libvhdi-20240303/pyvhdi/pyvhdi_disk_types.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-03-03 07:55:55.000000 libvhdi-20240303/pyvhdi/pyvhdi_guid.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41142 2024-03-03 08:07:00.000000 libvhdi-20240303/pyvhdi/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1355 2024-03-03 07:54:32.000000 libvhdi-20240303/pyvhdi/pyvhdi_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4080 2024-03-03 07:54:32.000000 libvhdi-20240303/pyvhdi/pyvhdi_file_object_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-03-03 07:54:32.000000 libvhdi-20240303/pyvhdi/pyvhdi_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-03-03 07:54:32.000000 libvhdi-20240303/pyvhdi/pyvhdi_guid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3618 2024-03-03 07:55:55.000000 libvhdi-20240303/pyvhdi/pyvhdi_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-03-03 08:06:59.000000 libvhdi-20240303/INSTALL
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:22:59.000000 libvhdi-20240303/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-03-03 08:06:32.000000 libvhdi-20240303/libcdata/libcdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-03-03 08:06:32.000000 libvhdi-20240303/libcdata/libcdata_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-03-03 08:06:32.000000 libvhdi-20240303/libcdata/libcdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-03-03 08:06:32.000000 libvhdi-20240303/libcdata/libcdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-03-03 08:06:32.000000 libvhdi-20240303/libcdata/libcdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-03-03 08:06:32.000000 libvhdi-20240303/libcdata/libcdata_btree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-03-03 08:06:32.000000 libvhdi-20240303/libcdata/libcdata_btree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-03-03 08:06:32.000000 libvhdi-20240303/libcdata/libcdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-03-03 08:06:32.000000 libvhdi-20240303/libcdata/libcdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-03-03 08:06:32.000000 libvhdi-20240303/libcdata/libcdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-03-03 08:06:32.000000 libvhdi-20240303/libcdata/libcdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-03-03 08:06:32.000000 libvhdi-20240303/libcdata/libcdata_btree_values_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1127 2024-03-03 08:06:32.000000 libvhdi-20240303/libcdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-03-03 08:06:32.000000 libvhdi-20240303/libcdata/libcdata_btree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-03-03 08:06:32.000000 libvhdi-20240303/libcdata/libcdata_range_list_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-03-03 08:06:32.000000 libvhdi-20240303/libcdata/libcdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-03-03 08:06:32.000000 libvhdi-20240303/libcdata/libcdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-03-03 08:06:32.000000 libvhdi-20240303/libcdata/libcdata_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-03-03 08:06:32.000000 libvhdi-20240303/libcdata/libcdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-03-03 08:06:32.000000 libvhdi-20240303/libcdata/libcdata_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-03-03 08:06:32.000000 libvhdi-20240303/libcdata/libcdata_tree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-03-03 08:06:32.000000 libvhdi-20240303/libcdata/libcdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-03-03 08:06:32.000000 libvhdi-20240303/libcdata/libcdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-03-03 08:06:32.000000 libvhdi-20240303/libcdata/libcdata_btree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-03-03 08:06:32.000000 libvhdi-20240303/libcdata/libcdata_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-03-03 08:06:32.000000 libvhdi-20240303/libcdata/libcdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31473 2024-03-03 08:06:59.000000 libvhdi-20240303/libcdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-03-03 08:06:32.000000 libvhdi-20240303/libcdata/libcdata_range_list_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-03-03 08:06:32.000000 libvhdi-20240303/libcdata/libcdata_btree_values_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-03-03 08:06:32.000000 libvhdi-20240303/libcdata/libcdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-03-03 07:54:29.000000 libvhdi-20240303/pyproject.toml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      480 2024-03-03 07:54:29.000000 libvhdi-20240303/setup.cfg.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-03-03 08:06:59.000000 libvhdi-20240303/config.sub
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-03-03 07:54:29.000000 libvhdi-20240303/setup.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1493 2024-03-03 07:54:29.000000 libvhdi-20240303/acinclude.m4
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:15:00.000000 libvhdi-20240303/config.rpath
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:22:59.000000 libvhdi-20240303/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-03-03 08:06:41.000000 libvhdi-20240303/libcthreads/libcthreads_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-03-03 08:06:41.000000 libvhdi-20240303/libcthreads/libcthreads_read_write_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-03-03 08:06:41.000000 libvhdi-20240303/libcthreads/libcthreads_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-03-03 08:06:41.000000 libvhdi-20240303/libcthreads/libcthreads_thread_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-03-03 08:06:41.000000 libvhdi-20240303/libcthreads/libcthreads_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-03-03 08:06:41.000000 libvhdi-20240303/libcthreads/libcthreads_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-03-03 08:06:41.000000 libvhdi-20240303/libcthreads/libcthreads_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-03-03 08:06:41.000000 libvhdi-20240303/libcthreads/libcthreads_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-03-03 08:06:41.000000 libvhdi-20240303/libcthreads/libcthreads_condition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-03-03 08:06:41.000000 libvhdi-20240303/libcthreads/libcthreads_repeating_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1171 2024-03-03 08:06:41.000000 libvhdi-20240303/libcthreads/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-03-03 08:06:41.000000 libvhdi-20240303/libcthreads/libcthreads_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-03-03 08:06:41.000000 libvhdi-20240303/libcthreads/libcthreads_mutex.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-03-03 08:06:41.000000 libvhdi-20240303/libcthreads/libcthreads_queue.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-03-03 08:06:41.000000 libvhdi-20240303/libcthreads/libcthreads_mutex.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-03-03 08:06:41.000000 libvhdi-20240303/libcthreads/libcthreads_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-03-03 08:06:41.000000 libvhdi-20240303/libcthreads/libcthreads_thread_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-03-03 08:06:41.000000 libvhdi-20240303/libcthreads/libcthreads_condition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-03-03 08:06:41.000000 libvhdi-20240303/libcthreads/libcthreads_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-03-03 08:06:41.000000 libvhdi-20240303/libcthreads/libcthreads_read_write_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-03-03 08:06:41.000000 libvhdi-20240303/libcthreads/libcthreads_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-03-03 08:06:41.000000 libvhdi-20240303/libcthreads/libcthreads_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-03-03 08:06:41.000000 libvhdi-20240303/libcthreads/libcthreads_thread_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-03-03 08:06:41.000000 libvhdi-20240303/libcthreads/libcthreads_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-03-03 08:06:41.000000 libvhdi-20240303/libcthreads/libcthreads_thread_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-03-03 08:06:41.000000 libvhdi-20240303/libcthreads/libcthreads_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-03-03 08:06:41.000000 libvhdi-20240303/libcthreads/libcthreads_repeating_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31879 2024-03-03 08:07:00.000000 libvhdi-20240303/libcthreads/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-03-03 08:06:41.000000 libvhdi-20240303/libcthreads/libcthreads_queue.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2399 2024-03-03 08:07:14.000000 libvhdi-20240303/libvhdi.spec
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-03-03 08:07:00.000000 libvhdi-20240303/test-driver
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:00.000000 libvhdi-20240303/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-03-03 08:06:39.000000 libvhdi-20240303/libcpath/libcpath_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-03-03 08:06:39.000000 libvhdi-20240303/libcpath/libcpath_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-03-03 08:06:39.000000 libvhdi-20240303/libcpath/libcpath_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      842 2024-03-03 08:06:39.000000 libvhdi-20240303/libcpath/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-03-03 08:06:39.000000 libvhdi-20240303/libcpath/libcpath_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-03-03 08:06:39.000000 libvhdi-20240303/libcpath/libcpath_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-03-03 08:06:39.000000 libvhdi-20240303/libcpath/libcpath_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-03-03 08:06:39.000000 libvhdi-20240303/libcpath/libcpath_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-03-03 08:06:39.000000 libvhdi-20240303/libcpath/libcpath_libcsplit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-03-03 08:06:39.000000 libvhdi-20240303/libcpath/libcpath_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-03-03 08:06:39.000000 libvhdi-20240303/libcpath/libcpath_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-03-03 08:06:39.000000 libvhdi-20240303/libcpath/libcpath_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29067 2024-03-03 08:07:00.000000 libvhdi-20240303/libcpath/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-03-03 08:06:39.000000 libvhdi-20240303/libcpath/libcpath_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-03-03 08:06:39.000000 libvhdi-20240303/libcpath/libcpath_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-03-03 08:06:39.000000 libvhdi-20240303/libcpath/libcpath_path.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-03-03 08:06:39.000000 libvhdi-20240303/libcpath/libcpath_path.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1381 2023-12-03 09:15:01.000000 libvhdi-20240303/ChangeLog
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/manuals/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      154 2023-12-03 09:15:02.000000 libvhdi-20240303/manuals/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5718 2024-03-03 07:54:32.000000 libvhdi-20240303/manuals/libvhdi.3
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25988 2024-03-03 08:07:00.000000 libvhdi-20240303/manuals/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1418 2024-03-03 07:54:32.000000 libvhdi-20240303/manuals/vhdiinfo.1
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/tests/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1803 2024-03-03 07:54:32.000000 libvhdi-20240303/tests/vhdi_test_functions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-03-03 07:54:32.000000 libvhdi-20240303/tests/vhdi_test_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24047 2024-03-03 07:55:13.000000 libvhdi-20240303/tests/vhdi_test_file_footer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9809 2024-03-03 07:55:13.000000 libvhdi-20240303/tests/vhdi_test_parent_locator_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4123 2024-03-03 07:54:32.000000 libvhdi-20240303/tests/vhdi_test_tools_signal.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3313 2024-03-03 07:54:32.000000 libvhdi-20240303/tests/test_vhdiinfo.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6369 2024-03-03 07:55:13.000000 libvhdi-20240303/tests/vhdi_test_metadata_values.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4065 2024-03-03 07:55:55.000000 libvhdi-20240303/tests/test_tools.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6758 2024-03-03 07:55:13.000000 libvhdi-20240303/tests/vhdi_test_block_allocation_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    42352 2024-03-03 07:55:13.000000 libvhdi-20240303/tests/vhdi_test_image_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3424 2024-03-03 07:55:13.000000 libvhdi-20240303/tests/pyvhdi_test_support.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5590 2024-03-03 07:54:32.000000 libvhdi-20240303/tests/vhdi_test_tools_info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10722 2024-03-03 07:55:13.000000 libvhdi-20240303/tests/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13423 2024-03-03 07:55:13.000000 libvhdi-20240303/tests/pyvhdi_test_file.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3099 2024-03-03 07:54:32.000000 libvhdi-20240303/tests/vhdi_test_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-03-03 07:54:32.000000 libvhdi-20240303/tests/vhdi_test_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4064 2024-03-03 07:54:32.000000 libvhdi-20240303/tests/vhdi_test_checksum.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    55225 2024-03-03 07:55:13.000000 libvhdi-20240303/tests/vhdi_test_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13247 2024-03-03 07:54:32.000000 libvhdi-20240303/tests/vhdi_test_functions.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4653 2024-03-03 07:54:32.000000 libvhdi-20240303/tests/vhdi_test_memory.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6313 2024-03-03 07:55:13.000000 libvhdi-20240303/tests/vhdi_test_metadata_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1706 2024-03-03 07:54:32.000000 libvhdi-20240303/tests/vhdi_test_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36919 2024-03-03 07:55:13.000000 libvhdi-20240303/tests/vhdi_test_dynamic_disk_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4531 2024-03-03 07:54:32.000000 libvhdi-20240303/tests/vhdi_test_getopt.c
--rwxr--r--   0 lordyesta  (1000) lordyesta  (1000)     1653 2024-03-03 07:54:32.000000 libvhdi-20240303/tests/test_manpage.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9669 2024-03-03 07:55:13.000000 libvhdi-20240303/tests/vhdi_test_parent_locator_entry.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4073 2024-03-03 07:54:32.000000 libvhdi-20240303/tests/test_python_module.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-03-03 07:54:32.000000 libvhdi-20240303/tests/vhdi_test_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1691 2024-03-03 07:54:32.000000 libvhdi-20240303/tests/vhdi_test_memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12143 2024-03-03 07:55:13.000000 libvhdi-20240303/tests/vhdi_test_block_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14178 2024-03-03 07:55:13.000000 libvhdi-20240303/tests/vhdi_test_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6201 2024-03-03 07:55:13.000000 libvhdi-20240303/tests/vhdi_test_region_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6817 2024-03-03 07:55:13.000000 libvhdi-20240303/tests/vhdi_test_sector_range_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1367 2024-03-03 07:54:32.000000 libvhdi-20240303/tests/vhdi_test_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4276 2024-03-03 07:54:32.000000 libvhdi-20240303/tests/vhdi_test_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-03-03 07:55:13.000000 libvhdi-20240303/tests/vhdi_test_region_table_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-03-03 07:54:32.000000 libvhdi-20240303/tests/test_runner.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-03-03 07:54:32.000000 libvhdi-20240303/tests/vhdi_test_libvhdi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8018 2024-03-03 07:55:13.000000 libvhdi-20240303/tests/vhdi_test_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1808 2024-03-03 07:54:32.000000 libvhdi-20240303/tests/vhdi_test_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-03-03 07:54:32.000000 libvhdi-20240303/tests/vhdi_test_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2425 2024-03-03 07:54:32.000000 libvhdi-20240303/tests/vhdi_test_tools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10465 2024-03-03 07:55:13.000000 libvhdi-20240303/tests/vhdi_test_metadata_table_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-03-03 07:54:32.000000 libvhdi-20240303/tests/vhdi_test_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18202 2024-03-03 07:55:13.000000 libvhdi-20240303/tests/vhdi_test_file_information.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    76059 2024-03-03 08:07:00.000000 libvhdi-20240303/tests/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10435 2024-03-03 07:55:13.000000 libvhdi-20240303/tests/vhdi_test_metadata_table_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8539 2024-03-03 07:54:32.000000 libvhdi-20240303/tests/vhdi_test_macros.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10217 2024-03-03 07:55:13.000000 libvhdi-20240303/tests/vhdi_test_region_table_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6313 2024-03-03 07:55:13.000000 libvhdi-20240303/tests/vhdi_test_parent_locator.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4391 2024-03-03 07:55:55.000000 libvhdi-20240303/tests/test_library.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      678 2024-03-03 07:54:29.000000 libvhdi-20240303/libvhdi.pc.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:00.000000 libvhdi-20240303/vhditools/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5895 2024-03-03 07:55:55.000000 libvhdi-20240303/vhditools/vhdiinfo.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5726 2024-03-03 07:54:32.000000 libvhdi-20240303/vhditools/vhditools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37173 2024-03-03 07:54:32.000000 libvhdi-20240303/vhditools/mount_dokan.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2955 2024-03-03 07:54:32.000000 libvhdi-20240303/vhditools/mount_file_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26443 2024-03-03 07:54:32.000000 libvhdi-20240303/vhditools/mount_fuse.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1932 2024-03-03 07:55:55.000000 libvhdi-20240303/vhditools/info_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4531 2024-03-03 07:54:32.000000 libvhdi-20240303/vhditools/vhditools_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5414 2024-03-03 07:54:32.000000 libvhdi-20240303/vhditools/mount_dokan.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1498 2024-03-03 07:54:32.000000 libvhdi-20240303/vhditools/vhditools_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3927 2024-03-03 07:54:32.000000 libvhdi-20240303/vhditools/vhditools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1501 2024-03-03 07:54:32.000000 libvhdi-20240303/vhditools/vhditools_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18788 2024-03-03 07:55:55.000000 libvhdi-20240303/vhditools/mount_file_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2024-03-03 07:54:32.000000 libvhdi-20240303/vhditools/vhditools_output.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1210 2024-03-03 07:54:32.000000 libvhdi-20240303/vhditools/vhditools_i18n.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-03-03 07:54:32.000000 libvhdi-20240303/vhditools/vhditools_signal.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10552 2024-03-03 07:54:32.000000 libvhdi-20240303/vhditools/byte_size_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1406 2024-03-03 07:54:32.000000 libvhdi-20240303/vhditools/vhditools_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2245 2023-12-03 09:15:04.000000 libvhdi-20240303/vhditools/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20694 2024-03-03 07:55:55.000000 libvhdi-20240303/vhditools/mount_file_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16485 2024-03-03 07:55:55.000000 libvhdi-20240303/vhditools/info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-03-03 07:54:32.000000 libvhdi-20240303/vhditools/vhditools_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3608 2024-03-03 07:54:32.000000 libvhdi-20240303/vhditools/mount_file_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-03-03 07:54:32.000000 libvhdi-20240303/vhditools/vhditools_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1480 2024-03-03 07:54:32.000000 libvhdi-20240303/vhditools/vhditools_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1808 2024-03-03 07:54:32.000000 libvhdi-20240303/vhditools/vhditools_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1778 2024-03-03 07:54:32.000000 libvhdi-20240303/vhditools/vhditools_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15191 2024-03-03 07:55:55.000000 libvhdi-20240303/vhditools/vhdimount.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2664 2024-03-03 07:54:32.000000 libvhdi-20240303/vhditools/mount_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-03-03 07:54:32.000000 libvhdi-20240303/vhditools/vhditools_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1745 2024-03-03 07:54:32.000000 libvhdi-20240303/vhditools/vhditools_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22344 2024-03-03 07:55:55.000000 libvhdi-20240303/vhditools/mount_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-03-03 07:54:32.000000 libvhdi-20240303/vhditools/vhditools_libvhdi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33263 2024-03-03 08:07:00.000000 libvhdi-20240303/vhditools/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-03-03 07:54:32.000000 libvhdi-20240303/vhditools/byte_size_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2762 2024-03-03 07:54:32.000000 libvhdi-20240303/vhditools/mount_fuse.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:01.000000 libvhdi-20240303/ossfuzz/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      967 2024-03-03 07:54:31.000000 libvhdi-20240303/ossfuzz/ossfuzz_libvhdi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      889 2023-12-03 09:15:09.000000 libvhdi-20240303/ossfuzz/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-03-03 07:54:31.000000 libvhdi-20240303/ossfuzz/ossfuzz_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2199 2024-03-03 07:54:31.000000 libvhdi-20240303/ossfuzz/file_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31221 2024-03-03 08:07:00.000000 libvhdi-20240303/ossfuzz/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-03-03 08:06:52.000000 libvhdi-20240303/ltmain.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:22:59.000000 libvhdi-20240303/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-03-03 08:06:40.000000 libvhdi-20240303/libcsplit/libcsplit_narrow_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-03-03 08:06:40.000000 libvhdi-20240303/libcsplit/libcsplit_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-03-03 08:06:40.000000 libvhdi-20240303/libcsplit/libcsplit_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-03-03 08:06:40.000000 libvhdi-20240303/libcsplit/libcsplit_wide_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-03-03 08:06:40.000000 libvhdi-20240303/libcsplit/libcsplit_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      884 2024-03-03 08:06:40.000000 libvhdi-20240303/libcsplit/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-03-03 08:06:40.000000 libvhdi-20240303/libcsplit/libcsplit_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-03-03 08:06:40.000000 libvhdi-20240303/libcsplit/libcsplit_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-03-03 08:06:40.000000 libvhdi-20240303/libcsplit/libcsplit_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-03-03 08:06:40.000000 libvhdi-20240303/libcsplit/libcsplit_wide_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-03-03 08:06:40.000000 libvhdi-20240303/libcsplit/libcsplit_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-03-03 08:06:40.000000 libvhdi-20240303/libcsplit/libcsplit_narrow_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-03-03 08:06:40.000000 libvhdi-20240303/libcsplit/libcsplit_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-03-03 08:06:40.000000 libvhdi-20240303/libcsplit/libcsplit_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-03-03 08:06:40.000000 libvhdi-20240303/libcsplit/libcsplit_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-03-03 08:06:40.000000 libvhdi-20240303/libcsplit/libcsplit_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29847 2024-03-03 08:07:00.000000 libvhdi-20240303/libcsplit/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-03-03 08:06:40.000000 libvhdi-20240303/libcsplit/libcsplit_narrow_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-03-03 08:06:40.000000 libvhdi-20240303/libcsplit/libcsplit_narrow_string.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:00.000000 libvhdi-20240303/libvhdi/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2609 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_region_type_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2423 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_file_footer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1395 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21525 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_dynamic_disk_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1485 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23167 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_block_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16640 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_parent_locator_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1700 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13950 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_image_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3053 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_block_descriptor.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1991 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1829 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_region_type_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2103 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1916 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_file_information.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1348 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_i18n.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2491 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/vhdi_file_footer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1956 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3349 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_checksum.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1780 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_metadata_table_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1087 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi.rc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19781 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_block_allocation_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4580 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3240 2023-12-03 09:15:05.000000 libvhdi-20240303/libvhdi/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1886 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_region_table_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32903 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_metadata_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8068 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_file_information.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1542 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_libfdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2627 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_parent_locator_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1085 2024-03-03 08:07:14.000000 libvhdi-20240303/libvhdi/libvhdi.rc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1987 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/vhdi_region_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10962 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_metadata_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3342 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_sector_range_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1707 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_i18n.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6784 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_metadata_table_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2846 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1688 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_sector_range_descriptor.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1780 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_parent_locator_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2844 2024-03-03 08:07:14.000000 libvhdi-20240303/libvhdi/libvhdi_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1827 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1859 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_metadata_table_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6440 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_parent_locator_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_metadata_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12001 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_region_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2084 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_region_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2349 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/vhdi_dynamic_disk_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1496 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_checksum.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2009 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/vhdi_metadata_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2213 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/vhdi_image_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14914 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_file_footer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1944 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/vhdi_parent_locator.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7984 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6598 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_region_table_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_parent_locator.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7278 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_metadata_table_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4109 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_metadata_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8384 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    95646 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1791 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_region_table_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11013 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2229 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_metadata_item_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38888 2024-03-03 08:07:00.000000 libvhdi-20240303/libvhdi/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11851 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_parent_locator.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3379 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_dynamic_disk_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2358 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_image_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3648 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_metadata_item_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2894 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_block_allocation_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6507 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/libvhdi_region_table_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-03-03 07:54:31.000000 libvhdi-20240303/libvhdi/vhdi_file_information.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:23:00.000000 libvhdi-20240303/po/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:15:03.000000 libvhdi-20240303/po/remove-potcdate.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:15:03.000000 libvhdi-20240303/po/POTFILES.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:15:03.000000 libvhdi-20240303/po/Makefile.in.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:15:03.000000 libvhdi-20240303/po/quot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:15:03.000000 libvhdi-20240303/po/en@quot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:15:03.000000 libvhdi-20240303/po/en@boldquot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:15:03.000000 libvhdi-20240303/po/boldquot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:15:03.000000 libvhdi-20240303/po/insert-header.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:15:04.000000 libvhdi-20240303/po/ChangeLog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1853 2024-03-03 08:07:14.000000 libvhdi-20240303/po/Makevars
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:15:04.000000 libvhdi-20240303/po/Makevars.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:15:03.000000 libvhdi-20240303/po/Rules-quot
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:22:59.000000 libvhdi-20240303/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_windows_1251.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_base16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_utf8_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_iso_8859_2.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_windows_932.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_mac_dingbats.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_base64_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_mac_turkish.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_unicode_character.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_mac_gaelic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_mac_arabic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_mac_thai.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_windows_874.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_iso_8859_15.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_iso_8859_16.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_windows_1255.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_utf7_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_koi8_u.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_iso_8859_6.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_iso_8859_14.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_base64_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_mac_centraleurroman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_mac_romanian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_iso_8859_6.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_iso_8859_9.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_mac_russian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_mac_dingbats.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_iso_8859_15.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_windows_936.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_mac_croatian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_scsu.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4197 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_utf32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_windows_936.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_iso_8859_10.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_mac_roman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_utf7_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_iso_8859_3.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_mac_thai.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_mac_farsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_mac_ukrainian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_mac_inuit.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_windows_932.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_windows_874.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_iso_8859_5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_iso_8859_10.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_url_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_mac_icelandic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_koi8_u.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_utf16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_windows_1253.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_iso_8859_4.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_mac_greek.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_mac_centraleurroman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_windows_1254.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_iso_8859_13.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_iso_8859_7.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_windows_1255.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_unicode_character.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_iso_8859_8.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_iso_8859_13.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_windows_949.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_mac_cyrillic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_mac_celtic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_iso_8859_4.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_windows_949.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_utf16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_mac_symbol.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_mac_roman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_windows_1257.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_windows_1254.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_windows_950.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_windows_1256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_base32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_windows_1253.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_iso_8859_16.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_utf8_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_windows_1250.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_iso_8859_2.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_koi8_r.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_iso_8859_5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_utf32_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_mac_icelandic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_windows_1256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_utf32_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_mac_romanian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_iso_8859_8.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_koi8_r.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_mac_cyrillic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_mac_arabic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_mac_croatian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_iso_8859_9.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_mac_greek.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_windows_1258.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_iso_8859_7.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    52591 2024-03-03 08:07:00.000000 libvhdi-20240303/libuna/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_iso_8859_3.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_windows_1250.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_scsu.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_windows_1252.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_mac_turkish.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_mac_ukrainian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_mac_russian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_windows_1258.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_mac_celtic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_byte_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_mac_gaelic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_utf32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_mac_symbol.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_windows_1257.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_mac_inuit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_mac_farsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_windows_950.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_url_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_windows_1251.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_windows_1252.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_codepage_iso_8859_14.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_base16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-03-03 08:06:47.000000 libvhdi-20240303/libuna/libuna_base32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39981 2024-03-03 08:06:59.000000 libvhdi-20240303/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:22:59.000000 libvhdi-20240303/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-03-03 08:06:37.000000 libvhdi-20240303/libcnotify/libcnotify_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-03-03 08:06:37.000000 libvhdi-20240303/libcnotify/libcnotify_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-03-03 08:06:37.000000 libvhdi-20240303/libcnotify/libcnotify_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-03-03 08:06:37.000000 libvhdi-20240303/libcnotify/libcnotify_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      728 2024-03-03 08:06:37.000000 libvhdi-20240303/libcnotify/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-03-03 08:06:37.000000 libvhdi-20240303/libcnotify/libcnotify_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-03-03 08:06:37.000000 libvhdi-20240303/libcnotify/libcnotify_verbose.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-03-03 08:06:37.000000 libvhdi-20240303/libcnotify/libcnotify_print.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-03-03 08:06:37.000000 libvhdi-20240303/libcnotify/libcnotify_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-03-03 08:06:37.000000 libvhdi-20240303/libcnotify/libcnotify_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-03-03 08:06:37.000000 libvhdi-20240303/libcnotify/libcnotify_verbose.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28901 2024-03-03 08:07:00.000000 libvhdi-20240303/libcnotify/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-03-03 08:06:37.000000 libvhdi-20240303/libcnotify/libcnotify_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-03-03 08:06:37.000000 libvhdi-20240303/libcnotify/libcnotify_print.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-03 08:22:59.000000 libvhdi-20240303/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-03-03 08:06:33.000000 libvhdi-20240303/libcerror/libcerror_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-03-03 08:06:33.000000 libvhdi-20240303/libcerror/libcerror_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-03-03 08:06:33.000000 libvhdi-20240303/libcerror/libcerror_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      640 2024-03-03 08:06:33.000000 libvhdi-20240303/libcerror/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-03-03 08:06:33.000000 libvhdi-20240303/libcerror/libcerror_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-03-03 08:06:33.000000 libvhdi-20240303/libcerror/libcerror_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-03-03 08:06:33.000000 libvhdi-20240303/libcerror/libcerror_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-03-03 08:06:33.000000 libvhdi-20240303/libcerror/libcerror_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-03-03 08:06:33.000000 libvhdi-20240303/libcerror/libcerror_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-03-03 08:06:33.000000 libvhdi-20240303/libcerror/libcerror_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-03-03 08:06:33.000000 libvhdi-20240303/libcerror/libcerror_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28414 2024-03-03 08:07:00.000000 libvhdi-20240303/libcerror/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56793 2024-03-03 08:06:55.000000 libvhdi-20240303/aclocal.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7443 2024-03-03 07:54:29.000000 libvhdi-20240303/configure.ac
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      411 2024-03-03 08:23:01.995611 libvhdi-20240303/PKG-INFO
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:12.000000 libvhdi-20240509/libfdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-09 05:22:04.000000 libvhdi-20240509/libfdata/libfdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37893 2024-05-09 05:22:04.000000 libvhdi-20240509/libfdata/libfdata_area.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9700 2024-05-09 05:22:04.000000 libvhdi-20240509/libfdata/libfdata_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2024-05-09 05:22:04.000000 libvhdi-20240509/libfdata/libfdata_cache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30931 2024-05-09 05:22:04.000000 libvhdi-20240509/libfdata/libfdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2024-05-09 05:22:04.000000 libvhdi-20240509/libfdata/libfdata_mapped_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-09 05:22:04.000000 libvhdi-20240509/libfdata/libfdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6533 2024-05-09 05:22:04.000000 libvhdi-20240509/libfdata/libfdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   107689 2024-05-09 05:22:04.000000 libvhdi-20240509/libfdata/libfdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-05-09 05:22:04.000000 libvhdi-20240509/libfdata/libfdata_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12090 2024-05-09 05:22:04.000000 libvhdi-20240509/libfdata/libfdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4017 2024-05-09 05:22:04.000000 libvhdi-20240509/libfdata/libfdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1287 2024-05-09 05:22:04.000000 libvhdi-20240509/libfdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-09 05:22:04.000000 libvhdi-20240509/libfdata/libfdata_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-09 05:22:04.000000 libvhdi-20240509/libfdata/libfdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-05-09 05:22:04.000000 libvhdi-20240509/libfdata/libfdata_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-05-09 05:22:04.000000 libvhdi-20240509/libfdata/libfdata_cache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66203 2024-05-09 05:22:04.000000 libvhdi-20240509/libfdata/libfdata_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-09 05:22:04.000000 libvhdi-20240509/libfdata/libfdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2092 2024-05-09 05:22:04.000000 libvhdi-20240509/libfdata/libfdata_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7327 2024-05-09 05:22:04.000000 libvhdi-20240509/libfdata/libfdata_area.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-09 05:22:04.000000 libvhdi-20240509/libfdata/libfdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-05-09 05:22:04.000000 libvhdi-20240509/libfdata/libfdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2024-05-09 05:22:04.000000 libvhdi-20240509/libfdata/libfdata_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1995 2024-05-09 05:22:04.000000 libvhdi-20240509/libfdata/libfdata_mapped_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2024-05-09 05:22:04.000000 libvhdi-20240509/libfdata/libfdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19329 2024-05-09 05:22:04.000000 libvhdi-20240509/libfdata/libfdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21271 2024-05-09 05:22:04.000000 libvhdi-20240509/libfdata/libfdata_segments_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2054 2024-05-09 05:22:04.000000 libvhdi-20240509/libfdata/libfdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-05-09 05:22:04.000000 libvhdi-20240509/libfdata/libfdata_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6013 2024-05-09 05:22:04.000000 libvhdi-20240509/libfdata/libfdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2804 2024-05-09 05:22:04.000000 libvhdi-20240509/libfdata/libfdata_segments_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32874 2024-05-09 05:22:19.000000 libvhdi-20240509/libfdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49670 2024-05-09 05:22:04.000000 libvhdi-20240509/libfdata/libfdata_vector.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-09 05:22:04.000000 libvhdi-20240509/libfdata/libfdata_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7810 2024-05-09 05:22:04.000000 libvhdi-20240509/libfdata/libfdata_vector.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-05-09 04:49:46.000000 libvhdi-20240509/COPYING
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-05-09 05:22:18.000000 libvhdi-20240509/install-sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 04:49:46.000000 libvhdi-20240509/NEWS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-05-09 05:22:19.000000 libvhdi-20240509/depcomp
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:12.000000 libvhdi-20240509/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-09 05:22:05.000000 libvhdi-20240509/libfguid/libfguid_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2024-05-09 05:22:05.000000 libvhdi-20240509/libfguid/libfguid_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2024-05-09 05:22:05.000000 libvhdi-20240509/libfguid/libfguid_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-09 05:22:05.000000 libvhdi-20240509/libfguid/libfguid_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      677 2024-05-09 05:22:05.000000 libvhdi-20240509/libfguid/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-09 05:22:05.000000 libvhdi-20240509/libfguid/libfguid_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-09 05:22:05.000000 libvhdi-20240509/libfguid/libfguid_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-05-09 05:22:05.000000 libvhdi-20240509/libfguid/libfguid_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2024-05-09 05:22:05.000000 libvhdi-20240509/libfguid/libfguid_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2024-05-09 05:22:05.000000 libvhdi-20240509/libfguid/libfguid_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-05-09 05:22:05.000000 libvhdi-20240509/libfguid/libfguid_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28675 2024-05-09 05:22:19.000000 libvhdi-20240509/libfguid/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-09 05:22:05.000000 libvhdi-20240509/libfguid/libfguid_error.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:11.000000 libvhdi-20240509/m4/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11734 2024-05-09 04:49:53.000000 libvhdi-20240509/m4/libcfile.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:15:05.000000 libvhdi-20240509/m4/tests.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9615 2024-05-09 04:49:53.000000 libvhdi-20240509/m4/libcpath.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:15:04.000000 libvhdi-20240509/m4/lib-prefix.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:15:05.000000 libvhdi-20240509/m4/progtest.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31495 2024-05-09 04:49:53.000000 libvhdi-20240509/m4/libuna.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:15:04.000000 libvhdi-20240509/m4/gettext.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:15:04.000000 libvhdi-20240509/m4/lib-ld.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8476 2024-05-09 04:49:53.000000 libvhdi-20240509/m4/libclocale.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17383 2024-05-09 04:49:53.000000 libvhdi-20240509/m4/libcdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7625 2024-05-09 04:49:53.000000 libvhdi-20240509/m4/libcsplit.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14127 2024-03-11 05:00:57.000000 libvhdi-20240509/m4/common.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11362 2024-05-09 04:49:53.000000 libvhdi-20240509/m4/libcthreads.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-05-09 05:22:12.000000 libvhdi-20240509/m4/ltversion.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-05-09 05:22:12.000000 libvhdi-20240509/m4/ltsugar.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15781 2024-05-09 04:49:53.000000 libvhdi-20240509/m4/libfdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:15:04.000000 libvhdi-20240509/m4/host-cpu-c-abi.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7058 2024-05-09 04:49:53.000000 libvhdi-20240509/m4/libfuse.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-05-09 05:22:12.000000 libvhdi-20240509/m4/libtool.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:15:04.000000 libvhdi-20240509/m4/po.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6501 2024-05-09 04:49:53.000000 libvhdi-20240509/m4/libcerror.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5886 2024-05-09 04:49:53.000000 libvhdi-20240509/m4/libcnotify.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5876 2024-05-09 04:49:53.000000 libvhdi-20240509/m4/libfguid.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11923 2024-05-09 04:49:53.000000 libvhdi-20240509/m4/libbfio.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:15:04.000000 libvhdi-20240509/m4/intlmacosx.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-05-09 05:22:13.000000 libvhdi-20240509/m4/lt~obsolete.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:15:04.000000 libvhdi-20240509/m4/lib-link.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:15:04.000000 libvhdi-20240509/m4/iconv.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-05-09 05:22:12.000000 libvhdi-20240509/m4/ltoptions.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:15:04.000000 libvhdi-20240509/m4/nls.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6476 2024-05-09 04:49:53.000000 libvhdi-20240509/m4/python.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:15:04.000000 libvhdi-20240509/m4/types.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7566 2024-05-09 04:49:53.000000 libvhdi-20240509/m4/libfcache.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2024-03-11 05:00:57.000000 libvhdi-20240509/m4/pthread.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:11.000000 libvhdi-20240509/include/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      410 2024-05-09 05:02:13.000000 libvhdi-20240509/include/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12120 2024-05-09 05:22:31.000000 libvhdi-20240509/include/libvhdi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12120 2024-05-09 04:49:49.000000 libvhdi-20240509/include/libvhdi.h.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:11.000000 libvhdi-20240509/include/libvhdi/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2125 2024-05-09 04:49:49.000000 libvhdi-20240509/include/libvhdi/definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2123 2024-05-09 05:22:31.000000 libvhdi-20240509/include/libvhdi/definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4933 2024-05-09 04:49:49.000000 libvhdi-20240509/include/libvhdi/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4802 2024-05-09 05:22:31.000000 libvhdi-20240509/include/libvhdi/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1539 2024-05-09 04:49:49.000000 libvhdi-20240509/include/libvhdi/features.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6689 2024-05-09 04:49:49.000000 libvhdi-20240509/include/libvhdi/error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-05-09 04:49:49.000000 libvhdi-20240509/include/libvhdi/extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1475 2024-05-09 05:22:31.000000 libvhdi-20240509/include/libvhdi/features.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5195 2024-05-09 04:49:49.000000 libvhdi-20240509/include/libvhdi/codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27032 2024-05-09 05:22:19.000000 libvhdi-20240509/include/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:11.000000 libvhdi-20240509/common/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-05-09 04:49:48.000000 libvhdi-20240509/common/config_borlandc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-05-09 04:49:49.000000 libvhdi-20240509/common/file_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-05-09 04:49:49.000000 libvhdi-20240509/common/memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-05-09 04:49:48.000000 libvhdi-20240509/common/byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-05-09 04:49:48.000000 libvhdi-20240509/common/common.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-05-09 04:49:49.000000 libvhdi-20240509/common/config_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-05-09 04:49:49.000000 libvhdi-20240509/common/system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      343 2024-05-09 05:02:13.000000 libvhdi-20240509/common/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-05-09 04:49:49.000000 libvhdi-20240509/common/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7373 2024-05-09 05:22:31.000000 libvhdi-20240509/common/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16257 2024-05-09 05:22:18.000000 libvhdi-20240509/common/config.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17220 2024-05-09 05:22:31.000000 libvhdi-20240509/common/config.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-05-09 04:49:49.000000 libvhdi-20240509/common/wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-05-09 04:49:49.000000 libvhdi-20240509/common/narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-05-09 04:49:49.000000 libvhdi-20240509/common/config_msc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24085 2024-05-09 05:22:19.000000 libvhdi-20240509/common/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:11.000000 libvhdi-20240509/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-05-09 05:21:56.000000 libvhdi-20240509/libclocale/libclocale_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-05-09 05:21:56.000000 libvhdi-20240509/libclocale/libclocale_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      775 2024-05-09 05:21:56.000000 libvhdi-20240509/libclocale/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-05-09 05:21:56.000000 libvhdi-20240509/libclocale/libclocale_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-05-09 05:21:56.000000 libvhdi-20240509/libclocale/libclocale_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-05-09 05:21:56.000000 libvhdi-20240509/libclocale/libclocale_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-05-09 05:21:56.000000 libvhdi-20240509/libclocale/libclocale_locale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-05-09 05:21:56.000000 libvhdi-20240509/libclocale/libclocale_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-05-09 05:21:56.000000 libvhdi-20240509/libclocale/libclocale_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-05-09 05:21:56.000000 libvhdi-20240509/libclocale/libclocale_locale.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29283 2024-05-09 05:22:19.000000 libvhdi-20240509/libclocale/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-05-09 05:21:56.000000 libvhdi-20240509/libclocale/libclocale_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-05-09 05:21:56.000000 libvhdi-20240509/libclocale/libclocale_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-05-09 05:21:56.000000 libvhdi-20240509/libclocale/libclocale_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3274 2024-05-09 04:49:46.000000 libvhdi-20240509/libvhdi.spec.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:12.000000 libvhdi-20240509/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-05-09 05:22:02.000000 libvhdi-20240509/libfcache/libfcache_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2024-05-09 05:22:02.000000 libvhdi-20240509/libfcache/libfcache_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2024-05-09 05:22:02.000000 libvhdi-20240509/libfcache/libfcache_cache_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-09 05:22:02.000000 libvhdi-20240509/libfcache/libfcache_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      876 2024-05-09 05:22:03.000000 libvhdi-20240509/libfcache/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-09 05:22:02.000000 libvhdi-20240509/libfcache/libfcache_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-09 05:22:02.000000 libvhdi-20240509/libfcache/libfcache_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2024-05-09 05:22:02.000000 libvhdi-20240509/libfcache/libfcache_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2024-05-09 05:22:02.000000 libvhdi-20240509/libfcache/libfcache_cache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-05-09 05:22:02.000000 libvhdi-20240509/libfcache/libfcache_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-09 05:22:02.000000 libvhdi-20240509/libfcache/libfcache_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2024-05-09 05:22:02.000000 libvhdi-20240509/libfcache/libfcache_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-09 05:22:02.000000 libvhdi-20240509/libfcache/libfcache_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2024-05-09 05:22:02.000000 libvhdi-20240509/libfcache/libfcache_cache_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29792 2024-05-09 05:22:19.000000 libvhdi-20240509/libfcache/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-05-09 05:22:02.000000 libvhdi-20240509/libfcache/libfcache_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-05-09 05:22:03.000000 libvhdi-20240509/libfcache/libfcache_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2024-05-09 05:22:02.000000 libvhdi-20240509/libfcache/libfcache_cache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2015 2024-05-09 05:05:24.000000 libvhdi-20240509/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:12.000000 libvhdi-20240509/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-05-09 05:21:51.000000 libvhdi-20240509/libbfio/libbfio_file_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-05-09 05:21:51.000000 libvhdi-20240509/libbfio/libbfio_file_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-05-09 05:21:51.000000 libvhdi-20240509/libbfio/libbfio_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-05-09 05:21:51.000000 libvhdi-20240509/libbfio/libbfio_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-05-09 05:21:51.000000 libvhdi-20240509/libbfio/libbfio_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-09 05:21:51.000000 libvhdi-20240509/libbfio/libbfio_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-05-09 05:21:51.000000 libvhdi-20240509/libbfio/libbfio_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-05-09 05:21:51.000000 libvhdi-20240509/libbfio/libbfio_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-05-09 05:21:51.000000 libvhdi-20240509/libbfio/libbfio_file_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-05-09 05:21:51.000000 libvhdi-20240509/libbfio/libbfio_file_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-05-09 05:21:51.000000 libvhdi-20240509/libbfio/libbfio_file_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-05-09 05:21:51.000000 libvhdi-20240509/libbfio/libbfio_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-05-09 05:21:51.000000 libvhdi-20240509/libbfio/libbfio_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-05-09 05:21:51.000000 libvhdi-20240509/libbfio/libbfio_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-05-09 05:21:51.000000 libvhdi-20240509/libbfio/libbfio_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2024-05-09 05:21:51.000000 libvhdi-20240509/libbfio/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-05-09 05:21:51.000000 libvhdi-20240509/libbfio/libbfio_libcfile.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-05-09 05:21:51.000000 libvhdi-20240509/libbfio/libbfio_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-05-09 05:21:51.000000 libvhdi-20240509/libbfio/libbfio_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-05-09 05:21:51.000000 libvhdi-20240509/libbfio/libbfio_file_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-05-09 05:21:51.000000 libvhdi-20240509/libbfio/libbfio_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-09 05:21:51.000000 libvhdi-20240509/libbfio/libbfio_memory_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-05-09 05:21:51.000000 libvhdi-20240509/libbfio/libbfio_file_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-05-09 05:21:51.000000 libvhdi-20240509/libbfio/libbfio_file_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-05-09 05:21:51.000000 libvhdi-20240509/libbfio/libbfio_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-05-09 05:21:51.000000 libvhdi-20240509/libbfio/libbfio_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-05-09 05:21:51.000000 libvhdi-20240509/libbfio/libbfio_memory_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-05-09 05:21:51.000000 libvhdi-20240509/libbfio/libbfio_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-05-09 05:21:51.000000 libvhdi-20240509/libbfio/libbfio_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-05-09 05:21:51.000000 libvhdi-20240509/libbfio/libbfio_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-05-09 05:21:51.000000 libvhdi-20240509/libbfio/libbfio_memory_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-05-09 05:21:51.000000 libvhdi-20240509/libbfio/libbfio_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-05-09 05:21:51.000000 libvhdi-20240509/libbfio/libbfio_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33135 2024-05-09 05:22:19.000000 libvhdi-20240509/libbfio/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-05-09 05:21:51.000000 libvhdi-20240509/libbfio/libbfio_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-05-09 05:21:51.000000 libvhdi-20240509/libbfio/libbfio_memory_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-05-09 05:21:51.000000 libvhdi-20240509/libbfio/libbfio_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-05-09 05:21:51.000000 libvhdi-20240509/libbfio/libbfio_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:15:01.000000 libvhdi-20240509/ABOUT-NLS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-05-09 05:22:18.000000 libvhdi-20240509/config.guess
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:11.000000 libvhdi-20240509/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1024 2024-05-09 04:49:53.000000 libvhdi-20240509/dpkg/copyright
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-05-09 04:49:46.000000 libvhdi-20240509/dpkg/libvhdi-tools.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-05-09 04:49:46.000000 libvhdi-20240509/dpkg/libvhdi.install
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:11.000000 libvhdi-20240509/dpkg/source/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-05-09 04:49:46.000000 libvhdi-20240509/dpkg/source/format
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2106 2024-05-09 04:49:46.000000 libvhdi-20240509/dpkg/control
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      761 2024-05-09 04:49:46.000000 libvhdi-20240509/dpkg/rules
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      120 2024-05-09 04:49:46.000000 libvhdi-20240509/dpkg/changelog.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      139 2024-05-09 05:22:31.000000 libvhdi-20240509/dpkg/changelog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-05-09 04:49:46.000000 libvhdi-20240509/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-05-09 04:49:46.000000 libvhdi-20240509/dpkg/libvhdi-dev.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-05-09 04:49:46.000000 libvhdi-20240509/dpkg/libvhdi-python3.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      479 2024-05-09 05:22:31.000000 libvhdi-20240509/setup.cfg
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-05-09 04:49:46.000000 libvhdi-20240509/COPYING.LESSER
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1712450 2024-05-09 05:22:17.000000 libvhdi-20240509/configure
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-05-09 05:22:18.000000 libvhdi-20240509/compile
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-05-09 05:22:18.000000 libvhdi-20240509/missing
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/libfdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6858 2024-05-09 04:50:14.000000 libvhdi-20240509/msvscpp/libfdata/libfdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/vhdi_test_dynamic_disk_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6016 2024-05-09 04:50:14.000000 libvhdi-20240509/msvscpp/vhdi_test_dynamic_disk_header/vhdi_test_dynamic_disk_header.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/vhdi_test_tools_info_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6008 2024-05-09 04:50:44.000000 libvhdi-20240509/msvscpp/vhdi_test_tools_info_handle/vhdi_test_tools_info_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/vhdi_test_region_table_entry/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5766 2024-05-09 04:50:14.000000 libvhdi-20240509/msvscpp/vhdi_test_region_table_entry/vhdi_test_region_table_entry.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/vhdi_test_region_table/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5748 2024-05-09 04:50:44.000000 libvhdi-20240509/msvscpp/vhdi_test_region_table/vhdi_test_region_table.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/vhdi_test_io_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5739 2024-05-09 04:50:14.000000 libvhdi-20240509/msvscpp/vhdi_test_io_handle/vhdi_test_io_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/vhdi_test_block_allocation_table/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5778 2024-05-09 04:50:44.000000 libvhdi-20240509/msvscpp/vhdi_test_block_allocation_table/vhdi_test_block_allocation_table.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/vhdi_test_parent_locator_entry/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5772 2024-05-09 04:50:14.000000 libvhdi-20240509/msvscpp/vhdi_test_parent_locator_entry/vhdi_test_parent_locator_entry.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/vhdi_test_support/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6388 2024-05-09 04:50:14.000000 libvhdi-20240509/msvscpp/vhdi_test_support/vhdi_test_support.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/vhdi_test_parent_locator_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5775 2024-05-09 04:50:14.000000 libvhdi-20240509/msvscpp/vhdi_test_parent_locator_header/vhdi_test_parent_locator_header.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/vhdi_test_metadata_table_entry/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5772 2024-05-09 04:50:14.000000 libvhdi-20240509/msvscpp/vhdi_test_metadata_table_entry/vhdi_test_metadata_table_entry.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2024-05-09 04:50:14.000000 libvhdi-20240509/msvscpp/libfguid/libfguid.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/vhdi_test_tools_output/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5675 2024-05-09 04:50:14.000000 libvhdi-20240509/msvscpp/vhdi_test_tools_output/vhdi_test_tools_output.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/vhdi_test_image_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5995 2024-05-09 04:50:14.000000 libvhdi-20240509/msvscpp/vhdi_test_image_header/vhdi_test_image_header.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/vhdi_test_error/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5484 2024-05-09 04:50:14.000000 libvhdi-20240509/msvscpp/vhdi_test_error/vhdi_test_error.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-05-09 04:50:14.000000 libvhdi-20240509/msvscpp/libclocale/libclocale.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2024-05-09 04:50:14.000000 libvhdi-20240509/msvscpp/libfcache/libfcache.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/vhdi_test_tools_signal/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5675 2024-05-09 04:50:14.000000 libvhdi-20240509/msvscpp/vhdi_test_tools_signal/vhdi_test_tools_signal.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2175 2024-05-09 05:02:27.000000 libvhdi-20240509/msvscpp/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-05-09 04:50:14.000000 libvhdi-20240509/msvscpp/libbfio/libbfio.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/vhdi_test_sector_range_descriptor/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5781 2024-05-09 04:50:14.000000 libvhdi-20240509/msvscpp/vhdi_test_sector_range_descriptor/vhdi_test_sector_range_descriptor.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/vhdi_test_parent_locator/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5754 2024-05-09 04:50:14.000000 libvhdi-20240509/msvscpp/vhdi_test_parent_locator/vhdi_test_parent_locator.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/vhdi_test_block_descriptor/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5760 2024-05-09 04:50:14.000000 libvhdi-20240509/msvscpp/vhdi_test_block_descriptor/vhdi_test_block_descriptor.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-05-09 04:50:14.000000 libvhdi-20240509/msvscpp/libcfile/libcfile.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/pyvhdi/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6506 2024-05-09 04:50:14.000000 libvhdi-20240509/msvscpp/pyvhdi/pyvhdi.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/vhdi_test_file_footer/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5992 2024-05-09 04:50:14.000000 libvhdi-20240509/msvscpp/vhdi_test_file_footer/vhdi_test_file_footer.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-05-09 04:50:14.000000 libvhdi-20240509/msvscpp/libcdata/libcdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/vhdi_test_metadata_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5757 2024-05-09 04:50:44.000000 libvhdi-20240509/msvscpp/vhdi_test_metadata_values/vhdi_test_metadata_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/vhdimount/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7556 2024-05-09 04:50:14.000000 libvhdi-20240509/msvscpp/vhdimount/vhdimount.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/vhdi_test_region_table_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5769 2024-05-09 04:50:14.000000 libvhdi-20240509/msvscpp/vhdi_test_region_table_header/vhdi_test_region_table_header.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/vhdiinfo/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6829 2024-05-09 04:50:14.000000 libvhdi-20240509/msvscpp/vhdiinfo/vhdiinfo.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-05-09 04:50:14.000000 libvhdi-20240509/msvscpp/libcthreads/libcthreads.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-05-09 04:50:14.000000 libvhdi-20240509/msvscpp/libcpath/libcpath.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/vhdi_test_file/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6461 2024-05-09 04:50:44.000000 libvhdi-20240509/msvscpp/vhdi_test_file/vhdi_test_file.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/vhdi_test_metadata_table/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5754 2024-05-09 04:50:44.000000 libvhdi-20240509/msvscpp/vhdi_test_metadata_table/vhdi_test_metadata_table.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/vhdi_test_metadata_table_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5775 2024-05-09 04:50:14.000000 libvhdi-20240509/msvscpp/vhdi_test_metadata_table_header/vhdi_test_metadata_table_header.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/vhdi_test_file_information/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6007 2024-05-09 04:50:14.000000 libvhdi-20240509/msvscpp/vhdi_test_file_information/vhdi_test_file_information.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39154 2024-05-09 04:50:44.000000 libvhdi-20240509/msvscpp/libvhdi.sln
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-05-09 04:50:14.000000 libvhdi-20240509/msvscpp/libcsplit/libcsplit.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/libvhdi/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11785 2024-05-09 04:50:14.000000 libvhdi-20240509/msvscpp/libvhdi/libvhdi.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-05-09 04:50:14.000000 libvhdi-20240509/msvscpp/libuna/libuna.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23250 2024-05-09 05:22:19.000000 libvhdi-20240509/msvscpp/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-05-09 04:50:14.000000 libvhdi-20240509/msvscpp/libcnotify/libcnotify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/vhdi_test_checksum/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5656 2024-05-09 04:50:44.000000 libvhdi-20240509/msvscpp/vhdi_test_checksum/vhdi_test_checksum.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-05-09 04:50:14.000000 libvhdi-20240509/msvscpp/libcerror/libcerror.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/msvscpp/vhdi_test_notify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5651 2024-05-09 04:50:44.000000 libvhdi-20240509/msvscpp/vhdi_test_notify/vhdi_test_notify.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-05-09 04:49:48.000000 libvhdi-20240509/AUTHORS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:12.000000 libvhdi-20240509/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-09 05:21:55.000000 libvhdi-20240509/libcfile/libcfile_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-05-09 05:21:55.000000 libvhdi-20240509/libcfile/libcfile_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-09 05:21:55.000000 libvhdi-20240509/libcfile/libcfile_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-05-09 05:21:55.000000 libvhdi-20240509/libcfile/libcfile_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-05-09 05:21:55.000000 libvhdi-20240509/libcfile/libcfile_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-05-09 05:21:55.000000 libvhdi-20240509/libcfile/libcfile_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      938 2024-05-09 05:21:55.000000 libvhdi-20240509/libcfile/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-05-09 05:21:55.000000 libvhdi-20240509/libcfile/libcfile_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-05-09 05:21:55.000000 libvhdi-20240509/libcfile/libcfile_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-05-09 05:21:55.000000 libvhdi-20240509/libcfile/libcfile_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-09 05:21:55.000000 libvhdi-20240509/libcfile/libcfile_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-05-09 05:21:55.000000 libvhdi-20240509/libcfile/libcfile_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-09 05:21:55.000000 libvhdi-20240509/libcfile/libcfile_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-09 05:21:55.000000 libvhdi-20240509/libcfile/libcfile_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-05-09 05:21:55.000000 libvhdi-20240509/libcfile/libcfile_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-09 05:21:55.000000 libvhdi-20240509/libcfile/libcfile_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-05-09 05:21:55.000000 libvhdi-20240509/libcfile/libcfile_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30116 2024-05-09 05:22:19.000000 libvhdi-20240509/libcfile/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-09 05:21:55.000000 libvhdi-20240509/libcfile/libcfile_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-05-09 05:21:55.000000 libvhdi-20240509/libcfile/libcfile_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-05-09 05:21:55.000000 libvhdi-20240509/libcfile/libcfile_winapi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-05-09 05:21:55.000000 libvhdi-20240509/libcfile/libcfile_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      613 2024-05-09 04:50:54.000000 libvhdi-20240509/README
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:12.000000 libvhdi-20240509/pyvhdi/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-05-09 04:49:51.000000 libvhdi-20240509/pyvhdi/pyvhdi_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-05-09 04:49:51.000000 libvhdi-20240509/pyvhdi/pyvhdi_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1603 2024-05-09 04:49:51.000000 libvhdi-20240509/pyvhdi/pyvhdi_disk_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33791 2024-05-09 04:49:51.000000 libvhdi-20240509/pyvhdi/pyvhdi_file_object_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1186 2024-05-09 05:03:03.000000 libvhdi-20240509/pyvhdi/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14542 2024-05-09 04:50:54.000000 libvhdi-20240509/pyvhdi/pyvhdi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1531 2024-05-09 04:49:51.000000 libvhdi-20240509/pyvhdi/pyvhdi_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-05-09 04:49:51.000000 libvhdi-20240509/pyvhdi/pyvhdi_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2030 2024-05-09 04:49:51.000000 libvhdi-20240509/pyvhdi/pyvhdi_python.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8858 2024-05-09 04:49:51.000000 libvhdi-20240509/pyvhdi/pyvhdi_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40871 2024-05-09 04:50:54.000000 libvhdi-20240509/pyvhdi/pyvhdi_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1847 2024-05-09 04:49:51.000000 libvhdi-20240509/pyvhdi/pyvhdi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1535 2024-05-09 04:49:51.000000 libvhdi-20240509/pyvhdi/pyvhdi_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-05-09 04:49:51.000000 libvhdi-20240509/pyvhdi/pyvhdi_libvhdi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-05-09 04:49:51.000000 libvhdi-20240509/pyvhdi/pyvhdi_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5797 2024-05-09 04:49:51.000000 libvhdi-20240509/pyvhdi/pyvhdi_disk_types.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-05-09 04:50:54.000000 libvhdi-20240509/pyvhdi/pyvhdi_guid.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41568 2024-05-09 05:22:19.000000 libvhdi-20240509/pyvhdi/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1355 2024-05-09 04:49:51.000000 libvhdi-20240509/pyvhdi/pyvhdi_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4080 2024-05-09 04:49:51.000000 libvhdi-20240509/pyvhdi/pyvhdi_file_object_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-05-09 04:49:51.000000 libvhdi-20240509/pyvhdi/pyvhdi_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-05-09 04:49:51.000000 libvhdi-20240509/pyvhdi/pyvhdi_guid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3618 2024-05-09 04:50:54.000000 libvhdi-20240509/pyvhdi/pyvhdi_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-05-09 05:22:18.000000 libvhdi-20240509/INSTALL
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:11.000000 libvhdi-20240509/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-05-09 05:21:52.000000 libvhdi-20240509/libcdata/libcdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-05-09 05:21:52.000000 libvhdi-20240509/libcdata/libcdata_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-05-09 05:21:52.000000 libvhdi-20240509/libcdata/libcdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-09 05:21:52.000000 libvhdi-20240509/libcdata/libcdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-09 05:21:52.000000 libvhdi-20240509/libcdata/libcdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-05-09 05:21:52.000000 libvhdi-20240509/libcdata/libcdata_btree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-05-09 05:21:52.000000 libvhdi-20240509/libcdata/libcdata_btree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-05-09 05:21:52.000000 libvhdi-20240509/libcdata/libcdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-05-09 05:21:52.000000 libvhdi-20240509/libcdata/libcdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-09 05:21:52.000000 libvhdi-20240509/libcdata/libcdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-05-09 05:21:52.000000 libvhdi-20240509/libcdata/libcdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-05-09 05:21:52.000000 libvhdi-20240509/libcdata/libcdata_btree_values_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1123 2024-05-09 05:21:52.000000 libvhdi-20240509/libcdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-05-09 05:21:52.000000 libvhdi-20240509/libcdata/libcdata_btree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-05-09 05:21:52.000000 libvhdi-20240509/libcdata/libcdata_range_list_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-05-09 05:21:52.000000 libvhdi-20240509/libcdata/libcdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-05-09 05:21:52.000000 libvhdi-20240509/libcdata/libcdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-05-09 05:21:52.000000 libvhdi-20240509/libcdata/libcdata_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-05-09 05:21:52.000000 libvhdi-20240509/libcdata/libcdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-05-09 05:21:52.000000 libvhdi-20240509/libcdata/libcdata_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-05-09 05:21:52.000000 libvhdi-20240509/libcdata/libcdata_tree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-09 05:21:52.000000 libvhdi-20240509/libcdata/libcdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-05-09 05:21:52.000000 libvhdi-20240509/libcdata/libcdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-05-09 05:21:52.000000 libvhdi-20240509/libcdata/libcdata_btree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-05-09 05:21:52.000000 libvhdi-20240509/libcdata/libcdata_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-05-09 05:21:52.000000 libvhdi-20240509/libcdata/libcdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32029 2024-05-09 05:22:19.000000 libvhdi-20240509/libcdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-05-09 05:21:52.000000 libvhdi-20240509/libcdata/libcdata_range_list_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-05-09 05:21:52.000000 libvhdi-20240509/libcdata/libcdata_btree_values_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-09 05:21:52.000000 libvhdi-20240509/libcdata/libcdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-05-09 04:49:46.000000 libvhdi-20240509/pyproject.toml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      480 2024-05-09 04:49:46.000000 libvhdi-20240509/setup.cfg.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-05-09 05:22:18.000000 libvhdi-20240509/config.sub
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-05-09 04:49:46.000000 libvhdi-20240509/setup.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1493 2024-05-09 04:49:46.000000 libvhdi-20240509/acinclude.m4
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:15:00.000000 libvhdi-20240509/config.rpath
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:11.000000 libvhdi-20240509/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-05-09 05:22:01.000000 libvhdi-20240509/libcthreads/libcthreads_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-05-09 05:22:01.000000 libvhdi-20240509/libcthreads/libcthreads_read_write_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-05-09 05:22:01.000000 libvhdi-20240509/libcthreads/libcthreads_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-05-09 05:22:01.000000 libvhdi-20240509/libcthreads/libcthreads_thread_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-05-09 05:22:01.000000 libvhdi-20240509/libcthreads/libcthreads_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-05-09 05:22:01.000000 libvhdi-20240509/libcthreads/libcthreads_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-05-09 05:22:01.000000 libvhdi-20240509/libcthreads/libcthreads_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-05-09 05:22:01.000000 libvhdi-20240509/libcthreads/libcthreads_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-05-09 05:22:01.000000 libvhdi-20240509/libcthreads/libcthreads_condition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-05-09 05:22:01.000000 libvhdi-20240509/libcthreads/libcthreads_repeating_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1167 2024-05-09 05:22:01.000000 libvhdi-20240509/libcthreads/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-05-09 05:22:01.000000 libvhdi-20240509/libcthreads/libcthreads_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-05-09 05:22:01.000000 libvhdi-20240509/libcthreads/libcthreads_mutex.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-05-09 05:22:01.000000 libvhdi-20240509/libcthreads/libcthreads_queue.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-05-09 05:22:01.000000 libvhdi-20240509/libcthreads/libcthreads_mutex.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-05-09 05:22:01.000000 libvhdi-20240509/libcthreads/libcthreads_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-05-09 05:22:01.000000 libvhdi-20240509/libcthreads/libcthreads_thread_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-05-09 05:22:01.000000 libvhdi-20240509/libcthreads/libcthreads_condition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-05-09 05:22:01.000000 libvhdi-20240509/libcthreads/libcthreads_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-05-09 05:22:01.000000 libvhdi-20240509/libcthreads/libcthreads_read_write_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-05-09 05:22:01.000000 libvhdi-20240509/libcthreads/libcthreads_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-05-09 05:22:01.000000 libvhdi-20240509/libcthreads/libcthreads_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-05-09 05:22:01.000000 libvhdi-20240509/libcthreads/libcthreads_thread_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-05-09 05:22:01.000000 libvhdi-20240509/libcthreads/libcthreads_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-05-09 05:22:01.000000 libvhdi-20240509/libcthreads/libcthreads_thread_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-05-09 05:22:01.000000 libvhdi-20240509/libcthreads/libcthreads_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-05-09 05:22:01.000000 libvhdi-20240509/libcthreads/libcthreads_repeating_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32468 2024-05-09 05:22:19.000000 libvhdi-20240509/libcthreads/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-05-09 05:22:01.000000 libvhdi-20240509/libcthreads/libcthreads_queue.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2401 2024-05-09 05:22:31.000000 libvhdi-20240509/libvhdi.spec
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-05-09 05:22:19.000000 libvhdi-20240509/test-driver
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:12.000000 libvhdi-20240509/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-05-09 05:21:59.000000 libvhdi-20240509/libcpath/libcpath_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-09 05:21:59.000000 libvhdi-20240509/libcpath/libcpath_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-05-09 05:21:59.000000 libvhdi-20240509/libcpath/libcpath_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      838 2024-05-09 05:21:59.000000 libvhdi-20240509/libcpath/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-09 05:21:59.000000 libvhdi-20240509/libcpath/libcpath_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-09 05:21:59.000000 libvhdi-20240509/libcpath/libcpath_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-05-09 05:21:59.000000 libvhdi-20240509/libcpath/libcpath_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-05-09 05:21:59.000000 libvhdi-20240509/libcpath/libcpath_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-05-09 05:21:59.000000 libvhdi-20240509/libcpath/libcpath_libcsplit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-05-09 05:21:59.000000 libvhdi-20240509/libcpath/libcpath_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-09 05:21:59.000000 libvhdi-20240509/libcpath/libcpath_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-09 05:21:59.000000 libvhdi-20240509/libcpath/libcpath_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29314 2024-05-09 05:22:19.000000 libvhdi-20240509/libcpath/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-05-09 05:21:59.000000 libvhdi-20240509/libcpath/libcpath_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-09 05:21:59.000000 libvhdi-20240509/libcpath/libcpath_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-05-09 05:21:59.000000 libvhdi-20240509/libcpath/libcpath_path.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-05-09 05:21:59.000000 libvhdi-20240509/libcpath/libcpath_path.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1381 2023-12-03 09:15:01.000000 libvhdi-20240509/ChangeLog
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/manuals/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      125 2024-05-09 05:02:51.000000 libvhdi-20240509/manuals/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5718 2024-05-09 04:49:53.000000 libvhdi-20240509/manuals/libvhdi.3
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26044 2024-05-09 05:22:19.000000 libvhdi-20240509/manuals/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1418 2024-05-09 04:49:53.000000 libvhdi-20240509/manuals/vhdiinfo.1
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/tests/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1803 2024-05-09 04:49:52.000000 libvhdi-20240509/tests/vhdi_test_functions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-09 04:49:52.000000 libvhdi-20240509/tests/vhdi_test_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24047 2024-05-09 04:50:44.000000 libvhdi-20240509/tests/vhdi_test_file_footer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9809 2024-05-09 04:50:44.000000 libvhdi-20240509/tests/vhdi_test_parent_locator_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4123 2024-05-09 04:49:52.000000 libvhdi-20240509/tests/vhdi_test_tools_signal.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3282 2024-05-09 04:49:52.000000 libvhdi-20240509/tests/test_vhdiinfo.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6369 2024-05-09 04:50:44.000000 libvhdi-20240509/tests/vhdi_test_metadata_values.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4034 2024-05-09 04:52:45.000000 libvhdi-20240509/tests/test_tools.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6758 2024-05-09 04:50:44.000000 libvhdi-20240509/tests/vhdi_test_block_allocation_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    42352 2024-05-09 04:50:44.000000 libvhdi-20240509/tests/vhdi_test_image_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3424 2024-05-09 04:50:54.000000 libvhdi-20240509/tests/pyvhdi_test_support.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5590 2024-05-09 04:49:52.000000 libvhdi-20240509/tests/vhdi_test_tools_info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10739 2024-05-09 05:03:45.000000 libvhdi-20240509/tests/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13423 2024-05-09 04:50:54.000000 libvhdi-20240509/tests/pyvhdi_test_file.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3099 2024-05-09 04:49:52.000000 libvhdi-20240509/tests/vhdi_test_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-05-09 04:49:52.000000 libvhdi-20240509/tests/vhdi_test_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4064 2024-05-09 04:49:52.000000 libvhdi-20240509/tests/vhdi_test_checksum.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    55225 2024-05-09 04:50:44.000000 libvhdi-20240509/tests/vhdi_test_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13247 2024-05-09 04:49:52.000000 libvhdi-20240509/tests/vhdi_test_functions.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4653 2024-05-09 04:49:52.000000 libvhdi-20240509/tests/vhdi_test_memory.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6313 2024-05-09 04:50:44.000000 libvhdi-20240509/tests/vhdi_test_metadata_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1706 2024-05-09 04:49:52.000000 libvhdi-20240509/tests/vhdi_test_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36919 2024-05-09 04:50:44.000000 libvhdi-20240509/tests/vhdi_test_dynamic_disk_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4531 2024-05-09 04:49:52.000000 libvhdi-20240509/tests/vhdi_test_getopt.c
+-rwxr--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-09 04:49:52.000000 libvhdi-20240509/tests/test_manpage.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9669 2024-05-09 04:50:44.000000 libvhdi-20240509/tests/vhdi_test_parent_locator_entry.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4403 2024-05-09 04:49:52.000000 libvhdi-20240509/tests/test_python_module.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-09 04:49:52.000000 libvhdi-20240509/tests/vhdi_test_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1691 2024-05-09 04:49:52.000000 libvhdi-20240509/tests/vhdi_test_memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12143 2024-05-09 04:50:44.000000 libvhdi-20240509/tests/vhdi_test_block_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14178 2024-05-09 04:50:44.000000 libvhdi-20240509/tests/vhdi_test_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6201 2024-05-09 04:50:44.000000 libvhdi-20240509/tests/vhdi_test_region_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6817 2024-05-09 04:50:44.000000 libvhdi-20240509/tests/vhdi_test_sector_range_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1367 2024-05-09 04:49:52.000000 libvhdi-20240509/tests/vhdi_test_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4276 2024-05-09 04:49:52.000000 libvhdi-20240509/tests/vhdi_test_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-05-09 04:50:44.000000 libvhdi-20240509/tests/vhdi_test_region_table_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-05-09 04:49:52.000000 libvhdi-20240509/tests/test_runner.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-05-09 04:49:52.000000 libvhdi-20240509/tests/vhdi_test_libvhdi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8018 2024-05-09 04:50:44.000000 libvhdi-20240509/tests/vhdi_test_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1808 2024-05-09 04:49:52.000000 libvhdi-20240509/tests/vhdi_test_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-05-09 04:49:52.000000 libvhdi-20240509/tests/vhdi_test_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2425 2024-05-09 04:49:52.000000 libvhdi-20240509/tests/vhdi_test_tools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10465 2024-05-09 04:50:44.000000 libvhdi-20240509/tests/vhdi_test_metadata_table_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-05-09 04:49:52.000000 libvhdi-20240509/tests/vhdi_test_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18202 2024-05-09 04:50:44.000000 libvhdi-20240509/tests/vhdi_test_file_information.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    77741 2024-05-09 05:22:19.000000 libvhdi-20240509/tests/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10435 2024-05-09 04:50:44.000000 libvhdi-20240509/tests/vhdi_test_metadata_table_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8539 2024-05-09 04:49:52.000000 libvhdi-20240509/tests/vhdi_test_macros.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10217 2024-05-09 04:50:44.000000 libvhdi-20240509/tests/vhdi_test_region_table_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6313 2024-05-09 04:50:44.000000 libvhdi-20240509/tests/vhdi_test_parent_locator.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4360 2024-05-09 04:52:21.000000 libvhdi-20240509/tests/test_library.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      678 2024-05-09 04:49:46.000000 libvhdi-20240509/libvhdi.pc.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:12.000000 libvhdi-20240509/vhditools/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5895 2024-05-09 04:50:54.000000 libvhdi-20240509/vhditools/vhdiinfo.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5726 2024-05-09 04:49:51.000000 libvhdi-20240509/vhditools/vhditools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37173 2024-05-09 04:49:51.000000 libvhdi-20240509/vhditools/mount_dokan.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2955 2024-05-09 04:49:51.000000 libvhdi-20240509/vhditools/mount_file_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26443 2024-05-09 04:50:54.000000 libvhdi-20240509/vhditools/mount_fuse.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1932 2024-05-09 04:50:54.000000 libvhdi-20240509/vhditools/info_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4531 2024-05-09 04:49:51.000000 libvhdi-20240509/vhditools/vhditools_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5414 2024-05-09 04:49:51.000000 libvhdi-20240509/vhditools/mount_dokan.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1498 2024-05-09 04:49:51.000000 libvhdi-20240509/vhditools/vhditools_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3927 2024-05-09 04:49:51.000000 libvhdi-20240509/vhditools/vhditools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1501 2024-05-09 04:49:51.000000 libvhdi-20240509/vhditools/vhditools_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18788 2024-05-09 04:50:54.000000 libvhdi-20240509/vhditools/mount_file_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2024-05-09 04:49:51.000000 libvhdi-20240509/vhditools/vhditools_output.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1210 2024-05-09 04:49:51.000000 libvhdi-20240509/vhditools/vhditools_i18n.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-05-09 04:49:51.000000 libvhdi-20240509/vhditools/vhditools_signal.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10552 2024-05-09 04:49:51.000000 libvhdi-20240509/vhditools/byte_size_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1406 2024-05-09 04:49:51.000000 libvhdi-20240509/vhditools/vhditools_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2241 2024-05-09 05:03:18.000000 libvhdi-20240509/vhditools/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20694 2024-05-09 04:50:54.000000 libvhdi-20240509/vhditools/mount_file_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16485 2024-05-09 04:50:54.000000 libvhdi-20240509/vhditools/info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-05-09 04:49:51.000000 libvhdi-20240509/vhditools/vhditools_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3608 2024-05-09 04:49:51.000000 libvhdi-20240509/vhditools/mount_file_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-05-09 04:49:51.000000 libvhdi-20240509/vhditools/vhditools_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1480 2024-05-09 04:49:51.000000 libvhdi-20240509/vhditools/vhditools_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1808 2024-05-09 04:49:51.000000 libvhdi-20240509/vhditools/vhditools_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1778 2024-05-09 04:49:51.000000 libvhdi-20240509/vhditools/vhditools_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15191 2024-05-09 04:50:54.000000 libvhdi-20240509/vhditools/vhdimount.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2664 2024-05-09 04:49:51.000000 libvhdi-20240509/vhditools/mount_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-05-09 04:49:51.000000 libvhdi-20240509/vhditools/vhditools_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1745 2024-05-09 04:49:51.000000 libvhdi-20240509/vhditools/vhditools_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22344 2024-05-09 04:50:54.000000 libvhdi-20240509/vhditools/mount_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-05-09 04:49:51.000000 libvhdi-20240509/vhditools/vhditools_libvhdi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33791 2024-05-09 05:22:19.000000 libvhdi-20240509/vhditools/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-05-09 04:49:51.000000 libvhdi-20240509/vhditools/byte_size_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2762 2024-05-09 04:50:54.000000 libvhdi-20240509/vhditools/mount_fuse.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/ossfuzz/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      967 2024-05-09 04:49:50.000000 libvhdi-20240509/ossfuzz/ossfuzz_libvhdi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      885 2024-05-09 05:02:41.000000 libvhdi-20240509/ossfuzz/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-05-09 04:49:50.000000 libvhdi-20240509/ossfuzz/ossfuzz_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2199 2024-05-09 04:49:50.000000 libvhdi-20240509/ossfuzz/file_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31338 2024-05-09 05:22:19.000000 libvhdi-20240509/ossfuzz/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-05-09 05:22:12.000000 libvhdi-20240509/ltmain.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:11.000000 libvhdi-20240509/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-05-09 05:22:00.000000 libvhdi-20240509/libcsplit/libcsplit_narrow_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-05-09 05:22:00.000000 libvhdi-20240509/libcsplit/libcsplit_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-05-09 05:22:00.000000 libvhdi-20240509/libcsplit/libcsplit_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-05-09 05:22:00.000000 libvhdi-20240509/libcsplit/libcsplit_wide_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-09 05:22:00.000000 libvhdi-20240509/libcsplit/libcsplit_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      880 2024-05-09 05:22:00.000000 libvhdi-20240509/libcsplit/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-09 05:22:00.000000 libvhdi-20240509/libcsplit/libcsplit_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-05-09 05:22:00.000000 libvhdi-20240509/libcsplit/libcsplit_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-09 05:22:00.000000 libvhdi-20240509/libcsplit/libcsplit_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-05-09 05:22:00.000000 libvhdi-20240509/libcsplit/libcsplit_wide_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-05-09 05:22:00.000000 libvhdi-20240509/libcsplit/libcsplit_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-05-09 05:22:00.000000 libvhdi-20240509/libcsplit/libcsplit_narrow_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-09 05:22:00.000000 libvhdi-20240509/libcsplit/libcsplit_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-09 05:22:00.000000 libvhdi-20240509/libcsplit/libcsplit_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-05-09 05:22:00.000000 libvhdi-20240509/libcsplit/libcsplit_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-05-09 05:22:00.000000 libvhdi-20240509/libcsplit/libcsplit_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30211 2024-05-09 05:22:19.000000 libvhdi-20240509/libcsplit/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-05-09 05:22:00.000000 libvhdi-20240509/libcsplit/libcsplit_narrow_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-05-09 05:22:00.000000 libvhdi-20240509/libcsplit/libcsplit_narrow_string.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:12.000000 libvhdi-20240509/libvhdi/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2609 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_region_type_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2423 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_file_footer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1395 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21525 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_dynamic_disk_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1485 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23167 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_block_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16640 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_parent_locator_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1700 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13950 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_image_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3053 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_block_descriptor.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1991 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1829 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_region_type_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2103 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1916 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_file_information.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1348 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_i18n.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2491 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/vhdi_file_footer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1956 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3349 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_checksum.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1780 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_metadata_table_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1087 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi.rc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19781 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_block_allocation_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4580 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3226 2024-05-09 05:04:00.000000 libvhdi-20240509/libvhdi/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1886 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_region_table_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32903 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_metadata_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8068 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_file_information.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1542 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_libfdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2627 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_parent_locator_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1085 2024-05-09 05:22:31.000000 libvhdi-20240509/libvhdi/libvhdi.rc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1987 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/vhdi_region_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10962 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_metadata_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3342 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_sector_range_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1707 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_i18n.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6784 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_metadata_table_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2846 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1688 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_sector_range_descriptor.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1780 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_parent_locator_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2844 2024-05-09 05:22:31.000000 libvhdi-20240509/libvhdi/libvhdi_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1827 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1859 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_metadata_table_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6440 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_parent_locator_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_metadata_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12001 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_region_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2084 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_region_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2349 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/vhdi_dynamic_disk_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1496 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_checksum.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2009 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/vhdi_metadata_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2213 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/vhdi_image_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14914 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_file_footer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1944 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/vhdi_parent_locator.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7984 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6598 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_region_table_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_parent_locator.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7278 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_metadata_table_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4109 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_metadata_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8384 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    95646 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1791 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_region_table_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11013 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2229 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_metadata_item_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40270 2024-05-09 05:22:19.000000 libvhdi-20240509/libvhdi/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11851 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_parent_locator.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3379 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_dynamic_disk_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2358 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_image_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3648 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_metadata_item_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2894 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_block_allocation_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6507 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/libvhdi_region_table_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-05-09 04:49:50.000000 libvhdi-20240509/libvhdi/vhdi_file_information.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:13.000000 libvhdi-20240509/po/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:15:03.000000 libvhdi-20240509/po/remove-potcdate.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:15:03.000000 libvhdi-20240509/po/POTFILES.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:15:03.000000 libvhdi-20240509/po/Makefile.in.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:15:03.000000 libvhdi-20240509/po/quot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:15:03.000000 libvhdi-20240509/po/en@quot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:15:03.000000 libvhdi-20240509/po/en@boldquot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:15:03.000000 libvhdi-20240509/po/boldquot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:15:03.000000 libvhdi-20240509/po/insert-header.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:15:04.000000 libvhdi-20240509/po/ChangeLog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1853 2024-05-09 05:22:31.000000 libvhdi-20240509/po/Makevars
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:15:04.000000 libvhdi-20240509/po/Makevars.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:15:03.000000 libvhdi-20240509/po/Rules-quot
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:12.000000 libvhdi-20240509/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_windows_1251.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_base16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_utf8_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_iso_8859_2.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_windows_932.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_mac_dingbats.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_base64_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_mac_turkish.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_unicode_character.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_mac_gaelic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_mac_arabic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_mac_thai.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_windows_874.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_iso_8859_15.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_iso_8859_16.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_windows_1255.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_utf7_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_koi8_u.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_iso_8859_6.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_iso_8859_14.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_base64_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_mac_centraleurroman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_mac_romanian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_iso_8859_6.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_iso_8859_9.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_mac_russian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_mac_dingbats.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_iso_8859_15.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_windows_936.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_mac_croatian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_scsu.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4193 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_utf32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_windows_936.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_iso_8859_10.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_mac_roman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_utf7_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_iso_8859_3.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_mac_thai.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_mac_farsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_mac_ukrainian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_mac_inuit.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_windows_932.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_windows_874.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_iso_8859_5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_iso_8859_10.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_url_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_mac_icelandic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_koi8_u.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_utf16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_windows_1253.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_iso_8859_4.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_mac_greek.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_mac_centraleurroman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_windows_1254.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_iso_8859_13.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_iso_8859_7.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_windows_1255.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_unicode_character.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_iso_8859_8.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_iso_8859_13.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_windows_949.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_mac_cyrillic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_mac_celtic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_iso_8859_4.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_windows_949.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_utf16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_mac_symbol.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_mac_roman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_windows_1257.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_windows_1254.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_windows_950.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_windows_1256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_base32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_windows_1253.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_iso_8859_16.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_utf8_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_windows_1250.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_iso_8859_2.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_koi8_r.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_iso_8859_5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_utf32_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_mac_icelandic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_windows_1256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_utf32_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_mac_romanian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_iso_8859_8.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_koi8_r.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_mac_cyrillic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_mac_arabic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_mac_croatian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_iso_8859_9.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_mac_greek.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_windows_1258.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_iso_8859_7.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    55795 2024-05-09 05:22:19.000000 libvhdi-20240509/libuna/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_iso_8859_3.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_windows_1250.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_scsu.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_windows_1252.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_mac_turkish.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_mac_ukrainian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_mac_russian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_windows_1258.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_mac_celtic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_byte_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_mac_gaelic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_utf32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_mac_symbol.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_windows_1257.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_mac_inuit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_mac_farsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_windows_950.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_url_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_windows_1251.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_windows_1252.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_codepage_iso_8859_14.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_base16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-05-09 05:22:08.000000 libvhdi-20240509/libuna/libuna_base32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39919 2024-05-09 05:22:18.000000 libvhdi-20240509/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:11.000000 libvhdi-20240509/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-05-09 05:21:58.000000 libvhdi-20240509/libcnotify/libcnotify_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-05-09 05:21:58.000000 libvhdi-20240509/libcnotify/libcnotify_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-05-09 05:21:58.000000 libvhdi-20240509/libcnotify/libcnotify_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-05-09 05:21:58.000000 libvhdi-20240509/libcnotify/libcnotify_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      724 2024-05-09 05:21:58.000000 libvhdi-20240509/libcnotify/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-05-09 05:21:58.000000 libvhdi-20240509/libcnotify/libcnotify_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-05-09 05:21:58.000000 libvhdi-20240509/libcnotify/libcnotify_verbose.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-05-09 05:21:58.000000 libvhdi-20240509/libcnotify/libcnotify_print.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-05-09 05:21:58.000000 libvhdi-20240509/libcnotify/libcnotify_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-05-09 05:21:58.000000 libvhdi-20240509/libcnotify/libcnotify_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-05-09 05:21:58.000000 libvhdi-20240509/libcnotify/libcnotify_verbose.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29152 2024-05-09 05:22:19.000000 libvhdi-20240509/libcnotify/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-05-09 05:21:58.000000 libvhdi-20240509/libcnotify/libcnotify_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-05-09 05:21:58.000000 libvhdi-20240509/libcnotify/libcnotify_print.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-09 06:52:11.000000 libvhdi-20240509/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-05-09 05:21:53.000000 libvhdi-20240509/libcerror/libcerror_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-05-09 05:21:53.000000 libvhdi-20240509/libcerror/libcerror_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-09 05:21:53.000000 libvhdi-20240509/libcerror/libcerror_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      636 2024-05-09 05:21:54.000000 libvhdi-20240509/libcerror/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-05-09 05:21:53.000000 libvhdi-20240509/libcerror/libcerror_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-09 05:21:53.000000 libvhdi-20240509/libcerror/libcerror_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-05-09 05:21:53.000000 libvhdi-20240509/libcerror/libcerror_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-05-09 05:21:53.000000 libvhdi-20240509/libcerror/libcerror_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-05-09 05:21:54.000000 libvhdi-20240509/libcerror/libcerror_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-05-09 05:21:53.000000 libvhdi-20240509/libcerror/libcerror_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-09 05:21:53.000000 libvhdi-20240509/libcerror/libcerror_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28619 2024-05-09 05:22:19.000000 libvhdi-20240509/libcerror/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56793 2024-05-09 05:22:15.000000 libvhdi-20240509/aclocal.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7443 2024-05-09 04:49:46.000000 libvhdi-20240509/configure.ac
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      411 2024-05-09 06:52:14.271221 libvhdi-20240509/PKG-INFO
```

### Comparing `libvhdi-20240303/libfdata/libfdata_error.h` & `libvhdi-20240509/libfdata/libfdata_error.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfdata/libfdata_area.c` & `libvhdi-20240509/libfdata/libfdata_area.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfdata/libfdata_stream.h` & `libvhdi-20240509/libfdata/libfdata_stream.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfdata/libfdata_cache.h` & `libvhdi-20240509/libfdata/libfdata_cache.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfdata/libfdata_range_list.c` & `libvhdi-20240509/libfdata/libfdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfdata/libfdata_mapped_range.c` & `libvhdi-20240509/libfdata/libfdata_mapped_range.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfdata/libfdata_libcerror.h` & `libvhdi-20240509/libfdata/libfdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfdata/libfdata_definitions.h` & `libvhdi-20240509/libfdata/libfdata_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBFDATA )
 #include <libfdata/definitions.h>
 
 /* The definitions in <libfdata/definitions.h> are copied here
  * for local use of libfdata
  */
 #else
-#define LIBFDATA_VERSION						20240114
+#define LIBFDATA_VERSION						20240415
 
 /* The libfdata version string
  */
-#define LIBFDATA_VERSION_STRING						"20240114"
+#define LIBFDATA_VERSION_STRING						"20240415"
 
 /* The library flag definitions
  */
 enum LIBFDATA_FLAGS
 {
 	/* The data is not managed by the library
 	 */
```

### Comparing `libvhdi-20240303/libfdata/libfdata_list.c` & `libvhdi-20240509/libfdata/libfdata_list.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfdata/libfdata_libcdata.h` & `libvhdi-20240509/libfdata/libfdata_libcdata.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfdata/libfdata_list.h` & `libvhdi-20240509/libfdata/libfdata_list.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfdata/libfdata_list_element.h` & `libvhdi-20240509/libfdata/libfdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfdata/Makefile.am` & `libvhdi-20240509/libfdata/Makefile.am`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFDATA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBFCACHE_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
@@ -31,19 +31,17 @@
 	libfdata_stream.c libfdata_stream.h \
 	libfdata_support.c libfdata_support.h \
 	libfdata_types.h \
 	libfdata_unused.h \
 	libfdata_vector.c libfdata_vector.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdata_la_SOURCES)
```

### Comparing `libvhdi-20240303/libfdata/libfdata_libcnotify.h` & `libvhdi-20240509/libfdata/libfdata_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfdata/libfdata_extern.h` & `libvhdi-20240509/libfdata/libfdata_extern.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfdata/libfdata_notify.c` & `libvhdi-20240509/libfdata/libfdata_notify.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfdata/libfdata_cache.c` & `libvhdi-20240509/libfdata/libfdata_cache.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfdata/libfdata_stream.c` & `libvhdi-20240509/libfdata/libfdata_stream.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfdata/libfdata_unused.h` & `libvhdi-20240509/libfdata/libfdata_unused.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfdata/libfdata_range.h` & `libvhdi-20240509/libfdata/libfdata_range.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfdata/libfdata_area.h` & `libvhdi-20240509/libfdata/libfdata_area.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfdata/libfdata_error.c` & `libvhdi-20240509/libfdata/libfdata_error.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfdata/libfdata_support.h` & `libvhdi-20240509/libfdata/libfdata_support.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfdata/libfdata_range.c` & `libvhdi-20240509/libfdata/libfdata_range.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfdata/libfdata_mapped_range.h` & `libvhdi-20240509/libfdata/libfdata_mapped_range.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfdata/libfdata_support.c` & `libvhdi-20240509/libfdata/libfdata_support.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfdata/libfdata_list_element.c` & `libvhdi-20240509/libfdata/libfdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfdata/libfdata_segments_array.c` & `libvhdi-20240509/libfdata/libfdata_segments_array.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfdata/libfdata_types.h` & `libvhdi-20240509/libfdata/libfdata_types.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfdata/libfdata_notify.h` & `libvhdi-20240509/libfdata/libfdata_notify.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfdata/libfdata_range_list.h` & `libvhdi-20240509/libfdata/libfdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfdata/libfdata_segments_array.h` & `libvhdi-20240509/libfdata/libfdata_segments_array.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfdata/Makefile.in` & `libvhdi-20240509/libfdata/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -463,14 +463,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -525,16 +527,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFDATA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFDATA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFDATA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFDATA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFDATA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBFCACHE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@PTHREAD_CPPFLAGS@ 
 
@@ -558,15 +560,16 @@
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_segments_array.c libfdata_segments_array.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_stream.c libfdata_stream.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_support.c libfdata_support.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_types.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_unused.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_vector.c libfdata_vector.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -778,24 +781,39 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfdata_area.Plo
+	-rm -f ./$(DEPDIR)/libfdata_cache.Plo
+	-rm -f ./$(DEPDIR)/libfdata_error.Plo
+	-rm -f ./$(DEPDIR)/libfdata_list.Plo
+	-rm -f ./$(DEPDIR)/libfdata_list_element.Plo
+	-rm -f ./$(DEPDIR)/libfdata_mapped_range.Plo
+	-rm -f ./$(DEPDIR)/libfdata_notify.Plo
+	-rm -f ./$(DEPDIR)/libfdata_range.Plo
+	-rm -f ./$(DEPDIR)/libfdata_range_list.Plo
+	-rm -f ./$(DEPDIR)/libfdata_segments_array.Plo
+	-rm -f ./$(DEPDIR)/libfdata_stream.Plo
+	-rm -f ./$(DEPDIR)/libfdata_support.Plo
+	-rm -f ./$(DEPDIR)/libfdata_vector.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -891,17 +909,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdata_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvhdi-20240303/libfdata/libfdata_vector.c` & `libvhdi-20240509/libfdata/libfdata_vector.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfdata/libfdata_libfcache.h` & `libvhdi-20240509/libfdata/libfdata_libfcache.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfdata/libfdata_vector.h` & `libvhdi-20240509/libfdata/libfdata_vector.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/COPYING` & `libvhdi-20240509/COPYING`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/install-sh` & `libvhdi-20240509/install-sh`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/depcomp` & `libvhdi-20240509/depcomp`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfguid/libfguid_error.c` & `libvhdi-20240509/libfguid/libfguid_error.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfguid/libfguid_support.h` & `libvhdi-20240509/libfguid/libfguid_support.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfguid/libfguid_identifier.h` & `libvhdi-20240509/libfguid/libfguid_identifier.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfguid/libfguid_libcerror.h` & `libvhdi-20240509/libfguid/libfguid_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfguid/Makefile.am` & `libvhdi-20240509/libfguid/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFGUID
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfguid.la
 
 libfguid_la_SOURCES = \
 	libfguid_definitions.h \
 	libfguid_extern.h \
@@ -13,19 +13,17 @@
 	libfguid_libcerror.h \
 	libfguid_identifier.c libfguid_identifier.h \
 	libfguid_support.c libfguid_support.h \
 	libfguid_types.h \
 	libfguid_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfguid ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfguid_la_SOURCES)
```

### Comparing `libvhdi-20240303/libfguid/libfguid_unused.h` & `libvhdi-20240509/libfguid/libfguid_unused.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfguid/libfguid_extern.h` & `libvhdi-20240509/libfguid/libfguid_extern.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfguid/libfguid_types.h` & `libvhdi-20240509/libfguid/libfguid_types.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfguid/libfguid_identifier.c` & `libvhdi-20240509/libfguid/libfguid_identifier.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfguid/libfguid_support.c` & `libvhdi-20240509/libfguid/libfguid_support.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfguid/libfguid_definitions.h` & `libvhdi-20240509/libfguid/libfguid_definitions.h`

 * *Files 6% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfguid/definitions.h> are copied here
  * for local use of libfguid
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFGUID_VERSION					20240116
+#define LIBFGUID_VERSION					20240415
 
 /* The version string
  */
-#define LIBFGUID_VERSION_STRING					"20240116"
+#define LIBFGUID_VERSION_STRING					"20240415"
 
 /* The byte order definitions
  */
 #define LIBFGUID_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define LIBFGUID_ENDIAN_LITTLE					_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The GUID identifier version definitions
```

### Comparing `libvhdi-20240303/libfguid/Makefile.in` & `libvhdi-20240509/libfguid/Makefile.in`

 * *Files 0% similar despite different names*

```diff
@@ -439,14 +439,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -501,30 +503,31 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFGUID_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFGUID_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFGUID_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFGUID_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFGUID_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFGUID_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFGUID_TRUE@noinst_LTLIBRARIES = libfguid.la
 @HAVE_LOCAL_LIBFGUID_TRUE@libfguid_la_SOURCES = \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_definitions.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_extern.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_error.c libfguid_error.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_libcerror.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_identifier.c libfguid_identifier.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_support.c libfguid_support.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_types.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -726,24 +729,29 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfguid_error.Plo
+	-rm -f ./$(DEPDIR)/libfguid_identifier.Plo
+	-rm -f ./$(DEPDIR)/libfguid_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -829,17 +837,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfguid ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfguid_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvhdi-20240303/libfguid/libfguid_error.h` & `libvhdi-20240509/libfguid/libfguid_error.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/m4/libcfile.m4` & `libvhdi-20240509/m4/libcfile.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcfile required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcfile is available
 dnl ac_libcfile_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCFILE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcfile" = xno],
     [ac_cv_libcfile=no],
     [ac_cv_libcfile=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcfile which returns "yes" and --with-libcfile= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect],
+      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcfile"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcfile}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcfile}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcfile],
           [1])
@@ -199,16 +201,17 @@
             libcfile_file_remove_wide,
             [ac_cv_libcfile_dummy=yes],
             [ac_cv_libcfile=no])
           ])
 
         ac_cv_libcfile_LIBADD="-lcfile"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_libcfile" != xyes],
+      [test "x$ac_cv_libcfile" != xyes && test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcfile in directory: $ac_cv_with_libcfile],
         [1])
       ])
     ])
 
   AS_IF(
@@ -354,15 +357,15 @@
   AS_IF(
     [test "x$ac_cv_func_unlink" != xyes],
     [AC_MSG_FAILURE(
       [Missing function: unlink],
       [1])
     ])
 
-  ac_cv_libcfile_CPPFLAGS="-I../libcfile";
+  ac_cv_libcfile_CPPFLAGS="-I../libcfile -I\$(top_srcdir)/libcfile";
   ac_cv_libcfile_LIBADD="../libcfile/libcfile.la";
 
   ac_cv_libcfile=local
   ])
 
 dnl Function to detect how to enable libcfile
 AC_DEFUN([AX_LIBCFILE_CHECK_ENABLE],
```

### Comparing `libvhdi-20240303/m4/tests.m4` & `libvhdi-20240509/m4/tests.m4`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/m4/libcpath.m4` & `libvhdi-20240509/m4/libcpath.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcpath required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcpath is available
 dnl ac_libcpath_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCPATH_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcpath" = xno],
     [ac_cv_libcpath=no],
     [ac_cv_libcpath=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcpath which returns "yes" and --with-libcpath= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect],
+      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcpath"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcpath}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcpath}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcpath],
           [1])
@@ -148,16 +150,17 @@
             libcpath_path_make_directory_wide,
             [ac_cv_libcpath_dummy=yes],
             [ac_cv_libcpath=no])
           ])
 
         ac_cv_libcpath_LIBADD="-lcpath"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_libcpath" != xyes],
+      [test "x$ac_cv_libcpath" != xyes && test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcpath in directory: $ac_cv_with_libcpath],
         [1])
       ])
     ])
 
   AS_IF(
@@ -269,15 +272,15 @@
     [AC_MSG_FAILURE(
       [Missing functions: getcwd],
       [1])
     ])
 
   AX_LIBCPATH_CHECK_FUNC_MKDIR
 
-  ac_cv_libcpath_CPPFLAGS="-I../libcpath";
+  ac_cv_libcpath_CPPFLAGS="-I../libcpath -I\$(top_srcdir)/libcpath";
   ac_cv_libcpath_LIBADD="../libcpath/libcpath.la";
 
   ac_cv_libcpath=local
   ])
 
 dnl Function to detect how to enable libcpath
 AC_DEFUN([AX_LIBCPATH_CHECK_ENABLE],
```

### Comparing `libvhdi-20240303/m4/lib-prefix.m4` & `libvhdi-20240509/m4/lib-prefix.m4`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/m4/progtest.m4` & `libvhdi-20240509/m4/progtest.m4`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/m4/libuna.m4` & `libvhdi-20240509/m4/libuna.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libuna or required headers and functions
 dnl
-dnl Version: 20230702
+dnl Version: 20240413
 
 dnl Function to detect if a specific libuna definition is available.
 AC_DEFUN([AX_LIBUNA_CHECK_DEFINITION],
   [AC_CACHE_CHECK(
     [if `$1' is defined],
     [$2],
     [AC_LANG_PUSH(C)
@@ -23,16 +23,18 @@
 dnl ac_libuna_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBUNA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libuna" = xno],
     [ac_cv_libuna=no],
     [ac_cv_libuna=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libuna which returns "yes" and --with-libuna= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect],
+      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libuna"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libuna}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libuna}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libuna],
           [1])
@@ -938,16 +940,17 @@
           [ac_cv_libuna_defines_compare_greater])
         AS_IF(
           [test "x$ac_cv_libuna_defines_utf16_stream_allow_unpaired_surrogate" != xyes],
           [ac_cv_libuna=no])
 
         ac_cv_libuna_LIBADD="-luna"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_libuna" != xyes],
+      [test "x$ac_cv_libuna" != xyes && test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libuna in directory: $ac_cv_with_libuna],
         [1])
       ])
     ])
 
   AS_IF(
@@ -969,15 +972,15 @@
     ])
   ])
 
 dnl Function to detect if libuna dependencies are available
 AC_DEFUN([AX_LIBUNA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
   ])
 
 dnl Function to detect how to enable libuna
 AC_DEFUN([AX_LIBUNA_CHECK_ENABLE],
```

### Comparing `libvhdi-20240303/m4/gettext.m4` & `libvhdi-20240509/m4/gettext.m4`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/m4/lib-ld.m4` & `libvhdi-20240509/m4/lib-ld.m4`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/m4/libclocale.m4` & `libvhdi-20240509/m4/libclocale.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libclocale required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libclocale is available
 dnl ac_libclocale_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCLOCALE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libclocale" = xno],
     [ac_cv_libclocale=no],
     [ac_cv_libclocale=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libclocale which returns "yes" and --with-libclocale= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect],
+      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libclocale"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libclocale}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libclocale}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libclocale],
           [1])
@@ -122,16 +124,17 @@
           clocale,
           libclocale_initialize,
           [ac_cv_libclocale_dummy=yes],
           [ac_cv_libclocale=no])
 
         ac_cv_libclocale_LIBADD="-lclocale"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_libclocale" != xyes],
+      [test "x$ac_cv_libclocale" != xyes && test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libclocale in directory: $ac_cv_with_libclocale],
         [1])
       ])
     ])
 
   AS_IF(
@@ -216,15 +219,15 @@
     [AC_MSG_FAILURE(
       [Missing function: setlocale],
       [1])
     ])
 
   AX_LIBCLOCALE_CHECK_FUNC_LANGINFO_CODESET
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
   ])
 
 dnl Function to detect how to enable libclocale
 AC_DEFUN([AX_LIBCLOCALE_CHECK_ENABLE],
```

### Comparing `libvhdi-20240303/m4/libcdata.m4` & `libvhdi-20240509/m4/libcdata.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcdata required headers and functions
 dnl
-dnl Version: 20230108
+dnl Version: 20240413
 
 dnl Function to detect if libcdata is available
 dnl ac_libcdata_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCDATA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcdata" = xno],
     [ac_cv_libcdata=no],
     [ac_cv_libcdata=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcdata which returns "yes" and --with-libcdata= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect],
+      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcdata"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcdata}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcdata],
           [1])
@@ -493,16 +495,17 @@
           cdata,
           libcdata_tree_node_get_leaf_node_list,
           [ac_cv_libcdata_dummy=yes],
           [ac_cv_libcdata=no])
 
         ac_cv_libcdata_LIBADD="-lcdata"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_libcdata" != xyes],
+      [test "x$ac_cv_libcdata" != xyes && test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcdata in directory: $ac_cv_with_libcdata],
         [1])
       ])
     ])
 
   AS_IF(
@@ -524,15 +527,15 @@
     ])
   ])
 
 dnl Function to detect if libcdata dependencies are available
 AC_DEFUN([AX_LIBCDATA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
   ])
 
 dnl Function to detect how to enable libcdata
 AC_DEFUN([AX_LIBCDATA_CHECK_ENABLE],
```

### Comparing `libvhdi-20240303/m4/libcsplit.m4` & `libvhdi-20240509/m4/libcsplit.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcsplit required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcsplit is available
 dnl ac_libcsplit_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCSPLIT_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcsplit" = xno],
     [ac_cv_libcsplit=no],
     [ac_cv_libcsplit=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcsplit which returns "yes" and --with-libcsplit= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect],
+      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcsplit"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcsplit}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcsplit}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcsplit],
           [1])
@@ -143,16 +145,17 @@
             libcsplit_wide_split_string_set_segment_by_index,
             [ac_cv_libcsplit_dummy=yes],
             [ac_cv_libcsplit=no])
           ])
 
         ac_cv_libcsplit_LIBADD="-lcsplit"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_libcsplit" != xyes],
+      [test "x$ac_cv_libcsplit" != xyes && test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcsplit in directory: $ac_cv_with_libcsplit],
         [1])
       ])
     ])
 
   AS_IF(
@@ -174,15 +177,15 @@
     ])
   ])
 
 dnl Function to detect if libcsplit dependencies are available
 AC_DEFUN([AX_LIBCSPLIT_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit";
+  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit -I\$(top_srcdir)/libcsplit";
   ac_cv_libcsplit_LIBADD="../libcsplit/libcsplit.la";
 
   ac_cv_libcsplit=local
   ])
 
 dnl Function to detect how to enable libcsplit
 AC_DEFUN([AX_LIBCSPLIT_CHECK_ENABLE],
```

### Comparing `libvhdi-20240303/m4/common.m4` & `libvhdi-20240509/m4/common.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for common headers and functions
 dnl
-dnl Version: 20181117
+dnl Version: 20240308
 
 dnl Function to test if a certain feature was disabled
 AC_DEFUN([AX_COMMON_ARG_DISABLE],
 [
   AC_ARG_ENABLE(
     [$1],
     [AS_HELP_STRING(
@@ -22,15 +22,15 @@
 dnl Function to test if a certain feature was enabled
 AC_DEFUN([AX_COMMON_ARG_ENABLE],
 [
   AC_ARG_ENABLE(
     [$1],
     [AS_HELP_STRING(
       [--enable-$1],
-      [$3 [default=$4]])],
+      [$3 @<:@default=$4@:>@])],
     [ac_cv_enable_$2=$enableval],
     [ac_cv_enable_$2=$4])dnl
 
     AC_CACHE_CHECK(
       [whether to enable $3],
       [ac_cv_enable_$2],
       [ac_cv_enable_$2=$4])dnl
@@ -39,15 +39,15 @@
 dnl Function to test if the location of a certain feature was provided
 AC_DEFUN([AX_COMMON_ARG_WITH],
 [
   AC_ARG_WITH(
     [$1],
     [AS_HELP_STRING(
       [--with-$1[[=$5]]],
-      [$3 [default=$4]])],
+      [$3 @<:@default=$4@:>@])],
     [ac_cv_with_$2=$withval],
     [ac_cv_with_$2=$4])dnl
 
     AC_CACHE_CHECK(
       [whether to use $3],
       [ac_cv_with_$2],
       [ac_cv_with_$2=$4])dnl
```

### Comparing `libvhdi-20240303/m4/libcthreads.m4` & `libvhdi-20240509/m4/libcthreads.m4`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcthreads required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcthreads is available
 dnl ac_libcthreads_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCTHREADS_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcthreads" = xno],
     [ac_cv_libcthreads=no],
     [ac_cv_libcthreads=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcthreads which returns "yes" and --with-libcthreads= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect],
+      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcthreads"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcthreads}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcthreads}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcthreads],
           [1])
@@ -244,15 +246,15 @@
           [ac_cv_libcthreads_dummy=yes],
           [ac_cv_libcthreads=no])
 
         ac_cv_libcthreads_LIBADD="-lcthreads"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_libcthreads" != xyes],
+      [test "x$ac_cv_libcthreads" != xyes && test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcthreads in directory: $ac_cv_with_libcthreads],
         [1])
       ])
     ])
 
   AS_IF(
@@ -286,15 +288,15 @@
     [dnl Check for enabling pthread support
     AX_PTHREAD_CHECK_ENABLE
       ac_cv_libcthreads_multi_threading=$ac_cv_pthread],
     [ac_cv_libcthreads_multi_threading="winapi"])
 
   AS_IF(
     [test "x$ac_cv_libcthreads_multi_threading" != xno],
-    [ac_cv_libcthreads_CPPFLAGS="-I../libcthreads";
+    [ac_cv_libcthreads_CPPFLAGS="-I../libcthreads -I\$(top_srcdir)/libcthreads";
     ac_cv_libcthreads_LIBADD="../libcthreads/libcthreads.la";
 
     ac_cv_libcthreads=local],
     [ac_cv_libcthreads=no])
   ])
 
 dnl Function to detect how to enable libcthreads
```

### Comparing `libvhdi-20240303/m4/ltversion.m4` & `libvhdi-20240509/m4/ltversion.m4`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/m4/ltsugar.m4` & `libvhdi-20240509/m4/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/m4/libfdata.m4` & `libvhdi-20240509/m4/libfdata.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Functions for libfdata
 dnl
-dnl Version: 20230318
+dnl Version: 20240413
 
 dnl Function to detect if libfdata is available
 dnl ac_libfdata_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFDATA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdata" = xno],
     [ac_cv_libfdata=no],
     [ac_cv_libfdata=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfdata which returns "yes" and --with-libfdata= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect],
+      [test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfdata"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdata}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfdata],
           [1])
@@ -450,16 +452,17 @@
         dnl TODO: add functions
 
         dnl Vector list functions
         dnl TODO: add functions
 
         ac_cv_libfdata_LIBADD="-lfdata"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_libfdata" != xyes],
+      [test "x$ac_cv_libfdata" != xyes && test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfdata in directory: $ac_cv_with_libfdata],
         [1])
       ])
     ])
 
   AS_IF(
@@ -481,15 +484,15 @@
     ])
   ])
 
 dnl Function to detect if libfdata dependencies are available
 AC_DEFUN([AX_LIBFDATA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfdata_CPPFLAGS="-I../libfdata";
+  ac_cv_libfdata_CPPFLAGS="-I../libfdata -I\$(top_srcdir)/libfdata";
   ac_cv_libfdata_LIBADD="../libfdata/libfdata.la";
 
   ac_cv_libfdata=local
   ])
 
 dnl Function to detect how to enable libfdata
 AC_DEFUN([AX_LIBFDATA_CHECK_ENABLE],
```

### Comparing `libvhdi-20240303/m4/host-cpu-c-abi.m4` & `libvhdi-20240509/m4/host-cpu-c-abi.m4`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/m4/libfuse.m4` & `libvhdi-20240509/m4/libfuse.m4`

 * *Files 13% similar despite different names*

```diff
@@ -1,62 +1,90 @@
 dnl Checks for libfuse required headers and functions
 dnl
-dnl Version: 20220118
+dnl Version: 20240413
 
 dnl Function to detect if libfuse is available
 dnl ac_libfuse_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFUSE_CHECK_LIB],
-  [dnl Check if parameters were provided
-  AS_IF(
-    [test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_with_libfuse" != xauto-detect],
-    [AS_IF(
-      [test -d "$ac_cv_with_libfuse"],
-      [CFLAGS="$CFLAGS -I${ac_cv_with_libfuse}/include"
-      LDFLAGS="$LDFLAGS -L${ac_cv_with_libfuse}/lib"],
-      [AC_MSG_WARN([no such directory: $ac_cv_with_libfuse])
-      ])
-    ])
-
-  AS_IF(
-    [test "x$ac_cv_with_libfuse" = xno],
+  [AS_IF(
+    [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfuse" = xno],
     [ac_cv_libfuse=no],
-    [dnl Check for a pkg-config file
+    [dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfuse which returns "yes" and --with-libfuse= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"],
-      [PKG_CHECK_MODULES(
-        [fuse],
-        [fuse >= 2.6],
-        [ac_cv_libfuse=libfuse],
-        [ac_cv_libfuse=no])
+      [test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xauto-detect && test "x$ac_cv_with_libfuse" != xyes],
+      [AS_IF(
+        [test -d "$ac_cv_with_libfuse"],
+        [CFLAGS="$CFLAGS -I${ac_cv_with_libfuse}/include"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_libfuse}/lib"],
+        [AC_MSG_FAILURE(
+          [no such directory: $ac_cv_with_libfuse],
+          [1])
+        ])],
+      [dnl Check for a pkg-config file
+      AS_IF(
+        [test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"],
+        [PKG_CHECK_MODULES(
+          [fuse3],
+          [fuse3 >= 3.0],
+          [ac_cv_libfuse=libfuse3],
+          [ac_cv_libfuse=no])
+
+        AS_IF(
+          [test "x$ac_cv_libfuse" = xno],
+          [PKG_CHECK_MODULES(
+            [fuse],
+            [fuse >= 2.6],
+            [ac_cv_libfuse=libfuse],
+            [ac_cv_libfuse=no])
+          ])
+
+        AS_IF(
+          [test "x$ac_cv_libfuse" = xlibfuse3],
+          [ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse3_CFLAGS -D_FILE_OFFSET_BITS=64"
+          ac_cv_libfuse_LIBADD="$pkg_cv_fuse3_LIBS"])
+
+        AS_IF(
+          [test "x$ac_cv_libfuse" = xlibfuse],
+          [ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse_CFLAGS -D_FILE_OFFSET_BITS=64"
+          ac_cv_libfuse_LIBADD="$pkg_cv_fuse_LIBS"])
+        ])
       ])
 
+    backup_CPPFLAGS="$CPPFLAGS"
+
+    dnl Check for libfuse and libfuse3
     AS_IF(
-      [test "x$ac_cv_libfuse" = xlibfuse],
-      [ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse_CFLAGS"
-      ac_cv_libfuse_LIBADD="$pkg_cv_fuse_LIBS"],
+      [test "x$ac_cv_libfuse" != xlibfuse && test "x$ac_cv_libfuse" != xlibfuse3],
       [dnl Check for headers
-      AC_CHECK_HEADERS(
-        [fuse.h],
-        [ac_cv_header_fuse_h=yes],
-        [ac_cv_header_fuse_h=no])
 
-      dnl libfuse sometimes requires -D_FILE_OFFSET_BITS=64 to be set
-      dnl macFuse requires -DFUSE_USE_VERSION=26 to be set
+      CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=30"
+      AC_CHECK_HEADERS([fuse.h])
+
       AS_IF(
-        [test "x$ac_cv_header_fuse_h" = xno],
-        [AS_UNSET([ac_cv_header_fuse_h])
-        CPPFLAGS="$CPPFLAGS -D_FILE_OFFSET_BITS=64 -DFUSE_USE_VERSION=26"
+        [test "x$ac_cv_header_fuse_h" = xyes],
+        [ac_cv_libfuse=libfuse3],
+        [CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=26"
         AC_CHECK_HEADERS([fuse.h])
-      ])
+
+        AS_IF(
+          [test "x$ac_cv_header_fuse_h" = xyes],
+          [ac_cv_libfuse=libfuse])
+        ])
 
       AS_IF(
         [test "x$ac_cv_header_fuse_h" = xno],
         [ac_cv_libfuse=no],
         [dnl Check for the individual functions
-        ac_cv_libfuse=libfuse
+        AC_CHECK_LIB(
+          fuse,
+          fuse_invalidate,
+          [ac_cv_libfuse=libfuse],
+          [ac_cv_libfuse=libfuse3])
 
         AC_CHECK_LIB(
           fuse,
           fuse_daemonize,
           [ac_cv_libfuse_dummy=yes],
           [ac_cv_libfuse=no])
         AC_CHECK_LIB(
@@ -71,32 +99,30 @@
           [ac_cv_libfuse=no])
         AC_CHECK_LIB(
           fuse,
           fuse_new,
           [ac_cv_libfuse_dummy=yes],
           [ac_cv_libfuse=no])
 
-        ac_cv_libfuse_LIBADD="-lfuse";
+        dnl libfuse and libfuse3 require -D_FILE_OFFSET_BITS=64 to be set
+        ac_cv_libfuse_CPPFLAGS="-D_FILE_OFFSET_BITS=64"
+
+        AS_IF(
+          [test "x$ac_cv_libfuse" = xlibfuse3],
+          [ac_cv_libfuse_LIBADD="-lfuse3"],
+          [ac_cv_libfuse_LIBADD="-lfuse"])
         ])
       ])
 
     dnl Check for libosxfuse
     AS_IF(
       [test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_header_fuse_h" = xno],
-      [CPPFLAGS="$CPPFLAGS -DFUSE_USE_VERSION=26"
+      [CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=26"
       AC_CHECK_HEADERS([osxfuse/fuse.h])
 
-      dnl libosxfuse sometimes requires -D_FILE_OFFSET_BITS=64 to be set
-      AS_IF(
-        [test "x$ac_cv_header_osxfuse_fuse_h" = xno],
-        [AS_UNSET([ac_cv_header_osxfuse_fuse_h])
-        CPPFLAGS="$CPPFLAGS -D_FILE_OFFSET_BITS=64"
-        AC_CHECK_HEADERS([osxfuse/fuse.h])
-      ])
-
       AS_IF(
         [test "x$ac_cv_header_osxfuse_fuse_h" = xno],
         [ac_cv_libfuse=no],
         [dnl Check for the individual functions
         ac_cv_libfuse=libosxfuse
 
         AC_CHECK_LIB(
@@ -116,27 +142,46 @@
           [ac_cv_libfuse=no])
         AC_CHECK_LIB(
           osxfuse,
           fuse_new,
           [ac_cv_libfuse_dummy=yes],
           [ac_cv_libfuse=no])
 
+        dnl libosxfuse requires -D_FILE_OFFSET_BITS=64 to be set
+        ac_cv_libfuse_CPPFLAGS="-D_FILE_OFFSET_BITS=64"
+
         ac_cv_libfuse_LIBADD="-losxfuse";
         ])
       ])
+
+    AS_IF(
+      [test "x$ac_cv_libfuse" != xyes && test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xauto-detect && test "x$ac_cv_with_libfuse" != xyes],
+      [AC_MSG_FAILURE(
+        [unable to find supported libfuse in directory: $ac_cv_with_libfuse],
+        [1])
+      ])
+
+    CPPFLAGS="$backup_CPPFLAGS"
     ])
 
   AS_IF(
     [test "x$ac_cv_libfuse" = xlibfuse],
     [AC_DEFINE(
       [HAVE_LIBFUSE],
       [1],
       [Define to 1 if you have the 'fuse' library (-lfuse).])
     ])
   AS_IF(
+    [test "x$ac_cv_libfuse" = xlibfuse3],
+    [AC_DEFINE(
+      [HAVE_LIBFUSE3],
+      [1],
+      [Define to 1 if you have the 'fuse3' library (-lfuse3).])
+    ])
+  AS_IF(
     [test "x$ac_cv_libfuse" = xlibosxfuse],
     [AC_DEFINE(
       [HAVE_LIBOSXFUSE],
       [1],
       [Define to 1 if you have the 'osxfuse' library (-losxfuse).])
     ])
 
@@ -179,14 +224,20 @@
   AS_IF(
     [test "x$ac_cv_libfuse" = xlibfuse],
     [AC_SUBST(
       [ax_libfuse_pc_libs_private],
       [-lfuse])
     ])
   AS_IF(
+    [test "x$ac_cv_libfuse" = xlibfuse3],
+    [AC_SUBST(
+      [ax_libfuse_pc_libs_private],
+      [-lfuse3])
+    ])
+  AS_IF(
     [test "x$ac_cv_libfuse" = xlibosxfuse],
     [AC_SUBST(
       [ax_libfuse_pc_libs_private],
       [-losxfuse])
     ])
 
   AS_IF(
@@ -194,9 +245,18 @@
     [AC_SUBST(
       [ax_libfuse_spec_requires],
       [fuse-libs])
     AC_SUBST(
       [ax_libfuse_spec_build_requires],
       [fuse-devel])
     ])
+  AS_IF(
+    [test "x$ac_cv_libfuse" = xlibfuse3],
+    [AC_SUBST(
+      [ax_libfuse_spec_requires],
+      [fuse3-libs])
+    AC_SUBST(
+      [ax_libfuse_spec_build_requires],
+      [fuse3-devel])
+    ])
   ])
```

### Comparing `libvhdi-20240303/m4/libtool.m4` & `libvhdi-20240509/m4/libtool.m4`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/m4/po.m4` & `libvhdi-20240509/m4/po.m4`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/m4/libcerror.m4` & `libvhdi-20240509/m4/libcerror.m4`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcerror required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcerror is available
 dnl ac_libcerror_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCERROR_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcerror" = xno],
     [ac_cv_libcerror=no],
     [ac_cv_libcerror=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcerror which returns "yes" and --with-libcerror= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect],
+      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcerror"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcerror}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcerror}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcerror],
           [1])
@@ -95,16 +97,17 @@
           cerror,
           libcerror_system_set_error,
           [ac_cv_libcerror_dummy=yes],
           [ac_cv_libcerror=no])
 
         ac_cv_libcerror_LIBADD="-lcerror"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_libcerror" != xyes],
+      [test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcerror in directory: $ac_cv_with_libcerror],
         [1])
       ])
     ])
 
   AS_IF(
@@ -162,15 +165,15 @@
       [test "x$ac_cv_func_strerror" != xyes],
       [AC_MSG_FAILURE(
         [Missing functions: strerror_r and strerror],
         [1])
       ])
     ])
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
   ])
 
 dnl Function to detect how to enable libcerror
 AC_DEFUN([AX_LIBCERROR_CHECK_ENABLE],
```

### Comparing `libvhdi-20240303/m4/libcnotify.m4` & `libvhdi-20240509/m4/libcnotify.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcnotify required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcnotify is available
 dnl ac_libcnotify_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCNOTIFY_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcnotify" = xno],
     [ac_cv_libcnotify=no],
     [ac_cv_libcnotify=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcnotify which returns "yes" and --with-libcnotify= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect],
+      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcnotify"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcnotify}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcnotify}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcnotify],
           [1])
@@ -92,16 +94,17 @@
           cnotify,
           libcnotify_verbose_set,
           [ac_cv_libcnotify_dummy=yes],
           [ac_cv_libcnotify=no])
 
         ac_cv_libcnotify_LIBADD="-lcnotify"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_libcnotify" != xyes],
+      [test "x$ac_with_libcnotify" != xyes && test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcnotify in directory: $ac_cv_with_libcnotify],
         [1])
       ])
     ])
 
   AS_IF(
@@ -134,15 +137,15 @@
       [Missing headers: stdarg.h and varargs.h],
       [1])
     ])
 
   dnl Headers included in libcnotify/libcnotify_stream.c
   AC_CHECK_HEADERS([errno.h])
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
   ])
 
 dnl Function to detect how to enable libcnotify
 AC_DEFUN([AX_LIBCNOTIFY_CHECK_ENABLE],
```

### Comparing `libvhdi-20240303/m4/libfguid.m4` & `libvhdi-20240509/m4/libfguid.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfguid required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libfguid is available
 dnl ac_libfguid_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFGUID_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfguid" = xno],
     [ac_cv_libfguid=no],
     [ac_cv_libfguid=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfguid which returns "yes" and --with-libfguid= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect],
+      [test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfguid"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfguid}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfguid}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfguid],
           [1])
@@ -103,16 +105,17 @@
           fguid,
           libfguid_identifier_copy_to_utf32_string_with_index,
           [ac_cv_libfguid_dummy=yes],
           [ac_cv_libfguid=no])
 
         ac_cv_libfguid_LIBADD="-lfguid"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_libfguid" != xyes],
+      [test "x$ac_cv_libfguid" != xyes && test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfguid in directory: $ac_cv_with_libfguid],
         [1])
       ])
     ])
 
   AS_IF(
@@ -134,15 +137,15 @@
     ])
   ])
 
 dnl Function to detect if libfguid dependencies are available
 AC_DEFUN([AX_LIBFGUID_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfguid_CPPFLAGS="-I../libfguid";
+  ac_cv_libfguid_CPPFLAGS="-I../libfguid -I\$(top_srcdir)/libfguid";
   ac_cv_libfguid_LIBADD="../libfguid/libfguid.la";
 
   ac_cv_libfguid=local
   ])
 
 
 dnl Function to detect how to enable libfguid
```

### Comparing `libvhdi-20240303/m4/libbfio.m4` & `libvhdi-20240509/m4/libbfio.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libbfio required headers and functions
 dnl
-dnl Version: 20201125
+dnl Version: 20240413
 
 dnl Function to detect if libbfio is available
 dnl ac_libbfio_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBBFIO_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libbfio" = xno],
     [ac_cv_libbfio=no],
     [ac_cv_libbfio=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libbfio which returns "yes" and --with-libbfio= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect],
+      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libbfio"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libbfio}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libbfio}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libbfio],
           [1])
@@ -316,16 +318,17 @@
             libbfio_file_pool_open_wide,
             [ac_cv_libbfio_dummy=yes],
             [ac_cv_libbfio=no])
           ])
 
         ac_cv_libbfio_LIBADD="-lbfio"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_libbfio" != xyes],
+      [test "x$ac_cv_libbfio" != xyes && test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libbfio in directory: $ac_cv_with_libbfio],
         [1])
       ])
     ])
 
   AS_IF(
@@ -347,15 +350,15 @@
     ])
   ])
 
 dnl Function to detect if libbfio dependencies are available
 AC_DEFUN([AX_LIBBFIO_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libbfio_CPPFLAGS="-I../libbfio";
+  ac_cv_libbfio_CPPFLAGS="-I../libbfio -I\$(top_srcdir)/libbfio";
   ac_cv_libbfio_LIBADD="../libbfio/libbfio.la";
 
   ac_cv_libbfio=local
   ])
 
 dnl Function to detect how to enable libbfio
 AC_DEFUN([AX_LIBBFIO_CHECK_ENABLE],
```

### Comparing `libvhdi-20240303/m4/intlmacosx.m4` & `libvhdi-20240509/m4/intlmacosx.m4`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/m4/lt~obsolete.m4` & `libvhdi-20240509/m4/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/m4/lib-link.m4` & `libvhdi-20240509/m4/lib-link.m4`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/m4/iconv.m4` & `libvhdi-20240509/m4/iconv.m4`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/m4/ltoptions.m4` & `libvhdi-20240509/m4/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/m4/nls.m4` & `libvhdi-20240509/m4/nls.m4`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/m4/python.m4` & `libvhdi-20240509/m4/python.m4`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Functions for Python bindings
 dnl
-dnl Version: 20231119
+dnl Version: 20240418
 
 dnl Function to check if the python binary is available
 dnl "python${PYTHON_VERSION} python python# python#.#"
 AC_DEFUN([AX_PROG_PYTHON],
   [AS_IF(
     [test "x${PYTHON_VERSION}" != x],
     [ax_python_progs="python${PYTHON_VERSION}"],
@@ -72,18 +72,20 @@
     PYTHON_LDFLAGS=`${PYTHON_CONFIG} --ldflags 2>/dev/null`;
 
     AC_MSG_CHECKING(
       [for Python libraries])
     AC_MSG_RESULT(
       [$PYTHON_LDFLAGS])
 
-    dnl For CygWin add the -no-undefined linker flag
+    dnl For CygWin and MinGW add the -no-undefined linker flag
     AS_CASE(
-      [$host_os],
-      [cygwin*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [$build],
+      [*-*-cygwin*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [*-*-mingw*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [*-*-msys*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
       [*],[])
 
     dnl Check for the existence of Python.h
     BACKUP_CPPFLAGS="${CPPFLAGS}"
     CPPFLAGS="${CPPFLAGS} ${PYTHON_INCLUDES}"
 
     AC_CHECK_HEADERS(
```

### Comparing `libvhdi-20240303/m4/types.m4` & `libvhdi-20240509/m4/types.m4`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/m4/libfcache.m4` & `libvhdi-20240509/m4/libfcache.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfcache required headers and functions
 dnl
-dnl Version: 20230115
+dnl Version: 20240413
 
 dnl Function to detect if libfcache is available
 dnl ac_libfcache_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFCACHE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfcache" = xno],
     [ac_cv_libfcache=no],
     [ac_cv_libfcache=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfcache which returns "yes" and --with-libfcache= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect],
+      [test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfcache"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfcache}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfcache}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfcache],
           [1])
@@ -147,16 +149,17 @@
           fcache,
           libfcache_date_time_get_timestamp,
           [ac_cv_libfcache_dummy=yes],
           [ac_cv_libfcache=no])
 
         ac_cv_libfcache_LIBADD="-lfcache"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_libfcache" != xyes],
+      [test "x$ac_cv_libfcache" != xyes && test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfcache in directory: $ac_cv_with_libfcache],
         [1])
       ])
     ])
 
   AS_IF(
@@ -192,15 +195,15 @@
   AS_IF(
     [test "x$ac_cv_func_time" != xyes],
     [AC_MSG_FAILURE(
       [Missing function: time],
       [1])
     ])
 
-  ac_cv_libfcache_CPPFLAGS="-I../libfcache";
+  ac_cv_libfcache_CPPFLAGS="-I../libfcache -I\$(top_srcdir)/libfcache";
   ac_cv_libfcache_LIBADD="../libfcache/libfcache.la";
 
   ac_cv_libfcache=local
   ])
 
 dnl Function to detect how to enable libfcache
 AC_DEFUN([AX_LIBFCACHE_CHECK_ENABLE],
```

### Comparing `libvhdi-20240303/m4/pthread.m4` & `libvhdi-20240509/m4/pthread.m4`

 * *Files 18% similar despite different names*

```diff
@@ -1,183 +1,196 @@
 dnl Functions for pthread
 dnl
-dnl Version: 20130509
+dnl Version: 20240308
 
 dnl Function to detect if pthread is available
 AC_DEFUN([AX_PTHREAD_CHECK_LIB],
- [dnl Check if parameters were provided
- AS_IF(
-  [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xno && test "x$ac_cv_with_pthread" != xauto-detect],
   [AS_IF(
-   [test -d "$ac_cv_with_pthread"],
-   [CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
-   LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"],
-   [AC_MSG_WARN([no such directory: $ac_cv_with_pthread])
-   ])
-  ])
-
- AS_IF(
-  [test "x$ac_cv_with_pthread" = xno],
-  [ac_cv_pthread=no],
-  [dnl Check for headers
-  AC_CHECK_HEADERS([pthread.h])
+    [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_pthread" = xno],
+    [ac_cv_pthread=no],
+    [ac_cv_pthread=check
+    dnl Check if parameters were provided
+    dnl For both --with-pthread which returns "yes" and --with-pthread= which returns ""
+    dnl treat them as auto-detection.
+    AS_IF(
+      [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes],
+      [AS_IF(
+        [test -d "$ac_cv_with_pthread"],
+        [CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"],
+        [AC_MSG_WARN([no such directory: $ac_cv_with_pthread])
+        ])
+      ])
+    ])
+
+    AS_IF(
+      [test "x$ac_cv_pthread" = xcheck],
+      [dnl Check for headers
+      AC_CHECK_HEADERS([pthread.h])
+
+      AS_IF(
+        [test "x$ac_cv_header_pthread_h" = xno],
+        [ac_cv_pthread=no],
+        [dnl Check for the individual functions
+        ac_cv_pthread=pthread
+
+        dnl Thread functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_create,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_exit,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_join,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Condition functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_broadcast,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_signal,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_wait,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Mutex functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_lock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_trylock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_unlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Read/Write lock functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_rdlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_wrlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_unlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        ac_cv_pthread_LIBADD="-lpthread";
+      ])
+
+    AS_IF(
+      [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes],
+      [AC_MSG_FAILURE(
+        [unable to find supported pthread in directory: $ac_cv_with_pthread],
+        [1])
+      ])
+    ])
 
   AS_IF(
-   [test "x$ac_cv_header_pthread_h" = xno],
-   [ac_cv_pthread=no],
-   [dnl Check for the individual functions
-   ac_cv_pthread=pthread
-
-   dnl Thread functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_create,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_exit,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_join,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Condition functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_broadcast,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_signal,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_wait,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Mutex functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_lock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_trylock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_unlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Read/Write lock functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_rdlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_wrlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_unlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   ac_cv_pthread_LIBADD="-lpthread";
-   ])
-  ])
+    [test "x$ac_cv_pthread" = xpthread],
+    [AC_DEFINE(
+      [HAVE_PTHREAD],
+      [1],
+      [Define to 1 if you have the 'pthread' library (-lpthread).])
+    ])
 
- AS_IF(
-  [test "x$ac_cv_pthread" = xpthread],
-  [AC_DEFINE(
-   [HAVE_PTHREAD],
-   [1],
-   [Define to 1 if you have the 'pthread' library (-lpthread).])
-  ])
-
- AS_IF(
-  [test "x$ac_cv_pthread" != xno],
-  [AC_SUBST(
-   [HAVE_PTHREAD],
-   [1]) ],
-  [AC_SUBST(
-   [HAVE_PTHREAD],
-   [0])
+  AS_IF(
+    [test "x$ac_cv_pthread" != xno],
+    [AC_SUBST(
+      [HAVE_PTHREAD],
+      [1]) ],
+    [AC_SUBST(
+      [HAVE_PTHREAD],
+      [0])
+    ])
   ])
- ])
 
 dnl Function to detect how to enable pthread
 AC_DEFUN([AX_PTHREAD_CHECK_ENABLE],
- [AX_COMMON_ARG_WITH(
-  [pthread],
-  [pthread],
-  [search for pthread in includedir and libdir or in the specified DIR, or no if not to use pthread],
-  [auto-detect],
-  [DIR])
-
- dnl Check for a shared library version
- AX_PTHREAD_CHECK_LIB
-
- AS_IF(
-  [test "x$ac_cv_pthread_CPPFLAGS" != "x"],
-  [AC_SUBST(
-   [PTHREAD_CPPFLAGS],
-   [$ac_cv_pthread_CPPFLAGS])
-  ])
- AS_IF(
-  [test "x$ac_cv_pthread_LIBADD" != "x"],
-  [AC_SUBST(
-   [PTHREAD_LIBADD],
-   [$ac_cv_pthread_LIBADD])
-  ])
+  [AX_COMMON_ARG_WITH(
+    [pthread],
+    [pthread],
+    [search for pthread in includedir and libdir or in the specified DIR, or no if not to use pthread],
+    [auto-detect],
+    [DIR])
 
- AS_IF(
-  [test "x$ac_cv_pthread" = xpthread],
-  [AC_SUBST(
-   [ax_pthread_pc_libs_private],
-   [-lpthread])
+  dnl Check for a shared library version
+  AX_PTHREAD_CHECK_LIB
+
+  AS_IF(
+    [test "x$ac_cv_pthread_CPPFLAGS" != "x"],
+    [AC_SUBST(
+      [PTHREAD_CPPFLAGS],
+      [$ac_cv_pthread_CPPFLAGS])
+    ])
+  AS_IF(
+    [test "x$ac_cv_pthread_LIBADD" != "x"],
+    [AC_SUBST(
+      [PTHREAD_LIBADD],
+      [$ac_cv_pthread_LIBADD])
+    ])
+
+  AS_IF(
+    [test "x$ac_cv_pthread" = xpthread],
+    [AC_SUBST(
+      [ax_pthread_pc_libs_private],
+      [-lpthread])
+    ])
   ])
- ])
```

### Comparing `libvhdi-20240303/include/libvhdi.h` & `libvhdi-20240509/include/libvhdi.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/include/libvhdi.h.in` & `libvhdi-20240509/include/libvhdi.h.in`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/include/libvhdi/definitions.h.in` & `libvhdi-20240509/include/libvhdi/definitions.h.in`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/include/libvhdi/definitions.h` & `libvhdi-20240509/include/libvhdi/definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -20,19 +20,19 @@
  */
 
 #if !defined( _LIBVHDI_DEFINITIONS_H )
 #define _LIBVHDI_DEFINITIONS_H
 
 #include <libvhdi/types.h>
 
-#define LIBVHDI_VERSION			20240303
+#define LIBVHDI_VERSION			20240509
 
 /* The version string
  */
-#define LIBVHDI_VERSION_STRING		"20240303"
+#define LIBVHDI_VERSION_STRING		"20240509"
 
 /* The access flags definitions
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBVHDI_ACCESS_FLAGS
```

### Comparing `libvhdi-20240303/include/libvhdi/types.h.in` & `libvhdi-20240509/include/libvhdi/types.h.in`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/include/libvhdi/types.h` & `libvhdi-20240509/include/libvhdi/types.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/include/libvhdi/features.h.in` & `libvhdi-20240509/include/libvhdi/features.h.in`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/include/libvhdi/error.h` & `libvhdi-20240509/include/libvhdi/error.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/include/libvhdi/extern.h` & `libvhdi-20240509/include/libvhdi/extern.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/include/libvhdi/features.h` & `libvhdi-20240509/include/libvhdi/features.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/include/libvhdi/codepage.h` & `libvhdi-20240509/include/libvhdi/codepage.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/include/Makefile.in` & `libvhdi-20240509/include/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -429,14 +429,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -507,15 +509,20 @@
 
 EXTRA_DIST = \
 	libvhdi.h.in \
 	libvhdi/definitions.h.in \
 	libvhdi/features.h.in \
 	libvhdi/types.h.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libvhdi.h \
+	libvhdi/definitions.h \
+	libvhdi/features.h \
+	libvhdi/types.h \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -712,23 +719,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -810,17 +819,10 @@
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-includeHEADERS \
 	uninstall-pkgincludeHEADERS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libvhdi.h
-	-rm -f libvhdi/definitions.h
-	-rm -f libvhdi/features.h
-	-rm -f libvhdi/types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libvhdi-20240303/common/config_borlandc.h` & `libvhdi-20240509/common/config_borlandc.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/common/file_stream.h` & `libvhdi-20240509/common/file_stream.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/common/memory.h` & `libvhdi-20240509/common/memory.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/common/byte_stream.h` & `libvhdi-20240509/common/byte_stream.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/common/common.h` & `libvhdi-20240509/common/common.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/common/config_winapi.h` & `libvhdi-20240509/common/config_winapi.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/common/system_string.h` & `libvhdi-20240509/common/system_string.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/common/types.h.in` & `libvhdi-20240509/common/types.h.in`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/common/types.h` & `libvhdi-20240509/common/types.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/common/config.h.in` & `libvhdi-20240509/common/config.h.in`

 * *Files 0% similar despite different names*

```diff
@@ -206,14 +206,17 @@
 
 /* Define to 1 if you have the <libfguid.h> header file. */
 #undef HAVE_LIBFGUID_H
 
 /* Define to 1 if you have the 'fuse' library (-lfuse). */
 #undef HAVE_LIBFUSE
 
+/* Define to 1 if you have the 'fuse3' library (-lfuse3). */
+#undef HAVE_LIBFUSE3
+
 /* Define to 1 if you have the <libintl.h> header file. */
 #undef HAVE_LIBINTL_H
 
 /* Define to 1 if you have the 'osxfuse' library (-losxfuse). */
 #undef HAVE_LIBOSXFUSE
 
 /* Define to 1 if you have the `una' library (-luna). */
```

### Comparing `libvhdi-20240303/common/config.h` & `libvhdi-20240509/common/config.h`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,18 @@
 /* Define to 1 if you have the `fguid' library (-lfguid). */
 /* #undef HAVE_LIBFGUID */
 
 /* Define to 1 if you have the <libfguid.h> header file. */
 /* #undef HAVE_LIBFGUID_H */
 
 /* Define to 1 if you have the 'fuse' library (-lfuse). */
-#define HAVE_LIBFUSE 1
+/* #undef HAVE_LIBFUSE */
+
+/* Define to 1 if you have the 'fuse3' library (-lfuse3). */
+#define HAVE_LIBFUSE3 1
 
 /* Define to 1 if you have the <libintl.h> header file. */
 #define HAVE_LIBINTL_H 1
 
 /* Define to 1 if you have the 'osxfuse' library (-losxfuse). */
 /* #undef HAVE_LIBOSXFUSE */
 
@@ -532,24 +535,24 @@
 /* Define to the address where bug reports for this package should be sent. */
 #define PACKAGE_BUGREPORT "joachim.metz@gmail.com"
 
 /* Define to the full name of this package. */
 #define PACKAGE_NAME "libvhdi"
 
 /* Define to the full name and version of this package. */
-#define PACKAGE_STRING "libvhdi 20240303"
+#define PACKAGE_STRING "libvhdi 20240509"
 
 /* Define to the one symbol short name of this package. */
 #define PACKAGE_TARNAME "libvhdi"
 
 /* Define to the home page for this package. */
 #define PACKAGE_URL ""
 
 /* Define to the version of this package. */
-#define PACKAGE_VERSION "20240303"
+#define PACKAGE_VERSION "20240509"
 
 /* The size of `int', as computed by sizeof. */
 #define SIZEOF_INT 4
 
 /* The size of `long', as computed by sizeof. */
 #define SIZEOF_LONG 8
 
@@ -570,15 +573,15 @@
 /* Define to 1 if strerror_r returns char *. */
 /* #undef STRERROR_R_CHAR_P */
 
 /* Define to 1 if your <sys/time.h> declares `struct tm'. */
 /* #undef TM_IN_SYS_TIME */
 
 /* Version number of package */
-#define VERSION "20240303"
+#define VERSION "20240509"
 
 /* Number of bits in a file offset, on hosts where this is settable. */
 /* #undef _FILE_OFFSET_BITS */
 
 /* Define for large files, on AIX-style hosts. */
 /* #undef _LARGE_FILES */
```

### Comparing `libvhdi-20240303/common/wide_string.h` & `libvhdi-20240509/common/wide_string.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/common/narrow_string.h` & `libvhdi-20240509/common/narrow_string.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/common/config_msc.h` & `libvhdi-20240509/common/config_msc.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/common/Makefile.in` & `libvhdi-20240509/common/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -399,14 +399,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -460,15 +462,17 @@
 sharedstatedir = @sharedstatedir@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
-AM_CPPFLAGS = -I$(top_srcdir)/include
+AM_CPPFLAGS = \
+	-I../include -I$(top_srcdir)/include
+
 EXTRA_DIST = \
 	byte_stream.h \
 	common.h \
 	config.h \
 	config_borlandc.h \
 	config_msc.h \
 	config_winapi.h \
@@ -476,15 +480,18 @@
 	memory.h \
 	narrow_string.h \
 	system_string.h \
 	types.h \
 	types.h.in \
 	wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	config.h \
+	types.h \
+	Makefile \
 	Makefile.in
 
 all: config.h
 	$(MAKE) $(AM_MAKEFLAGS) all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -652,23 +659,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-hdr distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -748,15 +757,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f config.h
-	-rm -f types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libvhdi-20240303/libclocale/libclocale_wide_string.c` & `libvhdi-20240509/libclocale/libclocale_wide_string.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libclocale/libclocale_support.h` & `libvhdi-20240509/libclocale/libclocale_support.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libclocale/Makefile.am` & `libvhdi-20240509/libclocale/Makefile.am`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 if HAVE_LOCAL_LIBCLOCALE
 AM_CPPFLAGS = \
 	-DLOCALEDIR=\"$(datadir)/locale\" \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libclocale.la
 
 libclocale_la_SOURCES = \
 	libclocale_codepage.c libclocale_codepage.h \
 	libclocale_definitions.h \
@@ -14,19 +14,17 @@
 	libclocale_libcerror.h \
 	libclocale_locale.c libclocale_locale.h \
 	libclocale_support.c libclocale_support.h \
 	libclocale_unused.h \
 	libclocale_wide_string.c libclocale_wide_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libclocale ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libclocale_la_SOURCES)
```

### Comparing `libvhdi-20240303/libclocale/libclocale_definitions.h` & `libvhdi-20240509/libclocale/libclocale_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 #include <libclocale/definitions.h>
 
 /* The definitions in <libclocale/definitions.h> are copied here
  * for local use of libclocale
  */
 #else
 
-#define LIBCLOCALE_VERSION					20240107
+#define LIBCLOCALE_VERSION					20240414
 
 /* The libclocale version string
  */
-#define LIBCLOCALE_VERSION_STRING				"20240107"
+#define LIBCLOCALE_VERSION_STRING				"20240414"
 
 /* The codepage feature flag definitions
  */
 enum LIBCLOCALE_CODEPAGES_FEATURE_FLAGS
 {
 	LIBCLOCALE_CODEPAGE_FEATURE_FLAG_HAVE_ISO_8859		= 0x00000001UL,
 	LIBCLOCALE_CODEPAGE_FEATURE_FLAG_HAVE_KOI8		= 0x00000002UL,
```

### Comparing `libvhdi-20240303/libclocale/libclocale_unused.h` & `libvhdi-20240509/libclocale/libclocale_unused.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libclocale/libclocale_libcerror.h` & `libvhdi-20240509/libclocale/libclocale_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libclocale/libclocale_locale.h` & `libvhdi-20240509/libclocale/libclocale_locale.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libclocale/libclocale_support.c` & `libvhdi-20240509/libclocale/libclocale_support.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libclocale/libclocale_codepage.c` & `libvhdi-20240509/libclocale/libclocale_codepage.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libclocale/libclocale_locale.c` & `libvhdi-20240509/libclocale/libclocale_locale.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libclocale/Makefile.in` & `libvhdi-20240509/libclocale/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -443,14 +443,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -506,30 +508,31 @@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCLOCALE_TRUE@AM_CPPFLAGS = \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	-DLOCALEDIR=\"$(datadir)/locale\" \
-@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCLOCALE_TRUE@noinst_LTLIBRARIES = libclocale.la
 @HAVE_LOCAL_LIBCLOCALE_TRUE@libclocale_la_SOURCES = \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_codepage.c libclocale_codepage.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_definitions.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_extern.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_libcerror.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_locale.c libclocale_locale.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_support.c libclocale_support.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_unused.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_wide_string.c libclocale_wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -732,24 +735,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libclocale_codepage.Plo
+	-rm -f ./$(DEPDIR)/libclocale_locale.Plo
+	-rm -f ./$(DEPDIR)/libclocale_support.Plo
+	-rm -f ./$(DEPDIR)/libclocale_wide_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -836,17 +845,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libclocale ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libclocale_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvhdi-20240303/libclocale/libclocale_extern.h` & `libvhdi-20240509/libclocale/libclocale_extern.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libclocale/libclocale_wide_string.h` & `libvhdi-20240509/libclocale/libclocale_wide_string.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libclocale/libclocale_codepage.h` & `libvhdi-20240509/libclocale/libclocale_codepage.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi.spec.in` & `libvhdi-20240509/libvhdi.spec.in`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfcache/libfcache_libcdata.h` & `libvhdi-20240509/libfcache/libfcache_libcdata.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfcache/libfcache_types.h` & `libvhdi-20240509/libfcache/libfcache_types.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfcache/libfcache_cache_value.c` & `libvhdi-20240509/libfcache/libfcache_cache_value.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfcache/libfcache_unused.h` & `libvhdi-20240509/libfcache/libfcache_unused.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfcache/Makefile.am` & `libvhdi-20240509/libfcache/Makefile.am`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFCACHE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfcache.la
 
@@ -19,19 +19,17 @@
 	libfcache_libcdata.h \
 	libfcache_libcerror.h \
 	libfcache_support.c libfcache_support.h \
 	libfcache_types.h \
 	libfcache_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfcache ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfcache_la_SOURCES)
```

### Comparing `libvhdi-20240303/libfcache/libfcache_support.h` & `libvhdi-20240509/libfcache/libfcache_support.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfcache/libfcache_error.h` & `libvhdi-20240509/libfcache/libfcache_error.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfcache/libfcache_support.c` & `libvhdi-20240509/libfcache/libfcache_support.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfcache/libfcache_cache.h` & `libvhdi-20240509/libfcache/libfcache_cache.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfcache/libfcache_error.c` & `libvhdi-20240509/libfcache/libfcache_error.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfcache/libfcache_libcerror.h` & `libvhdi-20240509/libfcache/libfcache_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfcache/libfcache_date_time.c` & `libvhdi-20240509/libfcache/libfcache_date_time.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfcache/libfcache_extern.h` & `libvhdi-20240509/libfcache/libfcache_extern.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfcache/libfcache_cache_value.h` & `libvhdi-20240509/libfcache/libfcache_cache_value.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfcache/Makefile.in` & `libvhdi-20240509/libfcache/Makefile.in`

 * *Files 0% similar despite different names*

```diff
@@ -446,14 +446,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -508,16 +510,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFCACHE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFCACHE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFCACHE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFCACHE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFCACHE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFCACHE_TRUE@noinst_LTLIBRARIES = libfcache.la
 @HAVE_LOCAL_LIBFCACHE_TRUE@libfcache_la_SOURCES = \
@@ -529,15 +531,16 @@
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_extern.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_libcdata.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_libcerror.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_support.c libfcache_support.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_types.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -741,24 +744,31 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfcache_cache.Plo
+	-rm -f ./$(DEPDIR)/libfcache_cache_value.Plo
+	-rm -f ./$(DEPDIR)/libfcache_date_time.Plo
+	-rm -f ./$(DEPDIR)/libfcache_error.Plo
+	-rm -f ./$(DEPDIR)/libfcache_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -846,17 +856,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfcache ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfcache_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvhdi-20240303/libfcache/libfcache_date_time.h` & `libvhdi-20240509/libfcache/libfcache_date_time.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libfcache/libfcache_definitions.h` & `libvhdi-20240509/libfcache/libfcache_definitions.h`

 * *Files 6% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBFCACHE )
 #include <libfcache/definitions.h>
 
 /* The definitions in <libfcache/definitions.h> are copied here
  * for local use of libfcache
  */
 #else
-#define LIBFCACHE_VERSION					20240112
+#define LIBFCACHE_VERSION					20240414
 
 /* The libfcache version string
  */
-#define LIBFCACHE_VERSION_STRING				"20240112"
+#define LIBFCACHE_VERSION_STRING				"20240414"
 
 /* The cache value flags definitions
  */
 enum LIBFCACHE_CACHE_VALUE_FLAGS
 {
 	/* The cache value is not managed by the library
 	 */
```

### Comparing `libvhdi-20240303/libfcache/libfcache_cache.c` & `libvhdi-20240509/libfcache/libfcache_cache.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/Makefile.am` & `libvhdi-20240509/Makefile.am`

 * *Files 10% similar despite different names*

```diff
@@ -58,16 +58,23 @@
 EXTRA_DIST = \
 	$(DPKG_FILES) \
 	$(GETTEXT_FILES) \
 	$(PKGCONFIG_FILES) \
 	$(SETUP_PY_FILES) \
 	$(SPEC_FILES)
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	config.status \
+	config.cache \
+	config.log \
+	libvhdi.pc \
+	libvhdi.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 
 pkgconfig_DATA = \
 	libvhdi.pc
 
 libtool:
@@ -90,19 +97,7 @@
 	(cd $(srcdir)/libbfio && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfcache && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfdata && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfguid && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libvhdi && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libvhdi.pc
-	-rm -f libvhdi.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
```

### Comparing `libvhdi-20240303/libbfio/libbfio_file_range.h` & `libvhdi-20240509/libbfio/libbfio_file_range.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvhdi-20240303/libbfio/libbfio_file_range_io_handle.c` & `libvhdi-20240509/libbfio/libbfio_file_range_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvhdi-20240303/libbfio/libbfio_support.c` & `libvhdi-20240509/libbfio/libbfio_support.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvhdi-20240303/libbfio/libbfio_libcpath.h` & `libvhdi-20240509/libbfio/libbfio_libcpath.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal libcpath header
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvhdi-20240303/libbfio/libbfio_error.h` & `libvhdi-20240509/libbfio/libbfio_error.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvhdi-20240303/libbfio/libbfio_libclocale.h` & `libvhdi-20240509/libbfio/libbfio_libclocale.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libclocale header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvhdi-20240303/libbfio/libbfio_error.c` & `libvhdi-20240509/libbfio/libbfio_error.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvhdi-20240303/libbfio/libbfio_libuna.h` & `libvhdi-20240509/libbfio/libbfio_libuna.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libuna header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvhdi-20240303/libbfio/libbfio_file_io_handle.h` & `libvhdi-20240509/libbfio/libbfio_file_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvhdi-20240303/libbfio/libbfio_file_pool.h` & `libvhdi-20240509/libbfio/libbfio_file_pool.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvhdi-20240303/libbfio/libbfio_file_range.c` & `libvhdi-20240509/libbfio/libbfio_file_range.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvhdi-20240303/libbfio/libbfio_types.h` & `libvhdi-20240509/libbfio/libbfio_types.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvhdi-20240303/libbfio/libbfio_unused.h` & `libvhdi-20240509/libbfio/libbfio_unused.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvhdi-20240303/libbfio/libbfio_libcdata.h` & `libvhdi-20240509/libbfio/libbfio_libcdata.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcdata header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvhdi-20240303/libbfio/libbfio_file.h` & `libvhdi-20240509/libbfio/libbfio_file.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvhdi-20240303/libbfio/Makefile.am` & `libvhdi-20240509/libbfio/Makefile.am`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBBFIO
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -38,17 +38,17 @@
 	libbfio_pool.c libbfio_pool.h \
 	libbfio_support.c libbfio_support.h \
 	libbfio_system_string.c libbfio_system_string.h \
 	libbfio_types.h \
 	libbfio_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libbfio ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libbfio_la_SOURCES)
```

### Comparing `libvhdi-20240303/libbfio/libbfio_libcfile.h` & `libvhdi-20240509/libbfio/libbfio_libcfile.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal libcfile header
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvhdi-20240303/libbfio/libbfio_definitions.h` & `libvhdi-20240509/libbfio/libbfio_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBBFIO )
 #include <libbfio/definitions.h>
 
 /* The definitions in <libbfio/definitions.h> are copied here
  * for local use of libbfio
  */
 #else
-#define LIBBFIO_VERSION					20221025
+#define LIBBFIO_VERSION					20240414
 
 /* The libbfio version string
  */
-#define LIBBFIO_VERSION_STRING				"20221025"
+#define LIBBFIO_VERSION_STRING				"20240414"
 
 /* The library flags definitions
  */
 enum LIBBFIO_FLAGS
 {
 	/* The IO handle is not managed by the library
 	 */
```

### Comparing `libvhdi-20240303/libbfio/libbfio_codepage.h` & `libvhdi-20240509/libbfio/libbfio_codepage.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Codepage functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvhdi-20240303/libbfio/libbfio_file_io_handle.c` & `libvhdi-20240509/libbfio/libbfio_file_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvhdi-20240303/libbfio/libbfio_support.h` & `libvhdi-20240509/libbfio/libbfio_support.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvhdi-20240303/libbfio/libbfio_memory_range.h` & `libvhdi-20240509/libbfio/libbfio_memory_range.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvhdi-20240303/libbfio/libbfio_file_pool.c` & `libvhdi-20240509/libbfio/libbfio_file_pool.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvhdi-20240303/libbfio/libbfio_file_range_io_handle.h` & `libvhdi-20240509/libbfio/libbfio_file_range_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvhdi-20240303/libbfio/libbfio_libcthreads.h` & `libvhdi-20240509/libbfio/libbfio_libcthreads.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcthreads header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvhdi-20240303/libbfio/libbfio_system_string.h` & `libvhdi-20240509/libbfio/libbfio_system_string.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * System string functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvhdi-20240303/libbfio/libbfio_memory_range_io_handle.c` & `libvhdi-20240509/libbfio/libbfio_memory_range_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvhdi-20240303/libbfio/libbfio_handle.c` & `libvhdi-20240509/libbfio/libbfio_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvhdi-20240303/libbfio/libbfio_file.c` & `libvhdi-20240509/libbfio/libbfio_file.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvhdi-20240303/libbfio/libbfio_handle.h` & `libvhdi-20240509/libbfio/libbfio_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvhdi-20240303/libbfio/libbfio_memory_range.c` & `libvhdi-20240509/libbfio/libbfio_memory_range.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvhdi-20240303/libbfio/libbfio_pool.c` & `libvhdi-20240509/libbfio/libbfio_pool.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvhdi-20240303/libbfio/libbfio_libcerror.h` & `libvhdi-20240509/libbfio/libbfio_libcerror.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvhdi-20240303/libbfio/Makefile.in` & `libvhdi-20240509/libbfio/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -464,14 +464,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -526,16 +528,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBBFIO_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBBFIO_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBBFIO_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBBFIO_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBBFIO_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCFILE_CPPFLAGS@ \
@@ -566,15 +568,16 @@
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_memory_range_io_handle.c libbfio_memory_range_io_handle.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_pool.c libbfio_pool.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_support.c libbfio_support.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_system_string.c libbfio_system_string.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_types.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -785,24 +788,38 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libbfio_error.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_pool.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_range.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_range_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_memory_range.Plo
+	-rm -f ./$(DEPDIR)/libbfio_memory_range_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_pool.Plo
+	-rm -f ./$(DEPDIR)/libbfio_support.Plo
+	-rm -f ./$(DEPDIR)/libbfio_system_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -871,14 +888,16 @@
 
 ps-am:
 
 sources: sources-am
 
 sources-am: sources-local
 
+splint: splint-am
+
 splint-am: splint-local
 
 uninstall-am:
 
 .MAKE: install-am install-strip
 
 .PHONY: CTAGS GTAGS TAGS all all-am am--depfiles check check-am clean \
@@ -889,23 +908,22 @@
 	install-data install-data-am install-dvi install-dvi-am \
 	install-exec install-exec-am install-html install-html-am \
 	install-info install-info-am install-man install-pdf \
 	install-pdf-am install-ps install-ps-am install-strip \
 	installcheck installcheck-am installdirs maintainer-clean \
 	maintainer-clean-generic mostlyclean mostlyclean-compile \
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
-	sources-am sources-local splint splint-am splint-local tags \
-	tags-am uninstall uninstall-am
+	sources-am sources-local splint-am splint-local tags tags-am \
+	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libbfio ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libbfio_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libvhdi-20240303/libbfio/libbfio_system_string.c` & `libvhdi-20240509/libbfio/libbfio_system_string.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * System string functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvhdi-20240303/libbfio/libbfio_memory_range_io_handle.h` & `libvhdi-20240509/libbfio/libbfio_memory_range_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvhdi-20240303/libbfio/libbfio_extern.h` & `libvhdi-20240509/libbfio/libbfio_extern.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvhdi-20240303/libbfio/libbfio_pool.h` & `libvhdi-20240509/libbfio/libbfio_pool.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvhdi-20240303/config.guess` & `libvhdi-20240509/config.guess`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/dpkg/copyright` & `libvhdi-20240509/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/dpkg/control` & `libvhdi-20240509/dpkg/control`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/dpkg/rules` & `libvhdi-20240509/dpkg/rules`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/COPYING.LESSER` & `libvhdi-20240509/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/configure` & `libvhdi-20240509/configure`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for libvhdi 20240303.
+# Generated by GNU Autoconf 2.71 for libvhdi 20240509.
 #
 # Report bugs to <joachim.metz@gmail.com>.
 #
 #
 # Copyright (C) 1992-1996, 1998-2017, 2020-2021 Free Software Foundation,
 # Inc.
 #
@@ -617,16 +617,16 @@
 subdirs=
 MFLAGS=
 MAKEFLAGS=
 
 # Identity of this package.
 PACKAGE_NAME='libvhdi'
 PACKAGE_TARNAME='libvhdi'
-PACKAGE_VERSION='20240303'
-PACKAGE_STRING='libvhdi 20240303'
+PACKAGE_VERSION='20240509'
+PACKAGE_STRING='libvhdi 20240509'
 PACKAGE_BUGREPORT='joachim.metz@gmail.com'
 PACKAGE_URL=''
 
 ac_unique_file="include/libvhdi.h.in"
 # Factoring default headers for most tests.
 ac_includes_default="\
 #include <stddef.h>
@@ -678,14 +678,16 @@
 ax_libfuse_spec_requires
 ax_libfuse_pc_libs_private
 LIBFUSE_LIBADD
 LIBFUSE_CPPFLAGS
 HAVE_LIBFUSE
 fuse_LIBS
 fuse_CFLAGS
+fuse3_LIBS
+fuse3_CFLAGS
 HAVE_PYTHON_TESTS_FALSE
 HAVE_PYTHON_TESTS_TRUE
 HAVE_PYTHON_FALSE
 HAVE_PYTHON_TRUE
 PYTHON_PACKAGE_DIR
 PYTHON_LIBRARY_DIR
 pyexecdir
@@ -1087,14 +1089,16 @@
 libbfio_LIBS
 libfcache_CFLAGS
 libfcache_LIBS
 libfdata_CFLAGS
 libfdata_LIBS
 libfguid_CFLAGS
 libfguid_LIBS
+fuse3_CFLAGS
+fuse3_LIBS
 fuse_CFLAGS
 fuse_LIBS'
 
 
 # Initialize some variables set by options.
 ac_init_help=
 ac_init_version=false
@@ -1637,15 +1641,15 @@
 #
 # Report the --help message.
 #
 if test "$ac_init_help" = "long"; then
   # Omit some internal or obsolete options to make the list less imposing.
   # This message is too long to be a string in the A/UX 3.1 sh.
   cat <<_ACEOF
-\`configure' configures libvhdi 20240303 to adapt to many kinds of systems.
+\`configure' configures libvhdi 20240509 to adapt to many kinds of systems.
 
 Usage: $0 [OPTION]... [VAR=VALUE]...
 
 To assign environment variables (e.g., CC, CFLAGS...), specify them as
 VAR=VALUE.  See below for descriptions of some of the useful variables.
 
 Defaults for the options are specified in brackets.
@@ -1708,15 +1712,15 @@
   --build=BUILD     configure for building on BUILD [guessed]
   --host=HOST       cross-compile to build programs to run on HOST [BUILD]
 _ACEOF
 fi
 
 if test -n "$ac_init_help"; then
   case $ac_init_help in
-     short | recursive ) echo "Configuration of libvhdi 20240303:";;
+     short | recursive ) echo "Configuration of libvhdi 20240509:";;
    esac
   cat <<\_ACEOF
 
 Optional Features:
   --disable-option-checking  ignore unrecognized --enable/--with options
   --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
   --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
@@ -1880,14 +1884,17 @@
               C compiler flags for libfdata, overriding pkg-config
   libfdata_LIBS
               linker flags for libfdata, overriding pkg-config
   libfguid_CFLAGS
               C compiler flags for libfguid, overriding pkg-config
   libfguid_LIBS
               linker flags for libfguid, overriding pkg-config
+  fuse3_CFLAGS
+              C compiler flags for fuse3, overriding pkg-config
+  fuse3_LIBS  linker flags for fuse3, overriding pkg-config
   fuse_CFLAGS C compiler flags for fuse, overriding pkg-config
   fuse_LIBS   linker flags for fuse, overriding pkg-config
 
 Use these variables to override the choices made by `configure' or to help
 it to find libraries and programs with nonstandard names/locations.
 
 Report bugs to <joachim.metz@gmail.com>.
@@ -1950,15 +1957,15 @@
     cd "$ac_pwd" || { ac_status=$?; break; }
   done
 fi
 
 test -n "$ac_init_help" && exit $ac_status
 if $ac_init_version; then
   cat <<\_ACEOF
-libvhdi configure 20240303
+libvhdi configure 20240509
 generated by GNU Autoconf 2.71
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This configure script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it.
 _ACEOF
   exit
@@ -2671,15 +2678,15 @@
     ac_configure_args_raw=`      printf "%s\n" "$ac_configure_args_raw" | sed "$ac_safe_unquote"`;;
 esac
 
 cat >config.log <<_ACEOF
 This file contains any messages produced by compilers while
 running configure, to aid debugging if configure makes a mistake.
 
-It was created by libvhdi $as_me 20240303, which was
+It was created by libvhdi $as_me 20240509, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   $ $0$ac_configure_args_raw
 
 _ACEOF
 exec 5>>config.log
 {
@@ -4160,15 +4167,15 @@
     CYGPATH_W=echo
   fi
 fi
 
 
 # Define the identity of the package.
  PACKAGE='libvhdi'
- VERSION='20240303'
+ VERSION='20240509'
 
 
 printf "%s\n" "#define PACKAGE \"$PACKAGE\"" >>confdefs.h
 
 
 printf "%s\n" "#define VERSION \"$VERSION\"" >>confdefs.h
 
@@ -23755,15 +23762,15 @@
 printf "%s\n" "$ac_cv_with_libcerror" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcerror" = xno
 then :
   ac_cv_libcerror=no
 else $as_nop
   ac_cv_libcerror=check
-        if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect
+                if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
 then :
   if test -d "$ac_cv_with_libcerror"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcerror}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcerror}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -24254,15 +24261,16 @@
 fi
 
 
         ac_cv_libcerror_LIBADD="-lcerror"
 fi
 
 fi
-    if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_libcerror" != xyes
+
+    if test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcerror in directory: $ac_cv_with_libcerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -24404,15 +24412,15 @@
 as_fn_error 1 "Missing functions: strerror_r and strerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCERROR 1" >>confdefs.h
@@ -24506,15 +24514,15 @@
     ac_cv_libcthreads_multi_threading="no"
 else $as_nop
       if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcthreads" = xno
 then :
   ac_cv_libcthreads=no
 else $as_nop
   ac_cv_libcthreads=check
-        if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect
+                if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes
 then :
   if test -d "$ac_cv_with_libcthreads"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcthreads}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcthreads}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -26146,15 +26154,15 @@
 
 
         ac_cv_libcthreads_LIBADD="-lcthreads"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_libcthreads" != xyes
+    if test "x$ac_cv_libcthreads" != xyes && test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcthreads in directory: $ac_cv_with_libcthreads
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -26208,47 +26216,52 @@
   printf %s "(cached) " >&6
 else $as_nop
   ac_cv_with_pthread=auto-detect
 fi
 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_with_pthread" >&5
 printf "%s\n" "$ac_cv_with_pthread" >&6; }
 
-   if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xno && test "x$ac_cv_with_pthread" != xauto-detect
+    if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_pthread" = xno
+then :
+  ac_cv_pthread=no
+else $as_nop
+  ac_cv_pthread=check
+                if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes
 then :
   if test -d "$ac_cv_with_pthread"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
-   LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"
 else $as_nop
   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: WARNING: no such directory: $ac_cv_with_pthread" >&5
 printf "%s\n" "$as_me: WARNING: no such directory: $ac_cv_with_pthread" >&2;}
 
 fi
 
 fi
 
- if test "x$ac_cv_with_pthread" = xno
+fi
+
+    if test "x$ac_cv_pthread" = xcheck
 then :
-  ac_cv_pthread=no
-else $as_nop
-    ac_fn_c_check_header_compile "$LINENO" "pthread.h" "ac_cv_header_pthread_h" "$ac_includes_default"
+        ac_fn_c_check_header_compile "$LINENO" "pthread.h" "ac_cv_header_pthread_h" "$ac_includes_default"
 if test "x$ac_cv_header_pthread_h" = xyes
 then :
   printf "%s\n" "#define HAVE_PTHREAD_H 1" >>confdefs.h
 
 fi
 
 
-  if test "x$ac_cv_header_pthread_h" = xno
+      if test "x$ac_cv_header_pthread_h" = xno
 then :
   ac_cv_pthread=no
 else $as_nop
-     ac_cv_pthread=pthread
+          ac_cv_pthread=pthread
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_create in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_create in -lpthread" >&5
 printf %s "checking for pthread_create in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_create+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26282,15 +26295,15 @@
 if test "x$ac_cv_lib_pthread_pthread_create" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_exit in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_exit in -lpthread" >&5
 printf %s "checking for pthread_exit in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_exit+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26324,15 +26337,15 @@
 if test "x$ac_cv_lib_pthread_pthread_exit" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_join in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_join in -lpthread" >&5
 printf %s "checking for pthread_join in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_join+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26367,15 +26380,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_init in -lpthread" >&5
 printf %s "checking for pthread_cond_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26409,15 +26422,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_destroy in -lpthread" >&5
 printf %s "checking for pthread_cond_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26451,15 +26464,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_broadcast in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_broadcast in -lpthread" >&5
 printf %s "checking for pthread_cond_broadcast in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_broadcast+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26493,15 +26506,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_broadcast" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_signal in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_signal in -lpthread" >&5
 printf %s "checking for pthread_cond_signal in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_signal+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26535,15 +26548,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_signal" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_wait in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_wait in -lpthread" >&5
 printf %s "checking for pthread_cond_wait in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_wait+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26578,15 +26591,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_init in -lpthread" >&5
 printf %s "checking for pthread_mutex_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26620,15 +26633,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_destroy in -lpthread" >&5
 printf %s "checking for pthread_mutex_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26662,15 +26675,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_lock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_lock in -lpthread" >&5
 printf %s "checking for pthread_mutex_lock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_lock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26704,15 +26717,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_lock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_trylock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_trylock in -lpthread" >&5
 printf %s "checking for pthread_mutex_trylock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_trylock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26746,15 +26759,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_trylock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_unlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_unlock in -lpthread" >&5
 printf %s "checking for pthread_mutex_unlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_unlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26789,15 +26802,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_init in -lpthread" >&5
 printf %s "checking for pthread_rwlock_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26831,15 +26844,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_destroy in -lpthread" >&5
 printf %s "checking for pthread_rwlock_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26873,15 +26886,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_rdlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_rdlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_rdlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_rdlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26915,15 +26928,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_rdlock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_wrlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_wrlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_wrlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_wrlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26957,15 +26970,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_wrlock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_unlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_unlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_unlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_unlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -27000,67 +27013,76 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-   ac_cv_pthread_LIBADD="-lpthread";
+        ac_cv_pthread_LIBADD="-lpthread";
+
+fi
+
+    if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes
+then :
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "unable to find supported pthread in directory: $ac_cv_with_pthread
+See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
- if test "x$ac_cv_pthread" = xpthread
+  if test "x$ac_cv_pthread" = xpthread
 then :
 
 printf "%s\n" "#define HAVE_PTHREAD 1" >>confdefs.h
 
 
 fi
 
- if test "x$ac_cv_pthread" != xno
+  if test "x$ac_cv_pthread" != xno
 then :
   HAVE_PTHREAD=1
 
 else $as_nop
   HAVE_PTHREAD=0
 
 
 fi
 
 
- if test "x$ac_cv_pthread_CPPFLAGS" != "x"
+  if test "x$ac_cv_pthread_CPPFLAGS" != "x"
 then :
   PTHREAD_CPPFLAGS=$ac_cv_pthread_CPPFLAGS
 
 
 fi
- if test "x$ac_cv_pthread_LIBADD" != "x"
+  if test "x$ac_cv_pthread_LIBADD" != "x"
 then :
   PTHREAD_LIBADD=$ac_cv_pthread_LIBADD
 
 
 fi
 
- if test "x$ac_cv_pthread" = xpthread
+  if test "x$ac_cv_pthread" = xpthread
 then :
   ax_pthread_pc_libs_private=-lpthread
 
 
 fi
 
       ac_cv_libcthreads_multi_threading=$ac_cv_pthread
 else $as_nop
   ac_cv_libcthreads_multi_threading="winapi"
 fi
 
   if test "x$ac_cv_libcthreads_multi_threading" != xno
 then :
-  ac_cv_libcthreads_CPPFLAGS="-I../libcthreads";
+  ac_cv_libcthreads_CPPFLAGS="-I../libcthreads -I\$(top_srcdir)/libcthreads";
     ac_cv_libcthreads_LIBADD="../libcthreads/libcthreads.la";
 
     ac_cv_libcthreads=local
 else $as_nop
   ac_cv_libcthreads=no
 fi
 
@@ -27148,15 +27170,15 @@
 printf "%s\n" "$ac_cv_with_libcdata" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcdata" = xno
 then :
   ac_cv_libcdata=no
 else $as_nop
   ac_cv_libcdata=check
-        if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect
+                if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes
 then :
   if test -d "$ac_cv_with_libcdata"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcdata}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -30927,15 +30949,16 @@
 fi
 
 
         ac_cv_libcdata_LIBADD="-lcdata"
 fi
 
 fi
-    if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_libcdata" != xyes
+
+    if test "x$ac_cv_libcdata" != xyes && test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcdata in directory: $ac_cv_with_libcdata
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -30960,15 +30983,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcdata" != xyes
 then :
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCDATA 1" >>confdefs.h
@@ -31038,15 +31061,15 @@
 printf "%s\n" "$ac_cv_with_libclocale" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libclocale" = xno
 then :
   ac_cv_libclocale=no
 else $as_nop
   ac_cv_libclocale=check
-        if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect
+                if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes
 then :
   if test -d "$ac_cv_with_libclocale"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libclocale}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libclocale}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -31593,15 +31616,16 @@
 fi
 
 
         ac_cv_libclocale_LIBADD="-lclocale"
 fi
 
 fi
-    if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_libclocale" != xyes
+
+    if test "x$ac_cv_libclocale" != xyes && test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libclocale in directory: $ac_cv_with_libclocale
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -31757,15 +31781,15 @@
 
 printf "%s\n" "#define HAVE_LANGINFO_CODESET 1" >>confdefs.h
 
 
 fi
 
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCLOCALE 1" >>confdefs.h
@@ -31835,15 +31859,15 @@
 printf "%s\n" "$ac_cv_with_libcnotify" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcnotify" = xno
 then :
   ac_cv_libcnotify=no
 else $as_nop
   ac_cv_libcnotify=check
-        if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect
+                if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes
 then :
   if test -d "$ac_cv_with_libcnotify"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcnotify}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcnotify}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -32293,15 +32317,16 @@
 fi
 
 
         ac_cv_libcnotify_LIBADD="-lcnotify"
 fi
 
 fi
-    if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_libcnotify" != xyes
+
+    if test "x$ac_with_libcnotify" != xyes && test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcnotify in directory: $ac_cv_with_libcnotify
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -32356,15 +32381,15 @@
 if test "x$ac_cv_header_errno_h" = xyes
 then :
   printf "%s\n" "#define HAVE_ERRNO_H 1" >>confdefs.h
 
 fi
 
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCNOTIFY 1" >>confdefs.h
@@ -32434,15 +32459,15 @@
 printf "%s\n" "$ac_cv_with_libcsplit" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcsplit" = xno
 then :
   ac_cv_libcsplit=no
 else $as_nop
   ac_cv_libcsplit=check
-        if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect
+                if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes
 then :
   if test -d "$ac_cv_with_libcsplit"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcsplit}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcsplit}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -33157,15 +33182,16 @@
 
 fi
 
         ac_cv_libcsplit_LIBADD="-lcsplit"
 fi
 
 fi
-    if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_libcsplit" != xyes
+
+    if test "x$ac_cv_libcsplit" != xyes && test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcsplit in directory: $ac_cv_with_libcsplit
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -33190,15 +33216,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcsplit" != xyes
 then :
 
-  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit";
+  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit -I\$(top_srcdir)/libcsplit";
   ac_cv_libcsplit_LIBADD="../libcsplit/libcsplit.la";
 
   ac_cv_libcsplit=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCSPLIT 1" >>confdefs.h
@@ -33268,15 +33294,15 @@
 printf "%s\n" "$ac_cv_with_libuna" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libuna" = xno
 then :
   ac_cv_libuna=no
 else $as_nop
   ac_cv_libuna=check
-        if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect
+                if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes
 then :
   if test -d "$ac_cv_with_libuna"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libuna}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libuna}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -40478,15 +40504,16 @@
   ac_cv_libuna=no
 fi
 
         ac_cv_libuna_LIBADD="-luna"
 fi
 
 fi
-    if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_libuna" != xyes
+
+    if test "x$ac_cv_libuna" != xyes && test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libuna in directory: $ac_cv_with_libuna
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -40511,15 +40538,15 @@
 
 fi
 
 
     if test "x$ac_cv_libuna" != xyes
 then :
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBUNA 1" >>confdefs.h
@@ -40589,15 +40616,15 @@
 printf "%s\n" "$ac_cv_with_libcfile" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcfile" = xno
 then :
   ac_cv_libcfile=no
 else $as_nop
   ac_cv_libcfile=check
-        if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect
+                if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes
 then :
   if test -d "$ac_cv_with_libcfile"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcfile}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcfile}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -41778,15 +41805,16 @@
 
 fi
 
         ac_cv_libcfile_LIBADD="-lcfile"
 fi
 
 fi
-    if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_libcfile" != xyes
+
+    if test "x$ac_cv_libcfile" != xyes && test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcfile in directory: $ac_cv_with_libcfile
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -42100,15 +42128,15 @@
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: unlink
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
-  ac_cv_libcfile_CPPFLAGS="-I../libcfile";
+  ac_cv_libcfile_CPPFLAGS="-I../libcfile -I\$(top_srcdir)/libcfile";
   ac_cv_libcfile_LIBADD="../libcfile/libcfile.la";
 
   ac_cv_libcfile=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCFILE 1" >>confdefs.h
@@ -42178,15 +42206,15 @@
 printf "%s\n" "$ac_cv_with_libcpath" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcpath" = xno
 then :
   ac_cv_libcpath=no
 else $as_nop
   ac_cv_libcpath=check
-        if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect
+                if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes
 then :
   if test -d "$ac_cv_with_libcpath"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcpath}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcpath}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -42983,15 +43011,16 @@
 
 fi
 
         ac_cv_libcpath_LIBADD="-lcpath"
 fi
 
 fi
-    if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_libcpath" != xyes
+
+    if test "x$ac_cv_libcpath" != xyes && test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcpath in directory: $ac_cv_with_libcpath
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -43181,15 +43210,15 @@
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: mkdir
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 
-  ac_cv_libcpath_CPPFLAGS="-I../libcpath";
+  ac_cv_libcpath_CPPFLAGS="-I../libcpath -I\$(top_srcdir)/libcpath";
   ac_cv_libcpath_LIBADD="../libcpath/libcpath.la";
 
   ac_cv_libcpath=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCPATH 1" >>confdefs.h
@@ -43259,15 +43288,15 @@
 printf "%s\n" "$ac_cv_with_libbfio" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libbfio" = xno
 then :
   ac_cv_libbfio=no
 else $as_nop
   ac_cv_libbfio=check
-        if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect
+                if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes
 then :
   if test -d "$ac_cv_with_libbfio"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libbfio}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libbfio}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -45377,15 +45406,16 @@
 
 fi
 
         ac_cv_libbfio_LIBADD="-lbfio"
 fi
 
 fi
-    if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_libbfio" != xyes
+
+    if test "x$ac_cv_libbfio" != xyes && test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libbfio in directory: $ac_cv_with_libbfio
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -45410,15 +45440,15 @@
 
 fi
 
 
     if test "x$ac_cv_libbfio" != xyes
 then :
 
-  ac_cv_libbfio_CPPFLAGS="-I../libbfio";
+  ac_cv_libbfio_CPPFLAGS="-I../libbfio -I\$(top_srcdir)/libbfio";
   ac_cv_libbfio_LIBADD="../libbfio/libbfio.la";
 
   ac_cv_libbfio=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBBFIO 1" >>confdefs.h
@@ -45488,15 +45518,15 @@
 printf "%s\n" "$ac_cv_with_libfcache" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfcache" = xno
 then :
   ac_cv_libfcache=no
 else $as_nop
   ac_cv_libfcache=check
-        if test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect
+                if test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes
 then :
   if test -d "$ac_cv_with_libfcache"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfcache}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfcache}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -46408,15 +46438,16 @@
 fi
 
 
         ac_cv_libfcache_LIBADD="-lfcache"
 fi
 
 fi
-    if test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_libfcache" != xyes
+
+    if test "x$ac_cv_libfcache" != xyes && test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfcache in directory: $ac_cv_with_libfcache
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -46509,15 +46540,15 @@
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: time
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
-  ac_cv_libfcache_CPPFLAGS="-I../libfcache";
+  ac_cv_libfcache_CPPFLAGS="-I../libfcache -I\$(top_srcdir)/libfcache";
   ac_cv_libfcache_LIBADD="../libfcache/libfcache.la";
 
   ac_cv_libfcache=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFCACHE 1" >>confdefs.h
@@ -46587,15 +46618,15 @@
 printf "%s\n" "$ac_cv_with_libfdata" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdata" = xno
 then :
   ac_cv_libfdata=no
 else $as_nop
   ac_cv_libfdata=check
-        if test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect
+                if test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes
 then :
   if test -d "$ac_cv_with_libfdata"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdata}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -49875,15 +49906,16 @@
 
 
 
         ac_cv_libfdata_LIBADD="-lfdata"
 fi
 
 fi
-    if test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_libfdata" != xyes
+
+    if test "x$ac_cv_libfdata" != xyes && test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfdata in directory: $ac_cv_with_libfdata
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -49908,15 +49940,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfdata" != xyes
 then :
 
-  ac_cv_libfdata_CPPFLAGS="-I../libfdata";
+  ac_cv_libfdata_CPPFLAGS="-I../libfdata -I\$(top_srcdir)/libfdata";
   ac_cv_libfdata_LIBADD="../libfdata/libfdata.la";
 
   ac_cv_libfdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFDATA 1" >>confdefs.h
@@ -49986,15 +50018,15 @@
 printf "%s\n" "$ac_cv_with_libfguid" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfguid" = xno
 then :
   ac_cv_libfguid=no
 else $as_nop
   ac_cv_libfguid=check
-        if test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect
+                if test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes
 then :
   if test -d "$ac_cv_with_libfguid"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfguid}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfguid}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -50568,15 +50600,16 @@
 fi
 
 
         ac_cv_libfguid_LIBADD="-lfguid"
 fi
 
 fi
-    if test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_libfguid" != xyes
+
+    if test "x$ac_cv_libfguid" != xyes && test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfguid in directory: $ac_cv_with_libfguid
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -50601,15 +50634,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfguid" != xyes
 then :
 
-  ac_cv_libfguid_CPPFLAGS="-I../libfguid";
+  ac_cv_libfguid_CPPFLAGS="-I../libfguid -I\$(top_srcdir)/libfguid";
   ac_cv_libfguid_LIBADD="../libfguid/libfguid.la";
 
   ac_cv_libfguid=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFGUID 1" >>confdefs.h
@@ -50920,16 +50953,20 @@
         PYTHON_LDFLAGS=`${PYTHON_CONFIG} --ldflags 2>/dev/null`;
 
     { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for Python libraries" >&5
 printf %s "checking for Python libraries... " >&6; }
     { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $PYTHON_LDFLAGS" >&5
 printf "%s\n" "$PYTHON_LDFLAGS" >&6; }
 
-        case $host_os in #(
-  cygwin*) :
+        case $build in #(
+  *-*-cygwin*) :
+    PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
+  *-*-mingw*) :
+    PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
+  *-*-msys*) :
     PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
   *) :
      ;; #(
   *) :
      ;;
 esac
 
@@ -51087,33 +51124,107 @@
   printf %s "(cached) " >&6
 else $as_nop
   ac_cv_with_libfuse=auto-detect
 fi
 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_with_libfuse" >&5
 printf "%s\n" "$ac_cv_with_libfuse" >&6; }
 
-      if test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_with_libfuse" != xauto-detect
+    if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfuse" = xno
+then :
+  ac_cv_libfuse=no
+else $as_nop
+              if test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xauto-detect && test "x$ac_cv_with_libfuse" != xyes
 then :
   if test -d "$ac_cv_with_libfuse"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfuse}/include"
-      LDFLAGS="$LDFLAGS -L${ac_cv_with_libfuse}/lib"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_libfuse}/lib"
+else $as_nop
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "no such directory: $ac_cv_with_libfuse
+See \`config.log' for more details" "$LINENO" 5; }
+
+fi
 else $as_nop
-  { printf "%s\n" "$as_me:${as_lineno-$LINENO}: WARNING: no such directory: $ac_cv_with_libfuse" >&5
-printf "%s\n" "$as_me: WARNING: no such directory: $ac_cv_with_libfuse" >&2;}
+        if test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"
+then :
 
+pkg_failed=no
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse3 >= 3.0" >&5
+printf %s "checking for fuse3 >= 3.0... " >&6; }
+
+if test -n "$fuse3_CFLAGS"; then
+    pkg_cv_fuse3_CFLAGS="$fuse3_CFLAGS"
+ elif test -n "$PKG_CONFIG"; then
+    if test -n "$PKG_CONFIG" && \
+    { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$PKG_CONFIG --exists --print-errors \"fuse3 >= 3.0\""; } >&5
+  ($PKG_CONFIG --exists --print-errors "fuse3 >= 3.0") 2>&5
+  ac_status=$?
+  printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$? = $ac_status" >&5
+  test $ac_status = 0; }; then
+  pkg_cv_fuse3_CFLAGS=`$PKG_CONFIG --cflags "fuse3 >= 3.0" 2>/dev/null`
+		      test "x$?" != "x0" && pkg_failed=yes
+else
+  pkg_failed=yes
+fi
+ else
+    pkg_failed=untried
 fi
+if test -n "$fuse3_LIBS"; then
+    pkg_cv_fuse3_LIBS="$fuse3_LIBS"
+ elif test -n "$PKG_CONFIG"; then
+    if test -n "$PKG_CONFIG" && \
+    { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$PKG_CONFIG --exists --print-errors \"fuse3 >= 3.0\""; } >&5
+  ($PKG_CONFIG --exists --print-errors "fuse3 >= 3.0") 2>&5
+  ac_status=$?
+  printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$? = $ac_status" >&5
+  test $ac_status = 0; }; then
+  pkg_cv_fuse3_LIBS=`$PKG_CONFIG --libs "fuse3 >= 3.0" 2>/dev/null`
+		      test "x$?" != "x0" && pkg_failed=yes
+else
+  pkg_failed=yes
+fi
+ else
+    pkg_failed=untried
+fi
+
+
 
+if test $pkg_failed = yes; then
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: no" >&5
+printf "%s\n" "no" >&6; }
+
+if $PKG_CONFIG --atleast-pkgconfig-version 0.20; then
+        _pkg_short_errors_supported=yes
+else
+        _pkg_short_errors_supported=no
 fi
+        if test $_pkg_short_errors_supported = yes; then
+                fuse3_PKG_ERRORS=`$PKG_CONFIG --short-errors --print-errors --cflags --libs "fuse3 >= 3.0" 2>&1`
+        else
+                fuse3_PKG_ERRORS=`$PKG_CONFIG --print-errors --cflags --libs "fuse3 >= 3.0" 2>&1`
+        fi
+        # Put the nasty error message in config.log where it belongs
+        echo "$fuse3_PKG_ERRORS" >&5
 
-  if test "x$ac_cv_with_libfuse" = xno
-then :
-  ac_cv_libfuse=no
-else $as_nop
-      if test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"
+        ac_cv_libfuse=no
+elif test $pkg_failed = untried; then
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: no" >&5
+printf "%s\n" "no" >&6; }
+        ac_cv_libfuse=no
+else
+        fuse3_CFLAGS=$pkg_cv_fuse3_CFLAGS
+        fuse3_LIBS=$pkg_cv_fuse3_LIBS
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: yes" >&5
+printf "%s\n" "yes" >&6; }
+        ac_cv_libfuse=libfuse3
+fi
+
+        if test "x$ac_cv_libfuse" = xno
 then :
 
 pkg_failed=no
 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse >= 2.6" >&5
 printf %s "checking for fuse >= 2.6... " >&6; }
 
 if test -n "$fuse_CFLAGS"; then
@@ -51181,51 +51292,110 @@
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: yes" >&5
 printf "%s\n" "yes" >&6; }
         ac_cv_libfuse=libfuse
 fi
 
 fi
 
-    if test "x$ac_cv_libfuse" = xlibfuse
+        if test "x$ac_cv_libfuse" = xlibfuse3
 then :
-  ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse_CFLAGS"
-      ac_cv_libfuse_LIBADD="$pkg_cv_fuse_LIBS"
-else $as_nop
-               for ac_header in fuse.h
-do :
-  ac_fn_c_check_header_compile "$LINENO" "fuse.h" "ac_cv_header_fuse_h" "$ac_includes_default"
+  ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse3_CFLAGS -D_FILE_OFFSET_BITS=64"
+          ac_cv_libfuse_LIBADD="$pkg_cv_fuse3_LIBS"
+fi
+
+        if test "x$ac_cv_libfuse" = xlibfuse
+then :
+  ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse_CFLAGS -D_FILE_OFFSET_BITS=64"
+          ac_cv_libfuse_LIBADD="$pkg_cv_fuse_LIBS"
+fi
+
+fi
+
+fi
+
+    backup_CPPFLAGS="$CPPFLAGS"
+
+        if test "x$ac_cv_libfuse" != xlibfuse && test "x$ac_cv_libfuse" != xlibfuse3
+then :
+
+      CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=30"
+      ac_fn_c_check_header_compile "$LINENO" "fuse.h" "ac_cv_header_fuse_h" "$ac_includes_default"
 if test "x$ac_cv_header_fuse_h" = xyes
 then :
   printf "%s\n" "#define HAVE_FUSE_H 1" >>confdefs.h
- ac_cv_header_fuse_h=yes
-else $as_nop
-  ac_cv_header_fuse_h=no
+
 fi
 
-done
 
-                  if test "x$ac_cv_header_fuse_h" = xno
+      if test "x$ac_cv_header_fuse_h" = xyes
 then :
-  { ac_cv_header_fuse_h=; unset ac_cv_header_fuse_h;}
-        CPPFLAGS="$CPPFLAGS -D_FILE_OFFSET_BITS=64 -DFUSE_USE_VERSION=26"
+  ac_cv_libfuse=libfuse3
+else $as_nop
+  CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=26"
         ac_fn_c_check_header_compile "$LINENO" "fuse.h" "ac_cv_header_fuse_h" "$ac_includes_default"
 if test "x$ac_cv_header_fuse_h" = xyes
 then :
   printf "%s\n" "#define HAVE_FUSE_H 1" >>confdefs.h
 
 fi
 
 
+        if test "x$ac_cv_header_fuse_h" = xyes
+then :
+  ac_cv_libfuse=libfuse
+fi
+
 fi
 
       if test "x$ac_cv_header_fuse_h" = xno
 then :
   ac_cv_libfuse=no
 else $as_nop
-          ac_cv_libfuse=libfuse
+          { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse_invalidate in -lfuse" >&5
+printf %s "checking for fuse_invalidate in -lfuse... " >&6; }
+if test ${ac_cv_lib_fuse_fuse_invalidate+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-lfuse  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char fuse_invalidate ();
+int
+main (void)
+{
+return fuse_invalidate ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_fuse_fuse_invalidate=yes
+else $as_nop
+  ac_cv_lib_fuse_fuse_invalidate=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_fuse_fuse_invalidate" >&5
+printf "%s\n" "$ac_cv_lib_fuse_fuse_invalidate" >&6; }
+if test "x$ac_cv_lib_fuse_fuse_invalidate" = xyes
+then :
+  ac_cv_libfuse=libfuse
+else $as_nop
+  ac_cv_libfuse=libfuse3
+fi
+
 
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse_daemonize in -lfuse" >&5
 printf %s "checking for fuse_daemonize in -lfuse... " >&6; }
 if test ${ac_cv_lib_fuse_fuse_daemonize+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
@@ -51388,45 +51558,38 @@
 then :
   ac_cv_libfuse_dummy=yes
 else $as_nop
   ac_cv_libfuse=no
 fi
 
 
-        ac_cv_libfuse_LIBADD="-lfuse";
+                ac_cv_libfuse_CPPFLAGS="-D_FILE_OFFSET_BITS=64"
 
+        if test "x$ac_cv_libfuse" = xlibfuse3
+then :
+  ac_cv_libfuse_LIBADD="-lfuse3"
+else $as_nop
+  ac_cv_libfuse_LIBADD="-lfuse"
 fi
 
 fi
 
-        if test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_header_fuse_h" = xno
-then :
-  CPPFLAGS="$CPPFLAGS -DFUSE_USE_VERSION=26"
-      ac_fn_c_check_header_compile "$LINENO" "osxfuse/fuse.h" "ac_cv_header_osxfuse_fuse_h" "$ac_includes_default"
-if test "x$ac_cv_header_osxfuse_fuse_h" = xyes
-then :
-  printf "%s\n" "#define HAVE_OSXFUSE_FUSE_H 1" >>confdefs.h
-
 fi
 
-
-            if test "x$ac_cv_header_osxfuse_fuse_h" = xno
+        if test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_header_fuse_h" = xno
 then :
-  { ac_cv_header_osxfuse_fuse_h=; unset ac_cv_header_osxfuse_fuse_h;}
-        CPPFLAGS="$CPPFLAGS -D_FILE_OFFSET_BITS=64"
-        ac_fn_c_check_header_compile "$LINENO" "osxfuse/fuse.h" "ac_cv_header_osxfuse_fuse_h" "$ac_includes_default"
+  CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=26"
+      ac_fn_c_check_header_compile "$LINENO" "osxfuse/fuse.h" "ac_cv_header_osxfuse_fuse_h" "$ac_includes_default"
 if test "x$ac_cv_header_osxfuse_fuse_h" = xyes
 then :
   printf "%s\n" "#define HAVE_OSXFUSE_FUSE_H 1" >>confdefs.h
 
 fi
 
 
-fi
-
       if test "x$ac_cv_header_osxfuse_fuse_h" = xno
 then :
   ac_cv_libfuse=no
 else $as_nop
           ac_cv_libfuse=libosxfuse
 
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse_daemonize in -losxfuse" >&5
@@ -51594,29 +51757,49 @@
 then :
   ac_cv_libfuse_dummy=yes
 else $as_nop
   ac_cv_libfuse=no
 fi
 
 
+                ac_cv_libfuse_CPPFLAGS="-D_FILE_OFFSET_BITS=64"
+
         ac_cv_libfuse_LIBADD="-losxfuse";
 
 fi
 
 fi
 
+    if test "x$ac_cv_libfuse" != xyes && test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xauto-detect && test "x$ac_cv_with_libfuse" != xyes
+then :
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "unable to find supported libfuse in directory: $ac_cv_with_libfuse
+See \`config.log' for more details" "$LINENO" 5; }
+
+fi
+
+    CPPFLAGS="$backup_CPPFLAGS"
+
 fi
 
   if test "x$ac_cv_libfuse" = xlibfuse
 then :
 
 printf "%s\n" "#define HAVE_LIBFUSE 1" >>confdefs.h
 
 
 fi
+  if test "x$ac_cv_libfuse" = xlibfuse3
+then :
+
+printf "%s\n" "#define HAVE_LIBFUSE3 1" >>confdefs.h
+
+
+fi
   if test "x$ac_cv_libfuse" = xlibosxfuse
 then :
 
 printf "%s\n" "#define HAVE_LIBOSXFUSE 1" >>confdefs.h
 
 
 fi
@@ -51647,14 +51830,20 @@
 
   if test "x$ac_cv_libfuse" = xlibfuse
 then :
   ax_libfuse_pc_libs_private=-lfuse
 
 
 fi
+  if test "x$ac_cv_libfuse" = xlibfuse3
+then :
+  ax_libfuse_pc_libs_private=-lfuse3
+
+
+fi
   if test "x$ac_cv_libfuse" = xlibosxfuse
 then :
   ax_libfuse_pc_libs_private=-losxfuse
 
 
 fi
 
@@ -51662,14 +51851,22 @@
 then :
   ax_libfuse_spec_requires=fuse-libs
 
     ax_libfuse_spec_build_requires=fuse-devel
 
 
 fi
+  if test "x$ac_cv_libfuse" = xlibfuse3
+then :
+  ax_libfuse_spec_requires=fuse3-libs
+
+    ax_libfuse_spec_build_requires=fuse3-devel
+
+
+fi
 
 
 ac_fn_c_check_header_compile "$LINENO" "signal.h" "ac_cv_header_signal_h" "$ac_includes_default"
 if test "x$ac_cv_header_signal_h" = xyes
 then :
   printf "%s\n" "#define HAVE_SIGNAL_H 1" >>confdefs.h
 
@@ -52583,15 +52780,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by libvhdi $as_me 20240303, which was
+This file was extended by libvhdi $as_me 20240509, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -52651,15 +52848,15 @@
 
 _ACEOF
 ac_cs_config=`printf "%s\n" "$ac_configure_args" | sed "$ac_safe_unquote"`
 ac_cs_config_escaped=`printf "%s\n" "$ac_cs_config" | sed "s/^ //; s/'/'\\\\\\\\''/g"`
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config='$ac_cs_config_escaped'
 ac_cs_version="\\
-libvhdi config.status 20240303
+libvhdi config.status 20240509
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `libvhdi-20240303/compile` & `libvhdi-20240509/compile`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/missing` & `libvhdi-20240509/missing`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/libfdata/libfdata.vcproj` & `libvhdi-20240509/msvscpp/libfdata/libfdata.vcproj`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/vhdi_test_dynamic_disk_header/vhdi_test_dynamic_disk_header.vcproj` & `libvhdi-20240509/msvscpp/vhdi_test_dynamic_disk_header/vhdi_test_dynamic_disk_header.vcproj`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/vhdi_test_tools_info_handle/vhdi_test_tools_info_handle.vcproj` & `libvhdi-20240509/msvscpp/vhdi_test_tools_info_handle/vhdi_test_tools_info_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/vhdi_test_region_table_entry/vhdi_test_region_table_entry.vcproj` & `libvhdi-20240509/msvscpp/vhdi_test_region_table_entry/vhdi_test_region_table_entry.vcproj`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/vhdi_test_region_table/vhdi_test_region_table.vcproj` & `libvhdi-20240509/msvscpp/vhdi_test_region_table/vhdi_test_region_table.vcproj`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/vhdi_test_io_handle/vhdi_test_io_handle.vcproj` & `libvhdi-20240509/msvscpp/vhdi_test_io_handle/vhdi_test_io_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/vhdi_test_block_allocation_table/vhdi_test_block_allocation_table.vcproj` & `libvhdi-20240509/msvscpp/vhdi_test_block_allocation_table/vhdi_test_block_allocation_table.vcproj`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/vhdi_test_parent_locator_entry/vhdi_test_parent_locator_entry.vcproj` & `libvhdi-20240509/msvscpp/vhdi_test_parent_locator_entry/vhdi_test_parent_locator_entry.vcproj`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/vhdi_test_support/vhdi_test_support.vcproj` & `libvhdi-20240509/msvscpp/vhdi_test_support/vhdi_test_support.vcproj`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/vhdi_test_parent_locator_header/vhdi_test_parent_locator_header.vcproj` & `libvhdi-20240509/msvscpp/vhdi_test_parent_locator_header/vhdi_test_parent_locator_header.vcproj`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/vhdi_test_metadata_table_entry/vhdi_test_metadata_table_entry.vcproj` & `libvhdi-20240509/msvscpp/vhdi_test_metadata_table_entry/vhdi_test_metadata_table_entry.vcproj`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/libfguid/libfguid.vcproj` & `libvhdi-20240509/msvscpp/libfguid/libfguid.vcproj`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/vhdi_test_tools_output/vhdi_test_tools_output.vcproj` & `libvhdi-20240509/msvscpp/vhdi_test_tools_output/vhdi_test_tools_output.vcproj`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/vhdi_test_image_header/vhdi_test_image_header.vcproj` & `libvhdi-20240509/msvscpp/vhdi_test_image_header/vhdi_test_image_header.vcproj`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/vhdi_test_error/vhdi_test_error.vcproj` & `libvhdi-20240509/msvscpp/vhdi_test_error/vhdi_test_error.vcproj`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/libclocale/libclocale.vcproj` & `libvhdi-20240509/msvscpp/libclocale/libclocale.vcproj`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/libfcache/libfcache.vcproj` & `libvhdi-20240509/msvscpp/libfcache/libfcache.vcproj`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/vhdi_test_tools_signal/vhdi_test_tools_signal.vcproj` & `libvhdi-20240509/msvscpp/vhdi_test_tools_signal/vhdi_test_tools_signal.vcproj`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/Makefile.am` & `libvhdi-20240509/msvscpp/Makefile.am`

 * *Files 2% similar despite different names*

```diff
@@ -43,13 +43,11 @@
 	vhdiinfo/vhdiinfo.vcproj \
 	vhdimount/vhdimount.vcproj \
 	libvhdi.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libvhdi-20240303/msvscpp/libbfio/libbfio.vcproj` & `libvhdi-20240509/msvscpp/libbfio/libbfio.vcproj`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/vhdi_test_sector_range_descriptor/vhdi_test_sector_range_descriptor.vcproj` & `libvhdi-20240509/msvscpp/vhdi_test_sector_range_descriptor/vhdi_test_sector_range_descriptor.vcproj`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/vhdi_test_parent_locator/vhdi_test_parent_locator.vcproj` & `libvhdi-20240509/msvscpp/vhdi_test_parent_locator/vhdi_test_parent_locator.vcproj`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/vhdi_test_block_descriptor/vhdi_test_block_descriptor.vcproj` & `libvhdi-20240509/msvscpp/vhdi_test_block_descriptor/vhdi_test_block_descriptor.vcproj`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/libcfile/libcfile.vcproj` & `libvhdi-20240509/msvscpp/libcfile/libcfile.vcproj`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/pyvhdi/pyvhdi.vcproj` & `libvhdi-20240509/msvscpp/pyvhdi/pyvhdi.vcproj`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/vhdi_test_file_footer/vhdi_test_file_footer.vcproj` & `libvhdi-20240509/msvscpp/vhdi_test_file_footer/vhdi_test_file_footer.vcproj`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/libcdata/libcdata.vcproj` & `libvhdi-20240509/msvscpp/libcdata/libcdata.vcproj`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/vhdi_test_metadata_values/vhdi_test_metadata_values.vcproj` & `libvhdi-20240509/msvscpp/vhdi_test_metadata_values/vhdi_test_metadata_values.vcproj`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/vhdimount/vhdimount.vcproj` & `libvhdi-20240509/msvscpp/vhdimount/vhdimount.vcproj`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/vhdi_test_region_table_header/vhdi_test_region_table_header.vcproj` & `libvhdi-20240509/msvscpp/vhdi_test_region_table_header/vhdi_test_region_table_header.vcproj`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/vhdiinfo/vhdiinfo.vcproj` & `libvhdi-20240509/msvscpp/vhdiinfo/vhdiinfo.vcproj`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/libcthreads/libcthreads.vcproj` & `libvhdi-20240509/msvscpp/libcthreads/libcthreads.vcproj`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/libcpath/libcpath.vcproj` & `libvhdi-20240509/msvscpp/libcpath/libcpath.vcproj`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/vhdi_test_file/vhdi_test_file.vcproj` & `libvhdi-20240509/msvscpp/vhdi_test_file/vhdi_test_file.vcproj`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/vhdi_test_metadata_table/vhdi_test_metadata_table.vcproj` & `libvhdi-20240509/msvscpp/vhdi_test_metadata_table/vhdi_test_metadata_table.vcproj`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/vhdi_test_metadata_table_header/vhdi_test_metadata_table_header.vcproj` & `libvhdi-20240509/msvscpp/vhdi_test_metadata_table_header/vhdi_test_metadata_table_header.vcproj`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/vhdi_test_file_information/vhdi_test_file_information.vcproj` & `libvhdi-20240509/msvscpp/vhdi_test_file_information/vhdi_test_file_information.vcproj`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/libvhdi.sln` & `libvhdi-20240509/msvscpp/libvhdi.sln`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/libcsplit/libcsplit.vcproj` & `libvhdi-20240509/msvscpp/libcsplit/libcsplit.vcproj`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/libvhdi/libvhdi.vcproj` & `libvhdi-20240509/msvscpp/libvhdi/libvhdi.vcproj`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/libuna/libuna.vcproj` & `libvhdi-20240509/msvscpp/libuna/libuna.vcproj`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/Makefile.in` & `libvhdi-20240509/msvscpp/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -381,14 +381,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -491,15 +493,16 @@
 	vhdiinfo/vhdiinfo.vcproj \
 	vhdimount/vhdimount.vcproj \
 	libvhdi.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -603,23 +606,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -698,13 +703,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libvhdi-20240303/msvscpp/libcnotify/libcnotify.vcproj` & `libvhdi-20240509/msvscpp/libcnotify/libcnotify.vcproj`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/vhdi_test_checksum/vhdi_test_checksum.vcproj` & `libvhdi-20240509/msvscpp/vhdi_test_checksum/vhdi_test_checksum.vcproj`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/libcerror/libcerror.vcproj` & `libvhdi-20240509/msvscpp/libcerror/libcerror.vcproj`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/msvscpp/vhdi_test_notify/vhdi_test_notify.vcproj` & `libvhdi-20240509/msvscpp/vhdi_test_notify/vhdi_test_notify.vcproj`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcfile/libcfile_extern.h` & `libvhdi-20240509/libcfile/libcfile_extern.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcfile/libcfile_support.h` & `libvhdi-20240509/libcfile/libcfile_support.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcfile/libcfile_unused.h` & `libvhdi-20240509/libcfile/libcfile_unused.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcfile/libcfile_notify.h` & `libvhdi-20240509/libcfile/libcfile_notify.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcfile/libcfile_support.c` & `libvhdi-20240509/libcfile/libcfile_support.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcfile/libcfile_types.h` & `libvhdi-20240509/libcfile/libcfile_types.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcfile/Makefile.am` & `libvhdi-20240509/libcfile/Makefile.am`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCFILE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcfile.la
 
@@ -22,19 +22,17 @@
 	libcfile_support.c libcfile_support.h \
 	libcfile_system_string.c libcfile_system_string.h \
 	libcfile_types.h \
 	libcfile_unused.h \
 	libcfile_winapi.c libcfile_winapi.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcfile ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcfile_la_SOURCES)
```

### Comparing `libvhdi-20240303/libcfile/libcfile_notify.c` & `libvhdi-20240509/libcfile/libcfile_notify.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcfile/libcfile_system_string.h` & `libvhdi-20240509/libcfile/libcfile_system_string.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcfile/libcfile_file.h` & `libvhdi-20240509/libcfile/libcfile_file.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcfile/libcfile_libcnotify.h` & `libvhdi-20240509/libcfile/libcfile_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcfile/libcfile_system_string.c` & `libvhdi-20240509/libcfile/libcfile_system_string.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcfile/libcfile_error.h` & `libvhdi-20240509/libcfile/libcfile_error.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcfile/libcfile_libcerror.h` & `libvhdi-20240509/libcfile/libcfile_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcfile/libcfile_file.c` & `libvhdi-20240509/libcfile/libcfile_file.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcfile/libcfile_libclocale.h` & `libvhdi-20240509/libcfile/libcfile_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcfile/libcfile_winapi.h` & `libvhdi-20240509/libcfile/libcfile_winapi.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcfile/Makefile.in` & `libvhdi-20240509/libcfile/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -446,14 +446,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -508,16 +510,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCFILE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCFILE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCFILE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCFILE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCFILE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBUNA_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCFILE_TRUE@noinst_LTLIBRARIES = libcfile.la
 @HAVE_LOCAL_LIBCFILE_TRUE@libcfile_la_SOURCES = \
@@ -532,15 +534,16 @@
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_notify.c libcfile_notify.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_support.c libcfile_support.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_system_string.c libcfile_system_string.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_types.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_unused.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_winapi.c libcfile_winapi.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -745,24 +748,32 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcfile_error.Plo
+	-rm -f ./$(DEPDIR)/libcfile_file.Plo
+	-rm -f ./$(DEPDIR)/libcfile_notify.Plo
+	-rm -f ./$(DEPDIR)/libcfile_support.Plo
+	-rm -f ./$(DEPDIR)/libcfile_system_string.Plo
+	-rm -f ./$(DEPDIR)/libcfile_winapi.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -851,17 +862,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcfile ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcfile_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvhdi-20240303/libcfile/libcfile_error.c` & `libvhdi-20240509/libcfile/libcfile_error.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcfile/libcfile_libuna.h` & `libvhdi-20240509/libcfile/libcfile_libuna.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcfile/libcfile_winapi.c` & `libvhdi-20240509/libcfile/libcfile_winapi.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcfile/libcfile_definitions.h` & `libvhdi-20240509/libcfile/libcfile_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcfile/definitions.h>
 
 /* The definitions in <libcfile/definitions.h> are copied here
  * for local use of libcfile
  */
 #else
 
-#define LIBCFILE_VERSION				20240106
+#define LIBCFILE_VERSION				20240414
 
 /* The libcfile version string
  */
-#define LIBCFILE_VERSION_STRING				"20240106"
+#define LIBCFILE_VERSION_STRING				"20240414"
 
 /* The file access flags
  * bit 1	set to 1 for read access
  * bit 2	set to 1 for write access
  * bit 3	set to 1 to truncate an existing file on write
  * bit 4-8	not used
  */
```

### Comparing `libvhdi-20240303/README` & `libvhdi-20240509/README`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/pyvhdi/pyvhdi_libcerror.h` & `libvhdi-20240509/pyvhdi/pyvhdi_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/pyvhdi/pyvhdi_libbfio.h` & `libvhdi-20240509/pyvhdi/pyvhdi_libbfio.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/pyvhdi/pyvhdi_disk_types.h` & `libvhdi-20240509/pyvhdi/pyvhdi_disk_types.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/pyvhdi/pyvhdi_file_object_io_handle.c` & `libvhdi-20240509/pyvhdi/pyvhdi_file_object_io_handle.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/pyvhdi/Makefile.am` & `libvhdi-20240509/pyvhdi/Makefile.am`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_PYTHON
 AM_CFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
 	@LIBCPATH_CPPFLAGS@ \
@@ -44,13 +44,11 @@
 	@LIBFGUID_LIBADD@
 
 pyvhdi_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 pyvhdi_la_LDFLAGS  = -module -avoid-version $(PYTHON_LDFLAGS)
 
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libvhdi-20240303/pyvhdi/pyvhdi.c` & `libvhdi-20240509/pyvhdi/pyvhdi.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/pyvhdi/pyvhdi_error.h` & `libvhdi-20240509/pyvhdi/pyvhdi_error.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/pyvhdi/pyvhdi_libclocale.h` & `libvhdi-20240509/pyvhdi/pyvhdi_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/pyvhdi/pyvhdi_python.h` & `libvhdi-20240509/pyvhdi/pyvhdi_python.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/pyvhdi/pyvhdi_integer.c` & `libvhdi-20240509/pyvhdi/pyvhdi_integer.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/pyvhdi/pyvhdi_file.c` & `libvhdi-20240509/pyvhdi/pyvhdi_file.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/pyvhdi/pyvhdi.h` & `libvhdi-20240509/pyvhdi/pyvhdi.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/pyvhdi/pyvhdi_integer.h` & `libvhdi-20240509/pyvhdi/pyvhdi_integer.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/pyvhdi/pyvhdi_libvhdi.h` & `libvhdi-20240509/pyvhdi/pyvhdi_libvhdi.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/pyvhdi/pyvhdi_error.c` & `libvhdi-20240509/pyvhdi/pyvhdi_error.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/pyvhdi/pyvhdi_disk_types.c` & `libvhdi-20240509/pyvhdi/pyvhdi_disk_types.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/pyvhdi/pyvhdi_guid.c` & `libvhdi-20240509/pyvhdi/pyvhdi_guid.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/pyvhdi/Makefile.in` & `libvhdi-20240509/pyvhdi/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -480,14 +480,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -542,16 +544,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_PYTHON_TRUE@AM_CFLAGS = \
-@HAVE_PYTHON_TRUE@	-I$(top_srcdir)/include \
-@HAVE_PYTHON_TRUE@	-I$(top_srcdir)/common \
+@HAVE_PYTHON_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_PYTHON_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_PYTHON_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCFILE_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCPATH_CPPFLAGS@ \
@@ -586,15 +588,16 @@
 @HAVE_PYTHON_TRUE@	@LIBCFILE_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBCPATH_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBBFIO_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBFGUID_LIBADD@
 
 @HAVE_PYTHON_TRUE@pyvhdi_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 @HAVE_PYTHON_TRUE@pyvhdi_la_LDFLAGS = -module -avoid-version $(PYTHON_LDFLAGS)
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -876,24 +879,33 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-pyexecLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/pyvhdi_la-pyvhdi.Plo
+	-rm -f ./$(DEPDIR)/pyvhdi_la-pyvhdi_disk_types.Plo
+	-rm -f ./$(DEPDIR)/pyvhdi_la-pyvhdi_error.Plo
+	-rm -f ./$(DEPDIR)/pyvhdi_la-pyvhdi_file.Plo
+	-rm -f ./$(DEPDIR)/pyvhdi_la-pyvhdi_file_object_io_handle.Plo
+	-rm -f ./$(DEPDIR)/pyvhdi_la-pyvhdi_guid.Plo
+	-rm -f ./$(DEPDIR)/pyvhdi_la-pyvhdi_integer.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -984,13 +996,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-pyexecLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libvhdi-20240303/pyvhdi/pyvhdi_libfguid.h` & `libvhdi-20240509/pyvhdi/pyvhdi_libfguid.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/pyvhdi/pyvhdi_file_object_io_handle.h` & `libvhdi-20240509/pyvhdi/pyvhdi_file_object_io_handle.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/pyvhdi/pyvhdi_unused.h` & `libvhdi-20240509/pyvhdi/pyvhdi_unused.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/pyvhdi/pyvhdi_guid.h` & `libvhdi-20240509/pyvhdi/pyvhdi_guid.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/pyvhdi/pyvhdi_file.h` & `libvhdi-20240509/pyvhdi/pyvhdi_file.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/INSTALL` & `libvhdi-20240509/INSTALL`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcdata/libcdata_list_element.h` & `libvhdi-20240509/libcdata/libcdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcdata/libcdata_array.h` & `libvhdi-20240509/libcdata/libcdata_array.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcdata/libcdata_definitions.h` & `libvhdi-20240509/libcdata/libcdata_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcdata/definitions.h>
 
 /* The definitions in <libcdata/definitions.h> are copied here
  * for local use of libcdata
  */
 #else
 
-#define LIBCDATA_VERSION				20240103
+#define LIBCDATA_VERSION				20240414
 
 /* The libcdata version string
  */
-#define LIBCDATA_VERSION_STRING				"20240103"
+#define LIBCDATA_VERSION_STRING				"20240414"
 
 /* The comparison function definitions
  */
 enum LIBCDATA_COMPARE_DEFINITIONS
 {
 	/* The first value is less than the second value
 	 */
```

### Comparing `libvhdi-20240303/libcdata/libcdata_libcerror.h` & `libvhdi-20240509/libcdata/libcdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcdata/libcdata_unused.h` & `libvhdi-20240509/libcdata/libcdata_unused.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcdata/libcdata_btree.h` & `libvhdi-20240509/libcdata/libcdata_btree.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcdata/libcdata_btree.c` & `libvhdi-20240509/libcdata/libcdata_btree.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcdata/libcdata_support.c` & `libvhdi-20240509/libcdata/libcdata_support.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcdata/libcdata_list.c` & `libvhdi-20240509/libcdata/libcdata_list.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcdata/libcdata_extern.h` & `libvhdi-20240509/libcdata/libcdata_extern.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcdata/libcdata_list.h` & `libvhdi-20240509/libcdata/libcdata_list.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcdata/libcdata_btree_values_list.h` & `libvhdi-20240509/libcdata/libcdata_btree_values_list.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcdata/Makefile.am` & `libvhdi-20240509/libcdata/Makefile.am`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCDATA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcdata.la
 
 libcdata_la_SOURCES = \
@@ -24,19 +24,17 @@
 	libcdata_range_list_value.c libcdata_range_list_value.h \
 	libcdata_support.c libcdata_support.h \
 	libcdata_tree_node.c libcdata_tree_node.h \
 	libcdata_types.h \
 	libcdata_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcdata_la_SOURCES)
```

### Comparing `libvhdi-20240303/libcdata/libcdata_btree_node.h` & `libvhdi-20240509/libcdata/libcdata_btree_node.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcdata/libcdata_range_list_value.h` & `libvhdi-20240509/libcdata/libcdata_range_list_value.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcdata/libcdata_range_list.h` & `libvhdi-20240509/libcdata/libcdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcdata/libcdata_range_list.c` & `libvhdi-20240509/libcdata/libcdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcdata/libcdata_array.c` & `libvhdi-20240509/libcdata/libcdata_array.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcdata/libcdata_list_element.c` & `libvhdi-20240509/libcdata/libcdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcdata/libcdata_libcthreads.h` & `libvhdi-20240509/libcdata/libcdata_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcdata/libcdata_tree_node.h` & `libvhdi-20240509/libcdata/libcdata_tree_node.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcdata/libcdata_error.h` & `libvhdi-20240509/libcdata/libcdata_error.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcdata/libcdata_types.h` & `libvhdi-20240509/libcdata/libcdata_types.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcdata/libcdata_btree_node.c` & `libvhdi-20240509/libcdata/libcdata_btree_node.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcdata/libcdata_tree_node.c` & `libvhdi-20240509/libcdata/libcdata_tree_node.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcdata/libcdata_support.h` & `libvhdi-20240509/libcdata/libcdata_support.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcdata/Makefile.in` & `libvhdi-20240509/libcdata/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -460,14 +460,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -522,16 +524,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCDATA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCDATA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCDATA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCDATA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCDATA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCDATA_TRUE@noinst_LTLIBRARIES = libcdata.la
 @HAVE_LOCAL_LIBCDATA_TRUE@libcdata_la_SOURCES = \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_array.c libcdata_array.h \
@@ -548,15 +550,16 @@
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_range_list.c libcdata_range_list.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_range_list_value.c libcdata_range_list_value.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_support.c libcdata_support.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_tree_node.c libcdata_tree_node.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_types.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -766,24 +769,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcdata_array.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree_node.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree_values_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_error.Plo
+	-rm -f ./$(DEPDIR)/libcdata_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_list_element.Plo
+	-rm -f ./$(DEPDIR)/libcdata_range_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_range_list_value.Plo
+	-rm -f ./$(DEPDIR)/libcdata_support.Plo
+	-rm -f ./$(DEPDIR)/libcdata_tree_node.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -877,17 +893,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcdata_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvhdi-20240303/libcdata/libcdata_range_list_value.c` & `libvhdi-20240509/libcdata/libcdata_range_list_value.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcdata/libcdata_btree_values_list.c` & `libvhdi-20240509/libcdata/libcdata_btree_values_list.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcdata/libcdata_error.c` & `libvhdi-20240509/libcdata/libcdata_error.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/config.sub` & `libvhdi-20240509/config.sub`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/setup.py` & `libvhdi-20240509/setup.py`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/acinclude.m4` & `libvhdi-20240509/acinclude.m4`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/config.rpath` & `libvhdi-20240509/config.rpath`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcthreads/libcthreads_thread.h` & `libvhdi-20240509/libcthreads/libcthreads_thread.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcthreads/libcthreads_read_write_lock.h` & `libvhdi-20240509/libcthreads/libcthreads_read_write_lock.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcthreads/libcthreads_thread.c` & `libvhdi-20240509/libcthreads/libcthreads_thread.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcthreads/libcthreads_thread_pool.h` & `libvhdi-20240509/libcthreads/libcthreads_thread_pool.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcthreads/libcthreads_support.h` & `libvhdi-20240509/libcthreads/libcthreads_support.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcthreads/libcthreads_lock.h` & `libvhdi-20240509/libcthreads/libcthreads_lock.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcthreads/libcthreads_unused.h` & `libvhdi-20240509/libcthreads/libcthreads_unused.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcthreads/libcthreads_lock.c` & `libvhdi-20240509/libcthreads/libcthreads_lock.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcthreads/libcthreads_condition.h` & `libvhdi-20240509/libcthreads/libcthreads_condition.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcthreads/libcthreads_repeating_thread.h` & `libvhdi-20240509/libcthreads/libcthreads_repeating_thread.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcthreads/Makefile.am` & `libvhdi-20240509/libcthreads/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCTHREADS
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcthreads.la
 
 libcthreads_la_SOURCES = \
 	libcthreads_condition.c libcthreads_condition.h \
@@ -22,19 +22,17 @@
 	libcthreads_thread.c libcthreads_thread.h \
 	libcthreads_thread_attributes.c libcthreads_thread_attributes.h \
 	libcthreads_thread_pool.c libcthreads_thread_pool.h \
 	libcthreads_types.h \
 	libcthreads_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcthreads ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcthreads_la_SOURCES)
```

### Comparing `libvhdi-20240303/libcthreads/libcthreads_support.c` & `libvhdi-20240509/libcthreads/libcthreads_support.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcthreads/libcthreads_mutex.c` & `libvhdi-20240509/libcthreads/libcthreads_mutex.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcthreads/libcthreads_queue.c` & `libvhdi-20240509/libcthreads/libcthreads_queue.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcthreads/libcthreads_mutex.h` & `libvhdi-20240509/libcthreads/libcthreads_mutex.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcthreads/libcthreads_types.h` & `libvhdi-20240509/libcthreads/libcthreads_types.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcthreads/libcthreads_thread_attributes.h` & `libvhdi-20240509/libcthreads/libcthreads_thread_attributes.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcthreads/libcthreads_condition.c` & `libvhdi-20240509/libcthreads/libcthreads_condition.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcthreads/libcthreads_error.c` & `libvhdi-20240509/libcthreads/libcthreads_error.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcthreads/libcthreads_read_write_lock.c` & `libvhdi-20240509/libcthreads/libcthreads_read_write_lock.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcthreads/libcthreads_libcerror.h` & `libvhdi-20240509/libcthreads/libcthreads_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcthreads/libcthreads_definitions.h` & `libvhdi-20240509/libcthreads/libcthreads_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcthreads/definitions.h>
 
 /* The definitions in <libcthreads/definitions.h> are copied here
  * for local use of libcthreads
  */
 #else
 
-#define LIBCTHREADS_VERSION				20240102
+#define LIBCTHREADS_VERSION				20240413
 
 /* The libcthreads version string
  */
-#define LIBCTHREADS_VERSION_STRING			"20240102"
+#define LIBCTHREADS_VERSION_STRING			"20240413"
 
 /* The comparison function definitions
  */
 enum LIBCTHREADS_COMPARE_DEFINITIONS
 {
 	/* The first value is less than the second value
 	 */
```

### Comparing `libvhdi-20240303/libcthreads/libcthreads_thread_pool.c` & `libvhdi-20240509/libcthreads/libcthreads_thread_pool.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcthreads/libcthreads_error.h` & `libvhdi-20240509/libcthreads/libcthreads_error.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcthreads/libcthreads_thread_attributes.c` & `libvhdi-20240509/libcthreads/libcthreads_thread_attributes.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcthreads/libcthreads_extern.h` & `libvhdi-20240509/libcthreads/libcthreads_extern.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcthreads/libcthreads_repeating_thread.c` & `libvhdi-20240509/libcthreads/libcthreads_repeating_thread.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcthreads/Makefile.in` & `libvhdi-20240509/libcthreads/Makefile.in`

 * *Files 5% similar despite different names*

```diff
@@ -464,14 +464,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -526,16 +528,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCTHREADS_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCTHREADS_TRUE@noinst_LTLIBRARIES = libcthreads.la
 @HAVE_LOCAL_LIBCTHREADS_TRUE@libcthreads_la_SOURCES = \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_condition.c libcthreads_condition.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_definitions.h \
@@ -550,15 +552,16 @@
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_support.c libcthreads_support.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread.c libcthreads_thread.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread_attributes.c libcthreads_thread_attributes.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread_pool.c libcthreads_thread_pool.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_types.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -768,24 +771,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcthreads_condition.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_error.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_lock.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_mutex.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_queue.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_read_write_lock.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_repeating_thread.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_support.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread_attributes.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread_pool.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -879,17 +895,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcthreads ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcthreads_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvhdi-20240303/libcthreads/libcthreads_queue.h` & `libvhdi-20240509/libcthreads/libcthreads_queue.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi.spec` & `libvhdi-20240509/libvhdi.spec`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name: libvhdi
-Version: 20240303
+Version: 20240509
 Release: 1
 Summary: Library to access the Virtual Hard Disk (VHD) image format
 Group: System Environment/Libraries
 License: LGPL-3.0-or-later
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/libvhdi
              
@@ -36,16 +36,16 @@
 
 %description -n libvhdi-python3
 Python 3 bindings for libvhdi
 
 %package -n libvhdi-tools
 Summary: Several tools for reading Virtual Hard Disk (VHD) image files
 Group: Applications/System
-Requires: libvhdi = %{version}-%{release} fuse-libs
-BuildRequires: fuse-devel
+Requires: libvhdi = %{version}-%{release} fuse3-libs
+BuildRequires: fuse3-devel
 
 %description -n libvhdi-tools
 Several tools for reading Virtual Hard Disk (VHD) image files
 
 %prep
 %setup -q
 
@@ -91,10 +91,10 @@
 %files -n libvhdi-tools
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_bindir}/*
 %{_mandir}/man1/*
 
 %changelog
-* Sun Mar  3 2024 Joachim Metz <joachim.metz@gmail.com> 20240303-1
+* Thu May  9 2024 Joachim Metz <joachim.metz@gmail.com> 20240509-1
 - Auto-generated
```

### Comparing `libvhdi-20240303/test-driver` & `libvhdi-20240509/test-driver`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcpath/libcpath_support.c` & `libvhdi-20240509/libcpath/libcpath_support.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcpath/libcpath_libcerror.h` & `libvhdi-20240509/libcpath/libcpath_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcpath/libcpath_definitions.h` & `libvhdi-20240509/libcpath/libcpath_definitions.h`

 * *Files 4% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcpath/definitions.h>
 
 /* The definitions in <libcpath/definitions.h> are copied here
  * for local use of libcpath
  */
 #else
 
-#define LIBCPATH_VERSION			20240109
+#define LIBCPATH_VERSION			20240414
 
 /* The libcpath version string
  */
-#define LIBCPATH_VERSION_STRING			"20240109"
+#define LIBCPATH_VERSION_STRING			"20240414"
 
 #if defined( WINAPI )
 #define LIBCPATH_SEPARATOR			'\\'
 
 #else
 #define LIBCPATH_SEPARATOR			'/'
```

### Comparing `libvhdi-20240303/libcpath/Makefile.am` & `libvhdi-20240509/libcpath/Makefile.am`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCPATH
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcpath.la
 
@@ -19,19 +19,17 @@
 	libcpath_libcsplit.h \
 	libcpath_libuna.h \
 	libcpath_support.c libcpath_support.h \
 	libcpath_system_string.c libcpath_system_string.h \
 	libcpath_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcpath ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcpath_la_SOURCES)
```

### Comparing `libvhdi-20240303/libcpath/libcpath_error.c` & `libvhdi-20240509/libcpath/libcpath_error.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcpath/libcpath_extern.h` & `libvhdi-20240509/libcpath/libcpath_extern.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcpath/libcpath_system_string.h` & `libvhdi-20240509/libcpath/libcpath_system_string.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcpath/libcpath_support.h` & `libvhdi-20240509/libcpath/libcpath_support.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcpath/libcpath_libcsplit.h` & `libvhdi-20240509/libcpath/libcpath_libcsplit.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcpath/libcpath_system_string.c` & `libvhdi-20240509/libcpath/libcpath_system_string.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcpath/libcpath_libclocale.h` & `libvhdi-20240509/libcpath/libcpath_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcpath/libcpath_error.h` & `libvhdi-20240509/libcpath/libcpath_error.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcpath/Makefile.in` & `libvhdi-20240509/libcpath/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -440,14 +440,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -502,16 +504,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCPATH_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCPATH_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCPATH_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCPATH_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCPATH_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBUNA_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCPATH_TRUE@noinst_LTLIBRARIES = libcpath.la
 @HAVE_LOCAL_LIBCPATH_TRUE@libcpath_la_SOURCES = \
@@ -523,15 +525,16 @@
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libclocale.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libcsplit.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libuna.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_support.c libcpath_support.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_system_string.c libcpath_system_string.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -734,24 +737,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcpath_error.Plo
+	-rm -f ./$(DEPDIR)/libcpath_path.Plo
+	-rm -f ./$(DEPDIR)/libcpath_support.Plo
+	-rm -f ./$(DEPDIR)/libcpath_system_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -838,17 +847,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcpath ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcpath_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvhdi-20240303/libcpath/libcpath_libuna.h` & `libvhdi-20240509/libcpath/libcpath_libuna.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcpath/libcpath_unused.h` & `libvhdi-20240509/libcpath/libcpath_unused.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcpath/libcpath_path.c` & `libvhdi-20240509/libcpath/libcpath_path.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcpath/libcpath_path.h` & `libvhdi-20240509/libcpath/libcpath_path.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/ChangeLog` & `libvhdi-20240509/ChangeLog`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/manuals/libvhdi.3` & `libvhdi-20240509/manuals/libvhdi.3`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/manuals/Makefile.in` & `libvhdi-20240509/manuals/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -413,14 +413,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -482,15 +484,16 @@
 	vhdiinfo.1 \
 	libvhdi.3
 
 EXTRA_DIST = \
 	vhdiinfo.1 \
 	libvhdi.3
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -683,23 +686,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -781,13 +786,10 @@
 	mostlyclean-libtool pdf pdf-am ps ps-am sources-am \
 	sources-local splint-am splint-local tags-am uninstall \
 	uninstall-am uninstall-man uninstall-man1 uninstall-man3
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libvhdi-20240303/manuals/vhdiinfo.1` & `libvhdi-20240509/manuals/vhdiinfo.1`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/vhdi_test_functions.h` & `libvhdi-20240509/tests/vhdi_test_functions.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/vhdi_test_libcnotify.h` & `libvhdi-20240509/tests/vhdi_test_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/vhdi_test_file_footer.c` & `libvhdi-20240509/tests/vhdi_test_file_footer.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/vhdi_test_parent_locator_header.c` & `libvhdi-20240509/tests/vhdi_test_parent_locator_header.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/vhdi_test_tools_signal.c` & `libvhdi-20240509/tests/vhdi_test_tools_signal.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/test_vhdiinfo.sh` & `libvhdi-20240509/tests/test_vhdiinfo.sh`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Info tool testing script
 #
-# Version: 20231005
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 PROFILES=("vhdiinfo");
 OPTIONS_PER_PROFILE=("");
@@ -28,20 +28,17 @@
 if ! test -x "${TEST_EXECUTABLE}";
 then
 	echo "Missing test executable: ${TEST_EXECUTABLE}";
 
 	exit ${EXIT_FAILURE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libvhdi-20240303/tests/vhdi_test_metadata_values.c` & `libvhdi-20240509/tests/vhdi_test_metadata_values.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/test_tools.sh` & `libvhdi-20240509/tests/test_library.sh`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 #!/usr/bin/env bash
-# Tests tools functions and types.
+# Tests library functions and types.
 #
-# Version: 20231007
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
-TOOLS_TESTS="info_handle output signal";
-TOOLS_TESTS_WITH_INPUT="";
+LIBRARY_TESTS="block_allocation_table block_descriptor checksum dynamic_disk_header error file_footer file_information image_header io_handle metadata_table metadata_table_entry metadata_table_header metadata_values notify parent_locator parent_locator_entry parent_locator_header region_table region_table_entry region_table_header sector_range_descriptor";
+LIBRARY_TESTS_WITH_INPUT="file support";
 OPTION_SETS=();
 
 INPUT_GLOB="*";
 
 run_test()
 {
 	local TEST_NAME=$1;
 
 	local TEST_DESCRIPTION="Testing: ${TEST_NAME}";
-	local TEST_EXECUTABLE="./vhdi_test_tools_${TEST_NAME}";
+	local TEST_EXECUTABLE="./vhdi_test_${TEST_NAME}";
 
 	if ! test -x "${TEST_EXECUTABLE}";
 	then
 		TEST_EXECUTABLE="${TEST_EXECUTABLE}.exe";
 	fi
 
 	# TODO: add support for TEST_PROFILE and OPTION_SETS?
@@ -33,15 +33,15 @@
 }
 
 run_test_with_input()
 {
 	local TEST_NAME=$1;
 
 	local TEST_DESCRIPTION="Testing: ${TEST_NAME}";
-	local TEST_EXECUTABLE="./vhdi_test_tools_${TEST_NAME}";
+	local TEST_EXECUTABLE="./vhdi_test_${TEST_NAME}";
 
 	if ! test -x "${TEST_EXECUTABLE}";
 	then
 		TEST_EXECUTABLE="${TEST_EXECUTABLE}.exe";
 	fi
 
 	if ! test -d "input";
@@ -55,15 +55,15 @@
 	if test ${RESULT} -eq ${EXIT_SUCCESS};
 	then
 		echo "No files or directories found in the test input directory";
 
 		return ${EXIT_IGNORE};
 	fi
 
-	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "vhditools");
+	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "libvhdi");
 
 	local IGNORE_LIST=$(read_ignore_list "${TEST_PROFILE_DIRECTORY}");
 
 	RESULT=${EXIT_SUCCESS};
 
 	for TEST_SET_INPUT_DIRECTORY in input/*;
 	do
@@ -132,38 +132,35 @@
 			break;
 		fi
 	done
 
 	return ${RESULT};
 }
 
-if test -n "${SKIP_TOOLS_TESTS}";
+if test -n "${SKIP_LIBRARY_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
 
 source ${TEST_RUNNER};
 
 RESULT=${EXIT_IGNORE};
 
-for TEST_NAME in ${TOOLS_TESTS};
+for TEST_NAME in ${LIBRARY_TESTS};
 do
 	run_test "${TEST_NAME}";
 	RESULT=$?;
 
 	if test ${RESULT} -ne ${EXIT_SUCCESS};
 	then
 		break;
@@ -171,15 +168,15 @@
 done
 
 if test ${RESULT} -ne ${EXIT_SUCCESS} && test ${RESULT} -ne ${EXIT_IGNORE};
 then
 	exit ${RESULT};
 fi
 
-for TEST_NAME in ${TOOLS_TESTS_WITH_INPUT};
+for TEST_NAME in ${LIBRARY_TESTS_WITH_INPUT};
 do
 	if test -d "input";
 	then
 		run_test_with_input "${TEST_NAME}";
 		RESULT=$?;
 	else
 		run_test "${TEST_NAME}";
```

### Comparing `libvhdi-20240303/tests/vhdi_test_block_allocation_table.c` & `libvhdi-20240509/tests/vhdi_test_block_allocation_table.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/vhdi_test_image_header.c` & `libvhdi-20240509/tests/vhdi_test_image_header.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/pyvhdi_test_support.py` & `libvhdi-20240509/tests/pyvhdi_test_support.py`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/vhdi_test_tools_info_handle.c` & `libvhdi-20240509/tests/vhdi_test_tools_info_handle.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/Makefile.am` & `libvhdi-20240509/tests/Makefile.am`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AUTOMAKE_OPTIONS = subdir-objects
 
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -447,13 +447,12 @@
 	vhdi_test_tools_signal.c \
 	vhdi_test_unused.h
 
 vhdi_test_tools_signal_LDADD = \
 	../libvhdi/libvhdi.la \
 	@LIBCERROR_LIBADD@
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
-
-distclean: clean
-	-rm -f Makefile
+DISTCLEANFILES = \
+	Makefile \
+	Makefile.in \
+	notify_stream.log
```

### Comparing `libvhdi-20240303/tests/pyvhdi_test_file.py` & `libvhdi-20240509/tests/pyvhdi_test_file.py`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/vhdi_test_error.c` & `libvhdi-20240509/tests/vhdi_test_error.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/vhdi_test_unused.h` & `libvhdi-20240509/tests/vhdi_test_unused.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/vhdi_test_checksum.c` & `libvhdi-20240509/tests/vhdi_test_checksum.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/vhdi_test_file.c` & `libvhdi-20240509/tests/vhdi_test_file.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/vhdi_test_functions.c` & `libvhdi-20240509/tests/vhdi_test_functions.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/vhdi_test_memory.c` & `libvhdi-20240509/tests/vhdi_test_memory.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/vhdi_test_metadata_table.c` & `libvhdi-20240509/tests/vhdi_test_metadata_table.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/vhdi_test_libbfio.h` & `libvhdi-20240509/tests/vhdi_test_libbfio.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/vhdi_test_dynamic_disk_header.c` & `libvhdi-20240509/tests/vhdi_test_dynamic_disk_header.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/vhdi_test_getopt.c` & `libvhdi-20240509/tests/vhdi_test_getopt.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/vhdi_test_parent_locator_entry.c` & `libvhdi-20240509/tests/vhdi_test_parent_locator_entry.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/test_python_module.sh` & `libvhdi-20240509/tests/test_python_module.sh`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 #!/usr/bin/env bash
 # Tests Python module functions and types.
 #
-# Version: 20240120
+# Version: 20240417
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_NO_TESTS_RAN=5;
 EXIT_IGNORE=77;
 
 TEST_FUNCTIONS="support";
 TEST_FUNCTIONS_WITH_INPUT="file";
 OPTION_SETS=();
 
 TEST_TOOL_DIRECTORY=".";
 INPUT_GLOB="*";
 
+LIBRARY_NAME="libvhdi";
+PYTHON_MODULE="pyvhdi";
+
 test_python_function()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pyvhdi_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	run_test_with_arguments "${TEST_DESCRIPTION}" "${TEST_SCRIPT}";
 	local RESULT=$?;
 
 	return ${RESULT};
 }
 
 test_python_function_with_input()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pyvhdi_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	if ! test -d "input";
 	then
 		echo "Test input directory not found.";
 
 		return ${EXIT_IGNORE};
 	fi
@@ -46,15 +49,15 @@
 	if test ${RESULT} -eq ${EXIT_SUCCESS};
 	then
 		echo "No files or directories found in the test input directory";
 
 		return ${EXIT_IGNORE};
 	fi
 
-	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "pyvhdi");
+	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "${PYTHON_MODULE}");
 
 	local IGNORE_LIST=$(read_ignore_list "${TEST_PROFILE_DIRECTORY}");
 
 	RESULT=${EXIT_SUCCESS};
 
 	for TEST_SET_INPUT_DIRECTORY in input/*;
 	do
@@ -121,30 +124,35 @@
 }
 
 if test -n "${SKIP_PYTHON_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
 
 source ${TEST_RUNNER};
 
+PLATFORM=`uname -s | sed 's/-.*$//'`;
+
+if test "${PLATFORM}" = "MINGW64_NT" || test "${PLATFORM}" = "MSYS_NT";
+then
+	cp ../${LIBRARY_NAME}/.libs/*.dll ../${PYTHON_MODULE}/.libs/;
+	cp ../${PYTHON_MODULE}/.libs/${PYTHON_MODULE}.dll ../${PYTHON_MODULE}/.libs/${PYTHON_MODULE}.pyd;
+fi
+
 RESULT=${EXIT_IGNORE};
 
 for TEST_FUNCTION in ${TEST_FUNCTIONS};
 do
 	test_python_function "${TEST_FUNCTION}";
 	RESULT=$?;
```

### Comparing `libvhdi-20240303/tests/vhdi_test_libcerror.h` & `libvhdi-20240509/tests/vhdi_test_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/vhdi_test_memory.h` & `libvhdi-20240509/tests/vhdi_test_memory.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/vhdi_test_block_descriptor.c` & `libvhdi-20240509/tests/vhdi_test_block_descriptor.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/vhdi_test_support.c` & `libvhdi-20240509/tests/vhdi_test_support.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/vhdi_test_region_table.c` & `libvhdi-20240509/tests/vhdi_test_region_table.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/vhdi_test_sector_range_descriptor.c` & `libvhdi-20240509/tests/vhdi_test_sector_range_descriptor.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/vhdi_test_libcpath.h` & `libvhdi-20240509/tests/vhdi_test_libcpath.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/vhdi_test_notify.c` & `libvhdi-20240509/tests/vhdi_test_notify.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/vhdi_test_region_table_header.c` & `libvhdi-20240509/tests/vhdi_test_region_table_header.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/test_runner.sh` & `libvhdi-20240509/tests/test_runner.sh`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/vhdi_test_libvhdi.h` & `libvhdi-20240509/tests/vhdi_test_libvhdi.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/vhdi_test_io_handle.c` & `libvhdi-20240509/tests/vhdi_test_io_handle.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/vhdi_test_getopt.h` & `libvhdi-20240509/tests/vhdi_test_getopt.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/vhdi_test_libclocale.h` & `libvhdi-20240509/tests/vhdi_test_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/vhdi_test_tools_output.c` & `libvhdi-20240509/tests/vhdi_test_tools_output.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/vhdi_test_metadata_table_header.c` & `libvhdi-20240509/tests/vhdi_test_metadata_table_header.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/vhdi_test_libuna.h` & `libvhdi-20240509/tests/vhdi_test_libuna.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/vhdi_test_file_information.c` & `libvhdi-20240509/tests/vhdi_test_file_information.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/Makefile.in` & `libvhdi-20240509/tests/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -866,14 +866,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -929,16 +931,16 @@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AUTOMAKE_OPTIONS = subdir-objects
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -1349,16 +1351,18 @@
 	vhdi_test_tools_signal.c \
 	vhdi_test_unused.h
 
 vhdi_test_tools_signal_LDADD = \
 	../libvhdi/libvhdi.la \
 	@LIBCERROR_LIBADD@
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	Makefile \
+	Makefile.in \
+	notify_stream.log
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .log .o .obj .test .test$(EXEEXT) .trs
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -1897,24 +1901,59 @@
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
 	-rm -f ../vhditools/$(DEPDIR)/$(am__dirstamp)
 	-rm -f ../vhditools/$(am__dirstamp)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-checkPROGRAMS clean-generic clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ../vhditools/$(DEPDIR)/byte_size_string.Po
+	-rm -f ../vhditools/$(DEPDIR)/info_handle.Po
+	-rm -f ../vhditools/$(DEPDIR)/vhditools_output.Po
+	-rm -f ../vhditools/$(DEPDIR)/vhditools_signal.Po
+	-rm -f ./$(DEPDIR)/vhdi_test_block_allocation_table.Po
+	-rm -f ./$(DEPDIR)/vhdi_test_block_descriptor.Po
+	-rm -f ./$(DEPDIR)/vhdi_test_checksum.Po
+	-rm -f ./$(DEPDIR)/vhdi_test_dynamic_disk_header.Po
+	-rm -f ./$(DEPDIR)/vhdi_test_error.Po
+	-rm -f ./$(DEPDIR)/vhdi_test_file.Po
+	-rm -f ./$(DEPDIR)/vhdi_test_file_footer.Po
+	-rm -f ./$(DEPDIR)/vhdi_test_file_information.Po
+	-rm -f ./$(DEPDIR)/vhdi_test_functions.Po
+	-rm -f ./$(DEPDIR)/vhdi_test_getopt.Po
+	-rm -f ./$(DEPDIR)/vhdi_test_image_header.Po
+	-rm -f ./$(DEPDIR)/vhdi_test_io_handle.Po
+	-rm -f ./$(DEPDIR)/vhdi_test_memory.Po
+	-rm -f ./$(DEPDIR)/vhdi_test_metadata_table.Po
+	-rm -f ./$(DEPDIR)/vhdi_test_metadata_table_entry.Po
+	-rm -f ./$(DEPDIR)/vhdi_test_metadata_table_header.Po
+	-rm -f ./$(DEPDIR)/vhdi_test_metadata_values.Po
+	-rm -f ./$(DEPDIR)/vhdi_test_notify.Po
+	-rm -f ./$(DEPDIR)/vhdi_test_parent_locator.Po
+	-rm -f ./$(DEPDIR)/vhdi_test_parent_locator_entry.Po
+	-rm -f ./$(DEPDIR)/vhdi_test_parent_locator_header.Po
+	-rm -f ./$(DEPDIR)/vhdi_test_region_table.Po
+	-rm -f ./$(DEPDIR)/vhdi_test_region_table_entry.Po
+	-rm -f ./$(DEPDIR)/vhdi_test_region_table_header.Po
+	-rm -f ./$(DEPDIR)/vhdi_test_sector_range_descriptor.Po
+	-rm -f ./$(DEPDIR)/vhdi_test_support.Po
+	-rm -f ./$(DEPDIR)/vhdi_test_tools_info_handle.Po
+	-rm -f ./$(DEPDIR)/vhdi_test_tools_output.Po
+	-rm -f ./$(DEPDIR)/vhdi_test_tools_signal.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -2030,13 +2069,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	recheck sources-am sources-local splint-am splint-local tags \
 	tags-am uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libvhdi-20240303/tests/vhdi_test_metadata_table_entry.c` & `libvhdi-20240509/tests/vhdi_test_metadata_table_entry.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/vhdi_test_macros.h` & `libvhdi-20240509/tests/vhdi_test_macros.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/vhdi_test_region_table_entry.c` & `libvhdi-20240509/tests/vhdi_test_region_table_entry.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/vhdi_test_parent_locator.c` & `libvhdi-20240509/tests/vhdi_test_parent_locator.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/tests/test_library.sh` & `libvhdi-20240509/tests/test_tools.sh`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 #!/usr/bin/env bash
-# Tests library functions and types.
+# Tests tools functions and types.
 #
-# Version: 20231007
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
-LIBRARY_TESTS="block_allocation_table block_descriptor checksum dynamic_disk_header error file_footer file_information image_header io_handle metadata_table metadata_table_entry metadata_table_header metadata_values notify parent_locator parent_locator_entry parent_locator_header region_table region_table_entry region_table_header sector_range_descriptor";
-LIBRARY_TESTS_WITH_INPUT="file support";
+TOOLS_TESTS="info_handle output signal";
+TOOLS_TESTS_WITH_INPUT="";
 OPTION_SETS=();
 
 INPUT_GLOB="*";
 
 run_test()
 {
 	local TEST_NAME=$1;
 
 	local TEST_DESCRIPTION="Testing: ${TEST_NAME}";
-	local TEST_EXECUTABLE="./vhdi_test_${TEST_NAME}";
+	local TEST_EXECUTABLE="./vhdi_test_tools_${TEST_NAME}";
 
 	if ! test -x "${TEST_EXECUTABLE}";
 	then
 		TEST_EXECUTABLE="${TEST_EXECUTABLE}.exe";
 	fi
 
 	# TODO: add support for TEST_PROFILE and OPTION_SETS?
@@ -33,15 +33,15 @@
 }
 
 run_test_with_input()
 {
 	local TEST_NAME=$1;
 
 	local TEST_DESCRIPTION="Testing: ${TEST_NAME}";
-	local TEST_EXECUTABLE="./vhdi_test_${TEST_NAME}";
+	local TEST_EXECUTABLE="./vhdi_test_tools_${TEST_NAME}";
 
 	if ! test -x "${TEST_EXECUTABLE}";
 	then
 		TEST_EXECUTABLE="${TEST_EXECUTABLE}.exe";
 	fi
 
 	if ! test -d "input";
@@ -55,15 +55,15 @@
 	if test ${RESULT} -eq ${EXIT_SUCCESS};
 	then
 		echo "No files or directories found in the test input directory";
 
 		return ${EXIT_IGNORE};
 	fi
 
-	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "libvhdi");
+	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "vhditools");
 
 	local IGNORE_LIST=$(read_ignore_list "${TEST_PROFILE_DIRECTORY}");
 
 	RESULT=${EXIT_SUCCESS};
 
 	for TEST_SET_INPUT_DIRECTORY in input/*;
 	do
@@ -132,38 +132,35 @@
 			break;
 		fi
 	done
 
 	return ${RESULT};
 }
 
-if test -n "${SKIP_LIBRARY_TESTS}";
+if test -n "${SKIP_TOOLS_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
 
 source ${TEST_RUNNER};
 
 RESULT=${EXIT_IGNORE};
 
-for TEST_NAME in ${LIBRARY_TESTS};
+for TEST_NAME in ${TOOLS_TESTS};
 do
 	run_test "${TEST_NAME}";
 	RESULT=$?;
 
 	if test ${RESULT} -ne ${EXIT_SUCCESS};
 	then
 		break;
@@ -171,15 +168,15 @@
 done
 
 if test ${RESULT} -ne ${EXIT_SUCCESS} && test ${RESULT} -ne ${EXIT_IGNORE};
 then
 	exit ${RESULT};
 fi
 
-for TEST_NAME in ${LIBRARY_TESTS_WITH_INPUT};
+for TEST_NAME in ${TOOLS_TESTS_WITH_INPUT};
 do
 	if test -d "input";
 	then
 		run_test_with_input "${TEST_NAME}";
 		RESULT=$?;
 	else
 		run_test "${TEST_NAME}";
```

### Comparing `libvhdi-20240303/libvhdi.pc.in` & `libvhdi-20240509/libvhdi.pc.in`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/vhditools/vhdiinfo.c` & `libvhdi-20240509/vhditools/vhdiinfo.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/vhditools/vhditools_signal.c` & `libvhdi-20240509/vhditools/vhditools_signal.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/vhditools/mount_dokan.c` & `libvhdi-20240509/vhditools/mount_dokan.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/vhditools/mount_file_system.h` & `libvhdi-20240509/vhditools/mount_file_system.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/vhditools/mount_fuse.c` & `libvhdi-20240509/vhditools/mount_fuse.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/vhditools/info_handle.h` & `libvhdi-20240509/vhditools/info_handle.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/vhditools/vhditools_getopt.c` & `libvhdi-20240509/vhditools/vhditools_getopt.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/vhditools/mount_dokan.h` & `libvhdi-20240509/vhditools/mount_dokan.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/vhditools/vhditools_libcnotify.h` & `libvhdi-20240509/vhditools/vhditools_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/vhditools/vhditools_output.c` & `libvhdi-20240509/vhditools/vhditools_output.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/vhditools/vhditools_libclocale.h` & `libvhdi-20240509/vhditools/vhditools_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/vhditools/mount_file_system.c` & `libvhdi-20240509/vhditools/mount_file_system.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/vhditools/vhditools_output.h` & `libvhdi-20240509/vhditools/vhditools_output.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/vhditools/vhditools_i18n.h` & `libvhdi-20240509/vhditools/vhditools_i18n.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/vhditools/vhditools_signal.h` & `libvhdi-20240509/vhditools/vhditools_signal.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/vhditools/byte_size_string.c` & `libvhdi-20240509/vhditools/byte_size_string.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/vhditools/vhditools_libcpath.h` & `libvhdi-20240509/vhditools/vhditools_libcpath.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/vhditools/Makefile.am` & `libvhdi-20240509/vhditools/Makefile.am`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -77,19 +77,17 @@
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCDATA_LIBADD@ \
 	../libvhdi/libvhdi.la \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on vhdiinfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(vhdiinfo_SOURCES)
 	@echo "Running splint on vhdimount ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(vhdimount_SOURCES)
```

### Comparing `libvhdi-20240303/vhditools/mount_file_entry.c` & `libvhdi-20240509/vhditools/mount_file_entry.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/vhditools/info_handle.c` & `libvhdi-20240509/vhditools/info_handle.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/vhditools/vhditools_libcdata.h` & `libvhdi-20240509/vhditools/vhditools_libcdata.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/vhditools/mount_file_entry.h` & `libvhdi-20240509/vhditools/mount_file_entry.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/vhditools/vhditools_libfguid.h` & `libvhdi-20240509/vhditools/vhditools_libfguid.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/vhditools/vhditools_libcerror.h` & `libvhdi-20240509/vhditools/vhditools_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/vhditools/vhditools_getopt.h` & `libvhdi-20240509/vhditools/vhditools_getopt.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/vhditools/vhditools_libuna.h` & `libvhdi-20240509/vhditools/vhditools_libuna.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/vhditools/vhdimount.c` & `libvhdi-20240509/vhditools/vhdimount.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/vhditools/mount_handle.h` & `libvhdi-20240509/vhditools/mount_handle.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/vhditools/vhditools_unused.h` & `libvhdi-20240509/vhditools/vhditools_unused.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/vhditools/vhditools_libbfio.h` & `libvhdi-20240509/vhditools/vhditools_libbfio.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/vhditools/mount_handle.c` & `libvhdi-20240509/vhditools/mount_handle.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/vhditools/vhditools_libvhdi.h` & `libvhdi-20240509/vhditools/vhditools_libvhdi.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/vhditools/Makefile.in` & `libvhdi-20240509/vhditools/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -447,14 +447,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -509,16 +511,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -586,15 +588,16 @@
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCDATA_LIBADD@ \
 	../libvhdi/libvhdi.la \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -851,23 +854,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-binPROGRAMS clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/byte_size_string.Po
+	-rm -f ./$(DEPDIR)/info_handle.Po
+	-rm -f ./$(DEPDIR)/mount_dokan.Po
+	-rm -f ./$(DEPDIR)/mount_file_entry.Po
+	-rm -f ./$(DEPDIR)/mount_file_system.Po
+	-rm -f ./$(DEPDIR)/mount_fuse.Po
+	-rm -f ./$(DEPDIR)/mount_handle.Po
+	-rm -f ./$(DEPDIR)/vhdiinfo.Po
+	-rm -f ./$(DEPDIR)/vhdimount.Po
+	-rm -f ./$(DEPDIR)/vhditools_getopt.Po
+	-rm -f ./$(DEPDIR)/vhditools_output.Po
+	-rm -f ./$(DEPDIR)/vhditools_signal.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -962,17 +979,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on vhdiinfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(vhdiinfo_SOURCES)
 	@echo "Running splint on vhdimount ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(vhdimount_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvhdi-20240303/vhditools/byte_size_string.h` & `libvhdi-20240509/vhditools/byte_size_string.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/vhditools/mount_fuse.h` & `libvhdi-20240509/vhditools/mount_fuse.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/ossfuzz/ossfuzz_libvhdi.h` & `libvhdi-20240509/ossfuzz/ossfuzz_libvhdi.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/ossfuzz/Makefile.am` & `libvhdi-20240509/ossfuzz/Makefile.am`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LIB_FUZZING_ENGINE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
 	@LIBCPATH_CPPFLAGS@ \
@@ -29,17 +29,15 @@
 	../libvhdi/libvhdi.la \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on file_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(file_fuzzer_SOURCES)
```

### Comparing `libvhdi-20240303/ossfuzz/ossfuzz_libbfio.h` & `libvhdi-20240509/ossfuzz/ossfuzz_libbfio.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/ossfuzz/file_fuzzer.cc` & `libvhdi-20240509/ossfuzz/file_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/ossfuzz/Makefile.in` & `libvhdi-20240509/ossfuzz/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -453,14 +453,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -515,16 +517,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@AM_CPPFLAGS = \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCFILE_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCPATH_CPPFLAGS@ \
@@ -544,15 +546,16 @@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCDATA_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	../libvhdi/libvhdi.la \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCNOTIFY_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCLOCALE_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCERROR_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .cc .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -794,23 +797,26 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-binPROGRAMS clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/file_fuzzer.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -894,17 +900,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on file_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(file_fuzzer_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libvhdi-20240303/ltmain.sh` & `libvhdi-20240509/ltmain.sh`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcsplit/libcsplit_narrow_string.c` & `libvhdi-20240509/libcsplit/libcsplit_narrow_string.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcsplit/libcsplit_definitions.h` & `libvhdi-20240509/libcsplit/libcsplit_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -31,17 +31,17 @@
 #include <libcsplit/definitions.h>
 
 /* The definitions in <libcsplit/definitions.h> are copied here
  * for local use of libcsplit
  */
 #else
 
-#define LIBCSPLIT_VERSION			20240110
+#define LIBCSPLIT_VERSION			20240414
 
 /* The libcsplit version string
  */
-#define LIBCSPLIT_VERSION_STRING		"20240110"
+#define LIBCSPLIT_VERSION_STRING		"20240414"
 
 #endif /* !defined( HAVE_LOCAL_LIBCSPLIT ) */
 
 #endif
```

### Comparing `libvhdi-20240303/libcsplit/libcsplit_types.h` & `libvhdi-20240509/libcsplit/libcsplit_types.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcsplit/libcsplit_wide_split_string.c` & `libvhdi-20240509/libcsplit/libcsplit_wide_split_string.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcsplit/libcsplit_support.h` & `libvhdi-20240509/libcsplit/libcsplit_support.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcsplit/Makefile.am` & `libvhdi-20240509/libcsplit/Makefile.am`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCSPLIT
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcsplit.la
 
 libcsplit_la_SOURCES = \
 	libcsplit_definitions.h \
 	libcsplit_error.c libcsplit_error.h \
@@ -16,19 +16,17 @@
 	libcsplit_support.c libcsplit_support.h \
 	libcsplit_types.h \
 	libcsplit_unused.h \
 	libcsplit_wide_split_string.c libcsplit_wide_split_string.h \
 	libcsplit_wide_string.c libcsplit_wide_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcsplit ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcsplit_la_SOURCES)
```

### Comparing `libvhdi-20240303/libcsplit/libcsplit_libcerror.h` & `libvhdi-20240509/libcsplit/libcsplit_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcsplit/libcsplit_wide_string.c` & `libvhdi-20240509/libcsplit/libcsplit_wide_string.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcsplit/libcsplit_unused.h` & `libvhdi-20240509/libcsplit/libcsplit_unused.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcsplit/libcsplit_wide_split_string.h` & `libvhdi-20240509/libcsplit/libcsplit_wide_split_string.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcsplit/libcsplit_error.c` & `libvhdi-20240509/libcsplit/libcsplit_error.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcsplit/libcsplit_narrow_split_string.c` & `libvhdi-20240509/libcsplit/libcsplit_narrow_split_string.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcsplit/libcsplit_extern.h` & `libvhdi-20240509/libcsplit/libcsplit_extern.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcsplit/libcsplit_error.h` & `libvhdi-20240509/libcsplit/libcsplit_error.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcsplit/libcsplit_support.c` & `libvhdi-20240509/libcsplit/libcsplit_support.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcsplit/libcsplit_wide_string.h` & `libvhdi-20240509/libcsplit/libcsplit_wide_string.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcsplit/Makefile.in` & `libvhdi-20240509/libcsplit/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -450,14 +450,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -512,16 +514,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCSPLIT_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCSPLIT_TRUE@noinst_LTLIBRARIES = libcsplit.la
 @HAVE_LOCAL_LIBCSPLIT_TRUE@libcsplit_la_SOURCES = \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_definitions.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_error.c libcsplit_error.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_extern.h \
@@ -530,15 +532,16 @@
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_libcerror.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_support.c libcsplit_support.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_types.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_unused.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_wide_split_string.c libcsplit_wide_split_string.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_wide_string.c libcsplit_wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -743,24 +746,32 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcsplit_error.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_narrow_split_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_narrow_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_support.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_wide_split_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_wide_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -849,17 +860,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcsplit ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcsplit_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvhdi-20240303/libcsplit/libcsplit_narrow_split_string.h` & `libvhdi-20240509/libcsplit/libcsplit_narrow_split_string.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcsplit/libcsplit_narrow_string.h` & `libvhdi-20240509/libcsplit/libcsplit_narrow_string.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_region_type_identifier.c` & `libvhdi-20240509/libvhdi/libvhdi_region_type_identifier.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_file_footer.h` & `libvhdi-20240509/libvhdi/libvhdi_file_footer.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_libfguid.h` & `libvhdi-20240509/libvhdi/libvhdi_libfguid.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_dynamic_disk_header.c` & `libvhdi-20240509/libvhdi/libvhdi_dynamic_disk_header.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_types.h` & `libvhdi-20240509/libvhdi/libvhdi_types.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_block_descriptor.c` & `libvhdi-20240509/libvhdi/libvhdi_block_descriptor.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_libcdata.h` & `libvhdi-20240509/libvhdi/libvhdi_libcdata.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_parent_locator_entry.c` & `libvhdi-20240509/libvhdi/libvhdi_parent_locator_entry.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_libbfio.h` & `libvhdi-20240509/libvhdi/libvhdi_libbfio.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_image_header.c` & `libvhdi-20240509/libvhdi/libvhdi_image_header.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_error.h` & `libvhdi-20240509/libvhdi/libvhdi_error.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_block_descriptor.h` & `libvhdi-20240509/libvhdi/libvhdi_block_descriptor.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_debug.h` & `libvhdi-20240509/libvhdi/libvhdi_debug.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_libcnotify.h` & `libvhdi-20240509/libvhdi/libvhdi_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_region_type_identifier.h` & `libvhdi-20240509/libvhdi/libvhdi_region_type_identifier.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_libcthreads.h` & `libvhdi-20240509/libvhdi/libvhdi_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_support.h` & `libvhdi-20240509/libvhdi/libvhdi_support.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_file_information.h` & `libvhdi-20240509/libvhdi/libvhdi_file_information.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_i18n.h` & `libvhdi-20240509/libvhdi/libvhdi_i18n.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/vhdi_file_footer.h` & `libvhdi-20240509/libvhdi/vhdi_file_footer.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_io_handle.h` & `libvhdi-20240509/libvhdi/libvhdi_io_handle.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_libclocale.h` & `libvhdi-20240509/libvhdi/libvhdi_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_libfcache.h` & `libvhdi-20240509/libvhdi/libvhdi_libfcache.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_checksum.c` & `libvhdi-20240509/libvhdi/libvhdi_checksum.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_metadata_table_header.h` & `libvhdi-20240509/libvhdi/libvhdi_metadata_table_header.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_unused.h` & `libvhdi-20240509/libvhdi/libvhdi_unused.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi.rc.in` & `libvhdi-20240509/libvhdi/libvhdi.rc.in`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_block_allocation_table.c` & `libvhdi-20240509/libvhdi/libvhdi_block_allocation_table.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_io_handle.c` & `libvhdi-20240509/libvhdi/libvhdi_io_handle.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/Makefile.am` & `libvhdi-20240509/libvhdi/Makefile.am`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 AM_CPPFLAGS = \
 	-DLOCALEDIR=\"$(datadir)/locale\" \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -91,21 +91,19 @@
 libvhdi_la_LDFLAGS = -no-undefined -version-info 1:0:0
 
 EXTRA_DIST = \
 	libvhdi_definitions.h.in \
 	libvhdi.rc \
 	libvhdi.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libvhdi_definitions.h \
+	libvhdi.rc \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f libvhdi_definitions.h
-	-rm -f libvhdi.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libvhdi ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libvhdi_la_SOURCES)
```

### Comparing `libvhdi-20240303/libvhdi/libvhdi_region_table_entry.h` & `libvhdi-20240509/libvhdi/libvhdi_region_table_entry.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_metadata_values.c` & `libvhdi-20240509/libvhdi/libvhdi_metadata_values.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_notify.h` & `libvhdi-20240509/libvhdi/libvhdi_notify.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_file_information.c` & `libvhdi-20240509/libvhdi/libvhdi_file_information.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_error.c` & `libvhdi-20240509/libvhdi/libvhdi_error.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_libfdata.h` & `libvhdi-20240509/libvhdi/libvhdi_libfdata.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_parent_locator_entry.h` & `libvhdi-20240509/libvhdi/libvhdi_parent_locator_entry.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi.rc` & `libvhdi-20240509/libvhdi/libvhdi.rc`

 * *Files 9% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library to access the Virtual Hard Disk (VHD) image format\0"
-      VALUE "FileVersion",		"20240303" "\0"
+      VALUE "FileVersion",		"20240509" "\0"
       VALUE "InternalName",		"libvhdi.dll\0"
       VALUE "LegalCopyright",		"(C) 2012-2024, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"libvhdi.dll\0"
       VALUE "ProductName",		"libvhdi\0"
-      VALUE "ProductVersion",		"20240303" "\0"
+      VALUE "ProductVersion",		"20240509" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libvhdi/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `libvhdi-20240303/libvhdi/vhdi_region_table.h` & `libvhdi-20240509/libvhdi/vhdi_region_table.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_metadata_table.c` & `libvhdi-20240509/libvhdi/libvhdi_metadata_table.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_sector_range_descriptor.c` & `libvhdi-20240509/libvhdi/libvhdi_sector_range_descriptor.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_libuna.h` & `libvhdi-20240509/libvhdi/libvhdi_libuna.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_i18n.c` & `libvhdi-20240509/libvhdi/libvhdi_i18n.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_metadata_table_header.c` & `libvhdi-20240509/libvhdi/libvhdi_metadata_table_header.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_definitions.h.in` & `libvhdi-20240509/libvhdi/libvhdi_definitions.h.in`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_sector_range_descriptor.h` & `libvhdi-20240509/libvhdi/libvhdi_sector_range_descriptor.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_parent_locator_header.h` & `libvhdi-20240509/libvhdi/libvhdi_parent_locator_header.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_definitions.h` & `libvhdi-20240509/libvhdi/libvhdi_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -33,19 +33,19 @@
 #if !defined( HAVE_LOCAL_LIBVHDI )
 #include <libvhdi/definitions.h>
 
 /* The definitions in <libvhdi/definitions.h> are copied here
  * for local use of libvhdi
  */
 #else
-#define LIBVHDI_VERSION						20240303
+#define LIBVHDI_VERSION						20240509
 
 /* The version string
  */
-#define LIBVHDI_VERSION_STRING					"20240303"
+#define LIBVHDI_VERSION_STRING					"20240509"
 
 /* The access flags definitions
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBVHDI_ACCESS_FLAGS
```

### Comparing `libvhdi-20240303/libvhdi/libvhdi.c` & `libvhdi-20240509/libvhdi/libvhdi.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_metadata_table_entry.h` & `libvhdi-20240509/libvhdi/libvhdi_metadata_table_entry.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_parent_locator_header.c` & `libvhdi-20240509/libvhdi/libvhdi_parent_locator_header.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_metadata_table.h` & `libvhdi-20240509/libvhdi/libvhdi_metadata_table.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_region_table.c` & `libvhdi-20240509/libvhdi/libvhdi_region_table.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_region_table.h` & `libvhdi-20240509/libvhdi/libvhdi_region_table.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/vhdi_dynamic_disk_header.h` & `libvhdi-20240509/libvhdi/vhdi_dynamic_disk_header.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_checksum.h` & `libvhdi-20240509/libvhdi/libvhdi_checksum.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_libcerror.h` & `libvhdi-20240509/libvhdi/libvhdi_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/vhdi_metadata_table.h` & `libvhdi-20240509/libvhdi/vhdi_metadata_table.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/vhdi_image_header.h` & `libvhdi-20240509/libvhdi/vhdi_image_header.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_codepage.h` & `libvhdi-20240509/libvhdi/libvhdi_codepage.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_file_footer.c` & `libvhdi-20240509/libvhdi/libvhdi_file_footer.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/vhdi_parent_locator.h` & `libvhdi-20240509/libvhdi/vhdi_parent_locator.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_file.h` & `libvhdi-20240509/libvhdi/libvhdi_file.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_region_table_entry.c` & `libvhdi-20240509/libvhdi/libvhdi_region_table_entry.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_notify.c` & `libvhdi-20240509/libvhdi/libvhdi_notify.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_parent_locator.h` & `libvhdi-20240509/libvhdi/libvhdi_parent_locator.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_metadata_table_entry.c` & `libvhdi-20240509/libvhdi/libvhdi_metadata_table_entry.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_metadata_values.h` & `libvhdi-20240509/libvhdi/libvhdi_metadata_values.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_debug.c` & `libvhdi-20240509/libvhdi/libvhdi_debug.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_file.c` & `libvhdi-20240509/libvhdi/libvhdi_file.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_region_table_header.h` & `libvhdi-20240509/libvhdi/libvhdi_region_table_header.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_support.c` & `libvhdi-20240509/libvhdi/libvhdi_support.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_metadata_item_identifier.h` & `libvhdi-20240509/libvhdi/libvhdi_metadata_item_identifier.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/Makefile.in` & `libvhdi-20240509/libvhdi/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -500,14 +500,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -563,16 +565,16 @@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AM_CPPFLAGS = \
 	-DLOCALEDIR=\"$(datadir)/locale\" \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -656,15 +658,18 @@
 
 libvhdi_la_LDFLAGS = -no-undefined -version-info 1:0:0
 EXTRA_DIST = \
 	libvhdi_definitions.h.in \
 	libvhdi.rc \
 	libvhdi.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libvhdi_definitions.h \
+	libvhdi.rc \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -922,24 +927,54 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libLTLIBRARIES clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libvhdi.Plo
+	-rm -f ./$(DEPDIR)/libvhdi_block_allocation_table.Plo
+	-rm -f ./$(DEPDIR)/libvhdi_block_descriptor.Plo
+	-rm -f ./$(DEPDIR)/libvhdi_checksum.Plo
+	-rm -f ./$(DEPDIR)/libvhdi_debug.Plo
+	-rm -f ./$(DEPDIR)/libvhdi_dynamic_disk_header.Plo
+	-rm -f ./$(DEPDIR)/libvhdi_error.Plo
+	-rm -f ./$(DEPDIR)/libvhdi_file.Plo
+	-rm -f ./$(DEPDIR)/libvhdi_file_footer.Plo
+	-rm -f ./$(DEPDIR)/libvhdi_file_information.Plo
+	-rm -f ./$(DEPDIR)/libvhdi_i18n.Plo
+	-rm -f ./$(DEPDIR)/libvhdi_image_header.Plo
+	-rm -f ./$(DEPDIR)/libvhdi_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libvhdi_metadata_item_identifier.Plo
+	-rm -f ./$(DEPDIR)/libvhdi_metadata_table.Plo
+	-rm -f ./$(DEPDIR)/libvhdi_metadata_table_entry.Plo
+	-rm -f ./$(DEPDIR)/libvhdi_metadata_table_header.Plo
+	-rm -f ./$(DEPDIR)/libvhdi_metadata_values.Plo
+	-rm -f ./$(DEPDIR)/libvhdi_notify.Plo
+	-rm -f ./$(DEPDIR)/libvhdi_parent_locator.Plo
+	-rm -f ./$(DEPDIR)/libvhdi_parent_locator_entry.Plo
+	-rm -f ./$(DEPDIR)/libvhdi_parent_locator_header.Plo
+	-rm -f ./$(DEPDIR)/libvhdi_region_table.Plo
+	-rm -f ./$(DEPDIR)/libvhdi_region_table_entry.Plo
+	-rm -f ./$(DEPDIR)/libvhdi_region_table_header.Plo
+	-rm -f ./$(DEPDIR)/libvhdi_region_type_identifier.Plo
+	-rm -f ./$(DEPDIR)/libvhdi_sector_range_descriptor.Plo
+	-rm -f ./$(DEPDIR)/libvhdi_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1050,19 +1085,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-libLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libvhdi_definitions.h
-	-rm -f libvhdi.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libvhdi ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libvhdi_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvhdi-20240303/libvhdi/libvhdi_parent_locator.c` & `libvhdi-20240509/libvhdi/libvhdi_parent_locator.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_extern.h` & `libvhdi-20240509/libvhdi/libvhdi_extern.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_dynamic_disk_header.h` & `libvhdi-20240509/libvhdi/libvhdi_dynamic_disk_header.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_image_header.h` & `libvhdi-20240509/libvhdi/libvhdi_image_header.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_metadata_item_identifier.c` & `libvhdi-20240509/libvhdi/libvhdi_metadata_item_identifier.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_block_allocation_table.h` & `libvhdi-20240509/libvhdi/libvhdi_block_allocation_table.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/libvhdi_region_table_header.c` & `libvhdi-20240509/libvhdi/libvhdi_region_table_header.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libvhdi/vhdi_file_information.h` & `libvhdi-20240509/libvhdi/vhdi_file_information.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/po/remove-potcdate.sin` & `libvhdi-20240509/po/remove-potcdate.sin`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/po/Makefile.in.in` & `libvhdi-20240509/po/Makefile.in.in`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/po/en@quot.header` & `libvhdi-20240509/po/en@quot.header`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/po/en@boldquot.header` & `libvhdi-20240509/po/en@boldquot.header`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/po/insert-header.sin` & `libvhdi-20240509/po/insert-header.sin`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/po/Makevars` & `libvhdi-20240509/po/Makevars`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/po/Makevars.in` & `libvhdi-20240509/po/Makevars.in`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/po/Rules-quot` & `libvhdi-20240509/po/Rules-quot`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_windows_1251.c` & `libvhdi-20240509/libuna/libuna_codepage_windows_1251.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_utf16_string.c` & `libvhdi-20240509/libuna/libuna_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_base16_stream.c` & `libvhdi-20240509/libuna/libuna_base16_stream.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_utf8_stream.h` & `libvhdi-20240509/libuna/libuna_utf8_stream.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_iso_8859_2.h` & `libvhdi-20240509/libuna/libuna_codepage_iso_8859_2.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_windows_932.c` & `libvhdi-20240509/libuna/libuna_codepage_windows_932.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_mac_dingbats.h` & `libvhdi-20240509/libuna/libuna_codepage_mac_dingbats.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_utf8_string.c` & `libvhdi-20240509/libuna/libuna_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_base64_stream.c` & `libvhdi-20240509/libuna/libuna_base64_stream.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_error.h` & `libvhdi-20240509/libuna/libuna_error.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_mac_turkish.h` & `libvhdi-20240509/libuna/libuna_codepage_mac_turkish.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_unicode_character.c` & `libvhdi-20240509/libuna/libuna_unicode_character.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_mac_gaelic.c` & `libvhdi-20240509/libuna/libuna_codepage_mac_gaelic.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_mac_arabic.h` & `libvhdi-20240509/libuna/libuna_codepage_mac_arabic.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_mac_thai.c` & `libvhdi-20240509/libuna/libuna_codepage_mac_thai.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_windows_874.h` & `libvhdi-20240509/libuna/libuna_codepage_windows_874.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_iso_8859_15.h` & `libvhdi-20240509/libuna/libuna_codepage_iso_8859_15.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_utf8_string.h` & `libvhdi-20240509/libuna/libuna_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_iso_8859_16.c` & `libvhdi-20240509/libuna/libuna_codepage_iso_8859_16.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_windows_1255.c` & `libvhdi-20240509/libuna/libuna_codepage_windows_1255.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_utf7_stream.c` & `libvhdi-20240509/libuna/libuna_utf7_stream.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_byte_stream.h` & `libvhdi-20240509/libuna/libuna_byte_stream.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_koi8_u.c` & `libvhdi-20240509/libuna/libuna_codepage_koi8_u.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_unused.h` & `libvhdi-20240509/libuna/libuna_unused.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_iso_8859_6.c` & `libvhdi-20240509/libuna/libuna_codepage_iso_8859_6.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_iso_8859_14.c` & `libvhdi-20240509/libuna/libuna_codepage_iso_8859_14.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_base64_stream.h` & `libvhdi-20240509/libuna/libuna_base64_stream.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_error.c` & `libvhdi-20240509/libuna/libuna_error.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_mac_centraleurroman.h` & `libvhdi-20240509/libuna/libuna_codepage_mac_centraleurroman.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_mac_romanian.c` & `libvhdi-20240509/libuna/libuna_codepage_mac_romanian.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_iso_8859_6.h` & `libvhdi-20240509/libuna/libuna_codepage_iso_8859_6.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_iso_8859_9.c` & `libvhdi-20240509/libuna/libuna_codepage_iso_8859_9.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_mac_russian.h` & `libvhdi-20240509/libuna/libuna_codepage_mac_russian.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_mac_dingbats.c` & `libvhdi-20240509/libuna/libuna_codepage_mac_dingbats.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_iso_8859_15.c` & `libvhdi-20240509/libuna/libuna_codepage_iso_8859_15.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_windows_936.c` & `libvhdi-20240509/libuna/libuna_codepage_windows_936.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_mac_croatian.h` & `libvhdi-20240509/libuna/libuna_codepage_mac_croatian.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_scsu.h` & `libvhdi-20240509/libuna/libuna_scsu.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/Makefile.am` & `libvhdi-20240509/libuna/Makefile.am`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBUNA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libuna.la
 
 libuna_la_SOURCES = \
 	libuna_base16_stream.c libuna_base16_stream.h \
 	libuna_base32_stream.c libuna_base32_stream.h \
@@ -73,19 +73,17 @@
 	libuna_utf32_stream.c libuna_utf32_stream.h \
 	libuna_utf32_string.c libuna_utf32_string.h \
 	libuna_utf7_stream.c libuna_utf7_stream.h \
 	libuna_utf8_stream.c libuna_utf8_stream.h \
 	libuna_utf8_string.c libuna_utf8_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libuna ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libuna_la_SOURCES)
```

### Comparing `libvhdi-20240303/libuna/libuna_utf32_stream.c` & `libvhdi-20240509/libuna/libuna_utf32_stream.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_windows_936.h` & `libvhdi-20240509/libuna/libuna_codepage_windows_936.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_iso_8859_10.c` & `libvhdi-20240509/libuna/libuna_codepage_iso_8859_10.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_mac_roman.c` & `libvhdi-20240509/libuna/libuna_codepage_mac_roman.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_utf7_stream.h` & `libvhdi-20240509/libuna/libuna_utf7_stream.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_iso_8859_3.h` & `libvhdi-20240509/libuna/libuna_codepage_iso_8859_3.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_mac_thai.h` & `libvhdi-20240509/libuna/libuna_codepage_mac_thai.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_mac_farsi.h` & `libvhdi-20240509/libuna/libuna_codepage_mac_farsi.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_mac_ukrainian.c` & `libvhdi-20240509/libuna/libuna_codepage_mac_ukrainian.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_mac_inuit.c` & `libvhdi-20240509/libuna/libuna_codepage_mac_inuit.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_windows_932.h` & `libvhdi-20240509/libuna/libuna_codepage_windows_932.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_windows_874.c` & `libvhdi-20240509/libuna/libuna_codepage_windows_874.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_iso_8859_5.c` & `libvhdi-20240509/libuna/libuna_codepage_iso_8859_5.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_iso_8859_10.h` & `libvhdi-20240509/libuna/libuna_codepage_iso_8859_10.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_definitions.h` & `libvhdi-20240509/libuna/libuna_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 
 /* The definitions in <libuna/definitions.h> are copied here
  * for local use of libuna
  */
 #else
 #include <byte_stream.h>
 
-#define LIBUNA_VERSION						20240130
+#define LIBUNA_VERSION						20240414
 
 /* The libuna version string
  */
-#define LIBUNA_VERSION_STRING					"20240130"
+#define LIBUNA_VERSION_STRING					"20240414"
 
 /* The endian definitions
  */
 #define	LIBUNA_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define	LIBUNA_ENDIAN_LITTLE					_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The codepage definitions
```

### Comparing `libvhdi-20240303/libuna/libuna_url_stream.h` & `libvhdi-20240509/libuna/libuna_url_stream.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_mac_icelandic.h` & `libvhdi-20240509/libuna/libuna_codepage_mac_icelandic.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_koi8_u.h` & `libvhdi-20240509/libuna/libuna_codepage_koi8_u.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_utf16_stream.c` & `libvhdi-20240509/libuna/libuna_utf16_stream.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_windows_1253.c` & `libvhdi-20240509/libuna/libuna_codepage_windows_1253.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_iso_8859_4.h` & `libvhdi-20240509/libuna/libuna_codepage_iso_8859_4.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_mac_greek.c` & `libvhdi-20240509/libuna/libuna_codepage_mac_greek.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_libcerror.h` & `libvhdi-20240509/libuna/libuna_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_mac_centraleurroman.c` & `libvhdi-20240509/libuna/libuna_codepage_mac_centraleurroman.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_windows_1254.c` & `libvhdi-20240509/libuna/libuna_codepage_windows_1254.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_iso_8859_13.h` & `libvhdi-20240509/libuna/libuna_codepage_iso_8859_13.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_iso_8859_7.h` & `libvhdi-20240509/libuna/libuna_codepage_iso_8859_7.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_windows_1255.h` & `libvhdi-20240509/libuna/libuna_codepage_windows_1255.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_unicode_character.h` & `libvhdi-20240509/libuna/libuna_unicode_character.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_iso_8859_8.h` & `libvhdi-20240509/libuna/libuna_codepage_iso_8859_8.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_iso_8859_13.c` & `libvhdi-20240509/libuna/libuna_codepage_iso_8859_13.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_windows_949.h` & `libvhdi-20240509/libuna/libuna_codepage_windows_949.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_mac_cyrillic.c` & `libvhdi-20240509/libuna/libuna_codepage_mac_cyrillic.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_mac_celtic.c` & `libvhdi-20240509/libuna/libuna_codepage_mac_celtic.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_support.h` & `libvhdi-20240509/libuna/libuna_support.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_iso_8859_4.c` & `libvhdi-20240509/libuna/libuna_codepage_iso_8859_4.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_windows_949.c` & `libvhdi-20240509/libuna/libuna_codepage_windows_949.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_utf16_stream.h` & `libvhdi-20240509/libuna/libuna_utf16_stream.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_mac_symbol.c` & `libvhdi-20240509/libuna/libuna_codepage_mac_symbol.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_mac_roman.h` & `libvhdi-20240509/libuna/libuna_codepage_mac_roman.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_windows_1257.c` & `libvhdi-20240509/libuna/libuna_codepage_windows_1257.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_windows_1254.h` & `libvhdi-20240509/libuna/libuna_codepage_windows_1254.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_windows_950.c` & `libvhdi-20240509/libuna/libuna_codepage_windows_950.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_extern.h` & `libvhdi-20240509/libuna/libuna_extern.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_windows_1256.c` & `libvhdi-20240509/libuna/libuna_codepage_windows_1256.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_types.h` & `libvhdi-20240509/libuna/libuna_types.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_base32_stream.h` & `libvhdi-20240509/libuna/libuna_base32_stream.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_windows_1253.h` & `libvhdi-20240509/libuna/libuna_codepage_windows_1253.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_iso_8859_16.h` & `libvhdi-20240509/libuna/libuna_codepage_iso_8859_16.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_utf8_stream.c` & `libvhdi-20240509/libuna/libuna_utf8_stream.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_windows_1250.h` & `libvhdi-20240509/libuna/libuna_codepage_windows_1250.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_iso_8859_2.c` & `libvhdi-20240509/libuna/libuna_codepage_iso_8859_2.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_support.c` & `libvhdi-20240509/libuna/libuna_support.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_koi8_r.c` & `libvhdi-20240509/libuna/libuna_codepage_koi8_r.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_iso_8859_5.h` & `libvhdi-20240509/libuna/libuna_codepage_iso_8859_5.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_utf16_string.h` & `libvhdi-20240509/libuna/libuna_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_utf32_string.c` & `libvhdi-20240509/libuna/libuna_utf32_string.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_mac_icelandic.c` & `libvhdi-20240509/libuna/libuna_codepage_mac_icelandic.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_windows_1256.h` & `libvhdi-20240509/libuna/libuna_codepage_windows_1256.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_utf32_string.h` & `libvhdi-20240509/libuna/libuna_utf32_string.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_mac_romanian.h` & `libvhdi-20240509/libuna/libuna_codepage_mac_romanian.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_iso_8859_8.c` & `libvhdi-20240509/libuna/libuna_codepage_iso_8859_8.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_koi8_r.h` & `libvhdi-20240509/libuna/libuna_codepage_koi8_r.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_mac_cyrillic.h` & `libvhdi-20240509/libuna/libuna_codepage_mac_cyrillic.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_mac_arabic.c` & `libvhdi-20240509/libuna/libuna_codepage_mac_arabic.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_mac_croatian.c` & `libvhdi-20240509/libuna/libuna_codepage_mac_croatian.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_iso_8859_9.h` & `libvhdi-20240509/libuna/libuna_codepage_iso_8859_9.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_mac_greek.h` & `libvhdi-20240509/libuna/libuna_codepage_mac_greek.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_windows_1258.h` & `libvhdi-20240509/libuna/libuna_codepage_windows_1258.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_iso_8859_7.c` & `libvhdi-20240509/libuna/libuna_codepage_iso_8859_7.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/Makefile.in` & `libvhdi-20240509/libuna/Makefile.in`

 * *Files 6% similar despite different names*

```diff
@@ -618,14 +618,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -680,16 +682,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBUNA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBUNA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBUNA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBUNA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBUNA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBUNA_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBUNA_TRUE@noinst_LTLIBRARIES = libuna.la
 @HAVE_LOCAL_LIBUNA_TRUE@libuna_la_SOURCES = \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base16_stream.c libuna_base16_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base32_stream.c libuna_base32_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base64_stream.c libuna_base64_stream.h \
@@ -755,15 +757,16 @@
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf16_string.c libuna_utf16_string.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf32_stream.c libuna_utf32_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf32_string.c libuna_utf32_string.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf7_stream.c libuna_utf7_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf8_stream.c libuna_utf8_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf8_string.c libuna_utf8_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -1025,24 +1028,89 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libuna_base16_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_base32_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_base64_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_byte_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_10.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_13.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_14.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_15.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_16.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_2.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_3.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_4.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_5.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_6.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_7.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_8.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_9.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_koi8_r.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_koi8_u.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_arabic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_celtic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_centraleurroman.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_croatian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_cyrillic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_dingbats.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_farsi.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_gaelic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_greek.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_icelandic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_inuit.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_roman.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_romanian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_russian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_symbol.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_thai.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_turkish.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_ukrainian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1250.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1251.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1252.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1253.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1254.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1255.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1256.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1257.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1258.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_874.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_932.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_936.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_949.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_950.Plo
+	-rm -f ./$(DEPDIR)/libuna_error.Plo
+	-rm -f ./$(DEPDIR)/libuna_scsu.Plo
+	-rm -f ./$(DEPDIR)/libuna_support.Plo
+	-rm -f ./$(DEPDIR)/libuna_unicode_character.Plo
+	-rm -f ./$(DEPDIR)/libuna_url_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf16_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf16_string.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf32_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf32_string.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf7_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf8_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf8_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1188,17 +1256,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libuna ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libuna_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvhdi-20240303/libuna/libuna_codepage_iso_8859_3.c` & `libvhdi-20240509/libuna/libuna_codepage_iso_8859_3.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_windows_1250.c` & `libvhdi-20240509/libuna/libuna_codepage_windows_1250.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_scsu.c` & `libvhdi-20240509/libuna/libuna_scsu.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_windows_1252.c` & `libvhdi-20240509/libuna/libuna_codepage_windows_1252.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_mac_turkish.c` & `libvhdi-20240509/libuna/libuna_codepage_mac_turkish.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_mac_ukrainian.h` & `libvhdi-20240509/libuna/libuna_codepage_mac_ukrainian.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_mac_russian.c` & `libvhdi-20240509/libuna/libuna_codepage_mac_russian.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_windows_1258.c` & `libvhdi-20240509/libuna/libuna_codepage_windows_1258.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_mac_celtic.h` & `libvhdi-20240509/libuna/libuna_codepage_mac_celtic.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_byte_stream.c` & `libvhdi-20240509/libuna/libuna_byte_stream.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_mac_gaelic.h` & `libvhdi-20240509/libuna/libuna_codepage_mac_gaelic.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_utf32_stream.h` & `libvhdi-20240509/libuna/libuna_utf32_stream.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_mac_symbol.h` & `libvhdi-20240509/libuna/libuna_codepage_mac_symbol.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_windows_1257.h` & `libvhdi-20240509/libuna/libuna_codepage_windows_1257.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_mac_inuit.h` & `libvhdi-20240509/libuna/libuna_codepage_mac_inuit.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_mac_farsi.c` & `libvhdi-20240509/libuna/libuna_codepage_mac_farsi.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_windows_950.h` & `libvhdi-20240509/libuna/libuna_codepage_windows_950.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_url_stream.c` & `libvhdi-20240509/libuna/libuna_url_stream.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_windows_1251.h` & `libvhdi-20240509/libuna/libuna_codepage_windows_1251.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_windows_1252.h` & `libvhdi-20240509/libuna/libuna_codepage_windows_1252.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_codepage_iso_8859_14.h` & `libvhdi-20240509/libuna/libuna_codepage_iso_8859_14.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_base16_stream.h` & `libvhdi-20240509/libuna/libuna_base16_stream.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libuna/libuna_base32_stream.c` & `libvhdi-20240509/libuna/libuna_base32_stream.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/Makefile.in` & `libvhdi-20240509/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -500,14 +500,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -624,16 +626,23 @@
 EXTRA_DIST = \
 	$(DPKG_FILES) \
 	$(GETTEXT_FILES) \
 	$(PKGCONFIG_FILES) \
 	$(SETUP_PY_FILES) \
 	$(SPEC_FILES)
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	config.status \
+	config.cache \
+	config.log \
+	libvhdi.pc \
+	libvhdi.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 pkgconfig_DATA = \
 	libvhdi.pc
 
 all: all-recursive
 
@@ -1050,23 +1059,26 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-recursive
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-recursive
+	-rm -f $(am__CONFIG_DISTCLEAN_FILES)
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-libtool \
 	distclean-tags
 
 dvi: dvi-recursive
 
 dvi-am:
 
@@ -1177,22 +1189,10 @@
 	(cd $(srcdir)/libbfio && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfcache && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfdata && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfguid && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libvhdi && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libvhdi.pc
-	-rm -f libvhdi.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libvhdi-20240303/libcnotify/libcnotify_definitions.h` & `libvhdi-20240509/libcnotify/libcnotify_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcnotify/definitions.h>
 
 /* The definitions in <libcnotify/definitions.h> are copied here
  * for local use of libcnotify
  */
 #else
 
-#define LIBCNOTIFY_VERSION				20240108
+#define LIBCNOTIFY_VERSION				20240414
 
 /* The libcnotify version string
  */
-#define LIBCNOTIFY_VERSION_STRING			"20240108"
+#define LIBCNOTIFY_VERSION_STRING			"20240414"
 
 /* The print data flags
  */
 enum LIBCNOTIFY_NOTIFY_PRINT_DATA_FLAGS
 {
 	LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA		= 0x01,
 };
```

### Comparing `libvhdi-20240303/libcnotify/libcnotify_extern.h` & `libvhdi-20240509/libcnotify/libcnotify_extern.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcnotify/libcnotify_support.c` & `libvhdi-20240509/libcnotify/libcnotify_support.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcnotify/libcnotify_stream.h` & `libvhdi-20240509/libcnotify/libcnotify_stream.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcnotify/Makefile.am` & `libvhdi-20240509/libcnotify/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCNOTIFY
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcnotify.la
 
 libcnotify_la_SOURCES = \
 	libcnotify_definitions.h \
 	libcnotify_extern.h \
@@ -13,19 +13,17 @@
 	libcnotify_print.c libcnotify_print.h \
 	libcnotify_stream.c libcnotify_stream.h \
 	libcnotify_support.c libcnotify_support.h \
 	libcnotify_unused.h \
 	libcnotify_verbose.c libcnotify_verbose.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcnotify ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcnotify_la_SOURCES)
```

### Comparing `libvhdi-20240303/libcnotify/libcnotify_unused.h` & `libvhdi-20240509/libcnotify/libcnotify_unused.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcnotify/libcnotify_verbose.h` & `libvhdi-20240509/libcnotify/libcnotify_verbose.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcnotify/libcnotify_print.h` & `libvhdi-20240509/libcnotify/libcnotify_print.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcnotify/libcnotify_stream.c` & `libvhdi-20240509/libcnotify/libcnotify_stream.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcnotify/libcnotify_support.h` & `libvhdi-20240509/libcnotify/libcnotify_support.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcnotify/libcnotify_verbose.c` & `libvhdi-20240509/libcnotify/libcnotify_verbose.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcnotify/Makefile.in` & `libvhdi-20240509/libcnotify/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -442,14 +442,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -504,30 +506,31 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@noinst_LTLIBRARIES = libcnotify.la
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@libcnotify_la_SOURCES = \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_definitions.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_extern.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_libcerror.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_print.c libcnotify_print.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_stream.c libcnotify_stream.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_support.c libcnotify_support.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_unused.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_verbose.c libcnotify_verbose.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -730,24 +733,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcnotify_print.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_stream.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_support.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_verbose.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -834,17 +843,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcnotify ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcnotify_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvhdi-20240303/libcnotify/libcnotify_libcerror.h` & `libvhdi-20240509/libcnotify/libcnotify_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcnotify/libcnotify_print.c` & `libvhdi-20240509/libcnotify/libcnotify_print.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcerror/libcerror_system.c` & `libvhdi-20240509/libcerror/libcerror_system.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcerror/libcerror_error.c` & `libvhdi-20240509/libcerror/libcerror_error.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcerror/libcerror_extern.h` & `libvhdi-20240509/libcerror/libcerror_extern.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcerror/Makefile.am` & `libvhdi-20240509/libcerror/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 if HAVE_LOCAL_LIBCERROR
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common 
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common 
 
 noinst_LTLIBRARIES = libcerror.la
 
 libcerror_la_SOURCES = \
 	libcerror_definitions.h \
 	libcerror_extern.h \
 	libcerror_error.c libcerror_error.h \
 	libcerror_support.c libcerror_support.h \
 	libcerror_system.c libcerror_system.h \
 	libcerror_types.h \
 	libcerror_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcerror ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcerror_la_SOURCES)
```

### Comparing `libvhdi-20240303/libcerror/libcerror_types.h` & `libvhdi-20240509/libcerror/libcerror_types.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcerror/libcerror_support.h` & `libvhdi-20240509/libcerror/libcerror_support.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcerror/libcerror_error.h` & `libvhdi-20240509/libcerror/libcerror_error.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcerror/libcerror_system.h` & `libvhdi-20240509/libcerror/libcerror_system.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcerror/libcerror_definitions.h` & `libvhdi-20240509/libcerror/libcerror_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcerror/definitions.h>
 
 /* The definitions in <libcerror/definitions.h> are copied here
  * for local use of libcerror
  */
 #else
 
-#define LIBCERROR_VERSION				20240101
+#define LIBCERROR_VERSION				20240413
 
 /* The libcerror version string
  */
-#define LIBCERROR_VERSION_STRING			"20240101"
+#define LIBCERROR_VERSION_STRING			"20240413"
 
 /* The error domains
  */
 enum LIBCERROR_ERROR_DOMAINS
 {
 	LIBCERROR_ERROR_DOMAIN_ARGUMENTS		= (int) 'a',
 	LIBCERROR_ERROR_DOMAIN_CONVERSION		= (int) 'c',
```

### Comparing `libvhdi-20240303/libcerror/libcerror_support.c` & `libvhdi-20240509/libcerror/libcerror_support.c`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcerror/libcerror_unused.h` & `libvhdi-20240509/libcerror/libcerror_unused.h`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/libcerror/Makefile.in` & `libvhdi-20240509/libcerror/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -439,14 +439,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -501,28 +503,29 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCERROR_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCERROR_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCERROR_TRUE@	-I$(top_srcdir)/common 
+@HAVE_LOCAL_LIBCERROR_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCERROR_TRUE@	-I../common -I$(top_srcdir)/common 
 
 @HAVE_LOCAL_LIBCERROR_TRUE@noinst_LTLIBRARIES = libcerror.la
 @HAVE_LOCAL_LIBCERROR_TRUE@libcerror_la_SOURCES = \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_definitions.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_extern.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_error.c libcerror_error.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_support.c libcerror_support.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_system.c libcerror_system.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_types.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -724,24 +727,29 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcerror_error.Plo
+	-rm -f ./$(DEPDIR)/libcerror_support.Plo
+	-rm -f ./$(DEPDIR)/libcerror_system.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -827,17 +835,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcerror ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcerror_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvhdi-20240303/aclocal.m4` & `libvhdi-20240509/aclocal.m4`

 * *Files identical despite different names*

### Comparing `libvhdi-20240303/configure.ac` & `libvhdi-20240509/configure.ac`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AC_PREREQ([2.71])
 
 AC_INIT(
  [libvhdi],
- [20240303],
+ [20240509],
  [joachim.metz@gmail.com])
 
 AC_CONFIG_SRCDIR(
  [include/libvhdi.h.in])
 
 AM_INIT_AUTOMAKE([gnu 1.6 tar-ustar])
 AM_EXTRA_RECURSIVE_TARGETS([sources splint])
```

