# Comparing `tmp/smarter_client-0.1.9.tar.gz` & `tmp/smarter_client-0.2.0.tar.gz`

## Comparing `smarter_client-0.1.9.tar` & `smarter_client-0.2.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    22281 2020-02-02 00:00:00.000000 smarter_client-0.1.9/.pylintrc
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 smarter_client-0.1.9/conftest.py
--rw-r--r--   0        0        0    55699 2020-02-02 00:00:00.000000 smarter_client-0.1.9/pdm.lock
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 smarter_client-0.1.9/requirements.txt
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 smarter_client-0.1.9/setup.cfg
--rw-r--r--   0        0        0     8685 2020-02-02 00:00:00.000000 smarter_client-0.1.9/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 smarter_client-0.1.9/.github/workflows/upload-previews.yml
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 smarter_client-0.1.9/.vscode/launch.json
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 smarter_client-0.1.9/.vscode/settings.json
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 smarter_client-0.1.9/smarter_client/__init__.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 smarter_client-0.1.9/smarter_client/_consts.py
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 smarter_client-0.1.9/smarter_client/dict_util.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 smarter_client-0.1.9/smarter_client/version.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 smarter_client-0.1.9/smarter_client/domain/__init__.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 smarter_client-0.1.9/smarter_client/domain/identity_toolkit_client.py
--rw-r--r--   0        0        0    11690 2020-02-02 00:00:00.000000 smarter_client-0.1.9/smarter_client/domain/models.py
--rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 smarter_client-0.1.9/smarter_client/domain/smarter_client.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 smarter_client-0.1.9/smarter_client/domain/decorators/session.py
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 smarter_client-0.1.9/smarter_client/managed_devices/__init__.py
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 smarter_client-0.1.9/smarter_client/managed_devices/base.py
--rw-r--r--   0        0        0     4132 2020-02-02 00:00:00.000000 smarter_client-0.1.9/smarter_client/managed_devices/kettle_v3.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smarter_client-0.1.9/src/smarter_kettle_client/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smarter_client-0.1.9/tests/__init__.py
--rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 smarter_client-0.1.9/tests/dict_util_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smarter_client-0.1.9/tests/domain/__init__.py
--rw-r--r--   0        0        0    10825 2020-02-02 00:00:00.000000 smarter_client-0.1.9/tests/domain/models_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smarter_client-0.1.9/tests/domain/decoorators/__init__.py
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 smarter_client-0.1.9/tests/domain/decoorators/session_test.py
--rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 smarter_client-0.1.9/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 smarter_client-0.1.9/LICENSE
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 smarter_client-0.1.9/README.md
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 smarter_client-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 smarter_client-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0    22281 2020-02-02 00:00:00.000000 smarter_client-0.2.0/.pylintrc
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 smarter_client-0.2.0/conftest.py
+-rw-r--r--   0        0        0    55968 2020-02-02 00:00:00.000000 smarter_client-0.2.0/pdm.lock
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 smarter_client-0.2.0/requirements.txt
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 smarter_client-0.2.0/setup.cfg
+-rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 smarter_client-0.2.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 smarter_client-0.2.0/.github/workflows/upload-previews.yml
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 smarter_client-0.2.0/.vscode/launch.json
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 smarter_client-0.2.0/.vscode/settings.json
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 smarter_client-0.2.0/smarter_client/__init__.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 smarter_client-0.2.0/smarter_client/_consts.py
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 smarter_client-0.2.0/smarter_client/dict_util.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 smarter_client-0.2.0/smarter_client/version.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 smarter_client-0.2.0/smarter_client/domain/__init__.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 smarter_client-0.2.0/smarter_client/domain/identity_toolkit_client.py
+-rw-r--r--   0        0        0    12154 2020-02-02 00:00:00.000000 smarter_client-0.2.0/smarter_client/domain/models.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 smarter_client-0.2.0/smarter_client/domain/smarter_client.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 smarter_client-0.2.0/smarter_client/domain/decorators/session.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 smarter_client-0.2.0/smarter_client/managed_devices/__init__.py
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 smarter_client-0.2.0/smarter_client/managed_devices/base.py
+-rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 smarter_client-0.2.0/smarter_client/managed_devices/kettle_v3.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smarter_client-0.2.0/src/smarter_kettle_client/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smarter_client-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 smarter_client-0.2.0/tests/dict_util_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smarter_client-0.2.0/tests/domain/__init__.py
+-rw-r--r--   0        0        0    13893 2020-02-02 00:00:00.000000 smarter_client-0.2.0/tests/domain/models_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smarter_client-0.2.0/tests/domain/decoorators/__init__.py
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 smarter_client-0.2.0/tests/domain/decoorators/session_test.py
+-rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 smarter_client-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 smarter_client-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 smarter_client-0.2.0/README.md
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 smarter_client-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 smarter_client-0.2.0/PKG-INFO
```

### Comparing `smarter_client-0.1.9/.pylintrc` & `smarter_client-0.2.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `smarter_client-0.1.9/conftest.py` & `smarter_client-0.2.0/conftest.py`

 * *Files identical despite different names*

### Comparing `smarter_client-0.1.9/pdm.lock` & `smarter_client-0.2.0/pdm.lock`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 # This file is @generated by PDM.
 # It is not intended for manual editing.
 
 [metadata]
 groups = ["default", "testing", "build"]
 strategy = ["cross_platform", "inherit_metadata"]
 lock_version = "4.4.1"
-content_hash = "sha256:783180abd8b5c4b2ca727fc9d895f4bff07d9fcf8f63eac865b010b229b29bef"
+content_hash = "sha256:eeab048ccad46114ddec3595bf43eb19fa5f2fcb6b51d91752012c44db2dc250"
 
 [[package]]
 name = "aiohttp"
