# Comparing `tmp/deflate-0.6.1.tar.gz` & `tmp/deflate-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deflate-0.6.1.tar", last modified: Tue May  7 01:23:30 2024, max compression
+gzip compressed data, was "deflate-0.7.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `deflate-0.6.1.tar` & `deflate-0.7.0.tar`

### file list

```diff
@@ -1,127 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:23:30.937849 deflate-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-07 01:23:28.000000 deflate-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-07 01:23:28.000000 deflate-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-05-07 01:23:30.937849 deflate-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-07 01:23:28.000000 deflate-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    11476 2024-05-07 01:23:28.000000 deflate-0.6.1/deflate.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:23:30.921849 deflate-0.6.1/deflate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-05-07 01:23:30.000000 deflate-0.6.1/deflate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-05-07 01:23:30.000000 deflate-0.6.1/deflate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 01:23:30.000000 deflate-0.6.1/deflate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 01:23:30.000000 deflate-0.6.1/deflate.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:23:30.925849 deflate-0.6.1/libdeflate/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/.cirrus.yml
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-07 01:23:28.000000 deflate-0.6.1/libdeflate/.git
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:23:30.921849 deflate-0.6.1/libdeflate/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:23:30.925849 deflate-0.6.1/libdeflate/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)    11369 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)    17355 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/NEWS.md
--rw-r--r--   0 runner    (1001) docker     (127)    10957 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    21710 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/common_defs.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:23:30.929849 deflate-0.6.1/libdeflate/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     5133 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/lib/adler32.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:23:30.929849 deflate-0.6.1/libdeflate/lib/arm/
--rw-r--r--   0 runner    (1001) docker     (127)    11677 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/lib/arm/adler32_impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/lib/arm/cpu_features.c
--rw-r--r--   0 runner    (1001) docker     (127)     7107 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/lib/arm/cpu_features.h
--rw-r--r--   0 runner    (1001) docker     (127)    20933 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/lib/arm/crc32_impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/lib/arm/crc32_pmull_helpers.h
--rw-r--r--   0 runner    (1001) docker     (127)     7401 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/lib/arm/crc32_pmull_wide.h
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/lib/arm/matchfinder_impl.h
--rw-r--r--   0 runner    (1001) docker     (127)    11499 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/lib/bt_matchfinder.h
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/lib/cpu_features_common.h
--rw-r--r--   0 runner    (1001) docker     (127)     9227 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/lib/crc32.c
--rw-r--r--   0 runner    (1001) docker     (127)    22006 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/lib/crc32_multipliers.h
--rw-r--r--   0 runner    (1001) docker     (127)    28471 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/lib/crc32_tables.h
--rw-r--r--   0 runner    (1001) docker     (127)    25048 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/lib/decompress_template.h
--rw-r--r--   0 runner    (1001) docker     (127)   138576 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/lib/deflate_compress.c
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/lib/deflate_compress.h
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/lib/deflate_constants.h
--rw-r--r--   0 runner    (1001) docker     (127)    49297 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/lib/deflate_decompress.c
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/lib/gzip_compress.c
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/lib/gzip_constants.h
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/lib/gzip_decompress.c
--rw-r--r--   0 runner    (1001) docker     (127)    13970 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/lib/hc_matchfinder.h
--rw-r--r--   0 runner    (1001) docker     (127)     7135 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/lib/ht_matchfinder.h
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/lib/lib_common.h
--rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/lib/matchfinder_common.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:23:30.929849 deflate-0.6.1/libdeflate/lib/riscv/
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/lib/riscv/matchfinder_impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/lib/utils.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:23:30.929849 deflate-0.6.1/libdeflate/lib/x86/
--rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/lib/x86/adler32_impl.h
--rw-r--r--   0 runner    (1001) docker     (127)    17524 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/lib/x86/adler32_template.h
--rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/lib/x86/cpu_features.c
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/lib/x86/cpu_features.h
--rw-r--r--   0 runner    (1001) docker     (127)     6178 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/lib/x86/crc32_impl.h
--rw-r--r--   0 runner    (1001) docker     (127)    16632 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/lib/x86/crc32_pclmul_template.h
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/lib/x86/decompress_impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/lib/x86/matchfinder_impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/lib/zlib_compress.c
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/lib/zlib_constants.h
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/lib/zlib_decompress.c
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/libdeflate-config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (127)    17098 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/libdeflate.h
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/libdeflate.pc.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:23:30.933849 deflate-0.6.1/libdeflate/programs/
--rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/programs/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    17356 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/programs/benchmark.c
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/programs/checksum.c
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/programs/config.h.in
--rw-r--r--   0 runner    (1001) docker     (127)    17688 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/programs/gzip.c
--rw-r--r--   0 runner    (1001) docker     (127)    11900 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/programs/prog_util.c
--rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/programs/prog_util.h
--rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/programs/test_checksums.c
--rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/programs/test_custom_malloc.c
--rw-r--r--   0 runner    (1001) docker     (127)    11890 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/programs/test_incomplete_codes.c
--rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/programs/test_invalid_streams.c
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/programs/test_litrunlen_overflow.c
--rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/programs/test_overread.c
--rw-r--r--   0 runner    (1001) docker     (127)    22742 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/programs/test_slow_decompression.c
--rw-r--r--   0 runner    (1001) docker     (127)     5181 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/programs/test_trailing_bytes.c
--rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/programs/test_util.c
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/programs/test_util.h
--rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/programs/tgetopt.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:23:30.933849 deflate-0.6.1/libdeflate/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2077 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/scripts/android_build.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1994 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/scripts/android_tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      247 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/scripts/benchmark.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      245 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/scripts/checksum.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     5237 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/scripts/checksum_benchmarks.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      471 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/scripts/cmake-helper.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     2425 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/scripts/deflate_benchmarks.sh
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/scripts/exec_tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1234 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/scripts/gen-release-archives.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      523 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/scripts/gen_bitreverse_tab.py
--rw-r--r--   0 runner    (1001) docker     (127)     7157 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/scripts/gen_crc32_multipliers.c
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/scripts/gen_crc32_tables.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     1273 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/scripts/gen_default_litlen_costs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      960 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/scripts/gen_offset_slot_map.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11897 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/scripts/gzip_tests.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:23:30.937849 deflate-0.6.1/libdeflate/scripts/libFuzzer/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/scripts/libFuzzer/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:23:30.937849 deflate-0.6.1/libdeflate/scripts/libFuzzer/deflate_compress/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:23:30.937849 deflate-0.6.1/libdeflate/scripts/libFuzzer/deflate_compress/corpus/
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/scripts/libFuzzer/deflate_compress/corpus/0
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/scripts/libFuzzer/deflate_compress/fuzz.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:23:30.937849 deflate-0.6.1/libdeflate/scripts/libFuzzer/deflate_decompress/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:23:30.937849 deflate-0.6.1/libdeflate/scripts/libFuzzer/deflate_decompress/corpus/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/scripts/libFuzzer/deflate_decompress/corpus/0
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/scripts/libFuzzer/deflate_decompress/fuzz.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     1772 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/scripts/libFuzzer/fuzz.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:23:30.937849 deflate-0.6.1/libdeflate/scripts/libFuzzer/gzip_decompress/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:23:30.937849 deflate-0.6.1/libdeflate/scripts/libFuzzer/gzip_decompress/corpus/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/scripts/libFuzzer/gzip_decompress/corpus/0
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/scripts/libFuzzer/gzip_decompress/fuzz.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:23:30.937849 deflate-0.6.1/libdeflate/scripts/libFuzzer/zlib_decompress/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:23:30.937849 deflate-0.6.1/libdeflate/scripts/libFuzzer/zlib_decompress/corpus/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/scripts/libFuzzer/zlib_decompress/corpus/0
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/scripts/libFuzzer/zlib_decompress/fuzz.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     9382 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/scripts/run_tests.sh
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/scripts/toolchain-i686-w64-mingw32.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-07 01:23:29.000000 deflate-0.6.1/libdeflate/scripts/toolchain-x86_64-w64-mingw32.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-07 01:23:30.937849 deflate-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-07 01:23:28.000000 deflate-0.6.1/setup.py
+-rw-r--r--   0        0        0       50 2022-11-09 12:37:21.000000 deflate-0.7.0/.clang-format
+-rw-r--r--   0        0        0      225 2022-11-09 12:37:21.000000 deflate-0.7.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1060 2022-11-09 12:37:21.000000 deflate-0.7.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      865 2022-11-09 12:37:21.000000 deflate-0.7.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0       97 2022-11-09 12:37:21.000000 deflate-0.7.0/.gitignore
+-rw-r--r--   0        0        0       90 2022-11-09 12:37:21.000000 deflate-0.7.0/.gitmodules
+-rw-r--r--   0        0        0      339 2022-11-09 12:37:21.000000 deflate-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       37 2022-11-09 12:37:21.000000 deflate-0.7.0/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2022-11-09 12:37:21.000000 deflate-0.7.0/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2022-11-09 12:37:21.000000 deflate-0.7.0/.pytest_cache/README.md
+-rw-r--r--   0        0        0     1206 2022-11-09 12:37:21.000000 deflate-0.7.0/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0    99510 2022-11-09 12:37:21.000000 deflate-0.7.0/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2022-11-09 12:37:21.000000 deflate-0.7.0/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        7 2022-11-09 12:37:21.000000 deflate-0.7.0/.python-version
+-rw-r--r--   0        0        0       35 2022-11-09 12:37:21.000000 deflate-0.7.0/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0      393 2022-11-09 12:37:21.000000 deflate-0.7.0/.ruff_cache/0.3.0/8413728815885562248
+-rw-r--r--   0        0        0      290 2022-11-09 12:37:21.000000 deflate-0.7.0/.ruff_cache/0.4.1/15537967479889239231
+-rw-r--r--   0        0        0      393 2022-11-09 12:37:21.000000 deflate-0.7.0/.ruff_cache/0.4.1/17758349274406298996
+-rw-r--r--   0        0        0      353 2022-11-09 12:37:21.000000 deflate-0.7.0/.ruff_cache/0.4.3/458006135455853641
+-rw-r--r--   0        0        0       43 2022-11-09 12:37:21.000000 deflate-0.7.0/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1763 2022-11-09 12:37:21.000000 deflate-0.7.0/CHANGELOG.md
+-rw-r--r--   0        0        0      929 2022-11-09 12:37:21.000000 deflate-0.7.0/CMakeLists.txt
+-rw-r--r--   0        0        0     1067 2022-11-09 12:37:21.000000 deflate-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1656 2022-11-09 12:37:21.000000 deflate-0.7.0/README.md
+-rw-r--r--   0        0        0      435 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/.cirrus.yml
+-rw-r--r--   0        0        0       35 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/.git
+-rw-r--r--   0        0        0    11369 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/.github/workflows/ci.yml
+-rw-r--r--   0        0        0       66 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/.gitignore
+-rw-r--r--   0        0        0    10739 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/CMakeLists.txt
+-rw-r--r--   0        0        0     1052 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/COPYING
+-rw-r--r--   0        0        0    17355 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/NEWS.md
+-rw-r--r--   0        0        0    10957 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/README.md
+-rw-r--r--   0        0        0    21710 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/common_defs.h
+-rw-r--r--   0        0        0     5133 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/lib/adler32.c
+-rw-r--r--   0        0        0    11677 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/lib/arm/adler32_impl.h
+-rw-r--r--   0        0        0     6329 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/lib/arm/cpu_features.c
+-rw-r--r--   0        0        0     7107 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/lib/arm/cpu_features.h
+-rw-r--r--   0        0        0    20933 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/lib/arm/crc32_impl.h
+-rw-r--r--   0        0        0     5329 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/lib/arm/crc32_pmull_helpers.h
+-rw-r--r--   0        0        0     7401 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/lib/arm/crc32_pmull_wide.h
+-rw-r--r--   0        0        0     2463 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/lib/arm/matchfinder_impl.h
+-rw-r--r--   0        0        0    11499 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/lib/bt_matchfinder.h
+-rw-r--r--   0        0        0     2788 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/lib/cpu_features_common.h
+-rw-r--r--   0        0        0     9227 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/lib/crc32.c
+-rw-r--r--   0        0        0    22006 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/lib/crc32_multipliers.h
+-rw-r--r--   0        0        0    28471 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/lib/crc32_tables.h
+-rw-r--r--   0        0        0    25048 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/lib/decompress_template.h
+-rw-r--r--   0        0        0   138576 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/lib/deflate_compress.c
+-rw-r--r--   0        0        0      398 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/lib/deflate_compress.h
+-rw-r--r--   0        0        0     1747 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/lib/deflate_constants.h
+-rw-r--r--   0        0        0    49297 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/lib/deflate_decompress.c
+-rw-r--r--   0        0        0     2665 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/lib/gzip_compress.c
+-rw-r--r--   0        0        0     1029 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/lib/gzip_constants.h
+-rw-r--r--   0        0        0     3996 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/lib/gzip_decompress.c
+-rw-r--r--   0        0        0    13970 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/lib/hc_matchfinder.h
+-rw-r--r--   0        0        0     7135 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/lib/ht_matchfinder.h
+-rw-r--r--   0        0        0     3624 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/lib/lib_common.h
+-rw-r--r--   0        0        0     7052 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/lib/matchfinder_common.h
+-rw-r--r--   0        0        0     3330 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/lib/riscv/matchfinder_impl.h
+-rw-r--r--   0        0        0     3425 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/lib/utils.c
+-rw-r--r--   0        0        0     4431 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/lib/x86/adler32_impl.h
+-rw-r--r--   0        0        0    17524 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/lib/x86/adler32_template.h
+-rw-r--r--   0        0        0     5388 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/lib/x86/cpu_features.c
+-rw-r--r--   0        0        0     5368 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/lib/x86/cpu_features.h
+-rw-r--r--   0        0        0     6178 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/lib/x86/crc32_impl.h
+-rw-r--r--   0        0        0    16632 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/lib/x86/crc32_pclmul_template.h
+-rw-r--r--   0        0        0     2190 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/lib/x86/decompress_impl.h
+-rw-r--r--   0        0        0     3726 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/lib/x86/matchfinder_impl.h
+-rw-r--r--   0        0        0     2618 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/lib/zlib_compress.c
+-rw-r--r--   0        0        0      488 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/lib/zlib_constants.h
+-rw-r--r--   0        0        0     3138 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/lib/zlib_decompress.c
+-rw-r--r--   0        0        0       78 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/libdeflate-config.cmake.in
+-rw-r--r--   0        0        0    17098 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/libdeflate.h
+-rw-r--r--   0        0        0      808 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/libdeflate.pc.in
+-rw-r--r--   0        0        0     4675 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/programs/CMakeLists.txt
+-rw-r--r--   0        0        0    17356 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/programs/benchmark.c
+-rw-r--r--   0        0        0     5033 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/programs/checksum.c
+-rw-r--r--   0        0        0      479 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/programs/config.h.in
+-rw-r--r--   0        0        0    17688 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/programs/gzip.c
+-rw-r--r--   0        0        0    11900 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/programs/prog_util.c
+-rw-r--r--   0        0        0     6662 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/programs/prog_util.h
+-rw-r--r--   0        0        0     5134 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/programs/test_checksums.c
+-rw-r--r--   0        0        0     3607 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/programs/test_custom_malloc.c
+-rw-r--r--   0        0        0    11890 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/programs/test_incomplete_codes.c
+-rw-r--r--   0        0        0     3913 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/programs/test_invalid_streams.c
+-rw-r--r--   0        0        0     2204 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/programs/test_litrunlen_overflow.c
+-rw-r--r--   0        0        0     2686 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/programs/test_overread.c
+-rw-r--r--   0        0        0    22742 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/programs/test_slow_decompression.c
+-rw-r--r--   0        0        0     5181 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/programs/test_trailing_bytes.c
+-rw-r--r--   0        0        0     5693 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/programs/test_util.c
+-rw-r--r--   0        0        0     2061 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/programs/test_util.h
+-rw-r--r--   0        0        0     3530 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/programs/tgetopt.c
+-rwxr-xr-x   0        0        0     2077 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/scripts/android_build.sh
+-rwxr-xr-x   0        0        0     1994 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/scripts/android_tests.sh
+-rwxr-xr-x   0        0        0      247 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/scripts/benchmark.sh
+-rwxr-xr-x   0        0        0      245 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/scripts/checksum.sh
+-rwxr-xr-x   0        0        0     5237 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/scripts/checksum_benchmarks.sh
+-rwxr-xr-x   0        0        0      471 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/scripts/cmake-helper.sh
+-rwxr-xr-x   0        0        0     2425 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/scripts/deflate_benchmarks.sh
+-rw-r--r--   0        0        0      686 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/scripts/exec_tests.sh
+-rwxr-xr-x   0        0        0     1234 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/scripts/gen-release-archives.sh
+-rwxr-xr-x   0        0        0      523 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/scripts/gen_bitreverse_tab.py
+-rw-r--r--   0        0        0     7157 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/scripts/gen_crc32_multipliers.c
+-rw-r--r--   0        0        0     3350 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/scripts/gen_crc32_tables.c
+-rwxr-xr-x   0        0        0     1273 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/scripts/gen_default_litlen_costs.py
+-rwxr-xr-x   0        0        0      960 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/scripts/gen_offset_slot_map.py
+-rwxr-xr-x   0        0        0    11897 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/scripts/gzip_tests.sh
+-rw-r--r--   0        0        0        7 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/scripts/libFuzzer/.gitignore
+-rw-r--r--   0        0        0      500 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/scripts/libFuzzer/deflate_compress/corpus/0
+-rw-r--r--   0        0        0     1208 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/scripts/libFuzzer/deflate_compress/fuzz.c
+-rw-r--r--   0        0        0      169 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/scripts/libFuzzer/deflate_decompress/corpus/0
+-rw-r--r--   0        0        0      451 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/scripts/libFuzzer/deflate_decompress/fuzz.c
+-rwxr-xr-x   0        0        0     1772 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/scripts/libFuzzer/fuzz.sh
+-rw-r--r--   0        0        0      187 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/scripts/libFuzzer/gzip_decompress/corpus/0
+-rw-r--r--   0        0        0      445 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/scripts/libFuzzer/gzip_decompress/fuzz.c
+-rw-r--r--   0        0        0      175 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/scripts/libFuzzer/zlib_decompress/corpus/0
+-rw-r--r--   0        0        0      445 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/scripts/libFuzzer/zlib_decompress/fuzz.c
+-rwxr-xr-x   0        0        0     9382 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/scripts/run_tests.sh
+-rw-r--r--   0        0        0      332 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/scripts/toolchain-i686-w64-mingw32.cmake
+-rw-r--r--   0        0        0      338 2022-11-09 12:37:21.000000 deflate-0.7.0/libdeflate/scripts/toolchain-x86_64-w64-mingw32.cmake
+-rw-r--r--   0        0        0     1542 2022-11-09 12:37:21.000000 deflate-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      672 2022-11-09 12:37:21.000000 deflate-0.7.0/requirements-dev.lock
+-rw-r--r--   0        0        0      207 2022-11-09 12:37:21.000000 deflate-0.7.0/requirements.lock
+-rw-r--r--   0        0        0     9439 2022-11-09 12:37:21.000000 deflate-0.7.0/src/deflate.c
+-rw-r--r--   0        0        0     1272 2022-11-09 12:37:21.000000 deflate-0.7.0/tests/test_adler32.py
+-rw-r--r--   0        0        0     2685 2022-11-09 12:37:21.000000 deflate-0.7.0/tests/test_compress.py
+-rw-r--r--   0        0        0     1218 2022-11-09 12:37:21.000000 deflate-0.7.0/tests/test_crc32.py
+-rw-r--r--   0        0        0     2658 2022-11-09 12:37:21.000000 deflate-0.7.0/PKG-INFO
```

