# Comparing `tmp/shareyourcloning_linkml-0.1.4a0.tar.gz` & `tmp/shareyourcloning_linkml-0.1.5a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shareyourcloning_linkml-0.1.4a0.tar", max compression
+gzip compressed data, was "shareyourcloning_linkml-0.1.5a0.tar", max compression
```

## Comparing `shareyourcloning_linkml-0.1.4a0.tar` & `shareyourcloning_linkml-0.1.5a0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1087 2024-05-08 11:34:24.551916 shareyourcloning_linkml-0.1.4a0/LICENSE
--rw-r--r--   0        0        0      923 2024-05-08 11:34:24.551916 shareyourcloning_linkml-0.1.4a0/README.md
--rw-r--r--   0        0        0    17584 2024-05-08 11:34:24.555916 shareyourcloning_linkml-0.1.4a0/project/excel/shareyourcloning_linkml.xlsx
--rw-r--r--   0        0        0     4170 2024-05-08 11:34:24.555916 shareyourcloning_linkml-0.1.4a0/project/graphql/shareyourcloning_linkml.graphql
--rw-r--r--   0        0        0     6881 2024-05-08 11:34:24.555916 shareyourcloning_linkml-0.1.4a0/project/jsonld/shareyourcloning_linkml.context.jsonld
--rw-r--r--   0        0        0    82573 2024-05-08 11:34:24.555916 shareyourcloning_linkml-0.1.4a0/project/jsonld/shareyourcloning_linkml.jsonld
--rw-r--r--   0        0        0    42013 2024-05-08 11:34:24.555916 shareyourcloning_linkml-0.1.4a0/project/jsonschema/shareyourcloning_linkml.schema.json
--rw-r--r--   0        0        0    54517 2024-05-08 11:34:24.555916 shareyourcloning_linkml-0.1.4a0/project/owl/shareyourcloning_linkml.owl.ttl
--rw-r--r--   0        0        0      400 2024-05-08 11:34:24.555916 shareyourcloning_linkml-0.1.4a0/project/prefixmap/shareyourcloning_linkml.yaml
--rw-r--r--   0        0        0     6097 2024-05-08 11:34:24.555916 shareyourcloning_linkml-0.1.4a0/project/protobuf/shareyourcloning_linkml.proto
--rw-r--r--   0        0        0    64703 2024-05-08 11:34:24.555916 shareyourcloning_linkml-0.1.4a0/project/python/shareyourcloning_linkml.py
--rw-r--r--   0        0        0    44003 2024-05-08 11:34:24.555916 shareyourcloning_linkml-0.1.4a0/project/shacl/shareyourcloning_linkml.shacl.ttl
--rw-r--r--   0        0        0     9599 2024-05-08 11:34:24.555916 shareyourcloning_linkml-0.1.4a0/project/shex/shareyourcloning_linkml.shex
--rw-r--r--   0        0        0    30549 2024-05-08 11:34:24.555916 shareyourcloning_linkml-0.1.4a0/project/sqlschema/shareyourcloning_linkml.sql
--rw-r--r--   0        0        0     1499 2024-05-08 11:34:34.396056 shareyourcloning_linkml-0.1.4a0/pyproject.toml
--rw-r--r--   0        0        0      186 2024-05-08 11:34:24.555916 shareyourcloning_linkml-0.1.4a0/src/shareyourcloning_linkml/_version.py
--rw-r--r--   0        0        0       41 2024-05-08 11:34:24.555916 shareyourcloning_linkml-0.1.4a0/src/shareyourcloning_linkml/datamodel/__init__.py
--rw-r--r--   0        0        0    25925 2024-05-08 11:34:24.555916 shareyourcloning_linkml-0.1.4a0/src/shareyourcloning_linkml/datamodel/_models.py
--rw-r--r--   0        0        0       42 2024-05-08 11:34:24.555916 shareyourcloning_linkml-0.1.4a0/src/shareyourcloning_linkml/datamodel/models.py
--rw-r--r--   0        0        0    15604 2024-05-08 11:34:24.555916 shareyourcloning_linkml-0.1.4a0/src/shareyourcloning_linkml/schema/shareyourcloning_linkml.yaml
--rw-r--r--   0        0        0     1877 1970-01-01 00:00:00.000000 shareyourcloning_linkml-0.1.4a0/PKG-INFO
+-rw-r--r--   0        0        0     1087 2024-05-08 16:47:39.665000 shareyourcloning_linkml-0.1.5a0/LICENSE
+-rw-r--r--   0        0        0      923 2024-05-08 16:47:39.665000 shareyourcloning_linkml-0.1.5a0/README.md
+-rw-r--r--   0        0        0    17584 2024-05-08 16:47:39.669000 shareyourcloning_linkml-0.1.5a0/project/excel/shareyourcloning_linkml.xlsx
+-rw-r--r--   0        0        0     4170 2024-05-08 16:47:39.669000 shareyourcloning_linkml-0.1.5a0/project/graphql/shareyourcloning_linkml.graphql
+-rw-r--r--   0        0        0     6881 2024-05-08 16:47:39.669000 shareyourcloning_linkml-0.1.5a0/project/jsonld/shareyourcloning_linkml.context.jsonld
+-rw-r--r--   0        0        0    82662 2024-05-08 16:47:39.669000 shareyourcloning_linkml-0.1.5a0/project/jsonld/shareyourcloning_linkml.jsonld
+-rw-r--r--   0        0        0    42020 2024-05-08 16:47:39.669000 shareyourcloning_linkml-0.1.5a0/project/jsonschema/shareyourcloning_linkml.schema.json
+-rw-r--r--   0        0        0    54517 2024-05-08 16:47:39.669000 shareyourcloning_linkml-0.1.5a0/project/owl/shareyourcloning_linkml.owl.ttl
+-rw-r--r--   0        0        0      400 2024-05-08 16:47:39.669000 shareyourcloning_linkml-0.1.5a0/project/prefixmap/shareyourcloning_linkml.yaml
+-rw-r--r--   0        0        0     6097 2024-05-08 16:47:39.669000 shareyourcloning_linkml-0.1.5a0/project/protobuf/shareyourcloning_linkml.proto
+-rw-r--r--   0        0        0    64643 2024-05-08 16:47:39.669000 shareyourcloning_linkml-0.1.5a0/project/python/shareyourcloning_linkml.py
+-rw-r--r--   0        0        0    44003 2024-05-08 16:47:39.669000 shareyourcloning_linkml-0.1.5a0/project/shacl/shareyourcloning_linkml.shacl.ttl
+-rw-r--r--   0        0        0     9599 2024-05-08 16:47:39.669000 shareyourcloning_linkml-0.1.5a0/project/shex/shareyourcloning_linkml.shex
+-rw-r--r--   0        0        0    30242 2024-05-08 16:47:39.669000 shareyourcloning_linkml-0.1.5a0/project/sqlschema/shareyourcloning_linkml.sql
+-rw-r--r--   0        0        0     1499 2024-05-08 16:47:52.165159 shareyourcloning_linkml-0.1.5a0/pyproject.toml
+-rw-r--r--   0        0        0      186 2024-05-08 16:47:39.669000 shareyourcloning_linkml-0.1.5a0/src/shareyourcloning_linkml/_version.py
+-rw-r--r--   0        0        0       41 2024-05-08 16:47:39.669000 shareyourcloning_linkml-0.1.5a0/src/shareyourcloning_linkml/datamodel/__init__.py
+-rw-r--r--   0        0        0    25928 2024-05-08 16:47:39.669000 shareyourcloning_linkml-0.1.5a0/src/shareyourcloning_linkml/datamodel/_models.py
+-rw-r--r--   0        0        0       42 2024-05-08 16:47:39.669000 shareyourcloning_linkml-0.1.5a0/src/shareyourcloning_linkml/datamodel/models.py
+-rw-r--r--   0        0        0    15636 2024-05-08 16:47:39.669000 shareyourcloning_linkml-0.1.5a0/src/shareyourcloning_linkml/schema/shareyourcloning_linkml.yaml
+-rw-r--r--   0        0        0     1877 1970-01-01 00:00:00.000000 shareyourcloning_linkml-0.1.5a0/PKG-INFO
```

### Comparing `shareyourcloning_linkml-0.1.4a0/LICENSE` & `shareyourcloning_linkml-0.1.5a0/LICENSE`

 * *Files identical despite different names*

### Comparing `shareyourcloning_linkml-0.1.4a0/README.md` & `shareyourcloning_linkml-0.1.5a0/README.md`

 * *Files identical despite different names*

### Comparing `shareyourcloning_linkml-0.1.4a0/project/excel/shareyourcloning_linkml.xlsx` & `shareyourcloning_linkml-0.1.5a0/project/excel/shareyourcloning_linkml.xlsx`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-00000000: 504b 0304 1400 0000 0800 d263 a858 465a  PK.........c.XFZ
+00000000: 504b 0304 1400 0000 0800 c68c a858 465a  PK...........XFZ
 00000010: c10c 8200 0000 b100 0000 1000 0000 646f  ..............do
 00000020: 6350 726f 7073 2f61 7070 2e78 6d6c 4d8e  cProps/app.xmlM.
 00000030: 4d0b c230 1044 ff4a e9dd 6e55 f020 3120  M..0.D.J..nU. 1 
 00000040: d4a3 e0c9 7b48 3736 9064 4376 85fc 7c53  ....{H76.dCv..|S
 00000050: c18f db3c de30 8cba 15ca 58c4 2377 3586  ...<.0....X.#w5.
 00000060: c4a7 7e11 c947 00b6 0b46 c343 d3a9 1947  ..~..G...F.C...G
 00000070: 251a 6958 1e40 ce79 8b13 d967 c424 b01b  %.iX.@.y...g.$..
 00000080: c703 6015 4c33 ce9b fc1d ecb5 3ae7 1cbc  ..`.L3......:...
 00000090: 35e2 29e9 abb7 8598 9c74 976a 3128 f897  5.)......t.j1(..
 000000a0: 6bf3 8e85 d7bc 1fb6 6ff9 6105 bf93 fa05  k.......o.a.....
-000000b0: 504b 0304 1400 0000 0800 d263 a858 9d88  PK.........c.X..
-000000c0: 5136 ee00 0000 cb01 0000 1100 0000 646f  Q6............do
+000000b0: 504b 0304 1400 0000 0800 c68c a858 f8af  PK...........X..
+000000c0: d4c1 ee00 0000 cb01 0000 1100 0000 646f  ..............do
 000000d0: 6350 726f 7073 2f63 6f72 652e 786d 6c95  cProps/core.xml.
-000000e0: 91c1 4ec3 300c 865f 65ea bd75 d26e 80a2  ..N.0.._e..u.n..
-000000f0: ac17 d04e 2021 3109 c42d 4abc 2da2 69a3  ...N !1..-J.-.i.
-00000100: c4a8 dddb 9396 ad1b 820b c7f8 fffc d956  ...............V
-00000110: a4f6 4277 019f 43e7 3190 c5b8 185c d346  ..Bw..C.1....\.F
-00000120: a1fd 3a3b 1079 0110 f501 9d8a 4522 da14  ..:;.y......E"..
-00000130: eeba e014 a567 d883 57fa 43ed 114a c66e  .....g..W.C..J.n
-00000140: c021 29a3 48c1 28cc fd6c cc4e 4aa3 67a5  .!).H.(..l.NJ.g.
-00000150: ff0c cd24 301a b041 872d 45e0 0587 0b4b  ...$0..A.-E....K
-00000160: 185c fcb3 614a 6672 8876 a6fa be2f fa6a  .\..aJfr.v.../.j
-00000170: e2d2 461c de9e 1e5f a6e5 73db 4652 adc6  ..F...._..s.FR..
-00000180: ac96 460b 1d50 5117 eaf1 227f 1c1a 0957  ..F..PQ..."....W
-00000190: 4579 9afd 5d40 b348 1304 1d3d aeb3 73f2  Ey..]@.H...=..s.
-000001a0: 5add 3f6c 3759 5db2 7299 b355 ceee b69c  Z.?l7Y].r..U....
-000001b0: 8b8a 896a f53e ba7e f45f 84ae 3376 67ff  ...j.>.~._..3vg.
-000001c0: 69bc bd32 9e05 b584 5fff 567f 0150 4b03  i..2...._.V..PK.
-000001d0: 0414 0000 0008 00d2 63a8 5899 5c9c 2310  ........c.X.\.#.
+000000e0: 91c1 4ec3 300c 865f 65ca bd75 d3c2 3445  ..N.0.._e..u..4E
+000000f0: 592f 4c3b 8184 c424 10b7 28f1 b688 268d  Y/L;...$..(...&.
+00000100: 12a3 766f 4f5b b66e 082e 1ce3 fff3 675b  ..voO[.n......g[
+00000110: 913a 08dd 467c 8e6d c048 16d3 a277 8d4f  .:..F|.m.H...w.O
+00000120: 4287 353b 1205 0190 f411 9d4a f940 f821  B.5;.......J.@.!
+00000130: dcb7 d129 1a9e f100 41e9 0f75 4028 8b62  ...)....A..u@(.b
+00000140: 090e 4919 450a 4661 1666 233b 2b8d 9e95  ..I.E.Fa.f#;+...
+00000150: e133 3693 c068 c006 1d7a 4ac0 730e 5796  .36..h...zJ.s.W.
+00000160: 30ba f467 c394 cc64 9fec 4c75 5d97 77d5  0..g...d..Lu].w.
+00000170: c40d 1b71 787b 7a7c 9996 cfac 4fa4 bc46  ...qx{z|....O..F
+00000180: 564b a385 8ea8 a88d f578 5138 f58d 849b  VK.......xQ8....
+00000190: a23c cffe 2ea0 590c 1304 9d02 aed9 2579  .<....Y.......%y
+000001a0: ad1e 36bb 2dab cba2 bccb 8afb ac58 edf8  ..6.-........X..
+000001b0: 5254 2bc1 f9fb e8fa d17f 15ba d6d8 bdfd  RT+.............
+000001c0: a7b1 ba31 5e04 b584 5fff 567f 0150 4b03  ...1^..._.V..PK.
+000001d0: 0414 0000 0008 00c6 8ca8 5899 5c9c 2310  ..........X.\.#.
 000001e0: 0600 009c 2700 0013 0000 0078 6c2f 7468  ....'......xl/th
 000001f0: 656d 652f 7468 656d 6531 2e78 6d6c ed5a  eme/theme1.xml.Z
 00000200: 5b73 da38 147e efaf d078 67f6 6d0b c636  [s.8.~...xg.m..6
 00000210: 81b6 b413 7369 76db b499 84ed 4e1f 8511  ....siv.....N...
 00000220: 588d 6c79 6491 847f bf47 3610 cb96 0ded  X.lyd....G6.....
 00000230: 924d ba9b 3c04 2ce9 fbce 4547 e7e8 3879  .M..<.,...EG..8y
 00000240: f3ee 2e62 e886 8894 f278 60d9 2fdb d6bb  ...b.....x`./...
@@ -123,15 +123,15 @@
 000007a0: 4ff9 259c 3bb4 7bf1 8120 9bfc d6db a4f6  O.%.;.{.. ......
 000007b0: dde0 0c7c d4ab 5aa5 642b 113f 4b07 7c1f  ...|..Z.d+.?K.|.
 000007c0: 9206 638c 5bf4 345f 8f14 62ad a6b1 adc6  ..c.[.4_..b.....
 000007d0: da31 0c79 8058 f30c a166 38df 8745 9a1a  .1.y.X...f8..E..
 000007e0: 33d5 8bac 398d 0a6f 41d5 40e5 3fdb d40d  3...9..oA.@.?...
 000007f0: 68f6 0d34 1c91 055e 3199 b636 a3e4 4e0a  h..4...^1..6..N.
 00000800: 3cdc feef 0db0 c2c4 8ee1 ed8b bf01 504b  <.............PK
-00000810: 0304 1400 0000 0800 d263 a858 bbe8 8b38  .........c.X...8
+00000810: 0304 1400 0000 0800 c68c a858 bbe8 8b38  ...........X...8
 00000820: 3801 0000 1102 0000 1800 0000 786c 2f77  8...........xl/w
 00000830: 6f72 6b73 6865 6574 732f 7368 6565 7431  orksheets/sheet1
 00000840: 2e78 6d6c 4d52 db6e 8330 0cfd 9528 1fd0  .xmlMR.n.0...(..
 00000850: d049 bba8 02a4 b6d3 b43d 4caa 5a6d 7b4e  .I.......=L.Zm{N
 00000860: c140 d424 6689 3bb6 bf9f 03bd 3d44 f838  .@.$f.;.....=D.8
 00000870: 3ee7 d826 f980 e110 3b00 12bf cefa 58c8  >..&....;.....X.
 00000880: 8ea8 5f28 15ab 0e9c 8e33 ecc1 f34d 83c1  .._(.....3...M..
@@ -146,15 +146,15 @@
 00000910: 618d f6cb d4d4 15f2 498a 1a1a 7db4 b4c5  a.......I...}...
 00000920: e115 4e33 dd5f 5b7c d6a4 cb3c e020 421a  ..N3._[|...<. B.
 00000930: b6cc ab14 244b 2e34 3e2d 6947 81f3 869d  ....$K.4>-iG....
 00000940: a834 75ae 88fd 1352 151f 669e db99 a4d2  .4u....R..f.....
 00000950: aade 7568 8d8f c242 c32a d9ec 910d c3e4  ..uh...B.*......
 00000960: 3d01 c27e 5ced 1e89 d08d 61c7 bf0c 422a  =..~\.....a...B*
 00000970: e0fb 0691 2e20 cd7e 7905 e53f 504b 0304  ..... .~y..?PK..
-00000980: 1400 0000 0800 d263 a858 0712 deaa ee01  .......c.X......
+00000980: 1400 0000 0800 c68c a858 0712 deaa ee01  .........X......
 00000990: 0000 2104 0000 1800 0000 786c 2f77 6f72  ..!.......xl/wor
 000009a0: 6b73 6865 6574 732f 7368 6565 7432 2e78  ksheets/sheet2.x
 000009b0: 6d6c 8554 db6e db30 0cfd 1543 cf45 95f4  ml.T.n.0...C.E..
 000009c0: 8ec0 36d0 240d d687 0245 8b75 8f81 62d3  ..6.$....E.u..b.
 000009d0: b610 5974 25ba 5eff 7e94 9db8 e996 602f  ..Yt%.^.~.....`/
 000009e0: 1649 9187 8717 39ee d06d 7d05 40d1 efda  .I....9..m}.@...
 000009f0: 589f 888a a899 49e9 b30a 6ae5 cfb1 01cb  X.....I...j.....
@@ -180,15 +180,15 @@
 00000b30: a4de f068 9b96 9ec0 7b5e d8d1 f8e0 1cba  ...h....{^......
 00000b40: 43a3 32bc ec73 a3ec b65f f0c0 3511 467b  C.2..s..._..5.F{
 00000b50: e2cc 61a6 ad51 d354 14ca 933a 2bc1 6ed8  ..a..Q.T...:+.n.
 00000b60: f1cc 5bd5 b00c 2296 a34b 2cbf f3fc c7e0  ..[..."..K,.....
 00000b70: 87a7 f3a4 5ca9 b940 0305 d737 39bf e505  ....\..@...79...
 00000b80: 74c3 2e0e 0a61 d333 d920 11d6 bd58 f113  t....a.3. ...X..
 00000b90: 0617 1cf8 be40 a451 096f 61fc 2ba4 7f00  .....@.Q.oa.+...
-00000ba0: 504b 0304 1400 0000 0800 d263 a858 a497  PK.........c.X..
+00000ba0: 504b 0304 1400 0000 0800 c68c a858 a497  PK...........X..
 00000bb0: 6e89 5601 0000 a502 0000 1800 0000 786c  n.V...........xl
 00000bc0: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
 00000bd0: 7433 2e78 6d6c 7552 db6e c230 0cfd 952a  t3.xmluR.n.0...*
 00000be0: 1f40 60d2 2e42 6da5 019a b687 4908 b4ed  .@`..Bm.....I...
 00000bf0: 39b4 2e8d 48e2 92b8 ebf8 fb39 2d97 6982  9...H......9-.i.
 00000c00: a7d8 ce39 c73e 4ed2 0efd 2ed4 0094 fc58  ...9.>N........X
 00000c10: e342 266a a266 2a65 286a b02a 8cb0 01c7  .B&j.f*e(j.*....
@@ -205,15 +205,15 @@
 00000cc0: 6397 f868 364f 8b18 c496 0cd4 2e2e 694d  c..h6O........iM
 00000cd0: 9eeb 9a3b 51ee 9485 5412 4f10 7359 1cf1  ...;Q...T.O.sY..
 00000ce0: b35b f800 fb16 5c71 8d33 bfc5 d1e5 15f4  .[....\q.3......
 00000cf0: e216 9a0e cd3f 75c9 6e4e 2b1a ecc5 e77b  .....?u.nN+....{
 00000d00: 577e ab5d 480c 54ac 331e 3df2 12fc b08f  W~.]H.T.3.=.....
 00000d10: 2121 6cfa e7de 2011 da3e acf9 1b81 8f00  !!l... ..>......
 00000d20: beaf 10e9 9cc4 f738 ffcc fc17 504b 0304  .......8....PK..
-00000d30: 1400 0000 0800 d263 a858 32c0 66ed 4c01  .......c.X2.f.L.
+00000d30: 1400 0000 0800 c68c a858 32c0 66ed 4c01  .........X2.f.L.
 00000d40: 0000 4d02 0000 1800 0000 786c 2f77 6f72  ..M.......xl/wor
 00000d50: 6b73 6865 6574 732f 7368 6565 7434 2e78  ksheets/sheet4.x
 00000d60: 6d6c 7552 db4e c330 0cfd 952a 1f40 3a24  mluR.N.0...*.@:$
 00000d70: 2e9a da4a 6c08 c103 d2b4 0978 4459 ebb6  ...Jl......xDY..
 00000d80: d192 b824 ee0a 7f8f d3ee c603 4fb1 4f7c  ...$........O.O|
 00000d90: 8e8f 9d64 03fa 5d68 0128 f9b6 c685 5cb4  ...d..]h.(....\.
 00000da0: 44dd 5cca 50b6 6055 b8c2 0e1c dfd4 e8ad  D.\.P.`U........
@@ -229,15 +229,15 @@
 00000e40: 6738 cc74 73b6 f8a8 4815 99c7 21f1 71d8  g8.ts...H...!.q.
 00000e50: 222b 6310 5b72 a176 7149 1bf2 8c6b ee44  "+c.[r.vqI...k.D
 00000e60: 45d9 d3e7 c07b 4697 4962 1f11 95e5 81b5  E....{F.Ib......
 00000e70: f88f 857b f0ad 72cd 5f8e e4ae c751 261b  ...{..r._....Q&.
 00000e80: 71cd afca 37da 85c4 40cd 5ae9 d51d 9bf5  q...7...@.Z.....
 00000e90: 93ef 2921 ecc6 67d9 2211 da31 6cf9 b9c1  ..)!..g."..1l...
 00000ea0: c702 beaf 11e9 94c4 bd9d 7e50 f10b 504b  ..........~P..PK
-00000eb0: 0304 1400 0000 0800 d263 a858 0840 26f8  .........c.X.@&.
+00000eb0: 0304 1400 0000 0800 c68c a858 0840 26f8  ...........X.@&.
 00000ec0: 5c01 0000 8b02 0000 1800 0000 786c 2f77  \...........xl/w
 00000ed0: 6f72 6b73 6865 6574 732f 7368 6565 7435  orksheets/sheet5
 00000ee0: 2e78 6d6c 7552 db4e c330 0cfd 952a 1f40  .xmluR.N.0...*.@
 00000ef0: 3624 2e42 6d25 3684 e001 6902 018f 286b  6$.Bm%6...i...(k
 00000f00: dd36 5a12 17c7 a38c afc7 e96e 20c1 537c  .6Z........n .S|
 00000f10: 3bf6 3976 f201 6915 3b00 ce3e bd0b b150  ;.9v..i.;..>...P
 00000f20: 1d73 7fa5 75ac 3af0 269e 600f 4132 0d92  .s..u.:.&.`.A2..
@@ -254,15 +254,15 @@
 00000fd0: 24b6 ccab 64a4 9152 6843 5ad2 1393 c4ad  $...d..RhCZ.....
 00000fe0: 4ce2 9220 32d9 91ee 1b84 af8d 875c b3f0  L.. 2........\..
 00000ff0: 4959 5ded d0b3 ffd0 d59a df06 b912 863f  IY]............?
 00001000: 50f3 ff50 f801 d499 d0fe c668 e1bc 5fc4  P..P.......h.._.
 00001010: 5644 3ad2 83a1 d686 9839 68a4 d7e4 e442  VD:......9h....B
 00001020: a4d2 56f5 d661 ecc7 a32e 9119 fd68 76f2  ..V..a.......hv.
 00001030: 5980 5281 e41b 443e 3869 eb87 ff57 7e03  Y.R...D>8i...W~.
-00001040: 504b 0304 1400 0000 0800 d263 a858 4ec7  PK.........c.XN.
+00001040: 504b 0304 1400 0000 0800 c68c a858 4ec7  PK...........XN.
 00001050: 5d80 8a01 0000 9103 0000 1800 0000 786c  ].............xl
 00001060: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
 00001070: 7436 2e78 6d6c 8553 6d4f dc30 0cfe 2b55  t6.xml.SmO.0..+U
 00001080: 7e00 3986 3626 d456 8263 ecf6 6112 026d  ~.9.6&.V.c..a..m
 00001090: 7c3c e55a b78d 2e8d 83e3 d2f1 efe7 f45e  |<.Z...........^
 000010a0: 00e9 2a3e c576 fc3c 7e1c 3bf9 88b4 8d1d  ..*>.v.<~.;.....
 000010b0: 0067 ff7a e763 a13a e670 a575 ac3a e84d  .g.z.c.:.p.u.:.M
@@ -282,15 +282,15 @@
 00001190: 6a4f 70f3 29c1 28d3 423f cfb0 9c63 1822  jOp.).(.B?...c."
 000011a0: d0da fa30 f009 d4ed 1caa b254 0dce d009  ...0.......T....
 000011b0: cc8f 39cc 5c91 bbd9 e606 3e8d f839 87e0  ..9.\.....>..9..
 000011c0: d770 aaf9 d5ac a4fa 63b6 96c9 1dd6 6137  .p......c.....a7
 000011d0: cab4 aabf 0db5 d6c7 cc41 232c 8bb3 4b19  .........A#,..K.
 000011e0: 38ed 66bf 7318 c3b4 da1b 64c6 7e32 3bf9  8.f.s.....d.~2;.
 000011f0: 3240 2941 ee1b 443e 3a69 f78e bfb0 fc0f  2@)A..D>:i......
-00001200: 504b 0304 1400 0000 0800 d263 a858 4409  PK.........c.XD.
+00001200: 504b 0304 1400 0000 0800 c68c a858 4409  PK...........XD.
 00001210: 9006 e701 0000 3704 0000 1800 0000 786c  ......7.......xl
 00001220: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
 00001230: 7437 2e78 6d6c 7554 4d6f a330 10fd 2bc8  t7.xmluTMo.0..+.
 00001240: e7aa 26d5 f643 1120 3549 dbed a152 d56a  ..&..C. 5I...R.j
 00001250: db63 e5c0 0056 8c4d ed61 69ff fd8e 4d42  .c...V.M.ai...MB
 00001260: 132d 5cf0 cc78 decc 1bfb 99a4 3776 e76a  .-\..x......7v.j
 00001270: 008c be1a a55d ca6a c476 c9b9 cb6b 6884  .....].j.v...kh.
@@ -316,15 +316,15 @@
 000013b0: f0e8 cfe1 099c 2319 8fc1 3b6b 8d3d 0e0a  ......#...;k.=..
 000013c0: 454f 60a5 84de 05d9 fbc9 52a6 a443 eaec  EO`.......R..C..
 000013d0: 6fba 5362 91b1 5238 1467 15e8 2d25 9e39  o.Sb..R8.g..-%.9
 000013e0: 2d5a b281 257c 4c49 f829 cfff 026e 7850  -Z..%|LI.)...nxP
 000013f0: 4fc2 5692 0654 50d2 7cf1 f935 c9d2 0e0a  O.V..TP.|..5....
 00001400: 1d1c 346d 60b2 3588 a609 664d 0f1b ac4f  ..4m`.5...fM...O
 00001410: a0fd d218 1c1d ff42 c67f 45f6 0f50 4b03  .......B..E..PK.
-00001420: 0414 0000 0008 00d2 63a8 5891 c100 8bd2  ........c.X.....
+00001420: 0414 0000 0008 00c6 8ca8 5891 c100 8bd2  ..........X.....
 00001430: 0100 00f6 0300 0018 0000 0078 6c2f 776f  ...........xl/wo
 00001440: 726b 7368 6565 7473 2f73 6865 6574 382e  rksheets/sheet8.
 00001450: 786d 6c8d 53db 6edb 300c fd15 43cf 43e5  xml.S.n.0...C.C.
 00001460: 14bd 21b0 0d34 4983 f5a1 40d1 62ed e3a0  ..!..4I...@.b...
 00001470: d8b4 2d44 165d 899e 97bf 1f65 276e ba25  ..-D.].....e'n.%
 00001480: c05e 24de 0ec5 4352 498f 6eeb 6b00 8a7e  .^$...CRI.n.k..~
 00001490: 37c6 fa54 d444 ed5c 4a9f d7d0 287f 812d  7..T.D.\J...(..-
@@ -348,16 +348,16 @@
 000015b0: 8627 5f63 bf72 d8ae b0b7 614b 06c3 63e8  .'_c.r....aK..c.
 000015c0: c313 78cf cb38 191f 9c43 776c 5486 1779  ..x..8...CwlT..y
 000015d0: 6194 dd0e cb1b 98a5 c268 4ffc 72f8 249d  a........hO.r.$.
 000015e0: 51b3 4ca8 a2a8 c0c2 373e 361c 2a12 39f9  Q.L.....7>6.*.9.
 000015f0: 12f9 b5c0 7f0c 7efc 0f4f ca55 9a99 1928  ......~..O.U...(
 00001600: 9958 7c71 cb5b e5c6 051b 15c2 7628 6183  .X|q.[......v(a.
 00001610: 44d8 0c62 cdff 125c 0860 7f89 4893 1216  D..b...\.`..H...
-00001620: 7cfa ead9 1f50 4b03 0414 0000 0008 00d2  |....PK.........
-00001630: 63a8 58d3 d762 9c0b 0200 0031 0500 0018  c.X..b.....1....
+00001620: 7cfa ead9 1f50 4b03 0414 0000 0008 00c6  |....PK.........
+00001630: 8ca8 58d3 d762 9c0b 0200 0031 0500 0018  ..X..b.....1....
 00001640: 0000 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
 00001650: 2f73 6865 6574 392e 786d 6cbd 544d 6fdb  /sheet9.xml.TMo.
 00001660: 300c fd2b 86ce 5d95 04eb 0702 dbc0 92b4  0..+..].........
 00001670: 4b0f 058a 16ed 8e81 62d3 b110 5974 257a  K.......b...Yt%z
 00001680: 5eff fd28 2771 b320 1e76 dac5 1629 bea7  ^..('q. .v...)..
 00001690: 4791 54dc a2db fa12 80a2 5f95 b13e 1125  G.T......._..>.%
 000016a0: 513d 95d2 6725 54ca 5f62 0d96 770a 7495  Q=..g%T._b..w.t.
@@ -385,15 +385,15 @@
 00001800: 4266 8930 da13 9f1c 46b4 316a 9c8a fc50  Bf.0....F.1j...P
 00001810: 8c2f 4563 ccc5 be2f 3a43 c4b2 8f8b e59f  ./Ec.../:C......
 00001820: 6287 c4cf 27d3 f9ff 13bf 577b c19f 3587  b...'.....W{..5.
 00001830: fe5d f089 c3ef 9e92 47e5 369a cb62 a0e0  .]......G.6..b..
 00001840: aa8c 2e6f 7820 dd6e 3677 0661 dd49 5823  ...ox .n6w.a.IX#
 00001850: 1156 ddb2 e427 0d5c 08e0 fd02 917a 23bc  .V...'.\.....z#.
 00001860: 0dfd 2b99 fe06 504b 0304 1400 0000 0800  ..+...PK........
-00001870: d263 a858 1a82 8f86 9c01 0000 1a04 0000  .c.X............
+00001870: c68c a858 1a82 8f86 9c01 0000 1a04 0000  ...X............
 00001880: 1900 0000 786c 2f77 6f72 6b73 6865 6574  ....xl/worksheet
 00001890: 732f 7368 6565 7431 302e 786d 6c7d 94db  s/sheet10.xml}..
 000018a0: 4ee4 300c 865f a5ca 0390 0109 58a1 b6d2  N.0.._......X...
 000018b0: 321c 1721 2110 bb97 a34c ebb6 1149 5c12  2..!!....L...I\.
 000018c0: 97ee bcfd 3a9d 0368 d570 35b6 e3ef cfef  ....:..h.p5.....
 000018d0: ca99 7c44 ff16 3a00 cafe 5ae3 4221 3aa2  ..|D..:...Z.B!:.
 000018e0: fe42 ca50 7560 5538 c21e 1c9f 34e8 ad22  .B.Pu`U8....4.."
@@ -414,15 +414,15 @@
 000019d0: ac74 3d83 5c27 5d92 f234 03dc a400 7073  .t=.\']..4....ps
 000019e0: fab7 697d af66 89bb 14a1 5d3f cc39 ba4f  ..i}.f....]?.9.O
 000019f0: 01bc def3 c4af 1441 9b1e 66fa 1f92 96fe  .......A..f.....
 00001a00: 1b40 f20a edf7 72bb 53f1 cd3c 2adf 6a17  .@....r.S..<*.j.
 00001a10: 3203 0dab 2c8e ce79 f3fc 7609 b709 613f  2...,..y..v...a?
 00001a20: bdb1 3512 a19d c28e df2e f8d8 c0e7 0d22  ..5............"
 00001a30: 1d92 f808 0e7f 07e5 3f50 4b03 0414 0000  ........?PK.....
-00001a40: 0008 00d2 63a8 5882 b2f4 9d67 0100 000f  ....c.X....g....
+00001a40: 0008 00c6 8ca8 5882 b2f4 9d67 0100 000f  ......X....g....
 00001a50: 0300 0019 0000 0078 6c2f 776f 726b 7368  .......xl/worksh
 00001a60: 6565 7473 2f73 6865 6574 3131 2e78 6d6c  eets/sheet11.xml
 00001a70: 7553 db4e c330 0cfd 952a 1f40 3624 2e9a  uS.N.0...*.@6$..
 00001a80: da4a 6c63 8207 a469 13f0 88b2 d66d a3e5  .Jlc...i.....m..
 00001a90: 46e2 51f6 f738 ed6e 48eb 536d c7c7 3e3e  F.Q..8.nH.Sm..>>
 00001aa0: 76d3 d6fa 6d68 0030 f9d5 ca84 8c35 886e  v...mh.0.....5.n
 00001ab0: c279 281a d022 dc58 0786 5e2a ebb5 4072  .y(..".X..^*..@r
@@ -440,15 +440,15 @@
 00001b70: e60a 2afc 82b2 8694 23d1 8841 5e1c 40d3  ..*.....#..A^.@.
 00001b80: 2190 8f6d 8750 b321 9434 6e87 5700 f321  !..m.P.!.4n.W..!
 00001b90: 00ed f43a e279 0881 7b77 8dd2 6290 52f9  ...:.y..{w..b.R.
 00001ba0: 3f9b 936e c765 f442 c643 7913 be96 2624  ?..n.e.B.Cy...&$
 00001bb0: 512b 5af1 cd03 c9ed 7be5 7b07 adeb 0e6b  Q+Z.....{.{....k
 00001bc0: 6311 adee cc86 0e16 7c4c a0f7 ca5a 3c39  c.......|L...Z<9
 00001bd0: 71f3 a77f 20ff 0350 4b03 0414 0000 0008  q... ..PK.......
-00001be0: 00d2 63a8 5882 b2f4 9d67 0100 000f 0300  ..c.X....g......
+00001be0: 00c6 8ca8 5882 b2f4 9d67 0100 000f 0300  ....X....g......
 00001bf0: 0019 0000 0078 6c2f 776f 726b 7368 6565  .....xl/workshee
 00001c00: 7473 2f73 6865 6574 3132 2e78 6d6c 7553  ts/sheet12.xmluS
 00001c10: db4e c330 0cfd 952a 1f40 3624 2e9a da4a  .N.0...*.@6$...J
 00001c20: 6c63 8207 a469 13f0 88b2 d66d a3e5 46e2  lc...i.....m..F.
 00001c30: 51f6 f738 ed6e 48eb 536d c7c7 3e3e 76d3  Q..8.nH.Sm..>>v.
 00001c40: d6fa 6d68 0030 f9d5 ca84 8c35 886e c279  ..mh.0.....5.n.y
 00001c50: 281a d022 dc58 0786 5e2a ebb5 4072 7dcd  (..".X..^*..@r}.
@@ -465,16 +465,16 @@
 00001d00: 8846 6c49 89d2 4491 d6e8 292e a913 e60a  .FlI..D...).....
 00001d10: 2afc 82b2 8694 23d1 8841 5e1c 40d3 2190  *.....#..A^.@.!.
 00001d20: 8f6d 8750 b321 9434 6e87 5700 f321 00ed  .m.P.!.4n.W..!..
 00001d30: f43a e279 0881 7b77 8dd2 6290 52f9 3f9b  .:.y..{w..b.R.?.
 00001d40: 936e c765 f442 c643 7913 be96 2624 512b  .n.e.B.Cy...&$Q+
 00001d50: 5af1 cd03 c9ed 7be5 7b07 adeb 0e6b 6311  Z.....{.{....kc.
 00001d60: adee cc86 0e16 7c4c a0f7 ca5a 3c39 71f3  ......|L...Z<9q.
-00001d70: a77f 20ff 0350 4b03 0414 0000 0008 00d2  .. ..PK.........
-00001d80: 63a8 58fb c712 8d4a 0100 0075 0200 0019  c.X....J...u....
+00001d70: a77f 20ff 0350 4b03 0414 0000 0008 00c6  .. ..PK.........
+00001d80: 8ca8 58fb c712 8d4a 0100 0075 0200 0019  ..X....J...u....
 00001d90: 0000 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
 00001da0: 2f73 6865 6574 3133 2e78 6d6c 7552 d94e  /sheet13.xmluR.N
 00001db0: c330 10fc 95c8 1f50 a748 1caa 9248 3408  .0.....P.H...H4.
 00001dc0: c103 52d5 0a78 7693 4d62 d5f6 067b 4be0  ..R..xv.Mb...{K.
 00001dd0: ef59 273d 10a2 4fde 6b66 676c 6703 fa5d  .Y'=..O.kfglg..]
 00001de0: e800 28f9 b2c6 855c 7444 fd42 ca50 7560  ..(....\tD.B.Pu`
 00001df0: 5598 610f 8e3b 0d7a ab88 53df cad0 7b50  U.a..;.z..S...{P
@@ -490,15 +490,15 @@
 00001e90: 4191 2a32 8f43 e2a3 d922 ab62 1057 f2a0  A.*2.C...".b.W..
 00001ea0: 76f1 9236 e4b9 ae79 1315 8194 a74c 124b  v..6...y.....L.K
 00001eb0: 8805 591d 00cb 4b00 70f5 3fe3 e565 7eaf  ..Y...K.p.?..e~.
 00001ec0: fe22 24ab 3b5a 9ee4 c6e7 7851 bed5 2e24  ."$.;Z....xQ...$
 00001ed0: 061a 664a 67b7 6cca 4ffe a684 b01f 9f6f  ..fJg.l.O......o
 00001ee0: 8b44 68c7 b0e3 6f01 3e0e 70bf 41a4 5312  .Dh...o.>.p.A.S.
 00001ef0: eff7 f4d3 8a1f 504b 0304 1400 0000 0800  ......PK........
-00001f00: d263 a858 f666 8318 5c01 0000 8b02 0000  .c.X.f..\.......
+00001f00: c68c a858 f666 8318 5c01 0000 8b02 0000  ...X.f..\.......
 00001f10: 1900 0000 786c 2f77 6f72 6b73 6865 6574  ....xl/worksheet
 00001f20: 732f 7368 6565 7431 342e 786d 6c75 52db  s/sheet14.xmluR.
 00001f30: 4ec3 300c fd95 2a1f b074 485c 34b5 95d8  N.0...*..tH\4...
 00001f40: 1082 07a4 6913 f088 b2d6 5da3 2571 97b8  ....i.....].%q..
 00001f50: 2bfc 3d4e 7745 624f b11d 9fe3 739c 643d  +.=NwEbO....s.d=
 00001f60: fa4d 6800 28f9 b6c6 855c 3444 ed44 ca50  .Mh.(....\4D.D.P
 00001f70: 3660 5518 610b 8e6f 6af4 5611 a77e 2d43  6`U.a..oj.V..~-C
@@ -515,15 +515,15 @@
 00002020: e446 ede2 9296 e4b9 ae79 1215 01b6 1db8  .F.......y......
 00002030: 1232 49ac 22d6 6479 c04c af61 0c96 2afa  .2I.".dy.L.a..*.
 00002040: fb07 33bb 86f1 b003 1fe0 ab44 db1a e01d  ..3........D....
 00002050: 1354 7ff1 9235 1f17 b137 111f e94d f9b5  .T...5...7...M..
 00002060: 7621 3150 336f 3aba 67ab 7eef 7a9f 10b6  v!1P3o:.g.~.z...
 00002070: c3a3 ae90 08ed 1036 fc59 c0c7 06be af11  .......6.Y......
 00002080: e994 c4ad 9ffe 5ff1 0b50 4b03 0414 0000  ......_..PK.....
-00002090: 0008 00d2 63a8 580c 5719 2b43 0100 0044  ....c.X.W.+C...D
+00002090: 0008 00c6 8ca8 580c 5719 2b43 0100 0044  ......X.W.+C...D
 000020a0: 0200 0019 0000 0078 6c2f 776f 726b 7368  .......xl/worksh
 000020b0: 6565 7473 2f73 6865 6574 3135 2e78 6d6c  eets/sheet15.xml
 000020c0: 7552 db4e c330 0cfd 952a 1fb0 6c48 5c34  uR.N.0...*..lH\4
 000020d0: b595 d810 8207 a469 13f0 9cad 6e1b 2d89  .......i....n.-.
 000020e0: 4be2 51f8 7bec 7617 78e0 293e 8e7d ceb1  K.Q.{.v.x.)>.}..
 000020f0: 93bc c7b8 4f2d 0065 5fde 8554 a896 a89b  ....O-.e_..T....
 00002100: 6b9d 762d 7893 26d8 41e0 9b1a a337 c430  k.v-x.&.A....7.0
@@ -538,15 +538,15 @@
 00002190: bddb 8ada 42dd a9ac 82da 1c1c adb1 7f82  ....B...........
 000021a0: e34c d717 8b0f 864c 9947 ecb3 28c3 96f9  .L.....L.G..(...
 000021b0: 4e02 91e4 421b 6449 1b8a 9cb7 ac44 a583  N...B.dI.....D..
 000021c0: 9a72 4dec 40b0 de1d eb17 ffd5 4751 fcdb  .rM.@.......GQ..
 000021d0: a059 ec34 c1a8 2edb 7d31 b1b1 2165 22c0  .Y.4....}1..!e".
 000021e0: 7b99 dcb2 c738 da1d 0161 37bc c616 89d0  {....8...a7.....
 000021f0: 0f61 cbaf 0c51 0af8 be46 a433 9075 9d3f  .a...Q...F.3.u.?
-00002200: 4ef9 0350 4b03 0414 0000 0008 00d2 63a8  N..PK.........c.
+00002200: 4ef9 0350 4b03 0414 0000 0008 00c6 8ca8  N..PK...........
 00002210: 5844 ff81 0869 0100 000c 0300 0019 0000  XD...i..........
 00002220: 0078 6c2f 776f 726b 7368 6565 7473 2f73  .xl/worksheets/s
 00002230: 6865 6574 3136 2e78 6d6c 7553 db6e 8330  heet16.xmluS.n.0
 00002240: 0cfd 1594 0f68 da49 bba8 02a4 b55d b53d  .....h.I.....].=
 00002250: 4caa 5a6d 7b0e 604a d45c 5862 c6fa f773  L.Zm{.`J.\Xb...s
 00002260: a0b7 49f0 84ed f81c 1f5f 885b eb0e be02  ..I......_.[....
 00002270: c0e8 572b e313 5621 d673 ce7d 5e81 167e  ..W+..V!.s.}^..~
@@ -564,15 +564,15 @@
 00002330: 69c2 9076 e828 2ea9 12a6 b974 79a3 848b  i..v.(.....ty...
 00002340: 3992 8a10 e3f9 09b3 18c3 08ef 4167 ea38  9...........Ag.8
 00002350: 8059 8e61 a4a9 1b1c 00ac c600 b4d0 61c4  .Y.a..........a.
 00002360: cb18 028f 350c e4af 4725 15ff b339 0ded  ....5...G%...9..
 00002370: bc89 7e8a e14a de85 db4b e323 0525 b14c  ..~..J...K.#.%.L
 00002380: 278f 346b d78f bd77 d0d6 dd55 6516 d1ea  '.4k...w...Ue...
 00002390: ceac e85a c185 047a 2fad c58b 13d6 7ef9  ...Z...z/.....~.
-000023a0: 01d2 3f50 4b03 0414 0000 0008 00d2 63a8  ..?PK.........c.
+000023a0: 01d2 3f50 4b03 0414 0000 0008 00c6 8ca8  ..?PK...........
 000023b0: 5811 26ee aa80 0100 0080 0300 0019 0000  X.&.............
 000023c0: 0078 6c2f 776f 726b 7368 6565 7473 2f73  .xl/worksheets/s
 000023d0: 6865 6574 3137 2e78 6d6c 7593 594f c330  heet17.xmlu.YO.0
 000023e0: 0c80 ff4a 951f 4006 1287 505b 898d 633c  ...J..@...P[..c<
 000023f0: 2021 10f0 88b2 d65d 2372 e1b8 94fd 7b9c   !.....]#r....{.
 00002400: ee00 a4f6 29b6 e3cf 47ec e4bd c78f d802  ....)...G.......
 00002410: 50f6 6d8d 8b85 6889 c2a5 94b1 6ac1 aa78  P.m...h.....j..x
@@ -592,15 +592,15 @@
 000024f0: 5f80 11a6 c9c5 1459 69ac 3aa3 c698 eb29  _......Yi.:....)
 00002500: 46c5 0876 6536 23cc cd14 a35d e868 04b8  F..ve6#....].h..
 00002510: 9d02 7889 c689 bb29 8236 0146 fc97 9325  ..x....).6.F...%
 00002520: d5ff bd25 0f6a 3ffd ede4 d266 3e28 5c6b  ...%.j?....f>(\k
 00002530: 1733 030d 4799 1d9d f37c 713b eaad 423e  .3..G....|q;..B>
 00002540: 0c9b bcf2 44de 0e62 cb3f 0430 39f0 7de3  ....D..b.?.09.}.
 00002550: 3d1d 94b4 6a87 4f57 fe00 504b 0304 1400  =...j.OW..PK....
-00002560: 0000 0800 d263 a858 44ff 8108 6901 0000  .....c.XD...i...
+00002560: 0000 0800 c68c a858 44ff 8108 6901 0000  .......XD...i...
 00002570: 0c03 0000 1900 0000 786c 2f77 6f72 6b73  ........xl/works
 00002580: 6865 6574 732f 7368 6565 7431 382e 786d  heets/sheet18.xm
 00002590: 6c75 53db 6e83 300c fd15 940f 68da 49bb  luS.n.0.....h.I.
 000025a0: a802 a4b5 5db5 3d4c aa5a 6d7b 0e60 4ad4  ....].=L.Zm{.`J.
 000025b0: 5c58 62c6 faf7 73a0 b749 f084 edf8 1c1f  \Xb...s..I......
 000025c0: 5f88 5beb 0ebe 02c0 e857 2be3 1356 21d6  _.[......W+..V!.
 000025d0: 73ce 7d5e 8116 7e62 6b30 f452 5aa7 0592  s.}^..~bk0.RZ...
@@ -618,15 +618,15 @@
 00002690: a6b9 7479 a384 8b39 928a 10e3 f909 b318  ..ty...9........
 000026a0: c308 ef41 67ea 3880 598e 61a4 a91b 1c00  ...Ag.8.Y.a.....
 000026b0: acc6 00b4 d061 c4cb 1802 8f35 0ce4 af47  .....a.....5...G
 000026c0: 2515 ffb3 390d edbc 897e 8ae1 4ade 85db  %...9....~..J...
 000026d0: 4be3 2305 25b1 4c27 8f34 6bd7 8fbd 77d0  K.#.%.L'.4k...w.
 000026e0: d6dd 5565 16d1 eace ace8 5ac1 8504 7a2f  ..Ue......Z...z/
 000026f0: adc5 8b13 d67e f901 d23f 504b 0304 1400  .....~...?PK....
-00002700: 0000 0800 d263 a858 44ff 8108 6901 0000  .....c.XD...i...
+00002700: 0000 0800 c68c a858 44ff 8108 6901 0000  .......XD...i...
 00002710: 0c03 0000 1900 0000 786c 2f77 6f72 6b73  ........xl/works
 00002720: 6865 6574 732f 7368 6565 7431 392e 786d  heets/sheet19.xm
 00002730: 6c75 53db 6e83 300c fd15 940f 68da 49bb  luS.n.0.....h.I.
 00002740: a802 a4b5 5db5 3d4c aa5a 6d7b 0e60 4ad4  ....].=L.Zm{.`J.
 00002750: 5c58 62c6 faf7 73a0 b749 f084 edf8 1c1f  \Xb...s..I......
 00002760: 5f88 5beb 0ebe 02c0 e857 2be3 1356 21d6  _.[......W+..V!.
 00002770: 73ce 7d5e 8116 7e62 6b30 f452 5aa7 0592  s.}^..~bk0.RZ...
@@ -644,15 +644,15 @@
 00002830: a6b9 7479 a384 8b39 928a 10e3 f909 b318  ..ty...9........
 00002840: c308 ef41 67ea 3880 598e 61a4 a91b 1c00  ...Ag.8.Y.a.....
 00002850: acc6 00b4 d061 c4cb 1802 8f35 0ce4 af47  .....a.....5...G
 00002860: 2515 ffb3 390d edbc 897e 8ae1 4ade 85db  %...9....~..J...
 00002870: 4be3 2305 25b1 4c27 8f34 6bd7 8fbd 77d0  K.#.%.L'.4k...w.
 00002880: d6dd 5565 16d1 eace ace8 5ac1 8504 7a2f  ..Ue......Z...z/
 00002890: adc5 8b13 d67e f901 d23f 504b 0304 1400  .....~...?PK....
-000028a0: 0000 0800 d263 a858 44ff 8108 6901 0000  .....c.XD...i...
+000028a0: 0000 0800 c68c a858 44ff 8108 6901 0000  .......XD...i...
 000028b0: 0c03 0000 1900 0000 786c 2f77 6f72 6b73  ........xl/works
 000028c0: 6865 6574 732f 7368 6565 7432 302e 786d  heets/sheet20.xm
 000028d0: 6c75 53db 6e83 300c fd15 940f 68da 49bb  luS.n.0.....h.I.
 000028e0: a802 a4b5 5db5 3d4c aa5a 6d7b 0e60 4ad4  ....].=L.Zm{.`J.
 000028f0: 5c58 62c6 faf7 73a0 b749 f084 edf8 1c1f  \Xb...s..I......
 00002900: 5f88 5beb 0ebe 02c0 e857 2be3 1356 21d6  _.[......W+..V!.
 00002910: 73ce 7d5e 8116 7e62 6b30 f452 5aa7 0592  s.}^..~bk0.RZ...
@@ -670,15 +670,15 @@
 000029d0: a6b9 7479 a384 8b39 928a 10e3 f909 b318  ..ty...9........
 000029e0: c308 ef41 67ea 3880 598e 61a4 a91b 1c00  ...Ag.8.Y.a.....
 000029f0: acc6 00b4 d061 c4cb 1802 8f35 0ce4 af47  .....a.....5...G
 00002a00: 2515 ffb3 390d edbc 897e 8ae1 4ade 85db  %...9....~..J...
 00002a10: 4be3 2305 25b1 4c27 8f34 6bd7 8fbd 77d0  K.#.%.L'.4k...w.
 00002a20: d6dd 5565 16d1 eace ace8 5ac1 8504 7a2f  ..Ue......Z...z/
 00002a30: adc5 8b13 d67e f901 d23f 504b 0304 1400  .....~...?PK....
-00002a40: 0000 0800 d263 a858 19ef 2f38 7b01 0000  .....c.X../8{...
+00002a40: 0000 0800 c68c a858 19ef 2f38 7b01 0000  .......X../8{...
 00002a50: 4b03 0000 1900 0000 786c 2f77 6f72 6b73  K.......xl/works
 00002a60: 6865 6574 732f 7368 6565 7432 312e 786d  heets/sheet21.xm
 00002a70: 6c75 93db 4ec3 300c 865f a5ca 0390 81c4  lu..N.0.._......
 00002a80: 41a8 adc4 364e 1748 6808 b844 59eb ae11  A...6N.Hh..DY...
 00002a90: 3914 c7a5 8ca7 c7e9 8e48 ed55 6dc7 9ff3  9........H.Um...
 00002aa0: 3b76 d3ce e367 a801 28f9 b1c6 854c d444  ;v...g..(....L.D
 00002ab0: cdb5 94a1 a8c1 aa70 e21b 707c 5279 b48a  .......p..p|Ry..
@@ -697,15 +697,15 @@
 00002b80: 0b8a c7b2 d8e2 d331 bcd0 58b4 46e1 0033  .......1..X.F..3
 00002b90: 1b63 5408 6097 663d c0cc c718 ed9a 9606  .cT.`.f=........
 00002ba0: 80db 3180 f761 98b8 1b23 68dd c040 fefd  ..1..a...#h..@..
 00002bb0: a8a4 f27f b6e4 37df 0d72 3384 b864 4f0a  ......7..r3..dO.
 00002bc0: 57da 85c4 40c5 5526 2797 3c2a dc4c 6de3  W...@.U&'.<*.Lm.
 00002bd0: 906f faa5 5c7a 226f 7bb3 e665 078c 097c  .o..\z"o{..e...|
 00002be0: 5e79 4f7b 276e cdfe ffc9 ff00 504b 0304  ^yO{'n......PK..
-00002bf0: 1400 0000 0800 d263 a858 caac fec0 7101  .......c.X....q.
+00002bf0: 1400 0000 0800 c68c a858 caac fec0 7101  .........X....q.
 00002c00: 0000 3e03 0000 1900 0000 786c 2f77 6f72  ..>.......xl/wor
 00002c10: 6b73 6865 6574 732f 7368 6565 7432 322e  ksheets/sheet22.
 00002c20: 786d 6c75 93db 6e83 300c 407f 05e5 039a  xmlu..n.0.@.....
 00002c30: 76d2 2eaa 0069 6dd7 6e0f 93aa 56db 9e53  v....im.n...V..S
 00002c40: 3010 3517 9698 b1fe fd1c 7a9d 044f d88e  0.5.......z..O..
 00002c50: 8fef c4ad 757b 5f01 60f4 ab95 f109 ab10  ....u{_.`.......
 00002c60: eb29 e73e ab40 0b3f b235 187a 29ac d302  .).>.@.?.5.z)...
@@ -723,15 +723,15 @@
 00002d20: 3261 5a36 3207 1f73 a41a 8285 6727 6236  2aZ62..s....g'b6
 00002d30: 4464 d265 8d12 ae87 990f 31c2 7bd0 3b75  Dd.e......1.{.;u
 00002d40: e861 1643 8c34 7583 3dc0 cb10 4027 d04f  .a.C.4u.=...@'.O
 00002d50: 2c87 083c d4d0 e3bf 1a2c 29ff efcd 69cc  ,..<.....,)...i.
 00002d60: e7dd 1de7 1eee ea5d b852 1a1f 2928 28ca  .......].R..)((.
 00002d70: 78f4 48db 71c7 451d 15b4 7577 873b 8b68  x.H.q.E...uw.;.h
 00002d80: 7527 5674 dfe0 8203 bd17 d6e2 4509 8772  u'Vt........E..r
-00002d90: f965 d23f 504b 0304 1400 0000 0800 d263  .e.?PK.........c
+00002d90: f965 d23f 504b 0304 1400 0000 0800 c68c  .e.?PK..........
 00002da0: a858 2513 3651 8301 0000 5703 0000 1900  .X%.6Q....W.....
 00002db0: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
 00002dc0: 7368 6565 7432 332e 786d 6c75 53db 6edb  sheet23.xmluS.n.
 00002dd0: 300c fd15 431f 50a5 1bba 0d85 6d60 4d2f  0...C.P.....m`M/
 00002de0: dbc3 80a2 c5b6 c740 b169 5b88 246a 145d  .......@.i[.$j.]
 00002df0: af7f 3fca b9b4 03e2 2793 14cf e1e1 c5e5  ..?.....'.......
 00002e00: 84b4 4b03 0017 7fbd 0ba9 5203 73bc d63a  ..K.......R.s..:
@@ -751,15 +751,15 @@
 00002ee0: 24e5 04dd 1c08 6e96 0864 4f93 a176 83ce  $.....n..dO..v..
 00002ef0: f678 06b8 5e02 1248 e904 8bc0 db25 a00d  .x..^..H.....%..
 00002f00: 71e4 3380 bbc5 1e47 3e8f b85f 42f0 6b3c  q.3....G>.._B.k<
 00002f10: 3784 8745 49ed ffd9 5ae6 7f5c ea7e 21f9  7..EI...Z..\.~!.
 00002f20: e07e 18ea 6d48 8583 4e58 5617 9f65 6db4  .~..mH..NXV..em.
 00002f30: dfe0 de61 8cf3 816e 9119 fd6c 0e72 f840  ...a...n...l.r.@
 00002f40: 3941 de3b 443e 39f9 824e ff52 fd0f 504b  9A.;D>9..N.R..PK
-00002f50: 0304 1400 0000 0800 d263 a858 a50c 764f  .........c.X..vO
+00002f50: 0304 1400 0000 0800 c68c a858 a50c 764f  ...........X..vO
 00002f60: 5301 0000 a402 0000 1900 0000 786c 2f77  S...........xl/w
 00002f70: 6f72 6b73 6865 6574 732f 7368 6565 7432  orksheets/sheet2
 00002f80: 342e 786d 6c75 52db 6ac3 300c fd95 e00f  4.xmluR.j.0.....
 00002f90: a8d3 c12e 9424 b0b6 8ced 6150 5ab6 3dbb  .....$....aPZ.=.
 00002fa0: 8992 98fa 365b 59d6 bf9f 9cf4 3668 9f2c  ....6[Y.....6h.,
 00002fb0: c93a 47e7 c8ce 7aeb 77a1 05c0 e457 2b13  .:G...z.w....W+.
 00002fc0: 72d6 22ba 19e7 a16c 418b 30b1 0e0c ddd4  r."....lA.0.....
@@ -776,15 +776,15 @@
 00003070: 3e9a 2db2 3206 7124 354a 1397 b441 4f75  >.-.2.q$5J...AOu
 00003080: 4993 b090 c675 9871 2409 b1c0 cb03 607e  I....u.q$.....`~
 00003090: 0b40 8bbe 8e58 dc42 e0de c195 fee5 4d49  .@...X.B......MI
 000030a0: d5ff 6e4e 668e 1b1a ddc5 d77b 17be 9126  ..nNf......{...&
 000030b0: 240a 6a62 4927 8fb4 033f ae63 4cd0 bae1  $.jbI'...?.cL...
 000030c0: b5b7 16d1 ea21 6ce9 1781 8f0d 745f 5b8b  .....!l.....t_[.
 000030d0: a724 3ec7 e963 167f 504b 0304 1400 0000  .$>..c..PK......
-000030e0: 0800 d263 a858 6517 5607 5c01 0000 b502  ...c.Xe.V.\.....
+000030e0: 0800 c68c a858 6517 5607 5c01 0000 b502  .....Xe.V.\.....
 000030f0: 0000 1900 0000 786c 2f77 6f72 6b73 6865  ......xl/workshe
 00003100: 6574 732f 7368 6565 7432 352e 786d 6c75  ets/sheet25.xmlu
 00003110: 52db 4ec3 300c fd95 2a1f b06c 485c 84da  R.N.0...*..lH\..
 00003120: 4ab0 09c1 03d2 0402 9eb3 d65d 2392 b873  J..........]#..s
 00003130: 5c0a 7f8f d35d 91d8 536c 27e7 d8e7 38f9  \....]..Sl'...8.
 00003140: 80f4 195b 00ce bebd 0bb1 502d 7377 ab75  ...[......P-sw.u
 00003150: ac5a f026 4eb0 8320 370d 9237 2c29 ad75  .Z.&N.. 7..7,).u
@@ -801,15 +801,15 @@
 00003200: 524b 7968 4332 e995 49ea 563a 7119 61d3  RKyhC2..I.V:q.a.
 00003210: 43a8 20e6 9a65 8c54 d4d5 0e74 7f16 843d  C. ..e.T...t...=
 00003220: fd0f 999f 8374 24c6 d27f 90c5 3948 0db1  .....t$.....9H..
 00003230: 22db 2527 ffc2 b4a8 db5b b695 9bd6 f96c  ".%'.....[.....l
 00003240: 686d 43cc 1c34 4237 9d5c 8b29 b4f5 679b  hmC..4B7.\.)..g.
 00003250: 3076 e3fa 57c8 8c7e 0c5b f956 40e9 81dc  0v..W..~.[.V@...
 00003260: 3788 7c48 d27e 0e3f b5fc 0550 4b03 0414  7.|H.~.?...PK...
-00003270: 0000 0008 00d2 63a8 58d2 05f1 4652 0200  ......c.X...FR..
+00003270: 0000 0008 00c6 8ca8 58d2 05f1 4652 0200  ........X...FR..
 00003280: 0047 0a00 000d 0000 0078 6c2f 7374 796c  .G.......xl/styl
 00003290: 6573 2e78 6d6c dd56 db8a db30 10fd 15e3  es.xml.V...0....
 000032a0: 0fa8 9398 9ab8 2479 a821 5068 cbc2 ee43  ......$y.!Ph...C
 000032b0: 5fe5 584e 04ba b8b2 bc24 fdfa 6a24 e7b6  _.XN.....$..j$..
 000032c0: 9be3 52fa 569b e099 393a 3367 a431 ceaa  ..R.V...9:3g.1..
 000032d0: 7727 c99f 0f9c bbe4 a8a4 eed7 e9c1 b9ee  w'..............
 000032e0: 5396 f5bb 0357 acff 603a ae3d d21a ab98  S....W..`:.=....
@@ -841,29 +841,29 @@
 00003480: 3031 367f 980d 78ca 9363 035b 9e18 51d8  016...x..c.[..Q.
 00003490: f2c4 ce13 04f6 9038 6509 0600 d622 0e3c  .......8e....".<
 000034a0: 1438 5124 02d4 a251 03ac 3ca7 7386 0ae1  .8Q$...Q..<.s...
 000034b0: 6b3e 0195 2584 6848 c1f4 1605 daa8 826e  k>..%.hH.......n
 000034c0: 705e f025 caf3 b204 1081 4046 9e43 885e  p^.%......@F.C.^
 000034d0: d809 08ca 2021 10ca f3f8 217d f33d cbce  .... !....!}.=..
 000034e0: dfb9 ecfa d771 f31b 504b 0304 1400 0000  .....q..PK......
-000034f0: 0800 d263 a858 b747 eb8a c000 0000 1602  ...c.X.G........
+000034f0: 0800 c68c a858 b747 eb8a c000 0000 1602  .....X.G........
 00003500: 0000 0b00 0000 5f72 656c 732f 2e72 656c  ......_rels/.rel
 00003510: 739d 924b 6e02 310c 40af 1265 5f4c a9c4  s..Kn.1.@..e_L..
 00003520: 0231 acd8 b043 880b b889 e7a3 99c4 9163  .1...C.........c
 00003530: c4f4 f68d d8c0 2068 114b ff9e 9e2d af0f  ...... h.K...-..
 00003540: 34a0 761c 73db a56c c630 c45c d956 35ad  4.v.s..l.0.\.V5.
 00003550: 00b2 6b29 609e 71a2 582a 354b 402d a134  ..k)`.q.X*5K@-.4
 00003560: 90d0 f5d8 102c e6f3 25c8 2dc3 6ed6 b74c  .....,..%.-.n..L
 00003570: 73fc 49f4 0a91 ebba 73b4 6577 0a14 f501  s.I.....s.ew....
 00003580: f8ae c39a 234a 435a d971 8033 4bff cddc  ....#JCZ.q.3K...
 00003590: cf0a d49a 9daf acec fca7 35f0 a6cc f3f5  ..........5.....
 000035a0: 2090 a247 4570 2cf4 91a4 4c8b 7694 af3e   ..GEp,...L.v..>
 000035b0: 9edd bea4 f3a5 6362 b478 dfe8 fff3 d0a8  ......cb.x......
 000035c0: 143d f9bf 9d30 a589 d2d7 4509 266f b0f9  .=...0....E.&o..
-000035d0: 0550 4b03 0414 0000 0008 00d2 63a8 58e7  .PK.........c.X.
+000035d0: 0550 4b03 0414 0000 0008 00c6 8ca8 58e7  .PK...........X.
 000035e0: f3f0 5ba5 0200 005f 0900 000f 0000 0078  ..[...._.......x
 000035f0: 6c2f 776f 726b 626f 6f6b 2e78 6d6c 8d96  l/workbook.xml..
 00003600: 6f6f 9b30 10c6 bf4a c407 1881 b6e9 1f35  oo.0...J.......5
 00003610: 952a dab5 99ba 350a 59df 1b7c 494e b57d  .*....5.Y..|IN.}
 00003620: cc36 6dc9 a79f 0165 6533 b1f6 26c4 67fb  .6m....ee3..&.g.
 00003630: c79d 791e dbd7 efa4 5f0b a2d7 c987 14ca  ..y....._.......
 00003640: 5ce9 79b4 b3b6 ba8a 6353 ee40 32f3 852a  \.y.....cS.@2..*
@@ -900,15 +900,15 @@
 00003830: 4f43 b648 7d5b 64ab 45be f4bf 461a dcf6  OC.H}[d.E...F...
 00003840: 7d0b 3c0b dcd2 6353 68e4 b83f 9259 c804  }.<...cSh..?.Y..
 00003850: a96f 8225 09e7 52cd 0cdc 7f58 5066 9419  .o.%..R....XPf..
 00003860: 3242 ea1b 2113 a4dc 3999 5bed e66c 9b21  2B..!...9.[..l.!
 00003870: 29e4 85b4 f742 7c38 7d39 6c50 016f 0f5e  )....B|8}9lP.o.^
 00003880: d376 b8bb 40e9 2e22 eda3 df3f 4ecf 5a41  .v..@.."...?N.ZA
 00003890: 6c6a 2132 177b 564f 6edb ff73 9c1f ee22  lj!2.{VOn..s..."
-000038a0: 37bf 0150 4b03 0414 0000 0008 00d2 63a8  7..PK.........c.
+000038a0: 37bf 0150 4b03 0414 0000 0008 00c6 8ca8  7..PK...........
 000038b0: 58f9 efd8 af3c 0100 00cd 0f00 001a 0000  X....<..........
 000038c0: 0078 6c2f 5f72 656c 732f 776f 726b 626f  .xl/_rels/workbo
 000038d0: 6f6b 2e78 6d6c 2e72 656c 73cd d741 8e82  ok.xml.rels..A..
 000038e0: 3014 c6f1 ab90 1ec0 f29e 8a3a 1157 6edc  0..........:.Wn.
 000038f0: 4ebc 4083 1588 4049 dbc9 e8ed 87c8 023f  N.@...@I.......?
 00003900: 328b d998 792b d212 1eff 4d7f 81fd a76d  2...y+....M....m
 00003910: 4cac 5d17 aaba 0fc9 bd6d ba90 ab2a c6fe  L.]......m...*..
@@ -924,15 +924,15 @@
 000039b0: 21dc 2441 6e42 ba49 82dd 8478 9304 bd09  !.$AnB.I...x....
 000039c0: f926 097e 1302 4e12 0427 249c 2418 4e88  .&.~..N..'$.$.N.
 000039d0: 3849 509c 9071 92e0 38a3 e32c c171 46c7  8IP..q..8..,.qF.
 000039e0: 5982 e33c fb00 97e0 38a3 e32c c171 46c7  Y..<....8..,.qF.
 000039f0: 5982 e38c 8ef3 5b1d 0ff1 d1d8 3005 8d6b  Y.....[.....0..k
 00003a00: 0c78 2bda 7178 d64e ef7f 2ec7 cdd9 b11a  .x+.qx.N........
 00003a10: 99d6 f0f7 7ef8 0150 4b03 0414 0000 0008  ....~..PK.......
-00003a20: 00d2 63a8 5872 079d 5874 0100 00bf 1000  ..c.Xr..Xt......
+00003a20: 00c6 8ca8 5872 079d 5874 0100 00bf 1000  ....Xr..Xt......
 00003a30: 0013 0000 005b 436f 6e74 656e 745f 5479  .....[Content_Ty
 00003a40: 7065 735d 2e78 6d6c cd98 cb6e c230 1045  pes].xml...n.0.E
 00003a50: 7f25 ca16 1163 b7a5 0f01 9bb6 db96 457f  .%...c........E.
 00003a60: c04d 26c4 c22f d986 c2df 7712 0a52 2bca  .M&../....w..R+.
 00003a70: 4354 ea6c 6225 9eb9 f7c6 231d 2919 bdad  CT.lb%....#.)...
 00003a80: 3dc4 6c65 b48d e3bc 49c9 3f30 16cb 068c  =.le....I.?0....
 00003a90: 8c85 f360 71a7 76c1 c884 b761 c6bc 2ce7  ...`q.v....a..,.
@@ -950,150 +950,150 @@
 00003b50: 1259 b75c 7ecc dfe7 bcd3 3f37 88a0 12e4  .Y.\~.....?7....
 00003b60: 8a4a 906b 2a41 6ea8 0419 5209 724b 25c8  .J.k*An...R.rK%.
 00003b70: 1d95 20f7 5482 f001 9924 64d8 cac9 c095  .. .T....$d.....
 00003b80: 93a1 2b27 8357 4e86 af9c 0c60 3919 c272  ..+'.WN....`9..r
 00003b90: 3288 e564 182b c830 5690 61ac 20c3 5841  2..d.+.0V.a. .XA
 00003ba0: 86b1 820c 63c5 bf32 f6dd b9f9 5f7f 4fb7  ....c..2...._.O.
 00003bb0: 6b61 a4b2 bb00 acfb 6f31 f904 504b 0102  ka......o1..PK..
-00003bc0: 1403 1400 0000 0800 d263 a858 465a c10c  .........c.XFZ..
+00003bc0: 1403 1400 0000 0800 c68c a858 465a c10c  ...........XFZ..
 00003bd0: 8200 0000 b100 0000 1000 0000 0000 0000  ................
 00003be0: 0000 0000 8001 0000 0000 646f 6350 726f  ..........docPro
 00003bf0: 7073 2f61 7070 2e78 6d6c 504b 0102 1403  ps/app.xmlPK....
-00003c00: 1400 0000 0800 d263 a858 9d88 5136 ee00  .......c.X..Q6..
+00003c00: 1400 0000 0800 c68c a858 f8af d4c1 ee00  .........X......
 00003c10: 0000 cb01 0000 1100 0000 0000 0000 0000  ................
 00003c20: 0000 8001 b000 0000 646f 6350 726f 7073  ........docProps
 00003c30: 2f63 6f72 652e 786d 6c50 4b01 0214 0314  /core.xmlPK.....
-00003c40: 0000 0008 00d2 63a8 5899 5c9c 2310 0600  ......c.X.\.#...
+00003c40: 0000 0008 00c6 8ca8 5899 5c9c 2310 0600  ........X.\.#...
 00003c50: 009c 2700 0013 0000 0000 0000 0000 0000  ..'.............
 00003c60: 0080 01cd 0100 0078 6c2f 7468 656d 652f  .......xl/theme/
 00003c70: 7468 656d 6531 2e78 6d6c 504b 0102 1403  theme1.xmlPK....
-00003c80: 1400 0000 0800 d263 a858 bbe8 8b38 3801  .......c.X...88.
+00003c80: 1400 0000 0800 c68c a858 bbe8 8b38 3801  .........X...88.
 00003c90: 0000 1102 0000 1800 0000 0000 0000 0000  ................
 00003ca0: 0000 8081 0e08 0000 786c 2f77 6f72 6b73  ........xl/works
 00003cb0: 6865 6574 732f 7368 6565 7431 2e78 6d6c  heets/sheet1.xml
-00003cc0: 504b 0102 1403 1400 0000 0800 d263 a858  PK...........c.X
+00003cc0: 504b 0102 1403 1400 0000 0800 c68c a858  PK.............X
 00003cd0: 0712 deaa ee01 0000 2104 0000 1800 0000  ........!.......
 00003ce0: 0000 0000 0000 0000 8081 7c09 0000 786c  ..........|...xl
 00003cf0: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
 00003d00: 7432 2e78 6d6c 504b 0102 1403 1400 0000  t2.xmlPK........
-00003d10: 0800 d263 a858 a497 6e89 5601 0000 a502  ...c.X..n.V.....
+00003d10: 0800 c68c a858 a497 6e89 5601 0000 a502  .....X..n.V.....
 00003d20: 0000 1800 0000 0000 0000 0000 0000 8081  ................
 00003d30: a00b 0000 786c 2f77 6f72 6b73 6865 6574  ....xl/worksheet
 00003d40: 732f 7368 6565 7433 2e78 6d6c 504b 0102  s/sheet3.xmlPK..
-00003d50: 1403 1400 0000 0800 d263 a858 32c0 66ed  .........c.X2.f.
+00003d50: 1403 1400 0000 0800 c68c a858 32c0 66ed  ...........X2.f.
 00003d60: 4c01 0000 4d02 0000 1800 0000 0000 0000  L...M...........
 00003d70: 0000 0000 8081 2c0d 0000 786c 2f77 6f72  ......,...xl/wor
 00003d80: 6b73 6865 6574 732f 7368 6565 7434 2e78  ksheets/sheet4.x
-00003d90: 6d6c 504b 0102 1403 1400 0000 0800 d263  mlPK...........c
+00003d90: 6d6c 504b 0102 1403 1400 0000 0800 c68c  mlPK............
 00003da0: a858 0840 26f8 5c01 0000 8b02 0000 1800  .X.@&.\.........
 00003db0: 0000 0000 0000 0000 0000 8081 ae0e 0000  ................
 00003dc0: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
 00003dd0: 6565 7435 2e78 6d6c 504b 0102 1403 1400  eet5.xmlPK......
-00003de0: 0000 0800 d263 a858 4ec7 5d80 8a01 0000  .....c.XN.].....
+00003de0: 0000 0800 c68c a858 4ec7 5d80 8a01 0000  .......XN.].....
 00003df0: 9103 0000 1800 0000 0000 0000 0000 0000  ................
 00003e00: 8081 4010 0000 786c 2f77 6f72 6b73 6865  ..@...xl/workshe
 00003e10: 6574 732f 7368 6565 7436 2e78 6d6c 504b  ets/sheet6.xmlPK
-00003e20: 0102 1403 1400 0000 0800 d263 a858 4409  ...........c.XD.
+00003e20: 0102 1403 1400 0000 0800 c68c a858 4409  .............XD.
 00003e30: 9006 e701 0000 3704 0000 1800 0000 0000  ......7.........
 00003e40: 0000 0000 0000 8081 0012 0000 786c 2f77  ............xl/w
 00003e50: 6f72 6b73 6865 6574 732f 7368 6565 7437  orksheets/sheet7
 00003e60: 2e78 6d6c 504b 0102 1403 1400 0000 0800  .xmlPK..........
-00003e70: d263 a858 91c1 008b d201 0000 f603 0000  .c.X............
+00003e70: c68c a858 91c1 008b d201 0000 f603 0000  ...X............
 00003e80: 1800 0000 0000 0000 0000 0000 8081 1d14  ................
 00003e90: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
 00003ea0: 7368 6565 7438 2e78 6d6c 504b 0102 1403  sheet8.xmlPK....
-00003eb0: 1400 0000 0800 d263 a858 d3d7 629c 0b02  .......c.X..b...
+00003eb0: 1400 0000 0800 c68c a858 d3d7 629c 0b02  .........X..b...
 00003ec0: 0000 3105 0000 1800 0000 0000 0000 0000  ..1.............
 00003ed0: 0000 8081 2516 0000 786c 2f77 6f72 6b73  ....%...xl/works
 00003ee0: 6865 6574 732f 7368 6565 7439 2e78 6d6c  heets/sheet9.xml
-00003ef0: 504b 0102 1403 1400 0000 0800 d263 a858  PK...........c.X
+00003ef0: 504b 0102 1403 1400 0000 0800 c68c a858  PK.............X
 00003f00: 1a82 8f86 9c01 0000 1a04 0000 1900 0000  ................
 00003f10: 0000 0000 0000 0000 8081 6618 0000 786c  ..........f...xl
 00003f20: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
 00003f30: 7431 302e 786d 6c50 4b01 0214 0314 0000  t10.xmlPK.......
-00003f40: 0008 00d2 63a8 5882 b2f4 9d67 0100 000f  ....c.X....g....
+00003f40: 0008 00c6 8ca8 5882 b2f4 9d67 0100 000f  ......X....g....
 00003f50: 0300 0019 0000 0000 0000 0000 0000 0080  ................
 00003f60: 8139 1a00 0078 6c2f 776f 726b 7368 6565  .9...xl/workshee
 00003f70: 7473 2f73 6865 6574 3131 2e78 6d6c 504b  ts/sheet11.xmlPK
-00003f80: 0102 1403 1400 0000 0800 d263 a858 82b2  ...........c.X..
+00003f80: 0102 1403 1400 0000 0800 c68c a858 82b2  .............X..
 00003f90: f49d 6701 0000 0f03 0000 1900 0000 0000  ..g.............
 00003fa0: 0000 0000 0000 8081 d71b 0000 786c 2f77  ............xl/w
 00003fb0: 6f72 6b73 6865 6574 732f 7368 6565 7431  orksheets/sheet1
 00003fc0: 322e 786d 6c50 4b01 0214 0314 0000 0008  2.xmlPK.........
-00003fd0: 00d2 63a8 58fb c712 8d4a 0100 0075 0200  ..c.X....J...u..
+00003fd0: 00c6 8ca8 58fb c712 8d4a 0100 0075 0200  ....X....J...u..
 00003fe0: 0019 0000 0000 0000 0000 0000 0080 8175  ...............u
 00003ff0: 1d00 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
 00004000: 2f73 6865 6574 3133 2e78 6d6c 504b 0102  /sheet13.xmlPK..
-00004010: 1403 1400 0000 0800 d263 a858 f666 8318  .........c.X.f..
+00004010: 1403 1400 0000 0800 c68c a858 f666 8318  ...........X.f..
 00004020: 5c01 0000 8b02 0000 1900 0000 0000 0000  \...............
 00004030: 0000 0000 8081 f61e 0000 786c 2f77 6f72  ..........xl/wor
 00004040: 6b73 6865 6574 732f 7368 6565 7431 342e  ksheets/sheet14.
-00004050: 786d 6c50 4b01 0214 0314 0000 0008 00d2  xmlPK...........
-00004060: 63a8 580c 5719 2b43 0100 0044 0200 0019  c.X.W.+C...D....
+00004050: 786d 6c50 4b01 0214 0314 0000 0008 00c6  xmlPK...........
+00004060: 8ca8 580c 5719 2b43 0100 0044 0200 0019  ..X.W.+C...D....
 00004070: 0000 0000 0000 0000 0000 0080 8189 2000  .............. .
 00004080: 0078 6c2f 776f 726b 7368 6565 7473 2f73  .xl/worksheets/s
 00004090: 6865 6574 3135 2e78 6d6c 504b 0102 1403  heet15.xmlPK....
-000040a0: 1400 0000 0800 d263 a858 44ff 8108 6901  .......c.XD...i.
+000040a0: 1400 0000 0800 c68c a858 44ff 8108 6901  .........XD...i.
 000040b0: 0000 0c03 0000 1900 0000 0000 0000 0000  ................
 000040c0: 0000 8081 0322 0000 786c 2f77 6f72 6b73  ....."..xl/works
 000040d0: 6865 6574 732f 7368 6565 7431 362e 786d  heets/sheet16.xm
-000040e0: 6c50 4b01 0214 0314 0000 0008 00d2 63a8  lPK...........c.
+000040e0: 6c50 4b01 0214 0314 0000 0008 00c6 8ca8  lPK.............
 000040f0: 5811 26ee aa80 0100 0080 0300 0019 0000  X.&.............
 00004100: 0000 0000 0000 0000 0080 81a3 2300 0078  ............#..x
 00004110: 6c2f 776f 726b 7368 6565 7473 2f73 6865  l/worksheets/she
 00004120: 6574 3137 2e78 6d6c 504b 0102 1403 1400  et17.xmlPK......
-00004130: 0000 0800 d263 a858 44ff 8108 6901 0000  .....c.XD...i...
+00004130: 0000 0800 c68c a858 44ff 8108 6901 0000  .......XD...i...
 00004140: 0c03 0000 1900 0000 0000 0000 0000 0000  ................
 00004150: 8081 5a25 0000 786c 2f77 6f72 6b73 6865  ..Z%..xl/workshe
 00004160: 6574 732f 7368 6565 7431 382e 786d 6c50  ets/sheet18.xmlP
-00004170: 4b01 0214 0314 0000 0008 00d2 63a8 5844  K...........c.XD
+00004170: 4b01 0214 0314 0000 0008 00c6 8ca8 5844  K.............XD
 00004180: ff81 0869 0100 000c 0300 0019 0000 0000  ...i............
 00004190: 0000 0000 0000 0080 81fa 2600 0078 6c2f  ..........&..xl/
 000041a0: 776f 726b 7368 6565 7473 2f73 6865 6574  worksheets/sheet
 000041b0: 3139 2e78 6d6c 504b 0102 1403 1400 0000  19.xmlPK........
-000041c0: 0800 d263 a858 44ff 8108 6901 0000 0c03  ...c.XD...i.....
+000041c0: 0800 c68c a858 44ff 8108 6901 0000 0c03  .....XD...i.....
 000041d0: 0000 1900 0000 0000 0000 0000 0000 8081  ................
 000041e0: 9a28 0000 786c 2f77 6f72 6b73 6865 6574  .(..xl/worksheet
 000041f0: 732f 7368 6565 7432 302e 786d 6c50 4b01  s/sheet20.xmlPK.
-00004200: 0214 0314 0000 0008 00d2 63a8 5819 ef2f  ..........c.X../
+00004200: 0214 0314 0000 0008 00c6 8ca8 5819 ef2f  ............X../
 00004210: 387b 0100 004b 0300 0019 0000 0000 0000  8{...K..........
 00004220: 0000 0000 0080 813a 2a00 0078 6c2f 776f  .......:*..xl/wo
 00004230: 726b 7368 6565 7473 2f73 6865 6574 3231  rksheets/sheet21
 00004240: 2e78 6d6c 504b 0102 1403 1400 0000 0800  .xmlPK..........
-00004250: d263 a858 caac fec0 7101 0000 3e03 0000  .c.X....q...>...
+00004250: c68c a858 caac fec0 7101 0000 3e03 0000  ...X....q...>...
 00004260: 1900 0000 0000 0000 0000 0000 8081 ec2b  ...............+
 00004270: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
 00004280: 7368 6565 7432 322e 786d 6c50 4b01 0214  sheet22.xmlPK...
-00004290: 0314 0000 0008 00d2 63a8 5825 1336 5183  ........c.X%.6Q.
+00004290: 0314 0000 0008 00c6 8ca8 5825 1336 5183  ..........X%.6Q.
 000042a0: 0100 0057 0300 0019 0000 0000 0000 0000  ...W............
 000042b0: 0000 0080 8194 2d00 0078 6c2f 776f 726b  ......-..xl/work
 000042c0: 7368 6565 7473 2f73 6865 6574 3233 2e78  sheets/sheet23.x
-000042d0: 6d6c 504b 0102 1403 1400 0000 0800 d263  mlPK...........c
+000042d0: 6d6c 504b 0102 1403 1400 0000 0800 c68c  mlPK............
 000042e0: a858 a50c 764f 5301 0000 a402 0000 1900  .X..vOS.........
 000042f0: 0000 0000 0000 0000 0000 8081 4e2f 0000  ............N/..
 00004300: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
 00004310: 6565 7432 342e 786d 6c50 4b01 0214 0314  eet24.xmlPK.....
-00004320: 0000 0008 00d2 63a8 5865 1756 075c 0100  ......c.Xe.V.\..
+00004320: 0000 0008 00c6 8ca8 5865 1756 075c 0100  ........Xe.V.\..
 00004330: 00b5 0200 0019 0000 0000 0000 0000 0000  ................
 00004340: 0080 81d8 3000 0078 6c2f 776f 726b 7368  ....0..xl/worksh
 00004350: 6565 7473 2f73 6865 6574 3235 2e78 6d6c  eets/sheet25.xml
-00004360: 504b 0102 1403 1400 0000 0800 d263 a858  PK...........c.X
+00004360: 504b 0102 1403 1400 0000 0800 c68c a858  PK.............X
 00004370: d205 f146 5202 0000 470a 0000 0d00 0000  ...FR...G.......
 00004380: 0000 0000 0000 0000 8001 6b32 0000 786c  ..........k2..xl
 00004390: 2f73 7479 6c65 732e 786d 6c50 4b01 0214  /styles.xmlPK...
-000043a0: 0314 0000 0008 00d2 63a8 58b7 47eb 8ac0  ........c.X.G...
+000043a0: 0314 0000 0008 00c6 8ca8 58b7 47eb 8ac0  ..........X.G...
 000043b0: 0000 0016 0200 000b 0000 0000 0000 0000  ................
 000043c0: 0000 0080 01e8 3400 005f 7265 6c73 2f2e  ......4.._rels/.
 000043d0: 7265 6c73 504b 0102 1403 1400 0000 0800  relsPK..........
-000043e0: d263 a858 e7f3 f05b a502 0000 5f09 0000  .c.X...[...._...
+000043e0: c68c a858 e7f3 f05b a502 0000 5f09 0000  ...X...[...._...
 000043f0: 0f00 0000 0000 0000 0000 0000 8001 d135  ...............5
 00004400: 0000 786c 2f77 6f72 6b62 6f6f 6b2e 786d  ..xl/workbook.xm
-00004410: 6c50 4b01 0214 0314 0000 0008 00d2 63a8  lPK...........c.
+00004410: 6c50 4b01 0214 0314 0000 0008 00c6 8ca8  lPK.............
 00004420: 58f9 efd8 af3c 0100 00cd 0f00 001a 0000  X....<..........
 00004430: 0000 0000 0000 0000 0080 01a3 3800 0078  ............8..x
 00004440: 6c2f 5f72 656c 732f 776f 726b 626f 6f6b  l/_rels/workbook
 00004450: 2e78 6d6c 2e72 656c 7350 4b01 0214 0314  .xml.relsPK.....
-00004460: 0000 0008 00d2 63a8 5872 079d 5874 0100  ......c.Xr..Xt..
+00004460: 0000 0008 00c6 8ca8 5872 079d 5874 0100  ........Xr..Xt..
 00004470: 00bf 1000 0013 0000 0000 0000 0000 0000  ................
 00004480: 0080 0117 3a00 005b 436f 6e74 656e 745f  ....:..[Content_
 00004490: 5479 7065 735d 2e78 6d6c 504b 0506 0000  Types].xmlPK....
 000044a0: 0000 2100 2100 de08 0000 bc3b 0000 0000  ..!.!......;....
```

### Comparing `shareyourcloning_linkml-0.1.4a0/project/graphql/shareyourcloning_linkml.graphql` & `shareyourcloning_linkml-0.1.5a0/project/graphql/shareyourcloning_linkml.graphql`

 * *Files identical despite different names*

### Comparing `shareyourcloning_linkml-0.1.4a0/project/jsonld/shareyourcloning_linkml.context.jsonld` & `shareyourcloning_linkml-0.1.5a0/project/jsonld/shareyourcloning_linkml.context.jsonld`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'comments'": "{'generation_date': '2024-05-08T17:38:06'}"}*

```diff
@@ -273,11 +273,11 @@
         },
         "user_input": {
             "@id": "user_input"
         }
     },
     "comments": {
         "description": "Auto generated by LinkML jsonld context generator",
-        "generation_date": "2024-05-08T12:30:30",
+        "generation_date": "2024-05-08T17:38:06",
         "source": "shareyourcloning_linkml.yaml"
     }
 }
```

### Comparing `shareyourcloning_linkml-0.1.4a0/project/jsonld/shareyourcloning_linkml.jsonld` & `shareyourcloning_linkml-0.1.5a0/project/jsonld/shareyourcloning_linkml.jsonld`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285101596173552%*

 * *Differences: {"'classes'": "{26: {'attributes': {2: {'inlined_as_list': True}}}}",*

 * * "'generation_date'": "'2024-05-08T17:38:06'",*

 * * "'slots'": "{50: {'inlined': True, 'inlined_as_list': True}}",*

 * * "'source_file_date'": "'2024-05-08T17:32:06'",*

 * * "'source_file_size'": '15636'}*

```diff
@@ -754,14 +754,15 @@
                     "name": "sources",
                     "range": "Source",
                     "required": true
                 },
                 {
                     "@type": "SlotDefinition",
                     "description": "The primers that are used in the cloning strategy",
+                    "inlined_as_list": true,
                     "multivalued": true,
                     "name": "primers",
                     "range": "Primer"
                 },
                 {
                     "@type": "SlotDefinition",
                     "description": "A description of the cloning strategy",
@@ -830,15 +831,15 @@
                 {
                     "description": "Full sequence of the plasmid performed by Addgene",
                     "text": "addgene-full"
                 }
             ]
         }
     ],
-    "generation_date": "2024-05-08T12:30:30",
+    "generation_date": "2024-05-08T17:38:06",
     "id": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
     "imports": [
         "linkml:types"
     ],
     "license": "MIT",
     "metamodel_version": "1.7.0",
     "name": "ShareYourCloning_LinkML",
@@ -1584,14 +1585,16 @@
             "@type": "SlotDefinition",
             "alias": "primers",
             "description": "The primers that are used in the cloning strategy",
             "domain_of": [
                 "CloningStrategy"
             ],
             "from_schema": "https://w3id.org/genestorian/ShareYourCloning_LinkML",
+            "inlined": true,
+            "inlined_as_list": true,
             "multivalued": true,
             "name": "cloningStrategy__primers",
             "owner": "CloningStrategy",
             "range": "Primer",
             "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/primers"
         },
         {
@@ -1965,16 +1968,16 @@
             "owner": "PolymeraseExtensionSource",
             "range": "Sequence",
             "slot_uri": "https://w3id.org/genestorian/ShareYourCloning_LinkML/input",
             "usage_slot_name": "input"
         }
     ],
     "source_file": "shareyourcloning_linkml.yaml",