-version = "3.9.3"
+version = "3.9.5"
 requires_python = ">=3.8"
 summary = "Async http client/server framework (asyncio)"
 groups = ["default"]
 dependencies = [
     "aiosignal>=1.1.2",
     "attrs>=17.3.0",
     "frozenlist>=1.1.1",
     "multidict<7.0,>=4.5",
     "yarl<2.0,>=1.0",
 ]
 files = [
-    {file = "aiohttp-3.9.3-cp312-cp312-macosx_10_9_universal2.whl", hash = "sha256:38a19bc3b686ad55804ae931012f78f7a534cce165d089a2059f658f6c91fa60"},
-    {file = "aiohttp-3.9.3-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:770d015888c2a598b377bd2f663adfd947d78c0124cfe7b959e1ef39f5b13869"},
-    {file = "aiohttp-3.9.3-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:ee43080e75fc92bf36219926c8e6de497f9b247301bbf88c5c7593d931426679"},
-    {file = "aiohttp-3.9.3-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:52df73f14ed99cee84865b95a3d9e044f226320a87af208f068ecc33e0c35b96"},
-    {file = "aiohttp-3.9.3-cp312-cp312-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:dc9b311743a78043b26ffaeeb9715dc360335e5517832f5a8e339f8a43581e4d"},
-    {file = "aiohttp-3.9.3-cp312-cp312-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:b955ed993491f1a5da7f92e98d5dad3c1e14dc175f74517c4e610b1f2456fb11"},
-    {file = "aiohttp-3.9.3-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:504b6981675ace64c28bf4a05a508af5cde526e36492c98916127f5a02354d53"},
-    {file = "aiohttp-3.9.3-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:a6fe5571784af92b6bc2fda8d1925cccdf24642d49546d3144948a6a1ed58ca5"},
-    {file = "aiohttp-3.9.3-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:ba39e9c8627edc56544c8628cc180d88605df3892beeb2b94c9bc857774848ca"},
-    {file = "aiohttp-3.9.3-cp312-cp312-musllinux_1_1_i686.whl", hash = "sha256:e5e46b578c0e9db71d04c4b506a2121c0cb371dd89af17a0586ff6769d4c58c1"},
-    {file = "aiohttp-3.9.3-cp312-cp312-musllinux_1_1_ppc64le.whl", hash = "sha256:938a9653e1e0c592053f815f7028e41a3062e902095e5a7dc84617c87267ebd5"},
-    {file = "aiohttp-3.9.3-cp312-cp312-musllinux_1_1_s390x.whl", hash = "sha256:c3452ea726c76e92f3b9fae4b34a151981a9ec0a4847a627c43d71a15ac32aa6"},
-    {file = "aiohttp-3.9.3-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:ff30218887e62209942f91ac1be902cc80cddb86bf00fbc6783b7a43b2bea26f"},
-    {file = "aiohttp-3.9.3-cp312-cp312-win32.whl", hash = "sha256:38f307b41e0bea3294a9a2a87833191e4bcf89bb0365e83a8be3a58b31fb7f38"},
-    {file = "aiohttp-3.9.3-cp312-cp312-win_amd64.whl", hash = "sha256:b791a3143681a520c0a17e26ae7465f1b6f99461a28019d1a2f425236e6eedb5"},
-    {file = "aiohttp-3.9.3.tar.gz", hash = "sha256:90842933e5d1ff760fae6caca4b2b3edba53ba8f4b71e95dacf2818a2aca06f7"},
+    {file = "aiohttp-3.9.5-cp312-cp312-macosx_10_9_universal2.whl", hash = "sha256:c7a4b7a6cf5b6eb11e109a9755fd4fda7d57395f8c575e166d363b9fc3ec4678"},
+    {file = "aiohttp-3.9.5-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:0a158704edf0abcac8ac371fbb54044f3270bdbc93e254a82b6c82be1ef08f3c"},
+    {file = "aiohttp-3.9.5-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:d153f652a687a8e95ad367a86a61e8d53d528b0530ef382ec5aaf533140ed00f"},
+    {file = "aiohttp-3.9.5-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:82a6a97d9771cb48ae16979c3a3a9a18b600a8505b1115cfe354dfb2054468b4"},
+    {file = "aiohttp-3.9.5-cp312-cp312-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:60cdbd56f4cad9f69c35eaac0fbbdf1f77b0ff9456cebd4902f3dd1cf096464c"},
+    {file = "aiohttp-3.9.5-cp312-cp312-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:8676e8fd73141ded15ea586de0b7cda1542960a7b9ad89b2b06428e97125d4fa"},
+    {file = "aiohttp-3.9.5-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:da00da442a0e31f1c69d26d224e1efd3a1ca5bcbf210978a2ca7426dfcae9f58"},
+    {file = "aiohttp-3.9.5-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:18f634d540dd099c262e9f887c8bbacc959847cfe5da7a0e2e1cf3f14dbf2daf"},
+    {file = "aiohttp-3.9.5-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:320e8618eda64e19d11bdb3bd04ccc0a816c17eaecb7e4945d01deee2a22f95f"},
+    {file = "aiohttp-3.9.5-cp312-cp312-musllinux_1_1_i686.whl", hash = "sha256:2faa61a904b83142747fc6a6d7ad8fccff898c849123030f8e75d5d967fd4a81"},
+    {file = "aiohttp-3.9.5-cp312-cp312-musllinux_1_1_ppc64le.whl", hash = "sha256:8c64a6dc3fe5db7b1b4d2b5cb84c4f677768bdc340611eca673afb7cf416ef5a"},
+    {file = "aiohttp-3.9.5-cp312-cp312-musllinux_1_1_s390x.whl", hash = "sha256:393c7aba2b55559ef7ab791c94b44f7482a07bf7640d17b341b79081f5e5cd1a"},
+    {file = "aiohttp-3.9.5-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:c671dc117c2c21a1ca10c116cfcd6e3e44da7fcde37bf83b2be485ab377b25da"},
+    {file = "aiohttp-3.9.5-cp312-cp312-win32.whl", hash = "sha256:5a7ee16aab26e76add4afc45e8f8206c95d1d75540f1039b84a03c3b3800dd59"},
+    {file = "aiohttp-3.9.5-cp312-cp312-win_amd64.whl", hash = "sha256:5ca51eadbd67045396bc92a4345d1790b7301c14d1848feaac1d6a6c9289e888"},
+    {file = "aiohttp-3.9.5.tar.gz", hash = "sha256:edea7d15772ceeb29db4aff55e482d4bcfb6ae160ce144f2682de02f6d693551"},
 ]
 
 [[package]]
 name = "aiosignal"
 version = "1.3.1"
 requires_python = ">=3.7"
 summary = "aiosignal: a list of registered asynchronous callbacks"