### Comparing `deflate-0.6.1/LICENSE` & `deflate-0.7.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2020-2022 Dan Watson
+Copyright (c) 2020 Dan Watson
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `deflate-0.6.1/PKG-INFO` & `deflate-0.7.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,53 +1,50 @@
 Metadata-Version: 2.1
 Name: deflate
-Version: 0.6.1
+Version: 0.7.0
 Summary: Python wrapper for libdeflate.
-Home-page: https://github.com/dcwatson/deflate
-Author: Dan Watson
-Author-email: dcwatson@gmail.com
-License: MIT
-Platform: UNKNOWN
+Author-Email: Dan Watson <dcwatson@gmail.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Archiving :: Compression
+Project-URL: Homepage, https://github.com/dcwatson/deflate
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # deflate API
 
 This is a very thin Python wrapper Eric Biggers' excellent
 [libdeflate](https://github.com/ebiggers/libdeflate).
 
-Currently, it only handles:
+Currently, it handles:
 
 ## Compression and decompression of gzip data, with a very basic API
 
 ```python
 import deflate
 level = 6  # The default; may be 1-12 for libdeflate.
 compressed = deflate.gzip_compress(b"hello world!" * 1000, level)
 original = deflate.gzip_decompress(compressed)
 ```
 
 ## Compression and decompression of raw DEFLATE or zlib data
 
-The size of the decompressed file needs to be kept through additional logic. Ditto for checksums.
+The original size of the decompressed data needs to be kept through additional logic.
 
 ```python
 import deflate
 level = 6  # The default; may be 1-12 for libdeflate.
 data = b"hello world!" * 1000
 # DEFLATE
 compressed = deflate.deflate_compress(data, level)
