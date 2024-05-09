# Comparing `tmp/nebx-0.1.1-py3-none-any.whl.zip` & `tmp/nebx-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 9119 bytes, number of entries: 21
--rw-rw-rw-  2.0 fat      369 b- defN 24-May-07 02:25 nebx/__init__.py
+Zip file size: 9861 bytes, number of entries: 21
+-rw-rw-rw-  2.0 fat      373 b- defN 24-May-08 14:00 nebx/__init__.py
 -rw-rw-rw-  2.0 fat      338 b- defN 24-May-07 02:48 nebx/types.py
 -rw-rw-rw-  2.0 fat      497 b- defN 24-May-07 03:30 nebx/core/ConcurrentTaskManager.py
--rw-rw-rw-  2.0 fat      155 b- defN 24-May-07 03:04 nebx/core/GeneralUtility.py
+-rw-rw-rw-  2.0 fat      827 b- defN 24-May-08 14:09 nebx/core/GeneralUtility.py
 -rw-rw-rw-  2.0 fat      719 b- defN 24-May-07 02:52 nebx/core/ScheduleManager.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-May-06 01:13 nebx/core/__init__.py
 -rw-rw-rw-  2.0 fat     1981 b- defN 24-May-06 08:14 nebx/core/http/HttpHeaderFaker.py
 -rw-rw-rw-  2.0 fat     2037 b- defN 24-May-07 02:55 nebx/core/http/RequestWrapperHttpx.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-May-06 14:14 nebx/core/http/__init__.py
 -rw-rw-rw-  2.0 fat     1294 b- defN 24-May-07 03:02 nebx/core/mail/SmtpMailer.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-May-06 08:25 nebx/core/mail/__init__.py
 -rw-rw-rw-  2.0 fat      292 b- defN 24-May-07 03:30 nebx/interfaces/IConcurrentTaskManager.py
 -rw-rw-rw-  2.0 fat      246 b- defN 24-May-07 02:53 nebx/interfaces/IHttpHeaderFaker.py
 -rw-rw-rw-  2.0 fat      302 b- defN 24-May-07 03:02 nebx/interfaces/IMailer.py
 -rw-rw-rw-  2.0 fat      431 b- defN 24-May-07 01:53 nebx/interfaces/IRequestWrapper.py
 -rw-rw-rw-  2.0 fat      247 b- defN 24-May-07 03:05 nebx/interfaces/__init__.py
--rw-rw-rw-  2.0 fat     2419 b- defN 24-May-07 06:17 nebx-0.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-07 06:17 nebx-0.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat     1085 b- defN 24-May-07 06:17 nebx-0.1.1.dist-info/license.txt
--rw-rw-rw-  2.0 fat        5 b- defN 24-May-07 06:17 nebx-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1719 b- defN 24-May-07 06:17 nebx-0.1.1.dist-info/RECORD
-21 files, 14228 bytes uncompressed, 6301 bytes compressed:  55.7%
+-rw-rw-rw-  2.0 fat     3398 b- defN 24-May-09 01:05 nebx-0.2.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-09 01:05 nebx-0.2.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat     1085 b- defN 24-May-09 01:05 nebx-0.2.0.dist-info/license.txt
+-rw-rw-rw-  2.0 fat        5 b- defN 24-May-09 01:05 nebx-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1719 b- defN 24-May-09 01:05 nebx-0.2.0.dist-info/RECORD
+21 files, 15883 bytes uncompressed, 7043 bytes compressed:  55.7%
```

## zipnote {}

```diff
@@ -42,23 +42,23 @@
 
 Filename: nebx/interfaces/IRequestWrapper.py
 Comment: 
 
 Filename: nebx/interfaces/__init__.py
 Comment: 
 
-Filename: nebx-0.1.1.dist-info/METADATA
+Filename: nebx-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: nebx-0.1.1.dist-info/WHEEL
+Filename: nebx-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: nebx-0.1.1.dist-info/license.txt
+Filename: nebx-0.2.0.dist-info/license.txt
 Comment: 
 
-Filename: nebx-0.1.1.dist-info/top_level.txt
+Filename: nebx-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: nebx-0.1.1.dist-info/RECORD
+Filename: nebx-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nebx/__init__.py

```diff
@@ -1,7 +1,9 @@
 ﻿from nebx.core.ConcurrentTaskManager import ConcurrentTaskManager
 from nebx.core.mail.SmtpMailer import SmtpMailer
 from nebx.core.ScheduleManager import ScheduleManager
-from nebx.core.GeneralUtility import *
 from nebx.core.http.RequestWrapperHttpx import RequestWrapperHttpx
 from nebx.core.http.HttpHeaderFaker import HttpHeaderFaker
+from nebx.core.GeneralUtility import *
+
+
 from nebx.types import *
```

## nebx/core/GeneralUtility.py