@@ -165,15 +165,15 @@
 ]
 
 [[package]]
 name = "coverage"
 version = "7.4.4"
 requires_python = ">=3.8"
 summary = "Code coverage measurement for Python"
-groups = ["default", "testing"]
+groups = ["testing"]
 files = [
     {file = "coverage-7.4.4-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:201bef2eea65e0e9c56343115ba3814e896afe6d36ffd37bab783261db430f76"},
     {file = "coverage-7.4.4-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:41c9c5f3de16b903b610d09650e5e27adbfa7f500302718c9ffd1c12cf9d6818"},
     {file = "coverage-7.4.4-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:d898fe162d26929b5960e4e138651f7427048e72c853607f2b200909794ed978"},
     {file = "coverage-7.4.4-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:3ea79bb50e805cd6ac058dfa3b5c8f6c040cb87fe83de10845857f5535d1db70"},
     {file = "coverage-7.4.4-cp312-cp312-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ce4b94265ca988c3f8e479e741693d143026632672e3ff924f25fab50518dd51"},
     {file = "coverage-7.4.4-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:00838a35b882694afda09f85e469c96367daa3f3f2b097d846a7216993d37f4c"},
@@ -187,15 +187,15 @@
 
 [[package]]
 name = "coverage"
 version = "7.4.4"
 extras = ["toml"]
 requires_python = ">=3.8"
 summary = "Code coverage measurement for Python"
-groups = ["default", "testing"]
+groups = ["testing"]
 dependencies = [
     "coverage==7.4.4",
 ]
 files = [
     {file = "coverage-7.4.4-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:201bef2eea65e0e9c56343115ba3814e896afe6d36ffd37bab783261db430f76"},
     {file = "coverage-7.4.4-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:41c9c5f3de16b903b610d09650e5e27adbfa7f500302718c9ffd1c12cf9d6818"},
     {file = "coverage-7.4.4-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:d898fe162d26929b5960e4e138651f7427048e72c853607f2b200909794ed978"},
@@ -348,15 +348,15 @@
 ]
 
 [[package]]
 name = "iniconfig"
 version = "2.0.0"
 requires_python = ">=3.7"
 summary = "brain-dead simple config-ini parsing"
-groups = ["default", "testing"]
+groups = ["testing"]
 files = [
     {file = "iniconfig-2.0.0-py3-none-any.whl", hash = "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"},
     {file = "iniconfig-2.0.0.tar.gz", hash = "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3"},
 ]
 
 [[package]]
 name = "isort"
@@ -385,15 +385,15 @@
 ]
 
 [[package]]
 name = "markupsafe"
 version = "2.1.5"
 requires_python = ">=3.7"
 summary = "Safely add untrusted strings to HTML/XML markup."
-groups = ["default", "testing"]
+groups = ["testing"]
 files = [
     {file = "MarkupSafe-2.1.5-cp312-cp312-macosx_10_9_universal2.whl", hash = "sha256:8dec4936e9c3100156f8a2dc89c4b88d5c435175ff03413b443469c7c8c5f4d1"},
     {file = "MarkupSafe-2.1.5-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:3c6b973f22eb18a789b1460b4b91bf04ae3f0c4234a0a6aa6b0a92f6f7b951d4"},
     {file = "MarkupSafe-2.1.5-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ac07bad82163452a6884fe8fa0963fb98c2346ba78d779ec06bd7a6262132aee"},
     {file = "MarkupSafe-2.1.5-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f5dfb42c4604dddc8e4305050aa6deb084540643ed5804d7455b5df8fe16f5e5"},
     {file = "MarkupSafe-2.1.5-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:ea3d8a3d18833cf4304cd2fc9cbb1efe188ca9b5efef2bdac7adc20594a0e46b"},
     {file = "MarkupSafe-2.1.5-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:d050b3361367a06d752db6ead6e7edeb0009be66bc3bae0ee9d97fb326badc2a"},
@@ -458,15 +458,15 @@
 ]
 
 [[package]]
 name = "packaging"
 version = "24.0"
 requires_python = ">=3.7"
 summary = "Core utilities for Python packages"
-groups = ["build", "default", "testing"]
+groups = ["build", "testing"]
 files = [
     {file = "packaging-24.0-py3-none-any.whl", hash = "sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5"},
     {file = "packaging-24.0.tar.gz", hash = "sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9"},
 ]
 
 [[package]]
 name = "platformdirs"
@@ -480,15 +480,15 @@
 ]
 
 [[package]]
 name = "pluggy"
 version = "1.4.0"
 requires_python = ">=3.8"
 summary = "plugin and hook calling mechanisms for python"
-groups = ["default", "testing"]
+groups = ["testing"]
 files = [
     {file = "pluggy-1.4.0-py3-none-any.whl", hash = "sha256:7db9f7b503d67d1c5b95f59773ebb58a8c1c288129a88665838012cfb07b8981"},
     {file = "pluggy-1.4.0.tar.gz", hash = "sha256:8c85c2876142a764e5b7548e7d9a0e0ddb46f5185161049a79b7e974454223be"},
 ]
 
 [[package]]
 name = "protobuf"
@@ -615,37 +615,37 @@
 files = [
     {file = "pyproject_hooks-1.0.0-py3-none-any.whl", hash = "sha256:283c11acd6b928d2f6a7c73fa0d01cb2bdc5f07c57a2eeb6e83d5e56b97976f8"},
     {file = "pyproject_hooks-1.0.0.tar.gz", hash = "sha256:f271b298b97f5955d53fb12b72c1fb1948c22c1a6b70b315c54cedaca0264ef5"},
 ]
 
 [[package]]
 name = "pyrebase4"