-    "source_file_date": "2024-05-08T12:30:24",
-    "source_file_size": 15604,
+    "source_file_date": "2024-05-08T17:32:06",
+    "source_file_size": 15636,
     "title": "ShareYourCloning_LinkML",
     "types": [
         {
             "@type": "TypeDefinition",
             "base": "str",
             "definition_uri": "https://w3id.org/linkml/String",
             "description": "A character string",
```

### Comparing `shareyourcloning_linkml-0.1.4a0/project/jsonschema/shareyourcloning_linkml.schema.json` & `shareyourcloning_linkml-0.1.5a0/project/jsonschema/shareyourcloning_linkml.schema.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999980623759921%*

 * *Differences: {"'$defs'": "{'CloningStrategy': {'properties': {'primers': {'items': {replace: "*

 * *            "OrderedDict([('$ref', '#/$defs/Primer')])}}}}}"}*

```diff
@@ -206,15 +206,15 @@
                 "description": {
                     "description": "A description of the cloning strategy",
                     "type": "string"
                 },
                 "primers": {
                     "description": "The primers that are used in the cloning strategy",
                     "items": {
-                        "type": "integer"
+                        "$ref": "#/$defs/Primer"
                     },
                     "type": "array"
                 },
                 "sequences": {
                     "description": "The sequences that are used in the cloning strategy",
                     "items": {
                         "anyOf": [
```

### Comparing `shareyourcloning_linkml-0.1.4a0/project/owl/shareyourcloning_linkml.owl.ttl` & `shareyourcloning_linkml-0.1.5a0/project/owl/shareyourcloning_linkml.owl.ttl`

 * *Files 0% similar despite different names*

```diff
@@ -9,124 +9,124 @@
 @prefix skos: <http://www.w3.org/2004/02/skos/core#> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
 
 shareyourcloning_linkml:CloningStrategy a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "CloningStrategy" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:minCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:sources ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty shareyourcloning_linkml:description ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom shareyourcloning_linkml:Primer ;
-            owl:onProperty shareyourcloning_linkml:primers ],
-        [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:description ],
         [ a owl:Restriction ;
+            owl:allValuesFrom shareyourcloning_linkml:Sequence ;
+            owl:onProperty shareyourcloning_linkml:sequences ],
+        [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:description ],
         [ a owl:Restriction ;
             owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:sequences ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:primers ],
         [ a owl:Restriction ;
-            owl:allValuesFrom shareyourcloning_linkml:Sequence ;
-            owl:onProperty shareyourcloning_linkml:sequences ],
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty shareyourcloning_linkml:description ],
         [ a owl:Restriction ;
             owl:allValuesFrom shareyourcloning_linkml:Source ;
+            owl:onProperty shareyourcloning_linkml:sources ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom shareyourcloning_linkml:Primer ;
+            owl:onProperty shareyourcloning_linkml:primers ],
+        [ a owl:Restriction ;
+            owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:sources ] ;
     skos:definition "Represents a cloning strategy" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:AssemblyJoin a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "AssemblyJoin" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:allValuesFrom shareyourcloning_linkml:AssemblyJoinComponent ;
+            owl:minCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:left ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:right ],
         [ a owl:Restriction ;
-            owl:minCardinality 1 ;
+            owl:allValuesFrom shareyourcloning_linkml:AssemblyJoinComponent ;
             owl:onProperty shareyourcloning_linkml:right ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:left ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:right ],
-        [ a owl:Restriction ;
             owl:minCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:left ],
+            owl:onProperty shareyourcloning_linkml:right ],
         [ a owl:Restriction ;
             owl:allValuesFrom shareyourcloning_linkml:AssemblyJoinComponent ;
             owl:onProperty shareyourcloning_linkml:left ] ;
     skos:definition "Represents a joint between two fragments in an assembly" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:SimpleSequenceLocation a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "SimpleSequenceLocation" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Integer ;
+            owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:start ],
         [ a owl:Restriction ;
             owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:end ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:Integer ;
-            owl:onProperty shareyourcloning_linkml:strand ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Integer ;
             owl:onProperty shareyourcloning_linkml:end ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
+            owl:allValuesFrom linkml:Integer ;
             owl:onProperty shareyourcloning_linkml:strand ],
         [ a owl:Restriction ;
-            owl:minCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:start ],
-        [ a owl:Restriction ;
             owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:end ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom linkml:Integer ;
             owl:onProperty shareyourcloning_linkml:start ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:end ],
+            owl:onProperty shareyourcloning_linkml:strand ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
+            owl:minCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:start ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:strand ] ;
     skos:definition "Represents a location within a sequence, for now support for ranges only" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:AddGeneIdSource a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "AddGeneIdSource" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:addgene_sequence_type ],
+            owl:minCardinality 0 ;
+            owl:onProperty shareyourcloning_linkml:sequence_file_url ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:sequence_file_url ],
+            owl:onProperty shareyourcloning_linkml:addgene_sequence_type ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
+            owl:allValuesFrom shareyourcloning_linkml:AddGeneSequenceType ;
             owl:onProperty shareyourcloning_linkml:addgene_sequence_type ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty shareyourcloning_linkml:sequence_file_url ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom shareyourcloning_linkml:AddGeneSequenceType ;
             owl:onProperty shareyourcloning_linkml:addgene_sequence_type ],
         [ a owl:Restriction ;
             owl:allValuesFrom [ a rdfs:Datatype ;
                     owl:intersectionOf ( linkml:String [ a rdfs:Datatype ;
                                 owl:onDatatype xsd:string ;
                                 owl:withRestrictions ( [ xsd:pattern "^https?:\\/\\/(www\\.)?[-a-zA-Z0-9@:%._\\+~#=]{1,256}\\.[a-zA-Z0-9()]{1,6}\\b([-a-zA-Z0-9()@:%_\\+.~#?&//=]*)$" ] ) ] ) ] ;
             owl:onProperty shareyourcloning_linkml:sequence_file_url ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:sequence_file_url ],
         shareyourcloning_linkml:RepositoryIdSource ;
     skos:definition "Represents the source of a sequence that is identified by an AddGene id" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 <https://w3id.org/genestorian/ShareYourCloning_LinkML/AddGeneSequenceType#addgene-full> a owl:Class,
         shareyourcloning_linkml:AddGeneSequenceType ;
     rdfs:label "addgene-full" ;
@@ -137,268 +137,268 @@
     rdfs:label "depositor-full" ;
     rdfs:subClassOf shareyourcloning_linkml:AddGeneSequenceType .
 
 shareyourcloning_linkml:AssemblyJoinComponent a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "AssemblyJoinComponent" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:minCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:location ],
-        [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:reverse_complemented ],
         [ a owl:Restriction ;
-            owl:allValuesFrom shareyourcloning_linkml:Sequence ;
-            owl:onProperty shareyourcloning_linkml:sequence ],
+            owl:allValuesFrom linkml:Boolean ;
+            owl:onProperty shareyourcloning_linkml:reverse_complemented ],
         [ a owl:Restriction ;
             owl:minCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:reverse_complemented ],
+            owl:onProperty shareyourcloning_linkml:location ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Boolean ;
-            owl:onProperty shareyourcloning_linkml:reverse_complemented ],
+            owl:allValuesFrom shareyourcloning_linkml:SimpleSequenceLocation ;
+            owl:onProperty shareyourcloning_linkml:location ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom shareyourcloning_linkml:Sequence ;
+            owl:onProperty shareyourcloning_linkml:sequence ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:location ],
         [ a owl:Restriction ;
+            owl:minCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:reverse_complemented ],
+        [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:sequence ],
         [ a owl:Restriction ;
             owl:minCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:sequence ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom shareyourcloning_linkml:SimpleSequenceLocation ;
-            owl:onProperty shareyourcloning_linkml:location ] ;
+            owl:onProperty shareyourcloning_linkml:sequence ] ;
     skos:definition "Represents a component of a join between two fragments in an assembly" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:CRISPRSource a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "CRISPRSource" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:allValuesFrom shareyourcloning_linkml:Primer ;
+            owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:guides ],
         [ a owl:Restriction ;
-            owl:minCardinality 1 ;
+            owl:allValuesFrom shareyourcloning_linkml:Primer ;
             owl:onProperty shareyourcloning_linkml:guides ],
         shareyourcloning_linkml:HomologousRecombinationSource ;
     skos:definition "Represents the source of a sequence that is generated by CRISPR" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:GenomeCoordinatesSource a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "GenomeCoordinatesSource" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty shareyourcloning_linkml:gene_id ],
+            owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:strand ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:gene_id ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty shareyourcloning_linkml:locus_tag ],
+            owl:allValuesFrom linkml:Integer ;
+            owl:onProperty shareyourcloning_linkml:gene_id ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty shareyourcloning_linkml:assembly_accession ],
+            owl:minCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:strand ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:end ],
+            owl:minCardinality 0 ;
+            owl:onProperty shareyourcloning_linkml:locus_tag ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty shareyourcloning_linkml:sequence_accession ],
+            owl:minCardinality 0 ;
+            owl:onProperty shareyourcloning_linkml:gene_id ],
         [ a owl:Restriction ;
             owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:start ],
         [ a owl:Restriction ;
-            owl:minCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:sequence_accession ],
-        [ a owl:Restriction ;
             owl:allValuesFrom linkml:String ;
-            owl:onProperty shareyourcloning_linkml:locus_tag ],
+            owl:onProperty shareyourcloning_linkml:sequence_accession ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:Integer ;
-            owl:onProperty shareyourcloning_linkml:gene_id ],
-        [ a owl:Restriction ;
-            owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:strand ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:Integer ;
-            owl:onProperty shareyourcloning_linkml:start ],
+            owl:onProperty shareyourcloning_linkml:end ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:sequence_accession ],
+            owl:onProperty shareyourcloning_linkml:locus_tag ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:start ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:assembly_accession ],
         [ a owl:Restriction ;
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty shareyourcloning_linkml:locus_tag ],
+        [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:strand ],
+            owl:onProperty shareyourcloning_linkml:assembly_accession ],
         [ a owl:Restriction ;
             owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:end ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:Integer ;
-            owl:onProperty shareyourcloning_linkml:end ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Integer ;
-            owl:onProperty shareyourcloning_linkml:strand ],
+            owl:onProperty shareyourcloning_linkml:start ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:assembly_accession ],
+            owl:onProperty shareyourcloning_linkml:end ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:locus_tag ],
+            owl:onProperty shareyourcloning_linkml:sequence_accession ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:start ],
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty shareyourcloning_linkml:assembly_accession ],
+        [ a owl:Restriction ;
+            owl:minCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:sequence_accession ],
         shareyourcloning_linkml:Source ;
     skos:definition "Represents the source of a sequence that is identified by genome coordinates, requested from NCBI" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:GibsonAssemblySource a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "GibsonAssemblySource" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:allValuesFrom owl:Thing ;
+            owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:input ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
+            owl:allValuesFrom owl:Thing ;
             owl:onProperty shareyourcloning_linkml:input ],
         shareyourcloning_linkml:AssemblySource ;
     skos:definition "Represents the source of a sequence that is generated by Gibson assembly" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:LigationSource a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "LigationSource" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:allValuesFrom owl:Thing ;
+            owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:input ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
+            owl:allValuesFrom owl:Thing ;
             owl:onProperty shareyourcloning_linkml:input ],
         shareyourcloning_linkml:AssemblySource ;
     skos:definition "Represents the source of a sequence that is generated by ligation with sticky or blunt ends." ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:ManuallyTypedSource a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "ManuallyTypedSource" ;
     rdfs:subClassOf [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:circular ],
+            owl:onProperty shareyourcloning_linkml:user_input ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
+            owl:onProperty shareyourcloning_linkml:circular ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:overhang_watson_3prime ],
         [ a owl:Restriction ;
+            owl:allValuesFrom [ a rdfs:Datatype ;
+                    owl:intersectionOf ( linkml:String [ a rdfs:Datatype ;
+                                owl:onDatatype xsd:string ;
+                                owl:withRestrictions ( [ xsd:pattern "^[acgtACGT]+$" ] ) ] ) ] ;
+            owl:onProperty shareyourcloning_linkml:user_input ],
+        [ a owl:Restriction ;
             owl:allValuesFrom linkml:Integer ;
             owl:onProperty shareyourcloning_linkml:overhang_crick_3prime ],
         [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:circular ],
+        [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:overhang_crick_3prime ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
+            owl:allValuesFrom linkml:Boolean ;
             owl:onProperty shareyourcloning_linkml:circular ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:overhang_crick_3prime ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:user_input ],
+            owl:minCardinality 0 ;
+            owl:onProperty shareyourcloning_linkml:overhang_watson_3prime ],
         [ a owl:Restriction ;
             owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:user_input ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:Integer ;
             owl:onProperty shareyourcloning_linkml:overhang_watson_3prime ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom [ a rdfs:Datatype ;
-                    owl:intersectionOf ( linkml:String [ a rdfs:Datatype ;
-                                owl:onDatatype xsd:string ;
-                                owl:withRestrictions ( [ xsd:pattern "^[acgtACGT]+$" ] ) ] ) ] ;
-            owl:onProperty shareyourcloning_linkml:user_input ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:overhang_watson_3prime ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Boolean ;
-            owl:onProperty shareyourcloning_linkml:circular ],
         shareyourcloning_linkml:Source ;
     skos:definition "Represents the source of a sequence that is manually typed by the user" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:NamedThing a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "NamedThing" ;
     rdfs:subClassOf [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:id ],
         [ a owl:Restriction ;
-            owl:minCardinality 1 ;
+            owl:allValuesFrom linkml:Integer ;
             owl:onProperty shareyourcloning_linkml:id ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Integer ;
+            owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:id ] ;
     skos:exactMatch schema1:Thing ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:OligoHybridizationSource a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "OligoHybridizationSource" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Integer ;
-            owl:onProperty shareyourcloning_linkml:overhang_crick_3prime ],
+            owl:allValuesFrom shareyourcloning_linkml:Primer ;
+            owl:onProperty shareyourcloning_linkml:forward_oligo ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:reverse_oligo ],
         [ a owl:Restriction ;
-            owl:allValuesFrom shareyourcloning_linkml:Primer ;
-            owl:onProperty shareyourcloning_linkml:reverse_oligo ],
+            owl:minCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:forward_oligo ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:forward_oligo ],
+            owl:onProperty shareyourcloning_linkml:overhang_crick_3prime ],
         [ a owl:Restriction ;
-            owl:allValuesFrom shareyourcloning_linkml:Primer ;
-            owl:onProperty shareyourcloning_linkml:forward_oligo ],
+            owl:minCardinality 0 ;
+            owl:onProperty shareyourcloning_linkml:overhang_crick_3prime ],
         [ a owl:Restriction ;
             owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:reverse_oligo ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty shareyourcloning_linkml:overhang_crick_3prime ],
+            owl:allValuesFrom shareyourcloning_linkml:Primer ;
+            owl:onProperty shareyourcloning_linkml:reverse_oligo ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
+            owl:allValuesFrom linkml:Integer ;
             owl:onProperty shareyourcloning_linkml:overhang_crick_3prime ],
         [ a owl:Restriction ;
-            owl:minCardinality 1 ;
+            owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:forward_oligo ],
         shareyourcloning_linkml:Source ;
     skos:definition "Represents the source of a sequence that is generated by oligo hybridization" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:PCRSource a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "PCRSource" ;
     rdfs:subClassOf [ a owl:Restriction ;
             owl:allValuesFrom shareyourcloning_linkml:Primer ;
-            owl:onProperty shareyourcloning_linkml:forward_primer ],
+            owl:onProperty shareyourcloning_linkml:reverse_primer ],
         [ a owl:Restriction ;
             owl:allValuesFrom shareyourcloning_linkml:Primer ;
+            owl:onProperty shareyourcloning_linkml:forward_primer ],
+        [ a owl:Restriction ;
+            owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:reverse_primer ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:forward_primer ],
+            owl:onProperty shareyourcloning_linkml:reverse_primer ],
         [ a owl:Restriction ;
             owl:allValuesFrom owl:Thing ;
             owl:onProperty shareyourcloning_linkml:input ],
         [ a owl:Restriction ;
-            owl:minCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:reverse_primer ],
-        [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:reverse_primer ],
+            owl:onProperty shareyourcloning_linkml:forward_primer ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:input ],
         [ a owl:Restriction ;
             owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:forward_primer ],
         shareyourcloning_linkml:AssemblySource ;
@@ -431,62 +431,62 @@
 shareyourcloning_linkml:RestrictionAndLigationSource a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "RestrictionAndLigationSource" ;
     rdfs:subClassOf [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:input ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty shareyourcloning_linkml:restriction_enzymes ],
-        [ a owl:Restriction ;
             owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:restriction_enzymes ],
         [ a owl:Restriction ;
             owl:allValuesFrom owl:Thing ;
             owl:onProperty shareyourcloning_linkml:input ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty shareyourcloning_linkml:restriction_enzymes ],
         shareyourcloning_linkml:AssemblySource ;
     skos:definition "Represents the source of a sequence that is generated by restriction and ligation" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:RestrictionEnzymeDigestionSource a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "RestrictionEnzymeDigestionSource" ;
     rdfs:subClassOf [ a owl:Restriction ;
             owl:allValuesFrom shareyourcloning_linkml:RestrictionSequenceCut ;
-            owl:onProperty shareyourcloning_linkml:left_edge ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty shareyourcloning_linkml:left_edge ],
+            owl:onProperty shareyourcloning_linkml:right_edge ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:right_edge ],
         [ a owl:Restriction ;
-            owl:allValuesFrom shareyourcloning_linkml:RestrictionSequenceCut ;
-            owl:onProperty shareyourcloning_linkml:right_edge ],
+            owl:minCardinality 0 ;
+            owl:onProperty shareyourcloning_linkml:left_edge ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:left_edge ],
         [ a owl:Restriction ;
+            owl:allValuesFrom shareyourcloning_linkml:RestrictionSequenceCut ;
+            owl:onProperty shareyourcloning_linkml:left_edge ],
+        [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:right_edge ],
         shareyourcloning_linkml:SequenceCutSource ;
     skos:definition "Represents the source of a sequence that is a subfragment of another sequence, generated by sequence cutting using restriction enzymes." ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:RestrictionSequenceCut a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "RestrictionSequenceCut" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
+            owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:restriction_enzyme ],
         [ a owl:Restriction ;
-            owl:minCardinality 1 ;
+            owl:allValuesFrom linkml:String ;
             owl:onProperty shareyourcloning_linkml:restriction_enzyme ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
+            owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:restriction_enzyme ],
         shareyourcloning_linkml:SequenceCut ;
     skos:definition "Represents a cut in a DNA sequence that is made by a restriction enzyme" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 <https://w3id.org/genestorian/ShareYourCloning_LinkML/SequenceFileFormat#fasta> a owl:Class,
         shareyourcloning_linkml:SequenceFileFormat ;
@@ -503,83 +503,83 @@
     rdfs:label "snapgene" ;
     rdfs:subClassOf shareyourcloning_linkml:SequenceFileFormat .
 
 shareyourcloning_linkml:TextFileSequence a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "TextFileSequence" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
+            owl:allValuesFrom linkml:Integer ;
             owl:onProperty shareyourcloning_linkml:overhang_crick_3prime ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
+            owl:onProperty shareyourcloning_linkml:overhang_watson_3prime ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:file_content ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:overhang_crick_3prime ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Integer ;
+            owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:overhang_crick_3prime ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:Integer ;
             owl:onProperty shareyourcloning_linkml:overhang_watson_3prime ],
         [ a owl:Restriction ;
             owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:sequence_file_format ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:file_content ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty shareyourcloning_linkml:file_content ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:overhang_watson_3prime ],
         [ a owl:Restriction ;
+            owl:allValuesFrom shareyourcloning_linkml:SequenceFileFormat ;
+            owl:onProperty shareyourcloning_linkml:sequence_file_format ],
+        [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:file_content ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty shareyourcloning_linkml:overhang_watson_3prime ],
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty shareyourcloning_linkml:file_content ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:sequence_file_format ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom shareyourcloning_linkml:SequenceFileFormat ;
-            owl:onProperty shareyourcloning_linkml:sequence_file_format ],
         shareyourcloning_linkml:Sequence ;
     skos:definition "A sequence (may have features) defined by the content of a text file" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:UploadedFileSource a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "UploadedFileSource" ;
     rdfs:subClassOf [ a owl:Restriction ;
             owl:allValuesFrom linkml:String ;
             owl:onProperty shareyourcloning_linkml:file_name ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty shareyourcloning_linkml:file_name ],
+            owl:onProperty shareyourcloning_linkml:index_in_file ],
         [ a owl:Restriction ;
-            owl:minCardinality 1 ;
+            owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:sequence_file_format ],
         [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:index_in_file ],
+        [ a owl:Restriction ;
             owl:allValuesFrom shareyourcloning_linkml:SequenceFileFormat ;
             owl:onProperty shareyourcloning_linkml:sequence_file_format ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Integer ;
-            owl:onProperty shareyourcloning_linkml:index_in_file ],
-        [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty shareyourcloning_linkml:index_in_file ],
+            owl:onProperty shareyourcloning_linkml:file_name ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
+            owl:minCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:sequence_file_format ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom linkml:Integer ;
             owl:onProperty shareyourcloning_linkml:index_in_file ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:file_name ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:sequence_file_format ],
         shareyourcloning_linkml:Source ;
     skos:definition "Represents the source of a sequence that is uploaded as a file" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:assembly a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "assembly" ;
@@ -630,86 +630,86 @@
     skos:definition "Represents the source of a sequence that is generated by homologous recombination" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:RepositoryIdSource a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "RepositoryIdSource" ;
     rdfs:subClassOf [ a owl:Restriction ;
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty shareyourcloning_linkml:repository_id ],
+        [ a owl:Restriction ;
             owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:repository_name ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:repository_name ],
+            owl:onProperty shareyourcloning_linkml:repository_id ],
         [ a owl:Restriction ;
             owl:allValuesFrom shareyourcloning_linkml:RepositoryName ;
             owl:onProperty shareyourcloning_linkml:repository_name ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty shareyourcloning_linkml:repository_id ],
+            owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:repository_name ],
         [ a owl:Restriction ;
             owl:minCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:repository_id ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:repository_id ],
         shareyourcloning_linkml:Source ;
     skos:definition "Represents the source of a sequence that is identified by a repository id" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:SequenceCut a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "SequenceCut" ;
     rdfs:subClassOf [ a owl:Restriction ;
+            owl:minCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:overhang ],
+        [ a owl:Restriction ;
             owl:allValuesFrom linkml:Integer ;
-            owl:onProperty shareyourcloning_linkml:cut_watson ],
+            owl:onProperty shareyourcloning_linkml:overhang ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:cut_watson ],
         [ a owl:Restriction ;
-            owl:minCardinality 1 ;
+            owl:allValuesFrom linkml:Integer ;
             owl:onProperty shareyourcloning_linkml:cut_watson ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Integer ;
+            owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:overhang ],
         [ a owl:Restriction ;
             owl:minCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:overhang ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:overhang ] ;
+            owl:onProperty shareyourcloning_linkml:cut_watson ] ;
     skos:definition "Represents a cut in a DNA sequence" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:SequenceCutSource a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "SequenceCutSource" ;
     rdfs:subClassOf [ a owl:Restriction ;
             owl:allValuesFrom shareyourcloning_linkml:SequenceCut ;
             owl:onProperty shareyourcloning_linkml:left_edge ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:right_edge ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty shareyourcloning_linkml:right_edge ],
-        [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:left_edge ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
+            owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:right_edge ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom owl:Thing ;
             owl:onProperty shareyourcloning_linkml:input ],
         [ a owl:Restriction ;
             owl:allValuesFrom shareyourcloning_linkml:SequenceCut ;
             owl:onProperty shareyourcloning_linkml:right_edge ],
         [ a owl:Restriction ;
-            owl:allValuesFrom owl:Thing ;
+            owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:input ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:left_edge ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty shareyourcloning_linkml:right_edge ],
         shareyourcloning_linkml:Source ;
     skos:definition "Represents the source of a sequence that is a subfragment of another sequence, generated by sequence cutting." ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:addgene_sequence_type a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "addgene_sequence_type" ;
@@ -921,56 +921,56 @@
 shareyourcloning_linkml:strand a owl:ObjectProperty,
         linkml:SlotDefinition .
 
 shareyourcloning_linkml:AssemblySource a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "AssemblySource" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Boolean ;
+            owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:circular ],
         [ a owl:Restriction ;
-            owl:minCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:assembly ],
+            owl:allValuesFrom linkml:Boolean ;
+            owl:onProperty shareyourcloning_linkml:circular ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
+            owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:circular ],
         [ a owl:Restriction ;
             owl:allValuesFrom shareyourcloning_linkml:AssemblyJoin ;
             owl:onProperty shareyourcloning_linkml:assembly ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:circular ],
+            owl:minCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:assembly ],
         shareyourcloning_linkml:Source ;
     skos:definition "Represents the source of a sequence that is an assembly of other sequences" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:Primer a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "Primer" ;
     rdfs:subClassOf [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty shareyourcloning_linkml:name ],
+        [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:sequence ],
+            owl:onProperty shareyourcloning_linkml:name ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
+            owl:allValuesFrom linkml:String ;
             owl:onProperty shareyourcloning_linkml:name ],
         [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty shareyourcloning_linkml:sequence ],
+        [ a owl:Restriction ;
             owl:allValuesFrom [ a rdfs:Datatype ;
                     owl:intersectionOf ( linkml:String [ a rdfs:Datatype ;
                                 owl:onDatatype xsd:string ;
                                 owl:withRestrictions ( [ xsd:pattern "^[acgtACGT]+$" ] ) ] ) ] ;
             owl:onProperty shareyourcloning_linkml:sequence ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty shareyourcloning_linkml:sequence ],
-        [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:name ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty shareyourcloning_linkml:name ],
+            owl:onProperty shareyourcloning_linkml:sequence ],
         shareyourcloning_linkml:Sequence ;
     skos:definition "An oligonucleotide or primer" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:SequenceFileFormat a owl:Class,
         linkml:EnumDefinition ;
     owl:unionOf ( <https://w3id.org/genestorian/ShareYourCloning_LinkML/SequenceFileFormat#fasta> <https://w3id.org/genestorian/ShareYourCloning_LinkML/SequenceFileFormat#genbank> <https://w3id.org/genestorian/ShareYourCloning_LinkML/SequenceFileFormat#snapgene> ) ;
@@ -985,62 +985,62 @@
     skos:definition "Taken from pydna's `dseq::ovhg`An integer describing the length of the crick strand overhang in the 5' of the molecule, or 3' of the crick strand" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:Sequence a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "Sequence" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:minCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:id ],
-        [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:type ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
+            owl:minCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:id ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom linkml:String ;
             owl:onProperty shareyourcloning_linkml:type ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
+            owl:allValuesFrom linkml:Integer ;
             owl:onProperty shareyourcloning_linkml:id ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Integer ;
+            owl:maxCardinality 1 ;
             owl:onProperty shareyourcloning_linkml:id ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
+            owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:type ],
         shareyourcloning_linkml:NamedThing ;
     skos:definition "Represents a sequence" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:Source a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "Source" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:type ],
-        [ a owl:Restriction ;
             owl:allValuesFrom shareyourcloning_linkml:Sequence ;
             owl:onProperty shareyourcloning_linkml:input ],
         [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty shareyourcloning_linkml:output ],
+        [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty shareyourcloning_linkml:type ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty shareyourcloning_linkml:output ],
+            owl:onProperty shareyourcloning_linkml:type ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty shareyourcloning_linkml:input ],
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty shareyourcloning_linkml:type ],
         [ a owl:Restriction ;
             owl:allValuesFrom shareyourcloning_linkml:Sequence ;
             owl:onProperty shareyourcloning_linkml:output ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty shareyourcloning_linkml:output ],
+            owl:onProperty shareyourcloning_linkml:input ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty shareyourcloning_linkml:type ],
+            owl:minCardinality 0 ;
+            owl:onProperty shareyourcloning_linkml:output ],
         shareyourcloning_linkml:NamedThing ;
     skos:definition "Represents the source of a sequence" ;
     skos:inScheme <https://w3id.org/genestorian/ShareYourCloning_LinkML> .
 
 shareyourcloning_linkml:input a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "input" ;
@@ -1059,105 +1059,105 @@
     rdfs:label "ShareYourCloning_LinkML" ;
     dcterms:license "MIT" ;
     dcterms:title "ShareYourCloning_LinkML" ;
     rdfs:seeAlso <https://genestorian.github.io/ShareYourCloning_LinkML> ;
     skos:definition "A LinkML data model for ShareYourCloning" .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:PCRSource ;
+    rdfs:subClassOf shareyourcloning_linkml:RepositoryIdSource ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:PCRSource .
+    owl:someValuesFrom shareyourcloning_linkml:RepositoryIdSource .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:RestrictionAndLigationSource ;
+    rdfs:subClassOf shareyourcloning_linkml:ManuallyTypedSource ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:RestrictionAndLigationSource .
+    owl:someValuesFrom shareyourcloning_linkml:ManuallyTypedSource .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:RestrictionEnzymeDigestionSource ;
+    rdfs:subClassOf shareyourcloning_linkml:PCRSource ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:RestrictionEnzymeDigestionSource .
+    owl:someValuesFrom shareyourcloning_linkml:PCRSource .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:GibsonAssemblySource ;
+    rdfs:subClassOf shareyourcloning_linkml:OligoHybridizationSource ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:GibsonAssemblySource .
+    owl:someValuesFrom shareyourcloning_linkml:OligoHybridizationSource .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:Sequence ;
+    rdfs:subClassOf shareyourcloning_linkml:CRISPRSource ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:Sequence .
+    owl:someValuesFrom shareyourcloning_linkml:CRISPRSource .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:PolymeraseExtensionSource ;
+    rdfs:subClassOf shareyourcloning_linkml:AddGeneIdSource ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:PolymeraseExtensionSource .
+    owl:someValuesFrom shareyourcloning_linkml:AddGeneIdSource .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:HomologousRecombinationSource ;
+    rdfs:subClassOf shareyourcloning_linkml:PolymeraseExtensionSource ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:HomologousRecombinationSource .
+    owl:someValuesFrom shareyourcloning_linkml:PolymeraseExtensionSource .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:AssemblySource ;
+    rdfs:subClassOf shareyourcloning_linkml:RestrictionAndLigationSource ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:AssemblySource .
+    owl:someValuesFrom shareyourcloning_linkml:RestrictionAndLigationSource .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:Source ;
+    rdfs:subClassOf shareyourcloning_linkml:Primer ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:Source .
+    owl:someValuesFrom shareyourcloning_linkml:Primer .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:LigationSource ;
+    rdfs:subClassOf shareyourcloning_linkml:GibsonAssemblySource ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:LigationSource .
+    owl:someValuesFrom shareyourcloning_linkml:GibsonAssemblySource .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:OligoHybridizationSource ;
+    rdfs:subClassOf shareyourcloning_linkml:Source ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:OligoHybridizationSource .
+    owl:someValuesFrom shareyourcloning_linkml:Source .
 
 [] a owl:Restriction ;
     rdfs:subClassOf shareyourcloning_linkml:TextFileSequence ;
     owl:onProperty shareyourcloning_linkml:type ;
     owl:someValuesFrom shareyourcloning_linkml:TextFileSequence .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:SequenceCutSource ;
+    rdfs:subClassOf shareyourcloning_linkml:AssemblySource ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:SequenceCutSource .
+    owl:someValuesFrom shareyourcloning_linkml:AssemblySource .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:UploadedFileSource ;
+    rdfs:subClassOf shareyourcloning_linkml:SequenceCutSource ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:UploadedFileSource .
+    owl:someValuesFrom shareyourcloning_linkml:SequenceCutSource .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:CRISPRSource ;
+    rdfs:subClassOf shareyourcloning_linkml:RestrictionEnzymeDigestionSource ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:CRISPRSource .
+    owl:someValuesFrom shareyourcloning_linkml:RestrictionEnzymeDigestionSource .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:ManuallyTypedSource ;
+    rdfs:subClassOf shareyourcloning_linkml:GenomeCoordinatesSource ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:ManuallyTypedSource .
+    owl:someValuesFrom shareyourcloning_linkml:GenomeCoordinatesSource .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:Primer ;
+    rdfs:subClassOf shareyourcloning_linkml:Sequence ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:Primer .
+    owl:someValuesFrom shareyourcloning_linkml:Sequence .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:RepositoryIdSource ;
+    rdfs:subClassOf shareyourcloning_linkml:HomologousRecombinationSource ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:RepositoryIdSource .
+    owl:someValuesFrom shareyourcloning_linkml:HomologousRecombinationSource .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:GenomeCoordinatesSource ;
+    rdfs:subClassOf shareyourcloning_linkml:UploadedFileSource ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:GenomeCoordinatesSource .
+    owl:someValuesFrom shareyourcloning_linkml:UploadedFileSource .
 
 [] a owl:Restriction ;
-    rdfs:subClassOf shareyourcloning_linkml:AddGeneIdSource ;
+    rdfs:subClassOf shareyourcloning_linkml:LigationSource ;
     owl:onProperty shareyourcloning_linkml:type ;
-    owl:someValuesFrom shareyourcloning_linkml:AddGeneIdSource .
+    owl:someValuesFrom shareyourcloning_linkml:LigationSource .
```

### Comparing `shareyourcloning_linkml-0.1.4a0/project/protobuf/shareyourcloning_linkml.proto` & `shareyourcloning_linkml-0.1.5a0/project/protobuf/shareyourcloning_linkml.proto`

 * *Files identical despite different names*

### Comparing `shareyourcloning_linkml-0.1.4a0/project/python/shareyourcloning_linkml.py` & `shareyourcloning_linkml-0.1.5a0/project/python/shareyourcloning_linkml.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Auto generated from shareyourcloning_linkml.yaml by pythongen.py version: 0.0.1
-# Generation date: 2024-05-08T12:30:31
+# Generation date: 2024-05-08T17:38:07
 # Schema: ShareYourCloning_LinkML
 #
 # id: https://w3id.org/genestorian/ShareYourCloning_LinkML
 # description: A LinkML data model for ShareYourCloning
 # license: MIT
 
 import dataclasses
@@ -1086,29 +1086,27 @@
     class_class_uri: ClassVar[URIRef] = SHAREYOURCLONING_LINKML["CloningStrategy"]
     class_class_curie: ClassVar[str] = "shareyourcloning_linkml:CloningStrategy"
     class_name: ClassVar[str] = "CloningStrategy"
     class_model_uri: ClassVar[URIRef] = SHAREYOURCLONING_LINKML.CloningStrategy
 
     sequences: Union[Dict[Union[int, SequenceId], Union[dict, Sequence]], List[Union[dict, Sequence]]] = empty_dict()
     sources: Union[Dict[Union[int, SourceId], Union[dict, Source]], List[Union[dict, Source]]] = empty_dict()
-    primers: Optional[Union[Union[int, PrimerId], List[Union[int, PrimerId]]]] = empty_list()
+    primers: Optional[Union[Dict[Union[int, PrimerId], Union[dict, Primer]], List[Union[dict, Primer]]]] = empty_dict()
     description: Optional[str] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.sequences):
             self.MissingRequiredField("sequences")
         self._normalize_inlined_as_list(slot_name="sequences", slot_type=Sequence, key_name="id", keyed=True)
 
         if self._is_empty(self.sources):
             self.MissingRequiredField("sources")
         self._normalize_inlined_as_list(slot_name="sources", slot_type=Source, key_name="id", keyed=True)
 
-        if not isinstance(self.primers, list):
-            self.primers = [self.primers] if self.primers is not None else []
-        self.primers = [v if isinstance(v, PrimerId) else PrimerId(v) for v in self.primers]
+        self._normalize_inlined_as_list(slot_name="primers", slot_type=Primer, key_name="id", keyed=True)
 
         if self.description is not None and not isinstance(self.description, str):
             self.description = str(self.description)
 
         super().__post_init__(**kwargs)
 
 
@@ -1618,15 +1616,15 @@
 
 slots.cloningStrategy__primers = Slot(
     uri=SHAREYOURCLONING_LINKML.primers,
     name="cloningStrategy__primers",
     curie=SHAREYOURCLONING_LINKML.curie("primers"),
     model_uri=SHAREYOURCLONING_LINKML.cloningStrategy__primers,
     domain=None,
-    range=Optional[Union[Union[int, PrimerId], List[Union[int, PrimerId]]]],
+    range=Optional[Union[Dict[Union[int, PrimerId], Union[dict, Primer]], List[Union[dict, Primer]]]],
 )
 
 slots.cloningStrategy__description = Slot(
     uri=SHAREYOURCLONING_LINKML.description,
     name="cloningStrategy__description",
     curie=SHAREYOURCLONING_LINKML.curie("description"),
     model_uri=SHAREYOURCLONING_LINKML.cloningStrategy__description,
```

### Comparing `shareyourcloning_linkml-0.1.4a0/project/shacl/shareyourcloning_linkml.shacl.ttl` & `shareyourcloning_linkml-0.1.5a0/project/shacl/shareyourcloning_linkml.shacl.ttl`

 * *Files 0% similar despite different names*

```diff
@@ -14,96 +14,96 @@
             sh:path schema1:identifier ] ;
     sh:targetClass schema1:Thing .
 
 shareyourcloning_linkml:AddGeneIdSource a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents the source of a sequence that is identified by an AddGene id" ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
-            sh:nodeKind sh:IRI ;
-            sh:order 4 ;
-            sh:path shareyourcloning_linkml:input ],
-        [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "Identifier of the sequence that is the output of this source." ;
-            sh:maxCount 1 ;
-            sh:nodeKind sh:IRI ;
-            sh:order 5 ;
-            sh:path shareyourcloning_linkml:output ],
-        [ sh:datatype xsd:string ;
-            sh:description "The URL of a sequence file" ;
-            sh:maxCount 1 ;
-            sh:order 0 ;
-            sh:path shareyourcloning_linkml:sequence_file_url ;
-            sh:pattern "^https?:\\/\\/(www\\.)?[-a-zA-Z0-9@:%._\\+~#=]{1,256}\\.[a-zA-Z0-9()]{1,6}\\b([-a-zA-Z0-9()@:%_\\+.~#?&//=]*)$" ],
-        [ sh:datatype xsd:string ;
-            sh:description "The id of the sequence in the repository" ;
+    sh:property [ sh:in ( "addgene" "genbank" ) ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
-            sh:order 3 ;
-            sh:path shareyourcloning_linkml:repository_id ],
+            sh:order 2 ;
+            sh:path shareyourcloning_linkml:repository_name ],
         [ sh:datatype xsd:string ;
             sh:description "The type of the source" ;
             sh:maxCount 1 ;
             sh:order 6 ;
             sh:path shareyourcloning_linkml:type ],
         [ sh:datatype xsd:integer ;
             sh:description "A unique identifier for a thing" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 7 ;
             sh:path schema1:identifier ],