```diff
@@ -1,6 +1,29 @@
 ﻿from typing import Coroutine
+import csv
+from iteration_utilities import unique_everseen
+from urllib.parse import urlparse
+from typing import Iterable
 
 
 async def async_task_sequence(coroutines: list[Coroutine]) -> None:
     for coro in coroutines:
         await coro
+
+
+def read_csv(file_path: str, delimiter: str = ",", remove_duplicates: bool = False) -> list[dict]:
+    data = []
+    with open(file_path, "r") as file:
+        reader = csv.DictReader(file, delimiter=delimiter)
+        for row in reader:
+            data.append(row)
+
+    return data if remove_duplicates is False else remove_duplicate(data)
+
+
+def remove_duplicate(data: Iterable) -> list[any]:
+    return list(unique_everseen(data))
+
+
+def get_domain_name(url: str) -> str:
+    result = urlparse(url)
+    return result.netloc
```

## Comparing `nebx-0.1.1.dist-info/license.txt` & `nebx-0.2.0.dist-info/license.txt`

 * *Files identical despite different names*

## Comparing `nebx-0.1.1.dist-info/RECORD` & `nebx-0.2.0.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-nebx/__init__.py,sha256=RAjWQkJD1HIvHfn-hCGgsLNRWkQ8jTE1LYcb2vPsEAo,369
+nebx/__init__.py,sha256=woKVi12aDyvrPE5SoxhM00ieMulYBMqjEs537W8Denk,373
 nebx/types.py,sha256=UBSD0ZktbTmIjeUTvIEJsUjtuDmfJV5YoUB75dkerE0,338
 nebx/core/ConcurrentTaskManager.py,sha256=jM6t5uE3B2_6NV4xAB84ge9tFryjyVMqquEsjfiLhQo,497
-nebx/core/GeneralUtility.py,sha256=IPE1Cb0CKSTV2o_rfHOSzqYLjQwpMiilLTHrnH4Az_0,155
+nebx/core/GeneralUtility.py,sha256=KqsHqujOaqMImDOeJw60-GUBGMQJaE_s5n4DyXnfW2I,827
 nebx/core/ScheduleManager.py,sha256=ajmNhHKfoDjq1bt3aAAQO8SxE8E4zcSRWe7NJD_tTgs,719
 nebx/core/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 nebx/core/http/HttpHeaderFaker.py,sha256=igryi7hxM2BgmR_Vo_wGi1aW1Vtu7Kuh_o5R_loW7ts,1981
 nebx/core/http/RequestWrapperHttpx.py,sha256=8poEMjrW8vPXtdoJH4UIF8_A9dkGWvgIb4Pd-0YsSck,2037
 nebx/core/http/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 nebx/core/mail/SmtpMailer.py,sha256=CMQJuvu6822hpsW6BiAeRlLaA1F6spNK0eQOFrLoklM,1294
 nebx/core/mail/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 nebx/interfaces/IConcurrentTaskManager.py,sha256=TLmM5zFK4nZiD13zE5DGLqY9capRhgWGeLBEUvwHqtk,292
 nebx/interfaces/IHttpHeaderFaker.py,sha256=ggadizXYOQ8cKgE-n2xtz5bT0kRmZM2DftNjY7OQ19s,246
 nebx/interfaces/IMailer.py,sha256=211KT7o3fho5X23fwV0u8QxwZTAq2KqVKGV6wUb3QQw,302
 nebx/interfaces/IRequestWrapper.py,sha256=ZbwQDCHZrRIwfA4Cl_73My83bf_e-hPUy_SrOdLrq98,431
 nebx/interfaces/__init__.py,sha256=LDpLNk-kLJ8HNx5vFdvTl94kEneqL6ejSGP5UjcbSLs,247
-nebx-0.1.1.dist-info/METADATA,sha256=Iwzulp2vpqRtm1PATgk6y8G467U4ena05iFALh2dfpY,2419
-nebx-0.1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-nebx-0.1.1.dist-info/license.txt,sha256=gIEAc9_FjY2KjP_JDPyhRp5IA0EFGCD6PUCP2yYU2tE,1085
-nebx-0.1.1.dist-info/top_level.txt,sha256=dKSKVLYBX-GbQFokq6OmGeo3faqjK9IYEct_ucfaLu8,5
-nebx-0.1.1.dist-info/RECORD,,
+nebx-0.2.0.dist-info/METADATA,sha256=ul-3LDEOgIAy4kOS2IoJhJOM6FFdHc7Q36gRM7DrmbM,3398
+nebx-0.2.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+nebx-0.2.0.dist-info/license.txt,sha256=gIEAc9_FjY2KjP_JDPyhRp5IA0EFGCD6PUCP2yYU2tE,1085
+nebx-0.2.0.dist-info/top_level.txt,sha256=dKSKVLYBX-GbQFokq6OmGeo3faqjK9IYEct_ucfaLu8,5
+nebx-0.2.0.dist-info/RECORD,,
```

