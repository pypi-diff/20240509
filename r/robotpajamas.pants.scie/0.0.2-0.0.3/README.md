# Comparing `tmp/robotpajamas.pants.scie-0.0.2-py3-none-any.whl.zip` & `tmp/robotpajamas.pants.scie-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 11399 bytes, number of entries: 12
--rw-r--r--  2.0 unx        0 b- defN 23-May-22 19:19 experimental/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-22 19:19 experimental/scie/__init__.py
--rw-r--r--  2.0 unx     2160 b- defN 23-May-22 19:19 experimental/scie/config.py
--rw-r--r--  2.0 unx      677 b- defN 23-May-22 19:19 experimental/scie/register.py
--rw-r--r--  2.0 unx    10467 b- defN 23-May-22 19:19 experimental/scie/rules.py
--rw-r--r--  2.0 unx     1535 b- defN 23-May-22 19:19 experimental/scie/subsystems.py
--rw-r--r--  2.0 unx     4247 b- defN 23-May-22 19:19 experimental/scie/target_types.py
--rw-r--r--  2.0 unx     4576 b- defN 23-May-22 19:19 robotpajamas.pants.scie-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-22 19:19 robotpajamas.pants.scie-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-May-22 19:19 robotpajamas.pants.scie-0.0.2.dist-info/namespace_packages.txt
--rw-r--r--  2.0 unx       13 b- defN 23-May-22 19:19 robotpajamas.pants.scie-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1070 b- defN 23-May-22 19:19 robotpajamas.pants.scie-0.0.2.dist-info/RECORD
-12 files, 24838 bytes uncompressed, 9559 bytes compressed:  61.5%
+Zip file size: 11539 bytes, number of entries: 12
+-rw-r--r--  2.0 unx        0 b- defN 24-May-09 13:32 experimental/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-09 13:32 experimental/scie/__init__.py
+-rw-r--r--  2.0 unx     2160 b- defN 24-May-09 13:32 experimental/scie/config.py
+-rw-r--r--  2.0 unx      686 b- defN 24-May-09 13:32 experimental/scie/register.py
+-rw-r--r--  2.0 unx    10446 b- defN 24-May-09 13:32 experimental/scie/rules.py
+-rw-r--r--  2.0 unx     1544 b- defN 24-May-09 13:32 experimental/scie/subsystems.py
+-rw-r--r--  2.0 unx     4183 b- defN 24-May-09 13:32 experimental/scie/target_types.py
+-rw-r--r--  2.0 unx     4956 b- defN 24-May-09 13:32 robotpajamas.pants.scie-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-09 13:32 robotpajamas.pants.scie-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-May-09 13:32 robotpajamas.pants.scie-0.0.3.dist-info/namespace_packages.txt
+-rw-r--r--  2.0 unx       13 b- defN 24-May-09 13:32 robotpajamas.pants.scie-0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1070 b- defN 24-May-09 13:32 robotpajamas.pants.scie-0.0.3.dist-info/RECORD
+12 files, 25151 bytes uncompressed, 9699 bytes compressed:  61.4%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: experimental/scie/subsystems.py
 Comment: 
 
 Filename: experimental/scie/target_types.py
 Comment: 
 
-Filename: robotpajamas.pants.scie-0.0.2.dist-info/METADATA
+Filename: robotpajamas.pants.scie-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: robotpajamas.pants.scie-0.0.2.dist-info/WHEEL
+Filename: robotpajamas.pants.scie-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: robotpajamas.pants.scie-0.0.2.dist-info/namespace_packages.txt
+Filename: robotpajamas.pants.scie-0.0.3.dist-info/namespace_packages.txt
 Comment: 
 
-Filename: robotpajamas.pants.scie-0.0.2.dist-info/top_level.txt
+Filename: robotpajamas.pants.scie-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: robotpajamas.pants.scie-0.0.2.dist-info/RECORD
+Filename: robotpajamas.pants.scie-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## experimental/scie/register.py

```diff
@@ -4,15 +4,15 @@
 """A Self Contained Interpreted Executable Launcher.
 
 See https://github.com/a-scie/jump for details.
 """
 
 from __future__ import annotations
 
-from typing import Iterable
+from collections.abc import Iterable
 
 from experimental.scie.rules import rules as scie_rules
 from experimental.scie.target_types import ScieTarget
 from pants.engine.rules import Rule
 from pants.engine.target import Target
 from pants.engine.unions import UnionRule
```

## experimental/scie/rules.py