+        [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "Identifier of the sequence that is the output of this source." ;
+            sh:maxCount 1 ;
+            sh:nodeKind sh:IRI ;
+            sh:order 5 ;
+            sh:path shareyourcloning_linkml:output ],
+        [ sh:datatype xsd:string ;
+            sh:description "The id of the sequence in the repository" ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:order 3 ;
+            sh:path shareyourcloning_linkml:repository_id ],
+        [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
+            sh:nodeKind sh:IRI ;
+            sh:order 4 ;
+            sh:path shareyourcloning_linkml:input ],
         [ sh:in ( "depositor-full" "addgene-full" ) ;
             sh:maxCount 1 ;
             sh:order 1 ;
             sh:path shareyourcloning_linkml:addgene_sequence_type ],
-        [ sh:in ( "addgene" "genbank" ) ;
+        [ sh:datatype xsd:string ;
+            sh:description "The URL of a sequence file" ;
             sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 2 ;
-            sh:path shareyourcloning_linkml:repository_name ] ;
+            sh:order 0 ;
+            sh:path shareyourcloning_linkml:sequence_file_url ;
+            sh:pattern "^https?:\\/\\/(www\\.)?[-a-zA-Z0-9@:%._\\+~#=]{1,256}\\.[a-zA-Z0-9()]{1,6}\\b([-a-zA-Z0-9()@:%_\\+.~#?&//=]*)$" ] ;
     sh:targetClass shareyourcloning_linkml:AddGeneIdSource .
 
 shareyourcloning_linkml:AssemblySource a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents the source of a sequence that is an assembly of other sequences" ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:datatype xsd:string ;