-version = "4.7.1"
+version = "4.8.0"
 summary = "A simple python wrapper for the Firebase API with current deps"
 groups = ["default"]
 dependencies = [
     "gcloud>=0.18.3",
     "oauth2client>=4.1.2",
     "pycryptodome>=3.6.4",
     "python-jwt>=2.0.1",
     "requests-toolbelt<1.0,>=0.7.1",
-    "requests<2.30,>=2.19.1",
+    "requests>=2.31",
     "urllib3<2,>=1.21.1",
 ]
 files = [
-    {file = "Pyrebase4-4.7.1-py3-none-any.whl", hash = "sha256:e5416123cb54b483f6223986bddd0209390bb8b05c20c7e62908d0dad9dce911"},
-    {file = "Pyrebase4-4.7.1.tar.gz", hash = "sha256:270f6827d0039d98846222c9f26646ba6c401cd89b7c038c3abe36f4801d7754"},
+    {file = "Pyrebase4-4.8.0-py3-none-any.whl", hash = "sha256:7352256f0f60e19adb018f1da87923182050c687c82a85460df3e05121d5eff2"},
+    {file = "pyrebase4-4.8.0.tar.gz", hash = "sha256:e749c791c7a44a123f246502f29d672a4ef688eb1cbfcd97c5ceca8afcdd72df"},
 ]
 
 [[package]]
 name = "pytest"
 version = "8.1.1"
 requires_python = ">=3.8"
 summary = "pytest: simple powerful testing with Python"
-groups = ["default", "testing"]
+groups = ["testing"]
 dependencies = [
     "colorama; sys_platform == \"win32\"",
     "iniconfig",
     "packaging",
     "pluggy<2.0,>=1.4",
 ]
 files = [
@@ -654,58 +654,58 @@
 ]
 
 [[package]]
 name = "pytest-asyncio"
 version = "0.23.6"
 requires_python = ">=3.8"
 summary = "Pytest support for asyncio"
-groups = ["default", "testing"]
+groups = ["testing"]
 dependencies = [
     "pytest<9,>=7.0.0",
 ]
 files = [
     {file = "pytest-asyncio-0.23.6.tar.gz", hash = "sha256:ffe523a89c1c222598c76856e76852b787504ddb72dd5d9b6617ffa8aa2cde5f"},
     {file = "pytest_asyncio-0.23.6-py3-none-any.whl", hash = "sha256:68516fdd1018ac57b846c9846b954f0393b26f094764a28c955eabb0536a4e8a"},
 ]
 
 [[package]]
 name = "pytest-cov"
 version = "5.0.0"
 requires_python = ">=3.8"
 summary = "Pytest plugin for measuring coverage."
-groups = ["default", "testing"]
+groups = ["testing"]
 dependencies = [
     "coverage[toml]>=5.2.1",
     "pytest>=4.6",
 ]
 files = [
     {file = "pytest-cov-5.0.0.tar.gz", hash = "sha256:5837b58e9f6ebd335b0f8060eecce69b662415b16dc503883a02f45dfeb14857"},
     {file = "pytest_cov-5.0.0-py3-none-any.whl", hash = "sha256:4f0764a1219df53214206bf1feea4633c3b558a2925c8b59f144f682861ce652"},
 ]
 
 [[package]]
 name = "pytest-localserver"
 version = "0.8.1"
 requires_python = ">=3.5"
 summary = "pytest plugin to test server connections locally."
-groups = ["default", "testing"]
+groups = ["testing"]
 dependencies = [
     "werkzeug>=0.10",
 ]
 files = [
     {file = "pytest-localserver-0.8.1.tar.gz", hash = "sha256:66569c34fef31a5750b16effd1cd1288a7a90b59155d005e7f916accd3dee4f1"},
     {file = "pytest_localserver-0.8.1-py3-none-any.whl", hash = "sha256:13bc3d9aca719a60a2d1e535c5f0a58c7c1c2ad749f6e9cf198a358f5345e1d0"},
 ]
 
 [[package]]
 name = "pytest-mock"
 version = "3.14.0"
 requires_python = ">=3.8"
 summary = "Thin-wrapper around the mock package for easier use with pytest"
-groups = ["default", "testing"]
+groups = ["testing"]
 dependencies = [
     "pytest>=6.2.5",
 ]
 files = [
     {file = "pytest-mock-3.14.0.tar.gz", hash = "sha256:2719255a1efeceadbc056d6bf3df3d1c5015530fb40cf347c0f9afac88410bd0"},
     {file = "pytest_mock-3.14.0-py3-none-any.whl", hash = "sha256:0b72c38033392a5f4621342fe11e9219ac11ec9d375f8e2a0c164539e0d70f6f"},
 ]
@@ -736,27 +736,27 @@
 files = [
     {file = "python_jwt-4.1.0-py2.py3-none-any.whl", hash = "sha256:1f4d44b6b9176375489c0374c71f18f27f52524e689174e11dd39a801170c91b"},
     {file = "python_jwt-4.1.0.tar.gz", hash = "sha256:f89af071d9bda4741bc80754bd1cfce73e434a2cbb7855086d8604a10bd3fdc5"},
 ]
 
 [[package]]
 name = "requests"
-version = "2.29.0"
+version = "2.31.0"
 requires_python = ">=3.7"
 summary = "Python HTTP for Humans."
 groups = ["default"]
 dependencies = [
     "certifi>=2017.4.17",
     "charset-normalizer<4,>=2",
     "idna<4,>=2.5",
-    "urllib3<1.27,>=1.21.1",
+    "urllib3<3,>=1.21.1",
 ]
 files = [
-    {file = "requests-2.29.0-py3-none-any.whl", hash = "sha256:e8f3c9be120d3333921d213eef078af392fba3933ab7ed2d1cba3b56f2568c3b"},
-    {file = "requests-2.29.0.tar.gz", hash = "sha256:f2e34a75f4749019bb0e3effb66683630e4ffeaf75819fb51bebef1bf5aef059"},
+    {file = "requests-2.31.0-py3-none-any.whl", hash = "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f"},
+    {file = "requests-2.31.0.tar.gz", hash = "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"},
 ]
 
 [[package]]
 name = "requests-toolbelt"
 version = "0.10.1"
 requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
 summary = "A utility belt for advanced users of python-requests"