@@ -61,46 +58,33 @@
 
 ```python
 import deflate
 crc32 = deflate.crc32(b"hello world! ")  # initial
 crc32 = deflate.crc32(b"hello universe!", crc32)  # continued
 ```
 
-
 ## Adler-32 computation
 
 ```python
 import deflate
 adler32 = deflate.adler32(b"hello world! ")  # initial
 adler32 = deflate.adler32(b"hello universe!", adler32)  # continued
 ```
 
 # Installation
 
-Installing `deflate` will either link to or compile `libdeflate`, depending on the
-following:
-
-1. If a `LIBDEFLATE_PREFIX` environment variable is set, it will always be used to look
-   for a system-installed `libdeflate`.
-2. If the `pkgconfig` package is installed, it will be used to automatically find (and
-   link to) a system-installed `libdeflate` if available.
-3. Falls back to compiling the bundled libdeflate code. This behavior can be triggered
-   manually by setting `USE_BUNDLED_DEFLATE=1`.
+`pip install deflate`
 
+By default, `deflate` will compile and statically link the bundled `libdeflate` when you
+build from source. To link to a system-installed `libdeflate`, set the
+`LIBDEFLATE_PREFIX` environment variable:
 
 ```
-export USE_BUNDLED_DEFLATE=no  # default is no
-export LIBDEFLATE_PREFIX=/path/to/lib/deflate  # default: no path given
-pip install pkgconfig  # optional, you also need pkg-config cli tool
-pip install deflate
+LIBDEFLATE_PREFIX=/opt/homebrew/Cellar/libdeflate/1.20 python -m build
 ```
 