-            sh:description "The type of the source" ;
-            sh:maxCount 1 ;
-            sh:order 4 ;
-            sh:path shareyourcloning_linkml:type ],
-        [ sh:datatype xsd:integer ;
-            sh:description "A unique identifier for a thing" ;
-            sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 5 ;
-            sh:path schema1:identifier ],
-        [ sh:class shareyourcloning_linkml:Sequence ;
+    sh:property [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
             sh:nodeKind sh:IRI ;
             sh:order 2 ;
             sh:path shareyourcloning_linkml:input ],
+        [ sh:datatype xsd:boolean ;
+            sh:description "Whether the assembly is circular or not" ;
+            sh:maxCount 1 ;
+            sh:order 0 ;
+            sh:path shareyourcloning_linkml:circular ],
+        [ sh:datatype xsd:string ;
+            sh:description "The type of the source" ;
+            sh:maxCount 1 ;
+            sh:order 4 ;
+            sh:path shareyourcloning_linkml:type ],
         [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "Identifier of the sequence that is the output of this source." ;
             sh:maxCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 3 ;
             sh:path shareyourcloning_linkml:output ],
-        [ sh:datatype xsd:boolean ;
-            sh:description "Whether the assembly is circular or not" ;
-            sh:maxCount 1 ;
-            sh:order 0 ;
-            sh:path shareyourcloning_linkml:circular ],
         [ sh:class shareyourcloning_linkml:AssemblyJoin ;
             sh:description "The joins between the fragments in the assembly" ;
             sh:minCount 1 ;
             sh:nodeKind sh:BlankNodeOrIRI ;
             sh:order 1 ;
-            sh:path shareyourcloning_linkml:assembly ] ;
+            sh:path shareyourcloning_linkml:assembly ],
+        [ sh:datatype xsd:integer ;
+            sh:description "A unique identifier for a thing" ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:order 5 ;
+            sh:path schema1:identifier ] ;
     sh:targetClass shareyourcloning_linkml:AssemblySource .
 
 shareyourcloning_linkml:CRISPRSource a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents the source of a sequence that is generated by CRISPR" ;
     sh:ignoredProperties ( rdf:type ) ;
     sh:property [ sh:class shareyourcloning_linkml:Sequence ;
@@ -113,773 +113,773 @@
             sh:path shareyourcloning_linkml:input ],
         [ sh:class shareyourcloning_linkml:Primer ;
             sh:description "The guide RNAs used in the CRISPR" ;
             sh:minCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 0 ;
             sh:path shareyourcloning_linkml:guides ],
