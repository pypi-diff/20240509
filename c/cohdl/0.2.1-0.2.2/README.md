# Comparing `tmp/cohdl-0.2.1.tar.gz` & `tmp/cohdl-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cohdl-0.2.1.tar", last modified: Sun May  5 16:22:44 2024, max compression
+gzip compressed data, was "cohdl-0.2.2.tar", last modified: Wed May  8 22:34:00 2024, max compression
```

## Comparing `cohdl-0.2.1.tar` & `cohdl-0.2.2.tar`

### file list

```diff
@@ -1,122 +1,156 @@
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-05 16:22:44.994070 cohdl-0.2.1/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1074 2024-05-05 11:51:07.000000 cohdl-0.2.1/LICENSE
--rw-r--r--   0 alexander  (1000) alexander  (1000)     3008 2024-05-05 16:22:44.994070 cohdl-0.2.1/PKG-INFO
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     2607 2024-05-05 12:08:05.000000 cohdl-0.2.1/README.md
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-05 16:22:44.986070 cohdl-0.2.1/cohdl/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1206 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/__init__.py
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-05 16:22:44.986070 cohdl-0.2.1/cohdl/_compiler/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)        0 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/_compiler/__init__.py
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-05 16:22:44.986070 cohdl-0.2.1/cohdl/_compiler/backend/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)       40 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/_compiler/backend/__init__.py
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-05 16:22:44.986070 cohdl-0.2.1/cohdl/_compiler/backend/vhdl/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)        0 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/_compiler/backend/vhdl/__init__.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)    14953 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/_compiler/backend/vhdl/_vhdl_assembler.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)    59351 2024-05-05 16:15:58.000000 cohdl-0.2.1/cohdl/_compiler/backend/vhdl/_vhdl_repr.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      197 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/_compiler/backend/vhdl/backend.py
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-05 16:22:44.986070 cohdl-0.2.1/cohdl/_compiler/frontend/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      101 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/_compiler/frontend/__init__.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      333 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/_compiler/frontend/_frontend.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)    44654 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/_compiler/frontend/_generate_ir.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)    80755 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/_compiler/frontend/_prepare_ast.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)    24995 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/_compiler/frontend/_prepare_ast_out.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      674 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/_compiler/frontend/_traceback.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     9253 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/_compiler/frontend/_value_branch.py
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-05 16:22:44.990070 cohdl-0.2.1/cohdl/_core/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1196 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/_core/__init__.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     3211 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/_core/_array.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      479 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/_core/_array.pyi
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     5806 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/_core/_bit.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1738 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/_core/_bit.pyi
--rw-rw-r--   0 alexander  (1000) alexander  (1000)    14468 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/_core/_bit_vector.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     3172 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/_core/_bit_vector.pyi
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     2799 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/_core/_boolean.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      771 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/_core/_boolean.pyi
--rw-rw-r--   0 alexander  (1000) alexander  (1000)    18973 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/_core/_collect_ast_and_scope.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     8679 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/_core/_context.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     3033 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/_core/_enum.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      931 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/_core/_inline.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     5152 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/_core/_integer.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1583 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/_core/_integer.pyi
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     7949 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/_core/_intrinsic.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     2334 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/_core/_intrinsic.pyi
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     4678 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/_core/_intrinsic_definitions.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     2493 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/_core/_intrinsic_definitions.pyi
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     2977 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/_core/_intrinsic_operations.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      171 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/_core/_intrinsic_operations.pyi
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-05 16:22:44.990070 cohdl-0.2.1/cohdl/_core/_ir/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      202 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/_core/_ir/__init__.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)    52172 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/_core/_ir/_repr.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1990 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/_core/_primitive_type.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)    11170 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/_core/_signed.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1665 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/_core/_signed.pyi
--rw-rw-r--   0 alexander  (1000) alexander  (1000)    40575 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/_core/_type_qualifier.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)    15649 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/_core/_type_qualifier.pyi
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     9715 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/_core/_unsigned.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1946 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/_core/_unsigned.pyi
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-05 16:22:44.990070 cohdl-0.2.1/cohdl/std/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     2147 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/std/__init__.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1033 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/std/_assignable_type.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      740 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/std/_assignable_type.pyi
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      897 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/std/_compile.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)    30291 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/std/_context.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)    16092 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/std/_context.pyi
--rw-rw-r--   0 alexander  (1000) alexander  (1000)    19919 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/std/_core_utility.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)    17969 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/std/_core_utility.pyi
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1196 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/std/_crc.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)    27180 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/std/_fixed.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     3193 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/std/_fixed.pyi
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     8818 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/std/_formal.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     3694 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/std/_prefix.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     3101 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/std/_prefix.pyi
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     7107 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/std/_record.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1034 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/std/_record.pyi
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     6710 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/std/_template.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     2939 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/std/_template.pyi
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-05 16:22:44.990070 cohdl-0.2.1/cohdl/std/axi/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)       25 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/std/axi/__init__.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      669 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/std/axi/_axi4_channel.py
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-05 16:22:44.990070 cohdl-0.2.1/cohdl/std/axi/axi4_light/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)       64 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/std/axi/axi4_light/__init__.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)    12135 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/std/axi/axi4_light/base.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     5185 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/std/axi/axi4_light/interconnect.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     7718 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/std/bitfield.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1688 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/std/bitfield.pyi
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     5399 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/std/enum.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     3795 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/std/enum.pyi
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-05 16:22:44.990070 cohdl-0.2.1/cohdl/std/formal/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      114 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/std/formal/__init__.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     2201 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/std/formal/_builtins.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     3097 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/std/formal/_checker.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)       97 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/std/formal/_configure.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     4002 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/std/formal/_sequence.py
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-05 16:22:44.990070 cohdl-0.2.1/cohdl/std/reg/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)       76 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/std/reg/__init__.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)    54518 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/std/reg/reg.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)    27950 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/std/reg/reg.pyi
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     9567 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/std/reg/system_rdl.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     6900 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/std/spi.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     4019 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/std/spi.pyi
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     6484 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/std/uart.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     2928 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/std/uart.pyi
--rw-rw-r--   0 alexander  (1000) alexander  (1000)    38693 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/std/utility.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)    25351 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/std/utility.pyi
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-05 16:22:44.990070 cohdl-0.2.1/cohdl/utility/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      177 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/utility/__init__.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1614 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/utility/code_writer.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     2917 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/utility/id_map.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     4473 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/utility/make_target.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      529 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/utility/merge_dicts.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      735 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/utility/source_location.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     2168 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/utility/span.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     2988 2024-05-05 11:51:07.000000 cohdl-0.2.1/cohdl/utility/virtual_traceback.py
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-05 16:22:44.990070 cohdl-0.2.1/cohdl.egg-info/
--rw-r--r--   0 alexander  (1000) alexander  (1000)     3008 2024-05-05 16:22:44.000000 cohdl-0.2.1/cohdl.egg-info/PKG-INFO
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     2825 2024-05-05 16:22:44.000000 cohdl-0.2.1/cohdl.egg-info/SOURCES.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)        1 2024-05-05 16:22:44.000000 cohdl-0.2.1/cohdl.egg-info/dependency_links.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)       24 2024-05-05 16:22:44.000000 cohdl-0.2.1/cohdl.egg-info/top_level.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      512 2024-05-05 16:20:48.000000 cohdl-0.2.1/pyproject.toml
--rw-rw-r--   0 alexander  (1000) alexander  (1000)       38 2024-05-05 16:22:44.994070 cohdl-0.2.1/setup.cfg
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-05 16:22:44.990070 cohdl-0.2.1/tests/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     7003 2024-05-05 11:51:07.000000 cohdl-0.2.1/tests/test_bit.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     8187 2024-05-05 11:51:07.000000 cohdl-0.2.1/tests/test_bitvector.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1986 2024-05-05 11:51:07.000000 cohdl-0.2.1/tests/test_unsigned.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-08 22:34:00.276839 cohdl-0.2.2/
+-rw-r--r--   0 alexander  (1000) alexander  (1000)     1074 2023-05-21 19:26:34.000000 cohdl-0.2.2/LICENSE
+-rw-r--r--   0 alexander  (1000) alexander  (1000)     3216 2024-05-08 22:34:00.276839 cohdl-0.2.2/PKG-INFO
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     2815 2024-05-08 22:28:33.000000 cohdl-0.2.2/README.md
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-08 22:34:00.268839 cohdl-0.2.2/cohdl/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1206 2024-03-24 17:00:13.000000 cohdl-0.2.2/cohdl/__init__.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-08 22:34:00.268839 cohdl-0.2.2/cohdl/_compiler/
+-rw-r--r--   0 alexander  (1000) alexander  (1000)        0 2023-05-21 19:26:34.000000 cohdl-0.2.2/cohdl/_compiler/__init__.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-08 22:34:00.268839 cohdl-0.2.2/cohdl/_compiler/backend/
+-rw-r--r--   0 alexander  (1000) alexander  (1000)       40 2023-05-21 19:26:34.000000 cohdl-0.2.2/cohdl/_compiler/backend/__init__.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-08 22:34:00.268839 cohdl-0.2.2/cohdl/_compiler/backend/vhdl/
+-rw-r--r--   0 alexander  (1000) alexander  (1000)        0 2023-05-21 19:26:34.000000 cohdl-0.2.2/cohdl/_compiler/backend/vhdl/__init__.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    14953 2024-04-08 18:41:42.000000 cohdl-0.2.2/cohdl/_compiler/backend/vhdl/_vhdl_assembler.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    59351 2024-05-05 16:10:56.000000 cohdl-0.2.2/cohdl/_compiler/backend/vhdl/_vhdl_repr.py
+-rw-r--r--   0 alexander  (1000) alexander  (1000)      197 2023-05-21 19:26:34.000000 cohdl-0.2.2/cohdl/_compiler/backend/vhdl/backend.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-08 22:34:00.268839 cohdl-0.2.2/cohdl/_compiler/frontend/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      101 2024-03-24 17:00:13.000000 cohdl-0.2.2/cohdl/_compiler/frontend/__init__.py
+-rw-r--r--   0 alexander  (1000) alexander  (1000)      333 2023-11-18 15:34:23.000000 cohdl-0.2.2/cohdl/_compiler/frontend/_frontend.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    44654 2024-05-04 12:15:38.000000 cohdl-0.2.2/cohdl/_compiler/frontend/_generate_ir.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    80755 2024-05-04 12:15:38.000000 cohdl-0.2.2/cohdl/_compiler/frontend/_prepare_ast.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    24995 2024-05-04 12:15:38.000000 cohdl-0.2.2/cohdl/_compiler/frontend/_prepare_ast_out.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      674 2024-03-24 17:00:13.000000 cohdl-0.2.2/cohdl/_compiler/frontend/_traceback.py
+-rw-r--r--   0 alexander  (1000) alexander  (1000)     9253 2024-04-12 20:17:32.000000 cohdl-0.2.2/cohdl/_compiler/frontend/_value_branch.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-08 22:34:00.268839 cohdl-0.2.2/cohdl/_core/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1196 2024-03-24 17:00:13.000000 cohdl-0.2.2/cohdl/_core/__init__.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     3211 2024-03-29 22:43:58.000000 cohdl-0.2.2/cohdl/_core/_array.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      479 2024-02-18 21:56:15.000000 cohdl-0.2.2/cohdl/_core/_array.pyi
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     5806 2024-03-29 22:49:48.000000 cohdl-0.2.2/cohdl/_core/_bit.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1738 2023-07-21 19:56:14.000000 cohdl-0.2.2/cohdl/_core/_bit.pyi
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    14468 2024-04-10 20:33:46.000000 cohdl-0.2.2/cohdl/_core/_bit_vector.py
+-rw-r--r--   0 alexander  (1000) alexander  (1000)     3172 2024-04-10 20:02:30.000000 cohdl-0.2.2/cohdl/_core/_bit_vector.pyi
+-rw-r--r--   0 alexander  (1000) alexander  (1000)     2799 2024-03-29 22:50:50.000000 cohdl-0.2.2/cohdl/_core/_boolean.py
+-rw-r--r--   0 alexander  (1000) alexander  (1000)      771 2024-03-28 21:57:17.000000 cohdl-0.2.2/cohdl/_core/_boolean.pyi
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    18973 2024-04-13 11:19:42.000000 cohdl-0.2.2/cohdl/_core/_collect_ast_and_scope.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     8679 2024-03-29 22:51:41.000000 cohdl-0.2.2/cohdl/_core/_context.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     3033 2024-03-30 00:23:42.000000 cohdl-0.2.2/cohdl/_core/_enum.py
+-rw-r--r--   0 alexander  (1000) alexander  (1000)      931 2023-05-21 19:26:34.000000 cohdl-0.2.2/cohdl/_core/_inline.py
+-rw-r--r--   0 alexander  (1000) alexander  (1000)     5152 2024-03-29 22:37:28.000000 cohdl-0.2.2/cohdl/_core/_integer.py
+-rw-r--r--   0 alexander  (1000) alexander  (1000)     1583 2023-05-21 19:26:34.000000 cohdl-0.2.2/cohdl/_core/_integer.pyi
+-rw-r--r--   0 alexander  (1000) alexander  (1000)     7949 2024-03-30 00:01:25.000000 cohdl-0.2.2/cohdl/_core/_intrinsic.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     2334 2023-07-27 17:52:02.000000 cohdl-0.2.2/cohdl/_core/_intrinsic.pyi
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     4678 2024-04-14 12:32:44.000000 cohdl-0.2.2/cohdl/_core/_intrinsic_definitions.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     2493 2024-04-14 15:15:11.000000 cohdl-0.2.2/cohdl/_core/_intrinsic_definitions.pyi
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     2977 2024-04-10 19:56:49.000000 cohdl-0.2.2/cohdl/_core/_intrinsic_operations.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      171 2023-07-07 22:47:53.000000 cohdl-0.2.2/cohdl/_core/_intrinsic_operations.pyi
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-08 22:34:00.268839 cohdl-0.2.2/cohdl/_core/_ir/
+-rw-r--r--   0 alexander  (1000) alexander  (1000)      202 2023-05-21 19:26:34.000000 cohdl-0.2.2/cohdl/_core/_ir/__init__.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    52172 2024-05-03 19:33:55.000000 cohdl-0.2.2/cohdl/_core/_ir/_repr.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1990 2024-05-01 19:30:41.000000 cohdl-0.2.2/cohdl/_core/_primitive_type.py
+-rw-r--r--   0 alexander  (1000) alexander  (1000)    11170 2024-03-30 00:19:47.000000 cohdl-0.2.2/cohdl/_core/_signed.py
+-rw-r--r--   0 alexander  (1000) alexander  (1000)     1665 2023-06-10 21:14:05.000000 cohdl-0.2.2/cohdl/_core/_signed.pyi
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    40575 2024-04-14 15:36:28.000000 cohdl-0.2.2/cohdl/_core/_type_qualifier.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    15649 2024-04-13 17:35:40.000000 cohdl-0.2.2/cohdl/_core/_type_qualifier.pyi
+-rw-r--r--   0 alexander  (1000) alexander  (1000)     9715 2024-03-29 22:55:52.000000 cohdl-0.2.2/cohdl/_core/_unsigned.py
+-rw-r--r--   0 alexander  (1000) alexander  (1000)     1946 2023-06-10 21:13:27.000000 cohdl-0.2.2/cohdl/_core/_unsigned.pyi
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-08 22:34:00.272839 cohdl-0.2.2/cohdl/std/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     2147 2024-04-14 12:05:16.000000 cohdl-0.2.2/cohdl/std/__init__.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1033 2024-02-25 22:34:28.000000 cohdl-0.2.2/cohdl/std/_assignable_type.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      740 2024-02-18 21:56:15.000000 cohdl-0.2.2/cohdl/std/_assignable_type.pyi
+-rw-r--r--   0 alexander  (1000) alexander  (1000)      897 2023-08-03 18:13:39.000000 cohdl-0.2.2/cohdl/std/_compile.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    30291 2024-04-14 13:29:53.000000 cohdl-0.2.2/cohdl/std/_context.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    16092 2024-04-08 19:47:33.000000 cohdl-0.2.2/cohdl/std/_context.pyi
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    19919 2024-04-14 15:01:53.000000 cohdl-0.2.2/cohdl/std/_core_utility.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    17969 2024-04-12 16:36:45.000000 cohdl-0.2.2/cohdl/std/_core_utility.pyi
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1196 2023-10-28 14:08:33.000000 cohdl-0.2.2/cohdl/std/_crc.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    27180 2024-03-29 23:35:37.000000 cohdl-0.2.2/cohdl/std/_fixed.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     3193 2024-03-28 21:49:56.000000 cohdl-0.2.2/cohdl/std/_fixed.pyi
+-rw-r--r--   0 alexander  (1000) alexander  (1000)     8818 2024-03-10 15:21:13.000000 cohdl-0.2.2/cohdl/std/_formal.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     3701 2024-05-08 22:28:33.000000 cohdl-0.2.2/cohdl/std/_prefix.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     3101 2024-04-14 15:12:50.000000 cohdl-0.2.2/cohdl/std/_prefix.pyi
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     7107 2024-04-14 12:43:25.000000 cohdl-0.2.2/cohdl/std/_record.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1034 2024-04-20 22:54:36.000000 cohdl-0.2.2/cohdl/std/_record.pyi
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     6710 2024-03-29 23:37:55.000000 cohdl-0.2.2/cohdl/std/_template.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     2939 2024-03-24 21:35:53.000000 cohdl-0.2.2/cohdl/std/_template.pyi
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-08 22:34:00.272839 cohdl-0.2.2/cohdl/std/axi/
+-rw-r--r--   0 alexander  (1000) alexander  (1000)       25 2023-05-21 19:26:34.000000 cohdl-0.2.2/cohdl/std/axi/__init__.py
+-rw-r--r--   0 alexander  (1000) alexander  (1000)      669 2023-07-26 17:24:39.000000 cohdl-0.2.2/cohdl/std/axi/_axi4_channel.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-08 22:34:00.272839 cohdl-0.2.2/cohdl/std/axi/axi4_light/
+-rw-r--r--   0 alexander  (1000) alexander  (1000)       64 2024-04-01 19:46:17.000000 cohdl-0.2.2/cohdl/std/axi/axi4_light/__init__.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    12135 2024-05-04 12:15:38.000000 cohdl-0.2.2/cohdl/std/axi/axi4_light/base.py
+-rw-r--r--   0 alexander  (1000) alexander  (1000)     5185 2024-03-30 00:12:17.000000 cohdl-0.2.2/cohdl/std/axi/axi4_light/interconnect.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     7718 2024-03-29 23:07:15.000000 cohdl-0.2.2/cohdl/std/bitfield.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1688 2024-02-18 21:56:15.000000 cohdl-0.2.2/cohdl/std/bitfield.pyi
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     5399 2024-03-10 16:46:08.000000 cohdl-0.2.2/cohdl/std/enum.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     3795 2024-03-10 14:55:57.000000 cohdl-0.2.2/cohdl/std/enum.pyi
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-08 22:34:00.272839 cohdl-0.2.2/cohdl/std/formal/
+-rw-r--r--   0 alexander  (1000) alexander  (1000)      114 2023-05-21 19:26:34.000000 cohdl-0.2.2/cohdl/std/formal/__init__.py
+-rw-r--r--   0 alexander  (1000) alexander  (1000)     2201 2024-03-10 15:21:43.000000 cohdl-0.2.2/cohdl/std/formal/_builtins.py
+-rw-r--r--   0 alexander  (1000) alexander  (1000)     3097 2024-03-10 15:21:50.000000 cohdl-0.2.2/cohdl/std/formal/_checker.py
+-rw-r--r--   0 alexander  (1000) alexander  (1000)       97 2023-05-21 19:26:34.000000 cohdl-0.2.2/cohdl/std/formal/_configure.py
+-rw-r--r--   0 alexander  (1000) alexander  (1000)     4002 2024-03-10 15:21:54.000000 cohdl-0.2.2/cohdl/std/formal/_sequence.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-08 22:34:00.272839 cohdl-0.2.2/cohdl/std/reg/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)       76 2024-03-10 21:01:32.000000 cohdl-0.2.2/cohdl/std/reg/__init__.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    54518 2024-05-04 12:15:38.000000 cohdl-0.2.2/cohdl/std/reg/reg.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    27950 2024-05-04 12:15:38.000000 cohdl-0.2.2/cohdl/std/reg/reg.pyi
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     9567 2024-03-29 21:32:25.000000 cohdl-0.2.2/cohdl/std/reg/system_rdl.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     6900 2024-03-29 23:50:31.000000 cohdl-0.2.2/cohdl/std/spi.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     4019 2023-08-03 20:48:26.000000 cohdl-0.2.2/cohdl/std/spi.pyi
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     6484 2024-03-29 23:51:13.000000 cohdl-0.2.2/cohdl/std/uart.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     2928 2023-11-08 21:20:11.000000 cohdl-0.2.2/cohdl/std/uart.pyi
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    38693 2024-05-01 11:16:35.000000 cohdl-0.2.2/cohdl/std/utility.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    25351 2024-04-14 14:51:46.000000 cohdl-0.2.2/cohdl/std/utility.pyi
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-08 22:34:00.272839 cohdl-0.2.2/cohdl/utility/
+-rw-r--r--   0 alexander  (1000) alexander  (1000)      177 2023-05-21 19:26:34.000000 cohdl-0.2.2/cohdl/utility/__init__.py
+-rw-r--r--   0 alexander  (1000) alexander  (1000)     1614 2024-03-10 18:22:50.000000 cohdl-0.2.2/cohdl/utility/code_writer.py
+-rw-r--r--   0 alexander  (1000) alexander  (1000)     2917 2023-05-21 19:26:34.000000 cohdl-0.2.2/cohdl/utility/id_map.py
+-rw-r--r--   0 alexander  (1000) alexander  (1000)     4473 2024-03-30 00:02:56.000000 cohdl-0.2.2/cohdl/utility/make_target.py
+-rw-r--r--   0 alexander  (1000) alexander  (1000)      529 2023-05-21 19:26:34.000000 cohdl-0.2.2/cohdl/utility/merge_dicts.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      735 2024-03-24 17:00:13.000000 cohdl-0.2.2/cohdl/utility/source_location.py
+-rw-r--r--   0 alexander  (1000) alexander  (1000)     2168 2023-05-21 19:26:34.000000 cohdl-0.2.2/cohdl/utility/span.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     2988 2024-03-24 17:00:13.000000 cohdl-0.2.2/cohdl/utility/virtual_traceback.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-08 22:34:00.276839 cohdl-0.2.2/cohdl.egg-info/
+-rw-r--r--   0 alexander  (1000) alexander  (1000)     3216 2024-05-08 22:34:00.000000 cohdl-0.2.2/cohdl.egg-info/PKG-INFO
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     3740 2024-05-08 22:34:00.000000 cohdl-0.2.2/cohdl.egg-info/SOURCES.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)        1 2024-05-08 22:34:00.000000 cohdl-0.2.2/cohdl.egg-info/dependency_links.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)       28 2024-05-08 22:34:00.000000 cohdl-0.2.2/cohdl.egg-info/top_level.txt
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-08 22:34:00.272839 cohdl-0.2.2/playground/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)        0 2024-02-22 20:20:56.000000 cohdl-0.2.2/playground/__init__.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-08 22:34:00.272839 cohdl-0.2.2/playground/old/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      577 2023-11-18 14:41:29.000000 cohdl-0.2.2/playground/old/context_manager.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-08 22:34:00.272839 cohdl-0.2.2/playground/old/experimental/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)        0 2024-01-28 20:29:22.000000 cohdl-0.2.2/playground/old/experimental/__init__.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-08 22:34:00.272839 cohdl-0.2.2/playground/old/experimental/reg/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)       19 2024-01-28 20:29:31.000000 cohdl-0.2.2/playground/old/experimental/reg/__init__.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     2599 2024-02-03 12:37:22.000000 cohdl-0.2.2/playground/old/experimental/reg/_meta.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    12426 2024-02-03 15:17:39.000000 cohdl-0.2.2/playground/old/experimental/reg/reg.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-08 22:34:00.276839 cohdl-0.2.2/playground/old/experimental/template/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)        0 2024-02-04 16:24:57.000000 cohdl-0.2.2/playground/old/experimental/template/__init__.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      877 2024-02-04 16:38:36.000000 cohdl-0.2.2/playground/old/experimental/template/template.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     8959 2024-01-27 15:28:18.000000 cohdl-0.2.2/playground/old/meta.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1525 2024-02-22 20:10:19.000000 cohdl-0.2.2/playground/old/playgroung.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-08 22:34:00.276839 cohdl-0.2.2/playground/old/registers/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    15387 2024-02-26 18:33:49.000000 cohdl-0.2.2/playground/old/registers/example.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     2958 2024-04-01 19:54:19.000000 cohdl-0.2.2/playground/old/registers/example_axi.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     3927 2024-02-26 21:58:03.000000 cohdl-0.2.2/playground/old/registers/example_synth.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1288 2024-01-27 20:58:35.000000 cohdl-0.2.2/playground/old/registers/interface.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1227 2024-01-28 20:58:57.000000 cohdl-0.2.2/playground/old/registers/meta.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    10204 2024-01-28 11:46:33.000000 cohdl-0.2.2/playground/old/registers/reg.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    11442 2024-01-26 23:07:52.000000 cohdl-0.2.2/playground/old/registers.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     6508 2024-02-05 18:34:01.000000 cohdl-0.2.2/playground/old/template.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1146 2024-02-06 19:52:19.000000 cohdl-0.2.2/playground/old/template_new.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     5489 2024-02-11 14:16:09.000000 cohdl-0.2.2/playground/old/template_new_new.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)        0 2024-03-10 20:43:30.000000 cohdl-0.2.2/playground/playground copy 2.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      276 2024-03-05 21:13:05.000000 cohdl-0.2.2/playground/playground copy.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     3804 2024-04-13 15:29:07.000000 cohdl-0.2.2/playground/playground.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1682 2024-05-08 19:02:59.000000 cohdl-0.2.2/playground/playground_trace.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      668 2024-05-04 11:40:41.000000 cohdl-0.2.2/playground/playground_union.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-08 22:34:00.276839 cohdl-0.2.2/playground/registers/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)        0 2024-02-22 20:20:49.000000 cohdl-0.2.2/playground/registers/__init__.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     4341 2024-04-30 18:31:42.000000 cohdl-0.2.2/playground/union.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      512 2024-05-08 22:28:59.000000 cohdl-0.2.2/pyproject.toml
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)       38 2024-05-08 22:34:00.276839 cohdl-0.2.2/setup.cfg
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-08 22:34:00.276839 cohdl-0.2.2/tests/
+-rw-r--r--   0 alexander  (1000) alexander  (1000)     7003 2023-05-21 19:26:34.000000 cohdl-0.2.2/tests/test_bit.py
+-rw-r--r--   0 alexander  (1000) alexander  (1000)     8187 2023-05-21 19:26:34.000000 cohdl-0.2.2/tests/test_bitvector.py
+-rw-r--r--   0 alexander  (1000) alexander  (1000)     1986 2023-05-21 19:26:34.000000 cohdl-0.2.2/tests/test_unsigned.py
```

### Comparing `cohdl-0.2.1/LICENSE` & `cohdl-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/PKG-INFO` & `cohdl-0.2.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,17 @@
-Metadata-Version: 2.1
-Name: cohdl
-Version: 0.2.1
-Summary: A Python to VHDL compiler
-Author-email: Alexander Forster <alexander.forster123@gmail.com>
-Project-URL: Homepage, https://github.com/alexander-forster/cohdl
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # CoHDL
 
 CoHDL is a hardware description language embedded in Python. It translates a subset of Python into synthesizable VHDL.
 
 ---