-
 # Testing
 
 ```
-pip install pytest
-pip install pytest-benchmark
-pytest
+pip install -r requirements-dev.lock
+python -m pytest
 ```
-
-
```

### Comparing `deflate-0.6.1/README.md` & `deflate-0.7.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # deflate API
 
 This is a very thin Python wrapper Eric Biggers' excellent
 [libdeflate](https://github.com/ebiggers/libdeflate).
 
-Currently, it only handles:
+Currently, it handles:
 
 ## Compression and decompression of gzip data, with a very basic API
 
 ```python
 import deflate
 level = 6  # The default; may be 1-12 for libdeflate.
 compressed = deflate.gzip_compress(b"hello world!" * 1000, level)
 original = deflate.gzip_decompress(compressed)
 ```
 
 ## Compression and decompression of raw DEFLATE or zlib data
 
-The size of the decompressed file needs to be kept through additional logic. Ditto for checksums.
+The original size of the decompressed data needs to be kept through additional logic.
 
 ```python
 import deflate
 level = 6  # The default; may be 1-12 for libdeflate.
 data = b"hello world!" * 1000
 # DEFLATE
 compressed = deflate.deflate_compress(data, level)
@@ -34,44 +34,33 @@
 
 ```python
 import deflate
 crc32 = deflate.crc32(b"hello world! ")  # initial
 crc32 = deflate.crc32(b"hello universe!", crc32)  # continued
 ```
 
-
 ## Adler-32 computation
 
 ```python
 import deflate
 adler32 = deflate.adler32(b"hello world! ")  # initial
 adler32 = deflate.adler32(b"hello universe!", adler32)  # continued
 ```
 
 # Installation
 
-Installing `deflate` will either link to or compile `libdeflate`, depending on the
-following:
-
-1. If a `LIBDEFLATE_PREFIX` environment variable is set, it will always be used to look
-   for a system-installed `libdeflate`.
-2. If the `pkgconfig` package is installed, it will be used to automatically find (and
-   link to) a system-installed `libdeflate` if available.
-3. Falls back to compiling the bundled libdeflate code. This behavior can be triggered
-   manually by setting `USE_BUNDLED_DEFLATE=1`.
+`pip install deflate`
 
+By default, `deflate` will compile and statically link the bundled `libdeflate` when you
+build from source. To link to a system-installed `libdeflate`, set the
+`LIBDEFLATE_PREFIX` environment variable:
 
 ```
-export USE_BUNDLED_DEFLATE=no  # default is no
-export LIBDEFLATE_PREFIX=/path/to/lib/deflate  # default: no path given
-pip install pkgconfig  # optional, you also need pkg-config cli tool
-pip install deflate
+LIBDEFLATE_PREFIX=/opt/homebrew/Cellar/libdeflate/1.20 python -m build
 ```
 
-
 # Testing
 
 ```
-pip install pytest
-pip install pytest-benchmark
-pytest
+pip install -r requirements-dev.lock
+python -m pytest
 ```
```

### Comparing `deflate-0.6.1/deflate.c` & `deflate-0.7.0/src/deflate.c`

 * *Files 26% similar despite different names*

```diff
@@ -1,316 +1,248 @@
 #define PY_SSIZE_T_CLEAN
-#include "libdeflate.h"
+
+// Can't use this until 3.11, when Py_buffer was stabilized
+// Also _PyBytes_Resize is not public API (although it seems like it should be)
+// #define Py_LIMITED_API 0x030b00f0
 #include <Python.h>
 
-#define MODULE_VERSION "0.6.1"
+#include "libdeflate.h"
 
-static PyObject *DeflateError;
+#define MODULE_VERSION "0.7.0"
 
-static PyObject *deflate_gzip_compress(PyObject *self, PyObject *args,
-                                       PyObject *kwargs) {
-    static char *keywords[] = {"data", "compresslevel", NULL};
-    Py_buffer data;
-    int compression_level = 6;
+static PyObject *DeflateError;
 
-    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "y*|i", keywords, &data,
-                                     &compression_level)) {
-        return NULL;
-    }
+typedef size_t (*CompressFunc)(struct libdeflate_compressor *, const void *, size_t,
+                               void *, size_t);
+typedef enum libdeflate_result (*DecompressFunc)(struct libdeflate_decompressor *,
+                                                 const void *, size_t, void *, size_t,
+                                                 size_t *);
+typedef size_t (*BoundFunc)(struct libdeflate_compressor *, size_t);
 
+static PyObject *compress(Py_buffer *data, int compression_level,
+                          CompressFunc compressfunc, BoundFunc boundfunc) {
     if (compression_level < 1 || compression_level > 12) {
-        PyBuffer_Release(&data);
-        PyErr_SetString(PyExc_ValueError, "compresslevel must be between 1 and 12.");
+        PyErr_SetString(PyExc_ValueError, "compresslevel must be between 1 and 12");
         return NULL;
     }
 
     struct libdeflate_compressor *compressor =
         libdeflate_alloc_compressor(compression_level);
-    size_t bound = libdeflate_gzip_compress_bound(compressor, data.len);
+    size_t bound = (*boundfunc)(compressor, data->len);
 
     PyObject *bytes = PyBytes_FromStringAndSize(NULL, bound);
     if (bytes == NULL) {
         libdeflate_free_compressor(compressor);
-        PyBuffer_Release(&data);
         return PyErr_NoMemory();
     }
 
-    size_t compressed_size = libdeflate_gzip_compress(compressor, data.buf, data.len,
-                                                      PyBytes_AsString(bytes), bound);
+    size_t compressed_size = (*compressfunc)(compressor, data->buf, data->len,
+                                             PyBytes_AsString(bytes), bound);
     libdeflate_free_compressor(compressor);
-    PyBuffer_Release(&data);
 
     if (compressed_size == 0) {
-        Py_XDECREF(bytes);
-        PyErr_SetString(DeflateError, "Compression failed.");
+        Py_DecRef(bytes);
+        PyErr_SetString(DeflateError, "Compression failed");
         return NULL;
     }
 
-    _PyBytes_Resize(&bytes, compressed_size);
+    if (compressed_size != bound) {
+        _PyBytes_Resize(&bytes, compressed_size);
+    }
 
     return bytes;
 }
 
-static PyObject *deflate_gzip_decompress(PyObject *self, PyObject *args,
-                                         PyObject *kwargs) {
-    static char *keywords[] = {"data", NULL};
-    Py_buffer data;
-
-    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "y*", keywords, &data)) {
-        return NULL;
-    }
-
-    if (data.len < 6) {
-        PyErr_SetString(DeflateError, "Invalid gzip data.");
-        PyBuffer_Release(&data);
-        return NULL;
-    }
-
-    // Very basic gzip header check before we go allocating memory.
-    uint8_t *bytes = (uint8_t *)data.buf;
-    if (bytes[0] != 0x1F || bytes[1] != 0x8B) {
-        PyErr_SetString(DeflateError, "Invalid gzip data.");
-        PyBuffer_Release(&data);
-        return NULL;
+static PyObject *decompress(Py_buffer *data, unsigned int originalsize,
+                            DecompressFunc decompressfunc) {
+    // Nothing in, nothing out.
+    if (originalsize == 0) {
+        return PyBytes_FromStringAndSize(NULL, 0);
     }
 
-    // The last 4 bytes of a gzip archive are the original data size, in little
-    // endian.
-    bytes = (uint8_t *)data.buf + (data.len - 4);
-    uint32_t size =
-        (bytes[0] << 0) | (bytes[1] << 8) | (bytes[2] << 16) | (bytes[3] << 24);
-    // TODO: upper bound on decompression size?
-
-    PyObject *output = PyBytes_FromStringAndSize(NULL, size);
+    PyObject *output = PyBytes_FromStringAndSize(NULL, originalsize);
     if (output == NULL) {
-        PyBuffer_Release(&data);
         return PyErr_NoMemory();
     }
 
-    if (Py_REFCNT(output) != 1) {
-        // Immortal object (b"" for instance)
-        return output;
-    }
-
     size_t decompressed_size;
     struct libdeflate_decompressor *decompressor = libdeflate_alloc_decompressor();
     enum libdeflate_result result =
-        libdeflate_gzip_decompress(decompressor, data.buf, data.len,
-                                   PyBytes_AsString(output), size, &decompressed_size);
+        (*decompressfunc)(decompressor, data->buf, data->len, PyBytes_AsString(output),
+                          originalsize, &decompressed_size);
     libdeflate_free_decompressor(decompressor);
 
-    // Resize the bytes object to the decompressed size and release the input buffer.
-    _PyBytes_Resize(&output, decompressed_size);
-    PyBuffer_Release(&data);
-
     if (result != LIBDEFLATE_SUCCESS) {
-        Py_XDECREF(output);
-        PyErr_SetString(DeflateError, "Decompression failed.");
+        Py_DecRef(output);
+        PyErr_SetString(DeflateError, "Decompression failed");
         return NULL;
     }
 
+    if (decompressed_size != originalsize) {
+        _PyBytes_Resize(&output, decompressed_size);
+    }
+
     return output;
 }
 
-static PyObject *deflate_crc32(PyObject *self, PyObject *args) {
+/* GZIP */
+
+static int read_gzip_size(Py_buffer *data, unsigned int *outsize) {
+    uint8_t *bytes = (uint8_t *)data->buf;
+    if ((data->len < 6) || (bytes[0] != 0x1F || bytes[1] != 0x8B)) {
+        return -1;
+    }
+
+    // The last 4 bytes of a gzip archive are the original data size, in little endian.
+    bytes += (data->len - 4);
+    (*outsize) = ((uint32_t)bytes[0] << 0) | ((uint32_t)bytes[1] << 8) |
+                 ((uint32_t)bytes[2] << 16) | ((uint32_t)bytes[3] << 24);
+
+    return 0;
+}
+
+static PyObject *deflate_gzip_compress(PyObject *self, PyObject *args,
+                                       PyObject *kwargs) {
+    static char *keywords[] = {"data", "compresslevel", NULL};
     Py_buffer data;
-    unsigned int crc = 0;
+    int compression_level = 6;
 
-    if (!PyArg_ParseTuple(args, "y*|I", &data, &crc)) {
+    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "y*|i", keywords, &data,
+                                     &compression_level)) {
         return NULL;
     }
 
-    crc = libdeflate_crc32(crc, data.buf, data.len);
+    PyObject *obj = compress(&data, compression_level, libdeflate_gzip_compress,
+                             libdeflate_gzip_compress_bound);
     PyBuffer_Release(&data);
-
-    return Py_BuildValue("I", crc);
+    return obj;
 }
 
-static PyObject *deflate_adler32(PyObject *self, PyObject *args) {
+static PyObject *deflate_gzip_decompress(PyObject *self, PyObject *args,
+                                         PyObject *kwargs) {
+    static char *keywords[] = {"data", "originalsize", NULL};
     Py_buffer data;
-    unsigned int adler = 1;
+    unsigned int originalsize = 0;
 
-    if (!PyArg_ParseTuple(args, "y*|I", &data, &adler)) {
+    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "y*|I", keywords, &data,
+                                     &originalsize)) {
         return NULL;
     }
 
-    adler = libdeflate_adler32(adler, data.buf, data.len);
-    PyBuffer_Release(&data);
+    if (originalsize == 0) {
+        if (read_gzip_size(&data, &originalsize) != 0) {
+            PyBuffer_Release(&data);
+            PyErr_SetString(PyExc_ValueError, "Invalid gzip data");
+            return NULL;
+        }
+    }
 
-    return Py_BuildValue("I", adler);
+    PyObject *obj = decompress(&data, originalsize, libdeflate_gzip_decompress);
+    PyBuffer_Release(&data);
+    return obj;
 }
 
+/* DEFLATE */
+
 static PyObject *deflate_deflate_compress(PyObject *self, PyObject *args,
                                           PyObject *kwargs) {
     static char *keywords[] = {"data", "compresslevel", NULL};
     Py_buffer data;
     int compression_level = 6;
 
     if (!PyArg_ParseTupleAndKeywords(args, kwargs, "y*|i", keywords, &data,
                                      &compression_level)) {
         return NULL;
     }
 
-    if (compression_level < 1 || compression_level > 12) {
-        PyBuffer_Release(&data);
-        PyErr_SetString(PyExc_ValueError, "compresslevel must be between 1 and 12.");
-        return NULL;
-    }
-
-    struct libdeflate_compressor *compressor =
-        libdeflate_alloc_compressor(compression_level);
-    size_t bound = libdeflate_deflate_compress_bound(compressor, data.len);
-
-    PyObject *bytes = PyBytes_FromStringAndSize(NULL, bound);
-    if (bytes == NULL) {
-        libdeflate_free_compressor(compressor);
-        PyBuffer_Release(&data);
-        return PyErr_NoMemory();
-    }
-
-    size_t compressed_size = libdeflate_deflate_compress(
-        compressor, data.buf, data.len, PyBytes_AsString(bytes), bound);
-    libdeflate_free_compressor(compressor);
+    PyObject *obj = compress(&data, compression_level, libdeflate_deflate_compress,
+                             libdeflate_deflate_compress_bound);
     PyBuffer_Release(&data);
-
-    if (compressed_size == 0) {
-        Py_XDECREF(bytes);
-        PyErr_SetString(DeflateError, "Compression failed.");
-        return NULL;
-    }
-
-    _PyBytes_Resize(&bytes, compressed_size);
-
-    return bytes;
+    return obj;
 }
 
 static PyObject *deflate_deflate_decompress(PyObject *self, PyObject *args,
                                             PyObject *kwargs) {
     static char *keywords[] = {"data", "originalsize", NULL};
     Py_buffer data;
-    unsigned int size = 0;
+    unsigned int originalsize = 0;
 
-    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "y*I", keywords, &data, &size)) {
+    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "y*I", keywords, &data,
+                                     &originalsize)) {
         return NULL;
     }
 
-    PyObject *output = PyBytes_FromStringAndSize(NULL, size);
-    if (output == NULL) {
-        PyBuffer_Release(&data);
-        return PyErr_NoMemory();
-    }
-
-    if (Py_REFCNT(output) != 1) {
-        // Immortal object (b"" for instance)
-        return output;
-    }
-
-    size_t decompressed_size;
-    struct libdeflate_decompressor *decompressor = libdeflate_alloc_decompressor();
-    enum libdeflate_result result = libdeflate_deflate_decompress(
-        decompressor, data.buf, data.len, PyBytes_AsString(output), size,
-        &decompressed_size);
-    libdeflate_free_decompressor(decompressor);
-
-    // Resize the bytes object to the decompressed size and release the input buffer.
-    _PyBytes_Resize(&output, decompressed_size);
+    PyObject *obj = decompress(&data, originalsize, libdeflate_deflate_decompress);
     PyBuffer_Release(&data);
-
-    if (result != LIBDEFLATE_SUCCESS) {
-        Py_XDECREF(output);
-        PyErr_SetString(DeflateError, "Decompression failed.");
-        return NULL;
-    }
-
-    return output;
+    return obj;
 }
 
+/* ZLIB */
+
 static PyObject *deflate_zlib_compress(PyObject *self, PyObject *args,
                                        PyObject *kwargs) {
     static char *keywords[] = {"data", "compresslevel", NULL};
     Py_buffer data;
     int compression_level = 6;
 
     if (!PyArg_ParseTupleAndKeywords(args, kwargs, "y*|i", keywords, &data,
                                      &compression_level)) {
         return NULL;
     }
 
-    if (compression_level < 1 || compression_level > 12) {
-        PyBuffer_Release(&data);
-        PyErr_SetString(PyExc_ValueError, "compresslevel must be between 1 and 12.");
-        return NULL;
-    }
-
-    struct libdeflate_compressor *compressor =
-        libdeflate_alloc_compressor(compression_level);
-    size_t bound = libdeflate_zlib_compress_bound(compressor, data.len);
-
-    PyObject *bytes = PyBytes_FromStringAndSize(NULL, bound);
-    if (bytes == NULL) {
-        libdeflate_free_compressor(compressor);
-        PyBuffer_Release(&data);
-        return PyErr_NoMemory();
-    }
-
-    size_t compressed_size = libdeflate_zlib_compress(compressor, data.buf, data.len,
-                                                      PyBytes_AsString(bytes), bound);
-    libdeflate_free_compressor(compressor);
+    PyObject *obj = compress(&data, compression_level, libdeflate_zlib_compress,
+                             libdeflate_zlib_compress_bound);
     PyBuffer_Release(&data);
-
-    if (compressed_size == 0) {
-        Py_XDECREF(bytes);
-        PyErr_SetString(DeflateError, "Compression failed.");
-        return NULL;
-    }
-
-    _PyBytes_Resize(&bytes, compressed_size);
-
-    return bytes;
+    return obj;
 }
 
 static PyObject *deflate_zlib_decompress(PyObject *self, PyObject *args,
                                          PyObject *kwargs) {
     static char *keywords[] = {"data", "originalsize", NULL};
     Py_buffer data;
-    unsigned int size = 0;
+    unsigned int originalsize = 0;
 
-    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "y*I", keywords, &data, &size)) {
+    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "y*I", keywords, &data,
+                                     &originalsize)) {
         return NULL;
     }
 
-    PyObject *output = PyBytes_FromStringAndSize(NULL, size);
-    if (output == NULL) {
-        PyBuffer_Release(&data);
-        return PyErr_NoMemory();
-    }
+    PyObject *obj = decompress(&data, originalsize, libdeflate_zlib_decompress);
+    PyBuffer_Release(&data);
+    return obj;
+}
 
-    if (Py_REFCNT(output) != 1) {
-        // Immortal object (b"" for instance)
-        return output;
-    }
+/* CRC-32/Adler-32 */
 
-    size_t decompressed_size;
-    struct libdeflate_decompressor *decompressor = libdeflate_alloc_decompressor();
-    enum libdeflate_result result =
-        libdeflate_zlib_decompress(decompressor, data.buf, data.len,
-                                   PyBytes_AsString(output), size, &decompressed_size);
-    libdeflate_free_decompressor(decompressor);
+static PyObject *deflate_crc32(PyObject *self, PyObject *args) {
+    Py_buffer data;
+    unsigned int crc = 0;
 
-    // Resize the bytes object to the decompressed size and release the input buffer.
-    _PyBytes_Resize(&output, decompressed_size);
+    if (!PyArg_ParseTuple(args, "y*|I", &data, &crc)) {
+        return NULL;
+    }
+
+    crc = libdeflate_crc32(crc, data.buf, data.len);
     PyBuffer_Release(&data);
 
-    if (result != LIBDEFLATE_SUCCESS) {
-        Py_XDECREF(output);
-        PyErr_SetString(DeflateError, "Decompression failed.");
+    return Py_BuildValue("I", crc);
+}
+
+static PyObject *deflate_adler32(PyObject *self, PyObject *args) {
+    Py_buffer data;
+    unsigned int adler = 1;
+
+    if (!PyArg_ParseTuple(args, "y*|I", &data, &adler)) {
         return NULL;
     }
 
-    return output;
+    adler = libdeflate_adler32(adler, data.buf, data.len);
+    PyBuffer_Release(&data);
+
+    return Py_BuildValue("I", adler);
 }
 
 static PyMethodDef deflate_methods[] = {
     {"gzip_compress", (PyCFunction)deflate_gzip_compress, METH_VARARGS | METH_KEYWORDS,
      "Compress data using gzip."},
     {"gzip_decompress", (PyCFunction)deflate_gzip_decompress,
      METH_VARARGS | METH_KEYWORDS, "Decompress gzip data."},
@@ -338,12 +270,12 @@
     PyObject *module = PyModule_Create(&deflate_module);
     if (module == NULL)
         return NULL;
 
     PyModule_AddStringConstant(module, "__version__", MODULE_VERSION);
 
     DeflateError = PyErr_NewException("deflate.DeflateError", NULL, NULL);
-    Py_INCREF(DeflateError);
+    Py_IncRef(DeflateError);
     PyModule_AddObject(module, "DeflateError", DeflateError);
 
     return module;
 }
```

### Comparing `deflate-0.6.1/libdeflate/.github/workflows/ci.yml` & `deflate-0.7.0/libdeflate/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/CMakeLists.txt` & `deflate-0.7.0/libdeflate/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/COPYING` & `deflate-0.7.0/libdeflate/COPYING`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/NEWS.md` & `deflate-0.7.0/libdeflate/NEWS.md`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/README.md` & `deflate-0.7.0/libdeflate/README.md`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/common_defs.h` & `deflate-0.7.0/libdeflate/common_defs.h`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/lib/adler32.c` & `deflate-0.7.0/libdeflate/lib/adler32.c`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/lib/arm/adler32_impl.h` & `deflate-0.7.0/libdeflate/lib/arm/adler32_impl.h`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/lib/arm/cpu_features.c` & `deflate-0.7.0/libdeflate/lib/arm/cpu_features.c`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/lib/arm/cpu_features.h` & `deflate-0.7.0/libdeflate/lib/arm/cpu_features.h`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/lib/arm/crc32_impl.h` & `deflate-0.7.0/libdeflate/lib/arm/crc32_impl.h`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/lib/arm/crc32_pmull_helpers.h` & `deflate-0.7.0/libdeflate/lib/arm/crc32_pmull_helpers.h`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/lib/arm/crc32_pmull_wide.h` & `deflate-0.7.0/libdeflate/lib/arm/crc32_pmull_wide.h`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/lib/arm/matchfinder_impl.h` & `deflate-0.7.0/libdeflate/lib/arm/matchfinder_impl.h`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/lib/bt_matchfinder.h` & `deflate-0.7.0/libdeflate/lib/bt_matchfinder.h`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/lib/cpu_features_common.h` & `deflate-0.7.0/libdeflate/lib/cpu_features_common.h`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/lib/crc32.c` & `deflate-0.7.0/libdeflate/lib/crc32.c`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/lib/crc32_multipliers.h` & `deflate-0.7.0/libdeflate/lib/crc32_multipliers.h`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/lib/crc32_tables.h` & `deflate-0.7.0/libdeflate/lib/crc32_tables.h`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/lib/decompress_template.h` & `deflate-0.7.0/libdeflate/lib/decompress_template.h`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/lib/deflate_compress.c` & `deflate-0.7.0/libdeflate/lib/deflate_compress.c`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/lib/deflate_constants.h` & `deflate-0.7.0/libdeflate/lib/deflate_constants.h`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/lib/deflate_decompress.c` & `deflate-0.7.0/libdeflate/lib/deflate_decompress.c`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/lib/gzip_compress.c` & `deflate-0.7.0/libdeflate/lib/gzip_compress.c`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/lib/gzip_constants.h` & `deflate-0.7.0/libdeflate/lib/gzip_constants.h`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/lib/gzip_decompress.c` & `deflate-0.7.0/libdeflate/lib/gzip_decompress.c`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/lib/hc_matchfinder.h` & `deflate-0.7.0/libdeflate/lib/hc_matchfinder.h`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/lib/ht_matchfinder.h` & `deflate-0.7.0/libdeflate/lib/ht_matchfinder.h`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/lib/lib_common.h` & `deflate-0.7.0/libdeflate/lib/lib_common.h`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/lib/matchfinder_common.h` & `deflate-0.7.0/libdeflate/lib/matchfinder_common.h`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/lib/riscv/matchfinder_impl.h` & `deflate-0.7.0/libdeflate/lib/riscv/matchfinder_impl.h`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/lib/utils.c` & `deflate-0.7.0/libdeflate/lib/utils.c`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/lib/x86/adler32_impl.h` & `deflate-0.7.0/libdeflate/lib/x86/adler32_impl.h`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/lib/x86/adler32_template.h` & `deflate-0.7.0/libdeflate/lib/x86/adler32_template.h`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/lib/x86/cpu_features.c` & `deflate-0.7.0/libdeflate/lib/x86/cpu_features.c`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/lib/x86/cpu_features.h` & `deflate-0.7.0/libdeflate/lib/x86/cpu_features.h`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/lib/x86/crc32_impl.h` & `deflate-0.7.0/libdeflate/lib/x86/crc32_impl.h`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/lib/x86/crc32_pclmul_template.h` & `deflate-0.7.0/libdeflate/lib/x86/crc32_pclmul_template.h`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/lib/x86/decompress_impl.h` & `deflate-0.7.0/libdeflate/lib/x86/decompress_impl.h`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/lib/x86/matchfinder_impl.h` & `deflate-0.7.0/libdeflate/lib/x86/matchfinder_impl.h`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/lib/zlib_compress.c` & `deflate-0.7.0/libdeflate/lib/zlib_compress.c`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/lib/zlib_decompress.c` & `deflate-0.7.0/libdeflate/lib/zlib_decompress.c`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/libdeflate.h` & `deflate-0.7.0/libdeflate/libdeflate.h`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/libdeflate.pc.in` & `deflate-0.7.0/libdeflate/libdeflate.pc.in`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/programs/CMakeLists.txt` & `deflate-0.7.0/libdeflate/programs/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/programs/benchmark.c` & `deflate-0.7.0/libdeflate/programs/benchmark.c`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/programs/checksum.c` & `deflate-0.7.0/libdeflate/programs/checksum.c`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/programs/gzip.c` & `deflate-0.7.0/libdeflate/programs/gzip.c`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/programs/prog_util.c` & `deflate-0.7.0/libdeflate/programs/prog_util.c`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/programs/prog_util.h` & `deflate-0.7.0/libdeflate/programs/prog_util.h`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/programs/test_checksums.c` & `deflate-0.7.0/libdeflate/programs/test_checksums.c`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/programs/test_custom_malloc.c` & `deflate-0.7.0/libdeflate/programs/test_custom_malloc.c`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/programs/test_incomplete_codes.c` & `deflate-0.7.0/libdeflate/programs/test_incomplete_codes.c`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/programs/test_invalid_streams.c` & `deflate-0.7.0/libdeflate/programs/test_invalid_streams.c`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/programs/test_litrunlen_overflow.c` & `deflate-0.7.0/libdeflate/programs/test_litrunlen_overflow.c`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/programs/test_overread.c` & `deflate-0.7.0/libdeflate/programs/test_overread.c`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/programs/test_slow_decompression.c` & `deflate-0.7.0/libdeflate/programs/test_slow_decompression.c`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/programs/test_trailing_bytes.c` & `deflate-0.7.0/libdeflate/programs/test_trailing_bytes.c`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/programs/test_util.c` & `deflate-0.7.0/libdeflate/programs/test_util.c`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/programs/test_util.h` & `deflate-0.7.0/libdeflate/programs/test_util.h`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/programs/tgetopt.c` & `deflate-0.7.0/libdeflate/programs/tgetopt.c`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/scripts/android_build.sh` & `deflate-0.7.0/libdeflate/scripts/android_build.sh`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/scripts/android_tests.sh` & `deflate-0.7.0/libdeflate/scripts/android_tests.sh`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/scripts/checksum_benchmarks.sh` & `deflate-0.7.0/libdeflate/scripts/checksum_benchmarks.sh`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/scripts/deflate_benchmarks.sh` & `deflate-0.7.0/libdeflate/scripts/deflate_benchmarks.sh`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/scripts/exec_tests.sh` & `deflate-0.7.0/libdeflate/scripts/exec_tests.sh`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/scripts/gen-release-archives.sh` & `deflate-0.7.0/libdeflate/scripts/gen-release-archives.sh`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/scripts/gen_bitreverse_tab.py` & `deflate-0.7.0/libdeflate/scripts/gen_bitreverse_tab.py`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/scripts/gen_crc32_multipliers.c` & `deflate-0.7.0/libdeflate/scripts/gen_crc32_multipliers.c`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/scripts/gen_crc32_tables.c` & `deflate-0.7.0/libdeflate/scripts/gen_crc32_tables.c`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/scripts/gen_default_litlen_costs.py` & `deflate-0.7.0/libdeflate/scripts/gen_default_litlen_costs.py`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/scripts/gen_offset_slot_map.py` & `deflate-0.7.0/libdeflate/scripts/gen_offset_slot_map.py`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/scripts/gzip_tests.sh` & `deflate-0.7.0/libdeflate/scripts/gzip_tests.sh`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/scripts/libFuzzer/deflate_compress/fuzz.c` & `deflate-0.7.0/libdeflate/scripts/libFuzzer/deflate_compress/fuzz.c`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/scripts/libFuzzer/fuzz.sh` & `deflate-0.7.0/libdeflate/scripts/libFuzzer/fuzz.sh`

 * *Files identical despite different names*

### Comparing `deflate-0.6.1/libdeflate/scripts/run_tests.sh` & `deflate-0.7.0/libdeflate/scripts/run_tests.sh`

 * *Files identical despite different names*