-        [ sh:datatype xsd:string ;
-            sh:description "The type of the source" ;
+        [ sh:datatype xsd:integer ;
+            sh:description "A unique identifier for a thing" ;
             sh:maxCount 1 ;
-            sh:order 5 ;
-            sh:path shareyourcloning_linkml:type ],
+            sh:minCount 1 ;
+            sh:order 6 ;
+            sh:path schema1:identifier ],
         [ sh:class shareyourcloning_linkml:AssemblyJoin ;
             sh:description "The joins between the fragments in the assembly" ;
             sh:minCount 1 ;
             sh:nodeKind sh:BlankNodeOrIRI ;
             sh:order 2 ;
             sh:path shareyourcloning_linkml:assembly ],
-        [ sh:datatype xsd:integer ;
-            sh:description "A unique identifier for a thing" ;
-            sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 6 ;
-            sh:path schema1:identifier ],
         [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "Identifier of the sequence that is the output of this source." ;
             sh:maxCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 4 ;
             sh:path shareyourcloning_linkml:output ],
         [ sh:datatype xsd:boolean ;
             sh:description "Whether the assembly is circular or not" ;
             sh:maxCount 1 ;
             sh:order 1 ;
-            sh:path shareyourcloning_linkml:circular ] ;
+            sh:path shareyourcloning_linkml:circular ],
+        [ sh:datatype xsd:string ;
+            sh:description "The type of the source" ;
+            sh:maxCount 1 ;
+            sh:order 5 ;
+            sh:path shareyourcloning_linkml:type ] ;
     sh:targetClass shareyourcloning_linkml:CRISPRSource .
 
 shareyourcloning_linkml:CloningStrategy a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents a cloning strategy" ;
     sh:ignoredProperties ( rdf:type ) ;
     sh:property [ sh:class shareyourcloning_linkml:Primer ;
             sh:description "The primers that are used in the cloning strategy" ;
             sh:nodeKind sh:IRI ;
             sh:order 2 ;
             sh:path shareyourcloning_linkml:primers ],