@@ -781,21 +781,21 @@
 files = [
     {file = "rsa-4.9-py3-none-any.whl", hash = "sha256:90260d9058e514786967344d0ef75fa8727eed8a7d2e43ce9f4bcf1b536174f7"},
     {file = "rsa-4.9.tar.gz", hash = "sha256:e38464a49c6c85d7f1351b0126661487a7e0a14a50f1675ec50eb34d4f20ef21"},
 ]
 
 [[package]]
 name = "setuptools"
-version = "69.2.0"
+version = "69.5.1"
 requires_python = ">=3.8"
 summary = "Easily download, build, install, upgrade, and uninstall Python packages"
 groups = ["default"]
 files = [
-    {file = "setuptools-69.2.0-py3-none-any.whl", hash = "sha256:c21c49fb1042386df081cb5d86759792ab89efca84cf114889191cd09aacc80c"},
-    {file = "setuptools-69.2.0.tar.gz", hash = "sha256:0ff4183f8f42cd8fa3acea16c45205521a4ef28f73c6391d8a25e92893134f2e"},
+    {file = "setuptools-69.5.1-py3-none-any.whl", hash = "sha256:c636ac361bc47580504644275c9ad802c50415c7522212252c033bd15f301f32"},
+    {file = "setuptools-69.5.1.tar.gz", hash = "sha256:6c1fccdac05a97e598fb0ae3bbed5904ccb317337a51139dcd51453611bbb987"},
 ]
 
 [[package]]
 name = "six"
 version = "1.16.0"
 requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*"
 summary = "Python 2 and 3 compatibility utilities"
@@ -849,14 +849,25 @@
 groups = ["default"]
 files = [
     {file = "typing_extensions-4.10.0-py3-none-any.whl", hash = "sha256:69b1a937c3a517342112fb4c6df7e72fc39a38e7891a5730ed4985b5214b5475"},
     {file = "typing_extensions-4.10.0.tar.gz", hash = "sha256:b0abd7c89e8fb96f98db18d86106ff1d90ab692004eb746cf6eda2682f91b3cb"},
 ]
 
 [[package]]
+name = "tzdata"
+version = "2024.1"
+requires_python = ">=2"
+summary = "Provider of IANA time zone data"
+groups = ["testing"]
+files = [
+    {file = "tzdata-2024.1-py2.py3-none-any.whl", hash = "sha256:9068bc196136463f5245e51efda838afa15aaeca9903f49050dfa2679db4d252"},
+    {file = "tzdata-2024.1.tar.gz", hash = "sha256:2674120f8d891909751c38abcdfd386ac0a5a1127954fbc332af6b5ceae07efd"},
+]
+
+[[package]]
 name = "urllib3"
 version = "1.26.18"
 requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*"
 summary = "HTTP library with thread-safe connection pooling, file post, and more."
 groups = ["default"]
 files = [
     {file = "urllib3-1.26.18-py2.py3-none-any.whl", hash = "sha256:34b97092d7e0a3a8cf7cd10e386f401b3737364026c45e622aa02903dffe0f07"},
@@ -864,15 +875,15 @@
 ]
 
 [[package]]
 name = "werkzeug"
 version = "3.0.2"
 requires_python = ">=3.8"
 summary = "The comprehensive WSGI web application library."
-groups = ["default", "testing"]
+groups = ["testing"]
 dependencies = [
     "MarkupSafe>=2.1.1",
 ]
 files = [
     {file = "werkzeug-3.0.2-py3-none-any.whl", hash = "sha256:3aac3f5da756f93030740bc235d3e09449efcf65f2f55e3602e1d851b8f48795"},
     {file = "werkzeug-3.0.2.tar.gz", hash = "sha256:e39b645a6ac92822588e7b39a692e7828724ceae0b0d702ef96701f90e70128d"},
 ]
```

### Comparing `smarter_client-0.1.9/.github/workflows/ci.yml` & `smarter_client-0.2.0/.github/workflows/ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,18 @@
 
       - uses: pdm-project/setup-pdm@v4
         with:
           python-version: ${{ matrix.python-version }}
           cache: true
           allow-python-prereleases: true
 
+      - name: install deps
+        run: |
+          pdm venv create --with-pip --force $PYTHON
+          pdm install -G testing
       # - name: Python Linter
         # uses: sunnysid3up/python-linter@master
         # with:
           # source: "smarter_kettle_client"
           # mypy-options: "--ignore-missing-imports --show-error-codes"
           # pylint-options: "--rcfile=.pylintrc"
       - run: pdm run -v pylint --rcfile .pylintrc smarter_client
```

### Comparing `smarter_client-0.1.9/.github/workflows/upload-previews.yml` & `smarter_client-0.2.0/.github/workflows/upload-previews.yml`

 * *Files identical despite different names*

### Comparing `smarter_client-0.1.9/smarter_client/dict_util.py` & `smarter_client-0.2.0/smarter_client/dict_util.py`

 * *Files 9% similar despite different names*

```diff
@@ -47,28 +47,17 @@
         return put
     else:
         parent[child] = put
 
     return new_dict
 
 
-def delete_dict(target: dict, path: str) -> dict:
+def delete_dict(target: dict, path: str, value: None = None) -> dict:
     new_dict = deepcopy(target)
     parent, child = _find_or_create_node(new_dict, path)
 
     if child is None:
         raise ValueError('Cannot delete root of dict')
     else:
         del parent[child]
 
     return new_dict
-
-# def xpatch_dict(target: dict, path: patch: dict):
-#   for key, value in source.items():
-#       if isinstance(value, dict):
-#           if key not in target:
-#               target[key] = {}
-#           patch_dict(target[key], value)
-#       if
-#       else:
-#           target[key] = value
-#   return target
```

### Comparing `smarter_client-0.1.9/smarter_client/version.py` & `smarter_client-0.2.0/smarter_client/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 """The `version` module holds the version information for Smarter Kettle Client."""
 from __future__ import annotations as _annotations
 
 __all__ = 'VERSION', 'version_info'
 