+
+## examples/introduction
+
+You can find an introduction and many examples in this [documentation repository](https://github.com/alexander-forster/cohdl_documentation).
+
 ## features
 
 At its core CoHDLs language model is very similar to VHDL. Designs are made up of signals and variables built from types like `Bit` and `BitVector`. There are concurrent contexts, for expressions that would appear in the architecture scope of VHDL entities and sequential contexts equivalent to VHDL processes.
 
 Code that uses only basic features also found in VHDL (if-statements, signal/variable assignments, arithmetic operators and so on) essentially looks like VHDL written in Python syntax. On top of that CoHDL supplies many additional features
 
 
@@ -69,8 +62,8 @@
 
 CoHDL requires Python3.10 or higher and has no further dependencies. You can install it by running
 
 ```shell
 python3 -m pip install cohdl
 ```
 
-in a terminal window. You should then be able to run the code snippets, found in the introduction directory of the git repository and implement own designs.
+in a terminal window. You should then be able to run the code snippets, found in the [introduction repository](https://github.com/alexander-forster/cohdl_documentation) and implement own designs.
```

### Comparing `cohdl-0.2.1/README.md` & `cohdl-0.2.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,29 @@
+Metadata-Version: 2.1
+Name: cohdl
+Version: 0.2.2
+Summary: A Python to VHDL compiler
+Author-email: Alexander Forster <alexander.forster123@gmail.com>
+Project-URL: Homepage, https://github.com/alexander-forster/cohdl
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # CoHDL
 
 CoHDL is a hardware description language embedded in Python. It translates a subset of Python into synthesizable VHDL.
 
 ---
+
+## examples/introduction
+
+You can find an introduction and many examples in this [documentation repository](https://github.com/alexander-forster/cohdl_documentation).
+
 ## features
 
 At its core CoHDLs language model is very similar to VHDL. Designs are made up of signals and variables built from types like `Bit` and `BitVector`. There are concurrent contexts, for expressions that would appear in the architecture scope of VHDL entities and sequential contexts equivalent to VHDL processes.
 
 Code that uses only basic features also found in VHDL (if-statements, signal/variable assignments, arithmetic operators and so on) essentially looks like VHDL written in Python syntax. On top of that CoHDL supplies many additional features
 
 
@@ -57,8 +74,8 @@
 
 CoHDL requires Python3.10 or higher and has no further dependencies. You can install it by running
 
 ```shell
 python3 -m pip install cohdl
 ```
 
-in a terminal window. You should then be able to run the code snippets, found in the introduction directory of the git repository and implement own designs.
+in a terminal window. You should then be able to run the code snippets, found in the [introduction repository](https://github.com/alexander-forster/cohdl_documentation) and implement own designs.
```

### Comparing `cohdl-0.2.1/cohdl/__init__.py` & `cohdl-0.2.2/cohdl/__init__.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/_compiler/backend/vhdl/_vhdl_assembler.py` & `cohdl-0.2.2/cohdl/_compiler/backend/vhdl/_vhdl_assembler.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/_compiler/backend/vhdl/_vhdl_repr.py` & `cohdl-0.2.2/cohdl/_compiler/backend/vhdl/_vhdl_repr.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/_compiler/frontend/_generate_ir.py` & `cohdl-0.2.2/cohdl/_compiler/frontend/_generate_ir.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/_compiler/frontend/_prepare_ast.py` & `cohdl-0.2.2/cohdl/_compiler/frontend/_prepare_ast.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/_compiler/frontend/_prepare_ast_out.py` & `cohdl-0.2.2/cohdl/_compiler/frontend/_prepare_ast_out.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/_compiler/frontend/_traceback.py` & `cohdl-0.2.2/cohdl/_compiler/frontend/_traceback.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/_compiler/frontend/_value_branch.py` & `cohdl-0.2.2/cohdl/_compiler/frontend/_value_branch.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/_core/__init__.py` & `cohdl-0.2.2/cohdl/_core/__init__.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/_core/_array.py` & `cohdl-0.2.2/cohdl/_core/_array.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/_core/_bit.py` & `cohdl-0.2.2/cohdl/_core/_bit.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/_core/_bit.pyi` & `cohdl-0.2.2/cohdl/_core/_bit.pyi`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/_core/_bit_vector.py` & `cohdl-0.2.2/cohdl/_core/_bit_vector.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/_core/_bit_vector.pyi` & `cohdl-0.2.2/cohdl/_core/_bit_vector.pyi`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/_core/_boolean.py` & `cohdl-0.2.2/cohdl/_core/_boolean.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/_core/_boolean.pyi` & `cohdl-0.2.2/cohdl/_core/_boolean.pyi`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/_core/_collect_ast_and_scope.py` & `cohdl-0.2.2/cohdl/_core/_collect_ast_and_scope.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/_core/_context.py` & `cohdl-0.2.2/cohdl/_core/_context.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/_core/_enum.py` & `cohdl-0.2.2/cohdl/_core/_enum.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/_core/_inline.py` & `cohdl-0.2.2/cohdl/_core/_inline.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/_core/_integer.py` & `cohdl-0.2.2/cohdl/_core/_integer.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/_core/_integer.pyi` & `cohdl-0.2.2/cohdl/_core/_integer.pyi`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/_core/_intrinsic.py` & `cohdl-0.2.2/cohdl/_core/_intrinsic.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/_core/_intrinsic.pyi` & `cohdl-0.2.2/cohdl/_core/_intrinsic.pyi`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/_core/_intrinsic_definitions.py` & `cohdl-0.2.2/cohdl/_core/_intrinsic_definitions.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/_core/_intrinsic_definitions.pyi` & `cohdl-0.2.2/cohdl/_core/_intrinsic_definitions.pyi`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/_core/_intrinsic_operations.py` & `cohdl-0.2.2/cohdl/_core/_intrinsic_operations.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/_core/_ir/_repr.py` & `cohdl-0.2.2/cohdl/_core/_ir/_repr.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/_core/_primitive_type.py` & `cohdl-0.2.2/cohdl/_core/_primitive_type.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/_core/_signed.py` & `cohdl-0.2.2/cohdl/_core/_signed.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/_core/_signed.pyi` & `cohdl-0.2.2/cohdl/_core/_signed.pyi`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/_core/_type_qualifier.py` & `cohdl-0.2.2/cohdl/_core/_type_qualifier.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/_core/_type_qualifier.pyi` & `cohdl-0.2.2/cohdl/_core/_type_qualifier.pyi`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/_core/_unsigned.py` & `cohdl-0.2.2/cohdl/_core/_unsigned.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/_core/_unsigned.pyi` & `cohdl-0.2.2/cohdl/_core/_unsigned.pyi`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/std/__init__.py` & `cohdl-0.2.2/cohdl/std/__init__.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/std/_assignable_type.py` & `cohdl-0.2.2/cohdl/std/_assignable_type.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/std/_assignable_type.pyi` & `cohdl-0.2.2/cohdl/std/_assignable_type.pyi`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/std/_compile.py` & `cohdl-0.2.2/cohdl/std/_compile.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/std/_context.py` & `cohdl-0.2.2/cohdl/std/_context.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/std/_context.pyi` & `cohdl-0.2.2/cohdl/std/_context.pyi`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/std/_core_utility.py` & `cohdl-0.2.2/cohdl/std/_core_utility.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/std/_core_utility.pyi` & `cohdl-0.2.2/cohdl/std/_core_utility.pyi`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/std/_crc.py` & `cohdl-0.2.2/cohdl/std/_crc.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/std/_fixed.py` & `cohdl-0.2.2/cohdl/std/_fixed.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/std/_fixed.pyi` & `cohdl-0.2.2/cohdl/std/_fixed.pyi`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/std/_formal.py` & `cohdl-0.2.2/cohdl/std/_formal.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/std/_prefix.py` & `cohdl-0.2.2/cohdl/std/_prefix.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
             assert len(args) == 1 and len(kwargs) == 0
             T = type(TypeQualifierBase.decay(args[0]))
         else:
             T = self.type
 
         if is_primitive_type(T) or T is bool or T is int:
             name = self.prefix.name(kwargs.get("name", None))
-            return self.qualifier[T](*args, **kwargs, name=name)
+            return self.qualifier[T](*args, **{**kwargs, "name": name})
         else:
             with self.prefix:
                 return T(
                     *args,
                     **kwargs,
                     _qualifier_=_NamedQualifier(None, self, None),
                 )
```

### Comparing `cohdl-0.2.1/cohdl/std/_prefix.pyi` & `cohdl-0.2.2/cohdl/std/_prefix.pyi`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/std/_record.py` & `cohdl-0.2.2/cohdl/std/_record.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/std/_record.pyi` & `cohdl-0.2.2/cohdl/std/_record.pyi`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/std/_template.py` & `cohdl-0.2.2/cohdl/std/_template.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/std/_template.pyi` & `cohdl-0.2.2/cohdl/std/_template.pyi`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/std/axi/_axi4_channel.py` & `cohdl-0.2.2/cohdl/std/axi/_axi4_channel.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/std/axi/axi4_light/base.py` & `cohdl-0.2.2/cohdl/std/axi/axi4_light/base.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/std/axi/axi4_light/interconnect.py` & `cohdl-0.2.2/cohdl/std/axi/axi4_light/interconnect.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/std/bitfield.py` & `cohdl-0.2.2/cohdl/std/bitfield.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/std/bitfield.pyi` & `cohdl-0.2.2/cohdl/std/bitfield.pyi`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/std/enum.py` & `cohdl-0.2.2/cohdl/std/enum.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/std/enum.pyi` & `cohdl-0.2.2/cohdl/std/enum.pyi`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/std/formal/_builtins.py` & `cohdl-0.2.2/cohdl/std/formal/_builtins.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/std/formal/_checker.py` & `cohdl-0.2.2/cohdl/std/formal/_checker.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/std/formal/_sequence.py` & `cohdl-0.2.2/cohdl/std/formal/_sequence.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/std/reg/reg.py` & `cohdl-0.2.2/cohdl/std/reg/reg.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/std/reg/reg.pyi` & `cohdl-0.2.2/cohdl/std/reg/reg.pyi`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/std/reg/system_rdl.py` & `cohdl-0.2.2/cohdl/std/reg/system_rdl.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/std/spi.py` & `cohdl-0.2.2/cohdl/std/spi.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/std/spi.pyi` & `cohdl-0.2.2/cohdl/std/spi.pyi`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/std/uart.py` & `cohdl-0.2.2/cohdl/std/uart.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/std/uart.pyi` & `cohdl-0.2.2/cohdl/std/uart.pyi`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/std/utility.py` & `cohdl-0.2.2/cohdl/std/utility.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/std/utility.pyi` & `cohdl-0.2.2/cohdl/std/utility.pyi`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/utility/code_writer.py` & `cohdl-0.2.2/cohdl/utility/code_writer.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/utility/id_map.py` & `cohdl-0.2.2/cohdl/utility/id_map.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/utility/make_target.py` & `cohdl-0.2.2/cohdl/utility/make_target.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/utility/merge_dicts.py` & `cohdl-0.2.2/cohdl/utility/merge_dicts.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/utility/source_location.py` & `cohdl-0.2.2/cohdl/utility/source_location.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/utility/span.py` & `cohdl-0.2.2/cohdl/utility/span.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl/utility/virtual_traceback.py` & `cohdl-0.2.2/cohdl/utility/virtual_traceback.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/cohdl.egg-info/PKG-INFO` & `cohdl-0.2.2/cohdl.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 Metadata-Version: 2.1
 Name: cohdl
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python to VHDL compiler
 Author-email: Alexander Forster <alexander.forster123@gmail.com>
 Project-URL: Homepage, https://github.com/alexander-forster/cohdl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CoHDL
 
 CoHDL is a hardware description language embedded in Python. It translates a subset of Python into synthesizable VHDL.
 
 ---
+
+## examples/introduction
+
+You can find an introduction and many examples in this [documentation repository](https://github.com/alexander-forster/cohdl_documentation).
+
 ## features
 
 At its core CoHDLs language model is very similar to VHDL. Designs are made up of signals and variables built from types like `Bit` and `BitVector`. There are concurrent contexts, for expressions that would appear in the architecture scope of VHDL entities and sequential contexts equivalent to VHDL processes.
 
 Code that uses only basic features also found in VHDL (if-statements, signal/variable assignments, arithmetic operators and so on) essentially looks like VHDL written in Python syntax. On top of that CoHDL supplies many additional features
 
 
@@ -69,8 +74,8 @@
 
 CoHDL requires Python3.10 or higher and has no further dependencies. You can install it by running
 
 ```shell
 python3 -m pip install cohdl
 ```
 
-in a terminal window. You should then be able to run the code snippets, found in the introduction directory of the git repository and implement own designs.
+in a terminal window. You should then be able to run the code snippets, found in the [introduction repository](https://github.com/alexander-forster/cohdl_documentation) and implement own designs.
```

### Comparing `cohdl-0.2.1/pyproject.toml` & `cohdl-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name="cohdl"
-version="0.2.1"
+version="0.2.2"
 
 authors = [
     { name = "Alexander Forster", email = "alexander.forster123@gmail.com" }
 ]
 
 description="A Python to VHDL compiler"
 readme = "README.md"
```

### Comparing `cohdl-0.2.1/tests/test_bit.py` & `cohdl-0.2.2/tests/test_bit.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/tests/test_bitvector.py` & `cohdl-0.2.2/tests/test_bitvector.py`

 * *Files identical despite different names*

### Comparing `cohdl-0.2.1/tests/test_unsigned.py` & `cohdl-0.2.2/tests/test_unsigned.py`

 * *Files identical despite different names*