```diff
@@ -1,17 +1,18 @@
 # Copyright 2023 Pants project contributors (see CONTRIBUTORS.md).
 # Licensed under the Apache License, Version 2.0 (see LICENSE).
 
 from __future__ import annotations
 
 import logging
 import os
-from dataclasses import asdict, dataclass, replace
+from collections.abc import Iterable, Mapping
+from dataclasses import asdict, dataclass
 from pathlib import PurePath
-from typing import Final, Iterable, Mapping
+from typing import Final
 
 import toml
 from experimental.scie.config import Command, Config, File, Interpreter, LiftConfig
 from experimental.scie.subsystems import Science
 from experimental.scie.target_types import (
     ScieBinaryNameField,
     ScieDependenciesField,
@@ -35,15 +36,15 @@
     DigestContents,
     FileContent,
     MergeDigests,
     Snapshot,
 )
 from pants.engine.platform import Platform
 from pants.engine.process import Process, ProcessResult
-from pants.engine.rules import Get, MultiGet, Rule, collect_rules, rule, rule_helper
+from pants.engine.rules import Get, MultiGet, Rule, collect_rules, rule
 from pants.engine.target import (
     DependenciesRequest,
     DescriptionField,
     FieldSetsPerTarget,
     FieldSetsPerTargetRequest,
     HydratedSources,
     HydrateSourcesRequest,
@@ -66,15 +67,14 @@
     binary_name: ScieBinaryNameField
     description: DescriptionField
     dependencies: ScieDependenciesField
     platforms: SciePlatformField
     lift: ScieLiftSourceField
 
 
-@rule_helper
 async def _get_interpreter_config(targets: Targets) -> Interpreter:
     # Get the interpreter_constraints for the Pex to determine which version of the Python Standalone to use
     constraints = await Get(
         InterpreterConstraints,
         InterpreterConstraintsRequest([tgt.address for tgt in targets]),
     )
     # TODO: Pull the interpreter_universe from somewhere else (Python Build standalone?)
@@ -108,15 +108,14 @@
 def _contains_pex(built_package: BuiltPackage) -> bool:
     return any(
         artifact.relpath is not None and artifact.relpath.endswith(".pex")
         for artifact in built_package.artifacts
     )
 
 
-@rule_helper
 async def _parse_lift_source(source: ScieLiftSourceField) -> Config:
     hydrated_source = await Get(HydratedSources, HydrateSourcesRequest(source))
     digest_contents = await Get(DigestContents, Digest, hydrated_source.snapshot.digest)
     content = digest_contents[0].content.decode("utf-8")
     lift_toml = toml.loads(content)
     logger.error(lift_toml)
     return Config(**lift_toml)
```

## experimental/scie/subsystems.py

```diff
@@ -1,30 +1,30 @@
 # Copyright 2022 Pants project contributors (see CONTRIBUTORS.md).
 # Licensed under the Apache License, Version 2.0 (see LICENSE).
 
 from __future__ import annotations
 
-from typing import Iterable
+from collections.abc import Iterable
 
 from pants.core.util_rules.external_tool import TemplatedExternalTool
 from pants.engine.rules import Rule, collect_rules
 from pants.engine.unions import UnionRule
 from pants.util.strutil import softwrap
 
 
 class Science(TemplatedExternalTool):
     options_scope = "science"
     help = softwrap("""A high level tool to build scies with.""")
 
-    default_version = "0.1.1"
+    default_version = "0.3.4"
     default_known_versions = [
-        "0.1.1|linux_arm64|f2082538b6dcd65326cf20ac5aee832f1743f278e36fba9af09fcf81597190ac|5570863",
-        "0.1.1|linux_x86_64|edfd24effab7c4ff07c581d278e363aa5e64e9f5e397f13596194ce4583adb3c|6465812",
-        "0.1.1|macos_arm64|68a8a09a4792e578da763e621d37695b0e7876dab3b10b54c970722875f05e9a|3455268",
-        "0.1.1|macos_x86_64|defcd967c9d51272a749030fcbb57871070cfb7e8943d9391d3a537da69251f0|3573076",
+        "0.3.4|linux_arm64|9d30ffffee826f52a69c056fcb7c5e9a25d48980c573066cf64dd7f987c13b66|8578528",
+        "0.3.4|linux_x86_64|926791a2243446711ed84b5465aa3786eed3c90d1654dd86ea82498fd5fcd4a2|9728714",
+        "0.3.4|macos_arm64|d1e6eefd9bc89f2edb39775435ee25ad7fd5b158431561ac6fbbbf1552f855c0|4303745",
+        "0.3.4|macos_x86_64|c3012fdd237a918db378bc215ec985aca0f26f42e8e4c80066032da94322897a|4502350",
     ]
 
     default_url_template = (
         "https://github.com/a-scie/lift/releases/download/v{version}/science-{platform}"
     )
 
     default_url_platform_mapping = {
```

## experimental/scie/target_types.py