-VERSION = '0.1.9'
+VERSION = '0.2.0'
 """The version of Smarter Kettle Client."""
 
 
 def version_short() -> str:
     """Return the `major.minor` part of version.
 
     It returns '2.1' if version is '2.1.1'.
```

### Comparing `smarter_client-0.1.9/smarter_client/domain/identity_toolkit_client.py` & `smarter_client-0.2.0/smarter_client/domain/identity_toolkit_client.py`

 * *Files identical despite different names*

### Comparing `smarter_client-0.1.9/smarter_client/domain/models.py` & `smarter_client-0.2.0/smarter_client/domain/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from abc import ABCMeta
 from abc import abstractmethod
 from typing import Any, Callable, Self
 from pprint import pprint
+from pyrebase.pyrebase import Stream
 
 import datetime
 from smarter_client.dict_util import delete_dict, patch_dict, put_dict
 from . import smarter_client
 
 
 class BaseEntity(metaclass=ABCMeta):
@@ -25,15 +26,15 @@
         self.identifier = identifier
 
         return self
 
     @classmethod
     def from_data(cls, client: smarter_client.SmarterClient, data: dict, identifier: str = None) -> Self:
         self = cls(client)
-        self._data = data
+        self._data = data or {}
         self.identifier = identifier
         self._init_data()
 
         return self
 
     def __init__(self, client: smarter_client.SmarterClient):
         self.client = client
@@ -216,35 +217,49 @@
 # </Command>
 
 
 class Device(BaseEntity):
     commands: Commands = None
     settings: Settings = None
     status: Status = None
-    _stream_close: Callable = None
+    _stream: Stream = None
 
     def __init__(self, client: smarter_client.SmarterClient):
         super().__init__(client)
 
     # Public methods
-    def watch(self, callback=lambda: None):
-        if self._stream_close is not None:
+    def watch(self, callback: Callable[[dict], None]):
+        if self._stream is not None:
             raise RuntimeError(
                 'Already watching device. Call unwatch() first. Support for multiple callbacks may be implemented in a later version')
 
         def on_data(event):
             self._on_event(event)
             callback(event)
-        self._stream_close = self.client.watch_device_attribute(
+        self._stream = self.client.watch_device_attribute(
             self.identifier, on_data)
 
     def unwatch(self):
-        if self._stream_close is not None:
-            self._stream_close()
-            self._stream_close = None
+        if self._stream is not None:
+            try:
+                self._stream.close()
+            except Exception as e:
+                print(f'Error closing stream: {e}')
+                # TODO: log
+            self._stream = None
+
+    @property
+    def is_watching(self):
+        """Returns True if the device is being watched."""
+        return self._stream is not None
+
+    @property
+    def is_stream_active(self):
+        """Experimental: Returns True if the stream connection is active."""
+        return self.is_watching and self._stream.sse.running
 
     # Private methods
     def _init_data(self):
         self.commands = Commands.from_data(
             self.client, self._data.get('commands'), self)
 
         self.settings = Settings.from_data(
@@ -275,20 +290,20 @@
         self.kind = data.get('kind')
         self.local_id = data.get('localId')
         self.email = data.get('email')
         self.display_name = data.get('displayName')
         self.id_token = data.get('idToken')
         self.registered = data.get('registered')
         self.refresh_token = data.get('refreshToken')
-        self.session_duration = data.get('expiresIn')
+        self.session_duration = int(data.get('expiresIn'))
 
-        self.expires_at = self._get_expiration_datetime(data)
+        self.expires_at = self._get_expiration_datetime()
 
-    def _get_expiration_datetime(self, data: dict):
-        return datetime.datetime.now() + datetime.timedelta(0, int(data.get('expiresIn')))
+    def _get_expiration_datetime(self):
+        return datetime.datetime.now() + datetime.timedelta(0, self.session_duration)
 
     def is_expired(self) -> bool:
         """
         Returns True if the session has expired.
         """
         return self.expires_at <= datetime.datetime.now()
 
@@ -299,15 +314,15 @@
         """
         return (self.expires_at - datetime.datetime.now()).total_seconds()
 
     def update(self, data: dict):
         self.id_token = data.get('idToken')
         self.refresh_token = data.get('refreshToken')
         self.local_id = data.get('userId')
-        self.expires_at = self._get_expiration_datetime(data)
+        self.expires_at = self._get_expiration_datetime()
 
 
 # </LoginSession>
 
 class Network(BaseEntity):
     access_tokens_fcm: dict[str, str] = None
     associated_devices: list[Device] = None
```

### Comparing `smarter_client-0.1.9/smarter_client/domain/smarter_client.py` & `smarter_client-0.2.0/smarter_client/domain/smarter_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Module contains implementation of Smarter Firebase API
 """
 from __future__ import annotations
 from typing import Callable
-from pyrebase.pyrebase import Stream
 import pyrebase
 
 from smarter_client.domain.decorators.session import refreshsession
 from .models import LoginSession
 from .._consts import API_KEY
 
 
@@ -75,13 +74,14 @@
         return database \
             .child('devices') \
             .child(device_id) \
             .child('commands') \
             .child(command) \
             .push(data, self.token)
 
+    # TODO fix leaky abstraction
     @refreshsession
-    def watch_device_attribute(self, device_id: str, callback) -> Callable:
+    def watch_device_attribute(self, device_id: str, callback) -> pyrebase.pyrebase.Stream:
         database = self.app.database()
         stream = database.child('devices').child(
             device_id).stream(callback, self.token)
-        return lambda: stream.close()
+        return stream
```

### Comparing `smarter_client-0.1.9/smarter_client/managed_devices/__init__.py` & `smarter_client-0.2.0/smarter_client/managed_devices/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """
 Module containing wrappers for specific devices
 """
 from smarter_client.domain import Network, Device
 from smarter_client.managed_devices.kettle_v3 import SmarterKettleV3
+from smarter_client.managed_devices.base import BaseDevice
 
 
 def load_from_network(network: Network, user_id: str) -> list[Device]:
     """
     Get devices from a given network
     """
+    network.fetch()
     return (
         wrapper for wrapper in
         (
             get_device_wrapper(device, user_id)
             for device in network.associated_devices
         )
         if wrapper is not None
@@ -24,10 +26,12 @@
     Get a device wrapper for a specific user by inferring the correct type
     from the device properties
     """
     device.fetch()
     model = device.status.get('device_model')
     match model:
         case 'SMKET01':