-        [ sh:class shareyourcloning_linkml:Source ;
-            sh:description "The sources of the sequences that are used in the cloning strategy" ;
-            sh:minCount 1 ;
-            sh:nodeKind sh:IRI ;
-            sh:order 1 ;
-            sh:path shareyourcloning_linkml:sources ],
+        [ sh:datatype xsd:string ;
+            sh:description "A description of the cloning strategy" ;
+            sh:maxCount 1 ;
+            sh:order 3 ;
+            sh:path shareyourcloning_linkml:description ],
         [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "The sequences that are used in the cloning strategy" ;
             sh:minCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 0 ;
             sh:path shareyourcloning_linkml:sequences ],
-        [ sh:datatype xsd:string ;
-            sh:description "A description of the cloning strategy" ;
-            sh:maxCount 1 ;
-            sh:order 3 ;
-            sh:path shareyourcloning_linkml:description ] ;
+        [ sh:class shareyourcloning_linkml:Source ;
+            sh:description "The sources of the sequences that are used in the cloning strategy" ;
+            sh:minCount 1 ;
+            sh:nodeKind sh:IRI ;
+            sh:order 1 ;
+            sh:path shareyourcloning_linkml:sources ] ;
     sh:targetClass shareyourcloning_linkml:CloningStrategy .
 
 shareyourcloning_linkml:GenomeCoordinatesSource a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents the source of a sequence that is identified by genome coordinates, requested from NCBI" ;
     sh:ignoredProperties ( rdf:type ) ;
     sh:property [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "Identifier of the sequence that is the output of this source." ;
-            sh:maxCount 1 ;
+            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
             sh:nodeKind sh:IRI ;
-            sh:order 8 ;
-            sh:path shareyourcloning_linkml:output ],
+            sh:order 7 ;
+            sh:path shareyourcloning_linkml:input ],
         [ sh:datatype xsd:string ;
-            sh:description "The locus tag of the sequence" ;
+            sh:description "The accession of the sequence" ;
             sh:maxCount 1 ;
-            sh:order 2 ;
-            sh:path shareyourcloning_linkml:locus_tag ],
+            sh:minCount 1 ;
+            sh:order 1 ;
+            sh:path shareyourcloning_linkml:sequence_accession ],
         [ sh:datatype xsd:integer ;
-            sh:description "The starting coordinate (1-based) of the sequence in the sequence accession" ;
+            sh:description "The gene id of the sequence" ;
             sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 4 ;
-            sh:path shareyourcloning_linkml:start ],
+            sh:order 3 ;
+            sh:path shareyourcloning_linkml:gene_id ],
         [ sh:datatype xsd:integer ;
             sh:description "The ending coordinate (1-based) of the sequence in the sequence accession" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 5 ;
             sh:path shareyourcloning_linkml:end ],
         [ sh:datatype xsd:integer ;
-            sh:description "The gene id of the sequence" ;
+            sh:description "A unique identifier for a thing" ;
             sh:maxCount 1 ;
-            sh:order 3 ;
-            sh:path shareyourcloning_linkml:gene_id ],
-        [ sh:datatype xsd:string ;
-            sh:description "The accession of the sequence" ;
+            sh:minCount 1 ;
+            sh:order 10 ;
+            sh:path schema1:identifier ],
+        [ sh:datatype xsd:integer ;
+            sh:description "The strand of the sequence in the sequence accession, should be 1 or -1" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
-            sh:order 1 ;
-            sh:path shareyourcloning_linkml:sequence_accession ],
+            sh:order 6 ;
+            sh:path shareyourcloning_linkml:strand ],
         [ sh:datatype xsd:string ;
             sh:description "The type of the source" ;
             sh:maxCount 1 ;
             sh:order 9 ;
             sh:path shareyourcloning_linkml:type ],
         [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
-            sh:nodeKind sh:IRI ;
-            sh:order 7 ;
-            sh:path shareyourcloning_linkml:input ],
-        [ sh:datatype xsd:string ;
-            sh:description "The accession of the assembly" ;
+            sh:description "Identifier of the sequence that is the output of this source." ;
             sh:maxCount 1 ;
-            sh:order 0 ;
-            sh:path shareyourcloning_linkml:assembly_accession ],
+            sh:nodeKind sh:IRI ;
+            sh:order 8 ;
+            sh:path shareyourcloning_linkml:output ],
         [ sh:datatype xsd:integer ;
-            sh:description "The strand of the sequence in the sequence accession, should be 1 or -1" ;
+            sh:description "The starting coordinate (1-based) of the sequence in the sequence accession" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
-            sh:order 6 ;
-            sh:path shareyourcloning_linkml:strand ],
-        [ sh:datatype xsd:integer ;
-            sh:description "A unique identifier for a thing" ;
+            sh:order 4 ;
+            sh:path shareyourcloning_linkml:start ],
+        [ sh:datatype xsd:string ;
+            sh:description "The locus tag of the sequence" ;
             sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 10 ;
-            sh:path schema1:identifier ] ;
+            sh:order 2 ;
+            sh:path shareyourcloning_linkml:locus_tag ],
+        [ sh:datatype xsd:string ;
+            sh:description "The accession of the assembly" ;
+            sh:maxCount 1 ;
+            sh:order 0 ;
+            sh:path shareyourcloning_linkml:assembly_accession ] ;
     sh:targetClass shareyourcloning_linkml:GenomeCoordinatesSource .
 
 shareyourcloning_linkml:GibsonAssemblySource a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents the source of a sequence that is generated by Gibson assembly" ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:class shareyourcloning_linkml:AssemblyJoin ;