```diff
@@ -5,16 +5,14 @@
 
 from enum import Enum
 
 from pants.core.goals.package import OutputPathField
 from pants.engine.target import (
     COMMON_TARGET_FIELDS,
     Dependencies,
-    DictStringToStringField,
-    NestedDictStringToStringField,
     OptionalSingleSourceField,
     StringSequenceField,
     Target,
 )
 from pants.util.strutil import softwrap
```

## Comparing `robotpajamas.pants.scie-0.0.2.dist-info/METADATA` & `robotpajamas.pants.scie-0.0.3.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 Metadata-Version: 2.1
 Name: robotpajamas.pants.scie
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Pants plugin adding support for packaging SCIE.
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://github.com/sureshjoshi/pants-plugins
 Project-URL: Source, https://github.com/sureshjoshi/pants-plugins
 Project-URL: Tracker, https://github.com/sureshjoshi/pants-plugins/issues
+Project-URL: Changelog, https://www.pantsbuild.org/docs/changelog
+Keywords: pants,pants-plugin,scie
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Software Development :: Build Tools
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # pants-scie-plugin
 
 This plugin provides a `scie_binary` target that can be used to create a single-file Python executable with an embedded Python interpreter, built via [scie-jump](https://github.com/a-scie/jump). 
 
 It uses [science](https://github.com/a-scie/lift) and a `.toml` configuration file to build the executable, expecting a `pex_binary` as a dependency.
 
 ## Installation
 
-This plugin was developed using Python 3.9 and Pants 2.16.0.rc3, but should work with Pants 2.15+ (however, your mileage may vary).
+This plugin was tested on Python 3.9 and Pants 2.20.
 
 Add the following to your `pants.toml` file:
 
 ```toml
 [GLOBAL]
 plugins = [
     ...
```

## Comparing `robotpajamas.pants.scie-0.0.2.dist-info/RECORD` & `robotpajamas.pants.scie-0.0.3.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 experimental/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 experimental/scie/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 experimental/scie/config.py,sha256=CxZPXqNUZ7Q8kc7RpJk8_tMqPxPUlxqIx2OQpKP-G9A,2160
-experimental/scie/register.py,sha256=oy-TfCP5G0Mgoc73h6wHqhPSfI8-WofKG8eAGdgCMi4,677
-experimental/scie/rules.py,sha256=idslPTRFaUJINoeqwJOXP48f8mnqgdXNvyBV6rrL_H4,10467
-experimental/scie/subsystems.py,sha256=TVZ7r9a9YUObOlRCijYv8d5BsS8kPsmJyz_llJCi0Qc,1535
-experimental/scie/target_types.py,sha256=5sqJO0YCU_LXXcBvaeBZFQ06qC5uhUOyD6R3XgDOm3I,4247
-robotpajamas.pants.scie-0.0.2.dist-info/METADATA,sha256=mksXA0YKa-AGZjiuBkwYmPa37t7EAkfwk61zf8DIi9E,4576
-robotpajamas.pants.scie-0.0.2.dist-info/WHEEL,sha256=ZL1lC_LiPDNRgDnOl2taCMc83aPEUZgHHv2h-LDgdiM,92
-robotpajamas.pants.scie-0.0.2.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-robotpajamas.pants.scie-0.0.2.dist-info/top_level.txt,sha256=WSY2rwaGHd8blqg-pL5FRbAjnA07FjL5jwB6CnTTaG8,13
-robotpajamas.pants.scie-0.0.2.dist-info/RECORD,,
+experimental/scie/register.py,sha256=HVojxBnR4hMhELCsTGlYCx0Rrg-IljanNniO2pdyy1s,686
+experimental/scie/rules.py,sha256=_RXGUaqxP9mnQw0ZaIVBI_374s3nZpAc8gLEYWEic74,10446
+experimental/scie/subsystems.py,sha256=hKKV_pAHUCyvMSLPFy-CQhkuFDm1oPvA1qqyzBn3zDY,1544
+experimental/scie/target_types.py,sha256=UgWYJ_ikI3GMUarJuHsVyCFsthaQp9O_X_A2P5HS0cc,4183
+robotpajamas.pants.scie-0.0.3.dist-info/METADATA,sha256=bFye4LtguJpaA5VZtrR1iChvC19NKcJUlYD3lY-EwUw,4956
+robotpajamas.pants.scie-0.0.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+robotpajamas.pants.scie-0.0.3.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+robotpajamas.pants.scie-0.0.3.dist-info/top_level.txt,sha256=WSY2rwaGHd8blqg-pL5FRbAjnA07FjL5jwB6CnTTaG8,13
+robotpajamas.pants.scie-0.0.3.dist-info/RECORD,,
```