-            return SmarterKettleV3.from_device(device, user_id)
+            managed = SmarterKettleV3.from_device(device, user_id)
+            managed.subscribe_status()
+            return managed
         case _:
             print(f'Unknown device model: {model}')
```

### Comparing `smarter_client-0.1.9/tests/dict_util_test.py` & `smarter_client-0.2.0/tests/dict_util_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     def test_deletes_nested(self, original_state: dict):
         expected = deepcopy(original_state)
         original_state['commands']['test_command']['test-instance'] = {
             'value': {'state': 'RCV'}
         }
 
         assert delete_dict(
-            original_state, 'commands/test_command/test-instance') == expected
+            original_state, 'commands/test_command/test-instance', None) == expected
 
     def test_delete_root_error(self, original_state: dict):
         with pytest.raises(ValueError):
             delete_dict(original_state, '/')
 
     def test_put_root(self, original_state: dict):
         assert put_dict(original_state, '/', {'new': 1}) == {'new': 1}
```

### Comparing `smarter_client-0.1.9/tests/domain/models_test.py` & `smarter_client-0.2.0/tests/domain/models_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,17 @@
-# from __future__ import annotations
-
-# from unittest.mock import MagicMock
 import datetime
 from typing import Type
-from unittest.mock import MagicMock, Mock, patch
+from unittest.mock import MagicMock, Mock
 from zoneinfo import ZoneInfo
+
 import pytest
 import time_machine
 
-import sys
-import types
-
-from smarter_client.domain.models import Command, CommandInstance, Commands, Device, LoginSession
+from smarter_client.domain.models import (Command, CommandInstance, Commands,
+                                          Device, LoginSession)
 from smarter_client.domain.smarter_client import SmarterClient
 
 
 @pytest.fixture
 def SmarterClientMock(mocker):
 
     mock = MagicMock(
@@ -147,15 +143,15 @@
                         'test-instance': {'value': 0, 'state': 'RCV'}
                     }
                 },
                 'settings': {
                     'network': 'network-1'
                 },
                 'status': {
-
+                    'default': True
                 }
             },
             'device-1'
         )
 
     def test_device_from_data_should_create_instance(self, device):
 
@@ -187,35 +183,99 @@
         callback = mocker.Mock()
         device.watch(callback)
 
         with pytest.raises(RuntimeError):
             device.watch(callback)
 
     def test_unwatch_does_not_raise_error(self, mocker, device: Device, SmarterClientMock: Type[SmarterClient]):
-        callback = mocker.Mock()
-        # device.watch(callback)
         device.unwatch()
 
     def test_unwatch_closes_stream(self, mocker, device: Device, SmarterClientMock: Type[SmarterClient]):
         mock_client = SmarterClientMock()
         callback = mocker.Mock()
-        stream_close_mock = mocker.Mock()
-        mock_client.watch_device_attribute.return_value = stream_close_mock
+        mock_stream = mocker.MagicMock()
+        mock_client.watch_device_attribute.return_value = mock_stream
         device.watch(callback)
 
         device.unwatch()
 
-        stream_close_mock.assert_called()
+        mock_stream.close.assert_called()
 
     def test_fetch_calls_client(self, device: Device, SmarterClientMock: Type[SmarterClient]):
         mock_client = SmarterClientMock()
         device.fetch()
 
         mock_client.get_device.assert_called_with('device-1')
 
+    def test_device_update_put(self, device: Device, SmarterClientMock: Type[SmarterClient], mocker):
+        device_callback = {}
+        watch_callback = mocker.Mock()
+        stream_mock = mocker.MagicMock()
+        mock_client = SmarterClientMock()
+
+        def device_watch_mock(self, cb):
+            device_callback['value'] = cb
+        mock_client.watch_device_attribute.side_effect = device_watch_mock
+        mock_client.watch_device_attribute.return_value = stream_mock
+
+        device.watch(watch_callback)
+
+        assert device_callback is not None
+        device_callback['value']({
+            'event': 'put',
+            'path': 'status',
+            'data': {'test': True}
+        })
+
+        assert device.status == {'test': True}
+
+    def test_device_update_patch(self, device: Device, SmarterClientMock: Type[SmarterClient], mocker):
+        device_callback = {}
+        watch_callback = mocker.Mock()
+        stream_mock = mocker.MagicMock()
+        mock_client = SmarterClientMock()
+
+        def device_watch_mock(self, cb):
+            device_callback['value'] = cb
+        mock_client.watch_device_attribute.side_effect = device_watch_mock
+        mock_client.watch_device_attribute.return_value = stream_mock
+
+        device.watch(watch_callback)
+
+        assert device_callback is not None
+        device_callback['value']({
+            'event': 'patch',
+            'path': 'status',
+            'data': {'test': True}
+        })
+
+        assert device.status == {'default': True, 'test': True}
+
+    def test_device_update_delete(self, device: Device, SmarterClientMock: Type[SmarterClient], mocker):
+        device_callback = {}
+        watch_callback = mocker.Mock()
+        stream_mock = mocker.MagicMock()
+        mock_client = SmarterClientMock()
+
+        def device_watch_mock(self, cb):
+            device_callback['value'] = cb
+        mock_client.watch_device_attribute.side_effect = device_watch_mock
+        mock_client.watch_device_attribute.return_value = stream_mock
+
+        device.watch(watch_callback)
+
+        assert device_callback is not None
+        device_callback['value']({
+            'event': 'put',
+            'path': 'status',
+            'data': None
+        })
+
+        assert device.status == {}
+
 
 class TestLoginSession:
     def test_login_session_from_data_should_create_instance(self):
         with time_machine.travel(datetime.datetime.fromtimestamp(0, tz=ZoneInfo('UTC')), tick=False):
             session = LoginSession(
                 {
                     'kind': 'test-kind',
@@ -306,20 +366,46 @@
                     'expiresIn': 100
                 }
             )
 
             traveler.shift(90)
             session.update({
                 'idToken': 'new-token',
-                'expiresIn': 101
+                'refreshToken': 'test-refresh'
             })
 
             assert session.id_token == 'new-token'