+    sh:property [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
+            sh:nodeKind sh:IRI ;
+            sh:order 2 ;
+            sh:path shareyourcloning_linkml:input ],
+        [ sh:class shareyourcloning_linkml:AssemblyJoin ;
             sh:description "The joins between the fragments in the assembly" ;
             sh:minCount 1 ;
             sh:nodeKind sh:BlankNodeOrIRI ;
             sh:order 1 ;
             sh:path shareyourcloning_linkml:assembly ],
-        [ sh:datatype xsd:integer ;
-            sh:description "A unique identifier for a thing" ;
-            sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 5 ;
-            sh:path schema1:identifier ],
         [ sh:datatype xsd:boolean ;
             sh:description "Whether the assembly is circular or not" ;
             sh:maxCount 1 ;
             sh:order 0 ;
             sh:path shareyourcloning_linkml:circular ],
+        [ sh:datatype xsd:string ;
+            sh:description "The type of the source" ;
+            sh:maxCount 1 ;
+            sh:order 4 ;
+            sh:path shareyourcloning_linkml:type ],
         [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "Identifier of the sequence that is the output of this source." ;
             sh:maxCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 3 ;
             sh:path shareyourcloning_linkml:output ],
-        [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
-            sh:nodeKind sh:IRI ;
-            sh:order 2 ;
-            sh:path shareyourcloning_linkml:input ],
-        [ sh:datatype xsd:string ;
-            sh:description "The type of the source" ;
+        [ sh:datatype xsd:integer ;
+            sh:description "A unique identifier for a thing" ;
             sh:maxCount 1 ;
-            sh:order 4 ;
-            sh:path shareyourcloning_linkml:type ] ;
+            sh:minCount 1 ;
+            sh:order 5 ;
+            sh:path schema1:identifier ] ;
     sh:targetClass shareyourcloning_linkml:GibsonAssemblySource .
 
 shareyourcloning_linkml:HomologousRecombinationSource a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents the source of a sequence that is generated by homologous recombination" ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:datatype xsd:string ;
+    sh:property [ sh:class shareyourcloning_linkml:AssemblyJoin ;
+            sh:description "The joins between the fragments in the assembly" ;
+            sh:minCount 1 ;
+            sh:nodeKind sh:BlankNodeOrIRI ;
+            sh:order 1 ;
+            sh:path shareyourcloning_linkml:assembly ],
+        [ sh:datatype xsd:string ;
             sh:description "The type of the source" ;
             sh:maxCount 1 ;
             sh:order 4 ;
             sh:path shareyourcloning_linkml:type ],
         [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
-            sh:nodeKind sh:IRI ;
-            sh:order 2 ;
-            sh:path shareyourcloning_linkml:input ],
-        [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "Identifier of the sequence that is the output of this source." ;
             sh:maxCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 3 ;
             sh:path shareyourcloning_linkml:output ],
-        [ sh:datatype xsd:boolean ;
-            sh:description "Whether the assembly is circular or not" ;
-            sh:maxCount 1 ;
-            sh:order 0 ;
-            sh:path shareyourcloning_linkml:circular ],
-        [ sh:class shareyourcloning_linkml:AssemblyJoin ;
-            sh:description "The joins between the fragments in the assembly" ;
-            sh:minCount 1 ;
-            sh:nodeKind sh:BlankNodeOrIRI ;
-            sh:order 1 ;
-            sh:path shareyourcloning_linkml:assembly ],
+        [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
+            sh:nodeKind sh:IRI ;
+            sh:order 2 ;
+            sh:path shareyourcloning_linkml:input ],
         [ sh:datatype xsd:integer ;
             sh:description "A unique identifier for a thing" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 5 ;
-            sh:path schema1:identifier ] ;
+            sh:path schema1:identifier ],
+        [ sh:datatype xsd:boolean ;
+            sh:description "Whether the assembly is circular or not" ;
+            sh:maxCount 1 ;
+            sh:order 0 ;
+            sh:path shareyourcloning_linkml:circular ] ;
     sh:targetClass shareyourcloning_linkml:HomologousRecombinationSource .
 
 shareyourcloning_linkml:LigationSource a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents the source of a sequence that is generated by ligation with sticky or blunt ends." ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:datatype xsd:integer ;
-            sh:description "A unique identifier for a thing" ;
-            sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 5 ;
-            sh:path schema1:identifier ],
-        [ sh:datatype xsd:string ;
-            sh:description "The type of the source" ;
-            sh:maxCount 1 ;
-            sh:order 4 ;
-            sh:path shareyourcloning_linkml:type ],
-        [ sh:datatype xsd:boolean ;
-            sh:description "Whether the assembly is circular or not" ;
-            sh:maxCount 1 ;
-            sh:order 0 ;
-            sh:path shareyourcloning_linkml:circular ],
+    sh:property [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
+            sh:nodeKind sh:IRI ;
+            sh:order 2 ;
+            sh:path shareyourcloning_linkml:input ],
         [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "Identifier of the sequence that is the output of this source." ;
             sh:maxCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 3 ;
             sh:path shareyourcloning_linkml:output ],
         [ sh:class shareyourcloning_linkml:AssemblyJoin ;
             sh:description "The joins between the fragments in the assembly" ;
             sh:minCount 1 ;
             sh:nodeKind sh:BlankNodeOrIRI ;
             sh:order 1 ;
             sh:path shareyourcloning_linkml:assembly ],
-        [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
-            sh:nodeKind sh:IRI ;
-            sh:order 2 ;
-            sh:path shareyourcloning_linkml:input ] ;
+        [ sh:datatype xsd:boolean ;
+            sh:description "Whether the assembly is circular or not" ;
+            sh:maxCount 1 ;
+            sh:order 0 ;
+            sh:path shareyourcloning_linkml:circular ],
+        [ sh:datatype xsd:integer ;
+            sh:description "A unique identifier for a thing" ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:order 5 ;
+            sh:path schema1:identifier ],
+        [ sh:datatype xsd:string ;
+            sh:description "The type of the source" ;
+            sh:maxCount 1 ;
+            sh:order 4 ;
+            sh:path shareyourcloning_linkml:type ] ;
     sh:targetClass shareyourcloning_linkml:LigationSource .
 
 shareyourcloning_linkml:ManuallyTypedSource a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents the source of a sequence that is manually typed by the user" ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:datatype xsd:string ;
-            sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 2 ;
-            sh:path shareyourcloning_linkml:user_input ;
-            sh:pattern "^[acgtACGT]+$" ],
-        [ sh:datatype xsd:boolean ;
+    sh:property [ sh:datatype xsd:boolean ;
             sh:description "Whether the sequence is circular or not" ;
             sh:maxCount 1 ;
             sh:order 3 ;
             sh:path shareyourcloning_linkml:circular ],
-        [ sh:datatype xsd:integer ;
-            sh:description "A unique identifier for a thing" ;
+        [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
+            sh:nodeKind sh:IRI ;
+            sh:order 4 ;
+            sh:path shareyourcloning_linkml:input ],
+        [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "Identifier of the sequence that is the output of this source." ;
             sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 7 ;
-            sh:path schema1:identifier ],
+            sh:nodeKind sh:IRI ;
+            sh:order 5 ;
+            sh:path shareyourcloning_linkml:output ],
         [ sh:datatype xsd:integer ;
             sh:defaultValue 0 ;
             sh:description "Taken from pydna's `dseq::ovhg`An integer describing the length of the crick strand overhang in the 5' of the molecule, or 3' of the crick strand" ;
             sh:maxCount 1 ;
             sh:order 0 ;
             sh:path shareyourcloning_linkml:overhang_crick_3prime ],
-        [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "Identifier of the sequence that is the output of this source." ;
+        [ sh:datatype xsd:string ;
             sh:maxCount 1 ;
-            sh:nodeKind sh:IRI ;
-            sh:order 5 ;
-            sh:path shareyourcloning_linkml:output ],
-        [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
-            sh:nodeKind sh:IRI ;
-            sh:order 4 ;
-            sh:path shareyourcloning_linkml:input ],
+            sh:minCount 1 ;
+            sh:order 2 ;
+            sh:path shareyourcloning_linkml:user_input ;
+            sh:pattern "^[acgtACGT]+$" ],
         [ sh:datatype xsd:integer ;
-            sh:defaultValue 0 ;
-            sh:description "The equivalent of `overhang_crick_3prime` but for the watson strand" ;
+            sh:description "A unique identifier for a thing" ;
             sh:maxCount 1 ;
-            sh:order 1 ;
-            sh:path shareyourcloning_linkml:overhang_watson_3prime ],
+            sh:minCount 1 ;
+            sh:order 7 ;
+            sh:path schema1:identifier ],
         [ sh:datatype xsd:string ;
             sh:description "The type of the source" ;
             sh:maxCount 1 ;
             sh:order 6 ;
-            sh:path shareyourcloning_linkml:type ] ;
+            sh:path shareyourcloning_linkml:type ],
+        [ sh:datatype xsd:integer ;
+            sh:defaultValue 0 ;
+            sh:description "The equivalent of `overhang_crick_3prime` but for the watson strand" ;
+            sh:maxCount 1 ;
+            sh:order 1 ;
+            sh:path shareyourcloning_linkml:overhang_watson_3prime ] ;
     sh:targetClass shareyourcloning_linkml:ManuallyTypedSource .
 
 shareyourcloning_linkml:OligoHybridizationSource a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents the source of a sequence that is generated by oligo hybridization" ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "Identifier of the sequence that is the output of this source." ;
-            sh:maxCount 1 ;
-            sh:nodeKind sh:IRI ;
-            sh:order 4 ;
-            sh:path shareyourcloning_linkml:output ],
-        [ sh:datatype xsd:string ;
-            sh:description "The type of the source" ;
-            sh:maxCount 1 ;
-            sh:order 5 ;
-            sh:path shareyourcloning_linkml:type ],
-        [ sh:datatype xsd:integer ;
+    sh:property [ sh:datatype xsd:integer ;
             sh:description "Taken from pydna's `dseq::ovhg`An integer describing the length of the crick strand overhang in the 5' of the molecule, or 3' of the crick strand" ;
             sh:maxCount 1 ;
             sh:order 0 ;
             sh:path shareyourcloning_linkml:overhang_crick_3prime ],
         [ sh:class shareyourcloning_linkml:Primer ;
-            sh:description "The reverse oligo used in the hybridization" ;
+            sh:description "The forward oligo used in the hybridization" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:nodeKind sh:IRI ;
-            sh:order 2 ;
-            sh:path shareyourcloning_linkml:reverse_oligo ],
+            sh:order 1 ;
+            sh:path shareyourcloning_linkml:forward_oligo ],
+        [ sh:datatype xsd:integer ;
+            sh:description "A unique identifier for a thing" ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:order 6 ;
+            sh:path schema1:identifier ],
         [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
             sh:nodeKind sh:IRI ;
             sh:order 3 ;
             sh:path shareyourcloning_linkml:input ],
         [ sh:class shareyourcloning_linkml:Primer ;
-            sh:description "The forward oligo used in the hybridization" ;
+            sh:description "The reverse oligo used in the hybridization" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:nodeKind sh:IRI ;
-            sh:order 1 ;
-            sh:path shareyourcloning_linkml:forward_oligo ],
-        [ sh:datatype xsd:integer ;
-            sh:description "A unique identifier for a thing" ;
+            sh:order 2 ;
+            sh:path shareyourcloning_linkml:reverse_oligo ],
+        [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "Identifier of the sequence that is the output of this source." ;
             sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 6 ;
-            sh:path schema1:identifier ] ;
+            sh:nodeKind sh:IRI ;
+            sh:order 4 ;
+            sh:path shareyourcloning_linkml:output ],
+        [ sh:datatype xsd:string ;
+            sh:description "The type of the source" ;
+            sh:maxCount 1 ;
+            sh:order 5 ;
+            sh:path shareyourcloning_linkml:type ] ;
     sh:targetClass shareyourcloning_linkml:OligoHybridizationSource .
 
 shareyourcloning_linkml:PCRSource a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents the source of a sequence that is generated by PCR" ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
-            sh:nodeKind sh:IRI ;
-            sh:order 4 ;
-            sh:path shareyourcloning_linkml:input ],
-        [ sh:class shareyourcloning_linkml:AssemblyJoin ;
+    sh:property [ sh:class shareyourcloning_linkml:AssemblyJoin ;
             sh:description "The joins between the fragments in the assembly" ;
             sh:minCount 1 ;
             sh:nodeKind sh:BlankNodeOrIRI ;
             sh:order 3 ;
             sh:path shareyourcloning_linkml:assembly ],
         [ sh:class shareyourcloning_linkml:Primer ;
             sh:description "The forward primer used in the PCR" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 0 ;
             sh:path shareyourcloning_linkml:forward_primer ],
-        [ sh:datatype xsd:boolean ;
-            sh:description "Whether the assembly is circular or not" ;
+        [ sh:datatype xsd:integer ;
+            sh:description "A unique identifier for a thing" ;
             sh:maxCount 1 ;
-            sh:order 2 ;
-            sh:path shareyourcloning_linkml:circular ],
+            sh:minCount 1 ;
+            sh:order 7 ;
+            sh:path schema1:identifier ],
         [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "Identifier of the sequence that is the output of this source." ;
             sh:maxCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 5 ;
             sh:path shareyourcloning_linkml:output ],
-        [ sh:datatype xsd:string ;
-            sh:description "The type of the source" ;
-            sh:maxCount 1 ;
-            sh:order 6 ;
-            sh:path shareyourcloning_linkml:type ],
         [ sh:class shareyourcloning_linkml:Primer ;
             sh:description "The reverse primer used in the PCR" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 1 ;
             sh:path shareyourcloning_linkml:reverse_primer ],
-        [ sh:datatype xsd:integer ;
-            sh:description "A unique identifier for a thing" ;
+        [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
+            sh:nodeKind sh:IRI ;
+            sh:order 4 ;
+            sh:path shareyourcloning_linkml:input ],
+        [ sh:datatype xsd:string ;
+            sh:description "The type of the source" ;
             sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 7 ;
-            sh:path schema1:identifier ] ;
+            sh:order 6 ;
+            sh:path shareyourcloning_linkml:type ],
+        [ sh:datatype xsd:boolean ;
+            sh:description "Whether the assembly is circular or not" ;
+            sh:maxCount 1 ;
+            sh:order 2 ;
+            sh:path shareyourcloning_linkml:circular ] ;
     sh:targetClass shareyourcloning_linkml:PCRSource .
 
 shareyourcloning_linkml:PolymeraseExtensionSource a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents the source of a sequence that is generated by polymerase extension" ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:datatype xsd:string ;
-            sh:description "The type of the source" ;
-            sh:maxCount 1 ;
-            sh:order 2 ;
-            sh:path shareyourcloning_linkml:type ],
-        [ sh:datatype xsd:integer ;
+    sh:property [ sh:datatype xsd:integer ;
             sh:description "A unique identifier for a thing" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 3 ;
             sh:path schema1:identifier ],
         [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "Identifier of the sequence that is the output of this source." ;
+            sh:maxCount 1 ;
+            sh:nodeKind sh:IRI ;
+            sh:order 1 ;
+            sh:path shareyourcloning_linkml:output ],
+        [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
             sh:nodeKind sh:IRI ;
             sh:order 0 ;
             sh:path shareyourcloning_linkml:input ],
-        [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "Identifier of the sequence that is the output of this source." ;
+        [ sh:datatype xsd:string ;
+            sh:description "The type of the source" ;
             sh:maxCount 1 ;
-            sh:nodeKind sh:IRI ;
-            sh:order 1 ;
-            sh:path shareyourcloning_linkml:output ] ;
+            sh:order 2 ;
+            sh:path shareyourcloning_linkml:type ] ;
     sh:targetClass shareyourcloning_linkml:PolymeraseExtensionSource .
 
 shareyourcloning_linkml:RepositoryIdSource a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents the source of a sequence that is identified by a repository id" ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
-            sh:nodeKind sh:IRI ;
-            sh:order 2 ;
-            sh:path shareyourcloning_linkml:input ],
-        [ sh:datatype xsd:string ;
+    sh:property [ sh:datatype xsd:string ;
             sh:description "The id of the sequence in the repository" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 1 ;
             sh:path shareyourcloning_linkml:repository_id ],
-        [ sh:in ( "addgene" "genbank" ) ;
-            sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 0 ;
-            sh:path shareyourcloning_linkml:repository_name ],
         [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "Identifier of the sequence that is the output of this source." ;
-            sh:maxCount 1 ;
+            sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
             sh:nodeKind sh:IRI ;
-            sh:order 3 ;
-            sh:path shareyourcloning_linkml:output ],
+            sh:order 2 ;
+            sh:path shareyourcloning_linkml:input ],
         [ sh:datatype xsd:integer ;
             sh:description "A unique identifier for a thing" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 5 ;
             sh:path schema1:identifier ],
+        [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "Identifier of the sequence that is the output of this source." ;
+            sh:maxCount 1 ;
+            sh:nodeKind sh:IRI ;
+            sh:order 3 ;
+            sh:path shareyourcloning_linkml:output ],
         [ sh:datatype xsd:string ;
             sh:description "The type of the source" ;
             sh:maxCount 1 ;
             sh:order 4 ;
-            sh:path shareyourcloning_linkml:type ] ;
+            sh:path shareyourcloning_linkml:type ],
+        [ sh:in ( "addgene" "genbank" ) ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:order 0 ;
+            sh:path shareyourcloning_linkml:repository_name ] ;
     sh:targetClass shareyourcloning_linkml:RepositoryIdSource .
 
 shareyourcloning_linkml:RestrictionAndLigationSource a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents the source of a sequence that is generated by restriction and ligation" ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:datatype xsd:integer ;
-            sh:description "A unique identifier for a thing" ;
-            sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 6 ;
-            sh:path schema1:identifier ],
-        [ sh:class shareyourcloning_linkml:Sequence ;
+    sh:property [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
             sh:nodeKind sh:IRI ;
             sh:order 3 ;
             sh:path shareyourcloning_linkml:input ],
         [ sh:datatype xsd:string ;
             sh:description "The type of the source" ;
             sh:maxCount 1 ;
             sh:order 5 ;
             sh:path shareyourcloning_linkml:type ],
-        [ sh:datatype xsd:string ;
-            sh:minCount 1 ;
-            sh:order 0 ;
-            sh:path shareyourcloning_linkml:restriction_enzymes ],
-        [ sh:datatype xsd:boolean ;
-            sh:description "Whether the assembly is circular or not" ;
-            sh:maxCount 1 ;
-            sh:order 1 ;
-            sh:path shareyourcloning_linkml:circular ],
         [ sh:class shareyourcloning_linkml:AssemblyJoin ;
             sh:description "The joins between the fragments in the assembly" ;
             sh:minCount 1 ;
             sh:nodeKind sh:BlankNodeOrIRI ;
             sh:order 2 ;
             sh:path shareyourcloning_linkml:assembly ],
         [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "Identifier of the sequence that is the output of this source." ;
             sh:maxCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 4 ;
-            sh:path shareyourcloning_linkml:output ] ;
+            sh:path shareyourcloning_linkml:output ],
+        [ sh:datatype xsd:integer ;
+            sh:description "A unique identifier for a thing" ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:order 6 ;
+            sh:path schema1:identifier ],
+        [ sh:datatype xsd:string ;
+            sh:minCount 1 ;
+            sh:order 0 ;
+            sh:path shareyourcloning_linkml:restriction_enzymes ],
+        [ sh:datatype xsd:boolean ;
+            sh:description "Whether the assembly is circular or not" ;
+            sh:maxCount 1 ;
+            sh:order 1 ;
+            sh:path shareyourcloning_linkml:circular ] ;
     sh:targetClass shareyourcloning_linkml:RestrictionAndLigationSource .
 
 shareyourcloning_linkml:RestrictionEnzymeDigestionSource a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents the source of a sequence that is a subfragment of another sequence, generated by sequence cutting using restriction enzymes." ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:class shareyourcloning_linkml:RestrictionSequenceCut ;
