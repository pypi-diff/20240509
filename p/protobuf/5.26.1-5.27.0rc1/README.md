# Comparing `tmp/protobuf-5.26.1.tar.gz` & `tmp/protobuf-5.27.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/protobuf-5.26.1.tar", last modified: Wed Mar 27 18:00:33 2024, max compression
+gzip compressed data, was "dist/protobuf-5.27.0rc1.tar", last modified: Thu Apr 18 00:15:09 2024, max compression
```

## Comparing `protobuf-5.26.1.tar` & `protobuf-5.27.0rc1.tar`

### file list

```diff
@@ -1,286 +1,286 @@
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1732 2000-01-01 00:00:00.000000 protobuf-5.26.1/LICENSE
--rw-r--r--   0 bazel     (1000) bazel     (1003)       39 2000-01-01 00:00:00.000000 protobuf-5.26.1/MANIFEST.in
--rw-r--r--   0 bazel     (1000) bazel     (1003)      818 2024-03-27 18:00:33.000000 protobuf-5.26.1/PKG-INFO
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4624 2000-01-01 00:00:00.000000 protobuf-5.26.1/README.md
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/google/
--rw-r--r--   0 bazel     (1000) bazel     (1003)      150 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/__init__.py
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/google/protobuf/
--rw-r--r--   0 bazel     (1000) bazel     (1003)      346 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/__init__.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1479 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/any_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2899 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/api_pb2.py
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/google/protobuf/compiler/
--rw-r--r--   0 bazel     (1000) bazel     (1003)        0 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/compiler/__init__.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3539 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/compiler/plugin_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    52063 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/descriptor.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)        1 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/descriptor.upb.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)   430985 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/descriptor.upb.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    67645 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/descriptor.upb_minitable.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4556 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/descriptor.upb_minitable.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    65671 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/descriptor.upbdefs.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     9059 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/descriptor.upbdefs.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5444 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/descriptor_database.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)   330696 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/descriptor_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    48373 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/descriptor_pool.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1554 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/duration_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1421 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/empty_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1512 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/field_mask_pb2.py
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/google/protobuf/internal/
--rw-r--r--   0 bazel     (1000) bazel     (1003)      272 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/internal/__init__.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    14073 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/internal/_parameterized.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4787 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/internal/api_implementation.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4082 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/internal/builder.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    21722 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/internal/containers.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    37437 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/internal/decoder.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    27297 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/internal/encoder.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3462 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/internal/enum_type_wrapper.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     7225 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/internal/extension_dict.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    10416 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/internal/field_mask.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2008 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/internal/message_listener.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)      425 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/internal/python_edition_defaults.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    56576 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/internal/python_message.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4080 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/internal/testing_refleaks.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    15450 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/internal/type_checkers.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    20380 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/internal/well_known_types.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     7087 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/internal/wire_format.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    35233 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/json_format.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    12844 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/message.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     8271 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/message_factory.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4203 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/proto_builder.py
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/google/protobuf/pyext/
--rw-r--r--   0 bazel     (1000) bazel     (1003)        0 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/pyext/__init__.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1704 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/pyext/cpp_message.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2413 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/reflection.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     7787 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/service.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    10058 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/service_reflection.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1534 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/source_context_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2812 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/struct_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     6709 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/symbol_database.py
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/google/protobuf/testdata/
--rw-r--r--   0 bazel     (1000) bazel     (1003)        0 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/testdata/__init__.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3621 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/text_encoding.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    62691 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/text_format.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1563 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/timestamp_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5191 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/type_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3127 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/unknown_fields.py
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/google/protobuf/util/
--rw-r--r--   0 bazel     (1000) bazel     (1003)        0 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/util/__init__.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2786 2000-01-01 00:00:00.000000 protobuf-5.26.1/google/protobuf/wrappers_pb2.py
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/protobuf.egg-info/
--rw-r--r--   0 bazel     (1000) bazel     (1003)      818 2024-03-27 18:00:33.000000 protobuf-5.26.1/protobuf.egg-info/PKG-INFO
--rw-r--r--   0 bazel     (1000) bazel     (1003)     7232 2024-03-27 18:00:33.000000 protobuf-5.26.1/protobuf.egg-info/SOURCES.txt
--rw-r--r--   0 bazel     (1000) bazel     (1003)        1 2024-03-27 18:00:33.000000 protobuf-5.26.1/protobuf.egg-info/dependency_links.txt
--rw-r--r--   0 bazel     (1000) bazel     (1003)        7 2024-03-27 18:00:33.000000 protobuf-5.26.1/protobuf.egg-info/namespace_packages.txt
--rw-r--r--   0 bazel     (1000) bazel     (1003)        7 2024-03-27 18:00:33.000000 protobuf-5.26.1/protobuf.egg-info/top_level.txt
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/python/
--rw-r--r--   0 bazel     (1000) bazel     (1003)    14972 2000-01-01 00:00:00.000000 protobuf-5.26.1/python/convert.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1909 2000-01-01 00:00:00.000000 protobuf-5.26.1/python/convert.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    76030 2000-01-01 00:00:00.000000 protobuf-5.26.1/python/descriptor.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2572 2000-01-01 00:00:00.000000 protobuf-5.26.1/python/descriptor.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    27874 2000-01-01 00:00:00.000000 protobuf-5.26.1/python/descriptor_containers.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4157 2000-01-01 00:00:00.000000 protobuf-5.26.1/python/descriptor_containers.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    23336 2000-01-01 00:00:00.000000 protobuf-5.26.1/python/descriptor_pool.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)      936 2000-01-01 00:00:00.000000 protobuf-5.26.1/python/descriptor_pool.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     8703 2000-01-01 00:00:00.000000 protobuf-5.26.1/python/extension_dict.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)      530 2000-01-01 00:00:00.000000 protobuf-5.26.1/python/extension_dict.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    19273 2000-01-01 00:00:00.000000 protobuf-5.26.1/python/map.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1610 2000-01-01 00:00:00.000000 protobuf-5.26.1/python/map.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    71894 2000-01-01 00:00:00.000000 protobuf-5.26.1/python/message.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3875 2000-01-01 00:00:00.000000 protobuf-5.26.1/python/message.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    12674 2000-01-01 00:00:00.000000 protobuf-5.26.1/python/protobuf.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     8085 2000-01-01 00:00:00.000000 protobuf-5.26.1/python/protobuf.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1642 2000-01-01 00:00:00.000000 protobuf-5.26.1/python/python_api.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    29250 2000-01-01 00:00:00.000000 protobuf-5.26.1/python/repeated.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2087 2000-01-01 00:00:00.000000 protobuf-5.26.1/python/repeated.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    10792 2000-01-01 00:00:00.000000 protobuf-5.26.1/python/unknown_fields.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)      531 2000-01-01 00:00:00.000000 protobuf-5.26.1/python/unknown_fields.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)       38 2024-03-27 18:00:33.000000 protobuf-5.26.1/setup.cfg
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2462 2000-01-01 00:00:00.000000 protobuf-5.26.1/setup.py
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/upb/
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/upb/base/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3581 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/base/descriptor_constants.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/upb/base/internal/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1130 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/base/internal/endian.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)      873 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/base/internal/log2.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1747 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/base/status.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1359 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/base/status.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1597 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/base/string_view.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)      820 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/base/upcast.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1189 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/generated_code_support.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/upb/hash/
--rw-r--r--   0 bazel     (1000) bazel     (1003)    23982 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/hash/common.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5511 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/hash/common.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2868 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/hash/int_table.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4857 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/hash/str_table.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/upb/lex/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1140 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/lex/atoi.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)      991 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/lex/atoi.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1525 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/lex/round_trip.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1042 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/lex/round_trip.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2775 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/lex/strtod.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)      586 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/lex/strtod.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)      909 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/lex/unicode.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1737 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/lex/unicode.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/upb/mem/
--rw-r--r--   0 bazel     (1000) bazel     (1003)      699 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mem/alloc.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2278 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mem/alloc.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    17946 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mem/arena.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2693 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mem/arena.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/upb/mem/internal/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3444 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mem/internal/arena.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/upb/message/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1824 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/accessors.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)    19056 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/accessors.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2609 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/accessors_split64.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4229 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/array.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3013 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/array.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2397 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/array_split64.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1401 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/compare.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)      871 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/compare.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1151 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/compat.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1213 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/compat.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    12165 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/copy.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1884 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/copy.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/upb/message/internal/
--rw-r--r--   0 bazel     (1000) bazel     (1003)    13453 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/internal/accessors.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4866 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/internal/array.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2030 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/internal/extension.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2148 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/internal/extension.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4892 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/internal/map.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1405 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/internal/map_entry.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2829 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/internal/map_sorter.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1828 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/internal/message.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3053 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/internal/message.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1625 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/internal/tagged_ptr.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)      541 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/internal/types.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3731 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/map.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4316 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/map.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1687 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/map_gencode_util.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5108 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/map_sorter.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2426 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/message.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1364 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/message.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    14898 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/promote.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     6063 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/promote.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1647 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/tagged_ptr.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1261 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/message/value.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/upb/mini_descriptor/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4811 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_descriptor/build_enum.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1484 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_descriptor/build_enum.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    33903 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_descriptor/decode.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4982 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_descriptor/decode.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/upb/mini_descriptor/internal/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1291 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_descriptor/internal/base92.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1723 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_descriptor/internal/base92.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1686 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_descriptor/internal/decoder.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    12665 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_descriptor/internal/encode.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3631 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_descriptor/internal/encode.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1034 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_descriptor/internal/modifiers.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2169 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_descriptor/internal/wire_constants.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4545 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_descriptor/link.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3566 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_descriptor/link.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/upb/mini_table/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4176 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_table/compat.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1376 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_table/compat.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)      920 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_table/enum.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1421 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_table/extension.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2733 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_table/extension_registry.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3577 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_table/extension_registry.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2392 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_table/field.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1669 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_table/file.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/upb/mini_table/internal/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1715 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_table/internal/enum.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1732 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_table/internal/extension.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     7109 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_table/internal/field.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1920 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_table/internal/file.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)      882 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_table/internal/message.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5789 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_table/internal/message.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2622 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_table/internal/size_log2.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1424 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_table/internal/sub.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2146 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_table/message.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3184 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_table/message.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1331 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/mini_table/sub.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/upb/port/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3197 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/port/atomic.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    10253 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/port/def.inc
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1400 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/port/undef.inc
--rw-r--r--   0 bazel     (1000) bazel     (1003)      972 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/port/vsnprintf_compat.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/upb/reflection/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1620 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/common.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)      826 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    17888 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/def_pool.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3593 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/def_pool.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)      958 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/def_type.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1711 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/def_type.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)      926 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/desc_state.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)    10834 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/enum_def.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2356 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/enum_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2027 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/enum_reserved_range.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)      815 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/enum_reserved_range.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5271 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/enum_value_def.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1245 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/enum_value_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2778 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/extension_range.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1057 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/extension_range.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    32976 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/field_def.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3447 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/field_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    14538 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/file_def.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2159 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/file_def.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/upb/reflection/internal/
--rw-r--r--   0 bazel     (1000) bazel     (1003)    13068 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/internal/def_builder.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     6985 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/internal/def_builder.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2068 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/internal/def_pool.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1108 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/internal/desc_state.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1204 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/internal/enum_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1059 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/internal/enum_reserved_range.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1184 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/internal/enum_value_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1021 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/internal/extension_range.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2238 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/internal/field_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1120 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/internal/file_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1813 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/internal/message_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1038 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/internal/message_reserved_range.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1087 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/internal/method_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1286 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/internal/oneof_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1078 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/internal/service_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)      849 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/internal/strdup2.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)      796 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/internal/strdup2.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)      960 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/internal/upb_edition_defaults.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     7801 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/message.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3386 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/message.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    27264 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/message_def.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     6403 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/message_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1995 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/message_reserved_range.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)      836 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/message_reserved_range.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3812 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/method_def.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1372 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/method_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     7367 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/oneof_def.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1836 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/oneof_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4039 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/service_def.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1408 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/reflection/service_def.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/upb/text/
--rw-r--r--   0 bazel     (1000) bazel     (1003)    15311 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/text/encode.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1454 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/text/encode.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/upb/util/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     9750 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/util/compare.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1580 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/util/compare.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    23869 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/util/def_to_proto.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1737 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/util/def_to_proto.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     9941 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/util/required_fields.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2842 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/util/required_fields.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/upb/wire/
--rw-r--r--   0 bazel     (1000) bazel     (1003)    52609 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/wire/decode.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5658 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/wire/decode.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    21988 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/wire/encode.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2272 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/wire/encode.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)      724 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/wire/eps_copy_input_stream.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)    17122 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/wire/eps_copy_input_stream.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/upb/wire/internal/
--rw-r--r--   0 bazel     (1000) bazel     (1003)      716 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/wire/internal/constants.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    50837 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/wire/internal/decode_fast.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3998 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/wire/internal/decode_fast.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4286 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/wire/internal/decoder.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1662 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/wire/internal/reader.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1451 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/wire/reader.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     6697 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/wire/reader.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)      620 2000-01-01 00:00:00.000000 protobuf-5.26.1/upb/wire/types.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-03-27 18:00:33.000000 protobuf-5.26.1/utf8_range/
--rw-r--r--   0 bazel     (1000) bazel     (1003)    17939 2000-01-01 00:00:00.000000 protobuf-5.26.1/utf8_range/utf8_range.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)      540 2000-01-01 00:00:00.000000 protobuf-5.26.1/utf8_range/utf8_range.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-04-18 00:15:09.000000 protobuf-5.27.0rc1/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1732 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/LICENSE
+-rw-r--r--   0 bazel     (1000) bazel     (1003)       39 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/MANIFEST.in
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      821 2024-04-18 00:15:09.000000 protobuf-5.27.0rc1/PKG-INFO
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4624 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/README.md
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-04-18 00:15:09.000000 protobuf-5.27.0rc1/google/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      150 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/__init__.py
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-04-18 00:15:09.000000 protobuf-5.27.0rc1/google/protobuf/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      349 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/__init__.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1733 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/any_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3153 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/api_pb2.py
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-04-18 00:15:09.000000 protobuf-5.27.0rc1/google/protobuf/compiler/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)        0 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/compiler/__init__.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3805 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/compiler/plugin_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    52106 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/descriptor.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)        1 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/descriptor.upb.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)   442992 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/descriptor.upb.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    71806 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/descriptor.upb_minitable.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4640 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/descriptor.upb_minitable.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    68617 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/descriptor.upbdefs.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     9334 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/descriptor.upbdefs.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5444 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/descriptor_database.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)   341736 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/descriptor_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    48430 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/descriptor_pool.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1813 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/duration_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1677 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/empty_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1773 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/field_mask_pb2.py
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-04-18 00:15:09.000000 protobuf-5.27.0rc1/google/protobuf/internal/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      272 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/internal/__init__.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    14073 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/internal/_parameterized.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4787 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/internal/api_implementation.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4082 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/internal/builder.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    21722 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/internal/containers.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    36387 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/internal/decoder.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    27297 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/internal/encoder.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3462 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/internal/enum_type_wrapper.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     7225 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/internal/extension_dict.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    10416 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/internal/field_mask.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2008 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/internal/message_listener.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      434 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/internal/python_edition_defaults.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    55408 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/internal/python_message.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4080 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/internal/testing_refleaks.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    15450 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/internal/type_checkers.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    20402 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/internal/well_known_types.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     7087 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/internal/wire_format.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    37073 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/json_format.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    12844 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/message.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     8271 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/message_factory.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4203 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/proto_builder.py
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-04-18 00:15:09.000000 protobuf-5.27.0rc1/google/protobuf/pyext/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)        0 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/pyext/__init__.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1704 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/pyext/cpp_message.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2413 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/reflection.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3121 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/runtime_version.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     7787 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/service.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    10058 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/service_reflection.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1799 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/source_context_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3069 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/struct_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     6709 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/symbol_database.py
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-04-18 00:15:09.000000 protobuf-5.27.0rc1/google/protobuf/testdata/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)        0 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/testdata/__init__.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3621 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/text_encoding.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    63535 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/text_format.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1823 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/timestamp_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5446 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/type_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3127 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/unknown_fields.py
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-04-18 00:15:09.000000 protobuf-5.27.0rc1/google/protobuf/util/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)        0 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/util/__init__.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3045 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/google/protobuf/wrappers_pb2.py
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-04-18 00:15:09.000000 protobuf-5.27.0rc1/protobuf.egg-info/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      821 2024-04-18 00:15:09.000000 protobuf-5.27.0rc1/protobuf.egg-info/PKG-INFO
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     7279 2024-04-18 00:15:09.000000 protobuf-5.27.0rc1/protobuf.egg-info/SOURCES.txt
+-rw-r--r--   0 bazel     (1000) bazel     (1003)        1 2024-04-18 00:15:09.000000 protobuf-5.27.0rc1/protobuf.egg-info/dependency_links.txt
+-rw-r--r--   0 bazel     (1000) bazel     (1003)        7 2024-04-18 00:15:09.000000 protobuf-5.27.0rc1/protobuf.egg-info/namespace_packages.txt
+-rw-r--r--   0 bazel     (1000) bazel     (1003)        7 2024-04-18 00:15:09.000000 protobuf-5.27.0rc1/protobuf.egg-info/top_level.txt
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-04-18 00:15:09.000000 protobuf-5.27.0rc1/python/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     9176 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/python/convert.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1577 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/python/convert.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    76511 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/python/descriptor.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2572 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/python/descriptor.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    27874 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/python/descriptor_containers.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4157 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/python/descriptor_containers.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    23481 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/python/descriptor_pool.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      936 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/python/descriptor_pool.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     8703 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/python/extension_dict.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      530 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/python/extension_dict.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    19451 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/python/map.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1610 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/python/map.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    72004 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/python/message.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3875 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/python/message.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    13415 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/python/protobuf.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     8434 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/python/protobuf.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1642 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/python/python_api.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    29318 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/python/repeated.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2087 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/python/repeated.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    10792 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/python/unknown_fields.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      531 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/python/unknown_fields.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)       38 2024-04-18 00:15:09.000000 protobuf-5.27.0rc1/setup.cfg
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2462 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/setup.py
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-04-18 00:15:09.000000 protobuf-5.27.0rc1/upb/
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-04-18 00:15:09.000000 protobuf-5.27.0rc1/upb/base/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3581 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/base/descriptor_constants.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-04-18 00:15:09.000000 protobuf-5.27.0rc1/upb/base/internal/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1130 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/base/internal/endian.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      873 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/base/internal/log2.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1747 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/base/status.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1359 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/base/status.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1597 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/base/string_view.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      820 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/base/upcast.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1189 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/generated_code_support.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-04-18 00:15:09.000000 protobuf-5.27.0rc1/upb/hash/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    23982 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/hash/common.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5511 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/hash/common.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2868 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/hash/int_table.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4857 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/hash/str_table.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-04-18 00:15:09.000000 protobuf-5.27.0rc1/upb/lex/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1140 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/lex/atoi.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      991 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/lex/atoi.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1525 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/lex/round_trip.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1042 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/lex/round_trip.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2775 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/lex/strtod.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      586 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/lex/strtod.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      909 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/lex/unicode.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1737 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/lex/unicode.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-04-18 00:15:09.000000 protobuf-5.27.0rc1/upb/mem/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      699 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/mem/alloc.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2278 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/mem/alloc.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    19954 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/mem/arena.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2937 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/mem/arena.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-04-18 00:15:09.000000 protobuf-5.27.0rc1/upb/mem/internal/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3515 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/mem/internal/arena.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-04-18 00:15:09.000000 protobuf-5.27.0rc1/upb/message/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1792 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/message/accessors.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    20096 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/message/accessors.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2609 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/message/accessors_split64.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4931 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/message/array.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3488 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/message/array.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     8478 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/message/compare.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2403 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/message/compare.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1145 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/message/compat.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1172 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/message/compat.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    12129 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/message/copy.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1884 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/message/copy.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-04-18 00:15:09.000000 protobuf-5.27.0rc1/upb/message/internal/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    14018 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/message/internal/accessors.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5116 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/message/internal/array.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     9532 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/message/internal/compare_unknown.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1504 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/message/internal/compare_unknown.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2012 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/message/internal/extension.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2052 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/message/internal/extension.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5263 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/message/internal/map.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1405 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/message/internal/map_entry.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2779 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/message/internal/map_sorter.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2510 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/message/internal/message.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3450 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/message/internal/message.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1577 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/message/internal/tagged_ptr.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1507 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/message/internal/types.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4430 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/message/map.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4524 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/message/map.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1687 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/message/map_gencode_util.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5108 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/message/map_sorter.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5135 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/message/message.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2163 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/message/message.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    14857 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/message/promote.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     6050 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/message/promote.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1522 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/message/tagged_ptr.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1261 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/message/value.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-04-18 00:15:09.000000 protobuf-5.27.0rc1/upb/mini_descriptor/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4796 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/mini_descriptor/build_enum.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1003 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/mini_descriptor/build_enum.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    34378 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/mini_descriptor/decode.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4982 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/mini_descriptor/decode.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-04-18 00:15:09.000000 protobuf-5.27.0rc1/upb/mini_descriptor/internal/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1291 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/mini_descriptor/internal/base92.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1723 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/mini_descriptor/internal/base92.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1686 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/mini_descriptor/internal/decoder.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    12665 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/mini_descriptor/internal/encode.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3631 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/mini_descriptor/internal/encode.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1034 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/mini_descriptor/internal/modifiers.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2169 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/mini_descriptor/internal/wire_constants.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4577 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/mini_descriptor/link.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3566 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/mini_descriptor/link.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-04-18 00:15:09.000000 protobuf-5.27.0rc1/upb/mini_table/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4176 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/mini_table/compat.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1376 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/mini_table/compat.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      864 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/mini_table/enum.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1172 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/mini_table/extension.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2733 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/mini_table/extension_registry.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3577 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/mini_table/extension_registry.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1684 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/mini_table/field.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1306 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/mini_table/file.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-04-18 00:15:09.000000 protobuf-5.27.0rc1/upb/mini_table/internal/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1705 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/mini_table/internal/enum.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1692 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/mini_table/internal/extension.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     6893 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/mini_table/internal/field.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1860 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/mini_table/internal/file.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      882 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/mini_table/internal/message.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     6491 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/mini_table/internal/message.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2622 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/mini_table/internal/size_log2.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1384 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/mini_table/internal/sub.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2146 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/mini_table/message.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3040 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/mini_table/message.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1094 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/mini_table/sub.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-04-18 00:15:09.000000 protobuf-5.27.0rc1/upb/port/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3197 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/port/atomic.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    10400 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/port/def.inc
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1398 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/port/undef.inc
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      972 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/port/vsnprintf_compat.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-04-18 00:15:09.000000 protobuf-5.27.0rc1/upb/reflection/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1620 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/common.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      826 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    17888 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/def_pool.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3552 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/def_pool.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      958 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/def_type.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1711 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/def_type.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      926 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/desc_state.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    10941 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/enum_def.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2416 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/enum_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2027 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/enum_reserved_range.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      815 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/enum_reserved_range.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5148 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/enum_value_def.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1245 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/enum_value_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2778 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/extension_range.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1057 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/extension_range.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    34466 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/field_def.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3591 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/field_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    15603 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/file_def.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2289 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/file_def.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-04-18 00:15:09.000000 protobuf-5.27.0rc1/upb/reflection/internal/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    13068 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/internal/def_builder.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     6985 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/internal/def_builder.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2068 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/internal/def_pool.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1108 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/internal/desc_state.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1204 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/internal/enum_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1059 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/internal/enum_reserved_range.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1184 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/internal/enum_value_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1021 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/internal/extension_range.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2238 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/internal/field_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1120 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/internal/file_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1813 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/internal/message_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1038 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/internal/message_reserved_range.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1087 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/internal/method_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1286 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/internal/oneof_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1078 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/internal/service_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      849 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/internal/strdup2.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      796 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/internal/strdup2.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      969 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/internal/upb_edition_defaults.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     8252 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/message.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3386 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/message.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    27484 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/message_def.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     6403 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/message_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1995 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/message_reserved_range.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      836 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/message_reserved_range.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3812 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/method_def.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1432 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/method_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     7367 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/oneof_def.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1836 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/oneof_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4039 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/service_def.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1499 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/reflection/service_def.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-04-18 00:15:09.000000 protobuf-5.27.0rc1/upb/text/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    15578 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/text/encode.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1454 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/text/encode.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-04-18 00:15:09.000000 protobuf-5.27.0rc1/upb/util/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    24464 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/util/def_to_proto.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1737 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/util/def_to_proto.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     9941 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/util/required_fields.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2842 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/util/required_fields.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-04-18 00:15:09.000000 protobuf-5.27.0rc1/upb/wire/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    54041 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/wire/decode.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     6190 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/wire/decode.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    22846 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/wire/encode.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2750 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/wire/encode.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      724 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/wire/eps_copy_input_stream.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    17093 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/wire/eps_copy_input_stream.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-04-18 00:15:09.000000 protobuf-5.27.0rc1/upb/wire/internal/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      716 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/wire/internal/constants.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    50516 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/wire/internal/decode_fast.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3998 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/wire/internal/decode_fast.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4286 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/wire/internal/decoder.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1635 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/wire/internal/reader.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1446 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/wire/reader.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     6570 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/wire/reader.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      620 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/upb/wire/types.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-04-18 00:15:09.000000 protobuf-5.27.0rc1/utf8_range/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    17939 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/utf8_range/utf8_range.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      540 2000-01-01 00:00:00.000000 protobuf-5.27.0rc1/utf8_range/utf8_range.h
```

### Comparing `protobuf-5.26.1/LICENSE` & `protobuf-5.27.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/PKG-INFO` & `protobuf-5.27.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protobuf
-Version: 5.26.1
+Version: 5.27.0rc1
 Summary: Protocol Buffers
 Home-page: https://developers.google.com/protocol-buffers/
 Download-URL: https://github.com/protocolbuffers/protobuf/releases
 Maintainer: protobuf@googlegroups.com
 Maintainer-email: protobuf@googlegroups.com
 License: BSD-3-Clause
 Project-URL: Source, https://github.com/protocolbuffers/protobuf
```

### Comparing `protobuf-5.26.1/README.md` & `protobuf-5.27.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/google/protobuf/any_pb2.py` & `protobuf-5.27.0rc1/google/protobuf/any_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
+# NO CHECKED-IN PROTOBUF GENCODE
 # source: google/protobuf/any.proto
-# Protobuf Python Version: 5.26.1
+# Protobuf Python Version: 5.27.0-rc1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import runtime_version as _runtime_version
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
+_runtime_version.ValidateProtobufRuntimeVersion(
+    _runtime_version.Domain.PUBLIC,
+    5,
+    27,
+    0,
+    '-rc1',
+    'google/protobuf/any.proto'
+)
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
```

### Comparing `protobuf-5.26.1/google/protobuf/api_pb2.py` & `protobuf-5.27.0rc1/google/protobuf/api_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
+# NO CHECKED-IN PROTOBUF GENCODE
 # source: google/protobuf/api.proto
-# Protobuf Python Version: 5.26.1
+# Protobuf Python Version: 5.27.0-rc1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import runtime_version as _runtime_version
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
+_runtime_version.ValidateProtobufRuntimeVersion(
+    _runtime_version.Domain.PUBLIC,
+    5,
+    27,
+    0,
+    '-rc1',
+    'google/protobuf/api.proto'
+)
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import source_context_pb2 as google_dot_protobuf_dot_source__context__pb2
 from google.protobuf import type_pb2 as google_dot_protobuf_dot_type__pb2
```

### Comparing `protobuf-5.26.1/google/protobuf/compiler/plugin_pb2.py` & `protobuf-5.27.0rc1/google/protobuf/compiler/plugin_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
+# NO CHECKED-IN PROTOBUF GENCODE
 # source: google/protobuf/compiler/plugin.proto
-# Protobuf Python Version: 5.26.1
+# Protobuf Python Version: 5.27.0-rc1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import runtime_version as _runtime_version
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
+_runtime_version.ValidateProtobufRuntimeVersion(
+    _runtime_version.Domain.PUBLIC,
+    5,
+    27,
+    0,
+    '-rc1',
+    'google/protobuf/compiler/plugin.proto'
+)
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import descriptor_pb2 as google_dot_protobuf_dot_descriptor__pb2
```

### Comparing `protobuf-5.26.1/google/protobuf/descriptor.py` & `protobuf-5.27.0rc1/google/protobuf/descriptor.py`

 * *Files 0% similar despite different names*

```diff
@@ -741,16 +741,19 @@
     """Whether the field distinguishes between unpopulated and default values.
 
     Raises:
       RuntimeError: singular field that is not linked with message nor file.
     """
     if self.label == FieldDescriptor.LABEL_REPEATED:
       return False
-    if (self.cpp_type == FieldDescriptor.CPPTYPE_MESSAGE or
-        self.containing_oneof):
+    if (
+        self.cpp_type == FieldDescriptor.CPPTYPE_MESSAGE
+        or self.is_extension
+        or self.containing_oneof
+    ):
       return True
 
     return (
         self._GetFeatures().field_presence
         != _FEATURESET_FIELD_PRESENCE_IMPLICIT
     )
```

### Comparing `protobuf-5.26.1/google/protobuf/descriptor.upb.h` & `protobuf-5.27.0rc1/google/protobuf/descriptor.upb.h`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 typedef struct google_protobuf_EnumValueDescriptorProto { upb_Message UPB_PRIVATE(base); } google_protobuf_EnumValueDescriptorProto;
 typedef struct google_protobuf_ServiceDescriptorProto { upb_Message UPB_PRIVATE(base); } google_protobuf_ServiceDescriptorProto;
 typedef struct google_protobuf_MethodDescriptorProto { upb_Message UPB_PRIVATE(base); } google_protobuf_MethodDescriptorProto;
 typedef struct google_protobuf_FileOptions { upb_Message UPB_PRIVATE(base); } google_protobuf_FileOptions;
 typedef struct google_protobuf_MessageOptions { upb_Message UPB_PRIVATE(base); } google_protobuf_MessageOptions;
 typedef struct google_protobuf_FieldOptions { upb_Message UPB_PRIVATE(base); } google_protobuf_FieldOptions;
 typedef struct google_protobuf_FieldOptions_EditionDefault { upb_Message UPB_PRIVATE(base); } google_protobuf_FieldOptions_EditionDefault;
+typedef struct google_protobuf_FieldOptions_FeatureSupport { upb_Message UPB_PRIVATE(base); } google_protobuf_FieldOptions_FeatureSupport;
 typedef struct google_protobuf_OneofOptions { upb_Message UPB_PRIVATE(base); } google_protobuf_OneofOptions;
 typedef struct google_protobuf_EnumOptions { upb_Message UPB_PRIVATE(base); } google_protobuf_EnumOptions;
 typedef struct google_protobuf_EnumValueOptions { upb_Message UPB_PRIVATE(base); } google_protobuf_EnumValueOptions;
 typedef struct google_protobuf_ServiceOptions { upb_Message UPB_PRIVATE(base); } google_protobuf_ServiceOptions;
 typedef struct google_protobuf_MethodOptions { upb_Message UPB_PRIVATE(base); } google_protobuf_MethodOptions;
 typedef struct google_protobuf_UninterpretedOption { upb_Message UPB_PRIVATE(base); } google_protobuf_UninterpretedOption;
 typedef struct google_protobuf_UninterpretedOption_NamePart { upb_Message UPB_PRIVATE(base); } google_protobuf_UninterpretedOption_NamePart;
@@ -52,14 +53,15 @@
 typedef struct google_protobuf_GeneratedCodeInfo { upb_Message UPB_PRIVATE(base); } google_protobuf_GeneratedCodeInfo;
 typedef struct google_protobuf_GeneratedCodeInfo_Annotation { upb_Message UPB_PRIVATE(base); } google_protobuf_GeneratedCodeInfo_Annotation;
 
 typedef enum {
   google_protobuf_EDITION_UNKNOWN = 0,
   google_protobuf_EDITION_1_TEST_ONLY = 1,
   google_protobuf_EDITION_2_TEST_ONLY = 2,
+  google_protobuf_EDITION_LEGACY = 900,
   google_protobuf_EDITION_PROTO2 = 998,
   google_protobuf_EDITION_PROTO3 = 999,
   google_protobuf_EDITION_2023 = 1000,
   google_protobuf_EDITION_2024 = 1001,
   google_protobuf_EDITION_99997_TEST_ONLY = 99997,
   google_protobuf_EDITION_99998_TEST_ONLY = 99998,
   google_protobuf_EDITION_99999_TEST_ONLY = 99999,
@@ -641,19 +643,19 @@
 UPB_INLINE bool google_protobuf_FileDescriptorProto_has_edition(const google_protobuf_FileDescriptorProto* msg) {
   const upb_MiniTableField field = {14, UPB_SIZE(48, 12), 69, 6, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
   return upb_Message_HasBaseField(UPB_UPCAST(msg), &field);
 }
 
 UPB_INLINE void google_protobuf_FileDescriptorProto_set_name(google_protobuf_FileDescriptorProto *msg, upb_StringView value) {
   const upb_MiniTableField field = {1, UPB_SIZE(52, 16), 64, kUpb_NoSub, 12, (int)kUpb_FieldMode_Scalar | (int)kUpb_LabelFlags_IsAlternate | ((int)kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FileDescriptorProto_set_package(google_protobuf_FileDescriptorProto *msg, upb_StringView value) {
   const upb_MiniTableField field = {2, UPB_SIZE(60, 32), 65, kUpb_NoSub, 12, (int)kUpb_FieldMode_Scalar | (int)kUpb_LabelFlags_IsAlternate | ((int)kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE upb_StringView* google_protobuf_FileDescriptorProto_mutable_dependency(google_protobuf_FileDescriptorProto* msg, size_t* size) {
   upb_MiniTableField field = {3, UPB_SIZE(12, 48), 0, kUpb_NoSub, 12, (int)kUpb_FieldMode_Array | (int)kUpb_LabelFlags_IsAlternate | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
   upb_Array* arr = upb_Message_GetMutableArray(UPB_UPCAST(msg), &field);
   if (arr) {
     if (size) *size = arr->UPB_PRIVATE(size);
     return (upb_StringView*)upb_Array_MutableDataPtr(arr);
@@ -797,27 +799,27 @@
   if (!arr || !sub) return NULL;
   UPB_PRIVATE(_upb_Array_Set)
   (arr, arr->UPB_PRIVATE(size) - 1, &sub, sizeof(sub));
   return sub;
 }
 UPB_INLINE void google_protobuf_FileDescriptorProto_set_options(google_protobuf_FileDescriptorProto *msg, google_protobuf_FileOptions* value) {
   const upb_MiniTableField field = {8, UPB_SIZE(32, 88), 66, 4, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE struct google_protobuf_FileOptions* google_protobuf_FileDescriptorProto_mutable_options(google_protobuf_FileDescriptorProto* msg, upb_Arena* arena) {
   struct google_protobuf_FileOptions* sub = (struct google_protobuf_FileOptions*)google_protobuf_FileDescriptorProto_options(msg);
   if (sub == NULL) {
     sub = (struct google_protobuf_FileOptions*)_upb_Message_New(&google__protobuf__FileOptions_msg_init, arena);
     if (sub) google_protobuf_FileDescriptorProto_set_options(msg, sub);
   }
   return sub;
 }
 UPB_INLINE void google_protobuf_FileDescriptorProto_set_source_code_info(google_protobuf_FileDescriptorProto *msg, google_protobuf_SourceCodeInfo* value) {
   const upb_MiniTableField field = {9, UPB_SIZE(36, 96), 67, 5, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE struct google_protobuf_SourceCodeInfo* google_protobuf_FileDescriptorProto_mutable_source_code_info(google_protobuf_FileDescriptorProto* msg, upb_Arena* arena) {
   struct google_protobuf_SourceCodeInfo* sub = (struct google_protobuf_SourceCodeInfo*)google_protobuf_FileDescriptorProto_source_code_info(msg);
   if (sub == NULL) {
     sub = (struct google_protobuf_SourceCodeInfo*)_upb_Message_New(&google__protobuf__SourceCodeInfo_msg_init, arena);
     if (sub) google_protobuf_FileDescriptorProto_set_source_code_info(msg, sub);
   }
@@ -877,19 +879,19 @@
   }
   UPB_PRIVATE(_upb_Array_Set)
   (arr, arr->UPB_PRIVATE(size) - 1, &val, sizeof(val));
   return true;
 }
 UPB_INLINE void google_protobuf_FileDescriptorProto_set_syntax(google_protobuf_FileDescriptorProto *msg, upb_StringView value) {
   const upb_MiniTableField field = {12, UPB_SIZE(68, 120), 68, kUpb_NoSub, 12, (int)kUpb_FieldMode_Scalar | (int)kUpb_LabelFlags_IsAlternate | ((int)kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FileDescriptorProto_set_edition(google_protobuf_FileDescriptorProto *msg, int32_t value) {
   const upb_MiniTableField field = {14, UPB_SIZE(48, 12), 69, 6, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 
 /* google.protobuf.DescriptorProto */
 
 UPB_INLINE google_protobuf_DescriptorProto* google_protobuf_DescriptorProto_new(upb_Arena* arena) {
   return (google_protobuf_DescriptorProto*)_upb_Message_New(&google__protobuf__DescriptorProto_msg_init, arena);
 }
@@ -1211,15 +1213,15 @@
     *size = arr ? arr->UPB_PRIVATE(size) : 0;
   }
   return arr;
 }
 
 UPB_INLINE void google_protobuf_DescriptorProto_set_name(google_protobuf_DescriptorProto *msg, upb_StringView value) {
   const upb_MiniTableField field = {1, UPB_SIZE(48, 16), 64, kUpb_NoSub, 12, (int)kUpb_FieldMode_Scalar | (int)kUpb_LabelFlags_IsAlternate | ((int)kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE google_protobuf_FieldDescriptorProto** google_protobuf_DescriptorProto_mutable_field(google_protobuf_DescriptorProto* msg, size_t* size) {
   upb_MiniTableField field = {2, UPB_SIZE(12, 32), 0, 0, 11, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
   upb_Array* arr = upb_Message_GetMutableArray(UPB_UPCAST(msg), &field);
   if (arr) {
     if (size) *size = arr->UPB_PRIVATE(size);
     return (google_protobuf_FieldDescriptorProto**)upb_Array_MutableDataPtr(arr);
@@ -1365,15 +1367,15 @@
   if (!arr || !sub) return NULL;
   UPB_PRIVATE(_upb_Array_Set)
   (arr, arr->UPB_PRIVATE(size) - 1, &sub, sizeof(sub));
   return sub;
 }
 UPB_INLINE void google_protobuf_DescriptorProto_set_options(google_protobuf_DescriptorProto *msg, google_protobuf_MessageOptions* value) {
   const upb_MiniTableField field = {7, UPB_SIZE(32, 72), 65, 5, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE struct google_protobuf_MessageOptions* google_protobuf_DescriptorProto_mutable_options(google_protobuf_DescriptorProto* msg, upb_Arena* arena) {
   struct google_protobuf_MessageOptions* sub = (struct google_protobuf_MessageOptions*)google_protobuf_DescriptorProto_options(msg);
   if (sub == NULL) {
     sub = (struct google_protobuf_MessageOptions*)_upb_Message_New(&google__protobuf__MessageOptions_msg_init, arena);
     if (sub) google_protobuf_DescriptorProto_set_options(msg, sub);
   }
@@ -1551,23 +1553,23 @@
 UPB_INLINE bool google_protobuf_DescriptorProto_ExtensionRange_has_options(const google_protobuf_DescriptorProto_ExtensionRange* msg) {
   const upb_MiniTableField field = {3, UPB_SIZE(20, 24), 66, 0, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
   return upb_Message_HasBaseField(UPB_UPCAST(msg), &field);
 }
 
 UPB_INLINE void google_protobuf_DescriptorProto_ExtensionRange_set_start(google_protobuf_DescriptorProto_ExtensionRange *msg, int32_t value) {
   const upb_MiniTableField field = {1, 12, 64, kUpb_NoSub, 5, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_DescriptorProto_ExtensionRange_set_end(google_protobuf_DescriptorProto_ExtensionRange *msg, int32_t value) {
   const upb_MiniTableField field = {2, 16, 65, kUpb_NoSub, 5, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_DescriptorProto_ExtensionRange_set_options(google_protobuf_DescriptorProto_ExtensionRange *msg, google_protobuf_ExtensionRangeOptions* value) {
   const upb_MiniTableField field = {3, UPB_SIZE(20, 24), 66, 0, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE struct google_protobuf_ExtensionRangeOptions* google_protobuf_DescriptorProto_ExtensionRange_mutable_options(google_protobuf_DescriptorProto_ExtensionRange* msg, upb_Arena* arena) {
   struct google_protobuf_ExtensionRangeOptions* sub = (struct google_protobuf_ExtensionRangeOptions*)google_protobuf_DescriptorProto_ExtensionRange_options(msg);
   if (sub == NULL) {
     sub = (struct google_protobuf_ExtensionRangeOptions*)_upb_Message_New(&google__protobuf__ExtensionRangeOptions_msg_init, arena);
     if (sub) google_protobuf_DescriptorProto_ExtensionRange_set_options(msg, sub);
   }
@@ -1641,19 +1643,19 @@
 UPB_INLINE bool google_protobuf_DescriptorProto_ReservedRange_has_end(const google_protobuf_DescriptorProto_ReservedRange* msg) {
   const upb_MiniTableField field = {2, 16, 65, kUpb_NoSub, 5, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
   return upb_Message_HasBaseField(UPB_UPCAST(msg), &field);
 }
 
 UPB_INLINE void google_protobuf_DescriptorProto_ReservedRange_set_start(google_protobuf_DescriptorProto_ReservedRange *msg, int32_t value) {
   const upb_MiniTableField field = {1, 12, 64, kUpb_NoSub, 5, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_DescriptorProto_ReservedRange_set_end(google_protobuf_DescriptorProto_ReservedRange *msg, int32_t value) {
   const upb_MiniTableField field = {2, 16, 65, kUpb_NoSub, 5, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 
 /* google.protobuf.ExtensionRangeOptions */
 
 UPB_INLINE google_protobuf_ExtensionRangeOptions* google_protobuf_ExtensionRangeOptions_new(upb_Arena* arena) {
   return (google_protobuf_ExtensionRangeOptions*)_upb_Message_New(&google__protobuf__ExtensionRangeOptions_msg_init, arena);
 }
@@ -1813,19 +1815,19 @@
   if (!arr || !sub) return NULL;
   UPB_PRIVATE(_upb_Array_Set)
   (arr, arr->UPB_PRIVATE(size) - 1, &sub, sizeof(sub));
   return sub;
 }
 UPB_INLINE void google_protobuf_ExtensionRangeOptions_set_verification(google_protobuf_ExtensionRangeOptions *msg, int32_t value) {
   const upb_MiniTableField field = {3, UPB_SIZE(16, 12), 64, 3, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_ExtensionRangeOptions_set_features(google_protobuf_ExtensionRangeOptions *msg, google_protobuf_FeatureSet* value) {
   const upb_MiniTableField field = {50, UPB_SIZE(20, 24), 65, 1, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE struct google_protobuf_FeatureSet* google_protobuf_ExtensionRangeOptions_mutable_features(google_protobuf_ExtensionRangeOptions* msg, upb_Arena* arena) {
   struct google_protobuf_FeatureSet* sub = (struct google_protobuf_FeatureSet*)google_protobuf_ExtensionRangeOptions_features(msg);
   if (sub == NULL) {
     sub = (struct google_protobuf_FeatureSet*)_upb_Message_New(&google__protobuf__FeatureSet_msg_init, arena);
     if (sub) google_protobuf_ExtensionRangeOptions_set_features(msg, sub);
   }
@@ -1977,31 +1979,31 @@
 UPB_INLINE bool google_protobuf_ExtensionRangeOptions_Declaration_has_repeated(const google_protobuf_ExtensionRangeOptions_Declaration* msg) {
   const upb_MiniTableField field = {6, 17, 68, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
   return upb_Message_HasBaseField(UPB_UPCAST(msg), &field);
 }
 
 UPB_INLINE void google_protobuf_ExtensionRangeOptions_Declaration_set_number(google_protobuf_ExtensionRangeOptions_Declaration *msg, int32_t value) {
   const upb_MiniTableField field = {1, 12, 64, kUpb_NoSub, 5, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_ExtensionRangeOptions_Declaration_set_full_name(google_protobuf_ExtensionRangeOptions_Declaration *msg, upb_StringView value) {
   const upb_MiniTableField field = {2, UPB_SIZE(20, 24), 65, kUpb_NoSub, 12, (int)kUpb_FieldMode_Scalar | (int)kUpb_LabelFlags_IsAlternate | ((int)kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_ExtensionRangeOptions_Declaration_set_type(google_protobuf_ExtensionRangeOptions_Declaration *msg, upb_StringView value) {
   const upb_MiniTableField field = {3, UPB_SIZE(28, 40), 66, kUpb_NoSub, 12, (int)kUpb_FieldMode_Scalar | (int)kUpb_LabelFlags_IsAlternate | ((int)kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_ExtensionRangeOptions_Declaration_set_reserved(google_protobuf_ExtensionRangeOptions_Declaration *msg, bool value) {
   const upb_MiniTableField field = {5, 16, 67, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_ExtensionRangeOptions_Declaration_set_repeated(google_protobuf_ExtensionRangeOptions_Declaration *msg, bool value) {
   const upb_MiniTableField field = {6, 17, 68, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 
 /* google.protobuf.FieldDescriptorProto */
 
 UPB_INLINE google_protobuf_FieldDescriptorProto* google_protobuf_FieldDescriptorProto_new(upb_Arena* arena) {
   return (google_protobuf_FieldDescriptorProto*)_upb_Message_New(&google__protobuf__FieldDescriptorProto_msg_init, arena);
 }
@@ -2211,63 +2213,63 @@
 UPB_INLINE bool google_protobuf_FieldDescriptorProto_has_proto3_optional(const google_protobuf_FieldDescriptorProto* msg) {
   const upb_MiniTableField field = {17, UPB_SIZE(32, 28), 74, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
   return upb_Message_HasBaseField(UPB_UPCAST(msg), &field);
 }
 
 UPB_INLINE void google_protobuf_FieldDescriptorProto_set_name(google_protobuf_FieldDescriptorProto *msg, upb_StringView value) {
   const upb_MiniTableField field = {1, UPB_SIZE(36, 32), 64, kUpb_NoSub, 12, (int)kUpb_FieldMode_Scalar | (int)kUpb_LabelFlags_IsAlternate | ((int)kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FieldDescriptorProto_set_extendee(google_protobuf_FieldDescriptorProto *msg, upb_StringView value) {
   const upb_MiniTableField field = {2, UPB_SIZE(44, 48), 65, kUpb_NoSub, 12, (int)kUpb_FieldMode_Scalar | (int)kUpb_LabelFlags_IsAlternate | ((int)kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FieldDescriptorProto_set_number(google_protobuf_FieldDescriptorProto *msg, int32_t value) {
   const upb_MiniTableField field = {3, 12, 66, kUpb_NoSub, 5, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FieldDescriptorProto_set_label(google_protobuf_FieldDescriptorProto *msg, int32_t value) {
   const upb_MiniTableField field = {4, 16, 67, 1, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FieldDescriptorProto_set_type(google_protobuf_FieldDescriptorProto *msg, int32_t value) {
   const upb_MiniTableField field = {5, 20, 68, 2, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FieldDescriptorProto_set_type_name(google_protobuf_FieldDescriptorProto *msg, upb_StringView value) {
   const upb_MiniTableField field = {6, UPB_SIZE(52, 64), 69, kUpb_NoSub, 12, (int)kUpb_FieldMode_Scalar | (int)kUpb_LabelFlags_IsAlternate | ((int)kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FieldDescriptorProto_set_default_value(google_protobuf_FieldDescriptorProto *msg, upb_StringView value) {
   const upb_MiniTableField field = {7, UPB_SIZE(60, 80), 70, kUpb_NoSub, 12, (int)kUpb_FieldMode_Scalar | (int)kUpb_LabelFlags_IsAlternate | ((int)kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FieldDescriptorProto_set_options(google_protobuf_FieldDescriptorProto *msg, google_protobuf_FieldOptions* value) {
   const upb_MiniTableField field = {8, UPB_SIZE(24, 96), 71, 0, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE struct google_protobuf_FieldOptions* google_protobuf_FieldDescriptorProto_mutable_options(google_protobuf_FieldDescriptorProto* msg, upb_Arena* arena) {
   struct google_protobuf_FieldOptions* sub = (struct google_protobuf_FieldOptions*)google_protobuf_FieldDescriptorProto_options(msg);
   if (sub == NULL) {
     sub = (struct google_protobuf_FieldOptions*)_upb_Message_New(&google__protobuf__FieldOptions_msg_init, arena);
     if (sub) google_protobuf_FieldDescriptorProto_set_options(msg, sub);
   }
   return sub;
 }
 UPB_INLINE void google_protobuf_FieldDescriptorProto_set_oneof_index(google_protobuf_FieldDescriptorProto *msg, int32_t value) {
   const upb_MiniTableField field = {9, UPB_SIZE(28, 24), 72, kUpb_NoSub, 5, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FieldDescriptorProto_set_json_name(google_protobuf_FieldDescriptorProto *msg, upb_StringView value) {
   const upb_MiniTableField field = {10, UPB_SIZE(68, 104), 73, kUpb_NoSub, 12, (int)kUpb_FieldMode_Scalar | (int)kUpb_LabelFlags_IsAlternate | ((int)kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FieldDescriptorProto_set_proto3_optional(google_protobuf_FieldDescriptorProto *msg, bool value) {
   const upb_MiniTableField field = {17, UPB_SIZE(32, 28), 74, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 
 /* google.protobuf.OneofDescriptorProto */
 
 UPB_INLINE google_protobuf_OneofDescriptorProto* google_protobuf_OneofDescriptorProto_new(upb_Arena* arena) {
   return (google_protobuf_OneofDescriptorProto*)_upb_Message_New(&google__protobuf__OneofDescriptorProto_msg_init, arena);
 }
@@ -2333,19 +2335,19 @@
 UPB_INLINE bool google_protobuf_OneofDescriptorProto_has_options(const google_protobuf_OneofDescriptorProto* msg) {
   const upb_MiniTableField field = {2, UPB_SIZE(12, 32), 65, 0, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
   return upb_Message_HasBaseField(UPB_UPCAST(msg), &field);
 }
 
 UPB_INLINE void google_protobuf_OneofDescriptorProto_set_name(google_protobuf_OneofDescriptorProto *msg, upb_StringView value) {
   const upb_MiniTableField field = {1, 16, 64, kUpb_NoSub, 12, (int)kUpb_FieldMode_Scalar | (int)kUpb_LabelFlags_IsAlternate | ((int)kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_OneofDescriptorProto_set_options(google_protobuf_OneofDescriptorProto *msg, google_protobuf_OneofOptions* value) {
   const upb_MiniTableField field = {2, UPB_SIZE(12, 32), 65, 0, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE struct google_protobuf_OneofOptions* google_protobuf_OneofDescriptorProto_mutable_options(google_protobuf_OneofDescriptorProto* msg, upb_Arena* arena) {
   struct google_protobuf_OneofOptions* sub = (struct google_protobuf_OneofOptions*)google_protobuf_OneofDescriptorProto_options(msg);
   if (sub == NULL) {
     sub = (struct google_protobuf_OneofOptions*)_upb_Message_New(&google__protobuf__OneofOptions_msg_init, arena);
     if (sub) google_protobuf_OneofDescriptorProto_set_options(msg, sub);
   }
@@ -2515,15 +2517,15 @@
     *size = arr ? arr->UPB_PRIVATE(size) : 0;
   }
   return arr;
 }
 
 UPB_INLINE void google_protobuf_EnumDescriptorProto_set_name(google_protobuf_EnumDescriptorProto *msg, upb_StringView value) {
   const upb_MiniTableField field = {1, UPB_SIZE(28, 16), 64, kUpb_NoSub, 12, (int)kUpb_FieldMode_Scalar | (int)kUpb_LabelFlags_IsAlternate | ((int)kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE google_protobuf_EnumValueDescriptorProto** google_protobuf_EnumDescriptorProto_mutable_value(google_protobuf_EnumDescriptorProto* msg, size_t* size) {
   upb_MiniTableField field = {2, UPB_SIZE(12, 32), 0, 0, 11, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
   upb_Array* arr = upb_Message_GetMutableArray(UPB_UPCAST(msg), &field);
   if (arr) {
     if (size) *size = arr->UPB_PRIVATE(size);
     return (google_protobuf_EnumValueDescriptorProto**)upb_Array_MutableDataPtr(arr);
@@ -2549,15 +2551,15 @@
   if (!arr || !sub) return NULL;
   UPB_PRIVATE(_upb_Array_Set)
   (arr, arr->UPB_PRIVATE(size) - 1, &sub, sizeof(sub));
   return sub;
 }
 UPB_INLINE void google_protobuf_EnumDescriptorProto_set_options(google_protobuf_EnumDescriptorProto *msg, google_protobuf_EnumOptions* value) {
   const upb_MiniTableField field = {3, UPB_SIZE(16, 40), 65, 1, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE struct google_protobuf_EnumOptions* google_protobuf_EnumDescriptorProto_mutable_options(google_protobuf_EnumDescriptorProto* msg, upb_Arena* arena) {
   struct google_protobuf_EnumOptions* sub = (struct google_protobuf_EnumOptions*)google_protobuf_EnumDescriptorProto_options(msg);
   if (sub == NULL) {
     sub = (struct google_protobuf_EnumOptions*)_upb_Message_New(&google__protobuf__EnumOptions_msg_init, arena);
     if (sub) google_protobuf_EnumDescriptorProto_set_options(msg, sub);
   }
@@ -2689,19 +2691,19 @@
 UPB_INLINE bool google_protobuf_EnumDescriptorProto_EnumReservedRange_has_end(const google_protobuf_EnumDescriptorProto_EnumReservedRange* msg) {
   const upb_MiniTableField field = {2, 16, 65, kUpb_NoSub, 5, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
   return upb_Message_HasBaseField(UPB_UPCAST(msg), &field);
 }
 
 UPB_INLINE void google_protobuf_EnumDescriptorProto_EnumReservedRange_set_start(google_protobuf_EnumDescriptorProto_EnumReservedRange *msg, int32_t value) {
   const upb_MiniTableField field = {1, 12, 64, kUpb_NoSub, 5, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_EnumDescriptorProto_EnumReservedRange_set_end(google_protobuf_EnumDescriptorProto_EnumReservedRange *msg, int32_t value) {
   const upb_MiniTableField field = {2, 16, 65, kUpb_NoSub, 5, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 
 /* google.protobuf.EnumValueDescriptorProto */
 
 UPB_INLINE google_protobuf_EnumValueDescriptorProto* google_protobuf_EnumValueDescriptorProto_new(upb_Arena* arena) {
   return (google_protobuf_EnumValueDescriptorProto*)_upb_Message_New(&google__protobuf__EnumValueDescriptorProto_msg_init, arena);
 }
@@ -2783,23 +2785,23 @@
 UPB_INLINE bool google_protobuf_EnumValueDescriptorProto_has_options(const google_protobuf_EnumValueDescriptorProto* msg) {
   const upb_MiniTableField field = {3, UPB_SIZE(16, 32), 66, 0, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
   return upb_Message_HasBaseField(UPB_UPCAST(msg), &field);
 }
 
 UPB_INLINE void google_protobuf_EnumValueDescriptorProto_set_name(google_protobuf_EnumValueDescriptorProto *msg, upb_StringView value) {
   const upb_MiniTableField field = {1, UPB_SIZE(20, 16), 64, kUpb_NoSub, 12, (int)kUpb_FieldMode_Scalar | (int)kUpb_LabelFlags_IsAlternate | ((int)kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_EnumValueDescriptorProto_set_number(google_protobuf_EnumValueDescriptorProto *msg, int32_t value) {
   const upb_MiniTableField field = {2, 12, 65, kUpb_NoSub, 5, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_EnumValueDescriptorProto_set_options(google_protobuf_EnumValueDescriptorProto *msg, google_protobuf_EnumValueOptions* value) {
   const upb_MiniTableField field = {3, UPB_SIZE(16, 32), 66, 0, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE struct google_protobuf_EnumValueOptions* google_protobuf_EnumValueDescriptorProto_mutable_options(google_protobuf_EnumValueDescriptorProto* msg, upb_Arena* arena) {
   struct google_protobuf_EnumValueOptions* sub = (struct google_protobuf_EnumValueOptions*)google_protobuf_EnumValueDescriptorProto_options(msg);
   if (sub == NULL) {
     sub = (struct google_protobuf_EnumValueOptions*)_upb_Message_New(&google__protobuf__EnumValueOptions_msg_init, arena);
     if (sub) google_protobuf_EnumValueDescriptorProto_set_options(msg, sub);
   }
@@ -2905,15 +2907,15 @@
 UPB_INLINE bool google_protobuf_ServiceDescriptorProto_has_options(const google_protobuf_ServiceDescriptorProto* msg) {
   const upb_MiniTableField field = {3, UPB_SIZE(16, 40), 65, 1, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
   return upb_Message_HasBaseField(UPB_UPCAST(msg), &field);
 }
 
 UPB_INLINE void google_protobuf_ServiceDescriptorProto_set_name(google_protobuf_ServiceDescriptorProto *msg, upb_StringView value) {
   const upb_MiniTableField field = {1, UPB_SIZE(20, 16), 64, kUpb_NoSub, 12, (int)kUpb_FieldMode_Scalar | (int)kUpb_LabelFlags_IsAlternate | ((int)kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE google_protobuf_MethodDescriptorProto** google_protobuf_ServiceDescriptorProto_mutable_method(google_protobuf_ServiceDescriptorProto* msg, size_t* size) {
   upb_MiniTableField field = {2, UPB_SIZE(12, 32), 0, 0, 11, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
   upb_Array* arr = upb_Message_GetMutableArray(UPB_UPCAST(msg), &field);
   if (arr) {
     if (size) *size = arr->UPB_PRIVATE(size);
     return (google_protobuf_MethodDescriptorProto**)upb_Array_MutableDataPtr(arr);
@@ -2939,15 +2941,15 @@
   if (!arr || !sub) return NULL;
   UPB_PRIVATE(_upb_Array_Set)
   (arr, arr->UPB_PRIVATE(size) - 1, &sub, sizeof(sub));
   return sub;
 }
 UPB_INLINE void google_protobuf_ServiceDescriptorProto_set_options(google_protobuf_ServiceDescriptorProto *msg, google_protobuf_ServiceOptions* value) {
   const upb_MiniTableField field = {3, UPB_SIZE(16, 40), 65, 1, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE struct google_protobuf_ServiceOptions* google_protobuf_ServiceDescriptorProto_mutable_options(google_protobuf_ServiceDescriptorProto* msg, upb_Arena* arena) {
   struct google_protobuf_ServiceOptions* sub = (struct google_protobuf_ServiceOptions*)google_protobuf_ServiceDescriptorProto_options(msg);
   if (sub == NULL) {
     sub = (struct google_protobuf_ServiceOptions*)_upb_Message_New(&google__protobuf__ServiceOptions_msg_init, arena);
     if (sub) google_protobuf_ServiceDescriptorProto_set_options(msg, sub);
   }
@@ -3085,43 +3087,43 @@
 UPB_INLINE bool google_protobuf_MethodDescriptorProto_has_server_streaming(const google_protobuf_MethodDescriptorProto* msg) {
   const upb_MiniTableField field = {6, UPB_SIZE(17, 10), 69, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
   return upb_Message_HasBaseField(UPB_UPCAST(msg), &field);
 }
 
 UPB_INLINE void google_protobuf_MethodDescriptorProto_set_name(google_protobuf_MethodDescriptorProto *msg, upb_StringView value) {
   const upb_MiniTableField field = {1, UPB_SIZE(20, 16), 64, kUpb_NoSub, 12, (int)kUpb_FieldMode_Scalar | (int)kUpb_LabelFlags_IsAlternate | ((int)kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_MethodDescriptorProto_set_input_type(google_protobuf_MethodDescriptorProto *msg, upb_StringView value) {
   const upb_MiniTableField field = {2, UPB_SIZE(28, 32), 65, kUpb_NoSub, 12, (int)kUpb_FieldMode_Scalar | (int)kUpb_LabelFlags_IsAlternate | ((int)kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_MethodDescriptorProto_set_output_type(google_protobuf_MethodDescriptorProto *msg, upb_StringView value) {
   const upb_MiniTableField field = {3, UPB_SIZE(36, 48), 66, kUpb_NoSub, 12, (int)kUpb_FieldMode_Scalar | (int)kUpb_LabelFlags_IsAlternate | ((int)kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_MethodDescriptorProto_set_options(google_protobuf_MethodDescriptorProto *msg, google_protobuf_MethodOptions* value) {
   const upb_MiniTableField field = {4, UPB_SIZE(12, 64), 67, 0, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE struct google_protobuf_MethodOptions* google_protobuf_MethodDescriptorProto_mutable_options(google_protobuf_MethodDescriptorProto* msg, upb_Arena* arena) {
   struct google_protobuf_MethodOptions* sub = (struct google_protobuf_MethodOptions*)google_protobuf_MethodDescriptorProto_options(msg);
   if (sub == NULL) {
     sub = (struct google_protobuf_MethodOptions*)_upb_Message_New(&google__protobuf__MethodOptions_msg_init, arena);
     if (sub) google_protobuf_MethodDescriptorProto_set_options(msg, sub);
   }
   return sub;
 }
 UPB_INLINE void google_protobuf_MethodDescriptorProto_set_client_streaming(google_protobuf_MethodDescriptorProto *msg, bool value) {
   const upb_MiniTableField field = {5, UPB_SIZE(16, 9), 68, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_MethodDescriptorProto_set_server_streaming(google_protobuf_MethodDescriptorProto *msg, bool value) {
   const upb_MiniTableField field = {6, UPB_SIZE(17, 10), 69, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 
 /* google.protobuf.FileOptions */
 
 UPB_INLINE google_protobuf_FileOptions* google_protobuf_FileOptions_new(upb_Arena* arena) {
   return (google_protobuf_FileOptions*)_upb_Message_New(&google__protobuf__FileOptions_msg_init, arena);
 }
@@ -3507,91 +3509,91 @@
     *size = arr ? arr->UPB_PRIVATE(size) : 0;
   }
   return arr;
 }
 
 UPB_INLINE void google_protobuf_FileOptions_set_java_package(google_protobuf_FileOptions *msg, upb_StringView value) {
   const upb_MiniTableField field = {1, UPB_SIZE(32, 24), 64, kUpb_NoSub, 12, (int)kUpb_FieldMode_Scalar | (int)kUpb_LabelFlags_IsAlternate | ((int)kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FileOptions_set_java_outer_classname(google_protobuf_FileOptions *msg, upb_StringView value) {
   const upb_MiniTableField field = {8, 40, 65, kUpb_NoSub, 12, (int)kUpb_FieldMode_Scalar | (int)kUpb_LabelFlags_IsAlternate | ((int)kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FileOptions_set_optimize_for(google_protobuf_FileOptions *msg, int32_t value) {
   const upb_MiniTableField field = {9, 12, 66, 2, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FileOptions_set_java_multiple_files(google_protobuf_FileOptions *msg, bool value) {
   const upb_MiniTableField field = {10, 16, 67, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FileOptions_set_go_package(google_protobuf_FileOptions *msg, upb_StringView value) {
   const upb_MiniTableField field = {11, UPB_SIZE(48, 56), 68, kUpb_NoSub, 12, (int)kUpb_FieldMode_Scalar | (int)kUpb_LabelFlags_IsAlternate | ((int)kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FileOptions_set_cc_generic_services(google_protobuf_FileOptions *msg, bool value) {
   const upb_MiniTableField field = {16, 17, 69, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FileOptions_set_java_generic_services(google_protobuf_FileOptions *msg, bool value) {
   const upb_MiniTableField field = {17, 18, 70, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FileOptions_set_py_generic_services(google_protobuf_FileOptions *msg, bool value) {
   const upb_MiniTableField field = {18, 19, 71, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FileOptions_set_java_generate_equals_and_hash(google_protobuf_FileOptions *msg, bool value) {
   const upb_MiniTableField field = {20, 20, 72, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FileOptions_set_deprecated(google_protobuf_FileOptions *msg, bool value) {
   const upb_MiniTableField field = {23, 21, 73, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FileOptions_set_java_string_check_utf8(google_protobuf_FileOptions *msg, bool value) {
   const upb_MiniTableField field = {27, 22, 74, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FileOptions_set_cc_enable_arenas(google_protobuf_FileOptions *msg, bool value) {
   const upb_MiniTableField field = {31, 23, 75, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FileOptions_set_objc_class_prefix(google_protobuf_FileOptions *msg, upb_StringView value) {
   const upb_MiniTableField field = {36, UPB_SIZE(56, 72), 76, kUpb_NoSub, 12, (int)kUpb_FieldMode_Scalar | (int)kUpb_LabelFlags_IsAlternate | ((int)kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FileOptions_set_csharp_namespace(google_protobuf_FileOptions *msg, upb_StringView value) {
   const upb_MiniTableField field = {37, UPB_SIZE(64, 88), 77, kUpb_NoSub, 12, (int)kUpb_FieldMode_Scalar | (int)kUpb_LabelFlags_IsAlternate | ((int)kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FileOptions_set_swift_prefix(google_protobuf_FileOptions *msg, upb_StringView value) {
   const upb_MiniTableField field = {39, UPB_SIZE(72, 104), 78, kUpb_NoSub, 12, (int)kUpb_FieldMode_Scalar | (int)kUpb_LabelFlags_IsAlternate | ((int)kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FileOptions_set_php_class_prefix(google_protobuf_FileOptions *msg, upb_StringView value) {
   const upb_MiniTableField field = {40, UPB_SIZE(80, 120), 79, kUpb_NoSub, 12, (int)kUpb_FieldMode_Scalar | (int)kUpb_LabelFlags_IsAlternate | ((int)kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FileOptions_set_php_namespace(google_protobuf_FileOptions *msg, upb_StringView value) {
   const upb_MiniTableField field = {41, UPB_SIZE(88, 136), 80, kUpb_NoSub, 12, (int)kUpb_FieldMode_Scalar | (int)kUpb_LabelFlags_IsAlternate | ((int)kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FileOptions_set_php_metadata_namespace(google_protobuf_FileOptions *msg, upb_StringView value) {
   const upb_MiniTableField field = {44, UPB_SIZE(96, 152), 81, kUpb_NoSub, 12, (int)kUpb_FieldMode_Scalar | (int)kUpb_LabelFlags_IsAlternate | ((int)kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FileOptions_set_ruby_package(google_protobuf_FileOptions *msg, upb_StringView value) {
   const upb_MiniTableField field = {45, UPB_SIZE(104, 168), 82, kUpb_NoSub, 12, (int)kUpb_FieldMode_Scalar | (int)kUpb_LabelFlags_IsAlternate | ((int)kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FileOptions_set_features(google_protobuf_FileOptions *msg, google_protobuf_FeatureSet* value) {
   const upb_MiniTableField field = {50, UPB_SIZE(24, 184), 83, 0, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE struct google_protobuf_FeatureSet* google_protobuf_FileOptions_mutable_features(google_protobuf_FileOptions* msg, upb_Arena* arena) {
   struct google_protobuf_FeatureSet* sub = (struct google_protobuf_FeatureSet*)google_protobuf_FileOptions_features(msg);
   if (sub == NULL) {
     sub = (struct google_protobuf_FeatureSet*)_upb_Message_New(&google__protobuf__FeatureSet_msg_init, arena);
     if (sub) google_protobuf_FileOptions_set_features(msg, sub);
   }
@@ -3791,35 +3793,35 @@
     *size = arr ? arr->UPB_PRIVATE(size) : 0;
   }
   return arr;
 }
 
 UPB_INLINE void google_protobuf_MessageOptions_set_message_set_wire_format(google_protobuf_MessageOptions *msg, bool value) {
   const upb_MiniTableField field = {1, 9, 64, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_MessageOptions_set_no_standard_descriptor_accessor(google_protobuf_MessageOptions *msg, bool value) {
   const upb_MiniTableField field = {2, 10, 65, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_MessageOptions_set_deprecated(google_protobuf_MessageOptions *msg, bool value) {
   const upb_MiniTableField field = {3, 11, 66, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_MessageOptions_set_map_entry(google_protobuf_MessageOptions *msg, bool value) {
   const upb_MiniTableField field = {7, 12, 67, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_MessageOptions_set_deprecated_legacy_json_field_conflicts(google_protobuf_MessageOptions *msg, bool value) {
   const upb_MiniTableField field = {11, 13, 68, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_MessageOptions_set_features(google_protobuf_MessageOptions *msg, google_protobuf_FeatureSet* value) {
   const upb_MiniTableField field = {12, 16, 69, 0, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE struct google_protobuf_FeatureSet* google_protobuf_MessageOptions_mutable_features(google_protobuf_MessageOptions* msg, upb_Arena* arena) {
   struct google_protobuf_FeatureSet* sub = (struct google_protobuf_FeatureSet*)google_protobuf_MessageOptions_features(msg);
   if (sub == NULL) {
     sub = (struct google_protobuf_FeatureSet*)_upb_Message_New(&google__protobuf__FeatureSet_msg_init, arena);
     if (sub) google_protobuf_MessageOptions_set_features(msg, sub);
   }
@@ -3889,27 +3891,27 @@
 UPB_INLINE char* google_protobuf_FieldOptions_serialize_ex(const google_protobuf_FieldOptions* msg, int options,
                                  upb_Arena* arena, size_t* len) {
   char* ptr;
   (void)upb_Encode(UPB_UPCAST(msg), &google__protobuf__FieldOptions_msg_init, options, arena, &ptr, len);
   return ptr;
 }
 UPB_INLINE void google_protobuf_FieldOptions_clear_ctype(google_protobuf_FieldOptions* msg) {
-  const upb_MiniTableField field = {1, 12, 64, 3, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
+  const upb_MiniTableField field = {1, 12, 64, 4, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
   upb_Message_ClearBaseField(UPB_UPCAST(msg), &field);
 }
 UPB_INLINE int32_t google_protobuf_FieldOptions_ctype(const google_protobuf_FieldOptions* msg) {
   int32_t default_val = 0;
   int32_t ret;
-  const upb_MiniTableField field = {1, 12, 64, 3, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
+  const upb_MiniTableField field = {1, 12, 64, 4, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
   _upb_Message_GetNonExtensionField(UPB_UPCAST(msg), &field,
                                     &default_val, &ret);
   return ret;
 }
 UPB_INLINE bool google_protobuf_FieldOptions_has_ctype(const google_protobuf_FieldOptions* msg) {
-  const upb_MiniTableField field = {1, 12, 64, 3, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
+  const upb_MiniTableField field = {1, 12, 64, 4, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
   return upb_Message_HasBaseField(UPB_UPCAST(msg), &field);
 }
 UPB_INLINE void google_protobuf_FieldOptions_clear_packed(google_protobuf_FieldOptions* msg) {
   const upb_MiniTableField field = {2, 16, 65, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
   upb_Message_ClearBaseField(UPB_UPCAST(msg), &field);
 }
 UPB_INLINE bool google_protobuf_FieldOptions_packed(const google_protobuf_FieldOptions* msg) {
@@ -3953,27 +3955,27 @@
   return ret;
 }
 UPB_INLINE bool google_protobuf_FieldOptions_has_lazy(const google_protobuf_FieldOptions* msg) {
   const upb_MiniTableField field = {5, 18, 67, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
   return upb_Message_HasBaseField(UPB_UPCAST(msg), &field);
 }
 UPB_INLINE void google_protobuf_FieldOptions_clear_jstype(google_protobuf_FieldOptions* msg) {
-  const upb_MiniTableField field = {6, 20, 68, 4, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
+  const upb_MiniTableField field = {6, 20, 68, 5, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
   upb_Message_ClearBaseField(UPB_UPCAST(msg), &field);
 }
 UPB_INLINE int32_t google_protobuf_FieldOptions_jstype(const google_protobuf_FieldOptions* msg) {
   int32_t default_val = 0;
   int32_t ret;
-  const upb_MiniTableField field = {6, 20, 68, 4, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
+  const upb_MiniTableField field = {6, 20, 68, 5, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
   _upb_Message_GetNonExtensionField(UPB_UPCAST(msg), &field,
                                     &default_val, &ret);
   return ret;
 }
 UPB_INLINE bool google_protobuf_FieldOptions_has_jstype(const google_protobuf_FieldOptions* msg) {
-  const upb_MiniTableField field = {6, 20, 68, 4, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
+  const upb_MiniTableField field = {6, 20, 68, 5, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
   return upb_Message_HasBaseField(UPB_UPCAST(msg), &field);
 }
 UPB_INLINE void google_protobuf_FieldOptions_clear_weak(google_protobuf_FieldOptions* msg) {
   const upb_MiniTableField field = {10, 24, 69, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
   upb_Message_ClearBaseField(UPB_UPCAST(msg), &field);
 }
 UPB_INLINE bool google_protobuf_FieldOptions_weak(const google_protobuf_FieldOptions* msg) {
@@ -4017,54 +4019,54 @@
   return ret;
 }
 UPB_INLINE bool google_protobuf_FieldOptions_has_debug_redact(const google_protobuf_FieldOptions* msg) {
   const upb_MiniTableField field = {16, 26, 71, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
   return upb_Message_HasBaseField(UPB_UPCAST(msg), &field);
 }
 UPB_INLINE void google_protobuf_FieldOptions_clear_retention(google_protobuf_FieldOptions* msg) {
-  const upb_MiniTableField field = {17, 28, 72, 5, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
+  const upb_MiniTableField field = {17, 28, 72, 6, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
   upb_Message_ClearBaseField(UPB_UPCAST(msg), &field);
 }
 UPB_INLINE int32_t google_protobuf_FieldOptions_retention(const google_protobuf_FieldOptions* msg) {
   int32_t default_val = 0;
   int32_t ret;
-  const upb_MiniTableField field = {17, 28, 72, 5, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
+  const upb_MiniTableField field = {17, 28, 72, 6, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
   _upb_Message_GetNonExtensionField(UPB_UPCAST(msg), &field,
                                     &default_val, &ret);
   return ret;
 }
 UPB_INLINE bool google_protobuf_FieldOptions_has_retention(const google_protobuf_FieldOptions* msg) {
-  const upb_MiniTableField field = {17, 28, 72, 5, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
+  const upb_MiniTableField field = {17, 28, 72, 6, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
   return upb_Message_HasBaseField(UPB_UPCAST(msg), &field);
 }
 UPB_INLINE void google_protobuf_FieldOptions_clear_targets(google_protobuf_FieldOptions* msg) {
-  const upb_MiniTableField field = {19, 32, 0, 6, 14, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_MiniTableField field = {19, 32, 0, 7, 14, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
   upb_Message_ClearBaseField(UPB_UPCAST(msg), &field);
 }
 UPB_INLINE int32_t const* google_protobuf_FieldOptions_targets(const google_protobuf_FieldOptions* msg, size_t* size) {
-  const upb_MiniTableField field = {19, 32, 0, 6, 14, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_MiniTableField field = {19, 32, 0, 7, 14, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
   const upb_Array* arr = upb_Message_GetArray(UPB_UPCAST(msg), &field);
   if (arr) {
     if (size) *size = arr->UPB_PRIVATE(size);
     return (int32_t const*)upb_Array_DataPtr(arr);
   } else {
     if (size) *size = 0;
     return NULL;
   }
 }
 UPB_INLINE const upb_Array* _google_protobuf_FieldOptions_targets_upb_array(const google_protobuf_FieldOptions* msg, size_t* size) {
-  const upb_MiniTableField field = {19, 32, 0, 6, 14, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_MiniTableField field = {19, 32, 0, 7, 14, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
   const upb_Array* arr = upb_Message_GetArray(UPB_UPCAST(msg), &field);
   if (size) {
     *size = arr ? arr->UPB_PRIVATE(size) : 0;
   }
   return arr;
 }
 UPB_INLINE upb_Array* _google_protobuf_FieldOptions_targets_mutable_upb_array(google_protobuf_FieldOptions* msg, size_t* size, upb_Arena* arena) {
-  const upb_MiniTableField field = {19, 32, 0, 6, 14, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_MiniTableField field = {19, 32, 0, 7, 14, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
   upb_Array* arr = upb_Message_GetOrCreateMutableArray(UPB_UPCAST(msg),
                                                        &field, arena);
   if (size) {
     *size = arr ? arr->UPB_PRIVATE(size) : 0;
   }
   return arr;
 }
@@ -4112,101 +4114,117 @@
                                     &default_val, &ret);
   return ret;
 }
 UPB_INLINE bool google_protobuf_FieldOptions_has_features(const google_protobuf_FieldOptions* msg) {
   const upb_MiniTableField field = {21, UPB_SIZE(40, 48), 73, 1, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
   return upb_Message_HasBaseField(UPB_UPCAST(msg), &field);
 }
+UPB_INLINE void google_protobuf_FieldOptions_clear_feature_support(google_protobuf_FieldOptions* msg) {
+  const upb_MiniTableField field = {22, UPB_SIZE(44, 56), 74, 2, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Message_ClearBaseField(UPB_UPCAST(msg), &field);
+}
+UPB_INLINE const google_protobuf_FieldOptions_FeatureSupport* google_protobuf_FieldOptions_feature_support(const google_protobuf_FieldOptions* msg) {
+  const google_protobuf_FieldOptions_FeatureSupport* default_val = NULL;
+  const google_protobuf_FieldOptions_FeatureSupport* ret;
+  const upb_MiniTableField field = {22, UPB_SIZE(44, 56), 74, 2, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  _upb_Message_GetNonExtensionField(UPB_UPCAST(msg), &field,
+                                    &default_val, &ret);
+  return ret;
+}
+UPB_INLINE bool google_protobuf_FieldOptions_has_feature_support(const google_protobuf_FieldOptions* msg) {
+  const upb_MiniTableField field = {22, UPB_SIZE(44, 56), 74, 2, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  return upb_Message_HasBaseField(UPB_UPCAST(msg), &field);
+}
 UPB_INLINE void google_protobuf_FieldOptions_clear_uninterpreted_option(google_protobuf_FieldOptions* msg) {
-  const upb_MiniTableField field = {999, UPB_SIZE(44, 56), 0, 2, 11, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_MiniTableField field = {999, UPB_SIZE(48, 64), 0, 3, 11, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
   upb_Message_ClearBaseField(UPB_UPCAST(msg), &field);
 }
 UPB_INLINE const google_protobuf_UninterpretedOption* const* google_protobuf_FieldOptions_uninterpreted_option(const google_protobuf_FieldOptions* msg, size_t* size) {
-  const upb_MiniTableField field = {999, UPB_SIZE(44, 56), 0, 2, 11, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_MiniTableField field = {999, UPB_SIZE(48, 64), 0, 3, 11, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
   const upb_Array* arr = upb_Message_GetArray(UPB_UPCAST(msg), &field);
   if (arr) {
     if (size) *size = arr->UPB_PRIVATE(size);
     return (const google_protobuf_UninterpretedOption* const*)upb_Array_DataPtr(arr);
   } else {
     if (size) *size = 0;
     return NULL;
   }
 }
 UPB_INLINE const upb_Array* _google_protobuf_FieldOptions_uninterpreted_option_upb_array(const google_protobuf_FieldOptions* msg, size_t* size) {
-  const upb_MiniTableField field = {999, UPB_SIZE(44, 56), 0, 2, 11, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_MiniTableField field = {999, UPB_SIZE(48, 64), 0, 3, 11, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
   const upb_Array* arr = upb_Message_GetArray(UPB_UPCAST(msg), &field);
   if (size) {
     *size = arr ? arr->UPB_PRIVATE(size) : 0;
   }
   return arr;
 }
 UPB_INLINE upb_Array* _google_protobuf_FieldOptions_uninterpreted_option_mutable_upb_array(google_protobuf_FieldOptions* msg, size_t* size, upb_Arena* arena) {
-  const upb_MiniTableField field = {999, UPB_SIZE(44, 56), 0, 2, 11, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_MiniTableField field = {999, UPB_SIZE(48, 64), 0, 3, 11, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
   upb_Array* arr = upb_Message_GetOrCreateMutableArray(UPB_UPCAST(msg),
                                                        &field, arena);
   if (size) {
     *size = arr ? arr->UPB_PRIVATE(size) : 0;
   }
   return arr;
 }
 
 UPB_INLINE void google_protobuf_FieldOptions_set_ctype(google_protobuf_FieldOptions *msg, int32_t value) {
-  const upb_MiniTableField field = {1, 12, 64, 3, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  const upb_MiniTableField field = {1, 12, 64, 4, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FieldOptions_set_packed(google_protobuf_FieldOptions *msg, bool value) {
   const upb_MiniTableField field = {2, 16, 65, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FieldOptions_set_deprecated(google_protobuf_FieldOptions *msg, bool value) {
   const upb_MiniTableField field = {3, 17, 66, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FieldOptions_set_lazy(google_protobuf_FieldOptions *msg, bool value) {
   const upb_MiniTableField field = {5, 18, 67, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FieldOptions_set_jstype(google_protobuf_FieldOptions *msg, int32_t value) {
-  const upb_MiniTableField field = {6, 20, 68, 4, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  const upb_MiniTableField field = {6, 20, 68, 5, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FieldOptions_set_weak(google_protobuf_FieldOptions *msg, bool value) {
   const upb_MiniTableField field = {10, 24, 69, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FieldOptions_set_unverified_lazy(google_protobuf_FieldOptions *msg, bool value) {
   const upb_MiniTableField field = {15, 25, 70, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FieldOptions_set_debug_redact(google_protobuf_FieldOptions *msg, bool value) {
   const upb_MiniTableField field = {16, 26, 71, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FieldOptions_set_retention(google_protobuf_FieldOptions *msg, int32_t value) {
-  const upb_MiniTableField field = {17, 28, 72, 5, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  const upb_MiniTableField field = {17, 28, 72, 6, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE int32_t* google_protobuf_FieldOptions_mutable_targets(google_protobuf_FieldOptions* msg, size_t* size) {
-  upb_MiniTableField field = {19, 32, 0, 6, 14, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_MiniTableField field = {19, 32, 0, 7, 14, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
   upb_Array* arr = upb_Message_GetMutableArray(UPB_UPCAST(msg), &field);
   if (arr) {
     if (size) *size = arr->UPB_PRIVATE(size);
     return (int32_t*)upb_Array_MutableDataPtr(arr);
   } else {
     if (size) *size = 0;
     return NULL;
   }
 }
 UPB_INLINE int32_t* google_protobuf_FieldOptions_resize_targets(google_protobuf_FieldOptions* msg, size_t size, upb_Arena* arena) {
-  upb_MiniTableField field = {19, 32, 0, 6, 14, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_MiniTableField field = {19, 32, 0, 7, 14, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
   return (int32_t*)upb_Message_ResizeArrayUninitialized(UPB_UPCAST(msg),
                                                    &field, size, arena);
 }
 UPB_INLINE bool google_protobuf_FieldOptions_add_targets(google_protobuf_FieldOptions* msg, int32_t val, upb_Arena* arena) {
-  upb_MiniTableField field = {19, 32, 0, 6, 14, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_MiniTableField field = {19, 32, 0, 7, 14, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
   upb_Array* arr = upb_Message_GetOrCreateMutableArray(
       UPB_UPCAST(msg), &field, arena);
   if (!arr || !UPB_PRIVATE(_upb_Array_ResizeUninitialized)(
                   arr, arr->UPB_PRIVATE(size) + 1, arena)) {
     return false;
   }
   UPB_PRIVATE(_upb_Array_Set)
@@ -4241,42 +4259,54 @@
   if (!arr || !sub) return NULL;
   UPB_PRIVATE(_upb_Array_Set)
   (arr, arr->UPB_PRIVATE(size) - 1, &sub, sizeof(sub));
   return sub;
 }
 UPB_INLINE void google_protobuf_FieldOptions_set_features(google_protobuf_FieldOptions *msg, google_protobuf_FeatureSet* value) {
   const upb_MiniTableField field = {21, UPB_SIZE(40, 48), 73, 1, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE struct google_protobuf_FeatureSet* google_protobuf_FieldOptions_mutable_features(google_protobuf_FieldOptions* msg, upb_Arena* arena) {
   struct google_protobuf_FeatureSet* sub = (struct google_protobuf_FeatureSet*)google_protobuf_FieldOptions_features(msg);
   if (sub == NULL) {
     sub = (struct google_protobuf_FeatureSet*)_upb_Message_New(&google__protobuf__FeatureSet_msg_init, arena);
     if (sub) google_protobuf_FieldOptions_set_features(msg, sub);
   }
   return sub;
 }
+UPB_INLINE void google_protobuf_FieldOptions_set_feature_support(google_protobuf_FieldOptions *msg, google_protobuf_FieldOptions_FeatureSupport* value) {
+  const upb_MiniTableField field = {22, UPB_SIZE(44, 56), 74, 2, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
+}
+UPB_INLINE struct google_protobuf_FieldOptions_FeatureSupport* google_protobuf_FieldOptions_mutable_feature_support(google_protobuf_FieldOptions* msg, upb_Arena* arena) {
+  struct google_protobuf_FieldOptions_FeatureSupport* sub = (struct google_protobuf_FieldOptions_FeatureSupport*)google_protobuf_FieldOptions_feature_support(msg);
+  if (sub == NULL) {
+    sub = (struct google_protobuf_FieldOptions_FeatureSupport*)_upb_Message_New(&google__protobuf__FieldOptions__FeatureSupport_msg_init, arena);
+    if (sub) google_protobuf_FieldOptions_set_feature_support(msg, sub);
+  }
+  return sub;
+}
 UPB_INLINE google_protobuf_UninterpretedOption** google_protobuf_FieldOptions_mutable_uninterpreted_option(google_protobuf_FieldOptions* msg, size_t* size) {
-  upb_MiniTableField field = {999, UPB_SIZE(44, 56), 0, 2, 11, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_MiniTableField field = {999, UPB_SIZE(48, 64), 0, 3, 11, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
   upb_Array* arr = upb_Message_GetMutableArray(UPB_UPCAST(msg), &field);
   if (arr) {
     if (size) *size = arr->UPB_PRIVATE(size);
     return (google_protobuf_UninterpretedOption**)upb_Array_MutableDataPtr(arr);
   } else {
     if (size) *size = 0;
     return NULL;
   }
 }
 UPB_INLINE google_protobuf_UninterpretedOption** google_protobuf_FieldOptions_resize_uninterpreted_option(google_protobuf_FieldOptions* msg, size_t size, upb_Arena* arena) {
-  upb_MiniTableField field = {999, UPB_SIZE(44, 56), 0, 2, 11, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_MiniTableField field = {999, UPB_SIZE(48, 64), 0, 3, 11, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
   return (google_protobuf_UninterpretedOption**)upb_Message_ResizeArrayUninitialized(UPB_UPCAST(msg),
                                                    &field, size, arena);
 }
 UPB_INLINE struct google_protobuf_UninterpretedOption* google_protobuf_FieldOptions_add_uninterpreted_option(google_protobuf_FieldOptions* msg, upb_Arena* arena) {
-  upb_MiniTableField field = {999, UPB_SIZE(44, 56), 0, 2, 11, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_MiniTableField field = {999, UPB_SIZE(48, 64), 0, 3, 11, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
   upb_Array* arr = upb_Message_GetOrCreateMutableArray(
       UPB_UPCAST(msg), &field, arena);
   if (!arr || !UPB_PRIVATE(_upb_Array_ResizeUninitialized)(
                   arr, arr->UPB_PRIVATE(size) + 1, arena)) {
     return NULL;
   }
   struct google_protobuf_UninterpretedOption* sub = (struct google_protobuf_UninterpretedOption*)_upb_Message_New(&google__protobuf__UninterpretedOption_msg_init, arena);
@@ -4353,19 +4383,137 @@
 UPB_INLINE bool google_protobuf_FieldOptions_EditionDefault_has_edition(const google_protobuf_FieldOptions_EditionDefault* msg) {
   const upb_MiniTableField field = {3, 12, 65, 0, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
   return upb_Message_HasBaseField(UPB_UPCAST(msg), &field);
 }
 
 UPB_INLINE void google_protobuf_FieldOptions_EditionDefault_set_value(google_protobuf_FieldOptions_EditionDefault *msg, upb_StringView value) {
   const upb_MiniTableField field = {2, 16, 64, kUpb_NoSub, 12, (int)kUpb_FieldMode_Scalar | (int)kUpb_LabelFlags_IsAlternate | ((int)kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FieldOptions_EditionDefault_set_edition(google_protobuf_FieldOptions_EditionDefault *msg, int32_t value) {
   const upb_MiniTableField field = {3, 12, 65, 0, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
+}
+
+/* google.protobuf.FieldOptions.FeatureSupport */
+
+UPB_INLINE google_protobuf_FieldOptions_FeatureSupport* google_protobuf_FieldOptions_FeatureSupport_new(upb_Arena* arena) {
+  return (google_protobuf_FieldOptions_FeatureSupport*)_upb_Message_New(&google__protobuf__FieldOptions__FeatureSupport_msg_init, arena);
+}
+UPB_INLINE google_protobuf_FieldOptions_FeatureSupport* google_protobuf_FieldOptions_FeatureSupport_parse(const char* buf, size_t size, upb_Arena* arena) {
+  google_protobuf_FieldOptions_FeatureSupport* ret = google_protobuf_FieldOptions_FeatureSupport_new(arena);
+  if (!ret) return NULL;
+  if (upb_Decode(buf, size, UPB_UPCAST(ret), &google__protobuf__FieldOptions__FeatureSupport_msg_init, NULL, 0, arena) !=
+      kUpb_DecodeStatus_Ok) {
+    return NULL;
+  }
+  return ret;
+}
+UPB_INLINE google_protobuf_FieldOptions_FeatureSupport* google_protobuf_FieldOptions_FeatureSupport_parse_ex(const char* buf, size_t size,
+                           const upb_ExtensionRegistry* extreg,
+                           int options, upb_Arena* arena) {
+  google_protobuf_FieldOptions_FeatureSupport* ret = google_protobuf_FieldOptions_FeatureSupport_new(arena);
+  if (!ret) return NULL;
+  if (upb_Decode(buf, size, UPB_UPCAST(ret), &google__protobuf__FieldOptions__FeatureSupport_msg_init, extreg, options,
+                 arena) != kUpb_DecodeStatus_Ok) {
+    return NULL;
+  }
+  return ret;
+}
+UPB_INLINE char* google_protobuf_FieldOptions_FeatureSupport_serialize(const google_protobuf_FieldOptions_FeatureSupport* msg, upb_Arena* arena, size_t* len) {
+  char* ptr;
+  (void)upb_Encode(UPB_UPCAST(msg), &google__protobuf__FieldOptions__FeatureSupport_msg_init, 0, arena, &ptr, len);
+  return ptr;
+}
+UPB_INLINE char* google_protobuf_FieldOptions_FeatureSupport_serialize_ex(const google_protobuf_FieldOptions_FeatureSupport* msg, int options,
+                                 upb_Arena* arena, size_t* len) {
+  char* ptr;
+  (void)upb_Encode(UPB_UPCAST(msg), &google__protobuf__FieldOptions__FeatureSupport_msg_init, options, arena, &ptr, len);
+  return ptr;
+}
+UPB_INLINE void google_protobuf_FieldOptions_FeatureSupport_clear_edition_introduced(google_protobuf_FieldOptions_FeatureSupport* msg) {
+  const upb_MiniTableField field = {1, 12, 64, 0, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
+  upb_Message_ClearBaseField(UPB_UPCAST(msg), &field);
+}
+UPB_INLINE int32_t google_protobuf_FieldOptions_FeatureSupport_edition_introduced(const google_protobuf_FieldOptions_FeatureSupport* msg) {
+  int32_t default_val = 0;
+  int32_t ret;
+  const upb_MiniTableField field = {1, 12, 64, 0, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
+  _upb_Message_GetNonExtensionField(UPB_UPCAST(msg), &field,
+                                    &default_val, &ret);
+  return ret;
+}
+UPB_INLINE bool google_protobuf_FieldOptions_FeatureSupport_has_edition_introduced(const google_protobuf_FieldOptions_FeatureSupport* msg) {
+  const upb_MiniTableField field = {1, 12, 64, 0, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
+  return upb_Message_HasBaseField(UPB_UPCAST(msg), &field);
+}
+UPB_INLINE void google_protobuf_FieldOptions_FeatureSupport_clear_edition_deprecated(google_protobuf_FieldOptions_FeatureSupport* msg) {
+  const upb_MiniTableField field = {2, 16, 65, 1, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
+  upb_Message_ClearBaseField(UPB_UPCAST(msg), &field);
+}
+UPB_INLINE int32_t google_protobuf_FieldOptions_FeatureSupport_edition_deprecated(const google_protobuf_FieldOptions_FeatureSupport* msg) {
+  int32_t default_val = 0;
+  int32_t ret;
+  const upb_MiniTableField field = {2, 16, 65, 1, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
+  _upb_Message_GetNonExtensionField(UPB_UPCAST(msg), &field,
+                                    &default_val, &ret);
+  return ret;
+}
+UPB_INLINE bool google_protobuf_FieldOptions_FeatureSupport_has_edition_deprecated(const google_protobuf_FieldOptions_FeatureSupport* msg) {
+  const upb_MiniTableField field = {2, 16, 65, 1, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
+  return upb_Message_HasBaseField(UPB_UPCAST(msg), &field);
+}
+UPB_INLINE void google_protobuf_FieldOptions_FeatureSupport_clear_deprecation_warning(google_protobuf_FieldOptions_FeatureSupport* msg) {
+  const upb_MiniTableField field = {3, 24, 66, kUpb_NoSub, 12, (int)kUpb_FieldMode_Scalar | (int)kUpb_LabelFlags_IsAlternate | ((int)kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
+  upb_Message_ClearBaseField(UPB_UPCAST(msg), &field);
+}
+UPB_INLINE upb_StringView google_protobuf_FieldOptions_FeatureSupport_deprecation_warning(const google_protobuf_FieldOptions_FeatureSupport* msg) {
+  upb_StringView default_val = upb_StringView_FromString("");
+  upb_StringView ret;
+  const upb_MiniTableField field = {3, 24, 66, kUpb_NoSub, 12, (int)kUpb_FieldMode_Scalar | (int)kUpb_LabelFlags_IsAlternate | ((int)kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
+  _upb_Message_GetNonExtensionField(UPB_UPCAST(msg), &field,
+                                    &default_val, &ret);
+  return ret;
+}
+UPB_INLINE bool google_protobuf_FieldOptions_FeatureSupport_has_deprecation_warning(const google_protobuf_FieldOptions_FeatureSupport* msg) {
+  const upb_MiniTableField field = {3, 24, 66, kUpb_NoSub, 12, (int)kUpb_FieldMode_Scalar | (int)kUpb_LabelFlags_IsAlternate | ((int)kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
+  return upb_Message_HasBaseField(UPB_UPCAST(msg), &field);
+}
+UPB_INLINE void google_protobuf_FieldOptions_FeatureSupport_clear_edition_removed(google_protobuf_FieldOptions_FeatureSupport* msg) {
+  const upb_MiniTableField field = {4, 20, 67, 2, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
+  upb_Message_ClearBaseField(UPB_UPCAST(msg), &field);
+}
+UPB_INLINE int32_t google_protobuf_FieldOptions_FeatureSupport_edition_removed(const google_protobuf_FieldOptions_FeatureSupport* msg) {
+  int32_t default_val = 0;
+  int32_t ret;
+  const upb_MiniTableField field = {4, 20, 67, 2, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
+  _upb_Message_GetNonExtensionField(UPB_UPCAST(msg), &field,
+                                    &default_val, &ret);
+  return ret;
+}
+UPB_INLINE bool google_protobuf_FieldOptions_FeatureSupport_has_edition_removed(const google_protobuf_FieldOptions_FeatureSupport* msg) {
+  const upb_MiniTableField field = {4, 20, 67, 2, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
+  return upb_Message_HasBaseField(UPB_UPCAST(msg), &field);
+}
+
+UPB_INLINE void google_protobuf_FieldOptions_FeatureSupport_set_edition_introduced(google_protobuf_FieldOptions_FeatureSupport *msg, int32_t value) {
+  const upb_MiniTableField field = {1, 12, 64, 0, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
+}
+UPB_INLINE void google_protobuf_FieldOptions_FeatureSupport_set_edition_deprecated(google_protobuf_FieldOptions_FeatureSupport *msg, int32_t value) {
+  const upb_MiniTableField field = {2, 16, 65, 1, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
+}
+UPB_INLINE void google_protobuf_FieldOptions_FeatureSupport_set_deprecation_warning(google_protobuf_FieldOptions_FeatureSupport *msg, upb_StringView value) {
+  const upb_MiniTableField field = {3, 24, 66, kUpb_NoSub, 12, (int)kUpb_FieldMode_Scalar | (int)kUpb_LabelFlags_IsAlternate | ((int)kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
+}
+UPB_INLINE void google_protobuf_FieldOptions_FeatureSupport_set_edition_removed(google_protobuf_FieldOptions_FeatureSupport *msg, int32_t value) {
+  const upb_MiniTableField field = {4, 20, 67, 2, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 
 /* google.protobuf.OneofOptions */
 
 UPB_INLINE google_protobuf_OneofOptions* google_protobuf_OneofOptions_new(upb_Arena* arena) {
   return (google_protobuf_OneofOptions*)_upb_Message_New(&google__protobuf__OneofOptions_msg_init, arena);
 }
@@ -4447,15 +4595,15 @@
     *size = arr ? arr->UPB_PRIVATE(size) : 0;
   }
   return arr;
 }
 
 UPB_INLINE void google_protobuf_OneofOptions_set_features(google_protobuf_OneofOptions *msg, google_protobuf_FeatureSet* value) {
   const upb_MiniTableField field = {1, UPB_SIZE(12, 16), 64, 0, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE struct google_protobuf_FeatureSet* google_protobuf_OneofOptions_mutable_features(google_protobuf_OneofOptions* msg, upb_Arena* arena) {
   struct google_protobuf_FeatureSet* sub = (struct google_protobuf_FeatureSet*)google_protobuf_OneofOptions_features(msg);
   if (sub == NULL) {
     sub = (struct google_protobuf_FeatureSet*)_upb_Message_New(&google__protobuf__FeatureSet_msg_init, arena);
     if (sub) google_protobuf_OneofOptions_set_features(msg, sub);
   }
@@ -4623,27 +4771,27 @@
     *size = arr ? arr->UPB_PRIVATE(size) : 0;
   }
   return arr;
 }
 
 UPB_INLINE void google_protobuf_EnumOptions_set_allow_alias(google_protobuf_EnumOptions *msg, bool value) {
   const upb_MiniTableField field = {2, 9, 64, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_EnumOptions_set_deprecated(google_protobuf_EnumOptions *msg, bool value) {
   const upb_MiniTableField field = {3, 10, 65, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_EnumOptions_set_deprecated_legacy_json_field_conflicts(google_protobuf_EnumOptions *msg, bool value) {
   const upb_MiniTableField field = {6, 11, 66, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_EnumOptions_set_features(google_protobuf_EnumOptions *msg, google_protobuf_FeatureSet* value) {
   const upb_MiniTableField field = {7, UPB_SIZE(12, 16), 67, 0, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE struct google_protobuf_FeatureSet* google_protobuf_EnumOptions_mutable_features(google_protobuf_EnumOptions* msg, upb_Arena* arena) {
   struct google_protobuf_FeatureSet* sub = (struct google_protobuf_FeatureSet*)google_protobuf_EnumOptions_features(msg);
   if (sub == NULL) {
     sub = (struct google_protobuf_FeatureSet*)_upb_Message_New(&google__protobuf__FeatureSet_msg_init, arena);
     if (sub) google_protobuf_EnumOptions_set_features(msg, sub);
   }
@@ -4795,31 +4943,31 @@
     *size = arr ? arr->UPB_PRIVATE(size) : 0;
   }
   return arr;
 }
 
 UPB_INLINE void google_protobuf_EnumValueOptions_set_deprecated(google_protobuf_EnumValueOptions *msg, bool value) {
   const upb_MiniTableField field = {1, 9, 64, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_EnumValueOptions_set_features(google_protobuf_EnumValueOptions *msg, google_protobuf_FeatureSet* value) {
   const upb_MiniTableField field = {2, UPB_SIZE(12, 16), 65, 0, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE struct google_protobuf_FeatureSet* google_protobuf_EnumValueOptions_mutable_features(google_protobuf_EnumValueOptions* msg, upb_Arena* arena) {
   struct google_protobuf_FeatureSet* sub = (struct google_protobuf_FeatureSet*)google_protobuf_EnumValueOptions_features(msg);
   if (sub == NULL) {
     sub = (struct google_protobuf_FeatureSet*)_upb_Message_New(&google__protobuf__FeatureSet_msg_init, arena);
     if (sub) google_protobuf_EnumValueOptions_set_features(msg, sub);
   }
   return sub;
 }
 UPB_INLINE void google_protobuf_EnumValueOptions_set_debug_redact(google_protobuf_EnumValueOptions *msg, bool value) {
   const upb_MiniTableField field = {3, UPB_SIZE(16, 10), 66, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE google_protobuf_UninterpretedOption** google_protobuf_EnumValueOptions_mutable_uninterpreted_option(google_protobuf_EnumValueOptions* msg, size_t* size) {
   upb_MiniTableField field = {999, UPB_SIZE(20, 24), 0, 1, 11, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
   upb_Array* arr = upb_Message_GetMutableArray(UPB_UPCAST(msg), &field);
   if (arr) {
     if (size) *size = arr->UPB_PRIVATE(size);
     return (google_protobuf_UninterpretedOption**)upb_Array_MutableDataPtr(arr);
@@ -4947,19 +5095,19 @@
     *size = arr ? arr->UPB_PRIVATE(size) : 0;
   }
   return arr;
 }
 
 UPB_INLINE void google_protobuf_ServiceOptions_set_deprecated(google_protobuf_ServiceOptions *msg, bool value) {
   const upb_MiniTableField field = {33, 9, 64, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_ServiceOptions_set_features(google_protobuf_ServiceOptions *msg, google_protobuf_FeatureSet* value) {
   const upb_MiniTableField field = {34, UPB_SIZE(12, 16), 65, 0, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE struct google_protobuf_FeatureSet* google_protobuf_ServiceOptions_mutable_features(google_protobuf_ServiceOptions* msg, upb_Arena* arena) {
   struct google_protobuf_FeatureSet* sub = (struct google_protobuf_FeatureSet*)google_protobuf_ServiceOptions_features(msg);
   if (sub == NULL) {
     sub = (struct google_protobuf_FeatureSet*)_upb_Message_New(&google__protobuf__FeatureSet_msg_init, arena);
     if (sub) google_protobuf_ServiceOptions_set_features(msg, sub);
   }
@@ -5111,23 +5259,23 @@
     *size = arr ? arr->UPB_PRIVATE(size) : 0;
   }
   return arr;
 }
 
 UPB_INLINE void google_protobuf_MethodOptions_set_deprecated(google_protobuf_MethodOptions *msg, bool value) {
   const upb_MiniTableField field = {33, 9, 64, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_MethodOptions_set_idempotency_level(google_protobuf_MethodOptions *msg, int32_t value) {
   const upb_MiniTableField field = {34, 12, 65, 2, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_MethodOptions_set_features(google_protobuf_MethodOptions *msg, google_protobuf_FeatureSet* value) {
   const upb_MiniTableField field = {35, 16, 66, 0, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE struct google_protobuf_FeatureSet* google_protobuf_MethodOptions_mutable_features(google_protobuf_MethodOptions* msg, upb_Arena* arena) {
   struct google_protobuf_FeatureSet* sub = (struct google_protobuf_FeatureSet*)google_protobuf_MethodOptions_features(msg);
   if (sub == NULL) {
     sub = (struct google_protobuf_FeatureSet*)_upb_Message_New(&google__protobuf__FeatureSet_msg_init, arena);
     if (sub) google_protobuf_MethodOptions_set_features(msg, sub);
   }
@@ -5357,35 +5505,35 @@
   if (!arr || !sub) return NULL;
   UPB_PRIVATE(_upb_Array_Set)
   (arr, arr->UPB_PRIVATE(size) - 1, &sub, sizeof(sub));
   return sub;
 }
 UPB_INLINE void google_protobuf_UninterpretedOption_set_identifier_value(google_protobuf_UninterpretedOption *msg, upb_StringView value) {
   const upb_MiniTableField field = {3, UPB_SIZE(16, 24), 64, kUpb_NoSub, 12, (int)kUpb_FieldMode_Scalar | (int)kUpb_LabelFlags_IsAlternate | ((int)kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_UninterpretedOption_set_positive_int_value(google_protobuf_UninterpretedOption *msg, uint64_t value) {
   const upb_MiniTableField field = {4, UPB_SIZE(24, 40), 65, kUpb_NoSub, 4, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_8Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_UninterpretedOption_set_negative_int_value(google_protobuf_UninterpretedOption *msg, int64_t value) {
   const upb_MiniTableField field = {5, UPB_SIZE(32, 48), 66, kUpb_NoSub, 3, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_8Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_UninterpretedOption_set_double_value(google_protobuf_UninterpretedOption *msg, double value) {
   const upb_MiniTableField field = {6, UPB_SIZE(40, 56), 67, kUpb_NoSub, 1, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_8Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_UninterpretedOption_set_string_value(google_protobuf_UninterpretedOption *msg, upb_StringView value) {
   const upb_MiniTableField field = {7, UPB_SIZE(48, 64), 68, kUpb_NoSub, 12, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_UninterpretedOption_set_aggregate_value(google_protobuf_UninterpretedOption *msg, upb_StringView value) {
   const upb_MiniTableField field = {8, UPB_SIZE(56, 80), 69, kUpb_NoSub, 12, (int)kUpb_FieldMode_Scalar | (int)kUpb_LabelFlags_IsAlternate | ((int)kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 
 /* google.protobuf.UninterpretedOption.NamePart */
 
 UPB_INLINE google_protobuf_UninterpretedOption_NamePart* google_protobuf_UninterpretedOption_NamePart_new(upb_Arena* arena) {
   return (google_protobuf_UninterpretedOption_NamePart*)_upb_Message_New(&google__protobuf__UninterpretedOption__NamePart_msg_init, arena);
 }
@@ -5451,19 +5599,19 @@
 UPB_INLINE bool google_protobuf_UninterpretedOption_NamePart_has_is_extension(const google_protobuf_UninterpretedOption_NamePart* msg) {
   const upb_MiniTableField field = {2, 9, 65, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
   return upb_Message_HasBaseField(UPB_UPCAST(msg), &field);
 }
 
 UPB_INLINE void google_protobuf_UninterpretedOption_NamePart_set_name_part(google_protobuf_UninterpretedOption_NamePart *msg, upb_StringView value) {
   const upb_MiniTableField field = {1, UPB_SIZE(12, 16), 64, kUpb_NoSub, 12, (int)kUpb_FieldMode_Scalar | (int)kUpb_LabelFlags_IsAlternate | ((int)kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_UninterpretedOption_NamePart_set_is_extension(google_protobuf_UninterpretedOption_NamePart *msg, bool value) {
   const upb_MiniTableField field = {2, 9, 65, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 
 /* google.protobuf.FeatureSet */
 
 UPB_INLINE google_protobuf_FeatureSet* google_protobuf_FeatureSet_new(upb_Arena* arena) {
   return (google_protobuf_FeatureSet*)_upb_Message_New(&google__protobuf__FeatureSet_msg_init, arena);
 }
@@ -5593,35 +5741,35 @@
 UPB_INLINE bool google_protobuf_FeatureSet_has_json_format(const google_protobuf_FeatureSet* msg) {
   const upb_MiniTableField field = {6, 32, 69, 5, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
   return upb_Message_HasBaseField(UPB_UPCAST(msg), &field);
 }
 
 UPB_INLINE void google_protobuf_FeatureSet_set_field_presence(google_protobuf_FeatureSet *msg, int32_t value) {
   const upb_MiniTableField field = {1, 12, 64, 0, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FeatureSet_set_enum_type(google_protobuf_FeatureSet *msg, int32_t value) {
   const upb_MiniTableField field = {2, 16, 65, 1, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FeatureSet_set_repeated_field_encoding(google_protobuf_FeatureSet *msg, int32_t value) {
   const upb_MiniTableField field = {3, 20, 66, 2, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FeatureSet_set_utf8_validation(google_protobuf_FeatureSet *msg, int32_t value) {
   const upb_MiniTableField field = {4, 24, 67, 3, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FeatureSet_set_message_encoding(google_protobuf_FeatureSet *msg, int32_t value) {
   const upb_MiniTableField field = {5, 28, 68, 4, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FeatureSet_set_json_format(google_protobuf_FeatureSet *msg, int32_t value) {
   const upb_MiniTableField field = {6, 32, 69, 5, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 
 /* google.protobuf.FeatureSetDefaults */
 
 UPB_INLINE google_protobuf_FeatureSetDefaults* google_protobuf_FeatureSetDefaults_new(upb_Arena* arena) {
   return (google_protobuf_FeatureSetDefaults*)_upb_Message_New(&google__protobuf__FeatureSetDefaults_msg_init, arena);
 }
@@ -5749,19 +5897,19 @@
   if (!arr || !sub) return NULL;
   UPB_PRIVATE(_upb_Array_Set)
   (arr, arr->UPB_PRIVATE(size) - 1, &sub, sizeof(sub));
   return sub;
 }
 UPB_INLINE void google_protobuf_FeatureSetDefaults_set_minimum_edition(google_protobuf_FeatureSetDefaults *msg, int32_t value) {
   const upb_MiniTableField field = {4, UPB_SIZE(16, 12), 64, 1, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FeatureSetDefaults_set_maximum_edition(google_protobuf_FeatureSetDefaults *msg, int32_t value) {
   const upb_MiniTableField field = {5, UPB_SIZE(20, 16), 65, 2, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 
 /* google.protobuf.FeatureSetDefaults.FeatureSetEditionDefault */
 
 UPB_INLINE google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault* google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault_new(upb_Arena* arena) {
   return (google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault*)_upb_Message_New(&google__protobuf__FeatureSetDefaults__FeatureSetEditionDefault_msg_init, arena);
 }
@@ -5792,62 +5940,90 @@
 }
 UPB_INLINE char* google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault_serialize_ex(const google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault* msg, int options,
                                  upb_Arena* arena, size_t* len) {
   char* ptr;
   (void)upb_Encode(UPB_UPCAST(msg), &google__protobuf__FeatureSetDefaults__FeatureSetEditionDefault_msg_init, options, arena, &ptr, len);
   return ptr;
 }
-UPB_INLINE void google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault_clear_features(google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault* msg) {
-  const upb_MiniTableField field = {2, UPB_SIZE(12, 16), 64, 0, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+UPB_INLINE void google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault_clear_edition(google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault* msg) {
+  const upb_MiniTableField field = {3, 12, 64, 2, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
   upb_Message_ClearBaseField(UPB_UPCAST(msg), &field);
 }
-UPB_INLINE const google_protobuf_FeatureSet* google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault_features(const google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault* msg) {
+UPB_INLINE int32_t google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault_edition(const google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault* msg) {
+  int32_t default_val = 0;
+  int32_t ret;
+  const upb_MiniTableField field = {3, 12, 64, 2, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
+  _upb_Message_GetNonExtensionField(UPB_UPCAST(msg), &field,
+                                    &default_val, &ret);
+  return ret;
+}
+UPB_INLINE bool google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault_has_edition(const google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault* msg) {
+  const upb_MiniTableField field = {3, 12, 64, 2, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
+  return upb_Message_HasBaseField(UPB_UPCAST(msg), &field);
+}
+UPB_INLINE void google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault_clear_overridable_features(google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault* msg) {
+  const upb_MiniTableField field = {4, 16, 65, 0, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Message_ClearBaseField(UPB_UPCAST(msg), &field);
+}
+UPB_INLINE const google_protobuf_FeatureSet* google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault_overridable_features(const google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault* msg) {
   const google_protobuf_FeatureSet* default_val = NULL;
   const google_protobuf_FeatureSet* ret;
-  const upb_MiniTableField field = {2, UPB_SIZE(12, 16), 64, 0, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_MiniTableField field = {4, 16, 65, 0, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
   _upb_Message_GetNonExtensionField(UPB_UPCAST(msg), &field,
                                     &default_val, &ret);
   return ret;
 }
-UPB_INLINE bool google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault_has_features(const google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault* msg) {
-  const upb_MiniTableField field = {2, UPB_SIZE(12, 16), 64, 0, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+UPB_INLINE bool google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault_has_overridable_features(const google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault* msg) {
+  const upb_MiniTableField field = {4, 16, 65, 0, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
   return upb_Message_HasBaseField(UPB_UPCAST(msg), &field);
 }
-UPB_INLINE void google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault_clear_edition(google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault* msg) {
-  const upb_MiniTableField field = {3, UPB_SIZE(16, 12), 65, 1, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
+UPB_INLINE void google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault_clear_fixed_features(google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault* msg) {
+  const upb_MiniTableField field = {5, UPB_SIZE(20, 24), 66, 1, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
   upb_Message_ClearBaseField(UPB_UPCAST(msg), &field);
 }
-UPB_INLINE int32_t google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault_edition(const google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault* msg) {
-  int32_t default_val = 0;
-  int32_t ret;
-  const upb_MiniTableField field = {3, UPB_SIZE(16, 12), 65, 1, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
+UPB_INLINE const google_protobuf_FeatureSet* google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault_fixed_features(const google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault* msg) {
+  const google_protobuf_FeatureSet* default_val = NULL;
+  const google_protobuf_FeatureSet* ret;
+  const upb_MiniTableField field = {5, UPB_SIZE(20, 24), 66, 1, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
   _upb_Message_GetNonExtensionField(UPB_UPCAST(msg), &field,
                                     &default_val, &ret);
   return ret;
 }
-UPB_INLINE bool google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault_has_edition(const google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault* msg) {
-  const upb_MiniTableField field = {3, UPB_SIZE(16, 12), 65, 1, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
+UPB_INLINE bool google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault_has_fixed_features(const google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault* msg) {
+  const upb_MiniTableField field = {5, UPB_SIZE(20, 24), 66, 1, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
   return upb_Message_HasBaseField(UPB_UPCAST(msg), &field);
 }
 
-UPB_INLINE void google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault_set_features(google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault *msg, google_protobuf_FeatureSet* value) {
-  const upb_MiniTableField field = {2, UPB_SIZE(12, 16), 64, 0, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+UPB_INLINE void google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault_set_edition(google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault *msg, int32_t value) {
+  const upb_MiniTableField field = {3, 12, 64, 2, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
-UPB_INLINE struct google_protobuf_FeatureSet* google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault_mutable_features(google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault* msg, upb_Arena* arena) {
-  struct google_protobuf_FeatureSet* sub = (struct google_protobuf_FeatureSet*)google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault_features(msg);
+UPB_INLINE void google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault_set_overridable_features(google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault *msg, google_protobuf_FeatureSet* value) {
+  const upb_MiniTableField field = {4, 16, 65, 0, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
+}
+UPB_INLINE struct google_protobuf_FeatureSet* google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault_mutable_overridable_features(google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault* msg, upb_Arena* arena) {
+  struct google_protobuf_FeatureSet* sub = (struct google_protobuf_FeatureSet*)google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault_overridable_features(msg);
   if (sub == NULL) {
     sub = (struct google_protobuf_FeatureSet*)_upb_Message_New(&google__protobuf__FeatureSet_msg_init, arena);
-    if (sub) google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault_set_features(msg, sub);
+    if (sub) google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault_set_overridable_features(msg, sub);
   }
   return sub;
 }
-UPB_INLINE void google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault_set_edition(google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault *msg, int32_t value) {
-  const upb_MiniTableField field = {3, UPB_SIZE(16, 12), 65, 1, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+UPB_INLINE void google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault_set_fixed_features(google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault *msg, google_protobuf_FeatureSet* value) {
+  const upb_MiniTableField field = {5, UPB_SIZE(20, 24), 66, 1, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
+}
+UPB_INLINE struct google_protobuf_FeatureSet* google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault_mutable_fixed_features(google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault* msg, upb_Arena* arena) {
+  struct google_protobuf_FeatureSet* sub = (struct google_protobuf_FeatureSet*)google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault_fixed_features(msg);
+  if (sub == NULL) {
+    sub = (struct google_protobuf_FeatureSet*)_upb_Message_New(&google__protobuf__FeatureSet_msg_init, arena);
+    if (sub) google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault_set_fixed_features(msg, sub);
+  }
+  return sub;
 }
 
 /* google.protobuf.SourceCodeInfo */
 
 UPB_INLINE google_protobuf_SourceCodeInfo* google_protobuf_SourceCodeInfo_new(upb_Arena* arena) {
   return (google_protobuf_SourceCodeInfo*)_upb_Message_New(&google__protobuf__SourceCodeInfo_msg_init, arena);
 }
@@ -6165,19 +6341,19 @@
   }
   UPB_PRIVATE(_upb_Array_Set)
   (arr, arr->UPB_PRIVATE(size) - 1, &val, sizeof(val));
   return true;
 }
 UPB_INLINE void google_protobuf_SourceCodeInfo_Location_set_leading_comments(google_protobuf_SourceCodeInfo_Location *msg, upb_StringView value) {
   const upb_MiniTableField field = {3, UPB_SIZE(24, 32), 64, kUpb_NoSub, 12, (int)kUpb_FieldMode_Scalar | (int)kUpb_LabelFlags_IsAlternate | ((int)kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_SourceCodeInfo_Location_set_trailing_comments(google_protobuf_SourceCodeInfo_Location *msg, upb_StringView value) {
   const upb_MiniTableField field = {4, UPB_SIZE(32, 48), 65, kUpb_NoSub, 12, (int)kUpb_FieldMode_Scalar | (int)kUpb_LabelFlags_IsAlternate | ((int)kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE upb_StringView* google_protobuf_SourceCodeInfo_Location_mutable_leading_detached_comments(google_protobuf_SourceCodeInfo_Location* msg, size_t* size) {
   upb_MiniTableField field = {6, UPB_SIZE(20, 64), 0, kUpb_NoSub, 12, (int)kUpb_FieldMode_Array | (int)kUpb_LabelFlags_IsAlternate | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
   upb_Array* arr = upb_Message_GetMutableArray(UPB_UPCAST(msg), &field);
   if (arr) {
     if (size) *size = arr->UPB_PRIVATE(size);
     return (upb_StringView*)upb_Array_MutableDataPtr(arr);
@@ -6463,27 +6639,27 @@
   }
   UPB_PRIVATE(_upb_Array_Set)
   (arr, arr->UPB_PRIVATE(size) - 1, &val, sizeof(val));
   return true;
 }
 UPB_INLINE void google_protobuf_GeneratedCodeInfo_Annotation_set_source_file(google_protobuf_GeneratedCodeInfo_Annotation *msg, upb_StringView value) {
   const upb_MiniTableField field = {2, UPB_SIZE(28, 32), 64, kUpb_NoSub, 12, (int)kUpb_FieldMode_Scalar | (int)kUpb_LabelFlags_IsAlternate | ((int)kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_GeneratedCodeInfo_Annotation_set_begin(google_protobuf_GeneratedCodeInfo_Annotation *msg, int32_t value) {
   const upb_MiniTableField field = {3, UPB_SIZE(16, 12), 65, kUpb_NoSub, 5, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_GeneratedCodeInfo_Annotation_set_end(google_protobuf_GeneratedCodeInfo_Annotation *msg, int32_t value) {
   const upb_MiniTableField field = {4, UPB_SIZE(20, 16), 66, kUpb_NoSub, 5, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_GeneratedCodeInfo_Annotation_set_semantic(google_protobuf_GeneratedCodeInfo_Annotation *msg, int32_t value) {
   const upb_MiniTableField field = {5, UPB_SIZE(24, 20), 67, 0, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
-  _upb_Message_SetNonExtensionField((upb_Message *)msg, &field, &value);
+  upb_Message_SetBaseField((upb_Message *)msg, &field, &value);
 }
 
 /* Max size 32 is google.protobuf.FileOptions */
 /* Max size 64 is google.protobuf.FileOptions */
 #define _UPB_MAXOPT_SIZE UPB_SIZE(112, 200)
 
 #ifdef __cplusplus
```

### Comparing `protobuf-5.26.1/google/protobuf/descriptor.upb_minitable.c` & `protobuf-5.27.0rc1/google/protobuf/descriptor.upb_minitable.c`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,17 @@
   {1, 8, 0, 0, 11, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)},
 };
 
 const upb_MiniTable google__protobuf__FileDescriptorSet_msg_init = {
   &google_protobuf_FileDescriptorSet_submsgs[0],
   &google_protobuf_FileDescriptorSet__fields[0],
   16, 1, kUpb_ExtMode_NonExtendable, 1, UPB_FASTTABLE_MASK(8), 0,
+#ifdef UPB_TRACING_ENABLED
+  "google.protobuf.FileDescriptorSet",
+#endif
   UPB_FASTTABLE_INIT({
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x000800003f00000a, &upb_prm_1bt_max192b},
   })
 };
 
 static const upb_MiniTableSub google_protobuf_FileDescriptorProto_submsgs[7] = {
@@ -56,14 +59,17 @@
   {14, UPB_SIZE(48, 12), 69, 6, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)},
 };
 
 const upb_MiniTable google__protobuf__FileDescriptorProto_msg_init = {
   &google_protobuf_FileDescriptorProto_submsgs[0],
   &google_protobuf_FileDescriptorProto__fields[0],
   UPB_SIZE(80, 136), 13, kUpb_ExtMode_NonExtendable, 12, UPB_FASTTABLE_MASK(120), 0,
+#ifdef UPB_TRACING_ENABLED
+  "google.protobuf.FileDescriptorProto",
+#endif
   UPB_FASTTABLE_INIT({
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x003000003f00001a, &upb_prs_1bt},
     {0x003800003f000022, &upb_prm_1bt_max128b},
     {0x004000003f01002a, &upb_prm_1bt_max128b},
@@ -104,14 +110,17 @@
   {10, UPB_SIZE(44, 96), 0, kUpb_NoSub, 12, (int)kUpb_FieldMode_Array | (int)kUpb_LabelFlags_IsAlternate | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)},
 };
 
 const upb_MiniTable google__protobuf__DescriptorProto_msg_init = {
   &google_protobuf_DescriptorProto_submsgs[0],
   &google_protobuf_DescriptorProto__fields[0],
   UPB_SIZE(56, 104), 10, kUpb_ExtMode_NonExtendable, 10, UPB_FASTTABLE_MASK(120), 0,
+#ifdef UPB_TRACING_ENABLED
+  "google.protobuf.DescriptorProto",
+#endif
   UPB_FASTTABLE_INIT({
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x002000003f000012, &upb_prm_1bt_max128b},
     {0x002800003f01001a, &upb_prm_1bt_max128b},
     {0x003000003f020022, &upb_prm_1bt_max128b},
     {0x003800003f03002a, &upb_prm_1bt_max64b},
@@ -138,25 +147,31 @@
   {3, UPB_SIZE(20, 24), 66, 0, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)},
 };
 
 const upb_MiniTable google__protobuf__DescriptorProto__ExtensionRange_msg_init = {
   &google_protobuf_DescriptorProto_ExtensionRange_submsgs[0],
   &google_protobuf_DescriptorProto_ExtensionRange__fields[0],
   UPB_SIZE(24, 32), 3, kUpb_ExtMode_NonExtendable, 3, UPB_FASTTABLE_MASK(255), 0,
+#ifdef UPB_TRACING_ENABLED
+  "google.protobuf.DescriptorProto.ExtensionRange",
+#endif
 };
 
 static const upb_MiniTableField google_protobuf_DescriptorProto_ReservedRange__fields[2] = {
   {1, 12, 64, kUpb_NoSub, 5, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)},
   {2, 16, 65, kUpb_NoSub, 5, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)},
 };
 
 const upb_MiniTable google__protobuf__DescriptorProto__ReservedRange_msg_init = {
   NULL,
   &google_protobuf_DescriptorProto_ReservedRange__fields[0],
   24, 2, kUpb_ExtMode_NonExtendable, 2, UPB_FASTTABLE_MASK(255), 0,
+#ifdef UPB_TRACING_ENABLED
+  "google.protobuf.DescriptorProto.ReservedRange",
+#endif
 };
 
 static const upb_MiniTableSub google_protobuf_ExtensionRangeOptions_submsgs[4] = {
   {.UPB_PRIVATE(submsg) = &google__protobuf__ExtensionRangeOptions__Declaration_msg_init},
   {.UPB_PRIVATE(submsg) = &google__protobuf__FeatureSet_msg_init},
   {.UPB_PRIVATE(submsg) = &google__protobuf__UninterpretedOption_msg_init},
   {.UPB_PRIVATE(subenum) = &google_protobuf_ExtensionRangeOptions_VerificationState_enum_init},
@@ -169,14 +184,17 @@
   {999, UPB_SIZE(24, 32), 0, 2, 11, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)},
 };
 
 const upb_MiniTable google__protobuf__ExtensionRangeOptions_msg_init = {
   &google_protobuf_ExtensionRangeOptions_submsgs[0],
   &google_protobuf_ExtensionRangeOptions__fields[0],
   UPB_SIZE(32, 40), 4, kUpb_ExtMode_Extendable, 0, UPB_FASTTABLE_MASK(248), 0,
+#ifdef UPB_TRACING_ENABLED
+  "google.protobuf.ExtensionRangeOptions",
+#endif
   UPB_FASTTABLE_INIT({
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x001000003f000012, &upb_prm_1bt_max64b},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
@@ -217,14 +235,17 @@
   {6, 17, 68, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)},
 };
 
 const upb_MiniTable google__protobuf__ExtensionRangeOptions__Declaration_msg_init = {
   NULL,
   &google_protobuf_ExtensionRangeOptions_Declaration__fields[0],
   UPB_SIZE(40, 56), 5, kUpb_ExtMode_NonExtendable, 3, UPB_FASTTABLE_MASK(255), 0,
+#ifdef UPB_TRACING_ENABLED
+  "google.protobuf.ExtensionRangeOptions.Declaration",
+#endif
 };
 
 static const upb_MiniTableSub google_protobuf_FieldDescriptorProto_submsgs[3] = {
   {.UPB_PRIVATE(submsg) = &google__protobuf__FieldOptions_msg_init},
   {.UPB_PRIVATE(subenum) = &google_protobuf_FieldDescriptorProto_Label_enum_init},
   {.UPB_PRIVATE(subenum) = &google_protobuf_FieldDescriptorProto_Type_enum_init},
 };
@@ -243,14 +264,17 @@
   {17, UPB_SIZE(32, 28), 74, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)},
 };
 
 const upb_MiniTable google__protobuf__FieldDescriptorProto_msg_init = {
   &google_protobuf_FieldDescriptorProto_submsgs[0],
   &google_protobuf_FieldDescriptorProto__fields[0],
   UPB_SIZE(80, 120), 11, kUpb_ExtMode_NonExtendable, 10, UPB_FASTTABLE_MASK(255), 0,
+#ifdef UPB_TRACING_ENABLED
+  "google.protobuf.FieldDescriptorProto",
+#endif
 };
 
 static const upb_MiniTableSub google_protobuf_OneofDescriptorProto_submsgs[1] = {
   {.UPB_PRIVATE(submsg) = &google__protobuf__OneofOptions_msg_init},
 };
 
 static const upb_MiniTableField google_protobuf_OneofDescriptorProto__fields[2] = {
@@ -258,14 +282,17 @@
   {2, UPB_SIZE(12, 32), 65, 0, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)},
 };
 
 const upb_MiniTable google__protobuf__OneofDescriptorProto_msg_init = {
   &google_protobuf_OneofDescriptorProto_submsgs[0],
   &google_protobuf_OneofDescriptorProto__fields[0],
   UPB_SIZE(24, 40), 2, kUpb_ExtMode_NonExtendable, 2, UPB_FASTTABLE_MASK(255), 0,
+#ifdef UPB_TRACING_ENABLED
+  "google.protobuf.OneofDescriptorProto",
+#endif
 };
 
 static const upb_MiniTableSub google_protobuf_EnumDescriptorProto_submsgs[3] = {
   {.UPB_PRIVATE(submsg) = &google__protobuf__EnumValueDescriptorProto_msg_init},
   {.UPB_PRIVATE(submsg) = &google__protobuf__EnumOptions_msg_init},
   {.UPB_PRIVATE(submsg) = &google__protobuf__EnumDescriptorProto__EnumReservedRange_msg_init},
 };
@@ -278,14 +305,17 @@
   {5, UPB_SIZE(24, 56), 0, kUpb_NoSub, 12, (int)kUpb_FieldMode_Array | (int)kUpb_LabelFlags_IsAlternate | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)},
 };
 
 const upb_MiniTable google__protobuf__EnumDescriptorProto_msg_init = {
   &google_protobuf_EnumDescriptorProto_submsgs[0],
   &google_protobuf_EnumDescriptorProto__fields[0],
   UPB_SIZE(40, 64), 5, kUpb_ExtMode_NonExtendable, 5, UPB_FASTTABLE_MASK(56), 0,
+#ifdef UPB_TRACING_ENABLED
+  "google.protobuf.EnumDescriptorProto",
+#endif
   UPB_FASTTABLE_INIT({
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x002000003f000012, &upb_prm_1bt_max64b},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x003000003f020022, &upb_prm_1bt_max64b},
     {0x003800003f00002a, &upb_prs_1bt},
@@ -299,14 +329,17 @@
   {2, 16, 65, kUpb_NoSub, 5, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)},
 };
 
 const upb_MiniTable google__protobuf__EnumDescriptorProto__EnumReservedRange_msg_init = {
   NULL,
   &google_protobuf_EnumDescriptorProto_EnumReservedRange__fields[0],
   24, 2, kUpb_ExtMode_NonExtendable, 2, UPB_FASTTABLE_MASK(255), 0,
+#ifdef UPB_TRACING_ENABLED
+  "google.protobuf.EnumDescriptorProto.EnumReservedRange",
+#endif
 };
 
 static const upb_MiniTableSub google_protobuf_EnumValueDescriptorProto_submsgs[1] = {
   {.UPB_PRIVATE(submsg) = &google__protobuf__EnumValueOptions_msg_init},
 };
 
 static const upb_MiniTableField google_protobuf_EnumValueDescriptorProto__fields[3] = {
@@ -315,14 +348,17 @@
   {3, UPB_SIZE(16, 32), 66, 0, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)},
 };
 
 const upb_MiniTable google__protobuf__EnumValueDescriptorProto_msg_init = {
   &google_protobuf_EnumValueDescriptorProto_submsgs[0],
   &google_protobuf_EnumValueDescriptorProto__fields[0],
   UPB_SIZE(32, 40), 3, kUpb_ExtMode_NonExtendable, 3, UPB_FASTTABLE_MASK(255), 0,
+#ifdef UPB_TRACING_ENABLED
+  "google.protobuf.EnumValueDescriptorProto",
+#endif
 };
 
 static const upb_MiniTableSub google_protobuf_ServiceDescriptorProto_submsgs[2] = {
   {.UPB_PRIVATE(submsg) = &google__protobuf__MethodDescriptorProto_msg_init},
   {.UPB_PRIVATE(submsg) = &google__protobuf__ServiceOptions_msg_init},
 };
 
@@ -332,14 +368,17 @@
   {3, UPB_SIZE(16, 40), 65, 1, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)},
 };
 
 const upb_MiniTable google__protobuf__ServiceDescriptorProto_msg_init = {
   &google_protobuf_ServiceDescriptorProto_submsgs[0],
   &google_protobuf_ServiceDescriptorProto__fields[0],
   UPB_SIZE(32, 48), 3, kUpb_ExtMode_NonExtendable, 3, UPB_FASTTABLE_MASK(24), 0,
+#ifdef UPB_TRACING_ENABLED
+  "google.protobuf.ServiceDescriptorProto",
+#endif
   UPB_FASTTABLE_INIT({
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x002000003f000012, &upb_prm_1bt_max128b},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
   })
 };
@@ -357,14 +396,17 @@
   {6, UPB_SIZE(17, 10), 69, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)},
 };
 
 const upb_MiniTable google__protobuf__MethodDescriptorProto_msg_init = {
   &google_protobuf_MethodDescriptorProto_submsgs[0],
   &google_protobuf_MethodDescriptorProto__fields[0],
   UPB_SIZE(48, 72), 6, kUpb_ExtMode_NonExtendable, 6, UPB_FASTTABLE_MASK(255), 0,
+#ifdef UPB_TRACING_ENABLED
+  "google.protobuf.MethodDescriptorProto",
+#endif
 };
 
 static const upb_MiniTableSub google_protobuf_FileOptions_submsgs[3] = {
   {.UPB_PRIVATE(submsg) = &google__protobuf__FeatureSet_msg_init},
   {.UPB_PRIVATE(submsg) = &google__protobuf__UninterpretedOption_msg_init},
   {.UPB_PRIVATE(subenum) = &google_protobuf_FileOptions_OptimizeMode_enum_init},
 };
@@ -393,14 +435,17 @@
   {999, UPB_SIZE(28, 192), 0, 1, 11, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)},
 };
 
 const upb_MiniTable google__protobuf__FileOptions_msg_init = {
   &google_protobuf_FileOptions_submsgs[0],
   &google_protobuf_FileOptions__fields[0],
   UPB_SIZE(112, 200), 21, kUpb_ExtMode_Extendable, 1, UPB_FASTTABLE_MASK(248), 0,
+#ifdef UPB_TRACING_ENABLED
+  "google.protobuf.FileOptions",
+#endif
   UPB_FASTTABLE_INIT({
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
@@ -448,14 +493,17 @@
   {999, UPB_SIZE(20, 24), 0, 1, 11, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)},
 };
 
 const upb_MiniTable google__protobuf__MessageOptions_msg_init = {
   &google_protobuf_MessageOptions_submsgs[0],
   &google_protobuf_MessageOptions__fields[0],
   UPB_SIZE(24, 32), 7, kUpb_ExtMode_Extendable, 3, UPB_FASTTABLE_MASK(248), 0,
+#ifdef UPB_TRACING_ENABLED
+  "google.protobuf.MessageOptions",
+#endif
   UPB_FASTTABLE_INIT({
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
@@ -484,44 +532,49 @@
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
   })
 };
 
-static const upb_MiniTableSub google_protobuf_FieldOptions_submsgs[7] = {
+static const upb_MiniTableSub google_protobuf_FieldOptions_submsgs[8] = {
   {.UPB_PRIVATE(submsg) = &google__protobuf__FieldOptions__EditionDefault_msg_init},
   {.UPB_PRIVATE(submsg) = &google__protobuf__FeatureSet_msg_init},
+  {.UPB_PRIVATE(submsg) = &google__protobuf__FieldOptions__FeatureSupport_msg_init},
   {.UPB_PRIVATE(submsg) = &google__protobuf__UninterpretedOption_msg_init},
   {.UPB_PRIVATE(subenum) = &google_protobuf_FieldOptions_CType_enum_init},
   {.UPB_PRIVATE(subenum) = &google_protobuf_FieldOptions_JSType_enum_init},
   {.UPB_PRIVATE(subenum) = &google_protobuf_FieldOptions_OptionRetention_enum_init},
   {.UPB_PRIVATE(subenum) = &google_protobuf_FieldOptions_OptionTargetType_enum_init},
 };
 
-static const upb_MiniTableField google_protobuf_FieldOptions__fields[13] = {
-  {1, 12, 64, 3, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)},
+static const upb_MiniTableField google_protobuf_FieldOptions__fields[14] = {
+  {1, 12, 64, 4, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)},
   {2, 16, 65, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)},
   {3, 17, 66, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)},
   {5, 18, 67, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)},
-  {6, 20, 68, 4, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)},
+  {6, 20, 68, 5, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)},
   {10, 24, 69, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)},
   {15, 25, 70, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)},
   {16, 26, 71, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)},
-  {17, 28, 72, 5, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)},
-  {19, 32, 0, 6, 14, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)},
+  {17, 28, 72, 6, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)},
+  {19, 32, 0, 7, 14, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)},
   {20, UPB_SIZE(36, 40), 0, 0, 11, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)},
   {21, UPB_SIZE(40, 48), 73, 1, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)},
-  {999, UPB_SIZE(44, 56), 0, 2, 11, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)},
+  {22, UPB_SIZE(44, 56), 74, 2, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)},
+  {999, UPB_SIZE(48, 64), 0, 3, 11, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)},
 };
 
 const upb_MiniTable google__protobuf__FieldOptions_msg_init = {
   &google_protobuf_FieldOptions_submsgs[0],
   &google_protobuf_FieldOptions__fields[0],
-  UPB_SIZE(48, 64), 13, kUpb_ExtMode_Extendable, 3, UPB_FASTTABLE_MASK(248), 0,
+  UPB_SIZE(56, 72), 14, kUpb_ExtMode_Extendable, 3, UPB_FASTTABLE_MASK(248), 0,
+#ifdef UPB_TRACING_ENABLED
+  "google.protobuf.FieldOptions",
+#endif
   UPB_FASTTABLE_INIT({
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
@@ -538,15 +591,15 @@
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x002800003f0001a2, &upb_prm_2bt_max64b},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
-    {0x003800003f023eba, &upb_prm_2bt_max128b},
+    {0x004000003f033eba, &upb_prm_2bt_max128b},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
@@ -563,14 +616,39 @@
   {3, 12, 65, 0, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)},
 };
 
 const upb_MiniTable google__protobuf__FieldOptions__EditionDefault_msg_init = {
   &google_protobuf_FieldOptions_EditionDefault_submsgs[0],
   &google_protobuf_FieldOptions_EditionDefault__fields[0],
   UPB_SIZE(24, 32), 2, kUpb_ExtMode_NonExtendable, 0, UPB_FASTTABLE_MASK(255), 0,
+#ifdef UPB_TRACING_ENABLED
+  "google.protobuf.FieldOptions.EditionDefault",
+#endif
+};
+
+static const upb_MiniTableSub google_protobuf_FieldOptions_FeatureSupport_submsgs[3] = {
+  {.UPB_PRIVATE(subenum) = &google_protobuf_Edition_enum_init},
+  {.UPB_PRIVATE(subenum) = &google_protobuf_Edition_enum_init},
+  {.UPB_PRIVATE(subenum) = &google_protobuf_Edition_enum_init},
+};
+
+static const upb_MiniTableField google_protobuf_FieldOptions_FeatureSupport__fields[4] = {
+  {1, 12, 64, 0, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)},
+  {2, 16, 65, 1, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)},
+  {3, 24, 66, kUpb_NoSub, 12, (int)kUpb_FieldMode_Scalar | (int)kUpb_LabelFlags_IsAlternate | ((int)kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)},
+  {4, 20, 67, 2, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)},
+};
+
+const upb_MiniTable google__protobuf__FieldOptions__FeatureSupport_msg_init = {
+  &google_protobuf_FieldOptions_FeatureSupport_submsgs[0],
+  &google_protobuf_FieldOptions_FeatureSupport__fields[0],
+  UPB_SIZE(32, 40), 4, kUpb_ExtMode_NonExtendable, 4, UPB_FASTTABLE_MASK(255), 0,
+#ifdef UPB_TRACING_ENABLED
+  "google.protobuf.FieldOptions.FeatureSupport",
+#endif
 };
 
 static const upb_MiniTableSub google_protobuf_OneofOptions_submsgs[2] = {
   {.UPB_PRIVATE(submsg) = &google__protobuf__FeatureSet_msg_init},
   {.UPB_PRIVATE(submsg) = &google__protobuf__UninterpretedOption_msg_init},
 };
 
@@ -579,14 +657,17 @@
   {999, UPB_SIZE(16, 24), 0, 1, 11, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)},
 };
 
 const upb_MiniTable google__protobuf__OneofOptions_msg_init = {
   &google_protobuf_OneofOptions_submsgs[0],
   &google_protobuf_OneofOptions__fields[0],
   UPB_SIZE(24, 32), 2, kUpb_ExtMode_Extendable, 1, UPB_FASTTABLE_MASK(248), 0,
+#ifdef UPB_TRACING_ENABLED
+  "google.protobuf.OneofOptions",
+#endif
   UPB_FASTTABLE_INIT({
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
@@ -632,14 +713,17 @@
   {999, UPB_SIZE(16, 24), 0, 1, 11, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)},
 };
 
 const upb_MiniTable google__protobuf__EnumOptions_msg_init = {
   &google_protobuf_EnumOptions_submsgs[0],
   &google_protobuf_EnumOptions__fields[0],
   UPB_SIZE(24, 32), 5, kUpb_ExtMode_Extendable, 0, UPB_FASTTABLE_MASK(248), 0,
+#ifdef UPB_TRACING_ENABLED
+  "google.protobuf.EnumOptions",
+#endif
   UPB_FASTTABLE_INIT({
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
@@ -684,14 +768,17 @@
   {999, UPB_SIZE(20, 24), 0, 1, 11, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)},
 };
 
 const upb_MiniTable google__protobuf__EnumValueOptions_msg_init = {
   &google_protobuf_EnumValueOptions_submsgs[0],
   &google_protobuf_EnumValueOptions__fields[0],
   UPB_SIZE(24, 32), 4, kUpb_ExtMode_Extendable, 3, UPB_FASTTABLE_MASK(248), 0,
+#ifdef UPB_TRACING_ENABLED
+  "google.protobuf.EnumValueOptions",
+#endif
   UPB_FASTTABLE_INIT({
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
@@ -735,14 +822,17 @@
   {999, UPB_SIZE(16, 24), 0, 1, 11, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)},
 };
 
 const upb_MiniTable google__protobuf__ServiceOptions_msg_init = {
   &google_protobuf_ServiceOptions_submsgs[0],
   &google_protobuf_ServiceOptions__fields[0],
   UPB_SIZE(24, 32), 3, kUpb_ExtMode_Extendable, 0, UPB_FASTTABLE_MASK(248), 0,
+#ifdef UPB_TRACING_ENABLED
+  "google.protobuf.ServiceOptions",
+#endif
   UPB_FASTTABLE_INIT({
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
@@ -788,14 +878,17 @@
   {999, UPB_SIZE(20, 24), 0, 1, 11, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)},
 };
 
 const upb_MiniTable google__protobuf__MethodOptions_msg_init = {
   &google_protobuf_MethodOptions_submsgs[0],
   &google_protobuf_MethodOptions__fields[0],
   UPB_SIZE(24, 32), 4, kUpb_ExtMode_Extendable, 0, UPB_FASTTABLE_MASK(248), 0,
+#ifdef UPB_TRACING_ENABLED
+  "google.protobuf.MethodOptions",
+#endif
   UPB_FASTTABLE_INIT({
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
@@ -842,14 +935,17 @@
   {8, UPB_SIZE(56, 80), 69, kUpb_NoSub, 12, (int)kUpb_FieldMode_Scalar | (int)kUpb_LabelFlags_IsAlternate | ((int)kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)},
 };
 
 const upb_MiniTable google__protobuf__UninterpretedOption_msg_init = {
   &google_protobuf_UninterpretedOption_submsgs[0],
   &google_protobuf_UninterpretedOption__fields[0],
   UPB_SIZE(64, 96), 7, kUpb_ExtMode_NonExtendable, 0, UPB_FASTTABLE_MASK(24), 0,
+#ifdef UPB_TRACING_ENABLED
+  "google.protobuf.UninterpretedOption",
+#endif
   UPB_FASTTABLE_INIT({
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x001000003f000012, &upb_prm_1bt_max64b},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
   })
 };
@@ -859,14 +955,17 @@
   {2, 9, 65, kUpb_NoSub, 8, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)},
 };
 
 const upb_MiniTable google__protobuf__UninterpretedOption__NamePart_msg_init = {
   NULL,
   &google_protobuf_UninterpretedOption_NamePart__fields[0],
   UPB_SIZE(24, 32), 2, kUpb_ExtMode_NonExtendable, 2, UPB_FASTTABLE_MASK(255), 2,
+#ifdef UPB_TRACING_ENABLED
+  "google.protobuf.UninterpretedOption.NamePart",
+#endif
 };
 
 static const upb_MiniTableSub google_protobuf_FeatureSet_submsgs[6] = {
   {.UPB_PRIVATE(subenum) = &google_protobuf_FeatureSet_FieldPresence_enum_init},
   {.UPB_PRIVATE(subenum) = &google_protobuf_FeatureSet_EnumType_enum_init},
   {.UPB_PRIVATE(subenum) = &google_protobuf_FeatureSet_RepeatedFieldEncoding_enum_init},
   {.UPB_PRIVATE(subenum) = &google_protobuf_FeatureSet_Utf8Validation_enum_init},
@@ -883,14 +982,17 @@
   {6, 32, 69, 5, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)},
 };
 
 const upb_MiniTable google__protobuf__FeatureSet_msg_init = {
   &google_protobuf_FeatureSet_submsgs[0],
   &google_protobuf_FeatureSet__fields[0],
   40, 6, kUpb_ExtMode_Extendable, 6, UPB_FASTTABLE_MASK(255), 0,
+#ifdef UPB_TRACING_ENABLED
+  "google.protobuf.FeatureSet",
+#endif
 };
 
 static const upb_MiniTableSub google_protobuf_FeatureSetDefaults_submsgs[3] = {
   {.UPB_PRIVATE(submsg) = &google__protobuf__FeatureSetDefaults__FeatureSetEditionDefault_msg_init},
   {.UPB_PRIVATE(subenum) = &google_protobuf_Edition_enum_init},
   {.UPB_PRIVATE(subenum) = &google_protobuf_Edition_enum_init},
 };
@@ -901,48 +1003,59 @@
   {5, UPB_SIZE(20, 16), 65, 2, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)},
 };
 
 const upb_MiniTable google__protobuf__FeatureSetDefaults_msg_init = {
   &google_protobuf_FeatureSetDefaults_submsgs[0],
   &google_protobuf_FeatureSetDefaults__fields[0],
   UPB_SIZE(24, 32), 3, kUpb_ExtMode_NonExtendable, 1, UPB_FASTTABLE_MASK(8), 0,
+#ifdef UPB_TRACING_ENABLED
+  "google.protobuf.FeatureSetDefaults",
+#endif
   UPB_FASTTABLE_INIT({
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x001800003f00000a, &upb_prm_1bt_max64b},
   })
 };
 
-static const upb_MiniTableSub google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault_submsgs[2] = {
+static const upb_MiniTableSub google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault_submsgs[3] = {
+  {.UPB_PRIVATE(submsg) = &google__protobuf__FeatureSet_msg_init},
   {.UPB_PRIVATE(submsg) = &google__protobuf__FeatureSet_msg_init},
   {.UPB_PRIVATE(subenum) = &google_protobuf_Edition_enum_init},
 };
 
-static const upb_MiniTableField google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault__fields[2] = {
-  {2, UPB_SIZE(12, 16), 64, 0, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)},
-  {3, UPB_SIZE(16, 12), 65, 1, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)},
+static const upb_MiniTableField google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault__fields[3] = {
+  {3, 12, 64, 2, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)},
+  {4, 16, 65, 0, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)},
+  {5, UPB_SIZE(20, 24), 66, 1, 11, (int)kUpb_FieldMode_Scalar | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)},
 };
 
 const upb_MiniTable google__protobuf__FeatureSetDefaults__FeatureSetEditionDefault_msg_init = {
   &google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault_submsgs[0],
   &google_protobuf_FeatureSetDefaults_FeatureSetEditionDefault__fields[0],
-  24, 2, kUpb_ExtMode_NonExtendable, 0, UPB_FASTTABLE_MASK(255), 0,
+  UPB_SIZE(24, 32), 3, kUpb_ExtMode_NonExtendable, 0, UPB_FASTTABLE_MASK(255), 0,
+#ifdef UPB_TRACING_ENABLED
+  "google.protobuf.FeatureSetDefaults.FeatureSetEditionDefault",
+#endif
 };
 
 static const upb_MiniTableSub google_protobuf_SourceCodeInfo_submsgs[1] = {
   {.UPB_PRIVATE(submsg) = &google__protobuf__SourceCodeInfo__Location_msg_init},
 };
 
 static const upb_MiniTableField google_protobuf_SourceCodeInfo__fields[1] = {
   {1, 8, 0, 0, 11, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)},
 };
 
 const upb_MiniTable google__protobuf__SourceCodeInfo_msg_init = {
   &google_protobuf_SourceCodeInfo_submsgs[0],
   &google_protobuf_SourceCodeInfo__fields[0],
   16, 1, kUpb_ExtMode_NonExtendable, 1, UPB_FASTTABLE_MASK(8), 0,
+#ifdef UPB_TRACING_ENABLED
+  "google.protobuf.SourceCodeInfo",
+#endif
   UPB_FASTTABLE_INIT({
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x000800003f00000a, &upb_prm_1bt_max128b},
   })
 };
 
 static const upb_MiniTableField google_protobuf_SourceCodeInfo_Location__fields[5] = {
@@ -953,14 +1066,17 @@
   {6, UPB_SIZE(20, 64), 0, kUpb_NoSub, 12, (int)kUpb_FieldMode_Array | (int)kUpb_LabelFlags_IsAlternate | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)},
 };
 
 const upb_MiniTable google__protobuf__SourceCodeInfo__Location_msg_init = {
   NULL,
   &google_protobuf_SourceCodeInfo_Location__fields[0],
   UPB_SIZE(40, 72), 5, kUpb_ExtMode_NonExtendable, 4, UPB_FASTTABLE_MASK(56), 0,
+#ifdef UPB_TRACING_ENABLED
+  "google.protobuf.SourceCodeInfo.Location",
+#endif
   UPB_FASTTABLE_INIT({
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x001000003f00000a, &upb_ppv4_1bt},
     {0x001800003f000012, &upb_ppv4_1bt},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
@@ -977,14 +1093,17 @@
   {1, 8, 0, 0, 11, (int)kUpb_FieldMode_Array | ((int)UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)},
 };
 
 const upb_MiniTable google__protobuf__GeneratedCodeInfo_msg_init = {
   &google_protobuf_GeneratedCodeInfo_submsgs[0],
   &google_protobuf_GeneratedCodeInfo__fields[0],
   16, 1, kUpb_ExtMode_NonExtendable, 1, UPB_FASTTABLE_MASK(8), 0,
+#ifdef UPB_TRACING_ENABLED
+  "google.protobuf.GeneratedCodeInfo",
+#endif
   UPB_FASTTABLE_INIT({
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x000800003f00000a, &upb_prm_1bt_max64b},
   })
 };
 
 static const upb_MiniTableSub google_protobuf_GeneratedCodeInfo_Annotation_submsgs[1] = {
@@ -999,21 +1118,24 @@
   {5, UPB_SIZE(24, 20), 67, 0, 14, (int)kUpb_FieldMode_Scalar | ((int)kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)},
 };
 
 const upb_MiniTable google__protobuf__GeneratedCodeInfo__Annotation_msg_init = {
   &google_protobuf_GeneratedCodeInfo_Annotation_submsgs[0],
   &google_protobuf_GeneratedCodeInfo_Annotation__fields[0],
   UPB_SIZE(40, 48), 5, kUpb_ExtMode_NonExtendable, 5, UPB_FASTTABLE_MASK(8), 0,
+#ifdef UPB_TRACING_ENABLED
+  "google.protobuf.GeneratedCodeInfo.Annotation",
+#endif
   UPB_FASTTABLE_INIT({
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x001800003f00000a, &upb_ppv4_1bt},
   })
 };
 
-static const upb_MiniTable *messages_layout[32] = {
+static const upb_MiniTable *messages_layout[33] = {
   &google__protobuf__FileDescriptorSet_msg_init,
   &google__protobuf__FileDescriptorProto_msg_init,
   &google__protobuf__DescriptorProto_msg_init,
   &google__protobuf__DescriptorProto__ExtensionRange_msg_init,
   &google__protobuf__DescriptorProto__ReservedRange_msg_init,
   &google__protobuf__ExtensionRangeOptions_msg_init,
   &google__protobuf__ExtensionRangeOptions__Declaration_msg_init,
@@ -1024,14 +1146,15 @@
   &google__protobuf__EnumValueDescriptorProto_msg_init,
   &google__protobuf__ServiceDescriptorProto_msg_init,
   &google__protobuf__MethodDescriptorProto_msg_init,
   &google__protobuf__FileOptions_msg_init,
   &google__protobuf__MessageOptions_msg_init,
   &google__protobuf__FieldOptions_msg_init,
   &google__protobuf__FieldOptions__EditionDefault_msg_init,
+  &google__protobuf__FieldOptions__FeatureSupport_msg_init,
   &google__protobuf__OneofOptions_msg_init,
   &google__protobuf__EnumOptions_msg_init,
   &google__protobuf__EnumValueOptions_msg_init,
   &google__protobuf__ServiceOptions_msg_init,
   &google__protobuf__MethodOptions_msg_init,
   &google__protobuf__UninterpretedOption_msg_init,
   &google__protobuf__UninterpretedOption__NamePart_msg_init,
@@ -1042,18 +1165,19 @@
   &google__protobuf__SourceCodeInfo__Location_msg_init,
   &google__protobuf__GeneratedCodeInfo_msg_init,
   &google__protobuf__GeneratedCodeInfo__Annotation_msg_init,
 };
 
 const upb_MiniTableEnum google_protobuf_Edition_enum_init = {
     64,
-    8,
+    9,
     {
         0x7,
         0x0,
+        0x384,
         0x3e6,
         0x3e7,
         0x3e8,
         0x3e9,
         0x1869d,
         0x1869e,
         0x1869f,
@@ -1225,14 +1349,14 @@
   &google_protobuf_MethodOptions_IdempotencyLevel_enum_init,
 };
 
 const upb_MiniTableFile google_protobuf_descriptor_proto_upb_file_layout = {
   messages_layout,
   enums_layout,
   NULL,
-  32,
+  33,
   17,
   0,
 };
 
 #include "upb/port/undef.inc"
```

### Comparing `protobuf-5.26.1/google/protobuf/descriptor.upb_minitable.h` & `protobuf-5.27.0rc1/google/protobuf/descriptor.upb_minitable.h`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 extern const upb_MiniTable google__protobuf__EnumValueDescriptorProto_msg_init;
 extern const upb_MiniTable google__protobuf__ServiceDescriptorProto_msg_init;
 extern const upb_MiniTable google__protobuf__MethodDescriptorProto_msg_init;
 extern const upb_MiniTable google__protobuf__FileOptions_msg_init;
 extern const upb_MiniTable google__protobuf__MessageOptions_msg_init;
 extern const upb_MiniTable google__protobuf__FieldOptions_msg_init;
 extern const upb_MiniTable google__protobuf__FieldOptions__EditionDefault_msg_init;
+extern const upb_MiniTable google__protobuf__FieldOptions__FeatureSupport_msg_init;
 extern const upb_MiniTable google__protobuf__OneofOptions_msg_init;
 extern const upb_MiniTable google__protobuf__EnumOptions_msg_init;
 extern const upb_MiniTable google__protobuf__EnumValueOptions_msg_init;
 extern const upb_MiniTable google__protobuf__ServiceOptions_msg_init;
 extern const upb_MiniTable google__protobuf__MethodOptions_msg_init;
 extern const upb_MiniTable google__protobuf__UninterpretedOption_msg_init;
 extern const upb_MiniTable google__protobuf__UninterpretedOption__NamePart_msg_init;
```

### Comparing `protobuf-5.26.1/google/protobuf/descriptor.upbdefs.c` & `protobuf-5.27.0rc1/google/protobuf/descriptor.upbdefs.c`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
  * Do not edit -- your changes will be discarded when the file is
  * regenerated. */
 
 #include "upb/reflection/def.h"
 #include "google/protobuf/descriptor.upbdefs.h"
 #include "google/protobuf/descriptor.upb_minitable.h"
 
-static const char descriptor[11630] = {'\n', ' ', 'g', 'o', 'o', 'g', 'l', 'e', '/', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '/', 'd', 'e', 's', 'c', 'r', 'i', 'p', 
+static const char descriptor[12155] = {'\n', ' ', 'g', 'o', 'o', 'g', 'l', 'e', '/', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '/', 'd', 'e', 's', 'c', 'r', 'i', 'p', 
 't', 'o', 'r', '.', 'p', 'r', 'o', 't', 'o', '\022', '\017', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 
 'f', '\"', 'M', '\n', '\021', 'F', 'i', 'l', 'e', 'D', 'e', 's', 'c', 'r', 'i', 'p', 't', 'o', 'r', 'S', 'e', 't', '\022', '8', '\n', 
 '\004', 'f', 'i', 'l', 'e', '\030', '\001', ' ', '\003', '(', '\013', '2', '$', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 
 'o', 'b', 'u', 'f', '.', 'F', 'i', 'l', 'e', 'D', 'e', 's', 'c', 'r', 'i', 'p', 't', 'o', 'r', 'P', 'r', 'o', 't', 'o', 'R', 
 '\004', 'f', 'i', 'l', 'e', '\"', '\230', '\005', '\n', '\023', 'F', 'i', 'l', 'e', 'D', 'e', 's', 'c', 'r', 'i', 'p', 't', 'o', 'r', 'P', 
 'r', 'o', 't', 'o', '\022', '\022', '\n', '\004', 'n', 'a', 'm', 'e', '\030', '\001', ' ', '\001', '(', '\t', 'R', '\004', 'n', 'a', 'm', 'e', '\022', 
 '\030', '\n', '\007', 'p', 'a', 'c', 'k', 'a', 'g', 'e', '\030', '\002', ' ', '\001', '(', '\t', 'R', '\007', 'p', 'a', 'c', 'k', 'a', 'g', 'e', 
@@ -235,15 +235,15 @@
 's', '\022', '7', '\n', '\010', 'f', 'e', 'a', 't', 'u', 'r', 'e', 's', '\030', '\014', ' ', '\001', '(', '\013', '2', '\033', '.', 'g', 'o', 'o', 
 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'F', 'e', 'a', 't', 'u', 'r', 'e', 'S', 'e', 't', 'R', '\010', 
 'f', 'e', 'a', 't', 'u', 'r', 'e', 's', '\022', 'X', '\n', '\024', 'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 
 '_', 'o', 'p', 't', 'i', 'o', 'n', '\030', '\347', '\007', ' ', '\003', '(', '\013', '2', '$', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 
 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'U', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 
 'o', 'n', 'R', '\023', 'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', '*', '\t', 
 '\010', '\350', '\007', '\020', '\200', '\200', '\200', '\200', '\002', 'J', '\004', '\010', '\004', '\020', '\005', 'J', '\004', '\010', '\005', '\020', '\006', 'J', '\004', '\010', '\006', 
-'\020', '\007', 'J', '\004', '\010', '\010', '\020', '\t', 'J', '\004', '\010', '\t', '\020', '\n', '\"', '\255', '\n', '\n', '\014', 'F', 'i', 'e', 'l', 'd', 'O', 
+'\020', '\007', 'J', '\004', '\010', '\010', '\020', '\t', 'J', '\004', '\010', '\t', '\020', '\n', '\"', '\235', '\r', '\n', '\014', 'F', 'i', 'e', 'l', 'd', 'O', 
 'p', 't', 'i', 'o', 'n', 's', '\022', 'A', '\n', '\005', 'c', 't', 'y', 'p', 'e', '\030', '\001', ' ', '\001', '(', '\016', '2', '#', '.', 'g', 
 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'F', 'i', 'e', 'l', 'd', 'O', 'p', 't', 'i', 'o', 
 'n', 's', '.', 'C', 'T', 'y', 'p', 'e', ':', '\006', 'S', 'T', 'R', 'I', 'N', 'G', 'R', '\005', 'c', 't', 'y', 'p', 'e', '\022', '\026', 
 '\n', '\006', 'p', 'a', 'c', 'k', 'e', 'd', '\030', '\002', ' ', '\001', '(', '\010', 'R', '\006', 'p', 'a', 'c', 'k', 'e', 'd', '\022', 'G', '\n', 
 '\006', 'j', 's', 't', 'y', 'p', 'e', '\030', '\006', ' ', '\001', '(', '\016', '2', '$', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 
 'o', 't', 'o', 'b', 'u', 'f', '.', 'F', 'i', 'e', 'l', 'd', 'O', 'p', 't', 'i', 'o', 'n', 's', '.', 'J', 'S', 'T', 'y', 'p', 
 'e', ':', '\t', 'J', 'S', '_', 'N', 'O', 'R', 'M', 'A', 'L', 'R', '\006', 'j', 's', 't', 'y', 'p', 'e', '\022', '\031', '\n', '\004', 'l', 
@@ -262,208 +262,229 @@
 'o', 'n', 's', '.', 'O', 'p', 't', 'i', 'o', 'n', 'T', 'a', 'r', 'g', 'e', 't', 'T', 'y', 'p', 'e', 'R', '\007', 't', 'a', 'r', 
 'g', 'e', 't', 's', '\022', 'W', '\n', '\020', 'e', 'd', 'i', 't', 'i', 'o', 'n', '_', 'd', 'e', 'f', 'a', 'u', 'l', 't', 's', '\030', 
 '\024', ' ', '\003', '(', '\013', '2', ',', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'F', 
 'i', 'e', 'l', 'd', 'O', 'p', 't', 'i', 'o', 'n', 's', '.', 'E', 'd', 'i', 't', 'i', 'o', 'n', 'D', 'e', 'f', 'a', 'u', 'l', 
 't', 'R', '\017', 'e', 'd', 'i', 't', 'i', 'o', 'n', 'D', 'e', 'f', 'a', 'u', 'l', 't', 's', '\022', '7', '\n', '\010', 'f', 'e', 'a', 
 't', 'u', 'r', 'e', 's', '\030', '\025', ' ', '\001', '(', '\013', '2', '\033', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 
 'o', 'b', 'u', 'f', '.', 'F', 'e', 'a', 't', 'u', 'r', 'e', 'S', 'e', 't', 'R', '\010', 'f', 'e', 'a', 't', 'u', 'r', 'e', 's', 
-'\022', 'X', '\n', '\024', 'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', '_', 'o', 'p', 't', 'i', 'o', 'n', '\030', 
-'\347', '\007', ' ', '\003', '(', '\013', '2', '$', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 
-'U', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', 'R', '\023', 'u', 'n', 'i', 'n', 
-'t', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', '\032', 'Z', '\n', '\016', 'E', 'd', 'i', 't', 'i', 'o', 
-'n', 'D', 'e', 'f', 'a', 'u', 'l', 't', '\022', '2', '\n', '\007', 'e', 'd', 'i', 't', 'i', 'o', 'n', '\030', '\003', ' ', '\001', '(', '\016', 
-'2', '\030', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'E', 'd', 'i', 't', 'i', 'o', 
-'n', 'R', '\007', 'e', 'd', 'i', 't', 'i', 'o', 'n', '\022', '\024', '\n', '\005', 'v', 'a', 'l', 'u', 'e', '\030', '\002', ' ', '\001', '(', '\t', 
-'R', '\005', 'v', 'a', 'l', 'u', 'e', '\"', '/', '\n', '\005', 'C', 'T', 'y', 'p', 'e', '\022', '\n', '\n', '\006', 'S', 'T', 'R', 'I', 'N', 
-'G', '\020', '\000', '\022', '\010', '\n', '\004', 'C', 'O', 'R', 'D', '\020', '\001', '\022', '\020', '\n', '\014', 'S', 'T', 'R', 'I', 'N', 'G', '_', 'P', 
-'I', 'E', 'C', 'E', '\020', '\002', '\"', '5', '\n', '\006', 'J', 'S', 'T', 'y', 'p', 'e', '\022', '\r', '\n', '\t', 'J', 'S', '_', 'N', 'O', 
-'R', 'M', 'A', 'L', '\020', '\000', '\022', '\r', '\n', '\t', 'J', 'S', '_', 'S', 'T', 'R', 'I', 'N', 'G', '\020', '\001', '\022', '\r', '\n', '\t', 
-'J', 'S', '_', 'N', 'U', 'M', 'B', 'E', 'R', '\020', '\002', '\"', 'U', '\n', '\017', 'O', 'p', 't', 'i', 'o', 'n', 'R', 'e', 't', 'e', 
-'n', 't', 'i', 'o', 'n', '\022', '\025', '\n', '\021', 'R', 'E', 'T', 'E', 'N', 'T', 'I', 'O', 'N', '_', 'U', 'N', 'K', 'N', 'O', 'W', 
-'N', '\020', '\000', '\022', '\025', '\n', '\021', 'R', 'E', 'T', 'E', 'N', 'T', 'I', 'O', 'N', '_', 'R', 'U', 'N', 'T', 'I', 'M', 'E', '\020', 
-'\001', '\022', '\024', '\n', '\020', 'R', 'E', 'T', 'E', 'N', 'T', 'I', 'O', 'N', '_', 'S', 'O', 'U', 'R', 'C', 'E', '\020', '\002', '\"', '\214', 
-'\002', '\n', '\020', 'O', 'p', 't', 'i', 'o', 'n', 'T', 'a', 'r', 'g', 'e', 't', 'T', 'y', 'p', 'e', '\022', '\027', '\n', '\023', 'T', 'A', 
-'R', 'G', 'E', 'T', '_', 'T', 'Y', 'P', 'E', '_', 'U', 'N', 'K', 'N', 'O', 'W', 'N', '\020', '\000', '\022', '\024', '\n', '\020', 'T', 'A', 
-'R', 'G', 'E', 'T', '_', 'T', 'Y', 'P', 'E', '_', 'F', 'I', 'L', 'E', '\020', '\001', '\022', '\037', '\n', '\033', 'T', 'A', 'R', 'G', 'E', 
-'T', '_', 'T', 'Y', 'P', 'E', '_', 'E', 'X', 'T', 'E', 'N', 'S', 'I', 'O', 'N', '_', 'R', 'A', 'N', 'G', 'E', '\020', '\002', '\022', 
-'\027', '\n', '\023', 'T', 'A', 'R', 'G', 'E', 'T', '_', 'T', 'Y', 'P', 'E', '_', 'M', 'E', 'S', 'S', 'A', 'G', 'E', '\020', '\003', '\022', 
-'\025', '\n', '\021', 'T', 'A', 'R', 'G', 'E', 'T', '_', 'T', 'Y', 'P', 'E', '_', 'F', 'I', 'E', 'L', 'D', '\020', '\004', '\022', '\025', '\n', 
-'\021', 'T', 'A', 'R', 'G', 'E', 'T', '_', 'T', 'Y', 'P', 'E', '_', 'O', 'N', 'E', 'O', 'F', '\020', '\005', '\022', '\024', '\n', '\020', 'T', 
-'A', 'R', 'G', 'E', 'T', '_', 'T', 'Y', 'P', 'E', '_', 'E', 'N', 'U', 'M', '\020', '\006', '\022', '\032', '\n', '\026', 'T', 'A', 'R', 'G', 
-'E', 'T', '_', 'T', 'Y', 'P', 'E', '_', 'E', 'N', 'U', 'M', '_', 'E', 'N', 'T', 'R', 'Y', '\020', '\007', '\022', '\027', '\n', '\023', 'T', 
-'A', 'R', 'G', 'E', 'T', '_', 'T', 'Y', 'P', 'E', '_', 'S', 'E', 'R', 'V', 'I', 'C', 'E', '\020', '\010', '\022', '\026', '\n', '\022', 'T', 
-'A', 'R', 'G', 'E', 'T', '_', 'T', 'Y', 'P', 'E', '_', 'M', 'E', 'T', 'H', 'O', 'D', '\020', '\t', '*', '\t', '\010', '\350', '\007', '\020', 
-'\200', '\200', '\200', '\200', '\002', 'J', '\004', '\010', '\004', '\020', '\005', 'J', '\004', '\010', '\022', '\020', '\023', '\"', '\254', '\001', '\n', '\014', 'O', 'n', 'e', 
-'o', 'f', 'O', 'p', 't', 'i', 'o', 'n', 's', '\022', '7', '\n', '\010', 'f', 'e', 'a', 't', 'u', 'r', 'e', 's', '\030', '\001', ' ', '\001', 
-'(', '\013', '2', '\033', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'F', 'e', 'a', 't', 
-'u', 'r', 'e', 'S', 'e', 't', 'R', '\010', 'f', 'e', 'a', 't', 'u', 'r', 'e', 's', '\022', 'X', '\n', '\024', 'u', 'n', 'i', 'n', 't', 
-'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', '_', 'o', 'p', 't', 'i', 'o', 'n', '\030', '\347', '\007', ' ', '\003', '(', '\013', '2', '$', '.', 
-'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'U', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 
-'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', 'R', '\023', 'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 
-'O', 'p', 't', 'i', 'o', 'n', '*', '\t', '\010', '\350', '\007', '\020', '\200', '\200', '\200', '\200', '\002', '\"', '\321', '\002', '\n', '\013', 'E', 'n', 'u', 
-'m', 'O', 'p', 't', 'i', 'o', 'n', 's', '\022', '\037', '\n', '\013', 'a', 'l', 'l', 'o', 'w', '_', 'a', 'l', 'i', 'a', 's', '\030', '\002', 
-' ', '\001', '(', '\010', 'R', '\n', 'a', 'l', 'l', 'o', 'w', 'A', 'l', 'i', 'a', 's', '\022', '%', '\n', '\n', 'd', 'e', 'p', 'r', 'e', 
-'c', 'a', 't', 'e', 'd', '\030', '\003', ' ', '\001', '(', '\010', ':', '\005', 'f', 'a', 'l', 's', 'e', 'R', '\n', 'd', 'e', 'p', 'r', 'e', 
-'c', 'a', 't', 'e', 'd', '\022', 'V', '\n', '&', 'd', 'e', 'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', '_', 'l', 'e', 'g', 'a', 'c', 
-'y', '_', 'j', 's', 'o', 'n', '_', 'f', 'i', 'e', 'l', 'd', '_', 'c', 'o', 'n', 'f', 'l', 'i', 'c', 't', 's', '\030', '\006', ' ', 
-'\001', '(', '\010', 'B', '\002', '\030', '\001', 'R', '\"', 'd', 'e', 'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', 'L', 'e', 'g', 'a', 'c', 'y', 
-'J', 's', 'o', 'n', 'F', 'i', 'e', 'l', 'd', 'C', 'o', 'n', 'f', 'l', 'i', 'c', 't', 's', '\022', '7', '\n', '\010', 'f', 'e', 'a', 
-'t', 'u', 'r', 'e', 's', '\030', '\007', ' ', '\001', '(', '\013', '2', '\033', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 
-'o', 'b', 'u', 'f', '.', 'F', 'e', 'a', 't', 'u', 'r', 'e', 'S', 'e', 't', 'R', '\010', 'f', 'e', 'a', 't', 'u', 'r', 'e', 's', 
+'\022', 'U', '\n', '\017', 'f', 'e', 'a', 't', 'u', 'r', 'e', '_', 's', 'u', 'p', 'p', 'o', 'r', 't', '\030', '\026', ' ', '\001', '(', '\013', 
+'2', ',', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'F', 'i', 'e', 'l', 'd', 'O', 
+'p', 't', 'i', 'o', 'n', 's', '.', 'F', 'e', 'a', 't', 'u', 'r', 'e', 'S', 'u', 'p', 'p', 'o', 'r', 't', 'R', '\016', 'f', 'e', 
+'a', 't', 'u', 'r', 'e', 'S', 'u', 'p', 'p', 'o', 'r', 't', '\022', 'X', '\n', '\024', 'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 
+'e', 't', 'e', 'd', '_', 'o', 'p', 't', 'i', 'o', 'n', '\030', '\347', '\007', ' ', '\003', '(', '\013', '2', '$', '.', 'g', 'o', 'o', 'g', 
+'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'U', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 
+'O', 'p', 't', 'i', 'o', 'n', 'R', '\023', 'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 
+'o', 'n', '\032', 'Z', '\n', '\016', 'E', 'd', 'i', 't', 'i', 'o', 'n', 'D', 'e', 'f', 'a', 'u', 'l', 't', '\022', '2', '\n', '\007', 'e', 
+'d', 'i', 't', 'i', 'o', 'n', '\030', '\003', ' ', '\001', '(', '\016', '2', '\030', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 
+'t', 'o', 'b', 'u', 'f', '.', 'E', 'd', 'i', 't', 'i', 'o', 'n', 'R', '\007', 'e', 'd', 'i', 't', 'i', 'o', 'n', '\022', '\024', '\n', 
+'\005', 'v', 'a', 'l', 'u', 'e', '\030', '\002', ' ', '\001', '(', '\t', 'R', '\005', 'v', 'a', 'l', 'u', 'e', '\032', '\226', '\002', '\n', '\016', 'F', 
+'e', 'a', 't', 'u', 'r', 'e', 'S', 'u', 'p', 'p', 'o', 'r', 't', '\022', 'G', '\n', '\022', 'e', 'd', 'i', 't', 'i', 'o', 'n', '_', 
+'i', 'n', 't', 'r', 'o', 'd', 'u', 'c', 'e', 'd', '\030', '\001', ' ', '\001', '(', '\016', '2', '\030', '.', 'g', 'o', 'o', 'g', 'l', 'e', 
+'.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'E', 'd', 'i', 't', 'i', 'o', 'n', 'R', '\021', 'e', 'd', 'i', 't', 'i', 'o', 
+'n', 'I', 'n', 't', 'r', 'o', 'd', 'u', 'c', 'e', 'd', '\022', 'G', '\n', '\022', 'e', 'd', 'i', 't', 'i', 'o', 'n', '_', 'd', 'e', 
+'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', '\030', '\002', ' ', '\001', '(', '\016', '2', '\030', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 
+'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'E', 'd', 'i', 't', 'i', 'o', 'n', 'R', '\021', 'e', 'd', 'i', 't', 'i', 'o', 'n', 'D', 
+'e', 'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', '\022', '/', '\n', '\023', 'd', 'e', 'p', 'r', 'e', 'c', 'a', 't', 'i', 'o', 'n', '_', 
+'w', 'a', 'r', 'n', 'i', 'n', 'g', '\030', '\003', ' ', '\001', '(', '\t', 'R', '\022', 'd', 'e', 'p', 'r', 'e', 'c', 'a', 't', 'i', 'o', 
+'n', 'W', 'a', 'r', 'n', 'i', 'n', 'g', '\022', 'A', '\n', '\017', 'e', 'd', 'i', 't', 'i', 'o', 'n', '_', 'r', 'e', 'm', 'o', 'v', 
+'e', 'd', '\030', '\004', ' ', '\001', '(', '\016', '2', '\030', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 
+'f', '.', 'E', 'd', 'i', 't', 'i', 'o', 'n', 'R', '\016', 'e', 'd', 'i', 't', 'i', 'o', 'n', 'R', 'e', 'm', 'o', 'v', 'e', 'd', 
+'\"', '/', '\n', '\005', 'C', 'T', 'y', 'p', 'e', '\022', '\n', '\n', '\006', 'S', 'T', 'R', 'I', 'N', 'G', '\020', '\000', '\022', '\010', '\n', '\004', 
+'C', 'O', 'R', 'D', '\020', '\001', '\022', '\020', '\n', '\014', 'S', 'T', 'R', 'I', 'N', 'G', '_', 'P', 'I', 'E', 'C', 'E', '\020', '\002', '\"', 
+'5', '\n', '\006', 'J', 'S', 'T', 'y', 'p', 'e', '\022', '\r', '\n', '\t', 'J', 'S', '_', 'N', 'O', 'R', 'M', 'A', 'L', '\020', '\000', '\022', 
+'\r', '\n', '\t', 'J', 'S', '_', 'S', 'T', 'R', 'I', 'N', 'G', '\020', '\001', '\022', '\r', '\n', '\t', 'J', 'S', '_', 'N', 'U', 'M', 'B', 
+'E', 'R', '\020', '\002', '\"', 'U', '\n', '\017', 'O', 'p', 't', 'i', 'o', 'n', 'R', 'e', 't', 'e', 'n', 't', 'i', 'o', 'n', '\022', '\025', 
+'\n', '\021', 'R', 'E', 'T', 'E', 'N', 'T', 'I', 'O', 'N', '_', 'U', 'N', 'K', 'N', 'O', 'W', 'N', '\020', '\000', '\022', '\025', '\n', '\021', 
+'R', 'E', 'T', 'E', 'N', 'T', 'I', 'O', 'N', '_', 'R', 'U', 'N', 'T', 'I', 'M', 'E', '\020', '\001', '\022', '\024', '\n', '\020', 'R', 'E', 
+'T', 'E', 'N', 'T', 'I', 'O', 'N', '_', 'S', 'O', 'U', 'R', 'C', 'E', '\020', '\002', '\"', '\214', '\002', '\n', '\020', 'O', 'p', 't', 'i', 
+'o', 'n', 'T', 'a', 'r', 'g', 'e', 't', 'T', 'y', 'p', 'e', '\022', '\027', '\n', '\023', 'T', 'A', 'R', 'G', 'E', 'T', '_', 'T', 'Y', 
+'P', 'E', '_', 'U', 'N', 'K', 'N', 'O', 'W', 'N', '\020', '\000', '\022', '\024', '\n', '\020', 'T', 'A', 'R', 'G', 'E', 'T', '_', 'T', 'Y', 
+'P', 'E', '_', 'F', 'I', 'L', 'E', '\020', '\001', '\022', '\037', '\n', '\033', 'T', 'A', 'R', 'G', 'E', 'T', '_', 'T', 'Y', 'P', 'E', '_', 
+'E', 'X', 'T', 'E', 'N', 'S', 'I', 'O', 'N', '_', 'R', 'A', 'N', 'G', 'E', '\020', '\002', '\022', '\027', '\n', '\023', 'T', 'A', 'R', 'G', 
+'E', 'T', '_', 'T', 'Y', 'P', 'E', '_', 'M', 'E', 'S', 'S', 'A', 'G', 'E', '\020', '\003', '\022', '\025', '\n', '\021', 'T', 'A', 'R', 'G', 
+'E', 'T', '_', 'T', 'Y', 'P', 'E', '_', 'F', 'I', 'E', 'L', 'D', '\020', '\004', '\022', '\025', '\n', '\021', 'T', 'A', 'R', 'G', 'E', 'T', 
+'_', 'T', 'Y', 'P', 'E', '_', 'O', 'N', 'E', 'O', 'F', '\020', '\005', '\022', '\024', '\n', '\020', 'T', 'A', 'R', 'G', 'E', 'T', '_', 'T', 
+'Y', 'P', 'E', '_', 'E', 'N', 'U', 'M', '\020', '\006', '\022', '\032', '\n', '\026', 'T', 'A', 'R', 'G', 'E', 'T', '_', 'T', 'Y', 'P', 'E', 
+'_', 'E', 'N', 'U', 'M', '_', 'E', 'N', 'T', 'R', 'Y', '\020', '\007', '\022', '\027', '\n', '\023', 'T', 'A', 'R', 'G', 'E', 'T', '_', 'T', 
+'Y', 'P', 'E', '_', 'S', 'E', 'R', 'V', 'I', 'C', 'E', '\020', '\010', '\022', '\026', '\n', '\022', 'T', 'A', 'R', 'G', 'E', 'T', '_', 'T', 
+'Y', 'P', 'E', '_', 'M', 'E', 'T', 'H', 'O', 'D', '\020', '\t', '*', '\t', '\010', '\350', '\007', '\020', '\200', '\200', '\200', '\200', '\002', 'J', '\004', 
+'\010', '\004', '\020', '\005', 'J', '\004', '\010', '\022', '\020', '\023', '\"', '\254', '\001', '\n', '\014', 'O', 'n', 'e', 'o', 'f', 'O', 'p', 't', 'i', 'o', 
+'n', 's', '\022', '7', '\n', '\010', 'f', 'e', 'a', 't', 'u', 'r', 'e', 's', '\030', '\001', ' ', '\001', '(', '\013', '2', '\033', '.', 'g', 'o', 
+'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'F', 'e', 'a', 't', 'u', 'r', 'e', 'S', 'e', 't', 'R', 
+'\010', 'f', 'e', 'a', 't', 'u', 'r', 'e', 's', '\022', 'X', '\n', '\024', 'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 
+'d', '_', 'o', 'p', 't', 'i', 'o', 'n', '\030', '\347', '\007', ' ', '\003', '(', '\013', '2', '$', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 
+'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'U', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 
+'i', 'o', 'n', 'R', '\023', 'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', '*', 
+'\t', '\010', '\350', '\007', '\020', '\200', '\200', '\200', '\200', '\002', '\"', '\321', '\002', '\n', '\013', 'E', 'n', 'u', 'm', 'O', 'p', 't', 'i', 'o', 'n', 
+'s', '\022', '\037', '\n', '\013', 'a', 'l', 'l', 'o', 'w', '_', 'a', 'l', 'i', 'a', 's', '\030', '\002', ' ', '\001', '(', '\010', 'R', '\n', 'a', 
+'l', 'l', 'o', 'w', 'A', 'l', 'i', 'a', 's', '\022', '%', '\n', '\n', 'd', 'e', 'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', '\030', '\003', 
+' ', '\001', '(', '\010', ':', '\005', 'f', 'a', 'l', 's', 'e', 'R', '\n', 'd', 'e', 'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', '\022', 'V', 
+'\n', '&', 'd', 'e', 'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', '_', 'l', 'e', 'g', 'a', 'c', 'y', '_', 'j', 's', 'o', 'n', '_', 
+'f', 'i', 'e', 'l', 'd', '_', 'c', 'o', 'n', 'f', 'l', 'i', 'c', 't', 's', '\030', '\006', ' ', '\001', '(', '\010', 'B', '\002', '\030', '\001', 
+'R', '\"', 'd', 'e', 'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', 'L', 'e', 'g', 'a', 'c', 'y', 'J', 's', 'o', 'n', 'F', 'i', 'e', 
+'l', 'd', 'C', 'o', 'n', 'f', 'l', 'i', 'c', 't', 's', '\022', '7', '\n', '\010', 'f', 'e', 'a', 't', 'u', 'r', 'e', 's', '\030', '\007', 
+' ', '\001', '(', '\013', '2', '\033', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'F', 'e', 
+'a', 't', 'u', 'r', 'e', 'S', 'e', 't', 'R', '\010', 'f', 'e', 'a', 't', 'u', 'r', 'e', 's', '\022', 'X', '\n', '\024', 'u', 'n', 'i', 
+'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', '_', 'o', 'p', 't', 'i', 'o', 'n', '\030', '\347', '\007', ' ', '\003', '(', '\013', '2', 
+'$', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'U', 'n', 'i', 'n', 't', 'e', 'r', 
+'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', 'R', '\023', 'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 
+'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', '*', '\t', '\010', '\350', '\007', '\020', '\200', '\200', '\200', '\200', '\002', 'J', '\004', '\010', '\005', '\020', '\006', 
+'\"', '\201', '\002', '\n', '\020', 'E', 'n', 'u', 'm', 'V', 'a', 'l', 'u', 'e', 'O', 'p', 't', 'i', 'o', 'n', 's', '\022', '%', '\n', '\n', 
+'d', 'e', 'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', '\030', '\001', ' ', '\001', '(', '\010', ':', '\005', 'f', 'a', 'l', 's', 'e', 'R', '\n', 
+'d', 'e', 'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', '\022', '7', '\n', '\010', 'f', 'e', 'a', 't', 'u', 'r', 'e', 's', '\030', '\002', ' ', 
+'\001', '(', '\013', '2', '\033', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'F', 'e', 'a', 
+'t', 'u', 'r', 'e', 'S', 'e', 't', 'R', '\010', 'f', 'e', 'a', 't', 'u', 'r', 'e', 's', '\022', '(', '\n', '\014', 'd', 'e', 'b', 'u', 
+'g', '_', 'r', 'e', 'd', 'a', 'c', 't', '\030', '\003', ' ', '\001', '(', '\010', ':', '\005', 'f', 'a', 'l', 's', 'e', 'R', '\013', 'd', 'e', 
+'b', 'u', 'g', 'R', 'e', 'd', 'a', 'c', 't', '\022', 'X', '\n', '\024', 'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 
+'d', '_', 'o', 'p', 't', 'i', 'o', 'n', '\030', '\347', '\007', ' ', '\003', '(', '\013', '2', '$', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 
+'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'U', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 
+'i', 'o', 'n', 'R', '\023', 'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', '*', 
+'\t', '\010', '\350', '\007', '\020', '\200', '\200', '\200', '\200', '\002', '\"', '\325', '\001', '\n', '\016', 'S', 'e', 'r', 'v', 'i', 'c', 'e', 'O', 'p', 't', 
+'i', 'o', 'n', 's', '\022', '7', '\n', '\010', 'f', 'e', 'a', 't', 'u', 'r', 'e', 's', '\030', '\"', ' ', '\001', '(', '\013', '2', '\033', '.', 
+'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'F', 'e', 'a', 't', 'u', 'r', 'e', 'S', 'e', 
+'t', 'R', '\010', 'f', 'e', 'a', 't', 'u', 'r', 'e', 's', '\022', '%', '\n', '\n', 'd', 'e', 'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', 
+'\030', '!', ' ', '\001', '(', '\010', ':', '\005', 'f', 'a', 'l', 's', 'e', 'R', '\n', 'd', 'e', 'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', 
 '\022', 'X', '\n', '\024', 'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', '_', 'o', 'p', 't', 'i', 'o', 'n', '\030', 
 '\347', '\007', ' ', '\003', '(', '\013', '2', '$', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 
 'U', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', 'R', '\023', 'u', 'n', 'i', 'n', 
 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', '*', '\t', '\010', '\350', '\007', '\020', '\200', '\200', '\200', '\200', 
-'\002', 'J', '\004', '\010', '\005', '\020', '\006', '\"', '\201', '\002', '\n', '\020', 'E', 'n', 'u', 'm', 'V', 'a', 'l', 'u', 'e', 'O', 'p', 't', 'i', 
-'o', 'n', 's', '\022', '%', '\n', '\n', 'd', 'e', 'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', '\030', '\001', ' ', '\001', '(', '\010', ':', '\005', 
-'f', 'a', 'l', 's', 'e', 'R', '\n', 'd', 'e', 'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', '\022', '7', '\n', '\010', 'f', 'e', 'a', 't', 
-'u', 'r', 'e', 's', '\030', '\002', ' ', '\001', '(', '\013', '2', '\033', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 
-'b', 'u', 'f', '.', 'F', 'e', 'a', 't', 'u', 'r', 'e', 'S', 'e', 't', 'R', '\010', 'f', 'e', 'a', 't', 'u', 'r', 'e', 's', '\022', 
-'(', '\n', '\014', 'd', 'e', 'b', 'u', 'g', '_', 'r', 'e', 'd', 'a', 'c', 't', '\030', '\003', ' ', '\001', '(', '\010', ':', '\005', 'f', 'a', 
-'l', 's', 'e', 'R', '\013', 'd', 'e', 'b', 'u', 'g', 'R', 'e', 'd', 'a', 'c', 't', '\022', 'X', '\n', '\024', 'u', 'n', 'i', 'n', 't', 
-'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', '_', 'o', 'p', 't', 'i', 'o', 'n', '\030', '\347', '\007', ' ', '\003', '(', '\013', '2', '$', '.', 
-'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'U', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 
-'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', 'R', '\023', 'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 
-'O', 'p', 't', 'i', 'o', 'n', '*', '\t', '\010', '\350', '\007', '\020', '\200', '\200', '\200', '\200', '\002', '\"', '\325', '\001', '\n', '\016', 'S', 'e', 'r', 
-'v', 'i', 'c', 'e', 'O', 'p', 't', 'i', 'o', 'n', 's', '\022', '7', '\n', '\010', 'f', 'e', 'a', 't', 'u', 'r', 'e', 's', '\030', '\"', 
-' ', '\001', '(', '\013', '2', '\033', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'F', 'e', 
-'a', 't', 'u', 'r', 'e', 'S', 'e', 't', 'R', '\010', 'f', 'e', 'a', 't', 'u', 'r', 'e', 's', '\022', '%', '\n', '\n', 'd', 'e', 'p', 
-'r', 'e', 'c', 'a', 't', 'e', 'd', '\030', '!', ' ', '\001', '(', '\010', ':', '\005', 'f', 'a', 'l', 's', 'e', 'R', '\n', 'd', 'e', 'p', 
-'r', 'e', 'c', 'a', 't', 'e', 'd', '\022', 'X', '\n', '\024', 'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', '_', 
-'o', 'p', 't', 'i', 'o', 'n', '\030', '\347', '\007', ' ', '\003', '(', '\013', '2', '$', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 
-'o', 't', 'o', 'b', 'u', 'f', '.', 'U', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 
-'n', 'R', '\023', 'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', '*', '\t', '\010', 
-'\350', '\007', '\020', '\200', '\200', '\200', '\200', '\002', '\"', '\231', '\003', '\n', '\r', 'M', 'e', 't', 'h', 'o', 'd', 'O', 'p', 't', 'i', 'o', 'n', 
-'s', '\022', '%', '\n', '\n', 'd', 'e', 'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', '\030', '!', ' ', '\001', '(', '\010', ':', '\005', 'f', 'a', 
-'l', 's', 'e', 'R', '\n', 'd', 'e', 'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', '\022', 'q', '\n', '\021', 'i', 'd', 'e', 'm', 'p', 'o', 
-'t', 'e', 'n', 'c', 'y', '_', 'l', 'e', 'v', 'e', 'l', '\030', '\"', ' ', '\001', '(', '\016', '2', '/', '.', 'g', 'o', 'o', 'g', 'l', 
-'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'M', 'e', 't', 'h', 'o', 'd', 'O', 'p', 't', 'i', 'o', 'n', 's', '.', 
-'I', 'd', 'e', 'm', 'p', 'o', 't', 'e', 'n', 'c', 'y', 'L', 'e', 'v', 'e', 'l', ':', '\023', 'I', 'D', 'E', 'M', 'P', 'O', 'T', 
-'E', 'N', 'C', 'Y', '_', 'U', 'N', 'K', 'N', 'O', 'W', 'N', 'R', '\020', 'i', 'd', 'e', 'm', 'p', 'o', 't', 'e', 'n', 'c', 'y', 
-'L', 'e', 'v', 'e', 'l', '\022', '7', '\n', '\010', 'f', 'e', 'a', 't', 'u', 'r', 'e', 's', '\030', '#', ' ', '\001', '(', '\013', '2', '\033', 
-'.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'F', 'e', 'a', 't', 'u', 'r', 'e', 'S', 
-'e', 't', 'R', '\010', 'f', 'e', 'a', 't', 'u', 'r', 'e', 's', '\022', 'X', '\n', '\024', 'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 
-'e', 't', 'e', 'd', '_', 'o', 'p', 't', 'i', 'o', 'n', '\030', '\347', '\007', ' ', '\003', '(', '\013', '2', '$', '.', 'g', 'o', 'o', 'g', 
-'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'U', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 
-'O', 'p', 't', 'i', 'o', 'n', 'R', '\023', 'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 
-'o', 'n', '\"', 'P', '\n', '\020', 'I', 'd', 'e', 'm', 'p', 'o', 't', 'e', 'n', 'c', 'y', 'L', 'e', 'v', 'e', 'l', '\022', '\027', '\n', 
-'\023', 'I', 'D', 'E', 'M', 'P', 'O', 'T', 'E', 'N', 'C', 'Y', '_', 'U', 'N', 'K', 'N', 'O', 'W', 'N', '\020', '\000', '\022', '\023', '\n', 
-'\017', 'N', 'O', '_', 'S', 'I', 'D', 'E', '_', 'E', 'F', 'F', 'E', 'C', 'T', 'S', '\020', '\001', '\022', '\016', '\n', '\n', 'I', 'D', 'E', 
-'M', 'P', 'O', 'T', 'E', 'N', 'T', '\020', '\002', '*', '\t', '\010', '\350', '\007', '\020', '\200', '\200', '\200', '\200', '\002', '\"', '\232', '\003', '\n', '\023', 
-'U', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', '\022', 'A', '\n', '\004', 'n', 'a', 
-'m', 'e', '\030', '\002', ' ', '\003', '(', '\013', '2', '-', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 
-'f', '.', 'U', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', '.', 'N', 'a', 'm', 
-'e', 'P', 'a', 'r', 't', 'R', '\004', 'n', 'a', 'm', 'e', '\022', ')', '\n', '\020', 'i', 'd', 'e', 'n', 't', 'i', 'f', 'i', 'e', 'r', 
-'_', 'v', 'a', 'l', 'u', 'e', '\030', '\003', ' ', '\001', '(', '\t', 'R', '\017', 'i', 'd', 'e', 'n', 't', 'i', 'f', 'i', 'e', 'r', 'V', 
-'a', 'l', 'u', 'e', '\022', ',', '\n', '\022', 'p', 'o', 's', 'i', 't', 'i', 'v', 'e', '_', 'i', 'n', 't', '_', 'v', 'a', 'l', 'u', 
-'e', '\030', '\004', ' ', '\001', '(', '\004', 'R', '\020', 'p', 'o', 's', 'i', 't', 'i', 'v', 'e', 'I', 'n', 't', 'V', 'a', 'l', 'u', 'e', 
-'\022', ',', '\n', '\022', 'n', 'e', 'g', 'a', 't', 'i', 'v', 'e', '_', 'i', 'n', 't', '_', 'v', 'a', 'l', 'u', 'e', '\030', '\005', ' ', 
-'\001', '(', '\003', 'R', '\020', 'n', 'e', 'g', 'a', 't', 'i', 'v', 'e', 'I', 'n', 't', 'V', 'a', 'l', 'u', 'e', '\022', '!', '\n', '\014', 
-'d', 'o', 'u', 'b', 'l', 'e', '_', 'v', 'a', 'l', 'u', 'e', '\030', '\006', ' ', '\001', '(', '\001', 'R', '\013', 'd', 'o', 'u', 'b', 'l', 
-'e', 'V', 'a', 'l', 'u', 'e', '\022', '!', '\n', '\014', 's', 't', 'r', 'i', 'n', 'g', '_', 'v', 'a', 'l', 'u', 'e', '\030', '\007', ' ', 
-'\001', '(', '\014', 'R', '\013', 's', 't', 'r', 'i', 'n', 'g', 'V', 'a', 'l', 'u', 'e', '\022', '\'', '\n', '\017', 'a', 'g', 'g', 'r', 'e', 
-'g', 'a', 't', 'e', '_', 'v', 'a', 'l', 'u', 'e', '\030', '\010', ' ', '\001', '(', '\t', 'R', '\016', 'a', 'g', 'g', 'r', 'e', 'g', 'a', 
-'t', 'e', 'V', 'a', 'l', 'u', 'e', '\032', 'J', '\n', '\010', 'N', 'a', 'm', 'e', 'P', 'a', 'r', 't', '\022', '\033', '\n', '\t', 'n', 'a', 
-'m', 'e', '_', 'p', 'a', 'r', 't', '\030', '\001', ' ', '\002', '(', '\t', 'R', '\010', 'n', 'a', 'm', 'e', 'P', 'a', 'r', 't', '\022', '!', 
-'\n', '\014', 'i', 's', '_', 'e', 'x', 't', 'e', 'n', 's', 'i', 'o', 'n', '\030', '\002', ' ', '\002', '(', '\010', 'R', '\013', 'i', 's', 'E', 
-'x', 't', 'e', 'n', 's', 'i', 'o', 'n', '\"', '\214', '\n', '\n', '\n', 'F', 'e', 'a', 't', 'u', 'r', 'e', 'S', 'e', 't', '\022', '\213', 
-'\001', '\n', '\016', 'f', 'i', 'e', 'l', 'd', '_', 'p', 'r', 'e', 's', 'e', 'n', 'c', 'e', '\030', '\001', ' ', '\001', '(', '\016', '2', ')', 
-'.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'F', 'e', 'a', 't', 'u', 'r', 'e', 'S', 
-'e', 't', '.', 'F', 'i', 'e', 'l', 'd', 'P', 'r', 'e', 's', 'e', 'n', 'c', 'e', 'B', '9', '\210', '\001', '\001', '\230', '\001', '\004', '\230', 
-'\001', '\001', '\242', '\001', '\r', '\022', '\010', 'E', 'X', 'P', 'L', 'I', 'C', 'I', 'T', '\030', '\346', '\007', '\242', '\001', '\r', '\022', '\010', 'I', 'M', 
-'P', 'L', 'I', 'C', 'I', 'T', '\030', '\347', '\007', '\242', '\001', '\r', '\022', '\010', 'E', 'X', 'P', 'L', 'I', 'C', 'I', 'T', '\030', '\350', '\007', 
-'R', '\r', 'f', 'i', 'e', 'l', 'd', 'P', 'r', 'e', 's', 'e', 'n', 'c', 'e', '\022', 'f', '\n', '\t', 'e', 'n', 'u', 'm', '_', 't', 
-'y', 'p', 'e', '\030', '\002', ' ', '\001', '(', '\016', '2', '$', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 
-'u', 'f', '.', 'F', 'e', 'a', 't', 'u', 'r', 'e', 'S', 'e', 't', '.', 'E', 'n', 'u', 'm', 'T', 'y', 'p', 'e', 'B', '#', '\210', 
-'\001', '\001', '\230', '\001', '\006', '\230', '\001', '\001', '\242', '\001', '\013', '\022', '\006', 'C', 'L', 'O', 'S', 'E', 'D', '\030', '\346', '\007', '\242', '\001', '\t', 
-'\022', '\004', 'O', 'P', 'E', 'N', '\030', '\347', '\007', 'R', '\010', 'e', 'n', 'u', 'm', 'T', 'y', 'p', 'e', '\022', '\222', '\001', '\n', '\027', 'r', 
-'e', 'p', 'e', 'a', 't', 'e', 'd', '_', 'f', 'i', 'e', 'l', 'd', '_', 'e', 'n', 'c', 'o', 'd', 'i', 'n', 'g', '\030', '\003', ' ', 
-'\001', '(', '\016', '2', '1', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'F', 'e', 'a', 
-'t', 'u', 'r', 'e', 'S', 'e', 't', '.', 'R', 'e', 'p', 'e', 'a', 't', 'e', 'd', 'F', 'i', 'e', 'l', 'd', 'E', 'n', 'c', 'o', 
-'d', 'i', 'n', 'g', 'B', '\'', '\210', '\001', '\001', '\230', '\001', '\004', '\230', '\001', '\001', '\242', '\001', '\r', '\022', '\010', 'E', 'X', 'P', 'A', 'N', 
-'D', 'E', 'D', '\030', '\346', '\007', '\242', '\001', '\013', '\022', '\006', 'P', 'A', 'C', 'K', 'E', 'D', '\030', '\347', '\007', 'R', '\025', 'r', 'e', 'p', 
-'e', 'a', 't', 'e', 'd', 'F', 'i', 'e', 'l', 'd', 'E', 'n', 'c', 'o', 'd', 'i', 'n', 'g', '\022', 'x', '\n', '\017', 'u', 't', 'f', 
-'8', '_', 'v', 'a', 'l', 'i', 'd', 'a', 't', 'i', 'o', 'n', '\030', '\004', ' ', '\001', '(', '\016', '2', '*', '.', 'g', 'o', 'o', 'g', 
-'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'F', 'e', 'a', 't', 'u', 'r', 'e', 'S', 'e', 't', '.', 'U', 't', 
-'f', '8', 'V', 'a', 'l', 'i', 'd', 'a', 't', 'i', 'o', 'n', 'B', '#', '\210', '\001', '\001', '\230', '\001', '\004', '\230', '\001', '\001', '\242', '\001', 
-'\t', '\022', '\004', 'N', 'O', 'N', 'E', '\030', '\346', '\007', '\242', '\001', '\013', '\022', '\006', 'V', 'E', 'R', 'I', 'F', 'Y', '\030', '\347', '\007', 'R', 
-'\016', 'u', 't', 'f', '8', 'V', 'a', 'l', 'i', 'd', 'a', 't', 'i', 'o', 'n', '\022', 'x', '\n', '\020', 'm', 'e', 's', 's', 'a', 'g', 
-'e', '_', 'e', 'n', 'c', 'o', 'd', 'i', 'n', 'g', '\030', '\005', ' ', '\001', '(', '\016', '2', '+', '.', 'g', 'o', 'o', 'g', 'l', 'e', 
-'.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'F', 'e', 'a', 't', 'u', 'r', 'e', 'S', 'e', 't', '.', 'M', 'e', 's', 's', 
-'a', 'g', 'e', 'E', 'n', 'c', 'o', 'd', 'i', 'n', 'g', 'B', ' ', '\210', '\001', '\001', '\230', '\001', '\004', '\230', '\001', '\001', '\242', '\001', '\024', 
-'\022', '\017', 'L', 'E', 'N', 'G', 'T', 'H', '_', 'P', 'R', 'E', 'F', 'I', 'X', 'E', 'D', '\030', '\346', '\007', 'R', '\017', 'm', 'e', 's', 
-'s', 'a', 'g', 'e', 'E', 'n', 'c', 'o', 'd', 'i', 'n', 'g', '\022', '|', '\n', '\013', 'j', 's', 'o', 'n', '_', 'f', 'o', 'r', 'm', 
-'a', 't', '\030', '\006', ' ', '\001', '(', '\016', '2', '&', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 
-'f', '.', 'F', 'e', 'a', 't', 'u', 'r', 'e', 'S', 'e', 't', '.', 'J', 's', 'o', 'n', 'F', 'o', 'r', 'm', 'a', 't', 'B', '3', 
-'\210', '\001', '\001', '\230', '\001', '\003', '\230', '\001', '\006', '\230', '\001', '\001', '\242', '\001', '\027', '\022', '\022', 'L', 'E', 'G', 'A', 'C', 'Y', '_', 'B', 
-'E', 'S', 'T', '_', 'E', 'F', 'F', 'O', 'R', 'T', '\030', '\346', '\007', '\242', '\001', '\n', '\022', '\005', 'A', 'L', 'L', 'O', 'W', '\030', '\347', 
-'\007', 'R', '\n', 'j', 's', 'o', 'n', 'F', 'o', 'r', 'm', 'a', 't', '\"', '\\', '\n', '\r', 'F', 'i', 'e', 'l', 'd', 'P', 'r', 'e', 
-'s', 'e', 'n', 'c', 'e', '\022', '\032', '\n', '\026', 'F', 'I', 'E', 'L', 'D', '_', 'P', 'R', 'E', 'S', 'E', 'N', 'C', 'E', '_', 'U', 
-'N', 'K', 'N', 'O', 'W', 'N', '\020', '\000', '\022', '\014', '\n', '\010', 'E', 'X', 'P', 'L', 'I', 'C', 'I', 'T', '\020', '\001', '\022', '\014', '\n', 
-'\010', 'I', 'M', 'P', 'L', 'I', 'C', 'I', 'T', '\020', '\002', '\022', '\023', '\n', '\017', 'L', 'E', 'G', 'A', 'C', 'Y', '_', 'R', 'E', 'Q', 
-'U', 'I', 'R', 'E', 'D', '\020', '\003', '\"', '7', '\n', '\010', 'E', 'n', 'u', 'm', 'T', 'y', 'p', 'e', '\022', '\025', '\n', '\021', 'E', 'N', 
-'U', 'M', '_', 'T', 'Y', 'P', 'E', '_', 'U', 'N', 'K', 'N', 'O', 'W', 'N', '\020', '\000', '\022', '\010', '\n', '\004', 'O', 'P', 'E', 'N', 
-'\020', '\001', '\022', '\n', '\n', '\006', 'C', 'L', 'O', 'S', 'E', 'D', '\020', '\002', '\"', 'V', '\n', '\025', 'R', 'e', 'p', 'e', 'a', 't', 'e', 
-'d', 'F', 'i', 'e', 'l', 'd', 'E', 'n', 'c', 'o', 'd', 'i', 'n', 'g', '\022', '#', '\n', '\037', 'R', 'E', 'P', 'E', 'A', 'T', 'E', 
-'D', '_', 'F', 'I', 'E', 'L', 'D', '_', 'E', 'N', 'C', 'O', 'D', 'I', 'N', 'G', '_', 'U', 'N', 'K', 'N', 'O', 'W', 'N', '\020', 
-'\000', '\022', '\n', '\n', '\006', 'P', 'A', 'C', 'K', 'E', 'D', '\020', '\001', '\022', '\014', '\n', '\010', 'E', 'X', 'P', 'A', 'N', 'D', 'E', 'D', 
-'\020', '\002', '\"', 'C', '\n', '\016', 'U', 't', 'f', '8', 'V', 'a', 'l', 'i', 'd', 'a', 't', 'i', 'o', 'n', '\022', '\033', '\n', '\027', 'U', 
-'T', 'F', '8', '_', 'V', 'A', 'L', 'I', 'D', 'A', 'T', 'I', 'O', 'N', '_', 'U', 'N', 'K', 'N', 'O', 'W', 'N', '\020', '\000', '\022', 
-'\n', '\n', '\006', 'V', 'E', 'R', 'I', 'F', 'Y', '\020', '\002', '\022', '\010', '\n', '\004', 'N', 'O', 'N', 'E', '\020', '\003', '\"', 'S', '\n', '\017', 
-'M', 'e', 's', 's', 'a', 'g', 'e', 'E', 'n', 'c', 'o', 'd', 'i', 'n', 'g', '\022', '\034', '\n', '\030', 'M', 'E', 'S', 'S', 'A', 'G', 
-'E', '_', 'E', 'N', 'C', 'O', 'D', 'I', 'N', 'G', '_', 'U', 'N', 'K', 'N', 'O', 'W', 'N', '\020', '\000', '\022', '\023', '\n', '\017', 'L', 
-'E', 'N', 'G', 'T', 'H', '_', 'P', 'R', 'E', 'F', 'I', 'X', 'E', 'D', '\020', '\001', '\022', '\r', '\n', '\t', 'D', 'E', 'L', 'I', 'M', 
-'I', 'T', 'E', 'D', '\020', '\002', '\"', 'H', '\n', '\n', 'J', 's', 'o', 'n', 'F', 'o', 'r', 'm', 'a', 't', '\022', '\027', '\n', '\023', 'J', 
-'S', 'O', 'N', '_', 'F', 'O', 'R', 'M', 'A', 'T', '_', 'U', 'N', 'K', 'N', 'O', 'W', 'N', '\020', '\000', '\022', '\t', '\n', '\005', 'A', 
-'L', 'L', 'O', 'W', '\020', '\001', '\022', '\026', '\n', '\022', 'L', 'E', 'G', 'A', 'C', 'Y', '_', 'B', 'E', 'S', 'T', '_', 'E', 'F', 'F', 
-'O', 'R', 'T', '\020', '\002', '*', '\006', '\010', '\350', '\007', '\020', '\351', '\007', '*', '\006', '\010', '\351', '\007', '\020', '\352', '\007', '*', '\006', '\010', '\352', 
-'\007', '\020', '\353', '\007', '*', '\006', '\010', '\213', 'N', '\020', '\220', 'N', '*', '\006', '\010', '\220', 'N', '\020', '\221', 'N', 'J', '\006', '\010', '\347', '\007', 
-'\020', '\350', '\007', '\"', '\376', '\002', '\n', '\022', 'F', 'e', 'a', 't', 'u', 'r', 'e', 'S', 'e', 't', 'D', 'e', 'f', 'a', 'u', 'l', 't', 
-'s', '\022', 'X', '\n', '\010', 'd', 'e', 'f', 'a', 'u', 'l', 't', 's', '\030', '\001', ' ', '\003', '(', '\013', '2', '<', '.', 'g', 'o', 'o', 
-'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'F', 'e', 'a', 't', 'u', 'r', 'e', 'S', 'e', 't', 'D', 'e', 
-'f', 'a', 'u', 'l', 't', 's', '.', 'F', 'e', 'a', 't', 'u', 'r', 'e', 'S', 'e', 't', 'E', 'd', 'i', 't', 'i', 'o', 'n', 'D', 
-'e', 'f', 'a', 'u', 'l', 't', 'R', '\010', 'd', 'e', 'f', 'a', 'u', 'l', 't', 's', '\022', 'A', '\n', '\017', 'm', 'i', 'n', 'i', 'm', 
-'u', 'm', '_', 'e', 'd', 'i', 't', 'i', 'o', 'n', '\030', '\004', ' ', '\001', '(', '\016', '2', '\030', '.', 'g', 'o', 'o', 'g', 'l', 'e', 
-'.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'E', 'd', 'i', 't', 'i', 'o', 'n', 'R', '\016', 'm', 'i', 'n', 'i', 'm', 'u', 
-'m', 'E', 'd', 'i', 't', 'i', 'o', 'n', '\022', 'A', '\n', '\017', 'm', 'a', 'x', 'i', 'm', 'u', 'm', '_', 'e', 'd', 'i', 't', 'i', 
-'o', 'n', '\030', '\005', ' ', '\001', '(', '\016', '2', '\030', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 
-'f', '.', 'E', 'd', 'i', 't', 'i', 'o', 'n', 'R', '\016', 'm', 'a', 'x', 'i', 'm', 'u', 'm', 'E', 'd', 'i', 't', 'i', 'o', 'n', 
-'\032', '\207', '\001', '\n', '\030', 'F', 'e', 'a', 't', 'u', 'r', 'e', 'S', 'e', 't', 'E', 'd', 'i', 't', 'i', 'o', 'n', 'D', 'e', 'f', 
-'a', 'u', 'l', 't', '\022', '2', '\n', '\007', 'e', 'd', 'i', 't', 'i', 'o', 'n', '\030', '\003', ' ', '\001', '(', '\016', '2', '\030', '.', 'g', 
-'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'E', 'd', 'i', 't', 'i', 'o', 'n', 'R', '\007', 'e', 
-'d', 'i', 't', 'i', 'o', 'n', '\022', '7', '\n', '\010', 'f', 'e', 'a', 't', 'u', 'r', 'e', 's', '\030', '\002', ' ', '\001', '(', '\013', '2', 
+'\002', '\"', '\231', '\003', '\n', '\r', 'M', 'e', 't', 'h', 'o', 'd', 'O', 'p', 't', 'i', 'o', 'n', 's', '\022', '%', '\n', '\n', 'd', 'e', 
+'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', '\030', '!', ' ', '\001', '(', '\010', ':', '\005', 'f', 'a', 'l', 's', 'e', 'R', '\n', 'd', 'e', 
+'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', '\022', 'q', '\n', '\021', 'i', 'd', 'e', 'm', 'p', 'o', 't', 'e', 'n', 'c', 'y', '_', 'l', 
+'e', 'v', 'e', 'l', '\030', '\"', ' ', '\001', '(', '\016', '2', '/', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 
+'b', 'u', 'f', '.', 'M', 'e', 't', 'h', 'o', 'd', 'O', 'p', 't', 'i', 'o', 'n', 's', '.', 'I', 'd', 'e', 'm', 'p', 'o', 't', 
+'e', 'n', 'c', 'y', 'L', 'e', 'v', 'e', 'l', ':', '\023', 'I', 'D', 'E', 'M', 'P', 'O', 'T', 'E', 'N', 'C', 'Y', '_', 'U', 'N', 
+'K', 'N', 'O', 'W', 'N', 'R', '\020', 'i', 'd', 'e', 'm', 'p', 'o', 't', 'e', 'n', 'c', 'y', 'L', 'e', 'v', 'e', 'l', '\022', '7', 
+'\n', '\010', 'f', 'e', 'a', 't', 'u', 'r', 'e', 's', '\030', '#', ' ', '\001', '(', '\013', '2', '\033', '.', 'g', 'o', 'o', 'g', 'l', 'e', 
+'.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'F', 'e', 'a', 't', 'u', 'r', 'e', 'S', 'e', 't', 'R', '\010', 'f', 'e', 'a', 
+'t', 'u', 'r', 'e', 's', '\022', 'X', '\n', '\024', 'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', '_', 'o', 'p', 
+'t', 'i', 'o', 'n', '\030', '\347', '\007', ' ', '\003', '(', '\013', '2', '$', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 
+'o', 'b', 'u', 'f', '.', 'U', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', 'R', 
+'\023', 'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', '\"', 'P', '\n', '\020', 'I', 
+'d', 'e', 'm', 'p', 'o', 't', 'e', 'n', 'c', 'y', 'L', 'e', 'v', 'e', 'l', '\022', '\027', '\n', '\023', 'I', 'D', 'E', 'M', 'P', 'O', 
+'T', 'E', 'N', 'C', 'Y', '_', 'U', 'N', 'K', 'N', 'O', 'W', 'N', '\020', '\000', '\022', '\023', '\n', '\017', 'N', 'O', '_', 'S', 'I', 'D', 
+'E', '_', 'E', 'F', 'F', 'E', 'C', 'T', 'S', '\020', '\001', '\022', '\016', '\n', '\n', 'I', 'D', 'E', 'M', 'P', 'O', 'T', 'E', 'N', 'T', 
+'\020', '\002', '*', '\t', '\010', '\350', '\007', '\020', '\200', '\200', '\200', '\200', '\002', '\"', '\232', '\003', '\n', '\023', 'U', 'n', 'i', 'n', 't', 'e', 'r', 
+'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', '\022', 'A', '\n', '\004', 'n', 'a', 'm', 'e', '\030', '\002', ' ', '\003', '(', 
+'\013', '2', '-', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'U', 'n', 'i', 'n', 't', 
+'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', '.', 'N', 'a', 'm', 'e', 'P', 'a', 'r', 't', 'R', '\004', 
+'n', 'a', 'm', 'e', '\022', ')', '\n', '\020', 'i', 'd', 'e', 'n', 't', 'i', 'f', 'i', 'e', 'r', '_', 'v', 'a', 'l', 'u', 'e', '\030', 
+'\003', ' ', '\001', '(', '\t', 'R', '\017', 'i', 'd', 'e', 'n', 't', 'i', 'f', 'i', 'e', 'r', 'V', 'a', 'l', 'u', 'e', '\022', ',', '\n', 
+'\022', 'p', 'o', 's', 'i', 't', 'i', 'v', 'e', '_', 'i', 'n', 't', '_', 'v', 'a', 'l', 'u', 'e', '\030', '\004', ' ', '\001', '(', '\004', 
+'R', '\020', 'p', 'o', 's', 'i', 't', 'i', 'v', 'e', 'I', 'n', 't', 'V', 'a', 'l', 'u', 'e', '\022', ',', '\n', '\022', 'n', 'e', 'g', 
+'a', 't', 'i', 'v', 'e', '_', 'i', 'n', 't', '_', 'v', 'a', 'l', 'u', 'e', '\030', '\005', ' ', '\001', '(', '\003', 'R', '\020', 'n', 'e', 
+'g', 'a', 't', 'i', 'v', 'e', 'I', 'n', 't', 'V', 'a', 'l', 'u', 'e', '\022', '!', '\n', '\014', 'd', 'o', 'u', 'b', 'l', 'e', '_', 
+'v', 'a', 'l', 'u', 'e', '\030', '\006', ' ', '\001', '(', '\001', 'R', '\013', 'd', 'o', 'u', 'b', 'l', 'e', 'V', 'a', 'l', 'u', 'e', '\022', 
+'!', '\n', '\014', 's', 't', 'r', 'i', 'n', 'g', '_', 'v', 'a', 'l', 'u', 'e', '\030', '\007', ' ', '\001', '(', '\014', 'R', '\013', 's', 't', 
+'r', 'i', 'n', 'g', 'V', 'a', 'l', 'u', 'e', '\022', '\'', '\n', '\017', 'a', 'g', 'g', 'r', 'e', 'g', 'a', 't', 'e', '_', 'v', 'a', 
+'l', 'u', 'e', '\030', '\010', ' ', '\001', '(', '\t', 'R', '\016', 'a', 'g', 'g', 'r', 'e', 'g', 'a', 't', 'e', 'V', 'a', 'l', 'u', 'e', 
+'\032', 'J', '\n', '\010', 'N', 'a', 'm', 'e', 'P', 'a', 'r', 't', '\022', '\033', '\n', '\t', 'n', 'a', 'm', 'e', '_', 'p', 'a', 'r', 't', 
+'\030', '\001', ' ', '\002', '(', '\t', 'R', '\010', 'n', 'a', 'm', 'e', 'P', 'a', 'r', 't', '\022', '!', '\n', '\014', 'i', 's', '_', 'e', 'x', 
+'t', 'e', 'n', 's', 'i', 'o', 'n', '\030', '\002', ' ', '\002', '(', '\010', 'R', '\013', 'i', 's', 'E', 'x', 't', 'e', 'n', 's', 'i', 'o', 
+'n', '\"', '\271', '\n', '\n', '\n', 'F', 'e', 'a', 't', 'u', 'r', 'e', 'S', 'e', 't', '\022', '\221', '\001', '\n', '\016', 'f', 'i', 'e', 'l', 
+'d', '_', 'p', 'r', 'e', 's', 'e', 'n', 'c', 'e', '\030', '\001', ' ', '\001', '(', '\016', '2', ')', '.', 'g', 'o', 'o', 'g', 'l', 'e', 
+'.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'F', 'e', 'a', 't', 'u', 'r', 'e', 'S', 'e', 't', '.', 'F', 'i', 'e', 'l', 
+'d', 'P', 'r', 'e', 's', 'e', 'n', 'c', 'e', 'B', '?', '\210', '\001', '\001', '\230', '\001', '\004', '\230', '\001', '\001', '\242', '\001', '\r', '\022', '\010', 
+'E', 'X', 'P', 'L', 'I', 'C', 'I', 'T', '\030', '\346', '\007', '\242', '\001', '\r', '\022', '\010', 'I', 'M', 'P', 'L', 'I', 'C', 'I', 'T', '\030', 
+'\347', '\007', '\242', '\001', '\r', '\022', '\010', 'E', 'X', 'P', 'L', 'I', 'C', 'I', 'T', '\030', '\350', '\007', '\262', '\001', '\003', '\010', '\350', '\007', 'R', 
+'\r', 'f', 'i', 'e', 'l', 'd', 'P', 'r', 'e', 's', 'e', 'n', 'c', 'e', '\022', 'l', '\n', '\t', 'e', 'n', 'u', 'm', '_', 't', 'y', 
+'p', 'e', '\030', '\002', ' ', '\001', '(', '\016', '2', '$', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 
+'f', '.', 'F', 'e', 'a', 't', 'u', 'r', 'e', 'S', 'e', 't', '.', 'E', 'n', 'u', 'm', 'T', 'y', 'p', 'e', 'B', ')', '\210', '\001', 
+'\001', '\230', '\001', '\006', '\230', '\001', '\001', '\242', '\001', '\013', '\022', '\006', 'C', 'L', 'O', 'S', 'E', 'D', '\030', '\346', '\007', '\242', '\001', '\t', '\022', 
+'\004', 'O', 'P', 'E', 'N', '\030', '\347', '\007', '\262', '\001', '\003', '\010', '\350', '\007', 'R', '\010', 'e', 'n', 'u', 'm', 'T', 'y', 'p', 'e', '\022', 
+'\230', '\001', '\n', '\027', 'r', 'e', 'p', 'e', 'a', 't', 'e', 'd', '_', 'f', 'i', 'e', 'l', 'd', '_', 'e', 'n', 'c', 'o', 'd', 'i', 
+'n', 'g', '\030', '\003', ' ', '\001', '(', '\016', '2', '1', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 
+'f', '.', 'F', 'e', 'a', 't', 'u', 'r', 'e', 'S', 'e', 't', '.', 'R', 'e', 'p', 'e', 'a', 't', 'e', 'd', 'F', 'i', 'e', 'l', 
+'d', 'E', 'n', 'c', 'o', 'd', 'i', 'n', 'g', 'B', '-', '\210', '\001', '\001', '\230', '\001', '\004', '\230', '\001', '\001', '\242', '\001', '\r', '\022', '\010', 
+'E', 'X', 'P', 'A', 'N', 'D', 'E', 'D', '\030', '\346', '\007', '\242', '\001', '\013', '\022', '\006', 'P', 'A', 'C', 'K', 'E', 'D', '\030', '\347', '\007', 
+'\262', '\001', '\003', '\010', '\350', '\007', 'R', '\025', 'r', 'e', 'p', 'e', 'a', 't', 'e', 'd', 'F', 'i', 'e', 'l', 'd', 'E', 'n', 'c', 'o', 
+'d', 'i', 'n', 'g', '\022', '~', '\n', '\017', 'u', 't', 'f', '8', '_', 'v', 'a', 'l', 'i', 'd', 'a', 't', 'i', 'o', 'n', '\030', '\004', 
+' ', '\001', '(', '\016', '2', '*', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'F', 'e', 
+'a', 't', 'u', 'r', 'e', 'S', 'e', 't', '.', 'U', 't', 'f', '8', 'V', 'a', 'l', 'i', 'd', 'a', 't', 'i', 'o', 'n', 'B', ')', 
+'\210', '\001', '\001', '\230', '\001', '\004', '\230', '\001', '\001', '\242', '\001', '\t', '\022', '\004', 'N', 'O', 'N', 'E', '\030', '\346', '\007', '\242', '\001', '\013', '\022', 
+'\006', 'V', 'E', 'R', 'I', 'F', 'Y', '\030', '\347', '\007', '\262', '\001', '\003', '\010', '\350', '\007', 'R', '\016', 'u', 't', 'f', '8', 'V', 'a', 'l', 
+'i', 'd', 'a', 't', 'i', 'o', 'n', '\022', '~', '\n', '\020', 'm', 'e', 's', 's', 'a', 'g', 'e', '_', 'e', 'n', 'c', 'o', 'd', 'i', 
+'n', 'g', '\030', '\005', ' ', '\001', '(', '\016', '2', '+', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 
+'f', '.', 'F', 'e', 'a', 't', 'u', 'r', 'e', 'S', 'e', 't', '.', 'M', 'e', 's', 's', 'a', 'g', 'e', 'E', 'n', 'c', 'o', 'd', 
+'i', 'n', 'g', 'B', '&', '\210', '\001', '\001', '\230', '\001', '\004', '\230', '\001', '\001', '\242', '\001', '\024', '\022', '\017', 'L', 'E', 'N', 'G', 'T', 'H', 
+'_', 'P', 'R', 'E', 'F', 'I', 'X', 'E', 'D', '\030', '\346', '\007', '\262', '\001', '\003', '\010', '\350', '\007', 'R', '\017', 'm', 'e', 's', 's', 'a', 
+'g', 'e', 'E', 'n', 'c', 'o', 'd', 'i', 'n', 'g', '\022', '\202', '\001', '\n', '\013', 'j', 's', 'o', 'n', '_', 'f', 'o', 'r', 'm', 'a', 
+'t', '\030', '\006', ' ', '\001', '(', '\016', '2', '&', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', 
+'.', 'F', 'e', 'a', 't', 'u', 'r', 'e', 'S', 'e', 't', '.', 'J', 's', 'o', 'n', 'F', 'o', 'r', 'm', 'a', 't', 'B', '9', '\210', 
+'\001', '\001', '\230', '\001', '\003', '\230', '\001', '\006', '\230', '\001', '\001', '\242', '\001', '\027', '\022', '\022', 'L', 'E', 'G', 'A', 'C', 'Y', '_', 'B', 'E', 
+'S', 'T', '_', 'E', 'F', 'F', 'O', 'R', 'T', '\030', '\346', '\007', '\242', '\001', '\n', '\022', '\005', 'A', 'L', 'L', 'O', 'W', '\030', '\347', '\007', 
+'\262', '\001', '\003', '\010', '\350', '\007', 'R', '\n', 'j', 's', 'o', 'n', 'F', 'o', 'r', 'm', 'a', 't', '\"', '\\', '\n', '\r', 'F', 'i', 'e', 
+'l', 'd', 'P', 'r', 'e', 's', 'e', 'n', 'c', 'e', '\022', '\032', '\n', '\026', 'F', 'I', 'E', 'L', 'D', '_', 'P', 'R', 'E', 'S', 'E', 
+'N', 'C', 'E', '_', 'U', 'N', 'K', 'N', 'O', 'W', 'N', '\020', '\000', '\022', '\014', '\n', '\010', 'E', 'X', 'P', 'L', 'I', 'C', 'I', 'T', 
+'\020', '\001', '\022', '\014', '\n', '\010', 'I', 'M', 'P', 'L', 'I', 'C', 'I', 'T', '\020', '\002', '\022', '\023', '\n', '\017', 'L', 'E', 'G', 'A', 'C', 
+'Y', '_', 'R', 'E', 'Q', 'U', 'I', 'R', 'E', 'D', '\020', '\003', '\"', '7', '\n', '\010', 'E', 'n', 'u', 'm', 'T', 'y', 'p', 'e', '\022', 
+'\025', '\n', '\021', 'E', 'N', 'U', 'M', '_', 'T', 'Y', 'P', 'E', '_', 'U', 'N', 'K', 'N', 'O', 'W', 'N', '\020', '\000', '\022', '\010', '\n', 
+'\004', 'O', 'P', 'E', 'N', '\020', '\001', '\022', '\n', '\n', '\006', 'C', 'L', 'O', 'S', 'E', 'D', '\020', '\002', '\"', 'V', '\n', '\025', 'R', 'e', 
+'p', 'e', 'a', 't', 'e', 'd', 'F', 'i', 'e', 'l', 'd', 'E', 'n', 'c', 'o', 'd', 'i', 'n', 'g', '\022', '#', '\n', '\037', 'R', 'E', 
+'P', 'E', 'A', 'T', 'E', 'D', '_', 'F', 'I', 'E', 'L', 'D', '_', 'E', 'N', 'C', 'O', 'D', 'I', 'N', 'G', '_', 'U', 'N', 'K', 
+'N', 'O', 'W', 'N', '\020', '\000', '\022', '\n', '\n', '\006', 'P', 'A', 'C', 'K', 'E', 'D', '\020', '\001', '\022', '\014', '\n', '\010', 'E', 'X', 'P', 
+'A', 'N', 'D', 'E', 'D', '\020', '\002', '\"', 'C', '\n', '\016', 'U', 't', 'f', '8', 'V', 'a', 'l', 'i', 'd', 'a', 't', 'i', 'o', 'n', 
+'\022', '\033', '\n', '\027', 'U', 'T', 'F', '8', '_', 'V', 'A', 'L', 'I', 'D', 'A', 'T', 'I', 'O', 'N', '_', 'U', 'N', 'K', 'N', 'O', 
+'W', 'N', '\020', '\000', '\022', '\n', '\n', '\006', 'V', 'E', 'R', 'I', 'F', 'Y', '\020', '\002', '\022', '\010', '\n', '\004', 'N', 'O', 'N', 'E', '\020', 
+'\003', '\"', 'S', '\n', '\017', 'M', 'e', 's', 's', 'a', 'g', 'e', 'E', 'n', 'c', 'o', 'd', 'i', 'n', 'g', '\022', '\034', '\n', '\030', 'M', 
+'E', 'S', 'S', 'A', 'G', 'E', '_', 'E', 'N', 'C', 'O', 'D', 'I', 'N', 'G', '_', 'U', 'N', 'K', 'N', 'O', 'W', 'N', '\020', '\000', 
+'\022', '\023', '\n', '\017', 'L', 'E', 'N', 'G', 'T', 'H', '_', 'P', 'R', 'E', 'F', 'I', 'X', 'E', 'D', '\020', '\001', '\022', '\r', '\n', '\t', 
+'D', 'E', 'L', 'I', 'M', 'I', 'T', 'E', 'D', '\020', '\002', '\"', 'H', '\n', '\n', 'J', 's', 'o', 'n', 'F', 'o', 'r', 'm', 'a', 't', 
+'\022', '\027', '\n', '\023', 'J', 'S', 'O', 'N', '_', 'F', 'O', 'R', 'M', 'A', 'T', '_', 'U', 'N', 'K', 'N', 'O', 'W', 'N', '\020', '\000', 
+'\022', '\t', '\n', '\005', 'A', 'L', 'L', 'O', 'W', '\020', '\001', '\022', '\026', '\n', '\022', 'L', 'E', 'G', 'A', 'C', 'Y', '_', 'B', 'E', 'S', 
+'T', '_', 'E', 'F', 'F', 'O', 'R', 'T', '\020', '\002', '*', '\006', '\010', '\350', '\007', '\020', '\351', '\007', '*', '\006', '\010', '\351', '\007', '\020', '\352', 
+'\007', '*', '\006', '\010', '\352', '\007', '\020', '\353', '\007', '*', '\006', '\010', '\206', 'N', '\020', '\207', 'N', '*', '\006', '\010', '\213', 'N', '\020', '\220', 'N', 
+'*', '\006', '\010', '\220', 'N', '\020', '\221', 'N', 'J', '\006', '\010', '\347', '\007', '\020', '\350', '\007', '\"', '\331', '\003', '\n', '\022', 'F', 'e', 'a', 't', 
+'u', 'r', 'e', 'S', 'e', 't', 'D', 'e', 'f', 'a', 'u', 'l', 't', 's', '\022', 'X', '\n', '\010', 'd', 'e', 'f', 'a', 'u', 'l', 't', 
+'s', '\030', '\001', ' ', '\003', '(', '\013', '2', '<', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', 
+'.', 'F', 'e', 'a', 't', 'u', 'r', 'e', 'S', 'e', 't', 'D', 'e', 'f', 'a', 'u', 'l', 't', 's', '.', 'F', 'e', 'a', 't', 'u', 
+'r', 'e', 'S', 'e', 't', 'E', 'd', 'i', 't', 'i', 'o', 'n', 'D', 'e', 'f', 'a', 'u', 'l', 't', 'R', '\010', 'd', 'e', 'f', 'a', 
+'u', 'l', 't', 's', '\022', 'A', '\n', '\017', 'm', 'i', 'n', 'i', 'm', 'u', 'm', '_', 'e', 'd', 'i', 't', 'i', 'o', 'n', '\030', '\004', 
+' ', '\001', '(', '\016', '2', '\030', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'E', 'd', 
+'i', 't', 'i', 'o', 'n', 'R', '\016', 'm', 'i', 'n', 'i', 'm', 'u', 'm', 'E', 'd', 'i', 't', 'i', 'o', 'n', '\022', 'A', '\n', '\017', 
+'m', 'a', 'x', 'i', 'm', 'u', 'm', '_', 'e', 'd', 'i', 't', 'i', 'o', 'n', '\030', '\005', ' ', '\001', '(', '\016', '2', '\030', '.', 'g', 
+'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'E', 'd', 'i', 't', 'i', 'o', 'n', 'R', '\016', 'm', 
+'a', 'x', 'i', 'm', 'u', 'm', 'E', 'd', 'i', 't', 'i', 'o', 'n', '\032', '\342', '\001', '\n', '\030', 'F', 'e', 'a', 't', 'u', 'r', 'e', 
+'S', 'e', 't', 'E', 'd', 'i', 't', 'i', 'o', 'n', 'D', 'e', 'f', 'a', 'u', 'l', 't', '\022', '2', '\n', '\007', 'e', 'd', 'i', 't', 
+'i', 'o', 'n', '\030', '\003', ' ', '\001', '(', '\016', '2', '\030', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 
+'u', 'f', '.', 'E', 'd', 'i', 't', 'i', 'o', 'n', 'R', '\007', 'e', 'd', 'i', 't', 'i', 'o', 'n', '\022', 'N', '\n', '\024', 'o', 'v', 
+'e', 'r', 'r', 'i', 'd', 'a', 'b', 'l', 'e', '_', 'f', 'e', 'a', 't', 'u', 'r', 'e', 's', '\030', '\004', ' ', '\001', '(', '\013', '2', 
 '\033', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'F', 'e', 'a', 't', 'u', 'r', 'e', 
-'S', 'e', 't', 'R', '\010', 'f', 'e', 'a', 't', 'u', 'r', 'e', 's', '\"', '\247', '\002', '\n', '\016', 'S', 'o', 'u', 'r', 'c', 'e', 'C', 
-'o', 'd', 'e', 'I', 'n', 'f', 'o', '\022', 'D', '\n', '\010', 'l', 'o', 'c', 'a', 't', 'i', 'o', 'n', '\030', '\001', ' ', '\003', '(', '\013', 
-'2', '(', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'S', 'o', 'u', 'r', 'c', 'e', 
-'C', 'o', 'd', 'e', 'I', 'n', 'f', 'o', '.', 'L', 'o', 'c', 'a', 't', 'i', 'o', 'n', 'R', '\010', 'l', 'o', 'c', 'a', 't', 'i', 
-'o', 'n', '\032', '\316', '\001', '\n', '\010', 'L', 'o', 'c', 'a', 't', 'i', 'o', 'n', '\022', '\026', '\n', '\004', 'p', 'a', 't', 'h', '\030', '\001', 
-' ', '\003', '(', '\005', 'B', '\002', '\020', '\001', 'R', '\004', 'p', 'a', 't', 'h', '\022', '\026', '\n', '\004', 's', 'p', 'a', 'n', '\030', '\002', ' ', 
-'\003', '(', '\005', 'B', '\002', '\020', '\001', 'R', '\004', 's', 'p', 'a', 'n', '\022', ')', '\n', '\020', 'l', 'e', 'a', 'd', 'i', 'n', 'g', '_', 
-'c', 'o', 'm', 'm', 'e', 'n', 't', 's', '\030', '\003', ' ', '\001', '(', '\t', 'R', '\017', 'l', 'e', 'a', 'd', 'i', 'n', 'g', 'C', 'o', 
-'m', 'm', 'e', 'n', 't', 's', '\022', '+', '\n', '\021', 't', 'r', 'a', 'i', 'l', 'i', 'n', 'g', '_', 'c', 'o', 'm', 'm', 'e', 'n', 
-'t', 's', '\030', '\004', ' ', '\001', '(', '\t', 'R', '\020', 't', 'r', 'a', 'i', 'l', 'i', 'n', 'g', 'C', 'o', 'm', 'm', 'e', 'n', 't', 
-'s', '\022', ':', '\n', '\031', 'l', 'e', 'a', 'd', 'i', 'n', 'g', '_', 'd', 'e', 't', 'a', 'c', 'h', 'e', 'd', '_', 'c', 'o', 'm', 
-'m', 'e', 'n', 't', 's', '\030', '\006', ' ', '\003', '(', '\t', 'R', '\027', 'l', 'e', 'a', 'd', 'i', 'n', 'g', 'D', 'e', 't', 'a', 'c', 
-'h', 'e', 'd', 'C', 'o', 'm', 'm', 'e', 'n', 't', 's', '\"', '\320', '\002', '\n', '\021', 'G', 'e', 'n', 'e', 'r', 'a', 't', 'e', 'd', 
-'C', 'o', 'd', 'e', 'I', 'n', 'f', 'o', '\022', 'M', '\n', '\n', 'a', 'n', 'n', 'o', 't', 'a', 't', 'i', 'o', 'n', '\030', '\001', ' ', 
-'\003', '(', '\013', '2', '-', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'G', 'e', 'n', 
-'e', 'r', 'a', 't', 'e', 'd', 'C', 'o', 'd', 'e', 'I', 'n', 'f', 'o', '.', 'A', 'n', 'n', 'o', 't', 'a', 't', 'i', 'o', 'n', 
-'R', '\n', 'a', 'n', 'n', 'o', 't', 'a', 't', 'i', 'o', 'n', '\032', '\353', '\001', '\n', '\n', 'A', 'n', 'n', 'o', 't', 'a', 't', 'i', 
-'o', 'n', '\022', '\026', '\n', '\004', 'p', 'a', 't', 'h', '\030', '\001', ' ', '\003', '(', '\005', 'B', '\002', '\020', '\001', 'R', '\004', 'p', 'a', 't', 
-'h', '\022', '\037', '\n', '\013', 's', 'o', 'u', 'r', 'c', 'e', '_', 'f', 'i', 'l', 'e', '\030', '\002', ' ', '\001', '(', '\t', 'R', '\n', 's', 
-'o', 'u', 'r', 'c', 'e', 'F', 'i', 'l', 'e', '\022', '\024', '\n', '\005', 'b', 'e', 'g', 'i', 'n', '\030', '\003', ' ', '\001', '(', '\005', 'R', 
-'\005', 'b', 'e', 'g', 'i', 'n', '\022', '\020', '\n', '\003', 'e', 'n', 'd', '\030', '\004', ' ', '\001', '(', '\005', 'R', '\003', 'e', 'n', 'd', '\022', 
-'R', '\n', '\010', 's', 'e', 'm', 'a', 'n', 't', 'i', 'c', '\030', '\005', ' ', '\001', '(', '\016', '2', '6', '.', 'g', 'o', 'o', 'g', 'l', 
-'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'G', 'e', 'n', 'e', 'r', 'a', 't', 'e', 'd', 'C', 'o', 'd', 'e', 'I', 
-'n', 'f', 'o', '.', 'A', 'n', 'n', 'o', 't', 'a', 't', 'i', 'o', 'n', '.', 'S', 'e', 'm', 'a', 'n', 't', 'i', 'c', 'R', '\010', 
-'s', 'e', 'm', 'a', 'n', 't', 'i', 'c', '\"', '(', '\n', '\010', 'S', 'e', 'm', 'a', 'n', 't', 'i', 'c', '\022', '\010', '\n', '\004', 'N', 
-'O', 'N', 'E', '\020', '\000', '\022', '\007', '\n', '\003', 'S', 'E', 'T', '\020', '\001', '\022', '\t', '\n', '\005', 'A', 'L', 'I', 'A', 'S', '\020', '\002', 
-'*', '\222', '\002', '\n', '\007', 'E', 'd', 'i', 't', 'i', 'o', 'n', '\022', '\023', '\n', '\017', 'E', 'D', 'I', 'T', 'I', 'O', 'N', '_', 'U', 
-'N', 'K', 'N', 'O', 'W', 'N', '\020', '\000', '\022', '\023', '\n', '\016', 'E', 'D', 'I', 'T', 'I', 'O', 'N', '_', 'P', 'R', 'O', 'T', 'O', 
+'S', 'e', 't', 'R', '\023', 'o', 'v', 'e', 'r', 'r', 'i', 'd', 'a', 'b', 'l', 'e', 'F', 'e', 'a', 't', 'u', 'r', 'e', 's', '\022', 
+'B', '\n', '\016', 'f', 'i', 'x', 'e', 'd', '_', 'f', 'e', 'a', 't', 'u', 'r', 'e', 's', '\030', '\005', ' ', '\001', '(', '\013', '2', '\033', 
+'.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'F', 'e', 'a', 't', 'u', 'r', 'e', 'S', 
+'e', 't', 'R', '\r', 'f', 'i', 'x', 'e', 'd', 'F', 'e', 'a', 't', 'u', 'r', 'e', 's', '\"', '\247', '\002', '\n', '\016', 'S', 'o', 'u', 
+'r', 'c', 'e', 'C', 'o', 'd', 'e', 'I', 'n', 'f', 'o', '\022', 'D', '\n', '\010', 'l', 'o', 'c', 'a', 't', 'i', 'o', 'n', '\030', '\001', 
+' ', '\003', '(', '\013', '2', '(', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'S', 'o', 
+'u', 'r', 'c', 'e', 'C', 'o', 'd', 'e', 'I', 'n', 'f', 'o', '.', 'L', 'o', 'c', 'a', 't', 'i', 'o', 'n', 'R', '\010', 'l', 'o', 
+'c', 'a', 't', 'i', 'o', 'n', '\032', '\316', '\001', '\n', '\010', 'L', 'o', 'c', 'a', 't', 'i', 'o', 'n', '\022', '\026', '\n', '\004', 'p', 'a', 
+'t', 'h', '\030', '\001', ' ', '\003', '(', '\005', 'B', '\002', '\020', '\001', 'R', '\004', 'p', 'a', 't', 'h', '\022', '\026', '\n', '\004', 's', 'p', 'a', 
+'n', '\030', '\002', ' ', '\003', '(', '\005', 'B', '\002', '\020', '\001', 'R', '\004', 's', 'p', 'a', 'n', '\022', ')', '\n', '\020', 'l', 'e', 'a', 'd', 
+'i', 'n', 'g', '_', 'c', 'o', 'm', 'm', 'e', 'n', 't', 's', '\030', '\003', ' ', '\001', '(', '\t', 'R', '\017', 'l', 'e', 'a', 'd', 'i', 
+'n', 'g', 'C', 'o', 'm', 'm', 'e', 'n', 't', 's', '\022', '+', '\n', '\021', 't', 'r', 'a', 'i', 'l', 'i', 'n', 'g', '_', 'c', 'o', 
+'m', 'm', 'e', 'n', 't', 's', '\030', '\004', ' ', '\001', '(', '\t', 'R', '\020', 't', 'r', 'a', 'i', 'l', 'i', 'n', 'g', 'C', 'o', 'm', 
+'m', 'e', 'n', 't', 's', '\022', ':', '\n', '\031', 'l', 'e', 'a', 'd', 'i', 'n', 'g', '_', 'd', 'e', 't', 'a', 'c', 'h', 'e', 'd', 
+'_', 'c', 'o', 'm', 'm', 'e', 'n', 't', 's', '\030', '\006', ' ', '\003', '(', '\t', 'R', '\027', 'l', 'e', 'a', 'd', 'i', 'n', 'g', 'D', 
+'e', 't', 'a', 'c', 'h', 'e', 'd', 'C', 'o', 'm', 'm', 'e', 'n', 't', 's', '\"', '\320', '\002', '\n', '\021', 'G', 'e', 'n', 'e', 'r', 
+'a', 't', 'e', 'd', 'C', 'o', 'd', 'e', 'I', 'n', 'f', 'o', '\022', 'M', '\n', '\n', 'a', 'n', 'n', 'o', 't', 'a', 't', 'i', 'o', 
+'n', '\030', '\001', ' ', '\003', '(', '\013', '2', '-', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', 
+'.', 'G', 'e', 'n', 'e', 'r', 'a', 't', 'e', 'd', 'C', 'o', 'd', 'e', 'I', 'n', 'f', 'o', '.', 'A', 'n', 'n', 'o', 't', 'a', 
+'t', 'i', 'o', 'n', 'R', '\n', 'a', 'n', 'n', 'o', 't', 'a', 't', 'i', 'o', 'n', '\032', '\353', '\001', '\n', '\n', 'A', 'n', 'n', 'o', 
+'t', 'a', 't', 'i', 'o', 'n', '\022', '\026', '\n', '\004', 'p', 'a', 't', 'h', '\030', '\001', ' ', '\003', '(', '\005', 'B', '\002', '\020', '\001', 'R', 
+'\004', 'p', 'a', 't', 'h', '\022', '\037', '\n', '\013', 's', 'o', 'u', 'r', 'c', 'e', '_', 'f', 'i', 'l', 'e', '\030', '\002', ' ', '\001', '(', 
+'\t', 'R', '\n', 's', 'o', 'u', 'r', 'c', 'e', 'F', 'i', 'l', 'e', '\022', '\024', '\n', '\005', 'b', 'e', 'g', 'i', 'n', '\030', '\003', ' ', 
+'\001', '(', '\005', 'R', '\005', 'b', 'e', 'g', 'i', 'n', '\022', '\020', '\n', '\003', 'e', 'n', 'd', '\030', '\004', ' ', '\001', '(', '\005', 'R', '\003', 
+'e', 'n', 'd', '\022', 'R', '\n', '\010', 's', 'e', 'm', 'a', 'n', 't', 'i', 'c', '\030', '\005', ' ', '\001', '(', '\016', '2', '6', '.', 'g', 
+'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'G', 'e', 'n', 'e', 'r', 'a', 't', 'e', 'd', 'C', 
+'o', 'd', 'e', 'I', 'n', 'f', 'o', '.', 'A', 'n', 'n', 'o', 't', 'a', 't', 'i', 'o', 'n', '.', 'S', 'e', 'm', 'a', 'n', 't', 
+'i', 'c', 'R', '\010', 's', 'e', 'm', 'a', 'n', 't', 'i', 'c', '\"', '(', '\n', '\010', 'S', 'e', 'm', 'a', 'n', 't', 'i', 'c', '\022', 
+'\010', '\n', '\004', 'N', 'O', 'N', 'E', '\020', '\000', '\022', '\007', '\n', '\003', 'S', 'E', 'T', '\020', '\001', '\022', '\t', '\n', '\005', 'A', 'L', 'I', 
+'A', 'S', '\020', '\002', '*', '\247', '\002', '\n', '\007', 'E', 'd', 'i', 't', 'i', 'o', 'n', '\022', '\023', '\n', '\017', 'E', 'D', 'I', 'T', 'I', 
+'O', 'N', '_', 'U', 'N', 'K', 'N', 'O', 'W', 'N', '\020', '\000', '\022', '\023', '\n', '\016', 'E', 'D', 'I', 'T', 'I', 'O', 'N', '_', 'L', 
+'E', 'G', 'A', 'C', 'Y', '\020', '\204', '\007', '\022', '\023', '\n', '\016', 'E', 'D', 'I', 'T', 'I', 'O', 'N', '_', 'P', 'R', 'O', 'T', 'O', 
 '2', '\020', '\346', '\007', '\022', '\023', '\n', '\016', 'E', 'D', 'I', 'T', 'I', 'O', 'N', '_', 'P', 'R', 'O', 'T', 'O', '3', '\020', '\347', '\007', 
 '\022', '\021', '\n', '\014', 'E', 'D', 'I', 'T', 'I', 'O', 'N', '_', '2', '0', '2', '3', '\020', '\350', '\007', '\022', '\021', '\n', '\014', 'E', 'D', 
 'I', 'T', 'I', 'O', 'N', '_', '2', '0', '2', '4', '\020', '\351', '\007', '\022', '\027', '\n', '\023', 'E', 'D', 'I', 'T', 'I', 'O', 'N', '_', 
 '1', '_', 'T', 'E', 'S', 'T', '_', 'O', 'N', 'L', 'Y', '\020', '\001', '\022', '\027', '\n', '\023', 'E', 'D', 'I', 'T', 'I', 'O', 'N', '_', 
 '2', '_', 'T', 'E', 'S', 'T', '_', 'O', 'N', 'L', 'Y', '\020', '\002', '\022', '\035', '\n', '\027', 'E', 'D', 'I', 'T', 'I', 'O', 'N', '_', 
 '9', '9', '9', '9', '7', '_', 'T', 'E', 'S', 'T', '_', 'O', 'N', 'L', 'Y', '\020', '\235', '\215', '\006', '\022', '\035', '\n', '\027', 'E', 'D', 
 'I', 'T', 'I', 'O', 'N', '_', '9', '9', '9', '9', '8', '_', 'T', 'E', 'S', 'T', '_', 'O', 'N', 'L', 'Y', '\020', '\236', '\215', '\006', 
@@ -481,9 +502,9 @@
   NULL
 };
 
 _upb_DefPool_Init google_protobuf_descriptor_proto_upbdefinit = {
   deps,
   &google_protobuf_descriptor_proto_upb_file_layout,
   "google/protobuf/descriptor.proto",
-  UPB_STRINGVIEW_INIT(descriptor, 11630)
+  UPB_STRINGVIEW_INIT(descriptor, 12155)
 };
```

### Comparing `protobuf-5.26.1/google/protobuf/descriptor.upbdefs.h` & `protobuf-5.27.0rc1/google/protobuf/descriptor.upbdefs.h`

 * *Files 1% similar despite different names*

```diff
@@ -104,14 +104,19 @@
 }
 
 UPB_INLINE const upb_MessageDef *google_protobuf_FieldOptions_EditionDefault_getmsgdef(upb_DefPool *s) {
   _upb_DefPool_LoadDefInit(s, &google_protobuf_descriptor_proto_upbdefinit);
   return upb_DefPool_FindMessageByName(s, "google.protobuf.FieldOptions.EditionDefault");
 }
 
+UPB_INLINE const upb_MessageDef *google_protobuf_FieldOptions_FeatureSupport_getmsgdef(upb_DefPool *s) {
+  _upb_DefPool_LoadDefInit(s, &google_protobuf_descriptor_proto_upbdefinit);
+  return upb_DefPool_FindMessageByName(s, "google.protobuf.FieldOptions.FeatureSupport");
+}
+
 UPB_INLINE const upb_MessageDef *google_protobuf_OneofOptions_getmsgdef(upb_DefPool *s) {
   _upb_DefPool_LoadDefInit(s, &google_protobuf_descriptor_proto_upbdefinit);
   return upb_DefPool_FindMessageByName(s, "google.protobuf.OneofOptions");
 }
 
 UPB_INLINE const upb_MessageDef *google_protobuf_EnumOptions_getmsgdef(upb_DefPool *s) {
   _upb_DefPool_LoadDefInit(s, &google_protobuf_descriptor_proto_upbdefinit);
```

### Comparing `protobuf-5.26.1/google/protobuf/descriptor_database.py` & `protobuf-5.27.0rc1/google/protobuf/descriptor_database.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/google/protobuf/descriptor_pb2.py` & `protobuf-5.27.0rc1/google/protobuf/descriptor_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
+# NO CHECKED-IN PROTOBUF GENCODE
 # source: google/protobuf/descriptor.proto
-# Protobuf Python Version: 5.26.1
+# Protobuf Python Version: 5.27.0-rc1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import runtime_version as _runtime_version
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
+_runtime_version.ValidateProtobufRuntimeVersion(
+    _runtime_version.Domain.PUBLIC,
+    5,
+    27,
+    0,
+    '-rc1',
+    'google/protobuf/descriptor.proto'
+)
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
@@ -18,18 +28,18 @@
   DESCRIPTOR = _descriptor.FileDescriptor(
     name='google/protobuf/descriptor.proto',
     package='google.protobuf',
     syntax='proto2',
     edition='EDITION_PROTO2',
     serialized_options=b'\n\023com.google.protobufB\020DescriptorProtosH\001Z-google.golang.org/protobuf/types/descriptorpb\370\001\001\242\002\003GPB\252\002\032Google.Protobuf.Reflection',
     create_key=_descriptor._internal_create_key,
-    serialized_pb=b'\n google/protobuf/descriptor.proto\x12\x0fgoogle.protobuf\"M\n\x11\x46ileDescriptorSet\x12\x38\n\x04\x66ile\x18\x01 \x03(\x0b\x32$.google.protobuf.FileDescriptorProtoR\x04\x66ile\"\x98\x05\n\x13\x46ileDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x18\n\x07package\x18\x02 \x01(\tR\x07package\x12\x1e\n\ndependency\x18\x03 \x03(\tR\ndependency\x12+\n\x11public_dependency\x18\n \x03(\x05R\x10publicDependency\x12\'\n\x0fweak_dependency\x18\x0b \x03(\x05R\x0eweakDependency\x12\x43\n\x0cmessage_type\x18\x04 \x03(\x0b\x32 .google.protobuf.DescriptorProtoR\x0bmessageType\x12\x41\n\tenum_type\x18\x05 \x03(\x0b\x32$.google.protobuf.EnumDescriptorProtoR\x08\x65numType\x12\x41\n\x07service\x18\x06 \x03(\x0b\x32\'.google.protobuf.ServiceDescriptorProtoR\x07service\x12\x43\n\textension\x18\x07 \x03(\x0b\x32%.google.protobuf.FieldDescriptorProtoR\textension\x12\x36\n\x07options\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.FileOptionsR\x07options\x12I\n\x10source_code_info\x18\t \x01(\x0b\x32\x1f.google.protobuf.SourceCodeInfoR\x0esourceCodeInfo\x12\x16\n\x06syntax\x18\x0c \x01(\tR\x06syntax\x12\x32\n\x07\x65\x64ition\x18\x0e \x01(\x0e\x32\x18.google.protobuf.EditionR\x07\x65\x64ition\"\xb9\x06\n\x0f\x44\x65scriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12;\n\x05\x66ield\x18\x02 \x03(\x0b\x32%.google.protobuf.FieldDescriptorProtoR\x05\x66ield\x12\x43\n\textension\x18\x06 \x03(\x0b\x32%.google.protobuf.FieldDescriptorProtoR\textension\x12\x41\n\x0bnested_type\x18\x03 \x03(\x0b\x32 .google.protobuf.DescriptorProtoR\nnestedType\x12\x41\n\tenum_type\x18\x04 \x03(\x0b\x32$.google.protobuf.EnumDescriptorProtoR\x08\x65numType\x12X\n\x0f\x65xtension_range\x18\x05 \x03(\x0b\x32/.google.protobuf.DescriptorProto.ExtensionRangeR\x0e\x65xtensionRange\x12\x44\n\noneof_decl\x18\x08 \x03(\x0b\x32%.google.protobuf.OneofDescriptorProtoR\toneofDecl\x12\x39\n\x07options\x18\x07 \x01(\x0b\x32\x1f.google.protobuf.MessageOptionsR\x07options\x12U\n\x0ereserved_range\x18\t \x03(\x0b\x32..google.protobuf.DescriptorProto.ReservedRangeR\rreservedRange\x12#\n\rreserved_name\x18\n \x03(\tR\x0creservedName\x1az\n\x0e\x45xtensionRange\x12\x14\n\x05start\x18\x01 \x01(\x05R\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\x05R\x03\x65nd\x12@\n\x07options\x18\x03 \x01(\x0b\x32&.google.protobuf.ExtensionRangeOptionsR\x07options\x1a\x37\n\rReservedRange\x12\x14\n\x05start\x18\x01 \x01(\x05R\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\x05R\x03\x65nd\"\xcc\x04\n\x15\x45xtensionRangeOptions\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\x12Y\n\x0b\x64\x65\x63laration\x18\x02 \x03(\x0b\x32\x32.google.protobuf.ExtensionRangeOptions.DeclarationB\x03\x88\x01\x02R\x0b\x64\x65\x63laration\x12\x37\n\x08\x66\x65\x61tures\x18\x32 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12m\n\x0cverification\x18\x03 \x01(\x0e\x32\x38.google.protobuf.ExtensionRangeOptions.VerificationState:\nUNVERIFIEDB\x03\x88\x01\x02R\x0cverification\x1a\x94\x01\n\x0b\x44\x65\x63laration\x12\x16\n\x06number\x18\x01 \x01(\x05R\x06number\x12\x1b\n\tfull_name\x18\x02 \x01(\tR\x08\x66ullName\x12\x12\n\x04type\x18\x03 \x01(\tR\x04type\x12\x1a\n\x08reserved\x18\x05 \x01(\x08R\x08reserved\x12\x1a\n\x08repeated\x18\x06 \x01(\x08R\x08repeatedJ\x04\x08\x04\x10\x05\"4\n\x11VerificationState\x12\x0f\n\x0b\x44\x45\x43LARATION\x10\x00\x12\x0e\n\nUNVERIFIED\x10\x01*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\xc1\x06\n\x14\x46ieldDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x16\n\x06number\x18\x03 \x01(\x05R\x06number\x12\x41\n\x05label\x18\x04 \x01(\x0e\x32+.google.protobuf.FieldDescriptorProto.LabelR\x05label\x12>\n\x04type\x18\x05 \x01(\x0e\x32*.google.protobuf.FieldDescriptorProto.TypeR\x04type\x12\x1b\n\ttype_name\x18\x06 \x01(\tR\x08typeName\x12\x1a\n\x08\x65xtendee\x18\x02 \x01(\tR\x08\x65xtendee\x12#\n\rdefault_value\x18\x07 \x01(\tR\x0c\x64\x65\x66\x61ultValue\x12\x1f\n\x0boneof_index\x18\t \x01(\x05R\noneofIndex\x12\x1b\n\tjson_name\x18\n \x01(\tR\x08jsonName\x12\x37\n\x07options\x18\x08 \x01(\x0b\x32\x1d.google.protobuf.FieldOptionsR\x07options\x12\'\n\x0fproto3_optional\x18\x11 \x01(\x08R\x0eproto3Optional\"\xb6\x02\n\x04Type\x12\x0f\n\x0bTYPE_DOUBLE\x10\x01\x12\x0e\n\nTYPE_FLOAT\x10\x02\x12\x0e\n\nTYPE_INT64\x10\x03\x12\x0f\n\x0bTYPE_UINT64\x10\x04\x12\x0e\n\nTYPE_INT32\x10\x05\x12\x10\n\x0cTYPE_FIXED64\x10\x06\x12\x10\n\x0cTYPE_FIXED32\x10\x07\x12\r\n\tTYPE_BOOL\x10\x08\x12\x0f\n\x0bTYPE_STRING\x10\t\x12\x0e\n\nTYPE_GROUP\x10\n\x12\x10\n\x0cTYPE_MESSAGE\x10\x0b\x12\x0e\n\nTYPE_BYTES\x10\x0c\x12\x0f\n\x0bTYPE_UINT32\x10\r\x12\r\n\tTYPE_ENUM\x10\x0e\x12\x11\n\rTYPE_SFIXED32\x10\x0f\x12\x11\n\rTYPE_SFIXED64\x10\x10\x12\x0f\n\x0bTYPE_SINT32\x10\x11\x12\x0f\n\x0bTYPE_SINT64\x10\x12\"C\n\x05Label\x12\x12\n\x0eLABEL_OPTIONAL\x10\x01\x12\x12\n\x0eLABEL_REPEATED\x10\x03\x12\x12\n\x0eLABEL_REQUIRED\x10\x02\"c\n\x14OneofDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x37\n\x07options\x18\x02 \x01(\x0b\x32\x1d.google.protobuf.OneofOptionsR\x07options\"\xe3\x02\n\x13\x45numDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12?\n\x05value\x18\x02 \x03(\x0b\x32).google.protobuf.EnumValueDescriptorProtoR\x05value\x12\x36\n\x07options\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.EnumOptionsR\x07options\x12]\n\x0ereserved_range\x18\x04 \x03(\x0b\x32\x36.google.protobuf.EnumDescriptorProto.EnumReservedRangeR\rreservedRange\x12#\n\rreserved_name\x18\x05 \x03(\tR\x0creservedName\x1a;\n\x11\x45numReservedRange\x12\x14\n\x05start\x18\x01 \x01(\x05R\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\x05R\x03\x65nd\"\x83\x01\n\x18\x45numValueDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x16\n\x06number\x18\x02 \x01(\x05R\x06number\x12;\n\x07options\x18\x03 \x01(\x0b\x32!.google.protobuf.EnumValueOptionsR\x07options\"\xa7\x01\n\x16ServiceDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12>\n\x06method\x18\x02 \x03(\x0b\x32&.google.protobuf.MethodDescriptorProtoR\x06method\x12\x39\n\x07options\x18\x03 \x01(\x0b\x32\x1f.google.protobuf.ServiceOptionsR\x07options\"\x89\x02\n\x15MethodDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x1d\n\ninput_type\x18\x02 \x01(\tR\tinputType\x12\x1f\n\x0boutput_type\x18\x03 \x01(\tR\noutputType\x12\x38\n\x07options\x18\x04 \x01(\x0b\x32\x1e.google.protobuf.MethodOptionsR\x07options\x12\x30\n\x10\x63lient_streaming\x18\x05 \x01(\x08:\x05\x66\x61lseR\x0f\x63lientStreaming\x12\x30\n\x10server_streaming\x18\x06 \x01(\x08:\x05\x66\x61lseR\x0fserverStreaming\"\x97\t\n\x0b\x46ileOptions\x12!\n\x0cjava_package\x18\x01 \x01(\tR\x0bjavaPackage\x12\x30\n\x14java_outer_classname\x18\x08 \x01(\tR\x12javaOuterClassname\x12\x35\n\x13java_multiple_files\x18\n \x01(\x08:\x05\x66\x61lseR\x11javaMultipleFiles\x12\x44\n\x1djava_generate_equals_and_hash\x18\x14 \x01(\x08\x42\x02\x18\x01R\x19javaGenerateEqualsAndHash\x12:\n\x16java_string_check_utf8\x18\x1b \x01(\x08:\x05\x66\x61lseR\x13javaStringCheckUtf8\x12S\n\x0coptimize_for\x18\t \x01(\x0e\x32).google.protobuf.FileOptions.OptimizeMode:\x05SPEEDR\x0boptimizeFor\x12\x1d\n\ngo_package\x18\x0b \x01(\tR\tgoPackage\x12\x35\n\x13\x63\x63_generic_services\x18\x10 \x01(\x08:\x05\x66\x61lseR\x11\x63\x63GenericServices\x12\x39\n\x15java_generic_services\x18\x11 \x01(\x08:\x05\x66\x61lseR\x13javaGenericServices\x12\x35\n\x13py_generic_services\x18\x12 \x01(\x08:\x05\x66\x61lseR\x11pyGenericServices\x12%\n\ndeprecated\x18\x17 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12.\n\x10\x63\x63_enable_arenas\x18\x1f \x01(\x08:\x04trueR\x0e\x63\x63\x45nableArenas\x12*\n\x11objc_class_prefix\x18$ \x01(\tR\x0fobjcClassPrefix\x12)\n\x10\x63sharp_namespace\x18% \x01(\tR\x0f\x63sharpNamespace\x12!\n\x0cswift_prefix\x18\' \x01(\tR\x0bswiftPrefix\x12(\n\x10php_class_prefix\x18( \x01(\tR\x0ephpClassPrefix\x12#\n\rphp_namespace\x18) \x01(\tR\x0cphpNamespace\x12\x34\n\x16php_metadata_namespace\x18, \x01(\tR\x14phpMetadataNamespace\x12!\n\x0cruby_package\x18- \x01(\tR\x0brubyPackage\x12\x37\n\x08\x66\x65\x61tures\x18\x32 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\":\n\x0cOptimizeMode\x12\t\n\x05SPEED\x10\x01\x12\r\n\tCODE_SIZE\x10\x02\x12\x10\n\x0cLITE_RUNTIME\x10\x03*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08*\x10+J\x04\x08&\x10\'\"\xf4\x03\n\x0eMessageOptions\x12<\n\x17message_set_wire_format\x18\x01 \x01(\x08:\x05\x66\x61lseR\x14messageSetWireFormat\x12L\n\x1fno_standard_descriptor_accessor\x18\x02 \x01(\x08:\x05\x66\x61lseR\x1cnoStandardDescriptorAccessor\x12%\n\ndeprecated\x18\x03 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12\x1b\n\tmap_entry\x18\x07 \x01(\x08R\x08mapEntry\x12V\n&deprecated_legacy_json_field_conflicts\x18\x0b \x01(\x08\x42\x02\x18\x01R\"deprecatedLegacyJsonFieldConflicts\x12\x37\n\x08\x66\x65\x61tures\x18\x0c \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07J\x04\x08\x08\x10\tJ\x04\x08\t\x10\n\"\xad\n\n\x0c\x46ieldOptions\x12\x41\n\x05\x63type\x18\x01 \x01(\x0e\x32#.google.protobuf.FieldOptions.CType:\x06STRINGR\x05\x63type\x12\x16\n\x06packed\x18\x02 \x01(\x08R\x06packed\x12G\n\x06jstype\x18\x06 \x01(\x0e\x32$.google.protobuf.FieldOptions.JSType:\tJS_NORMALR\x06jstype\x12\x19\n\x04lazy\x18\x05 \x01(\x08:\x05\x66\x61lseR\x04lazy\x12.\n\x0funverified_lazy\x18\x0f \x01(\x08:\x05\x66\x61lseR\x0eunverifiedLazy\x12%\n\ndeprecated\x18\x03 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12\x19\n\x04weak\x18\n \x01(\x08:\x05\x66\x61lseR\x04weak\x12(\n\x0c\x64\x65\x62ug_redact\x18\x10 \x01(\x08:\x05\x66\x61lseR\x0b\x64\x65\x62ugRedact\x12K\n\tretention\x18\x11 \x01(\x0e\x32-.google.protobuf.FieldOptions.OptionRetentionR\tretention\x12H\n\x07targets\x18\x13 \x03(\x0e\x32..google.protobuf.FieldOptions.OptionTargetTypeR\x07targets\x12W\n\x10\x65\x64ition_defaults\x18\x14 \x03(\x0b\x32,.google.protobuf.FieldOptions.EditionDefaultR\x0f\x65\x64itionDefaults\x12\x37\n\x08\x66\x65\x61tures\x18\x15 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\x1aZ\n\x0e\x45\x64itionDefault\x12\x32\n\x07\x65\x64ition\x18\x03 \x01(\x0e\x32\x18.google.protobuf.EditionR\x07\x65\x64ition\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value\"/\n\x05\x43Type\x12\n\n\x06STRING\x10\x00\x12\x08\n\x04\x43ORD\x10\x01\x12\x10\n\x0cSTRING_PIECE\x10\x02\"5\n\x06JSType\x12\r\n\tJS_NORMAL\x10\x00\x12\r\n\tJS_STRING\x10\x01\x12\r\n\tJS_NUMBER\x10\x02\"U\n\x0fOptionRetention\x12\x15\n\x11RETENTION_UNKNOWN\x10\x00\x12\x15\n\x11RETENTION_RUNTIME\x10\x01\x12\x14\n\x10RETENTION_SOURCE\x10\x02\"\x8c\x02\n\x10OptionTargetType\x12\x17\n\x13TARGET_TYPE_UNKNOWN\x10\x00\x12\x14\n\x10TARGET_TYPE_FILE\x10\x01\x12\x1f\n\x1bTARGET_TYPE_EXTENSION_RANGE\x10\x02\x12\x17\n\x13TARGET_TYPE_MESSAGE\x10\x03\x12\x15\n\x11TARGET_TYPE_FIELD\x10\x04\x12\x15\n\x11TARGET_TYPE_ONEOF\x10\x05\x12\x14\n\x10TARGET_TYPE_ENUM\x10\x06\x12\x1a\n\x16TARGET_TYPE_ENUM_ENTRY\x10\x07\x12\x17\n\x13TARGET_TYPE_SERVICE\x10\x08\x12\x16\n\x12TARGET_TYPE_METHOD\x10\t*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08\x04\x10\x05J\x04\x08\x12\x10\x13\"\xac\x01\n\x0cOneofOptions\x12\x37\n\x08\x66\x65\x61tures\x18\x01 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\xd1\x02\n\x0b\x45numOptions\x12\x1f\n\x0b\x61llow_alias\x18\x02 \x01(\x08R\nallowAlias\x12%\n\ndeprecated\x18\x03 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12V\n&deprecated_legacy_json_field_conflicts\x18\x06 \x01(\x08\x42\x02\x18\x01R\"deprecatedLegacyJsonFieldConflicts\x12\x37\n\x08\x66\x65\x61tures\x18\x07 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08\x05\x10\x06\"\x81\x02\n\x10\x45numValueOptions\x12%\n\ndeprecated\x18\x01 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12\x37\n\x08\x66\x65\x61tures\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12(\n\x0c\x64\x65\x62ug_redact\x18\x03 \x01(\x08:\x05\x66\x61lseR\x0b\x64\x65\x62ugRedact\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\xd5\x01\n\x0eServiceOptions\x12\x37\n\x08\x66\x65\x61tures\x18\" \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12%\n\ndeprecated\x18! \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\x99\x03\n\rMethodOptions\x12%\n\ndeprecated\x18! \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12q\n\x11idempotency_level\x18\" \x01(\x0e\x32/.google.protobuf.MethodOptions.IdempotencyLevel:\x13IDEMPOTENCY_UNKNOWNR\x10idempotencyLevel\x12\x37\n\x08\x66\x65\x61tures\x18# \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\"P\n\x10IdempotencyLevel\x12\x17\n\x13IDEMPOTENCY_UNKNOWN\x10\x00\x12\x13\n\x0fNO_SIDE_EFFECTS\x10\x01\x12\x0e\n\nIDEMPOTENT\x10\x02*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\x9a\x03\n\x13UninterpretedOption\x12\x41\n\x04name\x18\x02 \x03(\x0b\x32-.google.protobuf.UninterpretedOption.NamePartR\x04name\x12)\n\x10identifier_value\x18\x03 \x01(\tR\x0fidentifierValue\x12,\n\x12positive_int_value\x18\x04 \x01(\x04R\x10positiveIntValue\x12,\n\x12negative_int_value\x18\x05 \x01(\x03R\x10negativeIntValue\x12!\n\x0c\x64ouble_value\x18\x06 \x01(\x01R\x0b\x64oubleValue\x12!\n\x0cstring_value\x18\x07 \x01(\x0cR\x0bstringValue\x12\'\n\x0f\x61ggregate_value\x18\x08 \x01(\tR\x0e\x61ggregateValue\x1aJ\n\x08NamePart\x12\x1b\n\tname_part\x18\x01 \x02(\tR\x08namePart\x12!\n\x0cis_extension\x18\x02 \x02(\x08R\x0bisExtension\"\x8c\n\n\nFeatureSet\x12\x8b\x01\n\x0e\x66ield_presence\x18\x01 \x01(\x0e\x32).google.protobuf.FeatureSet.FieldPresenceB9\x88\x01\x01\x98\x01\x04\x98\x01\x01\xa2\x01\r\x12\x08\x45XPLICIT\x18\xe6\x07\xa2\x01\r\x12\x08IMPLICIT\x18\xe7\x07\xa2\x01\r\x12\x08\x45XPLICIT\x18\xe8\x07R\rfieldPresence\x12\x66\n\tenum_type\x18\x02 \x01(\x0e\x32$.google.protobuf.FeatureSet.EnumTypeB#\x88\x01\x01\x98\x01\x06\x98\x01\x01\xa2\x01\x0b\x12\x06\x43LOSED\x18\xe6\x07\xa2\x01\t\x12\x04OPEN\x18\xe7\x07R\x08\x65numType\x12\x92\x01\n\x17repeated_field_encoding\x18\x03 \x01(\x0e\x32\x31.google.protobuf.FeatureSet.RepeatedFieldEncodingB\'\x88\x01\x01\x98\x01\x04\x98\x01\x01\xa2\x01\r\x12\x08\x45XPANDED\x18\xe6\x07\xa2\x01\x0b\x12\x06PACKED\x18\xe7\x07R\x15repeatedFieldEncoding\x12x\n\x0futf8_validation\x18\x04 \x01(\x0e\x32*.google.protobuf.FeatureSet.Utf8ValidationB#\x88\x01\x01\x98\x01\x04\x98\x01\x01\xa2\x01\t\x12\x04NONE\x18\xe6\x07\xa2\x01\x0b\x12\x06VERIFY\x18\xe7\x07R\x0eutf8Validation\x12x\n\x10message_encoding\x18\x05 \x01(\x0e\x32+.google.protobuf.FeatureSet.MessageEncodingB \x88\x01\x01\x98\x01\x04\x98\x01\x01\xa2\x01\x14\x12\x0fLENGTH_PREFIXED\x18\xe6\x07R\x0fmessageEncoding\x12|\n\x0bjson_format\x18\x06 \x01(\x0e\x32&.google.protobuf.FeatureSet.JsonFormatB3\x88\x01\x01\x98\x01\x03\x98\x01\x06\x98\x01\x01\xa2\x01\x17\x12\x12LEGACY_BEST_EFFORT\x18\xe6\x07\xa2\x01\n\x12\x05\x41LLOW\x18\xe7\x07R\njsonFormat\"\\\n\rFieldPresence\x12\x1a\n\x16\x46IELD_PRESENCE_UNKNOWN\x10\x00\x12\x0c\n\x08\x45XPLICIT\x10\x01\x12\x0c\n\x08IMPLICIT\x10\x02\x12\x13\n\x0fLEGACY_REQUIRED\x10\x03\"7\n\x08\x45numType\x12\x15\n\x11\x45NUM_TYPE_UNKNOWN\x10\x00\x12\x08\n\x04OPEN\x10\x01\x12\n\n\x06\x43LOSED\x10\x02\"V\n\x15RepeatedFieldEncoding\x12#\n\x1fREPEATED_FIELD_ENCODING_UNKNOWN\x10\x00\x12\n\n\x06PACKED\x10\x01\x12\x0c\n\x08\x45XPANDED\x10\x02\"C\n\x0eUtf8Validation\x12\x1b\n\x17UTF8_VALIDATION_UNKNOWN\x10\x00\x12\n\n\x06VERIFY\x10\x02\x12\x08\n\x04NONE\x10\x03\"S\n\x0fMessageEncoding\x12\x1c\n\x18MESSAGE_ENCODING_UNKNOWN\x10\x00\x12\x13\n\x0fLENGTH_PREFIXED\x10\x01\x12\r\n\tDELIMITED\x10\x02\"H\n\nJsonFormat\x12\x17\n\x13JSON_FORMAT_UNKNOWN\x10\x00\x12\t\n\x05\x41LLOW\x10\x01\x12\x16\n\x12LEGACY_BEST_EFFORT\x10\x02*\x06\x08\xe8\x07\x10\xe9\x07*\x06\x08\xe9\x07\x10\xea\x07*\x06\x08\xea\x07\x10\xeb\x07*\x06\x08\x8bN\x10\x90N*\x06\x08\x90N\x10\x91NJ\x06\x08\xe7\x07\x10\xe8\x07\"\xfe\x02\n\x12\x46\x65\x61tureSetDefaults\x12X\n\x08\x64\x65\x66\x61ults\x18\x01 \x03(\x0b\x32<.google.protobuf.FeatureSetDefaults.FeatureSetEditionDefaultR\x08\x64\x65\x66\x61ults\x12\x41\n\x0fminimum_edition\x18\x04 \x01(\x0e\x32\x18.google.protobuf.EditionR\x0eminimumEdition\x12\x41\n\x0fmaximum_edition\x18\x05 \x01(\x0e\x32\x18.google.protobuf.EditionR\x0emaximumEdition\x1a\x87\x01\n\x18\x46\x65\x61tureSetEditionDefault\x12\x32\n\x07\x65\x64ition\x18\x03 \x01(\x0e\x32\x18.google.protobuf.EditionR\x07\x65\x64ition\x12\x37\n\x08\x66\x65\x61tures\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\"\xa7\x02\n\x0eSourceCodeInfo\x12\x44\n\x08location\x18\x01 \x03(\x0b\x32(.google.protobuf.SourceCodeInfo.LocationR\x08location\x1a\xce\x01\n\x08Location\x12\x16\n\x04path\x18\x01 \x03(\x05\x42\x02\x10\x01R\x04path\x12\x16\n\x04span\x18\x02 \x03(\x05\x42\x02\x10\x01R\x04span\x12)\n\x10leading_comments\x18\x03 \x01(\tR\x0fleadingComments\x12+\n\x11trailing_comments\x18\x04 \x01(\tR\x10trailingComments\x12:\n\x19leading_detached_comments\x18\x06 \x03(\tR\x17leadingDetachedComments\"\xd0\x02\n\x11GeneratedCodeInfo\x12M\n\nannotation\x18\x01 \x03(\x0b\x32-.google.protobuf.GeneratedCodeInfo.AnnotationR\nannotation\x1a\xeb\x01\n\nAnnotation\x12\x16\n\x04path\x18\x01 \x03(\x05\x42\x02\x10\x01R\x04path\x12\x1f\n\x0bsource_file\x18\x02 \x01(\tR\nsourceFile\x12\x14\n\x05\x62\x65gin\x18\x03 \x01(\x05R\x05\x62\x65gin\x12\x10\n\x03\x65nd\x18\x04 \x01(\x05R\x03\x65nd\x12R\n\x08semantic\x18\x05 \x01(\x0e\x32\x36.google.protobuf.GeneratedCodeInfo.Annotation.SemanticR\x08semantic\"(\n\x08Semantic\x12\x08\n\x04NONE\x10\x00\x12\x07\n\x03SET\x10\x01\x12\t\n\x05\x41LIAS\x10\x02*\x92\x02\n\x07\x45\x64ition\x12\x13\n\x0f\x45\x44ITION_UNKNOWN\x10\x00\x12\x13\n\x0e\x45\x44ITION_PROTO2\x10\xe6\x07\x12\x13\n\x0e\x45\x44ITION_PROTO3\x10\xe7\x07\x12\x11\n\x0c\x45\x44ITION_2023\x10\xe8\x07\x12\x11\n\x0c\x45\x44ITION_2024\x10\xe9\x07\x12\x17\n\x13\x45\x44ITION_1_TEST_ONLY\x10\x01\x12\x17\n\x13\x45\x44ITION_2_TEST_ONLY\x10\x02\x12\x1d\n\x17\x45\x44ITION_99997_TEST_ONLY\x10\x9d\x8d\x06\x12\x1d\n\x17\x45\x44ITION_99998_TEST_ONLY\x10\x9e\x8d\x06\x12\x1d\n\x17\x45\x44ITION_99999_TEST_ONLY\x10\x9f\x8d\x06\x12\x13\n\x0b\x45\x44ITION_MAX\x10\xff\xff\xff\xff\x07\x42~\n\x13\x63om.google.protobufB\x10\x44\x65scriptorProtosH\x01Z-google.golang.org/protobuf/types/descriptorpb\xf8\x01\x01\xa2\x02\x03GPB\xaa\x02\x1aGoogle.Protobuf.Reflection'
+    serialized_pb=b'\n google/protobuf/descriptor.proto\x12\x0fgoogle.protobuf\"M\n\x11\x46ileDescriptorSet\x12\x38\n\x04\x66ile\x18\x01 \x03(\x0b\x32$.google.protobuf.FileDescriptorProtoR\x04\x66ile\"\x98\x05\n\x13\x46ileDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x18\n\x07package\x18\x02 \x01(\tR\x07package\x12\x1e\n\ndependency\x18\x03 \x03(\tR\ndependency\x12+\n\x11public_dependency\x18\n \x03(\x05R\x10publicDependency\x12\'\n\x0fweak_dependency\x18\x0b \x03(\x05R\x0eweakDependency\x12\x43\n\x0cmessage_type\x18\x04 \x03(\x0b\x32 .google.protobuf.DescriptorProtoR\x0bmessageType\x12\x41\n\tenum_type\x18\x05 \x03(\x0b\x32$.google.protobuf.EnumDescriptorProtoR\x08\x65numType\x12\x41\n\x07service\x18\x06 \x03(\x0b\x32\'.google.protobuf.ServiceDescriptorProtoR\x07service\x12\x43\n\textension\x18\x07 \x03(\x0b\x32%.google.protobuf.FieldDescriptorProtoR\textension\x12\x36\n\x07options\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.FileOptionsR\x07options\x12I\n\x10source_code_info\x18\t \x01(\x0b\x32\x1f.google.protobuf.SourceCodeInfoR\x0esourceCodeInfo\x12\x16\n\x06syntax\x18\x0c \x01(\tR\x06syntax\x12\x32\n\x07\x65\x64ition\x18\x0e \x01(\x0e\x32\x18.google.protobuf.EditionR\x07\x65\x64ition\"\xb9\x06\n\x0f\x44\x65scriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12;\n\x05\x66ield\x18\x02 \x03(\x0b\x32%.google.protobuf.FieldDescriptorProtoR\x05\x66ield\x12\x43\n\textension\x18\x06 \x03(\x0b\x32%.google.protobuf.FieldDescriptorProtoR\textension\x12\x41\n\x0bnested_type\x18\x03 \x03(\x0b\x32 .google.protobuf.DescriptorProtoR\nnestedType\x12\x41\n\tenum_type\x18\x04 \x03(\x0b\x32$.google.protobuf.EnumDescriptorProtoR\x08\x65numType\x12X\n\x0f\x65xtension_range\x18\x05 \x03(\x0b\x32/.google.protobuf.DescriptorProto.ExtensionRangeR\x0e\x65xtensionRange\x12\x44\n\noneof_decl\x18\x08 \x03(\x0b\x32%.google.protobuf.OneofDescriptorProtoR\toneofDecl\x12\x39\n\x07options\x18\x07 \x01(\x0b\x32\x1f.google.protobuf.MessageOptionsR\x07options\x12U\n\x0ereserved_range\x18\t \x03(\x0b\x32..google.protobuf.DescriptorProto.ReservedRangeR\rreservedRange\x12#\n\rreserved_name\x18\n \x03(\tR\x0creservedName\x1az\n\x0e\x45xtensionRange\x12\x14\n\x05start\x18\x01 \x01(\x05R\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\x05R\x03\x65nd\x12@\n\x07options\x18\x03 \x01(\x0b\x32&.google.protobuf.ExtensionRangeOptionsR\x07options\x1a\x37\n\rReservedRange\x12\x14\n\x05start\x18\x01 \x01(\x05R\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\x05R\x03\x65nd\"\xcc\x04\n\x15\x45xtensionRangeOptions\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\x12Y\n\x0b\x64\x65\x63laration\x18\x02 \x03(\x0b\x32\x32.google.protobuf.ExtensionRangeOptions.DeclarationB\x03\x88\x01\x02R\x0b\x64\x65\x63laration\x12\x37\n\x08\x66\x65\x61tures\x18\x32 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12m\n\x0cverification\x18\x03 \x01(\x0e\x32\x38.google.protobuf.ExtensionRangeOptions.VerificationState:\nUNVERIFIEDB\x03\x88\x01\x02R\x0cverification\x1a\x94\x01\n\x0b\x44\x65\x63laration\x12\x16\n\x06number\x18\x01 \x01(\x05R\x06number\x12\x1b\n\tfull_name\x18\x02 \x01(\tR\x08\x66ullName\x12\x12\n\x04type\x18\x03 \x01(\tR\x04type\x12\x1a\n\x08reserved\x18\x05 \x01(\x08R\x08reserved\x12\x1a\n\x08repeated\x18\x06 \x01(\x08R\x08repeatedJ\x04\x08\x04\x10\x05\"4\n\x11VerificationState\x12\x0f\n\x0b\x44\x45\x43LARATION\x10\x00\x12\x0e\n\nUNVERIFIED\x10\x01*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\xc1\x06\n\x14\x46ieldDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x16\n\x06number\x18\x03 \x01(\x05R\x06number\x12\x41\n\x05label\x18\x04 \x01(\x0e\x32+.google.protobuf.FieldDescriptorProto.LabelR\x05label\x12>\n\x04type\x18\x05 \x01(\x0e\x32*.google.protobuf.FieldDescriptorProto.TypeR\x04type\x12\x1b\n\ttype_name\x18\x06 \x01(\tR\x08typeName\x12\x1a\n\x08\x65xtendee\x18\x02 \x01(\tR\x08\x65xtendee\x12#\n\rdefault_value\x18\x07 \x01(\tR\x0c\x64\x65\x66\x61ultValue\x12\x1f\n\x0boneof_index\x18\t \x01(\x05R\noneofIndex\x12\x1b\n\tjson_name\x18\n \x01(\tR\x08jsonName\x12\x37\n\x07options\x18\x08 \x01(\x0b\x32\x1d.google.protobuf.FieldOptionsR\x07options\x12\'\n\x0fproto3_optional\x18\x11 \x01(\x08R\x0eproto3Optional\"\xb6\x02\n\x04Type\x12\x0f\n\x0bTYPE_DOUBLE\x10\x01\x12\x0e\n\nTYPE_FLOAT\x10\x02\x12\x0e\n\nTYPE_INT64\x10\x03\x12\x0f\n\x0bTYPE_UINT64\x10\x04\x12\x0e\n\nTYPE_INT32\x10\x05\x12\x10\n\x0cTYPE_FIXED64\x10\x06\x12\x10\n\x0cTYPE_FIXED32\x10\x07\x12\r\n\tTYPE_BOOL\x10\x08\x12\x0f\n\x0bTYPE_STRING\x10\t\x12\x0e\n\nTYPE_GROUP\x10\n\x12\x10\n\x0cTYPE_MESSAGE\x10\x0b\x12\x0e\n\nTYPE_BYTES\x10\x0c\x12\x0f\n\x0bTYPE_UINT32\x10\r\x12\r\n\tTYPE_ENUM\x10\x0e\x12\x11\n\rTYPE_SFIXED32\x10\x0f\x12\x11\n\rTYPE_SFIXED64\x10\x10\x12\x0f\n\x0bTYPE_SINT32\x10\x11\x12\x0f\n\x0bTYPE_SINT64\x10\x12\"C\n\x05Label\x12\x12\n\x0eLABEL_OPTIONAL\x10\x01\x12\x12\n\x0eLABEL_REPEATED\x10\x03\x12\x12\n\x0eLABEL_REQUIRED\x10\x02\"c\n\x14OneofDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x37\n\x07options\x18\x02 \x01(\x0b\x32\x1d.google.protobuf.OneofOptionsR\x07options\"\xe3\x02\n\x13\x45numDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12?\n\x05value\x18\x02 \x03(\x0b\x32).google.protobuf.EnumValueDescriptorProtoR\x05value\x12\x36\n\x07options\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.EnumOptionsR\x07options\x12]\n\x0ereserved_range\x18\x04 \x03(\x0b\x32\x36.google.protobuf.EnumDescriptorProto.EnumReservedRangeR\rreservedRange\x12#\n\rreserved_name\x18\x05 \x03(\tR\x0creservedName\x1a;\n\x11\x45numReservedRange\x12\x14\n\x05start\x18\x01 \x01(\x05R\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\x05R\x03\x65nd\"\x83\x01\n\x18\x45numValueDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x16\n\x06number\x18\x02 \x01(\x05R\x06number\x12;\n\x07options\x18\x03 \x01(\x0b\x32!.google.protobuf.EnumValueOptionsR\x07options\"\xa7\x01\n\x16ServiceDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12>\n\x06method\x18\x02 \x03(\x0b\x32&.google.protobuf.MethodDescriptorProtoR\x06method\x12\x39\n\x07options\x18\x03 \x01(\x0b\x32\x1f.google.protobuf.ServiceOptionsR\x07options\"\x89\x02\n\x15MethodDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x1d\n\ninput_type\x18\x02 \x01(\tR\tinputType\x12\x1f\n\x0boutput_type\x18\x03 \x01(\tR\noutputType\x12\x38\n\x07options\x18\x04 \x01(\x0b\x32\x1e.google.protobuf.MethodOptionsR\x07options\x12\x30\n\x10\x63lient_streaming\x18\x05 \x01(\x08:\x05\x66\x61lseR\x0f\x63lientStreaming\x12\x30\n\x10server_streaming\x18\x06 \x01(\x08:\x05\x66\x61lseR\x0fserverStreaming\"\x97\t\n\x0b\x46ileOptions\x12!\n\x0cjava_package\x18\x01 \x01(\tR\x0bjavaPackage\x12\x30\n\x14java_outer_classname\x18\x08 \x01(\tR\x12javaOuterClassname\x12\x35\n\x13java_multiple_files\x18\n \x01(\x08:\x05\x66\x61lseR\x11javaMultipleFiles\x12\x44\n\x1djava_generate_equals_and_hash\x18\x14 \x01(\x08\x42\x02\x18\x01R\x19javaGenerateEqualsAndHash\x12:\n\x16java_string_check_utf8\x18\x1b \x01(\x08:\x05\x66\x61lseR\x13javaStringCheckUtf8\x12S\n\x0coptimize_for\x18\t \x01(\x0e\x32).google.protobuf.FileOptions.OptimizeMode:\x05SPEEDR\x0boptimizeFor\x12\x1d\n\ngo_package\x18\x0b \x01(\tR\tgoPackage\x12\x35\n\x13\x63\x63_generic_services\x18\x10 \x01(\x08:\x05\x66\x61lseR\x11\x63\x63GenericServices\x12\x39\n\x15java_generic_services\x18\x11 \x01(\x08:\x05\x66\x61lseR\x13javaGenericServices\x12\x35\n\x13py_generic_services\x18\x12 \x01(\x08:\x05\x66\x61lseR\x11pyGenericServices\x12%\n\ndeprecated\x18\x17 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12.\n\x10\x63\x63_enable_arenas\x18\x1f \x01(\x08:\x04trueR\x0e\x63\x63\x45nableArenas\x12*\n\x11objc_class_prefix\x18$ \x01(\tR\x0fobjcClassPrefix\x12)\n\x10\x63sharp_namespace\x18% \x01(\tR\x0f\x63sharpNamespace\x12!\n\x0cswift_prefix\x18\' \x01(\tR\x0bswiftPrefix\x12(\n\x10php_class_prefix\x18( \x01(\tR\x0ephpClassPrefix\x12#\n\rphp_namespace\x18) \x01(\tR\x0cphpNamespace\x12\x34\n\x16php_metadata_namespace\x18, \x01(\tR\x14phpMetadataNamespace\x12!\n\x0cruby_package\x18- \x01(\tR\x0brubyPackage\x12\x37\n\x08\x66\x65\x61tures\x18\x32 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\":\n\x0cOptimizeMode\x12\t\n\x05SPEED\x10\x01\x12\r\n\tCODE_SIZE\x10\x02\x12\x10\n\x0cLITE_RUNTIME\x10\x03*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08*\x10+J\x04\x08&\x10\'\"\xf4\x03\n\x0eMessageOptions\x12<\n\x17message_set_wire_format\x18\x01 \x01(\x08:\x05\x66\x61lseR\x14messageSetWireFormat\x12L\n\x1fno_standard_descriptor_accessor\x18\x02 \x01(\x08:\x05\x66\x61lseR\x1cnoStandardDescriptorAccessor\x12%\n\ndeprecated\x18\x03 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12\x1b\n\tmap_entry\x18\x07 \x01(\x08R\x08mapEntry\x12V\n&deprecated_legacy_json_field_conflicts\x18\x0b \x01(\x08\x42\x02\x18\x01R\"deprecatedLegacyJsonFieldConflicts\x12\x37\n\x08\x66\x65\x61tures\x18\x0c \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07J\x04\x08\x08\x10\tJ\x04\x08\t\x10\n\"\x9d\r\n\x0c\x46ieldOptions\x12\x41\n\x05\x63type\x18\x01 \x01(\x0e\x32#.google.protobuf.FieldOptions.CType:\x06STRINGR\x05\x63type\x12\x16\n\x06packed\x18\x02 \x01(\x08R\x06packed\x12G\n\x06jstype\x18\x06 \x01(\x0e\x32$.google.protobuf.FieldOptions.JSType:\tJS_NORMALR\x06jstype\x12\x19\n\x04lazy\x18\x05 \x01(\x08:\x05\x66\x61lseR\x04lazy\x12.\n\x0funverified_lazy\x18\x0f \x01(\x08:\x05\x66\x61lseR\x0eunverifiedLazy\x12%\n\ndeprecated\x18\x03 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12\x19\n\x04weak\x18\n \x01(\x08:\x05\x66\x61lseR\x04weak\x12(\n\x0c\x64\x65\x62ug_redact\x18\x10 \x01(\x08:\x05\x66\x61lseR\x0b\x64\x65\x62ugRedact\x12K\n\tretention\x18\x11 \x01(\x0e\x32-.google.protobuf.FieldOptions.OptionRetentionR\tretention\x12H\n\x07targets\x18\x13 \x03(\x0e\x32..google.protobuf.FieldOptions.OptionTargetTypeR\x07targets\x12W\n\x10\x65\x64ition_defaults\x18\x14 \x03(\x0b\x32,.google.protobuf.FieldOptions.EditionDefaultR\x0f\x65\x64itionDefaults\x12\x37\n\x08\x66\x65\x61tures\x18\x15 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12U\n\x0f\x66\x65\x61ture_support\x18\x16 \x01(\x0b\x32,.google.protobuf.FieldOptions.FeatureSupportR\x0e\x66\x65\x61tureSupport\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\x1aZ\n\x0e\x45\x64itionDefault\x12\x32\n\x07\x65\x64ition\x18\x03 \x01(\x0e\x32\x18.google.protobuf.EditionR\x07\x65\x64ition\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value\x1a\x96\x02\n\x0e\x46\x65\x61tureSupport\x12G\n\x12\x65\x64ition_introduced\x18\x01 \x01(\x0e\x32\x18.google.protobuf.EditionR\x11\x65\x64itionIntroduced\x12G\n\x12\x65\x64ition_deprecated\x18\x02 \x01(\x0e\x32\x18.google.protobuf.EditionR\x11\x65\x64itionDeprecated\x12/\n\x13\x64\x65precation_warning\x18\x03 \x01(\tR\x12\x64\x65precationWarning\x12\x41\n\x0f\x65\x64ition_removed\x18\x04 \x01(\x0e\x32\x18.google.protobuf.EditionR\x0e\x65\x64itionRemoved\"/\n\x05\x43Type\x12\n\n\x06STRING\x10\x00\x12\x08\n\x04\x43ORD\x10\x01\x12\x10\n\x0cSTRING_PIECE\x10\x02\"5\n\x06JSType\x12\r\n\tJS_NORMAL\x10\x00\x12\r\n\tJS_STRING\x10\x01\x12\r\n\tJS_NUMBER\x10\x02\"U\n\x0fOptionRetention\x12\x15\n\x11RETENTION_UNKNOWN\x10\x00\x12\x15\n\x11RETENTION_RUNTIME\x10\x01\x12\x14\n\x10RETENTION_SOURCE\x10\x02\"\x8c\x02\n\x10OptionTargetType\x12\x17\n\x13TARGET_TYPE_UNKNOWN\x10\x00\x12\x14\n\x10TARGET_TYPE_FILE\x10\x01\x12\x1f\n\x1bTARGET_TYPE_EXTENSION_RANGE\x10\x02\x12\x17\n\x13TARGET_TYPE_MESSAGE\x10\x03\x12\x15\n\x11TARGET_TYPE_FIELD\x10\x04\x12\x15\n\x11TARGET_TYPE_ONEOF\x10\x05\x12\x14\n\x10TARGET_TYPE_ENUM\x10\x06\x12\x1a\n\x16TARGET_TYPE_ENUM_ENTRY\x10\x07\x12\x17\n\x13TARGET_TYPE_SERVICE\x10\x08\x12\x16\n\x12TARGET_TYPE_METHOD\x10\t*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08\x04\x10\x05J\x04\x08\x12\x10\x13\"\xac\x01\n\x0cOneofOptions\x12\x37\n\x08\x66\x65\x61tures\x18\x01 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\xd1\x02\n\x0b\x45numOptions\x12\x1f\n\x0b\x61llow_alias\x18\x02 \x01(\x08R\nallowAlias\x12%\n\ndeprecated\x18\x03 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12V\n&deprecated_legacy_json_field_conflicts\x18\x06 \x01(\x08\x42\x02\x18\x01R\"deprecatedLegacyJsonFieldConflicts\x12\x37\n\x08\x66\x65\x61tures\x18\x07 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08\x05\x10\x06\"\x81\x02\n\x10\x45numValueOptions\x12%\n\ndeprecated\x18\x01 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12\x37\n\x08\x66\x65\x61tures\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12(\n\x0c\x64\x65\x62ug_redact\x18\x03 \x01(\x08:\x05\x66\x61lseR\x0b\x64\x65\x62ugRedact\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\xd5\x01\n\x0eServiceOptions\x12\x37\n\x08\x66\x65\x61tures\x18\" \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12%\n\ndeprecated\x18! \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\x99\x03\n\rMethodOptions\x12%\n\ndeprecated\x18! \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12q\n\x11idempotency_level\x18\" \x01(\x0e\x32/.google.protobuf.MethodOptions.IdempotencyLevel:\x13IDEMPOTENCY_UNKNOWNR\x10idempotencyLevel\x12\x37\n\x08\x66\x65\x61tures\x18# \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\"P\n\x10IdempotencyLevel\x12\x17\n\x13IDEMPOTENCY_UNKNOWN\x10\x00\x12\x13\n\x0fNO_SIDE_EFFECTS\x10\x01\x12\x0e\n\nIDEMPOTENT\x10\x02*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\x9a\x03\n\x13UninterpretedOption\x12\x41\n\x04name\x18\x02 \x03(\x0b\x32-.google.protobuf.UninterpretedOption.NamePartR\x04name\x12)\n\x10identifier_value\x18\x03 \x01(\tR\x0fidentifierValue\x12,\n\x12positive_int_value\x18\x04 \x01(\x04R\x10positiveIntValue\x12,\n\x12negative_int_value\x18\x05 \x01(\x03R\x10negativeIntValue\x12!\n\x0c\x64ouble_value\x18\x06 \x01(\x01R\x0b\x64oubleValue\x12!\n\x0cstring_value\x18\x07 \x01(\x0cR\x0bstringValue\x12\'\n\x0f\x61ggregate_value\x18\x08 \x01(\tR\x0e\x61ggregateValue\x1aJ\n\x08NamePart\x12\x1b\n\tname_part\x18\x01 \x02(\tR\x08namePart\x12!\n\x0cis_extension\x18\x02 \x02(\x08R\x0bisExtension\"\xb9\n\n\nFeatureSet\x12\x91\x01\n\x0e\x66ield_presence\x18\x01 \x01(\x0e\x32).google.protobuf.FeatureSet.FieldPresenceB?\x88\x01\x01\x98\x01\x04\x98\x01\x01\xa2\x01\r\x12\x08\x45XPLICIT\x18\xe6\x07\xa2\x01\r\x12\x08IMPLICIT\x18\xe7\x07\xa2\x01\r\x12\x08\x45XPLICIT\x18\xe8\x07\xb2\x01\x03\x08\xe8\x07R\rfieldPresence\x12l\n\tenum_type\x18\x02 \x01(\x0e\x32$.google.protobuf.FeatureSet.EnumTypeB)\x88\x01\x01\x98\x01\x06\x98\x01\x01\xa2\x01\x0b\x12\x06\x43LOSED\x18\xe6\x07\xa2\x01\t\x12\x04OPEN\x18\xe7\x07\xb2\x01\x03\x08\xe8\x07R\x08\x65numType\x12\x98\x01\n\x17repeated_field_encoding\x18\x03 \x01(\x0e\x32\x31.google.protobuf.FeatureSet.RepeatedFieldEncodingB-\x88\x01\x01\x98\x01\x04\x98\x01\x01\xa2\x01\r\x12\x08\x45XPANDED\x18\xe6\x07\xa2\x01\x0b\x12\x06PACKED\x18\xe7\x07\xb2\x01\x03\x08\xe8\x07R\x15repeatedFieldEncoding\x12~\n\x0futf8_validation\x18\x04 \x01(\x0e\x32*.google.protobuf.FeatureSet.Utf8ValidationB)\x88\x01\x01\x98\x01\x04\x98\x01\x01\xa2\x01\t\x12\x04NONE\x18\xe6\x07\xa2\x01\x0b\x12\x06VERIFY\x18\xe7\x07\xb2\x01\x03\x08\xe8\x07R\x0eutf8Validation\x12~\n\x10message_encoding\x18\x05 \x01(\x0e\x32+.google.protobuf.FeatureSet.MessageEncodingB&\x88\x01\x01\x98\x01\x04\x98\x01\x01\xa2\x01\x14\x12\x0fLENGTH_PREFIXED\x18\xe6\x07\xb2\x01\x03\x08\xe8\x07R\x0fmessageEncoding\x12\x82\x01\n\x0bjson_format\x18\x06 \x01(\x0e\x32&.google.protobuf.FeatureSet.JsonFormatB9\x88\x01\x01\x98\x01\x03\x98\x01\x06\x98\x01\x01\xa2\x01\x17\x12\x12LEGACY_BEST_EFFORT\x18\xe6\x07\xa2\x01\n\x12\x05\x41LLOW\x18\xe7\x07\xb2\x01\x03\x08\xe8\x07R\njsonFormat\"\\\n\rFieldPresence\x12\x1a\n\x16\x46IELD_PRESENCE_UNKNOWN\x10\x00\x12\x0c\n\x08\x45XPLICIT\x10\x01\x12\x0c\n\x08IMPLICIT\x10\x02\x12\x13\n\x0fLEGACY_REQUIRED\x10\x03\"7\n\x08\x45numType\x12\x15\n\x11\x45NUM_TYPE_UNKNOWN\x10\x00\x12\x08\n\x04OPEN\x10\x01\x12\n\n\x06\x43LOSED\x10\x02\"V\n\x15RepeatedFieldEncoding\x12#\n\x1fREPEATED_FIELD_ENCODING_UNKNOWN\x10\x00\x12\n\n\x06PACKED\x10\x01\x12\x0c\n\x08\x45XPANDED\x10\x02\"C\n\x0eUtf8Validation\x12\x1b\n\x17UTF8_VALIDATION_UNKNOWN\x10\x00\x12\n\n\x06VERIFY\x10\x02\x12\x08\n\x04NONE\x10\x03\"S\n\x0fMessageEncoding\x12\x1c\n\x18MESSAGE_ENCODING_UNKNOWN\x10\x00\x12\x13\n\x0fLENGTH_PREFIXED\x10\x01\x12\r\n\tDELIMITED\x10\x02\"H\n\nJsonFormat\x12\x17\n\x13JSON_FORMAT_UNKNOWN\x10\x00\x12\t\n\x05\x41LLOW\x10\x01\x12\x16\n\x12LEGACY_BEST_EFFORT\x10\x02*\x06\x08\xe8\x07\x10\xe9\x07*\x06\x08\xe9\x07\x10\xea\x07*\x06\x08\xea\x07\x10\xeb\x07*\x06\x08\x86N\x10\x87N*\x06\x08\x8bN\x10\x90N*\x06\x08\x90N\x10\x91NJ\x06\x08\xe7\x07\x10\xe8\x07\"\xd9\x03\n\x12\x46\x65\x61tureSetDefaults\x12X\n\x08\x64\x65\x66\x61ults\x18\x01 \x03(\x0b\x32<.google.protobuf.FeatureSetDefaults.FeatureSetEditionDefaultR\x08\x64\x65\x66\x61ults\x12\x41\n\x0fminimum_edition\x18\x04 \x01(\x0e\x32\x18.google.protobuf.EditionR\x0eminimumEdition\x12\x41\n\x0fmaximum_edition\x18\x05 \x01(\x0e\x32\x18.google.protobuf.EditionR\x0emaximumEdition\x1a\xe2\x01\n\x18\x46\x65\x61tureSetEditionDefault\x12\x32\n\x07\x65\x64ition\x18\x03 \x01(\x0e\x32\x18.google.protobuf.EditionR\x07\x65\x64ition\x12N\n\x14overridable_features\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x13overridableFeatures\x12\x42\n\x0e\x66ixed_features\x18\x05 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\rfixedFeatures\"\xa7\x02\n\x0eSourceCodeInfo\x12\x44\n\x08location\x18\x01 \x03(\x0b\x32(.google.protobuf.SourceCodeInfo.LocationR\x08location\x1a\xce\x01\n\x08Location\x12\x16\n\x04path\x18\x01 \x03(\x05\x42\x02\x10\x01R\x04path\x12\x16\n\x04span\x18\x02 \x03(\x05\x42\x02\x10\x01R\x04span\x12)\n\x10leading_comments\x18\x03 \x01(\tR\x0fleadingComments\x12+\n\x11trailing_comments\x18\x04 \x01(\tR\x10trailingComments\x12:\n\x19leading_detached_comments\x18\x06 \x03(\tR\x17leadingDetachedComments\"\xd0\x02\n\x11GeneratedCodeInfo\x12M\n\nannotation\x18\x01 \x03(\x0b\x32-.google.protobuf.GeneratedCodeInfo.AnnotationR\nannotation\x1a\xeb\x01\n\nAnnotation\x12\x16\n\x04path\x18\x01 \x03(\x05\x42\x02\x10\x01R\x04path\x12\x1f\n\x0bsource_file\x18\x02 \x01(\tR\nsourceFile\x12\x14\n\x05\x62\x65gin\x18\x03 \x01(\x05R\x05\x62\x65gin\x12\x10\n\x03\x65nd\x18\x04 \x01(\x05R\x03\x65nd\x12R\n\x08semantic\x18\x05 \x01(\x0e\x32\x36.google.protobuf.GeneratedCodeInfo.Annotation.SemanticR\x08semantic\"(\n\x08Semantic\x12\x08\n\x04NONE\x10\x00\x12\x07\n\x03SET\x10\x01\x12\t\n\x05\x41LIAS\x10\x02*\xa7\x02\n\x07\x45\x64ition\x12\x13\n\x0f\x45\x44ITION_UNKNOWN\x10\x00\x12\x13\n\x0e\x45\x44ITION_LEGACY\x10\x84\x07\x12\x13\n\x0e\x45\x44ITION_PROTO2\x10\xe6\x07\x12\x13\n\x0e\x45\x44ITION_PROTO3\x10\xe7\x07\x12\x11\n\x0c\x45\x44ITION_2023\x10\xe8\x07\x12\x11\n\x0c\x45\x44ITION_2024\x10\xe9\x07\x12\x17\n\x13\x45\x44ITION_1_TEST_ONLY\x10\x01\x12\x17\n\x13\x45\x44ITION_2_TEST_ONLY\x10\x02\x12\x1d\n\x17\x45\x44ITION_99997_TEST_ONLY\x10\x9d\x8d\x06\x12\x1d\n\x17\x45\x44ITION_99998_TEST_ONLY\x10\x9e\x8d\x06\x12\x1d\n\x17\x45\x44ITION_99999_TEST_ONLY\x10\x9f\x8d\x06\x12\x13\n\x0b\x45\x44ITION_MAX\x10\xff\xff\xff\xff\x07\x42~\n\x13\x63om.google.protobufB\x10\x44\x65scriptorProtosH\x01Z-google.golang.org/protobuf/types/descriptorpb\xf8\x01\x01\xa2\x02\x03GPB\xaa\x02\x1aGoogle.Protobuf.Reflection'
   )
 else:
-  DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n google/protobuf/descriptor.proto\x12\x0fgoogle.protobuf\"M\n\x11\x46ileDescriptorSet\x12\x38\n\x04\x66ile\x18\x01 \x03(\x0b\x32$.google.protobuf.FileDescriptorProtoR\x04\x66ile\"\x98\x05\n\x13\x46ileDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x18\n\x07package\x18\x02 \x01(\tR\x07package\x12\x1e\n\ndependency\x18\x03 \x03(\tR\ndependency\x12+\n\x11public_dependency\x18\n \x03(\x05R\x10publicDependency\x12\'\n\x0fweak_dependency\x18\x0b \x03(\x05R\x0eweakDependency\x12\x43\n\x0cmessage_type\x18\x04 \x03(\x0b\x32 .google.protobuf.DescriptorProtoR\x0bmessageType\x12\x41\n\tenum_type\x18\x05 \x03(\x0b\x32$.google.protobuf.EnumDescriptorProtoR\x08\x65numType\x12\x41\n\x07service\x18\x06 \x03(\x0b\x32\'.google.protobuf.ServiceDescriptorProtoR\x07service\x12\x43\n\textension\x18\x07 \x03(\x0b\x32%.google.protobuf.FieldDescriptorProtoR\textension\x12\x36\n\x07options\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.FileOptionsR\x07options\x12I\n\x10source_code_info\x18\t \x01(\x0b\x32\x1f.google.protobuf.SourceCodeInfoR\x0esourceCodeInfo\x12\x16\n\x06syntax\x18\x0c \x01(\tR\x06syntax\x12\x32\n\x07\x65\x64ition\x18\x0e \x01(\x0e\x32\x18.google.protobuf.EditionR\x07\x65\x64ition\"\xb9\x06\n\x0f\x44\x65scriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12;\n\x05\x66ield\x18\x02 \x03(\x0b\x32%.google.protobuf.FieldDescriptorProtoR\x05\x66ield\x12\x43\n\textension\x18\x06 \x03(\x0b\x32%.google.protobuf.FieldDescriptorProtoR\textension\x12\x41\n\x0bnested_type\x18\x03 \x03(\x0b\x32 .google.protobuf.DescriptorProtoR\nnestedType\x12\x41\n\tenum_type\x18\x04 \x03(\x0b\x32$.google.protobuf.EnumDescriptorProtoR\x08\x65numType\x12X\n\x0f\x65xtension_range\x18\x05 \x03(\x0b\x32/.google.protobuf.DescriptorProto.ExtensionRangeR\x0e\x65xtensionRange\x12\x44\n\noneof_decl\x18\x08 \x03(\x0b\x32%.google.protobuf.OneofDescriptorProtoR\toneofDecl\x12\x39\n\x07options\x18\x07 \x01(\x0b\x32\x1f.google.protobuf.MessageOptionsR\x07options\x12U\n\x0ereserved_range\x18\t \x03(\x0b\x32..google.protobuf.DescriptorProto.ReservedRangeR\rreservedRange\x12#\n\rreserved_name\x18\n \x03(\tR\x0creservedName\x1az\n\x0e\x45xtensionRange\x12\x14\n\x05start\x18\x01 \x01(\x05R\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\x05R\x03\x65nd\x12@\n\x07options\x18\x03 \x01(\x0b\x32&.google.protobuf.ExtensionRangeOptionsR\x07options\x1a\x37\n\rReservedRange\x12\x14\n\x05start\x18\x01 \x01(\x05R\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\x05R\x03\x65nd\"\xcc\x04\n\x15\x45xtensionRangeOptions\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\x12Y\n\x0b\x64\x65\x63laration\x18\x02 \x03(\x0b\x32\x32.google.protobuf.ExtensionRangeOptions.DeclarationB\x03\x88\x01\x02R\x0b\x64\x65\x63laration\x12\x37\n\x08\x66\x65\x61tures\x18\x32 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12m\n\x0cverification\x18\x03 \x01(\x0e\x32\x38.google.protobuf.ExtensionRangeOptions.VerificationState:\nUNVERIFIEDB\x03\x88\x01\x02R\x0cverification\x1a\x94\x01\n\x0b\x44\x65\x63laration\x12\x16\n\x06number\x18\x01 \x01(\x05R\x06number\x12\x1b\n\tfull_name\x18\x02 \x01(\tR\x08\x66ullName\x12\x12\n\x04type\x18\x03 \x01(\tR\x04type\x12\x1a\n\x08reserved\x18\x05 \x01(\x08R\x08reserved\x12\x1a\n\x08repeated\x18\x06 \x01(\x08R\x08repeatedJ\x04\x08\x04\x10\x05\"4\n\x11VerificationState\x12\x0f\n\x0b\x44\x45\x43LARATION\x10\x00\x12\x0e\n\nUNVERIFIED\x10\x01*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\xc1\x06\n\x14\x46ieldDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x16\n\x06number\x18\x03 \x01(\x05R\x06number\x12\x41\n\x05label\x18\x04 \x01(\x0e\x32+.google.protobuf.FieldDescriptorProto.LabelR\x05label\x12>\n\x04type\x18\x05 \x01(\x0e\x32*.google.protobuf.FieldDescriptorProto.TypeR\x04type\x12\x1b\n\ttype_name\x18\x06 \x01(\tR\x08typeName\x12\x1a\n\x08\x65xtendee\x18\x02 \x01(\tR\x08\x65xtendee\x12#\n\rdefault_value\x18\x07 \x01(\tR\x0c\x64\x65\x66\x61ultValue\x12\x1f\n\x0boneof_index\x18\t \x01(\x05R\noneofIndex\x12\x1b\n\tjson_name\x18\n \x01(\tR\x08jsonName\x12\x37\n\x07options\x18\x08 \x01(\x0b\x32\x1d.google.protobuf.FieldOptionsR\x07options\x12\'\n\x0fproto3_optional\x18\x11 \x01(\x08R\x0eproto3Optional\"\xb6\x02\n\x04Type\x12\x0f\n\x0bTYPE_DOUBLE\x10\x01\x12\x0e\n\nTYPE_FLOAT\x10\x02\x12\x0e\n\nTYPE_INT64\x10\x03\x12\x0f\n\x0bTYPE_UINT64\x10\x04\x12\x0e\n\nTYPE_INT32\x10\x05\x12\x10\n\x0cTYPE_FIXED64\x10\x06\x12\x10\n\x0cTYPE_FIXED32\x10\x07\x12\r\n\tTYPE_BOOL\x10\x08\x12\x0f\n\x0bTYPE_STRING\x10\t\x12\x0e\n\nTYPE_GROUP\x10\n\x12\x10\n\x0cTYPE_MESSAGE\x10\x0b\x12\x0e\n\nTYPE_BYTES\x10\x0c\x12\x0f\n\x0bTYPE_UINT32\x10\r\x12\r\n\tTYPE_ENUM\x10\x0e\x12\x11\n\rTYPE_SFIXED32\x10\x0f\x12\x11\n\rTYPE_SFIXED64\x10\x10\x12\x0f\n\x0bTYPE_SINT32\x10\x11\x12\x0f\n\x0bTYPE_SINT64\x10\x12\"C\n\x05Label\x12\x12\n\x0eLABEL_OPTIONAL\x10\x01\x12\x12\n\x0eLABEL_REPEATED\x10\x03\x12\x12\n\x0eLABEL_REQUIRED\x10\x02\"c\n\x14OneofDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x37\n\x07options\x18\x02 \x01(\x0b\x32\x1d.google.protobuf.OneofOptionsR\x07options\"\xe3\x02\n\x13\x45numDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12?\n\x05value\x18\x02 \x03(\x0b\x32).google.protobuf.EnumValueDescriptorProtoR\x05value\x12\x36\n\x07options\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.EnumOptionsR\x07options\x12]\n\x0ereserved_range\x18\x04 \x03(\x0b\x32\x36.google.protobuf.EnumDescriptorProto.EnumReservedRangeR\rreservedRange\x12#\n\rreserved_name\x18\x05 \x03(\tR\x0creservedName\x1a;\n\x11\x45numReservedRange\x12\x14\n\x05start\x18\x01 \x01(\x05R\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\x05R\x03\x65nd\"\x83\x01\n\x18\x45numValueDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x16\n\x06number\x18\x02 \x01(\x05R\x06number\x12;\n\x07options\x18\x03 \x01(\x0b\x32!.google.protobuf.EnumValueOptionsR\x07options\"\xa7\x01\n\x16ServiceDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12>\n\x06method\x18\x02 \x03(\x0b\x32&.google.protobuf.MethodDescriptorProtoR\x06method\x12\x39\n\x07options\x18\x03 \x01(\x0b\x32\x1f.google.protobuf.ServiceOptionsR\x07options\"\x89\x02\n\x15MethodDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x1d\n\ninput_type\x18\x02 \x01(\tR\tinputType\x12\x1f\n\x0boutput_type\x18\x03 \x01(\tR\noutputType\x12\x38\n\x07options\x18\x04 \x01(\x0b\x32\x1e.google.protobuf.MethodOptionsR\x07options\x12\x30\n\x10\x63lient_streaming\x18\x05 \x01(\x08:\x05\x66\x61lseR\x0f\x63lientStreaming\x12\x30\n\x10server_streaming\x18\x06 \x01(\x08:\x05\x66\x61lseR\x0fserverStreaming\"\x97\t\n\x0b\x46ileOptions\x12!\n\x0cjava_package\x18\x01 \x01(\tR\x0bjavaPackage\x12\x30\n\x14java_outer_classname\x18\x08 \x01(\tR\x12javaOuterClassname\x12\x35\n\x13java_multiple_files\x18\n \x01(\x08:\x05\x66\x61lseR\x11javaMultipleFiles\x12\x44\n\x1djava_generate_equals_and_hash\x18\x14 \x01(\x08\x42\x02\x18\x01R\x19javaGenerateEqualsAndHash\x12:\n\x16java_string_check_utf8\x18\x1b \x01(\x08:\x05\x66\x61lseR\x13javaStringCheckUtf8\x12S\n\x0coptimize_for\x18\t \x01(\x0e\x32).google.protobuf.FileOptions.OptimizeMode:\x05SPEEDR\x0boptimizeFor\x12\x1d\n\ngo_package\x18\x0b \x01(\tR\tgoPackage\x12\x35\n\x13\x63\x63_generic_services\x18\x10 \x01(\x08:\x05\x66\x61lseR\x11\x63\x63GenericServices\x12\x39\n\x15java_generic_services\x18\x11 \x01(\x08:\x05\x66\x61lseR\x13javaGenericServices\x12\x35\n\x13py_generic_services\x18\x12 \x01(\x08:\x05\x66\x61lseR\x11pyGenericServices\x12%\n\ndeprecated\x18\x17 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12.\n\x10\x63\x63_enable_arenas\x18\x1f \x01(\x08:\x04trueR\x0e\x63\x63\x45nableArenas\x12*\n\x11objc_class_prefix\x18$ \x01(\tR\x0fobjcClassPrefix\x12)\n\x10\x63sharp_namespace\x18% \x01(\tR\x0f\x63sharpNamespace\x12!\n\x0cswift_prefix\x18\' \x01(\tR\x0bswiftPrefix\x12(\n\x10php_class_prefix\x18( \x01(\tR\x0ephpClassPrefix\x12#\n\rphp_namespace\x18) \x01(\tR\x0cphpNamespace\x12\x34\n\x16php_metadata_namespace\x18, \x01(\tR\x14phpMetadataNamespace\x12!\n\x0cruby_package\x18- \x01(\tR\x0brubyPackage\x12\x37\n\x08\x66\x65\x61tures\x18\x32 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\":\n\x0cOptimizeMode\x12\t\n\x05SPEED\x10\x01\x12\r\n\tCODE_SIZE\x10\x02\x12\x10\n\x0cLITE_RUNTIME\x10\x03*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08*\x10+J\x04\x08&\x10\'\"\xf4\x03\n\x0eMessageOptions\x12<\n\x17message_set_wire_format\x18\x01 \x01(\x08:\x05\x66\x61lseR\x14messageSetWireFormat\x12L\n\x1fno_standard_descriptor_accessor\x18\x02 \x01(\x08:\x05\x66\x61lseR\x1cnoStandardDescriptorAccessor\x12%\n\ndeprecated\x18\x03 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12\x1b\n\tmap_entry\x18\x07 \x01(\x08R\x08mapEntry\x12V\n&deprecated_legacy_json_field_conflicts\x18\x0b \x01(\x08\x42\x02\x18\x01R\"deprecatedLegacyJsonFieldConflicts\x12\x37\n\x08\x66\x65\x61tures\x18\x0c \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07J\x04\x08\x08\x10\tJ\x04\x08\t\x10\n\"\xad\n\n\x0c\x46ieldOptions\x12\x41\n\x05\x63type\x18\x01 \x01(\x0e\x32#.google.protobuf.FieldOptions.CType:\x06STRINGR\x05\x63type\x12\x16\n\x06packed\x18\x02 \x01(\x08R\x06packed\x12G\n\x06jstype\x18\x06 \x01(\x0e\x32$.google.protobuf.FieldOptions.JSType:\tJS_NORMALR\x06jstype\x12\x19\n\x04lazy\x18\x05 \x01(\x08:\x05\x66\x61lseR\x04lazy\x12.\n\x0funverified_lazy\x18\x0f \x01(\x08:\x05\x66\x61lseR\x0eunverifiedLazy\x12%\n\ndeprecated\x18\x03 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12\x19\n\x04weak\x18\n \x01(\x08:\x05\x66\x61lseR\x04weak\x12(\n\x0c\x64\x65\x62ug_redact\x18\x10 \x01(\x08:\x05\x66\x61lseR\x0b\x64\x65\x62ugRedact\x12K\n\tretention\x18\x11 \x01(\x0e\x32-.google.protobuf.FieldOptions.OptionRetentionR\tretention\x12H\n\x07targets\x18\x13 \x03(\x0e\x32..google.protobuf.FieldOptions.OptionTargetTypeR\x07targets\x12W\n\x10\x65\x64ition_defaults\x18\x14 \x03(\x0b\x32,.google.protobuf.FieldOptions.EditionDefaultR\x0f\x65\x64itionDefaults\x12\x37\n\x08\x66\x65\x61tures\x18\x15 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\x1aZ\n\x0e\x45\x64itionDefault\x12\x32\n\x07\x65\x64ition\x18\x03 \x01(\x0e\x32\x18.google.protobuf.EditionR\x07\x65\x64ition\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value\"/\n\x05\x43Type\x12\n\n\x06STRING\x10\x00\x12\x08\n\x04\x43ORD\x10\x01\x12\x10\n\x0cSTRING_PIECE\x10\x02\"5\n\x06JSType\x12\r\n\tJS_NORMAL\x10\x00\x12\r\n\tJS_STRING\x10\x01\x12\r\n\tJS_NUMBER\x10\x02\"U\n\x0fOptionRetention\x12\x15\n\x11RETENTION_UNKNOWN\x10\x00\x12\x15\n\x11RETENTION_RUNTIME\x10\x01\x12\x14\n\x10RETENTION_SOURCE\x10\x02\"\x8c\x02\n\x10OptionTargetType\x12\x17\n\x13TARGET_TYPE_UNKNOWN\x10\x00\x12\x14\n\x10TARGET_TYPE_FILE\x10\x01\x12\x1f\n\x1bTARGET_TYPE_EXTENSION_RANGE\x10\x02\x12\x17\n\x13TARGET_TYPE_MESSAGE\x10\x03\x12\x15\n\x11TARGET_TYPE_FIELD\x10\x04\x12\x15\n\x11TARGET_TYPE_ONEOF\x10\x05\x12\x14\n\x10TARGET_TYPE_ENUM\x10\x06\x12\x1a\n\x16TARGET_TYPE_ENUM_ENTRY\x10\x07\x12\x17\n\x13TARGET_TYPE_SERVICE\x10\x08\x12\x16\n\x12TARGET_TYPE_METHOD\x10\t*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08\x04\x10\x05J\x04\x08\x12\x10\x13\"\xac\x01\n\x0cOneofOptions\x12\x37\n\x08\x66\x65\x61tures\x18\x01 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\xd1\x02\n\x0b\x45numOptions\x12\x1f\n\x0b\x61llow_alias\x18\x02 \x01(\x08R\nallowAlias\x12%\n\ndeprecated\x18\x03 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12V\n&deprecated_legacy_json_field_conflicts\x18\x06 \x01(\x08\x42\x02\x18\x01R\"deprecatedLegacyJsonFieldConflicts\x12\x37\n\x08\x66\x65\x61tures\x18\x07 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08\x05\x10\x06\"\x81\x02\n\x10\x45numValueOptions\x12%\n\ndeprecated\x18\x01 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12\x37\n\x08\x66\x65\x61tures\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12(\n\x0c\x64\x65\x62ug_redact\x18\x03 \x01(\x08:\x05\x66\x61lseR\x0b\x64\x65\x62ugRedact\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\xd5\x01\n\x0eServiceOptions\x12\x37\n\x08\x66\x65\x61tures\x18\" \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12%\n\ndeprecated\x18! \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\x99\x03\n\rMethodOptions\x12%\n\ndeprecated\x18! \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12q\n\x11idempotency_level\x18\" \x01(\x0e\x32/.google.protobuf.MethodOptions.IdempotencyLevel:\x13IDEMPOTENCY_UNKNOWNR\x10idempotencyLevel\x12\x37\n\x08\x66\x65\x61tures\x18# \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\"P\n\x10IdempotencyLevel\x12\x17\n\x13IDEMPOTENCY_UNKNOWN\x10\x00\x12\x13\n\x0fNO_SIDE_EFFECTS\x10\x01\x12\x0e\n\nIDEMPOTENT\x10\x02*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\x9a\x03\n\x13UninterpretedOption\x12\x41\n\x04name\x18\x02 \x03(\x0b\x32-.google.protobuf.UninterpretedOption.NamePartR\x04name\x12)\n\x10identifier_value\x18\x03 \x01(\tR\x0fidentifierValue\x12,\n\x12positive_int_value\x18\x04 \x01(\x04R\x10positiveIntValue\x12,\n\x12negative_int_value\x18\x05 \x01(\x03R\x10negativeIntValue\x12!\n\x0c\x64ouble_value\x18\x06 \x01(\x01R\x0b\x64oubleValue\x12!\n\x0cstring_value\x18\x07 \x01(\x0cR\x0bstringValue\x12\'\n\x0f\x61ggregate_value\x18\x08 \x01(\tR\x0e\x61ggregateValue\x1aJ\n\x08NamePart\x12\x1b\n\tname_part\x18\x01 \x02(\tR\x08namePart\x12!\n\x0cis_extension\x18\x02 \x02(\x08R\x0bisExtension\"\x8c\n\n\nFeatureSet\x12\x8b\x01\n\x0e\x66ield_presence\x18\x01 \x01(\x0e\x32).google.protobuf.FeatureSet.FieldPresenceB9\x88\x01\x01\x98\x01\x04\x98\x01\x01\xa2\x01\r\x12\x08\x45XPLICIT\x18\xe6\x07\xa2\x01\r\x12\x08IMPLICIT\x18\xe7\x07\xa2\x01\r\x12\x08\x45XPLICIT\x18\xe8\x07R\rfieldPresence\x12\x66\n\tenum_type\x18\x02 \x01(\x0e\x32$.google.protobuf.FeatureSet.EnumTypeB#\x88\x01\x01\x98\x01\x06\x98\x01\x01\xa2\x01\x0b\x12\x06\x43LOSED\x18\xe6\x07\xa2\x01\t\x12\x04OPEN\x18\xe7\x07R\x08\x65numType\x12\x92\x01\n\x17repeated_field_encoding\x18\x03 \x01(\x0e\x32\x31.google.protobuf.FeatureSet.RepeatedFieldEncodingB\'\x88\x01\x01\x98\x01\x04\x98\x01\x01\xa2\x01\r\x12\x08\x45XPANDED\x18\xe6\x07\xa2\x01\x0b\x12\x06PACKED\x18\xe7\x07R\x15repeatedFieldEncoding\x12x\n\x0futf8_validation\x18\x04 \x01(\x0e\x32*.google.protobuf.FeatureSet.Utf8ValidationB#\x88\x01\x01\x98\x01\x04\x98\x01\x01\xa2\x01\t\x12\x04NONE\x18\xe6\x07\xa2\x01\x0b\x12\x06VERIFY\x18\xe7\x07R\x0eutf8Validation\x12x\n\x10message_encoding\x18\x05 \x01(\x0e\x32+.google.protobuf.FeatureSet.MessageEncodingB \x88\x01\x01\x98\x01\x04\x98\x01\x01\xa2\x01\x14\x12\x0fLENGTH_PREFIXED\x18\xe6\x07R\x0fmessageEncoding\x12|\n\x0bjson_format\x18\x06 \x01(\x0e\x32&.google.protobuf.FeatureSet.JsonFormatB3\x88\x01\x01\x98\x01\x03\x98\x01\x06\x98\x01\x01\xa2\x01\x17\x12\x12LEGACY_BEST_EFFORT\x18\xe6\x07\xa2\x01\n\x12\x05\x41LLOW\x18\xe7\x07R\njsonFormat\"\\\n\rFieldPresence\x12\x1a\n\x16\x46IELD_PRESENCE_UNKNOWN\x10\x00\x12\x0c\n\x08\x45XPLICIT\x10\x01\x12\x0c\n\x08IMPLICIT\x10\x02\x12\x13\n\x0fLEGACY_REQUIRED\x10\x03\"7\n\x08\x45numType\x12\x15\n\x11\x45NUM_TYPE_UNKNOWN\x10\x00\x12\x08\n\x04OPEN\x10\x01\x12\n\n\x06\x43LOSED\x10\x02\"V\n\x15RepeatedFieldEncoding\x12#\n\x1fREPEATED_FIELD_ENCODING_UNKNOWN\x10\x00\x12\n\n\x06PACKED\x10\x01\x12\x0c\n\x08\x45XPANDED\x10\x02\"C\n\x0eUtf8Validation\x12\x1b\n\x17UTF8_VALIDATION_UNKNOWN\x10\x00\x12\n\n\x06VERIFY\x10\x02\x12\x08\n\x04NONE\x10\x03\"S\n\x0fMessageEncoding\x12\x1c\n\x18MESSAGE_ENCODING_UNKNOWN\x10\x00\x12\x13\n\x0fLENGTH_PREFIXED\x10\x01\x12\r\n\tDELIMITED\x10\x02\"H\n\nJsonFormat\x12\x17\n\x13JSON_FORMAT_UNKNOWN\x10\x00\x12\t\n\x05\x41LLOW\x10\x01\x12\x16\n\x12LEGACY_BEST_EFFORT\x10\x02*\x06\x08\xe8\x07\x10\xe9\x07*\x06\x08\xe9\x07\x10\xea\x07*\x06\x08\xea\x07\x10\xeb\x07*\x06\x08\x8bN\x10\x90N*\x06\x08\x90N\x10\x91NJ\x06\x08\xe7\x07\x10\xe8\x07\"\xfe\x02\n\x12\x46\x65\x61tureSetDefaults\x12X\n\x08\x64\x65\x66\x61ults\x18\x01 \x03(\x0b\x32<.google.protobuf.FeatureSetDefaults.FeatureSetEditionDefaultR\x08\x64\x65\x66\x61ults\x12\x41\n\x0fminimum_edition\x18\x04 \x01(\x0e\x32\x18.google.protobuf.EditionR\x0eminimumEdition\x12\x41\n\x0fmaximum_edition\x18\x05 \x01(\x0e\x32\x18.google.protobuf.EditionR\x0emaximumEdition\x1a\x87\x01\n\x18\x46\x65\x61tureSetEditionDefault\x12\x32\n\x07\x65\x64ition\x18\x03 \x01(\x0e\x32\x18.google.protobuf.EditionR\x07\x65\x64ition\x12\x37\n\x08\x66\x65\x61tures\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\"\xa7\x02\n\x0eSourceCodeInfo\x12\x44\n\x08location\x18\x01 \x03(\x0b\x32(.google.protobuf.SourceCodeInfo.LocationR\x08location\x1a\xce\x01\n\x08Location\x12\x16\n\x04path\x18\x01 \x03(\x05\x42\x02\x10\x01R\x04path\x12\x16\n\x04span\x18\x02 \x03(\x05\x42\x02\x10\x01R\x04span\x12)\n\x10leading_comments\x18\x03 \x01(\tR\x0fleadingComments\x12+\n\x11trailing_comments\x18\x04 \x01(\tR\x10trailingComments\x12:\n\x19leading_detached_comments\x18\x06 \x03(\tR\x17leadingDetachedComments\"\xd0\x02\n\x11GeneratedCodeInfo\x12M\n\nannotation\x18\x01 \x03(\x0b\x32-.google.protobuf.GeneratedCodeInfo.AnnotationR\nannotation\x1a\xeb\x01\n\nAnnotation\x12\x16\n\x04path\x18\x01 \x03(\x05\x42\x02\x10\x01R\x04path\x12\x1f\n\x0bsource_file\x18\x02 \x01(\tR\nsourceFile\x12\x14\n\x05\x62\x65gin\x18\x03 \x01(\x05R\x05\x62\x65gin\x12\x10\n\x03\x65nd\x18\x04 \x01(\x05R\x03\x65nd\x12R\n\x08semantic\x18\x05 \x01(\x0e\x32\x36.google.protobuf.GeneratedCodeInfo.Annotation.SemanticR\x08semantic\"(\n\x08Semantic\x12\x08\n\x04NONE\x10\x00\x12\x07\n\x03SET\x10\x01\x12\t\n\x05\x41LIAS\x10\x02*\x92\x02\n\x07\x45\x64ition\x12\x13\n\x0f\x45\x44ITION_UNKNOWN\x10\x00\x12\x13\n\x0e\x45\x44ITION_PROTO2\x10\xe6\x07\x12\x13\n\x0e\x45\x44ITION_PROTO3\x10\xe7\x07\x12\x11\n\x0c\x45\x44ITION_2023\x10\xe8\x07\x12\x11\n\x0c\x45\x44ITION_2024\x10\xe9\x07\x12\x17\n\x13\x45\x44ITION_1_TEST_ONLY\x10\x01\x12\x17\n\x13\x45\x44ITION_2_TEST_ONLY\x10\x02\x12\x1d\n\x17\x45\x44ITION_99997_TEST_ONLY\x10\x9d\x8d\x06\x12\x1d\n\x17\x45\x44ITION_99998_TEST_ONLY\x10\x9e\x8d\x06\x12\x1d\n\x17\x45\x44ITION_99999_TEST_ONLY\x10\x9f\x8d\x06\x12\x13\n\x0b\x45\x44ITION_MAX\x10\xff\xff\xff\xff\x07\x42~\n\x13\x63om.google.protobufB\x10\x44\x65scriptorProtosH\x01Z-google.golang.org/protobuf/types/descriptorpb\xf8\x01\x01\xa2\x02\x03GPB\xaa\x02\x1aGoogle.Protobuf.Reflection')
+  DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n google/protobuf/descriptor.proto\x12\x0fgoogle.protobuf\"M\n\x11\x46ileDescriptorSet\x12\x38\n\x04\x66ile\x18\x01 \x03(\x0b\x32$.google.protobuf.FileDescriptorProtoR\x04\x66ile\"\x98\x05\n\x13\x46ileDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x18\n\x07package\x18\x02 \x01(\tR\x07package\x12\x1e\n\ndependency\x18\x03 \x03(\tR\ndependency\x12+\n\x11public_dependency\x18\n \x03(\x05R\x10publicDependency\x12\'\n\x0fweak_dependency\x18\x0b \x03(\x05R\x0eweakDependency\x12\x43\n\x0cmessage_type\x18\x04 \x03(\x0b\x32 .google.protobuf.DescriptorProtoR\x0bmessageType\x12\x41\n\tenum_type\x18\x05 \x03(\x0b\x32$.google.protobuf.EnumDescriptorProtoR\x08\x65numType\x12\x41\n\x07service\x18\x06 \x03(\x0b\x32\'.google.protobuf.ServiceDescriptorProtoR\x07service\x12\x43\n\textension\x18\x07 \x03(\x0b\x32%.google.protobuf.FieldDescriptorProtoR\textension\x12\x36\n\x07options\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.FileOptionsR\x07options\x12I\n\x10source_code_info\x18\t \x01(\x0b\x32\x1f.google.protobuf.SourceCodeInfoR\x0esourceCodeInfo\x12\x16\n\x06syntax\x18\x0c \x01(\tR\x06syntax\x12\x32\n\x07\x65\x64ition\x18\x0e \x01(\x0e\x32\x18.google.protobuf.EditionR\x07\x65\x64ition\"\xb9\x06\n\x0f\x44\x65scriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12;\n\x05\x66ield\x18\x02 \x03(\x0b\x32%.google.protobuf.FieldDescriptorProtoR\x05\x66ield\x12\x43\n\textension\x18\x06 \x03(\x0b\x32%.google.protobuf.FieldDescriptorProtoR\textension\x12\x41\n\x0bnested_type\x18\x03 \x03(\x0b\x32 .google.protobuf.DescriptorProtoR\nnestedType\x12\x41\n\tenum_type\x18\x04 \x03(\x0b\x32$.google.protobuf.EnumDescriptorProtoR\x08\x65numType\x12X\n\x0f\x65xtension_range\x18\x05 \x03(\x0b\x32/.google.protobuf.DescriptorProto.ExtensionRangeR\x0e\x65xtensionRange\x12\x44\n\noneof_decl\x18\x08 \x03(\x0b\x32%.google.protobuf.OneofDescriptorProtoR\toneofDecl\x12\x39\n\x07options\x18\x07 \x01(\x0b\x32\x1f.google.protobuf.MessageOptionsR\x07options\x12U\n\x0ereserved_range\x18\t \x03(\x0b\x32..google.protobuf.DescriptorProto.ReservedRangeR\rreservedRange\x12#\n\rreserved_name\x18\n \x03(\tR\x0creservedName\x1az\n\x0e\x45xtensionRange\x12\x14\n\x05start\x18\x01 \x01(\x05R\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\x05R\x03\x65nd\x12@\n\x07options\x18\x03 \x01(\x0b\x32&.google.protobuf.ExtensionRangeOptionsR\x07options\x1a\x37\n\rReservedRange\x12\x14\n\x05start\x18\x01 \x01(\x05R\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\x05R\x03\x65nd\"\xcc\x04\n\x15\x45xtensionRangeOptions\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\x12Y\n\x0b\x64\x65\x63laration\x18\x02 \x03(\x0b\x32\x32.google.protobuf.ExtensionRangeOptions.DeclarationB\x03\x88\x01\x02R\x0b\x64\x65\x63laration\x12\x37\n\x08\x66\x65\x61tures\x18\x32 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12m\n\x0cverification\x18\x03 \x01(\x0e\x32\x38.google.protobuf.ExtensionRangeOptions.VerificationState:\nUNVERIFIEDB\x03\x88\x01\x02R\x0cverification\x1a\x94\x01\n\x0b\x44\x65\x63laration\x12\x16\n\x06number\x18\x01 \x01(\x05R\x06number\x12\x1b\n\tfull_name\x18\x02 \x01(\tR\x08\x66ullName\x12\x12\n\x04type\x18\x03 \x01(\tR\x04type\x12\x1a\n\x08reserved\x18\x05 \x01(\x08R\x08reserved\x12\x1a\n\x08repeated\x18\x06 \x01(\x08R\x08repeatedJ\x04\x08\x04\x10\x05\"4\n\x11VerificationState\x12\x0f\n\x0b\x44\x45\x43LARATION\x10\x00\x12\x0e\n\nUNVERIFIED\x10\x01*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\xc1\x06\n\x14\x46ieldDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x16\n\x06number\x18\x03 \x01(\x05R\x06number\x12\x41\n\x05label\x18\x04 \x01(\x0e\x32+.google.protobuf.FieldDescriptorProto.LabelR\x05label\x12>\n\x04type\x18\x05 \x01(\x0e\x32*.google.protobuf.FieldDescriptorProto.TypeR\x04type\x12\x1b\n\ttype_name\x18\x06 \x01(\tR\x08typeName\x12\x1a\n\x08\x65xtendee\x18\x02 \x01(\tR\x08\x65xtendee\x12#\n\rdefault_value\x18\x07 \x01(\tR\x0c\x64\x65\x66\x61ultValue\x12\x1f\n\x0boneof_index\x18\t \x01(\x05R\noneofIndex\x12\x1b\n\tjson_name\x18\n \x01(\tR\x08jsonName\x12\x37\n\x07options\x18\x08 \x01(\x0b\x32\x1d.google.protobuf.FieldOptionsR\x07options\x12\'\n\x0fproto3_optional\x18\x11 \x01(\x08R\x0eproto3Optional\"\xb6\x02\n\x04Type\x12\x0f\n\x0bTYPE_DOUBLE\x10\x01\x12\x0e\n\nTYPE_FLOAT\x10\x02\x12\x0e\n\nTYPE_INT64\x10\x03\x12\x0f\n\x0bTYPE_UINT64\x10\x04\x12\x0e\n\nTYPE_INT32\x10\x05\x12\x10\n\x0cTYPE_FIXED64\x10\x06\x12\x10\n\x0cTYPE_FIXED32\x10\x07\x12\r\n\tTYPE_BOOL\x10\x08\x12\x0f\n\x0bTYPE_STRING\x10\t\x12\x0e\n\nTYPE_GROUP\x10\n\x12\x10\n\x0cTYPE_MESSAGE\x10\x0b\x12\x0e\n\nTYPE_BYTES\x10\x0c\x12\x0f\n\x0bTYPE_UINT32\x10\r\x12\r\n\tTYPE_ENUM\x10\x0e\x12\x11\n\rTYPE_SFIXED32\x10\x0f\x12\x11\n\rTYPE_SFIXED64\x10\x10\x12\x0f\n\x0bTYPE_SINT32\x10\x11\x12\x0f\n\x0bTYPE_SINT64\x10\x12\"C\n\x05Label\x12\x12\n\x0eLABEL_OPTIONAL\x10\x01\x12\x12\n\x0eLABEL_REPEATED\x10\x03\x12\x12\n\x0eLABEL_REQUIRED\x10\x02\"c\n\x14OneofDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x37\n\x07options\x18\x02 \x01(\x0b\x32\x1d.google.protobuf.OneofOptionsR\x07options\"\xe3\x02\n\x13\x45numDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12?\n\x05value\x18\x02 \x03(\x0b\x32).google.protobuf.EnumValueDescriptorProtoR\x05value\x12\x36\n\x07options\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.EnumOptionsR\x07options\x12]\n\x0ereserved_range\x18\x04 \x03(\x0b\x32\x36.google.protobuf.EnumDescriptorProto.EnumReservedRangeR\rreservedRange\x12#\n\rreserved_name\x18\x05 \x03(\tR\x0creservedName\x1a;\n\x11\x45numReservedRange\x12\x14\n\x05start\x18\x01 \x01(\x05R\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\x05R\x03\x65nd\"\x83\x01\n\x18\x45numValueDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x16\n\x06number\x18\x02 \x01(\x05R\x06number\x12;\n\x07options\x18\x03 \x01(\x0b\x32!.google.protobuf.EnumValueOptionsR\x07options\"\xa7\x01\n\x16ServiceDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12>\n\x06method\x18\x02 \x03(\x0b\x32&.google.protobuf.MethodDescriptorProtoR\x06method\x12\x39\n\x07options\x18\x03 \x01(\x0b\x32\x1f.google.protobuf.ServiceOptionsR\x07options\"\x89\x02\n\x15MethodDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x1d\n\ninput_type\x18\x02 \x01(\tR\tinputType\x12\x1f\n\x0boutput_type\x18\x03 \x01(\tR\noutputType\x12\x38\n\x07options\x18\x04 \x01(\x0b\x32\x1e.google.protobuf.MethodOptionsR\x07options\x12\x30\n\x10\x63lient_streaming\x18\x05 \x01(\x08:\x05\x66\x61lseR\x0f\x63lientStreaming\x12\x30\n\x10server_streaming\x18\x06 \x01(\x08:\x05\x66\x61lseR\x0fserverStreaming\"\x97\t\n\x0b\x46ileOptions\x12!\n\x0cjava_package\x18\x01 \x01(\tR\x0bjavaPackage\x12\x30\n\x14java_outer_classname\x18\x08 \x01(\tR\x12javaOuterClassname\x12\x35\n\x13java_multiple_files\x18\n \x01(\x08:\x05\x66\x61lseR\x11javaMultipleFiles\x12\x44\n\x1djava_generate_equals_and_hash\x18\x14 \x01(\x08\x42\x02\x18\x01R\x19javaGenerateEqualsAndHash\x12:\n\x16java_string_check_utf8\x18\x1b \x01(\x08:\x05\x66\x61lseR\x13javaStringCheckUtf8\x12S\n\x0coptimize_for\x18\t \x01(\x0e\x32).google.protobuf.FileOptions.OptimizeMode:\x05SPEEDR\x0boptimizeFor\x12\x1d\n\ngo_package\x18\x0b \x01(\tR\tgoPackage\x12\x35\n\x13\x63\x63_generic_services\x18\x10 \x01(\x08:\x05\x66\x61lseR\x11\x63\x63GenericServices\x12\x39\n\x15java_generic_services\x18\x11 \x01(\x08:\x05\x66\x61lseR\x13javaGenericServices\x12\x35\n\x13py_generic_services\x18\x12 \x01(\x08:\x05\x66\x61lseR\x11pyGenericServices\x12%\n\ndeprecated\x18\x17 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12.\n\x10\x63\x63_enable_arenas\x18\x1f \x01(\x08:\x04trueR\x0e\x63\x63\x45nableArenas\x12*\n\x11objc_class_prefix\x18$ \x01(\tR\x0fobjcClassPrefix\x12)\n\x10\x63sharp_namespace\x18% \x01(\tR\x0f\x63sharpNamespace\x12!\n\x0cswift_prefix\x18\' \x01(\tR\x0bswiftPrefix\x12(\n\x10php_class_prefix\x18( \x01(\tR\x0ephpClassPrefix\x12#\n\rphp_namespace\x18) \x01(\tR\x0cphpNamespace\x12\x34\n\x16php_metadata_namespace\x18, \x01(\tR\x14phpMetadataNamespace\x12!\n\x0cruby_package\x18- \x01(\tR\x0brubyPackage\x12\x37\n\x08\x66\x65\x61tures\x18\x32 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\":\n\x0cOptimizeMode\x12\t\n\x05SPEED\x10\x01\x12\r\n\tCODE_SIZE\x10\x02\x12\x10\n\x0cLITE_RUNTIME\x10\x03*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08*\x10+J\x04\x08&\x10\'\"\xf4\x03\n\x0eMessageOptions\x12<\n\x17message_set_wire_format\x18\x01 \x01(\x08:\x05\x66\x61lseR\x14messageSetWireFormat\x12L\n\x1fno_standard_descriptor_accessor\x18\x02 \x01(\x08:\x05\x66\x61lseR\x1cnoStandardDescriptorAccessor\x12%\n\ndeprecated\x18\x03 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12\x1b\n\tmap_entry\x18\x07 \x01(\x08R\x08mapEntry\x12V\n&deprecated_legacy_json_field_conflicts\x18\x0b \x01(\x08\x42\x02\x18\x01R\"deprecatedLegacyJsonFieldConflicts\x12\x37\n\x08\x66\x65\x61tures\x18\x0c \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07J\x04\x08\x08\x10\tJ\x04\x08\t\x10\n\"\x9d\r\n\x0c\x46ieldOptions\x12\x41\n\x05\x63type\x18\x01 \x01(\x0e\x32#.google.protobuf.FieldOptions.CType:\x06STRINGR\x05\x63type\x12\x16\n\x06packed\x18\x02 \x01(\x08R\x06packed\x12G\n\x06jstype\x18\x06 \x01(\x0e\x32$.google.protobuf.FieldOptions.JSType:\tJS_NORMALR\x06jstype\x12\x19\n\x04lazy\x18\x05 \x01(\x08:\x05\x66\x61lseR\x04lazy\x12.\n\x0funverified_lazy\x18\x0f \x01(\x08:\x05\x66\x61lseR\x0eunverifiedLazy\x12%\n\ndeprecated\x18\x03 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12\x19\n\x04weak\x18\n \x01(\x08:\x05\x66\x61lseR\x04weak\x12(\n\x0c\x64\x65\x62ug_redact\x18\x10 \x01(\x08:\x05\x66\x61lseR\x0b\x64\x65\x62ugRedact\x12K\n\tretention\x18\x11 \x01(\x0e\x32-.google.protobuf.FieldOptions.OptionRetentionR\tretention\x12H\n\x07targets\x18\x13 \x03(\x0e\x32..google.protobuf.FieldOptions.OptionTargetTypeR\x07targets\x12W\n\x10\x65\x64ition_defaults\x18\x14 \x03(\x0b\x32,.google.protobuf.FieldOptions.EditionDefaultR\x0f\x65\x64itionDefaults\x12\x37\n\x08\x66\x65\x61tures\x18\x15 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12U\n\x0f\x66\x65\x61ture_support\x18\x16 \x01(\x0b\x32,.google.protobuf.FieldOptions.FeatureSupportR\x0e\x66\x65\x61tureSupport\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\x1aZ\n\x0e\x45\x64itionDefault\x12\x32\n\x07\x65\x64ition\x18\x03 \x01(\x0e\x32\x18.google.protobuf.EditionR\x07\x65\x64ition\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value\x1a\x96\x02\n\x0e\x46\x65\x61tureSupport\x12G\n\x12\x65\x64ition_introduced\x18\x01 \x01(\x0e\x32\x18.google.protobuf.EditionR\x11\x65\x64itionIntroduced\x12G\n\x12\x65\x64ition_deprecated\x18\x02 \x01(\x0e\x32\x18.google.protobuf.EditionR\x11\x65\x64itionDeprecated\x12/\n\x13\x64\x65precation_warning\x18\x03 \x01(\tR\x12\x64\x65precationWarning\x12\x41\n\x0f\x65\x64ition_removed\x18\x04 \x01(\x0e\x32\x18.google.protobuf.EditionR\x0e\x65\x64itionRemoved\"/\n\x05\x43Type\x12\n\n\x06STRING\x10\x00\x12\x08\n\x04\x43ORD\x10\x01\x12\x10\n\x0cSTRING_PIECE\x10\x02\"5\n\x06JSType\x12\r\n\tJS_NORMAL\x10\x00\x12\r\n\tJS_STRING\x10\x01\x12\r\n\tJS_NUMBER\x10\x02\"U\n\x0fOptionRetention\x12\x15\n\x11RETENTION_UNKNOWN\x10\x00\x12\x15\n\x11RETENTION_RUNTIME\x10\x01\x12\x14\n\x10RETENTION_SOURCE\x10\x02\"\x8c\x02\n\x10OptionTargetType\x12\x17\n\x13TARGET_TYPE_UNKNOWN\x10\x00\x12\x14\n\x10TARGET_TYPE_FILE\x10\x01\x12\x1f\n\x1bTARGET_TYPE_EXTENSION_RANGE\x10\x02\x12\x17\n\x13TARGET_TYPE_MESSAGE\x10\x03\x12\x15\n\x11TARGET_TYPE_FIELD\x10\x04\x12\x15\n\x11TARGET_TYPE_ONEOF\x10\x05\x12\x14\n\x10TARGET_TYPE_ENUM\x10\x06\x12\x1a\n\x16TARGET_TYPE_ENUM_ENTRY\x10\x07\x12\x17\n\x13TARGET_TYPE_SERVICE\x10\x08\x12\x16\n\x12TARGET_TYPE_METHOD\x10\t*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08\x04\x10\x05J\x04\x08\x12\x10\x13\"\xac\x01\n\x0cOneofOptions\x12\x37\n\x08\x66\x65\x61tures\x18\x01 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\xd1\x02\n\x0b\x45numOptions\x12\x1f\n\x0b\x61llow_alias\x18\x02 \x01(\x08R\nallowAlias\x12%\n\ndeprecated\x18\x03 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12V\n&deprecated_legacy_json_field_conflicts\x18\x06 \x01(\x08\x42\x02\x18\x01R\"deprecatedLegacyJsonFieldConflicts\x12\x37\n\x08\x66\x65\x61tures\x18\x07 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08\x05\x10\x06\"\x81\x02\n\x10\x45numValueOptions\x12%\n\ndeprecated\x18\x01 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12\x37\n\x08\x66\x65\x61tures\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12(\n\x0c\x64\x65\x62ug_redact\x18\x03 \x01(\x08:\x05\x66\x61lseR\x0b\x64\x65\x62ugRedact\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\xd5\x01\n\x0eServiceOptions\x12\x37\n\x08\x66\x65\x61tures\x18\" \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12%\n\ndeprecated\x18! \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\x99\x03\n\rMethodOptions\x12%\n\ndeprecated\x18! \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12q\n\x11idempotency_level\x18\" \x01(\x0e\x32/.google.protobuf.MethodOptions.IdempotencyLevel:\x13IDEMPOTENCY_UNKNOWNR\x10idempotencyLevel\x12\x37\n\x08\x66\x65\x61tures\x18# \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\"P\n\x10IdempotencyLevel\x12\x17\n\x13IDEMPOTENCY_UNKNOWN\x10\x00\x12\x13\n\x0fNO_SIDE_EFFECTS\x10\x01\x12\x0e\n\nIDEMPOTENT\x10\x02*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\x9a\x03\n\x13UninterpretedOption\x12\x41\n\x04name\x18\x02 \x03(\x0b\x32-.google.protobuf.UninterpretedOption.NamePartR\x04name\x12)\n\x10identifier_value\x18\x03 \x01(\tR\x0fidentifierValue\x12,\n\x12positive_int_value\x18\x04 \x01(\x04R\x10positiveIntValue\x12,\n\x12negative_int_value\x18\x05 \x01(\x03R\x10negativeIntValue\x12!\n\x0c\x64ouble_value\x18\x06 \x01(\x01R\x0b\x64oubleValue\x12!\n\x0cstring_value\x18\x07 \x01(\x0cR\x0bstringValue\x12\'\n\x0f\x61ggregate_value\x18\x08 \x01(\tR\x0e\x61ggregateValue\x1aJ\n\x08NamePart\x12\x1b\n\tname_part\x18\x01 \x02(\tR\x08namePart\x12!\n\x0cis_extension\x18\x02 \x02(\x08R\x0bisExtension\"\xb9\n\n\nFeatureSet\x12\x91\x01\n\x0e\x66ield_presence\x18\x01 \x01(\x0e\x32).google.protobuf.FeatureSet.FieldPresenceB?\x88\x01\x01\x98\x01\x04\x98\x01\x01\xa2\x01\r\x12\x08\x45XPLICIT\x18\xe6\x07\xa2\x01\r\x12\x08IMPLICIT\x18\xe7\x07\xa2\x01\r\x12\x08\x45XPLICIT\x18\xe8\x07\xb2\x01\x03\x08\xe8\x07R\rfieldPresence\x12l\n\tenum_type\x18\x02 \x01(\x0e\x32$.google.protobuf.FeatureSet.EnumTypeB)\x88\x01\x01\x98\x01\x06\x98\x01\x01\xa2\x01\x0b\x12\x06\x43LOSED\x18\xe6\x07\xa2\x01\t\x12\x04OPEN\x18\xe7\x07\xb2\x01\x03\x08\xe8\x07R\x08\x65numType\x12\x98\x01\n\x17repeated_field_encoding\x18\x03 \x01(\x0e\x32\x31.google.protobuf.FeatureSet.RepeatedFieldEncodingB-\x88\x01\x01\x98\x01\x04\x98\x01\x01\xa2\x01\r\x12\x08\x45XPANDED\x18\xe6\x07\xa2\x01\x0b\x12\x06PACKED\x18\xe7\x07\xb2\x01\x03\x08\xe8\x07R\x15repeatedFieldEncoding\x12~\n\x0futf8_validation\x18\x04 \x01(\x0e\x32*.google.protobuf.FeatureSet.Utf8ValidationB)\x88\x01\x01\x98\x01\x04\x98\x01\x01\xa2\x01\t\x12\x04NONE\x18\xe6\x07\xa2\x01\x0b\x12\x06VERIFY\x18\xe7\x07\xb2\x01\x03\x08\xe8\x07R\x0eutf8Validation\x12~\n\x10message_encoding\x18\x05 \x01(\x0e\x32+.google.protobuf.FeatureSet.MessageEncodingB&\x88\x01\x01\x98\x01\x04\x98\x01\x01\xa2\x01\x14\x12\x0fLENGTH_PREFIXED\x18\xe6\x07\xb2\x01\x03\x08\xe8\x07R\x0fmessageEncoding\x12\x82\x01\n\x0bjson_format\x18\x06 \x01(\x0e\x32&.google.protobuf.FeatureSet.JsonFormatB9\x88\x01\x01\x98\x01\x03\x98\x01\x06\x98\x01\x01\xa2\x01\x17\x12\x12LEGACY_BEST_EFFORT\x18\xe6\x07\xa2\x01\n\x12\x05\x41LLOW\x18\xe7\x07\xb2\x01\x03\x08\xe8\x07R\njsonFormat\"\\\n\rFieldPresence\x12\x1a\n\x16\x46IELD_PRESENCE_UNKNOWN\x10\x00\x12\x0c\n\x08\x45XPLICIT\x10\x01\x12\x0c\n\x08IMPLICIT\x10\x02\x12\x13\n\x0fLEGACY_REQUIRED\x10\x03\"7\n\x08\x45numType\x12\x15\n\x11\x45NUM_TYPE_UNKNOWN\x10\x00\x12\x08\n\x04OPEN\x10\x01\x12\n\n\x06\x43LOSED\x10\x02\"V\n\x15RepeatedFieldEncoding\x12#\n\x1fREPEATED_FIELD_ENCODING_UNKNOWN\x10\x00\x12\n\n\x06PACKED\x10\x01\x12\x0c\n\x08\x45XPANDED\x10\x02\"C\n\x0eUtf8Validation\x12\x1b\n\x17UTF8_VALIDATION_UNKNOWN\x10\x00\x12\n\n\x06VERIFY\x10\x02\x12\x08\n\x04NONE\x10\x03\"S\n\x0fMessageEncoding\x12\x1c\n\x18MESSAGE_ENCODING_UNKNOWN\x10\x00\x12\x13\n\x0fLENGTH_PREFIXED\x10\x01\x12\r\n\tDELIMITED\x10\x02\"H\n\nJsonFormat\x12\x17\n\x13JSON_FORMAT_UNKNOWN\x10\x00\x12\t\n\x05\x41LLOW\x10\x01\x12\x16\n\x12LEGACY_BEST_EFFORT\x10\x02*\x06\x08\xe8\x07\x10\xe9\x07*\x06\x08\xe9\x07\x10\xea\x07*\x06\x08\xea\x07\x10\xeb\x07*\x06\x08\x86N\x10\x87N*\x06\x08\x8bN\x10\x90N*\x06\x08\x90N\x10\x91NJ\x06\x08\xe7\x07\x10\xe8\x07\"\xd9\x03\n\x12\x46\x65\x61tureSetDefaults\x12X\n\x08\x64\x65\x66\x61ults\x18\x01 \x03(\x0b\x32<.google.protobuf.FeatureSetDefaults.FeatureSetEditionDefaultR\x08\x64\x65\x66\x61ults\x12\x41\n\x0fminimum_edition\x18\x04 \x01(\x0e\x32\x18.google.protobuf.EditionR\x0eminimumEdition\x12\x41\n\x0fmaximum_edition\x18\x05 \x01(\x0e\x32\x18.google.protobuf.EditionR\x0emaximumEdition\x1a\xe2\x01\n\x18\x46\x65\x61tureSetEditionDefault\x12\x32\n\x07\x65\x64ition\x18\x03 \x01(\x0e\x32\x18.google.protobuf.EditionR\x07\x65\x64ition\x12N\n\x14overridable_features\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x13overridableFeatures\x12\x42\n\x0e\x66ixed_features\x18\x05 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\rfixedFeatures\"\xa7\x02\n\x0eSourceCodeInfo\x12\x44\n\x08location\x18\x01 \x03(\x0b\x32(.google.protobuf.SourceCodeInfo.LocationR\x08location\x1a\xce\x01\n\x08Location\x12\x16\n\x04path\x18\x01 \x03(\x05\x42\x02\x10\x01R\x04path\x12\x16\n\x04span\x18\x02 \x03(\x05\x42\x02\x10\x01R\x04span\x12)\n\x10leading_comments\x18\x03 \x01(\tR\x0fleadingComments\x12+\n\x11trailing_comments\x18\x04 \x01(\tR\x10trailingComments\x12:\n\x19leading_detached_comments\x18\x06 \x03(\tR\x17leadingDetachedComments\"\xd0\x02\n\x11GeneratedCodeInfo\x12M\n\nannotation\x18\x01 \x03(\x0b\x32-.google.protobuf.GeneratedCodeInfo.AnnotationR\nannotation\x1a\xeb\x01\n\nAnnotation\x12\x16\n\x04path\x18\x01 \x03(\x05\x42\x02\x10\x01R\x04path\x12\x1f\n\x0bsource_file\x18\x02 \x01(\tR\nsourceFile\x12\x14\n\x05\x62\x65gin\x18\x03 \x01(\x05R\x05\x62\x65gin\x12\x10\n\x03\x65nd\x18\x04 \x01(\x05R\x03\x65nd\x12R\n\x08semantic\x18\x05 \x01(\x0e\x32\x36.google.protobuf.GeneratedCodeInfo.Annotation.SemanticR\x08semantic\"(\n\x08Semantic\x12\x08\n\x04NONE\x10\x00\x12\x07\n\x03SET\x10\x01\x12\t\n\x05\x41LIAS\x10\x02*\xa7\x02\n\x07\x45\x64ition\x12\x13\n\x0f\x45\x44ITION_UNKNOWN\x10\x00\x12\x13\n\x0e\x45\x44ITION_LEGACY\x10\x84\x07\x12\x13\n\x0e\x45\x44ITION_PROTO2\x10\xe6\x07\x12\x13\n\x0e\x45\x44ITION_PROTO3\x10\xe7\x07\x12\x11\n\x0c\x45\x44ITION_2023\x10\xe8\x07\x12\x11\n\x0c\x45\x44ITION_2024\x10\xe9\x07\x12\x17\n\x13\x45\x44ITION_1_TEST_ONLY\x10\x01\x12\x17\n\x13\x45\x44ITION_2_TEST_ONLY\x10\x02\x12\x1d\n\x17\x45\x44ITION_99997_TEST_ONLY\x10\x9d\x8d\x06\x12\x1d\n\x17\x45\x44ITION_99998_TEST_ONLY\x10\x9e\x8d\x06\x12\x1d\n\x17\x45\x44ITION_99999_TEST_ONLY\x10\x9f\x8d\x06\x12\x13\n\x0b\x45\x44ITION_MAX\x10\xff\xff\xff\xff\x07\x42~\n\x13\x63om.google.protobufB\x10\x44\x65scriptorProtosH\x01Z-google.golang.org/protobuf/types/descriptorpb\xf8\x01\x01\xa2\x02\x03GPB\xaa\x02\x1aGoogle.Protobuf.Reflection')
 
 _globals = globals()
 if not _descriptor._USE_C_DESCRIPTORS:
   _EDITION = _descriptor.EnumDescriptor(
     name='Edition',
     full_name='google.protobuf.Edition',
     filename=None,
@@ -38,60 +48,65 @@
     values=[
       _descriptor.EnumValueDescriptor(
         name='EDITION_UNKNOWN', index=0, number=0,
         serialized_options=None,
         type=None,
         create_key=_descriptor._internal_create_key),
       _descriptor.EnumValueDescriptor(
-        name='EDITION_PROTO2', index=1, number=998,
+        name='EDITION_LEGACY', index=1, number=900,
         serialized_options=None,
         type=None,
         create_key=_descriptor._internal_create_key),
       _descriptor.EnumValueDescriptor(
-        name='EDITION_PROTO3', index=2, number=999,
+        name='EDITION_PROTO2', index=2, number=998,
         serialized_options=None,
         type=None,
         create_key=_descriptor._internal_create_key),
       _descriptor.EnumValueDescriptor(
-        name='EDITION_2023', index=3, number=1000,
+        name='EDITION_PROTO3', index=3, number=999,
         serialized_options=None,
         type=None,
         create_key=_descriptor._internal_create_key),
       _descriptor.EnumValueDescriptor(
-        name='EDITION_2024', index=4, number=1001,
+        name='EDITION_2023', index=4, number=1000,
         serialized_options=None,
         type=None,
         create_key=_descriptor._internal_create_key),
       _descriptor.EnumValueDescriptor(
-        name='EDITION_1_TEST_ONLY', index=5, number=1,
+        name='EDITION_2024', index=5, number=1001,
         serialized_options=None,
         type=None,
         create_key=_descriptor._internal_create_key),
       _descriptor.EnumValueDescriptor(
-        name='EDITION_2_TEST_ONLY', index=6, number=2,
+        name='EDITION_1_TEST_ONLY', index=6, number=1,
         serialized_options=None,
         type=None,
         create_key=_descriptor._internal_create_key),
       _descriptor.EnumValueDescriptor(
-        name='EDITION_99997_TEST_ONLY', index=7, number=99997,
+        name='EDITION_2_TEST_ONLY', index=7, number=2,
         serialized_options=None,
         type=None,
         create_key=_descriptor._internal_create_key),
       _descriptor.EnumValueDescriptor(
-        name='EDITION_99998_TEST_ONLY', index=8, number=99998,
+        name='EDITION_99997_TEST_ONLY', index=8, number=99997,
         serialized_options=None,
         type=None,
         create_key=_descriptor._internal_create_key),
       _descriptor.EnumValueDescriptor(
-        name='EDITION_99999_TEST_ONLY', index=9, number=99999,
+        name='EDITION_99998_TEST_ONLY', index=9, number=99998,
         serialized_options=None,
         type=None,
         create_key=_descriptor._internal_create_key),
       _descriptor.EnumValueDescriptor(
-        name='EDITION_MAX', index=10, number=2147483647,
+        name='EDITION_99999_TEST_ONLY', index=10, number=99999,
+        serialized_options=None,
+        type=None,
+        create_key=_descriptor._internal_create_key),
+      _descriptor.EnumValueDescriptor(
+        name='EDITION_MAX', index=11, number=2147483647,
         serialized_options=None,
         type=None,
         create_key=_descriptor._internal_create_key),
     ],
     containing_type=None,
     serialized_options=None,
   )
@@ -1725,14 +1740,63 @@
     serialized_options=None,
     is_extendable=False,
     extension_ranges=[],
     oneofs=[
     ],
   )
 
+  _FIELDOPTIONS_FEATURESUPPORT = _descriptor.Descriptor(
+    name='FeatureSupport',
+    full_name='google.protobuf.FieldOptions.FeatureSupport',
+    filename=None,
+    file=DESCRIPTOR,
+    containing_type=None,
+    create_key=_descriptor._internal_create_key,
+    fields=[
+      _descriptor.FieldDescriptor(
+        name='edition_introduced', full_name='google.protobuf.FieldOptions.FeatureSupport.edition_introduced', index=0,
+        number=1, type=14, cpp_type=8, label=1,
+        has_default_value=False, default_value=0,
+        message_type=None, enum_type=None, containing_type=None,
+        is_extension=False, extension_scope=None,
+        serialized_options=None, json_name='editionIntroduced', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+      _descriptor.FieldDescriptor(
+        name='edition_deprecated', full_name='google.protobuf.FieldOptions.FeatureSupport.edition_deprecated', index=1,
+        number=2, type=14, cpp_type=8, label=1,
+        has_default_value=False, default_value=0,
+        message_type=None, enum_type=None, containing_type=None,
+        is_extension=False, extension_scope=None,
+        serialized_options=None, json_name='editionDeprecated', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+      _descriptor.FieldDescriptor(
+        name='deprecation_warning', full_name='google.protobuf.FieldOptions.FeatureSupport.deprecation_warning', index=2,
+        number=3, type=9, cpp_type=9, label=1,
+        has_default_value=False, default_value=b"".decode('utf-8'),
+        message_type=None, enum_type=None, containing_type=None,
+        is_extension=False, extension_scope=None,
+        serialized_options=None, json_name='deprecationWarning', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+      _descriptor.FieldDescriptor(
+        name='edition_removed', full_name='google.protobuf.FieldOptions.FeatureSupport.edition_removed', index=3,
+        number=4, type=14, cpp_type=8, label=1,
+        has_default_value=False, default_value=0,
+        message_type=None, enum_type=None, containing_type=None,
+        is_extension=False, extension_scope=None,
+        serialized_options=None, json_name='editionRemoved', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    ],
+    extensions=[
+    ],
+    nested_types=[],
+    enum_types=[
+    ],
+    serialized_options=None,
+    is_extendable=False,
+    extension_ranges=[],
+    oneofs=[
+    ],
+  )
+
   _FIELDOPTIONS = _descriptor.Descriptor(
     name='FieldOptions',
     full_name='google.protobuf.FieldOptions',
     filename=None,
     file=DESCRIPTOR,
     containing_type=None,
     create_key=_descriptor._internal_create_key,
@@ -1818,24 +1882,31 @@
         name='features', full_name='google.protobuf.FieldOptions.features', index=11,
         number=21, type=11, cpp_type=10, label=1,
         has_default_value=False, default_value=None,
         message_type=None, enum_type=None, containing_type=None,
         is_extension=False, extension_scope=None,
         serialized_options=None, json_name='features', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
       _descriptor.FieldDescriptor(
-        name='uninterpreted_option', full_name='google.protobuf.FieldOptions.uninterpreted_option', index=12,
+        name='feature_support', full_name='google.protobuf.FieldOptions.feature_support', index=12,
+        number=22, type=11, cpp_type=10, label=1,
+        has_default_value=False, default_value=None,
+        message_type=None, enum_type=None, containing_type=None,
+        is_extension=False, extension_scope=None,
+        serialized_options=None, json_name='featureSupport', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+      _descriptor.FieldDescriptor(
+        name='uninterpreted_option', full_name='google.protobuf.FieldOptions.uninterpreted_option', index=13,
         number=999, type=11, cpp_type=10, label=3,
         has_default_value=False, default_value=[],
         message_type=None, enum_type=None, containing_type=None,
         is_extension=False, extension_scope=None,
         serialized_options=None, json_name='uninterpretedOption', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     ],
     extensions=[
     ],
-    nested_types=[_FIELDOPTIONS_EDITIONDEFAULT, ],
+    nested_types=[_FIELDOPTIONS_EDITIONDEFAULT, _FIELDOPTIONS_FEATURESUPPORT, ],
     enum_types=[
       _FIELDOPTIONS_CTYPE,
       _FIELDOPTIONS_JSTYPE,
       _FIELDOPTIONS_OPTIONRETENTION,
       _FIELDOPTIONS_OPTIONTARGETTYPE,
     ],
     serialized_options=None,
@@ -2199,65 +2270,65 @@
     fields=[
       _descriptor.FieldDescriptor(
         name='field_presence', full_name='google.protobuf.FeatureSet.field_presence', index=0,
         number=1, type=14, cpp_type=8, label=1,
         has_default_value=False, default_value=0,
         message_type=None, enum_type=None, containing_type=None,
         is_extension=False, extension_scope=None,
-        serialized_options=b'\210\001\001\230\001\004\230\001\001\242\001\r\022\010EXPLICIT\030\346\007\242\001\r\022\010IMPLICIT\030\347\007\242\001\r\022\010EXPLICIT\030\350\007', json_name='fieldPresence', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+        serialized_options=b'\210\001\001\230\001\004\230\001\001\242\001\r\022\010EXPLICIT\030\346\007\242\001\r\022\010IMPLICIT\030\347\007\242\001\r\022\010EXPLICIT\030\350\007\262\001\003\010\350\007', json_name='fieldPresence', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
       _descriptor.FieldDescriptor(
         name='enum_type', full_name='google.protobuf.FeatureSet.enum_type', index=1,
         number=2, type=14, cpp_type=8, label=1,
         has_default_value=False, default_value=0,
         message_type=None, enum_type=None, containing_type=None,
         is_extension=False, extension_scope=None,
-        serialized_options=b'\210\001\001\230\001\006\230\001\001\242\001\013\022\006CLOSED\030\346\007\242\001\t\022\004OPEN\030\347\007', json_name='enumType', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+        serialized_options=b'\210\001\001\230\001\006\230\001\001\242\001\013\022\006CLOSED\030\346\007\242\001\t\022\004OPEN\030\347\007\262\001\003\010\350\007', json_name='enumType', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
       _descriptor.FieldDescriptor(
         name='repeated_field_encoding', full_name='google.protobuf.FeatureSet.repeated_field_encoding', index=2,
         number=3, type=14, cpp_type=8, label=1,
         has_default_value=False, default_value=0,
         message_type=None, enum_type=None, containing_type=None,
         is_extension=False, extension_scope=None,
-        serialized_options=b'\210\001\001\230\001\004\230\001\001\242\001\r\022\010EXPANDED\030\346\007\242\001\013\022\006PACKED\030\347\007', json_name='repeatedFieldEncoding', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+        serialized_options=b'\210\001\001\230\001\004\230\001\001\242\001\r\022\010EXPANDED\030\346\007\242\001\013\022\006PACKED\030\347\007\262\001\003\010\350\007', json_name='repeatedFieldEncoding', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
       _descriptor.FieldDescriptor(
         name='utf8_validation', full_name='google.protobuf.FeatureSet.utf8_validation', index=3,
         number=4, type=14, cpp_type=8, label=1,
         has_default_value=False, default_value=0,
         message_type=None, enum_type=None, containing_type=None,
         is_extension=False, extension_scope=None,
-        serialized_options=b'\210\001\001\230\001\004\230\001\001\242\001\t\022\004NONE\030\346\007\242\001\013\022\006VERIFY\030\347\007', json_name='utf8Validation', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+        serialized_options=b'\210\001\001\230\001\004\230\001\001\242\001\t\022\004NONE\030\346\007\242\001\013\022\006VERIFY\030\347\007\262\001\003\010\350\007', json_name='utf8Validation', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
       _descriptor.FieldDescriptor(
         name='message_encoding', full_name='google.protobuf.FeatureSet.message_encoding', index=4,
         number=5, type=14, cpp_type=8, label=1,
         has_default_value=False, default_value=0,
         message_type=None, enum_type=None, containing_type=None,
         is_extension=False, extension_scope=None,
-        serialized_options=b'\210\001\001\230\001\004\230\001\001\242\001\024\022\017LENGTH_PREFIXED\030\346\007', json_name='messageEncoding', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+        serialized_options=b'\210\001\001\230\001\004\230\001\001\242\001\024\022\017LENGTH_PREFIXED\030\346\007\262\001\003\010\350\007', json_name='messageEncoding', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
       _descriptor.FieldDescriptor(
         name='json_format', full_name='google.protobuf.FeatureSet.json_format', index=5,
         number=6, type=14, cpp_type=8, label=1,
         has_default_value=False, default_value=0,
         message_type=None, enum_type=None, containing_type=None,
         is_extension=False, extension_scope=None,
-        serialized_options=b'\210\001\001\230\001\003\230\001\006\230\001\001\242\001\027\022\022LEGACY_BEST_EFFORT\030\346\007\242\001\n\022\005ALLOW\030\347\007', json_name='jsonFormat', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+        serialized_options=b'\210\001\001\230\001\003\230\001\006\230\001\001\242\001\027\022\022LEGACY_BEST_EFFORT\030\346\007\242\001\n\022\005ALLOW\030\347\007\262\001\003\010\350\007', json_name='jsonFormat', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     ],
     extensions=[
     ],
     nested_types=[],
     enum_types=[
       _FEATURESET_FIELDPRESENCE,
       _FEATURESET_ENUMTYPE,
       _FEATURESET_REPEATEDFIELDENCODING,
       _FEATURESET_UTF8VALIDATION,
       _FEATURESET_MESSAGEENCODING,
       _FEATURESET_JSONFORMAT,
     ],
     serialized_options=None,
     is_extendable=True,
-    extension_ranges=[(1000, 1001), (1001, 1002), (1002, 1003), (9995, 10000), (10000, 10001), ],
+    extension_ranges=[(1000, 1001), (1001, 1002), (1002, 1003), (9990, 9991), (9995, 10000), (10000, 10001), ],
     oneofs=[
     ],
   )
 
 
   _FEATURESETDEFAULTS_FEATURESETEDITIONDEFAULT = _descriptor.Descriptor(
     name='FeatureSetEditionDefault',
@@ -2271,20 +2342,27 @@
         name='edition', full_name='google.protobuf.FeatureSetDefaults.FeatureSetEditionDefault.edition', index=0,
         number=3, type=14, cpp_type=8, label=1,
         has_default_value=False, default_value=0,
         message_type=None, enum_type=None, containing_type=None,
         is_extension=False, extension_scope=None,
         serialized_options=None, json_name='edition', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
       _descriptor.FieldDescriptor(
-        name='features', full_name='google.protobuf.FeatureSetDefaults.FeatureSetEditionDefault.features', index=1,
-        number=2, type=11, cpp_type=10, label=1,
+        name='overridable_features', full_name='google.protobuf.FeatureSetDefaults.FeatureSetEditionDefault.overridable_features', index=1,
+        number=4, type=11, cpp_type=10, label=1,
         has_default_value=False, default_value=None,
         message_type=None, enum_type=None, containing_type=None,
         is_extension=False, extension_scope=None,
-        serialized_options=None, json_name='features', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+        serialized_options=None, json_name='overridableFeatures', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+      _descriptor.FieldDescriptor(
+        name='fixed_features', full_name='google.protobuf.FeatureSetDefaults.FeatureSetEditionDefault.fixed_features', index=2,
+        number=5, type=11, cpp_type=10, label=1,
+        has_default_value=False, default_value=None,
+        message_type=None, enum_type=None, containing_type=None,
+        is_extension=False, extension_scope=None,
+        serialized_options=None, json_name='fixedFeatures', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     ],
     extensions=[
     ],
     nested_types=[],
     enum_types=[
     ],
     serialized_options=None,
@@ -2550,20 +2628,25 @@
   _FILEOPTIONS.fields_by_name['features'].message_type = _FEATURESET
   _FILEOPTIONS.fields_by_name['uninterpreted_option'].message_type = _UNINTERPRETEDOPTION
   _FILEOPTIONS_OPTIMIZEMODE.containing_type = _FILEOPTIONS
   _MESSAGEOPTIONS.fields_by_name['features'].message_type = _FEATURESET
   _MESSAGEOPTIONS.fields_by_name['uninterpreted_option'].message_type = _UNINTERPRETEDOPTION
   _FIELDOPTIONS_EDITIONDEFAULT.fields_by_name['edition'].enum_type = _EDITION
   _FIELDOPTIONS_EDITIONDEFAULT.containing_type = _FIELDOPTIONS
+  _FIELDOPTIONS_FEATURESUPPORT.fields_by_name['edition_introduced'].enum_type = _EDITION
+  _FIELDOPTIONS_FEATURESUPPORT.fields_by_name['edition_deprecated'].enum_type = _EDITION
+  _FIELDOPTIONS_FEATURESUPPORT.fields_by_name['edition_removed'].enum_type = _EDITION
+  _FIELDOPTIONS_FEATURESUPPORT.containing_type = _FIELDOPTIONS
   _FIELDOPTIONS.fields_by_name['ctype'].enum_type = _FIELDOPTIONS_CTYPE
   _FIELDOPTIONS.fields_by_name['jstype'].enum_type = _FIELDOPTIONS_JSTYPE
   _FIELDOPTIONS.fields_by_name['retention'].enum_type = _FIELDOPTIONS_OPTIONRETENTION
   _FIELDOPTIONS.fields_by_name['targets'].enum_type = _FIELDOPTIONS_OPTIONTARGETTYPE
   _FIELDOPTIONS.fields_by_name['edition_defaults'].message_type = _FIELDOPTIONS_EDITIONDEFAULT
   _FIELDOPTIONS.fields_by_name['features'].message_type = _FEATURESET
+  _FIELDOPTIONS.fields_by_name['feature_support'].message_type = _FIELDOPTIONS_FEATURESUPPORT
   _FIELDOPTIONS.fields_by_name['uninterpreted_option'].message_type = _UNINTERPRETEDOPTION
   _FIELDOPTIONS_CTYPE.containing_type = _FIELDOPTIONS
   _FIELDOPTIONS_JSTYPE.containing_type = _FIELDOPTIONS
   _FIELDOPTIONS_OPTIONRETENTION.containing_type = _FIELDOPTIONS
   _FIELDOPTIONS_OPTIONTARGETTYPE.containing_type = _FIELDOPTIONS
   _ONEOFOPTIONS.fields_by_name['features'].message_type = _FEATURESET
   _ONEOFOPTIONS.fields_by_name['uninterpreted_option'].message_type = _UNINTERPRETEDOPTION
@@ -2588,15 +2671,16 @@
   _FEATURESET_FIELDPRESENCE.containing_type = _FEATURESET
   _FEATURESET_ENUMTYPE.containing_type = _FEATURESET
   _FEATURESET_REPEATEDFIELDENCODING.containing_type = _FEATURESET
   _FEATURESET_UTF8VALIDATION.containing_type = _FEATURESET
   _FEATURESET_MESSAGEENCODING.containing_type = _FEATURESET
   _FEATURESET_JSONFORMAT.containing_type = _FEATURESET
   _FEATURESETDEFAULTS_FEATURESETEDITIONDEFAULT.fields_by_name['edition'].enum_type = _EDITION
-  _FEATURESETDEFAULTS_FEATURESETEDITIONDEFAULT.fields_by_name['features'].message_type = _FEATURESET
+  _FEATURESETDEFAULTS_FEATURESETEDITIONDEFAULT.fields_by_name['overridable_features'].message_type = _FEATURESET
+  _FEATURESETDEFAULTS_FEATURESETEDITIONDEFAULT.fields_by_name['fixed_features'].message_type = _FEATURESET
   _FEATURESETDEFAULTS_FEATURESETEDITIONDEFAULT.containing_type = _FEATURESETDEFAULTS
   _FEATURESETDEFAULTS.fields_by_name['defaults'].message_type = _FEATURESETDEFAULTS_FEATURESETEDITIONDEFAULT
   _FEATURESETDEFAULTS.fields_by_name['minimum_edition'].enum_type = _EDITION
   _FEATURESETDEFAULTS.fields_by_name['maximum_edition'].enum_type = _EDITION
   _SOURCECODEINFO_LOCATION.containing_type = _SOURCECODEINFO
   _SOURCECODEINFO.fields_by_name['location'].message_type = _SOURCECODEINFO_LOCATION
   _GENERATEDCODEINFO_ANNOTATION.fields_by_name['semantic'].enum_type = _GENERATEDCODEINFO_ANNOTATION_SEMANTIC
@@ -2762,17 +2846,23 @@
   _FIELDOPTIONS.fields[6]._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
   _FIELDOPTIONS.fields[7]._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
   _FIELDOPTIONS.fields[8]._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
   _FIELDOPTIONS.fields[9]._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
   _FIELDOPTIONS.fields[10]._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
   _FIELDOPTIONS.fields[11]._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
   _FIELDOPTIONS.fields[12]._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
+  _FIELDOPTIONS.fields[13]._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
   _FIELDOPTIONS_EDITIONDEFAULT._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
   _FIELDOPTIONS_EDITIONDEFAULT.fields[0]._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
   _FIELDOPTIONS_EDITIONDEFAULT.fields[1]._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
+  _FIELDOPTIONS_FEATURESUPPORT._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
+  _FIELDOPTIONS_FEATURESUPPORT.fields[0]._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
+  _FIELDOPTIONS_FEATURESUPPORT.fields[1]._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
+  _FIELDOPTIONS_FEATURESUPPORT.fields[2]._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
+  _FIELDOPTIONS_FEATURESUPPORT.fields[3]._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
   _ONEOFOPTIONS._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
   _ONEOFOPTIONS.fields[0]._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
   _ONEOFOPTIONS.fields[1]._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
   _ENUMOPTIONS._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
   _ENUMOPTIONS.fields[0]._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
   _ENUMOPTIONS.fields[1]._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
   _ENUMOPTIONS.fields[2]._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
@@ -2813,14 +2903,15 @@
   _FEATURESETDEFAULTS._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
   _FEATURESETDEFAULTS.fields[0]._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
   _FEATURESETDEFAULTS.fields[1]._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
   _FEATURESETDEFAULTS.fields[2]._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
   _FEATURESETDEFAULTS_FEATURESETEDITIONDEFAULT._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
   _FEATURESETDEFAULTS_FEATURESETEDITIONDEFAULT.fields[0]._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
   _FEATURESETDEFAULTS_FEATURESETEDITIONDEFAULT.fields[1]._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
+  _FEATURESETDEFAULTS_FEATURESETEDITIONDEFAULT.fields[2]._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
   _SOURCECODEINFO._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
   _SOURCECODEINFO.fields[0]._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
   _SOURCECODEINFO_LOCATION._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
   _SOURCECODEINFO_LOCATION.fields[0]._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["PACKED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
   _SOURCECODEINFO_LOCATION.fields[1]._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["PACKED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
   _SOURCECODEINFO_LOCATION.fields[2]._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
   _SOURCECODEINFO_LOCATION.fields[3]._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
@@ -2927,14 +3018,15 @@
   _EDITION.values[4]._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
   _EDITION.values[5]._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
   _EDITION.values[6]._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
   _EDITION.values[7]._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
   _EDITION.values[8]._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
   _EDITION.values[9]._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
   _EDITION.values[10]._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
+  _EDITION.values[11]._features = _ResolvedFeatures(field_presence=_FEATURESET_FIELDPRESENCE.values_by_name["EXPLICIT"].number,enum_type=_FEATURESET_ENUMTYPE.values_by_name["CLOSED"].number,repeated_field_encoding=_FEATURESET_REPEATEDFIELDENCODING.values_by_name["EXPANDED"].number,utf8_validation=_FEATURESET_UTF8VALIDATION.values_by_name["NONE"].number,message_encoding=_FEATURESET_MESSAGEENCODING.values_by_name["LENGTH_PREFIXED"].number,json_format=_FEATURESET_JSONFORMAT.values_by_name["LEGACY_BEST_EFFORT"].number)
 else:
   _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'google.protobuf.descriptor_pb2', _globals)
 if not _descriptor._USE_C_DESCRIPTORS:
   _globals['DESCRIPTOR']._loaded_options = None
   _globals['DESCRIPTOR']._serialized_options = b'\n\023com.google.protobufB\020DescriptorProtosH\001Z-google.golang.org/protobuf/types/descriptorpb\370\001\001\242\002\003GPB\252\002\032Google.Protobuf.Reflection'
   _globals['_EXTENSIONRANGEOPTIONS'].fields_by_name['declaration']._loaded_options = None
@@ -2944,33 +3036,33 @@
   _globals['_FILEOPTIONS'].fields_by_name['java_generate_equals_and_hash']._loaded_options = None
   _globals['_FILEOPTIONS'].fields_by_name['java_generate_equals_and_hash']._serialized_options = b'\030\001'
   _globals['_MESSAGEOPTIONS'].fields_by_name['deprecated_legacy_json_field_conflicts']._loaded_options = None
   _globals['_MESSAGEOPTIONS'].fields_by_name['deprecated_legacy_json_field_conflicts']._serialized_options = b'\030\001'
   _globals['_ENUMOPTIONS'].fields_by_name['deprecated_legacy_json_field_conflicts']._loaded_options = None
   _globals['_ENUMOPTIONS'].fields_by_name['deprecated_legacy_json_field_conflicts']._serialized_options = b'\030\001'
   _globals['_FEATURESET'].fields_by_name['field_presence']._loaded_options = None
-  _globals['_FEATURESET'].fields_by_name['field_presence']._serialized_options = b'\210\001\001\230\001\004\230\001\001\242\001\r\022\010EXPLICIT\030\346\007\242\001\r\022\010IMPLICIT\030\347\007\242\001\r\022\010EXPLICIT\030\350\007'
+  _globals['_FEATURESET'].fields_by_name['field_presence']._serialized_options = b'\210\001\001\230\001\004\230\001\001\242\001\r\022\010EXPLICIT\030\346\007\242\001\r\022\010IMPLICIT\030\347\007\242\001\r\022\010EXPLICIT\030\350\007\262\001\003\010\350\007'
   _globals['_FEATURESET'].fields_by_name['enum_type']._loaded_options = None
-  _globals['_FEATURESET'].fields_by_name['enum_type']._serialized_options = b'\210\001\001\230\001\006\230\001\001\242\001\013\022\006CLOSED\030\346\007\242\001\t\022\004OPEN\030\347\007'
+  _globals['_FEATURESET'].fields_by_name['enum_type']._serialized_options = b'\210\001\001\230\001\006\230\001\001\242\001\013\022\006CLOSED\030\346\007\242\001\t\022\004OPEN\030\347\007\262\001\003\010\350\007'
   _globals['_FEATURESET'].fields_by_name['repeated_field_encoding']._loaded_options = None
-  _globals['_FEATURESET'].fields_by_name['repeated_field_encoding']._serialized_options = b'\210\001\001\230\001\004\230\001\001\242\001\r\022\010EXPANDED\030\346\007\242\001\013\022\006PACKED\030\347\007'
+  _globals['_FEATURESET'].fields_by_name['repeated_field_encoding']._serialized_options = b'\210\001\001\230\001\004\230\001\001\242\001\r\022\010EXPANDED\030\346\007\242\001\013\022\006PACKED\030\347\007\262\001\003\010\350\007'
   _globals['_FEATURESET'].fields_by_name['utf8_validation']._loaded_options = None
-  _globals['_FEATURESET'].fields_by_name['utf8_validation']._serialized_options = b'\210\001\001\230\001\004\230\001\001\242\001\t\022\004NONE\030\346\007\242\001\013\022\006VERIFY\030\347\007'
+  _globals['_FEATURESET'].fields_by_name['utf8_validation']._serialized_options = b'\210\001\001\230\001\004\230\001\001\242\001\t\022\004NONE\030\346\007\242\001\013\022\006VERIFY\030\347\007\262\001\003\010\350\007'
   _globals['_FEATURESET'].fields_by_name['message_encoding']._loaded_options = None
-  _globals['_FEATURESET'].fields_by_name['message_encoding']._serialized_options = b'\210\001\001\230\001\004\230\001\001\242\001\024\022\017LENGTH_PREFIXED\030\346\007'
+  _globals['_FEATURESET'].fields_by_name['message_encoding']._serialized_options = b'\210\001\001\230\001\004\230\001\001\242\001\024\022\017LENGTH_PREFIXED\030\346\007\262\001\003\010\350\007'
   _globals['_FEATURESET'].fields_by_name['json_format']._loaded_options = None
-  _globals['_FEATURESET'].fields_by_name['json_format']._serialized_options = b'\210\001\001\230\001\003\230\001\006\230\001\001\242\001\027\022\022LEGACY_BEST_EFFORT\030\346\007\242\001\n\022\005ALLOW\030\347\007'
+  _globals['_FEATURESET'].fields_by_name['json_format']._serialized_options = b'\210\001\001\230\001\003\230\001\006\230\001\001\242\001\027\022\022LEGACY_BEST_EFFORT\030\346\007\242\001\n\022\005ALLOW\030\347\007\262\001\003\010\350\007'
   _globals['_SOURCECODEINFO_LOCATION'].fields_by_name['path']._loaded_options = None
   _globals['_SOURCECODEINFO_LOCATION'].fields_by_name['path']._serialized_options = b'\020\001'
   _globals['_SOURCECODEINFO_LOCATION'].fields_by_name['span']._loaded_options = None
   _globals['_SOURCECODEINFO_LOCATION'].fields_by_name['span']._serialized_options = b'\020\001'
   _globals['_GENERATEDCODEINFO_ANNOTATION'].fields_by_name['path']._loaded_options = None
   _globals['_GENERATEDCODEINFO_ANNOTATION'].fields_by_name['path']._serialized_options = b'\020\001'
-  _globals['_EDITION']._serialized_start=11228
-  _globals['_EDITION']._serialized_end=11502
+  _globals['_EDITION']._serialized_start=11732
+  _globals['_EDITION']._serialized_end=12027
   _globals['_FILEDESCRIPTORSET']._serialized_start=53
   _globals['_FILEDESCRIPTORSET']._serialized_end=130
   _globals['_FILEDESCRIPTORPROTO']._serialized_start=133
   _globals['_FILEDESCRIPTORPROTO']._serialized_end=797
   _globals['_DESCRIPTORPROTO']._serialized_start=800
   _globals['_DESCRIPTORPROTO']._serialized_end=1625
   _globals['_DESCRIPTORPROTO_EXTENSIONRANGE']._serialized_start=1446
@@ -3004,63 +3096,65 @@
   _globals['_FILEOPTIONS']._serialized_start=4086
   _globals['_FILEOPTIONS']._serialized_end=5261
   _globals['_FILEOPTIONS_OPTIMIZEMODE']._serialized_start=5180
   _globals['_FILEOPTIONS_OPTIMIZEMODE']._serialized_end=5238
   _globals['_MESSAGEOPTIONS']._serialized_start=5264
   _globals['_MESSAGEOPTIONS']._serialized_end=5764
   _globals['_FIELDOPTIONS']._serialized_start=5767
-  _globals['_FIELDOPTIONS']._serialized_end=7092
-  _globals['_FIELDOPTIONS_EDITIONDEFAULT']._serialized_start=6517
-  _globals['_FIELDOPTIONS_EDITIONDEFAULT']._serialized_end=6607
-  _globals['_FIELDOPTIONS_CTYPE']._serialized_start=6609
-  _globals['_FIELDOPTIONS_CTYPE']._serialized_end=6656
-  _globals['_FIELDOPTIONS_JSTYPE']._serialized_start=6658
-  _globals['_FIELDOPTIONS_JSTYPE']._serialized_end=6711
-  _globals['_FIELDOPTIONS_OPTIONRETENTION']._serialized_start=6713
-  _globals['_FIELDOPTIONS_OPTIONRETENTION']._serialized_end=6798
-  _globals['_FIELDOPTIONS_OPTIONTARGETTYPE']._serialized_start=6801
-  _globals['_FIELDOPTIONS_OPTIONTARGETTYPE']._serialized_end=7069
-  _globals['_ONEOFOPTIONS']._serialized_start=7095
-  _globals['_ONEOFOPTIONS']._serialized_end=7267
-  _globals['_ENUMOPTIONS']._serialized_start=7270
-  _globals['_ENUMOPTIONS']._serialized_end=7607
-  _globals['_ENUMVALUEOPTIONS']._serialized_start=7610
-  _globals['_ENUMVALUEOPTIONS']._serialized_end=7867
-  _globals['_SERVICEOPTIONS']._serialized_start=7870
-  _globals['_SERVICEOPTIONS']._serialized_end=8083
-  _globals['_METHODOPTIONS']._serialized_start=8086
-  _globals['_METHODOPTIONS']._serialized_end=8495
-  _globals['_METHODOPTIONS_IDEMPOTENCYLEVEL']._serialized_start=8404
-  _globals['_METHODOPTIONS_IDEMPOTENCYLEVEL']._serialized_end=8484
-  _globals['_UNINTERPRETEDOPTION']._serialized_start=8498
-  _globals['_UNINTERPRETEDOPTION']._serialized_end=8908
-  _globals['_UNINTERPRETEDOPTION_NAMEPART']._serialized_start=8834
-  _globals['_UNINTERPRETEDOPTION_NAMEPART']._serialized_end=8908
-  _globals['_FEATURESET']._serialized_start=8911
-  _globals['_FEATURESET']._serialized_end=10203
-  _globals['_FEATURESET_FIELDPRESENCE']._serialized_start=9690
-  _globals['_FEATURESET_FIELDPRESENCE']._serialized_end=9782
-  _globals['_FEATURESET_ENUMTYPE']._serialized_start=9784
-  _globals['_FEATURESET_ENUMTYPE']._serialized_end=9839
-  _globals['_FEATURESET_REPEATEDFIELDENCODING']._serialized_start=9841
-  _globals['_FEATURESET_REPEATEDFIELDENCODING']._serialized_end=9927
-  _globals['_FEATURESET_UTF8VALIDATION']._serialized_start=9929
-  _globals['_FEATURESET_UTF8VALIDATION']._serialized_end=9996
-  _globals['_FEATURESET_MESSAGEENCODING']._serialized_start=9998
-  _globals['_FEATURESET_MESSAGEENCODING']._serialized_end=10081
-  _globals['_FEATURESET_JSONFORMAT']._serialized_start=10083
-  _globals['_FEATURESET_JSONFORMAT']._serialized_end=10155
-  _globals['_FEATURESETDEFAULTS']._serialized_start=10206
-  _globals['_FEATURESETDEFAULTS']._serialized_end=10588
-  _globals['_FEATURESETDEFAULTS_FEATURESETEDITIONDEFAULT']._serialized_start=10453
-  _globals['_FEATURESETDEFAULTS_FEATURESETEDITIONDEFAULT']._serialized_end=10588
-  _globals['_SOURCECODEINFO']._serialized_start=10591
-  _globals['_SOURCECODEINFO']._serialized_end=10886
-  _globals['_SOURCECODEINFO_LOCATION']._serialized_start=10680
-  _globals['_SOURCECODEINFO_LOCATION']._serialized_end=10886
-  _globals['_GENERATEDCODEINFO']._serialized_start=10889
-  _globals['_GENERATEDCODEINFO']._serialized_end=11225
-  _globals['_GENERATEDCODEINFO_ANNOTATION']._serialized_start=10990
-  _globals['_GENERATEDCODEINFO_ANNOTATION']._serialized_end=11225
-  _globals['_GENERATEDCODEINFO_ANNOTATION_SEMANTIC']._serialized_start=11185
-  _globals['_GENERATEDCODEINFO_ANNOTATION_SEMANTIC']._serialized_end=11225
+  _globals['_FIELDOPTIONS']._serialized_end=7460
+  _globals['_FIELDOPTIONS_EDITIONDEFAULT']._serialized_start=6604
+  _globals['_FIELDOPTIONS_EDITIONDEFAULT']._serialized_end=6694
+  _globals['_FIELDOPTIONS_FEATURESUPPORT']._serialized_start=6697
+  _globals['_FIELDOPTIONS_FEATURESUPPORT']._serialized_end=6975
+  _globals['_FIELDOPTIONS_CTYPE']._serialized_start=6977
+  _globals['_FIELDOPTIONS_CTYPE']._serialized_end=7024
+  _globals['_FIELDOPTIONS_JSTYPE']._serialized_start=7026
+  _globals['_FIELDOPTIONS_JSTYPE']._serialized_end=7079
+  _globals['_FIELDOPTIONS_OPTIONRETENTION']._serialized_start=7081
+  _globals['_FIELDOPTIONS_OPTIONRETENTION']._serialized_end=7166
+  _globals['_FIELDOPTIONS_OPTIONTARGETTYPE']._serialized_start=7169
+  _globals['_FIELDOPTIONS_OPTIONTARGETTYPE']._serialized_end=7437
+  _globals['_ONEOFOPTIONS']._serialized_start=7463
+  _globals['_ONEOFOPTIONS']._serialized_end=7635
+  _globals['_ENUMOPTIONS']._serialized_start=7638
+  _globals['_ENUMOPTIONS']._serialized_end=7975
+  _globals['_ENUMVALUEOPTIONS']._serialized_start=7978
+  _globals['_ENUMVALUEOPTIONS']._serialized_end=8235
+  _globals['_SERVICEOPTIONS']._serialized_start=8238
+  _globals['_SERVICEOPTIONS']._serialized_end=8451
+  _globals['_METHODOPTIONS']._serialized_start=8454
+  _globals['_METHODOPTIONS']._serialized_end=8863
+  _globals['_METHODOPTIONS_IDEMPOTENCYLEVEL']._serialized_start=8772
+  _globals['_METHODOPTIONS_IDEMPOTENCYLEVEL']._serialized_end=8852
+  _globals['_UNINTERPRETEDOPTION']._serialized_start=8866
+  _globals['_UNINTERPRETEDOPTION']._serialized_end=9276
+  _globals['_UNINTERPRETEDOPTION_NAMEPART']._serialized_start=9202
+  _globals['_UNINTERPRETEDOPTION_NAMEPART']._serialized_end=9276
+  _globals['_FEATURESET']._serialized_start=9279
+  _globals['_FEATURESET']._serialized_end=10616
+  _globals['_FEATURESET_FIELDPRESENCE']._serialized_start=10095
+  _globals['_FEATURESET_FIELDPRESENCE']._serialized_end=10187
+  _globals['_FEATURESET_ENUMTYPE']._serialized_start=10189
+  _globals['_FEATURESET_ENUMTYPE']._serialized_end=10244
+  _globals['_FEATURESET_REPEATEDFIELDENCODING']._serialized_start=10246
+  _globals['_FEATURESET_REPEATEDFIELDENCODING']._serialized_end=10332
+  _globals['_FEATURESET_UTF8VALIDATION']._serialized_start=10334
+  _globals['_FEATURESET_UTF8VALIDATION']._serialized_end=10401
+  _globals['_FEATURESET_MESSAGEENCODING']._serialized_start=10403
+  _globals['_FEATURESET_MESSAGEENCODING']._serialized_end=10486
+  _globals['_FEATURESET_JSONFORMAT']._serialized_start=10488
+  _globals['_FEATURESET_JSONFORMAT']._serialized_end=10560
+  _globals['_FEATURESETDEFAULTS']._serialized_start=10619
+  _globals['_FEATURESETDEFAULTS']._serialized_end=11092
+  _globals['_FEATURESETDEFAULTS_FEATURESETEDITIONDEFAULT']._serialized_start=10866
+  _globals['_FEATURESETDEFAULTS_FEATURESETEDITIONDEFAULT']._serialized_end=11092
+  _globals['_SOURCECODEINFO']._serialized_start=11095
+  _globals['_SOURCECODEINFO']._serialized_end=11390
+  _globals['_SOURCECODEINFO_LOCATION']._serialized_start=11184
+  _globals['_SOURCECODEINFO_LOCATION']._serialized_end=11390
+  _globals['_GENERATEDCODEINFO']._serialized_start=11393
+  _globals['_GENERATEDCODEINFO']._serialized_end=11729
+  _globals['_GENERATEDCODEINFO_ANNOTATION']._serialized_start=11494
+  _globals['_GENERATEDCODEINFO_ANNOTATION']._serialized_end=11729
+  _globals['_GENERATEDCODEINFO_ANNOTATION_SEMANTIC']._serialized_start=11689
+  _globals['_GENERATEDCODEINFO_ANNOTATION_SEMANTIC']._serialized_end=11729
 # @@protoc_insertion_point(module_scope)
```

### Comparing `protobuf-5.26.1/google/protobuf/descriptor_pool.py` & `protobuf-5.27.0rc1/google/protobuf/descriptor_pool.py`

 * *Files 0% similar despite different names*

```diff
@@ -733,23 +733,24 @@
               ),
           )
       )
     found = None
     for d in self._edition_defaults.defaults:
       if d.edition > edition:
         break
-      found = d.features
+      found = d
     if found is None:
       raise TypeError(
           'No valid default found for edition %s!'
           % descriptor_pb2.Edition.Name(edition)
       )
 
     defaults = descriptor_pb2.FeatureSet()
-    defaults.CopyFrom(found)
+    defaults.CopyFrom(found.fixed_features)
+    defaults.MergeFrom(found.overridable_features)
     return defaults
 
   def _InternFeatures(self, features):
     serialized = features.SerializeToString()
     with _edition_defaults_lock:
       cached = self._feature_cache.get(serialized)
       if cached is None:
```

### Comparing `protobuf-5.26.1/google/protobuf/duration_pb2.py` & `protobuf-5.27.0rc1/google/protobuf/source_context_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: google/protobuf/duration.proto
-# Protobuf Python Version: 5.26.1
+# NO CHECKED-IN PROTOBUF GENCODE
+# source: google/protobuf/source_context.proto
+# Protobuf Python Version: 5.27.0-rc1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import runtime_version as _runtime_version
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
+_runtime_version.ValidateProtobufRuntimeVersion(
+    _runtime_version.Domain.PUBLIC,
+    5,
+    27,
+    0,
+    '-rc1',
+    'google/protobuf/source_context.proto'
+)
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1egoogle/protobuf/duration.proto\x12\x0fgoogle.protobuf\":\n\x08\x44uration\x12\x18\n\x07seconds\x18\x01 \x01(\x03R\x07seconds\x12\x14\n\x05nanos\x18\x02 \x01(\x05R\x05nanosB\x83\x01\n\x13\x63om.google.protobufB\rDurationProtoP\x01Z1google.golang.org/protobuf/types/known/durationpb\xf8\x01\x01\xa2\x02\x03GPB\xaa\x02\x1eGoogle.Protobuf.WellKnownTypesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$google/protobuf/source_context.proto\x12\x0fgoogle.protobuf\",\n\rSourceContext\x12\x1b\n\tfile_name\x18\x01 \x01(\tR\x08\x66ileNameB\x8a\x01\n\x13\x63om.google.protobufB\x12SourceContextProtoP\x01Z6google.golang.org/protobuf/types/known/sourcecontextpb\xa2\x02\x03GPB\xaa\x02\x1eGoogle.Protobuf.WellKnownTypesb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'google.protobuf.duration_pb2', _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'google.protobuf.source_context_pb2', _globals)
 if not _descriptor._USE_C_DESCRIPTORS:
   _globals['DESCRIPTOR']._loaded_options = None
-  _globals['DESCRIPTOR']._serialized_options = b'\n\023com.google.protobufB\rDurationProtoP\001Z1google.golang.org/protobuf/types/known/durationpb\370\001\001\242\002\003GPB\252\002\036Google.Protobuf.WellKnownTypes'
-  _globals['_DURATION']._serialized_start=51
-  _globals['_DURATION']._serialized_end=109
+  _globals['DESCRIPTOR']._serialized_options = b'\n\023com.google.protobufB\022SourceContextProtoP\001Z6google.golang.org/protobuf/types/known/sourcecontextpb\242\002\003GPB\252\002\036Google.Protobuf.WellKnownTypes'
+  _globals['_SOURCECONTEXT']._serialized_start=57
+  _globals['_SOURCECONTEXT']._serialized_end=101
 # @@protoc_insertion_point(module_scope)
```

### Comparing `protobuf-5.26.1/google/protobuf/empty_pb2.py` & `protobuf-5.27.0rc1/google/protobuf/empty_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
+# NO CHECKED-IN PROTOBUF GENCODE
 # source: google/protobuf/empty.proto
-# Protobuf Python Version: 5.26.1
+# Protobuf Python Version: 5.27.0-rc1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import runtime_version as _runtime_version
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
+_runtime_version.ValidateProtobufRuntimeVersion(
+    _runtime_version.Domain.PUBLIC,
+    5,
+    27,
+    0,
+    '-rc1',
+    'google/protobuf/empty.proto'
+)
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
```

### Comparing `protobuf-5.26.1/google/protobuf/field_mask_pb2.py` & `protobuf-5.27.0rc1/google/protobuf/field_mask_pb2.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
+# NO CHECKED-IN PROTOBUF GENCODE
 # source: google/protobuf/field_mask.proto
-# Protobuf Python Version: 5.26.1
+# Protobuf Python Version: 5.27.0-rc1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import runtime_version as _runtime_version
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
+_runtime_version.ValidateProtobufRuntimeVersion(
+    _runtime_version.Domain.PUBLIC,
+    5,
+    27,
+    0,
+    '-rc1',
+    'google/protobuf/field_mask.proto'
+)
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
```

### Comparing `protobuf-5.26.1/google/protobuf/internal/_parameterized.py` & `protobuf-5.27.0rc1/google/protobuf/internal/_parameterized.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/google/protobuf/internal/api_implementation.py` & `protobuf-5.27.0rc1/google/protobuf/internal/api_implementation.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/google/protobuf/internal/builder.py` & `protobuf-5.27.0rc1/google/protobuf/internal/builder.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/google/protobuf/internal/containers.py` & `protobuf-5.27.0rc1/google/protobuf/internal/containers.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/google/protobuf/internal/decoder.py` & `protobuf-5.27.0rc1/google/protobuf/internal/decoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -382,26 +382,20 @@
           if not message._unknown_fields:
             message._unknown_fields = []
           tag_bytes = encoder.TagBytes(field_number,
                                        wire_format.WIRETYPE_VARINT)
 
           message._unknown_fields.append(
               (tag_bytes, buffer[value_start_pos:pos].tobytes()))
-          if message._unknown_field_set is None:
-            message._unknown_field_set = containers.UnknownFieldSet()
-          message._unknown_field_set._add(
-              field_number, wire_format.WIRETYPE_VARINT, element)
           # pylint: enable=protected-access
       if pos > endpoint:
         if element in enum_type.values_by_number:
           del value[-1]   # Discard corrupt value.
         else:
           del message._unknown_fields[-1]
-          # pylint: disable=protected-access
-          del message._unknown_field_set._values[-1]
           # pylint: enable=protected-access
         raise _DecodeError('Packed element was truncated.')
       return pos
     return DecodePackedField
   elif is_repeated:
     tag_bytes = encoder.TagBytes(field_number, wire_format.WIRETYPE_VARINT)
     tag_len = len(tag_bytes)
@@ -427,18 +421,14 @@
         if element in enum_type.values_by_number:
           value.append(element)
         else:
           if not message._unknown_fields:
             message._unknown_fields = []
           message._unknown_fields.append(
               (tag_bytes, buffer[pos:new_pos].tobytes()))
-          if message._unknown_field_set is None:
-            message._unknown_field_set = containers.UnknownFieldSet()
-          message._unknown_field_set._add(
-              field_number, wire_format.WIRETYPE_VARINT, element)
         # pylint: enable=protected-access
         # Predict that the next tag is another copy of the same repeated
         # field.
         pos = new_pos + tag_len
         if buffer[new_pos:pos] != tag_bytes or new_pos >= end:
           # Prediction failed.  Return.
           if new_pos > end:
@@ -472,18 +462,14 @@
       else:
         if not message._unknown_fields:
           message._unknown_fields = []
         tag_bytes = encoder.TagBytes(field_number,
                                      wire_format.WIRETYPE_VARINT)
         message._unknown_fields.append(
             (tag_bytes, buffer[value_start_pos:pos].tobytes()))
-        if message._unknown_field_set is None:
-          message._unknown_field_set = containers.UnknownFieldSet()
-        message._unknown_field_set._add(
-            field_number, wire_format.WIRETYPE_VARINT, enum_value)
         # pylint: enable=protected-access
       return pos
     return DecodeField
 
 
 # --------------------------------------------------------------------
 
@@ -791,20 +777,14 @@
         # an end-group tag.
         raise _DecodeError('Unexpected end-group tag.')
     else:
       if not message._unknown_fields:
         message._unknown_fields = []
       message._unknown_fields.append(
           (MESSAGE_SET_ITEM_TAG, buffer[message_set_item_start:pos].tobytes()))
-      if message._unknown_field_set is None:
-        message._unknown_field_set = containers.UnknownFieldSet()
-      message._unknown_field_set._add(
-          type_id,
-          wire_format.WIRETYPE_LENGTH_DELIMITED,
-          buffer[message_start:message_end].tobytes())
       # pylint: enable=protected-access
 
     return pos
 
   return DecodeItem
```

### Comparing `protobuf-5.26.1/google/protobuf/internal/encoder.py` & `protobuf-5.27.0rc1/google/protobuf/internal/encoder.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/google/protobuf/internal/enum_type_wrapper.py` & `protobuf-5.27.0rc1/google/protobuf/internal/enum_type_wrapper.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/google/protobuf/internal/extension_dict.py` & `protobuf-5.27.0rc1/google/protobuf/internal/extension_dict.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/google/protobuf/internal/field_mask.py` & `protobuf-5.27.0rc1/google/protobuf/internal/field_mask.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/google/protobuf/internal/message_listener.py` & `protobuf-5.27.0rc1/google/protobuf/internal/message_listener.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/google/protobuf/internal/python_message.py` & `protobuf-5.27.0rc1/google/protobuf/internal/python_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,15 +236,14 @@
     message_descriptor: A Descriptor instance describing this message type.
     dictionary: Class dictionary to which we'll add a '__slots__' entry.
   """
   dictionary['__slots__'] = ['_cached_byte_size',
                              '_cached_byte_size_dirty',
                              '_fields',
                              '_unknown_fields',
-                             '_unknown_field_set',
                              '_is_present_in_parent',
                              '_listener',
                              '_listener_for_children',
                              '__weakref__',
                              '_oneofs']
 
 
@@ -499,17 +498,14 @@
     # Contains a mapping from oneof field descriptors to the descriptor
     # of the currently set field in that oneof field.
     self._oneofs = {}
 
     # _unknown_fields is () when empty for efficiency, and will be turned into
     # a list if fields are added.
     self._unknown_fields = ()
-    # _unknown_field_set is None when empty for efficiency, and will be
-    # turned into UnknownFieldSet struct if fields are added.
-    self._unknown_field_set = None      # pylint: disable=protected-access
     self._is_present_in_parent = False
     self._listener = message_listener_mod.NullMessageListener()
     self._listener_for_children = _Listener(self)
     for field_name, field_value in kwargs.items():
       field = _GetFieldByName(message_descriptor, field_name)
       if field is None:
         raise TypeError('%s() got an unexpected keyword argument "%s"' %
@@ -1140,46 +1136,37 @@
       Message object.
     """
     # Guard against internal misuse, since this function is called internally
     # quite extensively, and its easy to accidentally pass bytes.
     assert isinstance(buffer, memoryview)
     self._Modified()
     field_dict = self._fields
-    # pylint: disable=protected-access
-    unknown_field_set = self._unknown_field_set
     while pos != end:
       (tag_bytes, new_pos) = local_ReadTag(buffer, pos)
       field_decoder, field_des = message_set_decoders_by_tag.get(
           tag_bytes, (None, None)
       )
       if field_decoder:
         pos = field_decoder(buffer, new_pos, end, self, field_dict)
         continue
       field_des, is_packed = fields_by_tag.get(tag_bytes, (None, None))
       if field_des is None:
         if not self._unknown_fields:   # pylint: disable=protected-access
           self._unknown_fields = []    # pylint: disable=protected-access
-        if unknown_field_set is None:
-          # pylint: disable=protected-access
-          self._unknown_field_set = containers.UnknownFieldSet()
-          # pylint: disable=protected-access
-          unknown_field_set = self._unknown_field_set
         # pylint: disable=protected-access
         (tag, _) = decoder._DecodeVarint(tag_bytes, 0)
         field_number, wire_type = wire_format.UnpackTag(tag)
         if field_number == 0:
           raise message_mod.DecodeError('Field number 0 is illegal.')
         # TODO: remove old_pos.
         old_pos = new_pos
         (data, new_pos) = decoder._DecodeUnknownField(
             buffer, new_pos, wire_type)  # pylint: disable=protected-access
         if new_pos == -1:
           return pos
-        # pylint: disable=protected-access
-        unknown_field_set._add(field_number, wire_type, data)
         # TODO: remove _unknown_fields.
         new_pos = local_SkipField(buffer, old_pos, end, tag_bytes)
         if new_pos == -1:
           return pos
         self._unknown_fields.append(
             (tag_bytes, buffer[old_pos:new_pos].tobytes()))
         pos = new_pos
@@ -1332,18 +1319,14 @@
         if field.containing_oneof:
           self._UpdateOneofState(field)
 
     if msg._unknown_fields:
       if not self._unknown_fields:
         self._unknown_fields = []
       self._unknown_fields.extend(msg._unknown_fields)
-      # pylint: disable=protected-access
-      if self._unknown_field_set is None:
-        self._unknown_field_set = containers.UnknownFieldSet()
-      self._unknown_field_set._extend(msg._unknown_field_set)
 
   cls.MergeFrom = MergeFrom
 
 
 def _AddWhichOneofMethod(message_descriptor, cls):
   def WhichOneof(self, oneof_name):
     """Returns the name of the currently set field inside a oneof, or None."""
@@ -1362,32 +1345,27 @@
   cls.WhichOneof = WhichOneof
 
 
 def _Clear(self):
   # Clear fields.
   self._fields = {}
   self._unknown_fields = ()
-  # pylint: disable=protected-access
-  if self._unknown_field_set is not None:
-    self._unknown_field_set._clear()
-    self._unknown_field_set = None
 
   self._oneofs = {}
   self._Modified()
 
 
 def _UnknownFields(self):
   raise NotImplementedError('Please use the add-on feaure '
                             'unknown_fields.UnknownFieldSet(message) in '
                             'unknown_fields.py instead.')
 
 
 def _DiscardUnknownFields(self):
   self._unknown_fields = []
-  self._unknown_field_set = None      # pylint: disable=protected-access
   for field, value in self.ListFields():
     if field.cpp_type == _FieldDescriptor.CPPTYPE_MESSAGE:
       if _IsMapField(field):
         if _IsMessageMapField(field):
           for key in value:
             value[key].DiscardUnknownFields()
       elif field.label == _FieldDescriptor.LABEL_REPEATED:
@@ -1421,15 +1399,14 @@
   _AddSerializePartialToStringMethod(message_descriptor, cls)
   _AddMergeFromStringMethod(message_descriptor, cls)
   _AddIsInitializedMethod(message_descriptor, cls)
   _AddMergeFromMethod(cls)
   _AddWhichOneofMethod(message_descriptor, cls)
   # Adds methods which do not depend on cls.
   cls.Clear = _Clear
-  cls.UnknownFields = _UnknownFields
   cls.DiscardUnknownFields = _DiscardUnknownFields
   cls._SetListener = _SetListener
 
 
 def _AddPrivateHelperMethods(message_descriptor, cls):
   """Adds implementation of private helper methods to cls."""
```

### Comparing `protobuf-5.26.1/google/protobuf/internal/testing_refleaks.py` & `protobuf-5.27.0rc1/google/protobuf/internal/testing_refleaks.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/google/protobuf/internal/type_checkers.py` & `protobuf-5.27.0rc1/google/protobuf/internal/type_checkers.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/google/protobuf/internal/well_known_types.py` & `protobuf-5.27.0rc1/google/protobuf/internal/well_known_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -396,15 +396,15 @@
         (millis % _MILLIS_PER_SECOND) * _NANOS_PER_MILLISECOND)
 
   def FromSeconds(self, seconds):
     """Converts seconds to Duration."""
     self.seconds = seconds
     self.nanos = 0
 
-  def ToTimedelta(self):
+  def ToTimedelta(self) -> datetime.timedelta:
     """Converts Duration to timedelta."""
     return datetime.timedelta(
         seconds=self.seconds, microseconds=_RoundTowardZero(
             self.nanos, _NANOS_PER_MICROSECOND))
 
   def FromTimedelta(self, td):
     """Converts timedelta to Duration."""
```

### Comparing `protobuf-5.26.1/google/protobuf/internal/wire_format.py` & `protobuf-5.27.0rc1/google/protobuf/internal/wire_format.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/google/protobuf/json_format.py` & `protobuf-5.27.0rc1/google/protobuf/json_format.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,20 @@
   """Thrown if serialization to JSON fails."""
 
 
 class ParseError(Error):
   """Thrown in case of parsing error."""
 
 
+class EnumStringValueParseError(ParseError):
+  """Thrown if unknown string enum value is encountered.
+  This exception is suppressed if ignore_unknown_fields is set.
+  """
+
+
 def MessageToJson(
     message,
     preserving_proto_field_name=False,
     indent=2,
     sort_keys=False,
     use_integers_for_enums=False,
     descriptor_pool=None,
@@ -293,15 +299,15 @@
         else:
           return value
     elif field.cpp_type == descriptor.FieldDescriptor.CPPTYPE_STRING:
       if field.type == descriptor.FieldDescriptor.TYPE_BYTES:
         # Use base64 Data encoding for bytes
         return base64.b64encode(value).decode('utf-8')
       else:
-        return value
+        return str(value)
     elif field.cpp_type == descriptor.FieldDescriptor.CPPTYPE_BOOL:
       return bool(value)
     elif field.cpp_type in _INT64_TYPES:
       return str(value)
     elif field.cpp_type in _FLOAT_TYPES:
       if math.isinf(value):
         if value < 0.0:
@@ -654,39 +660,28 @@
               if item is None:
                 raise ParseError(
                     'null is not allowed to be used as an element'
                     ' in a repeated field at {0}.{1}[{2}]'.format(
                         path, name, index
                     )
                 )
-              getattr(message, field.name).append(
-                  _ConvertScalarFieldValue(
-                      item, field, '{0}.{1}[{2}]'.format(path, name, index)
-                  )
-              )
+              self._ConvertAndAppendScalar(
+                message, field, item, '{0}.{1}[{2}]'.format(path, name, index))
         elif field.cpp_type == descriptor.FieldDescriptor.CPPTYPE_MESSAGE:
           if field.is_extension:
             sub_message = message.Extensions[field]
           else:
             sub_message = getattr(message, field.name)
           sub_message.SetInParent()
           self.ConvertMessage(value, sub_message, '{0}.{1}'.format(path, name))
         else:
           if field.is_extension:
-            message.Extensions[field] = _ConvertScalarFieldValue(
-                value, field, '{0}.{1}'.format(path, name)
-            )
+            self._ConvertAndSetScalarExtension(message, field, value, '{0}.{1}'.format(path, name))
           else:
-            setattr(
-                message,
-                field.name,
-                _ConvertScalarFieldValue(
-                    value, field, '{0}.{1}'.format(path, name)
-                ),
-            )
+            self._ConvertAndSetScalar(message, field, value, '{0}.{1}'.format(path, name))
       except ParseError as e:
         if field and field.containing_oneof is None:
           raise ParseError(
               'Failed to parse {0} field: {1}.'.format(name, e)
           ) from e
         else:
           raise ParseError(str(e)) from e
@@ -791,19 +786,15 @@
           value[key], message.fields[key], '{0}.{1}'.format(path, key)
       )
     return
 
   def _ConvertWrapperMessage(self, value, message, path):
     """Convert a JSON representation into Wrapper message."""
     field = message.DESCRIPTOR.fields_by_name['value']
-    setattr(
-        message,
-        'value',
-        _ConvertScalarFieldValue(value, field, path='{0}.value'.format(path)),
-    )
+    self._ConvertAndSetScalar(message, field, value, path='{0}.value'.format(path))
 
   def _ConvertMapFieldValue(self, value, message, field, path):
     """Convert map field value for a message map field.
 
     Args:
       value: A JSON object to convert the map field value.
       message: A protocol message to record the converted data.
@@ -828,17 +819,59 @@
       if value_field.cpp_type == descriptor.FieldDescriptor.CPPTYPE_MESSAGE:
         self.ConvertMessage(
             value[key],
             getattr(message, field.name)[key_value],
             '{0}[{1}]'.format(path, key_value),
         )
       else:
-        getattr(message, field.name)[key_value] = _ConvertScalarFieldValue(
-            value[key], value_field, path='{0}[{1}]'.format(path, key_value)
-        )
+        self._ConvertAndSetScalarToMapKey(
+            message,
+            field,
+            key_value,
+            value[key],
+            path='{0}[{1}]'.format(path, key_value))
+
+  def _ConvertAndSetScalarExtension(self, message, extension_field, js_value, path):
+    """Convert scalar from js_value and assign it to message.Extensions[extension_field]."""
+    try:
+      message.Extensions[extension_field] = _ConvertScalarFieldValue(
+          js_value, extension_field, path)
+    except EnumStringValueParseError:
+      if not self.ignore_unknown_fields:
+        raise
+
+  def _ConvertAndSetScalar(self, message, field, js_value, path):
+    """Convert scalar from js_value and assign it to message.field."""
+    try:
+      setattr(
+          message,
+          field.name,
+          _ConvertScalarFieldValue(js_value, field, path))
+    except EnumStringValueParseError:
+      if not self.ignore_unknown_fields:
+        raise
+
+  def _ConvertAndAppendScalar(self, message, repeated_field, js_value, path):
+    """Convert scalar from js_value and append it to message.repeated_field."""
+    try:
+      getattr(message, repeated_field.name).append(
+          _ConvertScalarFieldValue(js_value, repeated_field, path))
+    except EnumStringValueParseError:
+      if not self.ignore_unknown_fields:
+        raise
+
+  def _ConvertAndSetScalarToMapKey(self, message, map_field, converted_key, js_value, path):
+    """Convert scalar from 'js_value' and add it to message.map_field[converted_key]."""
+    try:
+      getattr(message, map_field.name)[converted_key] = _ConvertScalarFieldValue(
+          js_value, map_field.message_type.fields_by_name['value'], path,
+      )
+    except EnumStringValueParseError:
+      if not self.ignore_unknown_fields:
+        raise
 
 
 def _ConvertScalarFieldValue(value, field, path, require_str=False):
   """Convert a single scalar field value.
 
   Args:
     value: A scalar value to convert the scalar field value.
@@ -847,14 +880,15 @@
     require_str: If True, the field value must be a str.
 
   Returns:
     The converted scalar field value
 
   Raises:
     ParseError: In case of convert problems.
+    EnumStringValueParseError: In case of unknown enum string value.
   """
   try:
     if field.cpp_type in _INT_TYPES:
       return _ConvertInteger(value)
     elif field.cpp_type in _FLOAT_TYPES:
       return _ConvertFloat(value, field)
     elif field.cpp_type == descriptor.FieldDescriptor.CPPTYPE_BOOL:
@@ -878,29 +912,33 @@
       # Convert an enum value.
       enum_value = field.enum_type.values_by_name.get(value, None)
       if enum_value is None:
         try:
           number = int(value)
           enum_value = field.enum_type.values_by_number.get(number, None)
         except ValueError as e:
-          raise ParseError(
+          # Since parsing to integer failed and lookup in values_by_name didn't
+          # find this name, we have an enum string value which is unknown.
+          raise EnumStringValueParseError(
               'Invalid enum value {0} for enum type {1}'.format(
                   value, field.enum_type.full_name
               )
           ) from e
         if enum_value is None:
           if field.enum_type.is_closed:
             raise ParseError(
                 'Invalid enum value {0} for enum type {1}'.format(
                     value, field.enum_type.full_name
                 )
             )
           else:
             return number
       return enum_value.number
+  except EnumStringValueParseError as e:
+    raise EnumStringValueParseError('{0} at {1}'.format(e, path)) from e
   except ParseError as e:
     raise ParseError('{0} at {1}'.format(e, path)) from e
 
 
 def _ConvertInteger(value):
   """Convert an integer.
```

### Comparing `protobuf-5.26.1/google/protobuf/message.py` & `protobuf-5.27.0rc1/google/protobuf/message.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/google/protobuf/message_factory.py` & `protobuf-5.27.0rc1/google/protobuf/message_factory.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/google/protobuf/proto_builder.py` & `protobuf-5.27.0rc1/google/protobuf/proto_builder.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/google/protobuf/pyext/cpp_message.py` & `protobuf-5.27.0rc1/google/protobuf/pyext/cpp_message.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/google/protobuf/reflection.py` & `protobuf-5.27.0rc1/google/protobuf/reflection.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/google/protobuf/service.py` & `protobuf-5.27.0rc1/google/protobuf/service.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/google/protobuf/service_reflection.py` & `protobuf-5.27.0rc1/google/protobuf/service_reflection.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/google/protobuf/source_context_pb2.py` & `protobuf-5.27.0rc1/google/protobuf/timestamp_pb2.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: google/protobuf/source_context.proto
-# Protobuf Python Version: 5.26.1
+# NO CHECKED-IN PROTOBUF GENCODE
+# source: google/protobuf/timestamp.proto
+# Protobuf Python Version: 5.27.0-rc1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import runtime_version as _runtime_version
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
+_runtime_version.ValidateProtobufRuntimeVersion(
+    _runtime_version.Domain.PUBLIC,
+    5,
+    27,
+    0,
+    '-rc1',
+    'google/protobuf/timestamp.proto'
+)
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$google/protobuf/source_context.proto\x12\x0fgoogle.protobuf\",\n\rSourceContext\x12\x1b\n\tfile_name\x18\x01 \x01(\tR\x08\x66ileNameB\x8a\x01\n\x13\x63om.google.protobufB\x12SourceContextProtoP\x01Z6google.golang.org/protobuf/types/known/sourcecontextpb\xa2\x02\x03GPB\xaa\x02\x1eGoogle.Protobuf.WellKnownTypesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1fgoogle/protobuf/timestamp.proto\x12\x0fgoogle.protobuf\";\n\tTimestamp\x12\x18\n\x07seconds\x18\x01 \x01(\x03R\x07seconds\x12\x14\n\x05nanos\x18\x02 \x01(\x05R\x05nanosB\x85\x01\n\x13\x63om.google.protobufB\x0eTimestampProtoP\x01Z2google.golang.org/protobuf/types/known/timestamppb\xf8\x01\x01\xa2\x02\x03GPB\xaa\x02\x1eGoogle.Protobuf.WellKnownTypesb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'google.protobuf.source_context_pb2', _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'google.protobuf.timestamp_pb2', _globals)
 if not _descriptor._USE_C_DESCRIPTORS:
   _globals['DESCRIPTOR']._loaded_options = None
-  _globals['DESCRIPTOR']._serialized_options = b'\n\023com.google.protobufB\022SourceContextProtoP\001Z6google.golang.org/protobuf/types/known/sourcecontextpb\242\002\003GPB\252\002\036Google.Protobuf.WellKnownTypes'
-  _globals['_SOURCECONTEXT']._serialized_start=57
-  _globals['_SOURCECONTEXT']._serialized_end=101
+  _globals['DESCRIPTOR']._serialized_options = b'\n\023com.google.protobufB\016TimestampProtoP\001Z2google.golang.org/protobuf/types/known/timestamppb\370\001\001\242\002\003GPB\252\002\036Google.Protobuf.WellKnownTypes'
+  _globals['_TIMESTAMP']._serialized_start=52
+  _globals['_TIMESTAMP']._serialized_end=111
 # @@protoc_insertion_point(module_scope)
```

### Comparing `protobuf-5.26.1/google/protobuf/struct_pb2.py` & `protobuf-5.27.0rc1/google/protobuf/struct_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
+# NO CHECKED-IN PROTOBUF GENCODE
 # source: google/protobuf/struct.proto
-# Protobuf Python Version: 5.26.1
+# Protobuf Python Version: 5.27.0-rc1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import runtime_version as _runtime_version
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
+_runtime_version.ValidateProtobufRuntimeVersion(
+    _runtime_version.Domain.PUBLIC,
+    5,
+    27,
+    0,
+    '-rc1',
+    'google/protobuf/struct.proto'
+)
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
```

### Comparing `protobuf-5.26.1/google/protobuf/symbol_database.py` & `protobuf-5.27.0rc1/google/protobuf/symbol_database.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/google/protobuf/text_encoding.py` & `protobuf-5.27.0rc1/google/protobuf/text_encoding.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/google/protobuf/text_format.py` & `protobuf-5.27.0rc1/google/protobuf/text_format.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,14 +181,47 @@
 
 def _IsMapEntry(field):
   return (field.type == descriptor.FieldDescriptor.TYPE_MESSAGE and
           field.message_type.has_options and
           field.message_type.GetOptions().map_entry)
 
 
+def _IsGroupLike(field):
+  """Determines if a field is consistent with a proto2 group.
+
+  Args:
+    field: The field descriptor.
+
+  Returns:
+    True if this field is group-like, false otherwise.
+  """
+  # Groups are always tag-delimited.
+  if (
+      field._GetFeatures().message_encoding
+      != descriptor._FEATURESET_MESSAGE_ENCODING_DELIMITED
+  ):
+    return False
+
+  # Group fields always are always the lowercase type name.
+  if field.name != field.message_type.name.lower():
+    return False
+
+  if field.message_type.file != field.file:
+    return False
+
+  # Group messages are always defined in the same scope as the field.  File
+  # level extensions will compare NULL == NULL here, which is why the file
+  # comparison above is necessary to ensure both come from the same file.
+  return (
+      field.message_type.containing_type == field.extension_scope
+      if field.is_extension
+      else field.message_type.containing_type == field.containing_type
+  )
+
+
 def PrintMessage(message,
                  out,
                  indent=0,
                  as_utf8=_as_utf8_default,
                  as_one_line=False,
                  use_short_repeated_primitives=False,
                  pointy_brackets=False,
@@ -527,15 +560,15 @@
         if (field.containing_type.GetOptions().message_set_wire_format and
             field.type == descriptor.FieldDescriptor.TYPE_MESSAGE and
             field.label == descriptor.FieldDescriptor.LABEL_OPTIONAL):
           out.write(field.message_type.full_name)
         else:
           out.write(field.full_name)
         out.write(']')
-      elif field.type == descriptor.FieldDescriptor.TYPE_GROUP:
+      elif _IsGroupLike(field):
         # For groups, use the capitalized name.
         out.write(field.message_type.name)
       else:
         out.write(field.name)
 
     if (self.force_colon or
         field.cpp_type != descriptor.FieldDescriptor.CPPTYPE_MESSAGE):
@@ -929,20 +962,18 @@
         field = message_descriptor.fields_by_name.get(name, None)
 
         # Group names are expected to be capitalized as they appear in the
         # .proto file, which actually matches their type names, not their field
         # names.
         if not field:
           field = message_descriptor.fields_by_name.get(name.lower(), None)
-          if field and field.type != descriptor.FieldDescriptor.TYPE_GROUP:
+          if field and not _IsGroupLike(field):
+            field = None
+          if field and field.message_type.name != name:
             field = None
-
-        if (field and field.type == descriptor.FieldDescriptor.TYPE_GROUP and
-            field.message_type.name != name):
-          field = None
 
       if not field and not self.allow_unknown_field:
         raise tokenizer.ParseErrorPreviousToken(
             'Message type "%s" has no field named "%s".' %
             (message_descriptor.full_name, name))
 
     if field:
```

### Comparing `protobuf-5.26.1/google/protobuf/type_pb2.py` & `protobuf-5.27.0rc1/google/protobuf/type_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
+# NO CHECKED-IN PROTOBUF GENCODE
 # source: google/protobuf/type.proto
-# Protobuf Python Version: 5.26.1
+# Protobuf Python Version: 5.27.0-rc1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import runtime_version as _runtime_version
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
+_runtime_version.ValidateProtobufRuntimeVersion(
+    _runtime_version.Domain.PUBLIC,
+    5,
+    27,
+    0,
+    '-rc1',
+    'google/protobuf/type.proto'
+)
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import any_pb2 as google_dot_protobuf_dot_any__pb2
 from google.protobuf import source_context_pb2 as google_dot_protobuf_dot_source__context__pb2
```

### Comparing `protobuf-5.26.1/google/protobuf/unknown_fields.py` & `protobuf-5.27.0rc1/google/protobuf/unknown_fields.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/google/protobuf/wrappers_pb2.py` & `protobuf-5.27.0rc1/google/protobuf/wrappers_pb2.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
+# NO CHECKED-IN PROTOBUF GENCODE
 # source: google/protobuf/wrappers.proto
-# Protobuf Python Version: 5.26.1
+# Protobuf Python Version: 5.27.0-rc1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import runtime_version as _runtime_version
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
+_runtime_version.ValidateProtobufRuntimeVersion(
+    _runtime_version.Domain.PUBLIC,
+    5,
+    27,
+    0,
+    '-rc1',
+    'google/protobuf/wrappers.proto'
+)
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
```

### Comparing `protobuf-5.26.1/protobuf.egg-info/PKG-INFO` & `protobuf-5.27.0rc1/protobuf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protobuf
-Version: 5.26.1
+Version: 5.27.0rc1
 Summary: Protocol Buffers
 Home-page: https://developers.google.com/protocol-buffers/
 Download-URL: https://github.com/protocolbuffers/protobuf/releases
 Maintainer: protobuf@googlegroups.com
 Maintainer-email: protobuf@googlegroups.com
 License: BSD-3-Clause
 Project-URL: Source, https://github.com/protocolbuffers/protobuf
```

### Comparing `protobuf-5.26.1/protobuf.egg-info/SOURCES.txt` & `protobuf-5.27.0rc1/protobuf.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 google/protobuf/empty_pb2.py
 google/protobuf/field_mask_pb2.py
 google/protobuf/json_format.py
 google/protobuf/message.py
 google/protobuf/message_factory.py
 google/protobuf/proto_builder.py
 google/protobuf/reflection.py
+google/protobuf/runtime_version.py
 google/protobuf/service.py
 google/protobuf/service_reflection.py
 google/protobuf/source_context_pb2.py
 google/protobuf/struct_pb2.py
 google/protobuf/symbol_database.py
 google/protobuf/text_encoding.py
 google/protobuf/text_format.py
@@ -110,15 +111,14 @@
 upb/mem/arena.h
 upb/mem/internal/arena.h
 upb/message/accessors.c
 upb/message/accessors.h
 upb/message/accessors_split64.h
 upb/message/array.c
 upb/message/array.h
-upb/message/array_split64.h
 upb/message/compare.c
 upb/message/compare.h
 upb/message/compat.c
 upb/message/compat.h
 upb/message/copy.c
 upb/message/copy.h
 upb/message/map.c
@@ -129,14 +129,16 @@
 upb/message/message.h
 upb/message/promote.c
 upb/message/promote.h
 upb/message/tagged_ptr.h
 upb/message/value.h
 upb/message/internal/accessors.h
 upb/message/internal/array.h
+upb/message/internal/compare_unknown.c
+upb/message/internal/compare_unknown.h
 upb/message/internal/extension.c
 upb/message/internal/extension.h
 upb/message/internal/map.h
 upb/message/internal/map_entry.h
 upb/message/internal/map_sorter.h
 upb/message/internal/message.c
 upb/message/internal/message.h
@@ -225,16 +227,14 @@
 upb/reflection/internal/oneof_def.h
 upb/reflection/internal/service_def.h
 upb/reflection/internal/strdup2.c
 upb/reflection/internal/strdup2.h
 upb/reflection/internal/upb_edition_defaults.h
 upb/text/encode.c
 upb/text/encode.h
-upb/util/compare.c
-upb/util/compare.h
 upb/util/def_to_proto.c
 upb/util/def_to_proto.h
 upb/util/required_fields.c
 upb/util/required_fields.h
 upb/wire/decode.c
 upb/wire/decode.h
 upb/wire/encode.c
```

### Comparing `protobuf-5.26.1/python/convert.h` & `protobuf-5.27.0rc1/upb/reflection/message.h`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,89 @@
 // Protocol Buffers - Google's data interchange format
 // Copyright 2023 Google LLC.  All rights reserved.
 //
 // Use of this source code is governed by a BSD-style
 // license that can be found in the LICENSE file or at
 // https://developers.google.com/open-source/licenses/bsd
 
-#ifndef PYUPB_CONVERT_H__
-#define PYUPB_CONVERT_H__
+#ifndef UPB_REFLECTION_MESSAGE_H_
+#define UPB_REFLECTION_MESSAGE_H_
 
-#include "protobuf.h"
-#include "upb/reflection/def.h"
-#include "upb/reflection/message.h"
-
-// Converts `val` to a Python object according to the type information in `f`.
-// Any newly-created Python objects that reference non-primitive data from `val`
-// will take a reference on `arena`; the caller must ensure that `val` belongs
-// to `arena`. If the conversion cannot be performed, returns NULL and sets a
-// Python error.
-PyObject* PyUpb_UpbToPy(upb_MessageValue val, const upb_FieldDef* f,
-                        PyObject* arena);
-
-// Converts `obj` to a upb_MessageValue `*val` according to the type information
-// in `f`. If `arena` is provided, any string data will be copied into `arena`,
-// otherwise the returned value will alias the Python-owned data (this can be
-// useful for an ephemeral upb_MessageValue).  If the conversion cannot be
-// performed, returns false.
-bool PyUpb_PyToUpb(PyObject* obj, const upb_FieldDef* f, upb_MessageValue* val,
-                   upb_Arena* arena);
-
-// Returns true if the given values (of type `f`) are equal.
-bool PyUpb_ValueEq(upb_MessageValue val1, upb_MessageValue val2,
-                   const upb_FieldDef* f);
-
-// Returns true if the two arrays (with element type `f`) are equal.
-bool PyUpb_Array_IsEqual(const upb_Array* arr1, const upb_Array* arr2,
-                         const upb_FieldDef* f);
-
-// Returns true if the given messages (of type `m`) are equal.
-bool upb_Message_IsEqual(const upb_Message* msg1, const upb_Message* msg2,
-                         const upb_MessageDef* m);
+#include <stddef.h>
 
-#endif  // PYUPB_CONVERT_H__
+#include "upb/mem/arena.h"
+#include "upb/message/map.h"
+#include "upb/message/message.h"
+#include "upb/reflection/common.h"
+
+// Must be last.
+#include "upb/port/def.inc"
+
+#ifdef __cplusplus
+extern "C" {
+#endif
+
+// Returns a mutable pointer to a map, array, or submessage value. If the given
+// arena is non-NULL this will construct a new object if it was not previously
+// present. May not be called for primitive fields.
+UPB_API upb_MutableMessageValue upb_Message_Mutable(upb_Message* msg,
+                                                    const upb_FieldDef* f,
+                                                    upb_Arena* a);
+
+// Returns the field that is set in the oneof, or NULL if none are set.
+UPB_API const upb_FieldDef* upb_Message_WhichOneof(const upb_Message* msg,
+                                                   const upb_OneofDef* o);
+
+// Clear all data and unknown fields.
+void upb_Message_ClearByDef(upb_Message* msg, const upb_MessageDef* m);
+
+// Clears any field presence and sets the value back to its default.
+UPB_API void upb_Message_ClearFieldByDef(upb_Message* msg,
+                                         const upb_FieldDef* f);
+
+// May only be called for fields where upb_FieldDef_HasPresence(f) == true.
+UPB_API bool upb_Message_HasFieldByDef(const upb_Message* msg,
+                                       const upb_FieldDef* f);
+
+// Returns the value in the message associated with this field def.
+UPB_API upb_MessageValue upb_Message_GetFieldByDef(const upb_Message* msg,
+                                                   const upb_FieldDef* f);
+
+// Sets the given field to the given value. For a msg/array/map/string, the
+// caller must ensure that the target data outlives |msg| (by living either in
+// the same arena or a different arena that outlives it).
+//
+// Returns false if allocation fails.
+UPB_API bool upb_Message_SetFieldByDef(upb_Message* msg, const upb_FieldDef* f,
+                                       upb_MessageValue val, upb_Arena* a);
+
+// Iterate over present fields.
+//
+// size_t iter = kUpb_Message_Begin;
+// const upb_FieldDef *f;
+// upb_MessageValue val;
+// while (upb_Message_Next(msg, m, ext_pool, &f, &val, &iter)) {
+//   process_field(f, val);
+// }
+//
+// If ext_pool is NULL, no extensions will be returned.  If the given symtab
+// returns extensions that don't match what is in this message, those extensions
+// will be skipped.
+
+#define kUpb_Message_Begin -1
+
+UPB_API bool upb_Message_Next(const upb_Message* msg, const upb_MessageDef* m,
+                              const upb_DefPool* ext_pool,
+                              const upb_FieldDef** f, upb_MessageValue* val,
+                              size_t* iter);
+
+// Clears all unknown field data from this message and all submessages.
+UPB_API bool upb_Message_DiscardUnknown(upb_Message* msg,
+                                        const upb_MessageDef* m, int maxdepth);
+
+#ifdef __cplusplus
+} /* extern "C" */
+#endif
+
+#include "upb/port/undef.inc"
+
+#endif /* UPB_REFLECTION_MESSAGE_H_ */
```

### Comparing `protobuf-5.26.1/python/descriptor.c` & `protobuf-5.27.0rc1/python/descriptor.c`

 * *Files 1% similar despite different names*

```diff
@@ -979,18 +979,31 @@
 }
 
 static PyObject* PyUpb_FieldDescriptor_GetName(PyUpb_DescriptorBase* self,
                                                void* closure) {
   return PyUnicode_FromString(upb_FieldDef_Name(self->def));
 }
 
+static char PyUpb_AsciiIsUpper(char ch) { return ch >= 'A' && ch <= 'Z'; }
+
+static char PyUpb_AsciiToLower(char ch) {
+  assert(PyUpb_AsciiIsUpper(ch));
+  return ch + ('a' - 'A');
+}
+
 static PyObject* PyUpb_FieldDescriptor_GetCamelCaseName(
     PyUpb_DescriptorBase* self, void* closure) {
-  // TODO: Ok to use jsonname here?
-  return PyUnicode_FromString(upb_FieldDef_JsonName(self->def));
+  // Camelcase is equivalent to JSON name except for potentially the first
+  // character.
+  const char* name = upb_FieldDef_JsonName(self->def);
+  size_t size = strlen(name);
+  return size > 0 && PyUpb_AsciiIsUpper(name[0])
+             ? PyUnicode_FromFormat("%c%s", PyUpb_AsciiToLower(name[0]),
+                                    name + 1)
+             : PyUnicode_FromStringAndSize(name, size);
 }
 
 static PyObject* PyUpb_FieldDescriptor_GetJsonName(PyUpb_DescriptorBase* self,
                                                    void* closure) {
   return PyUnicode_FromString(upb_FieldDef_JsonName(self->def));
 }
```

### Comparing `protobuf-5.26.1/python/descriptor.h` & `protobuf-5.27.0rc1/python/descriptor.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/python/descriptor_containers.c` & `protobuf-5.27.0rc1/python/descriptor_containers.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/python/descriptor_containers.h` & `protobuf-5.27.0rc1/python/descriptor_containers.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/python/descriptor_pool.c` & `protobuf-5.27.0rc1/python/descriptor_pool.c`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 #include "google/protobuf/descriptor.upbdefs.h"
 #include "python/convert.h"
 #include "python/descriptor.h"
 #include "python/message.h"
 #include "python/protobuf.h"
 #include "upb/base/upcast.h"
+#include "upb/message/compare.h"
 #include "upb/reflection/def.h"
 #include "upb/util/def_to_proto.h"
 
 // -----------------------------------------------------------------------------
 // DescriptorPool
 // -----------------------------------------------------------------------------
 
@@ -193,15 +194,17 @@
     // duplicate add.
     google_protobuf_FileDescriptorProto* existing = upb_FileDef_ToProto(file, arena);
     if (!existing) {
       PyErr_SetNone(PyExc_MemoryError);
       goto done;
     }
     const upb_MessageDef* m = PyUpb_DescriptorPool_GetFileProtoDef();
-    if (upb_Message_IsEqual(UPB_UPCAST(proto), UPB_UPCAST(existing), m)) {
+    const int options = kUpb_CompareOption_IncludeUnknownFields;
+    if (upb_Message_IsEqualByDef(UPB_UPCAST(proto), UPB_UPCAST(existing), m,
+                                 options)) {
       result = PyUpb_FileDescriptor_Get(file);
       goto done;
     }
   }
 
   if (self->db) {
     if (!PyUpb_DescriptorPool_LoadDependentFiles(self, proto)) goto done;
```

### Comparing `protobuf-5.26.1/python/descriptor_pool.h` & `protobuf-5.27.0rc1/python/descriptor_pool.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/python/extension_dict.c` & `protobuf-5.27.0rc1/python/extension_dict.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/python/extension_dict.h` & `protobuf-5.27.0rc1/python/extension_dict.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/python/map.c` & `protobuf-5.27.0rc1/python/map.c`

 * *Files 1% similar despite different names*

```diff
@@ -191,27 +191,27 @@
       memset(&u_val, 0, sizeof(u_val));
     }
     if (!PyUpb_MapContainer_Set(self, map, u_key, u_val, arena)) return false;
   }
   return PyUpb_UpbToPy(u_val, val_f, self->arena);
 }
 
-static PyObject* PyUpb_MapContainer_Contains(PyObject* _self, PyObject* key) {
+static int PyUpb_MapContainer_Contains(PyObject* _self, PyObject* key) {
   PyUpb_MapContainer* self = (PyUpb_MapContainer*)_self;
   upb_Map* map = PyUpb_MapContainer_GetIfReified(self);
-  if (!map) Py_RETURN_FALSE;
+  if (!map) return 0;
   const upb_FieldDef* f = PyUpb_MapContainer_GetField(self);
   const upb_MessageDef* entry_m = upb_FieldDef_MessageSubDef(f);
   const upb_FieldDef* key_f = upb_MessageDef_Field(entry_m, 0);
   upb_MessageValue u_key;
-  if (!PyUpb_PyToUpb(key, key_f, &u_key, NULL)) return NULL;
+  if (!PyUpb_PyToUpb(key, key_f, &u_key, NULL)) return -1;
   if (upb_Map_Get(map, u_key, NULL)) {
-    Py_RETURN_TRUE;
+    return 1;
   } else {
-    Py_RETURN_FALSE;
+    return 0;
   }
 }
 
 static PyObject* PyUpb_MapContainer_Clear(PyObject* _self, PyObject* key) {
   upb_Map* map = PyUpb_MapContainer_EnsureReified(_self);
   upb_Map_Clear(map);
   Py_RETURN_NONE;
@@ -335,16 +335,14 @@
 }
 
 // -----------------------------------------------------------------------------
 // ScalarMapContainer
 // -----------------------------------------------------------------------------
 
 static PyMethodDef PyUpb_ScalarMapContainer_Methods[] = {
-    {"__contains__", PyUpb_MapContainer_Contains, METH_O,
-     "Tests whether a key is a member of the map."},
     {"clear", PyUpb_MapContainer_Clear, METH_NOARGS,
      "Removes all elements from the map."},
     {"get", (PyCFunction)PyUpb_MapContainer_Get, METH_VARARGS | METH_KEYWORDS,
      "Gets the value for the given key if present, or otherwise a default"},
     {"GetEntryClass", PyUpb_MapContainer_GetEntryClass, METH_NOARGS,
      "Return the class used to build Entries of (key, value) pairs."},
     {"MergeFrom", PyUpb_MapContainer_MergeFrom, METH_O,
@@ -359,14 +357,15 @@
 };
 
 static PyType_Slot PyUpb_ScalarMapContainer_Slots[] = {
     {Py_tp_dealloc, PyUpb_MapContainer_Dealloc},
     {Py_mp_length, PyUpb_MapContainer_Length},
     {Py_mp_subscript, PyUpb_MapContainer_Subscript},
     {Py_mp_ass_subscript, PyUpb_MapContainer_AssignSubscript},
+    {Py_sq_contains, PyUpb_MapContainer_Contains},
     {Py_tp_methods, PyUpb_ScalarMapContainer_Methods},
     {Py_tp_iter, PyUpb_MapIterator_New},
     {Py_tp_repr, PyUpb_MapContainer_Repr},
     {0, NULL},
 };
 
 static PyType_Spec PyUpb_ScalarMapContainer_Spec = {
@@ -378,16 +377,14 @@
 };
 
 // -----------------------------------------------------------------------------
 // MessageMapContainer
 // -----------------------------------------------------------------------------
 
 static PyMethodDef PyUpb_MessageMapContainer_Methods[] = {
-    {"__contains__", PyUpb_MapContainer_Contains, METH_O,
-     "Tests whether the map contains this element."},
     {"clear", PyUpb_MapContainer_Clear, METH_NOARGS,
      "Removes all elements from the map."},
     {"get", (PyCFunction)PyUpb_MapContainer_Get, METH_VARARGS | METH_KEYWORDS,
      "Gets the value for the given key if present, or otherwise a default"},
     {"get_or_create", PyUpb_MapContainer_Subscript, METH_O,
      "Alias for getitem, useful to make explicit that the map is mutated."},
     {"GetEntryClass", PyUpb_MapContainer_GetEntryClass, METH_NOARGS,
@@ -404,14 +401,15 @@
 };
 
 static PyType_Slot PyUpb_MessageMapContainer_Slots[] = {
     {Py_tp_dealloc, PyUpb_MapContainer_Dealloc},
     {Py_mp_length, PyUpb_MapContainer_Length},
     {Py_mp_subscript, PyUpb_MapContainer_Subscript},
     {Py_mp_ass_subscript, PyUpb_MapContainer_AssignSubscript},
+    {Py_sq_contains, PyUpb_MapContainer_Contains},
     {Py_tp_methods, PyUpb_MessageMapContainer_Methods},
     {Py_tp_iter, PyUpb_MapIterator_New},
     {Py_tp_repr, PyUpb_MapContainer_Repr},
     {0, NULL}};
 
 static PyType_Spec PyUpb_MessageMapContainer_Spec = {
     PYUPB_MODULE_NAME ".MessageMapContainer", sizeof(PyUpb_MapContainer), 0,
@@ -473,33 +471,43 @@
 // -----------------------------------------------------------------------------
 // Top Level
 // -----------------------------------------------------------------------------
 
 static PyObject* GetMutableMappingBase(void) {
   PyObject* collections = NULL;
   PyObject* mapping = NULL;
-  PyObject* bases = NULL;
+  PyObject* base = NULL;
   if ((collections = PyImport_ImportModule("collections.abc")) &&
       (mapping = PyObject_GetAttrString(collections, "MutableMapping"))) {
-    bases = Py_BuildValue("(O)", mapping);
+    base = Py_BuildValue("O", mapping);
   }
   Py_XDECREF(collections);
   Py_XDECREF(mapping);
-  return bases;
+  return base;
 }
 
 bool PyUpb_Map_Init(PyObject* m) {
   PyUpb_ModuleState* state = PyUpb_ModuleState_GetFromModule(m);
-  PyObject* bases = GetMutableMappingBase();
-  if (!bases) return false;
+  PyObject* base = GetMutableMappingBase();
+  if (!base) return false;
+
+  const char* methods[] = {"keys", "items",   "values", "__eq__",     "__ne__",
+                           "pop",  "popitem", "update", "setdefault", NULL};
 
-  state->message_map_container_type =
-      PyUpb_AddClassWithBases(m, &PyUpb_MessageMapContainer_Spec, bases);
-  state->scalar_map_container_type =
-      PyUpb_AddClassWithBases(m, &PyUpb_ScalarMapContainer_Spec, bases);
+  state->message_map_container_type = PyUpb_AddClassWithRegister(
+      m, &PyUpb_MessageMapContainer_Spec, base, methods);
+  if (!state->message_map_container_type) {
+    return false;
+  }
+  state->scalar_map_container_type = PyUpb_AddClassWithRegister(
+      m, &PyUpb_ScalarMapContainer_Spec, base, methods);
+  if (!state->scalar_map_container_type) {
+    return false;
+  }
   state->map_iterator_type = PyUpb_AddClass(m, &PyUpb_MapIterator_Spec);
 
-  Py_DECREF(bases);
+  Py_DECREF(base);
+  Py_DECREF(methods);
 
   return state->message_map_container_type &&
          state->scalar_map_container_type && state->map_iterator_type;
 }
```

### Comparing `protobuf-5.26.1/python/map.h` & `protobuf-5.27.0rc1/python/map.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/python/message.c` & `protobuf-5.27.0rc1/python/message.c`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #include "python/message.h"
 
 #include "python/convert.h"
 #include "python/descriptor.h"
 #include "python/extension_dict.h"
 #include "python/map.h"
 #include "python/repeated.h"
+#include "upb/message/compare.h"
 #include "upb/message/copy.h"
 #include "upb/reflection/def.h"
 #include "upb/reflection/message.h"
 #include "upb/text/encode.h"
 #include "upb/util/required_fields.h"
 
 static const upb_MessageDef* PyUpb_MessageMeta_GetMsgdef(PyObject* cls);
@@ -571,15 +572,16 @@
   const upb_Message* m2_msg = PyUpb_Message_GetIfReified(_m2);
   const upb_DefPool* symtab = upb_FileDef_Pool(upb_MessageDef_File(m1_msgdef));
 
   const bool e1 = PyUpb_Message_IsEmpty(m1_msg, m1_msgdef, symtab);
   const bool e2 = PyUpb_Message_IsEmpty(m2_msg, m1_msgdef, symtab);
   if (e1 || e2) return e1 && e2;
 
-  return upb_Message_IsEqual(m1_msg, m2_msg, m1_msgdef);
+  const int options = kUpb_CompareOption_IncludeUnknownFields;
+  return upb_Message_IsEqualByDef(m1_msg, m2_msg, m1_msgdef, options);
 }
 
 static const upb_FieldDef* PyUpb_Message_InitAsMsg(PyUpb_Message* m,
                                                    upb_Arena* arena) {
   const upb_FieldDef* f = PyUpb_Message_GetFieldDef(m);
   const upb_MessageDef* m2 = upb_FieldDef_MessageSubDef(f);
   m->ptr.msg = upb_Message_New(upb_MessageDef_MiniTable(m2), arena);
```

### Comparing `protobuf-5.26.1/python/message.h` & `protobuf-5.27.0rc1/python/message.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/python/protobuf.c` & `protobuf-5.27.0rc1/python/protobuf.c`

 * *Files 7% similar despite different names*

```diff
@@ -319,14 +319,39 @@
   if (PyModule_AddObject(m, name, type) < 0) {
     Py_XDECREF(type);
     return NULL;
   }
   return (PyTypeObject*)type;
 }
 
+PyTypeObject* PyUpb_AddClassWithRegister(PyObject* m, PyType_Spec* spec,
+                                         PyObject* virtual_base,
+                                         const char** methods) {
+  PyObject* type = PyType_FromSpec(spec);
+  PyObject* ret1 = PyObject_CallMethod(virtual_base, "register", "O", type);
+  if (!ret1) {
+    Py_XDECREF(type);
+    return NULL;
+  }
+  for (size_t i = 0; methods[i] != NULL; i++) {
+    PyObject* method = PyObject_GetAttrString(virtual_base, methods[i]);
+    if (!method) {
+      Py_XDECREF(type);
+      return NULL;
+    }
+    int ret2 = PyObject_SetAttrString(type, methods[i], method);
+    if (ret2 < 0) {
+      Py_XDECREF(type);
+      return NULL;
+    }
+  }
+
+  return (PyTypeObject*)type;
+}
+
 const char* PyUpb_GetStrData(PyObject* obj) {
   if (PyUnicode_Check(obj)) {
     return PyUnicode_AsUTF8AndSize(obj, NULL);
   } else if (PyBytes_Check(obj)) {
     return PyBytes_AsString(obj);
   } else {
     return NULL;
```

### Comparing `protobuf-5.26.1/python/protobuf.h` & `protobuf-5.27.0rc1/python/protobuf.h`

 * *Files 2% similar despite different names*

```diff
@@ -176,14 +176,20 @@
 PyTypeObject* PyUpb_AddClass(PyObject* m, PyType_Spec* spec);
 
 // Like PyUpb_AddClass(), but allows you to specify a tuple of base classes
 // in `bases`.
 PyTypeObject* PyUpb_AddClassWithBases(PyObject* m, PyType_Spec* spec,
                                       PyObject* bases);
 
+// Like PyUpb_AddClass(), but allows you to specify a tuple of base classes in
+// `bases` to register as a "virtual subclass" with mixin methods.
+PyTypeObject* PyUpb_AddClassWithRegister(PyObject* m, PyType_Spec* spec,
+                                         PyObject* virtual_base,
+                                         const char** methods);
+
 // A function that implements the tp_new slot for types that we do not allow
 // users to create directly. This will immediately fail with an error message.
 PyObject* PyUpb_Forbidden_New(PyObject* cls, PyObject* args, PyObject* kwds);
 
 // Our standard dealloc func. It follows the guidance defined in:
 //   https://docs.python.org/3/c-api/typeobj.html#c.PyTypeObject.tp_dealloc
 // However it tests Py_TPFLAGS_HEAPTYPE dynamically so that a single dealloc
```

### Comparing `protobuf-5.26.1/python/python_api.h` & `protobuf-5.27.0rc1/python/python_api.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/python/repeated.c` & `protobuf-5.27.0rc1/python/repeated.c`

 * *Files 0% similar despite different names*

```diff
@@ -469,19 +469,22 @@
       // Must set before deleting as sort_func is a borrowed reference
       // and kwds might be the only thing keeping it alive.
       if (PyDict_SetItemString(kwds, "cmp", sort_func) == -1) return NULL;
       if (PyDict_DelItemString(kwds, "sort_function") == -1) return NULL;
     }
   }
 
+  if (PyUpb_RepeatedContainer_Length(pself) == 0) Py_RETURN_NONE;
+
   PyObject* ret = NULL;
   PyObject* full_slice = NULL;
   PyObject* list = NULL;
   PyObject* m = NULL;
   PyObject* res = NULL;
+
   if ((full_slice = PySlice_New(NULL, NULL, NULL)) &&
       (list = PyUpb_RepeatedContainer_Subscript(pself, full_slice)) &&
       (m = PyObject_GetAttrString(list, "sort")) &&
       (res = PyObject_Call(m, args, kwds)) &&
       PyUpb_RepeatedContainer_Assign(pself, list)) {
     Py_INCREF(Py_None);
     ret = Py_None;
```

### Comparing `protobuf-5.26.1/python/repeated.h` & `protobuf-5.27.0rc1/python/repeated.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/python/unknown_fields.c` & `protobuf-5.27.0rc1/python/unknown_fields.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/python/unknown_fields.h` & `protobuf-5.27.0rc1/python/unknown_fields.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/setup.py` & `protobuf-5.27.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/base/descriptor_constants.h` & `protobuf-5.27.0rc1/upb/base/descriptor_constants.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/base/internal/endian.h` & `protobuf-5.27.0rc1/upb/base/internal/endian.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/base/internal/log2.h` & `protobuf-5.27.0rc1/upb/base/internal/log2.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/base/status.c` & `protobuf-5.27.0rc1/upb/base/status.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/base/status.h` & `protobuf-5.27.0rc1/upb/base/status.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/base/string_view.h` & `protobuf-5.27.0rc1/upb/base/string_view.h`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 }
 
 UPB_INLINE bool upb_StringView_IsEqual(upb_StringView a, upb_StringView b) {
   return (a.size == b.size) && (!a.size || !memcmp(a.data, b.data, a.size));
 }
 
 // LINT.ThenChange(
-//  GoogleInternalName0,
+//  GoogleInternalName1,
 //  //depot/google3/third_party/upb/bits/golang/accessor.go:map_go_string,
 //  //depot/google3/third_party/upb/bits/typescript/string_view.ts
 // )
 
 #ifdef __cplusplus
 } /* extern "C" */
 #endif
```

### Comparing `protobuf-5.26.1/upb/base/upcast.h` & `protobuf-5.27.0rc1/upb/base/upcast.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/generated_code_support.h` & `protobuf-5.27.0rc1/upb/generated_code_support.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/hash/common.c` & `protobuf-5.27.0rc1/upb/hash/common.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/hash/common.h` & `protobuf-5.27.0rc1/upb/hash/common.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/hash/int_table.h` & `protobuf-5.27.0rc1/upb/hash/int_table.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/hash/str_table.h` & `protobuf-5.27.0rc1/upb/hash/str_table.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/lex/atoi.c` & `protobuf-5.27.0rc1/upb/lex/atoi.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/lex/atoi.h` & `protobuf-5.27.0rc1/upb/lex/atoi.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/lex/round_trip.c` & `protobuf-5.27.0rc1/upb/lex/round_trip.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/lex/round_trip.h` & `protobuf-5.27.0rc1/upb/lex/round_trip.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/lex/strtod.c` & `protobuf-5.27.0rc1/upb/lex/strtod.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/lex/strtod.h` & `protobuf-5.27.0rc1/upb/lex/strtod.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/lex/unicode.c` & `protobuf-5.27.0rc1/upb/lex/unicode.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/lex/unicode.h` & `protobuf-5.27.0rc1/upb/lex/unicode.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/mem/alloc.c` & `protobuf-5.27.0rc1/upb/mem/alloc.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/mem/alloc.h` & `protobuf-5.27.0rc1/upb/mem/alloc.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/mem/arena.c` & `protobuf-5.27.0rc1/upb/mem/arena.c`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 //
 // Use of this source code is governed by a BSD-style
 // license that can be found in the LICENSE file or at
 // https://developers.google.com/open-source/licenses/bsd
 
 #include "upb/mem/arena.h"
 
+#ifdef UPB_TRACING_ENABLED
+#include <stdatomic.h>
+#endif
+
 #include <stddef.h>
 #include <stdint.h>
 
 #include "upb/mem/alloc.h"
 #include "upb/mem/internal/arena.h"
 #include "upb/port/atomic.h"
 
@@ -113,14 +117,46 @@
   return alloc_uint | (has_initial ? 1 : 0);
 }
 
 static bool _upb_ArenaInternal_HasInitialBlock(upb_ArenaInternal* ai) {
   return ai->block_alloc & 0x1;
 }
 
+#ifdef UPB_TRACING_ENABLED
+static void (*_init_arena_trace_handler)(const upb_Arena*, size_t size) = NULL;
+static void (*_fuse_arena_trace_handler)(const upb_Arena*,
+                                         const upb_Arena*) = NULL;
+static void (*_free_arena_trace_handler)(const upb_Arena*) = NULL;
+
+void upb_Arena_SetTraceHandler(
+    void (*initArenaTraceHandler)(const upb_Arena*, size_t size),
+    void (*fuseArenaTraceHandler)(const upb_Arena*, const upb_Arena*),
+    void (*freeArenaTraceHandler)(const upb_Arena*)) {
+  _init_arena_trace_handler = initArenaTraceHandler;
+  _fuse_arena_trace_handler = fuseArenaTraceHandler;
+  _free_arena_trace_handler = freeArenaTraceHandler;
+}
+
+void upb_Arena_LogInit(const upb_Arena* arena, size_t size) {
+  if (_init_arena_trace_handler) {
+    _init_arena_trace_handler(arena, size);
+  }
+}
+void upb_Arena_LogFuse(const upb_Arena* arena1, const upb_Arena* arena2) {
+  if (_fuse_arena_trace_handler) {
+    _fuse_arena_trace_handler(arena1, arena2);
+  }
+}
+void upb_Arena_LogFree(const upb_Arena* arena) {
+  if (_free_arena_trace_handler) {
+    _free_arena_trace_handler(arena);
+  }
+}
+#endif  // UPB_TRACING_ENABLED
+
 static upb_ArenaRoot _upb_Arena_FindRoot(upb_Arena* a) {
   upb_ArenaInternal* ai = upb_Arena_Internal(a);
   uintptr_t poc = upb_Atomic_Load(&ai->parent_or_count, memory_order_acquire);
   while (_upb_Arena_IsTaggedPointer(poc)) {
     upb_ArenaInternal* next = _upb_Arena_PointerFromTagged(poc);
     UPB_ASSERT(ai != next);
     uintptr_t next_poc =
@@ -170,14 +206,29 @@
     local_fused_count++;
   }
 
   if (fused_count) *fused_count = local_fused_count;
   return memsize;
 }
 
+bool UPB_PRIVATE(_upb_Arena_Contains)(const upb_Arena* a, void* ptr) {
+  upb_ArenaInternal* ai = upb_Arena_Internal(a);
+  UPB_ASSERT(ai);
+
+  upb_MemBlock* block = upb_Atomic_Load(&ai->blocks, memory_order_relaxed);
+  while (block) {
+    uintptr_t beg = (uintptr_t)block;
+    uintptr_t end = beg + block->size;
+    if ((uintptr_t)ptr >= beg && (uintptr_t)ptr < end) return true;
+    block = upb_Atomic_Load(&block->next, memory_order_relaxed);
+  }
+
+  return false;
+}
+
 uint32_t upb_Arena_DebugRefCount(upb_Arena* a) {
   upb_ArenaInternal* ai = upb_Arena_Internal(a);
   // These loads could probably be relaxed, but given that this is debug-only,
   // it's not worth introducing a new variant for it.
   uintptr_t poc = upb_Atomic_Load(&ai->parent_or_count, memory_order_acquire);
   while (_upb_Arena_IsTaggedPointer(poc)) {
     ai = _upb_Arena_PointerFromTagged(poc);
@@ -261,34 +312,41 @@
   }
 
   /* Round block size down to alignof(*a) since we will allocate the arena
    * itself at the end. */
   n = UPB_ALIGN_DOWN(n, UPB_ALIGN_OF(upb_ArenaState));
 
   if (UPB_UNLIKELY(n < sizeof(upb_ArenaState))) {
+#ifdef UPB_TRACING_ENABLED
+    upb_Arena* ret = _upb_Arena_InitSlow(alloc);
+    upb_Arena_LogInit(ret, n);
+    return ret;
+#else
     return _upb_Arena_InitSlow(alloc);
+#endif
   }
 
   a = UPB_PTR_AT(mem, n - sizeof(upb_ArenaState), upb_ArenaState);
 
   upb_Atomic_Init(&a->body.parent_or_count, _upb_Arena_TaggedFromRefcount(1));
   upb_Atomic_Init(&a->body.next, NULL);
   upb_Atomic_Init(&a->body.tail, &a->body);
   upb_Atomic_Init(&a->body.blocks, NULL);
 
   a->body.block_alloc = _upb_Arena_MakeBlockAlloc(alloc, 1);
   a->head.UPB_PRIVATE(ptr) = mem;
   a->head.UPB_PRIVATE(end) = UPB_PTR_AT(mem, n - sizeof(upb_ArenaState), char);
-
+#ifdef UPB_TRACING_ENABLED
+  upb_Arena_LogInit(&a->head, n);
+#endif
   return &a->head;
 }
 
 static void _upb_Arena_DoFree(upb_ArenaInternal* ai) {
   UPB_ASSERT(_upb_Arena_RefCountFromTagged(ai->parent_or_count) == 1);
-
   while (ai != NULL) {
     // Load first since arena itself is likely from one of its blocks.
     upb_ArenaInternal* next_arena =
         (upb_ArenaInternal*)upb_Atomic_Load(&ai->next, memory_order_acquire);
     upb_alloc* block_alloc = _upb_ArenaInternal_BlockAlloc(ai);
     upb_MemBlock* block = upb_Atomic_Load(&ai->blocks, memory_order_acquire);
     while (block != NULL) {
@@ -311,14 +369,17 @@
     poc = upb_Atomic_Load(&ai->parent_or_count, memory_order_acquire);
   }
 
   // compare_exchange or fetch_sub are RMW operations, which are more
   // expensive then direct loads.  As an optimization, we only do RMW ops
   // when we need to update things for other threads to see.
   if (poc == _upb_Arena_TaggedFromRefcount(1)) {
+#ifdef UPB_TRACING_ENABLED
+    upb_Arena_LogFree(a);
+#endif
     _upb_Arena_DoFree(ai);
     return;
   }
 
   if (upb_Atomic_CompareExchangeWeak(
           &ai->parent_or_count, &poc,
           _upb_Arena_TaggedFromRefcount(_upb_Arena_RefCountFromTagged(poc) - 1),
@@ -430,14 +491,18 @@
                                           with_refs, memory_order_relaxed,
                                           memory_order_relaxed);
 }
 
 bool upb_Arena_Fuse(upb_Arena* a1, upb_Arena* a2) {
   if (a1 == a2) return true;  // trivial fuse
 
+#ifdef UPB_TRACING_ENABLED
+  upb_Arena_LogFuse(a1, a2);
+#endif
+
   upb_ArenaInternal* ai1 = upb_Arena_Internal(a1);
   upb_ArenaInternal* ai2 = upb_Arena_Internal(a2);
 
   // Do not fuse initial blocks since we cannot lifetime extend them.
   // Any other fuse scenario is allowed.
   if (_upb_ArenaInternal_HasInitialBlock(ai1) ||
       _upb_ArenaInternal_HasInitialBlock(ai2)) {
```

### Comparing `protobuf-5.26.1/upb/mem/arena.h` & `protobuf-5.27.0rc1/upb/mem/arena.h`

 * *Files 6% similar despite different names*

```diff
@@ -49,31 +49,33 @@
 size_t upb_Arena_SpaceAllocated(upb_Arena* a, size_t* fused_count);
 uint32_t upb_Arena_DebugRefCount(upb_Arena* a);
 
 UPB_API_INLINE upb_Arena* upb_Arena_New(void) {
   return upb_Arena_Init(NULL, 0, &upb_alloc_global);
 }
 
-UPB_API_INLINE void* upb_Arena_Malloc(struct upb_Arena* a, size_t size) {
-  return UPB_PRIVATE(_upb_Arena_Malloc)(a, size);
-}
+UPB_API_INLINE void* upb_Arena_Malloc(struct upb_Arena* a, size_t size);
 
 UPB_API_INLINE void* upb_Arena_Realloc(upb_Arena* a, void* ptr, size_t oldsize,
-                                       size_t size) {
-  return UPB_PRIVATE(_upb_Arena_Realloc)(a, ptr, oldsize, size);
-}
+                                       size_t size);
 
 // Shrinks the last alloc from arena.
 // REQUIRES: (ptr, oldsize) was the last malloc/realloc from this arena.
 // We could also add a upb_Arena_TryShrinkLast() which is simply a no-op if
 // this was not the last alloc.
 UPB_API_INLINE void upb_Arena_ShrinkLast(upb_Arena* a, void* ptr,
-                                         size_t oldsize, size_t size) {
-  UPB_PRIVATE(_upb_Arena_ShrinkLast)(a, ptr, oldsize, size);
-}
+                                         size_t oldsize, size_t size);
+
+#ifdef UPB_TRACING_ENABLED
+void upb_Arena_SetTraceHandler(void (*initArenaTraceHandler)(const upb_Arena*,
+                                                             size_t size),
+                               void (*fuseArenaTraceHandler)(const upb_Arena*,
+                                                             const upb_Arena*),
+                               void (*freeArenaTraceHandler)(const upb_Arena*));
+#endif
 
 #ifdef __cplusplus
 } /* extern "C" */
 #endif
 
 #include "upb/port/undef.inc"
```

### Comparing `protobuf-5.26.1/upb/mem/internal/arena.h` & `protobuf-5.27.0rc1/upb/mem/internal/arena.h`

 * *Files 12% similar despite different names*

```diff
@@ -36,20 +36,24 @@
 #endif
 
 void UPB_PRIVATE(_upb_Arena_SwapIn)(struct upb_Arena* des,
                                     const struct upb_Arena* src);
 void UPB_PRIVATE(_upb_Arena_SwapOut)(struct upb_Arena* des,
                                      const struct upb_Arena* src);
 
+// Returns whether |ptr| was allocated directly by |a| (so care must be used
+// with fused arenas).
+UPB_API bool UPB_ONLYBITS(_upb_Arena_Contains)(const struct upb_Arena* a,
+                                               void* ptr);
+
 UPB_INLINE size_t UPB_PRIVATE(_upb_ArenaHas)(const struct upb_Arena* a) {
   return (size_t)(a->UPB_ONLYBITS(end) - a->UPB_ONLYBITS(ptr));
 }
 
-UPB_INLINE void* UPB_PRIVATE(_upb_Arena_Malloc)(struct upb_Arena* a,
-                                                size_t size) {
+UPB_API_INLINE void* upb_Arena_Malloc(struct upb_Arena* a, size_t size) {
   void* UPB_PRIVATE(_upb_Arena_SlowMalloc)(struct upb_Arena * a, size_t size);
 
   size = UPB_ALIGN_MALLOC(size);
   const size_t span = size + UPB_ASAN_GUARD_SIZE;
   if (UPB_UNLIKELY(UPB_PRIVATE(_upb_ArenaHas)(a) < span)) {
     return UPB_PRIVATE(_upb_Arena_SlowMalloc)(a, span);
   }
@@ -61,16 +65,16 @@
   UPB_UNPOISON_MEMORY_REGION(ret, size);
 
   a->UPB_ONLYBITS(ptr) += span;
 
   return ret;
 }
 
-UPB_INLINE void* UPB_PRIVATE(_upb_Arena_Realloc)(struct upb_Arena* a, void* ptr,
-                                                 size_t oldsize, size_t size) {
+UPB_API_INLINE void* upb_Arena_Realloc(struct upb_Arena* a, void* ptr,
+                                       size_t oldsize, size_t size) {
   oldsize = UPB_ALIGN_MALLOC(oldsize);
   size = UPB_ALIGN_MALLOC(size);
   bool is_most_recent_alloc =
       (uintptr_t)ptr + oldsize == (uintptr_t)a->UPB_ONLYBITS(ptr);
 
   if (is_most_recent_alloc) {
     ptrdiff_t diff = size - oldsize;
@@ -78,26 +82,25 @@
       a->UPB_ONLYBITS(ptr) += diff;
       return ptr;
     }
   } else if (size <= oldsize) {
     return ptr;
   }
 
-  void* ret = UPB_PRIVATE(_upb_Arena_Malloc)(a, size);
+  void* ret = upb_Arena_Malloc(a, size);
 
   if (ret && oldsize > 0) {
     memcpy(ret, ptr, UPB_MIN(oldsize, size));
   }
 
   return ret;
 }
 
-UPB_INLINE void UPB_PRIVATE(_upb_Arena_ShrinkLast)(struct upb_Arena* a,
-                                                   void* ptr, size_t oldsize,
-                                                   size_t size) {
+UPB_API_INLINE void upb_Arena_ShrinkLast(struct upb_Arena* a, void* ptr,
+                                         size_t oldsize, size_t size) {
   oldsize = UPB_ALIGN_MALLOC(oldsize);
   size = UPB_ALIGN_MALLOC(size);
   // Must be the last alloc.
   UPB_ASSERT((char*)ptr + oldsize ==
              a->UPB_ONLYBITS(ptr) - UPB_ASAN_GUARD_SIZE);
   UPB_ASSERT(size <= oldsize);
   a->UPB_ONLYBITS(ptr) = (char*)ptr + size;
```

### Comparing `protobuf-5.26.1/upb/message/accessors.c` & `protobuf-5.27.0rc1/upb/message/accessors.c`

 * *Files 14% similar despite different names*

```diff
@@ -16,26 +16,27 @@
 #include "upb/mini_table/field.h"
 #include "upb/mini_table/message.h"
 #include "upb/mini_table/sub.h"
 
 // Must be last.
 #include "upb/port/def.inc"
 
-bool upb_Message_SetMapEntry(upb_Map* map, const upb_MiniTable* mini_table,
+bool upb_Message_SetMapEntry(upb_Map* map, const upb_MiniTable* m,
                              const upb_MiniTableField* f,
                              upb_Message* map_entry_message, upb_Arena* arena) {
+  UPB_ASSERT(!upb_Message_IsFrozen(map_entry_message));
+
   // TODO: use a variant of upb_MiniTable_GetSubMessageTable() here.
   const upb_MiniTable* map_entry_mini_table = upb_MiniTableSub_Message(
-      mini_table->UPB_PRIVATE(subs)[f->UPB_PRIVATE(submsg_index)]);
+      m->UPB_PRIVATE(subs)[f->UPB_PRIVATE(submsg_index)]);
   UPB_ASSERT(map_entry_mini_table);
-  UPB_ASSERT(map_entry_mini_table->UPB_PRIVATE(field_count) == 2);
   const upb_MiniTableField* map_entry_key_field =
-      &map_entry_mini_table->UPB_PRIVATE(fields)[0];
+      upb_MiniTable_MapKey(map_entry_mini_table);
   const upb_MiniTableField* map_entry_value_field =
-      &map_entry_mini_table->UPB_PRIVATE(fields)[1];
+      upb_MiniTable_MapValue(map_entry_mini_table);
   // Map key/value cannot have explicit defaults,
   // hence assuming a zero default is valid.
   upb_MessageValue default_val;
   memset(&default_val, 0, sizeof(upb_MessageValue));
   upb_MessageValue map_entry_key =
       upb_Message_GetField(map_entry_message, map_entry_key_field, default_val);
   upb_MessageValue map_entry_value = upb_Message_GetField(
```

### Comparing `protobuf-5.26.1/upb/message/accessors.h` & `protobuf-5.27.0rc1/upb/message/accessors.h`

 * *Files 8% similar despite different names*

```diff
@@ -36,38 +36,35 @@
 
 // Functions ending in BaseField() take a (upb_MiniTableField*) argument
 // and work only on non-extension fields.
 //
 // Functions ending in Extension() take a (upb_MiniTableExtension*) argument
 // and work only on extensions.
 
-UPB_API_INLINE void upb_Message_Clear(upb_Message* msg,
-                                      const upb_MiniTable* m) {
-  UPB_PRIVATE(_upb_Message_Clear)(msg, m);
-}
+UPB_API_INLINE void upb_Message_Clear(upb_Message* msg, const upb_MiniTable* m);
 
 UPB_API_INLINE void upb_Message_ClearBaseField(upb_Message* msg,
-                                               const upb_MiniTableField* f) {
-  UPB_PRIVATE(_upb_Message_ClearBaseField)(msg, f);
-}
+                                               const upb_MiniTableField* f);
 
-UPB_API_INLINE void upb_Message_ClearExtension(
-    upb_Message* msg, const upb_MiniTableExtension* e) {
-  UPB_PRIVATE(_upb_Message_ClearExtension)(msg, e);
-}
+UPB_API_INLINE void upb_Message_ClearExtension(upb_Message* msg,
+                                               const upb_MiniTableExtension* e);
 
 UPB_API_INLINE bool upb_Message_HasBaseField(const upb_Message* msg,
-                                             const upb_MiniTableField* f) {
-  return UPB_PRIVATE(_upb_Message_HasBaseField)(msg, f);
-}
+                                             const upb_MiniTableField* f);
 
 UPB_API_INLINE bool upb_Message_HasExtension(const upb_Message* msg,
-                                             const upb_MiniTableExtension* e) {
-  return UPB_PRIVATE(_upb_Message_HasExtension)(msg, e);
-}
+                                             const upb_MiniTableExtension* e);
+
+UPB_API_INLINE void upb_Message_SetBaseField(upb_Message* msg,
+                                             const upb_MiniTableField* f,
+                                             const void* val);
+
+UPB_API_INLINE bool upb_Message_SetExtension(upb_Message* msg,
+                                             const upb_MiniTableExtension* e,
+                                             const void* val, upb_Arena* a);
 
 UPB_API_INLINE uint32_t upb_Message_WhichOneofFieldNumber(
     const upb_Message* message, const upb_MiniTableField* oneof_field) {
   UPB_ASSUME(upb_MiniTableField_IsInOneof(oneof_field));
   return UPB_PRIVATE(_upb_Message_GetOneofCase)(message, oneof_field);
 }
 
@@ -85,22 +82,25 @@
                                    &default_val, &ret);
   } else {
     _upb_Message_GetNonExtensionField(msg, field, &default_val, &ret);
   }
   return ret;
 }
 
-UPB_INLINE bool upb_Message_SetField(upb_Message* msg,
-                                     const upb_MiniTableField* field,
-                                     upb_MessageValue val, upb_Arena* a) {
+// Sets the value of the given field in the given msg. The return value is true
+// if the operation completed successfully, or false if memory allocation
+// failed.
+UPB_INLINE bool UPB_PRIVATE(_upb_Message_SetField)(
+    upb_Message* msg, const upb_MiniTableField* field, upb_MessageValue val,
+    upb_Arena* a) {
   if (upb_MiniTableField_IsExtension(field)) {
     const upb_MiniTableExtension* ext = (const upb_MiniTableExtension*)field;
-    return _upb_Message_SetExtensionField(msg, ext, &val, a);
+    return upb_Message_SetExtension(msg, ext, &val, a);
   } else {
-    _upb_Message_SetNonExtensionField(msg, field, &val);
+    upb_Message_SetBaseField(msg, field, &val);
     return true;
   }
 }
 
 UPB_API_INLINE bool upb_Message_GetBool(const upb_Message* msg,
                                         const upb_MiniTableField* field,
                                         bool default_val) {
@@ -118,15 +118,15 @@
                                         bool value, upb_Arena* a) {
   UPB_ASSUME(upb_MiniTableField_CType(field) == kUpb_CType_Bool);
   UPB_ASSUME(UPB_PRIVATE(_upb_MiniTableField_GetRep)(field) ==
              kUpb_FieldRep_1Byte);
   UPB_ASSUME(upb_MiniTableField_IsScalar(field));
   upb_MessageValue val;
   val.bool_val = value;
-  return upb_Message_SetField(msg, field, val, a);
+  return UPB_PRIVATE(_upb_Message_SetField)(msg, field, val, a);
 }
 
 UPB_API_INLINE int32_t upb_Message_GetInt32(const upb_Message* msg,
                                             const upb_MiniTableField* field,
                                             int32_t default_val) {
   UPB_ASSUME(upb_MiniTableField_CType(field) == kUpb_CType_Int32 ||
              upb_MiniTableField_CType(field) == kUpb_CType_Enum);
@@ -145,15 +145,15 @@
   UPB_ASSUME(upb_MiniTableField_CType(field) == kUpb_CType_Int32 ||
              upb_MiniTableField_CType(field) == kUpb_CType_Enum);
   UPB_ASSUME(UPB_PRIVATE(_upb_MiniTableField_GetRep)(field) ==
              kUpb_FieldRep_4Byte);
   UPB_ASSUME(upb_MiniTableField_IsScalar(field));
   upb_MessageValue val;
   val.int32_val = value;
-  return upb_Message_SetField(msg, field, val, a);
+  return UPB_PRIVATE(_upb_Message_SetField)(msg, field, val, a);
 }
 
 UPB_API_INLINE uint32_t upb_Message_GetUInt32(const upb_Message* msg,
                                               const upb_MiniTableField* field,
                                               uint32_t default_val) {
   UPB_ASSUME(upb_MiniTableField_CType(field) == kUpb_CType_UInt32);
   UPB_ASSUME(UPB_PRIVATE(_upb_MiniTableField_GetRep)(field) ==
@@ -170,27 +170,27 @@
                                           uint32_t value, upb_Arena* a) {
   UPB_ASSUME(upb_MiniTableField_CType(field) == kUpb_CType_UInt32);
   UPB_ASSUME(UPB_PRIVATE(_upb_MiniTableField_GetRep)(field) ==
              kUpb_FieldRep_4Byte);
   UPB_ASSUME(upb_MiniTableField_IsScalar(field));
   upb_MessageValue val;
   val.uint32_val = value;
-  return upb_Message_SetField(msg, field, val, a);
+  return UPB_PRIVATE(_upb_Message_SetField)(msg, field, val, a);
 }
 
 UPB_API_INLINE void upb_Message_SetClosedEnum(
     upb_Message* msg, const upb_MiniTable* msg_mini_table,
     const upb_MiniTableField* field, int32_t value) {
   UPB_ASSERT(upb_MiniTableField_IsClosedEnum(field));
   UPB_ASSUME(UPB_PRIVATE(_upb_MiniTableField_GetRep)(field) ==
              kUpb_FieldRep_4Byte);
   UPB_ASSUME(upb_MiniTableField_IsScalar(field));
   UPB_ASSERT(upb_MiniTableEnum_CheckValue(
       upb_MiniTable_GetSubEnumTable(msg_mini_table, field), value));
-  _upb_Message_SetNonExtensionField(msg, field, &value);
+  upb_Message_SetBaseField(msg, field, &value);
 }
 
 UPB_API_INLINE int64_t upb_Message_GetInt64(const upb_Message* msg,
                                             const upb_MiniTableField* field,
                                             int64_t default_val) {
   UPB_ASSUME(upb_MiniTableField_CType(field) == kUpb_CType_Int64);
   UPB_ASSUME(UPB_PRIVATE(_upb_MiniTableField_GetRep)(field) ==
@@ -207,15 +207,15 @@
                                          int64_t value, upb_Arena* a) {
   UPB_ASSUME(upb_MiniTableField_CType(field) == kUpb_CType_Int64);
   UPB_ASSUME(UPB_PRIVATE(_upb_MiniTableField_GetRep)(field) ==
              kUpb_FieldRep_8Byte);
   UPB_ASSUME(upb_MiniTableField_IsScalar(field));
   upb_MessageValue val;
   val.int64_val = value;
-  return upb_Message_SetField(msg, field, val, a);
+  return UPB_PRIVATE(_upb_Message_SetField)(msg, field, val, a);
 }
 
 UPB_API_INLINE uint64_t upb_Message_GetUInt64(const upb_Message* msg,
                                               const upb_MiniTableField* field,
                                               uint64_t default_val) {
   UPB_ASSUME(upb_MiniTableField_CType(field) == kUpb_CType_UInt64);
   UPB_ASSUME(UPB_PRIVATE(_upb_MiniTableField_GetRep)(field) ==
@@ -232,15 +232,15 @@
                                           uint64_t value, upb_Arena* a) {
   UPB_ASSUME(upb_MiniTableField_CType(field) == kUpb_CType_UInt64);
   UPB_ASSUME(UPB_PRIVATE(_upb_MiniTableField_GetRep)(field) ==
              kUpb_FieldRep_8Byte);
   UPB_ASSUME(upb_MiniTableField_IsScalar(field));
   upb_MessageValue val;
   val.uint64_val = value;
-  return upb_Message_SetField(msg, field, val, a);
+  return UPB_PRIVATE(_upb_Message_SetField)(msg, field, val, a);
 }
 
 UPB_API_INLINE float upb_Message_GetFloat(const upb_Message* msg,
                                           const upb_MiniTableField* field,
                                           float default_val) {
   UPB_ASSUME(upb_MiniTableField_CType(field) == kUpb_CType_Float);
   UPB_ASSUME(UPB_PRIVATE(_upb_MiniTableField_GetRep)(field) ==
@@ -257,15 +257,15 @@
                                          float value, upb_Arena* a) {
   UPB_ASSUME(upb_MiniTableField_CType(field) == kUpb_CType_Float);
   UPB_ASSUME(UPB_PRIVATE(_upb_MiniTableField_GetRep)(field) ==
              kUpb_FieldRep_4Byte);
   UPB_ASSUME(upb_MiniTableField_IsScalar(field));
   upb_MessageValue val;
   val.float_val = value;
-  return upb_Message_SetField(msg, field, val, a);
+  return UPB_PRIVATE(_upb_Message_SetField)(msg, field, val, a);
 }
 
 UPB_API_INLINE double upb_Message_GetDouble(const upb_Message* msg,
                                             const upb_MiniTableField* field,
                                             double default_val) {
   UPB_ASSUME(upb_MiniTableField_CType(field) == kUpb_CType_Double);
   UPB_ASSUME(UPB_PRIVATE(_upb_MiniTableField_GetRep)(field) ==
@@ -282,15 +282,15 @@
                                           double value, upb_Arena* a) {
   UPB_ASSUME(upb_MiniTableField_CType(field) == kUpb_CType_Double);
   UPB_ASSUME(UPB_PRIVATE(_upb_MiniTableField_GetRep)(field) ==
              kUpb_FieldRep_8Byte);
   UPB_ASSUME(upb_MiniTableField_IsScalar(field));
   upb_MessageValue val;
   val.double_val = value;
-  return upb_Message_SetField(msg, field, val, a);
+  return UPB_PRIVATE(_upb_Message_SetField)(msg, field, val, a);
 }
 
 UPB_API_INLINE upb_StringView
 upb_Message_GetString(const upb_Message* msg, const upb_MiniTableField* field,
                       upb_StringView default_val) {
   UPB_ASSUME(upb_MiniTableField_CType(field) == kUpb_CType_String ||
              upb_MiniTableField_CType(field) == kUpb_CType_Bytes);
@@ -299,25 +299,29 @@
   UPB_ASSUME(upb_MiniTableField_IsScalar(field));
 
   upb_MessageValue def;
   def.str_val = default_val;
   return upb_Message_GetField(msg, field, def).str_val;
 }
 
+// Sets the value of a `string` or `bytes` field. The bytes of the value are not
+// copied, so it is the caller's responsibility to ensure that they remain valid
+// for the lifetime of `msg`. That might be done by copying them into the given
+// arena, or by fusing that arena with the arena the bytes live in, for example.
 UPB_API_INLINE bool upb_Message_SetString(upb_Message* msg,
                                           const upb_MiniTableField* field,
                                           upb_StringView value, upb_Arena* a) {
   UPB_ASSUME(upb_MiniTableField_CType(field) == kUpb_CType_String ||
              upb_MiniTableField_CType(field) == kUpb_CType_Bytes);
   UPB_ASSUME(UPB_PRIVATE(_upb_MiniTableField_GetRep)(field) ==
              kUpb_FieldRep_StringView);
   UPB_ASSUME(upb_MiniTableField_IsScalar(field));
   upb_MessageValue val;
   val.str_val = value;
-  return upb_Message_SetField(msg, field, val, a);
+  return UPB_PRIVATE(_upb_Message_SetField)(msg, field, val, a);
 }
 
 UPB_API_INLINE upb_TaggedMessagePtr upb_Message_GetTaggedMessagePtr(
     const upb_Message* msg, const upb_MiniTableField* field,
     upb_Message* default_val) {
   UPB_ASSUME(upb_MiniTableField_CType(field) == kUpb_CType_Message);
   UPB_ASSUME(UPB_PRIVATE(_upb_MiniTableField_GetRep)(field) ==
@@ -325,36 +329,43 @@
   UPB_ASSUME(upb_MiniTableField_IsScalar(field));
   upb_TaggedMessagePtr tagged;
   _upb_Message_GetNonExtensionField(msg, field, &default_val, &tagged);
   return tagged;
 }
 
 UPB_API_INLINE const upb_Message* upb_Message_GetMessage(
-    const upb_Message* msg, const upb_MiniTableField* field,
-    upb_Message* default_val) {
+    const upb_Message* msg, const upb_MiniTableField* field) {
   upb_TaggedMessagePtr tagged =
-      upb_Message_GetTaggedMessagePtr(msg, field, default_val);
+      upb_Message_GetTaggedMessagePtr(msg, field, NULL);
   return upb_TaggedMessagePtr_GetNonEmptyMessage(tagged);
 }
 
+UPB_API_INLINE upb_Message* upb_Message_GetMutableMessage(
+    upb_Message* msg, const upb_MiniTableField* field) {
+  return (upb_Message*)upb_Message_GetMessage(msg, field);
+}
+
 // For internal use only; users cannot set tagged messages because only the
 // parser and the message copier are allowed to directly create an empty
 // message.
 UPB_API_INLINE void _upb_Message_SetTaggedMessagePtr(
     upb_Message* msg, const upb_MiniTable* mini_table,
     const upb_MiniTableField* field, upb_TaggedMessagePtr sub_message) {
   UPB_ASSUME(upb_MiniTableField_CType(field) == kUpb_CType_Message);
   UPB_ASSUME(UPB_PRIVATE(_upb_MiniTableField_GetRep)(field) ==
              UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte));
   UPB_ASSUME(upb_MiniTableField_IsScalar(field));
   UPB_ASSERT(upb_MiniTableSub_Message(
       mini_table->UPB_PRIVATE(subs)[field->UPB_PRIVATE(submsg_index)]));
-  _upb_Message_SetNonExtensionField(msg, field, &sub_message);
+  upb_Message_SetBaseField(msg, field, &sub_message);
 }
 
+// Sets the value of a message-typed field. The `mini_table` and `field`
+// parameters belong to `msg`, not `sub_message`. The mini_tables of `msg` and
+// `sub_message` must have been linked for this to work correctly.
 UPB_API_INLINE void upb_Message_SetMessage(upb_Message* msg,
                                            const upb_MiniTable* mini_table,
                                            const upb_MiniTableField* field,
                                            upb_Message* sub_message) {
   _upb_Message_SetTaggedMessagePtr(
       msg, mini_table, field,
       UPB_PRIVATE(_upb_TaggedMessagePtr_Pack)(sub_message, false));
@@ -401,15 +412,15 @@
   if (!array) {
     array = UPB_PRIVATE(_upb_Array_New)(
         arena, 4, UPB_PRIVATE(_upb_MiniTableField_ElemSizeLg2)(field));
     // Check again due to: https://godbolt.org/z/7WfaoKG1r
     UPB_PRIVATE(_upb_MiniTableField_CheckIsArray)(field);
     upb_MessageValue val;
     val.array_val = array;
-    upb_Message_SetField(msg, field, val, arena);
+    UPB_PRIVATE(_upb_Message_SetField)(msg, field, val, arena);
   }
   return array;
 }
 
 UPB_API_INLINE void* upb_Message_ResizeArrayUninitialized(
     upb_Message* msg, const upb_MiniTableField* field, size_t size,
     upb_Arena* arena) {
@@ -437,17 +448,17 @@
 }
 
 UPB_API_INLINE upb_Map* upb_Message_GetOrCreateMutableMap(
     upb_Message* msg, const upb_MiniTable* map_entry_mini_table,
     const upb_MiniTableField* field, upb_Arena* arena) {
   UPB_ASSUME(upb_MiniTableField_CType(field) == kUpb_CType_Message);
   const upb_MiniTableField* map_entry_key_field =
-      &map_entry_mini_table->UPB_PRIVATE(fields)[0];
+      &map_entry_mini_table->UPB_ONLYBITS(fields)[0];
   const upb_MiniTableField* map_entry_value_field =
-      &map_entry_mini_table->UPB_PRIVATE(fields)[1];
+      &map_entry_mini_table->UPB_ONLYBITS(fields)[1];
   return _upb_Message_GetOrCreateMutableMap(
       msg, field,
       _upb_Map_CTypeSize(upb_MiniTableField_CType(map_entry_key_field)),
       _upb_Map_CTypeSize(upb_MiniTableField_CType(map_entry_value_field)),
       arena);
 }
```

### Comparing `protobuf-5.26.1/upb/message/accessors_split64.h` & `protobuf-5.27.0rc1/upb/message/accessors_split64.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/message/array.c` & `protobuf-5.27.0rc1/upb/message/array.c`

 * *Files 14% similar despite different names*

```diff
@@ -9,68 +9,75 @@
 
 #include <stdint.h>
 #include <string.h>
 
 #include "upb/base/descriptor_constants.h"
 #include "upb/mem/arena.h"
 #include "upb/message/internal/array.h"
+#include "upb/message/message.h"
+#include "upb/mini_table/field.h"
 #include "upb/mini_table/internal/size_log2.h"
+#include "upb/mini_table/message.h"
 
 // Must be last.
 #include "upb/port/def.inc"
 
 upb_Array* upb_Array_New(upb_Arena* a, upb_CType type) {
   const int lg2 = UPB_PRIVATE(_upb_CType_SizeLg2)(type);
   return UPB_PRIVATE(_upb_Array_New)(a, 4, lg2);
 }
 
 upb_MessageValue upb_Array_Get(const upb_Array* arr, size_t i) {
+  UPB_ASSERT(i < upb_Array_Size(arr));
   upb_MessageValue ret;
   const char* data = upb_Array_DataPtr(arr);
   const int lg2 = UPB_PRIVATE(_upb_Array_ElemSizeLg2)(arr);
-  UPB_ASSERT(i < arr->UPB_PRIVATE(size));
   memcpy(&ret, data + (i << lg2), 1 << lg2);
   return ret;
 }
 
 upb_MutableMessageValue upb_Array_GetMutable(upb_Array* arr, size_t i) {
+  UPB_ASSERT(i < upb_Array_Size(arr));
   upb_MutableMessageValue ret;
   char* data = upb_Array_MutableDataPtr(arr);
   const int lg2 = UPB_PRIVATE(_upb_Array_ElemSizeLg2)(arr);
-  UPB_ASSERT(i < arr->UPB_PRIVATE(size));
   memcpy(&ret, data + (i << lg2), 1 << lg2);
   return ret;
 }
 
 void upb_Array_Set(upb_Array* arr, size_t i, upb_MessageValue val) {
+  UPB_ASSERT(!upb_Array_IsFrozen(arr));
+  UPB_ASSERT(i < upb_Array_Size(arr));
   char* data = upb_Array_MutableDataPtr(arr);
   const int lg2 = UPB_PRIVATE(_upb_Array_ElemSizeLg2)(arr);
-  UPB_ASSERT(i < arr->UPB_PRIVATE(size));
   memcpy(data + (i << lg2), &val, 1 << lg2);
 }
 
 bool upb_Array_Append(upb_Array* arr, upb_MessageValue val, upb_Arena* arena) {
+  UPB_ASSERT(!upb_Array_IsFrozen(arr));
   UPB_ASSERT(arena);
   if (!UPB_PRIVATE(_upb_Array_ResizeUninitialized)(
           arr, arr->UPB_PRIVATE(size) + 1, arena)) {
     return false;
   }
   upb_Array_Set(arr, arr->UPB_PRIVATE(size) - 1, val);
   return true;
 }
 
 void upb_Array_Move(upb_Array* arr, size_t dst_idx, size_t src_idx,
                     size_t count) {
+  UPB_ASSERT(!upb_Array_IsFrozen(arr));
   const int lg2 = UPB_PRIVATE(_upb_Array_ElemSizeLg2)(arr);
   char* data = upb_Array_MutableDataPtr(arr);
   memmove(&data[dst_idx << lg2], &data[src_idx << lg2], count << lg2);
 }
 
 bool upb_Array_Insert(upb_Array* arr, size_t i, size_t count,
                       upb_Arena* arena) {
+  UPB_ASSERT(!upb_Array_IsFrozen(arr));
   UPB_ASSERT(arena);
   UPB_ASSERT(i <= arr->UPB_PRIVATE(size));
   UPB_ASSERT(count + arr->UPB_PRIVATE(size) >= count);
   const size_t oldsize = arr->UPB_PRIVATE(size);
   if (!UPB_PRIVATE(_upb_Array_ResizeUninitialized)(
           arr, arr->UPB_PRIVATE(size) + count, arena)) {
     return false;
@@ -80,22 +87,24 @@
 }
 
 /*
  *              i        end      arr->size
  * |------------|XXXXXXXX|--------|
  */
 void upb_Array_Delete(upb_Array* arr, size_t i, size_t count) {
+  UPB_ASSERT(!upb_Array_IsFrozen(arr));
   const size_t end = i + count;
   UPB_ASSERT(i <= end);
   UPB_ASSERT(end <= arr->UPB_PRIVATE(size));
   upb_Array_Move(arr, i, end, arr->UPB_PRIVATE(size) - end);
   arr->UPB_PRIVATE(size) -= count;
 }
 
 bool upb_Array_Resize(upb_Array* arr, size_t size, upb_Arena* arena) {
+  UPB_ASSERT(!upb_Array_IsFrozen(arr));
   const size_t oldsize = arr->UPB_PRIVATE(size);
   if (UPB_UNLIKELY(
           !UPB_PRIVATE(_upb_Array_ResizeUninitialized)(arr, size, arena))) {
     return false;
   }
   const size_t newsize = arr->UPB_PRIVATE(size);
   if (newsize > oldsize) {
@@ -120,7 +129,21 @@
   ptr = upb_Arena_Realloc(arena, ptr, old_bytes, new_bytes);
   if (!ptr) return false;
 
   UPB_PRIVATE(_upb_Array_SetTaggedPtr)(array, ptr, lg2);
   array->UPB_PRIVATE(capacity) = new_capacity;
   return true;
 }
+
+void upb_Array_Freeze(upb_Array* arr, const upb_MiniTable* m) {
+  if (upb_Array_IsFrozen(arr)) return;
+  UPB_PRIVATE(_upb_Array_ShallowFreeze)(arr);
+
+  if (m) {
+    const size_t size = upb_Array_Size(arr);
+
+    for (size_t i = 0; i < size; i++) {
+      upb_MessageValue val = upb_Array_Get(arr, i);
+      upb_Message_Freeze((upb_Message*)val.msg_val, m);
+    }
+  }
+}
```

### Comparing `protobuf-5.26.1/upb/message/array.h` & `protobuf-5.27.0rc1/upb/message/array.h`

 * *Files 24% similar despite different names*

```diff
@@ -10,31 +10,31 @@
 
 #include <stddef.h>
 
 #include "upb/base/descriptor_constants.h"
 #include "upb/mem/arena.h"
 #include "upb/message/internal/array.h"
 #include "upb/message/value.h"
+#include "upb/mini_table/field.h"
+#include "upb/mini_table/message.h"
 
 // Must be last.
 #include "upb/port/def.inc"
 
 typedef struct upb_Array upb_Array;
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 // Creates a new array on the given arena that holds elements of this type.
 UPB_API upb_Array* upb_Array_New(upb_Arena* a, upb_CType type);
 
 // Returns the number of elements in the array.
-UPB_API_INLINE size_t upb_Array_Size(const upb_Array* arr) {
-  return UPB_PRIVATE(_upb_Array_Size)(arr);
-}
+UPB_API_INLINE size_t upb_Array_Size(const upb_Array* arr);
 
 // Returns the given element, which must be within the array's current size.
 UPB_API upb_MessageValue upb_Array_Get(const upb_Array* arr, size_t i);
 
 // Returns a mutating pointer to the given element, which must be within the
 // array's current size.
 UPB_API upb_MutableMessageValue upb_Array_GetMutable(upb_Array* arr, size_t i);
@@ -59,27 +59,35 @@
                               upb_Arena* arena);
 
 // Deletes one or more elements from the array.
 // Existing elements are shifted left.
 // REQUIRES: `i + count <= upb_Array_Size(arr)`
 UPB_API void upb_Array_Delete(upb_Array* array, size_t i, size_t count);
 
+// Reserves |size| elements of storage for the array.
+UPB_API_INLINE bool upb_Array_Reserve(struct upb_Array* array, size_t size,
+                                      upb_Arena* arena);
+
 // Changes the size of a vector. New elements are initialized to NULL/0.
 // Returns false on allocation failure.
 UPB_API bool upb_Array_Resize(upb_Array* array, size_t size, upb_Arena* arena);
 
 // Returns pointer to array data.
-UPB_API_INLINE const void* upb_Array_DataPtr(const upb_Array* arr) {
-  return UPB_PRIVATE(_upb_Array_DataPtr)(arr);
-}
+UPB_API_INLINE const void* upb_Array_DataPtr(const upb_Array* arr);
 
 // Returns mutable pointer to array data.
-UPB_API_INLINE void* upb_Array_MutableDataPtr(upb_Array* arr) {
-  return UPB_PRIVATE(_upb_Array_MutableDataPtr)(arr);
-}
+UPB_API_INLINE void* upb_Array_MutableDataPtr(upb_Array* arr);
+
+// Mark an array and all of its descendents as frozen/immutable.
+// If the array elements are messages then |m| must point to the minitable for
+// those messages. Otherwise |m| must be NULL.
+UPB_API void upb_Array_Freeze(upb_Array* arr, const upb_MiniTable* m);
+
+// Returns whether an array has been frozen.
+UPB_API_INLINE bool upb_Array_IsFrozen(const upb_Array* arr);
 
 #ifdef __cplusplus
 } /* extern "C" */
 #endif
 
 #include "upb/port/undef.inc"
```

### Comparing `protobuf-5.26.1/upb/message/compat.c` & `protobuf-5.27.0rc1/upb/message/compat.c`

 * *Files 18% similar despite different names*

```diff
@@ -22,18 +22,18 @@
   size_t count;
   const upb_Extension* ext = UPB_PRIVATE(_upb_Message_Getexts)(msg, &count);
 
   UPB_ASSERT(index < count);
   return ext[index].ext;
 }
 
-const upb_Extension* upb_Message_FindExtensionByNumber(const upb_Message* msg,
-                                                       uint32_t field_number) {
+const upb_MiniTableExtension* upb_Message_FindExtensionByNumber(
+    const upb_Message* msg, uint32_t field_number) {
   size_t count;
   const upb_Extension* ext = UPB_PRIVATE(_upb_Message_Getexts)(msg, &count);
 
-  while (count--) {
-    if (upb_MiniTableExtension_Number(ext->ext) == field_number) return ext;
-    ext++;
+  for (; count--; ext++) {
+    const upb_MiniTableExtension* e = ext->ext;
+    if (upb_MiniTableExtension_Number(e) == field_number) return e;
   }
   return NULL;
 }
```

### Comparing `protobuf-5.26.1/upb/message/compat.h` & `protobuf-5.27.0rc1/upb/message/compat.h`

 * *Files 11% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 const upb_MiniTableExtension* upb_Message_ExtensionByIndex(
     const upb_Message* msg, size_t index);
 
-// Returns the extension with the given field number, or NULL on failure.
-const upb_Extension* upb_Message_FindExtensionByNumber(const upb_Message* msg,
-                                                       uint32_t field_number);
+// Returns the minitable with the given field number, or NULL on failure.
+const upb_MiniTableExtension* upb_Message_FindExtensionByNumber(
+    const upb_Message* msg, uint32_t field_number);
 
 #ifdef __cplusplus
 } /* extern "C" */
 #endif
 
 #include "upb/port/undef.inc"
```

### Comparing `protobuf-5.26.1/upb/message/copy.c` & `protobuf-5.27.0rc1/upb/message/copy.c`

 * *Files 4% similar despite different names*

```diff
@@ -92,15 +92,15 @@
   if (cloned_map == NULL) {
     return NULL;
   }
   upb_MessageValue key, val;
   size_t iter = kUpb_Map_Begin;
   while (upb_Map_Next(map, &key, &val, &iter)) {
     const upb_MiniTableField* value_field =
-        &map_entry_table->UPB_PRIVATE(fields)[1];
+        upb_MiniTable_MapValue(map_entry_table);
     const upb_MiniTable* value_sub =
         upb_MiniTableField_CType(value_field) == kUpb_CType_Message
             ? upb_MiniTable_GetSubMessageTable(map_entry_table, value_field)
             : NULL;
     upb_CType value_field_type = upb_MiniTableField_CType(value_field);
     if (!upb_Clone_MessageValue(&val, value_field_type, value_sub, arena)) {
       return NULL;
@@ -118,32 +118,31 @@
                                           upb_Message* clone,
                                           upb_Arena* arena) {
   // TODO: use a variant of upb_MiniTable_GetSubMessageTable() here.
   const upb_MiniTable* map_entry_table = upb_MiniTableSub_Message(
       mini_table->UPB_PRIVATE(subs)[f->UPB_PRIVATE(submsg_index)]);
   UPB_ASSERT(map_entry_table);
 
-  const upb_MiniTableField* key_field =
-      &map_entry_table->UPB_PRIVATE(fields)[0];
+  const upb_MiniTableField* key_field = upb_MiniTable_MapKey(map_entry_table);
   const upb_MiniTableField* value_field =
-      &map_entry_table->UPB_PRIVATE(fields)[1];
+      upb_MiniTable_MapValue(map_entry_table);
 
   upb_Map* cloned_map = upb_Map_DeepClone(
       map, upb_MiniTableField_CType(key_field),
       upb_MiniTableField_CType(value_field), map_entry_table, arena);
   if (!cloned_map) {
     return NULL;
   }
-  _upb_Message_SetNonExtensionField(clone, f, &cloned_map);
+  upb_Message_SetBaseField(clone, f, &cloned_map);
   return cloned_map;
 }
 
 upb_Array* upb_Array_DeepClone(const upb_Array* array, upb_CType value_type,
                                const upb_MiniTable* sub, upb_Arena* arena) {
-  const size_t size = array->UPB_PRIVATE(size);
+  const size_t size = upb_Array_Size(array);
   const int lg2 = UPB_PRIVATE(_upb_CType_SizeLg2)(value_type);
   upb_Array* cloned_array = UPB_PRIVATE(_upb_Array_New)(arena, size, lg2);
   if (!cloned_array) {
     return NULL;
   }
   if (!UPB_PRIVATE(_upb_Array_ResizeUninitialized)(cloned_array, size, arena)) {
     return NULL;
@@ -167,36 +166,36 @@
       array, upb_MiniTableField_CType(field),
       upb_MiniTableField_CType(field) == kUpb_CType_Message
           ? upb_MiniTable_GetSubMessageTable(mini_table, field)
           : NULL,
       arena);
 
   // Clear out upb_Array* due to parent memcpy.
-  _upb_Message_SetNonExtensionField(clone, field, &cloned_array);
+  upb_Message_SetBaseField(clone, field, &cloned_array);
   return true;
 }
 
 static bool upb_Clone_ExtensionValue(
     const upb_MiniTableExtension* mini_table_ext, const upb_Extension* source,
     upb_Extension* dest, upb_Arena* arena) {
   dest->data = source->data;
   return upb_Clone_MessageValue(
-      &dest->data,
-      upb_MiniTableField_CType(&mini_table_ext->UPB_PRIVATE(field)),
+      &dest->data, upb_MiniTableExtension_CType(mini_table_ext),
       upb_MiniTableExtension_GetSubMessage(mini_table_ext), arena);
 }
 
 upb_Message* _upb_Message_Copy(upb_Message* dst, const upb_Message* src,
                                const upb_MiniTable* mini_table,
                                upb_Arena* arena) {
   upb_StringView empty_string = upb_StringView_FromDataAndSize(NULL, 0);
   // Only copy message area skipping upb_Message_Internal.
   memcpy(dst + 1, src + 1, mini_table->UPB_PRIVATE(size) - sizeof(upb_Message));
-  for (size_t i = 0; i < mini_table->UPB_PRIVATE(field_count); ++i) {
-    const upb_MiniTableField* field = &mini_table->UPB_PRIVATE(fields)[i];
+  for (int i = 0; i < upb_MiniTable_FieldCount(mini_table); ++i) {
+    const upb_MiniTableField* field =
+        upb_MiniTable_GetFieldByIndex(mini_table, i);
     if (upb_MiniTableField_IsScalar(field)) {
       switch (upb_MiniTableField_CType(field)) {
         case kUpb_CType_Message: {
           upb_TaggedMessagePtr tagged =
               upb_Message_GetTaggedMessagePtr(src, field, NULL);
           const upb_Message* sub_message =
               UPB_PRIVATE(_upb_TaggedMessagePtr_GetMessage)(tagged);
@@ -262,23 +261,23 @@
         dst, msg_ext->ext, arena);
     if (!dst_ext) return NULL;
     if (upb_MiniTableField_IsScalar(field)) {
       if (!upb_Clone_ExtensionValue(msg_ext->ext, msg_ext, dst_ext, arena)) {
         return NULL;
       }
     } else {
-      upb_Array* msg_array = (upb_Array*)msg_ext->data.ptr;
+      upb_Array* msg_array = (upb_Array*)msg_ext->data.array_val;
       UPB_ASSERT(msg_array);
       upb_Array* cloned_array = upb_Array_DeepClone(
           msg_array, upb_MiniTableField_CType(field),
           upb_MiniTableExtension_GetSubMessage(msg_ext->ext), arena);
       if (!cloned_array) {
         return NULL;
       }
-      dst_ext->data.ptr = (void*)cloned_array;
+      dst_ext->data.array_val = cloned_array;
     }
   }
 
   // Clone unknowns.
   size_t unknown_size = 0;
   const char* ptr = upb_Message_GetUnknown(src, &unknown_size);
   if (unknown_size != 0) {
```

### Comparing `protobuf-5.26.1/upb/message/copy.h` & `protobuf-5.27.0rc1/upb/message/copy.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/message/internal/accessors.h` & `protobuf-5.27.0rc1/upb/message/internal/accessors.h`

 * *Files 6% similar despite different names*

```diff
@@ -198,15 +198,15 @@
 // we are left with ideal code.  This can happen either through through
 // literals or UPB_ASSUME():
 //
 //   // Via struct literals.
 //   bool FooMessage_set_bool_field(const upb_Message* msg, bool val) {
 //     const upb_MiniTableField field = {1, 0, 0, /* etc... */};
 //     // All value in "field" are compile-time known.
-//     _upb_Message_SetNonExtensionField(msg, &field, &value);
+//     upb_Message_SetBaseField(msg, &field, &value);
 //   }
 //
 //   // Via UPB_ASSUME().
 //   UPB_INLINE bool upb_Message_SetBool(upb_Message* msg,
 //                                       const upb_MiniTableField* field,
 //                                       bool value, upb_Arena* a) {
 //     UPB_ASSUME(field->UPB_PRIVATE(descriptortype) == kUpb_FieldType_Bool);
@@ -221,123 +221,133 @@
 // exception is the binary encoder/decoder, which need to be a bit more clever
 // about how they read/write the message data, for efficiency.
 //
 // These functions work on both extensions and non-extensions. If the field
 // of a setter is known to be a non-extension, the arena may be NULL and the
 // returned bool value may be ignored since it will always succeed.
 
-UPB_INLINE bool UPB_PRIVATE(_upb_Message_HasBaseField)(
-    const struct upb_Message* msg, const upb_MiniTableField* field) {
+UPB_API_INLINE bool upb_Message_HasBaseField(const struct upb_Message* msg,
+                                             const upb_MiniTableField* field) {
   UPB_ASSERT(upb_MiniTableField_HasPresence(field));
   UPB_ASSUME(!upb_MiniTableField_IsExtension(field));
   if (upb_MiniTableField_IsInOneof(field)) {
     return UPB_PRIVATE(_upb_Message_GetOneofCase)(msg, field) ==
            upb_MiniTableField_Number(field);
   } else {
     return UPB_PRIVATE(_upb_Message_GetHasbit)(msg, field);
   }
 }
 
-UPB_INLINE bool UPB_PRIVATE(_upb_Message_HasExtension)(
-    const struct upb_Message* msg, const upb_MiniTableExtension* ext) {
-  UPB_ASSERT(upb_MiniTableField_HasPresence(&ext->UPB_PRIVATE(field)));
-  return UPB_PRIVATE(_upb_Message_Getext)(msg, ext) != NULL;
+UPB_API_INLINE bool upb_Message_HasExtension(const struct upb_Message* msg,
+                                             const upb_MiniTableExtension* e) {
+  UPB_ASSERT(upb_MiniTableField_HasPresence(&e->UPB_PRIVATE(field)));
+  return UPB_PRIVATE(_upb_Message_Getext)(msg, e) != NULL;
 }
 
-static UPB_FORCEINLINE void _upb_Message_GetNonExtensionField(
+UPB_FORCEINLINE void _upb_Message_GetNonExtensionField(
     const struct upb_Message* msg, const upb_MiniTableField* field,
     const void* default_val, void* val) {
   UPB_ASSUME(!upb_MiniTableField_IsExtension(field));
   if ((upb_MiniTableField_IsInOneof(field) ||
        !UPB_PRIVATE(_upb_MiniTableField_DataIsZero)(field, default_val)) &&
-      !UPB_PRIVATE(_upb_Message_HasBaseField)(msg, field)) {
+      !upb_Message_HasBaseField(msg, field)) {
     UPB_PRIVATE(_upb_MiniTableField_DataCopy)(field, val, default_val);
     return;
   }
   UPB_PRIVATE(_upb_MiniTableField_DataCopy)
   (field, val, UPB_PRIVATE(_upb_Message_DataPtr)(msg, field));
 }
 
 UPB_INLINE void _upb_Message_GetExtensionField(
     const struct upb_Message* msg, const upb_MiniTableExtension* mt_ext,
     const void* default_val, void* val) {
-  const struct upb_Extension* ext =
-      UPB_PRIVATE(_upb_Message_Getext)(msg, mt_ext);
+  const upb_Extension* ext = UPB_PRIVATE(_upb_Message_Getext)(msg, mt_ext);
   const upb_MiniTableField* f = &mt_ext->UPB_PRIVATE(field);
   UPB_ASSUME(upb_MiniTableField_IsExtension(f));
 
   if (ext) {
     UPB_PRIVATE(_upb_MiniTableField_DataCopy)(f, val, &ext->data);
   } else {
     UPB_PRIVATE(_upb_MiniTableField_DataCopy)(f, val, default_val);
   }
 }
 
-UPB_INLINE void _upb_Message_SetNonExtensionField(
-    struct upb_Message* msg, const upb_MiniTableField* field, const void* val) {
-  UPB_ASSUME(!upb_MiniTableField_IsExtension(field));
-  UPB_PRIVATE(_upb_Message_SetPresence)(msg, field);
+UPB_API_INLINE void upb_Message_SetBaseField(struct upb_Message* msg,
+                                             const upb_MiniTableField* f,
+                                             const void* val) {
+  UPB_ASSERT(!upb_Message_IsFrozen(msg));
+  UPB_ASSUME(!upb_MiniTableField_IsExtension(f));
+  UPB_PRIVATE(_upb_Message_SetPresence)(msg, f);
   UPB_PRIVATE(_upb_MiniTableField_DataCopy)
-  (field, UPB_PRIVATE(_upb_Message_MutableDataPtr)(msg, field), val);
+  (f, UPB_PRIVATE(_upb_Message_MutableDataPtr)(msg, f), val);
 }
 
-UPB_INLINE bool _upb_Message_SetExtensionField(
-    struct upb_Message* msg, const upb_MiniTableExtension* mt_ext,
-    const void* val, upb_Arena* a) {
+UPB_API_INLINE bool upb_Message_SetExtension(struct upb_Message* msg,
+                                             const upb_MiniTableExtension* e,
+                                             const void* val, upb_Arena* a) {
+  UPB_ASSERT(!upb_Message_IsFrozen(msg));
   UPB_ASSERT(a);
-  struct upb_Extension* ext =
-      UPB_PRIVATE(_upb_Message_GetOrCreateExtension)(msg, mt_ext, a);
+  upb_Extension* ext =
+      UPB_PRIVATE(_upb_Message_GetOrCreateExtension)(msg, e, a);
   if (!ext) return false;
   UPB_PRIVATE(_upb_MiniTableField_DataCopy)
-  (&mt_ext->UPB_PRIVATE(field), &ext->data, val);
+  (&e->UPB_PRIVATE(field), &ext->data, val);
   return true;
 }
 
-UPB_INLINE void UPB_PRIVATE(_upb_Message_Clear)(struct upb_Message* msg,
-                                                const upb_MiniTable* m) {
+UPB_API_INLINE void upb_Message_Clear(struct upb_Message* msg,
+                                      const upb_MiniTable* m) {
+  UPB_ASSERT(!upb_Message_IsFrozen(msg));
+  upb_Message_Internal* in = UPB_PRIVATE(_upb_Message_GetInternal)(msg);
   memset(msg, 0, m->UPB_PRIVATE(size));
+  if (in) {
+    // Reset the internal buffer to empty.
+    in->unknown_end = sizeof(upb_Message_Internal);
+    in->ext_begin = in->size;
+    UPB_PRIVATE(_upb_Message_SetInternal)(msg, in);
+  }
 }
 
-UPB_INLINE void UPB_PRIVATE(_upb_Message_ClearBaseField)(
-    struct upb_Message* msg, const upb_MiniTableField* f) {
+UPB_API_INLINE void upb_Message_ClearBaseField(struct upb_Message* msg,
+                                               const upb_MiniTableField* f) {
+  UPB_ASSERT(!upb_Message_IsFrozen(msg));
   if (UPB_PRIVATE(_upb_MiniTableField_HasHasbit)(f)) {
     UPB_PRIVATE(_upb_Message_ClearHasbit)(msg, f);
   } else if (upb_MiniTableField_IsInOneof(f)) {
     uint32_t* ptr = UPB_PRIVATE(_upb_Message_OneofCasePtr)(msg, f);
     if (*ptr != upb_MiniTableField_Number(f)) return;
     *ptr = 0;
   }
   const char zeros[16] = {0};
   UPB_PRIVATE(_upb_MiniTableField_DataCopy)
   (f, UPB_PRIVATE(_upb_Message_MutableDataPtr)(msg, f), zeros);
 }
 
-UPB_INLINE void UPB_PRIVATE(_upb_Message_ClearExtension)(
+UPB_API_INLINE void upb_Message_ClearExtension(
     struct upb_Message* msg, const upb_MiniTableExtension* e) {
-  upb_Message_Internal* in = msg->internal;
+  UPB_ASSERT(!upb_Message_IsFrozen(msg));
+  upb_Message_Internal* in = UPB_PRIVATE(_upb_Message_GetInternal)(msg);
   if (!in) return;
-  const struct upb_Extension* base =
-      UPB_PTR_AT(in, in->ext_begin, struct upb_Extension);
-  struct upb_Extension* ext =
-      (struct upb_Extension*)UPB_PRIVATE(_upb_Message_Getext)(msg, e);
+  const upb_Extension* base = UPB_PTR_AT(in, in->ext_begin, upb_Extension);
+  upb_Extension* ext = (upb_Extension*)UPB_PRIVATE(_upb_Message_Getext)(msg, e);
   if (ext) {
     *ext = *base;
-    in->ext_begin += sizeof(struct upb_Extension);
+    in->ext_begin += sizeof(upb_Extension);
   }
 }
 
 UPB_INLINE void _upb_Message_AssertMapIsUntagged(
     const struct upb_Message* msg, const upb_MiniTableField* field) {
   UPB_UNUSED(msg);
   UPB_PRIVATE(_upb_MiniTableField_CheckIsMap)(field);
 #ifndef NDEBUG
   uintptr_t default_val = 0;
   uintptr_t tagged;
   _upb_Message_GetNonExtensionField(msg, field, &default_val, &tagged);
-  UPB_ASSERT(!UPB_PRIVATE(_upb_TaggedMessagePtr_IsEmpty)(tagged));
+  UPB_ASSERT(!upb_TaggedMessagePtr_IsEmpty(tagged));
 #endif
 }
 
 UPB_INLINE struct upb_Map* _upb_Message_GetOrCreateMutableMap(
     struct upb_Message* msg, const upb_MiniTableField* field, size_t key_size,
     size_t val_size, upb_Arena* arena) {
   UPB_PRIVATE(_upb_MiniTableField_CheckIsMap)(field);
@@ -345,15 +355,15 @@
   struct upb_Map* map = NULL;
   struct upb_Map* default_map_value = NULL;
   _upb_Message_GetNonExtensionField(msg, field, &default_map_value, &map);
   if (!map) {
     map = _upb_Map_New(arena, key_size, val_size);
     // Check again due to: https://godbolt.org/z/7WfaoKG1r
     UPB_PRIVATE(_upb_MiniTableField_CheckIsMap)(field);
-    _upb_Message_SetNonExtensionField(msg, field, &map);
+    upb_Message_SetBaseField(msg, field, &map);
   }
   return map;
 }
 
 #ifdef __cplusplus
 } /* extern "C" */
 #endif
```

### Comparing `protobuf-5.26.1/upb/message/internal/array.h` & `protobuf-5.27.0rc1/upb/message/internal/array.h`

 * *Files 7% similar despite different names*

```diff
@@ -20,30 +20,39 @@
 #define _UPB_ARRAY_MASK_LG2 0x3  // Encoded elem size.
 #define _UPB_ARRAY_MASK_ALL (_UPB_ARRAY_MASK_IMM | _UPB_ARRAY_MASK_LG2)
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
-// LINT.IfChange(struct_definition)
+// LINT.IfChange(upb_Array)
+
 // Our internal representation for repeated fields.
 struct upb_Array {
   // This is a tagged pointer. Bits #0 and #1 encode the elem size as follows:
   //   0 maps to elem size 1
   //   1 maps to elem size 4
   //   2 maps to elem size 8
   //   3 maps to elem size 16
   //
-  // Bit #2 contains the frozen/immutable flag (currently unimplemented).
+  // Bit #2 contains the frozen/immutable flag.
   uintptr_t UPB_ONLYBITS(data);
 
   size_t UPB_ONLYBITS(size);     // The number of elements in the array.
   size_t UPB_PRIVATE(capacity);  // Allocated storage. Measured in elements.
 };
 
+UPB_INLINE void UPB_PRIVATE(_upb_Array_ShallowFreeze)(struct upb_Array* arr) {
+  arr->UPB_ONLYBITS(data) |= _UPB_ARRAY_MASK_IMM;
+}
+
+UPB_API_INLINE bool upb_Array_IsFrozen(const struct upb_Array* arr) {
+  return (arr->UPB_ONLYBITS(data) & _UPB_ARRAY_MASK_IMM) != 0;
+}
+
 UPB_INLINE void UPB_PRIVATE(_upb_Array_SetTaggedPtr)(struct upb_Array* array,
                                                      void* data, size_t lg2) {
   UPB_ASSERT(lg2 != 1);
   UPB_ASSERT(lg2 <= 4);
   const size_t bits = lg2 - (lg2 != 0);
   array->UPB_ONLYBITS(data) = (uintptr_t)data | bits;
 }
@@ -51,23 +60,21 @@
 UPB_INLINE size_t
 UPB_PRIVATE(_upb_Array_ElemSizeLg2)(const struct upb_Array* array) {
   const size_t bits = array->UPB_ONLYBITS(data) & _UPB_ARRAY_MASK_LG2;
   const size_t lg2 = bits + (bits != 0);
   return lg2;
 }
 
-UPB_INLINE const void* UPB_PRIVATE(_upb_Array_DataPtr)(
-    const struct upb_Array* array) {
+UPB_API_INLINE const void* upb_Array_DataPtr(const struct upb_Array* array) {
   UPB_PRIVATE(_upb_Array_ElemSizeLg2)(array);  // Check assertions.
   return (void*)(array->UPB_ONLYBITS(data) & ~(uintptr_t)_UPB_ARRAY_MASK_ALL);
 }
 
-UPB_INLINE void* UPB_PRIVATE(_upb_Array_MutableDataPtr)(
-    struct upb_Array* array) {
-  return (void*)UPB_PRIVATE(_upb_Array_DataPtr)(array);
+UPB_API_INLINE void* upb_Array_MutableDataPtr(struct upb_Array* array) {
+  return (void*)upb_Array_DataPtr(array);
 }
 
 UPB_INLINE struct upb_Array* UPB_PRIVATE(_upb_Array_New)(upb_Arena* arena,
                                                          size_t init_capacity,
                                                          int elem_size_lg2) {
   UPB_ASSERT(elem_size_lg2 != 1);
   UPB_ASSERT(elem_size_lg2 <= 4);
@@ -83,50 +90,51 @@
   return array;
 }
 
 // Resizes the capacity of the array to be at least min_size.
 bool UPB_PRIVATE(_upb_Array_Realloc)(struct upb_Array* array, size_t min_size,
                                      upb_Arena* arena);
 
-UPB_INLINE bool UPB_PRIVATE(_upb_Array_Reserve)(struct upb_Array* array,
-                                                size_t size, upb_Arena* arena) {
+UPB_API_INLINE bool upb_Array_Reserve(struct upb_Array* array, size_t size,
+                                      upb_Arena* arena) {
+  UPB_ASSERT(!upb_Array_IsFrozen(array));
   if (array->UPB_PRIVATE(capacity) < size)
     return UPB_PRIVATE(_upb_Array_Realloc)(array, size, arena);
   return true;
 }
 
 // Resize without initializing new elements.
 UPB_INLINE bool UPB_PRIVATE(_upb_Array_ResizeUninitialized)(
     struct upb_Array* array, size_t size, upb_Arena* arena) {
+  UPB_ASSERT(!upb_Array_IsFrozen(array));
   UPB_ASSERT(size <= array->UPB_ONLYBITS(size) ||
              arena);  // Allow NULL arena when shrinking.
-  if (!UPB_PRIVATE(_upb_Array_Reserve)(array, size, arena)) return false;
+  if (!upb_Array_Reserve(array, size, arena)) return false;
   array->UPB_ONLYBITS(size) = size;
   return true;
 }
 
 // This function is intended for situations where elem_size is compile-time
 // constant or a known expression of the form (1 << lg2), so that the expression
 // i*elem_size does not result in an actual multiplication.
 UPB_INLINE void UPB_PRIVATE(_upb_Array_Set)(struct upb_Array* array, size_t i,
                                             const void* data,
                                             size_t elem_size) {
+  UPB_ASSERT(!upb_Array_IsFrozen(array));
   UPB_ASSERT(i < array->UPB_ONLYBITS(size));
   UPB_ASSERT(elem_size == 1U << UPB_PRIVATE(_upb_Array_ElemSizeLg2)(array));
-  char* arr_data = (char*)UPB_PRIVATE(_upb_Array_MutableDataPtr)(array);
+  char* arr_data = (char*)upb_Array_MutableDataPtr(array);
   memcpy(arr_data + (i * elem_size), data, elem_size);
 }
 
-UPB_INLINE size_t UPB_PRIVATE(_upb_Array_Size)(const struct upb_Array* arr) {
+UPB_API_INLINE size_t upb_Array_Size(const struct upb_Array* arr) {
   return arr->UPB_ONLYBITS(size);
 }
 
-// LINT.ThenChange(
-//  GoogleInternalName1,
-//)
+// LINT.ThenChange(GoogleInternalName0)
 
 #ifdef __cplusplus
 } /* extern "C" */
 #endif
 
 #undef _UPB_ARRAY_MASK_IMM
 #undef _UPB_ARRAY_MASK_LG2
```

### Comparing `protobuf-5.26.1/upb/message/internal/extension.c` & `protobuf-5.27.0rc1/upb/message/internal/extension.c`

 * *Files 24% similar despite different names*

```diff
@@ -14,50 +14,49 @@
 #include "upb/message/internal/message.h"
 #include "upb/message/internal/types.h"
 #include "upb/mini_table/extension.h"
 
 // Must be last.
 #include "upb/port/def.inc"
 
-const struct upb_Extension* UPB_PRIVATE(_upb_Message_Getext)(
+const upb_Extension* UPB_PRIVATE(_upb_Message_Getext)(
     const struct upb_Message* msg, const upb_MiniTableExtension* e) {
   size_t n;
-  const struct upb_Extension* ext = UPB_PRIVATE(_upb_Message_Getexts)(msg, &n);
+  const upb_Extension* ext = UPB_PRIVATE(_upb_Message_Getexts)(msg, &n);
 
   // For now we use linear search exclusively to find extensions.
   // If this becomes an issue due to messages with lots of extensions,
   // we can introduce a table of some sort.
   for (size_t i = 0; i < n; i++) {
     if (ext[i].ext == e) {
       return &ext[i];
     }
   }
 
   return NULL;
 }
 
-const struct upb_Extension* UPB_PRIVATE(_upb_Message_Getexts)(
+const upb_Extension* UPB_PRIVATE(_upb_Message_Getexts)(
     const struct upb_Message* msg, size_t* count) {
-  upb_Message_Internal* in = msg->internal;
+  upb_Message_Internal* in = UPB_PRIVATE(_upb_Message_GetInternal)(msg);
   if (in) {
-    *count = (in->size - in->ext_begin) / sizeof(struct upb_Extension);
+    *count = (in->size - in->ext_begin) / sizeof(upb_Extension);
     return UPB_PTR_AT(in, in->ext_begin, void);
   } else {
     *count = 0;
     return NULL;
   }
 }
 
-struct upb_Extension* UPB_PRIVATE(_upb_Message_GetOrCreateExtension)(
+upb_Extension* UPB_PRIVATE(_upb_Message_GetOrCreateExtension)(
     struct upb_Message* msg, const upb_MiniTableExtension* e, upb_Arena* a) {
-  struct upb_Extension* ext =
-      (struct upb_Extension*)UPB_PRIVATE(_upb_Message_Getext)(msg, e);
+  upb_Extension* ext = (upb_Extension*)UPB_PRIVATE(_upb_Message_Getext)(msg, e);
   if (ext) return ext;
-  if (!UPB_PRIVATE(_upb_Message_Realloc)(msg, sizeof(struct upb_Extension), a))
+  if (!UPB_PRIVATE(_upb_Message_Realloc)(msg, sizeof(upb_Extension), a))
     return NULL;
-  upb_Message_Internal* in = msg->internal;
-  in->ext_begin -= sizeof(struct upb_Extension);
+  upb_Message_Internal* in = UPB_PRIVATE(_upb_Message_GetInternal)(msg);
+  in->ext_begin -= sizeof(upb_Extension);
   ext = UPB_PTR_AT(in, in->ext_begin, void);
-  memset(ext, 0, sizeof(struct upb_Extension));
+  memset(ext, 0, sizeof(upb_Extension));
   ext->ext = e;
   return ext;
 }
```

### Comparing `protobuf-5.26.1/upb/message/internal/extension.h` & `protobuf-5.27.0rc1/upb/message/internal/extension.h`

 * *Files 22% similar despite different names*

```diff
@@ -4,58 +4,55 @@
 // Use of this source code is governed by a BSD-style
 // license that can be found in the LICENSE file or at
 // https://developers.google.com/open-source/licenses/bsd
 
 #ifndef UPB_MESSAGE_INTERNAL_EXTENSION_H_
 #define UPB_MESSAGE_INTERNAL_EXTENSION_H_
 
-#include "upb/base/string_view.h"
+#include <stddef.h>
+
 #include "upb/mem/arena.h"
-#include "upb/message/internal/message.h"
+#include "upb/message/value.h"
 #include "upb/mini_table/extension.h"
 
 // Must be last.
 #include "upb/port/def.inc"
 
 // The internal representation of an extension is self-describing: it contains
 // enough information that we can serialize it to binary format without needing
 // to look it up in a upb_ExtensionRegistry.
 //
 // This representation allocates 16 bytes to data on 64-bit platforms.
 // This is rather wasteful for scalars (in the extreme case of bool,
 // it wastes 15 bytes). We accept this because we expect messages to be
 // the most common extension type.
-struct upb_Extension {
+typedef struct {
   const upb_MiniTableExtension* ext;
-  union {
-    upb_StringView str;
-    void* ptr;
-    char scalar_data[8];
-  } data;
-};
+  upb_MessageValue data;
+} upb_Extension;
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 // Adds the given extension data to the given message.
 // |ext| is copied into the message instance.
 // This logically replaces any previously-added extension with this number.
-struct upb_Extension* UPB_PRIVATE(_upb_Message_GetOrCreateExtension)(
+upb_Extension* UPB_PRIVATE(_upb_Message_GetOrCreateExtension)(
     struct upb_Message* msg, const upb_MiniTableExtension* ext,
     upb_Arena* arena);
 
 // Returns an array of extensions for this message.
 // Note: the array is ordered in reverse relative to the order of creation.
-const struct upb_Extension* UPB_PRIVATE(_upb_Message_Getexts)(
+const upb_Extension* UPB_PRIVATE(_upb_Message_Getexts)(
     const struct upb_Message* msg, size_t* count);
 
 // Returns an extension for a message with a given mini table,
 // or NULL if no extension exists with this mini table.
-const struct upb_Extension* UPB_PRIVATE(_upb_Message_Getext)(
+const upb_Extension* UPB_PRIVATE(_upb_Message_Getext)(
     const struct upb_Message* msg, const upb_MiniTableExtension* ext);
 
 #ifdef __cplusplus
 } /* extern "C" */
 #endif
 
 #include "upb/port/undef.inc"
```

### Comparing `protobuf-5.26.1/upb/message/internal/map.h` & `protobuf-5.27.0rc1/upb/message/internal/map.h`

 * *Files 6% similar despite different names*

```diff
@@ -28,22 +28,31 @@
 // EVERYTHING BELOW THIS LINE IS INTERNAL - DO NOT USE /////////////////////////
 
 struct upb_Map {
   // Size of key and val, based on the map type.
   // Strings are represented as '0' because they must be handled specially.
   char key_size;
   char val_size;
+  bool UPB_PRIVATE(is_frozen);
 
   upb_strtable table;
 };
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
+UPB_INLINE void UPB_PRIVATE(_upb_Map_ShallowFreeze)(struct upb_Map* map) {
+  map->UPB_PRIVATE(is_frozen) = true;
+}
+
+UPB_API_INLINE bool upb_Map_IsFrozen(const struct upb_Map* map) {
+  return map->UPB_PRIVATE(is_frozen);
+}
+
 // Converting between internal table representation and user values.
 //
 // _upb_map_tokey() and _upb_map_fromkey() are inverses.
 // _upb_map_tovalue() and _upb_map_fromvalue() are inverses.
 //
 // These functions account for the fact that strings are treated differently
 // from other types when stored in a map.
@@ -93,19 +102,23 @@
   upb_strtable_next(&it);
   *iter = it.index;
   if (upb_strtable_done(&it)) return NULL;
   return (void*)str_tabent(&it);
 }
 
 UPB_INLINE void _upb_Map_Clear(struct upb_Map* map) {
+  UPB_ASSERT(!upb_Map_IsFrozen(map));
+
   upb_strtable_clear(&map->table);
 }
 
 UPB_INLINE bool _upb_Map_Delete(struct upb_Map* map, const void* key,
                                 size_t key_size, upb_value* val) {
+  UPB_ASSERT(!upb_Map_IsFrozen(map));
+
   upb_StringView k = _upb_map_tokey(key, key_size);
   return upb_strtable_remove2(&map->table, k.data, k.size, val);
 }
 
 UPB_INLINE bool _upb_Map_Get(const struct upb_Map* map, const void* key,
                              size_t key_size, void* val, size_t val_size) {
   upb_value tabval;
@@ -117,14 +130,16 @@
   return ret;
 }
 
 UPB_INLINE upb_MapInsertStatus _upb_Map_Insert(struct upb_Map* map,
                                                const void* key, size_t key_size,
                                                void* val, size_t val_size,
                                                upb_Arena* a) {
+  UPB_ASSERT(!upb_Map_IsFrozen(map));
+
   upb_StringView strkey = _upb_map_tokey(key, key_size);
   upb_value tabval = {0};
   if (!_upb_map_tovalue(val, val_size, &tabval, a)) {
     return kUpb_MapInsertStatus_OutOfMemory;
   }
 
   // TODO: add overwrite operation to minimize number of lookups.
```

### Comparing `protobuf-5.26.1/upb/message/internal/map_entry.h` & `protobuf-5.27.0rc1/upb/message/internal/map_entry.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/message/internal/map_sorter.h` & `protobuf-5.27.0rc1/upb/message/internal/map_sorter.h`

 * *Files 11% similar despite different names*

```diff
@@ -62,31 +62,30 @@
   upb_value val = {tabent->val.val};
   _upb_map_fromvalue(val, &ent->v, map->val_size);
   return true;
 }
 
 UPB_INLINE bool _upb_sortedmap_nextext(_upb_mapsorter* s,
                                        _upb_sortedmap* sorted,
-                                       const struct upb_Extension** ext) {
+                                       const upb_Extension** ext) {
   if (sorted->pos == sorted->end) return false;
-  *ext = (const struct upb_Extension*)s->entries[sorted->pos++];
+  *ext = (const upb_Extension*)s->entries[sorted->pos++];
   return true;
 }
 
 UPB_INLINE void _upb_mapsorter_popmap(_upb_mapsorter* s,
                                       _upb_sortedmap* sorted) {
   s->size = sorted->start;
 }
 
 bool _upb_mapsorter_pushmap(_upb_mapsorter* s, upb_FieldType key_type,
                             const struct upb_Map* map, _upb_sortedmap* sorted);
 
-bool _upb_mapsorter_pushexts(_upb_mapsorter* s,
-                             const struct upb_Extension* exts, size_t count,
-                             _upb_sortedmap* sorted);
+bool _upb_mapsorter_pushexts(_upb_mapsorter* s, const upb_Extension* exts,
+                             size_t count, _upb_sortedmap* sorted);
 
 #ifdef __cplusplus
 } /* extern "C" */
 #endif
 
 #include "upb/port/undef.inc"
```

### Comparing `protobuf-5.26.1/upb/message/internal/message.c` & `protobuf-5.27.0rc1/upb/message/internal/message.c`

 * *Files 24% similar despite different names*

```diff
@@ -21,25 +21,25 @@
 const double kUpb_Infinity = INFINITY;
 const double kUpb_NaN = NAN;
 
 bool UPB_PRIVATE(_upb_Message_Realloc)(struct upb_Message* msg, size_t need,
                                        upb_Arena* a) {
   const size_t overhead = sizeof(upb_Message_Internal);
 
-  upb_Message_Internal* in = msg->internal;
+  upb_Message_Internal* in = UPB_PRIVATE(_upb_Message_GetInternal)(msg);
   if (!in) {
     // No internal data, allocate from scratch.
     size_t size = UPB_MAX(128, upb_Log2CeilingSize(need + overhead));
     in = upb_Arena_Malloc(a, size);
     if (!in) return false;
 
     in->size = size;
     in->unknown_end = overhead;
     in->ext_begin = size;
-    msg->internal = in;
+    UPB_PRIVATE(_upb_Message_SetInternal)(msg, in);
   } else if (in->ext_begin - in->unknown_end < need) {
     // Internal data is too small, reallocate.
     size_t new_size = upb_Log2CeilingSize(in->size + need);
     size_t ext_bytes = in->size - in->ext_begin;
     size_t new_ext_begin = new_size - ext_bytes;
     in = upb_Arena_Realloc(a, in, in->size, new_size);
     if (!in) return false;
@@ -47,13 +47,30 @@
     if (ext_bytes) {
       // Need to move extension data to the end.
       char* ptr = (char*)in;
       memmove(ptr + new_ext_begin, ptr + in->ext_begin, ext_bytes);
     }
     in->ext_begin = new_ext_begin;
     in->size = new_size;
-    msg->internal = in;
+    UPB_PRIVATE(_upb_Message_SetInternal)(msg, in);
   }
 
   UPB_ASSERT(in->ext_begin - in->unknown_end >= need);
   return true;
 }
+
+#if UPB_TRACING_ENABLED
+static void (*_new_message_trace_handler)(const upb_MiniTable*,
+                                          const upb_Arena*);
+
+void UPB_PRIVATE(upb_Message_SetNewMessageTraceHandler)(
+    void (*new_message_trace_handler)(const upb_MiniTable*, const upb_Arena*)) {
+  _new_message_trace_handler = new_message_trace_handler;
+}
+
+void UPB_PRIVATE(upb_Message_LogNewMessage)(const upb_MiniTable* mini_table,
+                                            const upb_Arena* arena) {
+  if (_new_message_trace_handler) {
+    _new_message_trace_handler(mini_table, arena);
+  }
+}
+#endif
```

### Comparing `protobuf-5.26.1/upb/message/internal/message.h` & `protobuf-5.27.0rc1/upb/message/internal/message.h`

 * *Files 9% similar despite different names*

```diff
@@ -55,17 +55,27 @@
    *   extensions data: data[(ext_begin - overhead) .. (size - overhead)] */
   uint32_t unknown_end;
   uint32_t ext_begin;
   // Data follows, as if there were an array:
   //   char data[size - sizeof(upb_Message_Internal)];
 } upb_Message_Internal;
 
+#ifdef UPB_TRACING_ENABLED
+void UPB_PRIVATE(upb_Message_SetNewMessageTraceHandler)(
+    void (*newMessageTraceHandler)(const upb_MiniTable*, const upb_Arena*));
+void UPB_PRIVATE(upb_Message_LogNewMessage)(const upb_MiniTable* mini_table,
+                                            const upb_Arena* arena);
+#endif
+
 // Inline version upb_Message_New(), for internal use.
 UPB_INLINE struct upb_Message* _upb_Message_New(const upb_MiniTable* m,
                                                 upb_Arena* a) {
+#ifdef UPB_TRACING_ENABLED
+  UPB_PRIVATE(upb_Message_LogNewMessage)(m, a);
+#endif
   const int size = m->UPB_PRIVATE(size);
   struct upb_Message* msg = (struct upb_Message*)upb_Arena_Malloc(a, size);
   if (UPB_UNLIKELY(!msg)) return NULL;
   memset(msg, 0, size);
   return msg;
 }
```

### Comparing `protobuf-5.26.1/upb/message/internal/tagged_ptr.h` & `protobuf-5.27.0rc1/upb/message/internal/tagged_ptr.h`

 * *Files 14% similar despite different names*

```diff
@@ -22,32 +22,32 @@
 // Internal-only because empty messages cannot be created by the user.
 UPB_INLINE uintptr_t
 UPB_PRIVATE(_upb_TaggedMessagePtr_Pack)(struct upb_Message* ptr, bool empty) {
   UPB_ASSERT(((uintptr_t)ptr & 1) == 0);
   return (uintptr_t)ptr | (empty ? 1 : 0);
 }
 
-UPB_INLINE bool UPB_PRIVATE(_upb_TaggedMessagePtr_IsEmpty)(uintptr_t ptr) {
+UPB_API_INLINE bool upb_TaggedMessagePtr_IsEmpty(uintptr_t ptr) {
   return ptr & 1;
 }
 
 UPB_INLINE struct upb_Message* UPB_PRIVATE(_upb_TaggedMessagePtr_GetMessage)(
     uintptr_t ptr) {
   return (struct upb_Message*)(ptr & ~(uintptr_t)1);
 }
 
-UPB_INLINE struct upb_Message* UPB_PRIVATE(
-    _upb_TaggedMessagePtr_GetNonEmptyMessage)(uintptr_t ptr) {
-  UPB_ASSERT(!UPB_PRIVATE(_upb_TaggedMessagePtr_IsEmpty)(ptr));
+UPB_API_INLINE struct upb_Message* upb_TaggedMessagePtr_GetNonEmptyMessage(
+    uintptr_t ptr) {
+  UPB_ASSERT(!upb_TaggedMessagePtr_IsEmpty(ptr));
   return UPB_PRIVATE(_upb_TaggedMessagePtr_GetMessage)(ptr);
 }
 
 UPB_INLINE struct upb_Message* UPB_PRIVATE(
     _upb_TaggedMessagePtr_GetEmptyMessage)(uintptr_t ptr) {
-  UPB_ASSERT(UPB_PRIVATE(_upb_TaggedMessagePtr_IsEmpty)(ptr));
+  UPB_ASSERT(upb_TaggedMessagePtr_IsEmpty(ptr));
   return UPB_PRIVATE(_upb_TaggedMessagePtr_GetMessage)(ptr);
 }
 
 #ifdef __cplusplus
 } /* extern "C" */
 #endif
```

### Comparing `protobuf-5.26.1/upb/message/map.c` & `protobuf-5.27.0rc1/upb/message/map.c`

 * *Files 18% similar despite different names*

```diff
@@ -3,18 +3,28 @@
 //
 // Use of this source code is governed by a BSD-style
 // license that can be found in the LICENSE file or at
 // https://developers.google.com/open-source/licenses/bsd
 
 #include "upb/message/map.h"
 
+#include <stdint.h>
 #include <string.h>
 
+#include "upb/base/descriptor_constants.h"
+#include "upb/base/string_view.h"
+#include "upb/hash/common.h"
+#include "upb/hash/str_table.h"
 #include "upb/mem/arena.h"
 #include "upb/message/internal/map.h"
+#include "upb/message/map.h"
+#include "upb/message/message.h"
+#include "upb/message/value.h"
+#include "upb/mini_table/field.h"
+#include "upb/mini_table/message.h"
 
 // Must be last.
 #include "upb/port/def.inc"
 
 // Strings/bytes are special-cased in maps.
 char _upb_Map_CTypeSizeTable[12] = {
     [kUpb_CType_Bool] = 1,
@@ -104,19 +114,34 @@
   upb_MessageValue ret;
   i.t = &map->table;
   i.index = iter;
   _upb_map_fromvalue(upb_strtable_iter_value(&i), &ret, map->val_size);
   return ret;
 }
 
+void upb_Map_Freeze(upb_Map* map, const upb_MiniTable* m) {
+  if (upb_Map_IsFrozen(map)) return;
+  UPB_PRIVATE(_upb_Map_ShallowFreeze)(map);
+
+  if (m) {
+    size_t iter = kUpb_Map_Begin;
+    upb_MessageValue key, val;
+
+    while (upb_Map_Next(map, &key, &val, &iter)) {
+      upb_Message_Freeze((upb_Message*)val.msg_val, m);
+    }
+  }
+}
+
 // EVERYTHING BELOW THIS LINE IS INTERNAL - DO NOT USE /////////////////////////
 
 upb_Map* _upb_Map_New(upb_Arena* a, size_t key_size, size_t value_size) {
   upb_Map* map = upb_Arena_Malloc(a, sizeof(upb_Map));
   if (!map) return NULL;
 
   upb_strtable_init(&map->table, 4, a);
   map->key_size = key_size;
   map->val_size = value_size;
+  map->UPB_PRIVATE(is_frozen) = false;
 
   return map;
 }
```

### Comparing `protobuf-5.26.1/upb/message/map.h` & `protobuf-5.27.0rc1/upb/message/map.h`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 
 #include <stddef.h>
 
 #include "upb/base/descriptor_constants.h"
 #include "upb/mem/arena.h"
 #include "upb/message/internal/map.h"
 #include "upb/message/value.h"
+#include "upb/mini_table/field.h"
+#include "upb/mini_table/message.h"
 
 // Must be last.
 #include "upb/port/def.inc"
 
 typedef struct upb_Map upb_Map;
 
 #ifdef __cplusplus
@@ -57,29 +59,23 @@
 }
 
 // Deletes this key from the table. Returns true if the key was present.
 // If present and |val| is non-NULL, stores the deleted value.
 UPB_API bool upb_Map_Delete(upb_Map* map, upb_MessageValue key,
                             upb_MessageValue* val);
 
-// (DEPRECATED and going away soon. Do not use.)
-UPB_INLINE bool upb_Map_Delete2(upb_Map* map, upb_MessageValue key,
-                                upb_MessageValue* val) {
-  return upb_Map_Delete(map, key, val);
-}
-
 // Map iteration:
 //
 // size_t iter = kUpb_Map_Begin;
 // upb_MessageValue key, val;
 // while (upb_Map_Next(map, &key, &val, &iter)) {
 //   ...
 // }
 
-#define kUpb_Map_Begin ((size_t)-1)
+#define kUpb_Map_Begin ((size_t) - 1)
 
 // Advances to the next entry. Returns false if no more entries are present.
 // Otherwise returns true and populates both *key and *value.
 UPB_API bool upb_Map_Next(const upb_Map* map, upb_MessageValue* key,
                           upb_MessageValue* val, size_t* iter);
 
 // Sets the value for the entry pointed to by iter.
@@ -106,14 +102,22 @@
 // kUpb_Map_Begin (you must call next() at least once first).
 UPB_API bool upb_MapIterator_Done(const upb_Map* map, size_t iter);
 
 // Returns the key and value for this entry of the map.
 UPB_API upb_MessageValue upb_MapIterator_Key(const upb_Map* map, size_t iter);
 UPB_API upb_MessageValue upb_MapIterator_Value(const upb_Map* map, size_t iter);
 
+// Mark a map and all of its descendents as frozen/immutable.
+// If the map values are messages then |m| must point to the minitable for
+// those messages. Otherwise |m| must be NULL.
+UPB_API void upb_Map_Freeze(upb_Map* map, const upb_MiniTable* m);
+
+// Returns whether a map has been frozen.
+UPB_API_INLINE bool upb_Map_IsFrozen(const upb_Map* map);
+
 #ifdef __cplusplus
 } /* extern "C" */
 #endif
 
 #include "upb/port/undef.inc"
 
 #endif /* UPB_MESSAGE_MAP_H_ */
```

### Comparing `protobuf-5.26.1/upb/message/map_gencode_util.h` & `protobuf-5.27.0rc1/upb/message/map_gencode_util.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/message/map_sorter.c` & `protobuf-5.27.0rc1/upb/message/map_sorter.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/message/promote.c` & `protobuf-5.27.0rc1/upb/message/promote.c`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
   upb_Message* extension_msg = parse_result.message;
   // Add to extensions.
   upb_Extension* ext =
       UPB_PRIVATE(_upb_Message_GetOrCreateExtension)(msg, ext_table, arena);
   if (!ext) {
     return kUpb_GetExtension_OutOfMemory;
   }
-  ext->data.ptr = extension_msg;
+  ext->data.msg_val = extension_msg;
   value->msg_val = extension_msg;
   const char* delete_ptr = upb_Message_GetUnknown(msg, &len) + ofs;
   upb_Message_DeleteUnknown(msg, delete_ptr, result.len);
   return kUpb_GetExtension_Ok;
 }
 
 static upb_FindUnknownRet upb_FindUnknownRet_ParseError(void) {
@@ -192,15 +192,15 @@
 }
 
 upb_DecodeStatus upb_Array_PromoteMessages(upb_Array* arr,
                                            const upb_MiniTable* mini_table,
                                            int decode_options,
                                            upb_Arena* arena) {
   void** data = upb_Array_MutableDataPtr(arr);
-  size_t size = arr->UPB_PRIVATE(size);
+  size_t size = upb_Array_Size(arr);
   for (size_t i = 0; i < size; i++) {
     upb_TaggedMessagePtr tagged;
     memcpy(&tagged, &data[i], sizeof(tagged));
     if (!upb_TaggedMessagePtr_IsEmpty(tagged)) continue;
     upb_DecodeStatus status =
         upb_Message_PromoteOne(&tagged, mini_table, decode_options, arena);
     if (status != kUpb_DecodeStatus_Ok) return status;
@@ -239,15 +239,15 @@
   // Callers should check that message is not set first before calling
   // PromotoUnknownToMessage.
   UPB_ASSERT(upb_MiniTable_GetSubMessageTable(mini_table, field) ==
              sub_mini_table);
   bool is_oneof = upb_MiniTableField_IsInOneof(field);
   if (!is_oneof || UPB_PRIVATE(_upb_Message_GetOneofCase)(msg, field) ==
                        upb_MiniTableField_Number(field)) {
-    UPB_ASSERT(upb_Message_GetMessage(msg, field, NULL) == NULL);
+    UPB_ASSERT(upb_Message_GetMessage(msg, field) == NULL);
   }
   upb_UnknownToMessageRet ret;
   ret.status = kUpb_UnknownToMessage_Ok;
   do {
     unknown =
         upb_Message_FindUnknown(msg, upb_MiniTableField_Number(field),
                                 upb_DecodeOptions_GetMaxDepth(decode_options));
@@ -327,16 +327,15 @@
 upb_UnknownToMessage_Status upb_MiniTable_PromoteUnknownToMap(
     upb_Message* msg, const upb_MiniTable* mini_table,
     const upb_MiniTableField* field, int decode_options, upb_Arena* arena) {
   // TODO: use a variant of upb_MiniTable_GetSubMessageTable() here.
   const upb_MiniTable* map_entry_mini_table = upb_MiniTableSub_Message(
       mini_table->UPB_PRIVATE(subs)[field->UPB_PRIVATE(submsg_index)]);
   UPB_ASSERT(map_entry_mini_table);
-  UPB_ASSERT(map_entry_mini_table);
-  UPB_ASSERT(map_entry_mini_table->UPB_PRIVATE(field_count) == 2);
+  UPB_ASSERT(upb_MiniTable_FieldCount(map_entry_mini_table) == 2);
   UPB_ASSERT(upb_MiniTableField_IsMap(field));
   // Find all unknowns with given field number and parse.
   upb_FindUnknownRet unknown;
   while (1) {
     unknown =
         upb_Message_FindUnknown(msg, upb_MiniTableField_Number(field),
                                 upb_DecodeOptions_GetMaxDepth(decode_options));
```

### Comparing `protobuf-5.26.1/upb/message/promote.h` & `protobuf-5.27.0rc1/upb/message/promote.h`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 // license that can be found in the LICENSE file or at
 // https://developers.google.com/open-source/licenses/bsd
 
 #ifndef UPB_MESSAGE_PROMOTE_H_
 #define UPB_MESSAGE_PROMOTE_H_
 
 #include "upb/message/array.h"
-#include "upb/message/internal/extension.h"
 #include "upb/message/map.h"
+#include "upb/message/value.h"
 #include "upb/wire/decode.h"
 
 // Must be last.
 #include "upb/port/def.inc"
 
 #ifdef __cplusplus
 extern "C" {
```

### Comparing `protobuf-5.26.1/upb/message/tagged_ptr.h` & `protobuf-5.27.0rc1/upb/message/tagged_ptr.h`

 * *Files 13% similar despite different names*

```diff
@@ -30,22 +30,18 @@
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 // Users who enable unlinked sub-messages must use this to test whether a
 // message is empty before accessing it. If a message is empty, it must be
 // first promoted using the interfaces in message/promote.h.
-UPB_INLINE bool upb_TaggedMessagePtr_IsEmpty(upb_TaggedMessagePtr ptr) {
-  return UPB_PRIVATE(_upb_TaggedMessagePtr_IsEmpty)(ptr);
-}
+UPB_API_INLINE bool upb_TaggedMessagePtr_IsEmpty(upb_TaggedMessagePtr ptr);
 
-UPB_INLINE upb_Message* upb_TaggedMessagePtr_GetNonEmptyMessage(
-    upb_TaggedMessagePtr ptr) {
-  return UPB_PRIVATE(_upb_TaggedMessagePtr_GetNonEmptyMessage)(ptr);
-}
+UPB_API_INLINE upb_Message* upb_TaggedMessagePtr_GetNonEmptyMessage(
+    upb_TaggedMessagePtr ptr);
 
 #ifdef __cplusplus
 } /* extern "C" */
 #endif
 
 #include "upb/port/undef.inc"
```

### Comparing `protobuf-5.26.1/upb/message/value.h` & `protobuf-5.27.0rc1/upb/message/value.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/mini_descriptor/build_enum.c` & `protobuf-5.27.0rc1/upb/mini_descriptor/build_enum.c`

 * *Files 2% similar despite different names*

```diff
@@ -115,17 +115,17 @@
 static upb_MiniTableEnum* upb_MtDecoder_BuildMiniTableEnum(
     upb_MdEnumDecoder* const decoder, const char* const data,
     size_t const len) {
   if (UPB_SETJMP(decoder->base.err) != 0) return NULL;
   return upb_MtDecoder_DoBuildMiniTableEnum(decoder, data, len);
 }
 
-upb_MiniTableEnum* upb_MiniDescriptor_BuildEnum(const char* data, size_t len,
-                                                upb_Arena* arena,
-                                                upb_Status* status) {
+upb_MiniTableEnum* upb_MiniTableEnum_Build(const char* data, size_t len,
+                                           upb_Arena* arena,
+                                           upb_Status* status) {
   upb_MdEnumDecoder decoder = {
       .base =
           {
               .end = UPB_PTRADD(data, len),
               .status = status,
           },
       .arena = arena,
```

### Comparing `protobuf-5.26.1/upb/mini_descriptor/decode.c` & `protobuf-5.27.0rc1/upb/mini_descriptor/decode.c`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
   kUpb_LayoutItemType_OneofCase,   // Oneof case.
   kUpb_LayoutItemType_OneofField,  // Oneof field data.
   kUpb_LayoutItemType_Field,       // Non-oneof field data.
 
   kUpb_LayoutItemType_Max = kUpb_LayoutItemType_Field,
 } upb_LayoutItemType;
 
-#define kUpb_LayoutItem_IndexSentinel ((uint16_t)-1)
+#define kUpb_LayoutItem_IndexSentinel ((uint16_t) - 1)
 
 typedef struct {
   // Index of the corresponding field.  When this is a oneof field, the field's
   // offset will be the index of the next field in a linked list.
   uint16_t field_index;
   uint16_t offset;
   upb_FieldRep rep;
@@ -241,14 +241,20 @@
   }
   if (singular && required) {
     upb_MdDecoder_ErrorJmp(
         &d->base, "Field %" PRIu32 " cannot be both singular and required",
         upb_MiniTableField_Number(field));
   }
 
+  if (singular && upb_MiniTableField_IsSubMessage(field)) {
+    upb_MdDecoder_ErrorJmp(&d->base,
+                           "Field %" PRIu32 " cannot be a singular submessage",
+                           upb_MiniTableField_Number(field));
+  }
+
   if (singular) field->UPB_PRIVATE(offset) = kNoPresence;
   if (required) {
     field->UPB_PRIVATE(offset) = kRequiredPresence;
   }
 }
 
 static void upb_MtDecoder_PushItem(upb_MtDecoder* d, upb_LayoutItem item) {
@@ -727,14 +733,19 @@
 
   decoder->table->UPB_PRIVATE(size) = kUpb_Reserved_Hasbytes;
   decoder->table->UPB_PRIVATE(field_count) = 0;
   decoder->table->UPB_PRIVATE(ext) = kUpb_ExtMode_NonExtendable;
   decoder->table->UPB_PRIVATE(dense_below) = 0;
   decoder->table->UPB_PRIVATE(table_mask) = -1;
   decoder->table->UPB_PRIVATE(required_count) = 0;
+#if UPB_TRACING_ENABLED
+  // MiniTables built from MiniDescriptors will not be able to vend the message
+  // name unless it is explicitly set with upb_MiniTable_SetFullName().
+  decoder->table->UPB_PRIVATE(full_name) = 0;
+#endif
 
   // Strip off and verify the version tag.
   if (!len--) goto done;
   const char vers = *data++;
 
   switch (vers) {
     case kUpb_EncodedVersion_MapV1:
```

### Comparing `protobuf-5.26.1/upb/mini_descriptor/decode.h` & `protobuf-5.27.0rc1/upb/mini_descriptor/decode.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/mini_descriptor/internal/base92.c` & `protobuf-5.27.0rc1/upb/mini_descriptor/internal/base92.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/mini_descriptor/internal/base92.h` & `protobuf-5.27.0rc1/upb/mini_descriptor/internal/base92.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/mini_descriptor/internal/decoder.h` & `protobuf-5.27.0rc1/upb/mini_descriptor/internal/decoder.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/mini_descriptor/internal/encode.c` & `protobuf-5.27.0rc1/upb/mini_descriptor/internal/encode.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/mini_descriptor/internal/encode.h` & `protobuf-5.27.0rc1/upb/mini_descriptor/internal/encode.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/mini_descriptor/internal/modifiers.h` & `protobuf-5.27.0rc1/upb/mini_descriptor/internal/modifiers.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/mini_descriptor/internal/wire_constants.h` & `protobuf-5.27.0rc1/upb/mini_descriptor/internal/wire_constants.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/mini_descriptor/link.c` & `protobuf-5.27.0rc1/upb/mini_table/compat.c`

 * *Files 19% similar despite different names*

```diff
@@ -1,134 +1,114 @@
 // Protocol Buffers - Google's data interchange format
 // Copyright 2023 Google LLC.  All rights reserved.
 //
 // Use of this source code is governed by a BSD-style
 // license that can be found in the LICENSE file or at
 // https://developers.google.com/open-source/licenses/bsd
 
-#include "upb/mini_descriptor/link.h"
+#include "upb/mini_table/compat.h"
 
 #include <stddef.h>
 #include <stdint.h>
 
 #include "upb/base/descriptor_constants.h"
-#include "upb/mini_table/enum.h"
+#include "upb/hash/common.h"
+#include "upb/hash/int_table.h"
+#include "upb/mem/arena.h"
 #include "upb/mini_table/field.h"
 #include "upb/mini_table/message.h"
-#include "upb/mini_table/sub.h"
 
 // Must be last.
 #include "upb/port/def.inc"
 
-bool upb_MiniTable_SetSubMessage(upb_MiniTable* table,
-                                 upb_MiniTableField* field,
-                                 const upb_MiniTable* sub) {
-  UPB_ASSERT((uintptr_t)table->UPB_PRIVATE(fields) <= (uintptr_t)field &&
-             (uintptr_t)field < (uintptr_t)(table->UPB_PRIVATE(fields) +
-                                            table->UPB_PRIVATE(field_count)));
-  UPB_ASSERT(sub);
-
-  const bool sub_is_map = sub->UPB_PRIVATE(ext) & kUpb_ExtMode_IsMapEntry;
-
-  switch (field->UPB_PRIVATE(descriptortype)) {
-    case kUpb_FieldType_Message:
-      if (sub_is_map) {
-        const bool table_is_map =
-            table->UPB_PRIVATE(ext) & kUpb_ExtMode_IsMapEntry;
-        if (UPB_UNLIKELY(table_is_map)) return false;
-
-        field->UPB_PRIVATE(mode) =
-            (field->UPB_PRIVATE(mode) & ~kUpb_FieldMode_Mask) |
-            kUpb_FieldMode_Map;
-      }
-      break;
-
-    case kUpb_FieldType_Group:
-      if (UPB_UNLIKELY(sub_is_map)) return false;
-      break;
+// Checks if source and target mini table fields are identical.
+//
+// If the field is a sub message and sub messages are identical we record
+// the association in table.
+//
+// Hashing the source sub message mini table and it's equivalent in the table
+// stops recursing when a cycle is detected and instead just checks if the
+// destination table is equal.
+static upb_MiniTableEquals_Status upb_deep_check(const upb_MiniTable* src,
+                                                 const upb_MiniTable* dst,
+                                                 upb_inttable* table,
+                                                 upb_Arena** arena) {
+  if (src->UPB_PRIVATE(field_count) != dst->UPB_PRIVATE(field_count))
+    return kUpb_MiniTableEquals_NotEqual;
+  bool marked_src = false;
+  for (int i = 0; i < upb_MiniTable_FieldCount(src); i++) {
+    const upb_MiniTableField* src_field = upb_MiniTable_GetFieldByIndex(src, i);
+    const upb_MiniTableField* dst_field = upb_MiniTable_FindFieldByNumber(
+        dst, upb_MiniTableField_Number(src_field));
 
-    default:
+    if (upb_MiniTableField_CType(src_field) !=
+        upb_MiniTableField_CType(dst_field))
       return false;
-  }
-
-  upb_MiniTableSub* table_sub =
-      (void*)&table->UPB_PRIVATE(subs)[field->UPB_PRIVATE(submsg_index)];
-  // TODO: Add this assert back once YouTube is updated to not call
-  // this function repeatedly.
-  // UPB_ASSERT(UPB_PRIVATE(_upb_MiniTable_IsEmpty)(table_sub->submsg));
-  *table_sub = upb_MiniTableSub_FromMessage(sub);
-  return true;
-}
-
-bool upb_MiniTable_SetSubEnum(upb_MiniTable* table, upb_MiniTableField* field,
-                              const upb_MiniTableEnum* sub) {
-  UPB_ASSERT((uintptr_t)table->UPB_PRIVATE(fields) <= (uintptr_t)field &&
-             (uintptr_t)field < (uintptr_t)(table->UPB_PRIVATE(fields) +
-                                            table->UPB_PRIVATE(field_count)));
-  UPB_ASSERT(sub);
-
-  upb_MiniTableSub* table_sub =
-      (void*)&table->UPB_PRIVATE(subs)[field->UPB_PRIVATE(submsg_index)];
-  *table_sub = upb_MiniTableSub_FromEnum(sub);
-  return true;
-}
-
-uint32_t upb_MiniTable_GetSubList(const upb_MiniTable* mt,
-                                  const upb_MiniTableField** subs) {
-  uint32_t msg_count = 0;
-  uint32_t enum_count = 0;
-
-  for (int i = 0; i < mt->UPB_PRIVATE(field_count); i++) {
-    const upb_MiniTableField* f = &mt->UPB_PRIVATE(fields)[i];
-    if (upb_MiniTableField_CType(f) == kUpb_CType_Message) {
-      *subs = f;
-      ++subs;
-      msg_count++;
-    }
-  }
-
-  for (int i = 0; i < mt->UPB_PRIVATE(field_count); i++) {
-    const upb_MiniTableField* f = &mt->UPB_PRIVATE(fields)[i];
-    if (upb_MiniTableField_CType(f) == kUpb_CType_Enum) {
-      *subs = f;
-      ++subs;
-      enum_count++;
+    if (src_field->UPB_PRIVATE(mode) != dst_field->UPB_PRIVATE(mode))
+      return false;
+    if (src_field->UPB_PRIVATE(offset) != dst_field->UPB_PRIVATE(offset))
+      return false;
+    if (src_field->presence != dst_field->presence) return false;
+    if (src_field->UPB_PRIVATE(submsg_index) !=
+        dst_field->UPB_PRIVATE(submsg_index))
+      return kUpb_MiniTableEquals_NotEqual;
+
+    // Go no further if we are only checking for compatibility.
+    if (!table) continue;
+
+    if (upb_MiniTableField_CType(src_field) == kUpb_CType_Message) {
+      if (!*arena) {
+        *arena = upb_Arena_New();
+        if (!upb_inttable_init(table, *arena)) {
+          return kUpb_MiniTableEquals_OutOfMemory;
+        }
+      }
+      if (!marked_src) {
+        marked_src = true;
+        upb_value val;
+        val.val = (uint64_t)dst;
+        if (!upb_inttable_insert(table, (uintptr_t)src, val, *arena)) {
+          return kUpb_MiniTableEquals_OutOfMemory;
+        }
+      }
+      const upb_MiniTable* sub_src =
+          upb_MiniTable_GetSubMessageTable(src, src_field);
+      const upb_MiniTable* sub_dst =
+          upb_MiniTable_GetSubMessageTable(dst, dst_field);
+      if (sub_src != NULL) {
+        upb_value cmp;
+        if (upb_inttable_lookup(table, (uintptr_t)sub_src, &cmp)) {
+          // We already compared this src before. Check if same dst.
+          if (cmp.val != (uint64_t)sub_dst) {
+            return kUpb_MiniTableEquals_NotEqual;
+          }
+        } else {
+          // Recurse if not already visited.
+          upb_MiniTableEquals_Status s =
+              upb_deep_check(sub_src, sub_dst, table, arena);
+          if (s != kUpb_MiniTableEquals_Equal) {
+            return s;
+          }
+        }
+      }
     }
   }
-
-  return (msg_count << 16) | enum_count;
+  return kUpb_MiniTableEquals_Equal;
 }
 
-// The list of sub_tables and sub_enums must exactly match the number and order
-// of sub-message fields and sub-enum fields given by upb_MiniTable_GetSubList()
-// above.
-bool upb_MiniTable_Link(upb_MiniTable* mt, const upb_MiniTable** sub_tables,
-                        size_t sub_table_count,
-                        const upb_MiniTableEnum** sub_enums,
-                        size_t sub_enum_count) {
-  uint32_t msg_count = 0;
-  uint32_t enum_count = 0;
-
-  for (int i = 0; i < mt->UPB_PRIVATE(field_count); i++) {
-    upb_MiniTableField* f = (upb_MiniTableField*)&mt->UPB_PRIVATE(fields)[i];
-    if (upb_MiniTableField_CType(f) == kUpb_CType_Message) {
-      const upb_MiniTable* sub = sub_tables[msg_count++];
-      if (msg_count > sub_table_count) return false;
-      if (sub != NULL) {
-        if (!upb_MiniTable_SetSubMessage(mt, f, sub)) return false;
-      }
-    }
-  }
+bool upb_MiniTable_Compatible(const upb_MiniTable* src,
+                              const upb_MiniTable* dst) {
+  return upb_deep_check(src, dst, NULL, NULL);
+}
 
-  for (int i = 0; i < mt->UPB_PRIVATE(field_count); i++) {
-    upb_MiniTableField* f = (upb_MiniTableField*)&mt->UPB_PRIVATE(fields)[i];
-    if (upb_MiniTableField_IsClosedEnum(f)) {
-      const upb_MiniTableEnum* sub = sub_enums[enum_count++];
-      if (enum_count > sub_enum_count) return false;
-      if (sub != NULL) {
-        if (!upb_MiniTable_SetSubEnum(mt, f, sub)) return false;
-      }
-    }
+upb_MiniTableEquals_Status upb_MiniTable_Equals(const upb_MiniTable* src,
+                                                const upb_MiniTable* dst) {
+  // Arena allocated on demand for hash table.
+  upb_Arena* arena = NULL;
+  // Table to keep track of visited mini tables to guard against cycles.
+  upb_inttable table;
+  upb_MiniTableEquals_Status status = upb_deep_check(src, dst, &table, &arena);
+  if (arena) {
+    upb_Arena_Free(arena);
   }
-
-  return true;
+  return status;
 }
```

### Comparing `protobuf-5.26.1/upb/mini_descriptor/link.h` & `protobuf-5.27.0rc1/upb/mini_descriptor/link.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/mini_table/compat.h` & `protobuf-5.27.0rc1/upb/mini_table/compat.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/mini_table/enum.h` & `protobuf-5.27.0rc1/upb/mini_table/enum.h`

 * *Files 8% similar despite different names*

```diff
@@ -18,18 +18,16 @@
 typedef struct upb_MiniTableEnum upb_MiniTableEnum;
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 // Validates enum value against range defined by enum mini table.
-UPB_INLINE bool upb_MiniTableEnum_CheckValue(const upb_MiniTableEnum* e,
-                                             uint32_t val) {
-  return UPB_PRIVATE(_upb_MiniTableEnum_CheckValue)(e, val);
-}
+UPB_API_INLINE bool upb_MiniTableEnum_CheckValue(const upb_MiniTableEnum* e,
+                                                 uint32_t val);
 
 #ifdef __cplusplus
 } /* extern "C" */
 #endif
 
 #include "upb/port/undef.inc"
```

### Comparing `protobuf-5.26.1/upb/mini_table/extension.h` & `protobuf-5.27.0rc1/upb/mini_table/extension.h`

 * *Files 14% similar despite different names*

```diff
@@ -20,32 +20,24 @@
 typedef struct upb_MiniTableExtension upb_MiniTableExtension;
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 UPB_API_INLINE upb_CType
-upb_MiniTableExtension_CType(const upb_MiniTableExtension* e) {
-  return UPB_PRIVATE(_upb_MiniTableExtension_CType)(e);
-}
+upb_MiniTableExtension_CType(const upb_MiniTableExtension* e);
 
 UPB_API_INLINE uint32_t
-upb_MiniTableExtension_Number(const upb_MiniTableExtension* e) {
-  return UPB_PRIVATE(_upb_MiniTableExtension_Number)(e);
-}
+upb_MiniTableExtension_Number(const upb_MiniTableExtension* e);
 
 UPB_API_INLINE const upb_MiniTable* upb_MiniTableExtension_GetSubMessage(
-    const upb_MiniTableExtension* e) {
-  return UPB_PRIVATE(_upb_MiniTableExtension_GetSubMessage)(e);
-}
+    const upb_MiniTableExtension* e);
 
 UPB_API_INLINE void upb_MiniTableExtension_SetSubMessage(
-    upb_MiniTableExtension* e, const upb_MiniTable* m) {
-  UPB_PRIVATE(_upb_MiniTableExtension_SetSubMessage)(e, m);
-}
+    upb_MiniTableExtension* e, const upb_MiniTable* m);
 
 #ifdef __cplusplus
 } /* extern "C" */
 #endif
 
 #include "upb/port/undef.inc"
```

### Comparing `protobuf-5.26.1/upb/mini_table/extension_registry.c` & `protobuf-5.27.0rc1/upb/mini_table/extension_registry.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/mini_table/extension_registry.h` & `protobuf-5.27.0rc1/upb/mini_table/extension_registry.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/mini_table/field.h` & `protobuf-5.27.0rc1/upb/mini_table/field.h`

 * *Files 25% similar despite different names*

```diff
@@ -18,66 +18,40 @@
 
 typedef struct upb_MiniTableField upb_MiniTableField;
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
-UPB_API_INLINE upb_CType upb_MiniTableField_CType(const upb_MiniTableField* f) {
-  return UPB_PRIVATE(_upb_MiniTableField_CType)(f);
-}
-
-UPB_API_INLINE bool upb_MiniTableField_HasPresence(
-    const upb_MiniTableField* f) {
-  return UPB_PRIVATE(_upb_MiniTableField_HasPresence)(f);
-}
-
-UPB_API_INLINE bool upb_MiniTableField_IsArray(const upb_MiniTableField* f) {
-  return UPB_PRIVATE(_upb_MiniTableField_IsArray)(f);
-}
+UPB_API_INLINE upb_CType upb_MiniTableField_CType(const upb_MiniTableField* f);
+
+UPB_API_INLINE bool upb_MiniTableField_HasPresence(const upb_MiniTableField* f);
+
+UPB_API_INLINE bool upb_MiniTableField_IsArray(const upb_MiniTableField* f);
 
 UPB_API_INLINE bool upb_MiniTableField_IsClosedEnum(
-    const upb_MiniTableField* f) {
-  return UPB_PRIVATE(_upb_MiniTableField_IsClosedEnum)(f);
-}
-
-UPB_API_INLINE bool upb_MiniTableField_IsExtension(
-    const upb_MiniTableField* f) {
-  return UPB_PRIVATE(_upb_MiniTableField_IsExtension)(f);
-}
-
-UPB_API_INLINE bool upb_MiniTableField_IsInOneof(const upb_MiniTableField* f) {
-  return UPB_PRIVATE(_upb_MiniTableField_IsInOneof)(f);
-}
-
-UPB_API_INLINE bool upb_MiniTableField_IsMap(const upb_MiniTableField* f) {
-  return UPB_PRIVATE(_upb_MiniTableField_IsMap)(f);
-}
-
-UPB_API_INLINE bool upb_MiniTableField_IsPacked(const upb_MiniTableField* f) {
-  return UPB_PRIVATE(_upb_MiniTableField_IsPacked)(f);
-}
-
-UPB_API_INLINE bool upb_MiniTableField_IsScalar(const upb_MiniTableField* f) {
-  return UPB_PRIVATE(_upb_MiniTableField_IsScalar)(f);
-}
+    const upb_MiniTableField* f);
+
+UPB_API_INLINE bool upb_MiniTableField_IsExtension(const upb_MiniTableField* f);
+
+UPB_API_INLINE bool upb_MiniTableField_IsInOneof(const upb_MiniTableField* f);
+
+UPB_API_INLINE bool upb_MiniTableField_IsMap(const upb_MiniTableField* f);
+
+UPB_API_INLINE bool upb_MiniTableField_IsPacked(const upb_MiniTableField* f);
+
+UPB_API_INLINE bool upb_MiniTableField_IsScalar(const upb_MiniTableField* f);
 
 UPB_API_INLINE bool upb_MiniTableField_IsSubMessage(
-    const upb_MiniTableField* f) {
-  return UPB_PRIVATE(_upb_MiniTableField_IsSubMessage)(f);
-}
-
-UPB_API_INLINE uint32_t upb_MiniTableField_Number(const upb_MiniTableField* f) {
-  return UPB_PRIVATE(_upb_MiniTableField_Number)(f);
-}
+    const upb_MiniTableField* f);
+
+UPB_API_INLINE uint32_t upb_MiniTableField_Number(const upb_MiniTableField* f);
 
 UPB_API_INLINE upb_FieldType
-upb_MiniTableField_Type(const upb_MiniTableField* f) {
-  return UPB_PRIVATE(_upb_MiniTableField_Type)(f);
-}
+upb_MiniTableField_Type(const upb_MiniTableField* f);
 
 #ifdef __cplusplus
 } /* extern "C" */
 #endif
 
 #include "upb/port/undef.inc"
```

### Comparing `protobuf-5.26.1/upb/mini_table/file.h` & `protobuf-5.27.0rc1/upb/mini_table/file.h`

 * *Files 18% similar despite different names*

```diff
@@ -19,40 +19,27 @@
 typedef struct upb_MiniTableFile upb_MiniTableFile;
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 UPB_API_INLINE const upb_MiniTableEnum* upb_MiniTableFile_Enum(
-    const upb_MiniTableFile* f, int i) {
-  return UPB_PRIVATE(_upb_MiniTableFile_Enum)(f, i);
-}
-
-UPB_API_INLINE int upb_MiniTableFile_EnumCount(const upb_MiniTableFile* f) {
-  return UPB_PRIVATE(_upb_MiniTableFile_EnumCount)(f);
-}
+    const upb_MiniTableFile* f, int i);
+
+UPB_API_INLINE int upb_MiniTableFile_EnumCount(const upb_MiniTableFile* f);
 
 UPB_API_INLINE const upb_MiniTableExtension* upb_MiniTableFile_Extension(
-    const upb_MiniTableFile* f, int i) {
-  return UPB_PRIVATE(_upb_MiniTableFile_Extension)(f, i);
-}
-
-UPB_API_INLINE int upb_MiniTableFile_ExtensionCount(
-    const upb_MiniTableFile* f) {
-  return UPB_PRIVATE(_upb_MiniTableFile_ExtensionCount)(f);
-}
+    const upb_MiniTableFile* f, int i);
+
+UPB_API_INLINE int upb_MiniTableFile_ExtensionCount(const upb_MiniTableFile* f);
 
 UPB_API_INLINE const upb_MiniTable* upb_MiniTableFile_Message(
-    const upb_MiniTableFile* f, int i) {
-  return UPB_PRIVATE(_upb_MiniTableFile_Message)(f, i);
-}
-
-UPB_API_INLINE int upb_MiniTableFile_MessageCount(const upb_MiniTableFile* f) {
-  return UPB_PRIVATE(_upb_MiniTableFile_MessageCount)(f);
-}
+    const upb_MiniTableFile* f, int i);
+
+UPB_API_INLINE int upb_MiniTableFile_MessageCount(const upb_MiniTableFile* f);
 
 #ifdef __cplusplus
 } /* extern "C" */
 #endif
 
 #include "upb/port/undef.inc"
```

### Comparing `protobuf-5.26.1/upb/mini_table/internal/enum.h` & `protobuf-5.27.0rc1/upb/mini_table/internal/enum.h`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
   uint32_t UPB_PRIVATE(data)[];       // Bitmask + enumerated values follow.
 };
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
-UPB_INLINE bool UPB_PRIVATE(_upb_MiniTableEnum_CheckValue)(
+UPB_API_INLINE bool upb_MiniTableEnum_CheckValue(
     const struct upb_MiniTableEnum* e, uint32_t val) {
   if (UPB_LIKELY(val < 64)) {
     const uint64_t mask =
         e->UPB_PRIVATE(data)[0] | ((uint64_t)e->UPB_PRIVATE(data)[1] << 32);
     const uint64_t bit = 1ULL << val;
     return (mask & bit) != 0;
   }
```

### Comparing `protobuf-5.26.1/upb/mini_table/internal/field.h` & `protobuf-5.27.0rc1/upb/mini_table/internal/field.h`

 * *Files 12% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
   uint8_t UPB_PRIVATE(descriptortype);
 
   // upb_FieldMode | upb_LabelFlags | (upb_FieldRep << kUpb_FieldRep_Shift)
   uint8_t UPB_ONLYBITS(mode);
 };
 
-#define kUpb_NoSub ((uint16_t)-1)
+#define kUpb_NoSub ((uint16_t) - 1)
 
 typedef enum {
   kUpb_FieldMode_Map = 0,
   kUpb_FieldMode_Array = 1,
   kUpb_FieldMode_Scalar = 2,
 } upb_FieldMode;
 
@@ -80,58 +80,58 @@
 }
 
 UPB_INLINE upb_FieldRep
 UPB_PRIVATE(_upb_MiniTableField_GetRep)(const struct upb_MiniTableField* f) {
   return (upb_FieldRep)(f->UPB_ONLYBITS(mode) >> kUpb_FieldRep_Shift);
 }
 
-UPB_INLINE bool UPB_PRIVATE(_upb_MiniTableField_IsArray)(
+UPB_API_INLINE bool upb_MiniTableField_IsArray(
     const struct upb_MiniTableField* f) {
   return UPB_PRIVATE(_upb_MiniTableField_Mode)(f) == kUpb_FieldMode_Array;
 }
 
-UPB_INLINE bool UPB_PRIVATE(_upb_MiniTableField_IsMap)(
+UPB_API_INLINE bool upb_MiniTableField_IsMap(
     const struct upb_MiniTableField* f) {
   return UPB_PRIVATE(_upb_MiniTableField_Mode)(f) == kUpb_FieldMode_Map;
 }
 
-UPB_INLINE bool UPB_PRIVATE(_upb_MiniTableField_IsScalar)(
+UPB_API_INLINE bool upb_MiniTableField_IsScalar(
     const struct upb_MiniTableField* f) {
   return UPB_PRIVATE(_upb_MiniTableField_Mode)(f) == kUpb_FieldMode_Scalar;
 }
 
 UPB_INLINE bool UPB_PRIVATE(_upb_MiniTableField_IsAlternate)(
     const struct upb_MiniTableField* f) {
   return (f->UPB_ONLYBITS(mode) & kUpb_LabelFlags_IsAlternate) != 0;
 }
 
-UPB_INLINE bool UPB_PRIVATE(_upb_MiniTableField_IsExtension)(
+UPB_API_INLINE bool upb_MiniTableField_IsExtension(
     const struct upb_MiniTableField* f) {
   return (f->UPB_ONLYBITS(mode) & kUpb_LabelFlags_IsExtension) != 0;
 }
 
-UPB_INLINE bool UPB_PRIVATE(_upb_MiniTableField_IsPacked)(
+UPB_API_INLINE bool upb_MiniTableField_IsPacked(
     const struct upb_MiniTableField* f) {
   return (f->UPB_ONLYBITS(mode) & kUpb_LabelFlags_IsPacked) != 0;
 }
 
-UPB_INLINE upb_FieldType
-UPB_PRIVATE(_upb_MiniTableField_Type)(const struct upb_MiniTableField* f) {
+UPB_API_INLINE upb_FieldType
+upb_MiniTableField_Type(const struct upb_MiniTableField* f) {
   const upb_FieldType type = (upb_FieldType)f->UPB_PRIVATE(descriptortype);
   if (UPB_PRIVATE(_upb_MiniTableField_IsAlternate)(f)) {
     if (type == kUpb_FieldType_Int32) return kUpb_FieldType_Enum;
     if (type == kUpb_FieldType_Bytes) return kUpb_FieldType_String;
     UPB_ASSERT(false);
   }
   return type;
 }
 
-UPB_INLINE upb_CType
-UPB_PRIVATE(_upb_MiniTableField_CType)(const struct upb_MiniTableField* f) {
-  return upb_FieldType_CType(UPB_PRIVATE(_upb_MiniTableField_Type)(f));
+UPB_API_INLINE
+upb_CType upb_MiniTableField_CType(const struct upb_MiniTableField* f) {
+  return upb_FieldType_CType(upb_MiniTableField_Type(f));
 }
 
 UPB_INLINE bool UPB_PRIVATE(_upb_MiniTableField_HasHasbit)(
     const struct upb_MiniTableField* f) {
   return f->presence > 0;
 }
 
@@ -145,74 +145,74 @@
 UPB_INLINE size_t UPB_PRIVATE(_upb_MiniTableField_HasbitOffset)(
     const struct upb_MiniTableField* f) {
   UPB_ASSERT(UPB_PRIVATE(_upb_MiniTableField_HasHasbit)(f));
   const size_t index = f->presence;
   return index / 8;
 }
 
-UPB_INLINE bool UPB_PRIVATE(_upb_MiniTableField_IsClosedEnum)(
+UPB_API_INLINE bool upb_MiniTableField_IsClosedEnum(
     const struct upb_MiniTableField* f) {
   return f->UPB_PRIVATE(descriptortype) == kUpb_FieldType_Enum;
 }
 
-UPB_INLINE bool UPB_PRIVATE(_upb_MiniTableField_IsInOneof)(
+UPB_API_INLINE bool upb_MiniTableField_IsInOneof(
     const struct upb_MiniTableField* f) {
   return f->presence < 0;
 }
 
-UPB_INLINE bool UPB_PRIVATE(_upb_MiniTableField_IsSubMessage)(
+UPB_API_INLINE bool upb_MiniTableField_IsSubMessage(
     const struct upb_MiniTableField* f) {
   return f->UPB_PRIVATE(descriptortype) == kUpb_FieldType_Message ||
          f->UPB_PRIVATE(descriptortype) == kUpb_FieldType_Group;
 }
 
-UPB_INLINE bool UPB_PRIVATE(_upb_MiniTableField_HasPresence)(
+UPB_API_INLINE bool upb_MiniTableField_HasPresence(
     const struct upb_MiniTableField* f) {
-  if (UPB_PRIVATE(_upb_MiniTableField_IsExtension)(f)) {
-    return UPB_PRIVATE(_upb_MiniTableField_IsScalar)(f);
+  if (upb_MiniTableField_IsExtension(f)) {
+    return upb_MiniTableField_IsScalar(f);
   } else {
     return f->presence != 0;
   }
 }
 
-UPB_INLINE uint32_t
-UPB_PRIVATE(_upb_MiniTableField_Number)(const struct upb_MiniTableField* f) {
+UPB_API_INLINE uint32_t
+upb_MiniTableField_Number(const struct upb_MiniTableField* f) {
   return f->UPB_ONLYBITS(number);
 }
 
 UPB_INLINE uint16_t
 UPB_PRIVATE(_upb_MiniTableField_Offset)(const struct upb_MiniTableField* f) {
   return f->UPB_ONLYBITS(offset);
 }
 
 UPB_INLINE size_t UPB_PRIVATE(_upb_MiniTableField_OneofOffset)(
     const struct upb_MiniTableField* f) {
-  UPB_ASSERT(UPB_PRIVATE(_upb_MiniTableField_IsInOneof)(f));
+  UPB_ASSERT(upb_MiniTableField_IsInOneof(f));
   return ~(ptrdiff_t)f->presence;
 }
 
 UPB_INLINE void UPB_PRIVATE(_upb_MiniTableField_CheckIsArray)(
     const struct upb_MiniTableField* f) {
   UPB_ASSUME(UPB_PRIVATE(_upb_MiniTableField_GetRep)(f) ==
              kUpb_FieldRep_NativePointer);
-  UPB_ASSUME(UPB_PRIVATE(_upb_MiniTableField_IsArray)(f));
+  UPB_ASSUME(upb_MiniTableField_IsArray(f));
   UPB_ASSUME(f->presence == 0);
 }
 
 UPB_INLINE void UPB_PRIVATE(_upb_MiniTableField_CheckIsMap)(
     const struct upb_MiniTableField* f) {
   UPB_ASSUME(UPB_PRIVATE(_upb_MiniTableField_GetRep)(f) ==
              kUpb_FieldRep_NativePointer);
-  UPB_ASSUME(UPB_PRIVATE(_upb_MiniTableField_IsMap)(f));
+  UPB_ASSUME(upb_MiniTableField_IsMap(f));
   UPB_ASSUME(f->presence == 0);
 }
 
 UPB_INLINE size_t UPB_PRIVATE(_upb_MiniTableField_ElemSizeLg2)(
     const struct upb_MiniTableField* f) {
-  const upb_FieldType field_type = UPB_PRIVATE(_upb_MiniTableField_Type)(f);
+  const upb_FieldType field_type = upb_MiniTableField_Type(f);
   return UPB_PRIVATE(_upb_FieldType_SizeLg2)(field_type);
 }
 
 // LINT.ThenChange(//depot/google3/third_party/upb/bits/typescript/mini_table_field.ts)
 
 #ifdef __cplusplus
 } /* extern "C" */
```

### Comparing `protobuf-5.26.1/upb/mini_table/internal/file.h` & `protobuf-5.27.0rc1/upb/mini_table/internal/file.h`

 * *Files 10% similar despite different names*

```diff
@@ -20,42 +20,42 @@
   int UPB_PRIVATE(ext_count);
 };
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
-UPB_INLINE int UPB_PRIVATE(_upb_MiniTableFile_EnumCount)(
+UPB_API_INLINE int upb_MiniTableFile_EnumCount(
     const struct upb_MiniTableFile* f) {
   return f->UPB_PRIVATE(enum_count);
 }
 
-UPB_INLINE int UPB_PRIVATE(_upb_MiniTableFile_ExtensionCount)(
+UPB_API_INLINE int upb_MiniTableFile_ExtensionCount(
     const struct upb_MiniTableFile* f) {
   return f->UPB_PRIVATE(ext_count);
 }
 
-UPB_INLINE int UPB_PRIVATE(_upb_MiniTableFile_MessageCount)(
+UPB_API_INLINE int upb_MiniTableFile_MessageCount(
     const struct upb_MiniTableFile* f) {
   return f->UPB_PRIVATE(msg_count);
 }
 
-UPB_INLINE const struct upb_MiniTableEnum* UPB_PRIVATE(_upb_MiniTableFile_Enum)(
+UPB_API_INLINE const struct upb_MiniTableEnum* upb_MiniTableFile_Enum(
     const struct upb_MiniTableFile* f, int i) {
   UPB_ASSERT(i < f->UPB_PRIVATE(enum_count));
   return f->UPB_PRIVATE(enums)[i];
 }
 
-UPB_INLINE const struct upb_MiniTableExtension* UPB_PRIVATE(
-    _upb_MiniTableFile_Extension)(const struct upb_MiniTableFile* f, int i) {
+UPB_API_INLINE const struct upb_MiniTableExtension* upb_MiniTableFile_Extension(
+    const struct upb_MiniTableFile* f, int i) {
   UPB_ASSERT(i < f->UPB_PRIVATE(ext_count));
   return f->UPB_PRIVATE(exts)[i];
 }
 
-UPB_INLINE const struct upb_MiniTable* UPB_PRIVATE(_upb_MiniTableFile_Message)(
+UPB_API_INLINE const struct upb_MiniTable* upb_MiniTableFile_Message(
     const struct upb_MiniTableFile* f, int i) {
   UPB_ASSERT(i < f->UPB_PRIVATE(msg_count));
   return f->UPB_PRIVATE(msgs)[i];
 }
 
 #ifdef __cplusplus
 } /* extern "C" */
```

### Comparing `protobuf-5.26.1/upb/mini_table/internal/message.c` & `protobuf-5.27.0rc1/upb/mini_table/internal/message.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/mini_table/internal/message.h` & `protobuf-5.27.0rc1/upb/mini_table/internal/message.h`

 * *Files 23% similar despite different names*

```diff
@@ -54,106 +54,130 @@
   uint16_t UPB_ONLYBITS(field_count);
 
   uint8_t UPB_PRIVATE(ext);  // upb_ExtMode, uint8_t here so sizeof(ext) == 1
   uint8_t UPB_PRIVATE(dense_below);
   uint8_t UPB_PRIVATE(table_mask);
   uint8_t UPB_PRIVATE(required_count);  // Required fields have the low hasbits.
 
+#ifdef UPB_TRACING_ENABLED
+  const char* UPB_PRIVATE(full_name);
+#endif
+
+#ifdef UPB_FASTTABLE_ENABLED
   // To statically initialize the tables of variable length, we need a flexible
   // array member, and we need to compile in gnu99 mode (constant initialization
   // of flexible array members is a GNU extension, not in C99 unfortunately.
   _upb_FastTable_Entry UPB_PRIVATE(fasttable)[];
+#endif
 };
 // LINT.ThenChange(//depot/google3/third_party/upb/bits/typescript/mini_table.ts)
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 UPB_INLINE const struct upb_MiniTable* UPB_PRIVATE(_upb_MiniTable_Empty)(void) {
   extern const struct upb_MiniTable UPB_PRIVATE(_kUpb_MiniTable_Empty);
 
   return &UPB_PRIVATE(_kUpb_MiniTable_Empty);
 }
 
-UPB_INLINE int UPB_PRIVATE(_upb_MiniTable_FieldCount)(
-    const struct upb_MiniTable* m) {
+UPB_API_INLINE int upb_MiniTable_FieldCount(const struct upb_MiniTable* m) {
   return m->UPB_ONLYBITS(field_count);
 }
 
 UPB_INLINE bool UPB_PRIVATE(_upb_MiniTable_IsEmpty)(
     const struct upb_MiniTable* m) {
   extern const struct upb_MiniTable UPB_PRIVATE(_kUpb_MiniTable_Empty);
 
   return m == &UPB_PRIVATE(_kUpb_MiniTable_Empty);
 }
 
-UPB_INLINE const struct upb_MiniTableField* UPB_PRIVATE(
-    _upb_MiniTable_GetFieldByIndex)(const struct upb_MiniTable* m, uint32_t i) {
+UPB_API_INLINE const struct upb_MiniTableField* upb_MiniTable_GetFieldByIndex(
+    const struct upb_MiniTable* m, uint32_t i) {
   return &m->UPB_ONLYBITS(fields)[i];
 }
 
 UPB_INLINE const union upb_MiniTableSub* UPB_PRIVATE(
     _upb_MiniTable_GetSubByIndex)(const struct upb_MiniTable* m, uint32_t i) {
   return &m->UPB_PRIVATE(subs)[i];
 }
 
-UPB_INLINE const struct upb_MiniTable* UPB_PRIVATE(
-    _upb_MiniTable_GetSubMessageTable)(const struct upb_MiniTable* m,
-                                       const struct upb_MiniTableField* f) {
-  UPB_ASSERT(UPB_PRIVATE(_upb_MiniTableField_CType)(f) == kUpb_CType_Message);
-  const struct upb_MiniTable* ret = UPB_PRIVATE(_upb_MiniTableSub_Message)(
+UPB_API_INLINE const struct upb_MiniTable* upb_MiniTable_GetSubMessageTable(
+    const struct upb_MiniTable* m, const struct upb_MiniTableField* f) {
+  UPB_ASSERT(upb_MiniTableField_CType(f) == kUpb_CType_Message);
+  const struct upb_MiniTable* ret = upb_MiniTableSub_Message(
       m->UPB_PRIVATE(subs)[f->UPB_PRIVATE(submsg_index)]);
   UPB_ASSUME(ret);
   return UPB_PRIVATE(_upb_MiniTable_IsEmpty)(ret) ? NULL : ret;
 }
 
-UPB_INLINE const struct upb_MiniTableEnum* UPB_PRIVATE(
-    _upb_MiniTable_GetSubEnumTable)(const struct upb_MiniTable* m,
-                                    const struct upb_MiniTableField* f) {
-  UPB_ASSERT(UPB_PRIVATE(_upb_MiniTableField_CType)(f) == kUpb_CType_Enum);
-  return UPB_PRIVATE(_upb_MiniTableSub_Enum)(
+UPB_API_INLINE const struct upb_MiniTable* upb_MiniTable_SubMessage(
+    const struct upb_MiniTable* m, const struct upb_MiniTableField* f) {
+  if (upb_MiniTableField_CType(f) != kUpb_CType_Message) {
+    return NULL;
+  }
+  return upb_MiniTableSub_Message(
+      m->UPB_PRIVATE(subs)[f->UPB_PRIVATE(submsg_index)]);
+}
+
+UPB_API_INLINE const struct upb_MiniTableEnum* upb_MiniTable_GetSubEnumTable(
+    const struct upb_MiniTable* m, const struct upb_MiniTableField* f) {
+  UPB_ASSERT(upb_MiniTableField_CType(f) == kUpb_CType_Enum);
+  return upb_MiniTableSub_Enum(
       m->UPB_PRIVATE(subs)[f->UPB_PRIVATE(submsg_index)]);
 }
 
-UPB_INLINE const struct upb_MiniTableField* UPB_PRIVATE(_upb_MiniTable_MapKey)(
+UPB_API_INLINE const struct upb_MiniTableField* upb_MiniTable_MapKey(
     const struct upb_MiniTable* m) {
-  UPB_ASSERT(UPB_PRIVATE(_upb_MiniTable_FieldCount)(m) == 2);
-  const struct upb_MiniTableField* f =
-      UPB_PRIVATE(_upb_MiniTable_GetFieldByIndex)(m, 0);
-  UPB_ASSERT(UPB_PRIVATE(_upb_MiniTableField_Number)(f) == 1);
+  UPB_ASSERT(upb_MiniTable_FieldCount(m) == 2);
+  const struct upb_MiniTableField* f = upb_MiniTable_GetFieldByIndex(m, 0);
+  UPB_ASSERT(upb_MiniTableField_Number(f) == 1);
   return f;
 }
 
-UPB_INLINE const struct upb_MiniTableField* UPB_PRIVATE(
-    _upb_MiniTable_MapValue)(const struct upb_MiniTable* m) {
-  UPB_ASSERT(UPB_PRIVATE(_upb_MiniTable_FieldCount)(m) == 2);
-  const struct upb_MiniTableField* f =
-      UPB_PRIVATE(_upb_MiniTable_GetFieldByIndex)(m, 1);
-  UPB_ASSERT(UPB_PRIVATE(_upb_MiniTableField_Number)(f) == 2);
+UPB_API_INLINE const struct upb_MiniTableField* upb_MiniTable_MapValue(
+    const struct upb_MiniTable* m) {
+  UPB_ASSERT(upb_MiniTable_FieldCount(m) == 2);
+  const struct upb_MiniTableField* f = upb_MiniTable_GetFieldByIndex(m, 1);
+  UPB_ASSERT(upb_MiniTableField_Number(f) == 2);
   return f;
 }
 
-UPB_INLINE bool UPB_PRIVATE(_upb_MiniTable_MessageFieldIsLinked)(
+UPB_API_INLINE bool upb_MiniTable_FieldIsLinked(
     const struct upb_MiniTable* m, const struct upb_MiniTableField* f) {
-  return UPB_PRIVATE(_upb_MiniTable_GetSubMessageTable)(m, f) != NULL;
+  return upb_MiniTable_GetSubMessageTable(m, f) != NULL;
 }
 
 // Computes a bitmask in which the |m->required_count| lowest bits are set.
 //
 // Sample output:
 //    RequiredMask(1) => 0b1 (0x1)
 //    RequiredMask(5) => 0b11111 (0x1f)
 UPB_INLINE uint64_t
 UPB_PRIVATE(_upb_MiniTable_RequiredMask)(const struct upb_MiniTable* m) {
   int n = m->UPB_PRIVATE(required_count);
   UPB_ASSERT(0 < n && n <= 64);
   return (1ULL << n) - 1;
 }
 
+#ifdef UPB_TRACING_ENABLED
+UPB_INLINE const char* upb_MiniTable_FullName(
+    const struct upb_MiniTable* mini_table) {
+  return mini_table->UPB_PRIVATE(full_name);
+}
+// Initializes tracing proto name from language runtimes that construct
+// mini tables dynamically at runtime. The runtime is responsible for passing
+// controlling lifetime of name such as storing in same arena as mini_table.
+UPB_INLINE void upb_MiniTable_SetFullName(struct upb_MiniTable* mini_table,
+                                          const char* full_name) {
+  mini_table->UPB_PRIVATE(full_name) = full_name;
+}
+#endif
+
 #ifdef __cplusplus
 } /* extern "C" */
 #endif
 
 #include "upb/port/undef.inc"
 
 #endif /* UPB_MINI_TABLE_INTERNAL_MESSAGE_H_ */
```

### Comparing `protobuf-5.26.1/upb/mini_table/internal/size_log2.h` & `protobuf-5.27.0rc1/upb/mini_table/internal/size_log2.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/mini_table/internal/sub.h` & `protobuf-5.27.0rc1/upb/mini_table/internal/sub.h`

 * *Files 13% similar despite different names*

```diff
@@ -16,34 +16,34 @@
   const struct upb_MiniTableEnum* UPB_PRIVATE(subenum);
 };
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
-UPB_INLINE union upb_MiniTableSub UPB_PRIVATE(_upb_MiniTableSub_FromEnum)(
+UPB_API_INLINE union upb_MiniTableSub upb_MiniTableSub_FromEnum(
     const struct upb_MiniTableEnum* subenum) {
   union upb_MiniTableSub out;
   out.UPB_PRIVATE(subenum) = subenum;
   return out;
 }
 
-UPB_INLINE union upb_MiniTableSub UPB_PRIVATE(_upb_MiniTableSub_FromMessage)(
+UPB_API_INLINE union upb_MiniTableSub upb_MiniTableSub_FromMessage(
     const struct upb_MiniTable* submsg) {
   union upb_MiniTableSub out;
   out.UPB_PRIVATE(submsg) = submsg;
   return out;
 }
 
-UPB_INLINE const struct upb_MiniTableEnum* UPB_PRIVATE(_upb_MiniTableSub_Enum)(
+UPB_API_INLINE const struct upb_MiniTableEnum* upb_MiniTableSub_Enum(
     const union upb_MiniTableSub sub) {
   return sub.UPB_PRIVATE(subenum);
 }
 
-UPB_INLINE const struct upb_MiniTable* UPB_PRIVATE(_upb_MiniTableSub_Message)(
+UPB_API_INLINE const struct upb_MiniTable* upb_MiniTableSub_Message(
     const union upb_MiniTableSub sub) {
   return sub.UPB_PRIVATE(submsg);
 }
 
 #ifdef __cplusplus
 } /* extern "C" */
 #endif
```

### Comparing `protobuf-5.26.1/upb/mini_table/message.c` & `protobuf-5.27.0rc1/upb/mini_table/message.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/mini_table/message.h` & `protobuf-5.27.0rc1/upb/mini_table/message.h`

 * *Files 14% similar despite different names*

```diff
@@ -21,52 +21,43 @@
 extern "C" {
 #endif
 
 UPB_API const upb_MiniTableField* upb_MiniTable_FindFieldByNumber(
     const upb_MiniTable* m, uint32_t number);
 
 UPB_API_INLINE const upb_MiniTableField* upb_MiniTable_GetFieldByIndex(
-    const upb_MiniTable* m, uint32_t index) {
-  return UPB_PRIVATE(_upb_MiniTable_GetFieldByIndex)(m, index);
-}
-
-UPB_API_INLINE int upb_MiniTable_FieldCount(const upb_MiniTable* m) {
-  return UPB_PRIVATE(_upb_MiniTable_FieldCount)(m);
-}
+    const upb_MiniTable* m, uint32_t index);
 
+UPB_API_INLINE int upb_MiniTable_FieldCount(const upb_MiniTable* m);
+
+// DEPRECATED: use upb_MiniTable_SubMessage() instead
 // Returns the MiniTable for a message field, NULL if the field is unlinked.
 UPB_API_INLINE const upb_MiniTable* upb_MiniTable_GetSubMessageTable(
-    const upb_MiniTable* m, const upb_MiniTableField* f) {
-  return UPB_PRIVATE(_upb_MiniTable_GetSubMessageTable)(m, f);
-}
+    const upb_MiniTable* m, const upb_MiniTableField* f);
+
+// Returns the MiniTable for a message field if it is a submessage.
+UPB_API_INLINE const upb_MiniTable* upb_MiniTable_SubMessage(
+    const upb_MiniTable* m, const upb_MiniTableField* f);
 
 // Returns the MiniTableEnum for a message field, NULL if the field is unlinked.
 UPB_API_INLINE const upb_MiniTableEnum* upb_MiniTable_GetSubEnumTable(
-    const upb_MiniTable* m, const upb_MiniTableField* f) {
-  return UPB_PRIVATE(_upb_MiniTable_GetSubEnumTable)(m, f);
-}
+    const upb_MiniTable* m, const upb_MiniTableField* f);
 
 // Returns the MiniTableField for the key of a map.
 UPB_API_INLINE const upb_MiniTableField* upb_MiniTable_MapKey(
-    const upb_MiniTable* m) {
-  return UPB_PRIVATE(_upb_MiniTable_MapKey)(m);
-}
+    const upb_MiniTable* m);
 
 // Returns the MiniTableField for the value of a map.
 UPB_API_INLINE const upb_MiniTableField* upb_MiniTable_MapValue(
-    const upb_MiniTable* m) {
-  return UPB_PRIVATE(_upb_MiniTable_MapValue)(m);
-}
+    const upb_MiniTable* m);
 
 // Returns true if this MiniTable field is linked to a MiniTable for the
 // sub-message.
-UPB_API_INLINE bool upb_MiniTable_MessageFieldIsLinked(
-    const upb_MiniTable* m, const upb_MiniTableField* f) {
-  return UPB_PRIVATE(_upb_MiniTable_MessageFieldIsLinked)(m, f);
-}
+UPB_API_INLINE bool upb_MiniTable_FieldIsLinked(const upb_MiniTable* m,
+                                                const upb_MiniTableField* f);
 
 // If this field is in a oneof, returns the first field in the oneof.
 //
 // Otherwise returns NULL.
 //
 // Usage:
 //   const upb_MiniTableField* field = upb_MiniTable_GetOneof(m, f);
```

### Comparing `protobuf-5.26.1/upb/mini_table/sub.h` & `protobuf-5.27.0rc1/upb/mini_table/sub.h`

 * *Files 17% similar despite different names*

```diff
@@ -20,34 +20,26 @@
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 // Constructors
 
 UPB_API_INLINE upb_MiniTableSub
-upb_MiniTableSub_FromEnum(const upb_MiniTableEnum* subenum) {
-  return UPB_PRIVATE(_upb_MiniTableSub_FromEnum)(subenum);
-}
+upb_MiniTableSub_FromEnum(const upb_MiniTableEnum* subenum);
 
 UPB_API_INLINE upb_MiniTableSub
-upb_MiniTableSub_FromMessage(const upb_MiniTable* submsg) {
-  return UPB_PRIVATE(_upb_MiniTableSub_FromMessage)(submsg);
-}
+upb_MiniTableSub_FromMessage(const upb_MiniTable* submsg);
 
 // Getters
 
 UPB_API_INLINE const upb_MiniTableEnum* upb_MiniTableSub_Enum(
-    upb_MiniTableSub sub) {
-  return UPB_PRIVATE(_upb_MiniTableSub_Enum)(sub);
-}
+    upb_MiniTableSub sub);
 
 UPB_API_INLINE const upb_MiniTable* upb_MiniTableSub_Message(
-    upb_MiniTableSub sub) {
-  return UPB_PRIVATE(_upb_MiniTableSub_Message)(sub);
-}
+    upb_MiniTableSub sub);
 
 #ifdef __cplusplus
 } /* extern "C" */
 #endif
 
 #include "upb/port/undef.inc"
```

### Comparing `protobuf-5.26.1/upb/port/atomic.h` & `protobuf-5.27.0rc1/upb/port/atomic.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/port/def.inc` & `protobuf-5.27.0rc1/upb/port/def.inc`

 * *Files 2% similar despite different names*

```diff
@@ -113,25 +113,25 @@
 #else
 #define UPB_LIKELY(x) (x)
 #define UPB_UNLIKELY(x) (x)
 #endif
 
 // Macros for function attributes on compilers that support them.
 #ifdef __GNUC__
-#define UPB_FORCEINLINE __inline__ __attribute__((always_inline))
+#define UPB_FORCEINLINE __inline__ __attribute__((always_inline)) static
 #define UPB_NOINLINE __attribute__((noinline))
 #define UPB_NORETURN __attribute__((__noreturn__))
 #define UPB_PRINTF(str, first_vararg) __attribute__((format (printf, str, first_vararg)))
 #elif defined(_MSC_VER)
 #define UPB_NOINLINE
-#define UPB_FORCEINLINE
+#define UPB_FORCEINLINE static
 #define UPB_NORETURN __declspec(noreturn)
 #define UPB_PRINTF(str, first_vararg)
 #else  /* !defined(__GNUC__) */
-#define UPB_FORCEINLINE
+#define UPB_FORCEINLINE static
 #define UPB_NOINLINE
 #define UPB_NORETURN
 #define UPB_PRINTF(str, first_vararg)
 #endif
 
 #define UPB_MAX(x, y) ((x) > (y) ? (x) : (y))
 #define UPB_MIN(x, y) ((x) < (y) ? (x) : (y))
@@ -305,18 +305,18 @@
   ((void)(addr), (void)(size))
 #define UPB_UNPOISON_MEMORY_REGION(addr, size) \
   ((void)(addr), (void)(size))
 #endif
 
 /* Disable proto2 arena behavior (TEMPORARY) **********************************/
 
-#ifdef UPB_DISABLE_PROTO2_ENUM_CHECKING
-#define UPB_TREAT_PROTO2_ENUMS_LIKE_PROTO3 1
+#ifdef UPB_DISABLE_CLOSED_ENUM_CHECKING
+#define UPB_TREAT_CLOSED_ENUMS_LIKE_OPEN 1
 #else
-#define UPB_TREAT_PROTO2_ENUMS_LIKE_PROTO3 0
+#define UPB_TREAT_CLOSED_ENUMS_LIKE_OPEN 0
 #endif
 
 #if defined(__cplusplus)
 #if defined(__clang__) || UPB_GNUC_MIN(6, 0)
 // https://gcc.gnu.org/gcc-6/changes.html
 #if __cplusplus >= 201402L
 #define UPB_DEPRECATED [[deprecated]]
@@ -340,7 +340,13 @@
 #elif defined(UPB_BOOTSTRAP_STAGE0)
 #define UPB_DESC(sym) google_protobuf_##sym
 #define UPB_DESC_MINITABLE(sym) google__protobuf__##sym##_msg_init()
 #else
 #define UPB_DESC(sym) google_protobuf_##sym
 #define UPB_DESC_MINITABLE(sym) &google__protobuf__##sym##_msg_init
 #endif
+
+#ifdef UPB_TRACING_ENABLED
+#ifdef NDEBUG
+error UPB_TRACING_ENABLED Tracing should be disabled in production builds
+#endif
+#endif
```

### Comparing `protobuf-5.26.1/upb/port/undef.inc` & `protobuf-5.27.0rc1/upb/port/undef.inc`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 #undef UPB_FASTTABLE
 #undef UPB_FASTTABLE_INIT
 #undef UPB_POISON_MEMORY_REGION
 #undef UPB_UNPOISON_MEMORY_REGION
 #undef UPB_ASAN
 #undef UPB_ASAN_GUARD_SIZE
 #undef UPB_CLANG_ASAN
-#undef UPB_TREAT_PROTO2_ENUMS_LIKE_PROTO3
+#undef UPB_TREAT_CLOSED_ENUMS_LIKE_OPEN
 #undef UPB_DEPRECATED
 #undef UPB_GNUC_MIN
 #undef UPB_DESCRIPTOR_UPB_H_FILENAME
 #undef UPB_DESC
 #undef UPB_DESC_MINITABLE
 #undef UPB_IS_GOOGLE3
 #undef UPB_ATOMIC
```

### Comparing `protobuf-5.26.1/upb/port/vsnprintf_compat.h` & `protobuf-5.27.0rc1/upb/port/vsnprintf_compat.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/reflection/common.h` & `protobuf-5.27.0rc1/upb/reflection/common.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/reflection/def.h` & `protobuf-5.27.0rc1/upb/reflection/def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/reflection/def_pool.c` & `protobuf-5.27.0rc1/upb/reflection/def_pool.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/reflection/def_pool.h` & `protobuf-5.27.0rc1/upb/reflection/def_pool.h`

 * *Files 2% similar despite different names*

```diff
@@ -62,16 +62,16 @@
 const upb_FieldDef* upb_DefPool_FindExtensionByNameWithSize(
     const upb_DefPool* s, const char* name, size_t size);
 
 const upb_FieldDef* upb_DefPool_FindExtensionByNumber(const upb_DefPool* s,
                                                       const upb_MessageDef* m,
                                                       int32_t fieldnum);
 
-const upb_ServiceDef* upb_DefPool_FindServiceByName(const upb_DefPool* s,
-                                                    const char* name);
+UPB_API const upb_ServiceDef* upb_DefPool_FindServiceByName(
+  const upb_DefPool* s, const char* name);
 
 const upb_ServiceDef* upb_DefPool_FindServiceByNameWithSize(
     const upb_DefPool* s, const char* name, size_t size);
 
 const upb_FileDef* upb_DefPool_FindFileContainingSymbol(const upb_DefPool* s,
                                                         const char* name);
```

### Comparing `protobuf-5.26.1/upb/reflection/def_type.c` & `protobuf-5.27.0rc1/upb/reflection/def_type.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/reflection/def_type.h` & `protobuf-5.27.0rc1/upb/reflection/def_type.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/reflection/desc_state.c` & `protobuf-5.27.0rc1/upb/reflection/desc_state.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/reflection/enum_def.c` & `protobuf-5.27.0rc1/upb/reflection/enum_def.c`

 * *Files 2% similar despite different names*

```diff
@@ -156,15 +156,19 @@
 
 const upb_EnumValueDef* upb_EnumDef_Value(const upb_EnumDef* e, int i) {
   UPB_ASSERT(0 <= i && i < e->value_count);
   return _upb_EnumValueDef_At(e->values, i);
 }
 
 bool upb_EnumDef_IsClosed(const upb_EnumDef* e) {
-  if (UPB_TREAT_PROTO2_ENUMS_LIKE_PROTO3) return false;
+  if (UPB_TREAT_CLOSED_ENUMS_LIKE_OPEN) return false;
+  return upb_EnumDef_IsSpecifiedAsClosed(e);
+}
+
+bool upb_EnumDef_IsSpecifiedAsClosed(const upb_EnumDef* e) {
   return UPB_DESC(FeatureSet_enum_type)(e->resolved_features) ==
          UPB_DESC(FeatureSet_CLOSED);
 }
 
 bool upb_EnumDef_MiniDescriptorEncode(const upb_EnumDef* e, upb_Arena* a,
                                       upb_StringView* out) {
   upb_DescState s;
```

### Comparing `protobuf-5.26.1/upb/reflection/enum_def.h` & `protobuf-5.27.0rc1/upb/reflection/enum_def.h`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 UPB_API const upb_EnumValueDef* upb_EnumDef_FindValueByNameWithSize(
     const upb_EnumDef* e, const char* name, size_t size);
 UPB_API const upb_EnumValueDef* upb_EnumDef_FindValueByNumber(
     const upb_EnumDef* e, int32_t num);
 UPB_API const char* upb_EnumDef_FullName(const upb_EnumDef* e);
 bool upb_EnumDef_HasOptions(const upb_EnumDef* e);
 bool upb_EnumDef_IsClosed(const upb_EnumDef* e);
+bool upb_EnumDef_IsSpecifiedAsClosed(const upb_EnumDef* e);
 
 // Creates a mini descriptor string for an enum, returns true on success.
 bool upb_EnumDef_MiniDescriptorEncode(const upb_EnumDef* e, upb_Arena* a,
                                       upb_StringView* out);
 
 const char* upb_EnumDef_Name(const upb_EnumDef* e);
 const UPB_DESC(EnumOptions) * upb_EnumDef_Options(const upb_EnumDef* e);
```

### Comparing `protobuf-5.26.1/upb/reflection/enum_reserved_range.c` & `protobuf-5.27.0rc1/upb/reflection/enum_reserved_range.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/reflection/enum_reserved_range.h` & `protobuf-5.27.0rc1/upb/reflection/enum_reserved_range.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/reflection/enum_value_def.c` & `protobuf-5.27.0rc1/upb/reflection/enum_value_def.c`

 * *Files 2% similar despite different names*

```diff
@@ -109,23 +109,18 @@
   bool ok = _upb_EnumDef_Insert(e, v, ctx->arena);
   if (!ok) _upb_DefBuilder_OomErr(ctx);
 }
 
 static void _upb_EnumValueDef_CheckZeroValue(upb_DefBuilder* ctx,
                                              const upb_EnumDef* e,
                                              const upb_EnumValueDef* v, int n) {
-  if (upb_EnumDef_IsClosed(e) || n == 0 || v[0].number == 0) return;
-
-  // When the special UPB_TREAT_PROTO2_ENUMS_LIKE_PROTO3 is enabled, we have to
-  // exempt proto2 enums from this check, even when we are treating them as
+  // When the special UPB_TREAT_CLOSED_ENUMS_LIKE_OPEN is enabled, we have to
+  // exempt closed enums from this check, even when we are treating them as
   // open.
-  if (UPB_TREAT_PROTO2_ENUMS_LIKE_PROTO3 &&
-      upb_FileDef_Syntax(upb_EnumDef_File(e)) == kUpb_Syntax_Proto2) {
-    return;
-  }
+  if (upb_EnumDef_IsSpecifiedAsClosed(e) || n == 0 || v[0].number == 0) return;
 
   _upb_DefBuilder_Errf(ctx, "for open enums, the first value must be zero (%s)",
                        upb_EnumDef_FullName(e));
 }
 
 // Allocate and initialize an array of |n| enum value defs owned by |e|.
 upb_EnumValueDef* _upb_EnumValueDefs_New(
```

### Comparing `protobuf-5.26.1/upb/reflection/enum_value_def.h` & `protobuf-5.27.0rc1/upb/reflection/enum_value_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/reflection/extension_range.c` & `protobuf-5.27.0rc1/upb/reflection/extension_range.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/reflection/extension_range.h` & `protobuf-5.27.0rc1/upb/reflection/extension_range.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/reflection/field_def.c` & `protobuf-5.27.0rc1/upb/reflection/field_def.c`

 * *Files 2% similar despite different names*

```diff
@@ -106,35 +106,24 @@
   return f->full_name;
 }
 
 upb_CType upb_FieldDef_CType(const upb_FieldDef* f) {
   return upb_FieldType_CType(f->type_);
 }
 
-upb_FieldType upb_FieldDef_Type(const upb_FieldDef* f) {
-  // TODO: remove once we can deprecate kUpb_FieldType_Group.
-  if (f->type_ == kUpb_FieldType_Message &&
-      UPB_DESC(FeatureSet_message_encoding)(f->resolved_features) ==
-          UPB_DESC(FeatureSet_DELIMITED)) {
-    return kUpb_FieldType_Group;
-  }
-  return f->type_;
-}
+upb_FieldType upb_FieldDef_Type(const upb_FieldDef* f) { return f->type_; }
 
 uint32_t upb_FieldDef_Index(const upb_FieldDef* f) { return f->index_; }
 
-upb_Label upb_FieldDef_Label(const upb_FieldDef* f) {
-  // TODO: remove once we can deprecate kUpb_Label_Required.
-  if (UPB_DESC(FeatureSet_field_presence)(f->resolved_features) ==
-      UPB_DESC(FeatureSet_LEGACY_REQUIRED)) {
-    return kUpb_Label_Required;
-  }
-  return f->label_;
+uint32_t upb_FieldDef_LayoutIndex(const upb_FieldDef* f) {
+  return f->layout_index;
 }
 
+upb_Label upb_FieldDef_Label(const upb_FieldDef* f) { return f->label_; }
+
 uint32_t upb_FieldDef_Number(const upb_FieldDef* f) { return f->number_; }
 
 bool upb_FieldDef_IsExtension(const upb_FieldDef* f) { return f->is_extension; }
 
 bool _upb_FieldDef_IsPackable(const upb_FieldDef* f) {
   return upb_FieldDef_IsRepeated(f) && upb_FieldDef_IsPrimitive(f);
 }
@@ -257,14 +246,48 @@
 
 bool _upb_FieldDef_ValidateUtf8(const upb_FieldDef* f) {
   if (upb_FieldDef_Type(f) != kUpb_FieldType_String) return false;
   return UPB_DESC(FeatureSet_utf8_validation(f->resolved_features)) ==
          UPB_DESC(FeatureSet_VERIFY);
 }
 
+bool _upb_FieldDef_IsGroupLike(const upb_FieldDef* f) {
+  // Groups are always tag-delimited.
+  if (UPB_DESC(FeatureSet_message_encoding)(upb_FieldDef_ResolvedFeatures(f)) !=
+      UPB_DESC(FeatureSet_DELIMITED)) {
+    return false;
+  }
+
+  const upb_MessageDef* msg = upb_FieldDef_MessageSubDef(f);
+
+  // Group fields always are always the lowercase type name.
+  const char* mname = upb_MessageDef_Name(msg);
+  const char* fname = upb_FieldDef_Name(f);
+  size_t name_size = strlen(fname);
+  if (name_size != strlen(mname)) return false;
+  for (size_t i = 0; i < name_size; ++i) {
+    if ((mname[i] | 0x20) != fname[i]) {
+      // Case-insensitive ascii comparison.
+      return false;
+    }
+  }
+
+  if (upb_MessageDef_File(msg) != upb_FieldDef_File(f)) {
+    return false;
+  }
+
+  // Group messages are always defined in the same scope as the field.  File
+  // level extensions will compare NULL == NULL here, which is why the file
+  // comparison above is necessary to ensure both come from the same file.
+  return upb_FieldDef_IsExtension(f) ? upb_FieldDef_ExtensionScope(f) ==
+                                           upb_MessageDef_ContainingType(msg)
+                                     : upb_FieldDef_ContainingType(f) ==
+                                           upb_MessageDef_ContainingType(msg);
+}
+
 uint64_t _upb_FieldDef_Modifiers(const upb_FieldDef* f) {
   uint64_t out = upb_FieldDef_IsPacked(f) ? kUpb_FieldModifier_IsPacked : 0;
 
   if (upb_FieldDef_IsRepeated(f)) {
     out |= kUpb_FieldModifier_IsRepeated;
   } else if (upb_FieldDef_IsRequired(f)) {
     out |= kUpb_FieldModifier_IsRequired;
@@ -588,15 +611,14 @@
                                      field_proto,
                                  upb_MessageDef* m, upb_FieldDef* f) {
   // Must happen before _upb_DefBuilder_Add()
   f->file = _upb_DefBuilder_File(ctx);
 
   const upb_StringView name = UPB_DESC(FieldDescriptorProto_name)(field_proto);
   f->full_name = _upb_DefBuilder_MakeFullName(ctx, prefix, name);
-  f->label_ = (int)UPB_DESC(FieldDescriptorProto_label)(field_proto);
   f->number_ = UPB_DESC(FieldDescriptorProto_number)(field_proto);
   f->is_proto3_optional =
       UPB_DESC(FieldDescriptorProto_proto3_optional)(field_proto);
   f->msgdef = m;
   f->scope.oneof = NULL;
 
   UPB_DEF_SET_OPTIONS(f->opts, FieldDescriptorProto, FieldOptions, field_proto);
@@ -634,14 +656,22 @@
 
     _upb_OneofDef_Insert(ctx, oneof, f, name.data, name.size);
   }
 
   f->resolved_features = _upb_DefBuilder_DoResolveFeatures(
       ctx, parent_features, unresolved_features, implicit);
 
+  f->label_ = (int)UPB_DESC(FieldDescriptorProto_label)(field_proto);
+  if (f->label_ == kUpb_Label_Optional &&
+      // TODO: remove once we can deprecate kUpb_Label_Required.
+      UPB_DESC(FeatureSet_field_presence)(f->resolved_features) ==
+          UPB_DESC(FeatureSet_LEGACY_REQUIRED)) {
+    f->label_ = kUpb_Label_Required;
+  }
+
   if (!UPB_DESC(FieldDescriptorProto_has_name)(field_proto)) {
     _upb_DefBuilder_Errf(ctx, "field has no name");
   }
 
   f->has_json_name = UPB_DESC(FieldDescriptorProto_has_json_name)(field_proto);
   if (f->has_json_name) {
     const upb_StringView sv =
@@ -653,14 +683,20 @@
   if (!f->json_name) _upb_DefBuilder_OomErr(ctx);
 
   const bool has_type = UPB_DESC(FieldDescriptorProto_has_type)(field_proto);
   const bool has_type_name =
       UPB_DESC(FieldDescriptorProto_has_type_name)(field_proto);
 
   f->type_ = (int)UPB_DESC(FieldDescriptorProto_type)(field_proto);
+  if (f->type_ == kUpb_FieldType_Message &&
+      // TODO: remove once we can deprecate kUpb_FieldType_Group.
+      UPB_DESC(FeatureSet_message_encoding)(f->resolved_features) ==
+          UPB_DESC(FeatureSet_DELIMITED)) {
+    f->type_ = kUpb_FieldType_Group;
+  }
 
   if (has_type) {
     switch (f->type_) {
       case kUpb_FieldType_Message:
       case kUpb_FieldType_Group:
       case kUpb_FieldType_Enum:
         if (!has_type_name) {
@@ -702,18 +738,19 @@
       _upb_DefBuilder_Errf(ctx, "fields in oneof must have OPTIONAL label (%s)",
                            f->full_name);
     }
   }
 
   f->has_presence =
       (!upb_FieldDef_IsRepeated(f)) &&
-      (f->type_ == kUpb_FieldType_Message || f->type_ == kUpb_FieldType_Group ||
-       upb_FieldDef_ContainingOneof(f) ||
-       UPB_DESC(FeatureSet_field_presence)(f->resolved_features) !=
-           UPB_DESC(FeatureSet_IMPLICIT));
+      (f->is_extension ||
+       (f->type_ == kUpb_FieldType_Message ||
+        f->type_ == kUpb_FieldType_Group || upb_FieldDef_ContainingOneof(f) ||
+        UPB_DESC(FeatureSet_field_presence)(f->resolved_features) !=
+            UPB_DESC(FeatureSet_IMPLICIT)));
 }
 
 static void _upb_FieldDef_CreateExt(upb_DefBuilder* ctx, const char* prefix,
                                     const UPB_DESC(FeatureSet*) parent_features,
                                     const UPB_DESC(FieldDescriptorProto*)
                                         field_proto,
                                     upb_MessageDef* m, upb_FieldDef* f) {
```

### Comparing `protobuf-5.26.1/upb/reflection/field_def.h` & `protobuf-5.27.0rc1/upb/reflection/field_def.h`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 #ifndef UPB_REFLECTION_FIELD_DEF_H_
 #define UPB_REFLECTION_FIELD_DEF_H_
 
 #include <stdint.h>
 
 #include "upb/base/descriptor_constants.h"
 #include "upb/base/string_view.h"
+#include "upb/message/value.h"
 #include "upb/mini_table/extension.h"
 #include "upb/mini_table/field.h"
 #include "upb/reflection/common.h"
 
 // Must be last.
 #include "upb/port/def.inc"
 
@@ -51,16 +52,18 @@
 bool upb_FieldDef_IsPrimitive(const upb_FieldDef* f);
 UPB_API bool upb_FieldDef_IsRepeated(const upb_FieldDef* f);
 bool upb_FieldDef_IsRequired(const upb_FieldDef* f);
 bool upb_FieldDef_IsString(const upb_FieldDef* f);
 UPB_API bool upb_FieldDef_IsSubMessage(const upb_FieldDef* f);
 UPB_API const char* upb_FieldDef_JsonName(const upb_FieldDef* f);
 UPB_API upb_Label upb_FieldDef_Label(const upb_FieldDef* f);
+uint32_t upb_FieldDef_LayoutIndex(const upb_FieldDef* f);
 UPB_API const upb_MessageDef* upb_FieldDef_MessageSubDef(const upb_FieldDef* f);
 bool _upb_FieldDef_ValidateUtf8(const upb_FieldDef* f);
+bool _upb_FieldDef_IsGroupLike(const upb_FieldDef* f);
 
 // Creates a mini descriptor string for a field, returns true on success.
 bool upb_FieldDef_MiniDescriptorEncode(const upb_FieldDef* f, upb_Arena* a,
                                        upb_StringView* out);
 
 const upb_MiniTableField* upb_FieldDef_MiniTable(const upb_FieldDef* f);
 const upb_MiniTableExtension* upb_FieldDef_MiniTableExtension(
```

### Comparing `protobuf-5.26.1/upb/reflection/file_def.c` & `protobuf-5.27.0rc1/upb/reflection/file_def.c`

 * *Files 3% similar despite different names*

```diff
@@ -166,14 +166,25 @@
 const upb_DefPool* upb_FileDef_Pool(const upb_FileDef* f) { return f->symtab; }
 
 const upb_MiniTableExtension* _upb_FileDef_ExtensionMiniTable(
     const upb_FileDef* f, int i) {
   return f->ext_layouts[i];
 }
 
+// Note: Import cycles are not allowed so this will terminate.
+bool upb_FileDef_Resolves(const upb_FileDef* f, const char* path) {
+  if (!strcmp(f->name, path)) return true;
+
+  for (int i = 0; i < upb_FileDef_PublicDependencyCount(f); i++) {
+    const upb_FileDef* dep = upb_FileDef_PublicDependency(f, i);
+    if (upb_FileDef_Resolves(dep, path)) return true;
+  }
+  return false;
+}
+
 static char* strviewdup(upb_DefBuilder* ctx, upb_StringView view) {
   char* ret = upb_strdup2(view.data, view.size, _upb_DefBuilder_Arena(ctx));
   if (!ret) _upb_DefBuilder_OomErr(ctx);
   return ret;
 }
 
 static bool streql_view(upb_StringView view, const char* b) {
@@ -217,28 +228,43 @@
                          upb_FileDef_EditionName(max));
     return NULL;
   }
 
   size_t n;
   const UPB_DESC(FeatureSetDefaults_FeatureSetEditionDefault)* const* d =
       UPB_DESC(FeatureSetDefaults_defaults)(defaults, &n);
-  const UPB_DESC(FeatureSet)* ret = NULL;
+  const UPB_DESC(FeatureSetDefaults_FeatureSetEditionDefault)* result = NULL;
   for (size_t i = 0; i < n; i++) {
     if (UPB_DESC(FeatureSetDefaults_FeatureSetEditionDefault_edition)(d[i]) >
         edition) {
       break;
     }
-    ret = UPB_DESC(FeatureSetDefaults_FeatureSetEditionDefault_features)(d[i]);
+    result = d[i];
   }
-  if (ret == NULL) {
+  if (result == NULL) {
     _upb_DefBuilder_Errf(ctx, "No valid default found for edition %s",
                          upb_FileDef_EditionName(edition));
     return NULL;
   }
-  return ret;
+
+  // Merge the fixed and overridable features to get the edition's default
+  // feature set.
+  const UPB_DESC(FeatureSet)* fixed = UPB_DESC(
+      FeatureSetDefaults_FeatureSetEditionDefault_fixed_features)(result);
+  const UPB_DESC(FeatureSet)* overridable = UPB_DESC(
+      FeatureSetDefaults_FeatureSetEditionDefault_overridable_features)(result);
+  if (!fixed && !overridable) {
+    _upb_DefBuilder_Errf(ctx, "No valid default found for edition %s",
+                         upb_FileDef_EditionName(edition));
+    return NULL;
+  } else if (!fixed) {
+    return overridable;
+  }
+  return _upb_DefBuilder_DoResolveFeatures(ctx, fixed, overridable,
+                                           /*is_implicit=*/true);
 }
 
 // Allocate and initialize one file def, and add it to the context object.
 void _upb_FileDef_Create(upb_DefBuilder* ctx,
                          const UPB_DESC(FileDescriptorProto) * file_proto) {
   upb_FileDef* file = _upb_DefBuilder_Alloc(ctx, sizeof(upb_FileDef));
   ctx->file = file;
```

### Comparing `protobuf-5.26.1/upb/reflection/file_def.h` & `protobuf-5.27.0rc1/upb/reflection/file_def.h`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,17 @@
 
 const upb_MessageDef* upb_FileDef_TopLevelMessage(const upb_FileDef* f, int i);
 int upb_FileDef_TopLevelMessageCount(const upb_FileDef* f);
 
 const upb_FileDef* upb_FileDef_WeakDependency(const upb_FileDef* f, int i);
 int upb_FileDef_WeakDependencyCount(const upb_FileDef* f);
 
+// Returns whether |symbol| is transitively included by |f|
+bool upb_FileDef_Resolves(const upb_FileDef* f, const char* symbol);
+
 #ifdef __cplusplus
 } /* extern "C" */
 #endif
 
 #include "upb/port/undef.inc"
 
 #endif /* UPB_REFLECTION_FILE_DEF_H_ */
```

### Comparing `protobuf-5.26.1/upb/reflection/internal/def_builder.c` & `protobuf-5.27.0rc1/upb/reflection/internal/def_builder.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/reflection/internal/def_builder.h` & `protobuf-5.27.0rc1/upb/reflection/internal/def_builder.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/reflection/internal/def_pool.h` & `protobuf-5.27.0rc1/upb/reflection/internal/def_pool.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/reflection/internal/desc_state.h` & `protobuf-5.27.0rc1/upb/reflection/internal/desc_state.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/reflection/internal/enum_def.h` & `protobuf-5.27.0rc1/upb/reflection/internal/enum_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/reflection/internal/enum_reserved_range.h` & `protobuf-5.27.0rc1/upb/reflection/internal/enum_reserved_range.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/reflection/internal/enum_value_def.h` & `protobuf-5.27.0rc1/upb/reflection/internal/enum_value_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/reflection/internal/extension_range.h` & `protobuf-5.27.0rc1/upb/reflection/internal/extension_range.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/reflection/internal/field_def.h` & `protobuf-5.27.0rc1/upb/reflection/internal/field_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/reflection/internal/file_def.h` & `protobuf-5.27.0rc1/upb/reflection/internal/file_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/reflection/internal/message_def.h` & `protobuf-5.27.0rc1/upb/reflection/internal/message_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/reflection/internal/message_reserved_range.h` & `protobuf-5.27.0rc1/upb/reflection/internal/message_reserved_range.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/reflection/internal/method_def.h` & `protobuf-5.27.0rc1/upb/reflection/internal/method_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/reflection/internal/oneof_def.h` & `protobuf-5.27.0rc1/upb/reflection/internal/oneof_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/reflection/internal/service_def.h` & `protobuf-5.27.0rc1/upb/reflection/internal/service_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/reflection/internal/strdup2.c` & `protobuf-5.27.0rc1/upb/reflection/internal/strdup2.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/reflection/internal/strdup2.h` & `protobuf-5.27.0rc1/upb/reflection/internal/strdup2.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/reflection/internal/upb_edition_defaults.h` & `protobuf-5.27.0rc1/upb/reflection/internal/upb_edition_defaults.h`

 * *Files 8% similar despite different names*

```diff
@@ -9,12 +9,12 @@
 #define UPB_REFLECTION_UPB_EDITION_DEFAULTS_H_
 
 // This file contains the serialized FeatureSetDefaults object for
 // language-independent features and (possibly at some point) for upb-specific
 // features. This is used for feature resolution under Editions.
 // NOLINTBEGIN
 // clang-format off
-#define UPB_INTERNAL_UPB_EDITION_DEFAULTS "\n\021\022\014\010\001\020\002\030\002 \003(\0010\002\030\346\007\n\021\022\014\010\002\020\001\030\001 \002(\0010\001\030\347\007\n\021\022\014\010\001\020\001\030\001 \002(\0010\001\030\350\007 \346\007(\350\007"
+#define UPB_INTERNAL_UPB_EDITION_DEFAULTS "\n\023\030\346\007\"\000*\014\010\001\020\002\030\002 \003(\0010\002\n\023\030\347\007\"\000*\014\010\002\020\001\030\001 \002(\0010\001\n\023\030\350\007\"\014\010\001\020\001\030\001 \002(\0010\001*\000 \346\007(\350\007"
 // clang-format on
 // NOLINTEND
 
 #endif  // UPB_REFLECTION_UPB_EDITION_DEFAULTS_H_
```

### Comparing `protobuf-5.26.1/upb/reflection/message.c` & `protobuf-5.27.0rc1/upb/reflection/message.c`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 #include "upb/message/internal/extension.h"
 #include "upb/message/internal/message.h"
 #include "upb/message/map.h"
 #include "upb/message/message.h"
 #include "upb/mini_table/extension.h"
 #include "upb/mini_table/field.h"
 #include "upb/mini_table/internal/field.h"
+#include "upb/mini_table/internal/message.h"
+#include "upb/mini_table/message.h"
 #include "upb/reflection/def.h"
 #include "upb/reflection/def_pool.h"
 #include "upb/reflection/message_def.h"
 #include "upb/reflection/oneof_def.h"
 
 // Must be last.
 #include "upb/port/def.inc"
@@ -97,15 +99,23 @@
   upb_Message_SetFieldByDef(msg, f, val, a);
 
   return ret;
 }
 
 bool upb_Message_SetFieldByDef(upb_Message* msg, const upb_FieldDef* f,
                                upb_MessageValue val, upb_Arena* a) {
-  return upb_Message_SetField(msg, upb_FieldDef_MiniTable(f), val, a);
+  const upb_MiniTableField* m_f = upb_FieldDef_MiniTable(f);
+
+  if (upb_MiniTableField_IsExtension(m_f)) {
+    return upb_Message_SetExtension(msg, (const upb_MiniTableExtension*)m_f,
+                                    &val, a);
+  } else {
+    upb_Message_SetBaseField(msg, m_f, &val);
+    return true;
+  }
 }
 
 void upb_Message_ClearFieldByDef(upb_Message* msg, const upb_FieldDef* f) {
   const upb_MiniTableField* m_f = upb_FieldDef_MiniTable(f);
 
   if (upb_MiniTableField_IsExtension(m_f)) {
     upb_Message_ClearExtension(msg, (const upb_MiniTableExtension*)m_f);
@@ -117,27 +127,28 @@
 void upb_Message_ClearByDef(upb_Message* msg, const upb_MessageDef* m) {
   upb_Message_Clear(msg, upb_MessageDef_MiniTable(m));
 }
 
 bool upb_Message_Next(const upb_Message* msg, const upb_MessageDef* m,
                       const upb_DefPool* ext_pool, const upb_FieldDef** out_f,
                       upb_MessageValue* out_val, size_t* iter) {
+  const upb_MiniTable* mt = upb_MessageDef_MiniTable(m);
   size_t i = *iter;
-  size_t n = upb_MessageDef_FieldCount(m);
+  size_t n = upb_MiniTable_FieldCount(mt);
+  const upb_MessageValue zero = {0};
   UPB_UNUSED(ext_pool);
 
   // Iterate over normal fields, returning the first one that is set.
   while (++i < n) {
-    const upb_FieldDef* f = upb_MessageDef_Field(m, i);
-    const upb_MiniTableField* field = upb_FieldDef_MiniTable(f);
-    upb_MessageValue val = upb_Message_GetFieldByDef(msg, f);
+    const upb_MiniTableField* field = upb_MiniTable_GetFieldByIndex(mt, i);
+    upb_MessageValue val = upb_Message_GetField(msg, field, zero);
 
     // Skip field if unset or empty.
     if (upb_MiniTableField_HasPresence(field)) {
-      if (!upb_Message_HasFieldByDef(msg, f)) continue;
+      if (!upb_Message_HasBaseField(msg, field)) continue;
     } else {
       switch (UPB_PRIVATE(_upb_MiniTableField_Mode)(field)) {
         case kUpb_FieldMode_Map:
           if (!val.map_val || upb_Map_Size(val.map_val) == 0) continue;
           break;
         case kUpb_FieldMode_Array:
           if (!val.array_val || upb_Array_Size(val.array_val) == 0) continue;
@@ -146,15 +157,16 @@
           if (UPB_PRIVATE(_upb_MiniTableField_DataIsZero)(field, &val))
             continue;
           break;
       }
     }
 
     *out_val = val;
-    *out_f = f;
+    *out_f =
+        upb_MessageDef_FindFieldByNumber(m, upb_MiniTableField_Number(field));
     *iter = i;
     return true;
   }
 
   if (ext_pool) {
     // Return any extensions that are set.
     size_t count;
```

### Comparing `protobuf-5.26.1/upb/reflection/message_def.c` & `protobuf-5.27.0rc1/upb/reflection/message_def.c`

 * *Files 1% similar despite different names*

```diff
@@ -411,46 +411,51 @@
   }
 
   const upb_value field_v = _upb_DefType_Pack(f, UPB_DEFTYPE_FIELD);
   bool ok =
       _upb_MessageDef_Insert(m, shortname, shortnamelen, field_v, ctx->arena);
   if (!ok) _upb_DefBuilder_OomErr(ctx);
 
-  if (strcmp(shortname, json_name) != 0 &&
+  bool skip_json_conflicts =
+      UPB_DESC(MessageOptions_deprecated_legacy_json_field_conflicts)(
+          upb_MessageDef_Options(m));
+  if (!skip_json_conflicts && strcmp(shortname, json_name) != 0 &&
       UPB_DESC(FeatureSet_json_format)(m->resolved_features) ==
           UPB_DESC(FeatureSet_ALLOW) &&
       upb_strtable_lookup(&m->ntof, json_name, &v)) {
     _upb_DefBuilder_Errf(
         ctx, "duplicate json_name for (%s) with original field name (%s)",
         shortname, json_name);
   }
 
   if (upb_strtable_lookup(&m->jtof, json_name, &v)) {
-    _upb_DefBuilder_Errf(ctx, "duplicate json_name (%s)", json_name);
+    if (!skip_json_conflicts) {
+      _upb_DefBuilder_Errf(ctx, "duplicate json_name (%s)", json_name);
+    }
+  } else {
+    const size_t json_size = strlen(json_name);
+    ok = upb_strtable_insert(&m->jtof, json_name, json_size,
+                             upb_value_constptr(f), ctx->arena);
+    if (!ok) _upb_DefBuilder_OomErr(ctx);
   }
 
-  const size_t json_size = strlen(json_name);
-  ok = upb_strtable_insert(&m->jtof, json_name, json_size,
-                           upb_value_constptr(f), ctx->arena);
-  if (!ok) _upb_DefBuilder_OomErr(ctx);
-
   if (upb_inttable_lookup(&m->itof, field_number, NULL)) {
     _upb_DefBuilder_Errf(ctx, "duplicate field number (%u)", field_number);
   }
 
   ok = upb_inttable_insert(&m->itof, field_number, v, ctx->arena);
   if (!ok) _upb_DefBuilder_OomErr(ctx);
 }
 
 void _upb_MessageDef_CreateMiniTable(upb_DefBuilder* ctx, upb_MessageDef* m) {
   if (ctx->layout == NULL) {
     m->layout = _upb_MessageDef_MakeMiniTable(ctx, m);
   } else {
     m->layout = upb_MiniTableFile_Message(ctx->layout, ctx->msg_count++);
-    UPB_ASSERT(m->field_count == m->layout->UPB_PRIVATE(field_count));
+    UPB_ASSERT(m->field_count == upb_MiniTable_FieldCount(m->layout));
 
     // We don't need the result of this call, but it will assign layout_index
     // for all the fields in O(n lg n) time.
     _upb_FieldDefs_Sorted(m->fields, m->field_count, ctx->tmp_arena);
   }
 
   for (int i = 0; i < m->nested_msg_count; i++) {
@@ -500,15 +505,15 @@
     }
   }
 
 #ifndef NDEBUG
   for (int i = 0; i < m->field_count; i++) {
     const upb_FieldDef* f = upb_MessageDef_Field(m, i);
     const int layout_index = _upb_FieldDef_LayoutIndex(f);
-    UPB_ASSERT(layout_index < m->layout->UPB_PRIVATE(field_count));
+    UPB_ASSERT(layout_index < upb_MiniTable_FieldCount(m->layout));
     const upb_MiniTableField* mt_f =
         &m->layout->UPB_PRIVATE(fields)[layout_index];
     UPB_ASSERT(upb_FieldDef_Type(f) == upb_MiniTableField_Type(mt_f));
     UPB_ASSERT(upb_FieldDef_CType(f) == upb_MiniTableField_CType(mt_f));
     UPB_ASSERT(upb_FieldDef_HasPresence(f) ==
                upb_MiniTableField_HasPresence(mt_f));
   }
```

### Comparing `protobuf-5.26.1/upb/reflection/message_def.h` & `protobuf-5.27.0rc1/upb/reflection/message_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/reflection/message_reserved_range.c` & `protobuf-5.27.0rc1/upb/reflection/message_reserved_range.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/reflection/message_reserved_range.h` & `protobuf-5.27.0rc1/upb/reflection/message_reserved_range.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/reflection/method_def.c` & `protobuf-5.27.0rc1/upb/reflection/method_def.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/reflection/method_def.h` & `protobuf-5.27.0rc1/upb/reflection/method_def.h`

 * *Files 6% similar despite different names*

```diff
@@ -15,26 +15,27 @@
 // Must be last.
 #include "upb/port/def.inc"
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
-bool upb_MethodDef_ClientStreaming(const upb_MethodDef* m);
+UPB_API bool upb_MethodDef_ClientStreaming(const upb_MethodDef* m);
 const char* upb_MethodDef_FullName(const upb_MethodDef* m);
 bool upb_MethodDef_HasOptions(const upb_MethodDef* m);
 int upb_MethodDef_Index(const upb_MethodDef* m);
-const upb_MessageDef* upb_MethodDef_InputType(const upb_MethodDef* m);
-const char* upb_MethodDef_Name(const upb_MethodDef* m);
-const UPB_DESC(MethodOptions) * upb_MethodDef_Options(const upb_MethodDef* m);
+UPB_API const upb_MessageDef* upb_MethodDef_InputType(const upb_MethodDef* m);
+UPB_API const char* upb_MethodDef_Name(const upb_MethodDef* m);
+UPB_API const UPB_DESC(MethodOptions) *
+    upb_MethodDef_Options(const upb_MethodDef* m);
 const UPB_DESC(FeatureSet) *
     upb_MethodDef_ResolvedFeatures(const upb_MethodDef* m);
-const upb_MessageDef* upb_MethodDef_OutputType(const upb_MethodDef* m);
-bool upb_MethodDef_ServerStreaming(const upb_MethodDef* m);
-const upb_ServiceDef* upb_MethodDef_Service(const upb_MethodDef* m);
+UPB_API const upb_MessageDef* upb_MethodDef_OutputType(const upb_MethodDef* m);
+UPB_API bool upb_MethodDef_ServerStreaming(const upb_MethodDef* m);
+UPB_API const upb_ServiceDef* upb_MethodDef_Service(const upb_MethodDef* m);
 
 #ifdef __cplusplus
 } /* extern "C" */
 #endif
 
 #include "upb/port/undef.inc"
```

### Comparing `protobuf-5.26.1/upb/reflection/oneof_def.c` & `protobuf-5.27.0rc1/upb/reflection/oneof_def.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/reflection/oneof_def.h` & `protobuf-5.27.0rc1/upb/reflection/oneof_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/reflection/service_def.c` & `protobuf-5.27.0rc1/upb/reflection/service_def.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/reflection/service_def.h` & `protobuf-5.27.0rc1/upb/reflection/service_def.h`

 * *Files 13% similar despite different names*

```diff
@@ -15,24 +15,25 @@
 // Must be last.
 #include "upb/port/def.inc"
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
-const upb_FileDef* upb_ServiceDef_File(const upb_ServiceDef* s);
+UPB_API const upb_FileDef* upb_ServiceDef_File(const upb_ServiceDef* s);
 const upb_MethodDef* upb_ServiceDef_FindMethodByName(const upb_ServiceDef* s,
                                                      const char* name);
-const char* upb_ServiceDef_FullName(const upb_ServiceDef* s);
+UPB_API const char* upb_ServiceDef_FullName(const upb_ServiceDef* s);
 bool upb_ServiceDef_HasOptions(const upb_ServiceDef* s);
 int upb_ServiceDef_Index(const upb_ServiceDef* s);
-const upb_MethodDef* upb_ServiceDef_Method(const upb_ServiceDef* s, int i);
-int upb_ServiceDef_MethodCount(const upb_ServiceDef* s);
+UPB_API const upb_MethodDef* upb_ServiceDef_Method(const upb_ServiceDef* s,
+                                                   int i);
+UPB_API int upb_ServiceDef_MethodCount(const upb_ServiceDef* s);
 const char* upb_ServiceDef_Name(const upb_ServiceDef* s);
-const UPB_DESC(ServiceOptions) *
+UPB_API const UPB_DESC(ServiceOptions) *
     upb_ServiceDef_Options(const upb_ServiceDef* s);
 const UPB_DESC(FeatureSet) *
     upb_ServiceDef_ResolvedFeatures(const upb_ServiceDef* s);
 
 #ifdef __cplusplus
 } /* extern "C" */
 #endif
```

### Comparing `protobuf-5.26.1/upb/text/encode.c` & `protobuf-5.27.0rc1/upb/text/encode.c`

 * *Files 4% similar despite different names*

```diff
@@ -226,20 +226,27 @@
   }
   txtenc_putstr(e, "\"");
 }
 
 static void txtenc_field(txtenc* e, upb_MessageValue val,
                          const upb_FieldDef* f) {
   txtenc_indent(e);
-  const upb_CType type = upb_FieldDef_CType(f);
+  const upb_CType ctype = upb_FieldDef_CType(f);
   const bool is_ext = upb_FieldDef_IsExtension(f);
   const char* full = upb_FieldDef_FullName(f);
   const char* name = upb_FieldDef_Name(f);
 
-  if (type == kUpb_CType_Message) {
+  if (ctype == kUpb_CType_Message) {
+// begin:google_only
+//     // TODO: Turn this into a feature check and opensource it.
+//     if (_upb_FieldDef_IsGroupLike(f)) {
+//       const upb_MessageDef* m = upb_FieldDef_MessageSubDef(f);
+//       name = upb_MessageDef_Name(m);
+//     }
+// end:google_only
     if (is_ext) {
       txtenc_printf(e, "[%s] {", full);
     } else {
       txtenc_printf(e, "%s {", name);
     }
     txtenc_endfield(e);
     e->indent_depth++;
@@ -253,15 +260,15 @@
 
   if (is_ext) {
     txtenc_printf(e, "[%s]: ", full);
   } else {
     txtenc_printf(e, "%s: ", name);
   }
 
-  switch (type) {
+  switch (ctype) {
     case kUpb_CType_Bool:
       txtenc_putstr(e, val.bool_val ? "true" : "false");
       break;
     case kUpb_CType_Float: {
       char buf[32];
       _upb_EncodeRoundTripFloat(val.float_val, buf, sizeof(buf));
       txtenc_putstr(e, buf);
```

### Comparing `protobuf-5.26.1/upb/text/encode.h` & `protobuf-5.27.0rc1/upb/text/encode.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/util/compare.c` & `protobuf-5.27.0rc1/upb/message/internal/compare_unknown.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 // Protocol Buffers - Google's data interchange format
 // Copyright 2023 Google LLC.  All rights reserved.
 //
 // Use of this source code is governed by a BSD-style
 // license that can be found in the LICENSE file or at
 // https://developers.google.com/open-source/licenses/bsd
 
-#include "upb/util/compare.h"
+#include "upb/message/internal/compare_unknown.h"
 
 #include <stdlib.h>
 
 #include "upb/base/string_view.h"
 #include "upb/mem/alloc.h"
 #include "upb/wire/eps_copy_input_stream.h"
 #include "upb/wire/reader.h"
 #include "upb/wire/types.h"
+
 // Must be last.
 #include "upb/port/def.inc"
 
-struct upb_UnknownFields;
 typedef struct upb_UnknownFields upb_UnknownFields;
 
 typedef struct {
   uint32_t tag;
   union {
     uint64_t varint;
     uint64_t uint64;
@@ -264,19 +264,17 @@
   }
 
   upb_Arena_Free(ctx->arena);
   upb_gfree(ctx->tmp);
   return ret;
 }
 
-upb_UnknownCompareResult upb_Message_UnknownFieldsAreEqual(const char* buf1,
-                                                           size_t size1,
-                                                           const char* buf2,
-                                                           size_t size2,
-                                                           int max_depth) {
+upb_UnknownCompareResult UPB_PRIVATE(_upb_Message_UnknownFieldsAreEqual)(
+    const char* buf1, size_t size1, const char* buf2, size_t size2,
+    int max_depth) {
   if (size1 == 0 && size2 == 0) return kUpb_UnknownCompareResult_Equal;
   if (size1 == 0 || size2 == 0) return kUpb_UnknownCompareResult_NotEqual;
   if (memcmp(buf1, buf2, size1) == 0) return kUpb_UnknownCompareResult_Equal;
 
   upb_UnknownField_Context ctx = {
       .arena = upb_Arena_New(),
       .depth = max_depth,
```

### Comparing `protobuf-5.26.1/upb/util/compare.h` & `protobuf-5.27.0rc1/upb/message/internal/compare_unknown.h`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 // Protocol Buffers - Google's data interchange format
 // Copyright 2023 Google LLC.  All rights reserved.
 //
 // Use of this source code is governed by a BSD-style
 // license that can be found in the LICENSE file or at
 // https://developers.google.com/open-source/licenses/bsd
 
-#ifndef UPB_UTIL_COMPARE_H_
-#define UPB_UTIL_COMPARE_H_
+#ifndef UPB_MESSAGE_INTERNAL_COMPARE_UNKNOWN_H_
+#define UPB_MESSAGE_INTERNAL_COMPARE_UNKNOWN_H_
 
 #include <stddef.h>
 
+// Must be last.
+#include "upb/port/def.inc"
+
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 // Returns true if unknown fields from the two messages are equal when sorted
 // and varints are made canonical.
 //
@@ -29,18 +32,18 @@
 typedef enum {
   kUpb_UnknownCompareResult_Equal = 0,
   kUpb_UnknownCompareResult_NotEqual = 1,
   kUpb_UnknownCompareResult_OutOfMemory = 2,
   kUpb_UnknownCompareResult_MaxDepthExceeded = 3,
 } upb_UnknownCompareResult;
 
-upb_UnknownCompareResult upb_Message_UnknownFieldsAreEqual(const char* buf1,
-                                                           size_t size1,
-                                                           const char* buf2,
-                                                           size_t size2,
-                                                           int max_depth);
+upb_UnknownCompareResult UPB_PRIVATE(_upb_Message_UnknownFieldsAreEqual)(
+    const char* buf1, size_t size1, const char* buf2, size_t size2,
+    int max_depth);
 
 #ifdef __cplusplus
 } /* extern "C" */
 #endif
 
-#endif /* UPB_UTIL_COMPARE_H_ */
+#include "upb/port/undef.inc"
+
+#endif /* UPB_MESSAGE_INTERNAL_COMPARE_UNKNOWN_H_ */
```

### Comparing `protobuf-5.26.1/upb/util/def_to_proto.c` & `protobuf-5.27.0rc1/upb/util/def_to_proto.c`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,18 @@
 // https://developers.google.com/open-source/licenses/bsd
 
 #include "upb/util/def_to_proto.h"
 
 #include <inttypes.h>
 #include <math.h>
 
+#include "google/protobuf/descriptor.upb.h"
+#include "upb/base/descriptor_constants.h"
 #include "upb/port/vsnprintf_compat.h"
+#include "upb/reflection/def.h"
 #include "upb/reflection/enum_reserved_range.h"
 #include "upb/reflection/extension_range.h"
 #include "upb/reflection/internal/field_def.h"
 #include "upb/reflection/internal/file_def.h"
 #include "upb/reflection/message.h"
 #include "upb/reflection/message_reserved_range.h"
 
@@ -214,16 +217,28 @@
   google_protobuf_FieldDescriptorProto* proto =
       google_protobuf_FieldDescriptorProto_new(ctx->arena);
   CHK_OOM(proto);
 
   google_protobuf_FieldDescriptorProto_set_name(proto,
                                        strviewdup(ctx, upb_FieldDef_Name(f)));
   google_protobuf_FieldDescriptorProto_set_number(proto, upb_FieldDef_Number(f));
-  google_protobuf_FieldDescriptorProto_set_label(proto, upb_FieldDef_Label(f));
-  google_protobuf_FieldDescriptorProto_set_type(proto, upb_FieldDef_Type(f));
+
+  if (upb_FieldDef_IsRequired(f) &&
+      upb_FileDef_Edition(upb_FieldDef_File(f)) >= UPB_DESC(EDITION_2023)) {
+    google_protobuf_FieldDescriptorProto_set_label(
+        proto, UPB_DESC(FieldDescriptorProto_LABEL_OPTIONAL));
+  } else {
+    google_protobuf_FieldDescriptorProto_set_label(proto, upb_FieldDef_Label(f));
+  }
+  if (upb_FieldDef_Type(f) == kUpb_FieldType_Group &&
+      upb_FileDef_Edition(upb_FieldDef_File(f)) >= UPB_DESC(EDITION_2023)) {
+    google_protobuf_FieldDescriptorProto_set_type(proto, kUpb_FieldType_Message);
+  } else {
+    google_protobuf_FieldDescriptorProto_set_type(proto, upb_FieldDef_Type(f));
+  }
 
   if (upb_FieldDef_HasJsonName(f)) {
     google_protobuf_FieldDescriptorProto_set_json_name(
         proto, strviewdup(ctx, upb_FieldDef_JsonName(f)));
   }
 
   if (upb_FieldDef_IsSubMessage(f)) {
```

### Comparing `protobuf-5.26.1/upb/util/def_to_proto.h` & `protobuf-5.27.0rc1/upb/util/def_to_proto.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/util/required_fields.c` & `protobuf-5.27.0rc1/upb/util/required_fields.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/util/required_fields.h` & `protobuf-5.27.0rc1/upb/util/required_fields.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/wire/decode.c` & `protobuf-5.27.0rc1/upb/wire/decode.c`

 * *Files 2% similar despite different names*

```diff
@@ -148,45 +148,44 @@
 } _upb_DecodeLongVarintReturn;
 
 UPB_NOINLINE
 static _upb_DecodeLongVarintReturn _upb_Decoder_DecodeLongVarint(
     const char* ptr, uint64_t val) {
   _upb_DecodeLongVarintReturn ret = {NULL, 0};
   uint64_t byte;
-  int i;
-  for (i = 1; i < 10; i++) {
+  for (int i = 1; i < 10; i++) {
     byte = (uint8_t)ptr[i];
     val += (byte - 1) << (i * 7);
     if (!(byte & 0x80)) {
       ret.ptr = ptr + i + 1;
       ret.val = val;
       return ret;
     }
   }
   return ret;
 }
 
 UPB_FORCEINLINE
-static const char* _upb_Decoder_DecodeVarint(upb_Decoder* d, const char* ptr,
-                                             uint64_t* val) {
+const char* _upb_Decoder_DecodeVarint(upb_Decoder* d, const char* ptr,
+                                      uint64_t* val) {
   uint64_t byte = (uint8_t)*ptr;
   if (UPB_LIKELY((byte & 0x80) == 0)) {
     *val = byte;
     return ptr + 1;
   } else {
     _upb_DecodeLongVarintReturn res = _upb_Decoder_DecodeLongVarint(ptr, byte);
     if (!res.ptr) _upb_Decoder_ErrorJmp(d, kUpb_DecodeStatus_Malformed);
     *val = res.val;
     return res.ptr;
   }
 }
 
 UPB_FORCEINLINE
-static const char* _upb_Decoder_DecodeTag(upb_Decoder* d, const char* ptr,
-                                          uint32_t* val) {
+const char* _upb_Decoder_DecodeTag(upb_Decoder* d, const char* ptr,
+                                   uint32_t* val) {
   uint64_t byte = (uint8_t)*ptr;
   if (UPB_LIKELY((byte & 0x80) == 0)) {
     *val = byte;
     return ptr + 1;
   } else {
     const char* start = ptr;
     _upb_DecodeLongVarintReturn res = _upb_Decoder_DecodeLongVarint(ptr, byte);
@@ -195,16 +194,16 @@
     }
     *val = res.val;
     return res.ptr;
   }
 }
 
 UPB_FORCEINLINE
-static const char* upb_Decoder_DecodeSize(upb_Decoder* d, const char* ptr,
-                                          uint32_t* size) {
+const char* upb_Decoder_DecodeSize(upb_Decoder* d, const char* ptr,
+                                   uint32_t* size) {
   uint64_t size64;
   ptr = _upb_Decoder_DecodeVarint(d, ptr, &size64);
   if (size64 >= INT32_MAX ||
       !upb_EpsCopyInputStream_CheckSize(&d->input, ptr, (int)size64)) {
     _upb_Decoder_ErrorJmp(d, kUpb_DecodeStatus_Malformed);
   }
   *size = size64;
@@ -298,66 +297,67 @@
   if (!ptr) _upb_Decoder_ErrorJmp(d, kUpb_DecodeStatus_OutOfMemory);
   str->data = str_ptr;
   str->size = size;
   return ptr;
 }
 
 UPB_FORCEINLINE
-static const char* _upb_Decoder_RecurseSubMessage(upb_Decoder* d,
-                                                  const char* ptr,
-                                                  upb_Message* submsg,
-                                                  const upb_MiniTable* subl,
-                                                  uint32_t expected_end_group) {
+const char* _upb_Decoder_RecurseSubMessage(upb_Decoder* d, const char* ptr,
+                                           upb_Message* submsg,
+                                           const upb_MiniTable* subl,
+                                           uint32_t expected_end_group) {
   if (--d->depth < 0) {
     _upb_Decoder_ErrorJmp(d, kUpb_DecodeStatus_MaxDepthExceeded);
   }
   ptr = _upb_Decoder_DecodeMessage(d, ptr, submsg, subl);
   d->depth++;
   if (d->end_group != expected_end_group) {
     _upb_Decoder_ErrorJmp(d, kUpb_DecodeStatus_Malformed);
   }
   return ptr;
 }
 
 UPB_FORCEINLINE
-static const char* _upb_Decoder_DecodeSubMessage(
-    upb_Decoder* d, const char* ptr, upb_Message* submsg,
-    const upb_MiniTableSub* subs, const upb_MiniTableField* field, int size) {
+const char* _upb_Decoder_DecodeSubMessage(upb_Decoder* d, const char* ptr,
+                                          upb_Message* submsg,
+                                          const upb_MiniTableSub* subs,
+                                          const upb_MiniTableField* field,
+                                          int size) {
   int saved_delta = upb_EpsCopyInputStream_PushLimit(&d->input, ptr, size);
   const upb_MiniTable* subl = _upb_MiniTableSubs_MessageByField(subs, field);
   UPB_ASSERT(subl);
   ptr = _upb_Decoder_RecurseSubMessage(d, ptr, submsg, subl, DECODE_NOGROUP);
   upb_EpsCopyInputStream_PopLimit(&d->input, ptr, saved_delta);
   return ptr;
 }
 
 UPB_FORCEINLINE
-static const char* _upb_Decoder_DecodeGroup(upb_Decoder* d, const char* ptr,
-                                            upb_Message* submsg,
-                                            const upb_MiniTable* subl,
-                                            uint32_t number) {
+const char* _upb_Decoder_DecodeGroup(upb_Decoder* d, const char* ptr,
+                                     upb_Message* submsg,
+                                     const upb_MiniTable* subl,
+                                     uint32_t number) {
   if (_upb_Decoder_IsDone(d, &ptr)) {
     _upb_Decoder_ErrorJmp(d, kUpb_DecodeStatus_Malformed);
   }
   ptr = _upb_Decoder_RecurseSubMessage(d, ptr, submsg, subl, number);
   d->end_group = DECODE_NOGROUP;
   return ptr;
 }
 
 UPB_FORCEINLINE
-static const char* _upb_Decoder_DecodeUnknownGroup(upb_Decoder* d,
-                                                   const char* ptr,
-                                                   uint32_t number) {
+const char* _upb_Decoder_DecodeUnknownGroup(upb_Decoder* d, const char* ptr,
+                                            uint32_t number) {
   return _upb_Decoder_DecodeGroup(d, ptr, NULL, NULL, number);
 }
 
 UPB_FORCEINLINE
-static const char* _upb_Decoder_DecodeKnownGroup(
-    upb_Decoder* d, const char* ptr, upb_Message* submsg,
-    const upb_MiniTableSub* subs, const upb_MiniTableField* field) {
+const char* _upb_Decoder_DecodeKnownGroup(upb_Decoder* d, const char* ptr,
+                                          upb_Message* submsg,
+                                          const upb_MiniTableSub* subs,
+                                          const upb_MiniTableField* field) {
   const upb_MiniTable* subl = _upb_MiniTableSubs_MessageByField(subs, field);
   UPB_ASSERT(subl);
   return _upb_Decoder_DecodeGroup(d, ptr, submsg, subl,
                                   field->UPB_PRIVATE(number));
 }
 
 static char* upb_Decoder_EncodeVarint32(uint32_t val, char* ptr) {
@@ -379,18 +379,17 @@
 
   if (!UPB_PRIVATE(_upb_Message_AddUnknown)(msg, buf, end - buf, &d->arena)) {
     _upb_Decoder_ErrorJmp(d, kUpb_DecodeStatus_OutOfMemory);
   }
 }
 
 UPB_FORCEINLINE
-static bool _upb_Decoder_CheckEnum(upb_Decoder* d, const char* ptr,
-                                   upb_Message* msg, const upb_MiniTableEnum* e,
-                                   const upb_MiniTableField* field,
-                                   wireval* val) {
+bool _upb_Decoder_CheckEnum(upb_Decoder* d, const char* ptr, upb_Message* msg,
+                            const upb_MiniTableEnum* e,
+                            const upb_MiniTableField* field, wireval* val) {
   const uint32_t v = val->uint32_val;
 
   if (UPB_LIKELY(upb_MiniTableEnum_CheckValue(e, v))) return true;
 
   // Unrecognized enum goes into unknown fields.
   // For packed fields the tag could be arbitrarily far in the past,
   // so we just re-encode the tag and value here.
@@ -416,17 +415,18 @@
                          arr->UPB_PRIVATE(size) * 4, void);
   arr->UPB_PRIVATE(size)++;
   memcpy(mem, val, 4);
   return ptr;
 }
 
 UPB_FORCEINLINE
-static const char* _upb_Decoder_DecodeFixedPacked(
-    upb_Decoder* d, const char* ptr, upb_Array* arr, wireval* val,
-    const upb_MiniTableField* field, int lg2) {
+const char* _upb_Decoder_DecodeFixedPacked(upb_Decoder* d, const char* ptr,
+                                           upb_Array* arr, wireval* val,
+                                           const upb_MiniTableField* field,
+                                           int lg2) {
   int mask = (1 << lg2) - 1;
   size_t count = val->size >> lg2;
   if ((val->size & mask) != 0) {
     // Length isn't a round multiple of elem size.
     _upb_Decoder_ErrorJmp(d, kUpb_DecodeStatus_Malformed);
   }
   _upb_Decoder_Reserve(d, arr, count);
@@ -453,17 +453,18 @@
     upb_EpsCopyInputStream_PopLimit(&d->input, ptr, delta);
   }
 
   return ptr;
 }
 
 UPB_FORCEINLINE
-static const char* _upb_Decoder_DecodeVarintPacked(
-    upb_Decoder* d, const char* ptr, upb_Array* arr, wireval* val,
-    const upb_MiniTableField* field, int lg2) {
+const char* _upb_Decoder_DecodeVarintPacked(upb_Decoder* d, const char* ptr,
+                                            upb_Array* arr, wireval* val,
+                                            const upb_MiniTableField* field,
+                                            int lg2) {
   int scale = 1 << lg2;
   int saved_limit = upb_EpsCopyInputStream_PushLimit(&d->input, ptr, val->size);
   char* out = UPB_PTR_AT(upb_Array_MutableDataPtr(arr),
                          arr->UPB_PRIVATE(size) << lg2, void);
   while (!_upb_Decoder_IsDone(d, &ptr)) {
     wireval elem;
     ptr = _upb_Decoder_DecodeVarint(d, ptr, &elem.uint64_val);
@@ -698,15 +699,15 @@
                               field, val)) {
     return ptr;
   }
 
   // Set presence if necessary.
   if (UPB_PRIVATE(_upb_MiniTableField_HasHasbit)(field)) {
     UPB_PRIVATE(_upb_Message_SetHasbit)(msg, field);
-  } else if (UPB_PRIVATE(_upb_MiniTableField_IsInOneof)(field)) {
+  } else if (upb_MiniTableField_IsInOneof(field)) {
     // Oneof case
     uint32_t* oneof_case = UPB_PRIVATE(_upb_Message_OneofCasePtr)(msg, field);
     if (op == kUpb_DecodeOp_SubMessage &&
         *oneof_case != field->UPB_PRIVATE(number)) {
       memset(mem, 0, sizeof(void*));
     }
     *oneof_case = field->UPB_PRIVATE(number);
@@ -761,17 +762,16 @@
     d->missing_required =
         !UPB_PRIVATE(_upb_Message_IsInitializedShallow)(msg, m);
   }
   return ptr;
 }
 
 UPB_FORCEINLINE
-static bool _upb_Decoder_TryFastDispatch(upb_Decoder* d, const char** ptr,
-                                         upb_Message* msg,
-                                         const upb_MiniTable* m) {
+bool _upb_Decoder_TryFastDispatch(upb_Decoder* d, const char** ptr,
+                                  upb_Message* msg, const upb_MiniTable* m) {
 #if UPB_FASTTABLE
   if (m && m->UPB_PRIVATE(table_mask) != (unsigned char)-1) {
     uint16_t tag = _upb_FastDecoder_LoadTag(*ptr);
     intptr_t table = decode_totable(m);
     *ptr = _upb_FastDecoder_TagDispatch(d, *ptr, msg, table, 0, tag);
     return true;
   }
@@ -1001,17 +1001,16 @@
       [kUpb_FakeFieldType_MessageSetItem] = kUpb_DecodeOp_UnknownField,
   };
 
   return kVarintOps[field->UPB_PRIVATE(descriptortype)];
 }
 
 UPB_FORCEINLINE
-static void _upb_Decoder_CheckUnlinked(upb_Decoder* d, const upb_MiniTable* mt,
-                                       const upb_MiniTableField* field,
-                                       int* op) {
+void _upb_Decoder_CheckUnlinked(upb_Decoder* d, const upb_MiniTable* mt,
+                                const upb_MiniTableField* field, int* op) {
   // If sub-message is not linked, treat as unknown.
   if (field->UPB_PRIVATE(mode) & kUpb_LabelFlags_IsExtension) return;
   const upb_MiniTable* mt_sub =
       _upb_MiniTableSubs_MessageByField(mt->UPB_PRIVATE(subs), field);
   if ((d->options & kUpb_DecodeOption_ExperimentalAllowUnlinked) ||
       !UPB_PRIVATE(_upb_MiniTable_IsEmpty)(mt_sub)) {
     return;
@@ -1029,17 +1028,16 @@
     } while (upb_MiniTable_NextOneofField(mt, &oneof));
   }
 #endif  // NDEBUG
   *op = kUpb_DecodeOp_UnknownField;
 }
 
 UPB_FORCEINLINE
-static void _upb_Decoder_MaybeVerifyUtf8(upb_Decoder* d,
-                                         const upb_MiniTableField* field,
-                                         int* op) {
+void _upb_Decoder_MaybeVerifyUtf8(upb_Decoder* d,
+                                  const upb_MiniTableField* field, int* op) {
   if ((field->UPB_ONLYBITS(mode) & kUpb_LabelFlags_IsAlternate) &&
       UPB_UNLIKELY(d->options & kUpb_DecodeOption_AlwaysValidateUtf8))
     *op = kUpb_DecodeOp_String;
 }
 
 static int _upb_Decoder_GetDelimitedOp(upb_Decoder* d, const upb_MiniTable* mt,
                                        const upb_MiniTableField* field) {
@@ -1101,19 +1099,18 @@
     _upb_Decoder_MaybeVerifyUtf8(d, field, &op);
   }
 
   return op;
 }
 
 UPB_FORCEINLINE
-static const char* _upb_Decoder_DecodeWireValue(upb_Decoder* d, const char* ptr,
-                                                const upb_MiniTable* mt,
-                                                const upb_MiniTableField* field,
-                                                int wire_type, wireval* val,
-                                                int* op) {
+const char* _upb_Decoder_DecodeWireValue(upb_Decoder* d, const char* ptr,
+                                         const upb_MiniTable* mt,
+                                         const upb_MiniTableField* field,
+                                         int wire_type, wireval* val, int* op) {
   static const unsigned kFixed32OkMask = (1 << kUpb_FieldType_Float) |
                                          (1 << kUpb_FieldType_Fixed32) |
                                          (1 << kUpb_FieldType_SFixed32);
 
   static const unsigned kFixed64OkMask = (1 << kUpb_FieldType_Double) |
                                          (1 << kUpb_FieldType_Fixed64) |
                                          (1 << kUpb_FieldType_SFixed64);
@@ -1155,18 +1152,19 @@
     default:
       break;
   }
   _upb_Decoder_ErrorJmp(d, kUpb_DecodeStatus_Malformed);
 }
 
 UPB_FORCEINLINE
-static const char* _upb_Decoder_DecodeKnownField(
-    upb_Decoder* d, const char* ptr, upb_Message* msg,
-    const upb_MiniTable* layout, const upb_MiniTableField* field, int op,
-    wireval* val) {
+const char* _upb_Decoder_DecodeKnownField(upb_Decoder* d, const char* ptr,
+                                          upb_Message* msg,
+                                          const upb_MiniTable* layout,
+                                          const upb_MiniTableField* field,
+                                          int op, wireval* val) {
   const upb_MiniTableSub* subs = layout->UPB_PRIVATE(subs);
   uint8_t mode = field->UPB_PRIVATE(mode);
 
   if (UPB_UNLIKELY(mode & kUpb_LabelFlags_IsExtension)) {
     const upb_MiniTableExtension* ext_layout =
         (const upb_MiniTableExtension*)field;
     upb_Extension* ext = UPB_PRIVATE(_upb_Message_GetOrCreateExtension)(
@@ -1364,17 +1362,18 @@
 
   UPB_PRIVATE(_upb_Arena_SwapOut)(arena, &decoder->arena);
 
   return decoder->status;
 }
 
 upb_DecodeStatus upb_Decode(const char* buf, size_t size, upb_Message* msg,
-                            const upb_MiniTable* m,
+                            const upb_MiniTable* mt,
                             const upb_ExtensionRegistry* extreg, int options,
                             upb_Arena* arena) {
+  UPB_ASSERT(!upb_Message_IsFrozen(msg));
   upb_Decoder decoder;
   unsigned depth = (unsigned)options >> 16;
 
   upb_EpsCopyInputStream_Init(&decoder.input, &buf, size,
                               options & kUpb_DecodeOption_AliasString);
 
   decoder.extreg = extreg;
@@ -1388,12 +1387,47 @@
   // Violating the encapsulation of the arena for performance reasons.
   // This is a temporary arena that we swap into and swap out of when we are
   // done.  The temporary arena only needs to be able to handle allocation,
   // not fuse or free, so it does not need many of the members to be initialized
   // (particularly parent_or_count).
   UPB_PRIVATE(_upb_Arena_SwapIn)(&decoder.arena, arena);
 
-  return upb_Decoder_Decode(&decoder, buf, msg, m, arena);
+  return upb_Decoder_Decode(&decoder, buf, msg, mt, arena);
+}
+
+upb_DecodeStatus upb_DecodeLengthPrefixed(const char* buf, size_t size,
+                                          upb_Message* msg,
+                                          size_t* num_bytes_read,
+                                          const upb_MiniTable* mt,
+                                          const upb_ExtensionRegistry* extreg,
+                                          int options, upb_Arena* arena) {
+  // To avoid needing to make a Decoder just to decode the initial length,
+  // hand-decode the leading varint for the message length here.
+  uint64_t msg_len = 0;
+  for (size_t i = 0;; ++i) {
+    if (i >= size || i > 9) {
+      return kUpb_DecodeStatus_Malformed;
+    }
+    uint64_t b = *buf;
+    buf++;
+    msg_len += (b & 0x7f) << (i * 7);
+    if ((b & 0x80) == 0) {
+      *num_bytes_read = i + 1 + msg_len;
+      break;
+    }
+  }
+
+  // If the total number of bytes we would read (= the bytes from the varint
+  // plus however many bytes that varint says we should read) is larger then the
+  // input buffer then error as malformed.
+  if (*num_bytes_read > size) {
+    return kUpb_DecodeStatus_Malformed;
+  }
+  if (msg_len > INT32_MAX) {
+    return kUpb_DecodeStatus_Malformed;
+  }
+
+  return upb_Decode(buf, msg_len, msg, mt, extreg, options, arena);
 }
 
 #undef OP_FIXPCK_LG2
 #undef OP_VARPCK_LG2
```

### Comparing `protobuf-5.26.1/upb/wire/decode.h` & `protobuf-5.27.0rc1/upb/wire/decode.h`

 * *Files 4% similar despite different names*

```diff
@@ -106,14 +106,15 @@
 // Enforce an upper bound on recursion depth.
 UPB_INLINE int upb_Decode_LimitDepth(uint32_t decode_options, uint32_t limit) {
   uint32_t max_depth = upb_DecodeOptions_GetMaxDepth(decode_options);
   if (max_depth > limit) max_depth = limit;
   return upb_DecodeOptions_MaxDepth(max_depth) | (decode_options & 0xffff);
 }
 
+// LINT.IfChange
 typedef enum {
   kUpb_DecodeStatus_Ok = 0,
   kUpb_DecodeStatus_Malformed = 1,    // Wire format was corrupt
   kUpb_DecodeStatus_OutOfMemory = 2,  // Arena alloc failed
   kUpb_DecodeStatus_BadUtf8 = 3,      // String field had bad UTF-8
   kUpb_DecodeStatus_MaxDepthExceeded =
       4,  // Exceeded upb_DecodeOptions_MaxDepth
@@ -123,20 +124,29 @@
   kUpb_DecodeStatus_MissingRequired = 5,
 
   // Unlinked sub-message field was present, but
   // kUpb_DecodeOptions_ExperimentalAllowUnlinked was not specified in the list
   // of options.
   kUpb_DecodeStatus_UnlinkedSubMessage = 6,
 } upb_DecodeStatus;
+// LINT.ThenChange(//depot/google3/third_party/protobuf/rust/upb.rs:decode_status)
 
 UPB_API upb_DecodeStatus upb_Decode(const char* buf, size_t size,
-                                    upb_Message* msg, const upb_MiniTable* l,
+                                    upb_Message* msg, const upb_MiniTable* mt,
                                     const upb_ExtensionRegistry* extreg,
                                     int options, upb_Arena* arena);
 
+// Same as upb_Decode but with a varint-encoded length prepended.
+// On success 'num_bytes_read' will be set to the how many bytes were read,
+// on failure the contents of num_bytes_read is undefined.
+UPB_API upb_DecodeStatus upb_DecodeLengthPrefixed(
+    const char* buf, size_t size, upb_Message* msg, size_t* num_bytes_read,
+    const upb_MiniTable* mt, const upb_ExtensionRegistry* extreg, int options,
+    upb_Arena* arena);
+
 #ifdef __cplusplus
 } /* extern "C" */
 #endif
 
 #include "upb/port/undef.inc"
 
 #endif /* UPB_WIRE_DECODE_H_ */
```

### Comparing `protobuf-5.26.1/upb/wire/encode.c` & `protobuf-5.27.0rc1/upb/wire/encode.c`

 * *Files 6% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 
   e->ptr -= bytes;
 }
 
 /* Call to ensure that at least "bytes" bytes are available for writing at
  * e->ptr.  Returns false if the bytes could not be allocated. */
 UPB_FORCEINLINE
-static void encode_reserve(upb_encstate* e, size_t bytes) {
+void encode_reserve(upb_encstate* e, size_t bytes) {
   if ((size_t)(e->ptr - e->buf) < bytes) {
     encode_growbuffer(e, bytes);
     return;
   }
 
   e->ptr -= bytes;
 }
@@ -148,15 +148,15 @@
   len = encode_varint64(val, e->ptr);
   start = e->ptr + UPB_PB_VARINT_MAX_LEN - len;
   memmove(start, e->ptr, len);
   e->ptr = start;
 }
 
 UPB_FORCEINLINE
-static void encode_varint(upb_encstate* e, uint64_t val) {
+void encode_varint(upb_encstate* e, uint64_t val) {
   if (val < 128 && e->ptr != e->buf) {
     --e->ptr;
     *e->ptr = val;
   } else {
     encode_longvarint(e, val);
   }
 }
@@ -178,15 +178,15 @@
 static void encode_tag(upb_encstate* e, uint32_t field_number,
                        uint8_t wire_type) {
   encode_varint(e, (field_number << 3) | wire_type);
 }
 
 static void encode_fixedarray(upb_encstate* e, const upb_Array* arr,
                               size_t elem_size, uint32_t tag) {
-  size_t bytes = arr->UPB_PRIVATE(size) * elem_size;
+  size_t bytes = upb_Array_Size(arr) * elem_size;
   const char* data = upb_Array_DataPtr(arr);
   const char* ptr = data + bytes - elem_size;
 
   if (tag || !upb_IsLittleEndian()) {
     while (true) {
       if (elem_size == 4) {
         uint32_t val;
@@ -275,15 +275,15 @@
       upb_TaggedMessagePtr submsg = *(upb_TaggedMessagePtr*)field_mem;
       const upb_MiniTable* subm =
           upb_MiniTableSub_Message(subs[f->UPB_PRIVATE(submsg_index)]);
       if (submsg == 0) {
         return;
       }
       if (--e->depth == 0) encode_err(e, kUpb_EncodeStatus_MaxDepthExceeded);
-      encode_tag(e, f->UPB_PRIVATE(number), kUpb_WireType_EndGroup);
+      encode_tag(e, upb_MiniTableField_Number(f), kUpb_WireType_EndGroup);
       encode_TaggedMessagePtr(e, submsg, subm, &size);
       wire_type = kUpb_WireType_StartGroup;
       e->depth++;
       break;
     }
     case kUpb_FieldType_Message: {
       size_t size;
@@ -301,32 +301,32 @@
       break;
     }
     default:
       UPB_UNREACHABLE();
   }
 #undef CASE
 
-  encode_tag(e, f->UPB_PRIVATE(number), wire_type);
+  encode_tag(e, upb_MiniTableField_Number(f), wire_type);
 }
 
 static void encode_array(upb_encstate* e, const upb_Message* msg,
                          const upb_MiniTableSub* subs,
                          const upb_MiniTableField* f) {
   const upb_Array* arr = *UPB_PTR_AT(msg, f->UPB_PRIVATE(offset), upb_Array*);
   bool packed = upb_MiniTableField_IsPacked(f);
   size_t pre_len = e->limit - e->ptr;
 
-  if (arr == NULL || arr->UPB_PRIVATE(size) == 0) {
+  if (arr == NULL || upb_Array_Size(arr) == 0) {
     return;
   }
 
 #define VARINT_CASE(ctype, encode)                                         \
   {                                                                        \
     const ctype* start = upb_Array_DataPtr(arr);                           \
-    const ctype* ptr = start + arr->UPB_PRIVATE(size);                     \
+    const ctype* ptr = start + upb_Array_Size(arr);                        \
     uint32_t tag =                                                         \
         packed ? 0 : (f->UPB_PRIVATE(number) << 3) | kUpb_WireType_Varint; \
     do {                                                                   \
       ptr--;                                                               \
       encode_varint(e, encode);                                            \
       if (tag) encode_varint(e, tag);                                      \
     } while (ptr != start);                                                \
@@ -363,69 +363,69 @@
     case kUpb_FieldType_SInt32:
       VARINT_CASE(int32_t, encode_zz32(*ptr));
     case kUpb_FieldType_SInt64:
       VARINT_CASE(int64_t, encode_zz64(*ptr));
     case kUpb_FieldType_String:
     case kUpb_FieldType_Bytes: {
       const upb_StringView* start = upb_Array_DataPtr(arr);
-      const upb_StringView* ptr = start + arr->UPB_PRIVATE(size);
+      const upb_StringView* ptr = start + upb_Array_Size(arr);
       do {
         ptr--;
         encode_bytes(e, ptr->data, ptr->size);
         encode_varint(e, ptr->size);
-        encode_tag(e, f->UPB_PRIVATE(number), kUpb_WireType_Delimited);
+        encode_tag(e, upb_MiniTableField_Number(f), kUpb_WireType_Delimited);
       } while (ptr != start);
       return;
     }
     case kUpb_FieldType_Group: {
       const upb_TaggedMessagePtr* start = upb_Array_DataPtr(arr);
-      const upb_TaggedMessagePtr* ptr = start + arr->UPB_PRIVATE(size);
+      const upb_TaggedMessagePtr* ptr = start + upb_Array_Size(arr);
       const upb_MiniTable* subm =
           upb_MiniTableSub_Message(subs[f->UPB_PRIVATE(submsg_index)]);
       if (--e->depth == 0) encode_err(e, kUpb_EncodeStatus_MaxDepthExceeded);
       do {
         size_t size;
         ptr--;
-        encode_tag(e, f->UPB_PRIVATE(number), kUpb_WireType_EndGroup);
+        encode_tag(e, upb_MiniTableField_Number(f), kUpb_WireType_EndGroup);
         encode_TaggedMessagePtr(e, *ptr, subm, &size);
-        encode_tag(e, f->UPB_PRIVATE(number), kUpb_WireType_StartGroup);
+        encode_tag(e, upb_MiniTableField_Number(f), kUpb_WireType_StartGroup);
       } while (ptr != start);
       e->depth++;
       return;
     }
     case kUpb_FieldType_Message: {
       const upb_TaggedMessagePtr* start = upb_Array_DataPtr(arr);
-      const upb_TaggedMessagePtr* ptr = start + arr->UPB_PRIVATE(size);
+      const upb_TaggedMessagePtr* ptr = start + upb_Array_Size(arr);
       const upb_MiniTable* subm =
           upb_MiniTableSub_Message(subs[f->UPB_PRIVATE(submsg_index)]);
       if (--e->depth == 0) encode_err(e, kUpb_EncodeStatus_MaxDepthExceeded);
       do {
         size_t size;
         ptr--;
         encode_TaggedMessagePtr(e, *ptr, subm, &size);
         encode_varint(e, size);
-        encode_tag(e, f->UPB_PRIVATE(number), kUpb_WireType_Delimited);
+        encode_tag(e, upb_MiniTableField_Number(f), kUpb_WireType_Delimited);
       } while (ptr != start);
       e->depth++;
       return;
     }
   }
 #undef VARINT_CASE
 
   if (packed) {
     encode_varint(e, e->limit - e->ptr - pre_len);
-    encode_tag(e, f->UPB_PRIVATE(number), kUpb_WireType_Delimited);
+    encode_tag(e, upb_MiniTableField_Number(f), kUpb_WireType_Delimited);
   }
 }
 
 static void encode_mapentry(upb_encstate* e, uint32_t number,
                             const upb_MiniTable* layout,
                             const upb_MapEntry* ent) {
-  const upb_MiniTableField* key_field = &layout->UPB_PRIVATE(fields)[0];
-  const upb_MiniTableField* val_field = &layout->UPB_PRIVATE(fields)[1];
+  const upb_MiniTableField* key_field = upb_MiniTable_MapKey(layout);
+  const upb_MiniTableField* val_field = upb_MiniTable_MapValue(layout);
   size_t pre_len = e->limit - e->ptr;
   size_t size;
   encode_scalar(e, &ent->v, layout->UPB_PRIVATE(subs), val_field);
   encode_scalar(e, &ent->k, layout->UPB_PRIVATE(subs), key_field);
   size = (e->limit - e->ptr) - pre_len;
   encode_varint(e, size);
   encode_tag(e, number, kUpb_WireType_Delimited);
@@ -433,37 +433,37 @@
 
 static void encode_map(upb_encstate* e, const upb_Message* msg,
                        const upb_MiniTableSub* subs,
                        const upb_MiniTableField* f) {
   const upb_Map* map = *UPB_PTR_AT(msg, f->UPB_PRIVATE(offset), const upb_Map*);
   const upb_MiniTable* layout =
       upb_MiniTableSub_Message(subs[f->UPB_PRIVATE(submsg_index)]);
-  UPB_ASSERT(layout->UPB_PRIVATE(field_count) == 2);
+  UPB_ASSERT(upb_MiniTable_FieldCount(layout) == 2);
 
   if (!map || !upb_Map_Size(map)) return;
 
   if (e->options & kUpb_EncodeOption_Deterministic) {
     _upb_sortedmap sorted;
     _upb_mapsorter_pushmap(
         &e->sorter, layout->UPB_PRIVATE(fields)[0].UPB_PRIVATE(descriptortype),
         map, &sorted);
     upb_MapEntry ent;
     while (_upb_sortedmap_next(&e->sorter, map, &sorted, &ent)) {
-      encode_mapentry(e, f->UPB_PRIVATE(number), layout, &ent);
+      encode_mapentry(e, upb_MiniTableField_Number(f), layout, &ent);
     }
     _upb_mapsorter_popmap(&e->sorter, &sorted);
   } else {
     intptr_t iter = UPB_STRTABLE_BEGIN;
     upb_StringView key;
     upb_value val;
     while (upb_strtable_next2(&map->table, &key, &val, &iter)) {
       upb_MapEntry ent;
       _upb_map_fromkey(key, &ent.k, map->key_size);
       _upb_map_fromvalue(val, &ent.v, map->val_size);
-      encode_mapentry(e, f->UPB_PRIVATE(number), layout, &ent);
+      encode_mapentry(e, upb_MiniTableField_Number(f), layout, &ent);
     }
   }
 }
 
 static bool encode_shouldencode(upb_encstate* e, const upb_Message* msg,
                                 const upb_MiniTableSub* subs,
                                 const upb_MiniTableField* f) {
@@ -495,15 +495,15 @@
     }
   } else if (UPB_PRIVATE(_upb_MiniTableField_HasHasbit)(f)) {
     // Proto2 presence: hasbit.
     return UPB_PRIVATE(_upb_Message_GetHasbit)(msg, f);
   } else {
     // Field is in a oneof.
     return UPB_PRIVATE(_upb_Message_GetOneofCase)(msg, f) ==
-           f->UPB_PRIVATE(number);
+           upb_MiniTableField_Number(f);
   }
 }
 
 static void encode_field(upb_encstate* e, const upb_Message* msg,
                          const upb_MiniTableSub* subs,
                          const upb_MiniTableField* field) {
   switch (UPB_PRIVATE(_upb_MiniTableField_Mode)(field)) {
@@ -521,15 +521,15 @@
       UPB_UNREACHABLE();
   }
 }
 
 static void encode_msgset_item(upb_encstate* e, const upb_Extension* ext) {
   size_t size;
   encode_tag(e, kUpb_MsgSet_Item, kUpb_WireType_EndGroup);
-  encode_message(e, ext->data.ptr,
+  encode_message(e, ext->data.msg_val,
                  upb_MiniTableExtension_GetSubMessage(ext->ext), &size);
   encode_varint(e, size);
   encode_tag(e, kUpb_MsgSet_Message, kUpb_WireType_Delimited);
   encode_varint(e, upb_MiniTableExtension_Number(ext->ext));
   encode_tag(e, kUpb_MsgSet_TypeId, kUpb_WireType_Varint);
   encode_tag(e, kUpb_MsgSet_Item, kUpb_WireType_StartGroup);
 }
@@ -585,15 +585,15 @@
         for (; ext != end; ext++) {
           encode_ext(e, ext, m->UPB_PRIVATE(ext) == kUpb_ExtMode_IsMessageSet);
         }
       }
     }
   }
 
-  if (m->UPB_PRIVATE(field_count)) {
+  if (upb_MiniTable_FieldCount(m)) {
     const upb_MiniTableField* f =
         &m->UPB_PRIVATE(fields)[m->UPB_PRIVATE(field_count)];
     const upb_MiniTableField* first = &m->UPB_PRIVATE(fields)[0];
     while (f != first) {
       f--;
       if (encode_shouldencode(e, msg, m->UPB_PRIVATE(subs), f)) {
         encode_field(e, msg, m->UPB_PRIVATE(subs), f);
@@ -603,22 +603,26 @@
 
   *size = (e->limit - e->ptr) - pre_len;
 }
 
 static upb_EncodeStatus upb_Encoder_Encode(upb_encstate* const encoder,
                                            const upb_Message* const msg,
                                            const upb_MiniTable* const l,
-                                           char** const buf,
-                                           size_t* const size) {
+                                           char** const buf, size_t* const size,
+                                           bool prepend_len) {
   // Unfortunately we must continue to perform hackery here because there are
   // code paths which blindly copy the returned pointer without bothering to
   // check for errors until much later (b/235839510). So we still set *buf to
   // NULL on error and we still set it to non-NULL on a successful empty result.
   if (UPB_SETJMP(encoder->err) == 0) {
-    encode_message(encoder, msg, l, size);
+    size_t encoded_msg_size;
+    encode_message(encoder, msg, l, &encoded_msg_size);
+    if (prepend_len) {
+      encode_varint(encoder, encoded_msg_size);
+    }
     *size = encoder->limit - encoder->ptr;
     if (*size == 0) {
       static char ch;
       *buf = &ch;
     } else {
       UPB_ASSERT(encoder->ptr);
       *buf = encoder->ptr;
@@ -629,24 +633,38 @@
     *size = 0;
   }
 
   _upb_mapsorter_destroy(&encoder->sorter);
   return encoder->status;
 }
 
-upb_EncodeStatus upb_Encode(const upb_Message* msg, const upb_MiniTable* l,
-                            int options, upb_Arena* arena, char** buf,
-                            size_t* size) {
+static upb_EncodeStatus _upb_Encode(const upb_Message* msg,
+                                    const upb_MiniTable* l, int options,
+                                    upb_Arena* arena, char** buf, size_t* size,
+                                    bool prepend_len) {
   upb_encstate e;
   unsigned depth = (unsigned)options >> 16;
 
   e.status = kUpb_EncodeStatus_Ok;
   e.arena = arena;
   e.buf = NULL;
   e.limit = NULL;
   e.ptr = NULL;
   e.depth = depth ? depth : kUpb_WireFormat_DefaultDepthLimit;
   e.options = options;
   _upb_mapsorter_init(&e.sorter);
 
-  return upb_Encoder_Encode(&e, msg, l, buf, size);
+  return upb_Encoder_Encode(&e, msg, l, buf, size, prepend_len);
+}
+
+upb_EncodeStatus upb_Encode(const upb_Message* msg, const upb_MiniTable* l,
+                            int options, upb_Arena* arena, char** buf,
+                            size_t* size) {
+  return _upb_Encode(msg, l, options, arena, buf, size, false);
+}
+
+upb_EncodeStatus upb_EncodeLengthPrefixed(const upb_Message* msg,
+                                          const upb_MiniTable* l, int options,
+                                          upb_Arena* arena, char** buf,
+                                          size_t* size) {
+  return _upb_Encode(msg, l, options, arena, buf, size, true);
 }
```

### Comparing `protobuf-5.26.1/upb/wire/encode.h` & `protobuf-5.27.0rc1/upb/wire/encode.h`

 * *Files 8% similar despite different names*

```diff
@@ -29,29 +29,31 @@
    * instances of this binary. There are no guarantees across different
    * binary builds.
    *
    * If your proto contains maps, the encoder will need to malloc()/free()
    * memory during encode. */
   kUpb_EncodeOption_Deterministic = 1,
 
-  // When set, unknown fields are not printed.
+  // When set, unknown fields are not encoded.
   kUpb_EncodeOption_SkipUnknown = 2,
 
   // When set, the encode will fail if any required fields are missing.
   kUpb_EncodeOption_CheckRequired = 4,
 };
 
+// LINT.IfChange
 typedef enum {
   kUpb_EncodeStatus_Ok = 0,
   kUpb_EncodeStatus_OutOfMemory = 1,  // Arena alloc failed
   kUpb_EncodeStatus_MaxDepthExceeded = 2,
 
   // kUpb_EncodeOption_CheckRequired failed but the parse otherwise succeeded.
   kUpb_EncodeStatus_MissingRequired = 3,
 } upb_EncodeStatus;
+// LINT.ThenChange(//depot/google3/third_party/protobuf/rust/upb.rs:encode_status)
 
 UPB_INLINE uint32_t upb_EncodeOptions_MaxDepth(uint16_t depth) {
   return (uint32_t)depth << 16;
 }
 
 UPB_INLINE uint16_t upb_EncodeOptions_GetMaxDepth(uint32_t options) {
   return options >> 16;
@@ -64,14 +66,20 @@
   return upb_EncodeOptions_MaxDepth(max_depth) | (encode_options & 0xffff);
 }
 
 UPB_API upb_EncodeStatus upb_Encode(const upb_Message* msg,
                                     const upb_MiniTable* l, int options,
                                     upb_Arena* arena, char** buf, size_t* size);
 
+// Encodes the message prepended by a varint of the serialized length.
+UPB_API upb_EncodeStatus upb_EncodeLengthPrefixed(const upb_Message* msg,
+                                                  const upb_MiniTable* l,
+                                                  int options, upb_Arena* arena,
+                                                  char** buf, size_t* size);
+
 #ifdef __cplusplus
 } /* extern "C" */
 #endif
 
 #include "upb/port/undef.inc"
 
 #endif /* UPB_WIRE_ENCODE_H_ */
```

### Comparing `protobuf-5.26.1/upb/wire/eps_copy_input_stream.c` & `protobuf-5.27.0rc1/upb/wire/eps_copy_input_stream.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/wire/eps_copy_input_stream.h` & `protobuf-5.27.0rc1/upb/wire/eps_copy_input_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -33,16 +33,16 @@
   kUpb_EpsCopyInputStream_NoDelta = 2
 };
 
 typedef struct {
   const char* end;        // Can read up to SlopBytes bytes beyond this.
   const char* limit_ptr;  // For bounds checks, = end + UPB_MIN(limit, 0)
   uintptr_t aliasing;
-  int limit;              // Submessage limit relative to end
-  bool error;             // To distinguish between EOF and error.
+  int limit;   // Submessage limit relative to end
+  bool error;  // To distinguish between EOF and error.
   char patch[kUpb_EpsCopyInputStream_SlopBytes * 2];
 } upb_EpsCopyInputStream;
 
 // Returns true if the stream is in the error state. A stream enters the error
 // state when the user reads past a limit (caught in IsDone()) or the
 // ZeroCopyInputStream returns an error.
 UPB_INLINE bool upb_EpsCopyInputStream_IsError(upb_EpsCopyInputStream* e) {
@@ -371,15 +371,15 @@
     upb_EpsCopyInputStream* e, const char* ptr, void* ctx);
 
 // Tries to perform a fast-path handling of the given delimited message data.
 // If the sub-message beginning at `*ptr` and extending for `len` is short and
 // fits within this buffer, calls `func` with `ctx` as a parameter, where the
 // pushing and popping of limits is handled automatically and with lower cost
 // than the normal PushLimit()/PopLimit() sequence.
-static UPB_FORCEINLINE bool upb_EpsCopyInputStream_TryParseDelimitedFast(
+UPB_FORCEINLINE bool upb_EpsCopyInputStream_TryParseDelimitedFast(
     upb_EpsCopyInputStream* e, const char** ptr, int len,
     upb_EpsCopyInputStream_ParseDelimitedFunc* func, void* ctx) {
   if (!upb_EpsCopyInputStream_CheckSubMessageSizeAvailable(e, *ptr, len)) {
     return false;
   }
 
   // Fast case: Sub-message is <128 bytes and fits in the current buffer.
```

### Comparing `protobuf-5.26.1/upb/wire/internal/constants.h` & `protobuf-5.27.0rc1/upb/wire/internal/constants.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/wire/internal/decode_fast.c` & `protobuf-5.27.0rc1/upb/wire/internal/decode_fast.c`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
   ptr = _upb_EpsCopyInputStream_IsDoneFallbackInline(
       &d->input, ptr, overrun, _upb_Decoder_BufferFlipCallback);
   data = _upb_FastDecoder_LoadTag(ptr);
   UPB_MUSTTAIL return _upb_FastDecoder_TagDispatch(UPB_PARSE_ARGS);
 }
 
 UPB_FORCEINLINE
-static const char* fastdecode_dispatch(UPB_PARSE_PARAMS) {
+const char* fastdecode_dispatch(UPB_PARSE_PARAMS) {
   int overrun;
   switch (upb_EpsCopyInputStream_IsDoneStatus(&d->input, ptr, &overrun)) {
     case kUpb_IsDoneStatus_Done:
       ((uint32_t*)msg)[2] |= hasbits;  // Sync hasbits.
       const upb_MiniTable* m = decode_totablep(table);
       return UPB_UNLIKELY(m->UPB_PRIVATE(required_count))
                  ? _upb_Decoder_CheckRequired(d, ptr, msg, m)
@@ -76,24 +76,24 @@
 
   // Read two bytes of tag data (for a one-byte tag, the high byte is junk).
   data = _upb_FastDecoder_LoadTag(ptr);
   UPB_MUSTTAIL return _upb_FastDecoder_TagDispatch(UPB_PARSE_ARGS);
 }
 
 UPB_FORCEINLINE
-static bool fastdecode_checktag(uint16_t data, int tagbytes) {
+bool fastdecode_checktag(uint16_t data, int tagbytes) {
   if (tagbytes == 1) {
     return (data & 0xff) == 0;
   } else {
     return data == 0;
   }
 }
 
 UPB_FORCEINLINE
-static const char* fastdecode_longsize(const char* ptr, int* size) {
+const char* fastdecode_longsize(const char* ptr, int* size) {
   int i;
   UPB_ASSERT(*size & 0x80);
   *size &= 0xff;
   for (i = 0; i < 3; i++) {
     ptr++;
     size_t byte = (uint8_t)ptr[-1];
     *size += (byte - 1) << (7 + 7 * i);
@@ -105,15 +105,15 @@
   // for a 32 bit varint.
   if (UPB_UNLIKELY(byte >= 8)) return NULL;
   *size += (byte - 1) << 28;
   return ptr;
 }
 
 UPB_FORCEINLINE
-static const char* fastdecode_delimited(
+const char* fastdecode_delimited(
     upb_Decoder* d, const char* ptr,
     upb_EpsCopyInputStream_ParseDelimitedFunc* func, void* ctx) {
   ptr++;
 
   // Sign-extend so varint greater than one byte becomes negative, causing
   // fast delimited parse to fail.
   int len = (int8_t)ptr[-1];
@@ -158,16 +158,16 @@
 typedef struct {
   void* dst;
   fastdecode_next next;
   uint32_t tag;
 } fastdecode_nextret;
 
 UPB_FORCEINLINE
-static void* fastdecode_resizearr(upb_Decoder* d, void* dst,
-                                  fastdecode_arr* farr, int valbytes) {
+void* fastdecode_resizearr(upb_Decoder* d, void* dst, fastdecode_arr* farr,
+                           int valbytes) {
   if (UPB_UNLIKELY(dst == farr->end)) {
     size_t old_capacity = farr->arr->UPB_PRIVATE(capacity);
     size_t old_bytes = old_capacity * valbytes;
     size_t new_capacity = old_capacity * 2;
     size_t new_bytes = new_capacity * valbytes;
     char* old_ptr = upb_Array_MutableDataPtr(farr->arr);
     char* new_ptr = upb_Arena_Realloc(&d->arena, old_ptr, old_bytes, new_bytes);
@@ -177,36 +177,34 @@
     dst = (void*)(new_ptr + (old_capacity * valbytes));
     farr->end = (void*)(new_ptr + (new_capacity * valbytes));
   }
   return dst;
 }
 
 UPB_FORCEINLINE
-static bool fastdecode_tagmatch(uint32_t tag, uint64_t data, int tagbytes) {
+bool fastdecode_tagmatch(uint32_t tag, uint64_t data, int tagbytes) {
   if (tagbytes == 1) {
     return (uint8_t)tag == (uint8_t)data;
   } else {
     return (uint16_t)tag == (uint16_t)data;
   }
 }
 
 UPB_FORCEINLINE
-static void fastdecode_commitarr(void* dst, fastdecode_arr* farr,
-                                 int valbytes) {
+void fastdecode_commitarr(void* dst, fastdecode_arr* farr, int valbytes) {
   farr->arr->UPB_PRIVATE(size) =
       (size_t)((char*)dst - (char*)upb_Array_MutableDataPtr(farr->arr)) /
       valbytes;
 }
 
 UPB_FORCEINLINE
-static fastdecode_nextret fastdecode_nextrepeated(upb_Decoder* d, void* dst,
-                                                  const char** ptr,
-                                                  fastdecode_arr* farr,
-                                                  uint64_t data, int tagbytes,
-                                                  int valbytes) {
+fastdecode_nextret fastdecode_nextrepeated(upb_Decoder* d, void* dst,
+                                           const char** ptr,
+                                           fastdecode_arr* farr, uint64_t data,
+                                           int tagbytes, int valbytes) {
   fastdecode_nextret ret;
   dst = (char*)dst + valbytes;
 
   if (UPB_LIKELY(!_upb_Decoder_IsDone(d, ptr))) {
     ret.tag = _upb_FastDecoder_LoadTag(*ptr);
     if (fastdecode_tagmatch(ret.tag, data, tagbytes)) {
       ret.next = FD_NEXT_SAMEFIELD;
@@ -220,24 +218,23 @@
   }
 
   ret.dst = dst;
   return ret;
 }
 
 UPB_FORCEINLINE
-static void* fastdecode_fieldmem(upb_Message* msg, uint64_t data) {
+void* fastdecode_fieldmem(upb_Message* msg, uint64_t data) {
   size_t ofs = data >> 48;
   return (char*)msg + ofs;
 }
 
 UPB_FORCEINLINE
-static void* fastdecode_getfield(upb_Decoder* d, const char* ptr,
-                                 upb_Message* msg, uint64_t* data,
-                                 uint64_t* hasbits, fastdecode_arr* farr,
-                                 int valbytes, upb_card card) {
+void* fastdecode_getfield(upb_Decoder* d, const char* ptr, upb_Message* msg,
+                          uint64_t* data, uint64_t* hasbits,
+                          fastdecode_arr* farr, int valbytes, upb_card card) {
   switch (card) {
     case CARD_s: {
       uint8_t hasbit_index = *data >> 24;
       // Set hasbit and return pointer to scalar field.
       *hasbits |= 1ull << hasbit_index;
       return fastdecode_fieldmem(msg, *data);
     }
@@ -268,15 +265,15 @@
     }
     default:
       UPB_UNREACHABLE();
   }
 }
 
 UPB_FORCEINLINE
-static bool fastdecode_flippacked(uint64_t* data, int tagbytes) {
+bool fastdecode_flippacked(uint64_t* data, int tagbytes) {
   *data ^= (0x2 ^ 0x0);  // Patch data to match packed wiretype.
   return fastdecode_checktag(*data, tagbytes);
 }
 
 #define FASTDECODE_CHECKPACKED(tagbytes, card, func)                \
   if (UPB_UNLIKELY(!fastdecode_checktag(data, tagbytes))) {         \
     if (card == CARD_r && fastdecode_flippacked(&data, tagbytes)) { \
@@ -284,15 +281,15 @@
     }                                                               \
     RETURN_GENERIC("packed check tag mismatch\n");                  \
   }
 
 /* varint fields **************************************************************/
 
 UPB_FORCEINLINE
-static uint64_t fastdecode_munge(uint64_t val, int valbytes, bool zigzag) {
+uint64_t fastdecode_munge(uint64_t val, int valbytes, bool zigzag) {
   if (valbytes == 1) {
     return val != 0;
   } else if (zigzag) {
     if (valbytes == 4) {
       uint32_t n = val;
       return (n >> 1) ^ -(int32_t)(n & 1);
     } else if (valbytes == 8) {
@@ -300,15 +297,15 @@
     }
     UPB_UNREACHABLE();
   }
   return val;
 }
 
 UPB_FORCEINLINE
-static const char* fastdecode_varint64(const char* ptr, uint64_t* val) {
+const char* fastdecode_varint64(const char* ptr, uint64_t* val) {
   ptr++;
   *val = (uint8_t)ptr[-1];
   if (UPB_UNLIKELY(*val & 0x80)) {
     int i;
     for (i = 0; i < 8; i++) {
       ptr++;
       uint64_t byte = (uint8_t)ptr[-1];
@@ -375,16 +372,16 @@
   uint8_t valbytes;
   bool zigzag;
   void* dst;
   fastdecode_arr farr;
 } fastdecode_varintdata;
 
 UPB_FORCEINLINE
-static const char* fastdecode_topackedvarint(upb_EpsCopyInputStream* e,
-                                             const char* ptr, void* ctx) {
+const char* fastdecode_topackedvarint(upb_EpsCopyInputStream* e,
+                                      const char* ptr, void* ctx) {
   upb_Decoder* d = (upb_Decoder*)e;
   fastdecode_varintdata* data = ctx;
   void* dst = data->dst;
   uint64_t val;
 
   while (!_upb_Decoder_IsDone(d, &ptr)) {
     dst = fastdecode_resizearr(d, dst, &data->farr, data->valbytes);
@@ -655,17 +652,16 @@
     struct upb_Decoder* d, const char* ptr, upb_Message* msg, intptr_t table,
     uint64_t hasbits, uint64_t data) {
   upb_StringView* dst = (upb_StringView*)data;
   FASTDECODE_LONGSTRING(d, ptr, msg, table, hasbits, dst, false);
 }
 
 UPB_FORCEINLINE
-static void fastdecode_docopy(upb_Decoder* d, const char* ptr, uint32_t size,
-                              int copy, char* data, size_t data_offset,
-                              upb_StringView* dst) {
+void fastdecode_docopy(upb_Decoder* d, const char* ptr, uint32_t size, int copy,
+                       char* data, size_t data_offset, upb_StringView* dst) {
   d->arena.UPB_PRIVATE(ptr) += copy;
   dst->data = data + data_offset;
   UPB_UNPOISON_MEMORY_REGION(data, copy);
   memcpy(data, ptr, copy);
   UPB_POISON_MEMORY_REGION(data + data_offset + size,
                            copy - data_offset - size);
 }
@@ -888,16 +884,16 @@
 
 typedef struct {
   intptr_t table;
   upb_Message* msg;
 } fastdecode_submsgdata;
 
 UPB_FORCEINLINE
-static const char* fastdecode_tosubmsg(upb_EpsCopyInputStream* e,
-                                       const char* ptr, void* ctx) {
+const char* fastdecode_tosubmsg(upb_EpsCopyInputStream* e, const char* ptr,
+                                void* ctx) {
   upb_Decoder* d = (upb_Decoder*)e;
   fastdecode_submsgdata* submsg = ctx;
   ptr = fastdecode_dispatch(d, ptr, submsg->msg, submsg->table, 0, 0);
   UPB_ASSUME(ptr != NULL);
   return ptr;
 }
```

### Comparing `protobuf-5.26.1/upb/wire/internal/decode_fast.h` & `protobuf-5.27.0rc1/upb/wire/internal/decode_fast.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/wire/internal/decoder.h` & `protobuf-5.27.0rc1/upb/wire/internal/decoder.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/upb/wire/internal/reader.h` & `protobuf-5.27.0rc1/upb/wire/internal/reader.h`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 UPB_PRIVATE(_upb_WireReader_LongVarint)
 UPB_PRIVATE(_upb_WireReader_ReadLongVarint)(const char* ptr, uint64_t val);
 
-static UPB_FORCEINLINE const char* UPB_PRIVATE(_upb_WireReader_ReadVarint)(
+UPB_FORCEINLINE const char* UPB_PRIVATE(_upb_WireReader_ReadVarint)(
     const char* ptr, uint64_t* val, int maxlen, uint64_t maxval) {
   uint64_t byte = (uint8_t)*ptr;
   if (UPB_LIKELY((byte & 0x80) == 0)) {
     *val = (uint32_t)byte;
     return ptr + 1;
   }
   const char* start = ptr;
@@ -40,19 +40,19 @@
       res.val > maxval) {
     return NULL;  // Malformed.
   }
   *val = res.val;
   return res.ptr;
 }
 
-UPB_INLINE uint32_t UPB_PRIVATE(_upb_WireReader_GetFieldNumber)(uint32_t tag) {
+UPB_API_INLINE uint32_t upb_WireReader_GetFieldNumber(uint32_t tag) {
   return tag >> kUpb_WireReader_WireTypeBits;
 }
 
-UPB_INLINE uint8_t UPB_PRIVATE(_upb_WireReader_GetWireType)(uint32_t tag) {
+UPB_API_INLINE uint8_t upb_WireReader_GetWireType(uint32_t tag) {
   return tag & kUpb_WireReader_WireTypeMask;
 }
 
 #ifdef __cplusplus
 } /* extern "C" */
 #endif
```

### Comparing `protobuf-5.26.1/upb/wire/reader.c` & `protobuf-5.27.0rc1/upb/wire/reader.c`

 * *Files 7% similar despite different names*

```diff
@@ -16,16 +16,15 @@
 // Must be last.
 #include "upb/port/def.inc"
 
 UPB_NOINLINE UPB_PRIVATE(_upb_WireReader_LongVarint)
     UPB_PRIVATE(_upb_WireReader_ReadLongVarint)(const char* ptr, uint64_t val) {
   UPB_PRIVATE(_upb_WireReader_LongVarint) ret = {NULL, 0};
   uint64_t byte;
-  int i;
-  for (i = 1; i < 10; i++) {
+  for (int i = 1; i < 10; i++) {
     byte = (uint8_t)ptr[i];
     val += (byte - 1) << (i * 7);
     if (!(byte & 0x80)) {
       ret.ptr = ptr + i + 1;
       ret.val = val;
       return ret;
     }
```

### Comparing `protobuf-5.26.1/upb/wire/reader.h` & `protobuf-5.27.0rc1/upb/wire/reader.h`

 * *Files 3% similar despite different names*

```diff
@@ -28,32 +28,28 @@
 
 // Parses a tag into `tag`, and returns a pointer past the end of the tag, or
 // NULL if there was an error in the tag data.
 //
 // REQUIRES: there must be at least 10 bytes of data available at `ptr`.
 // Bounds checks must be performed before calling this function, preferably
 // by calling upb_EpsCopyInputStream_IsDone().
-static UPB_FORCEINLINE const char* upb_WireReader_ReadTag(const char* ptr,
-                                                          uint32_t* tag) {
+UPB_FORCEINLINE const char* upb_WireReader_ReadTag(const char* ptr,
+                                                   uint32_t* tag) {
   uint64_t val;
   ptr = UPB_PRIVATE(_upb_WireReader_ReadVarint)(ptr, &val, 5, UINT32_MAX);
   if (!ptr) return NULL;
   *tag = val;
   return ptr;
 }
 
 // Given a tag, returns the field number.
-UPB_INLINE uint32_t upb_WireReader_GetFieldNumber(uint32_t tag) {
-  return UPB_PRIVATE(_upb_WireReader_GetFieldNumber)(tag);
-}
+UPB_API_INLINE uint32_t upb_WireReader_GetFieldNumber(uint32_t tag);
 
 // Given a tag, returns the wire type.
-UPB_INLINE uint8_t upb_WireReader_GetWireType(uint32_t tag) {
-  return UPB_PRIVATE(_upb_WireReader_GetWireType)(tag);
-}
+UPB_API_INLINE uint8_t upb_WireReader_GetWireType(uint32_t tag);
 
 UPB_INLINE const char* upb_WireReader_ReadVarint(const char* ptr,
                                                  uint64_t* val) {
   return UPB_PRIVATE(_upb_WireReader_ReadVarint)(ptr, val, 10, UINT64_MAX);
 }
 
 // Skips data for a varint, returning a pointer past the end of the varint, or
```

### Comparing `protobuf-5.26.1/upb/wire/types.h` & `protobuf-5.27.0rc1/upb/wire/types.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/utf8_range/utf8_range.c` & `protobuf-5.27.0rc1/utf8_range/utf8_range.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.26.1/utf8_range/utf8_range.h` & `protobuf-5.27.0rc1/utf8_range/utf8_range.h`

 * *Files identical despite different names*