-            assert session.expires_in == 101
-            assert session.expires_at == datetime.datetime.fromtimestamp(191)
+            assert session.expires_in == 100
+            assert session.expires_at == datetime.datetime.fromtimestamp(190)
+
+    def test_refresh_updates_time(self):
+        with time_machine.travel(datetime.datetime.fromtimestamp(0, tz=ZoneInfo('UTC')), tick=False) as traveler:
+            session = LoginSession(
+                {
+                    'kind': 'test-kind',
+                    'localId': 'test-id',
+                    'email': 'test-email',
+                    'displayName': 'test-display-name',
+                    'idToken': 'test-token',
+                    'registered': True,
+                    'refreshToken': 'test-refresh',
+                    'expiresIn': 100
+                }
+            )
+
+            traveler.shift(99)
+
+            session.update({
+                'idToken': 'new-token',
+                'localId': 'test-id',
+                'refreshToken': 'test-refresh',
+            })
+
+            assert session.expires_at == datetime.datetime.fromtimestamp(
+                199)
 
 
 class TestNetwork:
     pass
 
 
 class TestSettings:
```

### Comparing `smarter_client-0.1.9/tests/domain/decoorators/session_test.py` & `smarter_client-0.2.0/tests/domain/decoorators/session_test.py`

 * *Files identical despite different names*

### Comparing `smarter_client-0.1.9/.gitignore` & `smarter_client-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `smarter_client-0.1.9/LICENSE` & `smarter_client-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smarter_client-0.1.9/README.md` & `smarter_client-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `smarter_client-0.1.9/pyproject.toml` & `smarter_client-0.2.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -2,24 +2,19 @@
 name = "smarter-client"
 description = "Smarter Kettle client library"
 authors = [
     { name = "Kirill Birger", email = "kbirger@gmail.com" },
     { name = "@kbirger" },
 ]
 dependencies = [
-    "astroid==3.1.0",
-    "pylint==3.1.0",
-    "pytest>=6.2.0",
-    "pytest-cov>=2.4.0",
-    "pytest-localserver>=0.4.1",
-    "pytest-asyncio>=0.16.0",
-    "pytest-mock>=3.6.1",
-    "aiohttp>=3.9.3",
-    "pyrebase4==4.7.1",
-    "setuptools>=69.2.0",
+    "astroid~=3.1",
+    "pylint~=3.1",
+    "aiohttp~=3.9",
+    "setuptools>=69.5.1",
+    "pyrebase4>=4.8.0",
 ]
 dynamic = ['version']
 requires-python = ">=3.12.2"
 readme = "README.md"
 license = { text = "MIT" }
 keywords = ["smarter kettle python"]
 classifiers = [
@@ -29,28 +24,32 @@
 ]
 [tool.pdm]
 distribution = false
 
 [tool.hatch.version]
 path = 'smarter_client/version.py'
 
+[tool.hatch.metadata]
+allow-direct-references = true
+
 [tool.pdm.dev-dependencies]
 testing = [
-    "pytest>=6.2.0",
-    "pytest-cov>=2.4.0",
-    "pytest-localserver>=0.4.1",
-    "pytest-asyncio>=0.16.0",
-    "pytest-mock>=3.6.1",
+    "pytest>=8.1",
+    "pytest-cov>=5.0.0",
+    "pytest-localserver>=0.8.1",
+    "pytest-asyncio>=0.23.6",
+    "pytest-mock>=3.14.0",
     "time-machine>=2.14.1",
+    "tzdata>=2024.1",
 ]
 
 
 build = ["build"]
 
 [project.urls]
 Homepage = "https://www.github.com/kbirger/smarter-kettle-client"
 "Release Notes" = "https://www.github.com/kbirger/smarter-kettle-client"
 Source = "https://www.github.com/kbirger/smarter-kettle-client"
 
 [build-system]
 requires = ["hatchling"]
-build-backend = "hatchling.build"
+build-backend = "hatchling.build"
```

### Comparing `smarter_client-0.1.9/PKG-INFO` & `smarter_client-0.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,28 @@
 Metadata-Version: 2.3
 Name: smarter-client
-Version: 0.1.9
+Version: 0.2.0
 Summary: Smarter Kettle client library
 Project-URL: Homepage, https://www.github.com/kbirger/smarter-kettle-client
 Project-URL: Release Notes, https://www.github.com/kbirger/smarter-kettle-client
 Project-URL: Source, https://www.github.com/kbirger/smarter-kettle-client
 Author: @kbirger
 Author-email: Kirill Birger <kbirger@gmail.com>
 License: MIT
 License-File: LICENSE
 Keywords: smarter kettle python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.12.2
-Requires-Dist: aiohttp>=3.9.3
-Requires-Dist: astroid==3.1.0
-Requires-Dist: pylint==3.1.0
-Requires-Dist: pyrebase4==4.7.1
-Requires-Dist: pytest-asyncio>=0.16.0
-Requires-Dist: pytest-cov>=2.4.0
-Requires-Dist: pytest-localserver>=0.4.1
-Requires-Dist: pytest-mock>=3.6.1
-Requires-Dist: pytest>=6.2.0
-Requires-Dist: setuptools>=69.2.0
+Requires-Dist: aiohttp~=3.9
+Requires-Dist: astroid~=3.1
+Requires-Dist: pylint~=3.1
+Requires-Dist: pyrebase4>=4.8.0
+Requires-Dist: setuptools>=69.5.1
 Description-Content-Type: text/markdown
 
 # smarter-kettle-client
 Python client for Smarter Kettle integration
 
 [![CI](https://github.com/kbirger/smarter-kettle-client/actions/workflows/ci.yml/badge.svg)](https://github.com/kbirger/smarter-kettle-client/actions/workflows/ci.yml)
 [![Coverage](https://coverage-badge.samuelcolvin.workers.dev/kbirger/smarter-kettle-client.svg)](https://coverage-badge.samuelcolvin.workers.dev/redirect/kbirger/smarter-kettle-client)
```