-            sh:maxCount 1 ;
-            sh:nodeKind sh:BlankNodeOrIRI ;
-            sh:order 0 ;
-            sh:path shareyourcloning_linkml:left_edge ],
-        [ sh:class shareyourcloning_linkml:RestrictionSequenceCut ;
-            sh:maxCount 1 ;
-            sh:nodeKind sh:BlankNodeOrIRI ;
-            sh:order 1 ;
-            sh:path shareyourcloning_linkml:right_edge ],
-        [ sh:datatype xsd:string ;
-            sh:description "The type of the source" ;
-            sh:maxCount 1 ;
-            sh:order 4 ;
-            sh:path shareyourcloning_linkml:type ],
-        [ sh:class shareyourcloning_linkml:Sequence ;
+    sh:property [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
             sh:nodeKind sh:IRI ;
             sh:order 2 ;
             sh:path shareyourcloning_linkml:input ],
         [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "Identifier of the sequence that is the output of this source." ;
             sh:maxCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 3 ;
             sh:path shareyourcloning_linkml:output ],
+        [ sh:class shareyourcloning_linkml:RestrictionSequenceCut ;
+            sh:maxCount 1 ;
+            sh:nodeKind sh:BlankNodeOrIRI ;
+            sh:order 0 ;
+            sh:path shareyourcloning_linkml:left_edge ],
+        [ sh:datatype xsd:string ;
+            sh:description "The type of the source" ;
+            sh:maxCount 1 ;
+            sh:order 4 ;
+            sh:path shareyourcloning_linkml:type ],
         [ sh:datatype xsd:integer ;
             sh:description "A unique identifier for a thing" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 5 ;
-            sh:path schema1:identifier ] ;
+            sh:path schema1:identifier ],
+        [ sh:class shareyourcloning_linkml:RestrictionSequenceCut ;
+            sh:maxCount 1 ;
+            sh:nodeKind sh:BlankNodeOrIRI ;
+            sh:order 1 ;
+            sh:path shareyourcloning_linkml:right_edge ] ;
     sh:targetClass shareyourcloning_linkml:RestrictionEnzymeDigestionSource .
 
 shareyourcloning_linkml:SequenceCutSource a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents the source of a sequence that is a subfragment of another sequence, generated by sequence cutting." ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:class shareyourcloning_linkml:SequenceCut ;
-            sh:maxCount 1 ;
-            sh:nodeKind sh:BlankNodeOrIRI ;
-            sh:order 0 ;
-            sh:path shareyourcloning_linkml:left_edge ],
-        [ sh:datatype xsd:integer ;
-            sh:description "A unique identifier for a thing" ;
-            sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 5 ;
-            sh:path schema1:identifier ],
-        [ sh:datatype xsd:string ;
+    sh:property [ sh:datatype xsd:string ;
             sh:description "The type of the source" ;
             sh:maxCount 1 ;
             sh:order 4 ;
             sh:path shareyourcloning_linkml:type ],
         [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
             sh:nodeKind sh:IRI ;
             sh:order 2 ;
             sh:path shareyourcloning_linkml:input ],
         [ sh:class shareyourcloning_linkml:SequenceCut ;
             sh:maxCount 1 ;
             sh:nodeKind sh:BlankNodeOrIRI ;
             sh:order 1 ;
             sh:path shareyourcloning_linkml:right_edge ],
+        [ sh:datatype xsd:integer ;
+            sh:description "A unique identifier for a thing" ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:order 5 ;
+            sh:path schema1:identifier ],
         [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "Identifier of the sequence that is the output of this source." ;
             sh:maxCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 3 ;
-            sh:path shareyourcloning_linkml:output ] ;
+            sh:path shareyourcloning_linkml:output ],
+        [ sh:class shareyourcloning_linkml:SequenceCut ;
+            sh:maxCount 1 ;
+            sh:nodeKind sh:BlankNodeOrIRI ;
+            sh:order 0 ;
+            sh:path shareyourcloning_linkml:left_edge ] ;
     sh:targetClass shareyourcloning_linkml:SequenceCutSource .
 
 shareyourcloning_linkml:TextFileSequence a sh:NodeShape ;
     sh:closed true ;
     sh:description "A sequence (may have features) defined by the content of a text file" ;
     sh:ignoredProperties ( rdf:type ) ;
     sh:property [ sh:datatype xsd:integer ;
-            sh:defaultValue 0 ;
-            sh:description "The equivalent of `overhang_crick_3prime` but for the watson strand" ;
-            sh:maxCount 1 ;
-            sh:order 2 ;
-            sh:path shareyourcloning_linkml:overhang_watson_3prime ],
-        [ sh:description "The format of a sequence file" ;
-            sh:in ( "fasta" "genbank" "snapgene" ) ;
-            sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 0 ;
-            sh:path shareyourcloning_linkml:sequence_file_format ],
-        [ sh:datatype xsd:string ;
-            sh:description "The type of the source" ;
-            sh:maxCount 1 ;
-            sh:order 5 ;
-            sh:path shareyourcloning_linkml:type ],
-        [ sh:datatype xsd:integer ;
             sh:description "A unique identifier for a thing" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 4 ;
             sh:path schema1:identifier ],
+        [ sh:datatype xsd:integer ;
+            sh:defaultValue 0 ;
+            sh:description "Taken from pydna's `dseq::ovhg`An integer describing the length of the crick strand overhang in the 5' of the molecule, or 3' of the crick strand" ;
+            sh:maxCount 1 ;
+            sh:order 1 ;
+            sh:path shareyourcloning_linkml:overhang_crick_3prime ],
         [ sh:datatype xsd:string ;
             sh:maxCount 1 ;
             sh:order 3 ;
             sh:path shareyourcloning_linkml:file_content ],
         [ sh:datatype xsd:integer ;
             sh:defaultValue 0 ;
-            sh:description "Taken from pydna's `dseq::ovhg`An integer describing the length of the crick strand overhang in the 5' of the molecule, or 3' of the crick strand" ;
+            sh:description "The equivalent of `overhang_crick_3prime` but for the watson strand" ;
             sh:maxCount 1 ;
-            sh:order 1 ;
-            sh:path shareyourcloning_linkml:overhang_crick_3prime ] ;
+            sh:order 2 ;
+            sh:path shareyourcloning_linkml:overhang_watson_3prime ],
+        [ sh:datatype xsd:string ;
+            sh:description "The type of the source" ;
+            sh:maxCount 1 ;
+            sh:order 5 ;
+            sh:path shareyourcloning_linkml:type ],
+        [ sh:description "The format of a sequence file" ;
+            sh:in ( "fasta" "genbank" "snapgene" ) ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:order 0 ;
+            sh:path shareyourcloning_linkml:sequence_file_format ] ;
     sh:targetClass shareyourcloning_linkml:TextFileSequence .
 
 shareyourcloning_linkml:UploadedFileSource a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents the source of a sequence that is uploaded as a file" ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:description "Identifier of the sequence that is the output of this source." ;
+    sh:property [ sh:description "The format of a sequence file" ;
+            sh:in ( "fasta" "genbank" "snapgene" ) ;
             sh:maxCount 1 ;
-            sh:nodeKind sh:IRI ;
-            sh:order 4 ;
-            sh:path shareyourcloning_linkml:output ],
+            sh:minCount 1 ;
+            sh:order 0 ;
+            sh:path shareyourcloning_linkml:sequence_file_format ],
         [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
             sh:nodeKind sh:IRI ;
             sh:order 3 ;
             sh:path shareyourcloning_linkml:input ],
-        [ sh:description "The format of a sequence file" ;
-            sh:in ( "fasta" "genbank" "snapgene" ) ;
+        [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:description "Identifier of the sequence that is the output of this source." ;
             sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 0 ;
-            sh:path shareyourcloning_linkml:sequence_file_format ],
+            sh:nodeKind sh:IRI ;
+            sh:order 4 ;
+            sh:path shareyourcloning_linkml:output ],
         [ sh:datatype xsd:integer ;
-            sh:description "The index of the sequence in the file" ;
+            sh:description "A unique identifier for a thing" ;
             sh:maxCount 1 ;
-            sh:order 2 ;
-            sh:path shareyourcloning_linkml:index_in_file ],
+            sh:minCount 1 ;
+            sh:order 6 ;
+            sh:path schema1:identifier ],
         [ sh:datatype xsd:string ;
             sh:description "The name of the file" ;
             sh:maxCount 1 ;
             sh:order 1 ;
             sh:path shareyourcloning_linkml:file_name ],
-        [ sh:datatype xsd:integer ;
-            sh:description "A unique identifier for a thing" ;
-            sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 6 ;
-            sh:path schema1:identifier ],
         [ sh:datatype xsd:string ;
             sh:description "The type of the source" ;
             sh:maxCount 1 ;
             sh:order 5 ;
-            sh:path shareyourcloning_linkml:type ] ;
+            sh:path shareyourcloning_linkml:type ],
+        [ sh:datatype xsd:integer ;
+            sh:description "The index of the sequence in the file" ;
+            sh:maxCount 1 ;
+            sh:order 2 ;
+            sh:path shareyourcloning_linkml:index_in_file ] ;
     sh:targetClass shareyourcloning_linkml:UploadedFileSource .
 
 shareyourcloning_linkml:SimpleSequenceLocation a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents a location within a sequence, for now support for ranges only" ;
     sh:ignoredProperties ( rdf:type ) ;
     sh:property [ sh:datatype xsd:integer ;
             sh:description "The starting coordinate (1-based) of the location" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 0 ;
             sh:path shareyourcloning_linkml:start ],
         [ sh:datatype xsd:integer ;
+            sh:description "The strand of the location, should be 1 or -1 or null" ;
+            sh:maxCount 1 ;
+            sh:order 2 ;
+            sh:path shareyourcloning_linkml:strand ],
+        [ sh:datatype xsd:integer ;
             sh:description "The ending coordinate (1-based) of the location" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 1 ;
-            sh:path shareyourcloning_linkml:end ],
-        [ sh:datatype xsd:integer ;
-            sh:description "The strand of the location, should be 1 or -1 or null" ;
-            sh:maxCount 1 ;
-            sh:order 2 ;
-            sh:path shareyourcloning_linkml:strand ] ;
+            sh:path shareyourcloning_linkml:end ] ;
     sh:targetClass shareyourcloning_linkml:SimpleSequenceLocation .
 
 shareyourcloning_linkml:Source a sh:NodeShape ;
     sh:closed false ;
     sh:description "Represents the source of a sequence" ;
     sh:ignoredProperties ( rdf:type ) ;
     sh:property [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "Identifier of the sequence that is the output of this source." ;
             sh:maxCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 1 ;
             sh:path shareyourcloning_linkml:output ],
-        [ sh:datatype xsd:string ;
-            sh:description "The type of the source" ;
-            sh:maxCount 1 ;
-            sh:order 2 ;
-            sh:path shareyourcloning_linkml:type ],
         [ sh:class shareyourcloning_linkml:Sequence ;
             sh:description "The sequences that are an input to this source. If the source represents external import of a sequence, it's empty." ;
             sh:nodeKind sh:IRI ;
             sh:order 0 ;
             sh:path shareyourcloning_linkml:input ],
         [ sh:datatype xsd:integer ;
             sh:description "A unique identifier for a thing" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 3 ;
-            sh:path schema1:identifier ] ;
+            sh:path schema1:identifier ],
+        [ sh:datatype xsd:string ;
+            sh:description "The type of the source" ;
+            sh:maxCount 1 ;
+            sh:order 2 ;
+            sh:path shareyourcloning_linkml:type ] ;
     sh:targetClass shareyourcloning_linkml:Source .
 
 shareyourcloning_linkml:AssemblyJoinComponent a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents a component of a join between two fragments in an assembly" ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:class shareyourcloning_linkml:Sequence ;
-            sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:nodeKind sh:IRI ;
-            sh:order 0 ;
-            sh:path shareyourcloning_linkml:sequence ],
-        [ sh:class shareyourcloning_linkml:SimpleSequenceLocation ;
+    sh:property [ sh:class shareyourcloning_linkml:SimpleSequenceLocation ;
             sh:description "Location of the overlap in the fragment. Might be an empty location (start == end) to indicate blunt join." ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:nodeKind sh:BlankNodeOrIRI ;
             sh:order 1 ;
             sh:path shareyourcloning_linkml:location ],
+        [ sh:class shareyourcloning_linkml:Sequence ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:nodeKind sh:IRI ;
+            sh:order 0 ;
+            sh:path shareyourcloning_linkml:sequence ],
         [ sh:datatype xsd:boolean ;
             sh:description "Whether the sequence is reverse complemented in the join" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 2 ;
             sh:path shareyourcloning_linkml:reverse_complemented ] ;
     sh:targetClass shareyourcloning_linkml:AssemblyJoinComponent .
 
 shareyourcloning_linkml:RestrictionSequenceCut a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents a cut in a DNA sequence that is made by a restriction enzyme" ;
     sh:ignoredProperties ( rdf:type ) ;
     sh:property [ sh:datatype xsd:integer ;
-            sh:description "The length of the overhang that is left after the cut. It can be negative, same meaning as in pydna's `dseq::ovhg` and biopython's `Bio.Restriction.RestrictionType.ovhg`." ;
+            sh:description "The position of the cut in the watson strand. The cut is made before the base at this position (zero-based), so that cut position 1 cuts after the first base." ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
-            sh:order 2 ;
-            sh:path shareyourcloning_linkml:overhang ],
+            sh:order 1 ;
+            sh:path shareyourcloning_linkml:cut_watson ],
         [ sh:datatype xsd:string ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 0 ;
             sh:path shareyourcloning_linkml:restriction_enzyme ],
         [ sh:datatype xsd:integer ;
-            sh:description "The position of the cut in the watson strand. The cut is made before the base at this position (zero-based), so that cut position 1 cuts after the first base." ;
+            sh:description "The length of the overhang that is left after the cut. It can be negative, same meaning as in pydna's `dseq::ovhg` and biopython's `Bio.Restriction.RestrictionType.ovhg`." ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
-            sh:order 1 ;
-            sh:path shareyourcloning_linkml:cut_watson ] ;
+            sh:order 2 ;
+            sh:path shareyourcloning_linkml:overhang ] ;
     sh:targetClass shareyourcloning_linkml:RestrictionSequenceCut .
 
 shareyourcloning_linkml:SequenceCut a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents a cut in a DNA sequence" ;
     sh:ignoredProperties ( rdf:type ) ;
     sh:property [ sh:datatype xsd:integer ;
@@ -896,35 +896,35 @@
             sh:path shareyourcloning_linkml:cut_watson ] ;
     sh:targetClass shareyourcloning_linkml:SequenceCut .
 
 shareyourcloning_linkml:Primer a sh:NodeShape ;
     sh:closed true ;
     sh:description "An oligonucleotide or primer" ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:datatype xsd:integer ;
+    sh:property [ sh:datatype xsd:string ;
+            sh:maxCount 1 ;
+            sh:order 1 ;
+            sh:path shareyourcloning_linkml:sequence ;
+            sh:pattern "^[acgtACGT]+$" ],
+        [ sh:datatype xsd:string ;
+            sh:description "A human-readable name for a thing" ;
+            sh:maxCount 1 ;
+            sh:order 0 ;
+            sh:path schema1:name ],
+        [ sh:datatype xsd:integer ;
             sh:description "A unique identifier for a thing" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 2 ;
             sh:path schema1:identifier ],
         [ sh:datatype xsd:string ;
             sh:description "The type of the source" ;
             sh:maxCount 1 ;
             sh:order 3 ;
-            sh:path shareyourcloning_linkml:type ],
-        [ sh:datatype xsd:string ;
-            sh:maxCount 1 ;
-            sh:order 1 ;
-            sh:path shareyourcloning_linkml:sequence ;
-            sh:pattern "^[acgtACGT]+$" ],
-        [ sh:datatype xsd:string ;
-            sh:description "A human-readable name for a thing" ;
-            sh:maxCount 1 ;
-            sh:order 0 ;
-            sh:path schema1:name ] ;
+            sh:path shareyourcloning_linkml:type ] ;
     sh:targetClass shareyourcloning_linkml:Primer .
 
 shareyourcloning_linkml:AssemblyJoin a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents a joint between two fragments in an assembly" ;
     sh:ignoredProperties ( rdf:type ) ;
     sh:property [ sh:class shareyourcloning_linkml:AssemblyJoinComponent ;
```

### Comparing `shareyourcloning_linkml-0.1.4a0/project/shex/shareyourcloning_linkml.shex` & `shareyourcloning_linkml-0.1.5a0/project/shex/shareyourcloning_linkml.shex`

 * *Files identical despite different names*

### Comparing `shareyourcloning_linkml-0.1.4a0/project/sqlschema/shareyourcloning_linkml.sql` & `shareyourcloning_linkml-0.1.5a0/project/sqlschema/shareyourcloning_linkml.sql`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 --     * Slot: id Description: A unique identifier for a thing
 --     * Slot: type Description: The type of the source
 -- # Class: "Primer" Description: "An oligonucleotide or primer"
 --     * Slot: name Description: A human-readable name for a thing
 --     * Slot: sequence Description:
 --     * Slot: id Description: A unique identifier for a thing
 --     * Slot: type Description: The type of the source
+--     * Slot: CloningStrategy_id Description: Autocreated FK slot
 -- # Class: "SequenceCut" Description: "Represents a cut in a DNA sequence"
 --     * Slot: id Description:
 --     * Slot: cut_watson Description: The position of the cut in the watson strand. The cut is made before the base at this position (zero-based), so that cut position 1 cuts after the first base.
 --     * Slot: overhang Description: The length of the overhang that is left after the cut. It can be negative, same meaning as in pydna's `dseq::ovhg` and biopython's `Bio.Restriction.RestrictionType.ovhg`.
 -- # Class: "RestrictionSequenceCut" Description: "Represents a cut in a DNA sequence that is made by a restriction enzyme"
 --     * Slot: id Description:
 --     * Slot: restriction_enzyme Description:
@@ -207,38 +208,28 @@
 --     * Slot: input_id Description: The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.
 -- # Class: "OligoHybridizationSource_input" Description: ""
 --     * Slot: OligoHybridizationSource_id Description: Autocreated FK slot
 --     * Slot: input_id Description: The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.
 -- # Class: "PolymeraseExtensionSource_input" Description: ""
 --     * Slot: PolymeraseExtensionSource_id Description: Autocreated FK slot
 --     * Slot: input_id Description: The sequences that are an input to this source. If the source represents external import of a sequence, it's empty.
--- # Class: "CloningStrategy_primers" Description: ""
---     * Slot: CloningStrategy_id Description: Autocreated FK slot
---     * Slot: primers_id Description: The primers that are used in the cloning strategy
 
 CREATE TABLE "NamedThing" (
 	id INTEGER NOT NULL,
 	PRIMARY KEY (id)
 );
 CREATE TABLE "TextFileSequence" (
 	sequence_file_format VARCHAR(8) NOT NULL,
 	overhang_crick_3prime INTEGER,
 	overhang_watson_3prime INTEGER,
 	file_content TEXT,
 	id INTEGER NOT NULL,
 	type TEXT,
 	PRIMARY KEY (id)
 );
-CREATE TABLE "Primer" (
-	name TEXT,
-	sequence TEXT,
-	id INTEGER NOT NULL,
-	type TEXT,
-	PRIMARY KEY (id)
-);
 CREATE TABLE "SequenceCut" (
 	id INTEGER NOT NULL,
 	cut_watson INTEGER NOT NULL,
 	overhang INTEGER NOT NULL,
 	PRIMARY KEY (id)
 );
 CREATE TABLE "RestrictionSequenceCut" (
@@ -263,20 +254,22 @@
 CREATE TABLE "Sequence" (
 	id INTEGER NOT NULL,
 	type TEXT,
 	"CloningStrategy_id" INTEGER,
 	PRIMARY KEY (id),
 	FOREIGN KEY("CloningStrategy_id") REFERENCES "CloningStrategy" (id)
 );
-CREATE TABLE "CloningStrategy_primers" (
+CREATE TABLE "Primer" (
+	name TEXT,
+	sequence TEXT,
+	id INTEGER NOT NULL,
+	type TEXT,
 	"CloningStrategy_id" INTEGER,
-	primers_id INTEGER,
-	PRIMARY KEY ("CloningStrategy_id", primers_id),
-	FOREIGN KEY("CloningStrategy_id") REFERENCES "CloningStrategy" (id),
-	FOREIGN KEY(primers_id) REFERENCES "Primer" (id)
+	PRIMARY KEY (id),
+	FOREIGN KEY("CloningStrategy_id") REFERENCES "CloningStrategy" (id)
 );
 CREATE TABLE "Source" (
 	output INTEGER,
 	type TEXT,
 	id INTEGER NOT NULL,
 	"CloningStrategy_id" INTEGER,
 	PRIMARY KEY (id),
```

### Comparing `shareyourcloning_linkml-0.1.4a0/pyproject.toml` & `shareyourcloning_linkml-0.1.5a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 authors = ["Manuel Lera-Ramirez <manuel.lera-ramirez@ucl.ac.uk>"]
 description = "A LinkML data model for ShareYourCloning"
 include = ["README.md", "src/shareyourcloning_linkml/schema", "project"]
 license = "MIT"
 name = "shareyourcloning-linkml"
 readme = "README.md"
-version = "0.1.4a0"
+version = "0.1.5a0"
 
 homepage = "https://github.com/genestorian/ShareYourCloning_LinkML"
 repository = "https://github.com/genestorian/ShareYourCloning_LinkML"
 documentation = "https://genestorian.github.io/ShareYourCloning_LinkML"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `shareyourcloning_linkml-0.1.4a0/src/shareyourcloning_linkml/datamodel/_models.py` & `shareyourcloning_linkml-0.1.5a0/src/shareyourcloning_linkml/datamodel/_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -576,15 +576,15 @@
             CRISPRSource,
             RestrictionEnzymeDigestionSource,
             AddGeneIdSource,
         ]
     ] = Field(
         default_factory=list, description="""The sources of the sequences that are used in the cloning strategy"""
     )
-    primers: Optional[List[int]] = Field(
+    primers: Optional[List[Primer]] = Field(
         default_factory=list, description="""The primers that are used in the cloning strategy"""
     )
     description: Optional[str] = Field(None, description="""A description of the cloning strategy""")
 
 
 # Model rebuild
 # see https://pydantic-docs.helpmanual.io/usage/models/#rebuilding-a-model
```

### Comparing `shareyourcloning_linkml-0.1.4a0/src/shareyourcloning_linkml/schema/shareyourcloning_linkml.yaml` & `shareyourcloning_linkml-0.1.5a0/src/shareyourcloning_linkml/schema/shareyourcloning_linkml.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -463,14 +463,15 @@
           inlined_as_list: true
       - primers:
           range: Primer
           description: >-
             The primers that are used in the cloning strategy
           required: false
           multivalued: true
+          inlined_as_list: true
       - description:
           range: string
           description: >-
             A description of the cloning strategy
 
 slots:
   id:
```

### Comparing `shareyourcloning_linkml-0.1.4a0/PKG-INFO` & `shareyourcloning_linkml-0.1.5a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareyourcloning-linkml
-Version: 0.1.4a0
+Version: 0.1.5a0
 Summary: A LinkML data model for ShareYourCloning
 Home-page: https://github.com/genestorian/ShareYourCloning_LinkML
 License: MIT
 Author: Manuel Lera-Ramirez
 Author-email: manuel.lera-ramirez@ucl.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
```

