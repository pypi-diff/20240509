# Comparing `tmp/pytextclassifier-1.3.7.tar.gz` & `tmp/pytextclassifier-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytextclassifier-1.3.7.tar", last modified: Wed Oct 18 07:57:09 2023, max compression
+gzip compressed data, was "pytextclassifier-1.3.8.tar", last modified: Thu May  9 02:21:46 2024, max compression
```

## Comparing `pytextclassifier-1.3.7.tar` & `pytextclassifier-1.3.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-10-18 07:57:09.880955 pytextclassifier-1.3.7/
--rw-r--r--   0 xuming     (501) staff       (20)    11357 2021-08-05 02:59:50.000000 pytextclassifier-1.3.7/LICENSE
--rw-r--r--   0 xuming     (501) staff       (20)    27157 2023-10-18 07:57:09.881317 pytextclassifier-1.3.7/PKG-INFO
--rw-r--r--   0 xuming     (501) staff       (20)    21984 2023-09-18 09:23:37.000000 pytextclassifier-1.3.7/README.md
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-10-18 07:57:09.876636 pytextclassifier-1.3.7/examples/
--rw-r--r--   0 xuming     (501) staff       (20)   616465 2022-03-29 07:45:47.000000 pytextclassifier-1.3.7/examples/thucnews_train_1w.txt
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-10-18 07:57:09.874305 pytextclassifier-1.3.7/pytextclassifier/
--rw-r--r--   0 xuming     (501) staff       (20)      640 2023-10-18 07:55:33.000000 pytextclassifier-1.3.7/pytextclassifier/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     2468 2023-06-14 12:38:54.000000 pytextclassifier-1.3.7/pytextclassifier/base_classifier.py
--rw-r--r--   0 xuming     (501) staff       (20)    39035 2023-06-14 12:38:54.000000 pytextclassifier-1.3.7/pytextclassifier/bert_classfication_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)    87598 2023-10-18 04:05:37.000000 pytextclassifier-1.3.7/pytextclassifier/bert_classification_model.py
--rw-r--r--   0 xuming     (501) staff       (20)    11170 2023-10-18 06:29:12.000000 pytextclassifier-1.3.7/pytextclassifier/bert_classifier.py
--rwxr-xr-x   0 xuming     (501) staff       (20)    29987 2023-05-09 08:58:29.000000 pytextclassifier-1.3.7/pytextclassifier/bert_multi_label_classification_model.py
--rw-r--r--   0 xuming     (501) staff       (20)    11050 2023-10-18 04:08:34.000000 pytextclassifier-1.3.7/pytextclassifier/classic_classifier.py
--rw-r--r--   0 xuming     (501) staff       (20)     1329 2023-10-18 04:08:34.000000 pytextclassifier-1.3.7/pytextclassifier/data_helper.py
--rw-r--r--   0 xuming     (501) staff       (20)    21704 2023-10-18 04:11:21.000000 pytextclassifier-1.3.7/pytextclassifier/fasttext_classifier.py
--rw-r--r--   0 xuming     (501) staff       (20)    17438 2021-10-25 11:27:11.000000 pytextclassifier-1.3.7/pytextclassifier/stopwords.txt
--rw-r--r--   0 xuming     (501) staff       (20)     7304 2023-05-09 08:44:44.000000 pytextclassifier-1.3.7/pytextclassifier/textcluster.py
--rw-r--r--   0 xuming     (501) staff       (20)    19072 2023-10-18 04:11:21.000000 pytextclassifier-1.3.7/pytextclassifier/textcnn_classifier.py
--rw-r--r--   0 xuming     (501) staff       (20)    19709 2023-10-18 04:11:21.000000 pytextclassifier-1.3.7/pytextclassifier/textrnn_classifier.py
--rw-r--r--   0 xuming     (501) staff       (20)      852 2022-04-12 06:51:36.000000 pytextclassifier-1.3.7/pytextclassifier/time_util.py
--rw-r--r--   0 xuming     (501) staff       (20)     2331 2023-06-14 12:38:54.000000 pytextclassifier-1.3.7/pytextclassifier/tokenizer.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-10-18 07:57:09.876361 pytextclassifier-1.3.7/pytextclassifier.egg-info/
--rw-r--r--   0 xuming     (501) staff       (20)    27157 2023-10-18 07:57:09.000000 pytextclassifier-1.3.7/pytextclassifier.egg-info/PKG-INFO
--rw-r--r--   0 xuming     (501) staff       (20)      848 2023-10-18 07:57:09.000000 pytextclassifier-1.3.7/pytextclassifier.egg-info/SOURCES.txt
--rw-r--r--   0 xuming     (501) staff       (20)        1 2023-10-18 07:57:09.000000 pytextclassifier-1.3.7/pytextclassifier.egg-info/dependency_links.txt
--rw-r--r--   0 xuming     (501) staff       (20)       52 2023-10-18 07:57:09.000000 pytextclassifier-1.3.7/pytextclassifier.egg-info/requires.txt
--rw-r--r--   0 xuming     (501) staff       (20)       17 2023-10-18 07:57:09.000000 pytextclassifier-1.3.7/pytextclassifier.egg-info/top_level.txt
--rw-r--r--   0 xuming     (501) staff       (20)      309 2023-10-18 07:57:09.881834 pytextclassifier-1.3.7/setup.cfg
--rw-r--r--   0 xuming     (501) staff       (20)     1444 2023-10-18 07:55:33.000000 pytextclassifier-1.3.7/setup.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2024-05-09 02:21:46.043271 pytextclassifier-1.3.8/
+-rw-r--r--   0 xuming     (501) staff       (20)    11357 2021-08-05 02:59:50.000000 pytextclassifier-1.3.8/LICENSE
+-rw-r--r--   0 xuming     (501) staff       (20)    22590 2024-05-09 02:21:46.043678 pytextclassifier-1.3.8/PKG-INFO
+-rw-r--r--   0 xuming     (501) staff       (20)    21802 2024-05-09 02:20:52.000000 pytextclassifier-1.3.8/README.md
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2024-05-09 02:21:46.041489 pytextclassifier-1.3.8/examples/
+-rw-r--r--   0 xuming     (501) staff       (20)   616465 2022-03-29 07:45:47.000000 pytextclassifier-1.3.8/examples/thucnews_train_1w.txt
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2024-05-09 02:21:46.038761 pytextclassifier-1.3.8/pytextclassifier/
+-rw-r--r--   0 xuming     (501) staff       (20)      640 2024-05-09 02:20:26.000000 pytextclassifier-1.3.8/pytextclassifier/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     2468 2023-06-14 12:38:54.000000 pytextclassifier-1.3.8/pytextclassifier/base_classifier.py
+-rw-r--r--   0 xuming     (501) staff       (20)    39035 2023-06-14 12:38:54.000000 pytextclassifier-1.3.8/pytextclassifier/bert_classfication_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)    87597 2024-05-09 02:10:56.000000 pytextclassifier-1.3.8/pytextclassifier/bert_classification_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)    11338 2024-05-09 02:17:22.000000 pytextclassifier-1.3.8/pytextclassifier/bert_classifier.py
+-rwxr-xr-x   0 xuming     (501) staff       (20)    29987 2023-05-09 08:58:29.000000 pytextclassifier-1.3.8/pytextclassifier/bert_multi_label_classification_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)    11050 2023-10-18 04:08:34.000000 pytextclassifier-1.3.8/pytextclassifier/classic_classifier.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1329 2023-10-18 04:08:34.000000 pytextclassifier-1.3.8/pytextclassifier/data_helper.py
+-rw-r--r--   0 xuming     (501) staff       (20)    21704 2023-10-18 04:11:21.000000 pytextclassifier-1.3.8/pytextclassifier/fasttext_classifier.py
+-rw-r--r--   0 xuming     (501) staff       (20)    17438 2021-10-25 11:27:11.000000 pytextclassifier-1.3.8/pytextclassifier/stopwords.txt
+-rw-r--r--   0 xuming     (501) staff       (20)     7304 2023-05-09 08:44:44.000000 pytextclassifier-1.3.8/pytextclassifier/textcluster.py
+-rw-r--r--   0 xuming     (501) staff       (20)    19072 2023-10-18 04:11:21.000000 pytextclassifier-1.3.8/pytextclassifier/textcnn_classifier.py
+-rw-r--r--   0 xuming     (501) staff       (20)    19709 2023-10-18 04:11:21.000000 pytextclassifier-1.3.8/pytextclassifier/textrnn_classifier.py
+-rw-r--r--   0 xuming     (501) staff       (20)      852 2022-04-12 06:51:36.000000 pytextclassifier-1.3.8/pytextclassifier/time_util.py
+-rw-r--r--   0 xuming     (501) staff       (20)     2331 2023-06-14 12:38:54.000000 pytextclassifier-1.3.8/pytextclassifier/tokenizer.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2024-05-09 02:21:46.041074 pytextclassifier-1.3.8/pytextclassifier.egg-info/
+-rw-r--r--   0 xuming     (501) staff       (20)    22590 2024-05-09 02:21:45.000000 pytextclassifier-1.3.8/pytextclassifier.egg-info/PKG-INFO
+-rw-r--r--   0 xuming     (501) staff       (20)      848 2024-05-09 02:21:45.000000 pytextclassifier-1.3.8/pytextclassifier.egg-info/SOURCES.txt
+-rw-r--r--   0 xuming     (501) staff       (20)        1 2024-05-09 02:21:45.000000 pytextclassifier-1.3.8/pytextclassifier.egg-info/dependency_links.txt
+-rw-r--r--   0 xuming     (501) staff       (20)       52 2024-05-09 02:21:45.000000 pytextclassifier-1.3.8/pytextclassifier.egg-info/requires.txt
+-rw-r--r--   0 xuming     (501) staff       (20)       17 2024-05-09 02:21:45.000000 pytextclassifier-1.3.8/pytextclassifier.egg-info/top_level.txt
+-rw-r--r--   0 xuming     (501) staff       (20)      309 2024-05-09 02:21:46.044943 pytextclassifier-1.3.8/setup.cfg
+-rw-r--r--   0 xuming     (501) staff       (20)     1444 2024-05-09 02:20:26.000000 pytextclassifier-1.3.8/setup.py
```

### Comparing `pytextclassifier-1.3.7/LICENSE` & `pytextclassifier-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pytextclassifier-1.3.7/PKG-INFO` & `pytextclassifier-1.3.8/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,1698 +1,1412 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7079 7465  : 2.1.Name: pyte
 00000020: 7874 636c 6173 7369 6669 6572 0a56 6572  xtclassifier.Ver
-00000030: 7369 6f6e 3a20 312e 332e 370a 5375 6d6d  sion: 1.3.7.Summ
+00000030: 7369 6f6e 3a20 312e 332e 380a 5375 6d6d  sion: 1.3.8.Summ
 00000040: 6172 793a 2054 6578 7420 436c 6173 7369  ary: Text Classi
 00000050: 6669 6572 2c20 5465 7874 2043 6c61 7373  fier, Text Class
 00000060: 6966 6963 6174 696f 6e0a 486f 6d65 2d70  ification.Home-p
 00000070: 6167 653a 2068 7474 7073 3a2f 2f67 6974  age: https://git
 00000080: 6875 622e 636f 6d2f 7368 6962 696e 6736  hub.com/shibing6
 00000090: 3234 2f70 7974 6578 7463 6c61 7373 6966  24/pytextclassif
 000000a0: 6965 720a 4175 7468 6f72 3a20 5875 4d69  ier.Author: XuMi
 000000b0: 6e67 0a41 7574 686f 722d 656d 6169 6c3a  ng.Author-email:
 000000c0: 2078 756d 696e 6736 3234 4071 712e 636f   xuming624@qq.co
 000000d0: 6d0a 4c69 6365 6e73 653a 2041 7061 6368  m.License: Apach
-000000e0: 6520 322e 300a 4465 7363 7269 7074 696f  e 2.0.Descriptio
-000000f0: 6e3a 203c 6469 7620 616c 6967 6e3d 2263  n: <div align="c
-00000100: 656e 7465 7222 3e0a 2020 2020 2020 2020  enter">.        
-00000110: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
-00000120: 3a2f 2f67 6974 6875 622e 636f 6d2f 7368  ://github.com/sh
-00000130: 6962 696e 6736 3234 2f70 7974 6578 7463  ibing624/pytextc
-00000140: 6c61 7373 6966 6965 7222 3e0a 2020 2020  lassifier">.    
-00000150: 2020 2020 2020 2020 3c69 6d67 2073 7263          <img src
-00000160: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
-00000170: 2e63 6f6d 2f73 6869 6269 6e67 3632 342f  .com/shibing624/
-00000180: 7079 7465 7874 636c 6173 7369 6669 6572  pytextclassifier
-00000190: 2f62 6c6f 622f 6d61 7374 6572 2f64 6f63  /blob/master/doc
-000001a0: 732f 6c6f 676f 2e70 6e67 2220 616c 743d  s/logo.png" alt=
-000001b0: 224c 6f67 6f22 2068 6569 6768 743d 2231  "Logo" height="1
-000001c0: 3536 223e 0a20 2020 2020 2020 2020 203c  56">.          <
-000001d0: 2f61 3e0a 2020 2020 2020 2020 3c2f 6469  /a>.        </di
-000001e0: 763e 0a20 2020 2020 2020 200a 2020 2020  v>.        .    
-000001f0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
-00000200: 2d2d 2d2d 2d0a 2020 2020 2020 2020 0a20  -----.        . 
-00000210: 2020 2020 2020 2023 2050 7954 6578 7443         # PyTextC
-00000220: 6c61 7373 6966 6965 723a 2050 7974 686f  lassifier: Pytho
-00000230: 6e20 5465 7874 2043 6c61 7373 6966 6965  n Text Classifie
-00000240: 720a 2020 2020 2020 2020 5b21 5b50 7950  r.        [![PyP
-00000250: 4920 7665 7273 696f 6e5d 2868 7474 7073  I version](https
-00000260: 3a2f 2f62 6164 6765 2e66 7572 792e 696f  ://badge.fury.io
-00000270: 2f70 792f 7079 7465 7874 636c 6173 7369  /py/pytextclassi
-00000280: 6669 6572 2e73 7667 295d 2868 7474 7073  fier.svg)](https
-00000290: 3a2f 2f62 6164 6765 2e66 7572 792e 696f  ://badge.fury.io
-000002a0: 2f70 792f 7079 7465 7874 636c 6173 7369  /py/pytextclassi
-000002b0: 6669 6572 290a 2020 2020 2020 2020 5b21  fier).        [!
-000002c0: 5b44 6f77 6e6c 6f61 6473 5d28 6874 7470  [Downloads](http
-000002d0: 733a 2f2f 7374 6174 6963 2e70 6570 792e  s://static.pepy.
-000002e0: 7465 6368 2f62 6164 6765 2f70 7974 6578  tech/badge/pytex
-000002f0: 7463 6c61 7373 6966 6965 7229 5d28 6874  tclassifier)](ht
-00000300: 7470 733a 2f2f 7065 7079 2e74 6563 682f  tps://pepy.tech/
-00000310: 7072 6f6a 6563 742f 7079 7465 7874 636c  project/pytextcl
-00000320: 6173 7369 6669 6572 290a 2020 2020 2020  assifier).      
-00000330: 2020 5b21 5b43 6f6e 7472 6962 7574 696f    [![Contributio
-00000340: 6e73 2077 656c 636f 6d65 5d28 6874 7470  ns welcome](http
-00000350: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000360: 696f 2f62 6164 6765 2f63 6f6e 7472 6962  io/badge/contrib
-00000370: 7574 696f 6e73 2d77 656c 636f 6d65 2d62  utions-welcome-b
-00000380: 7269 6768 7467 7265 656e 2e73 7667 295d  rightgreen.svg)]
-00000390: 2843 4f4e 5452 4942 5554 494e 472e 6d64  (CONTRIBUTING.md
-000003a0: 290a 2020 2020 2020 2020 5b21 5b47 6974  ).        [![Git
-000003b0: 4875 6220 636f 6e74 7269 6275 746f 7273  Hub contributors
-000003c0: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-000003d0: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
-000003e0: 636f 6e74 7269 6275 746f 7273 2f73 6869  contributors/shi
-000003f0: 6269 6e67 3632 342f 7079 7465 7874 636c  bing624/pytextcl
-00000400: 6173 7369 6669 6572 2e73 7667 295d 2868  assifier.svg)](h
-00000410: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000420: 6d2f 7368 6962 696e 6736 3234 2f70 7974  m/shibing624/pyt
-00000430: 6578 7463 6c61 7373 6966 6965 722f 6772  extclassifier/gr
-00000440: 6170 6873 2f63 6f6e 7472 6962 7574 6f72  aphs/contributor
-00000450: 7329 0a20 2020 2020 2020 205b 215b 4c69  s).        [![Li
-00000460: 6365 6e73 6520 4170 6163 6865 2032 2e30  cense Apache 2.0
-00000470: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-00000480: 6965 6c64 732e 696f 2f62 6164 6765 2f6c  ields.io/badge/l
-00000490: 6963 656e 7365 2d41 7061 6368 6525 3230  icense-Apache%20
-000004a0: 322e 302d 626c 7565 2e73 7667 295d 284c  2.0-blue.svg)](L
-000004b0: 4943 454e 5345 290a 2020 2020 2020 2020  ICENSE).        
-000004c0: 5b21 5b70 7974 686f 6e5f 7665 7369 6f6e  [![python_vesion
-000004d0: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-000004e0: 6965 6c64 732e 696f 2f62 6164 6765 2f50  ields.io/badge/P
-000004f0: 7974 686f 6e2d 332e 3525 3242 2d67 7265  ython-3.5%2B-gre
-00000500: 656e 2e73 7667 295d 2872 6571 7569 7265  en.svg)](require
-00000510: 6d65 6e74 732e 7478 7429 0a20 2020 2020  ments.txt).     
-00000520: 2020 205b 215b 4769 7448 7562 2069 7373     [![GitHub iss
-00000530: 7565 735d 2868 7474 7073 3a2f 2f69 6d67  ues](https://img
-00000540: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
-00000550: 7562 2f69 7373 7565 732f 7368 6962 696e  ub/issues/shibin
-00000560: 6736 3234 2f70 7974 6578 7463 6c61 7373  g624/pytextclass
-00000570: 6966 6965 722e 7376 6729 5d28 6874 7470  ifier.svg)](http
-00000580: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
-00000590: 6869 6269 6e67 3632 342f 7079 7465 7874  hibing624/pytext
-000005a0: 636c 6173 7369 6669 6572 2f69 7373 7565  classifier/issue
-000005b0: 7329 0a20 2020 2020 2020 205b 215b 5765  s).        [![We
-000005c0: 6368 6174 2047 726f 7570 5d28 6874 7470  chat Group](http
-000005d0: 3a2f 2f76 6c6f 672e 7366 7963 2e6c 7464  ://vlog.sfyc.ltd
-000005e0: 2f77 6563 6861 745f 6576 6572 7964 6179  /wechat_everyday
-000005f0: 2f77 7867 726f 7570 5f6c 6f67 6f2e 706e  /wxgroup_logo.pn
-00000600: 673f 696d 6167 6556 6965 7732 2f30 2f77  g?imageView2/0/w
-00000610: 2f36 302f 682f 3230 295d 2823 436f 6e74  /60/h/20)](#Cont
-00000620: 6163 7429 0a20 2020 2020 2020 200a 2020  act).        .  
-00000630: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
-00000640: 2320 496e 7472 6f64 7563 7469 6f6e 0a20  # Introduction. 
-00000650: 2020 2020 2020 2050 7954 6578 7443 6c61         PyTextCla
-00000660: 7373 6966 6965 723a 2050 7974 686f 6e20  ssifier: Python 
-00000670: 5465 7874 2043 6c61 7373 6966 6965 722e  Text Classifier.
-00000680: 2049 7420 6361 6e20 6265 2061 7070 6c69   It can be appli
-00000690: 6564 2074 6f20 7468 6520 6669 656c 6473  ed to the fields
-000006a0: 206f 6620 7365 6e74 696d 656e 7420 706f   of sentiment po
-000006b0: 6c61 7269 7479 2061 6e61 6c79 7369 732c  larity analysis,
-000006c0: 2074 6578 7420 7269 736b 2063 6c61 7373   text risk class
-000006d0: 6966 6963 6174 696f 6e20 616e 6420 736f  ification and so
-000006e0: 206f 6e2c 0a20 2020 2020 2020 2061 6e64   on,.        and
-000006f0: 2069 7420 7375 7070 6f72 7473 206d 756c   it supports mul
-00000700: 7469 706c 6520 636c 6173 7369 6669 6361  tiple classifica
-00000710: 7469 6f6e 2061 6c67 6f72 6974 686d 7320  tion algorithms 
-00000720: 616e 6420 636c 7573 7465 7269 6e67 2061  and clustering a
-00000730: 6c67 6f72 6974 686d 732e 0a20 2020 2020  lgorithms..     
-00000740: 2020 200a 2020 2020 2020 2020 2a2a 7079     .        **py
-00000750: 7465 7874 636c 6173 7369 6669 6572 2a2a  textclassifier**
-00000760: 2069 7320 6120 7079 7468 6f6e 204f 7065   is a python Ope
-00000770: 6e20 536f 7572 6365 2054 6f6f 6c6b 6974  n Source Toolkit
-00000780: 2066 6f72 2074 6578 7420 636c 6173 7369   for text classi
-00000790: 6669 6361 7469 6f6e 2e20 5468 6520 676f  fication. The go
-000007a0: 616c 2069 7320 746f 2069 6d70 6c65 6d65  al is to impleme
-000007b0: 6e74 0a20 2020 2020 2020 2074 6578 7420  nt.        text 
-000007c0: 616e 616c 7973 6973 2061 6c67 6f72 6974  analysis algorit
-000007d0: 686d 2c20 736f 2074 6f20 6163 6869 6576  hm, so to achiev
-000007e0: 6520 7468 6520 7573 6520 696e 2074 6865  e the use in the
-000007f0: 2070 726f 6475 6374 696f 6e20 656e 7669   production envi
-00000800: 726f 6e6d 656e 742e 0a20 2020 2020 2020  ronment..       
-00000810: 200a 2020 2020 2020 2020 e696 87e6 9cac   .        ......
-00000820: e588 86e7 b1bb e599 a8ef bc8c e68f 90e4  ................
-00000830: be9b e5a4 9ae7 a78d e696 87e6 9cac e588  ................
-00000840: 86e7 b1bb e592 8ce8 819a e7b1 bbe7 ae97  ................
-00000850: e6b3 95ef bc8c e694 afe6 8c81 e58f a5e5  ................
-00000860: ad90 e592 8ce6 9687 e6a1 a3e7 baa7 e79a  ................
-00000870: 84e6 9687 e69c ace5 8886 e7b1 bbe4 bbbb  ................
-00000880: e58a a1ef bc8c e694 afe6 8c81 e4ba 8ce5  ................
-00000890: 8886 e7b1 bbe3 8081 e5a4 9ae5 8886 e7b1  ................
-000008a0: bbe3 8081 e5a4 9ae6 a087 e7ad bee5 8886  ................
-000008b0: e7b1 bbe3 8081 e5a4 9ae5 b182 e7ba a7e5  ................
-000008c0: 8886 e7b1 bbe5 928c 4b6d 6561 6e73 e881  ........Kmeans..
-000008d0: 9ae7 b1bb efbc 8ce5 bc80 e7ae b1e5 8db3  ................
-000008e0: e794 a8e3 8082 7079 7468 6f6e 33e5 bc80  ......python3...
-000008f0: e58f 91e3 8082 0a20 2020 2020 2020 200a  .......        .
-00000900: 2020 2020 2020 2020 2a2a 4775 6964 652a          **Guide*
-00000910: 2a0a 2020 2020 2020 2020 0a20 2020 2020  *.        .     
-00000920: 2020 202d 205b 4665 6174 7572 655d 2823     - [Feature](#
-00000930: 4665 6174 7572 6529 0a20 2020 2020 2020  Feature).       
-00000940: 202d 205b 496e 7374 616c 6c5d 2823 696e   - [Install](#in
-00000950: 7374 616c 6c29 0a20 2020 2020 2020 202d  stall).        -
-00000960: 205b 5573 6167 655d 2823 7573 6167 6529   [Usage](#usage)
-00000970: 0a20 2020 2020 2020 202d 205b 4461 7461  .        - [Data
-00000980: 7365 745d 2823 4461 7461 7365 7429 0a20  set](#Dataset). 
-00000990: 2020 2020 2020 202d 205b 436f 6e74 6163         - [Contac
-000009a0: 745d 2823 436f 6e74 6163 7429 0a20 2020  t](#Contact).   
-000009b0: 2020 2020 202d 205b 4369 7461 7469 6f6e       - [Citation
-000009c0: 5d28 2343 6974 6174 696f 6e29 0a20 2020  ](#Citation).   
-000009d0: 2020 2020 202d 205b 5265 6665 7265 6e63       - [Referenc
-000009e0: 655d 2823 7265 6665 7265 6e63 6529 0a20  e](#reference). 
-000009f0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00000a00: 2323 2046 6561 7475 7265 0a20 2020 2020  ## Feature.     
-00000a10: 2020 200a 2020 2020 2020 2020 2a2a 7079     .        **py
-00000a20: 7465 7874 636c 6173 7369 6669 6572 2a2a  textclassifier**
-00000a30: 2068 6173 2074 6865 2063 6861 7261 6374   has the charact
-00000a40: 6572 6973 7469 6373 0a20 2020 2020 2020  eristics.       
-00000a50: 206f 6620 636c 6561 7220 616c 676f 7269   of clear algori
-00000a60: 7468 6d2c 2068 6967 6820 7065 7266 6f72  thm, high perfor
-00000a70: 6d61 6e63 6520 616e 6420 6375 7374 6f6d  mance and custom
-00000a80: 697a 6162 6c65 2063 6f72 7075 732e 0a20  izable corpus.. 
-00000a90: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00000aa0: 4675 6e63 7469 6f6e 73ef bc9a 0a20 2020  Functions....   
-00000ab0: 2020 2020 2023 2323 2043 6c61 7373 6966       ### Classif
-00000ac0: 6965 720a 2020 2020 2020 2020 2020 2d20  ier.          - 
-00000ad0: 5b78 5d20 4c6f 6769 7374 6963 5265 6772  [x] LogisticRegr
-00000ae0: 6573 7369 6f6e 0a20 2020 2020 2020 2020  ession.         
-00000af0: 202d 205b 785d 2052 616e 646f 6d20 466f   - [x] Random Fo
-00000b00: 7265 7374 0a20 2020 2020 2020 2020 202d  rest.          -
-00000b10: 205b 785d 2044 6563 6973 696f 6e20 5472   [x] Decision Tr
-00000b20: 6565 0a20 2020 2020 2020 2020 202d 205b  ee.          - [
-00000b30: 785d 204b 2d4e 6561 7265 7374 204e 6569  x] K-Nearest Nei
-00000b40: 6768 626f 7572 730a 2020 2020 2020 2020  ghbours.        
-00000b50: 2020 2d20 5b78 5d20 4e61 6976 6520 6261    - [x] Naive ba
-00000b60: 7965 730a 2020 2020 2020 2020 2020 2d20  yes.          - 
-00000b70: 5b78 5d20 5867 626f 6f73 740a 2020 2020  [x] Xgboost.    
-00000b80: 2020 2020 2020 2d20 5b78 5d20 5375 7070        - [x] Supp
-00000b90: 6f72 7420 5665 6374 6f72 204d 6163 6869  ort Vector Machi
-00000ba0: 6e65 2853 564d 290a 2020 2020 2020 2020  ne(SVM).        
-00000bb0: 2020 2d20 5b78 5d20 5465 7874 434e 4e0a    - [x] TextCNN.
-00000bc0: 2020 2020 2020 2020 2020 2d20 5b78 5d20            - [x] 
-00000bd0: 5465 7874 524e 4e0a 2020 2020 2020 2020  TextRNN.        
-00000be0: 2020 2d20 5b78 5d20 4661 7374 7465 7874    - [x] Fasttext
-00000bf0: 0a20 2020 2020 2020 2020 202d 205b 785d  .          - [x]
-00000c00: 2042 4552 540a 2020 2020 2020 2020 0a20   BERT.        . 
-00000c10: 2020 2020 2020 2023 2323 2043 6c75 7374         ### Clust
-00000c20: 6572 0a20 2020 2020 2020 2020 202d 205b  er.          - [
-00000c30: 785d 204d 696e 6942 6174 6368 4b6d 6561  x] MiniBatchKmea
-00000c40: 6e73 0a20 2020 2020 2020 200a 2020 2020  ns.        .    
-00000c50: 2020 2020 5768 696c 6520 7072 6f76 6964      While provid
-00000c60: 696e 6720 7269 6368 2066 756e 6374 696f  ing rich functio
-00000c70: 6e73 2c20 2a2a 7079 7465 7874 636c 6173  ns, **pytextclas
-00000c80: 7369 6669 6572 2a2a 2069 6e74 6572 6e61  sifier** interna
-00000c90: 6c20 6d6f 6475 6c65 7320 6164 6865 7265  l modules adhere
-00000ca0: 2074 6f20 6c6f 7720 636f 7570 6c69 6e67   to low coupling
-00000cb0: 2c20 6d6f 6465 6c20 6164 6865 7265 6e63  , model adherenc
-00000cc0: 6520 746f 2069 6e65 7274 206c 6f61 6469  e to inert loadi
-00000cd0: 6e67 2c20 6469 6374 696f 6e61 7279 2070  ng, dictionary p
-00000ce0: 7562 6c69 6361 7469 6f6e 2c20 616e 6420  ublication, and 
-00000cf0: 6561 7379 2074 6f20 7573 652e 0a20 2020  easy to use..   
-00000d00: 2020 2020 200a 2020 2020 2020 2020 2323       .        ##
-00000d10: 2049 6e73 7461 6c6c 0a20 2020 2020 2020   Install.       
-00000d20: 200a 2020 2020 2020 2020 2d20 5265 7175   .        - Requ
-00000d30: 6972 656d 656e 7473 2061 6e64 2049 6e73  irements and Ins
-00000d40: 7461 6c6c 6174 696f 6e0a 2020 2020 2020  tallation.      
-00000d50: 2020 0a20 2020 2020 2020 2060 6060 0a20    .        ```. 
-00000d60: 2020 2020 2020 2070 6970 3320 696e 7374         pip3 inst
-00000d70: 616c 6c20 746f 7263 6820 2320 636f 6e64  all torch # cond
-00000d80: 6120 696e 7374 616c 6c20 7079 746f 7263  a install pytorc
-00000d90: 680a 2020 2020 2020 2020 7069 7033 2069  h.        pip3 i
-00000da0: 6e73 7461 6c6c 2070 7974 6578 7463 6c61  nstall pytextcla
-00000db0: 7373 6966 6965 720a 2020 2020 2020 2020  ssifier.        
-00000dc0: 6060 600a 2020 2020 2020 2020 0a20 2020  ```.        .   
-00000dd0: 2020 2020 206f 720a 2020 2020 2020 2020       or.        
-00000de0: 0a20 2020 2020 2020 2060 6060 0a20 2020  .        ```.   
-00000df0: 2020 2020 2067 6974 2063 6c6f 6e65 2068       git clone h
-00000e00: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000e10: 6d2f 7368 6962 696e 6736 3234 2f70 7974  m/shibing624/pyt
-00000e20: 6578 7463 6c61 7373 6966 6965 722e 6769  extclassifier.gi
-00000e30: 740a 2020 2020 2020 2020 6364 2070 7974  t.        cd pyt
-00000e40: 6578 7463 6c61 7373 6966 6965 720a 2020  extclassifier.  
-00000e50: 2020 2020 2020 7079 7468 6f6e 3320 7365        python3 se
-00000e60: 7475 702e 7079 2069 6e73 7461 6c6c 0a20  tup.py install. 
-00000e70: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
-00000e80: 2020 200a 2020 2020 2020 2020 0a20 2020     .        .   
-00000e90: 2020 2020 2023 2320 5573 6167 650a 2020       ## Usage.  
-00000ea0: 2020 2020 2020 2323 2320 5465 7874 2043        ### Text C
-00000eb0: 6c61 7373 6966 6965 720a 2020 2020 2020  lassifier.      
-00000ec0: 2020 0a20 2020 2020 2020 2023 2323 2045    .        ### E
-00000ed0: 6e67 6c69 7368 2054 6578 7420 436c 6173  nglish Text Clas
-00000ee0: 7369 6669 6572 0a20 2020 2020 2020 200a  sifier.        .
-00000ef0: 2020 2020 2020 2020 496e 636c 7564 696e          Includin
-00000f00: 6720 6d6f 6465 6c20 7472 6169 6e69 6e67  g model training
-00000f10: 2c20 7361 7669 6e67 2c20 7072 6564 6963  , saving, predic
-00000f20: 742c 2065 7661 6c75 6174 652c 2066 6f72  t, evaluate, for
-00000f30: 2065 7861 6d70 6c65 205b 6578 616d 706c   example [exampl
-00000f40: 6573 2f6c 725f 656e 5f63 6c61 7373 6966  es/lr_en_classif
-00000f50: 6963 6174 696f 6e5f 6465 6d6f 2e70 795d  ication_demo.py]
-00000f60: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000f70: 636f 6d2f 7368 6962 696e 6736 3234 2f70  com/shibing624/p
-00000f80: 7974 6578 7463 6c61 7373 6966 6965 722f  ytextclassifier/
-00000f90: 626c 6f62 2f6d 6173 7465 722f 6578 616d  blob/master/exam
-00000fa0: 706c 6573 2f6c 725f 656e 5f63 6c61 7373  ples/lr_en_class
-00000fb0: 6966 6963 6174 696f 6e5f 6465 6d6f 2e70  ification_demo.p
-00000fc0: 7929 3a0a 2020 2020 2020 2020 0a20 2020  y):.        .   
-00000fd0: 2020 2020 2060 6060 7079 7468 6f6e 0a20       ```python. 
-00000fe0: 2020 2020 2020 2069 6d70 6f72 7420 7379         import sy
-00000ff0: 730a 2020 2020 2020 2020 0a20 2020 2020  s.        .     
-00001000: 2020 2073 7973 2e70 6174 682e 6170 7065     sys.path.appe
-00001010: 6e64 2827 2e2e 2729 0a20 2020 2020 2020  nd('..').       
-00001020: 2066 726f 6d20 7079 7465 7874 636c 6173   from pytextclas
-00001030: 7369 6669 6572 2069 6d70 6f72 7420 436c  sifier import Cl
-00001040: 6173 7369 6343 6c61 7373 6966 6965 720a  assicClassifier.
-00001050: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00001060: 2069 6620 5f5f 6e61 6d65 5f5f 203d 3d20   if __name__ == 
-00001070: 275f 5f6d 6169 6e5f 5f27 3a0a 2020 2020  '__main__':.    
-00001080: 2020 2020 2020 2020 6d20 3d20 436c 6173          m = Clas
-00001090: 7369 6343 6c61 7373 6966 6965 7228 6f75  sicClassifier(ou
-000010a0: 7470 7574 5f64 6972 3d27 6d6f 6465 6c73  tput_dir='models
-000010b0: 2f6c 7227 2c20 6d6f 6465 6c5f 6e61 6d65  /lr', model_name
-000010c0: 5f6f 725f 6d6f 6465 6c3d 276c 7227 290a  _or_model='lr').
-000010d0: 2020 2020 2020 2020 2020 2020 2320 436c              # Cl
-000010e0: 6173 7369 6343 6c61 7373 6966 6965 7220  assicClassifier 
-000010f0: 7375 7070 6f72 7420 6d6f 6465 6c5f 6e61  support model_na
-00001100: 6d65 efbc 9a6c 722c 2072 616e 646f 6d5f  me...lr, random_
-00001110: 666f 7265 7374 2c20 6465 6369 7369 6f6e  forest, decision
-00001120: 5f74 7265 652c 206b 6e6e 2c20 6261 7965  _tree, knn, baye
-00001130: 732c 2073 766d 2c20 7867 626f 6f73 740a  s, svm, xgboost.
-00001140: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00001150: 7428 6d29 0a20 2020 2020 2020 2020 2020  t(m).           
-00001160: 2064 6174 6120 3d20 5b0a 2020 2020 2020   data = [.      
-00001170: 2020 2020 2020 2020 2020 2827 6564 7563            ('educ
-00001180: 6174 696f 6e27 2c20 2753 7475 6465 6e74  ation', 'Student
-00001190: 2064 6562 7420 746f 2063 6f73 7420 4272   debt to cost Br
-000011a0: 6974 6169 6e20 6269 6c6c 696f 6e73 2077  itain billions w
-000011b0: 6974 6869 6e20 6465 6361 6465 7327 292c  ithin decades'),
-000011c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000011d0: 2028 2765 6475 6361 7469 6f6e 272c 2027   ('education', '
-000011e0: 4368 696e 6573 6520 6564 7563 6174 696f  Chinese educatio
-000011f0: 6e20 666f 7220 5456 2065 7870 6572 696d  n for TV experim
-00001200: 656e 7427 292c 0a20 2020 2020 2020 2020  ent'),.         
-00001210: 2020 2020 2020 2028 2773 706f 7274 7327         ('sports'
-00001220: 2c20 274d 6964 646c 6520 4561 7374 2061  , 'Middle East a
-00001230: 6e64 2041 7369 6120 626f 6f73 7420 696e  nd Asia boost in
-00001240: 7665 7374 6d65 6e74 2069 6e20 746f 7020  vestment in top 
-00001250: 6c65 7665 6c20 7370 6f72 7473 2729 2c0a  level sports'),.
-00001260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001270: 2827 7370 6f72 7473 272c 2027 5375 6d6d  ('sports', 'Summ
-00001280: 6974 2053 6572 6965 7320 6c6f 6f6b 206c  it Series look l
-00001290: 6175 6e63 6865 7320 4842 4f20 4361 6e61  aunches HBO Cana
-000012a0: 6461 2073 706f 7274 7320 646f 6320 7365  da sports doc se
-000012b0: 7269 6573 3a20 4d75 6468 6172 2729 0a20  ries: Mudhar'). 
-000012c0: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
-000012d0: 2020 2020 2020 2020 2023 2074 7261 696e           # train
-000012e0: 2061 6e64 2073 6176 6520 6265 7374 206d   and save best m
-000012f0: 6f64 656c 0a20 2020 2020 2020 2020 2020  odel.           
-00001300: 206d 2e74 7261 696e 2864 6174 6129 0a20   m.train(data). 
-00001310: 2020 2020 2020 2020 2020 2023 206c 6f61             # loa
-00001320: 6420 6265 7374 206d 6f64 656c 2066 726f  d best model fro
-00001330: 6d20 6d6f 6465 6c5f 6469 720a 2020 2020  m model_dir.    
-00001340: 2020 2020 2020 2020 6d2e 6c6f 6164 5f6d          m.load_m
-00001350: 6f64 656c 2829 0a20 2020 2020 2020 2020  odel().         
-00001360: 2020 2070 7265 6469 6374 5f6c 6162 656c     predict_label
-00001370: 2c20 7072 6564 6963 745f 7072 6f62 6120  , predict_proba 
-00001380: 3d20 6d2e 7072 6564 6963 7428 5b0a 2020  = m.predict([.  
-00001390: 2020 2020 2020 2020 2020 2020 2020 2741                'A
-000013a0: 6262 6f74 7420 676f 7665 726e 6d65 6e74  bbott government
-000013b0: 2073 7065 6e64 7320 2438 206d 696c 6c69   spends $8 milli
-000013c0: 6f6e 206f 6e20 6869 6768 6572 2065 6475  on on higher edu
-000013d0: 6361 7469 6f6e 206d 6564 6961 2062 6c69  cation media bli
-000013e0: 747a 275d 290a 2020 2020 2020 2020 2020  tz']).          
-000013f0: 2020 7072 696e 7428 6627 7072 6564 6963    print(f'predic
-00001400: 745f 6c61 6265 6c3a 207b 7072 6564 6963  t_label: {predic
-00001410: 745f 6c61 6265 6c7d 2c20 7072 6564 6963  t_label}, predic
-00001420: 745f 7072 6f62 613a 207b 7072 6564 6963  t_proba: {predic
-00001430: 745f 7072 6f62 617d 2729 0a20 2020 2020  t_proba}').     
-00001440: 2020 200a 2020 2020 2020 2020 2020 2020     .            
-00001450: 7465 7374 5f64 6174 6120 3d20 5b0a 2020  test_data = [.  
-00001460: 2020 2020 2020 2020 2020 2020 2020 2827                ('
-00001470: 6564 7563 6174 696f 6e27 2c20 2741 6262  education', 'Abb
-00001480: 6f74 7420 676f 7665 726e 6d65 6e74 2073  ott government s
-00001490: 7065 6e64 7320 2438 206d 696c 6c69 6f6e  pends $8 million
-000014a0: 206f 6e20 6869 6768 6572 2065 6475 6361   on higher educa
-000014b0: 7469 6f6e 206d 6564 6961 2062 6c69 747a  tion media blitz
-000014c0: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
-000014d0: 2020 2020 2827 7370 6f72 7473 272c 2027      ('sports', '
-000014e0: 4d69 6464 6c65 2045 6173 7420 616e 6420  Middle East and 
-000014f0: 4173 6961 2062 6f6f 7374 2069 6e76 6573  Asia boost inves
-00001500: 746d 656e 7420 696e 2074 6f70 206c 6576  tment in top lev
-00001510: 656c 2073 706f 7274 7327 292c 0a20 2020  el sports'),.   
-00001520: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
-00001530: 2020 2020 2020 2061 6363 5f73 636f 7265         acc_score
-00001540: 203d 206d 2e65 7661 6c75 6174 655f 6d6f   = m.evaluate_mo
-00001550: 6465 6c28 7465 7374 5f64 6174 6129 0a20  del(test_data). 
-00001560: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00001570: 2866 2761 6363 5f73 636f 7265 3a20 7b61  (f'acc_score: {a
-00001580: 6363 5f73 636f 7265 7d27 290a 2020 2020  cc_score}').    
-00001590: 2020 2020 6060 600a 2020 2020 2020 2020      ```.        
-000015a0: 0a20 2020 2020 2020 206f 7574 7075 743a  .        output:
-000015b0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-000015c0: 2020 6060 600a 2020 2020 2020 2020 436c    ```.        Cl
-000015d0: 6173 7369 6343 6c61 7373 6966 6965 7220  assicClassifier 
-000015e0: 696e 7374 616e 6365 2028 4c6f 6769 7374  instance (Logist
-000015f0: 6963 5265 6772 6573 7369 6f6e 2866 6974  icRegression(fit
-00001600: 5f69 6e74 6572 6365 7074 3d46 616c 7365  _intercept=False
-00001610: 292c 2073 746f 7077 6f72 6473 2073 697a  ), stopwords siz
-00001620: 653a 2032 3433 3829 0a20 2020 2020 2020  e: 2438).       
-00001630: 2070 7265 6469 6374 5f6c 6162 656c 3a20   predict_label: 
-00001640: 5b27 6564 7563 6174 696f 6e27 5d2c 2070  ['education'], p
-00001650: 7265 6469 6374 5f70 726f 6261 3a20 5b30  redict_proba: [0
-00001660: 2e35 3337 3832 3336 3335 3834 3932 3131  .537823635849211
-00001670: 325d 0a20 2020 2020 2020 2061 6363 5f73  2].        acc_s
-00001680: 636f 7265 3a20 312e 300a 2020 2020 2020  core: 1.0.      
-00001690: 2020 6060 600a 2020 2020 2020 2020 0a20    ```.        . 
-000016a0: 2020 2020 2020 2023 2323 2043 6869 6e65         ### Chine
-000016b0: 7365 2054 6578 7420 436c 6173 7369 6669  se Text Classifi
-000016c0: 6572 28e4 b8ad e696 87e6 9687 e69c ace5  er(.............
-000016d0: 8886 e7b1 bb29 0a20 2020 2020 2020 200a  .....).        .
-000016e0: 2020 2020 2020 2020 5465 7874 2063 6c61          Text cla
-000016f0: 7373 6966 6963 6174 696f 6e20 636f 6d70  ssification comp
-00001700: 6174 6962 6c65 2077 6974 6820 4368 696e  atible with Chin
-00001710: 6573 6520 616e 6420 456e 676c 6973 6820  ese and English 
-00001720: 636f 7270 6f72 612e 0a20 2020 2020 2020  corpora..       
-00001730: 200a 2020 2020 2020 2020 6578 616d 706c   .        exampl
-00001740: 6520 5b65 7861 6d70 6c65 732f 6c72 5f63  e [examples/lr_c
-00001750: 6c61 7373 6966 6963 6174 696f 6e5f 6465  lassification_de
-00001760: 6d6f 2e70 795d 2868 7474 7073 3a2f 2f67  mo.py](https://g
-00001770: 6974 6875 622e 636f 6d2f 7368 6962 696e  ithub.com/shibin
-00001780: 6736 3234 2f70 7974 6578 7463 6c61 7373  g624/pytextclass
-00001790: 6966 6965 722f 626c 6f62 2f6d 6173 7465  ifier/blob/maste
-000017a0: 722f 6578 616d 706c 6573 2f6c 725f 636c  r/examples/lr_cl
-000017b0: 6173 7369 6669 6361 7469 6f6e 5f64 656d  assification_dem
-000017c0: 6f2e 7079 290a 2020 2020 2020 2020 0a20  o.py).        . 
-000017d0: 2020 2020 2020 2060 6060 7079 7468 6f6e         ```python
-000017e0: 0a20 2020 2020 2020 2069 6d70 6f72 7420  .        import 
-000017f0: 7379 730a 2020 2020 2020 2020 0a20 2020  sys.        .   
-00001800: 2020 2020 2073 7973 2e70 6174 682e 6170       sys.path.ap
-00001810: 7065 6e64 2827 2e2e 2729 0a20 2020 2020  pend('..').     
-00001820: 2020 2066 726f 6d20 7079 7465 7874 636c     from pytextcl
-00001830: 6173 7369 6669 6572 2069 6d70 6f72 7420  assifier import 
-00001840: 436c 6173 7369 6343 6c61 7373 6966 6965  ClassicClassifie
-00001850: 720a 2020 2020 2020 2020 0a20 2020 2020  r.        .     
-00001860: 2020 2069 6620 5f5f 6e61 6d65 5f5f 203d     if __name__ =
-00001870: 3d20 275f 5f6d 6169 6e5f 5f27 3a0a 2020  = '__main__':.  
-00001880: 2020 2020 2020 2020 2020 6d20 3d20 436c            m = Cl
-00001890: 6173 7369 6343 6c61 7373 6966 6965 7228  assicClassifier(
-000018a0: 6f75 7470 7574 5f64 6972 3d27 6d6f 6465  output_dir='mode
-000018b0: 6c73 2f6c 722d 746f 7927 2c20 6d6f 6465  ls/lr-toy', mode
-000018c0: 6c5f 6e61 6d65 5f6f 725f 6d6f 6465 6c3d  l_name_or_model=
-000018d0: 276c 7227 290a 2020 2020 2020 2020 2020  'lr').          
-000018e0: 2020 2320 e7bb 8fe5 85b8 e588 86e7 b1bb    # ............
-000018f0: e696 b9e6 b395 efbc 8ce6 94af e68c 81e7  ................
-00001900: 9a84 e6a8 a1e5 9e8b e58c 85e6 8bac efbc  ................
-00001910: 9a6c 722c 2072 616e 646f 6d5f 666f 7265  .lr, random_fore
-00001920: 7374 2c20 6465 6369 7369 6f6e 5f74 7265  st, decision_tre
-00001930: 652c 206b 6e6e 2c20 6261 7965 732c 2073  e, knn, bayes, s
-00001940: 766d 2c20 7867 626f 6f73 740a 2020 2020  vm, xgboost.    
-00001950: 2020 2020 2020 2020 6461 7461 203d 205b          data = [
-00001960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001970: 2028 2765 6475 6361 7469 6f6e 272c 2027   ('education', '
-00001980: e590 8de5 b888 e68c 87e5 afbc e689 98e7  ................
-00001990: a68f e8af ade6 b395 e68a 80e5 b7a7 efbc  ................
-000019a0: 9ae5 908d e8af 8de7 9a84 e5a4 8de6 95b0  ................
-000019b0: e5bd a2e5 bc8f 2729 2c0a 2020 2020 2020  ......'),.      
-000019c0: 2020 2020 2020 2020 2020 2827 6564 7563            ('educ
-000019d0: 6174 696f 6e27 2c20 27e4 b8ad e59b bde9  ation', '.......
-000019e0: ab98 e880 83e6 8890 e7bb a9e6 b5b7 e5a4  ................
-000019f0: 96e8 aea4 e58f af20 e698 afe2 809c e78b  ....... ........
-00001a00: bce6 9da5 e4ba 86e2 809d e590 97ef bc9f  ................
-00001a10: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
-00001a20: 2020 2020 2827 6564 7563 6174 696f 6e27      ('education'
-00001a30: 2c20 27e5 85ac e58a a1e5 9198 e880 83e8  , '.............
-00001a40: 9991 e8b6 8ae6 9da5 e8b6 8ae5 9083 e9a6  ................
-00001a50: 99ef bc8c e8bf 99e6 98af e680 8ee4 b988  ................
-00001a60: e59b 9ee4 ba8b efbc 9f27 292c 0a20 2020  .........'),.   
-00001a70: 2020 2020 2020 2020 2020 2020 2028 2773               ('s
-00001a80: 706f 7274 7327 2c20 27e5 9bbe e696 87ef  ports', '.......
-00001a90: bc9a e6b3 95e7 bd91 e5ad 9fe8 8fb2 e5b0  ................
-00001aa0: 94e6 96af e88b a6e6 8898 e8bf 9b31 36e5  .............16.
-00001ab0: bcba 20e5 ad9f e88f b2e5 b094 e696 afe6  .. .............
-00001ac0: 8092 e590 bc27 292c 0a20 2020 2020 2020  .....'),.       
-00001ad0: 2020 2020 2020 2020 2028 2773 706f 7274           ('sport
-00001ae0: 7327 2c20 27e5 9b9b e5b7 9de4 b8b9 e6a3  s', '...........
-00001af0: b1e4 b8be e8a1 8ce5 85a8 e59b bde9 95bf  ................
-00001b00: e8b7 9de7 99bb e5b1 b1e6 8c91 e688 98e8  ................
-00001b10: b59b 20e8 bf91 e4b8 87e4 baba e58f 82e4  .. .............
-00001b20: b88e 2729 2c0a 2020 2020 2020 2020 2020  ..'),.          
-00001b30: 2020 2020 2020 2827 7370 6f72 7473 272c        ('sports',
-00001b40: 2027 e7b1 b3e5 85b0 e5ae a2e5 9cba 38e6   '............8.
-00001b50: 8898 e4b8 8de8 b4a5 e59b bde7 b1b3 3130  ..............10
-00001b60: e5b9 b4e8 bf9e e883 9c27 292c 0a20 2020  .........'),.   
-00001b70: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
-00001b80: 2020 2020 2020 206d 2e74 7261 696e 2864         m.train(d
-00001b90: 6174 6129 0a20 2020 2020 2020 2020 2020  ata).           
-00001ba0: 2070 7269 6e74 286d 290a 2020 2020 2020   print(m).      
-00001bb0: 2020 2020 2020 2320 6c6f 6164 2062 6573        # load bes
-00001bc0: 7420 6d6f 6465 6c20 6672 6f6d 206d 6f64  t model from mod
-00001bd0: 656c 5f64 6972 0a20 2020 2020 2020 2020  el_dir.         
-00001be0: 2020 206d 2e6c 6f61 645f 6d6f 6465 6c28     m.load_model(
-00001bf0: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
-00001c00: 6564 6963 745f 6c61 6265 6c2c 2070 7265  edict_label, pre
-00001c10: 6469 6374 5f70 726f 6261 203d 206d 2e70  dict_proba = m.p
-00001c20: 7265 6469 6374 285b 27e7 a68f e5bb bae6  redict(['.......
-00001c30: 98a5 e5ad a3e5 85ac e58a a1e5 9198 e880  ................
-00001c40: 83e8 af95 e68a a5e5 908d 3138 e697 a5e6  ..........18....
-00001c50: 88aa e6ad a220 32e6 9c88 36e6 97a5 e880  ..... 2...6.....
-00001c60: 83e8 af95 272c 0a20 2020 2020 2020 2020  ....',.         
-00001c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c90: 2020 2020 2020 2020 2020 2020 2027 e684               '..
-00001ca0: 8fe7 94b2 e9a6 96e8 bdae e8a1 a5e8 b59b  ................
-00001cb0: e4ba a4e6 8898 e8ae b0e5 bd95 3ae7 b1b3  ............:...
-00001cc0: e585 b0e5 aea2 e59c ba38 e688 98e4 b88d  .........8......
-00001cd0: e8b4 a5e5 9bbd e7b1 b331 30e5 b9b4 e8bf  .........10.....
-00001ce0: 9ee8 839c 275d 290a 2020 2020 2020 2020  ....']).        
-00001cf0: 2020 2020 7072 696e 7428 6627 7072 6564      print(f'pred
-00001d00: 6963 745f 6c61 6265 6c3a 207b 7072 6564  ict_label: {pred
-00001d10: 6963 745f 6c61 6265 6c7d 2c20 7072 6564  ict_label}, pred
-00001d20: 6963 745f 7072 6f62 613a 207b 7072 6564  ict_proba: {pred
-00001d30: 6963 745f 7072 6f62 617d 2729 0a20 2020  ict_proba}').   
-00001d40: 2020 2020 200a 2020 2020 2020 2020 2020       .          
-00001d50: 2020 7465 7374 5f64 6174 6120 3d20 5b0a    test_data = [.
-00001d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d70: 2827 6564 7563 6174 696f 6e27 2c20 27e7  ('education', '.
-00001d80: a68f e5bb bae6 98a5 e5ad a3e5 85ac e58a  ................
-00001d90: a1e5 9198 e880 83e8 af95 e68a a5e5 908d  ................
-00001da0: 3138 e697 a5e6 88aa e6ad a220 32e6 9c88  18......... 2...
-00001db0: 36e6 97a5 e880 83e8 af95 2729 2c0a 2020  6.........'),.  
-00001dc0: 2020 2020 2020 2020 2020 2020 2020 2827                ('
-00001dd0: 7370 6f72 7473 272c 2027 e684 8fe7 94b2  sports', '......
-00001de0: e9a6 96e8 bdae e8a1 a5e8 b59b e4ba a4e6  ................
-00001df0: 8898 e8ae b0e5 bd95 3ae7 b1b3 e585 b0e5  ........:.......
-00001e00: aea2 e59c ba38 e688 98e4 b88d e8b4 a5e5  .....8..........
-00001e10: 9bbd e7b1 b331 30e5 b9b4 e8bf 9ee8 839c  .....10.........
-00001e20: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
-00001e30: 5d0a 2020 2020 2020 2020 2020 2020 6163  ].            ac
-00001e40: 635f 7363 6f72 6520 3d20 6d2e 6576 616c  c_score = m.eval
-00001e50: 7561 7465 5f6d 6f64 656c 2874 6573 745f  uate_model(test_
-00001e60: 6461 7461 290a 2020 2020 2020 2020 2020  data).          
-00001e70: 2020 7072 696e 7428 6627 6163 635f 7363    print(f'acc_sc
-00001e80: 6f72 653a 207b 6163 635f 7363 6f72 657d  ore: {acc_score}
-00001e90: 2729 2020 2320 312e 300a 2020 2020 2020  ')  # 1.0.      
-00001ea0: 2020 0a20 2020 2020 2020 2020 2020 2023    .            #
-00001eb0: 2323 2320 7472 6169 6e20 6d6f 6465 6c20  ### train model 
-00001ec0: 7769 7468 2031 7720 6461 7461 0a20 2020  with 1w data.   
-00001ed0: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
-00001ee0: 2d27 202a 2034 3229 0a20 2020 2020 2020  -' * 42).       
-00001ef0: 2020 2020 206d 203d 2043 6c61 7373 6963       m = Classic
-00001f00: 436c 6173 7369 6669 6572 286f 7574 7075  Classifier(outpu
-00001f10: 745f 6469 723d 276d 6f64 656c 732f 6c72  t_dir='models/lr
-00001f20: 272c 206d 6f64 656c 5f6e 616d 655f 6f72  ', model_name_or
-00001f30: 5f6d 6f64 656c 3d27 6c72 2729 0a20 2020  _model='lr').   
-00001f40: 2020 2020 2020 2020 2064 6174 615f 6669           data_fi
-00001f50: 6c65 203d 2027 7468 7563 6e65 7773 5f74  le = 'thucnews_t
-00001f60: 7261 696e 5f31 772e 7478 7427 0a20 2020  rain_1w.txt'.   
-00001f70: 2020 2020 2020 2020 206d 2e74 7261 696e           m.train
-00001f80: 2864 6174 615f 6669 6c65 290a 2020 2020  (data_file).    
-00001f90: 2020 2020 2020 2020 6d2e 6c6f 6164 5f6d          m.load_m
-00001fa0: 6f64 656c 2829 0a20 2020 2020 2020 2020  odel().         
-00001fb0: 2020 2070 7265 6469 6374 5f6c 6162 656c     predict_label
-00001fc0: 2c20 7072 6564 6963 745f 7072 6f62 6120  , predict_proba 
-00001fd0: 3d20 6d2e 7072 6564 6963 7428 0a20 2020  = m.predict(.   
-00001fe0: 2020 2020 2020 2020 2020 2020 205b 27e9               ['.
-00001ff0: a1ba e4b9 89e5 8c97 e4ba ace8 8b8f e6b4  ................
-00002000: bb38 38e5 b9b3 e7b1 b3e8 b5b7 e7b2 bee8  .88.............
-00002010: a385 e688 bfe5 9ca8 e594 ae27 2c0a 2020  ...........',.  
-00002020: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00002030: e7be 8e45 422d 35e9 a1b9 e79b aee2 809c  ...EB-5.........
-00002040: 3135 e697 a5e5 bfab e980 9fe7 a7bb e6b0  15..............
-00002050: 91e2 809d e5b0 86e6 8ea8 e8bf 9f27 5d29  .............'])
-00002060: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00002070: 6e74 2866 2770 7265 6469 6374 5f6c 6162  nt(f'predict_lab
-00002080: 656c 3a20 7b70 7265 6469 6374 5f6c 6162  el: {predict_lab
-00002090: 656c 7d2c 2070 7265 6469 6374 5f70 726f  el}, predict_pro
-000020a0: 6261 3a20 7b70 7265 6469 6374 5f70 726f  ba: {predict_pro
-000020b0: 6261 7d27 290a 2020 2020 2020 2020 6060  ba}').        ``
-000020c0: 600a 2020 2020 2020 2020 0a20 2020 2020  `.        .     
-000020d0: 2020 206f 7574 7075 743a 0a20 2020 2020     output:.     
-000020e0: 2020 200a 2020 2020 2020 2020 6060 600a     .        ```.
-000020f0: 2020 2020 2020 2020 436c 6173 7369 6343          ClassicC
-00002100: 6c61 7373 6966 6965 7220 696e 7374 616e  lassifier instan
-00002110: 6365 2028 4c6f 6769 7374 6963 5265 6772  ce (LogisticRegr
-00002120: 6573 7369 6f6e 2866 6974 5f69 6e74 6572  ession(fit_inter
-00002130: 6365 7074 3d46 616c 7365 292c 2073 746f  cept=False), sto
-00002140: 7077 6f72 6473 2073 697a 653a 2032 3433  pwords size: 243
-00002150: 3829 0a20 2020 2020 2020 2070 7265 6469  8).        predi
-00002160: 6374 5f6c 6162 656c 3a20 5b27 6564 7563  ct_label: ['educ
-00002170: 6174 696f 6e27 2027 7370 6f72 7473 275d  ation' 'sports']
-00002180: 2c20 7072 6564 6963 745f 7072 6f62 613a  , predict_proba:
-00002190: 205b 302e 352c 2030 2e35 3938 3934 3138   [0.5, 0.5989418
-000021a0: 3036 3734 3135 3334 5d0a 2020 2020 2020  06741534].      
-000021b0: 2020 6163 635f 7363 6f72 653a 2031 2e30    acc_score: 1.0
-000021c0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-000021d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000021e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000021f0: 2d2d 2d0a 2020 2020 2020 2020 7072 6564  ---.        pred
-00002200: 6963 745f 6c61 6265 6c3a 205b 2772 6561  ict_label: ['rea
-00002210: 6c74 7927 2027 6564 7563 6174 696f 6e27  lty' 'education'
-00002220: 5d2c 2070 7265 6469 6374 5f70 726f 6261  ], predict_proba
-00002230: 3a20 5b30 2e37 3330 3239 3536 3932 3336  : [0.73029569236
-00002240: 3137 3337 322c 2030 2e32 3536 3530 3035  17372, 0.2565005
-00002250: 3434 3533 3232 3932 335d 0a20 2020 2020  445322923].     
-00002260: 2020 2060 6060 0a20 2020 2020 2020 200a     ```.        .
-00002270: 2020 2020 2020 2020 2323 2320 5669 7375          ### Visu
-00002280: 616c 2046 6561 7475 7265 2049 6d70 6f72  al Feature Impor
-00002290: 7461 6e63 650a 2020 2020 2020 2020 0a20  tance.        . 
-000022a0: 2020 2020 2020 2053 686f 7720 6665 6174         Show feat
-000022b0: 7572 6520 7765 6967 6874 7320 6f66 206d  ure weights of m
-000022c0: 6f64 656c 2c20 616e 6420 7072 6564 6963  odel, and predic
-000022d0: 7469 6f6e 2077 6f72 6420 7765 6967 6874  tion word weight
-000022e0: 2c20 666f 7220 6578 616d 706c 6520 5b65  , for example [e
-000022f0: 7861 6d70 6c65 732f 7669 7375 616c 5f66  xamples/visual_f
-00002300: 6561 7475 7265 5f69 6d70 6f72 7461 6e63  eature_importanc
-00002310: 652e 6970 796e 625d 2868 7474 7073 3a2f  e.ipynb](https:/
-00002320: 2f67 6974 6875 622e 636f 6d2f 7368 6962  /github.com/shib
-00002330: 696e 6736 3234 2f70 7974 6578 7463 6c61  ing624/pytextcla
-00002340: 7373 6966 6965 722f 626c 6f62 2f6d 6173  ssifier/blob/mas
-00002350: 7465 722f 6578 616d 706c 6573 2f76 6973  ter/examples/vis
-00002360: 7561 6c5f 6665 6174 7572 655f 696d 706f  ual_feature_impo
-00002370: 7274 616e 6365 2e69 7079 6e62 290a 2020  rtance.ipynb).  
-00002380: 2020 2020 2020 0a20 2020 2020 2020 2060        .        `
-00002390: 6060 7079 7468 6f6e 0a20 2020 2020 2020  ``python.       
-000023a0: 2069 6d70 6f72 7420 7379 730a 2020 2020   import sys.    
-000023b0: 2020 2020 0a20 2020 2020 2020 2073 7973      .        sys
-000023c0: 2e70 6174 682e 6170 7065 6e64 2827 2e2e  .path.append('..
-000023d0: 2729 0a20 2020 2020 2020 2066 726f 6d20  ').        from 
-000023e0: 7079 7465 7874 636c 6173 7369 6669 6572  pytextclassifier
-000023f0: 2069 6d70 6f72 7420 436c 6173 7369 6343   import ClassicC
-00002400: 6c61 7373 6966 6965 720a 2020 2020 2020  lassifier.      
-00002410: 2020 696d 706f 7274 206a 6965 6261 0a20    import jieba. 
-00002420: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00002430: 7463 203d 2043 6c61 7373 6963 436c 6173  tc = ClassicClas
-00002440: 7369 6669 6572 286f 7574 7075 745f 6469  sifier(output_di
-00002450: 723d 276d 6f64 656c 732f 6c72 2d74 6f79  r='models/lr-toy
-00002460: 272c 206d 6f64 656c 5f6e 616d 655f 6f72  ', model_name_or
-00002470: 5f6d 6f64 656c 3d27 6c72 2729 0a20 2020  _model='lr').   
-00002480: 2020 2020 2064 6174 6120 3d20 5b0a 2020       data = [.  
-00002490: 2020 2020 2020 2020 2020 2827 6564 7563            ('educ
-000024a0: 6174 696f 6e27 2c20 27e5 908d e5b8 88e6  ation', '.......
-000024b0: 8c87 e5af bce6 8998 e7a6 8fe8 afad e6b3  ................
-000024c0: 95e6 8a80 e5b7 a7ef bc9a e590 8de8 af8d  ................
-000024d0: e79a 84e5 a48d e695 b0e5 bda2 e5bc 8f27  ...............'
-000024e0: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
-000024f0: 2765 6475 6361 7469 6f6e 272c 2027 e4b8  'education', '..
-00002500: ade5 9bbd e9ab 98e8 8083 e688 90e7 bba9  ................
-00002510: e6b5 b7e5 a496 e8ae a4e5 8faf 20e6 98af  ............ ...
-00002520: e280 9ce7 8bbc e69d a5e4 ba86 e280 9de5  ................
-00002530: 9097 efbc 9f27 292c 0a20 2020 2020 2020  .....'),.       
-00002540: 2020 2020 2028 2773 706f 7274 7327 2c20       ('sports', 
-00002550: 27e5 9bbe e696 87ef bc9a e6b3 95e7 bd91  '...............
-00002560: e5ad 9fe8 8fb2 e5b0 94e6 96af e88b a6e6  ................
-00002570: 8898 e8bf 9b31 36e5 bcba 20e5 ad9f e88f  .....16... .....
-00002580: b2e5 b094 e696 afe6 8092 e590 bc27 292c  .............'),
-00002590: 0a20 2020 2020 2020 2020 2020 2028 2773  .            ('s
-000025a0: 706f 7274 7327 2c20 27e5 9b9b e5b7 9de4  ports', '.......
-000025b0: b8b9 e6a3 b1e4 b8be e8a1 8ce5 85a8 e59b  ................
-000025c0: bde9 95bf e8b7 9de7 99bb e5b1 b1e6 8c91  ................
-000025d0: e688 98e8 b59b 20e8 bf91 e4b8 87e4 baba  ...... .........
-000025e0: e58f 82e4 b88e 2729 2c0a 2020 2020 2020  ......'),.      
-000025f0: 2020 2020 2020 2827 7370 6f72 7473 272c        ('sports',
-00002600: 2027 e7b1 b3e5 85b0 e5ae a2e5 9cba 38e6   '............8.
-00002610: 8898 e4b8 8de8 b4a5 e59b bde7 b1b3 3130  ..............10
-00002620: e5b9 b4e8 bf9e e883 9c27 290a 2020 2020  .........').    
-00002630: 2020 2020 5d0a 2020 2020 2020 2020 7463      ].        tc
-00002640: 2e74 7261 696e 2864 6174 6129 0a20 2020  .train(data).   
-00002650: 2020 2020 2069 6d70 6f72 7420 656c 6935       import eli5
-00002660: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00002670: 2020 696e 6665 725f 6461 7461 203d 205b    infer_data = [
-00002680: 27e9 ab98 e880 83e6 8c87 e5af bce6 8998  '...............
-00002690: e7a6 8fe8 afad e6b3 95e6 8a80 e5b7 a7e5  ................
-000026a0: 9bbd e999 85e8 aea4 e58f af27 2c0a 2020  ...........',.  
-000026b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026c0: 2020 2020 27e6 848f e794 b2e9 a696 e8bd      '...........
-000026d0: aee8 a1a5 e8b5 9be4 baa4 e688 98e8 aeb0  ................
-000026e0: e5bd 953a e7b1 b3e5 85b0 e5ae a2e5 9cba  ...:............
-000026f0: 38e6 8898 e4b8 8de8 b4a5 e59b bde7 b1b3  8...............
-00002700: 3130 e5b9 b4e8 bf9e e883 9c27 5d0a 2020  10.........'].  
-00002710: 2020 2020 2020 656c 6935 2e73 686f 775f        eli5.show_
-00002720: 7765 6967 6874 7328 7463 2e6d 6f64 656c  weights(tc.model
-00002730: 2c20 7665 633d 7463 2e66 6561 7475 7265  , vec=tc.feature
-00002740: 290a 2020 2020 2020 2020 7365 675f 696e  ).        seg_in
-00002750: 6665 725f 6461 7461 203d 205b 2720 272e  fer_data = [' '.
-00002760: 6a6f 696e 286a 6965 6261 2e6c 6375 7428  join(jieba.lcut(
-00002770: 6929 2920 666f 7220 6920 696e 2069 6e66  i)) for i in inf
-00002780: 6572 5f64 6174 615d 0a20 2020 2020 2020  er_data].       
-00002790: 2065 6c69 352e 7368 6f77 5f70 7265 6469   eli5.show_predi
-000027a0: 6374 696f 6e28 7463 2e6d 6f64 656c 2c20  ction(tc.model, 
-000027b0: 7365 675f 696e 6665 725f 6461 7461 5b30  seg_infer_data[0
-000027c0: 5d2c 2076 6563 3d74 632e 6665 6174 7572  ], vec=tc.featur
-000027d0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-000027e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027f0: 7461 7267 6574 5f6e 616d 6573 3d5b 2765  target_names=['e
-00002800: 6475 6361 7469 6f6e 272c 2027 7370 6f72  ducation', 'spor
-00002810: 7473 275d 290a 2020 2020 2020 2020 6060  ts']).        ``
-00002820: 600a 2020 2020 2020 2020 0a20 2020 2020  `.        .     
-00002830: 2020 206f 7574 7075 743a 0a20 2020 2020     output:.     
-00002840: 2020 200a 2020 2020 2020 2020 215b 696d     .        ![im
-00002850: 672e 706e 675d 2864 6f63 732f 696d 672e  g.png](docs/img.
-00002860: 706e 6729 0a20 2020 2020 2020 200a 2020  png).        .  
-00002870: 2020 2020 2020 2323 2320 4465 6570 2043        ### Deep C
-00002880: 6c61 7373 6966 6963 6174 696f 6e20 6d6f  lassification mo
-00002890: 6465 6c0a 2020 2020 2020 2020 0a20 2020  del.        .   
-000028a0: 2020 2020 20e6 9cac e9a1 b9e7 9bae e694       ...........
-000028b0: afe6 8c81 e4bb a5e4 b88b e6b7 b1e5 baa6  ................
-000028c0: e588 86e7 b1bb e6a8 a1e5 9e8b efbc 9a46  ...............F
-000028d0: 6173 7454 6578 74e3 8081 5465 7874 434e  astText...TextCN
-000028e0: 4ee3 8081 5465 7874 524e 4ee3 8081 4265  N...TextRNN...Be
-000028f0: 7274 e6a8 a1e5 9e8b efbc 8c60 696d 706f  rt.........`impo
-00002900: 7274 60e6 a8a1 e59e 8be5 afb9 e5ba 94e7  rt`.............
-00002910: 9a84 e696 b9e6 b395 e69d a5e8 b083 e794  ................
-00002920: a8ef bc9a 0a20 2020 2020 2020 2060 6060  .....        ```
-00002930: 7079 7468 6f6e 0a20 2020 2020 2020 2066  python.        f
-00002940: 726f 6d20 7079 7465 7874 636c 6173 7369  rom pytextclassi
-00002950: 6669 6572 2069 6d70 6f72 7420 4661 7374  fier import Fast
-00002960: 5465 7874 436c 6173 7369 6669 6572 2c20  TextClassifier, 
-00002970: 5465 7874 434e 4e43 6c61 7373 6966 6965  TextCNNClassifie
-00002980: 722c 2054 6578 7452 4e4e 436c 6173 7369  r, TextRNNClassi
-00002990: 6669 6572 2c20 4265 7274 436c 6173 7369  fier, BertClassi
-000029a0: 6669 6572 0a20 2020 2020 2020 2060 6060  fier.        ```
-000029b0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-000029c0: 2020 e4b8 8be9 9da2 e4bb a546 6173 7454    .........FastT
-000029d0: 6578 74e6 a8a1 e59e 8be4 b8ba e7a4 bae4  ext.............
-000029e0: be8b efbc 8ce5 85b6 e4bb 96e6 a8a1 e59e  ................
-000029f0: 8be7 9a84 e4bd bfe7 94a8 e696 b9e6 b395  ................
-00002a00: e7b1 bbe4 bcbc e380 820a 2020 2020 2020  ..........      
-00002a10: 2020 0a20 2020 2020 2020 2023 2323 2046    .        ### F
-00002a20: 6173 7454 6578 7420 e6a8 a1e5 9e8b 0a20  astText ....... 
-00002a30: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00002a40: e8ae ade7 bb83 e592 8ce9 a284 e6b5 8b60  ...............`
-00002a50: 4661 7374 5465 7874 60e6 a8a1 e59e 8be7  FastText`.......
-00002a60: a4ba e4be 8b5b 6578 616d 706c 6573 2f66  .....[examples/f
-00002a70: 6173 7474 6578 745f 636c 6173 7369 6669  asttext_classifi
-00002a80: 6361 7469 6f6e 5f64 656d 6f2e 7079 5d28  cation_demo.py](
-00002a90: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00002aa0: 6f6d 2f73 6869 6269 6e67 3632 342f 7079  om/shibing624/py
-00002ab0: 7465 7874 636c 6173 7369 6669 6572 2f62  textclassifier/b
-00002ac0: 6c6f 622f 6d61 7374 6572 2f65 7861 6d70  lob/master/examp
-00002ad0: 6c65 732f 6661 7374 7465 7874 5f63 6c61  les/fasttext_cla
-00002ae0: 7373 6966 6963 6174 696f 6e5f 6465 6d6f  ssification_demo
-00002af0: 2e70 7929 0a20 2020 2020 2020 200a 2020  .py).        .  
-00002b00: 2020 2020 2020 6060 6070 7974 686f 6e0a        ```python.
-00002b10: 2020 2020 2020 2020 696d 706f 7274 2073          import s
-00002b20: 7973 0a20 2020 2020 2020 200a 2020 2020  ys.        .    
-00002b30: 2020 2020 7379 732e 7061 7468 2e61 7070      sys.path.app
-00002b40: 656e 6428 272e 2e27 290a 2020 2020 2020  end('..').      
-00002b50: 2020 6672 6f6d 2070 7974 6578 7463 6c61    from pytextcla
-00002b60: 7373 6966 6965 7220 696d 706f 7274 2046  ssifier import F
-00002b70: 6173 7454 6578 7443 6c61 7373 6966 6965  astTextClassifie
-00002b80: 722c 206c 6f61 645f 6461 7461 0a20 2020  r, load_data.   
-00002b90: 2020 2020 200a 2020 2020 2020 2020 6966       .        if
-00002ba0: 205f 5f6e 616d 655f 5f20 3d3d 2027 5f5f   __name__ == '__
-00002bb0: 6d61 696e 5f5f 273a 0a20 2020 2020 2020  main__':.       
-00002bc0: 2020 2020 206d 203d 2046 6173 7454 6578       m = FastTex
-00002bd0: 7443 6c61 7373 6966 6965 7228 6f75 7470  tClassifier(outp
-00002be0: 7574 5f64 6972 3d27 6d6f 6465 6c73 2f66  ut_dir='models/f
-00002bf0: 6173 7474 6578 742d 746f 7927 290a 2020  asttext-toy').  
-00002c00: 2020 2020 2020 2020 2020 6461 7461 203d            data =
-00002c10: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
-00002c20: 2020 2028 2765 6475 6361 7469 6f6e 272c     ('education',
-00002c30: 2027 e590 8de5 b888 e68c 87e5 afbc e689   '..............
-00002c40: 98e7 a68f e8af ade6 b395 e68a 80e5 b7a7  ................
-00002c50: efbc 9ae5 908d e8af 8de7 9a84 e5a4 8de6  ................
-00002c60: 95b0 e5bd a2e5 bc8f 2729 2c0a 2020 2020  ........'),.    
-00002c70: 2020 2020 2020 2020 2020 2020 2827 6564              ('ed
-00002c80: 7563 6174 696f 6e27 2c20 27e4 b8ad e59b  ucation', '.....
-00002c90: bde9 ab98 e880 83e6 8890 e7bb a9e6 b5b7  ................
-00002ca0: e5a4 96e8 aea4 e58f af20 e698 afe2 809c  ......... ......
-00002cb0: e78b bce6 9da5 e4ba 86e2 809d e590 97ef  ................
-00002cc0: bc9f 2729 2c0a 2020 2020 2020 2020 2020  ..'),.          
-00002cd0: 2020 2020 2020 2827 6564 7563 6174 696f        ('educatio
-00002ce0: 6e27 2c20 27e5 85ac e58a a1e5 9198 e880  n', '...........
-00002cf0: 83e8 9991 e8b6 8ae6 9da5 e8b6 8ae5 9083  ................
-00002d00: e9a6 99ef bc8c e8bf 99e6 98af e680 8ee4  ................
-00002d10: b988 e59b 9ee4 ba8b efbc 9f27 292c 0a20  ...........'),. 
-00002d20: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-00002d30: 2773 706f 7274 7327 2c20 27e5 9bbe e696  'sports', '.....
-00002d40: 87ef bc9a e6b3 95e7 bd91 e5ad 9fe8 8fb2  ................
-00002d50: e5b0 94e6 96af e88b a6e6 8898 e8bf 9b31  ...............1
-00002d60: 36e5 bcba 20e5 ad9f e88f b2e5 b094 e696  6... ...........
-00002d70: afe6 8092 e590 bc27 292c 0a20 2020 2020  .......'),.     
-00002d80: 2020 2020 2020 2020 2020 2028 2773 706f             ('spo
-00002d90: 7274 7327 2c20 27e5 9b9b e5b7 9de4 b8b9  rts', '.........
-00002da0: e6a3 b1e4 b8be e8a1 8ce5 85a8 e59b bde9  ................
-00002db0: 95bf e8b7 9de7 99bb e5b1 b1e6 8c91 e688  ................
-00002dc0: 98e8 b59b 20e8 bf91 e4b8 87e4 baba e58f  .... ...........
-00002dd0: 82e4 b88e 2729 2c0a 2020 2020 2020 2020  ....'),.        
-00002de0: 2020 2020 2020 2020 2827 7370 6f72 7473          ('sports
-00002df0: 272c 2027 e7b1 b3e5 85b0 e5ae a2e5 9cba  ', '............
-00002e00: 38e6 8898 e4b8 8de8 b4a5 e4bf 9de6 8c81  8...............
-00002e10: e8bf 9ee8 839c 2729 2c0a 2020 2020 2020  ......'),.      
-00002e20: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
-00002e30: 2020 2020 6d2e 7472 6169 6e28 6461 7461      m.train(data
-00002e40: 2c20 6e75 6d5f 6570 6f63 6873 3d33 290a  , num_epochs=3).
-00002e50: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00002e60: 7428 6d29 0a20 2020 2020 2020 2020 2020  t(m).           
-00002e70: 2023 206c 6f61 6420 7472 6169 6e65 6420   # load trained 
-00002e80: 6265 7374 206d 6f64 656c 0a20 2020 2020  best model.     
-00002e90: 2020 2020 2020 206d 2e6c 6f61 645f 6d6f         m.load_mo
-00002ea0: 6465 6c28 290a 2020 2020 2020 2020 2020  del().          
-00002eb0: 2020 7072 6564 6963 745f 6c61 6265 6c2c    predict_label,
-00002ec0: 2070 7265 6469 6374 5f70 726f 6261 203d   predict_proba =
-00002ed0: 206d 2e70 7265 6469 6374 285b 27e7 a68f   m.predict(['...
-00002ee0: e5bb bae6 98a5 e5ad a3e5 85ac e58a a1e5  ................
-00002ef0: 9198 e880 83e8 af95 e68a a5e5 908d 3138  ..............18
-00002f00: e697 a5e6 88aa e6ad a220 32e6 9c88 36e6  ......... 2...6.
-00002f10: 97a5 e880 83e8 af95 272c 0a20 2020 2020  ........',.     
-00002f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f50: 2027 e684 8fe7 94b2 e9a6 96e8 bdae e8a1   '..............
-00002f60: a5e8 b59b e4ba a4e6 8898 e8ae b0e5 bd95  ................
-00002f70: 3ae7 b1b3 e585 b0e5 aea2 e59c ba38 e688  :............8..
-00002f80: 98e4 b88d e8b4 a5e5 9bbd e7b1 b331 30e5  .............10.
-00002f90: b9b4 e8bf 9ee8 839c 275d 290a 2020 2020  ........']).    
-00002fa0: 2020 2020 2020 2020 7072 696e 7428 6627          print(f'
-00002fb0: 7072 6564 6963 745f 6c61 6265 6c3a 207b  predict_label: {
-00002fc0: 7072 6564 6963 745f 6c61 6265 6c7d 2c20  predict_label}, 
-00002fd0: 7072 6564 6963 745f 7072 6f62 613a 207b  predict_proba: {
-00002fe0: 7072 6564 6963 745f 7072 6f62 617d 2729  predict_proba}')
-00002ff0: 0a20 2020 2020 2020 2020 2020 2074 6573  .            tes
-00003000: 745f 6461 7461 203d 205b 0a20 2020 2020  t_data = [.     
-00003010: 2020 2020 2020 2020 2020 2028 2765 6475             ('edu
-00003020: 6361 7469 6f6e 272c 2027 e7a6 8fe5 bbba  cation', '......
-00003030: e698 a5e5 ada3 e585 ace5 8aa1 e591 98e8  ................
-00003040: 8083 e8af 95e6 8aa5 e590 8d31 38e6 97a5  ...........18...
-00003050: e688 aae6 ada2 2032 e69c 8836 e697 a5e8  ...... 2...6....
-00003060: 8083 e8af 9527 292c 0a20 2020 2020 2020  .....'),.       
-00003070: 2020 2020 2020 2020 2028 2773 706f 7274           ('sport
-00003080: 7327 2c20 27e6 848f e794 b2e9 a696 e8bd  s', '...........
-00003090: aee8 a1a5 e8b5 9be4 baa4 e688 98e8 aeb0  ................
-000030a0: e5bd 953a e7b1 b3e5 85b0 e5ae a2e5 9cba  ...:............
-000030b0: 38e6 8898 e4b8 8de8 b4a5 e59b bde7 b1b3  8...............
-000030c0: 3130 e5b9 b4e8 bf9e e883 9c27 292c 0a20  10.........'),. 
-000030d0: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
-000030e0: 2020 2020 2020 2020 2061 6363 5f73 636f           acc_sco
-000030f0: 7265 203d 206d 2e65 7661 6c75 6174 655f  re = m.evaluate_
-00003100: 6d6f 6465 6c28 7465 7374 5f64 6174 6129  model(test_data)
-00003110: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00003120: 6e74 2866 2761 6363 5f73 636f 7265 3a20  nt(f'acc_score: 
-00003130: 7b61 6363 5f73 636f 7265 7d27 2920 2023  {acc_score}')  #
-00003140: 2031 2e30 0a20 2020 2020 2020 200a 2020   1.0.        .  
-00003150: 2020 2020 2020 2020 2020 2323 2323 2074            #### t
-00003160: 7261 696e 206d 6f64 656c 2077 6974 6820  rain model with 
-00003170: 3177 2064 6174 610a 2020 2020 2020 2020  1w data.        
-00003180: 2020 2020 7072 696e 7428 272d 2720 2a20      print('-' * 
-00003190: 3432 290a 2020 2020 2020 2020 2020 2020  42).            
-000031a0: 6461 7461 5f66 696c 6520 3d20 2774 6875  data_file = 'thu
-000031b0: 636e 6577 735f 7472 6169 6e5f 3177 2e74  cnews_train_1w.t
-000031c0: 7874 270a 2020 2020 2020 2020 2020 2020  xt'.            
-000031d0: 6d20 3d20 4661 7374 5465 7874 436c 6173  m = FastTextClas
-000031e0: 7369 6669 6572 286f 7574 7075 745f 6469  sifier(output_di
-000031f0: 723d 276d 6f64 656c 732f 6661 7374 7465  r='models/fastte
-00003200: 7874 2729 0a20 2020 2020 2020 2020 2020  xt').           
-00003210: 206d 2e74 7261 696e 2864 6174 615f 6669   m.train(data_fi
-00003220: 6c65 2c20 6e61 6d65 733d 2827 6c61 6265  le, names=('labe
-00003230: 6c73 272c 2027 7465 7874 2729 2c20 6e75  ls', 'text'), nu
-00003240: 6d5f 6570 6f63 6873 3d33 290a 2020 2020  m_epochs=3).    
-00003250: 2020 2020 2020 2020 2320 6c6f 6164 2062          # load b
-00003260: 6573 7420 7472 6169 6e65 6420 6d6f 6465  est trained mode
-00003270: 6c20 6672 6f6d 206d 6f64 656c 5f64 6972  l from model_dir
-00003280: 0a20 2020 2020 2020 2020 2020 206d 2e6c  .            m.l
-00003290: 6f61 645f 6d6f 6465 6c28 290a 2020 2020  oad_model().    
-000032a0: 2020 2020 2020 2020 7072 6564 6963 745f          predict_
-000032b0: 6c61 6265 6c2c 2070 7265 6469 6374 5f70  label, predict_p
-000032c0: 726f 6261 203d 206d 2e70 7265 6469 6374  roba = m.predict
-000032d0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000032e0: 2020 5b27 e9a1 bae4 b989 e58c 97e4 baac    ['............
-000032f0: e88b 8fe6 b4bb 3838 e5b9 b3e7 b1b3 e8b5  ......88........
-00003300: b7e7 b2be e8a3 85e6 88bf e59c a8e5 94ae  ................
-00003310: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-00003320: 2020 2020 27e7 be8e 4542 2d35 e9a1 b9e7      '...EB-5....
-00003330: 9bae e280 9c31 35e6 97a5 e5bf abe9 809f  .....15.........
-00003340: e7a7 bbe6 b091 e280 9de5 b086 e68e a8e8  ................
-00003350: bf9f 275d 0a20 2020 2020 2020 2020 2020  ..'].           
-00003360: 2029 0a20 2020 2020 2020 2020 2020 2070   ).            p
-00003370: 7269 6e74 2866 2770 7265 6469 6374 5f6c  rint(f'predict_l
-00003380: 6162 656c 3a20 7b70 7265 6469 6374 5f6c  abel: {predict_l
-00003390: 6162 656c 7d2c 2070 7265 6469 6374 5f70  abel}, predict_p
-000033a0: 726f 6261 3a20 7b70 7265 6469 6374 5f70  roba: {predict_p
-000033b0: 726f 6261 7d27 290a 2020 2020 2020 2020  roba}').        
-000033c0: 2020 2020 782c 2079 2c20 6466 203d 206c      x, y, df = l
-000033d0: 6f61 645f 6461 7461 2864 6174 615f 6669  oad_data(data_fi
-000033e0: 6c65 290a 2020 2020 2020 2020 2020 2020  le).            
-000033f0: 7465 7374 5f64 6174 6120 3d20 6466 5b3a  test_data = df[:
-00003400: 3130 305d 0a20 2020 2020 2020 2020 2020  100].           
+000000e0: 6520 322e 300a 4b65 7977 6f72 6473 3a20  e 2.0.Keywords: 
+000000f0: 7079 7465 7874 636c 6173 7369 6669 6572  pytextclassifier
+00000100: 2c74 6578 7463 6c61 7373 6966 6965 722c  ,textclassifier,
+00000110: 636c 6173 7369 6669 6572 2c74 6578 7463  classifier,textc
+00000120: 6c61 7373 6966 6963 6174 696f 6e0a 436c  lassification.Cl
+00000130: 6173 7369 6669 6572 3a20 496e 7465 6e64  assifier: Intend
+00000140: 6564 2041 7564 6965 6e63 6520 3a3a 2053  ed Audience :: S
+00000150: 6369 656e 6365 2f52 6573 6561 7263 680a  cience/Research.
+00000160: 436c 6173 7369 6669 6572 3a20 4f70 6572  Classifier: Oper
+00000170: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
+00000180: 4f53 2049 6e64 6570 656e 6465 6e74 0a43  OS Independent.C
+00000190: 6c61 7373 6966 6965 723a 204c 6963 656e  lassifier: Licen
+000001a0: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
+000001b0: 6564 203a 3a20 4170 6163 6865 2053 6f66  ed :: Apache Sof
+000001c0: 7477 6172 6520 4c69 6365 6e73 650a 436c  tware License.Cl
+000001d0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+000001e0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+000001f0: 3a20 5079 7468 6f6e 0a43 6c61 7373 6966  : Python.Classif
+00000200: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+00000210: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000220: 686f 6e20 3a3a 2032 2e37 0a43 6c61 7373  hon :: 2.7.Class
+00000230: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+00000240: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000250: 7974 686f 6e20 3a3a 2033 0a43 6c61 7373  ython :: 3.Class
+00000260: 6966 6965 723a 2054 6f70 6963 203a 3a20  ifier: Topic :: 
+00000270: 5465 7874 2050 726f 6365 7373 696e 6720  Text Processing 
+00000280: 3a3a 204c 696e 6775 6973 7469 630a 436c  :: Linguistic.Cl
+00000290: 6173 7369 6669 6572 3a20 546f 7069 6320  assifier: Topic 
+000002a0: 3a3a 2053 6369 656e 7469 6669 632f 456e  :: Scientific/En
+000002b0: 6769 6e65 6572 696e 6720 3a3a 2041 7274  gineering :: Art
+000002c0: 6966 6963 6961 6c20 496e 7465 6c6c 6967  ificial Intellig
+000002d0: 656e 6365 0a44 6573 6372 6970 7469 6f6e  ence.Description
+000002e0: 2d43 6f6e 7465 6e74 2d54 7970 653a 2074  -Content-Type: t
+000002f0: 6578 742f 6d61 726b 646f 776e 0a4c 6963  ext/markdown.Lic
+00000300: 656e 7365 2d46 696c 653a 204c 4943 454e  ense-File: LICEN
+00000310: 5345 0a0a 3c64 6976 2061 6c69 676e 3d22  SE..<div align="
+00000320: 6365 6e74 6572 223e 0a20 203c 6120 6872  center">.  <a hr
+00000330: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+00000340: 7562 2e63 6f6d 2f73 6869 6269 6e67 3632  ub.com/shibing62
+00000350: 342f 7079 7465 7874 636c 6173 7369 6669  4/pytextclassifi
+00000360: 6572 223e 0a20 2020 203c 696d 6720 7372  er">.    <img sr
+00000370: 633d 2268 7474 7073 3a2f 2f67 6974 6875  c="https://githu
+00000380: 622e 636f 6d2f 7368 6962 696e 6736 3234  b.com/shibing624
+00000390: 2f70 7974 6578 7463 6c61 7373 6966 6965  /pytextclassifie
+000003a0: 722f 626c 6f62 2f6d 6173 7465 722f 646f  r/blob/master/do
+000003b0: 6373 2f6c 6f67 6f2e 706e 6722 2061 6c74  cs/logo.png" alt
+000003c0: 3d22 4c6f 676f 2220 6865 6967 6874 3d22  ="Logo" height="
+000003d0: 3135 3622 3e0a 2020 3c2f 613e 0a3c 2f64  156">.  </a>.</d
+000003e0: 6976 3e0a 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  iv>..-----------
+000003f0: 2d2d 2d2d 2d2d 0a0a 2320 5079 5465 7874  ------..# PyText
+00000400: 436c 6173 7369 6669 6572 3a20 5079 7468  Classifier: Pyth
+00000410: 6f6e 2054 6578 7420 436c 6173 7369 6669  on Text Classifi
+00000420: 6572 0a5b 215b 5079 5049 2076 6572 7369  er.[![PyPI versi
+00000430: 6f6e 5d28 6874 7470 733a 2f2f 6261 6467  on](https://badg
+00000440: 652e 6675 7279 2e69 6f2f 7079 2f70 7974  e.fury.io/py/pyt
+00000450: 6578 7463 6c61 7373 6966 6965 722e 7376  extclassifier.sv
+00000460: 6729 5d28 6874 7470 733a 2f2f 6261 6467  g)](https://badg
+00000470: 652e 6675 7279 2e69 6f2f 7079 2f70 7974  e.fury.io/py/pyt
+00000480: 6578 7463 6c61 7373 6966 6965 7229 0a5b  extclassifier).[
+00000490: 215b 446f 776e 6c6f 6164 735d 2868 7474  ![Downloads](htt
+000004a0: 7073 3a2f 2f73 7461 7469 632e 7065 7079  ps://static.pepy
+000004b0: 2e74 6563 682f 6261 6467 652f 7079 7465  .tech/badge/pyte
+000004c0: 7874 636c 6173 7369 6669 6572 295d 2868  xtclassifier)](h
+000004d0: 7474 7073 3a2f 2f70 6570 792e 7465 6368  ttps://pepy.tech
+000004e0: 2f70 726f 6a65 6374 2f70 7974 6578 7463  /project/pytextc
+000004f0: 6c61 7373 6966 6965 7229 0a5b 215b 436f  lassifier).[![Co
+00000500: 6e74 7269 6275 7469 6f6e 7320 7765 6c63  ntributions welc
+00000510: 6f6d 655d 2868 7474 7073 3a2f 2f69 6d67  ome](https://img
+00000520: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
+00000530: 652f 636f 6e74 7269 6275 7469 6f6e 732d  e/contributions-
+00000540: 7765 6c63 6f6d 652d 6272 6967 6874 6772  welcome-brightgr
+00000550: 6565 6e2e 7376 6729 5d28 434f 4e54 5249  een.svg)](CONTRI
+00000560: 4255 5449 4e47 2e6d 6429 0a5b 215b 4c69  BUTING.md).[![Li
+00000570: 6365 6e73 6520 4170 6163 6865 2032 2e30  cense Apache 2.0
+00000580: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00000590: 6965 6c64 732e 696f 2f62 6164 6765 2f6c  ields.io/badge/l
+000005a0: 6963 656e 7365 2d41 7061 6368 6525 3230  icense-Apache%20
+000005b0: 322e 302d 626c 7565 2e73 7667 295d 284c  2.0-blue.svg)](L
+000005c0: 4943 454e 5345 290a 5b21 5b70 7974 686f  ICENSE).[![pytho
+000005d0: 6e5f 7665 7369 6f6e 5d28 6874 7470 733a  n_vesion](https:
+000005e0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000005f0: 2f62 6164 6765 2f50 7974 686f 6e2d 332e  /badge/Python-3.
+00000600: 3525 3242 2d67 7265 656e 2e73 7667 295d  5%2B-green.svg)]
+00000610: 2872 6571 7569 7265 6d65 6e74 732e 7478  (requirements.tx
+00000620: 7429 0a5b 215b 4769 7448 7562 2069 7373  t).[![GitHub iss
+00000630: 7565 735d 2868 7474 7073 3a2f 2f69 6d67  ues](https://img
+00000640: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
+00000650: 7562 2f69 7373 7565 732f 7368 6962 696e  ub/issues/shibin
+00000660: 6736 3234 2f70 7974 6578 7463 6c61 7373  g624/pytextclass
+00000670: 6966 6965 722e 7376 6729 5d28 6874 7470  ifier.svg)](http
+00000680: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
+00000690: 6869 6269 6e67 3632 342f 7079 7465 7874  hibing624/pytext
+000006a0: 636c 6173 7369 6669 6572 2f69 7373 7565  classifier/issue
+000006b0: 7329 0a5b 215b 5765 6368 6174 2047 726f  s).[![Wechat Gro
+000006c0: 7570 5d28 6874 7470 733a 2f2f 696d 672e  up](https://img.
+000006d0: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
+000006e0: 2f77 6563 6861 742d 6772 6f75 702d 6772  /wechat-group-gr
+000006f0: 6565 6e2e 7376 673f 6c6f 676f 3d77 6563  een.svg?logo=wec
+00000700: 6861 7429 5d28 2343 6f6e 7461 6374 290a  hat)](#Contact).
+00000710: 0a0a 2323 2049 6e74 726f 6475 6374 696f  ..## Introductio
+00000720: 6e0a 5079 5465 7874 436c 6173 7369 6669  n.PyTextClassifi
+00000730: 6572 3a20 5079 7468 6f6e 2054 6578 7420  er: Python Text 
+00000740: 436c 6173 7369 6669 6572 2e20 4974 2063  Classifier. It c
+00000750: 616e 2062 6520 6170 706c 6965 6420 746f  an be applied to
+00000760: 2074 6865 2066 6965 6c64 7320 6f66 2073   the fields of s
+00000770: 656e 7469 6d65 6e74 2070 6f6c 6172 6974  entiment polarit
+00000780: 7920 616e 616c 7973 6973 2c20 7465 7874  y analysis, text
+00000790: 2072 6973 6b20 636c 6173 7369 6669 6361   risk classifica
+000007a0: 7469 6f6e 2061 6e64 2073 6f20 6f6e 2c0a  tion and so on,.
+000007b0: 616e 6420 6974 2073 7570 706f 7274 7320  and it supports 
+000007c0: 6d75 6c74 6970 6c65 2063 6c61 7373 6966  multiple classif
+000007d0: 6963 6174 696f 6e20 616c 676f 7269 7468  ication algorith
+000007e0: 6d73 2061 6e64 2063 6c75 7374 6572 696e  ms and clusterin
+000007f0: 6720 616c 676f 7269 7468 6d73 2e0a 0a2a  g algorithms...*
+00000800: 2a70 7974 6578 7463 6c61 7373 6966 6965  *pytextclassifie
+00000810: 722a 2a20 6973 2061 2070 7974 686f 6e20  r** is a python 
+00000820: 4f70 656e 2053 6f75 7263 6520 546f 6f6c  Open Source Tool
+00000830: 6b69 7420 666f 7220 7465 7874 2063 6c61  kit for text cla
+00000840: 7373 6966 6963 6174 696f 6e2e 2054 6865  ssification. The
+00000850: 2067 6f61 6c20 6973 2074 6f20 696d 706c   goal is to impl
+00000860: 656d 656e 740a 7465 7874 2061 6e61 6c79  ement.text analy
+00000870: 7369 7320 616c 676f 7269 7468 6d2c 2073  sis algorithm, s
+00000880: 6f20 746f 2061 6368 6965 7665 2074 6865  o to achieve the
+00000890: 2075 7365 2069 6e20 7468 6520 7072 6f64   use in the prod
+000008a0: 7563 7469 6f6e 2065 6e76 6972 6f6e 6d65  uction environme
+000008b0: 6e74 2e0a 0ae6 9687 e69c ace5 8886 e7b1  nt..............
+000008c0: bbe5 99a8 efbc 8ce6 8f90 e4be 9be5 a49a  ................
+000008d0: e7a7 8de6 9687 e69c ace5 8886 e7b1 bbe5  ................
+000008e0: 928c e881 9ae7 b1bb e7ae 97e6 b395 efbc  ................
+000008f0: 8ce6 94af e68c 81e5 8fa5 e5ad 90e5 928c  ................
+00000900: e696 87e6 a1a3 e7ba a7e7 9a84 e696 87e6  ................
+00000910: 9cac e588 86e7 b1bb e4bb bbe5 8aa1 efbc  ................
+00000920: 8ce6 94af e68c 81e4 ba8c e588 86e7 b1bb  ................
+00000930: e380 81e5 a49a e588 86e7 b1bb e380 81e5  ................
+00000940: a49a e6a0 87e7 adbe e588 86e7 b1bb e380  ................
+00000950: 81e5 a49a e5b1 82e7 baa7 e588 86e7 b1bb  ................
+00000960: e592 8c4b 6d65 616e 73e8 819a e7b1 bbef  ...Kmeans.......
+00000970: bc8c e5bc 80e7 aeb1 e58d b3e7 94a8 e380  ................
+00000980: 8270 7974 686f 6e33 e5bc 80e5 8f91 e380  .python3........
+00000990: 820a 0a2a 2a47 7569 6465 2a2a 0a0a 2d20  ...**Guide**..- 
+000009a0: 5b46 6561 7475 7265 5d28 2346 6561 7475  [Feature](#Featu
+000009b0: 7265 290a 2d20 5b49 6e73 7461 6c6c 5d28  re).- [Install](
+000009c0: 2369 6e73 7461 6c6c 290a 2d20 5b55 7361  #install).- [Usa
+000009d0: 6765 5d28 2375 7361 6765 290a 2d20 5b44  ge](#usage).- [D
+000009e0: 6174 6173 6574 5d28 2344 6174 6173 6574  ataset](#Dataset
+000009f0: 290a 2d20 5b43 6f6e 7461 6374 5d28 2343  ).- [Contact](#C
+00000a00: 6f6e 7461 6374 290a 2d20 5b43 6974 6174  ontact).- [Citat
+00000a10: 696f 6e5d 2823 4369 7461 7469 6f6e 290a  ion](#Citation).
+00000a20: 2d20 5b52 6566 6572 656e 6365 5d28 2372  - [Reference](#r
+00000a30: 6566 6572 656e 6365 290a 0a23 2320 4665  eference)..## Fe
+00000a40: 6174 7572 650a 0a2a 2a70 7974 6578 7463  ature..**pytextc
+00000a50: 6c61 7373 6966 6965 722a 2a20 6861 7320  lassifier** has 
+00000a60: 7468 6520 6368 6172 6163 7465 7269 7374  the characterist
+00000a70: 6963 730a 6f66 2063 6c65 6172 2061 6c67  ics.of clear alg
+00000a80: 6f72 6974 686d 2c20 6869 6768 2070 6572  orithm, high per
+00000a90: 666f 726d 616e 6365 2061 6e64 2063 7573  formance and cus
+00000aa0: 746f 6d69 7a61 626c 6520 636f 7270 7573  tomizable corpus
+00000ab0: 2e0a 0a46 756e 6374 696f 6e73 efbc 9a0a  ...Functions....
+00000ac0: 2323 2320 436c 6173 7369 6669 6572 0a20  ### Classifier. 
+00000ad0: 202d 205b 785d 204c 6f67 6973 7469 6352   - [x] LogisticR
+00000ae0: 6567 7265 7373 696f 6e0a 2020 2d20 5b78  egression.  - [x
+00000af0: 5d20 5261 6e64 6f6d 2046 6f72 6573 740a  ] Random Forest.
+00000b00: 2020 2d20 5b78 5d20 4465 6369 7369 6f6e    - [x] Decision
+00000b10: 2054 7265 650a 2020 2d20 5b78 5d20 4b2d   Tree.  - [x] K-
+00000b20: 4e65 6172 6573 7420 4e65 6967 6862 6f75  Nearest Neighbou
+00000b30: 7273 0a20 202d 205b 785d 204e 6169 7665  rs.  - [x] Naive
+00000b40: 2062 6179 6573 0a20 202d 205b 785d 2058   bayes.  - [x] X
+00000b50: 6762 6f6f 7374 0a20 202d 205b 785d 2053  gboost.  - [x] S
+00000b60: 7570 706f 7274 2056 6563 746f 7220 4d61  upport Vector Ma
+00000b70: 6368 696e 6528 5356 4d29 0a20 202d 205b  chine(SVM).  - [
+00000b80: 785d 2054 6578 7443 4e4e 0a20 202d 205b  x] TextCNN.  - [
+00000b90: 785d 2054 6578 7452 4e4e 0a20 202d 205b  x] TextRNN.  - [
+00000ba0: 785d 2046 6173 7474 6578 740a 2020 2d20  x] Fasttext.  - 
+00000bb0: 5b78 5d20 4245 5254 0a0a 2323 2320 436c  [x] BERT..### Cl
+00000bc0: 7573 7465 720a 2020 2d20 5b78 5d20 4d69  uster.  - [x] Mi
+00000bd0: 6e69 4261 7463 684b 6d65 616e 730a 0a57  niBatchKmeans..W
+00000be0: 6869 6c65 2070 726f 7669 6469 6e67 2072  hile providing r
+00000bf0: 6963 6820 6675 6e63 7469 6f6e 732c 202a  ich functions, *
+00000c00: 2a70 7974 6578 7463 6c61 7373 6966 6965  *pytextclassifie
+00000c10: 722a 2a20 696e 7465 726e 616c 206d 6f64  r** internal mod
+00000c20: 756c 6573 2061 6468 6572 6520 746f 206c  ules adhere to l
+00000c30: 6f77 2063 6f75 706c 696e 672c 206d 6f64  ow coupling, mod
+00000c40: 656c 2061 6468 6572 656e 6365 2074 6f20  el adherence to 
+00000c50: 696e 6572 7420 6c6f 6164 696e 672c 2064  inert loading, d
+00000c60: 6963 7469 6f6e 6172 7920 7075 626c 6963  ictionary public
+00000c70: 6174 696f 6e2c 2061 6e64 2065 6173 7920  ation, and easy 
+00000c80: 746f 2075 7365 2e0a 0a23 2320 496e 7374  to use...## Inst
+00000c90: 616c 6c0a 0a2d 2052 6571 7569 7265 6d65  all..- Requireme
+00000ca0: 6e74 7320 616e 6420 496e 7374 616c 6c61  nts and Installa
+00000cb0: 7469 6f6e 0a0a 6060 600a 7069 7033 2069  tion..```.pip3 i
+00000cc0: 6e73 7461 6c6c 2074 6f72 6368 2023 2063  nstall torch # c
+00000cd0: 6f6e 6461 2069 6e73 7461 6c6c 2070 7974  onda install pyt
+00000ce0: 6f72 6368 0a70 6970 3320 696e 7374 616c  orch.pip3 instal
+00000cf0: 6c20 7079 7465 7874 636c 6173 7369 6669  l pytextclassifi
+00000d00: 6572 0a60 6060 0a0a 6f72 0a0a 6060 600a  er.```..or..```.
+00000d10: 6769 7420 636c 6f6e 6520 6874 7470 733a  git clone https:
+00000d20: 2f2f 6769 7468 7562 2e63 6f6d 2f73 6869  //github.com/shi
+00000d30: 6269 6e67 3632 342f 7079 7465 7874 636c  bing624/pytextcl
+00000d40: 6173 7369 6669 6572 2e67 6974 0a63 6420  assifier.git.cd 
+00000d50: 7079 7465 7874 636c 6173 7369 6669 6572  pytextclassifier
+00000d60: 0a70 7974 686f 6e33 2073 6574 7570 2e70  .python3 setup.p
+00000d70: 7920 696e 7374 616c 6c0a 6060 600a 0a0a  y install.```...
+00000d80: 2323 2055 7361 6765 0a23 2323 2054 6578  ## Usage.### Tex
+00000d90: 7420 436c 6173 7369 6669 6572 0a0a 2323  t Classifier..##
+00000da0: 2320 456e 676c 6973 6820 5465 7874 2043  # English Text C
+00000db0: 6c61 7373 6966 6965 720a 0a49 6e63 6c75  lassifier..Inclu
+00000dc0: 6469 6e67 206d 6f64 656c 2074 7261 696e  ding model train
+00000dd0: 696e 672c 2073 6176 696e 672c 2070 7265  ing, saving, pre
+00000de0: 6469 6374 2c20 6576 616c 7561 7465 2c20  dict, evaluate, 
+00000df0: 666f 7220 6578 616d 706c 6520 5b65 7861  for example [exa
+00000e00: 6d70 6c65 732f 6c72 5f65 6e5f 636c 6173  mples/lr_en_clas
+00000e10: 7369 6669 6361 7469 6f6e 5f64 656d 6f2e  sification_demo.
+00000e20: 7079 5d28 6874 7470 733a 2f2f 6769 7468  py](https://gith
+00000e30: 7562 2e63 6f6d 2f73 6869 6269 6e67 3632  ub.com/shibing62
+00000e40: 342f 7079 7465 7874 636c 6173 7369 6669  4/pytextclassifi
+00000e50: 6572 2f62 6c6f 622f 6d61 7374 6572 2f65  er/blob/master/e
+00000e60: 7861 6d70 6c65 732f 6c72 5f65 6e5f 636c  xamples/lr_en_cl
+00000e70: 6173 7369 6669 6361 7469 6f6e 5f64 656d  assification_dem
+00000e80: 6f2e 7079 293a 0a0a 6060 6070 7974 686f  o.py):..```pytho
+00000e90: 6e0a 696d 706f 7274 2073 7973 0a0a 7379  n.import sys..sy
+00000ea0: 732e 7061 7468 2e61 7070 656e 6428 272e  s.path.append('.
+00000eb0: 2e27 290a 6672 6f6d 2070 7974 6578 7463  .').from pytextc
+00000ec0: 6c61 7373 6966 6965 7220 696d 706f 7274  lassifier import
+00000ed0: 2043 6c61 7373 6963 436c 6173 7369 6669   ClassicClassifi
+00000ee0: 6572 0a0a 6966 205f 5f6e 616d 655f 5f20  er..if __name__ 
+00000ef0: 3d3d 2027 5f5f 6d61 696e 5f5f 273a 0a20  == '__main__':. 
+00000f00: 2020 206d 203d 2043 6c61 7373 6963 436c     m = ClassicCl
+00000f10: 6173 7369 6669 6572 286f 7574 7075 745f  assifier(output_
+00000f20: 6469 723d 276d 6f64 656c 732f 6c72 272c  dir='models/lr',
+00000f30: 206d 6f64 656c 5f6e 616d 655f 6f72 5f6d   model_name_or_m
+00000f40: 6f64 656c 3d27 6c72 2729 0a20 2020 2023  odel='lr').    #
+00000f50: 2043 6c61 7373 6963 436c 6173 7369 6669   ClassicClassifi
+00000f60: 6572 2073 7570 706f 7274 206d 6f64 656c  er support model
+00000f70: 5f6e 616d 65ef bc9a 6c72 2c20 7261 6e64  _name...lr, rand
+00000f80: 6f6d 5f66 6f72 6573 742c 2064 6563 6973  om_forest, decis
+00000f90: 696f 6e5f 7472 6565 2c20 6b6e 6e2c 2062  ion_tree, knn, b
+00000fa0: 6179 6573 2c20 7376 6d2c 2078 6762 6f6f  ayes, svm, xgboo
+00000fb0: 7374 0a20 2020 2070 7269 6e74 286d 290a  st.    print(m).
+00000fc0: 2020 2020 6461 7461 203d 205b 0a20 2020      data = [.   
+00000fd0: 2020 2020 2028 2765 6475 6361 7469 6f6e       ('education
+00000fe0: 272c 2027 5374 7564 656e 7420 6465 6274  ', 'Student debt
+00000ff0: 2074 6f20 636f 7374 2042 7269 7461 696e   to cost Britain
+00001000: 2062 696c 6c69 6f6e 7320 7769 7468 696e   billions within
+00001010: 2064 6563 6164 6573 2729 2c0a 2020 2020   decades'),.    
+00001020: 2020 2020 2827 6564 7563 6174 696f 6e27      ('education'
+00001030: 2c20 2743 6869 6e65 7365 2065 6475 6361  , 'Chinese educa
+00001040: 7469 6f6e 2066 6f72 2054 5620 6578 7065  tion for TV expe
+00001050: 7269 6d65 6e74 2729 2c0a 2020 2020 2020  riment'),.      
+00001060: 2020 2827 7370 6f72 7473 272c 2027 4d69    ('sports', 'Mi
+00001070: 6464 6c65 2045 6173 7420 616e 6420 4173  ddle East and As
+00001080: 6961 2062 6f6f 7374 2069 6e76 6573 746d  ia boost investm
+00001090: 656e 7420 696e 2074 6f70 206c 6576 656c  ent in top level
+000010a0: 2073 706f 7274 7327 292c 0a20 2020 2020   sports'),.     
+000010b0: 2020 2028 2773 706f 7274 7327 2c20 2753     ('sports', 'S
+000010c0: 756d 6d69 7420 5365 7269 6573 206c 6f6f  ummit Series loo
+000010d0: 6b20 6c61 756e 6368 6573 2048 424f 2043  k launches HBO C
+000010e0: 616e 6164 6120 7370 6f72 7473 2064 6f63  anada sports doc
+000010f0: 2073 6572 6965 733a 204d 7564 6861 7227   series: Mudhar'
+00001100: 290a 2020 2020 5d0a 2020 2020 2320 7472  ).    ].    # tr
+00001110: 6169 6e20 616e 6420 7361 7665 2062 6573  ain and save bes
+00001120: 7420 6d6f 6465 6c0a 2020 2020 6d2e 7472  t model.    m.tr
+00001130: 6169 6e28 6461 7461 290a 2020 2020 2320  ain(data).    # 
+00001140: 6c6f 6164 2062 6573 7420 6d6f 6465 6c20  load best model 
+00001150: 6672 6f6d 206d 6f64 656c 5f64 6972 0a20  from model_dir. 
+00001160: 2020 206d 2e6c 6f61 645f 6d6f 6465 6c28     m.load_model(
+00001170: 290a 2020 2020 7072 6564 6963 745f 6c61  ).    predict_la
+00001180: 6265 6c2c 2070 7265 6469 6374 5f70 726f  bel, predict_pro
+00001190: 6261 203d 206d 2e70 7265 6469 6374 285b  ba = m.predict([
+000011a0: 0a20 2020 2020 2020 2027 4162 626f 7474  .        'Abbott
+000011b0: 2067 6f76 6572 6e6d 656e 7420 7370 656e   government spen
+000011c0: 6473 2024 3820 6d69 6c6c 696f 6e20 6f6e  ds $8 million on
+000011d0: 2068 6967 6865 7220 6564 7563 6174 696f   higher educatio
+000011e0: 6e20 6d65 6469 6120 626c 6974 7a27 5d29  n media blitz'])
+000011f0: 0a20 2020 2070 7269 6e74 2866 2770 7265  .    print(f'pre
+00001200: 6469 6374 5f6c 6162 656c 3a20 7b70 7265  dict_label: {pre
+00001210: 6469 6374 5f6c 6162 656c 7d2c 2070 7265  dict_label}, pre
+00001220: 6469 6374 5f70 726f 6261 3a20 7b70 7265  dict_proba: {pre
+00001230: 6469 6374 5f70 726f 6261 7d27 290a 0a20  dict_proba}').. 
+00001240: 2020 2074 6573 745f 6461 7461 203d 205b     test_data = [
+00001250: 0a20 2020 2020 2020 2028 2765 6475 6361  .        ('educa
+00001260: 7469 6f6e 272c 2027 4162 626f 7474 2067  tion', 'Abbott g
+00001270: 6f76 6572 6e6d 656e 7420 7370 656e 6473  overnment spends
+00001280: 2024 3820 6d69 6c6c 696f 6e20 6f6e 2068   $8 million on h
+00001290: 6967 6865 7220 6564 7563 6174 696f 6e20  igher education 
+000012a0: 6d65 6469 6120 626c 6974 7a27 292c 0a20  media blitz'),. 
+000012b0: 2020 2020 2020 2028 2773 706f 7274 7327         ('sports'
+000012c0: 2c20 274d 6964 646c 6520 4561 7374 2061  , 'Middle East a
+000012d0: 6e64 2041 7369 6120 626f 6f73 7420 696e  nd Asia boost in
+000012e0: 7665 7374 6d65 6e74 2069 6e20 746f 7020  vestment in top 
+000012f0: 6c65 7665 6c20 7370 6f72 7473 2729 2c0a  level sports'),.
+00001300: 2020 2020 5d0a 2020 2020 6163 635f 7363      ].    acc_sc
+00001310: 6f72 6520 3d20 6d2e 6576 616c 7561 7465  ore = m.evaluate
+00001320: 5f6d 6f64 656c 2874 6573 745f 6461 7461  _model(test_data
+00001330: 290a 2020 2020 7072 696e 7428 6627 6163  ).    print(f'ac
+00001340: 635f 7363 6f72 653a 207b 6163 635f 7363  c_score: {acc_sc
+00001350: 6f72 657d 2729 0a60 6060 0a0a 6f75 7470  ore}').```..outp
+00001360: 7574 3a0a 0a60 6060 0a43 6c61 7373 6963  ut:..```.Classic
+00001370: 436c 6173 7369 6669 6572 2069 6e73 7461  Classifier insta
+00001380: 6e63 6520 284c 6f67 6973 7469 6352 6567  nce (LogisticReg
+00001390: 7265 7373 696f 6e28 6669 745f 696e 7465  ression(fit_inte
+000013a0: 7263 6570 743d 4661 6c73 6529 2c20 7374  rcept=False), st
+000013b0: 6f70 776f 7264 7320 7369 7a65 3a20 3234  opwords size: 24
+000013c0: 3338 290a 7072 6564 6963 745f 6c61 6265  38).predict_labe
+000013d0: 6c3a 205b 2765 6475 6361 7469 6f6e 275d  l: ['education']
+000013e0: 2c20 7072 6564 6963 745f 7072 6f62 613a  , predict_proba:
+000013f0: 205b 302e 3533 3738 3233 3633 3538 3439   [0.537823635849
+00001400: 3231 3132 5d0a 6163 635f 7363 6f72 653a  2112].acc_score:
+00001410: 2031 2e30 0a60 6060 0a0a 2323 2320 4368   1.0.```..### Ch
+00001420: 696e 6573 6520 5465 7874 2043 6c61 7373  inese Text Class
+00001430: 6966 6965 7228 e4b8 ade6 9687 e696 87e6  ifier(..........
+00001440: 9cac e588 86e7 b1bb 290a 0a54 6578 7420  ........)..Text 
+00001450: 636c 6173 7369 6669 6361 7469 6f6e 2063  classification c
+00001460: 6f6d 7061 7469 626c 6520 7769 7468 2043  ompatible with C
+00001470: 6869 6e65 7365 2061 6e64 2045 6e67 6c69  hinese and Engli
+00001480: 7368 2063 6f72 706f 7261 2e0a 0a65 7861  sh corpora...exa
+00001490: 6d70 6c65 205b 6578 616d 706c 6573 2f6c  mple [examples/l
+000014a0: 725f 636c 6173 7369 6669 6361 7469 6f6e  r_classification
+000014b0: 5f64 656d 6f2e 7079 5d28 6874 7470 733a  _demo.py](https:
+000014c0: 2f2f 6769 7468 7562 2e63 6f6d 2f73 6869  //github.com/shi
+000014d0: 6269 6e67 3632 342f 7079 7465 7874 636c  bing624/pytextcl
+000014e0: 6173 7369 6669 6572 2f62 6c6f 622f 6d61  assifier/blob/ma
+000014f0: 7374 6572 2f65 7861 6d70 6c65 732f 6c72  ster/examples/lr
+00001500: 5f63 6c61 7373 6966 6963 6174 696f 6e5f  _classification_
+00001510: 6465 6d6f 2e70 7929 0a0a 6060 6070 7974  demo.py)..```pyt
+00001520: 686f 6e0a 696d 706f 7274 2073 7973 0a0a  hon.import sys..
+00001530: 7379 732e 7061 7468 2e61 7070 656e 6428  sys.path.append(
+00001540: 272e 2e27 290a 6672 6f6d 2070 7974 6578  '..').from pytex
+00001550: 7463 6c61 7373 6966 6965 7220 696d 706f  tclassifier impo
+00001560: 7274 2043 6c61 7373 6963 436c 6173 7369  rt ClassicClassi
+00001570: 6669 6572 0a0a 6966 205f 5f6e 616d 655f  fier..if __name_
+00001580: 5f20 3d3d 2027 5f5f 6d61 696e 5f5f 273a  _ == '__main__':
+00001590: 0a20 2020 206d 203d 2043 6c61 7373 6963  .    m = Classic
+000015a0: 436c 6173 7369 6669 6572 286f 7574 7075  Classifier(outpu
+000015b0: 745f 6469 723d 276d 6f64 656c 732f 6c72  t_dir='models/lr
+000015c0: 2d74 6f79 272c 206d 6f64 656c 5f6e 616d  -toy', model_nam
+000015d0: 655f 6f72 5f6d 6f64 656c 3d27 6c72 2729  e_or_model='lr')
+000015e0: 0a20 2020 2023 20e7 bb8f e585 b8e5 8886  .    # .........
+000015f0: e7b1 bbe6 96b9 e6b3 95ef bc8c e694 afe6  ................
+00001600: 8c81 e79a 84e6 a8a1 e59e 8be5 8c85 e68b  ................
+00001610: acef bc9a 6c72 2c20 7261 6e64 6f6d 5f66  ....lr, random_f
+00001620: 6f72 6573 742c 2064 6563 6973 696f 6e5f  orest, decision_
+00001630: 7472 6565 2c20 6b6e 6e2c 2062 6179 6573  tree, knn, bayes
+00001640: 2c20 7376 6d2c 2078 6762 6f6f 7374 0a20  , svm, xgboost. 
+00001650: 2020 2064 6174 6120 3d20 5b0a 2020 2020     data = [.    
+00001660: 2020 2020 2827 6564 7563 6174 696f 6e27      ('education'
+00001670: 2c20 27e5 908d e5b8 88e6 8c87 e5af bce6  , '.............
+00001680: 8998 e7a6 8fe8 afad e6b3 95e6 8a80 e5b7  ................
+00001690: a7ef bc9a e590 8de8 af8d e79a 84e5 a48d  ................
+000016a0: e695 b0e5 bda2 e5bc 8f27 292c 0a20 2020  .........'),.   
+000016b0: 2020 2020 2028 2765 6475 6361 7469 6f6e       ('education
+000016c0: 272c 2027 e4b8 ade5 9bbd e9ab 98e8 8083  ', '............
+000016d0: e688 90e7 bba9 e6b5 b7e5 a496 e8ae a4e5  ................
+000016e0: 8faf 20e6 98af e280 9ce7 8bbc e69d a5e4  .. .............
+000016f0: ba86 e280 9de5 9097 efbc 9f27 292c 0a20  ...........'),. 
+00001700: 2020 2020 2020 2028 2765 6475 6361 7469         ('educati
+00001710: 6f6e 272c 2027 e585 ace5 8aa1 e591 98e8  on', '..........
+00001720: 8083 e899 91e8 b68a e69d a5e8 b68a e590  ................
+00001730: 83e9 a699 efbc 8ce8 bf99 e698 afe6 808e  ................
+00001740: e4b9 88e5 9b9e e4ba 8bef bc9f 2729 2c0a  ............'),.
+00001750: 2020 2020 2020 2020 2827 7370 6f72 7473          ('sports
+00001760: 272c 2027 e59b bee6 9687 efbc 9ae6 b395  ', '............
+00001770: e7bd 91e5 ad9f e88f b2e5 b094 e696 afe8  ................
+00001780: 8ba6 e688 98e8 bf9b 3136 e5bc ba20 e5ad  ........16... ..
+00001790: 9fe8 8fb2 e5b0 94e6 96af e680 92e5 90bc  ................
+000017a0: 2729 2c0a 2020 2020 2020 2020 2827 7370  '),.        ('sp
+000017b0: 6f72 7473 272c 2027 e59b 9be5 b79d e4b8  orts', '........
+000017c0: b9e6 a3b1 e4b8 bee8 a18c e585 a8e5 9bbd  ................
+000017d0: e995 bfe8 b79d e799 bbe5 b1b1 e68c 91e6  ................
+000017e0: 8898 e8b5 9b20 e8bf 91e4 b887 e4ba bae5  ..... ..........
+000017f0: 8f82 e4b8 8e27 292c 0a20 2020 2020 2020  .....'),.       
+00001800: 2028 2773 706f 7274 7327 2c20 27e7 b1b3   ('sports', '...
+00001810: e585 b0e5 aea2 e59c ba38 e688 98e4 b88d  .........8......
+00001820: e8b4 a5e5 9bbd e7b1 b331 30e5 b9b4 e8bf  .........10.....
+00001830: 9ee8 839c 2729 2c0a 2020 2020 5d0a 2020  ....'),.    ].  
+00001840: 2020 6d2e 7472 6169 6e28 6461 7461 290a    m.train(data).
+00001850: 2020 2020 7072 696e 7428 6d29 0a20 2020      print(m).   
+00001860: 2023 206c 6f61 6420 6265 7374 206d 6f64   # load best mod
+00001870: 656c 2066 726f 6d20 6d6f 6465 6c5f 6469  el from model_di
+00001880: 720a 2020 2020 6d2e 6c6f 6164 5f6d 6f64  r.    m.load_mod
+00001890: 656c 2829 0a20 2020 2070 7265 6469 6374  el().    predict
+000018a0: 5f6c 6162 656c 2c20 7072 6564 6963 745f  _label, predict_
+000018b0: 7072 6f62 6120 3d20 6d2e 7072 6564 6963  proba = m.predic
+000018c0: 7428 5b27 e7a6 8fe5 bbba e698 a5e5 ada3  t(['............
+000018d0: e585 ace5 8aa1 e591 98e8 8083 e8af 95e6  ................
+000018e0: 8aa5 e590 8d31 38e6 97a5 e688 aae6 ada2  .....18.........
+000018f0: 2032 e69c 8836 e697 a5e8 8083 e8af 9527   2...6.........'
+00001900: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001930: 27e6 848f e794 b2e9 a696 e8bd aee8 a1a5  '...............
+00001940: e8b5 9be4 baa4 e688 98e8 aeb0 e5bd 953a  ...............:
+00001950: e7b1 b3e5 85b0 e5ae a2e5 9cba 38e6 8898  ............8...
+00001960: e4b8 8de8 b4a5 e59b bde7 b1b3 3130 e5b9  ............10..
+00001970: b4e8 bf9e e883 9c27 5d29 0a20 2020 2070  .......']).    p
+00001980: 7269 6e74 2866 2770 7265 6469 6374 5f6c  rint(f'predict_l
+00001990: 6162 656c 3a20 7b70 7265 6469 6374 5f6c  abel: {predict_l
+000019a0: 6162 656c 7d2c 2070 7265 6469 6374 5f70  abel}, predict_p
+000019b0: 726f 6261 3a20 7b70 7265 6469 6374 5f70  roba: {predict_p
+000019c0: 726f 6261 7d27 290a 0a20 2020 2074 6573  roba}')..    tes
+000019d0: 745f 6461 7461 203d 205b 0a20 2020 2020  t_data = [.     
+000019e0: 2020 2028 2765 6475 6361 7469 6f6e 272c     ('education',
+000019f0: 2027 e7a6 8fe5 bbba e698 a5e5 ada3 e585   '..............
+00001a00: ace5 8aa1 e591 98e8 8083 e8af 95e6 8aa5  ................
+00001a10: e590 8d31 38e6 97a5 e688 aae6 ada2 2032  ...18......... 2
+00001a20: e69c 8836 e697 a5e8 8083 e8af 9527 292c  ...6.........'),
+00001a30: 0a20 2020 2020 2020 2028 2773 706f 7274  .        ('sport
+00001a40: 7327 2c20 27e6 848f e794 b2e9 a696 e8bd  s', '...........
+00001a50: aee8 a1a5 e8b5 9be4 baa4 e688 98e8 aeb0  ................
+00001a60: e5bd 953a e7b1 b3e5 85b0 e5ae a2e5 9cba  ...:............
+00001a70: 38e6 8898 e4b8 8de8 b4a5 e59b bde7 b1b3  8...............
+00001a80: 3130 e5b9 b4e8 bf9e e883 9c27 292c 0a20  10.........'),. 
+00001a90: 2020 205d 0a20 2020 2061 6363 5f73 636f     ].    acc_sco
+00001aa0: 7265 203d 206d 2e65 7661 6c75 6174 655f  re = m.evaluate_
+00001ab0: 6d6f 6465 6c28 7465 7374 5f64 6174 6129  model(test_data)
+00001ac0: 0a20 2020 2070 7269 6e74 2866 2761 6363  .    print(f'acc
+00001ad0: 5f73 636f 7265 3a20 7b61 6363 5f73 636f  _score: {acc_sco
+00001ae0: 7265 7d27 2920 2023 2031 2e30 0a0a 2020  re}')  # 1.0..  
+00001af0: 2020 2323 2323 2074 7261 696e 206d 6f64    #### train mod
+00001b00: 656c 2077 6974 6820 3177 2064 6174 610a  el with 1w data.
+00001b10: 2020 2020 7072 696e 7428 272d 2720 2a20      print('-' * 
+00001b20: 3432 290a 2020 2020 6d20 3d20 436c 6173  42).    m = Clas
+00001b30: 7369 6343 6c61 7373 6966 6965 7228 6f75  sicClassifier(ou
+00001b40: 7470 7574 5f64 6972 3d27 6d6f 6465 6c73  tput_dir='models
+00001b50: 2f6c 7227 2c20 6d6f 6465 6c5f 6e61 6d65  /lr', model_name
+00001b60: 5f6f 725f 6d6f 6465 6c3d 276c 7227 290a  _or_model='lr').
+00001b70: 2020 2020 6461 7461 5f66 696c 6520 3d20      data_file = 
+00001b80: 2774 6875 636e 6577 735f 7472 6169 6e5f  'thucnews_train_
+00001b90: 3177 2e74 7874 270a 2020 2020 6d2e 7472  1w.txt'.    m.tr
+00001ba0: 6169 6e28 6461 7461 5f66 696c 6529 0a20  ain(data_file). 
+00001bb0: 2020 206d 2e6c 6f61 645f 6d6f 6465 6c28     m.load_model(
+00001bc0: 290a 2020 2020 7072 6564 6963 745f 6c61  ).    predict_la
+00001bd0: 6265 6c2c 2070 7265 6469 6374 5f70 726f  bel, predict_pro
+00001be0: 6261 203d 206d 2e70 7265 6469 6374 280a  ba = m.predict(.
+00001bf0: 2020 2020 2020 2020 5b27 e9a1 bae4 b989          ['......
+00001c00: e58c 97e4 baac e88b 8fe6 b4bb 3838 e5b9  ............88..
+00001c10: b3e7 b1b3 e8b5 b7e7 b2be e8a3 85e6 88bf  ................
+00001c20: e59c a8e5 94ae 272c 0a20 2020 2020 2020  ......',.       
+00001c30: 2020 27e7 be8e 4542 2d35 e9a1 b9e7 9bae    '...EB-5......
+00001c40: e280 9c31 35e6 97a5 e5bf abe9 809f e7a7  ...15...........
+00001c50: bbe6 b091 e280 9de5 b086 e68e a8e8 bf9f  ................
+00001c60: 275d 290a 2020 2020 7072 696e 7428 6627  ']).    print(f'
+00001c70: 7072 6564 6963 745f 6c61 6265 6c3a 207b  predict_label: {
+00001c80: 7072 6564 6963 745f 6c61 6265 6c7d 2c20  predict_label}, 
+00001c90: 7072 6564 6963 745f 7072 6f62 613a 207b  predict_proba: {
+00001ca0: 7072 6564 6963 745f 7072 6f62 617d 2729  predict_proba}')
+00001cb0: 0a60 6060 0a0a 6f75 7470 7574 3a0a 0a60  .```..output:..`
+00001cc0: 6060 0a43 6c61 7373 6963 436c 6173 7369  ``.ClassicClassi
+00001cd0: 6669 6572 2069 6e73 7461 6e63 6520 284c  fier instance (L
+00001ce0: 6f67 6973 7469 6352 6567 7265 7373 696f  ogisticRegressio
+00001cf0: 6e28 6669 745f 696e 7465 7263 6570 743d  n(fit_intercept=
+00001d00: 4661 6c73 6529 2c20 7374 6f70 776f 7264  False), stopword
+00001d10: 7320 7369 7a65 3a20 3234 3338 290a 7072  s size: 2438).pr
+00001d20: 6564 6963 745f 6c61 6265 6c3a 205b 2765  edict_label: ['e
+00001d30: 6475 6361 7469 6f6e 2720 2773 706f 7274  ducation' 'sport
+00001d40: 7327 5d2c 2070 7265 6469 6374 5f70 726f  s'], predict_pro
+00001d50: 6261 3a20 5b30 2e35 2c20 302e 3539 3839  ba: [0.5, 0.5989
+00001d60: 3431 3830 3637 3431 3533 345d 0a61 6363  41806741534].acc
+00001d70: 5f73 636f 7265 3a20 312e 300a 2d2d 2d2d  _score: 1.0.----
+00001d80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001d90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001da0: 2d2d 2d2d 2d2d 0a70 7265 6469 6374 5f6c  ------.predict_l
+00001db0: 6162 656c 3a20 5b27 7265 616c 7479 2720  abel: ['realty' 
+00001dc0: 2765 6475 6361 7469 6f6e 275d 2c20 7072  'education'], pr
+00001dd0: 6564 6963 745f 7072 6f62 613a 205b 302e  edict_proba: [0.
+00001de0: 3733 3032 3935 3639 3233 3631 3733 3732  7302956923617372
+00001df0: 2c20 302e 3235 3635 3030 3534 3435 3332  , 0.256500544532
+00001e00: 3239 3233 5d0a 6060 600a 0a23 2323 2056  2923].```..### V
+00001e10: 6973 7561 6c20 4665 6174 7572 6520 496d  isual Feature Im
+00001e20: 706f 7274 616e 6365 0a0a 5368 6f77 2066  portance..Show f
+00001e30: 6561 7475 7265 2077 6569 6768 7473 206f  eature weights o
+00001e40: 6620 6d6f 6465 6c2c 2061 6e64 2070 7265  f model, and pre
+00001e50: 6469 6374 696f 6e20 776f 7264 2077 6569  diction word wei
+00001e60: 6768 742c 2066 6f72 2065 7861 6d70 6c65  ght, for example
+00001e70: 205b 6578 616d 706c 6573 2f76 6973 7561   [examples/visua
+00001e80: 6c5f 6665 6174 7572 655f 696d 706f 7274  l_feature_import
+00001e90: 616e 6365 2e69 7079 6e62 5d28 6874 7470  ance.ipynb](http
+00001ea0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
+00001eb0: 6869 6269 6e67 3632 342f 7079 7465 7874  hibing624/pytext
+00001ec0: 636c 6173 7369 6669 6572 2f62 6c6f 622f  classifier/blob/
+00001ed0: 6d61 7374 6572 2f65 7861 6d70 6c65 732f  master/examples/
+00001ee0: 7669 7375 616c 5f66 6561 7475 7265 5f69  visual_feature_i
+00001ef0: 6d70 6f72 7461 6e63 652e 6970 796e 6229  mportance.ipynb)
+00001f00: 0a0a 6060 6070 7974 686f 6e0a 696d 706f  ..```python.impo
+00001f10: 7274 2073 7973 0a0a 7379 732e 7061 7468  rt sys..sys.path
+00001f20: 2e61 7070 656e 6428 272e 2e27 290a 6672  .append('..').fr
+00001f30: 6f6d 2070 7974 6578 7463 6c61 7373 6966  om pytextclassif
+00001f40: 6965 7220 696d 706f 7274 2043 6c61 7373  ier import Class
+00001f50: 6963 436c 6173 7369 6669 6572 0a69 6d70  icClassifier.imp
+00001f60: 6f72 7420 6a69 6562 610a 0a74 6320 3d20  ort jieba..tc = 
+00001f70: 436c 6173 7369 6343 6c61 7373 6966 6965  ClassicClassifie
+00001f80: 7228 6f75 7470 7574 5f64 6972 3d27 6d6f  r(output_dir='mo
+00001f90: 6465 6c73 2f6c 722d 746f 7927 2c20 6d6f  dels/lr-toy', mo
+00001fa0: 6465 6c5f 6e61 6d65 5f6f 725f 6d6f 6465  del_name_or_mode
+00001fb0: 6c3d 276c 7227 290a 6461 7461 203d 205b  l='lr').data = [
+00001fc0: 0a20 2020 2028 2765 6475 6361 7469 6f6e  .    ('education
+00001fd0: 272c 2027 e590 8de5 b888 e68c 87e5 afbc  ', '............
+00001fe0: e689 98e7 a68f e8af ade6 b395 e68a 80e5  ................
+00001ff0: b7a7 efbc 9ae5 908d e8af 8de7 9a84 e5a4  ................
+00002000: 8de6 95b0 e5bd a2e5 bc8f 2729 2c0a 2020  ..........'),.  
+00002010: 2020 2827 6564 7563 6174 696f 6e27 2c20    ('education', 
+00002020: 27e4 b8ad e59b bde9 ab98 e880 83e6 8890  '...............
+00002030: e7bb a9e6 b5b7 e5a4 96e8 aea4 e58f af20  ............... 
+00002040: e698 afe2 809c e78b bce6 9da5 e4ba 86e2  ................
+00002050: 809d e590 97ef bc9f 2729 2c0a 2020 2020  ........'),.    
+00002060: 2827 7370 6f72 7473 272c 2027 e59b bee6  ('sports', '....
+00002070: 9687 efbc 9ae6 b395 e7bd 91e5 ad9f e88f  ................
+00002080: b2e5 b094 e696 afe8 8ba6 e688 98e8 bf9b  ................
+00002090: 3136 e5bc ba20 e5ad 9fe8 8fb2 e5b0 94e6  16... ..........
+000020a0: 96af e680 92e5 90bc 2729 2c0a 2020 2020  ........'),.    
+000020b0: 2827 7370 6f72 7473 272c 2027 e59b 9be5  ('sports', '....
+000020c0: b79d e4b8 b9e6 a3b1 e4b8 bee8 a18c e585  ................
+000020d0: a8e5 9bbd e995 bfe8 b79d e799 bbe5 b1b1  ................
+000020e0: e68c 91e6 8898 e8b5 9b20 e8bf 91e4 b887  ......... ......
+000020f0: e4ba bae5 8f82 e4b8 8e27 292c 0a20 2020  .........'),.   
+00002100: 2028 2773 706f 7274 7327 2c20 27e7 b1b3   ('sports', '...
+00002110: e585 b0e5 aea2 e59c ba38 e688 98e4 b88d  .........8......
+00002120: e8b4 a5e5 9bbd e7b1 b331 30e5 b9b4 e8bf  .........10.....
+00002130: 9ee8 839c 2729 0a5d 0a74 632e 7472 6169  ....').].tc.trai
+00002140: 6e28 6461 7461 290a 696d 706f 7274 2065  n(data).import e
+00002150: 6c69 350a 0a69 6e66 6572 5f64 6174 6120  li5..infer_data 
+00002160: 3d20 5b27 e9ab 98e8 8083 e68c 87e5 afbc  = ['............
+00002170: e689 98e7 a68f e8af ade6 b395 e68a 80e5  ................
+00002180: b7a7 e59b bde9 9985 e8ae a4e5 8faf 272c  ..............',
+00002190: 0a20 2020 2020 2020 2020 2020 2020 2027  .              '
+000021a0: e684 8fe7 94b2 e9a6 96e8 bdae e8a1 a5e8  ................
+000021b0: b59b e4ba a4e6 8898 e8ae b0e5 bd95 3ae7  ..............:.
+000021c0: b1b3 e585 b0e5 aea2 e59c ba38 e688 98e4  ...........8....
+000021d0: b88d e8b4 a5e5 9bbd e7b1 b331 30e5 b9b4  ...........10...
+000021e0: e8bf 9ee8 839c 275d 0a65 6c69 352e 7368  ......'].eli5.sh
+000021f0: 6f77 5f77 6569 6768 7473 2874 632e 6d6f  ow_weights(tc.mo
+00002200: 6465 6c2c 2076 6563 3d74 632e 6665 6174  del, vec=tc.feat
+00002210: 7572 6529 0a73 6567 5f69 6e66 6572 5f64  ure).seg_infer_d
+00002220: 6174 6120 3d20 5b27 2027 2e6a 6f69 6e28  ata = [' '.join(
+00002230: 6a69 6562 612e 6c63 7574 2869 2929 2066  jieba.lcut(i)) f
+00002240: 6f72 2069 2069 6e20 696e 6665 725f 6461  or i in infer_da
+00002250: 7461 5d0a 656c 6935 2e73 686f 775f 7072  ta].eli5.show_pr
+00002260: 6564 6963 7469 6f6e 2874 632e 6d6f 6465  ediction(tc.mode
+00002270: 6c2c 2073 6567 5f69 6e66 6572 5f64 6174  l, seg_infer_dat
+00002280: 615b 305d 2c20 7665 633d 7463 2e66 6561  a[0], vec=tc.fea
+00002290: 7475 7265 2c0a 2020 2020 2020 2020 2020  ture,.          
+000022a0: 2020 2020 2020 2020 2020 2074 6172 6765             targe
+000022b0: 745f 6e61 6d65 733d 5b27 6564 7563 6174  t_names=['educat
+000022c0: 696f 6e27 2c20 2773 706f 7274 7327 5d29  ion', 'sports'])
+000022d0: 0a60 6060 0a0a 6f75 7470 7574 3a0a 0a21  .```..output:..!
+000022e0: 5b69 6d67 2e70 6e67 5d28 646f 6373 2f69  [img.png](docs/i
+000022f0: 6d67 2e70 6e67 290a 0a23 2323 2044 6565  mg.png)..### Dee
+00002300: 7020 436c 6173 7369 6669 6361 7469 6f6e  p Classification
+00002310: 206d 6f64 656c 0a0a e69c ace9 a1b9 e79b   model..........
+00002320: aee6 94af e68c 81e4 bba5 e4b8 8be6 b7b1  ................
+00002330: e5ba a6e5 8886 e7b1 bbe6 a8a1 e59e 8bef  ................
+00002340: bc9a 4661 7374 5465 7874 e380 8154 6578  ..FastText...Tex
+00002350: 7443 4e4e e380 8154 6578 7452 4e4e e380  tCNN...TextRNN..
+00002360: 8142 6572 74e6 a8a1 e59e 8bef bc8c 6069  .Bert.........`i
+00002370: 6d70 6f72 7460 e6a8 a1e5 9e8b e5af b9e5  mport`..........
+00002380: ba94 e79a 84e6 96b9 e6b3 95e6 9da5 e8b0  ................
+00002390: 83e7 94a8 efbc 9a0a 6060 6070 7974 686f  ........```pytho
+000023a0: 6e0a 6672 6f6d 2070 7974 6578 7463 6c61  n.from pytextcla
+000023b0: 7373 6966 6965 7220 696d 706f 7274 2046  ssifier import F
+000023c0: 6173 7454 6578 7443 6c61 7373 6966 6965  astTextClassifie
+000023d0: 722c 2054 6578 7443 4e4e 436c 6173 7369  r, TextCNNClassi
+000023e0: 6669 6572 2c20 5465 7874 524e 4e43 6c61  fier, TextRNNCla
+000023f0: 7373 6966 6965 722c 2042 6572 7443 6c61  ssifier, BertCla
+00002400: 7373 6966 6965 720a 6060 600a 0ae4 b88b  ssifier.```.....
+00002410: e99d a2e4 bba5 4661 7374 5465 7874 e6a8  ......FastText..
+00002420: a1e5 9e8b e4b8 bae7 a4ba e4be 8bef bc8c  ................
+00002430: e585 b6e4 bb96 e6a8 a1e5 9e8b e79a 84e4  ................
+00002440: bdbf e794 a8e6 96b9 e6b3 95e7 b1bb e4bc  ................
+00002450: bce3 8082 0a0a 2323 2320 4661 7374 5465  ......### FastTe
+00002460: 7874 20e6 a8a1 e59e 8b0a 0ae8 aead e7bb  xt .............
+00002470: 83e5 928c e9a2 84e6 b58b 6046 6173 7454  ..........`FastT
+00002480: 6578 7460 e6a8 a1e5 9e8b e7a4 bae4 be8b  ext`............
+00002490: 5b65 7861 6d70 6c65 732f 6661 7374 7465  [examples/fastte
+000024a0: 7874 5f63 6c61 7373 6966 6963 6174 696f  xt_classificatio
+000024b0: 6e5f 6465 6d6f 2e70 795d 2868 7474 7073  n_demo.py](https
+000024c0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7368  ://github.com/sh
+000024d0: 6962 696e 6736 3234 2f70 7974 6578 7463  ibing624/pytextc
+000024e0: 6c61 7373 6966 6965 722f 626c 6f62 2f6d  lassifier/blob/m
+000024f0: 6173 7465 722f 6578 616d 706c 6573 2f66  aster/examples/f
+00002500: 6173 7474 6578 745f 636c 6173 7369 6669  asttext_classifi
+00002510: 6361 7469 6f6e 5f64 656d 6f2e 7079 290a  cation_demo.py).
+00002520: 0a60 6060 7079 7468 6f6e 0a69 6d70 6f72  .```python.impor
+00002530: 7420 7379 730a 0a73 7973 2e70 6174 682e  t sys..sys.path.
+00002540: 6170 7065 6e64 2827 2e2e 2729 0a66 726f  append('..').fro
+00002550: 6d20 7079 7465 7874 636c 6173 7369 6669  m pytextclassifi
+00002560: 6572 2069 6d70 6f72 7420 4661 7374 5465  er import FastTe
+00002570: 7874 436c 6173 7369 6669 6572 2c20 6c6f  xtClassifier, lo
+00002580: 6164 5f64 6174 610a 0a69 6620 5f5f 6e61  ad_data..if __na
+00002590: 6d65 5f5f 203d 3d20 275f 5f6d 6169 6e5f  me__ == '__main_
+000025a0: 5f27 3a0a 2020 2020 6d20 3d20 4661 7374  _':.    m = Fast
+000025b0: 5465 7874 436c 6173 7369 6669 6572 286f  TextClassifier(o
+000025c0: 7574 7075 745f 6469 723d 276d 6f64 656c  utput_dir='model
+000025d0: 732f 6661 7374 7465 7874 2d74 6f79 2729  s/fasttext-toy')
+000025e0: 0a20 2020 2064 6174 6120 3d20 5b0a 2020  .    data = [.  
+000025f0: 2020 2020 2020 2827 6564 7563 6174 696f        ('educatio
+00002600: 6e27 2c20 27e5 908d e5b8 88e6 8c87 e5af  n', '...........
+00002610: bce6 8998 e7a6 8fe8 afad e6b3 95e6 8a80  ................
+00002620: e5b7 a7ef bc9a e590 8de8 af8d e79a 84e5  ................
+00002630: a48d e695 b0e5 bda2 e5bc 8f27 292c 0a20  ...........'),. 
+00002640: 2020 2020 2020 2028 2765 6475 6361 7469         ('educati
+00002650: 6f6e 272c 2027 e4b8 ade5 9bbd e9ab 98e8  on', '..........
+00002660: 8083 e688 90e7 bba9 e6b5 b7e5 a496 e8ae  ................
+00002670: a4e5 8faf 20e6 98af e280 9ce7 8bbc e69d  .... ...........
+00002680: a5e4 ba86 e280 9de5 9097 efbc 9f27 292c  .............'),
+00002690: 0a20 2020 2020 2020 2028 2765 6475 6361  .        ('educa
+000026a0: 7469 6f6e 272c 2027 e585 ace5 8aa1 e591  tion', '........
+000026b0: 98e8 8083 e899 91e8 b68a e69d a5e8 b68a  ................
+000026c0: e590 83e9 a699 efbc 8ce8 bf99 e698 afe6  ................
+000026d0: 808e e4b9 88e5 9b9e e4ba 8bef bc9f 2729  ..............')
+000026e0: 2c0a 2020 2020 2020 2020 2827 7370 6f72  ,.        ('spor
+000026f0: 7473 272c 2027 e59b bee6 9687 efbc 9ae6  ts', '..........
+00002700: b395 e7bd 91e5 ad9f e88f b2e5 b094 e696  ................
+00002710: afe8 8ba6 e688 98e8 bf9b 3136 e5bc ba20  ..........16... 
+00002720: e5ad 9fe8 8fb2 e5b0 94e6 96af e680 92e5  ................
+00002730: 90bc 2729 2c0a 2020 2020 2020 2020 2827  ..'),.        ('
+00002740: 7370 6f72 7473 272c 2027 e59b 9be5 b79d  sports', '......
+00002750: e4b8 b9e6 a3b1 e4b8 bee8 a18c e585 a8e5  ................
+00002760: 9bbd e995 bfe8 b79d e799 bbe5 b1b1 e68c  ................
+00002770: 91e6 8898 e8b5 9b20 e8bf 91e4 b887 e4ba  ....... ........
+00002780: bae5 8f82 e4b8 8e27 292c 0a20 2020 2020  .......'),.     
+00002790: 2020 2028 2773 706f 7274 7327 2c20 27e7     ('sports', '.
+000027a0: b1b3 e585 b0e5 aea2 e59c ba38 e688 98e4  ...........8....
+000027b0: b88d e8b4 a5e4 bf9d e68c 81e8 bf9e e883  ................
+000027c0: 9c27 292c 0a20 2020 205d 0a20 2020 206d  .'),.    ].    m
+000027d0: 2e74 7261 696e 2864 6174 612c 206e 756d  .train(data, num
+000027e0: 5f65 706f 6368 733d 3329 0a20 2020 2070  _epochs=3).    p
+000027f0: 7269 6e74 286d 290a 2020 2020 2320 6c6f  rint(m).    # lo
+00002800: 6164 2074 7261 696e 6564 2062 6573 7420  ad trained best 
+00002810: 6d6f 6465 6c0a 2020 2020 6d2e 6c6f 6164  model.    m.load
+00002820: 5f6d 6f64 656c 2829 0a20 2020 2070 7265  _model().    pre
+00002830: 6469 6374 5f6c 6162 656c 2c20 7072 6564  dict_label, pred
+00002840: 6963 745f 7072 6f62 6120 3d20 6d2e 7072  ict_proba = m.pr
+00002850: 6564 6963 7428 5b27 e7a6 8fe5 bbba e698  edict(['........
+00002860: a5e5 ada3 e585 ace5 8aa1 e591 98e8 8083  ................
+00002870: e8af 95e6 8aa5 e590 8d31 38e6 97a5 e688  .........18.....
+00002880: aae6 ada2 2032 e69c 8836 e697 a5e8 8083  .... 2...6......
+00002890: e8af 9527 2c0a 2020 2020 2020 2020 2020  ...',.          
+000028a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028c0: 2020 2020 27e6 848f e794 b2e9 a696 e8bd      '...........
+000028d0: aee8 a1a5 e8b5 9be4 baa4 e688 98e8 aeb0  ................
+000028e0: e5bd 953a e7b1 b3e5 85b0 e5ae a2e5 9cba  ...:............
+000028f0: 38e6 8898 e4b8 8de8 b4a5 e59b bde7 b1b3  8...............
+00002900: 3130 e5b9 b4e8 bf9e e883 9c27 5d29 0a20  10.........']). 
+00002910: 2020 2070 7269 6e74 2866 2770 7265 6469     print(f'predi
+00002920: 6374 5f6c 6162 656c 3a20 7b70 7265 6469  ct_label: {predi
+00002930: 6374 5f6c 6162 656c 7d2c 2070 7265 6469  ct_label}, predi
+00002940: 6374 5f70 726f 6261 3a20 7b70 7265 6469  ct_proba: {predi
+00002950: 6374 5f70 726f 6261 7d27 290a 2020 2020  ct_proba}').    
+00002960: 7465 7374 5f64 6174 6120 3d20 5b0a 2020  test_data = [.  
+00002970: 2020 2020 2020 2827 6564 7563 6174 696f        ('educatio
+00002980: 6e27 2c20 27e7 a68f e5bb bae6 98a5 e5ad  n', '...........
+00002990: a3e5 85ac e58a a1e5 9198 e880 83e8 af95  ................
+000029a0: e68a a5e5 908d 3138 e697 a5e6 88aa e6ad  ......18........
+000029b0: a220 32e6 9c88 36e6 97a5 e880 83e8 af95  . 2...6.........
+000029c0: 2729 2c0a 2020 2020 2020 2020 2827 7370  '),.        ('sp
+000029d0: 6f72 7473 272c 2027 e684 8fe7 94b2 e9a6  orts', '........
+000029e0: 96e8 bdae e8a1 a5e8 b59b e4ba a4e6 8898  ................
+000029f0: e8ae b0e5 bd95 3ae7 b1b3 e585 b0e5 aea2  ......:.........
+00002a00: e59c ba38 e688 98e4 b88d e8b4 a5e5 9bbd  ...8............
+00002a10: e7b1 b331 30e5 b9b4 e8bf 9ee8 839c 2729  ...10.........')
+00002a20: 2c0a 2020 2020 5d0a 2020 2020 6163 635f  ,.    ].    acc_
+00002a30: 7363 6f72 6520 3d20 6d2e 6576 616c 7561  score = m.evalua
+00002a40: 7465 5f6d 6f64 656c 2874 6573 745f 6461  te_model(test_da
+00002a50: 7461 290a 2020 2020 7072 696e 7428 6627  ta).    print(f'
+00002a60: 6163 635f 7363 6f72 653a 207b 6163 635f  acc_score: {acc_
+00002a70: 7363 6f72 657d 2729 2020 2320 312e 300a  score}')  # 1.0.
+00002a80: 0a20 2020 2023 2323 2320 7472 6169 6e20  .    #### train 
+00002a90: 6d6f 6465 6c20 7769 7468 2031 7720 6461  model with 1w da
+00002aa0: 7461 0a20 2020 2070 7269 6e74 2827 2d27  ta.    print('-'
+00002ab0: 202a 2034 3229 0a20 2020 2064 6174 615f   * 42).    data_
+00002ac0: 6669 6c65 203d 2027 7468 7563 6e65 7773  file = 'thucnews
+00002ad0: 5f74 7261 696e 5f31 772e 7478 7427 0a20  _train_1w.txt'. 
+00002ae0: 2020 206d 203d 2046 6173 7454 6578 7443     m = FastTextC
+00002af0: 6c61 7373 6966 6965 7228 6f75 7470 7574  lassifier(output
+00002b00: 5f64 6972 3d27 6d6f 6465 6c73 2f66 6173  _dir='models/fas
+00002b10: 7474 6578 7427 290a 2020 2020 6d2e 7472  ttext').    m.tr
+00002b20: 6169 6e28 6461 7461 5f66 696c 652c 206e  ain(data_file, n
+00002b30: 616d 6573 3d28 276c 6162 656c 7327 2c20  ames=('labels', 
+00002b40: 2774 6578 7427 292c 206e 756d 5f65 706f  'text'), num_epo
+00002b50: 6368 733d 3329 0a20 2020 2023 206c 6f61  chs=3).    # loa
+00002b60: 6420 6265 7374 2074 7261 696e 6564 206d  d best trained m
+00002b70: 6f64 656c 2066 726f 6d20 6d6f 6465 6c5f  odel from model_
+00002b80: 6469 720a 2020 2020 6d2e 6c6f 6164 5f6d  dir.    m.load_m
+00002b90: 6f64 656c 2829 0a20 2020 2070 7265 6469  odel().    predi
+00002ba0: 6374 5f6c 6162 656c 2c20 7072 6564 6963  ct_label, predic
+00002bb0: 745f 7072 6f62 6120 3d20 6d2e 7072 6564  t_proba = m.pred
+00002bc0: 6963 7428 0a20 2020 2020 2020 205b 27e9  ict(.        ['.
+00002bd0: a1ba e4b9 89e5 8c97 e4ba ace8 8b8f e6b4  ................
+00002be0: bb38 38e5 b9b3 e7b1 b3e8 b5b7 e7b2 bee8  .88.............
+00002bf0: a385 e688 bfe5 9ca8 e594 ae27 2c0a 2020  ...........',.  
+00002c00: 2020 2020 2020 2027 e7be 8e45 422d 35e9         '...EB-5.
+00002c10: a1b9 e79b aee2 809c 3135 e697 a5e5 bfab  ........15......
+00002c20: e980 9fe7 a7bb e6b0 91e2 809d e5b0 86e6  ................
+00002c30: 8ea8 e8bf 9f27 5d0a 2020 2020 290a 2020  .....'].    ).  
+00002c40: 2020 7072 696e 7428 6627 7072 6564 6963    print(f'predic
+00002c50: 745f 6c61 6265 6c3a 207b 7072 6564 6963  t_label: {predic
+00002c60: 745f 6c61 6265 6c7d 2c20 7072 6564 6963  t_label}, predic
+00002c70: 745f 7072 6f62 613a 207b 7072 6564 6963  t_proba: {predic
+00002c80: 745f 7072 6f62 617d 2729 0a20 2020 2078  t_proba}').    x
+00002c90: 2c20 792c 2064 6620 3d20 6c6f 6164 5f64  , y, df = load_d
+00002ca0: 6174 6128 6461 7461 5f66 696c 6529 0a20  ata(data_file). 
+00002cb0: 2020 2074 6573 745f 6461 7461 203d 2064     test_data = d
+00002cc0: 665b 3a31 3030 5d0a 2020 2020 6163 635f  f[:100].    acc_
+00002cd0: 7363 6f72 6520 3d20 6d2e 6576 616c 7561  score = m.evalua
+00002ce0: 7465 5f6d 6f64 656c 2874 6573 745f 6461  te_model(test_da
+00002cf0: 7461 290a 2020 2020 7072 696e 7428 6627  ta).    print(f'
+00002d00: 6163 635f 7363 6f72 653a 207b 6163 635f  acc_score: {acc_
+00002d10: 7363 6f72 657d 2729 0a60 6060 0a0a 2323  score}').```..##
+00002d20: 2320 4245 5254 20e7 b1bb e6a8 a1e5 9e8b  # BERT .........
+00002d30: 0a0a 2323 2323 20e5 a49a e588 86e7 b1bb  ..#### .........
+00002d40: e6a8 a1e5 9e8b 0ae8 aead e7bb 83e5 928c  ................
+00002d50: e9a2 84e6 b58b 6042 4552 5460 e5a4 9ae5  ......`BERT`....
+00002d60: 8886 e7b1 bbe6 a8a1 e59e 8bef bc8c e7a4  ................
+00002d70: bae4 be8b 5b65 7861 6d70 6c65 732f 6265  ....[examples/be
+00002d80: 7274 5f63 6c61 7373 6966 6963 6174 696f  rt_classificatio
+00002d90: 6e5f 7a68 5f64 656d 6f2e 7079 5d28 6874  n_zh_demo.py](ht
+00002da0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00002db0: 2f73 6869 6269 6e67 3632 342f 7079 7465  /shibing624/pyte
+00002dc0: 7874 636c 6173 7369 6669 6572 2f62 6c6f  xtclassifier/blo
+00002dd0: 622f 6d61 7374 6572 2f65 7861 6d70 6c65  b/master/example
+00002de0: 732f 6265 7274 5f63 6c61 7373 6966 6963  s/bert_classific
+00002df0: 6174 696f 6e5f 7a68 5f64 656d 6f2e 7079  ation_zh_demo.py
+00002e00: 290a 0a60 6060 7079 7468 6f6e 0a69 6d70  )..```python.imp
+00002e10: 6f72 7420 7379 730a 0a73 7973 2e70 6174  ort sys..sys.pat
+00002e20: 682e 6170 7065 6e64 2827 2e2e 2729 0a66  h.append('..').f
+00002e30: 726f 6d20 7079 7465 7874 636c 6173 7369  rom pytextclassi
+00002e40: 6669 6572 2069 6d70 6f72 7420 4265 7274  fier import Bert
+00002e50: 436c 6173 7369 6669 6572 0a0a 6966 205f  Classifier..if _
+00002e60: 5f6e 616d 655f 5f20 3d3d 2027 5f5f 6d61  _name__ == '__ma
+00002e70: 696e 5f5f 273a 0a20 2020 206d 203d 2042  in__':.    m = B
+00002e80: 6572 7443 6c61 7373 6966 6965 7228 6f75  ertClassifier(ou
+00002e90: 7470 7574 5f64 6972 3d27 6d6f 6465 6c73  tput_dir='models
+00002ea0: 2f62 6572 742d 6368 696e 6573 652d 746f  /bert-chinese-to
+00002eb0: 7927 2c20 6e75 6d5f 636c 6173 7365 733d  y', num_classes=
+00002ec0: 322c 0a20 2020 2020 2020 2020 2020 2020  2,.             
+00002ed0: 2020 2020 2020 2020 2020 6d6f 6465 6c5f            model_
+00002ee0: 7479 7065 3d27 6265 7274 272c 206d 6f64  type='bert', mod
+00002ef0: 656c 5f6e 616d 653d 2762 6572 742d 6261  el_name='bert-ba
+00002f00: 7365 2d63 6869 6e65 7365 272c 206e 756d  se-chinese', num
+00002f10: 5f65 706f 6368 733d 3229 0a20 2020 2023  _epochs=2).    #
+00002f20: 206d 6f64 656c 5f74 7970 653a 2073 7570   model_type: sup
+00002f30: 706f 7274 2027 6265 7274 272c 2027 616c  port 'bert', 'al
+00002f40: 6265 7274 272c 2027 726f 6265 7274 6127  bert', 'roberta'
+00002f50: 2c20 2778 6c6e 6574 270a 2020 2020 2320  , 'xlnet'.    # 
+00002f60: 6d6f 6465 6c5f 6e61 6d65 3a20 7375 7070  model_name: supp
+00002f70: 6f72 7420 2762 6572 742d 6261 7365 2d63  ort 'bert-base-c
+00002f80: 6869 6e65 7365 272c 2027 6265 7274 2d62  hinese', 'bert-b
+00002f90: 6173 652d 6361 7365 6427 2c20 2762 6572  ase-cased', 'ber
+00002fa0: 742d 6261 7365 2d6d 756c 7469 6c69 6e67  t-base-multiling
+00002fb0: 7561 6c2d 6361 7365 6427 202e 2e2e 0a20  ual-cased' .... 
+00002fc0: 2020 2064 6174 6120 3d20 5b0a 2020 2020     data = [.    
+00002fd0: 2020 2020 2827 6564 7563 6174 696f 6e27      ('education'
+00002fe0: 2c20 27e5 908d e5b8 88e6 8c87 e5af bce6  , '.............
+00002ff0: 8998 e7a6 8fe8 afad e6b3 95e6 8a80 e5b7  ................
+00003000: a7ef bc9a e590 8de8 af8d e79a 84e5 a48d  ................
+00003010: e695 b0e5 bda2 e5bc 8f27 292c 0a20 2020  .........'),.   
+00003020: 2020 2020 2028 2765 6475 6361 7469 6f6e       ('education
+00003030: 272c 2027 e4b8 ade5 9bbd e9ab 98e8 8083  ', '............
+00003040: e688 90e7 bba9 e6b5 b7e5 a496 e8ae a4e5  ................
+00003050: 8faf 20e6 98af e280 9ce7 8bbc e69d a5e4  .. .............
+00003060: ba86 e280 9de5 9097 efbc 9f27 292c 0a20  ...........'),. 
+00003070: 2020 2020 2020 2028 2765 6475 6361 7469         ('educati
+00003080: 6f6e 272c 2027 e585 ace5 8aa1 e591 98e8  on', '..........
+00003090: 8083 e899 91e8 b68a e69d a5e8 b68a e590  ................
+000030a0: 83e9 a699 efbc 8ce8 bf99 e698 afe6 808e  ................
+000030b0: e4b9 88e5 9b9e e4ba 8bef bc9f 2729 2c0a  ............'),.
+000030c0: 2020 2020 2020 2020 2827 7370 6f72 7473          ('sports
+000030d0: 272c 2027 e59b bee6 9687 efbc 9ae6 b395  ', '............
+000030e0: e7bd 91e5 ad9f e88f b2e5 b094 e696 afe8  ................
+000030f0: 8ba6 e688 98e8 bf9b 3136 e5bc ba20 e5ad  ........16... ..
+00003100: 9fe8 8fb2 e5b0 94e6 96af e680 92e5 90bc  ................
+00003110: 2729 2c0a 2020 2020 2020 2020 2827 7370  '),.        ('sp
+00003120: 6f72 7473 272c 2027 e59b 9be5 b79d e4b8  orts', '........
+00003130: b9e6 a3b1 e4b8 bee8 a18c e585 a8e5 9bbd  ................
+00003140: e995 bfe8 b79d e799 bbe5 b1b1 e68c 91e6  ................
+00003150: 8898 e8b5 9b20 e8bf 91e4 b887 e4ba bae5  ..... ..........
+00003160: 8f82 e4b8 8e27 292c 0a20 2020 2020 2020  .....'),.       
+00003170: 2028 2773 706f 7274 7327 2c20 27e7 b1b3   ('sports', '...
+00003180: e585 b0e5 aea2 e59c ba38 e688 98e4 b88d  .........8......
+00003190: e8b4 a5e5 9bbd e7b1 b331 30e5 b9b4 e8bf  .........10.....
+000031a0: 9ee8 839c 2729 2c0a 2020 2020 5d0a 2020  ....'),.    ].  
+000031b0: 2020 6d2e 7472 6169 6e28 6461 7461 290a    m.train(data).
+000031c0: 2020 2020 7072 696e 7428 6d29 0a20 2020      print(m).   
+000031d0: 2023 206c 6f61 6420 7472 6169 6e65 6420   # load trained 
+000031e0: 6265 7374 206d 6f64 656c 2066 726f 6d20  best model from 
+000031f0: 6d6f 6465 6c5f 6469 720a 2020 2020 6d2e  model_dir.    m.
+00003200: 6c6f 6164 5f6d 6f64 656c 2829 0a20 2020  load_model().   
+00003210: 2070 7265 6469 6374 5f6c 6162 656c 2c20   predict_label, 
+00003220: 7072 6564 6963 745f 7072 6f62 6120 3d20  predict_proba = 
+00003230: 6d2e 7072 6564 6963 7428 5b27 e7a6 8fe5  m.predict(['....
+00003240: bbba e698 a5e5 ada3 e585 ace5 8aa1 e591  ................
+00003250: 98e8 8083 e8af 95e6 8aa5 e590 8d31 38e6  .............18.
+00003260: 97a5 e688 aae6 ada2 2032 e69c 8836 e697  ........ 2...6..
+00003270: a5e8 8083 e8af 9527 2c0a 2020 2020 2020  .......',.      
+00003280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000032a0: 2020 2020 2020 2020 27e6 848f e794 b2e9          '.......
+000032b0: a696 e8bd aee8 a1a5 e8b5 9be4 baa4 e688  ................
+000032c0: 98e8 aeb0 e5bd 953a e7b1 b3e5 85b0 e5ae  .......:........
+000032d0: a2e5 9cba 38e6 8898 e4b8 8de8 b4a5 e59b  ....8...........
+000032e0: bde7 b1b3 3130 e5b9 b4e8 bf9e e883 9c27  ....10.........'
+000032f0: 5d29 0a20 2020 2070 7269 6e74 2866 2770  ]).    print(f'p
+00003300: 7265 6469 6374 5f6c 6162 656c 3a20 7b70  redict_label: {p
+00003310: 7265 6469 6374 5f6c 6162 656c 7d2c 2070  redict_label}, p
+00003320: 7265 6469 6374 5f70 726f 6261 3a20 7b70  redict_proba: {p
+00003330: 7265 6469 6374 5f70 726f 6261 7d27 290a  redict_proba}').
+00003340: 0a20 2020 2074 6573 745f 6461 7461 203d  .    test_data =
+00003350: 205b 0a20 2020 2020 2020 2028 2765 6475   [.        ('edu
+00003360: 6361 7469 6f6e 272c 2027 e7a6 8fe5 bbba  cation', '......
+00003370: e698 a5e5 ada3 e585 ace5 8aa1 e591 98e8  ................
+00003380: 8083 e8af 95e6 8aa5 e590 8d31 38e6 97a5  ...........18...
+00003390: e688 aae6 ada2 2032 e69c 8836 e697 a5e8  ...... 2...6....
+000033a0: 8083 e8af 9527 292c 0a20 2020 2020 2020  .....'),.       
+000033b0: 2028 2773 706f 7274 7327 2c20 27e6 848f   ('sports', '...
+000033c0: e794 b2e9 a696 e8bd aee8 a1a5 e8b5 9be4  ................
+000033d0: baa4 e688 98e8 aeb0 e5bd 953a e7b1 b3e5  ...........:....
+000033e0: 85b0 e5ae a2e5 9cba 38e6 8898 e4b8 8de8  ........8.......
+000033f0: b4a5 e59b bde7 b1b3 3130 e5b9 b4e8 bf9e  ........10......
+00003400: e883 9c27 292c 0a20 2020 205d 0a20 2020  ...'),.    ].   
 00003410: 2061 6363 5f73 636f 7265 203d 206d 2e65   acc_score = m.e
 00003420: 7661 6c75 6174 655f 6d6f 6465 6c28 7465  valuate_model(te
-00003430: 7374 5f64 6174 6129 0a20 2020 2020 2020  st_data).       
-00003440: 2020 2020 2070 7269 6e74 2866 2761 6363       print(f'acc
-00003450: 5f73 636f 7265 3a20 7b61 6363 5f73 636f  _score: {acc_sco
-00003460: 7265 7d27 290a 2020 2020 2020 2020 6060  re}').        ``
-00003470: 600a 2020 2020 2020 2020 0a20 2020 2020  `.        .     
-00003480: 2020 2023 2323 2042 4552 5420 e7b1 bbe6     ### BERT ....
-00003490: a8a1 e59e 8b0a 2020 2020 2020 2020 0a20  ......        . 
-000034a0: 2020 2020 2020 2023 2323 2320 e5a4 9ae5         #### ....
-000034b0: 8886 e7b1 bbe6 a8a1 e59e 8b0a 2020 2020  ............    
-000034c0: 2020 2020 e8ae ade7 bb83 e592 8ce9 a284      ............
-000034d0: e6b5 8b60 4245 5254 60e5 a49a e588 86e7  ...`BERT`.......
-000034e0: b1bb e6a8 a1e5 9e8b efbc 8ce7 a4ba e4be  ................
-000034f0: 8b5b 6578 616d 706c 6573 2f62 6572 745f  .[examples/bert_
-00003500: 636c 6173 7369 6669 6361 7469 6f6e 5f7a  classification_z
-00003510: 685f 6465 6d6f 2e70 795d 2868 7474 7073  h_demo.py](https
-00003520: 3a2f 2f67 6974 6875 622e 636f 6d2f 7368  ://github.com/sh
-00003530: 6962 696e 6736 3234 2f70 7974 6578 7463  ibing624/pytextc
-00003540: 6c61 7373 6966 6965 722f 626c 6f62 2f6d  lassifier/blob/m
-00003550: 6173 7465 722f 6578 616d 706c 6573 2f62  aster/examples/b
-00003560: 6572 745f 636c 6173 7369 6669 6361 7469  ert_classificati
-00003570: 6f6e 5f7a 685f 6465 6d6f 2e70 7929 0a20  on_zh_demo.py). 
-00003580: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00003590: 6060 6070 7974 686f 6e0a 2020 2020 2020  ```python.      
-000035a0: 2020 696d 706f 7274 2073 7973 0a20 2020    import sys.   
-000035b0: 2020 2020 200a 2020 2020 2020 2020 7379       .        sy
-000035c0: 732e 7061 7468 2e61 7070 656e 6428 272e  s.path.append('.
-000035d0: 2e27 290a 2020 2020 2020 2020 6672 6f6d  .').        from
-000035e0: 2070 7974 6578 7463 6c61 7373 6966 6965   pytextclassifie
-000035f0: 7220 696d 706f 7274 2042 6572 7443 6c61  r import BertCla
-00003600: 7373 6966 6965 720a 2020 2020 2020 2020  ssifier.        
-00003610: 0a20 2020 2020 2020 2069 6620 5f5f 6e61  .        if __na
-00003620: 6d65 5f5f 203d 3d20 275f 5f6d 6169 6e5f  me__ == '__main_
-00003630: 5f27 3a0a 2020 2020 2020 2020 2020 2020  _':.            
-00003640: 6d20 3d20 4265 7274 436c 6173 7369 6669  m = BertClassifi
-00003650: 6572 286f 7574 7075 745f 6469 723d 276d  er(output_dir='m
-00003660: 6f64 656c 732f 6265 7274 2d63 6869 6e65  odels/bert-chine
-00003670: 7365 2d74 6f79 272c 206e 756d 5f63 6c61  se-toy', num_cla
-00003680: 7373 6573 3d32 2c0a 2020 2020 2020 2020  sses=2,.        
-00003690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000036a0: 2020 2020 2020 206d 6f64 656c 5f74 7970         model_typ
-000036b0: 653d 2762 6572 7427 2c20 6d6f 6465 6c5f  e='bert', model_
-000036c0: 6e61 6d65 3d27 6265 7274 2d62 6173 652d  name='bert-base-
-000036d0: 6368 696e 6573 6527 2c20 6e75 6d5f 6570  chinese', num_ep
-000036e0: 6f63 6873 3d32 290a 2020 2020 2020 2020  ochs=2).        
-000036f0: 2020 2020 2320 6d6f 6465 6c5f 7479 7065      # model_type
-00003700: 3a20 7375 7070 6f72 7420 2762 6572 7427  : support 'bert'
-00003710: 2c20 2761 6c62 6572 7427 2c20 2772 6f62  , 'albert', 'rob
-00003720: 6572 7461 272c 2027 786c 6e65 7427 0a20  erta', 'xlnet'. 
-00003730: 2020 2020 2020 2020 2020 2023 206d 6f64             # mod
-00003740: 656c 5f6e 616d 653a 2073 7570 706f 7274  el_name: support
-00003750: 2027 6265 7274 2d62 6173 652d 6368 696e   'bert-base-chin
-00003760: 6573 6527 2c20 2762 6572 742d 6261 7365  ese', 'bert-base
-00003770: 2d63 6173 6564 272c 2027 6265 7274 2d62  -cased', 'bert-b
-00003780: 6173 652d 6d75 6c74 696c 696e 6775 616c  ase-multilingual
-00003790: 2d63 6173 6564 2720 2e2e 2e0a 2020 2020  -cased' ....    
-000037a0: 2020 2020 2020 2020 6461 7461 203d 205b          data = [
-000037b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000037c0: 2028 2765 6475 6361 7469 6f6e 272c 2027   ('education', '
-000037d0: e590 8de5 b888 e68c 87e5 afbc e689 98e7  ................
-000037e0: a68f e8af ade6 b395 e68a 80e5 b7a7 efbc  ................
-000037f0: 9ae5 908d e8af 8de7 9a84 e5a4 8de6 95b0  ................
-00003800: e5bd a2e5 bc8f 2729 2c0a 2020 2020 2020  ......'),.      
-00003810: 2020 2020 2020 2020 2020 2827 6564 7563            ('educ
-00003820: 6174 696f 6e27 2c20 27e4 b8ad e59b bde9  ation', '.......
-00003830: ab98 e880 83e6 8890 e7bb a9e6 b5b7 e5a4  ................
-00003840: 96e8 aea4 e58f af20 e698 afe2 809c e78b  ....... ........
-00003850: bce6 9da5 e4ba 86e2 809d e590 97ef bc9f  ................
-00003860: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
-00003870: 2020 2020 2827 6564 7563 6174 696f 6e27      ('education'
-00003880: 2c20 27e5 85ac e58a a1e5 9198 e880 83e8  , '.............
-00003890: 9991 e8b6 8ae6 9da5 e8b6 8ae5 9083 e9a6  ................
-000038a0: 99ef bc8c e8bf 99e6 98af e680 8ee4 b988  ................
-000038b0: e59b 9ee4 ba8b efbc 9f27 292c 0a20 2020  .........'),.   
-000038c0: 2020 2020 2020 2020 2020 2020 2028 2773               ('s
-000038d0: 706f 7274 7327 2c20 27e5 9bbe e696 87ef  ports', '.......
-000038e0: bc9a e6b3 95e7 bd91 e5ad 9fe8 8fb2 e5b0  ................
-000038f0: 94e6 96af e88b a6e6 8898 e8bf 9b31 36e5  .............16.
-00003900: bcba 20e5 ad9f e88f b2e5 b094 e696 afe6  .. .............
-00003910: 8092 e590 bc27 292c 0a20 2020 2020 2020  .....'),.       
-00003920: 2020 2020 2020 2020 2028 2773 706f 7274           ('sport
-00003930: 7327 2c20 27e5 9b9b e5b7 9de4 b8b9 e6a3  s', '...........
-00003940: b1e4 b8be e8a1 8ce5 85a8 e59b bde9 95bf  ................
-00003950: e8b7 9de7 99bb e5b1 b1e6 8c91 e688 98e8  ................
-00003960: b59b 20e8 bf91 e4b8 87e4 baba e58f 82e4  .. .............
-00003970: b88e 2729 2c0a 2020 2020 2020 2020 2020  ..'),.          
-00003980: 2020 2020 2020 2827 7370 6f72 7473 272c        ('sports',
-00003990: 2027 e7b1 b3e5 85b0 e5ae a2e5 9cba 38e6   '............8.
-000039a0: 8898 e4b8 8de8 b4a5 e59b bde7 b1b3 3130  ..............10
-000039b0: e5b9 b4e8 bf9e e883 9c27 292c 0a20 2020  .........'),.   
-000039c0: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
-000039d0: 2020 2020 2020 206d 2e74 7261 696e 2864         m.train(d
-000039e0: 6174 6129 0a20 2020 2020 2020 2020 2020  ata).           
-000039f0: 2070 7269 6e74 286d 290a 2020 2020 2020   print(m).      
-00003a00: 2020 2020 2020 2320 6c6f 6164 2074 7261        # load tra
-00003a10: 696e 6564 2062 6573 7420 6d6f 6465 6c20  ined best model 
-00003a20: 6672 6f6d 206d 6f64 656c 5f64 6972 0a20  from model_dir. 
-00003a30: 2020 2020 2020 2020 2020 206d 2e6c 6f61             m.loa
-00003a40: 645f 6d6f 6465 6c28 290a 2020 2020 2020  d_model().      
-00003a50: 2020 2020 2020 7072 6564 6963 745f 6c61        predict_la
-00003a60: 6265 6c2c 2070 7265 6469 6374 5f70 726f  bel, predict_pro
-00003a70: 6261 203d 206d 2e70 7265 6469 6374 285b  ba = m.predict([
-00003a80: 27e7 a68f e5bb bae6 98a5 e5ad a3e5 85ac  '...............
-00003a90: e58a a1e5 9198 e880 83e8 af95 e68a a5e5  ................
-00003aa0: 908d 3138 e697 a5e6 88aa e6ad a220 32e6  ..18......... 2.
-00003ab0: 9c88 36e6 97a5 e880 83e8 af95 272c 0a20  ..6.........',. 
-00003ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003af0: 2020 2020 2027 e684 8fe7 94b2 e9a6 96e8       '..........
-00003b00: bdae e8a1 a5e8 b59b e4ba a4e6 8898 e8ae  ................
-00003b10: b0e5 bd95 3ae7 b1b3 e585 b0e5 aea2 e59c  ....:...........
-00003b20: ba38 e688 98e4 b88d e8b4 a5e5 9bbd e7b1  .8..............
-00003b30: b331 30e5 b9b4 e8bf 9ee8 839c 275d 290a  .10.........']).
-00003b40: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00003b50: 7428 6627 7072 6564 6963 745f 6c61 6265  t(f'predict_labe
-00003b60: 6c3a 207b 7072 6564 6963 745f 6c61 6265  l: {predict_labe
-00003b70: 6c7d 2c20 7072 6564 6963 745f 7072 6f62  l}, predict_prob
-00003b80: 613a 207b 7072 6564 6963 745f 7072 6f62  a: {predict_prob
-00003b90: 617d 2729 0a20 2020 2020 2020 200a 2020  a}').        .  
-00003ba0: 2020 2020 2020 2020 2020 7465 7374 5f64            test_d
-00003bb0: 6174 6120 3d20 5b0a 2020 2020 2020 2020  ata = [.        
-00003bc0: 2020 2020 2020 2020 2827 6564 7563 6174          ('educat
-00003bd0: 696f 6e27 2c20 27e7 a68f e5bb bae6 98a5  ion', '.........
-00003be0: e5ad a3e5 85ac e58a a1e5 9198 e880 83e8  ................
-00003bf0: af95 e68a a5e5 908d 3138 e697 a5e6 88aa  ........18......
-00003c00: e6ad a220 32e6 9c88 36e6 97a5 e880 83e8  ... 2...6.......
-00003c10: af95 2729 2c0a 2020 2020 2020 2020 2020  ..'),.          
-00003c20: 2020 2020 2020 2827 7370 6f72 7473 272c        ('sports',
-00003c30: 2027 e684 8fe7 94b2 e9a6 96e8 bdae e8a1   '..............
-00003c40: a5e8 b59b e4ba a4e6 8898 e8ae b0e5 bd95  ................
-00003c50: 3ae7 b1b3 e585 b0e5 aea2 e59c ba38 e688  :............8..
-00003c60: 98e4 b88d e8b4 a5e5 9bbd e7b1 b331 30e5  .............10.
-00003c70: b9b4 e8bf 9ee8 839c 2729 2c0a 2020 2020  ........'),.    
-00003c80: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
-00003c90: 2020 2020 2020 6163 635f 7363 6f72 6520        acc_score 
-00003ca0: 3d20 6d2e 6576 616c 7561 7465 5f6d 6f64  = m.evaluate_mod
-00003cb0: 656c 2874 6573 745f 6461 7461 290a 2020  el(test_data).  
-00003cc0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00003cd0: 6627 6163 635f 7363 6f72 653a 207b 6163  f'acc_score: {ac
-00003ce0: 635f 7363 6f72 657d 2729 0a20 2020 2020  c_score}').     
-00003cf0: 2020 200a 2020 2020 2020 2020 2020 2020     .            
-00003d00: 2320 7472 6169 6e20 6d6f 6465 6c20 7769  # train model wi
-00003d10: 7468 2031 7720 6461 7461 2066 696c 6520  th 1w data file 
-00003d20: 616e 6420 3130 2063 6c61 7373 6573 0a20  and 10 classes. 
-00003d30: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00003d40: 2827 2d27 202a 2034 3229 0a20 2020 2020  ('-' * 42).     
-00003d50: 2020 2020 2020 206d 203d 2042 6572 7443         m = BertC
-00003d60: 6c61 7373 6966 6965 7228 6f75 7470 7574  lassifier(output
-00003d70: 5f64 6972 3d27 6d6f 6465 6c73 2f62 6572  _dir='models/ber
-00003d80: 742d 6368 696e 6573 6527 2c20 6e75 6d5f  t-chinese', num_
-00003d90: 636c 6173 7365 733d 3130 2c0a 2020 2020  classes=10,.    
-00003da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003db0: 2020 2020 2020 2020 2020 206d 6f64 656c             model
-00003dc0: 5f74 7970 653d 2762 6572 7427 2c20 6d6f  _type='bert', mo
-00003dd0: 6465 6c5f 6e61 6d65 3d27 6265 7274 2d62  del_name='bert-b
-00003de0: 6173 652d 6368 696e 6573 6527 2c20 6e75  ase-chinese', nu
-00003df0: 6d5f 6570 6f63 6873 3d32 2c0a 2020 2020  m_epochs=2,.    
-00003e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003e10: 2020 2020 2020 2020 2020 2061 7267 733d             args=
-00003e20: 7b22 6e6f 5f63 6163 6865 223a 2054 7275  {"no_cache": Tru
-00003e30: 652c 2022 6c61 7a79 5f6c 6f61 6469 6e67  e, "lazy_loading
-00003e40: 223a 2054 7275 652c 2022 6c61 7a79 5f74  ": True, "lazy_t
-00003e50: 6578 745f 636f 6c75 6d6e 223a 2031 2c20  ext_column": 1, 
-00003e60: 226c 617a 795f 6c61 6265 6c73 5f63 6f6c  "lazy_labels_col
-00003e70: 756d 6e22 3a20 302c 207d 290a 2020 2020  umn": 0, }).    
-00003e80: 2020 2020 2020 2020 6461 7461 5f66 696c          data_fil
-00003e90: 6520 3d20 2774 6875 636e 6577 735f 7472  e = 'thucnews_tr
-00003ea0: 6169 6e5f 3177 2e74 7874 270a 2020 2020  ain_1w.txt'.    
-00003eb0: 2020 2020 2020 2020 2320 e5a6 82e6 9e9c          # ......
-00003ec0: e8ae ade7 bb83 e695 b0e6 8dae e8b6 85e8  ................
-00003ed0: bf87 e799 bee4 b887 e69d a1ef bc8c e5bb  ................
-00003ee0: bae8 aeae e4bd bfe7 94a8 6c61 7a79 5f6c  ..........lazy_l
-00003ef0: 6f61 6469 6e67 e6a8 a1e5 bc8f efbc 8ce5  oading..........
-00003f00: 878f e5b0 91e5 8685 e5ad 98e5 8da0 e794  ................
-00003f10: a80a 2020 2020 2020 2020 2020 2020 6d2e  ..            m.
-00003f20: 7472 6169 6e28 6461 7461 5f66 696c 652c  train(data_file,
-00003f30: 2074 6573 745f 7369 7a65 3d30 2c20 6e61   test_size=0, na
-00003f40: 6d65 733d 2827 6c61 6265 6c73 272c 2027  mes=('labels', '
-00003f50: 7465 7874 2729 290a 2020 2020 2020 2020  text')).        
-00003f60: 2020 2020 6d2e 6c6f 6164 5f6d 6f64 656c      m.load_model
-00003f70: 2829 0a20 2020 2020 2020 2020 2020 2070  ().            p
-00003f80: 7265 6469 6374 5f6c 6162 656c 2c20 7072  redict_label, pr
-00003f90: 6564 6963 745f 7072 6f62 6120 3d20 6d2e  edict_proba = m.
-00003fa0: 7072 6564 6963 7428 0a20 2020 2020 2020  predict(.       
-00003fb0: 2020 2020 2020 2020 205b 27e9 a1ba e4b9           ['.....
-00003fc0: 89e5 8c97 e4ba ace8 8b8f e6b4 bb38 38e5  .............88.
-00003fd0: b9b3 e7b1 b3e8 b5b7 e7b2 bee8 a385 e688  ................
-00003fe0: bfe5 9ca8 e594 ae27 2c0a 2020 2020 2020  .......',.      
-00003ff0: 2020 2020 2020 2020 2020 2027 e7be 8e45             '...E
-00004000: 422d 35e9 a1b9 e79b aee2 809c 3135 e697  B-5.........15..
-00004010: a5e5 bfab e980 9fe7 a7bb e6b0 91e2 809d  ................
-00004020: e5b0 86e6 8ea8 e8bf 9f27 2c0a 2020 2020  .........',.    
-00004030: 2020 2020 2020 2020 2020 2020 2027 e681               '..
-00004040: 92e7 949f 4148 e6ba a2e6 8c87 e694 b6e5  ....AH..........
-00004050: b9b3 2041 e882 a1e5 afb9 48e8 82a1 e68a  .. A......H.....
-00004060: 98e4 bbb7 312e 3935 2527 5d29 0a20 2020  ....1.95%']).   
-00004070: 2020 2020 2020 2020 2070 7269 6e74 2866           print(f
-00004080: 2770 7265 6469 6374 5f6c 6162 656c 3a20  'predict_label: 
-00004090: 7b70 7265 6469 6374 5f6c 6162 656c 7d2c  {predict_label},
-000040a0: 2070 7265 6469 6374 5f70 726f 6261 3a20   predict_proba: 
-000040b0: 7b70 7265 6469 6374 5f70 726f 6261 7d27  {predict_proba}'
-000040c0: 290a 2020 2020 2020 2020 6060 600a 2020  ).        ```.  
-000040d0: 2020 2020 2020 5053 efbc 9ae5 a682 e69e        PS........
-000040e0: 9ce8 aead e7bb 83e6 95b0 e68d aee8 b685  ................
-000040f0: e8bf 87e7 99be e4b8 87e6 9da1 efbc 8ce5  ................
-00004100: bbba e8ae aee4 bdbf e794 a86c 617a 795f  ...........lazy_
-00004110: 6c6f 6164 696e 67e6 a8a1 e5bc 8fef bc8c  loading.........
-00004120: e587 8fe5 b091 e586 85e5 ad98 e58d a0e7  ................
-00004130: 94a8 0a20 2020 2020 2020 200a 2020 2020  ...        .    
-00004140: 2020 2020 2323 2323 20e5 a49a e6a0 87e7      #### .......
-00004150: adbe e588 86e7 b1bb e6a8 a1e5 9e8b 0a20  ............... 
-00004160: 2020 2020 2020 20e5 8886 e7b1 bbe5 8faf         .........
-00004170: e4bb a5e5 8886 e4b8 bae5 a49a e588 86e7  ................
-00004180: b1bb e592 8ce5 a49a e6a0 87e7 adbe e588  ................
-00004190: 86e7 b1bb e380 82e5 a49a e588 86e7 b1bb  ................
-000041a0: e79a 84e6 a087 e7ad bee6 98af e68e 92e4  ................
-000041b0: bb96 e79a 84ef bc8c e880 8ce5 a49a e6a0  ................
-000041c0: 87e7 adbe e588 86e7 b1bb e79a 84e6 8980  ................
-000041d0: e69c 89e6 a087 e7ad bee6 98af e4b8 8de6  ................
-000041e0: 8e92 e4bb 96e7 9a84 e380 820a 2020 2020  ............    
-000041f0: 2020 2020 0a20 2020 2020 2020 20e5 a49a      .        ...
-00004200: e6a0 87e7 adbe e588 86e7 b1bb e6af 94e8  ................
-00004210: be83 e79b b4e8 a782 e79a 84e7 9086 e8a7  ................
-00004220: a3e6 98af efbc 8ce4 b880 e4b8 aae6 a0b7  ................
-00004230: e69c ace5 8faf e4bb a5e5 908c e697 b6e6  ................
-00004240: 8ba5 e69c 89e5 87a0 e4b8 aae7 b1bb e588  ................
-00004250: abe6 a087 e7ad beef bc8c 0a20 2020 2020  ...........     
-00004260: 2020 20e6 af94 e5a6 82e4 b880 e9a6 96e6     .............
-00004270: ad8c e79a 84e6 a087 e7ad bee5 8faf e4bb  ................
-00004280: a5e6 98af e6b5 81e8 a18c e380 81e8 bdbb  ................
-00004290: e5bf abef bc8c e4b8 80e9 83a8 e794 b5e5  ................
-000042a0: bdb1 e79a 84e6 a087 e7ad bee5 8faf e4bb  ................
-000042b0: a5e6 98af e58a a8e4 bd9c e380 81e5 969c  ................
-000042c0: e589 a7e3 8081 e690 9ee7 ac91 e7ad 89ef  ................
-000042d0: bc8c e8bf 99e9 83bd e698 afe5 a49a e6a0  ................
-000042e0: 87e7 adbe e588 86e7 b1bb e79a 84e6 8385  ................
-000042f0: e586 b5e3 8082 0a20 2020 2020 2020 200a  .......        .
-00004300: 2020 2020 2020 2020 e8ae ade7 bb83 e592          ........
-00004310: 8ce9 a284 e6b5 8b60 4245 5254 60e5 a49a  .......`BERT`...
-00004320: e6a0 87e7 adbe e588 86e7 b1bb e6a8 a1e5  ................
-00004330: 9e8b efbc 8ce7 a4ba e4be 8b5b 6578 616d  ...........[exam
-00004340: 706c 6573 2f62 6572 745f 6d75 6c74 696c  ples/bert_multil
-00004350: 6162 656c 5f63 6c61 7373 6966 6963 6174  abel_classificat
-00004360: 696f 6e5f 7a68 5f64 656d 6f2e 7079 2e70  ion_zh_demo.py.p
-00004370: 795d 2868 7474 7073 3a2f 2f67 6974 6875  y](https://githu
-00004380: 622e 636f 6d2f 7368 6962 696e 6736 3234  b.com/shibing624
-00004390: 2f70 7974 6578 7463 6c61 7373 6966 6965  /pytextclassifie
-000043a0: 722f 626c 6f62 2f6d 6173 7465 722f 6578  r/blob/master/ex
-000043b0: 616d 706c 6573 2f62 6572 745f 6d75 6c74  amples/bert_mult
-000043c0: 696c 6162 656c 5f63 6c61 7373 6966 6963  ilabel_classific
-000043d0: 6174 696f 6e5f 7a68 5f64 656d 6f2e 7079  ation_zh_demo.py
-000043e0: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-000043f0: 2020 2060 6060 7079 7468 6f6e 0a20 2020     ```python.   
-00004400: 2020 2020 2069 6d70 6f72 7420 7379 730a       import sys.
-00004410: 2020 2020 2020 2020 696d 706f 7274 2070          import p
-00004420: 616e 6461 7320 6173 2070 640a 2020 2020  andas as pd.    
-00004430: 2020 2020 0a20 2020 2020 2020 2073 7973      .        sys
-00004440: 2e70 6174 682e 6170 7065 6e64 2827 2e2e  .path.append('..
-00004450: 2729 0a20 2020 2020 2020 2066 726f 6d20  ').        from 
-00004460: 7079 7465 7874 636c 6173 7369 6669 6572  pytextclassifier
-00004470: 2069 6d70 6f72 7420 4265 7274 436c 6173   import BertClas
-00004480: 7369 6669 6572 0a20 2020 2020 2020 200a  sifier.        .
-00004490: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-000044a0: 2064 6566 206c 6f61 645f 6a64 5f64 6174   def load_jd_dat
-000044b0: 6128 6669 6c65 5f70 6174 6829 3a0a 2020  a(file_path):.  
-000044c0: 2020 2020 2020 2020 2020 2222 220a 2020            """.  
-000044d0: 2020 2020 2020 2020 2020 4c6f 6164 206a            Load j
-000044e0: 6420 6461 7461 2066 726f 6d20 6669 6c65  d data from file
-000044f0: 2e0a 2020 2020 2020 2020 2020 2020 4070  ..            @p
-00004500: 6172 616d 2066 696c 655f 7061 7468 3a20  aram file_path: 
-00004510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004520: 2066 6f72 6d61 743a 2063 6f6e 7465 6e74   format: content
-00004530: 2ce5 85b6 e4bb 962c e4ba 92e8 8194 e4ba  ,......,........
-00004540: 92e9 809a 2ce4 baa7 e593 81e5 8a9f e880  ....,...........
-00004550: 972c e6bb 91e8 bdae e68f 90e6 898b 2ce5  .,............,.
-00004560: a3b0 e99f b32c 4150 50e6 938d e68e a7e6  .....,APP.......
-00004570: 80a7 2ce5 91bc e590 b8e7 81af 2ce5 a496  ..,.........,...
-00004580: e8a7 822c e5ba 95e5 baa7 2ce5 88b6 e783  ...,......,.....
-00004590: ade8 8c83 e59b b42c e981 a5e6 8ea7 e599  .......,........
-000045a0: a8e7 94b5 e6b1 a02c e591 b3e9 8193 2ce5  .......,......,.
-000045b0: 88b6 e783 ade6 9588 e69e 9c2c e8a1 a3e7  ...........,....
-000045c0: 89a9 e783 98e5 b9b2 2ce4 bd93 e7a7 afe5  ........,.......
-000045d0: a4a7 e5b0 8f0a 2020 2020 2020 2020 2020  ......          
-000045e0: 2020 4072 6574 7572 6e3a 200a 2020 2020    @return: .    
-000045f0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00004600: 2020 2020 2020 2020 6461 7461 203d 205b          data = [
-00004610: 5d0a 2020 2020 2020 2020 2020 2020 7769  ].            wi
-00004620: 7468 206f 7065 6e28 6669 6c65 5f70 6174  th open(file_pat
-00004630: 682c 2027 7227 2c20 656e 636f 6469 6e67  h, 'r', encoding
-00004640: 3d27 7574 662d 3827 2920 6173 2066 3a0a  ='utf-8') as f:.
-00004650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004660: 666f 7220 6c69 6e65 2069 6e20 663a 0a20  for line in f:. 
-00004670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004680: 2020 206c 696e 6520 3d20 6c69 6e65 2e73     line = line.s
-00004690: 7472 6970 2829 0a20 2020 2020 2020 2020  trip().         
-000046a0: 2020 2020 2020 2020 2020 2069 6620 6c69             if li
-000046b0: 6e65 2e73 7461 7274 7377 6974 6828 2723  ne.startswith('#
-000046c0: 2729 3a0a 2020 2020 2020 2020 2020 2020  '):.            
-000046d0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-000046e0: 696e 7565 0a20 2020 2020 2020 2020 2020  inue.           
-000046f0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-00004700: 6c69 6e65 3a0a 2020 2020 2020 2020 2020  line:.          
-00004710: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00004720: 6e74 696e 7565 0a20 2020 2020 2020 2020  ntinue.         
-00004730: 2020 2020 2020 2020 2020 2074 6572 6d73             terms
-00004740: 203d 206c 696e 652e 7370 6c69 7428 272c   = line.split(',
-00004750: 2729 0a20 2020 2020 2020 2020 2020 2020  ').             
-00004760: 2020 2020 2020 2069 6620 6c65 6e28 7465         if len(te
-00004770: 726d 7329 2021 3d20 3136 3a0a 2020 2020  rms) != 16:.    
-00004780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004790: 2020 2020 636f 6e74 696e 7565 0a20 2020      continue.   
-000047a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000047b0: 2076 616c 203d 205b 696e 7428 6929 2066   val = [int(i) f
-000047c0: 6f72 2069 2069 6e20 7465 726d 735b 313a  or i in terms[1:
-000047d0: 5d5d 0a20 2020 2020 2020 2020 2020 2020  ]].             
-000047e0: 2020 2020 2020 2064 6174 612e 6170 7065         data.appe
-000047f0: 6e64 285b 7465 726d 735b 305d 2c20 7661  nd([terms[0], va
-00004800: 6c5d 290a 2020 2020 2020 2020 2020 2020  l]).            
-00004810: 7265 7475 726e 2064 6174 610a 2020 2020  return data.    
-00004820: 2020 2020 0a20 2020 2020 2020 200a 2020      .        .  
-00004830: 2020 2020 2020 6966 205f 5f6e 616d 655f        if __name_
-00004840: 5f20 3d3d 2027 5f5f 6d61 696e 5f5f 273a  _ == '__main__':
-00004850: 0a20 2020 2020 2020 2020 2020 2023 206d  .            # m
-00004860: 6f64 656c 5f74 7970 653a 2073 7570 706f  odel_type: suppo
-00004870: 7274 2027 6265 7274 272c 2027 616c 6265  rt 'bert', 'albe
-00004880: 7274 272c 2027 726f 6265 7274 6127 2c20  rt', 'roberta', 
-00004890: 2778 6c6e 6574 270a 2020 2020 2020 2020  'xlnet'.        
-000048a0: 2020 2020 2320 6d6f 6465 6c5f 6e61 6d65      # model_name
-000048b0: 3a20 7375 7070 6f72 7420 2762 6572 742d  : support 'bert-
-000048c0: 6261 7365 2d63 6869 6e65 7365 272c 2027  base-chinese', '
-000048d0: 6265 7274 2d62 6173 652d 6361 7365 6427  bert-base-cased'
-000048e0: 2c20 2762 6572 742d 6261 7365 2d6d 756c  , 'bert-base-mul
-000048f0: 7469 6c69 6e67 7561 6c2d 6361 7365 6427  tilingual-cased'
-00004900: 202e 2e2e 0a20 2020 2020 2020 2020 2020   ....           
-00004910: 206d 203d 2042 6572 7443 6c61 7373 6966   m = BertClassif
-00004920: 6965 7228 6f75 7470 7574 5f64 6972 3d27  ier(output_dir='
-00004930: 6d6f 6465 6c73 2f6d 756c 7469 6c61 6265  models/multilabe
-00004940: 6c2d 6265 7274 2d7a 682d 6d6f 6465 6c27  l-bert-zh-model'
-00004950: 2c20 6e75 6d5f 636c 6173 7365 733d 3135  , num_classes=15
-00004960: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00004970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004980: 206d 6f64 656c 5f74 7970 653d 2762 6572   model_type='ber
-00004990: 7427 2c20 6d6f 6465 6c5f 6e61 6d65 3d27  t', model_name='
-000049a0: 6265 7274 2d62 6173 652d 6368 696e 6573  bert-base-chines
-000049b0: 6527 2c20 6e75 6d5f 6570 6f63 6873 3d32  e', num_epochs=2
-000049c0: 2c20 6d75 6c74 695f 6c61 6265 6c3d 5472  , multi_label=Tr
-000049d0: 7565 290a 2020 2020 2020 2020 2020 2020  ue).            
-000049e0: 2320 5472 6169 6e20 616e 6420 4576 616c  # Train and Eval
-000049f0: 7561 7469 6f6e 2064 6174 6120 6e65 6564  uation data need
-00004a00: 7320 746f 2062 6520 696e 2061 2050 616e  s to be in a Pan
-00004a10: 6461 7320 4461 7461 6672 616d 6520 636f  das Dataframe co
-00004a20: 6e74 6169 6e69 6e67 2061 7420 6c65 6173  ntaining at leas
-00004a30: 7420 7477 6f20 636f 6c75 6d6e 732c 2061  t two columns, a
-00004a40: 2027 7465 7874 2720 616e 6420 6120 276c   'text' and a 'l
-00004a50: 6162 656c 7327 2063 6f6c 756d 6e2e 2054  abels' column. T
-00004a60: 6865 2060 6c61 6265 6c73 6020 636f 6c75  he `labels` colu
-00004a70: 6d6e 2073 686f 756c 6420 636f 6e74 6169  mn should contai
-00004a80: 6e20 6d75 6c74 692d 686f 7420 656e 636f  n multi-hot enco
-00004a90: 6465 6420 6c69 7374 732e 0a20 2020 2020  ded lists..     
-00004aa0: 2020 2020 2020 2074 7261 696e 5f64 6174         train_dat
-00004ab0: 6120 3d20 5b0a 2020 2020 2020 2020 2020  a = [.          
-00004ac0: 2020 2020 2020 5b22 e4b8 80e4 b8aa e5b0        ["........
-00004ad0: 8fe6 97b6 e688 bfe9 97b4 e4bb 8de7 84b6  ................
-00004ae0: e6b2 a1e6 9a96 e592 8c22 2c20 5b30 2c20  .........", [0, 
-00004af0: 302c 2030 2c20 302c 2030 2c20 302c 2030  0, 0, 0, 0, 0, 0
-00004b00: 2c20 302c 2030 2c20 302c 2030 2c20 302c  , 0, 0, 0, 0, 0,
-00004b10: 2031 2c20 302c 2030 5d5d 2c0a 2020 2020   1, 0, 0]],.    
-00004b20: 2020 2020 2020 2020 2020 2020 5b22 e880              ["..
-00004b30: 97e7 94b5 e683 85e5 86b5 efbc 9ae8 bf99  ................
-00004b40: e4b8 aae6 b2a1 e69c 89e6 b3a8 e684 8f22  ..............."
-00004b50: 2c20 5b30 2c20 302c 2031 2c20 302c 2030  , [0, 0, 1, 0, 0
-00004b60: 2c20 302c 2030 2c20 302c 2030 2c20 302c  , 0, 0, 0, 0, 0,
-00004b70: 2030 2c20 302c 2030 2c20 302c 2030 5d5d   0, 0, 0, 0, 0]]
-00004b80: 2c0a 2020 2020 2020 2020 2020 2020 5d0a  ,.            ].
-00004b90: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00004ba0: 203d 206c 6f61 645f 6a64 5f64 6174 6128   = load_jd_data(
-00004bb0: 276d 756c 7469 6c61 6265 6c5f 6a64 5f63  'multilabel_jd_c
-00004bc0: 6f6d 6d65 6e74 732e 6373 7627 290a 2020  omments.csv').  
-00004bd0: 2020 2020 2020 2020 2020 7472 6169 6e5f            train_
-00004be0: 6461 7461 2e65 7874 656e 6428 6461 7461  data.extend(data
-00004bf0: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
-00004c00: 696e 7428 7472 6169 6e5f 6461 7461 5b3a  int(train_data[:
-00004c10: 355d 290a 2020 2020 2020 2020 2020 2020  5]).            
-00004c20: 7472 6169 6e5f 6466 203d 2070 642e 4461  train_df = pd.Da
-00004c30: 7461 4672 616d 6528 7472 6169 6e5f 6461  taFrame(train_da
-00004c40: 7461 2c20 636f 6c75 6d6e 733d 5b22 7465  ta, columns=["te
-00004c50: 7874 222c 2022 6c61 6265 6c73 225d 290a  xt", "labels"]).
-00004c60: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00004c70: 2020 2020 2070 7269 6e74 2874 7261 696e       print(train
-00004c80: 5f64 662e 6865 6164 2829 290a 2020 2020  _df.head()).    
-00004c90: 2020 2020 2020 2020 6d2e 7472 6169 6e28          m.train(
-00004ca0: 7472 6169 6e5f 6466 290a 2020 2020 2020  train_df).      
-00004cb0: 2020 2020 2020 7072 696e 7428 6d29 0a20        print(m). 
-00004cc0: 2020 2020 2020 2020 2020 2023 2045 7661             # Eva
-00004cd0: 6c75 6174 6520 7468 6520 6d6f 6465 6c0a  luate the model.
-00004ce0: 2020 2020 2020 2020 2020 2020 6163 635f              acc_
-00004cf0: 7363 6f72 6520 3d20 6d2e 6576 616c 7561  score = m.evalua
-00004d00: 7465 5f6d 6f64 656c 2874 7261 696e 5f64  te_model(train_d
-00004d10: 665b 3a32 305d 290a 2020 2020 2020 2020  f[:20]).        
-00004d20: 2020 2020 7072 696e 7428 6627 6163 635f      print(f'acc_
-00004d30: 7363 6f72 653a 207b 6163 635f 7363 6f72  score: {acc_scor
-00004d40: 657d 2729 0a20 2020 2020 2020 200a 2020  e}').        .  
-00004d50: 2020 2020 2020 2020 2020 2320 6c6f 6164            # load
-00004d60: 2074 7261 696e 6564 2062 6573 7420 6d6f   trained best mo
-00004d70: 6465 6c20 6672 6f6d 206d 6f64 656c 5f64  del from model_d
-00004d80: 6972 0a20 2020 2020 2020 2020 2020 206d  ir.            m
-00004d90: 2e6c 6f61 645f 6d6f 6465 6c28 290a 2020  .load_model().  
-00004da0: 2020 2020 2020 2020 2020 7072 6564 6963            predic
-00004db0: 745f 6c61 6265 6c2c 2070 7265 6469 6374  t_label, predict
-00004dc0: 5f70 726f 6261 203d 206d 2e70 7265 6469  _proba = m.predi
-00004dd0: 6374 285b 27e4 b880 e4b8 aae5 b08f e697  ct(['...........
-00004de0: b6e6 88bf e997 b4e4 bb8d e784 b6e6 b2a1  ................
-00004df0: e69a 96e5 928c 272c 2027 e880 97e7 94b5  ......', '......
-00004e00: e683 85e5 86b5 efbc 9ae8 bf99 e4b8 aae6  ................
-00004e10: b2a1 e69c 89e6 b3a8 e684 8f27 5d29 0a20  ...........']). 
-00004e20: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00004e30: 2866 2770 7265 6469 6374 5f6c 6162 656c  (f'predict_label
-00004e40: 3a20 7b70 7265 6469 6374 5f6c 6162 656c  : {predict_label
-00004e50: 7d2c 2070 7265 6469 6374 5f70 726f 6261  }, predict_proba
-00004e60: 3a20 7b70 7265 6469 6374 5f70 726f 6261  : {predict_proba
-00004e70: 7d27 290a 2020 2020 2020 2020 6060 600a  }').        ```.
-00004e80: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00004e90: 2023 2320 4576 616c 7561 7469 6f6e 0a20   ## Evaluation. 
-00004ea0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00004eb0: 2323 2320 4461 7461 7365 740a 2020 2020  ### Dataset.    
-00004ec0: 2020 2020 0a20 2020 2020 2020 2031 2e20      .        1. 
-00004ed0: 5448 5543 4e65 7773 e4b8 ade6 9687 e696  THUCNews........
-00004ee0: 87e6 9cac e695 b0e6 8dae e99b 86ef bc88  ................
-00004ef0: 312e 3536 4742 efbc 89ef bc9a e5ae 98e6  1.56GB..........
-00004f00: 96b9 5be4 b88b e8bd bde5 9cb0 e59d 805d  ..[............]
-00004f10: 2868 7474 703a 2f2f 7468 7563 7463 2e74  (http://thuctc.t
-00004f20: 6875 6e6c 702e 6f72 672f 29ef bc8c e68a  hunlp.org/).....
-00004f30: bde6 a0b7 e4ba 8631 30e4 b887 e69d a154  .......10......T
-00004f40: 4855 434e 6577 73e4 b8ad e696 87e6 9687  HUCNews.........
-00004f50: e69c ac31 30e5 8886 e7b1 bbe6 95b0 e68d  ...10...........
-00004f60: aee9 9b86 efbc 8836 4d42 efbc 89ef bc8c  .......6MB......
-00004f70: e59c b0e5 9d80 efbc 9a5b 6578 616d 706c  .........[exampl
-00004f80: 6573 2f74 6875 636e 6577 735f 7472 6169  es/thucnews_trai
-00004f90: 6e5f 3130 772e 7478 745d 2868 7474 7073  n_10w.txt](https
-00004fa0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7368  ://github.com/sh
-00004fb0: 6962 696e 6736 3234 2f70 7974 6578 7463  ibing624/pytextc
-00004fc0: 6c61 7373 6966 6965 722f 626c 6f62 2f6d  lassifier/blob/m
-00004fd0: 6173 7465 722f 6578 616d 706c 6573 2f74  aster/examples/t
-00004fe0: 6875 636e 6577 735f 7472 6169 6e5f 3130  hucnews_train_10
-00004ff0: 772e 7478 7429 e380 820a 2020 2020 2020  w.txt)....      
-00005000: 2020 322e 2054 4e45 5753 e4bb 8ae6 97a5    2. TNEWS......
-00005010: e5a4 b4e6 9da1 e4b8 ade6 9687 e696 b0e9  ................
-00005020: 97bb efbc 88e7 9fad e696 87e6 9cac efbc  ................
-00005030: 89e5 8886 e7b1 bb20 5368 6f72 7420 5465  ....... Short Te
-00005040: 7874 2043 6c61 7373 6966 6963 6169 746f  xt Classificaito
-00005050: 6e20 666f 7220 4e65 7773 efbc 8ce8 afa5  n for News......
-00005060: e695 b0e6 8dae e99b 8628 352e 314d 4229  .........(5.1MB)
-00005070: e69d a5e8 87aa e4bb 8ae6 97a5 e5a4 b4e6  ................
-00005080: 9da1 e79a 84e6 96b0 e997 bbe7 8988 e59d  ................
-00005090: 97ef bc8c e585 b1e6 8f90 e58f 96e4 ba86  ................
-000050a0: 3135 e4b8 aae7 b1bb e588 abe7 9a84 e696  15..............
-000050b0: b0e9 97bb efbc 8ce5 8c85 e68b ace6 9785  ................
-000050c0: e6b8 b8ef bc8c e695 99e8 82b2 efbc 8ce9  ................
-000050d0: 8791 e89e 8def bc8c e586 9be4 ba8b e7ad  ................
-000050e0: 89ef bc8c e59c b0e5 9d80 efbc 9a5b 746e  .............[tn
-000050f0: 6577 735f 7075 626c 6963 2e7a 6970 5d28  ews_public.zip](
-00005100: 6874 7470 733a 2f2f 7374 6f72 6167 652e  https://storage.
-00005110: 676f 6f67 6c65 6170 6973 2e63 6f6d 2f63  googleapis.com/c
-00005120: 6c75 6562 656e 6368 6d61 726b 2f74 6173  luebenchmark/tas
-00005130: 6b73 2f74 6e65 7773 5f70 7562 6c69 632e  ks/tnews_public.
-00005140: 7a69 7029 0a20 2020 2020 2020 200a 2020  zip).        .  
-00005150: 2020 2020 2020 2323 2320 4576 616c 7561        ### Evalua
-00005160: 7469 6f6e 2052 6573 756c 740a 2020 2020  tion Result.    
-00005170: 2020 2020 e59c a854 4855 434e 6577 73e4      ...THUCNews.
-00005180: b8ad e696 87e6 9687 e69c ac31 30e5 8886  ...........10...
-00005190: e7b1 bbe6 95b0 e68d aee9 9b86 efbc 8836  ...............6
-000051a0: 4d42 efbc 89e4 b88a e8af 84e4 bcb0 efbc  MB..............
-000051b0: 8ce6 a8a1 e59e 8be5 9ca8 e6b5 8be8 af95  ................
-000051c0: e99b 8628 7465 7374 29e8 af84 e6b5 8be6  ...(test).......
-000051d0: 9588 e69e 9ce5 a682 e4b8 8bef bc9a 0a20  ............... 
-000051e0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-000051f0: e6a8 a1e5 9e8b 7c61 6363 7ce8 afb4 e698  ......|acc|.....
-00005200: 8e0a 2020 2020 2020 2020 2d2d 7c2d 2d7c  ..        --|--|
-00005210: 2d2d 0a20 2020 2020 2020 204c 527c 302e  --.        LR|0.
-00005220: 3838 3033 7ce9 80bb e8be 91e5 9b9e e5bd  8803|...........
-00005230: 924c 6f67 6973 7469 6373 2052 6567 7265  .Logistics Regre
-00005240: 7373 696f 6e0a 2020 2020 2020 2020 5465  ssion.        Te
-00005250: 7874 434e 4e7c 302e 3838 3039 7c4b 696d  xtCNN|0.8809|Kim
-00005260: 2032 3031 3420 e7bb 8fe5 85b8 e79a 8443   2014 .........C
-00005270: 4e4e e696 87e6 9cac e588 86e7 b1bb 0a20  NN............. 
-00005280: 2020 2020 2020 2054 6578 7452 4e4e 5f41         TextRNN_A
-00005290: 7474 7c30 2e39 3032 327c 4269 4c53 544d  tt|0.9022|BiLSTM
-000052a0: 2b41 7474 656e 7469 6f6e 0a20 2020 2020  +Attention.     
-000052b0: 2020 2046 6173 7454 6578 747c 302e 3931     FastText|0.91
-000052c0: 3737 7c62 6f77 2b62 6967 7261 6d2b 7472  77|bow+bigram+tr
-000052d0: 6967 7261 6def bc8c 20e6 9588 e69e 9ce5  igram... .......
-000052e0: 87ba e5a5 87e7 9a84 e5a5 bd0a 2020 2020  ............    
-000052f0: 2020 2020 4450 434e 4e7c 302e 3931 3235      DPCNN|0.9125
-00005300: 7ce6 b7b1 e5b1 82e9 8791 e5ad 97e5 a194  |...............
-00005310: 434e 4e0a 2020 2020 2020 2020 5472 616e  CNN.        Tran
-00005320: 7366 6f72 6d65 727c 302e 3839 3931 7ce6  sformer|0.8991|.
-00005330: 9588 e69e 9ce8 be83 e5b7 ae0a 2020 2020  ............    
-00005340: 2020 2020 4245 5254 2d62 6173 657c 2a2a      BERT-base|**
-00005350: 302e 3934 3833 2a2a 7c62 6572 7420 2b20  0.9483**|bert + 
-00005360: 6663 0a20 2020 2020 2020 2045 524e 4945  fc.        ERNIE
-00005370: 7c30 2e39 3436 317c e6af 9462 6572 74e7  |0.9461|...bert.
-00005380: 95a5 e5b7 ae0a 2020 2020 2020 2020 0a20  ......        . 
-00005390: 2020 2020 2020 20e5 9ca8 e4b8 ade6 9687         .........
-000053a0: e696 b0e9 97bb e79f ade6 9687 e69c ace5  ................
-000053b0: 8886 e7b1 bbe6 95b0 e68d aee9 9b86 544e  ..............TN
-000053c0: 4557 53e4 b88a e8af 84e4 bcb0 efbc 8ce6  EWS.............
-000053d0: a8a1 e59e 8be5 9ca8 e5bc 80e5 8f91 e99b  ................
-000053e0: 8628 6465 7629 e8af 84e6 b58b e695 88e6  .(dev)..........
-000053f0: 9e9c e5a6 82e4 b88b efbc 9a0a 2020 2020  ............    
-00005400: 2020 2020 0a20 2020 2020 2020 20e6 a8a1      .        ...
-00005410: e59e 8b7c 6163 637c e8af b4e6 988e 0a20  ...|acc|....... 
-00005420: 2020 2020 2020 202d 2d7c 2d2d 7c2d 2d0a         --|--|--.
-00005430: 2020 2020 2020 2020 4245 5254 2d62 6173          BERT-bas
-00005440: 657c 2a2a 302e 3536 3630 2a2a 7ce6 9cac  e|**0.5660**|...
-00005450: e9a1 b9e7 9bae e5ae 9ee7 8eb0 0a20 2020  .............   
-00005460: 2020 2020 2042 4552 542d 6261 7365 7c30       BERT-base|0
-00005470: 2e35 3630 397c 434c 5545 2042 656e 6368  .5609|CLUE Bench
-00005480: 6d61 726b 204c 6561 6465 7262 6f61 7264  mark Leaderboard
-00005490: e7bb 93e6 9e9c 205b 434c 5545 6265 6e63  ...... [CLUEbenc
-000054a0: 686d 6172 6b5d 2868 7474 7073 3a2f 2f67  hmark](https://g
-000054b0: 6974 6875 622e 636f 6d2f 434c 5545 6265  ithub.com/CLUEbe
-000054c0: 6e63 686d 6172 6b2f 434c 5545 290a 2020  nchmark/CLUE).  
-000054d0: 2020 2020 2020 0a20 2020 2020 2020 202d        .        -
-000054e0: 20e4 bba5 e4b8 8ae7 bb93 e69e 9ce5 9d87   ...............
-000054f0: e4b8 bae5 8886 e7b1 bbe7 9a84 e587 86e7  ................
-00005500: a1ae e78e 87ef bc88 6163 6375 7261 6379  ........accuracy
-00005510: efbc 89e7 bb93 e69e 9c0a 2020 2020 2020  ..........      
-00005520: 2020 2d20 5448 5543 4e65 7773 e695 b0e6    - THUCNews....
-00005530: 8dae e99b 86e8 af84 e6b5 8be7 bb93 e69e  ................
-00005540: 9ce5 8faf e4bb a5e5 9fba e4ba 8e60 6578  .............`ex
-00005550: 616d 706c 6573 2f74 6875 636e 6577 735f  amples/thucnews_
-00005560: 7472 6169 6e5f 3130 772e 7478 7460 e695  train_10w.txt`..
-00005570: b0e6 8dae e794 a860 6578 616d 706c 6573  .......`examples
-00005580: 60e4 b88b e79a 84e5 9084 e6a8 a1e5 9e8b  `...............
-00005590: 6465 6d6f e5a4 8de7 8eb0 0a20 2020 2020  demo.......     
-000055a0: 2020 202d 2054 4e45 5753 e695 b0e6 8dae     - TNEWS......
-000055b0: e99b 86e8 af84 e6b5 8be7 bb93 e69e 9ce5  ................
-000055c0: 8faf e4bb a5e4 b88b e8bd bd54 4e45 5753  ...........TNEWS
-000055d0: e695 b0e6 8dae e99b 86ef bc8c e8bf 90e8  ................
-000055e0: a18c 6065 7861 6d70 6c65 732f 6265 7274  ..`examples/bert
-000055f0: 5f63 6c61 7373 6966 6963 6174 696f 6e5f  _classification_
-00005600: 746e 6577 735f 6465 6d6f 2e70 7960 e5a4  tnews_demo.py`..
-00005610: 8de7 8eb0 0a20 2020 2020 2020 200a 2020  .....        .  
-00005620: 2020 2020 2020 2323 2320 e591 bde4 bba4        ### ......
-00005630: e8a1 8ce8 b083 e794 a80a 2020 2020 2020  ..........      
-00005640: 2020 0a20 2020 2020 2020 20e6 8f90 e4be    .        .....
-00005650: 9be5 8886 e7b1 bbe6 a8a1 e59e 8be5 91bd  ................
-00005660: e4bb a4e8 a18c e8b0 83e7 94a8 e884 9ae6  ................
-00005670: 9cac efbc 8ce6 9687 e4bb b6e6 a091 efbc  ................
-00005680: 9a0a 2020 2020 2020 2020 6060 6062 6173  ..        ```bas
-00005690: 680a 2020 2020 2020 2020 7079 7465 7874  h.        pytext
-000056a0: 636c 6173 7369 6669 6572 0a20 2020 2020  classifier.     
-000056b0: 2020 20e2 949c e294 80e2 9480 2062 6572     ......... ber
-000056c0: 745f 636c 6173 7369 6669 6572 2e70 790a  t_classifier.py.
-000056d0: 2020 2020 2020 2020 e294 9ce2 9480 e294          ........
-000056e0: 8020 6661 7374 7465 7874 5f63 6c61 7373  . fasttext_class
-000056f0: 6966 6965 722e 7079 0a20 2020 2020 2020  ifier.py.       
-00005700: 20e2 949c e294 80e2 9480 2063 6c61 7373   ......... class
-00005710: 6963 5f63 6c61 7373 6966 6965 722e 7079  ic_classifier.py
-00005720: 0a20 2020 2020 2020 20e2 949c e294 80e2  .        .......
-00005730: 9480 2074 6578 7463 6e6e 5f63 6c61 7373  .. textcnn_class
-00005740: 6966 6965 722e 7079 0a20 2020 2020 2020  ifier.py.       
-00005750: 20e2 9494 e294 80e2 9480 2074 6578 7472   ......... textr
-00005760: 6e6e 5f63 6c61 7373 6966 6965 722e 7079  nn_classifier.py
-00005770: 0a20 2020 2020 2020 2060 6060 0a20 2020  .        ```.   
-00005780: 2020 2020 200a 2020 2020 2020 2020 e6af       .        ..
-00005790: 8fe4 b8aa e696 87e4 bbb6 e5af b9e5 ba94  ................
-000057a0: e4b8 80e4 b8aa e6a8 a1e5 9e8b e696 b9e6  ................
-000057b0: b395 efbc 8ce5 9084 e6a8 a1e5 9e8b e5ae  ................
-000057c0: 8ce5 85a8 e78b ace7 ab8b efbc 8ce5 8faf  ................
-000057d0: e4bb a5e7 9bb4 e68e a5e8 bf90 e8a1 8cef  ................
-000057e0: bc8c e4b9 9fe6 96b9 e4be bfe4 bfae e694  ................
-000057f0: b9ef bc8c e694 afe6 8c81 e980 9ae8 bf87  ................
-00005800: 6061 7267 7061 7273 6560 20e4 bfae e694  `argparse` .....
-00005810: b960 2d2d 6461 7461 5f70 6174 6860 e7ad  .`--data_path`..
-00005820: 89e5 8f82 e695 b0e3 8082 0a20 2020 2020  ...........     
-00005830: 2020 200a 2020 2020 2020 2020 e79b b4e6     .        ....
-00005840: 8ea5 e59c a8e7 bb88 e7ab afe8 b083 e794  ................
-00005850: a866 6173 7474 6578 74e6 a8a1 e59e 8be8  .fasttext.......
-00005860: aead e7bb 83ef bc9a 0a20 2020 2020 2020  .........       
-00005870: 2060 6060 6261 7368 0a20 2020 2020 2020   ```bash.       
-00005880: 2070 7974 686f 6e20 2d6d 2070 7974 6578   python -m pytex
-00005890: 7463 6c61 7373 6966 6965 722e 6661 7374  tclassifier.fast
-000058a0: 7465 7874 5f63 6c61 7373 6966 6965 7220  text_classifier 
-000058b0: 2d68 0a20 2020 2020 2020 2060 6060 0a20  -h.        ```. 
-000058c0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-000058d0: 2323 2054 6578 7420 436c 7573 7465 720a  ## Text Cluster.
-000058e0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-000058f0: 200a 2020 2020 2020 2020 5465 7874 2063   .        Text c
-00005900: 6c75 7374 6572 696e 672c 2066 6f72 2065  lustering, for e
-00005910: 7861 6d70 6c65 205b 6578 616d 706c 6573  xample [examples
-00005920: 2f63 6c75 7374 6572 5f64 656d 6f2e 7079  /cluster_demo.py
-00005930: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00005940: 2e63 6f6d 2f73 6869 6269 6e67 3632 342f  .com/shibing624/
-00005950: 7079 7465 7874 636c 6173 7369 6669 6572  pytextclassifier
-00005960: 2f62 6c6f 622f 6d61 7374 6572 2f65 7861  /blob/master/exa
-00005970: 6d70 6c65 732f 636c 7573 7465 725f 6465  mples/cluster_de
-00005980: 6d6f 2e70 7929 0a20 2020 2020 2020 200a  mo.py).        .
-00005990: 2020 2020 2020 2020 6060 6070 7974 686f          ```pytho
-000059a0: 6e0a 2020 2020 2020 2020 696d 706f 7274  n.        import
-000059b0: 2073 7973 0a20 2020 2020 2020 200a 2020   sys.        .  
-000059c0: 2020 2020 2020 7379 732e 7061 7468 2e61        sys.path.a
-000059d0: 7070 656e 6428 272e 2e27 290a 2020 2020  ppend('..').    
-000059e0: 2020 2020 6672 6f6d 2070 7974 6578 7463      from pytextc
-000059f0: 6c61 7373 6966 6965 722e 7465 7874 636c  lassifier.textcl
-00005a00: 7573 7465 7220 696d 706f 7274 2054 6578  uster import Tex
-00005a10: 7443 6c75 7374 6572 0a20 2020 2020 2020  tCluster.       
-00005a20: 200a 2020 2020 2020 2020 6966 205f 5f6e   .        if __n
-00005a30: 616d 655f 5f20 3d3d 2027 5f5f 6d61 696e  ame__ == '__main
-00005a40: 5f5f 273a 0a20 2020 2020 2020 2020 2020  __':.           
-00005a50: 206d 203d 2054 6578 7443 6c75 7374 6572   m = TextCluster
-00005a60: 286f 7574 7075 745f 6469 723d 276d 6f64  (output_dir='mod
-00005a70: 656c 732f 636c 7573 7465 722d 746f 7927  els/cluster-toy'
-00005a80: 2c20 6e5f 636c 7573 7465 7273 3d32 290a  , n_clusters=2).
-00005a90: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00005aa0: 7428 6d29 0a20 2020 2020 2020 2020 2020  t(m).           
-00005ab0: 2064 6174 6120 3d20 5b0a 2020 2020 2020   data = [.      
-00005ac0: 2020 2020 2020 2020 2020 2753 7475 6465            'Stude
-00005ad0: 6e74 2064 6562 7420 746f 2063 6f73 7420  nt debt to cost 
-00005ae0: 4272 6974 6169 6e20 6269 6c6c 696f 6e73  Britain billions
-00005af0: 2077 6974 6869 6e20 6465 6361 6465 7327   within decades'
-00005b00: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00005b10: 2020 2743 6869 6e65 7365 2065 6475 6361    'Chinese educa
-00005b20: 7469 6f6e 2066 6f72 2054 5620 6578 7065  tion for TV expe
-00005b30: 7269 6d65 6e74 272c 0a20 2020 2020 2020  riment',.       
-00005b40: 2020 2020 2020 2020 2027 4162 626f 7474           'Abbott
-00005b50: 2067 6f76 6572 6e6d 656e 7420 7370 656e   government spen
-00005b60: 6473 2024 3820 6d69 6c6c 696f 6e20 6f6e  ds $8 million on
-00005b70: 2068 6967 6865 7220 6564 7563 6174 696f   higher educatio
-00005b80: 6e27 2c0a 2020 2020 2020 2020 2020 2020  n',.            
-00005b90: 2020 2020 274d 6964 646c 6520 4561 7374      'Middle East
-00005ba0: 2061 6e64 2041 7369 6120 626f 6f73 7420   and Asia boost 
-00005bb0: 696e 7665 7374 6d65 6e74 2069 6e20 746f  investment in to
-00005bc0: 7020 6c65 7665 6c20 7370 6f72 7473 272c  p level sports',
-00005bd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005be0: 2027 5375 6d6d 6974 2053 6572 6965 7320   'Summit Series 
-00005bf0: 6c6f 6f6b 206c 6175 6e63 6865 7320 4842  look launches HB
-00005c00: 4f20 4361 6e61 6461 2073 706f 7274 7320  O Canada sports 
-00005c10: 646f 6320 7365 7269 6573 3a20 4d75 6468  doc series: Mudh
-00005c20: 6172 270a 2020 2020 2020 2020 2020 2020  ar'.            
-00005c30: 5d0a 2020 2020 2020 2020 2020 2020 6d2e  ].            m.
-00005c40: 7472 6169 6e28 6461 7461 290a 2020 2020  train(data).    
-00005c50: 2020 2020 2020 2020 6d2e 6c6f 6164 5f6d          m.load_m
-00005c60: 6f64 656c 2829 0a20 2020 2020 2020 2020  odel().         
-00005c70: 2020 2072 203d 206d 2e70 7265 6469 6374     r = m.predict
-00005c80: 285b 2741 6262 6f74 7420 676f 7665 726e  (['Abbott govern
-00005c90: 6d65 6e74 2073 7065 6e64 7320 2438 206d  ment spends $8 m
-00005ca0: 696c 6c69 6f6e 206f 6e20 6869 6768 6572  illion on higher
-00005cb0: 2065 6475 6361 7469 6f6e 206d 6564 6961   education media
-00005cc0: 2062 6c69 747a 272c 0a20 2020 2020 2020   blitz',.       
-00005cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ce0: 2020 2020 274d 6964 646c 6520 4561 7374      'Middle East
-00005cf0: 2061 6e64 2041 7369 6120 626f 6f73 7420   and Asia boost 
-00005d00: 696e 7665 7374 6d65 6e74 2069 6e20 746f  investment in to
-00005d10: 7020 6c65 7665 6c20 7370 6f72 7473 275d  p level sports']
-00005d20: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
-00005d30: 696e 7428 7229 0a20 2020 2020 2020 200a  int(r).        .
-00005d40: 2020 2020 2020 2020 2020 2020 2323 2323              ####
-00005d50: 2323 2323 2323 2320 6c6f 6164 2063 6869  ####### load chi
-00005d60: 6e65 7365 2074 7261 696e 2064 6174 6120  nese train data 
-00005d70: 6672 6f6d 2031 7720 6461 7461 2066 696c  from 1w data fil
-00005d80: 650a 2020 2020 2020 2020 2020 2020 6672  e.            fr
-00005d90: 6f6d 2073 6b6c 6561 726e 2e66 6561 7475  om sklearn.featu
-00005da0: 7265 5f65 7874 7261 6374 696f 6e2e 7465  re_extraction.te
-00005db0: 7874 2069 6d70 6f72 7420 5466 6964 6656  xt import TfidfV
-00005dc0: 6563 746f 7269 7a65 720a 2020 2020 2020  ectorizer.      
-00005dd0: 2020 0a20 2020 2020 2020 2020 2020 2074    .            t
-00005de0: 636c 7573 7465 7220 3d20 5465 7874 436c  cluster = TextCl
-00005df0: 7573 7465 7228 6f75 7470 7574 5f64 6972  uster(output_dir
-00005e00: 3d27 6d6f 6465 6c73 2f63 6c75 7374 6572  ='models/cluster
-00005e10: 272c 2066 6561 7475 7265 3d54 6669 6466  ', feature=Tfidf
-00005e20: 5665 6374 6f72 697a 6572 286e 6772 616d  Vectorizer(ngram
-00005e30: 5f72 616e 6765 3d28 312c 2032 2929 2c20  _range=(1, 2)), 
-00005e40: 6e5f 636c 7573 7465 7273 3d31 3029 0a20  n_clusters=10). 
-00005e50: 2020 2020 2020 2020 2020 2064 6174 6120             data 
-00005e60: 3d20 7463 6c75 7374 6572 2e6c 6f61 645f  = tcluster.load_
-00005e70: 6669 6c65 5f64 6174 6128 2774 6875 636e  file_data('thucn
-00005e80: 6577 735f 7472 6169 6e5f 3177 2e74 7874  ews_train_1w.txt
-00005e90: 272c 2073 6570 3d27 5c74 272c 2075 7365  ', sep='\t', use
-00005ea0: 5f63 6f6c 3d31 290a 2020 2020 2020 2020  _col=1).        
-00005eb0: 2020 2020 6665 6174 7572 652c 206c 6162      feature, lab
-00005ec0: 656c 7320 3d20 7463 6c75 7374 6572 2e74  els = tcluster.t
-00005ed0: 7261 696e 2864 6174 615b 3a35 3030 305d  rain(data[:5000]
-00005ee0: 290a 2020 2020 2020 2020 2020 2020 7463  ).            tc
-00005ef0: 6c75 7374 6572 2e73 686f 775f 636c 7573  luster.show_clus
-00005f00: 7465 7273 2866 6561 7475 7265 2c20 6c61  ters(feature, la
-00005f10: 6265 6c73 2c20 276d 6f64 656c 732f 636c  bels, 'models/cl
-00005f20: 7573 7465 722f 636c 7573 7465 725f 7472  uster/cluster_tr
-00005f30: 6169 6e5f 7365 675f 7361 6d70 6c65 732e  ain_seg_samples.
-00005f40: 706e 6727 290a 2020 2020 2020 2020 2020  png').          
-00005f50: 2020 7220 3d20 7463 6c75 7374 6572 2e70    r = tcluster.p
-00005f60: 7265 6469 6374 2864 6174 615b 3a33 305d  redict(data[:30]
-00005f70: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
-00005f80: 696e 7428 7229 0a20 2020 2020 2020 2060  int(r).        `
-00005f90: 6060 0a20 2020 2020 2020 200a 2020 2020  ``.        .    
-00005fa0: 2020 2020 6f75 7470 7574 3a0a 2020 2020      output:.    
-00005fb0: 2020 2020 0a20 2020 2020 2020 2060 6060      .        ```
-00005fc0: 0a20 2020 2020 2020 2054 6578 7443 6c75  .        TextClu
-00005fd0: 7374 6572 2069 6e73 7461 6e63 6520 284d  ster instance (M
-00005fe0: 696e 6942 6174 6368 4b4d 6561 6e73 286e  iniBatchKMeans(n
-00005ff0: 5f63 6c75 7374 6572 733d 322c 206e 5f69  _clusters=2, n_i
-00006000: 6e69 743d 3130 292c 203c 7079 7465 7874  nit=10), <pytext
-00006010: 636c 6173 7369 6669 6572 2e75 7469 6c73  classifier.utils
-00006020: 2e74 6f6b 656e 697a 6572 2e54 6f6b 656e  .tokenizer.Token
-00006030: 697a 6572 206f 626a 6563 7420 6174 2030  izer object at 0
-00006040: 7837 6638 3062 6434 3638 3262 303e 2c20  x7f80bd4682b0>, 
-00006050: 5466 6964 6656 6563 746f 7269 7a65 7228  TfidfVectorizer(
-00006060: 6e67 7261 6d5f 7261 6e67 653d 2831 2c20  ngram_range=(1, 
-00006070: 3229 2929 0a20 2020 2020 2020 205b 3120  2))).        [1 
-00006080: 3120 3120 3120 3120 3120 3120 3120 3120  1 1 1 1 1 1 1 1 
-00006090: 3120 3120 3820 3120 3120 3120 3120 3120  1 1 8 1 1 1 1 1 
-000060a0: 3120 3120 3120 3120 3120 3920 3120 3120  1 1 1 1 1 9 1 1 
-000060b0: 3820 3120 3120 3920 315d 0a20 2020 2020  8 1 1 9 1].     
-000060c0: 2020 2060 6060 0a20 2020 2020 2020 2063     ```.        c
-000060d0: 6c75 7374 6572 696e 6720 706c 6f74 2069  lustering plot i
-000060e0: 6d61 6765 3a0a 2020 2020 2020 2020 0a20  mage:.        . 
-000060f0: 2020 2020 2020 2021 5b63 6c75 7374 6572         ![cluster
-00006100: 5f69 6d61 6765 5d28 6874 7470 733a 2f2f  _image](https://
-00006110: 6769 7468 7562 2e63 6f6d 2f73 6869 6269  github.com/shibi
-00006120: 6e67 3632 342f 7079 7465 7874 636c 6173  ng624/pytextclas
-00006130: 7369 6669 6572 2f62 6c6f 622f 6d61 7374  sifier/blob/mast
-00006140: 6572 2f64 6f63 732f 636c 7573 7465 725f  er/docs/cluster_
-00006150: 7472 6169 6e5f 7365 675f 7361 6d70 6c65  train_seg_sample
-00006160: 732e 706e 6729 0a20 2020 2020 2020 200a  s.png).        .
-00006170: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00006180: 2023 2320 436f 6e74 6163 740a 2020 2020   ## Contact.    
-00006190: 2020 2020 0a20 2020 2020 2020 202d 2049      .        - I
-000061a0: 7373 7565 28e5 bbba e8ae ae29 efbc 9a5b  ssue(......)...[
-000061b0: 215b 4769 7448 7562 2069 7373 7565 735d  ![GitHub issues]
-000061c0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-000061d0: 656c 6473 2e69 6f2f 6769 7468 7562 2f69  elds.io/github/i
-000061e0: 7373 7565 732f 7368 6962 696e 6736 3234  ssues/shibing624
-000061f0: 2f70 7974 6578 7463 6c61 7373 6966 6965  /pytextclassifie
-00006200: 722e 7376 6729 5d28 6874 7470 733a 2f2f  r.svg)](https://
-00006210: 6769 7468 7562 2e63 6f6d 2f73 6869 6269  github.com/shibi
-00006220: 6e67 3632 342f 7079 7465 7874 636c 6173  ng624/pytextclas
-00006230: 7369 6669 6572 2f69 7373 7565 7329 0a20  sifier/issues). 
-00006240: 2020 2020 2020 202d 20e9 82ae e4bb b6e6         - .......
-00006250: 8891 efbc 9a78 756d 696e 673a 2078 756d  .....xuming: xum
-00006260: 696e 6736 3234 4071 712e 636f 6d0a 2020  ing624@qq.com.  
-00006270: 2020 2020 2020 2d20 e5be aee4 bfa1 e688        - ........
-00006280: 91ef bc9a e58a a0e6 8891 2ae5 beae e4bf  ..........*.....
-00006290: a1e5 8fb7 efbc 9a78 756d 696e 6736 3234  .......xuming624
-000062a0: 2a2c 20e8 bf9b 5079 7468 6f6e 2d4e 4c50  *, ...Python-NLP
-000062b0: e4ba a4e6 b581 e7be a4ef bc8c e5a4 87e6  ................
-000062c0: b3a8 efbc 9a2a e5a7 93e5 908d 2de5 85ac  .....*......-...
-000062d0: e58f b8e5 908d 2d4e 4c50 2a0a 2020 2020  ......-NLP*.    
-000062e0: 2020 2020 3c69 6d67 2073 7263 3d22 646f      <img src="do
-000062f0: 6373 2f77 6563 6861 742e 6a70 6567 2220  cs/wechat.jpeg" 
-00006300: 7769 6474 683d 2232 3030 2220 2f3e 0a20  width="200" />. 
-00006310: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00006320: 0a20 2020 2020 2020 2023 2320 4369 7461  .        ## Cita
-00006330: 7469 6f6e 0a20 2020 2020 2020 200a 2020  tion.        .  
-00006340: 2020 2020 2020 e5a6 82e6 9e9c e4bd a0e5        ..........
-00006350: 9ca8 e7a0 94e7 a9b6 e4b8 ade4 bdbf e794  ................
-00006360: a8e4 ba86 7079 7465 7874 636c 6173 7369  ....pytextclassi
-00006370: 6669 6572 efbc 8ce8 afb7 e68c 89e5 a682  fier............
-00006380: e4b8 8be6 a0bc e5bc 8fe5 bc95 e794 a8ef  ................
-00006390: bc9a 0a20 2020 2020 2020 200a 2020 2020  ...        .    
-000063a0: 2020 2020 4150 413a 0a20 2020 2020 2020      APA:.       
-000063b0: 2060 6060 6c61 7465 780a 2020 2020 2020   ```latex.      
-000063c0: 2020 5875 2c20 4d2e 2050 7974 6578 7463    Xu, M. Pytextc
-000063d0: 6c61 7373 6966 6965 723a 2054 6578 7420  lassifier: Text 
-000063e0: 636c 6173 7369 6669 6572 2074 6f6f 6c6b  classifier toolk
-000063f0: 6974 2066 6f72 204e 4c50 2028 5665 7273  it for NLP (Vers
-00006400: 696f 6e20 312e 322e 3029 205b 436f 6d70  ion 1.2.0) [Comp
-00006410: 7574 6572 2073 6f66 7477 6172 655d 2e20  uter software]. 
-00006420: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00006430: 6f6d 2f73 6869 6269 6e67 3632 342f 7079  om/shibing624/py
-00006440: 7465 7874 636c 6173 7369 6669 6572 0a20  textclassifier. 
-00006450: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
-00006460: 2020 200a 2020 2020 2020 2020 4269 6254     .        BibT
-00006470: 6558 3a0a 2020 2020 2020 2020 6060 606c  eX:.        ```l
-00006480: 6174 6578 0a20 2020 2020 2020 2040 6d69  atex.        @mi
-00006490: 7363 7b50 7974 6578 7463 6c61 7373 6966  sc{Pytextclassif
-000064a0: 6965 722c 0a20 2020 2020 2020 2020 2074  ier,.          t
-000064b0: 6974 6c65 3d7b 5079 7465 7874 636c 6173  itle={Pytextclas
-000064c0: 7369 6669 6572 3a20 5465 7874 2063 6c61  sifier: Text cla
-000064d0: 7373 6966 6965 7220 746f 6f6c 6b69 7420  ssifier toolkit 
-000064e0: 666f 7220 4e4c 507d 2c0a 2020 2020 2020  for NLP},.      
-000064f0: 2020 2020 6175 7468 6f72 3d7b 5875 204d      author={Xu M
-00006500: 696e 677d 2c0a 2020 2020 2020 2020 2020  ing},.          
-00006510: 7965 6172 3d7b 3230 3232 7d2c 0a20 2020  year={2022},.   
-00006520: 2020 2020 2020 2068 6f77 7075 626c 6973         howpublis
-00006530: 6865 643d 7b5c 7572 6c7b 6874 7470 733a  hed={\url{https:
-00006540: 2f2f 6769 7468 7562 2e63 6f6d 2f73 6869  //github.com/shi
-00006550: 6269 6e67 3632 342f 7079 7465 7874 636c  bing624/pytextcl
-00006560: 6173 7369 6669 6572 7d7d 2c0a 2020 2020  assifier}},.    
-00006570: 2020 2020 7d0a 2020 2020 2020 2020 6060      }.        ``
-00006580: 600a 2020 2020 2020 2020 0a20 2020 2020  `.        .     
-00006590: 2020 200a 2020 2020 2020 2020 2323 204c     .        ## L
-000065a0: 6963 656e 7365 0a20 2020 2020 2020 200a  icense.        .
-000065b0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-000065c0: 20e6 8e88 e69d 83e5 8d8f e8ae aee4 b8ba   ...............
-000065d0: 205b 5468 6520 4170 6163 6865 204c 6963   [The Apache Lic
-000065e0: 656e 7365 2032 2e30 5d28 4c49 4345 4e53  ense 2.0](LICENS
-000065f0: 4529 efbc 8ce5 8faf e585 8de8 b4b9 e794  E)..............
-00006600: a8e5 819a e595 86e4 b89a e794 a8e9 8094  ................
-00006610: e380 82e8 afb7 e59c a8e4 baa7 e593 81e8  ................
-00006620: afb4 e698 8ee4 b8ad e999 84e5 8aa0 2a2a  ..............**
-00006630: 7079 7465 7874 636c 6173 7369 6669 6572  pytextclassifier
-00006640: 2a2a e79a 84e9 93be e68e a5e5 928c e68e  **..............
-00006650: 88e6 9d83 e58d 8fe8 aeae e380 820a 2020  ..............  
-00006660: 2020 2020 2020 0a20 2020 2020 2020 200a        .        .
-00006670: 2020 2020 2020 2020 2323 2043 6f6e 7472          ## Contr
-00006680: 6962 7574 650a 2020 2020 2020 2020 e9a1  ibute.        ..
-00006690: b9e7 9bae e4bb a3e7 a081 e8bf 98e5 be88  ................
-000066a0: e7b2 97e7 b399 efbc 8ce5 a682 e69e 9ce5  ................
-000066b0: a4a7 e5ae b6e5 afb9 e4bb a3e7 a081 e69c  ................
-000066c0: 89e6 8980 e694 b9e8 bf9b efbc 8ce6 aca2  ................
-000066d0: e8bf 8ee6 8f90 e4ba a4e5 9b9e e69c ace9  ................
-000066e0: a1b9 e79b aeef bc8c e59c a8e6 8f90 e4ba  ................
-000066f0: a4e4 b98b e589 8def bc8c e6b3 a8e6 848f  ................
-00006700: e4bb a5e4 b88b e4b8 a4e7 82b9 efbc 9a0a  ................
-00006710: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00006720: 2020 2d20 e59c a860 7465 7374 7360 e6b7    - ...`tests`..
-00006730: bbe5 8aa0 e79b b8e5 ba94 e79a 84e5 8d95  ................
-00006740: e585 83e6 b58b e8af 950a 2020 2020 2020  ..........      
-00006750: 2020 202d 20e4 bdbf e794 a860 7079 7468     - ......`pyth
-00006760: 6f6e 2073 6574 7570 2e70 7920 7465 7374  on setup.py test
-00006770: 60e6 9da5 e8bf 90e8 a18c e689 80e6 9c89  `...............
-00006780: e58d 95e5 8583 e6b5 8be8 af95 efbc 8ce7  ................
-00006790: a1ae e4bf 9de6 8980 e69c 89e5 8d95 e6b5  ................
-000067a0: 8be9 83bd e698 afe9 809a e8bf 87e7 9a84  ................
-000067b0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-000067c0: 2020 e4b9 8be5 908e e58d b3e5 8faf e68f    ..............
-000067d0: 90e4 baa4 5052 e380 820a 2020 2020 2020  ....PR....      
-000067e0: 2020 0a20 2020 2020 2020 200a 4b65 7977    .        .Keyw
-000067f0: 6f72 6473 3a20 7079 7465 7874 636c 6173  ords: pytextclas
-00006800: 7369 6669 6572 2c74 6578 7463 6c61 7373  sifier,textclass
-00006810: 6966 6965 722c 636c 6173 7369 6669 6572  ifier,classifier
-00006820: 2c74 6578 7463 6c61 7373 6966 6963 6174  ,textclassificat
-00006830: 696f 6e0a 506c 6174 666f 726d 3a20 554e  ion.Platform: UN
-00006840: 4b4e 4f57 4e0a 436c 6173 7369 6669 6572  KNOWN.Classifier
-00006850: 3a20 496e 7465 6e64 6564 2041 7564 6965  : Intended Audie
-00006860: 6e63 6520 3a3a 2053 6369 656e 6365 2f52  nce :: Science/R
-00006870: 6573 6561 7263 680a 436c 6173 7369 6669  esearch.Classifi
-00006880: 6572 3a20 4f70 6572 6174 696e 6720 5379  er: Operating Sy
-00006890: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
-000068a0: 656e 6465 6e74 0a43 6c61 7373 6966 6965  endent.Classifie
-000068b0: 723a 204c 6963 656e 7365 203a 3a20 4f53  r: License :: OS
-000068c0: 4920 4170 7072 6f76 6564 203a 3a20 4170  I Approved :: Ap
-000068d0: 6163 6865 2053 6f66 7477 6172 6520 4c69  ache Software Li
-000068e0: 6365 6e73 650a 436c 6173 7369 6669 6572  cense.Classifier
-000068f0: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-00006900: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00006910: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-00006920: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00006930: 6520 3a3a 2050 7974 686f 6e20 3a3a 2032  e :: Python :: 2
-00006940: 2e37 0a43 6c61 7373 6966 6965 723a 2050  .7.Classifier: P
-00006950: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00006960: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00006970: 2033 0a43 6c61 7373 6966 6965 723a 2054   3.Classifier: T
-00006980: 6f70 6963 203a 3a20 5465 7874 2050 726f  opic :: Text Pro
-00006990: 6365 7373 696e 6720 3a3a 204c 696e 6775  cessing :: Lingu
-000069a0: 6973 7469 630a 436c 6173 7369 6669 6572  istic.Classifier
-000069b0: 3a20 546f 7069 6320 3a3a 2053 6369 656e  : Topic :: Scien
-000069c0: 7469 6669 632f 456e 6769 6e65 6572 696e  tific/Engineerin
-000069d0: 6720 3a3a 2041 7274 6966 6963 6961 6c20  g :: Artificial 
-000069e0: 496e 7465 6c6c 6967 656e 6365 0a44 6573  Intelligence.Des
-000069f0: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
-00006a00: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
-00006a10: 646f 776e 0a                             down.
+00003430: 7374 5f64 6174 6129 0a20 2020 2070 7269  st_data).    pri
+00003440: 6e74 2866 2761 6363 5f73 636f 7265 3a20  nt(f'acc_score: 
+00003450: 7b61 6363 5f73 636f 7265 7d27 290a 0a20  {acc_score}').. 
+00003460: 2020 2023 2074 7261 696e 206d 6f64 656c     # train model
+00003470: 2077 6974 6820 3177 2064 6174 6120 6669   with 1w data fi
+00003480: 6c65 2061 6e64 2031 3020 636c 6173 7365  le and 10 classe
+00003490: 730a 2020 2020 7072 696e 7428 272d 2720  s.    print('-' 
+000034a0: 2a20 3432 290a 2020 2020 6d20 3d20 4265  * 42).    m = Be
+000034b0: 7274 436c 6173 7369 6669 6572 286f 7574  rtClassifier(out
+000034c0: 7075 745f 6469 723d 276d 6f64 656c 732f  put_dir='models/
+000034d0: 6265 7274 2d63 6869 6e65 7365 272c 206e  bert-chinese', n
+000034e0: 756d 5f63 6c61 7373 6573 3d31 302c 0a20  um_classes=10,. 
+000034f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003500: 2020 2020 2020 6d6f 6465 6c5f 7479 7065        model_type
+00003510: 3d27 6265 7274 272c 206d 6f64 656c 5f6e  ='bert', model_n
+00003520: 616d 653d 2762 6572 742d 6261 7365 2d63  ame='bert-base-c
+00003530: 6869 6e65 7365 272c 206e 756d 5f65 706f  hinese', num_epo
+00003540: 6368 733d 322c 0a20 2020 2020 2020 2020  chs=2,.         
+00003550: 2020 2020 2020 2020 2020 2020 2020 6172                ar
+00003560: 6773 3d7b 226e 6f5f 6361 6368 6522 3a20  gs={"no_cache": 
+00003570: 5472 7565 2c20 226c 617a 795f 6c6f 6164  True, "lazy_load
+00003580: 696e 6722 3a20 5472 7565 2c20 226c 617a  ing": True, "laz
+00003590: 795f 7465 7874 5f63 6f6c 756d 6e22 3a20  y_text_column": 
+000035a0: 312c 2022 6c61 7a79 5f6c 6162 656c 735f  1, "lazy_labels_
+000035b0: 636f 6c75 6d6e 223a 2030 2c20 7d29 0a20  column": 0, }). 
+000035c0: 2020 2064 6174 615f 6669 6c65 203d 2027     data_file = '
+000035d0: 7468 7563 6e65 7773 5f74 7261 696e 5f31  thucnews_train_1
+000035e0: 772e 7478 7427 0a20 2020 2023 20e5 a682  w.txt'.    # ...
+000035f0: e69e 9ce8 aead e7bb 83e6 95b0 e68d aee8  ................
+00003600: b685 e8bf 87e7 99be e4b8 87e6 9da1 efbc  ................
+00003610: 8ce5 bbba e8ae aee4 bdbf e794 a86c 617a  .............laz
+00003620: 795f 6c6f 6164 696e 67e6 a8a1 e5bc 8fef  y_loading.......
+00003630: bc8c e587 8fe5 b091 e586 85e5 ad98 e58d  ................
+00003640: a0e7 94a8 0a20 2020 206d 2e74 7261 696e  .....    m.train
+00003650: 2864 6174 615f 6669 6c65 2c20 7465 7374  (data_file, test
+00003660: 5f73 697a 653d 302c 206e 616d 6573 3d28  _size=0, names=(
+00003670: 276c 6162 656c 7327 2c20 2774 6578 7427  'labels', 'text'
+00003680: 2929 0a20 2020 206d 2e6c 6f61 645f 6d6f  )).    m.load_mo
+00003690: 6465 6c28 290a 2020 2020 7072 6564 6963  del().    predic
+000036a0: 745f 6c61 6265 6c2c 2070 7265 6469 6374  t_label, predict
+000036b0: 5f70 726f 6261 203d 206d 2e70 7265 6469  _proba = m.predi
+000036c0: 6374 280a 2020 2020 2020 2020 5b27 e9a1  ct(.        ['..
+000036d0: bae4 b989 e58c 97e4 baac e88b 8fe6 b4bb  ................
+000036e0: 3838 e5b9 b3e7 b1b3 e8b5 b7e7 b2be e8a3  88..............
+000036f0: 85e6 88bf e59c a8e5 94ae 272c 0a20 2020  ..........',.   
+00003700: 2020 2020 2020 27e7 be8e 4542 2d35 e9a1        '...EB-5..
+00003710: b9e7 9bae e280 9c31 35e6 97a5 e5bf abe9  .......15.......
+00003720: 809f e7a7 bbe6 b091 e280 9de5 b086 e68e  ................
+00003730: a8e8 bf9f 272c 0a20 2020 2020 2020 2020  ....',.         
+00003740: 27e6 8192 e794 9f41 48e6 baa2 e68c 87e6  '......AH.......
+00003750: 94b6 e5b9 b320 41e8 82a1 e5af b948 e882  ..... A......H..
+00003760: a1e6 8a98 e4bb b731 2e39 3525 275d 290a  .......1.95%']).
+00003770: 2020 2020 7072 696e 7428 6627 7072 6564      print(f'pred
+00003780: 6963 745f 6c61 6265 6c3a 207b 7072 6564  ict_label: {pred
+00003790: 6963 745f 6c61 6265 6c7d 2c20 7072 6564  ict_label}, pred
+000037a0: 6963 745f 7072 6f62 613a 207b 7072 6564  ict_proba: {pred
+000037b0: 6963 745f 7072 6f62 617d 2729 0a60 6060  ict_proba}').```
+000037c0: 0a50 53ef bc9a e5a6 82e6 9e9c e8ae ade7  .PS.............
+000037d0: bb83 e695 b0e6 8dae e8b6 85e8 bf87 e799  ................
+000037e0: bee4 b887 e69d a1ef bc8c e5bb bae8 aeae  ................
+000037f0: e4bd bfe7 94a8 6c61 7a79 5f6c 6f61 6469  ......lazy_loadi
+00003800: 6e67 e6a8 a1e5 bc8f efbc 8ce5 878f e5b0  ng..............
+00003810: 91e5 8685 e5ad 98e5 8da0 e794 a80a 0a23  ...............#
+00003820: 2323 2320 e5a4 9ae6 a087 e7ad bee5 8886  ### ............
+00003830: e7b1 bbe6 a8a1 e59e 8b0a e588 86e7 b1bb  ................
+00003840: e58f afe4 bba5 e588 86e4 b8ba e5a4 9ae5  ................
+00003850: 8886 e7b1 bbe5 928c e5a4 9ae6 a087 e7ad  ................
+00003860: bee5 8886 e7b1 bbe3 8082 e5a4 9ae5 8886  ................
+00003870: e7b1 bbe7 9a84 e6a0 87e7 adbe e698 afe6  ................
+00003880: 8e92 e4bb 96e7 9a84 efbc 8ce8 808c e5a4  ................
+00003890: 9ae6 a087 e7ad bee5 8886 e7b1 bbe7 9a84  ................
+000038a0: e689 80e6 9c89 e6a0 87e7 adbe e698 afe4  ................
+000038b0: b88d e68e 92e4 bb96 e79a 84e3 8082 0a0a  ................
+000038c0: e5a4 9ae6 a087 e7ad bee5 8886 e7b1 bbe6  ................
+000038d0: af94 e8be 83e7 9bb4 e8a7 82e7 9a84 e790  ................
+000038e0: 86e8 a7a3 e698 afef bc8c e4b8 80e4 b8aa  ................
+000038f0: e6a0 b7e6 9cac e58f afe4 bba5 e590 8ce6  ................
+00003900: 97b6 e68b a5e6 9c89 e587 a0e4 b8aa e7b1  ................
+00003910: bbe5 88ab e6a0 87e7 adbe efbc 8c0a e6af  ................
+00003920: 94e5 a682 e4b8 80e9 a696 e6ad 8ce7 9a84  ................
+00003930: e6a0 87e7 adbe e58f afe4 bba5 e698 afe6  ................
+00003940: b581 e8a1 8ce3 8081 e8bd bbe5 bfab efbc  ................
+00003950: 8ce4 b880 e983 a8e7 94b5 e5bd b1e7 9a84  ................
+00003960: e6a0 87e7 adbe e58f afe4 bba5 e698 afe5  ................
+00003970: 8aa8 e4bd 9ce3 8081 e596 9ce5 89a7 e380  ................
+00003980: 81e6 909e e7ac 91e7 ad89 efbc 8ce8 bf99  ................
+00003990: e983 bde6 98af e5a4 9ae6 a087 e7ad bee5  ................
+000039a0: 8886 e7b1 bbe7 9a84 e683 85e5 86b5 e380  ................
+000039b0: 820a 0ae8 aead e7bb 83e5 928c e9a2 84e6  ................
+000039c0: b58b 6042 4552 5460 e5a4 9ae6 a087 e7ad  ..`BERT`........
+000039d0: bee5 8886 e7b1 bbe6 a8a1 e59e 8bef bc8c  ................
+000039e0: e7a4 bae4 be8b 5b65 7861 6d70 6c65 732f  ......[examples/
+000039f0: 6265 7274 5f6d 756c 7469 6c61 6265 6c5f  bert_multilabel_
+00003a00: 636c 6173 7369 6669 6361 7469 6f6e 5f7a  classification_z
+00003a10: 685f 6465 6d6f 2e70 792e 7079 5d28 6874  h_demo.py.py](ht
+00003a20: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00003a30: 2f73 6869 6269 6e67 3632 342f 7079 7465  /shibing624/pyte
+00003a40: 7874 636c 6173 7369 6669 6572 2f62 6c6f  xtclassifier/blo
+00003a50: 622f 6d61 7374 6572 2f65 7861 6d70 6c65  b/master/example
+00003a60: 732f 6265 7274 5f6d 756c 7469 6c61 6265  s/bert_multilabe
+00003a70: 6c5f 636c 6173 7369 6669 6361 7469 6f6e  l_classification
+00003a80: 5f7a 685f 6465 6d6f 2e70 7929 0a0a 6060  _zh_demo.py)..``
+00003a90: 6070 7974 686f 6e0a 696d 706f 7274 2073  `python.import s
+00003aa0: 7973 0a69 6d70 6f72 7420 7061 6e64 6173  ys.import pandas
+00003ab0: 2061 7320 7064 0a0a 7379 732e 7061 7468   as pd..sys.path
+00003ac0: 2e61 7070 656e 6428 272e 2e27 290a 6672  .append('..').fr
+00003ad0: 6f6d 2070 7974 6578 7463 6c61 7373 6966  om pytextclassif
+00003ae0: 6965 7220 696d 706f 7274 2042 6572 7443  ier import BertC
+00003af0: 6c61 7373 6966 6965 720a 0a0a 6465 6620  lassifier...def 
+00003b00: 6c6f 6164 5f6a 645f 6461 7461 2866 696c  load_jd_data(fil
+00003b10: 655f 7061 7468 293a 0a20 2020 2022 2222  e_path):.    """
+00003b20: 0a20 2020 204c 6f61 6420 6a64 2064 6174  .    Load jd dat
+00003b30: 6120 6672 6f6d 2066 696c 652e 0a20 2020  a from file..   
+00003b40: 2040 7061 7261 6d20 6669 6c65 5f70 6174   @param file_pat
+00003b50: 683a 200a 2020 2020 2020 2020 666f 726d  h: .        form
+00003b60: 6174 3a20 636f 6e74 656e 742c e585 b6e4  at: content,....
+00003b70: bb96 2ce4 ba92 e881 94e4 ba92 e980 9a2c  ..,............,
+00003b80: e4ba a7e5 9381 e58a 9fe8 8097 2ce6 bb91  ............,...
+00003b90: e8bd aee6 8f90 e689 8b2c e5a3 b0e9 9fb3  .........,......
+00003ba0: 2c41 5050 e693 8de6 8ea7 e680 a72c e591  ,APP.........,..
+00003bb0: bce5 90b8 e781 af2c e5a4 96e8 a782 2ce5  .......,......,.
+00003bc0: ba95 e5ba a72c e588 b6e7 83ad e88c 83e5  .....,..........
+00003bd0: 9bb4 2ce9 81a5 e68e a7e5 99a8 e794 b5e6  ..,.............
+00003be0: b1a0 2ce5 91b3 e981 932c e588 b6e7 83ad  ..,......,......
+00003bf0: e695 88e6 9e9c 2ce8 a1a3 e789 a9e7 8398  ......,.........
+00003c00: e5b9 b22c e4bd 93e7 a7af e5a4 a7e5 b08f  ...,............
+00003c10: 0a20 2020 2040 7265 7475 726e 3a20 0a20  .    @return: . 
+00003c20: 2020 2022 2222 0a20 2020 2064 6174 6120     """.    data 
+00003c30: 3d20 5b5d 0a20 2020 2077 6974 6820 6f70  = [].    with op
+00003c40: 656e 2866 696c 655f 7061 7468 2c20 2772  en(file_path, 'r
+00003c50: 272c 2065 6e63 6f64 696e 673d 2775 7466  ', encoding='utf
+00003c60: 2d38 2729 2061 7320 663a 0a20 2020 2020  -8') as f:.     
+00003c70: 2020 2066 6f72 206c 696e 6520 696e 2066     for line in f
+00003c80: 3a0a 2020 2020 2020 2020 2020 2020 6c69  :.            li
+00003c90: 6e65 203d 206c 696e 652e 7374 7269 7028  ne = line.strip(
+00003ca0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00003cb0: 206c 696e 652e 7374 6172 7473 7769 7468   line.startswith
+00003cc0: 2827 2327 293a 0a20 2020 2020 2020 2020  ('#'):.         
+00003cd0: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
+00003ce0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00003cf0: 6f74 206c 696e 653a 0a20 2020 2020 2020  ot line:.       
+00003d00: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
+00003d10: 650a 2020 2020 2020 2020 2020 2020 7465  e.            te
+00003d20: 726d 7320 3d20 6c69 6e65 2e73 706c 6974  rms = line.split
+00003d30: 2827 2c27 290a 2020 2020 2020 2020 2020  (',').          
+00003d40: 2020 6966 206c 656e 2874 6572 6d73 2920    if len(terms) 
+00003d50: 213d 2031 363a 0a20 2020 2020 2020 2020  != 16:.         
+00003d60: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
+00003d70: 2020 2020 2020 2020 2020 2020 7661 6c20              val 
+00003d80: 3d20 5b69 6e74 2869 2920 666f 7220 6920  = [int(i) for i 
+00003d90: 696e 2074 6572 6d73 5b31 3a5d 5d0a 2020  in terms[1:]].  
+00003da0: 2020 2020 2020 2020 2020 6461 7461 2e61            data.a
+00003db0: 7070 656e 6428 5b74 6572 6d73 5b30 5d2c  ppend([terms[0],
+00003dc0: 2076 616c 5d29 0a20 2020 2072 6574 7572   val]).    retur
+00003dd0: 6e20 6461 7461 0a0a 0a69 6620 5f5f 6e61  n data...if __na
+00003de0: 6d65 5f5f 203d 3d20 275f 5f6d 6169 6e5f  me__ == '__main_
+00003df0: 5f27 3a0a 2020 2020 2320 6d6f 6465 6c5f  _':.    # model_
+00003e00: 7479 7065 3a20 7375 7070 6f72 7420 2762  type: support 'b
+00003e10: 6572 7427 2c20 2761 6c62 6572 7427 2c20  ert', 'albert', 
+00003e20: 2772 6f62 6572 7461 272c 2027 786c 6e65  'roberta', 'xlne
+00003e30: 7427 0a20 2020 2023 206d 6f64 656c 5f6e  t'.    # model_n
+00003e40: 616d 653a 2073 7570 706f 7274 2027 6265  ame: support 'be
+00003e50: 7274 2d62 6173 652d 6368 696e 6573 6527  rt-base-chinese'
+00003e60: 2c20 2762 6572 742d 6261 7365 2d63 6173  , 'bert-base-cas
+00003e70: 6564 272c 2027 6265 7274 2d62 6173 652d  ed', 'bert-base-
+00003e80: 6d75 6c74 696c 696e 6775 616c 2d63 6173  multilingual-cas
+00003e90: 6564 2720 2e2e 2e0a 2020 2020 6d20 3d20  ed' ....    m = 
+00003ea0: 4265 7274 436c 6173 7369 6669 6572 286f  BertClassifier(o
+00003eb0: 7574 7075 745f 6469 723d 276d 6f64 656c  utput_dir='model
+00003ec0: 732f 6d75 6c74 696c 6162 656c 2d62 6572  s/multilabel-ber
+00003ed0: 742d 7a68 2d6d 6f64 656c 272c 206e 756d  t-zh-model', num
+00003ee0: 5f63 6c61 7373 6573 3d31 352c 0a20 2020  _classes=15,.   
+00003ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f00: 2020 2020 6d6f 6465 6c5f 7479 7065 3d27      model_type='
+00003f10: 6265 7274 272c 206d 6f64 656c 5f6e 616d  bert', model_nam
+00003f20: 653d 2762 6572 742d 6261 7365 2d63 6869  e='bert-base-chi
+00003f30: 6e65 7365 272c 206e 756d 5f65 706f 6368  nese', num_epoch
+00003f40: 733d 322c 206d 756c 7469 5f6c 6162 656c  s=2, multi_label
+00003f50: 3d54 7275 6529 0a20 2020 2023 2054 7261  =True).    # Tra
+00003f60: 696e 2061 6e64 2045 7661 6c75 6174 696f  in and Evaluatio
+00003f70: 6e20 6461 7461 206e 6565 6473 2074 6f20  n data needs to 
+00003f80: 6265 2069 6e20 6120 5061 6e64 6173 2044  be in a Pandas D
+00003f90: 6174 6166 7261 6d65 2063 6f6e 7461 696e  ataframe contain
+00003fa0: 696e 6720 6174 206c 6561 7374 2074 776f  ing at least two
+00003fb0: 2063 6f6c 756d 6e73 2c20 6120 2774 6578   columns, a 'tex
+00003fc0: 7427 2061 6e64 2061 2027 6c61 6265 6c73  t' and a 'labels
+00003fd0: 2720 636f 6c75 6d6e 2e20 5468 6520 606c  ' column. The `l
+00003fe0: 6162 656c 7360 2063 6f6c 756d 6e20 7368  abels` column sh
+00003ff0: 6f75 6c64 2063 6f6e 7461 696e 206d 756c  ould contain mul
+00004000: 7469 2d68 6f74 2065 6e63 6f64 6564 206c  ti-hot encoded l
+00004010: 6973 7473 2e0a 2020 2020 7472 6169 6e5f  ists..    train_
+00004020: 6461 7461 203d 205b 0a20 2020 2020 2020  data = [.       
+00004030: 205b 22e4 b880 e4b8 aae5 b08f e697 b6e6   [".............
+00004040: 88bf e997 b4e4 bb8d e784 b6e6 b2a1 e69a  ................
+00004050: 96e5 928c 222c 205b 302c 2030 2c20 302c  ....", [0, 0, 0,
+00004060: 2030 2c20 302c 2030 2c20 302c 2030 2c20   0, 0, 0, 0, 0, 
+00004070: 302c 2030 2c20 302c 2030 2c20 312c 2030  0, 0, 0, 0, 1, 0
+00004080: 2c20 305d 5d2c 0a20 2020 2020 2020 205b  , 0]],.        [
+00004090: 22e8 8097 e794 b5e6 8385 e586 b5ef bc9a  "...............
+000040a0: e8bf 99e4 b8aa e6b2 a1e6 9c89 e6b3 a8e6  ................
+000040b0: 848f 222c 205b 302c 2030 2c20 312c 2030  ..", [0, 0, 1, 0
+000040c0: 2c20 302c 2030 2c20 302c 2030 2c20 302c  , 0, 0, 0, 0, 0,
+000040d0: 2030 2c20 302c 2030 2c20 302c 2030 2c20   0, 0, 0, 0, 0, 
+000040e0: 305d 5d2c 0a20 2020 205d 0a20 2020 2064  0]],.    ].    d
+000040f0: 6174 6120 3d20 6c6f 6164 5f6a 645f 6461  ata = load_jd_da
+00004100: 7461 2827 6d75 6c74 696c 6162 656c 5f6a  ta('multilabel_j
+00004110: 645f 636f 6d6d 656e 7473 2e63 7376 2729  d_comments.csv')
+00004120: 0a20 2020 2074 7261 696e 5f64 6174 612e  .    train_data.
+00004130: 6578 7465 6e64 2864 6174 6129 0a20 2020  extend(data).   
+00004140: 2070 7269 6e74 2874 7261 696e 5f64 6174   print(train_dat
+00004150: 615b 3a35 5d29 0a20 2020 2074 7261 696e  a[:5]).    train
+00004160: 5f64 6620 3d20 7064 2e44 6174 6146 7261  _df = pd.DataFra
+00004170: 6d65 2874 7261 696e 5f64 6174 612c 2063  me(train_data, c
+00004180: 6f6c 756d 6e73 3d5b 2274 6578 7422 2c20  olumns=["text", 
+00004190: 226c 6162 656c 7322 5d29 0a0a 2020 2020  "labels"])..    
+000041a0: 7072 696e 7428 7472 6169 6e5f 6466 2e68  print(train_df.h
+000041b0: 6561 6428 2929 0a20 2020 206d 2e74 7261  ead()).    m.tra
+000041c0: 696e 2874 7261 696e 5f64 6629 0a20 2020  in(train_df).   
+000041d0: 2070 7269 6e74 286d 290a 2020 2020 2320   print(m).    # 
+000041e0: 4576 616c 7561 7465 2074 6865 206d 6f64  Evaluate the mod
+000041f0: 656c 0a20 2020 2061 6363 5f73 636f 7265  el.    acc_score
+00004200: 203d 206d 2e65 7661 6c75 6174 655f 6d6f   = m.evaluate_mo
+00004210: 6465 6c28 7472 6169 6e5f 6466 5b3a 3230  del(train_df[:20
+00004220: 5d29 0a20 2020 2070 7269 6e74 2866 2761  ]).    print(f'a
+00004230: 6363 5f73 636f 7265 3a20 7b61 6363 5f73  cc_score: {acc_s
+00004240: 636f 7265 7d27 290a 0a20 2020 2023 206c  core}')..    # l
+00004250: 6f61 6420 7472 6169 6e65 6420 6265 7374  oad trained best
+00004260: 206d 6f64 656c 2066 726f 6d20 6d6f 6465   model from mode
+00004270: 6c5f 6469 720a 2020 2020 6d2e 6c6f 6164  l_dir.    m.load
+00004280: 5f6d 6f64 656c 2829 0a20 2020 2070 7265  _model().    pre
+00004290: 6469 6374 5f6c 6162 656c 2c20 7072 6564  dict_label, pred
+000042a0: 6963 745f 7072 6f62 6120 3d20 6d2e 7072  ict_proba = m.pr
+000042b0: 6564 6963 7428 5b27 e4b8 80e4 b8aa e5b0  edict(['........
+000042c0: 8fe6 97b6 e688 bfe9 97b4 e4bb 8de7 84b6  ................
+000042d0: e6b2 a1e6 9a96 e592 8c27 2c20 27e8 8097  .........', '...
+000042e0: e794 b5e6 8385 e586 b5ef bc9a e8bf 99e4  ................
+000042f0: b8aa e6b2 a1e6 9c89 e6b3 a8e6 848f 275d  ..............']
+00004300: 290a 2020 2020 7072 696e 7428 6627 7072  ).    print(f'pr
+00004310: 6564 6963 745f 6c61 6265 6c3a 207b 7072  edict_label: {pr
+00004320: 6564 6963 745f 6c61 6265 6c7d 2c20 7072  edict_label}, pr
+00004330: 6564 6963 745f 7072 6f62 613a 207b 7072  edict_proba: {pr
+00004340: 6564 6963 745f 7072 6f62 617d 2729 0a60  edict_proba}').`
+00004350: 6060 0a0a 2323 2045 7661 6c75 6174 696f  ``..## Evaluatio
+00004360: 6e0a 0a23 2323 2044 6174 6173 6574 0a0a  n..### Dataset..
+00004370: 312e 2054 4855 434e 6577 73e4 b8ad e696  1. THUCNews.....
+00004380: 87e6 9687 e69c ace6 95b0 e68d aee9 9b86  ................
+00004390: efbc 8831 2e35 3647 42ef bc89 efbc 9ae5  ...1.56GB.......
+000043a0: ae98 e696 b95b e4b8 8be8 bdbd e59c b0e5  .....[..........
+000043b0: 9d80 5d28 6874 7470 3a2f 2f74 6875 6374  ..](http://thuct
+000043c0: 632e 7468 756e 6c70 2e6f 7267 2f29 efbc  c.thunlp.org/)..
+000043d0: 8ce6 8abd e6a0 b7e4 ba86 3130 e4b8 87e6  ..........10....
+000043e0: 9da1 5448 5543 4e65 7773 e4b8 ade6 9687  ..THUCNews......
+000043f0: e696 87e6 9cac 3130 e588 86e7 b1bb e695  ......10........
+00004400: b0e6 8dae e99b 86ef bc88 364d 42ef bc89  ..........6MB...
+00004410: efbc 8ce5 9cb0 e59d 80ef bc9a 5b65 7861  ............[exa
+00004420: 6d70 6c65 732f 7468 7563 6e65 7773 5f74  mples/thucnews_t
+00004430: 7261 696e 5f31 3077 2e74 7874 5d28 6874  rain_10w.txt](ht
+00004440: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00004450: 2f73 6869 6269 6e67 3632 342f 7079 7465  /shibing624/pyte
+00004460: 7874 636c 6173 7369 6669 6572 2f62 6c6f  xtclassifier/blo
+00004470: 622f 6d61 7374 6572 2f65 7861 6d70 6c65  b/master/example
+00004480: 732f 7468 7563 6e65 7773 5f74 7261 696e  s/thucnews_train
+00004490: 5f31 3077 2e74 7874 29e3 8082 0a32 2e20  _10w.txt)....2. 
+000044a0: 544e 4557 53e4 bb8a e697 a5e5 a4b4 e69d  TNEWS...........
+000044b0: a1e4 b8ad e696 87e6 96b0 e997 bbef bc88  ................
+000044c0: e79f ade6 9687 e69c acef bc89 e588 86e7  ................
+000044d0: b1bb 2053 686f 7274 2054 6578 7420 436c  .. Short Text Cl
+000044e0: 6173 7369 6669 6361 6974 6f6e 2066 6f72  assificaiton for
+000044f0: 204e 6577 73ef bc8c e8af a5e6 95b0 e68d   News...........
+00004500: aee9 9b86 2835 2e31 4d42 29e6 9da5 e887  ....(5.1MB).....
+00004510: aae4 bb8a e697 a5e5 a4b4 e69d a1e7 9a84  ................
+00004520: e696 b0e9 97bb e789 88e5 9d97 efbc 8ce5  ................
+00004530: 85b1 e68f 90e5 8f96 e4ba 8631 35e4 b8aa  ...........15...
+00004540: e7b1 bbe5 88ab e79a 84e6 96b0 e997 bbef  ................
+00004550: bc8c e58c 85e6 8bac e697 85e6 b8b8 efbc  ................
+00004560: 8ce6 9599 e882 b2ef bc8c e987 91e8 9e8d  ................
+00004570: efbc 8ce5 869b e4ba 8be7 ad89 efbc 8ce5  ................
+00004580: 9cb0 e59d 80ef bc9a 5b74 6e65 7773 5f70  ........[tnews_p
+00004590: 7562 6c69 632e 7a69 705d 2868 7474 7073  ublic.zip](https
+000045a0: 3a2f 2f73 746f 7261 6765 2e67 6f6f 676c  ://storage.googl
+000045b0: 6561 7069 732e 636f 6d2f 636c 7565 6265  eapis.com/cluebe
+000045c0: 6e63 686d 6172 6b2f 7461 736b 732f 746e  nchmark/tasks/tn
+000045d0: 6577 735f 7075 626c 6963 2e7a 6970 290a  ews_public.zip).
+000045e0: 0a23 2323 2045 7661 6c75 6174 696f 6e20  .### Evaluation 
+000045f0: 5265 7375 6c74 0ae5 9ca8 5448 5543 4e65  Result....THUCNe
+00004600: 7773 e4b8 ade6 9687 e696 87e6 9cac 3130  ws............10
+00004610: e588 86e7 b1bb e695 b0e6 8dae e99b 86ef  ................
+00004620: bc88 364d 42ef bc89 e4b8 8ae8 af84 e4bc  ..6MB...........
+00004630: b0ef bc8c e6a8 a1e5 9e8b e59c a8e6 b58b  ................
+00004640: e8af 95e9 9b86 2874 6573 7429 e8af 84e6  ......(test)....
+00004650: b58b e695 88e6 9e9c e5a6 82e4 b88b efbc  ................
+00004660: 9a0a 0ae6 a8a1 e59e 8b7c 6163 637c e8af  .........|acc|..
+00004670: b4e6 988e 0a2d 2d7c 2d2d 7c2d 2d0a 4c52  .....--|--|--.LR
+00004680: 7c30 2e38 3830 337c e980 bbe8 be91 e59b  |0.8803|........
+00004690: 9ee5 bd92 4c6f 6769 7374 6963 7320 5265  ....Logistics Re
+000046a0: 6772 6573 7369 6f6e 0a54 6578 7443 4e4e  gression.TextCNN
+000046b0: 7c30 2e38 3830 397c 4b69 6d20 3230 3134  |0.8809|Kim 2014
+000046c0: 20e7 bb8f e585 b8e7 9a84 434e 4ee6 9687   .........CNN...
+000046d0: e69c ace5 8886 e7b1 bb0a 5465 7874 524e  ..........TextRN
+000046e0: 4e5f 4174 747c 302e 3930 3232 7c42 694c  N_Att|0.9022|BiL
+000046f0: 5354 4d2b 4174 7465 6e74 696f 6e0a 4661  STM+Attention.Fa
+00004700: 7374 5465 7874 7c30 2e39 3137 377c 626f  stText|0.9177|bo
+00004710: 772b 6269 6772 616d 2b74 7269 6772 616d  w+bigram+trigram
+00004720: efbc 8c20 e695 88e6 9e9c e587 bae5 a587  ... ............
+00004730: e79a 84e5 a5bd 0a44 5043 4e4e 7c30 2e39  .......DPCNN|0.9
+00004740: 3132 357c e6b7 b1e5 b182 e987 91e5 ad97  125|............
+00004750: e5a1 9443 4e4e 0a54 7261 6e73 666f 726d  ...CNN.Transform
+00004760: 6572 7c30 2e38 3939 317c e695 88e6 9e9c  er|0.8991|......
+00004770: e8be 83e5 b7ae 0a42 4552 542d 6261 7365  .......BERT-base
+00004780: 7c2a 2a30 2e39 3438 332a 2a7c 6265 7274  |**0.9483**|bert
+00004790: 202b 2066 630a 4552 4e49 457c 302e 3934   + fc.ERNIE|0.94
+000047a0: 3631 7ce6 af94 6265 7274 e795 a5e5 b7ae  61|...bert......
+000047b0: 0a0a e59c a8e4 b8ad e696 87e6 96b0 e997  ................
+000047c0: bbe7 9fad e696 87e6 9cac e588 86e7 b1bb  ................
+000047d0: e695 b0e6 8dae e99b 8654 4e45 5753 e4b8  .........TNEWS..
+000047e0: 8ae8 af84 e4bc b0ef bc8c e6a8 a1e5 9e8b  ................
+000047f0: e59c a8e5 bc80 e58f 91e9 9b86 2864 6576  ............(dev
+00004800: 29e8 af84 e6b5 8be6 9588 e69e 9ce5 a682  )...............
+00004810: e4b8 8bef bc9a 0a0a e6a8 a1e5 9e8b 7c61  ..............|a
+00004820: 6363 7ce8 afb4 e698 8e0a 2d2d 7c2d 2d7c  cc|.......--|--|
+00004830: 2d2d 0a42 4552 542d 6261 7365 7c2a 2a30  --.BERT-base|**0
+00004840: 2e35 3636 302a 2a7c e69c ace9 a1b9 e79b  .5660**|........
+00004850: aee5 ae9e e78e b00a 4245 5254 2d62 6173  ........BERT-bas
+00004860: 657c 302e 3536 3039 7c43 4c55 4520 4265  e|0.5609|CLUE Be
+00004870: 6e63 686d 6172 6b20 4c65 6164 6572 626f  nchmark Leaderbo
+00004880: 6172 64e7 bb93 e69e 9c20 5b43 4c55 4562  ard...... [CLUEb
+00004890: 656e 6368 6d61 726b 5d28 6874 7470 733a  enchmark](https:
+000048a0: 2f2f 6769 7468 7562 2e63 6f6d 2f43 4c55  //github.com/CLU
+000048b0: 4562 656e 6368 6d61 726b 2f43 4c55 4529  Ebenchmark/CLUE)
+000048c0: 0a0a 2d20 e4bb a5e4 b88a e7bb 93e6 9e9c  ..- ............
+000048d0: e59d 87e4 b8ba e588 86e7 b1bb e79a 84e5  ................
+000048e0: 8786 e7a1 aee7 8e87 efbc 8861 6363 7572  ...........accur
+000048f0: 6163 79ef bc89 e7bb 93e6 9e9c 0a2d 2054  acy..........- T
+00004900: 4855 434e 6577 73e6 95b0 e68d aee9 9b86  HUCNews.........
+00004910: e8af 84e6 b58b e7bb 93e6 9e9c e58f afe4  ................
+00004920: bba5 e59f bae4 ba8e 6065 7861 6d70 6c65  ........`example
+00004930: 732f 7468 7563 6e65 7773 5f74 7261 696e  s/thucnews_train
+00004940: 5f31 3077 2e74 7874 60e6 95b0 e68d aee7  _10w.txt`.......
+00004950: 94a8 6065 7861 6d70 6c65 7360 e4b8 8be7  ..`examples`....
+00004960: 9a84 e590 84e6 a8a1 e59e 8b64 656d 6fe5  ...........demo.
+00004970: a48d e78e b00a 2d20 544e 4557 53e6 95b0  ......- TNEWS...
+00004980: e68d aee9 9b86 e8af 84e6 b58b e7bb 93e6  ................
+00004990: 9e9c e58f afe4 bba5 e4b8 8be8 bdbd 544e  ..............TN
+000049a0: 4557 53e6 95b0 e68d aee9 9b86 efbc 8ce8  EWS.............
+000049b0: bf90 e8a1 8c60 6578 616d 706c 6573 2f62  .....`examples/b
+000049c0: 6572 745f 636c 6173 7369 6669 6361 7469  ert_classificati
+000049d0: 6f6e 5f74 6e65 7773 5f64 656d 6f2e 7079  on_tnews_demo.py
+000049e0: 60e5 a48d e78e b00a 0a23 2323 20e5 91bd  `........### ...
+000049f0: e4bb a4e8 a18c e8b0 83e7 94a8 0a0a e68f  ................
+00004a00: 90e4 be9b e588 86e7 b1bb e6a8 a1e5 9e8b  ................
+00004a10: e591 bde4 bba4 e8a1 8ce8 b083 e794 a8e8  ................
+00004a20: 849a e69c acef bc8c e696 87e4 bbb6 e6a0  ................
+00004a30: 91ef bc9a 0a60 6060 6261 7368 0a70 7974  .....```bash.pyt
+00004a40: 6578 7463 6c61 7373 6966 6965 720a e294  extclassifier...
+00004a50: 9ce2 9480 e294 8020 6265 7274 5f63 6c61  ....... bert_cla
+00004a60: 7373 6966 6965 722e 7079 0ae2 949c e294  ssifier.py......
+00004a70: 80e2 9480 2066 6173 7474 6578 745f 636c  .... fasttext_cl
+00004a80: 6173 7369 6669 6572 2e70 790a e294 9ce2  assifier.py.....
+00004a90: 9480 e294 8020 636c 6173 7369 635f 636c  ..... classic_cl
+00004aa0: 6173 7369 6669 6572 2e70 790a e294 9ce2  assifier.py.....
+00004ab0: 9480 e294 8020 7465 7874 636e 6e5f 636c  ..... textcnn_cl
+00004ac0: 6173 7369 6669 6572 2e70 790a e294 94e2  assifier.py.....
+00004ad0: 9480 e294 8020 7465 7874 726e 6e5f 636c  ..... textrnn_cl
+00004ae0: 6173 7369 6669 6572 2e70 790a 6060 600a  assifier.py.```.
+00004af0: 0ae6 af8f e4b8 aae6 9687 e4bb b6e5 afb9  ................
+00004b00: e5ba 94e4 b880 e4b8 aae6 a8a1 e59e 8be6  ................
+00004b10: 96b9 e6b3 95ef bc8c e590 84e6 a8a1 e59e  ................
+00004b20: 8be5 ae8c e585 a8e7 8bac e7ab 8bef bc8c  ................
+00004b30: e58f afe4 bba5 e79b b4e6 8ea5 e8bf 90e8  ................
+00004b40: a18c efbc 8ce4 b99f e696 b9e4 bebf e4bf  ................
+00004b50: aee6 94b9 efbc 8ce6 94af e68c 81e9 809a  ................
+00004b60: e8bf 8760 6172 6770 6172 7365 6020 e4bf  ...`argparse` ..
+00004b70: aee6 94b9 602d 2d64 6174 615f 7061 7468  ....`--data_path
+00004b80: 60e7 ad89 e58f 82e6 95b0 e380 820a 0ae7  `...............
+00004b90: 9bb4 e68e a5e5 9ca8 e7bb 88e7 abaf e8b0  ................
+00004ba0: 83e7 94a8 6661 7374 7465 7874 e6a8 a1e5  ....fasttext....
+00004bb0: 9e8b e8ae ade7 bb83 efbc 9a0a 6060 6062  ............```b
+00004bc0: 6173 680a 7079 7468 6f6e 202d 6d20 7079  ash.python -m py
+00004bd0: 7465 7874 636c 6173 7369 6669 6572 2e66  textclassifier.f
+00004be0: 6173 7474 6578 745f 636c 6173 7369 6669  asttext_classifi
+00004bf0: 6572 202d 680a 6060 600a 0a23 2320 5465  er -h.```..## Te
+00004c00: 7874 2043 6c75 7374 6572 0a0a 0a54 6578  xt Cluster...Tex
+00004c10: 7420 636c 7573 7465 7269 6e67 2c20 666f  t clustering, fo
+00004c20: 7220 6578 616d 706c 6520 5b65 7861 6d70  r example [examp
+00004c30: 6c65 732f 636c 7573 7465 725f 6465 6d6f  les/cluster_demo
+00004c40: 2e70 795d 2868 7474 7073 3a2f 2f67 6974  .py](https://git
+00004c50: 6875 622e 636f 6d2f 7368 6962 696e 6736  hub.com/shibing6
+00004c60: 3234 2f70 7974 6578 7463 6c61 7373 6966  24/pytextclassif
+00004c70: 6965 722f 626c 6f62 2f6d 6173 7465 722f  ier/blob/master/
+00004c80: 6578 616d 706c 6573 2f63 6c75 7374 6572  examples/cluster
+00004c90: 5f64 656d 6f2e 7079 290a 0a60 6060 7079  _demo.py)..```py
+00004ca0: 7468 6f6e 0a69 6d70 6f72 7420 7379 730a  thon.import sys.
+00004cb0: 0a73 7973 2e70 6174 682e 6170 7065 6e64  .sys.path.append
+00004cc0: 2827 2e2e 2729 0a66 726f 6d20 7079 7465  ('..').from pyte
+00004cd0: 7874 636c 6173 7369 6669 6572 2e74 6578  xtclassifier.tex
+00004ce0: 7463 6c75 7374 6572 2069 6d70 6f72 7420  tcluster import 
+00004cf0: 5465 7874 436c 7573 7465 720a 0a69 6620  TextCluster..if 
+00004d00: 5f5f 6e61 6d65 5f5f 203d 3d20 275f 5f6d  __name__ == '__m
+00004d10: 6169 6e5f 5f27 3a0a 2020 2020 6d20 3d20  ain__':.    m = 
+00004d20: 5465 7874 436c 7573 7465 7228 6f75 7470  TextCluster(outp
+00004d30: 7574 5f64 6972 3d27 6d6f 6465 6c73 2f63  ut_dir='models/c
+00004d40: 6c75 7374 6572 2d74 6f79 272c 206e 5f63  luster-toy', n_c
+00004d50: 6c75 7374 6572 733d 3229 0a20 2020 2070  lusters=2).    p
+00004d60: 7269 6e74 286d 290a 2020 2020 6461 7461  rint(m).    data
+00004d70: 203d 205b 0a20 2020 2020 2020 2027 5374   = [.        'St
+00004d80: 7564 656e 7420 6465 6274 2074 6f20 636f  udent debt to co
+00004d90: 7374 2042 7269 7461 696e 2062 696c 6c69  st Britain billi
+00004da0: 6f6e 7320 7769 7468 696e 2064 6563 6164  ons within decad
+00004db0: 6573 272c 0a20 2020 2020 2020 2027 4368  es',.        'Ch
+00004dc0: 696e 6573 6520 6564 7563 6174 696f 6e20  inese education 
+00004dd0: 666f 7220 5456 2065 7870 6572 696d 656e  for TV experimen
+00004de0: 7427 2c0a 2020 2020 2020 2020 2741 6262  t',.        'Abb
+00004df0: 6f74 7420 676f 7665 726e 6d65 6e74 2073  ott government s
+00004e00: 7065 6e64 7320 2438 206d 696c 6c69 6f6e  pends $8 million
+00004e10: 206f 6e20 6869 6768 6572 2065 6475 6361   on higher educa
+00004e20: 7469 6f6e 272c 0a20 2020 2020 2020 2027  tion',.        '
+00004e30: 4d69 6464 6c65 2045 6173 7420 616e 6420  Middle East and 
+00004e40: 4173 6961 2062 6f6f 7374 2069 6e76 6573  Asia boost inves
+00004e50: 746d 656e 7420 696e 2074 6f70 206c 6576  tment in top lev
+00004e60: 656c 2073 706f 7274 7327 2c0a 2020 2020  el sports',.    
+00004e70: 2020 2020 2753 756d 6d69 7420 5365 7269      'Summit Seri
+00004e80: 6573 206c 6f6f 6b20 6c61 756e 6368 6573  es look launches
+00004e90: 2048 424f 2043 616e 6164 6120 7370 6f72   HBO Canada spor
+00004ea0: 7473 2064 6f63 2073 6572 6965 733a 204d  ts doc series: M
+00004eb0: 7564 6861 7227 0a20 2020 205d 0a20 2020  udhar'.    ].   
+00004ec0: 206d 2e74 7261 696e 2864 6174 6129 0a20   m.train(data). 
+00004ed0: 2020 206d 2e6c 6f61 645f 6d6f 6465 6c28     m.load_model(
+00004ee0: 290a 2020 2020 7220 3d20 6d2e 7072 6564  ).    r = m.pred
+00004ef0: 6963 7428 5b27 4162 626f 7474 2067 6f76  ict(['Abbott gov
+00004f00: 6572 6e6d 656e 7420 7370 656e 6473 2024  ernment spends $
+00004f10: 3820 6d69 6c6c 696f 6e20 6f6e 2068 6967  8 million on hig
+00004f20: 6865 7220 6564 7563 6174 696f 6e20 6d65  her education me
+00004f30: 6469 6120 626c 6974 7a27 2c0a 2020 2020  dia blitz',.    
+00004f40: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00004f50: 4d69 6464 6c65 2045 6173 7420 616e 6420  Middle East and 
+00004f60: 4173 6961 2062 6f6f 7374 2069 6e76 6573  Asia boost inves
+00004f70: 746d 656e 7420 696e 2074 6f70 206c 6576  tment in top lev
+00004f80: 656c 2073 706f 7274 7327 5d29 0a20 2020  el sports']).   
+00004f90: 2070 7269 6e74 2872 290a 0a20 2020 2023   print(r)..    #
+00004fa0: 2323 2323 2323 2323 2323 206c 6f61 6420  ########## load 
+00004fb0: 6368 696e 6573 6520 7472 6169 6e20 6461  chinese train da
+00004fc0: 7461 2066 726f 6d20 3177 2064 6174 6120  ta from 1w data 
+00004fd0: 6669 6c65 0a20 2020 2066 726f 6d20 736b  file.    from sk
+00004fe0: 6c65 6172 6e2e 6665 6174 7572 655f 6578  learn.feature_ex
+00004ff0: 7472 6163 7469 6f6e 2e74 6578 7420 696d  traction.text im
+00005000: 706f 7274 2054 6669 6466 5665 6374 6f72  port TfidfVector
+00005010: 697a 6572 0a0a 2020 2020 7463 6c75 7374  izer..    tclust
+00005020: 6572 203d 2054 6578 7443 6c75 7374 6572  er = TextCluster
+00005030: 286f 7574 7075 745f 6469 723d 276d 6f64  (output_dir='mod
+00005040: 656c 732f 636c 7573 7465 7227 2c20 6665  els/cluster', fe
+00005050: 6174 7572 653d 5466 6964 6656 6563 746f  ature=TfidfVecto
+00005060: 7269 7a65 7228 6e67 7261 6d5f 7261 6e67  rizer(ngram_rang
+00005070: 653d 2831 2c20 3229 292c 206e 5f63 6c75  e=(1, 2)), n_clu
+00005080: 7374 6572 733d 3130 290a 2020 2020 6461  sters=10).    da
+00005090: 7461 203d 2074 636c 7573 7465 722e 6c6f  ta = tcluster.lo
+000050a0: 6164 5f66 696c 655f 6461 7461 2827 7468  ad_file_data('th
+000050b0: 7563 6e65 7773 5f74 7261 696e 5f31 772e  ucnews_train_1w.
+000050c0: 7478 7427 2c20 7365 703d 275c 7427 2c20  txt', sep='\t', 
+000050d0: 7573 655f 636f 6c3d 3129 0a20 2020 2066  use_col=1).    f
+000050e0: 6561 7475 7265 2c20 6c61 6265 6c73 203d  eature, labels =
+000050f0: 2074 636c 7573 7465 722e 7472 6169 6e28   tcluster.train(
+00005100: 6461 7461 5b3a 3530 3030 5d29 0a20 2020  data[:5000]).   
+00005110: 2074 636c 7573 7465 722e 7368 6f77 5f63   tcluster.show_c
+00005120: 6c75 7374 6572 7328 6665 6174 7572 652c  lusters(feature,
+00005130: 206c 6162 656c 732c 2027 6d6f 6465 6c73   labels, 'models
+00005140: 2f63 6c75 7374 6572 2f63 6c75 7374 6572  /cluster/cluster
+00005150: 5f74 7261 696e 5f73 6567 5f73 616d 706c  _train_seg_sampl
+00005160: 6573 2e70 6e67 2729 0a20 2020 2072 203d  es.png').    r =
+00005170: 2074 636c 7573 7465 722e 7072 6564 6963   tcluster.predic
+00005180: 7428 6461 7461 5b3a 3330 5d29 0a20 2020  t(data[:30]).   
+00005190: 2070 7269 6e74 2872 290a 6060 600a 0a6f   print(r).```..o
+000051a0: 7574 7075 743a 0a0a 6060 600a 5465 7874  utput:..```.Text
+000051b0: 436c 7573 7465 7220 696e 7374 616e 6365  Cluster instance
+000051c0: 2028 4d69 6e69 4261 7463 684b 4d65 616e   (MiniBatchKMean
+000051d0: 7328 6e5f 636c 7573 7465 7273 3d32 2c20  s(n_clusters=2, 
+000051e0: 6e5f 696e 6974 3d31 3029 2c20 3c70 7974  n_init=10), <pyt
+000051f0: 6578 7463 6c61 7373 6966 6965 722e 7574  extclassifier.ut
+00005200: 696c 732e 746f 6b65 6e69 7a65 722e 546f  ils.tokenizer.To
+00005210: 6b65 6e69 7a65 7220 6f62 6a65 6374 2061  kenizer object a
+00005220: 7420 3078 3766 3830 6264 3436 3832 6230  t 0x7f80bd4682b0
+00005230: 3e2c 2054 6669 6466 5665 6374 6f72 697a  >, TfidfVectoriz
+00005240: 6572 286e 6772 616d 5f72 616e 6765 3d28  er(ngram_range=(
+00005250: 312c 2032 2929 290a 5b31 2031 2031 2031  1, 2))).[1 1 1 1
+00005260: 2031 2031 2031 2031 2031 2031 2031 2038   1 1 1 1 1 1 1 8
+00005270: 2031 2031 2031 2031 2031 2031 2031 2031   1 1 1 1 1 1 1 1
+00005280: 2031 2031 2039 2031 2031 2038 2031 2031   1 1 9 1 1 8 1 1
+00005290: 2039 2031 5d0a 6060 600a 636c 7573 7465   9 1].```.cluste
+000052a0: 7269 6e67 2070 6c6f 7420 696d 6167 653a  ring plot image:
+000052b0: 0a0a 215b 636c 7573 7465 725f 696d 6167  ..![cluster_imag
+000052c0: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
+000052d0: 622e 636f 6d2f 7368 6962 696e 6736 3234  b.com/shibing624
+000052e0: 2f70 7974 6578 7463 6c61 7373 6966 6965  /pytextclassifie
+000052f0: 722f 626c 6f62 2f6d 6173 7465 722f 646f  r/blob/master/do
+00005300: 6373 2f63 6c75 7374 6572 5f74 7261 696e  cs/cluster_train
+00005310: 5f73 6567 5f73 616d 706c 6573 2e70 6e67  _seg_samples.png
+00005320: 290a 0a0a 2323 2043 6f6e 7461 6374 0a0a  )...## Contact..
+00005330: 2d20 4973 7375 6528 e5bb bae8 aeae 29ef  - Issue(......).
+00005340: bc9a 5b21 5b47 6974 4875 6220 6973 7375  ..[![GitHub issu
+00005350: 6573 5d28 6874 7470 733a 2f2f 696d 672e  es](https://img.
+00005360: 7368 6965 6c64 732e 696f 2f67 6974 6875  shields.io/githu
+00005370: 622f 6973 7375 6573 2f73 6869 6269 6e67  b/issues/shibing
+00005380: 3632 342f 7079 7465 7874 636c 6173 7369  624/pytextclassi
+00005390: 6669 6572 2e73 7667 295d 2868 7474 7073  fier.svg)](https
+000053a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7368  ://github.com/sh
+000053b0: 6962 696e 6736 3234 2f70 7974 6578 7463  ibing624/pytextc
+000053c0: 6c61 7373 6966 6965 722f 6973 7375 6573  lassifier/issues
+000053d0: 290a 2d20 e982 aee4 bbb6 e688 91ef bc9a  ).- ............
+000053e0: 7875 6d69 6e67 3a20 7875 6d69 6e67 3632  xuming: xuming62
+000053f0: 3440 7171 2e63 6f6d 0a2d 20e5 beae e4bf  4@qq.com.- .....
+00005400: a1e6 8891 efbc 9ae5 8aa0 e688 912a e5be  .............*..
+00005410: aee4 bfa1 e58f b7ef bc9a 7875 6d69 6e67  ..........xuming
+00005420: 3632 342a 2c20 e8bf 9b50 7974 686f 6e2d  624*, ...Python-
+00005430: 4e4c 50e4 baa4 e6b5 81e7 bea4 efbc 8ce5  NLP.............
+00005440: a487 e6b3 a8ef bc9a 2ae5 a793 e590 8d2d  ........*......-
+00005450: e585 ace5 8fb8 e590 8d2d 4e4c 502a 0a3c  .........-NLP*.<
+00005460: 696d 6720 7372 633d 2264 6f63 732f 7765  img src="docs/we
+00005470: 6368 6174 2e6a 7065 6722 2077 6964 7468  chat.jpeg" width
+00005480: 3d22 3230 3022 202f 3e0a 0a0a 2323 2043  ="200" />...## C
+00005490: 6974 6174 696f 6e0a 0ae5 a682 e69e 9ce4  itation.........
+000054a0: bda0 e59c a8e7 a094 e7a9 b6e4 b8ad e4bd  ................
+000054b0: bfe7 94a8 e4ba 8670 7974 6578 7463 6c61  .......pytextcla
+000054c0: 7373 6966 6965 72ef bc8c e8af b7e6 8c89  ssifier.........
+000054d0: e5a6 82e4 b88b e6a0 bce5 bc8f e5bc 95e7  ................
+000054e0: 94a8 efbc 9a0a 0a41 5041 3a0a 6060 606c  .......APA:.```l
+000054f0: 6174 6578 0a58 752c 204d 2e20 5079 7465  atex.Xu, M. Pyte
+00005500: 7874 636c 6173 7369 6669 6572 3a20 5465  xtclassifier: Te
+00005510: 7874 2063 6c61 7373 6966 6965 7220 746f  xt classifier to
+00005520: 6f6c 6b69 7420 666f 7220 4e4c 5020 2856  olkit for NLP (V
+00005530: 6572 7369 6f6e 2031 2e32 2e30 2920 5b43  ersion 1.2.0) [C
+00005540: 6f6d 7075 7465 7220 736f 6674 7761 7265  omputer software
+00005550: 5d2e 2068 7474 7073 3a2f 2f67 6974 6875  ]. https://githu
+00005560: 622e 636f 6d2f 7368 6962 696e 6736 3234  b.com/shibing624
+00005570: 2f70 7974 6578 7463 6c61 7373 6966 6965  /pytextclassifie
+00005580: 720a 6060 600a 0a42 6962 5465 583a 0a60  r.```..BibTeX:.`
+00005590: 6060 6c61 7465 780a 406d 6973 637b 5079  ``latex.@misc{Py
+000055a0: 7465 7874 636c 6173 7369 6669 6572 2c0a  textclassifier,.
+000055b0: 2020 7469 746c 653d 7b50 7974 6578 7463    title={Pytextc
+000055c0: 6c61 7373 6966 6965 723a 2054 6578 7420  lassifier: Text 
+000055d0: 636c 6173 7369 6669 6572 2074 6f6f 6c6b  classifier toolk
+000055e0: 6974 2066 6f72 204e 4c50 7d2c 0a20 2061  it for NLP},.  a
+000055f0: 7574 686f 723d 7b58 7520 4d69 6e67 7d2c  uthor={Xu Ming},
+00005600: 0a20 2079 6561 723d 7b32 3032 327d 2c0a  .  year={2022},.
+00005610: 2020 686f 7770 7562 6c69 7368 6564 3d7b    howpublished={
+00005620: 5c75 726c 7b68 7474 7073 3a2f 2f67 6974  \url{https://git
+00005630: 6875 622e 636f 6d2f 7368 6962 696e 6736  hub.com/shibing6
+00005640: 3234 2f70 7974 6578 7463 6c61 7373 6966  24/pytextclassif
+00005650: 6965 727d 7d2c 0a7d 0a60 6060 0a0a 0a23  ier}},.}.```...#
+00005660: 2320 4c69 6365 6e73 650a 0a0a e68e 88e6  # License.......
+00005670: 9d83 e58d 8fe8 aeae e4b8 ba20 5b54 6865  ........... [The
+00005680: 2041 7061 6368 6520 4c69 6365 6e73 6520   Apache License 
+00005690: 322e 305d 284c 4943 454e 5345 29ef bc8c  2.0](LICENSE)...
+000056a0: e58f afe5 858d e8b4 b9e7 94a8 e581 9ae5  ................
+000056b0: 9586 e4b8 9ae7 94a8 e980 94e3 8082 e8af  ................
+000056c0: b7e5 9ca8 e4ba a7e5 9381 e8af b4e6 988e  ................
+000056d0: e4b8 ade9 9984 e58a a02a 2a70 7974 6578  .........**pytex
+000056e0: 7463 6c61 7373 6966 6965 722a 2ae7 9a84  tclassifier**...
+000056f0: e993 bee6 8ea5 e592 8ce6 8e88 e69d 83e5  ................
+00005700: 8d8f e8ae aee3 8082 0a0a 0a23 2320 436f  ...........## Co
+00005710: 6e74 7269 6275 7465 0ae9 a1b9 e79b aee4  ntribute........
+00005720: bba3 e7a0 81e8 bf98 e5be 88e7 b297 e7b3  ................
+00005730: 99ef bc8c e5a6 82e6 9e9c e5a4 a7e5 aeb6  ................
+00005740: e5af b9e4 bba3 e7a0 81e6 9c89 e689 80e6  ................
+00005750: 94b9 e8bf 9bef bc8c e6ac a2e8 bf8e e68f  ................
+00005760: 90e4 baa4 e59b 9ee6 9cac e9a1 b9e7 9bae  ................
+00005770: efbc 8ce5 9ca8 e68f 90e4 baa4 e4b9 8be5  ................
+00005780: 898d efbc 8ce6 b3a8 e684 8fe4 bba5 e4b8  ................
+00005790: 8be4 b8a4 e782 b9ef bc9a 0a0a 202d 20e5  ............ - .
+000057a0: 9ca8 6074 6573 7473 60e6 b7bb e58a a0e7  ..`tests`.......
+000057b0: 9bb8 e5ba 94e7 9a84 e58d 95e5 8583 e6b5  ................
+000057c0: 8be8 af95 0a20 2d20 e4bd bfe7 94a8 6070  ..... - ......`p
+000057d0: 7974 686f 6e20 7365 7475 702e 7079 2074  ython setup.py t
+000057e0: 6573 7460 e69d a5e8 bf90 e8a1 8ce6 8980  est`............
+000057f0: e69c 89e5 8d95 e585 83e6 b58b e8af 95ef  ................
+00005800: bc8c e7a1 aee4 bf9d e689 80e6 9c89 e58d  ................
+00005810: 95e6 b58b e983 bde6 98af e980 9ae8 bf87  ................
+00005820: e79a 840a 0ae4 b98b e590 8ee5 8db3 e58f  ................
+00005830: afe6 8f90 e4ba a450 52e3 8082 0a0a       .......PR.....
```

### Comparing `pytextclassifier-1.3.7/README.md` & `pytextclassifier-1.3.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,18 @@
 
 -----------------
 
 # PyTextClassifier: Python Text Classifier
 [![PyPI version](https://badge.fury.io/py/pytextclassifier.svg)](https://badge.fury.io/py/pytextclassifier)
 [![Downloads](https://static.pepy.tech/badge/pytextclassifier)](https://pepy.tech/project/pytextclassifier)
 [![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](CONTRIBUTING.md)
-[![GitHub contributors](https://img.shields.io/github/contributors/shibing624/pytextclassifier.svg)](https://github.com/shibing624/pytextclassifier/graphs/contributors)
 [![License Apache 2.0](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](LICENSE)
 [![python_vesion](https://img.shields.io/badge/Python-3.5%2B-green.svg)](requirements.txt)
 [![GitHub issues](https://img.shields.io/github/issues/shibing624/pytextclassifier.svg)](https://github.com/shibing624/pytextclassifier/issues)
-[![Wechat Group](http://vlog.sfyc.ltd/wechat_everyday/wxgroup_logo.png?imageView2/0/w/60/h/20)](#Contact)
+[![Wechat Group](https://img.shields.io/badge/wechat-group-green.svg?logo=wechat)](#Contact)
 
 
 ## Introduction
 PyTextClassifier: Python Text Classifier. It can be applied to the fields of sentiment polarity analysis, text risk classification and so on,
 and it supports multiple classification algorithms and clustering algorithms.
 
 **pytextclassifier** is a python Open Source Toolkit for text classification. The goal is to implement
```

### Comparing `pytextclassifier-1.3.7/examples/thucnews_train_1w.txt` & `pytextclassifier-1.3.8/examples/thucnews_train_1w.txt`

 * *Files identical despite different names*

### Comparing `pytextclassifier-1.3.7/pytextclassifier/__init__.py` & `pytextclassifier-1.3.8/pytextclassifier/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 @author:XuMing(xuming624@qq.com)
 @description: 
 """
-__version__ = '1.3.7'
+__version__ = '1.3.8'
 
 from pytextclassifier.classic_classifier import ClassicClassifier
 from pytextclassifier.fasttext_classifier import FastTextClassifier
 from pytextclassifier.textcnn_classifier import TextCNNClassifier
 from pytextclassifier.textrnn_classifier import TextRNNClassifier
 from pytextclassifier.bert_classifier import BertClassifier
 from pytextclassifier.base_classifier import load_data
```

### Comparing `pytextclassifier-1.3.7/pytextclassifier/base_classifier.py` & `pytextclassifier-1.3.8/pytextclassifier/base_classifier.py`

 * *Files identical despite different names*

### Comparing `pytextclassifier-1.3.7/pytextclassifier/bert_classfication_utils.py` & `pytextclassifier-1.3.8/pytextclassifier/bert_classfication_utils.py`

 * *Files identical despite different names*

### Comparing `pytextclassifier-1.3.7/pytextclassifier/bert_classification_model.py` & `pytextclassifier-1.3.8/pytextclassifier/bert_classification_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,14 @@
     get_constant_schedule,
     get_constant_schedule_with_warmup,
     get_linear_schedule_with_warmup,
     get_cosine_schedule_with_warmup,
     get_cosine_with_hard_restarts_schedule_with_warmup,
     get_polynomial_decay_schedule_with_warmup,
 )
-
 sys.path.append('..')
 from pytextclassifier.bert_classfication_utils import (
     BertClassificationArgs,
     InputExample,
     LazyClassificationDataset,
     ClassificationDataset,
     load_hf_dataset,
```

### Comparing `pytextclassifier-1.3.7/pytextclassifier/bert_classifier.py` & `pytextclassifier-1.3.8/pytextclassifier/bert_classifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,24 +109,34 @@
         @param test_size:
         @return:
         """
         logger.debug('train model ...')
         SEED = 1
         set_seed(SEED)
         # load data
-        X, y, data_df = load_data(data_list_or_path, header=header, names=names, delimiter=delimiter,
-                                  labels_sep=self.labels_sep, is_train=True)
+        X, y, data_df = load_data(
+            data_list_or_path,
+            header=header,
+            names=names,
+            delimiter=delimiter,
+            labels_sep=self.labels_sep,
+            is_train=True
+        )
         if self.output_dir:
             os.makedirs(self.output_dir, exist_ok=True)
         labels_map = self.build_labels_map(y, self.label_vocab_path, self.multi_label, self.labels_sep)
         labels_list = sorted(list(labels_map.keys()))
         if dev_data_list_or_path is not None:
-            dev_X, dev_y, dev_df = load_data(dev_data_list_or_path, header=header, names=names,
-                                             delimiter=delimiter, labels_sep=self.labels_sep,
-                                             is_train=False)
+            dev_X, dev_y, dev_df = load_data(
+                dev_data_list_or_path,
+                header=header, names=names,
+                delimiter=delimiter,
+                labels_sep=self.labels_sep,
+                is_train=False
+            )
             train_data = data_df
             dev_data = dev_df
         else:
             if test_size > 0:
                 train_data, dev_data = train_test_split(data_df, test_size=test_size, random_state=SEED)
             else:
                 train_data = data_df
@@ -167,46 +177,57 @@
             return predictions, raw_outputs
         else:
             # predict probability
             predict_probs = [1 - np.exp(-np.max(raw_output)) for raw_output, prediction in
                              zip(raw_outputs, predictions)]
             return predictions, predict_probs
 
-    def evaluate_model(self, data_list_or_path, header=None,
-                       names=('labels', 'text'), delimiter='\t', **kwargs):
+    def evaluate_model(
+            self,
+            data_list_or_path,
+            header=None,
+            names=('labels', 'text'),
+            delimiter='\t',
+            **kwargs
+    ):
         """
         Evaluate model with data_list_or_path
         @param data_list_or_path:
         @param header:
         @param names:
         @param delimiter:
         @param kwargs:
         @return:
         """
         if self.train_args.lazy_loading:
             eval_df = data_list_or_path
         else:
-            X_test, y_test, eval_df = load_data(data_list_or_path, header=header, names=names, delimiter=delimiter,
-                                                labels_sep=self.labels_sep)
+            X_test, y_test, eval_df = load_data(
+                data_list_or_path,
+                header=header,
+                names=names,
+                delimiter=delimiter,
+                labels_sep=self.labels_sep
+            )
         if not self.is_trained:
             self.load_model()
         result, model_outputs, wrong_predictions = self.model.eval_model(
             eval_df,
             output_dir=self.output_dir,
             **kwargs,
         )
         return result
 
     def load_model(self):
         """
         Load model from output_dir
         @return:
         """
-        model_path = os.path.join(self.output_dir, 'pytorch_model.bin')
-        if os.path.exists(model_path):
+        model_config_file = os.path.join(self.output_dir, 'config.json')
+        if os.path.exists(model_config_file):
             labels_map = json.load(open(self.label_vocab_path, 'r', encoding='utf-8'))
             labels_list = sorted(list(labels_map.keys()))
             num_classes = len(labels_map)
             assert num_classes == self.num_classes, f'num_classes not match, {num_classes} != {self.num_classes}'
             self.train_args.update_from_dict({'labels_map': labels_map, 'labels_list': labels_list})
             self.model = BertClassificationModel(
                 model_type=self.model_type,
@@ -214,15 +235,15 @@
                 num_labels=self.num_classes,
                 multi_label=self.multi_label,
                 args=self.train_args,
                 use_cuda=self.use_cuda,
             )
             self.is_trained = True
         else:
-            logger.error(f'{model_path} not exists.')
+            logger.error(f'{model_config_file} not exists.')
             self.is_trained = False
         return self.is_trained
 
     @staticmethod
     def build_labels_map(y, label_vocab_path, multi_label=False, labels_sep=','):
         """
         Build labels map
```

### Comparing `pytextclassifier-1.3.7/pytextclassifier/bert_multi_label_classification_model.py` & `pytextclassifier-1.3.8/pytextclassifier/bert_multi_label_classification_model.py`

 * *Files identical despite different names*

### Comparing `pytextclassifier-1.3.7/pytextclassifier/classic_classifier.py` & `pytextclassifier-1.3.8/pytextclassifier/classic_classifier.py`

 * *Files identical despite different names*

### Comparing `pytextclassifier-1.3.7/pytextclassifier/data_helper.py` & `pytextclassifier-1.3.8/pytextclassifier/data_helper.py`

 * *Files identical despite different names*

### Comparing `pytextclassifier-1.3.7/pytextclassifier/fasttext_classifier.py` & `pytextclassifier-1.3.8/pytextclassifier/fasttext_classifier.py`

 * *Files identical despite different names*

### Comparing `pytextclassifier-1.3.7/pytextclassifier/stopwords.txt` & `pytextclassifier-1.3.8/pytextclassifier/stopwords.txt`

 * *Files identical despite different names*

### Comparing `pytextclassifier-1.3.7/pytextclassifier/textcluster.py` & `pytextclassifier-1.3.8/pytextclassifier/textcluster.py`

 * *Files identical despite different names*

### Comparing `pytextclassifier-1.3.7/pytextclassifier/textcnn_classifier.py` & `pytextclassifier-1.3.8/pytextclassifier/textcnn_classifier.py`

 * *Files identical despite different names*

### Comparing `pytextclassifier-1.3.7/pytextclassifier/textrnn_classifier.py` & `pytextclassifier-1.3.8/pytextclassifier/textrnn_classifier.py`

 * *Files identical despite different names*

### Comparing `pytextclassifier-1.3.7/pytextclassifier/time_util.py` & `pytextclassifier-1.3.8/pytextclassifier/time_util.py`

 * *Files identical despite different names*

### Comparing `pytextclassifier-1.3.7/pytextclassifier/tokenizer.py` & `pytextclassifier-1.3.8/pytextclassifier/tokenizer.py`

 * *Files identical despite different names*

### Comparing `pytextclassifier-1.3.7/pytextclassifier.egg-info/PKG-INFO` & `pytextclassifier-1.3.8/pytextclassifier.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,1698 +1,1412 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7079 7465  : 2.1.Name: pyte
 00000020: 7874 636c 6173 7369 6669 6572 0a56 6572  xtclassifier.Ver
-00000030: 7369 6f6e 3a20 312e 332e 370a 5375 6d6d  sion: 1.3.7.Summ
+00000030: 7369 6f6e 3a20 312e 332e 380a 5375 6d6d  sion: 1.3.8.Summ
 00000040: 6172 793a 2054 6578 7420 436c 6173 7369  ary: Text Classi
 00000050: 6669 6572 2c20 5465 7874 2043 6c61 7373  fier, Text Class
 00000060: 6966 6963 6174 696f 6e0a 486f 6d65 2d70  ification.Home-p
 00000070: 6167 653a 2068 7474 7073 3a2f 2f67 6974  age: https://git
 00000080: 6875 622e 636f 6d2f 7368 6962 696e 6736  hub.com/shibing6
 00000090: 3234 2f70 7974 6578 7463 6c61 7373 6966  24/pytextclassif
 000000a0: 6965 720a 4175 7468 6f72 3a20 5875 4d69  ier.Author: XuMi
 000000b0: 6e67 0a41 7574 686f 722d 656d 6169 6c3a  ng.Author-email:
 000000c0: 2078 756d 696e 6736 3234 4071 712e 636f   xuming624@qq.co
 000000d0: 6d0a 4c69 6365 6e73 653a 2041 7061 6368  m.License: Apach
-000000e0: 6520 322e 300a 4465 7363 7269 7074 696f  e 2.0.Descriptio
-000000f0: 6e3a 203c 6469 7620 616c 6967 6e3d 2263  n: <div align="c
-00000100: 656e 7465 7222 3e0a 2020 2020 2020 2020  enter">.        
-00000110: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
-00000120: 3a2f 2f67 6974 6875 622e 636f 6d2f 7368  ://github.com/sh
-00000130: 6962 696e 6736 3234 2f70 7974 6578 7463  ibing624/pytextc
-00000140: 6c61 7373 6966 6965 7222 3e0a 2020 2020  lassifier">.    
-00000150: 2020 2020 2020 2020 3c69 6d67 2073 7263          <img src
-00000160: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
-00000170: 2e63 6f6d 2f73 6869 6269 6e67 3632 342f  .com/shibing624/
-00000180: 7079 7465 7874 636c 6173 7369 6669 6572  pytextclassifier
-00000190: 2f62 6c6f 622f 6d61 7374 6572 2f64 6f63  /blob/master/doc
-000001a0: 732f 6c6f 676f 2e70 6e67 2220 616c 743d  s/logo.png" alt=
-000001b0: 224c 6f67 6f22 2068 6569 6768 743d 2231  "Logo" height="1
-000001c0: 3536 223e 0a20 2020 2020 2020 2020 203c  56">.          <
-000001d0: 2f61 3e0a 2020 2020 2020 2020 3c2f 6469  /a>.        </di
-000001e0: 763e 0a20 2020 2020 2020 200a 2020 2020  v>.        .    
-000001f0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
-00000200: 2d2d 2d2d 2d0a 2020 2020 2020 2020 0a20  -----.        . 
-00000210: 2020 2020 2020 2023 2050 7954 6578 7443         # PyTextC
-00000220: 6c61 7373 6966 6965 723a 2050 7974 686f  lassifier: Pytho
-00000230: 6e20 5465 7874 2043 6c61 7373 6966 6965  n Text Classifie
-00000240: 720a 2020 2020 2020 2020 5b21 5b50 7950  r.        [![PyP
-00000250: 4920 7665 7273 696f 6e5d 2868 7474 7073  I version](https
-00000260: 3a2f 2f62 6164 6765 2e66 7572 792e 696f  ://badge.fury.io
-00000270: 2f70 792f 7079 7465 7874 636c 6173 7369  /py/pytextclassi
-00000280: 6669 6572 2e73 7667 295d 2868 7474 7073  fier.svg)](https
-00000290: 3a2f 2f62 6164 6765 2e66 7572 792e 696f  ://badge.fury.io
-000002a0: 2f70 792f 7079 7465 7874 636c 6173 7369  /py/pytextclassi
-000002b0: 6669 6572 290a 2020 2020 2020 2020 5b21  fier).        [!
-000002c0: 5b44 6f77 6e6c 6f61 6473 5d28 6874 7470  [Downloads](http
-000002d0: 733a 2f2f 7374 6174 6963 2e70 6570 792e  s://static.pepy.
-000002e0: 7465 6368 2f62 6164 6765 2f70 7974 6578  tech/badge/pytex
-000002f0: 7463 6c61 7373 6966 6965 7229 5d28 6874  tclassifier)](ht
-00000300: 7470 733a 2f2f 7065 7079 2e74 6563 682f  tps://pepy.tech/
-00000310: 7072 6f6a 6563 742f 7079 7465 7874 636c  project/pytextcl
-00000320: 6173 7369 6669 6572 290a 2020 2020 2020  assifier).      
-00000330: 2020 5b21 5b43 6f6e 7472 6962 7574 696f    [![Contributio
-00000340: 6e73 2077 656c 636f 6d65 5d28 6874 7470  ns welcome](http
-00000350: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000360: 696f 2f62 6164 6765 2f63 6f6e 7472 6962  io/badge/contrib
-00000370: 7574 696f 6e73 2d77 656c 636f 6d65 2d62  utions-welcome-b
-00000380: 7269 6768 7467 7265 656e 2e73 7667 295d  rightgreen.svg)]
-00000390: 2843 4f4e 5452 4942 5554 494e 472e 6d64  (CONTRIBUTING.md
-000003a0: 290a 2020 2020 2020 2020 5b21 5b47 6974  ).        [![Git
-000003b0: 4875 6220 636f 6e74 7269 6275 746f 7273  Hub contributors
-000003c0: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-000003d0: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
-000003e0: 636f 6e74 7269 6275 746f 7273 2f73 6869  contributors/shi
-000003f0: 6269 6e67 3632 342f 7079 7465 7874 636c  bing624/pytextcl
-00000400: 6173 7369 6669 6572 2e73 7667 295d 2868  assifier.svg)](h
-00000410: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000420: 6d2f 7368 6962 696e 6736 3234 2f70 7974  m/shibing624/pyt
-00000430: 6578 7463 6c61 7373 6966 6965 722f 6772  extclassifier/gr
-00000440: 6170 6873 2f63 6f6e 7472 6962 7574 6f72  aphs/contributor
-00000450: 7329 0a20 2020 2020 2020 205b 215b 4c69  s).        [![Li
-00000460: 6365 6e73 6520 4170 6163 6865 2032 2e30  cense Apache 2.0
-00000470: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-00000480: 6965 6c64 732e 696f 2f62 6164 6765 2f6c  ields.io/badge/l
-00000490: 6963 656e 7365 2d41 7061 6368 6525 3230  icense-Apache%20
-000004a0: 322e 302d 626c 7565 2e73 7667 295d 284c  2.0-blue.svg)](L
-000004b0: 4943 454e 5345 290a 2020 2020 2020 2020  ICENSE).        
-000004c0: 5b21 5b70 7974 686f 6e5f 7665 7369 6f6e  [![python_vesion
-000004d0: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-000004e0: 6965 6c64 732e 696f 2f62 6164 6765 2f50  ields.io/badge/P
-000004f0: 7974 686f 6e2d 332e 3525 3242 2d67 7265  ython-3.5%2B-gre
-00000500: 656e 2e73 7667 295d 2872 6571 7569 7265  en.svg)](require
-00000510: 6d65 6e74 732e 7478 7429 0a20 2020 2020  ments.txt).     
-00000520: 2020 205b 215b 4769 7448 7562 2069 7373     [![GitHub iss
-00000530: 7565 735d 2868 7474 7073 3a2f 2f69 6d67  ues](https://img
-00000540: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
-00000550: 7562 2f69 7373 7565 732f 7368 6962 696e  ub/issues/shibin
-00000560: 6736 3234 2f70 7974 6578 7463 6c61 7373  g624/pytextclass
-00000570: 6966 6965 722e 7376 6729 5d28 6874 7470  ifier.svg)](http
-00000580: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
-00000590: 6869 6269 6e67 3632 342f 7079 7465 7874  hibing624/pytext
-000005a0: 636c 6173 7369 6669 6572 2f69 7373 7565  classifier/issue
-000005b0: 7329 0a20 2020 2020 2020 205b 215b 5765  s).        [![We
-000005c0: 6368 6174 2047 726f 7570 5d28 6874 7470  chat Group](http
-000005d0: 3a2f 2f76 6c6f 672e 7366 7963 2e6c 7464  ://vlog.sfyc.ltd
-000005e0: 2f77 6563 6861 745f 6576 6572 7964 6179  /wechat_everyday
-000005f0: 2f77 7867 726f 7570 5f6c 6f67 6f2e 706e  /wxgroup_logo.pn
-00000600: 673f 696d 6167 6556 6965 7732 2f30 2f77  g?imageView2/0/w
-00000610: 2f36 302f 682f 3230 295d 2823 436f 6e74  /60/h/20)](#Cont
-00000620: 6163 7429 0a20 2020 2020 2020 200a 2020  act).        .  
-00000630: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
-00000640: 2320 496e 7472 6f64 7563 7469 6f6e 0a20  # Introduction. 
-00000650: 2020 2020 2020 2050 7954 6578 7443 6c61         PyTextCla
-00000660: 7373 6966 6965 723a 2050 7974 686f 6e20  ssifier: Python 
-00000670: 5465 7874 2043 6c61 7373 6966 6965 722e  Text Classifier.
-00000680: 2049 7420 6361 6e20 6265 2061 7070 6c69   It can be appli
-00000690: 6564 2074 6f20 7468 6520 6669 656c 6473  ed to the fields
-000006a0: 206f 6620 7365 6e74 696d 656e 7420 706f   of sentiment po
-000006b0: 6c61 7269 7479 2061 6e61 6c79 7369 732c  larity analysis,
-000006c0: 2074 6578 7420 7269 736b 2063 6c61 7373   text risk class
-000006d0: 6966 6963 6174 696f 6e20 616e 6420 736f  ification and so
-000006e0: 206f 6e2c 0a20 2020 2020 2020 2061 6e64   on,.        and
-000006f0: 2069 7420 7375 7070 6f72 7473 206d 756c   it supports mul
-00000700: 7469 706c 6520 636c 6173 7369 6669 6361  tiple classifica
-00000710: 7469 6f6e 2061 6c67 6f72 6974 686d 7320  tion algorithms 
-00000720: 616e 6420 636c 7573 7465 7269 6e67 2061  and clustering a
-00000730: 6c67 6f72 6974 686d 732e 0a20 2020 2020  lgorithms..     
-00000740: 2020 200a 2020 2020 2020 2020 2a2a 7079     .        **py
-00000750: 7465 7874 636c 6173 7369 6669 6572 2a2a  textclassifier**
-00000760: 2069 7320 6120 7079 7468 6f6e 204f 7065   is a python Ope
-00000770: 6e20 536f 7572 6365 2054 6f6f 6c6b 6974  n Source Toolkit
-00000780: 2066 6f72 2074 6578 7420 636c 6173 7369   for text classi
-00000790: 6669 6361 7469 6f6e 2e20 5468 6520 676f  fication. The go
-000007a0: 616c 2069 7320 746f 2069 6d70 6c65 6d65  al is to impleme
-000007b0: 6e74 0a20 2020 2020 2020 2074 6578 7420  nt.        text 
-000007c0: 616e 616c 7973 6973 2061 6c67 6f72 6974  analysis algorit
-000007d0: 686d 2c20 736f 2074 6f20 6163 6869 6576  hm, so to achiev
-000007e0: 6520 7468 6520 7573 6520 696e 2074 6865  e the use in the
-000007f0: 2070 726f 6475 6374 696f 6e20 656e 7669   production envi
-00000800: 726f 6e6d 656e 742e 0a20 2020 2020 2020  ronment..       
-00000810: 200a 2020 2020 2020 2020 e696 87e6 9cac   .        ......
-00000820: e588 86e7 b1bb e599 a8ef bc8c e68f 90e4  ................
-00000830: be9b e5a4 9ae7 a78d e696 87e6 9cac e588  ................
-00000840: 86e7 b1bb e592 8ce8 819a e7b1 bbe7 ae97  ................
-00000850: e6b3 95ef bc8c e694 afe6 8c81 e58f a5e5  ................
-00000860: ad90 e592 8ce6 9687 e6a1 a3e7 baa7 e79a  ................
-00000870: 84e6 9687 e69c ace5 8886 e7b1 bbe4 bbbb  ................
-00000880: e58a a1ef bc8c e694 afe6 8c81 e4ba 8ce5  ................
-00000890: 8886 e7b1 bbe3 8081 e5a4 9ae5 8886 e7b1  ................
-000008a0: bbe3 8081 e5a4 9ae6 a087 e7ad bee5 8886  ................
-000008b0: e7b1 bbe3 8081 e5a4 9ae5 b182 e7ba a7e5  ................
-000008c0: 8886 e7b1 bbe5 928c 4b6d 6561 6e73 e881  ........Kmeans..
-000008d0: 9ae7 b1bb efbc 8ce5 bc80 e7ae b1e5 8db3  ................
-000008e0: e794 a8e3 8082 7079 7468 6f6e 33e5 bc80  ......python3...
-000008f0: e58f 91e3 8082 0a20 2020 2020 2020 200a  .......        .
-00000900: 2020 2020 2020 2020 2a2a 4775 6964 652a          **Guide*
-00000910: 2a0a 2020 2020 2020 2020 0a20 2020 2020  *.        .     
-00000920: 2020 202d 205b 4665 6174 7572 655d 2823     - [Feature](#
-00000930: 4665 6174 7572 6529 0a20 2020 2020 2020  Feature).       
-00000940: 202d 205b 496e 7374 616c 6c5d 2823 696e   - [Install](#in
-00000950: 7374 616c 6c29 0a20 2020 2020 2020 202d  stall).        -
-00000960: 205b 5573 6167 655d 2823 7573 6167 6529   [Usage](#usage)
-00000970: 0a20 2020 2020 2020 202d 205b 4461 7461  .        - [Data
-00000980: 7365 745d 2823 4461 7461 7365 7429 0a20  set](#Dataset). 
-00000990: 2020 2020 2020 202d 205b 436f 6e74 6163         - [Contac
-000009a0: 745d 2823 436f 6e74 6163 7429 0a20 2020  t](#Contact).   
-000009b0: 2020 2020 202d 205b 4369 7461 7469 6f6e       - [Citation
-000009c0: 5d28 2343 6974 6174 696f 6e29 0a20 2020  ](#Citation).   
-000009d0: 2020 2020 202d 205b 5265 6665 7265 6e63       - [Referenc
-000009e0: 655d 2823 7265 6665 7265 6e63 6529 0a20  e](#reference). 
-000009f0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00000a00: 2323 2046 6561 7475 7265 0a20 2020 2020  ## Feature.     
-00000a10: 2020 200a 2020 2020 2020 2020 2a2a 7079     .        **py
-00000a20: 7465 7874 636c 6173 7369 6669 6572 2a2a  textclassifier**
-00000a30: 2068 6173 2074 6865 2063 6861 7261 6374   has the charact
-00000a40: 6572 6973 7469 6373 0a20 2020 2020 2020  eristics.       
-00000a50: 206f 6620 636c 6561 7220 616c 676f 7269   of clear algori
-00000a60: 7468 6d2c 2068 6967 6820 7065 7266 6f72  thm, high perfor
-00000a70: 6d61 6e63 6520 616e 6420 6375 7374 6f6d  mance and custom
-00000a80: 697a 6162 6c65 2063 6f72 7075 732e 0a20  izable corpus.. 
-00000a90: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00000aa0: 4675 6e63 7469 6f6e 73ef bc9a 0a20 2020  Functions....   
-00000ab0: 2020 2020 2023 2323 2043 6c61 7373 6966       ### Classif
-00000ac0: 6965 720a 2020 2020 2020 2020 2020 2d20  ier.          - 
-00000ad0: 5b78 5d20 4c6f 6769 7374 6963 5265 6772  [x] LogisticRegr
-00000ae0: 6573 7369 6f6e 0a20 2020 2020 2020 2020  ession.         
-00000af0: 202d 205b 785d 2052 616e 646f 6d20 466f   - [x] Random Fo
-00000b00: 7265 7374 0a20 2020 2020 2020 2020 202d  rest.          -
-00000b10: 205b 785d 2044 6563 6973 696f 6e20 5472   [x] Decision Tr
-00000b20: 6565 0a20 2020 2020 2020 2020 202d 205b  ee.          - [
-00000b30: 785d 204b 2d4e 6561 7265 7374 204e 6569  x] K-Nearest Nei
-00000b40: 6768 626f 7572 730a 2020 2020 2020 2020  ghbours.        
-00000b50: 2020 2d20 5b78 5d20 4e61 6976 6520 6261    - [x] Naive ba
-00000b60: 7965 730a 2020 2020 2020 2020 2020 2d20  yes.          - 
-00000b70: 5b78 5d20 5867 626f 6f73 740a 2020 2020  [x] Xgboost.    
-00000b80: 2020 2020 2020 2d20 5b78 5d20 5375 7070        - [x] Supp
-00000b90: 6f72 7420 5665 6374 6f72 204d 6163 6869  ort Vector Machi
-00000ba0: 6e65 2853 564d 290a 2020 2020 2020 2020  ne(SVM).        
-00000bb0: 2020 2d20 5b78 5d20 5465 7874 434e 4e0a    - [x] TextCNN.
-00000bc0: 2020 2020 2020 2020 2020 2d20 5b78 5d20            - [x] 
-00000bd0: 5465 7874 524e 4e0a 2020 2020 2020 2020  TextRNN.        
-00000be0: 2020 2d20 5b78 5d20 4661 7374 7465 7874    - [x] Fasttext
-00000bf0: 0a20 2020 2020 2020 2020 202d 205b 785d  .          - [x]
-00000c00: 2042 4552 540a 2020 2020 2020 2020 0a20   BERT.        . 
-00000c10: 2020 2020 2020 2023 2323 2043 6c75 7374         ### Clust
-00000c20: 6572 0a20 2020 2020 2020 2020 202d 205b  er.          - [
-00000c30: 785d 204d 696e 6942 6174 6368 4b6d 6561  x] MiniBatchKmea
-00000c40: 6e73 0a20 2020 2020 2020 200a 2020 2020  ns.        .    
-00000c50: 2020 2020 5768 696c 6520 7072 6f76 6964      While provid
-00000c60: 696e 6720 7269 6368 2066 756e 6374 696f  ing rich functio
-00000c70: 6e73 2c20 2a2a 7079 7465 7874 636c 6173  ns, **pytextclas
-00000c80: 7369 6669 6572 2a2a 2069 6e74 6572 6e61  sifier** interna
-00000c90: 6c20 6d6f 6475 6c65 7320 6164 6865 7265  l modules adhere
-00000ca0: 2074 6f20 6c6f 7720 636f 7570 6c69 6e67   to low coupling
-00000cb0: 2c20 6d6f 6465 6c20 6164 6865 7265 6e63  , model adherenc
-00000cc0: 6520 746f 2069 6e65 7274 206c 6f61 6469  e to inert loadi
-00000cd0: 6e67 2c20 6469 6374 696f 6e61 7279 2070  ng, dictionary p
-00000ce0: 7562 6c69 6361 7469 6f6e 2c20 616e 6420  ublication, and 
-00000cf0: 6561 7379 2074 6f20 7573 652e 0a20 2020  easy to use..   
-00000d00: 2020 2020 200a 2020 2020 2020 2020 2323       .        ##
-00000d10: 2049 6e73 7461 6c6c 0a20 2020 2020 2020   Install.       
-00000d20: 200a 2020 2020 2020 2020 2d20 5265 7175   .        - Requ
-00000d30: 6972 656d 656e 7473 2061 6e64 2049 6e73  irements and Ins
-00000d40: 7461 6c6c 6174 696f 6e0a 2020 2020 2020  tallation.      
-00000d50: 2020 0a20 2020 2020 2020 2060 6060 0a20    .        ```. 
-00000d60: 2020 2020 2020 2070 6970 3320 696e 7374         pip3 inst
-00000d70: 616c 6c20 746f 7263 6820 2320 636f 6e64  all torch # cond
-00000d80: 6120 696e 7374 616c 6c20 7079 746f 7263  a install pytorc
-00000d90: 680a 2020 2020 2020 2020 7069 7033 2069  h.        pip3 i
-00000da0: 6e73 7461 6c6c 2070 7974 6578 7463 6c61  nstall pytextcla
-00000db0: 7373 6966 6965 720a 2020 2020 2020 2020  ssifier.        
-00000dc0: 6060 600a 2020 2020 2020 2020 0a20 2020  ```.        .   
-00000dd0: 2020 2020 206f 720a 2020 2020 2020 2020       or.        
-00000de0: 0a20 2020 2020 2020 2060 6060 0a20 2020  .        ```.   
-00000df0: 2020 2020 2067 6974 2063 6c6f 6e65 2068       git clone h
-00000e00: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000e10: 6d2f 7368 6962 696e 6736 3234 2f70 7974  m/shibing624/pyt
-00000e20: 6578 7463 6c61 7373 6966 6965 722e 6769  extclassifier.gi
-00000e30: 740a 2020 2020 2020 2020 6364 2070 7974  t.        cd pyt
-00000e40: 6578 7463 6c61 7373 6966 6965 720a 2020  extclassifier.  
-00000e50: 2020 2020 2020 7079 7468 6f6e 3320 7365        python3 se
-00000e60: 7475 702e 7079 2069 6e73 7461 6c6c 0a20  tup.py install. 
-00000e70: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
-00000e80: 2020 200a 2020 2020 2020 2020 0a20 2020     .        .   
-00000e90: 2020 2020 2023 2320 5573 6167 650a 2020       ## Usage.  
-00000ea0: 2020 2020 2020 2323 2320 5465 7874 2043        ### Text C
-00000eb0: 6c61 7373 6966 6965 720a 2020 2020 2020  lassifier.      
-00000ec0: 2020 0a20 2020 2020 2020 2023 2323 2045    .        ### E
-00000ed0: 6e67 6c69 7368 2054 6578 7420 436c 6173  nglish Text Clas
-00000ee0: 7369 6669 6572 0a20 2020 2020 2020 200a  sifier.        .
-00000ef0: 2020 2020 2020 2020 496e 636c 7564 696e          Includin
-00000f00: 6720 6d6f 6465 6c20 7472 6169 6e69 6e67  g model training
-00000f10: 2c20 7361 7669 6e67 2c20 7072 6564 6963  , saving, predic
-00000f20: 742c 2065 7661 6c75 6174 652c 2066 6f72  t, evaluate, for
-00000f30: 2065 7861 6d70 6c65 205b 6578 616d 706c   example [exampl
-00000f40: 6573 2f6c 725f 656e 5f63 6c61 7373 6966  es/lr_en_classif
-00000f50: 6963 6174 696f 6e5f 6465 6d6f 2e70 795d  ication_demo.py]
-00000f60: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000f70: 636f 6d2f 7368 6962 696e 6736 3234 2f70  com/shibing624/p
-00000f80: 7974 6578 7463 6c61 7373 6966 6965 722f  ytextclassifier/
-00000f90: 626c 6f62 2f6d 6173 7465 722f 6578 616d  blob/master/exam
-00000fa0: 706c 6573 2f6c 725f 656e 5f63 6c61 7373  ples/lr_en_class
-00000fb0: 6966 6963 6174 696f 6e5f 6465 6d6f 2e70  ification_demo.p
-00000fc0: 7929 3a0a 2020 2020 2020 2020 0a20 2020  y):.        .   
-00000fd0: 2020 2020 2060 6060 7079 7468 6f6e 0a20       ```python. 
-00000fe0: 2020 2020 2020 2069 6d70 6f72 7420 7379         import sy
-00000ff0: 730a 2020 2020 2020 2020 0a20 2020 2020  s.        .     
-00001000: 2020 2073 7973 2e70 6174 682e 6170 7065     sys.path.appe
-00001010: 6e64 2827 2e2e 2729 0a20 2020 2020 2020  nd('..').       
-00001020: 2066 726f 6d20 7079 7465 7874 636c 6173   from pytextclas
-00001030: 7369 6669 6572 2069 6d70 6f72 7420 436c  sifier import Cl
-00001040: 6173 7369 6343 6c61 7373 6966 6965 720a  assicClassifier.
-00001050: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00001060: 2069 6620 5f5f 6e61 6d65 5f5f 203d 3d20   if __name__ == 
-00001070: 275f 5f6d 6169 6e5f 5f27 3a0a 2020 2020  '__main__':.    
-00001080: 2020 2020 2020 2020 6d20 3d20 436c 6173          m = Clas
-00001090: 7369 6343 6c61 7373 6966 6965 7228 6f75  sicClassifier(ou
-000010a0: 7470 7574 5f64 6972 3d27 6d6f 6465 6c73  tput_dir='models
-000010b0: 2f6c 7227 2c20 6d6f 6465 6c5f 6e61 6d65  /lr', model_name
-000010c0: 5f6f 725f 6d6f 6465 6c3d 276c 7227 290a  _or_model='lr').
-000010d0: 2020 2020 2020 2020 2020 2020 2320 436c              # Cl
-000010e0: 6173 7369 6343 6c61 7373 6966 6965 7220  assicClassifier 
-000010f0: 7375 7070 6f72 7420 6d6f 6465 6c5f 6e61  support model_na
-00001100: 6d65 efbc 9a6c 722c 2072 616e 646f 6d5f  me...lr, random_
-00001110: 666f 7265 7374 2c20 6465 6369 7369 6f6e  forest, decision
-00001120: 5f74 7265 652c 206b 6e6e 2c20 6261 7965  _tree, knn, baye
-00001130: 732c 2073 766d 2c20 7867 626f 6f73 740a  s, svm, xgboost.
-00001140: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00001150: 7428 6d29 0a20 2020 2020 2020 2020 2020  t(m).           
-00001160: 2064 6174 6120 3d20 5b0a 2020 2020 2020   data = [.      
-00001170: 2020 2020 2020 2020 2020 2827 6564 7563            ('educ
-00001180: 6174 696f 6e27 2c20 2753 7475 6465 6e74  ation', 'Student
-00001190: 2064 6562 7420 746f 2063 6f73 7420 4272   debt to cost Br
-000011a0: 6974 6169 6e20 6269 6c6c 696f 6e73 2077  itain billions w
-000011b0: 6974 6869 6e20 6465 6361 6465 7327 292c  ithin decades'),
-000011c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000011d0: 2028 2765 6475 6361 7469 6f6e 272c 2027   ('education', '
-000011e0: 4368 696e 6573 6520 6564 7563 6174 696f  Chinese educatio
-000011f0: 6e20 666f 7220 5456 2065 7870 6572 696d  n for TV experim
-00001200: 656e 7427 292c 0a20 2020 2020 2020 2020  ent'),.         
-00001210: 2020 2020 2020 2028 2773 706f 7274 7327         ('sports'
-00001220: 2c20 274d 6964 646c 6520 4561 7374 2061  , 'Middle East a
-00001230: 6e64 2041 7369 6120 626f 6f73 7420 696e  nd Asia boost in
-00001240: 7665 7374 6d65 6e74 2069 6e20 746f 7020  vestment in top 
-00001250: 6c65 7665 6c20 7370 6f72 7473 2729 2c0a  level sports'),.
-00001260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001270: 2827 7370 6f72 7473 272c 2027 5375 6d6d  ('sports', 'Summ
-00001280: 6974 2053 6572 6965 7320 6c6f 6f6b 206c  it Series look l
-00001290: 6175 6e63 6865 7320 4842 4f20 4361 6e61  aunches HBO Cana
-000012a0: 6461 2073 706f 7274 7320 646f 6320 7365  da sports doc se
-000012b0: 7269 6573 3a20 4d75 6468 6172 2729 0a20  ries: Mudhar'). 
-000012c0: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
-000012d0: 2020 2020 2020 2020 2023 2074 7261 696e           # train
-000012e0: 2061 6e64 2073 6176 6520 6265 7374 206d   and save best m
-000012f0: 6f64 656c 0a20 2020 2020 2020 2020 2020  odel.           
-00001300: 206d 2e74 7261 696e 2864 6174 6129 0a20   m.train(data). 
-00001310: 2020 2020 2020 2020 2020 2023 206c 6f61             # loa
-00001320: 6420 6265 7374 206d 6f64 656c 2066 726f  d best model fro
-00001330: 6d20 6d6f 6465 6c5f 6469 720a 2020 2020  m model_dir.    
-00001340: 2020 2020 2020 2020 6d2e 6c6f 6164 5f6d          m.load_m
-00001350: 6f64 656c 2829 0a20 2020 2020 2020 2020  odel().         
-00001360: 2020 2070 7265 6469 6374 5f6c 6162 656c     predict_label
-00001370: 2c20 7072 6564 6963 745f 7072 6f62 6120  , predict_proba 
-00001380: 3d20 6d2e 7072 6564 6963 7428 5b0a 2020  = m.predict([.  
-00001390: 2020 2020 2020 2020 2020 2020 2020 2741                'A
-000013a0: 6262 6f74 7420 676f 7665 726e 6d65 6e74  bbott government
-000013b0: 2073 7065 6e64 7320 2438 206d 696c 6c69   spends $8 milli
-000013c0: 6f6e 206f 6e20 6869 6768 6572 2065 6475  on on higher edu
-000013d0: 6361 7469 6f6e 206d 6564 6961 2062 6c69  cation media bli
-000013e0: 747a 275d 290a 2020 2020 2020 2020 2020  tz']).          
-000013f0: 2020 7072 696e 7428 6627 7072 6564 6963    print(f'predic
-00001400: 745f 6c61 6265 6c3a 207b 7072 6564 6963  t_label: {predic
-00001410: 745f 6c61 6265 6c7d 2c20 7072 6564 6963  t_label}, predic
-00001420: 745f 7072 6f62 613a 207b 7072 6564 6963  t_proba: {predic
-00001430: 745f 7072 6f62 617d 2729 0a20 2020 2020  t_proba}').     
-00001440: 2020 200a 2020 2020 2020 2020 2020 2020     .            
-00001450: 7465 7374 5f64 6174 6120 3d20 5b0a 2020  test_data = [.  
-00001460: 2020 2020 2020 2020 2020 2020 2020 2827                ('
-00001470: 6564 7563 6174 696f 6e27 2c20 2741 6262  education', 'Abb
-00001480: 6f74 7420 676f 7665 726e 6d65 6e74 2073  ott government s
-00001490: 7065 6e64 7320 2438 206d 696c 6c69 6f6e  pends $8 million
-000014a0: 206f 6e20 6869 6768 6572 2065 6475 6361   on higher educa
-000014b0: 7469 6f6e 206d 6564 6961 2062 6c69 747a  tion media blitz
-000014c0: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
-000014d0: 2020 2020 2827 7370 6f72 7473 272c 2027      ('sports', '
-000014e0: 4d69 6464 6c65 2045 6173 7420 616e 6420  Middle East and 
-000014f0: 4173 6961 2062 6f6f 7374 2069 6e76 6573  Asia boost inves
-00001500: 746d 656e 7420 696e 2074 6f70 206c 6576  tment in top lev
-00001510: 656c 2073 706f 7274 7327 292c 0a20 2020  el sports'),.   
-00001520: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
-00001530: 2020 2020 2020 2061 6363 5f73 636f 7265         acc_score
-00001540: 203d 206d 2e65 7661 6c75 6174 655f 6d6f   = m.evaluate_mo
-00001550: 6465 6c28 7465 7374 5f64 6174 6129 0a20  del(test_data). 
-00001560: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00001570: 2866 2761 6363 5f73 636f 7265 3a20 7b61  (f'acc_score: {a
-00001580: 6363 5f73 636f 7265 7d27 290a 2020 2020  cc_score}').    
-00001590: 2020 2020 6060 600a 2020 2020 2020 2020      ```.        
-000015a0: 0a20 2020 2020 2020 206f 7574 7075 743a  .        output:
-000015b0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-000015c0: 2020 6060 600a 2020 2020 2020 2020 436c    ```.        Cl
-000015d0: 6173 7369 6343 6c61 7373 6966 6965 7220  assicClassifier 
-000015e0: 696e 7374 616e 6365 2028 4c6f 6769 7374  instance (Logist
-000015f0: 6963 5265 6772 6573 7369 6f6e 2866 6974  icRegression(fit
-00001600: 5f69 6e74 6572 6365 7074 3d46 616c 7365  _intercept=False
-00001610: 292c 2073 746f 7077 6f72 6473 2073 697a  ), stopwords siz
-00001620: 653a 2032 3433 3829 0a20 2020 2020 2020  e: 2438).       
-00001630: 2070 7265 6469 6374 5f6c 6162 656c 3a20   predict_label: 
-00001640: 5b27 6564 7563 6174 696f 6e27 5d2c 2070  ['education'], p
-00001650: 7265 6469 6374 5f70 726f 6261 3a20 5b30  redict_proba: [0
-00001660: 2e35 3337 3832 3336 3335 3834 3932 3131  .537823635849211
-00001670: 325d 0a20 2020 2020 2020 2061 6363 5f73  2].        acc_s
-00001680: 636f 7265 3a20 312e 300a 2020 2020 2020  core: 1.0.      
-00001690: 2020 6060 600a 2020 2020 2020 2020 0a20    ```.        . 
-000016a0: 2020 2020 2020 2023 2323 2043 6869 6e65         ### Chine
-000016b0: 7365 2054 6578 7420 436c 6173 7369 6669  se Text Classifi
-000016c0: 6572 28e4 b8ad e696 87e6 9687 e69c ace5  er(.............
-000016d0: 8886 e7b1 bb29 0a20 2020 2020 2020 200a  .....).        .
-000016e0: 2020 2020 2020 2020 5465 7874 2063 6c61          Text cla
-000016f0: 7373 6966 6963 6174 696f 6e20 636f 6d70  ssification comp
-00001700: 6174 6962 6c65 2077 6974 6820 4368 696e  atible with Chin
-00001710: 6573 6520 616e 6420 456e 676c 6973 6820  ese and English 
-00001720: 636f 7270 6f72 612e 0a20 2020 2020 2020  corpora..       
-00001730: 200a 2020 2020 2020 2020 6578 616d 706c   .        exampl
-00001740: 6520 5b65 7861 6d70 6c65 732f 6c72 5f63  e [examples/lr_c
-00001750: 6c61 7373 6966 6963 6174 696f 6e5f 6465  lassification_de
-00001760: 6d6f 2e70 795d 2868 7474 7073 3a2f 2f67  mo.py](https://g
-00001770: 6974 6875 622e 636f 6d2f 7368 6962 696e  ithub.com/shibin
-00001780: 6736 3234 2f70 7974 6578 7463 6c61 7373  g624/pytextclass
-00001790: 6966 6965 722f 626c 6f62 2f6d 6173 7465  ifier/blob/maste
-000017a0: 722f 6578 616d 706c 6573 2f6c 725f 636c  r/examples/lr_cl
-000017b0: 6173 7369 6669 6361 7469 6f6e 5f64 656d  assification_dem
-000017c0: 6f2e 7079 290a 2020 2020 2020 2020 0a20  o.py).        . 
-000017d0: 2020 2020 2020 2060 6060 7079 7468 6f6e         ```python
-000017e0: 0a20 2020 2020 2020 2069 6d70 6f72 7420  .        import 
-000017f0: 7379 730a 2020 2020 2020 2020 0a20 2020  sys.        .   
-00001800: 2020 2020 2073 7973 2e70 6174 682e 6170       sys.path.ap
-00001810: 7065 6e64 2827 2e2e 2729 0a20 2020 2020  pend('..').     
-00001820: 2020 2066 726f 6d20 7079 7465 7874 636c     from pytextcl
-00001830: 6173 7369 6669 6572 2069 6d70 6f72 7420  assifier import 
-00001840: 436c 6173 7369 6343 6c61 7373 6966 6965  ClassicClassifie
-00001850: 720a 2020 2020 2020 2020 0a20 2020 2020  r.        .     
-00001860: 2020 2069 6620 5f5f 6e61 6d65 5f5f 203d     if __name__ =
-00001870: 3d20 275f 5f6d 6169 6e5f 5f27 3a0a 2020  = '__main__':.  
-00001880: 2020 2020 2020 2020 2020 6d20 3d20 436c            m = Cl
-00001890: 6173 7369 6343 6c61 7373 6966 6965 7228  assicClassifier(
-000018a0: 6f75 7470 7574 5f64 6972 3d27 6d6f 6465  output_dir='mode
-000018b0: 6c73 2f6c 722d 746f 7927 2c20 6d6f 6465  ls/lr-toy', mode
-000018c0: 6c5f 6e61 6d65 5f6f 725f 6d6f 6465 6c3d  l_name_or_model=
-000018d0: 276c 7227 290a 2020 2020 2020 2020 2020  'lr').          
-000018e0: 2020 2320 e7bb 8fe5 85b8 e588 86e7 b1bb    # ............
-000018f0: e696 b9e6 b395 efbc 8ce6 94af e68c 81e7  ................
-00001900: 9a84 e6a8 a1e5 9e8b e58c 85e6 8bac efbc  ................
-00001910: 9a6c 722c 2072 616e 646f 6d5f 666f 7265  .lr, random_fore
-00001920: 7374 2c20 6465 6369 7369 6f6e 5f74 7265  st, decision_tre
-00001930: 652c 206b 6e6e 2c20 6261 7965 732c 2073  e, knn, bayes, s
-00001940: 766d 2c20 7867 626f 6f73 740a 2020 2020  vm, xgboost.    
-00001950: 2020 2020 2020 2020 6461 7461 203d 205b          data = [
-00001960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001970: 2028 2765 6475 6361 7469 6f6e 272c 2027   ('education', '
-00001980: e590 8de5 b888 e68c 87e5 afbc e689 98e7  ................
-00001990: a68f e8af ade6 b395 e68a 80e5 b7a7 efbc  ................
-000019a0: 9ae5 908d e8af 8de7 9a84 e5a4 8de6 95b0  ................
-000019b0: e5bd a2e5 bc8f 2729 2c0a 2020 2020 2020  ......'),.      
-000019c0: 2020 2020 2020 2020 2020 2827 6564 7563            ('educ
-000019d0: 6174 696f 6e27 2c20 27e4 b8ad e59b bde9  ation', '.......
-000019e0: ab98 e880 83e6 8890 e7bb a9e6 b5b7 e5a4  ................
-000019f0: 96e8 aea4 e58f af20 e698 afe2 809c e78b  ....... ........
-00001a00: bce6 9da5 e4ba 86e2 809d e590 97ef bc9f  ................
-00001a10: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
-00001a20: 2020 2020 2827 6564 7563 6174 696f 6e27      ('education'
-00001a30: 2c20 27e5 85ac e58a a1e5 9198 e880 83e8  , '.............
-00001a40: 9991 e8b6 8ae6 9da5 e8b6 8ae5 9083 e9a6  ................
-00001a50: 99ef bc8c e8bf 99e6 98af e680 8ee4 b988  ................
-00001a60: e59b 9ee4 ba8b efbc 9f27 292c 0a20 2020  .........'),.   
-00001a70: 2020 2020 2020 2020 2020 2020 2028 2773               ('s
-00001a80: 706f 7274 7327 2c20 27e5 9bbe e696 87ef  ports', '.......
-00001a90: bc9a e6b3 95e7 bd91 e5ad 9fe8 8fb2 e5b0  ................
-00001aa0: 94e6 96af e88b a6e6 8898 e8bf 9b31 36e5  .............16.
-00001ab0: bcba 20e5 ad9f e88f b2e5 b094 e696 afe6  .. .............
-00001ac0: 8092 e590 bc27 292c 0a20 2020 2020 2020  .....'),.       
-00001ad0: 2020 2020 2020 2020 2028 2773 706f 7274           ('sport
-00001ae0: 7327 2c20 27e5 9b9b e5b7 9de4 b8b9 e6a3  s', '...........
-00001af0: b1e4 b8be e8a1 8ce5 85a8 e59b bde9 95bf  ................
-00001b00: e8b7 9de7 99bb e5b1 b1e6 8c91 e688 98e8  ................
-00001b10: b59b 20e8 bf91 e4b8 87e4 baba e58f 82e4  .. .............
-00001b20: b88e 2729 2c0a 2020 2020 2020 2020 2020  ..'),.          
-00001b30: 2020 2020 2020 2827 7370 6f72 7473 272c        ('sports',
-00001b40: 2027 e7b1 b3e5 85b0 e5ae a2e5 9cba 38e6   '............8.
-00001b50: 8898 e4b8 8de8 b4a5 e59b bde7 b1b3 3130  ..............10
-00001b60: e5b9 b4e8 bf9e e883 9c27 292c 0a20 2020  .........'),.   
-00001b70: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
-00001b80: 2020 2020 2020 206d 2e74 7261 696e 2864         m.train(d
-00001b90: 6174 6129 0a20 2020 2020 2020 2020 2020  ata).           
-00001ba0: 2070 7269 6e74 286d 290a 2020 2020 2020   print(m).      
-00001bb0: 2020 2020 2020 2320 6c6f 6164 2062 6573        # load bes
-00001bc0: 7420 6d6f 6465 6c20 6672 6f6d 206d 6f64  t model from mod
-00001bd0: 656c 5f64 6972 0a20 2020 2020 2020 2020  el_dir.         
-00001be0: 2020 206d 2e6c 6f61 645f 6d6f 6465 6c28     m.load_model(
-00001bf0: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
-00001c00: 6564 6963 745f 6c61 6265 6c2c 2070 7265  edict_label, pre
-00001c10: 6469 6374 5f70 726f 6261 203d 206d 2e70  dict_proba = m.p
-00001c20: 7265 6469 6374 285b 27e7 a68f e5bb bae6  redict(['.......
-00001c30: 98a5 e5ad a3e5 85ac e58a a1e5 9198 e880  ................
-00001c40: 83e8 af95 e68a a5e5 908d 3138 e697 a5e6  ..........18....
-00001c50: 88aa e6ad a220 32e6 9c88 36e6 97a5 e880  ..... 2...6.....
-00001c60: 83e8 af95 272c 0a20 2020 2020 2020 2020  ....',.         
-00001c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c90: 2020 2020 2020 2020 2020 2020 2027 e684               '..
-00001ca0: 8fe7 94b2 e9a6 96e8 bdae e8a1 a5e8 b59b  ................
-00001cb0: e4ba a4e6 8898 e8ae b0e5 bd95 3ae7 b1b3  ............:...
-00001cc0: e585 b0e5 aea2 e59c ba38 e688 98e4 b88d  .........8......
-00001cd0: e8b4 a5e5 9bbd e7b1 b331 30e5 b9b4 e8bf  .........10.....
-00001ce0: 9ee8 839c 275d 290a 2020 2020 2020 2020  ....']).        
-00001cf0: 2020 2020 7072 696e 7428 6627 7072 6564      print(f'pred
-00001d00: 6963 745f 6c61 6265 6c3a 207b 7072 6564  ict_label: {pred
-00001d10: 6963 745f 6c61 6265 6c7d 2c20 7072 6564  ict_label}, pred
-00001d20: 6963 745f 7072 6f62 613a 207b 7072 6564  ict_proba: {pred
-00001d30: 6963 745f 7072 6f62 617d 2729 0a20 2020  ict_proba}').   
-00001d40: 2020 2020 200a 2020 2020 2020 2020 2020       .          
-00001d50: 2020 7465 7374 5f64 6174 6120 3d20 5b0a    test_data = [.
-00001d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d70: 2827 6564 7563 6174 696f 6e27 2c20 27e7  ('education', '.
-00001d80: a68f e5bb bae6 98a5 e5ad a3e5 85ac e58a  ................
-00001d90: a1e5 9198 e880 83e8 af95 e68a a5e5 908d  ................
-00001da0: 3138 e697 a5e6 88aa e6ad a220 32e6 9c88  18......... 2...
-00001db0: 36e6 97a5 e880 83e8 af95 2729 2c0a 2020  6.........'),.  
-00001dc0: 2020 2020 2020 2020 2020 2020 2020 2827                ('
-00001dd0: 7370 6f72 7473 272c 2027 e684 8fe7 94b2  sports', '......
-00001de0: e9a6 96e8 bdae e8a1 a5e8 b59b e4ba a4e6  ................
-00001df0: 8898 e8ae b0e5 bd95 3ae7 b1b3 e585 b0e5  ........:.......
-00001e00: aea2 e59c ba38 e688 98e4 b88d e8b4 a5e5  .....8..........
-00001e10: 9bbd e7b1 b331 30e5 b9b4 e8bf 9ee8 839c  .....10.........
-00001e20: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
-00001e30: 5d0a 2020 2020 2020 2020 2020 2020 6163  ].            ac
-00001e40: 635f 7363 6f72 6520 3d20 6d2e 6576 616c  c_score = m.eval
-00001e50: 7561 7465 5f6d 6f64 656c 2874 6573 745f  uate_model(test_
-00001e60: 6461 7461 290a 2020 2020 2020 2020 2020  data).          
-00001e70: 2020 7072 696e 7428 6627 6163 635f 7363    print(f'acc_sc
-00001e80: 6f72 653a 207b 6163 635f 7363 6f72 657d  ore: {acc_score}
-00001e90: 2729 2020 2320 312e 300a 2020 2020 2020  ')  # 1.0.      
-00001ea0: 2020 0a20 2020 2020 2020 2020 2020 2023    .            #
-00001eb0: 2323 2320 7472 6169 6e20 6d6f 6465 6c20  ### train model 
-00001ec0: 7769 7468 2031 7720 6461 7461 0a20 2020  with 1w data.   
-00001ed0: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
-00001ee0: 2d27 202a 2034 3229 0a20 2020 2020 2020  -' * 42).       
-00001ef0: 2020 2020 206d 203d 2043 6c61 7373 6963       m = Classic
-00001f00: 436c 6173 7369 6669 6572 286f 7574 7075  Classifier(outpu
-00001f10: 745f 6469 723d 276d 6f64 656c 732f 6c72  t_dir='models/lr
-00001f20: 272c 206d 6f64 656c 5f6e 616d 655f 6f72  ', model_name_or
-00001f30: 5f6d 6f64 656c 3d27 6c72 2729 0a20 2020  _model='lr').   
-00001f40: 2020 2020 2020 2020 2064 6174 615f 6669           data_fi
-00001f50: 6c65 203d 2027 7468 7563 6e65 7773 5f74  le = 'thucnews_t
-00001f60: 7261 696e 5f31 772e 7478 7427 0a20 2020  rain_1w.txt'.   
-00001f70: 2020 2020 2020 2020 206d 2e74 7261 696e           m.train
-00001f80: 2864 6174 615f 6669 6c65 290a 2020 2020  (data_file).    
-00001f90: 2020 2020 2020 2020 6d2e 6c6f 6164 5f6d          m.load_m
-00001fa0: 6f64 656c 2829 0a20 2020 2020 2020 2020  odel().         
-00001fb0: 2020 2070 7265 6469 6374 5f6c 6162 656c     predict_label
-00001fc0: 2c20 7072 6564 6963 745f 7072 6f62 6120  , predict_proba 
-00001fd0: 3d20 6d2e 7072 6564 6963 7428 0a20 2020  = m.predict(.   
-00001fe0: 2020 2020 2020 2020 2020 2020 205b 27e9               ['.
-00001ff0: a1ba e4b9 89e5 8c97 e4ba ace8 8b8f e6b4  ................
-00002000: bb38 38e5 b9b3 e7b1 b3e8 b5b7 e7b2 bee8  .88.............
-00002010: a385 e688 bfe5 9ca8 e594 ae27 2c0a 2020  ...........',.  
-00002020: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00002030: e7be 8e45 422d 35e9 a1b9 e79b aee2 809c  ...EB-5.........
-00002040: 3135 e697 a5e5 bfab e980 9fe7 a7bb e6b0  15..............
-00002050: 91e2 809d e5b0 86e6 8ea8 e8bf 9f27 5d29  .............'])
-00002060: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00002070: 6e74 2866 2770 7265 6469 6374 5f6c 6162  nt(f'predict_lab
-00002080: 656c 3a20 7b70 7265 6469 6374 5f6c 6162  el: {predict_lab
-00002090: 656c 7d2c 2070 7265 6469 6374 5f70 726f  el}, predict_pro
-000020a0: 6261 3a20 7b70 7265 6469 6374 5f70 726f  ba: {predict_pro
-000020b0: 6261 7d27 290a 2020 2020 2020 2020 6060  ba}').        ``
-000020c0: 600a 2020 2020 2020 2020 0a20 2020 2020  `.        .     
-000020d0: 2020 206f 7574 7075 743a 0a20 2020 2020     output:.     
-000020e0: 2020 200a 2020 2020 2020 2020 6060 600a     .        ```.
-000020f0: 2020 2020 2020 2020 436c 6173 7369 6343          ClassicC
-00002100: 6c61 7373 6966 6965 7220 696e 7374 616e  lassifier instan
-00002110: 6365 2028 4c6f 6769 7374 6963 5265 6772  ce (LogisticRegr
-00002120: 6573 7369 6f6e 2866 6974 5f69 6e74 6572  ession(fit_inter
-00002130: 6365 7074 3d46 616c 7365 292c 2073 746f  cept=False), sto
-00002140: 7077 6f72 6473 2073 697a 653a 2032 3433  pwords size: 243
-00002150: 3829 0a20 2020 2020 2020 2070 7265 6469  8).        predi
-00002160: 6374 5f6c 6162 656c 3a20 5b27 6564 7563  ct_label: ['educ
-00002170: 6174 696f 6e27 2027 7370 6f72 7473 275d  ation' 'sports']
-00002180: 2c20 7072 6564 6963 745f 7072 6f62 613a  , predict_proba:
-00002190: 205b 302e 352c 2030 2e35 3938 3934 3138   [0.5, 0.5989418
-000021a0: 3036 3734 3135 3334 5d0a 2020 2020 2020  06741534].      
-000021b0: 2020 6163 635f 7363 6f72 653a 2031 2e30    acc_score: 1.0
-000021c0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-000021d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000021e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000021f0: 2d2d 2d0a 2020 2020 2020 2020 7072 6564  ---.        pred
-00002200: 6963 745f 6c61 6265 6c3a 205b 2772 6561  ict_label: ['rea
-00002210: 6c74 7927 2027 6564 7563 6174 696f 6e27  lty' 'education'
-00002220: 5d2c 2070 7265 6469 6374 5f70 726f 6261  ], predict_proba
-00002230: 3a20 5b30 2e37 3330 3239 3536 3932 3336  : [0.73029569236
-00002240: 3137 3337 322c 2030 2e32 3536 3530 3035  17372, 0.2565005
-00002250: 3434 3533 3232 3932 335d 0a20 2020 2020  445322923].     
-00002260: 2020 2060 6060 0a20 2020 2020 2020 200a     ```.        .
-00002270: 2020 2020 2020 2020 2323 2320 5669 7375          ### Visu
-00002280: 616c 2046 6561 7475 7265 2049 6d70 6f72  al Feature Impor
-00002290: 7461 6e63 650a 2020 2020 2020 2020 0a20  tance.        . 
-000022a0: 2020 2020 2020 2053 686f 7720 6665 6174         Show feat
-000022b0: 7572 6520 7765 6967 6874 7320 6f66 206d  ure weights of m
-000022c0: 6f64 656c 2c20 616e 6420 7072 6564 6963  odel, and predic
-000022d0: 7469 6f6e 2077 6f72 6420 7765 6967 6874  tion word weight
-000022e0: 2c20 666f 7220 6578 616d 706c 6520 5b65  , for example [e
-000022f0: 7861 6d70 6c65 732f 7669 7375 616c 5f66  xamples/visual_f
-00002300: 6561 7475 7265 5f69 6d70 6f72 7461 6e63  eature_importanc
-00002310: 652e 6970 796e 625d 2868 7474 7073 3a2f  e.ipynb](https:/
-00002320: 2f67 6974 6875 622e 636f 6d2f 7368 6962  /github.com/shib
-00002330: 696e 6736 3234 2f70 7974 6578 7463 6c61  ing624/pytextcla
-00002340: 7373 6966 6965 722f 626c 6f62 2f6d 6173  ssifier/blob/mas
-00002350: 7465 722f 6578 616d 706c 6573 2f76 6973  ter/examples/vis
-00002360: 7561 6c5f 6665 6174 7572 655f 696d 706f  ual_feature_impo
-00002370: 7274 616e 6365 2e69 7079 6e62 290a 2020  rtance.ipynb).  
-00002380: 2020 2020 2020 0a20 2020 2020 2020 2060        .        `
-00002390: 6060 7079 7468 6f6e 0a20 2020 2020 2020  ``python.       
-000023a0: 2069 6d70 6f72 7420 7379 730a 2020 2020   import sys.    
-000023b0: 2020 2020 0a20 2020 2020 2020 2073 7973      .        sys
-000023c0: 2e70 6174 682e 6170 7065 6e64 2827 2e2e  .path.append('..
-000023d0: 2729 0a20 2020 2020 2020 2066 726f 6d20  ').        from 
-000023e0: 7079 7465 7874 636c 6173 7369 6669 6572  pytextclassifier
-000023f0: 2069 6d70 6f72 7420 436c 6173 7369 6343   import ClassicC
-00002400: 6c61 7373 6966 6965 720a 2020 2020 2020  lassifier.      
-00002410: 2020 696d 706f 7274 206a 6965 6261 0a20    import jieba. 
-00002420: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00002430: 7463 203d 2043 6c61 7373 6963 436c 6173  tc = ClassicClas
-00002440: 7369 6669 6572 286f 7574 7075 745f 6469  sifier(output_di
-00002450: 723d 276d 6f64 656c 732f 6c72 2d74 6f79  r='models/lr-toy
-00002460: 272c 206d 6f64 656c 5f6e 616d 655f 6f72  ', model_name_or
-00002470: 5f6d 6f64 656c 3d27 6c72 2729 0a20 2020  _model='lr').   
-00002480: 2020 2020 2064 6174 6120 3d20 5b0a 2020       data = [.  
-00002490: 2020 2020 2020 2020 2020 2827 6564 7563            ('educ
-000024a0: 6174 696f 6e27 2c20 27e5 908d e5b8 88e6  ation', '.......
-000024b0: 8c87 e5af bce6 8998 e7a6 8fe8 afad e6b3  ................
-000024c0: 95e6 8a80 e5b7 a7ef bc9a e590 8de8 af8d  ................
-000024d0: e79a 84e5 a48d e695 b0e5 bda2 e5bc 8f27  ...............'
-000024e0: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
-000024f0: 2765 6475 6361 7469 6f6e 272c 2027 e4b8  'education', '..
-00002500: ade5 9bbd e9ab 98e8 8083 e688 90e7 bba9  ................
-00002510: e6b5 b7e5 a496 e8ae a4e5 8faf 20e6 98af  ............ ...
-00002520: e280 9ce7 8bbc e69d a5e4 ba86 e280 9de5  ................
-00002530: 9097 efbc 9f27 292c 0a20 2020 2020 2020  .....'),.       
-00002540: 2020 2020 2028 2773 706f 7274 7327 2c20       ('sports', 
-00002550: 27e5 9bbe e696 87ef bc9a e6b3 95e7 bd91  '...............
-00002560: e5ad 9fe8 8fb2 e5b0 94e6 96af e88b a6e6  ................
-00002570: 8898 e8bf 9b31 36e5 bcba 20e5 ad9f e88f  .....16... .....
-00002580: b2e5 b094 e696 afe6 8092 e590 bc27 292c  .............'),
-00002590: 0a20 2020 2020 2020 2020 2020 2028 2773  .            ('s
-000025a0: 706f 7274 7327 2c20 27e5 9b9b e5b7 9de4  ports', '.......
-000025b0: b8b9 e6a3 b1e4 b8be e8a1 8ce5 85a8 e59b  ................
-000025c0: bde9 95bf e8b7 9de7 99bb e5b1 b1e6 8c91  ................
-000025d0: e688 98e8 b59b 20e8 bf91 e4b8 87e4 baba  ...... .........
-000025e0: e58f 82e4 b88e 2729 2c0a 2020 2020 2020  ......'),.      
-000025f0: 2020 2020 2020 2827 7370 6f72 7473 272c        ('sports',
-00002600: 2027 e7b1 b3e5 85b0 e5ae a2e5 9cba 38e6   '............8.
-00002610: 8898 e4b8 8de8 b4a5 e59b bde7 b1b3 3130  ..............10
-00002620: e5b9 b4e8 bf9e e883 9c27 290a 2020 2020  .........').    
-00002630: 2020 2020 5d0a 2020 2020 2020 2020 7463      ].        tc
-00002640: 2e74 7261 696e 2864 6174 6129 0a20 2020  .train(data).   
-00002650: 2020 2020 2069 6d70 6f72 7420 656c 6935       import eli5
-00002660: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00002670: 2020 696e 6665 725f 6461 7461 203d 205b    infer_data = [
-00002680: 27e9 ab98 e880 83e6 8c87 e5af bce6 8998  '...............
-00002690: e7a6 8fe8 afad e6b3 95e6 8a80 e5b7 a7e5  ................
-000026a0: 9bbd e999 85e8 aea4 e58f af27 2c0a 2020  ...........',.  
-000026b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026c0: 2020 2020 27e6 848f e794 b2e9 a696 e8bd      '...........
-000026d0: aee8 a1a5 e8b5 9be4 baa4 e688 98e8 aeb0  ................
-000026e0: e5bd 953a e7b1 b3e5 85b0 e5ae a2e5 9cba  ...:............
-000026f0: 38e6 8898 e4b8 8de8 b4a5 e59b bde7 b1b3  8...............
-00002700: 3130 e5b9 b4e8 bf9e e883 9c27 5d0a 2020  10.........'].  
-00002710: 2020 2020 2020 656c 6935 2e73 686f 775f        eli5.show_
-00002720: 7765 6967 6874 7328 7463 2e6d 6f64 656c  weights(tc.model
-00002730: 2c20 7665 633d 7463 2e66 6561 7475 7265  , vec=tc.feature
-00002740: 290a 2020 2020 2020 2020 7365 675f 696e  ).        seg_in
-00002750: 6665 725f 6461 7461 203d 205b 2720 272e  fer_data = [' '.
-00002760: 6a6f 696e 286a 6965 6261 2e6c 6375 7428  join(jieba.lcut(
-00002770: 6929 2920 666f 7220 6920 696e 2069 6e66  i)) for i in inf
-00002780: 6572 5f64 6174 615d 0a20 2020 2020 2020  er_data].       
-00002790: 2065 6c69 352e 7368 6f77 5f70 7265 6469   eli5.show_predi
-000027a0: 6374 696f 6e28 7463 2e6d 6f64 656c 2c20  ction(tc.model, 
-000027b0: 7365 675f 696e 6665 725f 6461 7461 5b30  seg_infer_data[0
-000027c0: 5d2c 2076 6563 3d74 632e 6665 6174 7572  ], vec=tc.featur
-000027d0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-000027e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027f0: 7461 7267 6574 5f6e 616d 6573 3d5b 2765  target_names=['e
-00002800: 6475 6361 7469 6f6e 272c 2027 7370 6f72  ducation', 'spor
-00002810: 7473 275d 290a 2020 2020 2020 2020 6060  ts']).        ``
-00002820: 600a 2020 2020 2020 2020 0a20 2020 2020  `.        .     
-00002830: 2020 206f 7574 7075 743a 0a20 2020 2020     output:.     
-00002840: 2020 200a 2020 2020 2020 2020 215b 696d     .        ![im
-00002850: 672e 706e 675d 2864 6f63 732f 696d 672e  g.png](docs/img.
-00002860: 706e 6729 0a20 2020 2020 2020 200a 2020  png).        .  
-00002870: 2020 2020 2020 2323 2320 4465 6570 2043        ### Deep C
-00002880: 6c61 7373 6966 6963 6174 696f 6e20 6d6f  lassification mo
-00002890: 6465 6c0a 2020 2020 2020 2020 0a20 2020  del.        .   
-000028a0: 2020 2020 20e6 9cac e9a1 b9e7 9bae e694       ...........
-000028b0: afe6 8c81 e4bb a5e4 b88b e6b7 b1e5 baa6  ................
-000028c0: e588 86e7 b1bb e6a8 a1e5 9e8b efbc 9a46  ...............F
-000028d0: 6173 7454 6578 74e3 8081 5465 7874 434e  astText...TextCN
-000028e0: 4ee3 8081 5465 7874 524e 4ee3 8081 4265  N...TextRNN...Be
-000028f0: 7274 e6a8 a1e5 9e8b efbc 8c60 696d 706f  rt.........`impo
-00002900: 7274 60e6 a8a1 e59e 8be5 afb9 e5ba 94e7  rt`.............
-00002910: 9a84 e696 b9e6 b395 e69d a5e8 b083 e794  ................
-00002920: a8ef bc9a 0a20 2020 2020 2020 2060 6060  .....        ```
-00002930: 7079 7468 6f6e 0a20 2020 2020 2020 2066  python.        f
-00002940: 726f 6d20 7079 7465 7874 636c 6173 7369  rom pytextclassi
-00002950: 6669 6572 2069 6d70 6f72 7420 4661 7374  fier import Fast
-00002960: 5465 7874 436c 6173 7369 6669 6572 2c20  TextClassifier, 
-00002970: 5465 7874 434e 4e43 6c61 7373 6966 6965  TextCNNClassifie
-00002980: 722c 2054 6578 7452 4e4e 436c 6173 7369  r, TextRNNClassi
-00002990: 6669 6572 2c20 4265 7274 436c 6173 7369  fier, BertClassi
-000029a0: 6669 6572 0a20 2020 2020 2020 2060 6060  fier.        ```
-000029b0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-000029c0: 2020 e4b8 8be9 9da2 e4bb a546 6173 7454    .........FastT
-000029d0: 6578 74e6 a8a1 e59e 8be4 b8ba e7a4 bae4  ext.............
-000029e0: be8b efbc 8ce5 85b6 e4bb 96e6 a8a1 e59e  ................
-000029f0: 8be7 9a84 e4bd bfe7 94a8 e696 b9e6 b395  ................
-00002a00: e7b1 bbe4 bcbc e380 820a 2020 2020 2020  ..........      
-00002a10: 2020 0a20 2020 2020 2020 2023 2323 2046    .        ### F
-00002a20: 6173 7454 6578 7420 e6a8 a1e5 9e8b 0a20  astText ....... 
-00002a30: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00002a40: e8ae ade7 bb83 e592 8ce9 a284 e6b5 8b60  ...............`
-00002a50: 4661 7374 5465 7874 60e6 a8a1 e59e 8be7  FastText`.......
-00002a60: a4ba e4be 8b5b 6578 616d 706c 6573 2f66  .....[examples/f
-00002a70: 6173 7474 6578 745f 636c 6173 7369 6669  asttext_classifi
-00002a80: 6361 7469 6f6e 5f64 656d 6f2e 7079 5d28  cation_demo.py](
-00002a90: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00002aa0: 6f6d 2f73 6869 6269 6e67 3632 342f 7079  om/shibing624/py
-00002ab0: 7465 7874 636c 6173 7369 6669 6572 2f62  textclassifier/b
-00002ac0: 6c6f 622f 6d61 7374 6572 2f65 7861 6d70  lob/master/examp
-00002ad0: 6c65 732f 6661 7374 7465 7874 5f63 6c61  les/fasttext_cla
-00002ae0: 7373 6966 6963 6174 696f 6e5f 6465 6d6f  ssification_demo
-00002af0: 2e70 7929 0a20 2020 2020 2020 200a 2020  .py).        .  
-00002b00: 2020 2020 2020 6060 6070 7974 686f 6e0a        ```python.
-00002b10: 2020 2020 2020 2020 696d 706f 7274 2073          import s
-00002b20: 7973 0a20 2020 2020 2020 200a 2020 2020  ys.        .    
-00002b30: 2020 2020 7379 732e 7061 7468 2e61 7070      sys.path.app
-00002b40: 656e 6428 272e 2e27 290a 2020 2020 2020  end('..').      
-00002b50: 2020 6672 6f6d 2070 7974 6578 7463 6c61    from pytextcla
-00002b60: 7373 6966 6965 7220 696d 706f 7274 2046  ssifier import F
-00002b70: 6173 7454 6578 7443 6c61 7373 6966 6965  astTextClassifie
-00002b80: 722c 206c 6f61 645f 6461 7461 0a20 2020  r, load_data.   
-00002b90: 2020 2020 200a 2020 2020 2020 2020 6966       .        if
-00002ba0: 205f 5f6e 616d 655f 5f20 3d3d 2027 5f5f   __name__ == '__
-00002bb0: 6d61 696e 5f5f 273a 0a20 2020 2020 2020  main__':.       
-00002bc0: 2020 2020 206d 203d 2046 6173 7454 6578       m = FastTex
-00002bd0: 7443 6c61 7373 6966 6965 7228 6f75 7470  tClassifier(outp
-00002be0: 7574 5f64 6972 3d27 6d6f 6465 6c73 2f66  ut_dir='models/f
-00002bf0: 6173 7474 6578 742d 746f 7927 290a 2020  asttext-toy').  
-00002c00: 2020 2020 2020 2020 2020 6461 7461 203d            data =
-00002c10: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
-00002c20: 2020 2028 2765 6475 6361 7469 6f6e 272c     ('education',
-00002c30: 2027 e590 8de5 b888 e68c 87e5 afbc e689   '..............
-00002c40: 98e7 a68f e8af ade6 b395 e68a 80e5 b7a7  ................
-00002c50: efbc 9ae5 908d e8af 8de7 9a84 e5a4 8de6  ................
-00002c60: 95b0 e5bd a2e5 bc8f 2729 2c0a 2020 2020  ........'),.    
-00002c70: 2020 2020 2020 2020 2020 2020 2827 6564              ('ed
-00002c80: 7563 6174 696f 6e27 2c20 27e4 b8ad e59b  ucation', '.....
-00002c90: bde9 ab98 e880 83e6 8890 e7bb a9e6 b5b7  ................
-00002ca0: e5a4 96e8 aea4 e58f af20 e698 afe2 809c  ......... ......
-00002cb0: e78b bce6 9da5 e4ba 86e2 809d e590 97ef  ................
-00002cc0: bc9f 2729 2c0a 2020 2020 2020 2020 2020  ..'),.          
-00002cd0: 2020 2020 2020 2827 6564 7563 6174 696f        ('educatio
-00002ce0: 6e27 2c20 27e5 85ac e58a a1e5 9198 e880  n', '...........
-00002cf0: 83e8 9991 e8b6 8ae6 9da5 e8b6 8ae5 9083  ................
-00002d00: e9a6 99ef bc8c e8bf 99e6 98af e680 8ee4  ................
-00002d10: b988 e59b 9ee4 ba8b efbc 9f27 292c 0a20  ...........'),. 
-00002d20: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-00002d30: 2773 706f 7274 7327 2c20 27e5 9bbe e696  'sports', '.....
-00002d40: 87ef bc9a e6b3 95e7 bd91 e5ad 9fe8 8fb2  ................
-00002d50: e5b0 94e6 96af e88b a6e6 8898 e8bf 9b31  ...............1
-00002d60: 36e5 bcba 20e5 ad9f e88f b2e5 b094 e696  6... ...........
-00002d70: afe6 8092 e590 bc27 292c 0a20 2020 2020  .......'),.     
-00002d80: 2020 2020 2020 2020 2020 2028 2773 706f             ('spo
-00002d90: 7274 7327 2c20 27e5 9b9b e5b7 9de4 b8b9  rts', '.........
-00002da0: e6a3 b1e4 b8be e8a1 8ce5 85a8 e59b bde9  ................
-00002db0: 95bf e8b7 9de7 99bb e5b1 b1e6 8c91 e688  ................
-00002dc0: 98e8 b59b 20e8 bf91 e4b8 87e4 baba e58f  .... ...........
-00002dd0: 82e4 b88e 2729 2c0a 2020 2020 2020 2020  ....'),.        
-00002de0: 2020 2020 2020 2020 2827 7370 6f72 7473          ('sports
-00002df0: 272c 2027 e7b1 b3e5 85b0 e5ae a2e5 9cba  ', '............
-00002e00: 38e6 8898 e4b8 8de8 b4a5 e4bf 9de6 8c81  8...............
-00002e10: e8bf 9ee8 839c 2729 2c0a 2020 2020 2020  ......'),.      
-00002e20: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
-00002e30: 2020 2020 6d2e 7472 6169 6e28 6461 7461      m.train(data
-00002e40: 2c20 6e75 6d5f 6570 6f63 6873 3d33 290a  , num_epochs=3).
-00002e50: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00002e60: 7428 6d29 0a20 2020 2020 2020 2020 2020  t(m).           
-00002e70: 2023 206c 6f61 6420 7472 6169 6e65 6420   # load trained 
-00002e80: 6265 7374 206d 6f64 656c 0a20 2020 2020  best model.     
-00002e90: 2020 2020 2020 206d 2e6c 6f61 645f 6d6f         m.load_mo
-00002ea0: 6465 6c28 290a 2020 2020 2020 2020 2020  del().          
-00002eb0: 2020 7072 6564 6963 745f 6c61 6265 6c2c    predict_label,
-00002ec0: 2070 7265 6469 6374 5f70 726f 6261 203d   predict_proba =
-00002ed0: 206d 2e70 7265 6469 6374 285b 27e7 a68f   m.predict(['...
-00002ee0: e5bb bae6 98a5 e5ad a3e5 85ac e58a a1e5  ................
-00002ef0: 9198 e880 83e8 af95 e68a a5e5 908d 3138  ..............18
-00002f00: e697 a5e6 88aa e6ad a220 32e6 9c88 36e6  ......... 2...6.
-00002f10: 97a5 e880 83e8 af95 272c 0a20 2020 2020  ........',.     
-00002f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f50: 2027 e684 8fe7 94b2 e9a6 96e8 bdae e8a1   '..............
-00002f60: a5e8 b59b e4ba a4e6 8898 e8ae b0e5 bd95  ................
-00002f70: 3ae7 b1b3 e585 b0e5 aea2 e59c ba38 e688  :............8..
-00002f80: 98e4 b88d e8b4 a5e5 9bbd e7b1 b331 30e5  .............10.
-00002f90: b9b4 e8bf 9ee8 839c 275d 290a 2020 2020  ........']).    
-00002fa0: 2020 2020 2020 2020 7072 696e 7428 6627          print(f'
-00002fb0: 7072 6564 6963 745f 6c61 6265 6c3a 207b  predict_label: {
-00002fc0: 7072 6564 6963 745f 6c61 6265 6c7d 2c20  predict_label}, 
-00002fd0: 7072 6564 6963 745f 7072 6f62 613a 207b  predict_proba: {
-00002fe0: 7072 6564 6963 745f 7072 6f62 617d 2729  predict_proba}')
-00002ff0: 0a20 2020 2020 2020 2020 2020 2074 6573  .            tes
-00003000: 745f 6461 7461 203d 205b 0a20 2020 2020  t_data = [.     
-00003010: 2020 2020 2020 2020 2020 2028 2765 6475             ('edu
-00003020: 6361 7469 6f6e 272c 2027 e7a6 8fe5 bbba  cation', '......
-00003030: e698 a5e5 ada3 e585 ace5 8aa1 e591 98e8  ................
-00003040: 8083 e8af 95e6 8aa5 e590 8d31 38e6 97a5  ...........18...
-00003050: e688 aae6 ada2 2032 e69c 8836 e697 a5e8  ...... 2...6....
-00003060: 8083 e8af 9527 292c 0a20 2020 2020 2020  .....'),.       
-00003070: 2020 2020 2020 2020 2028 2773 706f 7274           ('sport
-00003080: 7327 2c20 27e6 848f e794 b2e9 a696 e8bd  s', '...........
-00003090: aee8 a1a5 e8b5 9be4 baa4 e688 98e8 aeb0  ................
-000030a0: e5bd 953a e7b1 b3e5 85b0 e5ae a2e5 9cba  ...:............
-000030b0: 38e6 8898 e4b8 8de8 b4a5 e59b bde7 b1b3  8...............
-000030c0: 3130 e5b9 b4e8 bf9e e883 9c27 292c 0a20  10.........'),. 
-000030d0: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
-000030e0: 2020 2020 2020 2020 2061 6363 5f73 636f           acc_sco
-000030f0: 7265 203d 206d 2e65 7661 6c75 6174 655f  re = m.evaluate_
-00003100: 6d6f 6465 6c28 7465 7374 5f64 6174 6129  model(test_data)
-00003110: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00003120: 6e74 2866 2761 6363 5f73 636f 7265 3a20  nt(f'acc_score: 
-00003130: 7b61 6363 5f73 636f 7265 7d27 2920 2023  {acc_score}')  #
-00003140: 2031 2e30 0a20 2020 2020 2020 200a 2020   1.0.        .  
-00003150: 2020 2020 2020 2020 2020 2323 2323 2074            #### t
-00003160: 7261 696e 206d 6f64 656c 2077 6974 6820  rain model with 
-00003170: 3177 2064 6174 610a 2020 2020 2020 2020  1w data.        
-00003180: 2020 2020 7072 696e 7428 272d 2720 2a20      print('-' * 
-00003190: 3432 290a 2020 2020 2020 2020 2020 2020  42).            
-000031a0: 6461 7461 5f66 696c 6520 3d20 2774 6875  data_file = 'thu
-000031b0: 636e 6577 735f 7472 6169 6e5f 3177 2e74  cnews_train_1w.t
-000031c0: 7874 270a 2020 2020 2020 2020 2020 2020  xt'.            
-000031d0: 6d20 3d20 4661 7374 5465 7874 436c 6173  m = FastTextClas
-000031e0: 7369 6669 6572 286f 7574 7075 745f 6469  sifier(output_di
-000031f0: 723d 276d 6f64 656c 732f 6661 7374 7465  r='models/fastte
-00003200: 7874 2729 0a20 2020 2020 2020 2020 2020  xt').           
-00003210: 206d 2e74 7261 696e 2864 6174 615f 6669   m.train(data_fi
-00003220: 6c65 2c20 6e61 6d65 733d 2827 6c61 6265  le, names=('labe
-00003230: 6c73 272c 2027 7465 7874 2729 2c20 6e75  ls', 'text'), nu
-00003240: 6d5f 6570 6f63 6873 3d33 290a 2020 2020  m_epochs=3).    
-00003250: 2020 2020 2020 2020 2320 6c6f 6164 2062          # load b
-00003260: 6573 7420 7472 6169 6e65 6420 6d6f 6465  est trained mode
-00003270: 6c20 6672 6f6d 206d 6f64 656c 5f64 6972  l from model_dir
-00003280: 0a20 2020 2020 2020 2020 2020 206d 2e6c  .            m.l
-00003290: 6f61 645f 6d6f 6465 6c28 290a 2020 2020  oad_model().    
-000032a0: 2020 2020 2020 2020 7072 6564 6963 745f          predict_
-000032b0: 6c61 6265 6c2c 2070 7265 6469 6374 5f70  label, predict_p
-000032c0: 726f 6261 203d 206d 2e70 7265 6469 6374  roba = m.predict
-000032d0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000032e0: 2020 5b27 e9a1 bae4 b989 e58c 97e4 baac    ['............
-000032f0: e88b 8fe6 b4bb 3838 e5b9 b3e7 b1b3 e8b5  ......88........
-00003300: b7e7 b2be e8a3 85e6 88bf e59c a8e5 94ae  ................
-00003310: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-00003320: 2020 2020 27e7 be8e 4542 2d35 e9a1 b9e7      '...EB-5....
-00003330: 9bae e280 9c31 35e6 97a5 e5bf abe9 809f  .....15.........
-00003340: e7a7 bbe6 b091 e280 9de5 b086 e68e a8e8  ................
-00003350: bf9f 275d 0a20 2020 2020 2020 2020 2020  ..'].           
-00003360: 2029 0a20 2020 2020 2020 2020 2020 2070   ).            p
-00003370: 7269 6e74 2866 2770 7265 6469 6374 5f6c  rint(f'predict_l
-00003380: 6162 656c 3a20 7b70 7265 6469 6374 5f6c  abel: {predict_l
-00003390: 6162 656c 7d2c 2070 7265 6469 6374 5f70  abel}, predict_p
-000033a0: 726f 6261 3a20 7b70 7265 6469 6374 5f70  roba: {predict_p
-000033b0: 726f 6261 7d27 290a 2020 2020 2020 2020  roba}').        
-000033c0: 2020 2020 782c 2079 2c20 6466 203d 206c      x, y, df = l
-000033d0: 6f61 645f 6461 7461 2864 6174 615f 6669  oad_data(data_fi
-000033e0: 6c65 290a 2020 2020 2020 2020 2020 2020  le).            
-000033f0: 7465 7374 5f64 6174 6120 3d20 6466 5b3a  test_data = df[:
-00003400: 3130 305d 0a20 2020 2020 2020 2020 2020  100].           
+000000e0: 6520 322e 300a 4b65 7977 6f72 6473 3a20  e 2.0.Keywords: 
+000000f0: 7079 7465 7874 636c 6173 7369 6669 6572  pytextclassifier
+00000100: 2c74 6578 7463 6c61 7373 6966 6965 722c  ,textclassifier,
+00000110: 636c 6173 7369 6669 6572 2c74 6578 7463  classifier,textc
+00000120: 6c61 7373 6966 6963 6174 696f 6e0a 436c  lassification.Cl
+00000130: 6173 7369 6669 6572 3a20 496e 7465 6e64  assifier: Intend
+00000140: 6564 2041 7564 6965 6e63 6520 3a3a 2053  ed Audience :: S
+00000150: 6369 656e 6365 2f52 6573 6561 7263 680a  cience/Research.
+00000160: 436c 6173 7369 6669 6572 3a20 4f70 6572  Classifier: Oper
+00000170: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
+00000180: 4f53 2049 6e64 6570 656e 6465 6e74 0a43  OS Independent.C
+00000190: 6c61 7373 6966 6965 723a 204c 6963 656e  lassifier: Licen
+000001a0: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
+000001b0: 6564 203a 3a20 4170 6163 6865 2053 6f66  ed :: Apache Sof
+000001c0: 7477 6172 6520 4c69 6365 6e73 650a 436c  tware License.Cl
+000001d0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+000001e0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+000001f0: 3a20 5079 7468 6f6e 0a43 6c61 7373 6966  : Python.Classif
+00000200: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+00000210: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000220: 686f 6e20 3a3a 2032 2e37 0a43 6c61 7373  hon :: 2.7.Class
+00000230: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+00000240: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000250: 7974 686f 6e20 3a3a 2033 0a43 6c61 7373  ython :: 3.Class
+00000260: 6966 6965 723a 2054 6f70 6963 203a 3a20  ifier: Topic :: 
+00000270: 5465 7874 2050 726f 6365 7373 696e 6720  Text Processing 
+00000280: 3a3a 204c 696e 6775 6973 7469 630a 436c  :: Linguistic.Cl
+00000290: 6173 7369 6669 6572 3a20 546f 7069 6320  assifier: Topic 
+000002a0: 3a3a 2053 6369 656e 7469 6669 632f 456e  :: Scientific/En
+000002b0: 6769 6e65 6572 696e 6720 3a3a 2041 7274  gineering :: Art
+000002c0: 6966 6963 6961 6c20 496e 7465 6c6c 6967  ificial Intellig
+000002d0: 656e 6365 0a44 6573 6372 6970 7469 6f6e  ence.Description
+000002e0: 2d43 6f6e 7465 6e74 2d54 7970 653a 2074  -Content-Type: t
+000002f0: 6578 742f 6d61 726b 646f 776e 0a4c 6963  ext/markdown.Lic
+00000300: 656e 7365 2d46 696c 653a 204c 4943 454e  ense-File: LICEN
+00000310: 5345 0a0a 3c64 6976 2061 6c69 676e 3d22  SE..<div align="
+00000320: 6365 6e74 6572 223e 0a20 203c 6120 6872  center">.  <a hr
+00000330: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+00000340: 7562 2e63 6f6d 2f73 6869 6269 6e67 3632  ub.com/shibing62
+00000350: 342f 7079 7465 7874 636c 6173 7369 6669  4/pytextclassifi
+00000360: 6572 223e 0a20 2020 203c 696d 6720 7372  er">.    <img sr
+00000370: 633d 2268 7474 7073 3a2f 2f67 6974 6875  c="https://githu
+00000380: 622e 636f 6d2f 7368 6962 696e 6736 3234  b.com/shibing624
+00000390: 2f70 7974 6578 7463 6c61 7373 6966 6965  /pytextclassifie
+000003a0: 722f 626c 6f62 2f6d 6173 7465 722f 646f  r/blob/master/do
+000003b0: 6373 2f6c 6f67 6f2e 706e 6722 2061 6c74  cs/logo.png" alt
+000003c0: 3d22 4c6f 676f 2220 6865 6967 6874 3d22  ="Logo" height="
+000003d0: 3135 3622 3e0a 2020 3c2f 613e 0a3c 2f64  156">.  </a>.</d
+000003e0: 6976 3e0a 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  iv>..-----------
+000003f0: 2d2d 2d2d 2d2d 0a0a 2320 5079 5465 7874  ------..# PyText
+00000400: 436c 6173 7369 6669 6572 3a20 5079 7468  Classifier: Pyth
+00000410: 6f6e 2054 6578 7420 436c 6173 7369 6669  on Text Classifi
+00000420: 6572 0a5b 215b 5079 5049 2076 6572 7369  er.[![PyPI versi
+00000430: 6f6e 5d28 6874 7470 733a 2f2f 6261 6467  on](https://badg
+00000440: 652e 6675 7279 2e69 6f2f 7079 2f70 7974  e.fury.io/py/pyt
+00000450: 6578 7463 6c61 7373 6966 6965 722e 7376  extclassifier.sv
+00000460: 6729 5d28 6874 7470 733a 2f2f 6261 6467  g)](https://badg
+00000470: 652e 6675 7279 2e69 6f2f 7079 2f70 7974  e.fury.io/py/pyt
+00000480: 6578 7463 6c61 7373 6966 6965 7229 0a5b  extclassifier).[
+00000490: 215b 446f 776e 6c6f 6164 735d 2868 7474  ![Downloads](htt
+000004a0: 7073 3a2f 2f73 7461 7469 632e 7065 7079  ps://static.pepy
+000004b0: 2e74 6563 682f 6261 6467 652f 7079 7465  .tech/badge/pyte
+000004c0: 7874 636c 6173 7369 6669 6572 295d 2868  xtclassifier)](h
+000004d0: 7474 7073 3a2f 2f70 6570 792e 7465 6368  ttps://pepy.tech
+000004e0: 2f70 726f 6a65 6374 2f70 7974 6578 7463  /project/pytextc
+000004f0: 6c61 7373 6966 6965 7229 0a5b 215b 436f  lassifier).[![Co
+00000500: 6e74 7269 6275 7469 6f6e 7320 7765 6c63  ntributions welc
+00000510: 6f6d 655d 2868 7474 7073 3a2f 2f69 6d67  ome](https://img
+00000520: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
+00000530: 652f 636f 6e74 7269 6275 7469 6f6e 732d  e/contributions-
+00000540: 7765 6c63 6f6d 652d 6272 6967 6874 6772  welcome-brightgr
+00000550: 6565 6e2e 7376 6729 5d28 434f 4e54 5249  een.svg)](CONTRI
+00000560: 4255 5449 4e47 2e6d 6429 0a5b 215b 4c69  BUTING.md).[![Li
+00000570: 6365 6e73 6520 4170 6163 6865 2032 2e30  cense Apache 2.0
+00000580: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00000590: 6965 6c64 732e 696f 2f62 6164 6765 2f6c  ields.io/badge/l
+000005a0: 6963 656e 7365 2d41 7061 6368 6525 3230  icense-Apache%20
+000005b0: 322e 302d 626c 7565 2e73 7667 295d 284c  2.0-blue.svg)](L
+000005c0: 4943 454e 5345 290a 5b21 5b70 7974 686f  ICENSE).[![pytho
+000005d0: 6e5f 7665 7369 6f6e 5d28 6874 7470 733a  n_vesion](https:
+000005e0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000005f0: 2f62 6164 6765 2f50 7974 686f 6e2d 332e  /badge/Python-3.
+00000600: 3525 3242 2d67 7265 656e 2e73 7667 295d  5%2B-green.svg)]
+00000610: 2872 6571 7569 7265 6d65 6e74 732e 7478  (requirements.tx
+00000620: 7429 0a5b 215b 4769 7448 7562 2069 7373  t).[![GitHub iss
+00000630: 7565 735d 2868 7474 7073 3a2f 2f69 6d67  ues](https://img
+00000640: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
+00000650: 7562 2f69 7373 7565 732f 7368 6962 696e  ub/issues/shibin
+00000660: 6736 3234 2f70 7974 6578 7463 6c61 7373  g624/pytextclass
+00000670: 6966 6965 722e 7376 6729 5d28 6874 7470  ifier.svg)](http
+00000680: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
+00000690: 6869 6269 6e67 3632 342f 7079 7465 7874  hibing624/pytext
+000006a0: 636c 6173 7369 6669 6572 2f69 7373 7565  classifier/issue
+000006b0: 7329 0a5b 215b 5765 6368 6174 2047 726f  s).[![Wechat Gro
+000006c0: 7570 5d28 6874 7470 733a 2f2f 696d 672e  up](https://img.
+000006d0: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
+000006e0: 2f77 6563 6861 742d 6772 6f75 702d 6772  /wechat-group-gr
+000006f0: 6565 6e2e 7376 673f 6c6f 676f 3d77 6563  een.svg?logo=wec
+00000700: 6861 7429 5d28 2343 6f6e 7461 6374 290a  hat)](#Contact).
+00000710: 0a0a 2323 2049 6e74 726f 6475 6374 696f  ..## Introductio
+00000720: 6e0a 5079 5465 7874 436c 6173 7369 6669  n.PyTextClassifi
+00000730: 6572 3a20 5079 7468 6f6e 2054 6578 7420  er: Python Text 
+00000740: 436c 6173 7369 6669 6572 2e20 4974 2063  Classifier. It c
+00000750: 616e 2062 6520 6170 706c 6965 6420 746f  an be applied to
+00000760: 2074 6865 2066 6965 6c64 7320 6f66 2073   the fields of s
+00000770: 656e 7469 6d65 6e74 2070 6f6c 6172 6974  entiment polarit
+00000780: 7920 616e 616c 7973 6973 2c20 7465 7874  y analysis, text
+00000790: 2072 6973 6b20 636c 6173 7369 6669 6361   risk classifica
+000007a0: 7469 6f6e 2061 6e64 2073 6f20 6f6e 2c0a  tion and so on,.
+000007b0: 616e 6420 6974 2073 7570 706f 7274 7320  and it supports 
+000007c0: 6d75 6c74 6970 6c65 2063 6c61 7373 6966  multiple classif
+000007d0: 6963 6174 696f 6e20 616c 676f 7269 7468  ication algorith
+000007e0: 6d73 2061 6e64 2063 6c75 7374 6572 696e  ms and clusterin
+000007f0: 6720 616c 676f 7269 7468 6d73 2e0a 0a2a  g algorithms...*
+00000800: 2a70 7974 6578 7463 6c61 7373 6966 6965  *pytextclassifie
+00000810: 722a 2a20 6973 2061 2070 7974 686f 6e20  r** is a python 
+00000820: 4f70 656e 2053 6f75 7263 6520 546f 6f6c  Open Source Tool
+00000830: 6b69 7420 666f 7220 7465 7874 2063 6c61  kit for text cla
+00000840: 7373 6966 6963 6174 696f 6e2e 2054 6865  ssification. The
+00000850: 2067 6f61 6c20 6973 2074 6f20 696d 706c   goal is to impl
+00000860: 656d 656e 740a 7465 7874 2061 6e61 6c79  ement.text analy
+00000870: 7369 7320 616c 676f 7269 7468 6d2c 2073  sis algorithm, s
+00000880: 6f20 746f 2061 6368 6965 7665 2074 6865  o to achieve the
+00000890: 2075 7365 2069 6e20 7468 6520 7072 6f64   use in the prod
+000008a0: 7563 7469 6f6e 2065 6e76 6972 6f6e 6d65  uction environme
+000008b0: 6e74 2e0a 0ae6 9687 e69c ace5 8886 e7b1  nt..............
+000008c0: bbe5 99a8 efbc 8ce6 8f90 e4be 9be5 a49a  ................
+000008d0: e7a7 8de6 9687 e69c ace5 8886 e7b1 bbe5  ................
+000008e0: 928c e881 9ae7 b1bb e7ae 97e6 b395 efbc  ................
+000008f0: 8ce6 94af e68c 81e5 8fa5 e5ad 90e5 928c  ................
+00000900: e696 87e6 a1a3 e7ba a7e7 9a84 e696 87e6  ................
+00000910: 9cac e588 86e7 b1bb e4bb bbe5 8aa1 efbc  ................
+00000920: 8ce6 94af e68c 81e4 ba8c e588 86e7 b1bb  ................
+00000930: e380 81e5 a49a e588 86e7 b1bb e380 81e5  ................
+00000940: a49a e6a0 87e7 adbe e588 86e7 b1bb e380  ................
+00000950: 81e5 a49a e5b1 82e7 baa7 e588 86e7 b1bb  ................
+00000960: e592 8c4b 6d65 616e 73e8 819a e7b1 bbef  ...Kmeans.......
+00000970: bc8c e5bc 80e7 aeb1 e58d b3e7 94a8 e380  ................
+00000980: 8270 7974 686f 6e33 e5bc 80e5 8f91 e380  .python3........
+00000990: 820a 0a2a 2a47 7569 6465 2a2a 0a0a 2d20  ...**Guide**..- 
+000009a0: 5b46 6561 7475 7265 5d28 2346 6561 7475  [Feature](#Featu
+000009b0: 7265 290a 2d20 5b49 6e73 7461 6c6c 5d28  re).- [Install](
+000009c0: 2369 6e73 7461 6c6c 290a 2d20 5b55 7361  #install).- [Usa
+000009d0: 6765 5d28 2375 7361 6765 290a 2d20 5b44  ge](#usage).- [D
+000009e0: 6174 6173 6574 5d28 2344 6174 6173 6574  ataset](#Dataset
+000009f0: 290a 2d20 5b43 6f6e 7461 6374 5d28 2343  ).- [Contact](#C
+00000a00: 6f6e 7461 6374 290a 2d20 5b43 6974 6174  ontact).- [Citat
+00000a10: 696f 6e5d 2823 4369 7461 7469 6f6e 290a  ion](#Citation).
+00000a20: 2d20 5b52 6566 6572 656e 6365 5d28 2372  - [Reference](#r
+00000a30: 6566 6572 656e 6365 290a 0a23 2320 4665  eference)..## Fe
+00000a40: 6174 7572 650a 0a2a 2a70 7974 6578 7463  ature..**pytextc
+00000a50: 6c61 7373 6966 6965 722a 2a20 6861 7320  lassifier** has 
+00000a60: 7468 6520 6368 6172 6163 7465 7269 7374  the characterist
+00000a70: 6963 730a 6f66 2063 6c65 6172 2061 6c67  ics.of clear alg
+00000a80: 6f72 6974 686d 2c20 6869 6768 2070 6572  orithm, high per
+00000a90: 666f 726d 616e 6365 2061 6e64 2063 7573  formance and cus
+00000aa0: 746f 6d69 7a61 626c 6520 636f 7270 7573  tomizable corpus
+00000ab0: 2e0a 0a46 756e 6374 696f 6e73 efbc 9a0a  ...Functions....
+00000ac0: 2323 2320 436c 6173 7369 6669 6572 0a20  ### Classifier. 
+00000ad0: 202d 205b 785d 204c 6f67 6973 7469 6352   - [x] LogisticR
+00000ae0: 6567 7265 7373 696f 6e0a 2020 2d20 5b78  egression.  - [x
+00000af0: 5d20 5261 6e64 6f6d 2046 6f72 6573 740a  ] Random Forest.
+00000b00: 2020 2d20 5b78 5d20 4465 6369 7369 6f6e    - [x] Decision
+00000b10: 2054 7265 650a 2020 2d20 5b78 5d20 4b2d   Tree.  - [x] K-
+00000b20: 4e65 6172 6573 7420 4e65 6967 6862 6f75  Nearest Neighbou
+00000b30: 7273 0a20 202d 205b 785d 204e 6169 7665  rs.  - [x] Naive
+00000b40: 2062 6179 6573 0a20 202d 205b 785d 2058   bayes.  - [x] X
+00000b50: 6762 6f6f 7374 0a20 202d 205b 785d 2053  gboost.  - [x] S
+00000b60: 7570 706f 7274 2056 6563 746f 7220 4d61  upport Vector Ma
+00000b70: 6368 696e 6528 5356 4d29 0a20 202d 205b  chine(SVM).  - [
+00000b80: 785d 2054 6578 7443 4e4e 0a20 202d 205b  x] TextCNN.  - [
+00000b90: 785d 2054 6578 7452 4e4e 0a20 202d 205b  x] TextRNN.  - [
+00000ba0: 785d 2046 6173 7474 6578 740a 2020 2d20  x] Fasttext.  - 
+00000bb0: 5b78 5d20 4245 5254 0a0a 2323 2320 436c  [x] BERT..### Cl
+00000bc0: 7573 7465 720a 2020 2d20 5b78 5d20 4d69  uster.  - [x] Mi
+00000bd0: 6e69 4261 7463 684b 6d65 616e 730a 0a57  niBatchKmeans..W
+00000be0: 6869 6c65 2070 726f 7669 6469 6e67 2072  hile providing r
+00000bf0: 6963 6820 6675 6e63 7469 6f6e 732c 202a  ich functions, *
+00000c00: 2a70 7974 6578 7463 6c61 7373 6966 6965  *pytextclassifie
+00000c10: 722a 2a20 696e 7465 726e 616c 206d 6f64  r** internal mod
+00000c20: 756c 6573 2061 6468 6572 6520 746f 206c  ules adhere to l
+00000c30: 6f77 2063 6f75 706c 696e 672c 206d 6f64  ow coupling, mod
+00000c40: 656c 2061 6468 6572 656e 6365 2074 6f20  el adherence to 
+00000c50: 696e 6572 7420 6c6f 6164 696e 672c 2064  inert loading, d
+00000c60: 6963 7469 6f6e 6172 7920 7075 626c 6963  ictionary public
+00000c70: 6174 696f 6e2c 2061 6e64 2065 6173 7920  ation, and easy 
+00000c80: 746f 2075 7365 2e0a 0a23 2320 496e 7374  to use...## Inst
+00000c90: 616c 6c0a 0a2d 2052 6571 7569 7265 6d65  all..- Requireme
+00000ca0: 6e74 7320 616e 6420 496e 7374 616c 6c61  nts and Installa
+00000cb0: 7469 6f6e 0a0a 6060 600a 7069 7033 2069  tion..```.pip3 i
+00000cc0: 6e73 7461 6c6c 2074 6f72 6368 2023 2063  nstall torch # c
+00000cd0: 6f6e 6461 2069 6e73 7461 6c6c 2070 7974  onda install pyt
+00000ce0: 6f72 6368 0a70 6970 3320 696e 7374 616c  orch.pip3 instal
+00000cf0: 6c20 7079 7465 7874 636c 6173 7369 6669  l pytextclassifi
+00000d00: 6572 0a60 6060 0a0a 6f72 0a0a 6060 600a  er.```..or..```.
+00000d10: 6769 7420 636c 6f6e 6520 6874 7470 733a  git clone https:
+00000d20: 2f2f 6769 7468 7562 2e63 6f6d 2f73 6869  //github.com/shi
+00000d30: 6269 6e67 3632 342f 7079 7465 7874 636c  bing624/pytextcl
+00000d40: 6173 7369 6669 6572 2e67 6974 0a63 6420  assifier.git.cd 
+00000d50: 7079 7465 7874 636c 6173 7369 6669 6572  pytextclassifier
+00000d60: 0a70 7974 686f 6e33 2073 6574 7570 2e70  .python3 setup.p
+00000d70: 7920 696e 7374 616c 6c0a 6060 600a 0a0a  y install.```...
+00000d80: 2323 2055 7361 6765 0a23 2323 2054 6578  ## Usage.### Tex
+00000d90: 7420 436c 6173 7369 6669 6572 0a0a 2323  t Classifier..##
+00000da0: 2320 456e 676c 6973 6820 5465 7874 2043  # English Text C
+00000db0: 6c61 7373 6966 6965 720a 0a49 6e63 6c75  lassifier..Inclu
+00000dc0: 6469 6e67 206d 6f64 656c 2074 7261 696e  ding model train
+00000dd0: 696e 672c 2073 6176 696e 672c 2070 7265  ing, saving, pre
+00000de0: 6469 6374 2c20 6576 616c 7561 7465 2c20  dict, evaluate, 
+00000df0: 666f 7220 6578 616d 706c 6520 5b65 7861  for example [exa
+00000e00: 6d70 6c65 732f 6c72 5f65 6e5f 636c 6173  mples/lr_en_clas
+00000e10: 7369 6669 6361 7469 6f6e 5f64 656d 6f2e  sification_demo.
+00000e20: 7079 5d28 6874 7470 733a 2f2f 6769 7468  py](https://gith
+00000e30: 7562 2e63 6f6d 2f73 6869 6269 6e67 3632  ub.com/shibing62
+00000e40: 342f 7079 7465 7874 636c 6173 7369 6669  4/pytextclassifi
+00000e50: 6572 2f62 6c6f 622f 6d61 7374 6572 2f65  er/blob/master/e
+00000e60: 7861 6d70 6c65 732f 6c72 5f65 6e5f 636c  xamples/lr_en_cl
+00000e70: 6173 7369 6669 6361 7469 6f6e 5f64 656d  assification_dem
+00000e80: 6f2e 7079 293a 0a0a 6060 6070 7974 686f  o.py):..```pytho
+00000e90: 6e0a 696d 706f 7274 2073 7973 0a0a 7379  n.import sys..sy
+00000ea0: 732e 7061 7468 2e61 7070 656e 6428 272e  s.path.append('.
+00000eb0: 2e27 290a 6672 6f6d 2070 7974 6578 7463  .').from pytextc
+00000ec0: 6c61 7373 6966 6965 7220 696d 706f 7274  lassifier import
+00000ed0: 2043 6c61 7373 6963 436c 6173 7369 6669   ClassicClassifi
+00000ee0: 6572 0a0a 6966 205f 5f6e 616d 655f 5f20  er..if __name__ 
+00000ef0: 3d3d 2027 5f5f 6d61 696e 5f5f 273a 0a20  == '__main__':. 
+00000f00: 2020 206d 203d 2043 6c61 7373 6963 436c     m = ClassicCl
+00000f10: 6173 7369 6669 6572 286f 7574 7075 745f  assifier(output_
+00000f20: 6469 723d 276d 6f64 656c 732f 6c72 272c  dir='models/lr',
+00000f30: 206d 6f64 656c 5f6e 616d 655f 6f72 5f6d   model_name_or_m
+00000f40: 6f64 656c 3d27 6c72 2729 0a20 2020 2023  odel='lr').    #
+00000f50: 2043 6c61 7373 6963 436c 6173 7369 6669   ClassicClassifi
+00000f60: 6572 2073 7570 706f 7274 206d 6f64 656c  er support model
+00000f70: 5f6e 616d 65ef bc9a 6c72 2c20 7261 6e64  _name...lr, rand
+00000f80: 6f6d 5f66 6f72 6573 742c 2064 6563 6973  om_forest, decis
+00000f90: 696f 6e5f 7472 6565 2c20 6b6e 6e2c 2062  ion_tree, knn, b
+00000fa0: 6179 6573 2c20 7376 6d2c 2078 6762 6f6f  ayes, svm, xgboo
+00000fb0: 7374 0a20 2020 2070 7269 6e74 286d 290a  st.    print(m).
+00000fc0: 2020 2020 6461 7461 203d 205b 0a20 2020      data = [.   
+00000fd0: 2020 2020 2028 2765 6475 6361 7469 6f6e       ('education
+00000fe0: 272c 2027 5374 7564 656e 7420 6465 6274  ', 'Student debt
+00000ff0: 2074 6f20 636f 7374 2042 7269 7461 696e   to cost Britain
+00001000: 2062 696c 6c69 6f6e 7320 7769 7468 696e   billions within
+00001010: 2064 6563 6164 6573 2729 2c0a 2020 2020   decades'),.    
+00001020: 2020 2020 2827 6564 7563 6174 696f 6e27      ('education'
+00001030: 2c20 2743 6869 6e65 7365 2065 6475 6361  , 'Chinese educa
+00001040: 7469 6f6e 2066 6f72 2054 5620 6578 7065  tion for TV expe
+00001050: 7269 6d65 6e74 2729 2c0a 2020 2020 2020  riment'),.      
+00001060: 2020 2827 7370 6f72 7473 272c 2027 4d69    ('sports', 'Mi
+00001070: 6464 6c65 2045 6173 7420 616e 6420 4173  ddle East and As
+00001080: 6961 2062 6f6f 7374 2069 6e76 6573 746d  ia boost investm
+00001090: 656e 7420 696e 2074 6f70 206c 6576 656c  ent in top level
+000010a0: 2073 706f 7274 7327 292c 0a20 2020 2020   sports'),.     
+000010b0: 2020 2028 2773 706f 7274 7327 2c20 2753     ('sports', 'S
+000010c0: 756d 6d69 7420 5365 7269 6573 206c 6f6f  ummit Series loo
+000010d0: 6b20 6c61 756e 6368 6573 2048 424f 2043  k launches HBO C
+000010e0: 616e 6164 6120 7370 6f72 7473 2064 6f63  anada sports doc
+000010f0: 2073 6572 6965 733a 204d 7564 6861 7227   series: Mudhar'
+00001100: 290a 2020 2020 5d0a 2020 2020 2320 7472  ).    ].    # tr
+00001110: 6169 6e20 616e 6420 7361 7665 2062 6573  ain and save bes
+00001120: 7420 6d6f 6465 6c0a 2020 2020 6d2e 7472  t model.    m.tr
+00001130: 6169 6e28 6461 7461 290a 2020 2020 2320  ain(data).    # 
+00001140: 6c6f 6164 2062 6573 7420 6d6f 6465 6c20  load best model 
+00001150: 6672 6f6d 206d 6f64 656c 5f64 6972 0a20  from model_dir. 
+00001160: 2020 206d 2e6c 6f61 645f 6d6f 6465 6c28     m.load_model(
+00001170: 290a 2020 2020 7072 6564 6963 745f 6c61  ).    predict_la
+00001180: 6265 6c2c 2070 7265 6469 6374 5f70 726f  bel, predict_pro
+00001190: 6261 203d 206d 2e70 7265 6469 6374 285b  ba = m.predict([
+000011a0: 0a20 2020 2020 2020 2027 4162 626f 7474  .        'Abbott
+000011b0: 2067 6f76 6572 6e6d 656e 7420 7370 656e   government spen
+000011c0: 6473 2024 3820 6d69 6c6c 696f 6e20 6f6e  ds $8 million on
+000011d0: 2068 6967 6865 7220 6564 7563 6174 696f   higher educatio
+000011e0: 6e20 6d65 6469 6120 626c 6974 7a27 5d29  n media blitz'])
+000011f0: 0a20 2020 2070 7269 6e74 2866 2770 7265  .    print(f'pre
+00001200: 6469 6374 5f6c 6162 656c 3a20 7b70 7265  dict_label: {pre
+00001210: 6469 6374 5f6c 6162 656c 7d2c 2070 7265  dict_label}, pre
+00001220: 6469 6374 5f70 726f 6261 3a20 7b70 7265  dict_proba: {pre
+00001230: 6469 6374 5f70 726f 6261 7d27 290a 0a20  dict_proba}').. 
+00001240: 2020 2074 6573 745f 6461 7461 203d 205b     test_data = [
+00001250: 0a20 2020 2020 2020 2028 2765 6475 6361  .        ('educa
+00001260: 7469 6f6e 272c 2027 4162 626f 7474 2067  tion', 'Abbott g
+00001270: 6f76 6572 6e6d 656e 7420 7370 656e 6473  overnment spends
+00001280: 2024 3820 6d69 6c6c 696f 6e20 6f6e 2068   $8 million on h
+00001290: 6967 6865 7220 6564 7563 6174 696f 6e20  igher education 
+000012a0: 6d65 6469 6120 626c 6974 7a27 292c 0a20  media blitz'),. 
+000012b0: 2020 2020 2020 2028 2773 706f 7274 7327         ('sports'
+000012c0: 2c20 274d 6964 646c 6520 4561 7374 2061  , 'Middle East a
+000012d0: 6e64 2041 7369 6120 626f 6f73 7420 696e  nd Asia boost in
+000012e0: 7665 7374 6d65 6e74 2069 6e20 746f 7020  vestment in top 
+000012f0: 6c65 7665 6c20 7370 6f72 7473 2729 2c0a  level sports'),.
+00001300: 2020 2020 5d0a 2020 2020 6163 635f 7363      ].    acc_sc
+00001310: 6f72 6520 3d20 6d2e 6576 616c 7561 7465  ore = m.evaluate
+00001320: 5f6d 6f64 656c 2874 6573 745f 6461 7461  _model(test_data
+00001330: 290a 2020 2020 7072 696e 7428 6627 6163  ).    print(f'ac
+00001340: 635f 7363 6f72 653a 207b 6163 635f 7363  c_score: {acc_sc
+00001350: 6f72 657d 2729 0a60 6060 0a0a 6f75 7470  ore}').```..outp
+00001360: 7574 3a0a 0a60 6060 0a43 6c61 7373 6963  ut:..```.Classic
+00001370: 436c 6173 7369 6669 6572 2069 6e73 7461  Classifier insta
+00001380: 6e63 6520 284c 6f67 6973 7469 6352 6567  nce (LogisticReg
+00001390: 7265 7373 696f 6e28 6669 745f 696e 7465  ression(fit_inte
+000013a0: 7263 6570 743d 4661 6c73 6529 2c20 7374  rcept=False), st
+000013b0: 6f70 776f 7264 7320 7369 7a65 3a20 3234  opwords size: 24
+000013c0: 3338 290a 7072 6564 6963 745f 6c61 6265  38).predict_labe
+000013d0: 6c3a 205b 2765 6475 6361 7469 6f6e 275d  l: ['education']
+000013e0: 2c20 7072 6564 6963 745f 7072 6f62 613a  , predict_proba:
+000013f0: 205b 302e 3533 3738 3233 3633 3538 3439   [0.537823635849
+00001400: 3231 3132 5d0a 6163 635f 7363 6f72 653a  2112].acc_score:
+00001410: 2031 2e30 0a60 6060 0a0a 2323 2320 4368   1.0.```..### Ch
+00001420: 696e 6573 6520 5465 7874 2043 6c61 7373  inese Text Class
+00001430: 6966 6965 7228 e4b8 ade6 9687 e696 87e6  ifier(..........
+00001440: 9cac e588 86e7 b1bb 290a 0a54 6578 7420  ........)..Text 
+00001450: 636c 6173 7369 6669 6361 7469 6f6e 2063  classification c
+00001460: 6f6d 7061 7469 626c 6520 7769 7468 2043  ompatible with C
+00001470: 6869 6e65 7365 2061 6e64 2045 6e67 6c69  hinese and Engli
+00001480: 7368 2063 6f72 706f 7261 2e0a 0a65 7861  sh corpora...exa
+00001490: 6d70 6c65 205b 6578 616d 706c 6573 2f6c  mple [examples/l
+000014a0: 725f 636c 6173 7369 6669 6361 7469 6f6e  r_classification
+000014b0: 5f64 656d 6f2e 7079 5d28 6874 7470 733a  _demo.py](https:
+000014c0: 2f2f 6769 7468 7562 2e63 6f6d 2f73 6869  //github.com/shi
+000014d0: 6269 6e67 3632 342f 7079 7465 7874 636c  bing624/pytextcl
+000014e0: 6173 7369 6669 6572 2f62 6c6f 622f 6d61  assifier/blob/ma
+000014f0: 7374 6572 2f65 7861 6d70 6c65 732f 6c72  ster/examples/lr
+00001500: 5f63 6c61 7373 6966 6963 6174 696f 6e5f  _classification_
+00001510: 6465 6d6f 2e70 7929 0a0a 6060 6070 7974  demo.py)..```pyt
+00001520: 686f 6e0a 696d 706f 7274 2073 7973 0a0a  hon.import sys..
+00001530: 7379 732e 7061 7468 2e61 7070 656e 6428  sys.path.append(
+00001540: 272e 2e27 290a 6672 6f6d 2070 7974 6578  '..').from pytex
+00001550: 7463 6c61 7373 6966 6965 7220 696d 706f  tclassifier impo
+00001560: 7274 2043 6c61 7373 6963 436c 6173 7369  rt ClassicClassi
+00001570: 6669 6572 0a0a 6966 205f 5f6e 616d 655f  fier..if __name_
+00001580: 5f20 3d3d 2027 5f5f 6d61 696e 5f5f 273a  _ == '__main__':
+00001590: 0a20 2020 206d 203d 2043 6c61 7373 6963  .    m = Classic
+000015a0: 436c 6173 7369 6669 6572 286f 7574 7075  Classifier(outpu
+000015b0: 745f 6469 723d 276d 6f64 656c 732f 6c72  t_dir='models/lr
+000015c0: 2d74 6f79 272c 206d 6f64 656c 5f6e 616d  -toy', model_nam
+000015d0: 655f 6f72 5f6d 6f64 656c 3d27 6c72 2729  e_or_model='lr')
+000015e0: 0a20 2020 2023 20e7 bb8f e585 b8e5 8886  .    # .........
+000015f0: e7b1 bbe6 96b9 e6b3 95ef bc8c e694 afe6  ................
+00001600: 8c81 e79a 84e6 a8a1 e59e 8be5 8c85 e68b  ................
+00001610: acef bc9a 6c72 2c20 7261 6e64 6f6d 5f66  ....lr, random_f
+00001620: 6f72 6573 742c 2064 6563 6973 696f 6e5f  orest, decision_
+00001630: 7472 6565 2c20 6b6e 6e2c 2062 6179 6573  tree, knn, bayes
+00001640: 2c20 7376 6d2c 2078 6762 6f6f 7374 0a20  , svm, xgboost. 
+00001650: 2020 2064 6174 6120 3d20 5b0a 2020 2020     data = [.    
+00001660: 2020 2020 2827 6564 7563 6174 696f 6e27      ('education'
+00001670: 2c20 27e5 908d e5b8 88e6 8c87 e5af bce6  , '.............
+00001680: 8998 e7a6 8fe8 afad e6b3 95e6 8a80 e5b7  ................
+00001690: a7ef bc9a e590 8de8 af8d e79a 84e5 a48d  ................
+000016a0: e695 b0e5 bda2 e5bc 8f27 292c 0a20 2020  .........'),.   
+000016b0: 2020 2020 2028 2765 6475 6361 7469 6f6e       ('education
+000016c0: 272c 2027 e4b8 ade5 9bbd e9ab 98e8 8083  ', '............
+000016d0: e688 90e7 bba9 e6b5 b7e5 a496 e8ae a4e5  ................
+000016e0: 8faf 20e6 98af e280 9ce7 8bbc e69d a5e4  .. .............
+000016f0: ba86 e280 9de5 9097 efbc 9f27 292c 0a20  ...........'),. 
+00001700: 2020 2020 2020 2028 2765 6475 6361 7469         ('educati
+00001710: 6f6e 272c 2027 e585 ace5 8aa1 e591 98e8  on', '..........
+00001720: 8083 e899 91e8 b68a e69d a5e8 b68a e590  ................
+00001730: 83e9 a699 efbc 8ce8 bf99 e698 afe6 808e  ................
+00001740: e4b9 88e5 9b9e e4ba 8bef bc9f 2729 2c0a  ............'),.
+00001750: 2020 2020 2020 2020 2827 7370 6f72 7473          ('sports
+00001760: 272c 2027 e59b bee6 9687 efbc 9ae6 b395  ', '............
+00001770: e7bd 91e5 ad9f e88f b2e5 b094 e696 afe8  ................
+00001780: 8ba6 e688 98e8 bf9b 3136 e5bc ba20 e5ad  ........16... ..
+00001790: 9fe8 8fb2 e5b0 94e6 96af e680 92e5 90bc  ................
+000017a0: 2729 2c0a 2020 2020 2020 2020 2827 7370  '),.        ('sp
+000017b0: 6f72 7473 272c 2027 e59b 9be5 b79d e4b8  orts', '........
+000017c0: b9e6 a3b1 e4b8 bee8 a18c e585 a8e5 9bbd  ................
+000017d0: e995 bfe8 b79d e799 bbe5 b1b1 e68c 91e6  ................
+000017e0: 8898 e8b5 9b20 e8bf 91e4 b887 e4ba bae5  ..... ..........
+000017f0: 8f82 e4b8 8e27 292c 0a20 2020 2020 2020  .....'),.       
+00001800: 2028 2773 706f 7274 7327 2c20 27e7 b1b3   ('sports', '...
+00001810: e585 b0e5 aea2 e59c ba38 e688 98e4 b88d  .........8......
+00001820: e8b4 a5e5 9bbd e7b1 b331 30e5 b9b4 e8bf  .........10.....
+00001830: 9ee8 839c 2729 2c0a 2020 2020 5d0a 2020  ....'),.    ].  
+00001840: 2020 6d2e 7472 6169 6e28 6461 7461 290a    m.train(data).
+00001850: 2020 2020 7072 696e 7428 6d29 0a20 2020      print(m).   
+00001860: 2023 206c 6f61 6420 6265 7374 206d 6f64   # load best mod
+00001870: 656c 2066 726f 6d20 6d6f 6465 6c5f 6469  el from model_di
+00001880: 720a 2020 2020 6d2e 6c6f 6164 5f6d 6f64  r.    m.load_mod
+00001890: 656c 2829 0a20 2020 2070 7265 6469 6374  el().    predict
+000018a0: 5f6c 6162 656c 2c20 7072 6564 6963 745f  _label, predict_
+000018b0: 7072 6f62 6120 3d20 6d2e 7072 6564 6963  proba = m.predic
+000018c0: 7428 5b27 e7a6 8fe5 bbba e698 a5e5 ada3  t(['............
+000018d0: e585 ace5 8aa1 e591 98e8 8083 e8af 95e6  ................
+000018e0: 8aa5 e590 8d31 38e6 97a5 e688 aae6 ada2  .....18.........
+000018f0: 2032 e69c 8836 e697 a5e8 8083 e8af 9527   2...6.........'
+00001900: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001930: 27e6 848f e794 b2e9 a696 e8bd aee8 a1a5  '...............
+00001940: e8b5 9be4 baa4 e688 98e8 aeb0 e5bd 953a  ...............:
+00001950: e7b1 b3e5 85b0 e5ae a2e5 9cba 38e6 8898  ............8...
+00001960: e4b8 8de8 b4a5 e59b bde7 b1b3 3130 e5b9  ............10..
+00001970: b4e8 bf9e e883 9c27 5d29 0a20 2020 2070  .......']).    p
+00001980: 7269 6e74 2866 2770 7265 6469 6374 5f6c  rint(f'predict_l
+00001990: 6162 656c 3a20 7b70 7265 6469 6374 5f6c  abel: {predict_l
+000019a0: 6162 656c 7d2c 2070 7265 6469 6374 5f70  abel}, predict_p
+000019b0: 726f 6261 3a20 7b70 7265 6469 6374 5f70  roba: {predict_p
+000019c0: 726f 6261 7d27 290a 0a20 2020 2074 6573  roba}')..    tes
+000019d0: 745f 6461 7461 203d 205b 0a20 2020 2020  t_data = [.     
+000019e0: 2020 2028 2765 6475 6361 7469 6f6e 272c     ('education',
+000019f0: 2027 e7a6 8fe5 bbba e698 a5e5 ada3 e585   '..............
+00001a00: ace5 8aa1 e591 98e8 8083 e8af 95e6 8aa5  ................
+00001a10: e590 8d31 38e6 97a5 e688 aae6 ada2 2032  ...18......... 2
+00001a20: e69c 8836 e697 a5e8 8083 e8af 9527 292c  ...6.........'),
+00001a30: 0a20 2020 2020 2020 2028 2773 706f 7274  .        ('sport
+00001a40: 7327 2c20 27e6 848f e794 b2e9 a696 e8bd  s', '...........
+00001a50: aee8 a1a5 e8b5 9be4 baa4 e688 98e8 aeb0  ................
+00001a60: e5bd 953a e7b1 b3e5 85b0 e5ae a2e5 9cba  ...:............
+00001a70: 38e6 8898 e4b8 8de8 b4a5 e59b bde7 b1b3  8...............
+00001a80: 3130 e5b9 b4e8 bf9e e883 9c27 292c 0a20  10.........'),. 
+00001a90: 2020 205d 0a20 2020 2061 6363 5f73 636f     ].    acc_sco
+00001aa0: 7265 203d 206d 2e65 7661 6c75 6174 655f  re = m.evaluate_
+00001ab0: 6d6f 6465 6c28 7465 7374 5f64 6174 6129  model(test_data)
+00001ac0: 0a20 2020 2070 7269 6e74 2866 2761 6363  .    print(f'acc
+00001ad0: 5f73 636f 7265 3a20 7b61 6363 5f73 636f  _score: {acc_sco
+00001ae0: 7265 7d27 2920 2023 2031 2e30 0a0a 2020  re}')  # 1.0..  
+00001af0: 2020 2323 2323 2074 7261 696e 206d 6f64    #### train mod
+00001b00: 656c 2077 6974 6820 3177 2064 6174 610a  el with 1w data.
+00001b10: 2020 2020 7072 696e 7428 272d 2720 2a20      print('-' * 
+00001b20: 3432 290a 2020 2020 6d20 3d20 436c 6173  42).    m = Clas
+00001b30: 7369 6343 6c61 7373 6966 6965 7228 6f75  sicClassifier(ou
+00001b40: 7470 7574 5f64 6972 3d27 6d6f 6465 6c73  tput_dir='models
+00001b50: 2f6c 7227 2c20 6d6f 6465 6c5f 6e61 6d65  /lr', model_name
+00001b60: 5f6f 725f 6d6f 6465 6c3d 276c 7227 290a  _or_model='lr').
+00001b70: 2020 2020 6461 7461 5f66 696c 6520 3d20      data_file = 
+00001b80: 2774 6875 636e 6577 735f 7472 6169 6e5f  'thucnews_train_
+00001b90: 3177 2e74 7874 270a 2020 2020 6d2e 7472  1w.txt'.    m.tr
+00001ba0: 6169 6e28 6461 7461 5f66 696c 6529 0a20  ain(data_file). 
+00001bb0: 2020 206d 2e6c 6f61 645f 6d6f 6465 6c28     m.load_model(
+00001bc0: 290a 2020 2020 7072 6564 6963 745f 6c61  ).    predict_la
+00001bd0: 6265 6c2c 2070 7265 6469 6374 5f70 726f  bel, predict_pro
+00001be0: 6261 203d 206d 2e70 7265 6469 6374 280a  ba = m.predict(.
+00001bf0: 2020 2020 2020 2020 5b27 e9a1 bae4 b989          ['......
+00001c00: e58c 97e4 baac e88b 8fe6 b4bb 3838 e5b9  ............88..
+00001c10: b3e7 b1b3 e8b5 b7e7 b2be e8a3 85e6 88bf  ................
+00001c20: e59c a8e5 94ae 272c 0a20 2020 2020 2020  ......',.       
+00001c30: 2020 27e7 be8e 4542 2d35 e9a1 b9e7 9bae    '...EB-5......
+00001c40: e280 9c31 35e6 97a5 e5bf abe9 809f e7a7  ...15...........
+00001c50: bbe6 b091 e280 9de5 b086 e68e a8e8 bf9f  ................
+00001c60: 275d 290a 2020 2020 7072 696e 7428 6627  ']).    print(f'
+00001c70: 7072 6564 6963 745f 6c61 6265 6c3a 207b  predict_label: {
+00001c80: 7072 6564 6963 745f 6c61 6265 6c7d 2c20  predict_label}, 
+00001c90: 7072 6564 6963 745f 7072 6f62 613a 207b  predict_proba: {
+00001ca0: 7072 6564 6963 745f 7072 6f62 617d 2729  predict_proba}')
+00001cb0: 0a60 6060 0a0a 6f75 7470 7574 3a0a 0a60  .```..output:..`
+00001cc0: 6060 0a43 6c61 7373 6963 436c 6173 7369  ``.ClassicClassi
+00001cd0: 6669 6572 2069 6e73 7461 6e63 6520 284c  fier instance (L
+00001ce0: 6f67 6973 7469 6352 6567 7265 7373 696f  ogisticRegressio
+00001cf0: 6e28 6669 745f 696e 7465 7263 6570 743d  n(fit_intercept=
+00001d00: 4661 6c73 6529 2c20 7374 6f70 776f 7264  False), stopword
+00001d10: 7320 7369 7a65 3a20 3234 3338 290a 7072  s size: 2438).pr
+00001d20: 6564 6963 745f 6c61 6265 6c3a 205b 2765  edict_label: ['e
+00001d30: 6475 6361 7469 6f6e 2720 2773 706f 7274  ducation' 'sport
+00001d40: 7327 5d2c 2070 7265 6469 6374 5f70 726f  s'], predict_pro
+00001d50: 6261 3a20 5b30 2e35 2c20 302e 3539 3839  ba: [0.5, 0.5989
+00001d60: 3431 3830 3637 3431 3533 345d 0a61 6363  41806741534].acc
+00001d70: 5f73 636f 7265 3a20 312e 300a 2d2d 2d2d  _score: 1.0.----
+00001d80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001d90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001da0: 2d2d 2d2d 2d2d 0a70 7265 6469 6374 5f6c  ------.predict_l
+00001db0: 6162 656c 3a20 5b27 7265 616c 7479 2720  abel: ['realty' 
+00001dc0: 2765 6475 6361 7469 6f6e 275d 2c20 7072  'education'], pr
+00001dd0: 6564 6963 745f 7072 6f62 613a 205b 302e  edict_proba: [0.
+00001de0: 3733 3032 3935 3639 3233 3631 3733 3732  7302956923617372
+00001df0: 2c20 302e 3235 3635 3030 3534 3435 3332  , 0.256500544532
+00001e00: 3239 3233 5d0a 6060 600a 0a23 2323 2056  2923].```..### V
+00001e10: 6973 7561 6c20 4665 6174 7572 6520 496d  isual Feature Im
+00001e20: 706f 7274 616e 6365 0a0a 5368 6f77 2066  portance..Show f
+00001e30: 6561 7475 7265 2077 6569 6768 7473 206f  eature weights o
+00001e40: 6620 6d6f 6465 6c2c 2061 6e64 2070 7265  f model, and pre
+00001e50: 6469 6374 696f 6e20 776f 7264 2077 6569  diction word wei
+00001e60: 6768 742c 2066 6f72 2065 7861 6d70 6c65  ght, for example
+00001e70: 205b 6578 616d 706c 6573 2f76 6973 7561   [examples/visua
+00001e80: 6c5f 6665 6174 7572 655f 696d 706f 7274  l_feature_import
+00001e90: 616e 6365 2e69 7079 6e62 5d28 6874 7470  ance.ipynb](http
+00001ea0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
+00001eb0: 6869 6269 6e67 3632 342f 7079 7465 7874  hibing624/pytext
+00001ec0: 636c 6173 7369 6669 6572 2f62 6c6f 622f  classifier/blob/
+00001ed0: 6d61 7374 6572 2f65 7861 6d70 6c65 732f  master/examples/
+00001ee0: 7669 7375 616c 5f66 6561 7475 7265 5f69  visual_feature_i
+00001ef0: 6d70 6f72 7461 6e63 652e 6970 796e 6229  mportance.ipynb)
+00001f00: 0a0a 6060 6070 7974 686f 6e0a 696d 706f  ..```python.impo
+00001f10: 7274 2073 7973 0a0a 7379 732e 7061 7468  rt sys..sys.path
+00001f20: 2e61 7070 656e 6428 272e 2e27 290a 6672  .append('..').fr
+00001f30: 6f6d 2070 7974 6578 7463 6c61 7373 6966  om pytextclassif
+00001f40: 6965 7220 696d 706f 7274 2043 6c61 7373  ier import Class
+00001f50: 6963 436c 6173 7369 6669 6572 0a69 6d70  icClassifier.imp
+00001f60: 6f72 7420 6a69 6562 610a 0a74 6320 3d20  ort jieba..tc = 
+00001f70: 436c 6173 7369 6343 6c61 7373 6966 6965  ClassicClassifie
+00001f80: 7228 6f75 7470 7574 5f64 6972 3d27 6d6f  r(output_dir='mo
+00001f90: 6465 6c73 2f6c 722d 746f 7927 2c20 6d6f  dels/lr-toy', mo
+00001fa0: 6465 6c5f 6e61 6d65 5f6f 725f 6d6f 6465  del_name_or_mode
+00001fb0: 6c3d 276c 7227 290a 6461 7461 203d 205b  l='lr').data = [
+00001fc0: 0a20 2020 2028 2765 6475 6361 7469 6f6e  .    ('education
+00001fd0: 272c 2027 e590 8de5 b888 e68c 87e5 afbc  ', '............
+00001fe0: e689 98e7 a68f e8af ade6 b395 e68a 80e5  ................
+00001ff0: b7a7 efbc 9ae5 908d e8af 8de7 9a84 e5a4  ................
+00002000: 8de6 95b0 e5bd a2e5 bc8f 2729 2c0a 2020  ..........'),.  
+00002010: 2020 2827 6564 7563 6174 696f 6e27 2c20    ('education', 
+00002020: 27e4 b8ad e59b bde9 ab98 e880 83e6 8890  '...............
+00002030: e7bb a9e6 b5b7 e5a4 96e8 aea4 e58f af20  ............... 
+00002040: e698 afe2 809c e78b bce6 9da5 e4ba 86e2  ................
+00002050: 809d e590 97ef bc9f 2729 2c0a 2020 2020  ........'),.    
+00002060: 2827 7370 6f72 7473 272c 2027 e59b bee6  ('sports', '....
+00002070: 9687 efbc 9ae6 b395 e7bd 91e5 ad9f e88f  ................
+00002080: b2e5 b094 e696 afe8 8ba6 e688 98e8 bf9b  ................
+00002090: 3136 e5bc ba20 e5ad 9fe8 8fb2 e5b0 94e6  16... ..........
+000020a0: 96af e680 92e5 90bc 2729 2c0a 2020 2020  ........'),.    
+000020b0: 2827 7370 6f72 7473 272c 2027 e59b 9be5  ('sports', '....
+000020c0: b79d e4b8 b9e6 a3b1 e4b8 bee8 a18c e585  ................
+000020d0: a8e5 9bbd e995 bfe8 b79d e799 bbe5 b1b1  ................
+000020e0: e68c 91e6 8898 e8b5 9b20 e8bf 91e4 b887  ......... ......
+000020f0: e4ba bae5 8f82 e4b8 8e27 292c 0a20 2020  .........'),.   
+00002100: 2028 2773 706f 7274 7327 2c20 27e7 b1b3   ('sports', '...
+00002110: e585 b0e5 aea2 e59c ba38 e688 98e4 b88d  .........8......
+00002120: e8b4 a5e5 9bbd e7b1 b331 30e5 b9b4 e8bf  .........10.....
+00002130: 9ee8 839c 2729 0a5d 0a74 632e 7472 6169  ....').].tc.trai
+00002140: 6e28 6461 7461 290a 696d 706f 7274 2065  n(data).import e
+00002150: 6c69 350a 0a69 6e66 6572 5f64 6174 6120  li5..infer_data 
+00002160: 3d20 5b27 e9ab 98e8 8083 e68c 87e5 afbc  = ['............
+00002170: e689 98e7 a68f e8af ade6 b395 e68a 80e5  ................
+00002180: b7a7 e59b bde9 9985 e8ae a4e5 8faf 272c  ..............',
+00002190: 0a20 2020 2020 2020 2020 2020 2020 2027  .              '
+000021a0: e684 8fe7 94b2 e9a6 96e8 bdae e8a1 a5e8  ................
+000021b0: b59b e4ba a4e6 8898 e8ae b0e5 bd95 3ae7  ..............:.
+000021c0: b1b3 e585 b0e5 aea2 e59c ba38 e688 98e4  ...........8....
+000021d0: b88d e8b4 a5e5 9bbd e7b1 b331 30e5 b9b4  ...........10...
+000021e0: e8bf 9ee8 839c 275d 0a65 6c69 352e 7368  ......'].eli5.sh
+000021f0: 6f77 5f77 6569 6768 7473 2874 632e 6d6f  ow_weights(tc.mo
+00002200: 6465 6c2c 2076 6563 3d74 632e 6665 6174  del, vec=tc.feat
+00002210: 7572 6529 0a73 6567 5f69 6e66 6572 5f64  ure).seg_infer_d
+00002220: 6174 6120 3d20 5b27 2027 2e6a 6f69 6e28  ata = [' '.join(
+00002230: 6a69 6562 612e 6c63 7574 2869 2929 2066  jieba.lcut(i)) f
+00002240: 6f72 2069 2069 6e20 696e 6665 725f 6461  or i in infer_da
+00002250: 7461 5d0a 656c 6935 2e73 686f 775f 7072  ta].eli5.show_pr
+00002260: 6564 6963 7469 6f6e 2874 632e 6d6f 6465  ediction(tc.mode
+00002270: 6c2c 2073 6567 5f69 6e66 6572 5f64 6174  l, seg_infer_dat
+00002280: 615b 305d 2c20 7665 633d 7463 2e66 6561  a[0], vec=tc.fea
+00002290: 7475 7265 2c0a 2020 2020 2020 2020 2020  ture,.          
+000022a0: 2020 2020 2020 2020 2020 2074 6172 6765             targe
+000022b0: 745f 6e61 6d65 733d 5b27 6564 7563 6174  t_names=['educat
+000022c0: 696f 6e27 2c20 2773 706f 7274 7327 5d29  ion', 'sports'])
+000022d0: 0a60 6060 0a0a 6f75 7470 7574 3a0a 0a21  .```..output:..!
+000022e0: 5b69 6d67 2e70 6e67 5d28 646f 6373 2f69  [img.png](docs/i
+000022f0: 6d67 2e70 6e67 290a 0a23 2323 2044 6565  mg.png)..### Dee
+00002300: 7020 436c 6173 7369 6669 6361 7469 6f6e  p Classification
+00002310: 206d 6f64 656c 0a0a e69c ace9 a1b9 e79b   model..........
+00002320: aee6 94af e68c 81e4 bba5 e4b8 8be6 b7b1  ................
+00002330: e5ba a6e5 8886 e7b1 bbe6 a8a1 e59e 8bef  ................
+00002340: bc9a 4661 7374 5465 7874 e380 8154 6578  ..FastText...Tex
+00002350: 7443 4e4e e380 8154 6578 7452 4e4e e380  tCNN...TextRNN..
+00002360: 8142 6572 74e6 a8a1 e59e 8bef bc8c 6069  .Bert.........`i
+00002370: 6d70 6f72 7460 e6a8 a1e5 9e8b e5af b9e5  mport`..........
+00002380: ba94 e79a 84e6 96b9 e6b3 95e6 9da5 e8b0  ................
+00002390: 83e7 94a8 efbc 9a0a 6060 6070 7974 686f  ........```pytho
+000023a0: 6e0a 6672 6f6d 2070 7974 6578 7463 6c61  n.from pytextcla
+000023b0: 7373 6966 6965 7220 696d 706f 7274 2046  ssifier import F
+000023c0: 6173 7454 6578 7443 6c61 7373 6966 6965  astTextClassifie
+000023d0: 722c 2054 6578 7443 4e4e 436c 6173 7369  r, TextCNNClassi
+000023e0: 6669 6572 2c20 5465 7874 524e 4e43 6c61  fier, TextRNNCla
+000023f0: 7373 6966 6965 722c 2042 6572 7443 6c61  ssifier, BertCla
+00002400: 7373 6966 6965 720a 6060 600a 0ae4 b88b  ssifier.```.....
+00002410: e99d a2e4 bba5 4661 7374 5465 7874 e6a8  ......FastText..
+00002420: a1e5 9e8b e4b8 bae7 a4ba e4be 8bef bc8c  ................
+00002430: e585 b6e4 bb96 e6a8 a1e5 9e8b e79a 84e4  ................
+00002440: bdbf e794 a8e6 96b9 e6b3 95e7 b1bb e4bc  ................
+00002450: bce3 8082 0a0a 2323 2320 4661 7374 5465  ......### FastTe
+00002460: 7874 20e6 a8a1 e59e 8b0a 0ae8 aead e7bb  xt .............
+00002470: 83e5 928c e9a2 84e6 b58b 6046 6173 7454  ..........`FastT
+00002480: 6578 7460 e6a8 a1e5 9e8b e7a4 bae4 be8b  ext`............
+00002490: 5b65 7861 6d70 6c65 732f 6661 7374 7465  [examples/fastte
+000024a0: 7874 5f63 6c61 7373 6966 6963 6174 696f  xt_classificatio
+000024b0: 6e5f 6465 6d6f 2e70 795d 2868 7474 7073  n_demo.py](https
+000024c0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7368  ://github.com/sh
+000024d0: 6962 696e 6736 3234 2f70 7974 6578 7463  ibing624/pytextc
+000024e0: 6c61 7373 6966 6965 722f 626c 6f62 2f6d  lassifier/blob/m
+000024f0: 6173 7465 722f 6578 616d 706c 6573 2f66  aster/examples/f
+00002500: 6173 7474 6578 745f 636c 6173 7369 6669  asttext_classifi
+00002510: 6361 7469 6f6e 5f64 656d 6f2e 7079 290a  cation_demo.py).
+00002520: 0a60 6060 7079 7468 6f6e 0a69 6d70 6f72  .```python.impor
+00002530: 7420 7379 730a 0a73 7973 2e70 6174 682e  t sys..sys.path.
+00002540: 6170 7065 6e64 2827 2e2e 2729 0a66 726f  append('..').fro
+00002550: 6d20 7079 7465 7874 636c 6173 7369 6669  m pytextclassifi
+00002560: 6572 2069 6d70 6f72 7420 4661 7374 5465  er import FastTe
+00002570: 7874 436c 6173 7369 6669 6572 2c20 6c6f  xtClassifier, lo
+00002580: 6164 5f64 6174 610a 0a69 6620 5f5f 6e61  ad_data..if __na
+00002590: 6d65 5f5f 203d 3d20 275f 5f6d 6169 6e5f  me__ == '__main_
+000025a0: 5f27 3a0a 2020 2020 6d20 3d20 4661 7374  _':.    m = Fast
+000025b0: 5465 7874 436c 6173 7369 6669 6572 286f  TextClassifier(o
+000025c0: 7574 7075 745f 6469 723d 276d 6f64 656c  utput_dir='model
+000025d0: 732f 6661 7374 7465 7874 2d74 6f79 2729  s/fasttext-toy')
+000025e0: 0a20 2020 2064 6174 6120 3d20 5b0a 2020  .    data = [.  
+000025f0: 2020 2020 2020 2827 6564 7563 6174 696f        ('educatio
+00002600: 6e27 2c20 27e5 908d e5b8 88e6 8c87 e5af  n', '...........
+00002610: bce6 8998 e7a6 8fe8 afad e6b3 95e6 8a80  ................
+00002620: e5b7 a7ef bc9a e590 8de8 af8d e79a 84e5  ................
+00002630: a48d e695 b0e5 bda2 e5bc 8f27 292c 0a20  ...........'),. 
+00002640: 2020 2020 2020 2028 2765 6475 6361 7469         ('educati
+00002650: 6f6e 272c 2027 e4b8 ade5 9bbd e9ab 98e8  on', '..........
+00002660: 8083 e688 90e7 bba9 e6b5 b7e5 a496 e8ae  ................
+00002670: a4e5 8faf 20e6 98af e280 9ce7 8bbc e69d  .... ...........
+00002680: a5e4 ba86 e280 9de5 9097 efbc 9f27 292c  .............'),
+00002690: 0a20 2020 2020 2020 2028 2765 6475 6361  .        ('educa
+000026a0: 7469 6f6e 272c 2027 e585 ace5 8aa1 e591  tion', '........
+000026b0: 98e8 8083 e899 91e8 b68a e69d a5e8 b68a  ................
+000026c0: e590 83e9 a699 efbc 8ce8 bf99 e698 afe6  ................
+000026d0: 808e e4b9 88e5 9b9e e4ba 8bef bc9f 2729  ..............')
+000026e0: 2c0a 2020 2020 2020 2020 2827 7370 6f72  ,.        ('spor
+000026f0: 7473 272c 2027 e59b bee6 9687 efbc 9ae6  ts', '..........
+00002700: b395 e7bd 91e5 ad9f e88f b2e5 b094 e696  ................
+00002710: afe8 8ba6 e688 98e8 bf9b 3136 e5bc ba20  ..........16... 
+00002720: e5ad 9fe8 8fb2 e5b0 94e6 96af e680 92e5  ................
+00002730: 90bc 2729 2c0a 2020 2020 2020 2020 2827  ..'),.        ('
+00002740: 7370 6f72 7473 272c 2027 e59b 9be5 b79d  sports', '......
+00002750: e4b8 b9e6 a3b1 e4b8 bee8 a18c e585 a8e5  ................
+00002760: 9bbd e995 bfe8 b79d e799 bbe5 b1b1 e68c  ................
+00002770: 91e6 8898 e8b5 9b20 e8bf 91e4 b887 e4ba  ....... ........
+00002780: bae5 8f82 e4b8 8e27 292c 0a20 2020 2020  .......'),.     
+00002790: 2020 2028 2773 706f 7274 7327 2c20 27e7     ('sports', '.
+000027a0: b1b3 e585 b0e5 aea2 e59c ba38 e688 98e4  ...........8....
+000027b0: b88d e8b4 a5e4 bf9d e68c 81e8 bf9e e883  ................
+000027c0: 9c27 292c 0a20 2020 205d 0a20 2020 206d  .'),.    ].    m
+000027d0: 2e74 7261 696e 2864 6174 612c 206e 756d  .train(data, num
+000027e0: 5f65 706f 6368 733d 3329 0a20 2020 2070  _epochs=3).    p
+000027f0: 7269 6e74 286d 290a 2020 2020 2320 6c6f  rint(m).    # lo
+00002800: 6164 2074 7261 696e 6564 2062 6573 7420  ad trained best 
+00002810: 6d6f 6465 6c0a 2020 2020 6d2e 6c6f 6164  model.    m.load
+00002820: 5f6d 6f64 656c 2829 0a20 2020 2070 7265  _model().    pre
+00002830: 6469 6374 5f6c 6162 656c 2c20 7072 6564  dict_label, pred
+00002840: 6963 745f 7072 6f62 6120 3d20 6d2e 7072  ict_proba = m.pr
+00002850: 6564 6963 7428 5b27 e7a6 8fe5 bbba e698  edict(['........
+00002860: a5e5 ada3 e585 ace5 8aa1 e591 98e8 8083  ................
+00002870: e8af 95e6 8aa5 e590 8d31 38e6 97a5 e688  .........18.....
+00002880: aae6 ada2 2032 e69c 8836 e697 a5e8 8083  .... 2...6......
+00002890: e8af 9527 2c0a 2020 2020 2020 2020 2020  ...',.          
+000028a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028c0: 2020 2020 27e6 848f e794 b2e9 a696 e8bd      '...........
+000028d0: aee8 a1a5 e8b5 9be4 baa4 e688 98e8 aeb0  ................
+000028e0: e5bd 953a e7b1 b3e5 85b0 e5ae a2e5 9cba  ...:............
+000028f0: 38e6 8898 e4b8 8de8 b4a5 e59b bde7 b1b3  8...............
+00002900: 3130 e5b9 b4e8 bf9e e883 9c27 5d29 0a20  10.........']). 
+00002910: 2020 2070 7269 6e74 2866 2770 7265 6469     print(f'predi
+00002920: 6374 5f6c 6162 656c 3a20 7b70 7265 6469  ct_label: {predi
+00002930: 6374 5f6c 6162 656c 7d2c 2070 7265 6469  ct_label}, predi
+00002940: 6374 5f70 726f 6261 3a20 7b70 7265 6469  ct_proba: {predi
+00002950: 6374 5f70 726f 6261 7d27 290a 2020 2020  ct_proba}').    
+00002960: 7465 7374 5f64 6174 6120 3d20 5b0a 2020  test_data = [.  
+00002970: 2020 2020 2020 2827 6564 7563 6174 696f        ('educatio
+00002980: 6e27 2c20 27e7 a68f e5bb bae6 98a5 e5ad  n', '...........
+00002990: a3e5 85ac e58a a1e5 9198 e880 83e8 af95  ................
+000029a0: e68a a5e5 908d 3138 e697 a5e6 88aa e6ad  ......18........
+000029b0: a220 32e6 9c88 36e6 97a5 e880 83e8 af95  . 2...6.........
+000029c0: 2729 2c0a 2020 2020 2020 2020 2827 7370  '),.        ('sp
+000029d0: 6f72 7473 272c 2027 e684 8fe7 94b2 e9a6  orts', '........
+000029e0: 96e8 bdae e8a1 a5e8 b59b e4ba a4e6 8898  ................
+000029f0: e8ae b0e5 bd95 3ae7 b1b3 e585 b0e5 aea2  ......:.........
+00002a00: e59c ba38 e688 98e4 b88d e8b4 a5e5 9bbd  ...8............
+00002a10: e7b1 b331 30e5 b9b4 e8bf 9ee8 839c 2729  ...10.........')
+00002a20: 2c0a 2020 2020 5d0a 2020 2020 6163 635f  ,.    ].    acc_
+00002a30: 7363 6f72 6520 3d20 6d2e 6576 616c 7561  score = m.evalua
+00002a40: 7465 5f6d 6f64 656c 2874 6573 745f 6461  te_model(test_da
+00002a50: 7461 290a 2020 2020 7072 696e 7428 6627  ta).    print(f'
+00002a60: 6163 635f 7363 6f72 653a 207b 6163 635f  acc_score: {acc_
+00002a70: 7363 6f72 657d 2729 2020 2320 312e 300a  score}')  # 1.0.
+00002a80: 0a20 2020 2023 2323 2320 7472 6169 6e20  .    #### train 
+00002a90: 6d6f 6465 6c20 7769 7468 2031 7720 6461  model with 1w da
+00002aa0: 7461 0a20 2020 2070 7269 6e74 2827 2d27  ta.    print('-'
+00002ab0: 202a 2034 3229 0a20 2020 2064 6174 615f   * 42).    data_
+00002ac0: 6669 6c65 203d 2027 7468 7563 6e65 7773  file = 'thucnews
+00002ad0: 5f74 7261 696e 5f31 772e 7478 7427 0a20  _train_1w.txt'. 
+00002ae0: 2020 206d 203d 2046 6173 7454 6578 7443     m = FastTextC
+00002af0: 6c61 7373 6966 6965 7228 6f75 7470 7574  lassifier(output
+00002b00: 5f64 6972 3d27 6d6f 6465 6c73 2f66 6173  _dir='models/fas
+00002b10: 7474 6578 7427 290a 2020 2020 6d2e 7472  ttext').    m.tr
+00002b20: 6169 6e28 6461 7461 5f66 696c 652c 206e  ain(data_file, n
+00002b30: 616d 6573 3d28 276c 6162 656c 7327 2c20  ames=('labels', 
+00002b40: 2774 6578 7427 292c 206e 756d 5f65 706f  'text'), num_epo
+00002b50: 6368 733d 3329 0a20 2020 2023 206c 6f61  chs=3).    # loa
+00002b60: 6420 6265 7374 2074 7261 696e 6564 206d  d best trained m
+00002b70: 6f64 656c 2066 726f 6d20 6d6f 6465 6c5f  odel from model_
+00002b80: 6469 720a 2020 2020 6d2e 6c6f 6164 5f6d  dir.    m.load_m
+00002b90: 6f64 656c 2829 0a20 2020 2070 7265 6469  odel().    predi
+00002ba0: 6374 5f6c 6162 656c 2c20 7072 6564 6963  ct_label, predic
+00002bb0: 745f 7072 6f62 6120 3d20 6d2e 7072 6564  t_proba = m.pred
+00002bc0: 6963 7428 0a20 2020 2020 2020 205b 27e9  ict(.        ['.
+00002bd0: a1ba e4b9 89e5 8c97 e4ba ace8 8b8f e6b4  ................
+00002be0: bb38 38e5 b9b3 e7b1 b3e8 b5b7 e7b2 bee8  .88.............
+00002bf0: a385 e688 bfe5 9ca8 e594 ae27 2c0a 2020  ...........',.  
+00002c00: 2020 2020 2020 2027 e7be 8e45 422d 35e9         '...EB-5.
+00002c10: a1b9 e79b aee2 809c 3135 e697 a5e5 bfab  ........15......
+00002c20: e980 9fe7 a7bb e6b0 91e2 809d e5b0 86e6  ................
+00002c30: 8ea8 e8bf 9f27 5d0a 2020 2020 290a 2020  .....'].    ).  
+00002c40: 2020 7072 696e 7428 6627 7072 6564 6963    print(f'predic
+00002c50: 745f 6c61 6265 6c3a 207b 7072 6564 6963  t_label: {predic
+00002c60: 745f 6c61 6265 6c7d 2c20 7072 6564 6963  t_label}, predic
+00002c70: 745f 7072 6f62 613a 207b 7072 6564 6963  t_proba: {predic
+00002c80: 745f 7072 6f62 617d 2729 0a20 2020 2078  t_proba}').    x
+00002c90: 2c20 792c 2064 6620 3d20 6c6f 6164 5f64  , y, df = load_d
+00002ca0: 6174 6128 6461 7461 5f66 696c 6529 0a20  ata(data_file). 
+00002cb0: 2020 2074 6573 745f 6461 7461 203d 2064     test_data = d
+00002cc0: 665b 3a31 3030 5d0a 2020 2020 6163 635f  f[:100].    acc_
+00002cd0: 7363 6f72 6520 3d20 6d2e 6576 616c 7561  score = m.evalua
+00002ce0: 7465 5f6d 6f64 656c 2874 6573 745f 6461  te_model(test_da
+00002cf0: 7461 290a 2020 2020 7072 696e 7428 6627  ta).    print(f'
+00002d00: 6163 635f 7363 6f72 653a 207b 6163 635f  acc_score: {acc_
+00002d10: 7363 6f72 657d 2729 0a60 6060 0a0a 2323  score}').```..##
+00002d20: 2320 4245 5254 20e7 b1bb e6a8 a1e5 9e8b  # BERT .........
+00002d30: 0a0a 2323 2323 20e5 a49a e588 86e7 b1bb  ..#### .........
+00002d40: e6a8 a1e5 9e8b 0ae8 aead e7bb 83e5 928c  ................
+00002d50: e9a2 84e6 b58b 6042 4552 5460 e5a4 9ae5  ......`BERT`....
+00002d60: 8886 e7b1 bbe6 a8a1 e59e 8bef bc8c e7a4  ................
+00002d70: bae4 be8b 5b65 7861 6d70 6c65 732f 6265  ....[examples/be
+00002d80: 7274 5f63 6c61 7373 6966 6963 6174 696f  rt_classificatio
+00002d90: 6e5f 7a68 5f64 656d 6f2e 7079 5d28 6874  n_zh_demo.py](ht
+00002da0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00002db0: 2f73 6869 6269 6e67 3632 342f 7079 7465  /shibing624/pyte
+00002dc0: 7874 636c 6173 7369 6669 6572 2f62 6c6f  xtclassifier/blo
+00002dd0: 622f 6d61 7374 6572 2f65 7861 6d70 6c65  b/master/example
+00002de0: 732f 6265 7274 5f63 6c61 7373 6966 6963  s/bert_classific
+00002df0: 6174 696f 6e5f 7a68 5f64 656d 6f2e 7079  ation_zh_demo.py
+00002e00: 290a 0a60 6060 7079 7468 6f6e 0a69 6d70  )..```python.imp
+00002e10: 6f72 7420 7379 730a 0a73 7973 2e70 6174  ort sys..sys.pat
+00002e20: 682e 6170 7065 6e64 2827 2e2e 2729 0a66  h.append('..').f
+00002e30: 726f 6d20 7079 7465 7874 636c 6173 7369  rom pytextclassi
+00002e40: 6669 6572 2069 6d70 6f72 7420 4265 7274  fier import Bert
+00002e50: 436c 6173 7369 6669 6572 0a0a 6966 205f  Classifier..if _
+00002e60: 5f6e 616d 655f 5f20 3d3d 2027 5f5f 6d61  _name__ == '__ma
+00002e70: 696e 5f5f 273a 0a20 2020 206d 203d 2042  in__':.    m = B
+00002e80: 6572 7443 6c61 7373 6966 6965 7228 6f75  ertClassifier(ou
+00002e90: 7470 7574 5f64 6972 3d27 6d6f 6465 6c73  tput_dir='models
+00002ea0: 2f62 6572 742d 6368 696e 6573 652d 746f  /bert-chinese-to
+00002eb0: 7927 2c20 6e75 6d5f 636c 6173 7365 733d  y', num_classes=
+00002ec0: 322c 0a20 2020 2020 2020 2020 2020 2020  2,.             
+00002ed0: 2020 2020 2020 2020 2020 6d6f 6465 6c5f            model_
+00002ee0: 7479 7065 3d27 6265 7274 272c 206d 6f64  type='bert', mod
+00002ef0: 656c 5f6e 616d 653d 2762 6572 742d 6261  el_name='bert-ba
+00002f00: 7365 2d63 6869 6e65 7365 272c 206e 756d  se-chinese', num
+00002f10: 5f65 706f 6368 733d 3229 0a20 2020 2023  _epochs=2).    #
+00002f20: 206d 6f64 656c 5f74 7970 653a 2073 7570   model_type: sup
+00002f30: 706f 7274 2027 6265 7274 272c 2027 616c  port 'bert', 'al
+00002f40: 6265 7274 272c 2027 726f 6265 7274 6127  bert', 'roberta'
+00002f50: 2c20 2778 6c6e 6574 270a 2020 2020 2320  , 'xlnet'.    # 
+00002f60: 6d6f 6465 6c5f 6e61 6d65 3a20 7375 7070  model_name: supp
+00002f70: 6f72 7420 2762 6572 742d 6261 7365 2d63  ort 'bert-base-c
+00002f80: 6869 6e65 7365 272c 2027 6265 7274 2d62  hinese', 'bert-b
+00002f90: 6173 652d 6361 7365 6427 2c20 2762 6572  ase-cased', 'ber
+00002fa0: 742d 6261 7365 2d6d 756c 7469 6c69 6e67  t-base-multiling
+00002fb0: 7561 6c2d 6361 7365 6427 202e 2e2e 0a20  ual-cased' .... 
+00002fc0: 2020 2064 6174 6120 3d20 5b0a 2020 2020     data = [.    
+00002fd0: 2020 2020 2827 6564 7563 6174 696f 6e27      ('education'
+00002fe0: 2c20 27e5 908d e5b8 88e6 8c87 e5af bce6  , '.............
+00002ff0: 8998 e7a6 8fe8 afad e6b3 95e6 8a80 e5b7  ................
+00003000: a7ef bc9a e590 8de8 af8d e79a 84e5 a48d  ................
+00003010: e695 b0e5 bda2 e5bc 8f27 292c 0a20 2020  .........'),.   
+00003020: 2020 2020 2028 2765 6475 6361 7469 6f6e       ('education
+00003030: 272c 2027 e4b8 ade5 9bbd e9ab 98e8 8083  ', '............
+00003040: e688 90e7 bba9 e6b5 b7e5 a496 e8ae a4e5  ................
+00003050: 8faf 20e6 98af e280 9ce7 8bbc e69d a5e4  .. .............
+00003060: ba86 e280 9de5 9097 efbc 9f27 292c 0a20  ...........'),. 
+00003070: 2020 2020 2020 2028 2765 6475 6361 7469         ('educati
+00003080: 6f6e 272c 2027 e585 ace5 8aa1 e591 98e8  on', '..........
+00003090: 8083 e899 91e8 b68a e69d a5e8 b68a e590  ................
+000030a0: 83e9 a699 efbc 8ce8 bf99 e698 afe6 808e  ................
+000030b0: e4b9 88e5 9b9e e4ba 8bef bc9f 2729 2c0a  ............'),.
+000030c0: 2020 2020 2020 2020 2827 7370 6f72 7473          ('sports
+000030d0: 272c 2027 e59b bee6 9687 efbc 9ae6 b395  ', '............
+000030e0: e7bd 91e5 ad9f e88f b2e5 b094 e696 afe8  ................
+000030f0: 8ba6 e688 98e8 bf9b 3136 e5bc ba20 e5ad  ........16... ..
+00003100: 9fe8 8fb2 e5b0 94e6 96af e680 92e5 90bc  ................
+00003110: 2729 2c0a 2020 2020 2020 2020 2827 7370  '),.        ('sp
+00003120: 6f72 7473 272c 2027 e59b 9be5 b79d e4b8  orts', '........
+00003130: b9e6 a3b1 e4b8 bee8 a18c e585 a8e5 9bbd  ................
+00003140: e995 bfe8 b79d e799 bbe5 b1b1 e68c 91e6  ................
+00003150: 8898 e8b5 9b20 e8bf 91e4 b887 e4ba bae5  ..... ..........
+00003160: 8f82 e4b8 8e27 292c 0a20 2020 2020 2020  .....'),.       
+00003170: 2028 2773 706f 7274 7327 2c20 27e7 b1b3   ('sports', '...
+00003180: e585 b0e5 aea2 e59c ba38 e688 98e4 b88d  .........8......
+00003190: e8b4 a5e5 9bbd e7b1 b331 30e5 b9b4 e8bf  .........10.....
+000031a0: 9ee8 839c 2729 2c0a 2020 2020 5d0a 2020  ....'),.    ].  
+000031b0: 2020 6d2e 7472 6169 6e28 6461 7461 290a    m.train(data).
+000031c0: 2020 2020 7072 696e 7428 6d29 0a20 2020      print(m).   
+000031d0: 2023 206c 6f61 6420 7472 6169 6e65 6420   # load trained 
+000031e0: 6265 7374 206d 6f64 656c 2066 726f 6d20  best model from 
+000031f0: 6d6f 6465 6c5f 6469 720a 2020 2020 6d2e  model_dir.    m.
+00003200: 6c6f 6164 5f6d 6f64 656c 2829 0a20 2020  load_model().   
+00003210: 2070 7265 6469 6374 5f6c 6162 656c 2c20   predict_label, 
+00003220: 7072 6564 6963 745f 7072 6f62 6120 3d20  predict_proba = 
+00003230: 6d2e 7072 6564 6963 7428 5b27 e7a6 8fe5  m.predict(['....
+00003240: bbba e698 a5e5 ada3 e585 ace5 8aa1 e591  ................
+00003250: 98e8 8083 e8af 95e6 8aa5 e590 8d31 38e6  .............18.
+00003260: 97a5 e688 aae6 ada2 2032 e69c 8836 e697  ........ 2...6..
+00003270: a5e8 8083 e8af 9527 2c0a 2020 2020 2020  .......',.      
+00003280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000032a0: 2020 2020 2020 2020 27e6 848f e794 b2e9          '.......
+000032b0: a696 e8bd aee8 a1a5 e8b5 9be4 baa4 e688  ................
+000032c0: 98e8 aeb0 e5bd 953a e7b1 b3e5 85b0 e5ae  .......:........
+000032d0: a2e5 9cba 38e6 8898 e4b8 8de8 b4a5 e59b  ....8...........
+000032e0: bde7 b1b3 3130 e5b9 b4e8 bf9e e883 9c27  ....10.........'
+000032f0: 5d29 0a20 2020 2070 7269 6e74 2866 2770  ]).    print(f'p
+00003300: 7265 6469 6374 5f6c 6162 656c 3a20 7b70  redict_label: {p
+00003310: 7265 6469 6374 5f6c 6162 656c 7d2c 2070  redict_label}, p
+00003320: 7265 6469 6374 5f70 726f 6261 3a20 7b70  redict_proba: {p
+00003330: 7265 6469 6374 5f70 726f 6261 7d27 290a  redict_proba}').
+00003340: 0a20 2020 2074 6573 745f 6461 7461 203d  .    test_data =
+00003350: 205b 0a20 2020 2020 2020 2028 2765 6475   [.        ('edu
+00003360: 6361 7469 6f6e 272c 2027 e7a6 8fe5 bbba  cation', '......
+00003370: e698 a5e5 ada3 e585 ace5 8aa1 e591 98e8  ................
+00003380: 8083 e8af 95e6 8aa5 e590 8d31 38e6 97a5  ...........18...
+00003390: e688 aae6 ada2 2032 e69c 8836 e697 a5e8  ...... 2...6....
+000033a0: 8083 e8af 9527 292c 0a20 2020 2020 2020  .....'),.       
+000033b0: 2028 2773 706f 7274 7327 2c20 27e6 848f   ('sports', '...
+000033c0: e794 b2e9 a696 e8bd aee8 a1a5 e8b5 9be4  ................
+000033d0: baa4 e688 98e8 aeb0 e5bd 953a e7b1 b3e5  ...........:....
+000033e0: 85b0 e5ae a2e5 9cba 38e6 8898 e4b8 8de8  ........8.......
+000033f0: b4a5 e59b bde7 b1b3 3130 e5b9 b4e8 bf9e  ........10......
+00003400: e883 9c27 292c 0a20 2020 205d 0a20 2020  ...'),.    ].   
 00003410: 2061 6363 5f73 636f 7265 203d 206d 2e65   acc_score = m.e
 00003420: 7661 6c75 6174 655f 6d6f 6465 6c28 7465  valuate_model(te
-00003430: 7374 5f64 6174 6129 0a20 2020 2020 2020  st_data).       
-00003440: 2020 2020 2070 7269 6e74 2866 2761 6363       print(f'acc
-00003450: 5f73 636f 7265 3a20 7b61 6363 5f73 636f  _score: {acc_sco
-00003460: 7265 7d27 290a 2020 2020 2020 2020 6060  re}').        ``
-00003470: 600a 2020 2020 2020 2020 0a20 2020 2020  `.        .     
-00003480: 2020 2023 2323 2042 4552 5420 e7b1 bbe6     ### BERT ....
-00003490: a8a1 e59e 8b0a 2020 2020 2020 2020 0a20  ......        . 
-000034a0: 2020 2020 2020 2023 2323 2320 e5a4 9ae5         #### ....
-000034b0: 8886 e7b1 bbe6 a8a1 e59e 8b0a 2020 2020  ............    
-000034c0: 2020 2020 e8ae ade7 bb83 e592 8ce9 a284      ............
-000034d0: e6b5 8b60 4245 5254 60e5 a49a e588 86e7  ...`BERT`.......
-000034e0: b1bb e6a8 a1e5 9e8b efbc 8ce7 a4ba e4be  ................
-000034f0: 8b5b 6578 616d 706c 6573 2f62 6572 745f  .[examples/bert_
-00003500: 636c 6173 7369 6669 6361 7469 6f6e 5f7a  classification_z
-00003510: 685f 6465 6d6f 2e70 795d 2868 7474 7073  h_demo.py](https
-00003520: 3a2f 2f67 6974 6875 622e 636f 6d2f 7368  ://github.com/sh
-00003530: 6962 696e 6736 3234 2f70 7974 6578 7463  ibing624/pytextc
-00003540: 6c61 7373 6966 6965 722f 626c 6f62 2f6d  lassifier/blob/m
-00003550: 6173 7465 722f 6578 616d 706c 6573 2f62  aster/examples/b
-00003560: 6572 745f 636c 6173 7369 6669 6361 7469  ert_classificati
-00003570: 6f6e 5f7a 685f 6465 6d6f 2e70 7929 0a20  on_zh_demo.py). 
-00003580: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00003590: 6060 6070 7974 686f 6e0a 2020 2020 2020  ```python.      
-000035a0: 2020 696d 706f 7274 2073 7973 0a20 2020    import sys.   
-000035b0: 2020 2020 200a 2020 2020 2020 2020 7379       .        sy
-000035c0: 732e 7061 7468 2e61 7070 656e 6428 272e  s.path.append('.
-000035d0: 2e27 290a 2020 2020 2020 2020 6672 6f6d  .').        from
-000035e0: 2070 7974 6578 7463 6c61 7373 6966 6965   pytextclassifie
-000035f0: 7220 696d 706f 7274 2042 6572 7443 6c61  r import BertCla
-00003600: 7373 6966 6965 720a 2020 2020 2020 2020  ssifier.        
-00003610: 0a20 2020 2020 2020 2069 6620 5f5f 6e61  .        if __na
-00003620: 6d65 5f5f 203d 3d20 275f 5f6d 6169 6e5f  me__ == '__main_
-00003630: 5f27 3a0a 2020 2020 2020 2020 2020 2020  _':.            
-00003640: 6d20 3d20 4265 7274 436c 6173 7369 6669  m = BertClassifi
-00003650: 6572 286f 7574 7075 745f 6469 723d 276d  er(output_dir='m
-00003660: 6f64 656c 732f 6265 7274 2d63 6869 6e65  odels/bert-chine
-00003670: 7365 2d74 6f79 272c 206e 756d 5f63 6c61  se-toy', num_cla
-00003680: 7373 6573 3d32 2c0a 2020 2020 2020 2020  sses=2,.        
-00003690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000036a0: 2020 2020 2020 206d 6f64 656c 5f74 7970         model_typ
-000036b0: 653d 2762 6572 7427 2c20 6d6f 6465 6c5f  e='bert', model_
-000036c0: 6e61 6d65 3d27 6265 7274 2d62 6173 652d  name='bert-base-
-000036d0: 6368 696e 6573 6527 2c20 6e75 6d5f 6570  chinese', num_ep
-000036e0: 6f63 6873 3d32 290a 2020 2020 2020 2020  ochs=2).        
-000036f0: 2020 2020 2320 6d6f 6465 6c5f 7479 7065      # model_type
-00003700: 3a20 7375 7070 6f72 7420 2762 6572 7427  : support 'bert'
-00003710: 2c20 2761 6c62 6572 7427 2c20 2772 6f62  , 'albert', 'rob
-00003720: 6572 7461 272c 2027 786c 6e65 7427 0a20  erta', 'xlnet'. 
-00003730: 2020 2020 2020 2020 2020 2023 206d 6f64             # mod
-00003740: 656c 5f6e 616d 653a 2073 7570 706f 7274  el_name: support
-00003750: 2027 6265 7274 2d62 6173 652d 6368 696e   'bert-base-chin
-00003760: 6573 6527 2c20 2762 6572 742d 6261 7365  ese', 'bert-base
-00003770: 2d63 6173 6564 272c 2027 6265 7274 2d62  -cased', 'bert-b
-00003780: 6173 652d 6d75 6c74 696c 696e 6775 616c  ase-multilingual
-00003790: 2d63 6173 6564 2720 2e2e 2e0a 2020 2020  -cased' ....    
-000037a0: 2020 2020 2020 2020 6461 7461 203d 205b          data = [
-000037b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000037c0: 2028 2765 6475 6361 7469 6f6e 272c 2027   ('education', '
-000037d0: e590 8de5 b888 e68c 87e5 afbc e689 98e7  ................
-000037e0: a68f e8af ade6 b395 e68a 80e5 b7a7 efbc  ................
-000037f0: 9ae5 908d e8af 8de7 9a84 e5a4 8de6 95b0  ................
-00003800: e5bd a2e5 bc8f 2729 2c0a 2020 2020 2020  ......'),.      
-00003810: 2020 2020 2020 2020 2020 2827 6564 7563            ('educ
-00003820: 6174 696f 6e27 2c20 27e4 b8ad e59b bde9  ation', '.......
-00003830: ab98 e880 83e6 8890 e7bb a9e6 b5b7 e5a4  ................
-00003840: 96e8 aea4 e58f af20 e698 afe2 809c e78b  ....... ........
-00003850: bce6 9da5 e4ba 86e2 809d e590 97ef bc9f  ................
-00003860: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
-00003870: 2020 2020 2827 6564 7563 6174 696f 6e27      ('education'
-00003880: 2c20 27e5 85ac e58a a1e5 9198 e880 83e8  , '.............
-00003890: 9991 e8b6 8ae6 9da5 e8b6 8ae5 9083 e9a6  ................
-000038a0: 99ef bc8c e8bf 99e6 98af e680 8ee4 b988  ................
-000038b0: e59b 9ee4 ba8b efbc 9f27 292c 0a20 2020  .........'),.   
-000038c0: 2020 2020 2020 2020 2020 2020 2028 2773               ('s
-000038d0: 706f 7274 7327 2c20 27e5 9bbe e696 87ef  ports', '.......
-000038e0: bc9a e6b3 95e7 bd91 e5ad 9fe8 8fb2 e5b0  ................
-000038f0: 94e6 96af e88b a6e6 8898 e8bf 9b31 36e5  .............16.
-00003900: bcba 20e5 ad9f e88f b2e5 b094 e696 afe6  .. .............
-00003910: 8092 e590 bc27 292c 0a20 2020 2020 2020  .....'),.       
-00003920: 2020 2020 2020 2020 2028 2773 706f 7274           ('sport
-00003930: 7327 2c20 27e5 9b9b e5b7 9de4 b8b9 e6a3  s', '...........
-00003940: b1e4 b8be e8a1 8ce5 85a8 e59b bde9 95bf  ................
-00003950: e8b7 9de7 99bb e5b1 b1e6 8c91 e688 98e8  ................
-00003960: b59b 20e8 bf91 e4b8 87e4 baba e58f 82e4  .. .............
-00003970: b88e 2729 2c0a 2020 2020 2020 2020 2020  ..'),.          
-00003980: 2020 2020 2020 2827 7370 6f72 7473 272c        ('sports',
-00003990: 2027 e7b1 b3e5 85b0 e5ae a2e5 9cba 38e6   '............8.
-000039a0: 8898 e4b8 8de8 b4a5 e59b bde7 b1b3 3130  ..............10
-000039b0: e5b9 b4e8 bf9e e883 9c27 292c 0a20 2020  .........'),.   
-000039c0: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
-000039d0: 2020 2020 2020 206d 2e74 7261 696e 2864         m.train(d
-000039e0: 6174 6129 0a20 2020 2020 2020 2020 2020  ata).           
-000039f0: 2070 7269 6e74 286d 290a 2020 2020 2020   print(m).      
-00003a00: 2020 2020 2020 2320 6c6f 6164 2074 7261        # load tra
-00003a10: 696e 6564 2062 6573 7420 6d6f 6465 6c20  ined best model 
-00003a20: 6672 6f6d 206d 6f64 656c 5f64 6972 0a20  from model_dir. 
-00003a30: 2020 2020 2020 2020 2020 206d 2e6c 6f61             m.loa
-00003a40: 645f 6d6f 6465 6c28 290a 2020 2020 2020  d_model().      
-00003a50: 2020 2020 2020 7072 6564 6963 745f 6c61        predict_la
-00003a60: 6265 6c2c 2070 7265 6469 6374 5f70 726f  bel, predict_pro
-00003a70: 6261 203d 206d 2e70 7265 6469 6374 285b  ba = m.predict([
-00003a80: 27e7 a68f e5bb bae6 98a5 e5ad a3e5 85ac  '...............
-00003a90: e58a a1e5 9198 e880 83e8 af95 e68a a5e5  ................
-00003aa0: 908d 3138 e697 a5e6 88aa e6ad a220 32e6  ..18......... 2.
-00003ab0: 9c88 36e6 97a5 e880 83e8 af95 272c 0a20  ..6.........',. 
-00003ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003af0: 2020 2020 2027 e684 8fe7 94b2 e9a6 96e8       '..........
-00003b00: bdae e8a1 a5e8 b59b e4ba a4e6 8898 e8ae  ................
-00003b10: b0e5 bd95 3ae7 b1b3 e585 b0e5 aea2 e59c  ....:...........
-00003b20: ba38 e688 98e4 b88d e8b4 a5e5 9bbd e7b1  .8..............
-00003b30: b331 30e5 b9b4 e8bf 9ee8 839c 275d 290a  .10.........']).
-00003b40: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00003b50: 7428 6627 7072 6564 6963 745f 6c61 6265  t(f'predict_labe
-00003b60: 6c3a 207b 7072 6564 6963 745f 6c61 6265  l: {predict_labe
-00003b70: 6c7d 2c20 7072 6564 6963 745f 7072 6f62  l}, predict_prob
-00003b80: 613a 207b 7072 6564 6963 745f 7072 6f62  a: {predict_prob
-00003b90: 617d 2729 0a20 2020 2020 2020 200a 2020  a}').        .  
-00003ba0: 2020 2020 2020 2020 2020 7465 7374 5f64            test_d
-00003bb0: 6174 6120 3d20 5b0a 2020 2020 2020 2020  ata = [.        
-00003bc0: 2020 2020 2020 2020 2827 6564 7563 6174          ('educat
-00003bd0: 696f 6e27 2c20 27e7 a68f e5bb bae6 98a5  ion', '.........
-00003be0: e5ad a3e5 85ac e58a a1e5 9198 e880 83e8  ................
-00003bf0: af95 e68a a5e5 908d 3138 e697 a5e6 88aa  ........18......
-00003c00: e6ad a220 32e6 9c88 36e6 97a5 e880 83e8  ... 2...6.......
-00003c10: af95 2729 2c0a 2020 2020 2020 2020 2020  ..'),.          
-00003c20: 2020 2020 2020 2827 7370 6f72 7473 272c        ('sports',
-00003c30: 2027 e684 8fe7 94b2 e9a6 96e8 bdae e8a1   '..............
-00003c40: a5e8 b59b e4ba a4e6 8898 e8ae b0e5 bd95  ................
-00003c50: 3ae7 b1b3 e585 b0e5 aea2 e59c ba38 e688  :............8..
-00003c60: 98e4 b88d e8b4 a5e5 9bbd e7b1 b331 30e5  .............10.
-00003c70: b9b4 e8bf 9ee8 839c 2729 2c0a 2020 2020  ........'),.    
-00003c80: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
-00003c90: 2020 2020 2020 6163 635f 7363 6f72 6520        acc_score 
-00003ca0: 3d20 6d2e 6576 616c 7561 7465 5f6d 6f64  = m.evaluate_mod
-00003cb0: 656c 2874 6573 745f 6461 7461 290a 2020  el(test_data).  
-00003cc0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00003cd0: 6627 6163 635f 7363 6f72 653a 207b 6163  f'acc_score: {ac
-00003ce0: 635f 7363 6f72 657d 2729 0a20 2020 2020  c_score}').     
-00003cf0: 2020 200a 2020 2020 2020 2020 2020 2020     .            
-00003d00: 2320 7472 6169 6e20 6d6f 6465 6c20 7769  # train model wi
-00003d10: 7468 2031 7720 6461 7461 2066 696c 6520  th 1w data file 
-00003d20: 616e 6420 3130 2063 6c61 7373 6573 0a20  and 10 classes. 
-00003d30: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00003d40: 2827 2d27 202a 2034 3229 0a20 2020 2020  ('-' * 42).     
-00003d50: 2020 2020 2020 206d 203d 2042 6572 7443         m = BertC
-00003d60: 6c61 7373 6966 6965 7228 6f75 7470 7574  lassifier(output
-00003d70: 5f64 6972 3d27 6d6f 6465 6c73 2f62 6572  _dir='models/ber
-00003d80: 742d 6368 696e 6573 6527 2c20 6e75 6d5f  t-chinese', num_
-00003d90: 636c 6173 7365 733d 3130 2c0a 2020 2020  classes=10,.    
-00003da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003db0: 2020 2020 2020 2020 2020 206d 6f64 656c             model
-00003dc0: 5f74 7970 653d 2762 6572 7427 2c20 6d6f  _type='bert', mo
-00003dd0: 6465 6c5f 6e61 6d65 3d27 6265 7274 2d62  del_name='bert-b
-00003de0: 6173 652d 6368 696e 6573 6527 2c20 6e75  ase-chinese', nu
-00003df0: 6d5f 6570 6f63 6873 3d32 2c0a 2020 2020  m_epochs=2,.    
-00003e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003e10: 2020 2020 2020 2020 2020 2061 7267 733d             args=
-00003e20: 7b22 6e6f 5f63 6163 6865 223a 2054 7275  {"no_cache": Tru
-00003e30: 652c 2022 6c61 7a79 5f6c 6f61 6469 6e67  e, "lazy_loading
-00003e40: 223a 2054 7275 652c 2022 6c61 7a79 5f74  ": True, "lazy_t
-00003e50: 6578 745f 636f 6c75 6d6e 223a 2031 2c20  ext_column": 1, 
-00003e60: 226c 617a 795f 6c61 6265 6c73 5f63 6f6c  "lazy_labels_col
-00003e70: 756d 6e22 3a20 302c 207d 290a 2020 2020  umn": 0, }).    
-00003e80: 2020 2020 2020 2020 6461 7461 5f66 696c          data_fil
-00003e90: 6520 3d20 2774 6875 636e 6577 735f 7472  e = 'thucnews_tr
-00003ea0: 6169 6e5f 3177 2e74 7874 270a 2020 2020  ain_1w.txt'.    
-00003eb0: 2020 2020 2020 2020 2320 e5a6 82e6 9e9c          # ......
-00003ec0: e8ae ade7 bb83 e695 b0e6 8dae e8b6 85e8  ................
-00003ed0: bf87 e799 bee4 b887 e69d a1ef bc8c e5bb  ................
-00003ee0: bae8 aeae e4bd bfe7 94a8 6c61 7a79 5f6c  ..........lazy_l
-00003ef0: 6f61 6469 6e67 e6a8 a1e5 bc8f efbc 8ce5  oading..........
-00003f00: 878f e5b0 91e5 8685 e5ad 98e5 8da0 e794  ................
-00003f10: a80a 2020 2020 2020 2020 2020 2020 6d2e  ..            m.
-00003f20: 7472 6169 6e28 6461 7461 5f66 696c 652c  train(data_file,
-00003f30: 2074 6573 745f 7369 7a65 3d30 2c20 6e61   test_size=0, na
-00003f40: 6d65 733d 2827 6c61 6265 6c73 272c 2027  mes=('labels', '
-00003f50: 7465 7874 2729 290a 2020 2020 2020 2020  text')).        
-00003f60: 2020 2020 6d2e 6c6f 6164 5f6d 6f64 656c      m.load_model
-00003f70: 2829 0a20 2020 2020 2020 2020 2020 2070  ().            p
-00003f80: 7265 6469 6374 5f6c 6162 656c 2c20 7072  redict_label, pr
-00003f90: 6564 6963 745f 7072 6f62 6120 3d20 6d2e  edict_proba = m.
-00003fa0: 7072 6564 6963 7428 0a20 2020 2020 2020  predict(.       
-00003fb0: 2020 2020 2020 2020 205b 27e9 a1ba e4b9           ['.....
-00003fc0: 89e5 8c97 e4ba ace8 8b8f e6b4 bb38 38e5  .............88.
-00003fd0: b9b3 e7b1 b3e8 b5b7 e7b2 bee8 a385 e688  ................
-00003fe0: bfe5 9ca8 e594 ae27 2c0a 2020 2020 2020  .......',.      
-00003ff0: 2020 2020 2020 2020 2020 2027 e7be 8e45             '...E
-00004000: 422d 35e9 a1b9 e79b aee2 809c 3135 e697  B-5.........15..
-00004010: a5e5 bfab e980 9fe7 a7bb e6b0 91e2 809d  ................
-00004020: e5b0 86e6 8ea8 e8bf 9f27 2c0a 2020 2020  .........',.    
-00004030: 2020 2020 2020 2020 2020 2020 2027 e681               '..
-00004040: 92e7 949f 4148 e6ba a2e6 8c87 e694 b6e5  ....AH..........
-00004050: b9b3 2041 e882 a1e5 afb9 48e8 82a1 e68a  .. A......H.....
-00004060: 98e4 bbb7 312e 3935 2527 5d29 0a20 2020  ....1.95%']).   
-00004070: 2020 2020 2020 2020 2070 7269 6e74 2866           print(f
-00004080: 2770 7265 6469 6374 5f6c 6162 656c 3a20  'predict_label: 
-00004090: 7b70 7265 6469 6374 5f6c 6162 656c 7d2c  {predict_label},
-000040a0: 2070 7265 6469 6374 5f70 726f 6261 3a20   predict_proba: 
-000040b0: 7b70 7265 6469 6374 5f70 726f 6261 7d27  {predict_proba}'
-000040c0: 290a 2020 2020 2020 2020 6060 600a 2020  ).        ```.  
-000040d0: 2020 2020 2020 5053 efbc 9ae5 a682 e69e        PS........
-000040e0: 9ce8 aead e7bb 83e6 95b0 e68d aee8 b685  ................
-000040f0: e8bf 87e7 99be e4b8 87e6 9da1 efbc 8ce5  ................
-00004100: bbba e8ae aee4 bdbf e794 a86c 617a 795f  ...........lazy_
-00004110: 6c6f 6164 696e 67e6 a8a1 e5bc 8fef bc8c  loading.........
-00004120: e587 8fe5 b091 e586 85e5 ad98 e58d a0e7  ................
-00004130: 94a8 0a20 2020 2020 2020 200a 2020 2020  ...        .    
-00004140: 2020 2020 2323 2323 20e5 a49a e6a0 87e7      #### .......
-00004150: adbe e588 86e7 b1bb e6a8 a1e5 9e8b 0a20  ............... 
-00004160: 2020 2020 2020 20e5 8886 e7b1 bbe5 8faf         .........
-00004170: e4bb a5e5 8886 e4b8 bae5 a49a e588 86e7  ................
-00004180: b1bb e592 8ce5 a49a e6a0 87e7 adbe e588  ................
-00004190: 86e7 b1bb e380 82e5 a49a e588 86e7 b1bb  ................
-000041a0: e79a 84e6 a087 e7ad bee6 98af e68e 92e4  ................
-000041b0: bb96 e79a 84ef bc8c e880 8ce5 a49a e6a0  ................
-000041c0: 87e7 adbe e588 86e7 b1bb e79a 84e6 8980  ................
-000041d0: e69c 89e6 a087 e7ad bee6 98af e4b8 8de6  ................
-000041e0: 8e92 e4bb 96e7 9a84 e380 820a 2020 2020  ............    
-000041f0: 2020 2020 0a20 2020 2020 2020 20e5 a49a      .        ...
-00004200: e6a0 87e7 adbe e588 86e7 b1bb e6af 94e8  ................
-00004210: be83 e79b b4e8 a782 e79a 84e7 9086 e8a7  ................
-00004220: a3e6 98af efbc 8ce4 b880 e4b8 aae6 a0b7  ................
-00004230: e69c ace5 8faf e4bb a5e5 908c e697 b6e6  ................
-00004240: 8ba5 e69c 89e5 87a0 e4b8 aae7 b1bb e588  ................
-00004250: abe6 a087 e7ad beef bc8c 0a20 2020 2020  ...........     
-00004260: 2020 20e6 af94 e5a6 82e4 b880 e9a6 96e6     .............
-00004270: ad8c e79a 84e6 a087 e7ad bee5 8faf e4bb  ................
-00004280: a5e6 98af e6b5 81e8 a18c e380 81e8 bdbb  ................
-00004290: e5bf abef bc8c e4b8 80e9 83a8 e794 b5e5  ................
-000042a0: bdb1 e79a 84e6 a087 e7ad bee5 8faf e4bb  ................
-000042b0: a5e6 98af e58a a8e4 bd9c e380 81e5 969c  ................
-000042c0: e589 a7e3 8081 e690 9ee7 ac91 e7ad 89ef  ................
-000042d0: bc8c e8bf 99e9 83bd e698 afe5 a49a e6a0  ................
-000042e0: 87e7 adbe e588 86e7 b1bb e79a 84e6 8385  ................
-000042f0: e586 b5e3 8082 0a20 2020 2020 2020 200a  .......        .
-00004300: 2020 2020 2020 2020 e8ae ade7 bb83 e592          ........
-00004310: 8ce9 a284 e6b5 8b60 4245 5254 60e5 a49a  .......`BERT`...
-00004320: e6a0 87e7 adbe e588 86e7 b1bb e6a8 a1e5  ................
-00004330: 9e8b efbc 8ce7 a4ba e4be 8b5b 6578 616d  ...........[exam
-00004340: 706c 6573 2f62 6572 745f 6d75 6c74 696c  ples/bert_multil
-00004350: 6162 656c 5f63 6c61 7373 6966 6963 6174  abel_classificat
-00004360: 696f 6e5f 7a68 5f64 656d 6f2e 7079 2e70  ion_zh_demo.py.p
-00004370: 795d 2868 7474 7073 3a2f 2f67 6974 6875  y](https://githu
-00004380: 622e 636f 6d2f 7368 6962 696e 6736 3234  b.com/shibing624
-00004390: 2f70 7974 6578 7463 6c61 7373 6966 6965  /pytextclassifie
-000043a0: 722f 626c 6f62 2f6d 6173 7465 722f 6578  r/blob/master/ex
-000043b0: 616d 706c 6573 2f62 6572 745f 6d75 6c74  amples/bert_mult
-000043c0: 696c 6162 656c 5f63 6c61 7373 6966 6963  ilabel_classific
-000043d0: 6174 696f 6e5f 7a68 5f64 656d 6f2e 7079  ation_zh_demo.py
-000043e0: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-000043f0: 2020 2060 6060 7079 7468 6f6e 0a20 2020     ```python.   
-00004400: 2020 2020 2069 6d70 6f72 7420 7379 730a       import sys.
-00004410: 2020 2020 2020 2020 696d 706f 7274 2070          import p
-00004420: 616e 6461 7320 6173 2070 640a 2020 2020  andas as pd.    
-00004430: 2020 2020 0a20 2020 2020 2020 2073 7973      .        sys
-00004440: 2e70 6174 682e 6170 7065 6e64 2827 2e2e  .path.append('..
-00004450: 2729 0a20 2020 2020 2020 2066 726f 6d20  ').        from 
-00004460: 7079 7465 7874 636c 6173 7369 6669 6572  pytextclassifier
-00004470: 2069 6d70 6f72 7420 4265 7274 436c 6173   import BertClas
-00004480: 7369 6669 6572 0a20 2020 2020 2020 200a  sifier.        .
-00004490: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-000044a0: 2064 6566 206c 6f61 645f 6a64 5f64 6174   def load_jd_dat
-000044b0: 6128 6669 6c65 5f70 6174 6829 3a0a 2020  a(file_path):.  
-000044c0: 2020 2020 2020 2020 2020 2222 220a 2020            """.  
-000044d0: 2020 2020 2020 2020 2020 4c6f 6164 206a            Load j
-000044e0: 6420 6461 7461 2066 726f 6d20 6669 6c65  d data from file
-000044f0: 2e0a 2020 2020 2020 2020 2020 2020 4070  ..            @p
-00004500: 6172 616d 2066 696c 655f 7061 7468 3a20  aram file_path: 
-00004510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004520: 2066 6f72 6d61 743a 2063 6f6e 7465 6e74   format: content
-00004530: 2ce5 85b6 e4bb 962c e4ba 92e8 8194 e4ba  ,......,........
-00004540: 92e9 809a 2ce4 baa7 e593 81e5 8a9f e880  ....,...........
-00004550: 972c e6bb 91e8 bdae e68f 90e6 898b 2ce5  .,............,.
-00004560: a3b0 e99f b32c 4150 50e6 938d e68e a7e6  .....,APP.......
-00004570: 80a7 2ce5 91bc e590 b8e7 81af 2ce5 a496  ..,.........,...
-00004580: e8a7 822c e5ba 95e5 baa7 2ce5 88b6 e783  ...,......,.....
-00004590: ade8 8c83 e59b b42c e981 a5e6 8ea7 e599  .......,........
-000045a0: a8e7 94b5 e6b1 a02c e591 b3e9 8193 2ce5  .......,......,.
-000045b0: 88b6 e783 ade6 9588 e69e 9c2c e8a1 a3e7  ...........,....
-000045c0: 89a9 e783 98e5 b9b2 2ce4 bd93 e7a7 afe5  ........,.......
-000045d0: a4a7 e5b0 8f0a 2020 2020 2020 2020 2020  ......          
-000045e0: 2020 4072 6574 7572 6e3a 200a 2020 2020    @return: .    
-000045f0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00004600: 2020 2020 2020 2020 6461 7461 203d 205b          data = [
-00004610: 5d0a 2020 2020 2020 2020 2020 2020 7769  ].            wi
-00004620: 7468 206f 7065 6e28 6669 6c65 5f70 6174  th open(file_pat
-00004630: 682c 2027 7227 2c20 656e 636f 6469 6e67  h, 'r', encoding
-00004640: 3d27 7574 662d 3827 2920 6173 2066 3a0a  ='utf-8') as f:.
-00004650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004660: 666f 7220 6c69 6e65 2069 6e20 663a 0a20  for line in f:. 
-00004670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004680: 2020 206c 696e 6520 3d20 6c69 6e65 2e73     line = line.s
-00004690: 7472 6970 2829 0a20 2020 2020 2020 2020  trip().         
-000046a0: 2020 2020 2020 2020 2020 2069 6620 6c69             if li
-000046b0: 6e65 2e73 7461 7274 7377 6974 6828 2723  ne.startswith('#
-000046c0: 2729 3a0a 2020 2020 2020 2020 2020 2020  '):.            
-000046d0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-000046e0: 696e 7565 0a20 2020 2020 2020 2020 2020  inue.           
-000046f0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-00004700: 6c69 6e65 3a0a 2020 2020 2020 2020 2020  line:.          
-00004710: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00004720: 6e74 696e 7565 0a20 2020 2020 2020 2020  ntinue.         
-00004730: 2020 2020 2020 2020 2020 2074 6572 6d73             terms
-00004740: 203d 206c 696e 652e 7370 6c69 7428 272c   = line.split(',
-00004750: 2729 0a20 2020 2020 2020 2020 2020 2020  ').             
-00004760: 2020 2020 2020 2069 6620 6c65 6e28 7465         if len(te
-00004770: 726d 7329 2021 3d20 3136 3a0a 2020 2020  rms) != 16:.    
-00004780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004790: 2020 2020 636f 6e74 696e 7565 0a20 2020      continue.   
-000047a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000047b0: 2076 616c 203d 205b 696e 7428 6929 2066   val = [int(i) f
-000047c0: 6f72 2069 2069 6e20 7465 726d 735b 313a  or i in terms[1:
-000047d0: 5d5d 0a20 2020 2020 2020 2020 2020 2020  ]].             
-000047e0: 2020 2020 2020 2064 6174 612e 6170 7065         data.appe
-000047f0: 6e64 285b 7465 726d 735b 305d 2c20 7661  nd([terms[0], va
-00004800: 6c5d 290a 2020 2020 2020 2020 2020 2020  l]).            
-00004810: 7265 7475 726e 2064 6174 610a 2020 2020  return data.    
-00004820: 2020 2020 0a20 2020 2020 2020 200a 2020      .        .  
-00004830: 2020 2020 2020 6966 205f 5f6e 616d 655f        if __name_
-00004840: 5f20 3d3d 2027 5f5f 6d61 696e 5f5f 273a  _ == '__main__':
-00004850: 0a20 2020 2020 2020 2020 2020 2023 206d  .            # m
-00004860: 6f64 656c 5f74 7970 653a 2073 7570 706f  odel_type: suppo
-00004870: 7274 2027 6265 7274 272c 2027 616c 6265  rt 'bert', 'albe
-00004880: 7274 272c 2027 726f 6265 7274 6127 2c20  rt', 'roberta', 
-00004890: 2778 6c6e 6574 270a 2020 2020 2020 2020  'xlnet'.        
-000048a0: 2020 2020 2320 6d6f 6465 6c5f 6e61 6d65      # model_name
-000048b0: 3a20 7375 7070 6f72 7420 2762 6572 742d  : support 'bert-
-000048c0: 6261 7365 2d63 6869 6e65 7365 272c 2027  base-chinese', '
-000048d0: 6265 7274 2d62 6173 652d 6361 7365 6427  bert-base-cased'
-000048e0: 2c20 2762 6572 742d 6261 7365 2d6d 756c  , 'bert-base-mul
-000048f0: 7469 6c69 6e67 7561 6c2d 6361 7365 6427  tilingual-cased'
-00004900: 202e 2e2e 0a20 2020 2020 2020 2020 2020   ....           
-00004910: 206d 203d 2042 6572 7443 6c61 7373 6966   m = BertClassif
-00004920: 6965 7228 6f75 7470 7574 5f64 6972 3d27  ier(output_dir='
-00004930: 6d6f 6465 6c73 2f6d 756c 7469 6c61 6265  models/multilabe
-00004940: 6c2d 6265 7274 2d7a 682d 6d6f 6465 6c27  l-bert-zh-model'
-00004950: 2c20 6e75 6d5f 636c 6173 7365 733d 3135  , num_classes=15
-00004960: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00004970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004980: 206d 6f64 656c 5f74 7970 653d 2762 6572   model_type='ber
-00004990: 7427 2c20 6d6f 6465 6c5f 6e61 6d65 3d27  t', model_name='
-000049a0: 6265 7274 2d62 6173 652d 6368 696e 6573  bert-base-chines
-000049b0: 6527 2c20 6e75 6d5f 6570 6f63 6873 3d32  e', num_epochs=2
-000049c0: 2c20 6d75 6c74 695f 6c61 6265 6c3d 5472  , multi_label=Tr
-000049d0: 7565 290a 2020 2020 2020 2020 2020 2020  ue).            
-000049e0: 2320 5472 6169 6e20 616e 6420 4576 616c  # Train and Eval
-000049f0: 7561 7469 6f6e 2064 6174 6120 6e65 6564  uation data need
-00004a00: 7320 746f 2062 6520 696e 2061 2050 616e  s to be in a Pan
-00004a10: 6461 7320 4461 7461 6672 616d 6520 636f  das Dataframe co
-00004a20: 6e74 6169 6e69 6e67 2061 7420 6c65 6173  ntaining at leas
-00004a30: 7420 7477 6f20 636f 6c75 6d6e 732c 2061  t two columns, a
-00004a40: 2027 7465 7874 2720 616e 6420 6120 276c   'text' and a 'l
-00004a50: 6162 656c 7327 2063 6f6c 756d 6e2e 2054  abels' column. T
-00004a60: 6865 2060 6c61 6265 6c73 6020 636f 6c75  he `labels` colu
-00004a70: 6d6e 2073 686f 756c 6420 636f 6e74 6169  mn should contai
-00004a80: 6e20 6d75 6c74 692d 686f 7420 656e 636f  n multi-hot enco
-00004a90: 6465 6420 6c69 7374 732e 0a20 2020 2020  ded lists..     
-00004aa0: 2020 2020 2020 2074 7261 696e 5f64 6174         train_dat
-00004ab0: 6120 3d20 5b0a 2020 2020 2020 2020 2020  a = [.          
-00004ac0: 2020 2020 2020 5b22 e4b8 80e4 b8aa e5b0        ["........
-00004ad0: 8fe6 97b6 e688 bfe9 97b4 e4bb 8de7 84b6  ................
-00004ae0: e6b2 a1e6 9a96 e592 8c22 2c20 5b30 2c20  .........", [0, 
-00004af0: 302c 2030 2c20 302c 2030 2c20 302c 2030  0, 0, 0, 0, 0, 0
-00004b00: 2c20 302c 2030 2c20 302c 2030 2c20 302c  , 0, 0, 0, 0, 0,
-00004b10: 2031 2c20 302c 2030 5d5d 2c0a 2020 2020   1, 0, 0]],.    
-00004b20: 2020 2020 2020 2020 2020 2020 5b22 e880              ["..
-00004b30: 97e7 94b5 e683 85e5 86b5 efbc 9ae8 bf99  ................
-00004b40: e4b8 aae6 b2a1 e69c 89e6 b3a8 e684 8f22  ..............."
-00004b50: 2c20 5b30 2c20 302c 2031 2c20 302c 2030  , [0, 0, 1, 0, 0
-00004b60: 2c20 302c 2030 2c20 302c 2030 2c20 302c  , 0, 0, 0, 0, 0,
-00004b70: 2030 2c20 302c 2030 2c20 302c 2030 5d5d   0, 0, 0, 0, 0]]
-00004b80: 2c0a 2020 2020 2020 2020 2020 2020 5d0a  ,.            ].
-00004b90: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00004ba0: 203d 206c 6f61 645f 6a64 5f64 6174 6128   = load_jd_data(
-00004bb0: 276d 756c 7469 6c61 6265 6c5f 6a64 5f63  'multilabel_jd_c
-00004bc0: 6f6d 6d65 6e74 732e 6373 7627 290a 2020  omments.csv').  
-00004bd0: 2020 2020 2020 2020 2020 7472 6169 6e5f            train_
-00004be0: 6461 7461 2e65 7874 656e 6428 6461 7461  data.extend(data
-00004bf0: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
-00004c00: 696e 7428 7472 6169 6e5f 6461 7461 5b3a  int(train_data[:
-00004c10: 355d 290a 2020 2020 2020 2020 2020 2020  5]).            
-00004c20: 7472 6169 6e5f 6466 203d 2070 642e 4461  train_df = pd.Da
-00004c30: 7461 4672 616d 6528 7472 6169 6e5f 6461  taFrame(train_da
-00004c40: 7461 2c20 636f 6c75 6d6e 733d 5b22 7465  ta, columns=["te
-00004c50: 7874 222c 2022 6c61 6265 6c73 225d 290a  xt", "labels"]).
-00004c60: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00004c70: 2020 2020 2070 7269 6e74 2874 7261 696e       print(train
-00004c80: 5f64 662e 6865 6164 2829 290a 2020 2020  _df.head()).    
-00004c90: 2020 2020 2020 2020 6d2e 7472 6169 6e28          m.train(
-00004ca0: 7472 6169 6e5f 6466 290a 2020 2020 2020  train_df).      
-00004cb0: 2020 2020 2020 7072 696e 7428 6d29 0a20        print(m). 
-00004cc0: 2020 2020 2020 2020 2020 2023 2045 7661             # Eva
-00004cd0: 6c75 6174 6520 7468 6520 6d6f 6465 6c0a  luate the model.
-00004ce0: 2020 2020 2020 2020 2020 2020 6163 635f              acc_
-00004cf0: 7363 6f72 6520 3d20 6d2e 6576 616c 7561  score = m.evalua
-00004d00: 7465 5f6d 6f64 656c 2874 7261 696e 5f64  te_model(train_d
-00004d10: 665b 3a32 305d 290a 2020 2020 2020 2020  f[:20]).        
-00004d20: 2020 2020 7072 696e 7428 6627 6163 635f      print(f'acc_
-00004d30: 7363 6f72 653a 207b 6163 635f 7363 6f72  score: {acc_scor
-00004d40: 657d 2729 0a20 2020 2020 2020 200a 2020  e}').        .  
-00004d50: 2020 2020 2020 2020 2020 2320 6c6f 6164            # load
-00004d60: 2074 7261 696e 6564 2062 6573 7420 6d6f   trained best mo
-00004d70: 6465 6c20 6672 6f6d 206d 6f64 656c 5f64  del from model_d
-00004d80: 6972 0a20 2020 2020 2020 2020 2020 206d  ir.            m
-00004d90: 2e6c 6f61 645f 6d6f 6465 6c28 290a 2020  .load_model().  
-00004da0: 2020 2020 2020 2020 2020 7072 6564 6963            predic
-00004db0: 745f 6c61 6265 6c2c 2070 7265 6469 6374  t_label, predict
-00004dc0: 5f70 726f 6261 203d 206d 2e70 7265 6469  _proba = m.predi
-00004dd0: 6374 285b 27e4 b880 e4b8 aae5 b08f e697  ct(['...........
-00004de0: b6e6 88bf e997 b4e4 bb8d e784 b6e6 b2a1  ................
-00004df0: e69a 96e5 928c 272c 2027 e880 97e7 94b5  ......', '......
-00004e00: e683 85e5 86b5 efbc 9ae8 bf99 e4b8 aae6  ................
-00004e10: b2a1 e69c 89e6 b3a8 e684 8f27 5d29 0a20  ...........']). 
-00004e20: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00004e30: 2866 2770 7265 6469 6374 5f6c 6162 656c  (f'predict_label
-00004e40: 3a20 7b70 7265 6469 6374 5f6c 6162 656c  : {predict_label
-00004e50: 7d2c 2070 7265 6469 6374 5f70 726f 6261  }, predict_proba
-00004e60: 3a20 7b70 7265 6469 6374 5f70 726f 6261  : {predict_proba
-00004e70: 7d27 290a 2020 2020 2020 2020 6060 600a  }').        ```.
-00004e80: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00004e90: 2023 2320 4576 616c 7561 7469 6f6e 0a20   ## Evaluation. 
-00004ea0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00004eb0: 2323 2320 4461 7461 7365 740a 2020 2020  ### Dataset.    
-00004ec0: 2020 2020 0a20 2020 2020 2020 2031 2e20      .        1. 
-00004ed0: 5448 5543 4e65 7773 e4b8 ade6 9687 e696  THUCNews........
-00004ee0: 87e6 9cac e695 b0e6 8dae e99b 86ef bc88  ................
-00004ef0: 312e 3536 4742 efbc 89ef bc9a e5ae 98e6  1.56GB..........
-00004f00: 96b9 5be4 b88b e8bd bde5 9cb0 e59d 805d  ..[............]
-00004f10: 2868 7474 703a 2f2f 7468 7563 7463 2e74  (http://thuctc.t
-00004f20: 6875 6e6c 702e 6f72 672f 29ef bc8c e68a  hunlp.org/).....
-00004f30: bde6 a0b7 e4ba 8631 30e4 b887 e69d a154  .......10......T
-00004f40: 4855 434e 6577 73e4 b8ad e696 87e6 9687  HUCNews.........
-00004f50: e69c ac31 30e5 8886 e7b1 bbe6 95b0 e68d  ...10...........
-00004f60: aee9 9b86 efbc 8836 4d42 efbc 89ef bc8c  .......6MB......
-00004f70: e59c b0e5 9d80 efbc 9a5b 6578 616d 706c  .........[exampl
-00004f80: 6573 2f74 6875 636e 6577 735f 7472 6169  es/thucnews_trai
-00004f90: 6e5f 3130 772e 7478 745d 2868 7474 7073  n_10w.txt](https
-00004fa0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7368  ://github.com/sh
-00004fb0: 6962 696e 6736 3234 2f70 7974 6578 7463  ibing624/pytextc
-00004fc0: 6c61 7373 6966 6965 722f 626c 6f62 2f6d  lassifier/blob/m
-00004fd0: 6173 7465 722f 6578 616d 706c 6573 2f74  aster/examples/t
-00004fe0: 6875 636e 6577 735f 7472 6169 6e5f 3130  hucnews_train_10
-00004ff0: 772e 7478 7429 e380 820a 2020 2020 2020  w.txt)....      
-00005000: 2020 322e 2054 4e45 5753 e4bb 8ae6 97a5    2. TNEWS......
-00005010: e5a4 b4e6 9da1 e4b8 ade6 9687 e696 b0e9  ................
-00005020: 97bb efbc 88e7 9fad e696 87e6 9cac efbc  ................
-00005030: 89e5 8886 e7b1 bb20 5368 6f72 7420 5465  ....... Short Te
-00005040: 7874 2043 6c61 7373 6966 6963 6169 746f  xt Classificaito
-00005050: 6e20 666f 7220 4e65 7773 efbc 8ce8 afa5  n for News......
-00005060: e695 b0e6 8dae e99b 8628 352e 314d 4229  .........(5.1MB)
-00005070: e69d a5e8 87aa e4bb 8ae6 97a5 e5a4 b4e6  ................
-00005080: 9da1 e79a 84e6 96b0 e997 bbe7 8988 e59d  ................
-00005090: 97ef bc8c e585 b1e6 8f90 e58f 96e4 ba86  ................
-000050a0: 3135 e4b8 aae7 b1bb e588 abe7 9a84 e696  15..............
-000050b0: b0e9 97bb efbc 8ce5 8c85 e68b ace6 9785  ................
-000050c0: e6b8 b8ef bc8c e695 99e8 82b2 efbc 8ce9  ................
-000050d0: 8791 e89e 8def bc8c e586 9be4 ba8b e7ad  ................
-000050e0: 89ef bc8c e59c b0e5 9d80 efbc 9a5b 746e  .............[tn
-000050f0: 6577 735f 7075 626c 6963 2e7a 6970 5d28  ews_public.zip](
-00005100: 6874 7470 733a 2f2f 7374 6f72 6167 652e  https://storage.
-00005110: 676f 6f67 6c65 6170 6973 2e63 6f6d 2f63  googleapis.com/c
-00005120: 6c75 6562 656e 6368 6d61 726b 2f74 6173  luebenchmark/tas
-00005130: 6b73 2f74 6e65 7773 5f70 7562 6c69 632e  ks/tnews_public.
-00005140: 7a69 7029 0a20 2020 2020 2020 200a 2020  zip).        .  
-00005150: 2020 2020 2020 2323 2320 4576 616c 7561        ### Evalua
-00005160: 7469 6f6e 2052 6573 756c 740a 2020 2020  tion Result.    
-00005170: 2020 2020 e59c a854 4855 434e 6577 73e4      ...THUCNews.
-00005180: b8ad e696 87e6 9687 e69c ac31 30e5 8886  ...........10...
-00005190: e7b1 bbe6 95b0 e68d aee9 9b86 efbc 8836  ...............6
-000051a0: 4d42 efbc 89e4 b88a e8af 84e4 bcb0 efbc  MB..............
-000051b0: 8ce6 a8a1 e59e 8be5 9ca8 e6b5 8be8 af95  ................
-000051c0: e99b 8628 7465 7374 29e8 af84 e6b5 8be6  ...(test).......
-000051d0: 9588 e69e 9ce5 a682 e4b8 8bef bc9a 0a20  ............... 
-000051e0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-000051f0: e6a8 a1e5 9e8b 7c61 6363 7ce8 afb4 e698  ......|acc|.....
-00005200: 8e0a 2020 2020 2020 2020 2d2d 7c2d 2d7c  ..        --|--|
-00005210: 2d2d 0a20 2020 2020 2020 204c 527c 302e  --.        LR|0.
-00005220: 3838 3033 7ce9 80bb e8be 91e5 9b9e e5bd  8803|...........
-00005230: 924c 6f67 6973 7469 6373 2052 6567 7265  .Logistics Regre
-00005240: 7373 696f 6e0a 2020 2020 2020 2020 5465  ssion.        Te
-00005250: 7874 434e 4e7c 302e 3838 3039 7c4b 696d  xtCNN|0.8809|Kim
-00005260: 2032 3031 3420 e7bb 8fe5 85b8 e79a 8443   2014 .........C
-00005270: 4e4e e696 87e6 9cac e588 86e7 b1bb 0a20  NN............. 
-00005280: 2020 2020 2020 2054 6578 7452 4e4e 5f41         TextRNN_A
-00005290: 7474 7c30 2e39 3032 327c 4269 4c53 544d  tt|0.9022|BiLSTM
-000052a0: 2b41 7474 656e 7469 6f6e 0a20 2020 2020  +Attention.     
-000052b0: 2020 2046 6173 7454 6578 747c 302e 3931     FastText|0.91
-000052c0: 3737 7c62 6f77 2b62 6967 7261 6d2b 7472  77|bow+bigram+tr
-000052d0: 6967 7261 6def bc8c 20e6 9588 e69e 9ce5  igram... .......
-000052e0: 87ba e5a5 87e7 9a84 e5a5 bd0a 2020 2020  ............    
-000052f0: 2020 2020 4450 434e 4e7c 302e 3931 3235      DPCNN|0.9125
-00005300: 7ce6 b7b1 e5b1 82e9 8791 e5ad 97e5 a194  |...............
-00005310: 434e 4e0a 2020 2020 2020 2020 5472 616e  CNN.        Tran
-00005320: 7366 6f72 6d65 727c 302e 3839 3931 7ce6  sformer|0.8991|.
-00005330: 9588 e69e 9ce8 be83 e5b7 ae0a 2020 2020  ............    
-00005340: 2020 2020 4245 5254 2d62 6173 657c 2a2a      BERT-base|**
-00005350: 302e 3934 3833 2a2a 7c62 6572 7420 2b20  0.9483**|bert + 
-00005360: 6663 0a20 2020 2020 2020 2045 524e 4945  fc.        ERNIE
-00005370: 7c30 2e39 3436 317c e6af 9462 6572 74e7  |0.9461|...bert.
-00005380: 95a5 e5b7 ae0a 2020 2020 2020 2020 0a20  ......        . 
-00005390: 2020 2020 2020 20e5 9ca8 e4b8 ade6 9687         .........
-000053a0: e696 b0e9 97bb e79f ade6 9687 e69c ace5  ................
-000053b0: 8886 e7b1 bbe6 95b0 e68d aee9 9b86 544e  ..............TN
-000053c0: 4557 53e4 b88a e8af 84e4 bcb0 efbc 8ce6  EWS.............
-000053d0: a8a1 e59e 8be5 9ca8 e5bc 80e5 8f91 e99b  ................
-000053e0: 8628 6465 7629 e8af 84e6 b58b e695 88e6  .(dev)..........
-000053f0: 9e9c e5a6 82e4 b88b efbc 9a0a 2020 2020  ............    
-00005400: 2020 2020 0a20 2020 2020 2020 20e6 a8a1      .        ...
-00005410: e59e 8b7c 6163 637c e8af b4e6 988e 0a20  ...|acc|....... 
-00005420: 2020 2020 2020 202d 2d7c 2d2d 7c2d 2d0a         --|--|--.
-00005430: 2020 2020 2020 2020 4245 5254 2d62 6173          BERT-bas
-00005440: 657c 2a2a 302e 3536 3630 2a2a 7ce6 9cac  e|**0.5660**|...
-00005450: e9a1 b9e7 9bae e5ae 9ee7 8eb0 0a20 2020  .............   
-00005460: 2020 2020 2042 4552 542d 6261 7365 7c30       BERT-base|0
-00005470: 2e35 3630 397c 434c 5545 2042 656e 6368  .5609|CLUE Bench
-00005480: 6d61 726b 204c 6561 6465 7262 6f61 7264  mark Leaderboard
-00005490: e7bb 93e6 9e9c 205b 434c 5545 6265 6e63  ...... [CLUEbenc
-000054a0: 686d 6172 6b5d 2868 7474 7073 3a2f 2f67  hmark](https://g
-000054b0: 6974 6875 622e 636f 6d2f 434c 5545 6265  ithub.com/CLUEbe
-000054c0: 6e63 686d 6172 6b2f 434c 5545 290a 2020  nchmark/CLUE).  
-000054d0: 2020 2020 2020 0a20 2020 2020 2020 202d        .        -
-000054e0: 20e4 bba5 e4b8 8ae7 bb93 e69e 9ce5 9d87   ...............
-000054f0: e4b8 bae5 8886 e7b1 bbe7 9a84 e587 86e7  ................
-00005500: a1ae e78e 87ef bc88 6163 6375 7261 6379  ........accuracy
-00005510: efbc 89e7 bb93 e69e 9c0a 2020 2020 2020  ..........      
-00005520: 2020 2d20 5448 5543 4e65 7773 e695 b0e6    - THUCNews....
-00005530: 8dae e99b 86e8 af84 e6b5 8be7 bb93 e69e  ................
-00005540: 9ce5 8faf e4bb a5e5 9fba e4ba 8e60 6578  .............`ex
-00005550: 616d 706c 6573 2f74 6875 636e 6577 735f  amples/thucnews_
-00005560: 7472 6169 6e5f 3130 772e 7478 7460 e695  train_10w.txt`..
-00005570: b0e6 8dae e794 a860 6578 616d 706c 6573  .......`examples
-00005580: 60e4 b88b e79a 84e5 9084 e6a8 a1e5 9e8b  `...............
-00005590: 6465 6d6f e5a4 8de7 8eb0 0a20 2020 2020  demo.......     
-000055a0: 2020 202d 2054 4e45 5753 e695 b0e6 8dae     - TNEWS......
-000055b0: e99b 86e8 af84 e6b5 8be7 bb93 e69e 9ce5  ................
-000055c0: 8faf e4bb a5e4 b88b e8bd bd54 4e45 5753  ...........TNEWS
-000055d0: e695 b0e6 8dae e99b 86ef bc8c e8bf 90e8  ................
-000055e0: a18c 6065 7861 6d70 6c65 732f 6265 7274  ..`examples/bert
-000055f0: 5f63 6c61 7373 6966 6963 6174 696f 6e5f  _classification_
-00005600: 746e 6577 735f 6465 6d6f 2e70 7960 e5a4  tnews_demo.py`..
-00005610: 8de7 8eb0 0a20 2020 2020 2020 200a 2020  .....        .  
-00005620: 2020 2020 2020 2323 2320 e591 bde4 bba4        ### ......
-00005630: e8a1 8ce8 b083 e794 a80a 2020 2020 2020  ..........      
-00005640: 2020 0a20 2020 2020 2020 20e6 8f90 e4be    .        .....
-00005650: 9be5 8886 e7b1 bbe6 a8a1 e59e 8be5 91bd  ................
-00005660: e4bb a4e8 a18c e8b0 83e7 94a8 e884 9ae6  ................
-00005670: 9cac efbc 8ce6 9687 e4bb b6e6 a091 efbc  ................
-00005680: 9a0a 2020 2020 2020 2020 6060 6062 6173  ..        ```bas
-00005690: 680a 2020 2020 2020 2020 7079 7465 7874  h.        pytext
-000056a0: 636c 6173 7369 6669 6572 0a20 2020 2020  classifier.     
-000056b0: 2020 20e2 949c e294 80e2 9480 2062 6572     ......... ber
-000056c0: 745f 636c 6173 7369 6669 6572 2e70 790a  t_classifier.py.
-000056d0: 2020 2020 2020 2020 e294 9ce2 9480 e294          ........
-000056e0: 8020 6661 7374 7465 7874 5f63 6c61 7373  . fasttext_class
-000056f0: 6966 6965 722e 7079 0a20 2020 2020 2020  ifier.py.       
-00005700: 20e2 949c e294 80e2 9480 2063 6c61 7373   ......... class
-00005710: 6963 5f63 6c61 7373 6966 6965 722e 7079  ic_classifier.py
-00005720: 0a20 2020 2020 2020 20e2 949c e294 80e2  .        .......
-00005730: 9480 2074 6578 7463 6e6e 5f63 6c61 7373  .. textcnn_class
-00005740: 6966 6965 722e 7079 0a20 2020 2020 2020  ifier.py.       
-00005750: 20e2 9494 e294 80e2 9480 2074 6578 7472   ......... textr
-00005760: 6e6e 5f63 6c61 7373 6966 6965 722e 7079  nn_classifier.py
-00005770: 0a20 2020 2020 2020 2060 6060 0a20 2020  .        ```.   
-00005780: 2020 2020 200a 2020 2020 2020 2020 e6af       .        ..
-00005790: 8fe4 b8aa e696 87e4 bbb6 e5af b9e5 ba94  ................
-000057a0: e4b8 80e4 b8aa e6a8 a1e5 9e8b e696 b9e6  ................
-000057b0: b395 efbc 8ce5 9084 e6a8 a1e5 9e8b e5ae  ................
-000057c0: 8ce5 85a8 e78b ace7 ab8b efbc 8ce5 8faf  ................
-000057d0: e4bb a5e7 9bb4 e68e a5e8 bf90 e8a1 8cef  ................
-000057e0: bc8c e4b9 9fe6 96b9 e4be bfe4 bfae e694  ................
-000057f0: b9ef bc8c e694 afe6 8c81 e980 9ae8 bf87  ................
-00005800: 6061 7267 7061 7273 6560 20e4 bfae e694  `argparse` .....
-00005810: b960 2d2d 6461 7461 5f70 6174 6860 e7ad  .`--data_path`..
-00005820: 89e5 8f82 e695 b0e3 8082 0a20 2020 2020  ...........     
-00005830: 2020 200a 2020 2020 2020 2020 e79b b4e6     .        ....
-00005840: 8ea5 e59c a8e7 bb88 e7ab afe8 b083 e794  ................
-00005850: a866 6173 7474 6578 74e6 a8a1 e59e 8be8  .fasttext.......
-00005860: aead e7bb 83ef bc9a 0a20 2020 2020 2020  .........       
-00005870: 2060 6060 6261 7368 0a20 2020 2020 2020   ```bash.       
-00005880: 2070 7974 686f 6e20 2d6d 2070 7974 6578   python -m pytex
-00005890: 7463 6c61 7373 6966 6965 722e 6661 7374  tclassifier.fast
-000058a0: 7465 7874 5f63 6c61 7373 6966 6965 7220  text_classifier 
-000058b0: 2d68 0a20 2020 2020 2020 2060 6060 0a20  -h.        ```. 
-000058c0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-000058d0: 2323 2054 6578 7420 436c 7573 7465 720a  ## Text Cluster.
-000058e0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-000058f0: 200a 2020 2020 2020 2020 5465 7874 2063   .        Text c
-00005900: 6c75 7374 6572 696e 672c 2066 6f72 2065  lustering, for e
-00005910: 7861 6d70 6c65 205b 6578 616d 706c 6573  xample [examples
-00005920: 2f63 6c75 7374 6572 5f64 656d 6f2e 7079  /cluster_demo.py
-00005930: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00005940: 2e63 6f6d 2f73 6869 6269 6e67 3632 342f  .com/shibing624/
-00005950: 7079 7465 7874 636c 6173 7369 6669 6572  pytextclassifier
-00005960: 2f62 6c6f 622f 6d61 7374 6572 2f65 7861  /blob/master/exa
-00005970: 6d70 6c65 732f 636c 7573 7465 725f 6465  mples/cluster_de
-00005980: 6d6f 2e70 7929 0a20 2020 2020 2020 200a  mo.py).        .
-00005990: 2020 2020 2020 2020 6060 6070 7974 686f          ```pytho
-000059a0: 6e0a 2020 2020 2020 2020 696d 706f 7274  n.        import
-000059b0: 2073 7973 0a20 2020 2020 2020 200a 2020   sys.        .  
-000059c0: 2020 2020 2020 7379 732e 7061 7468 2e61        sys.path.a
-000059d0: 7070 656e 6428 272e 2e27 290a 2020 2020  ppend('..').    
-000059e0: 2020 2020 6672 6f6d 2070 7974 6578 7463      from pytextc
-000059f0: 6c61 7373 6966 6965 722e 7465 7874 636c  lassifier.textcl
-00005a00: 7573 7465 7220 696d 706f 7274 2054 6578  uster import Tex
-00005a10: 7443 6c75 7374 6572 0a20 2020 2020 2020  tCluster.       
-00005a20: 200a 2020 2020 2020 2020 6966 205f 5f6e   .        if __n
-00005a30: 616d 655f 5f20 3d3d 2027 5f5f 6d61 696e  ame__ == '__main
-00005a40: 5f5f 273a 0a20 2020 2020 2020 2020 2020  __':.           
-00005a50: 206d 203d 2054 6578 7443 6c75 7374 6572   m = TextCluster
-00005a60: 286f 7574 7075 745f 6469 723d 276d 6f64  (output_dir='mod
-00005a70: 656c 732f 636c 7573 7465 722d 746f 7927  els/cluster-toy'
-00005a80: 2c20 6e5f 636c 7573 7465 7273 3d32 290a  , n_clusters=2).
-00005a90: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00005aa0: 7428 6d29 0a20 2020 2020 2020 2020 2020  t(m).           
-00005ab0: 2064 6174 6120 3d20 5b0a 2020 2020 2020   data = [.      
-00005ac0: 2020 2020 2020 2020 2020 2753 7475 6465            'Stude
-00005ad0: 6e74 2064 6562 7420 746f 2063 6f73 7420  nt debt to cost 
-00005ae0: 4272 6974 6169 6e20 6269 6c6c 696f 6e73  Britain billions
-00005af0: 2077 6974 6869 6e20 6465 6361 6465 7327   within decades'
-00005b00: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00005b10: 2020 2743 6869 6e65 7365 2065 6475 6361    'Chinese educa
-00005b20: 7469 6f6e 2066 6f72 2054 5620 6578 7065  tion for TV expe
-00005b30: 7269 6d65 6e74 272c 0a20 2020 2020 2020  riment',.       
-00005b40: 2020 2020 2020 2020 2027 4162 626f 7474           'Abbott
-00005b50: 2067 6f76 6572 6e6d 656e 7420 7370 656e   government spen
-00005b60: 6473 2024 3820 6d69 6c6c 696f 6e20 6f6e  ds $8 million on
-00005b70: 2068 6967 6865 7220 6564 7563 6174 696f   higher educatio
-00005b80: 6e27 2c0a 2020 2020 2020 2020 2020 2020  n',.            
-00005b90: 2020 2020 274d 6964 646c 6520 4561 7374      'Middle East
-00005ba0: 2061 6e64 2041 7369 6120 626f 6f73 7420   and Asia boost 
-00005bb0: 696e 7665 7374 6d65 6e74 2069 6e20 746f  investment in to
-00005bc0: 7020 6c65 7665 6c20 7370 6f72 7473 272c  p level sports',
-00005bd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005be0: 2027 5375 6d6d 6974 2053 6572 6965 7320   'Summit Series 
-00005bf0: 6c6f 6f6b 206c 6175 6e63 6865 7320 4842  look launches HB
-00005c00: 4f20 4361 6e61 6461 2073 706f 7274 7320  O Canada sports 
-00005c10: 646f 6320 7365 7269 6573 3a20 4d75 6468  doc series: Mudh
-00005c20: 6172 270a 2020 2020 2020 2020 2020 2020  ar'.            
-00005c30: 5d0a 2020 2020 2020 2020 2020 2020 6d2e  ].            m.
-00005c40: 7472 6169 6e28 6461 7461 290a 2020 2020  train(data).    
-00005c50: 2020 2020 2020 2020 6d2e 6c6f 6164 5f6d          m.load_m
-00005c60: 6f64 656c 2829 0a20 2020 2020 2020 2020  odel().         
-00005c70: 2020 2072 203d 206d 2e70 7265 6469 6374     r = m.predict
-00005c80: 285b 2741 6262 6f74 7420 676f 7665 726e  (['Abbott govern
-00005c90: 6d65 6e74 2073 7065 6e64 7320 2438 206d  ment spends $8 m
-00005ca0: 696c 6c69 6f6e 206f 6e20 6869 6768 6572  illion on higher
-00005cb0: 2065 6475 6361 7469 6f6e 206d 6564 6961   education media
-00005cc0: 2062 6c69 747a 272c 0a20 2020 2020 2020   blitz',.       
-00005cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ce0: 2020 2020 274d 6964 646c 6520 4561 7374      'Middle East
-00005cf0: 2061 6e64 2041 7369 6120 626f 6f73 7420   and Asia boost 
-00005d00: 696e 7665 7374 6d65 6e74 2069 6e20 746f  investment in to
-00005d10: 7020 6c65 7665 6c20 7370 6f72 7473 275d  p level sports']
-00005d20: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
-00005d30: 696e 7428 7229 0a20 2020 2020 2020 200a  int(r).        .
-00005d40: 2020 2020 2020 2020 2020 2020 2323 2323              ####
-00005d50: 2323 2323 2323 2320 6c6f 6164 2063 6869  ####### load chi
-00005d60: 6e65 7365 2074 7261 696e 2064 6174 6120  nese train data 
-00005d70: 6672 6f6d 2031 7720 6461 7461 2066 696c  from 1w data fil
-00005d80: 650a 2020 2020 2020 2020 2020 2020 6672  e.            fr
-00005d90: 6f6d 2073 6b6c 6561 726e 2e66 6561 7475  om sklearn.featu
-00005da0: 7265 5f65 7874 7261 6374 696f 6e2e 7465  re_extraction.te
-00005db0: 7874 2069 6d70 6f72 7420 5466 6964 6656  xt import TfidfV
-00005dc0: 6563 746f 7269 7a65 720a 2020 2020 2020  ectorizer.      
-00005dd0: 2020 0a20 2020 2020 2020 2020 2020 2074    .            t
-00005de0: 636c 7573 7465 7220 3d20 5465 7874 436c  cluster = TextCl
-00005df0: 7573 7465 7228 6f75 7470 7574 5f64 6972  uster(output_dir
-00005e00: 3d27 6d6f 6465 6c73 2f63 6c75 7374 6572  ='models/cluster
-00005e10: 272c 2066 6561 7475 7265 3d54 6669 6466  ', feature=Tfidf
-00005e20: 5665 6374 6f72 697a 6572 286e 6772 616d  Vectorizer(ngram
-00005e30: 5f72 616e 6765 3d28 312c 2032 2929 2c20  _range=(1, 2)), 
-00005e40: 6e5f 636c 7573 7465 7273 3d31 3029 0a20  n_clusters=10). 
-00005e50: 2020 2020 2020 2020 2020 2064 6174 6120             data 
-00005e60: 3d20 7463 6c75 7374 6572 2e6c 6f61 645f  = tcluster.load_
-00005e70: 6669 6c65 5f64 6174 6128 2774 6875 636e  file_data('thucn
-00005e80: 6577 735f 7472 6169 6e5f 3177 2e74 7874  ews_train_1w.txt
-00005e90: 272c 2073 6570 3d27 5c74 272c 2075 7365  ', sep='\t', use
-00005ea0: 5f63 6f6c 3d31 290a 2020 2020 2020 2020  _col=1).        
-00005eb0: 2020 2020 6665 6174 7572 652c 206c 6162      feature, lab
-00005ec0: 656c 7320 3d20 7463 6c75 7374 6572 2e74  els = tcluster.t
-00005ed0: 7261 696e 2864 6174 615b 3a35 3030 305d  rain(data[:5000]
-00005ee0: 290a 2020 2020 2020 2020 2020 2020 7463  ).            tc
-00005ef0: 6c75 7374 6572 2e73 686f 775f 636c 7573  luster.show_clus
-00005f00: 7465 7273 2866 6561 7475 7265 2c20 6c61  ters(feature, la
-00005f10: 6265 6c73 2c20 276d 6f64 656c 732f 636c  bels, 'models/cl
-00005f20: 7573 7465 722f 636c 7573 7465 725f 7472  uster/cluster_tr
-00005f30: 6169 6e5f 7365 675f 7361 6d70 6c65 732e  ain_seg_samples.
-00005f40: 706e 6727 290a 2020 2020 2020 2020 2020  png').          
-00005f50: 2020 7220 3d20 7463 6c75 7374 6572 2e70    r = tcluster.p
-00005f60: 7265 6469 6374 2864 6174 615b 3a33 305d  redict(data[:30]
-00005f70: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
-00005f80: 696e 7428 7229 0a20 2020 2020 2020 2060  int(r).        `
-00005f90: 6060 0a20 2020 2020 2020 200a 2020 2020  ``.        .    
-00005fa0: 2020 2020 6f75 7470 7574 3a0a 2020 2020      output:.    
-00005fb0: 2020 2020 0a20 2020 2020 2020 2060 6060      .        ```
-00005fc0: 0a20 2020 2020 2020 2054 6578 7443 6c75  .        TextClu
-00005fd0: 7374 6572 2069 6e73 7461 6e63 6520 284d  ster instance (M
-00005fe0: 696e 6942 6174 6368 4b4d 6561 6e73 286e  iniBatchKMeans(n
-00005ff0: 5f63 6c75 7374 6572 733d 322c 206e 5f69  _clusters=2, n_i
-00006000: 6e69 743d 3130 292c 203c 7079 7465 7874  nit=10), <pytext
-00006010: 636c 6173 7369 6669 6572 2e75 7469 6c73  classifier.utils
-00006020: 2e74 6f6b 656e 697a 6572 2e54 6f6b 656e  .tokenizer.Token
-00006030: 697a 6572 206f 626a 6563 7420 6174 2030  izer object at 0
-00006040: 7837 6638 3062 6434 3638 3262 303e 2c20  x7f80bd4682b0>, 
-00006050: 5466 6964 6656 6563 746f 7269 7a65 7228  TfidfVectorizer(
-00006060: 6e67 7261 6d5f 7261 6e67 653d 2831 2c20  ngram_range=(1, 
-00006070: 3229 2929 0a20 2020 2020 2020 205b 3120  2))).        [1 
-00006080: 3120 3120 3120 3120 3120 3120 3120 3120  1 1 1 1 1 1 1 1 
-00006090: 3120 3120 3820 3120 3120 3120 3120 3120  1 1 8 1 1 1 1 1 
-000060a0: 3120 3120 3120 3120 3120 3920 3120 3120  1 1 1 1 1 9 1 1 
-000060b0: 3820 3120 3120 3920 315d 0a20 2020 2020  8 1 1 9 1].     
-000060c0: 2020 2060 6060 0a20 2020 2020 2020 2063     ```.        c
-000060d0: 6c75 7374 6572 696e 6720 706c 6f74 2069  lustering plot i
-000060e0: 6d61 6765 3a0a 2020 2020 2020 2020 0a20  mage:.        . 
-000060f0: 2020 2020 2020 2021 5b63 6c75 7374 6572         ![cluster
-00006100: 5f69 6d61 6765 5d28 6874 7470 733a 2f2f  _image](https://
-00006110: 6769 7468 7562 2e63 6f6d 2f73 6869 6269  github.com/shibi
-00006120: 6e67 3632 342f 7079 7465 7874 636c 6173  ng624/pytextclas
-00006130: 7369 6669 6572 2f62 6c6f 622f 6d61 7374  sifier/blob/mast
-00006140: 6572 2f64 6f63 732f 636c 7573 7465 725f  er/docs/cluster_
-00006150: 7472 6169 6e5f 7365 675f 7361 6d70 6c65  train_seg_sample
-00006160: 732e 706e 6729 0a20 2020 2020 2020 200a  s.png).        .
-00006170: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00006180: 2023 2320 436f 6e74 6163 740a 2020 2020   ## Contact.    
-00006190: 2020 2020 0a20 2020 2020 2020 202d 2049      .        - I
-000061a0: 7373 7565 28e5 bbba e8ae ae29 efbc 9a5b  ssue(......)...[
-000061b0: 215b 4769 7448 7562 2069 7373 7565 735d  ![GitHub issues]
-000061c0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-000061d0: 656c 6473 2e69 6f2f 6769 7468 7562 2f69  elds.io/github/i
-000061e0: 7373 7565 732f 7368 6962 696e 6736 3234  ssues/shibing624
-000061f0: 2f70 7974 6578 7463 6c61 7373 6966 6965  /pytextclassifie
-00006200: 722e 7376 6729 5d28 6874 7470 733a 2f2f  r.svg)](https://
-00006210: 6769 7468 7562 2e63 6f6d 2f73 6869 6269  github.com/shibi
-00006220: 6e67 3632 342f 7079 7465 7874 636c 6173  ng624/pytextclas
-00006230: 7369 6669 6572 2f69 7373 7565 7329 0a20  sifier/issues). 
-00006240: 2020 2020 2020 202d 20e9 82ae e4bb b6e6         - .......
-00006250: 8891 efbc 9a78 756d 696e 673a 2078 756d  .....xuming: xum
-00006260: 696e 6736 3234 4071 712e 636f 6d0a 2020  ing624@qq.com.  
-00006270: 2020 2020 2020 2d20 e5be aee4 bfa1 e688        - ........
-00006280: 91ef bc9a e58a a0e6 8891 2ae5 beae e4bf  ..........*.....
-00006290: a1e5 8fb7 efbc 9a78 756d 696e 6736 3234  .......xuming624
-000062a0: 2a2c 20e8 bf9b 5079 7468 6f6e 2d4e 4c50  *, ...Python-NLP
-000062b0: e4ba a4e6 b581 e7be a4ef bc8c e5a4 87e6  ................
-000062c0: b3a8 efbc 9a2a e5a7 93e5 908d 2de5 85ac  .....*......-...
-000062d0: e58f b8e5 908d 2d4e 4c50 2a0a 2020 2020  ......-NLP*.    
-000062e0: 2020 2020 3c69 6d67 2073 7263 3d22 646f      <img src="do
-000062f0: 6373 2f77 6563 6861 742e 6a70 6567 2220  cs/wechat.jpeg" 
-00006300: 7769 6474 683d 2232 3030 2220 2f3e 0a20  width="200" />. 
-00006310: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00006320: 0a20 2020 2020 2020 2023 2320 4369 7461  .        ## Cita
-00006330: 7469 6f6e 0a20 2020 2020 2020 200a 2020  tion.        .  
-00006340: 2020 2020 2020 e5a6 82e6 9e9c e4bd a0e5        ..........
-00006350: 9ca8 e7a0 94e7 a9b6 e4b8 ade4 bdbf e794  ................
-00006360: a8e4 ba86 7079 7465 7874 636c 6173 7369  ....pytextclassi
-00006370: 6669 6572 efbc 8ce8 afb7 e68c 89e5 a682  fier............
-00006380: e4b8 8be6 a0bc e5bc 8fe5 bc95 e794 a8ef  ................
-00006390: bc9a 0a20 2020 2020 2020 200a 2020 2020  ...        .    
-000063a0: 2020 2020 4150 413a 0a20 2020 2020 2020      APA:.       
-000063b0: 2060 6060 6c61 7465 780a 2020 2020 2020   ```latex.      
-000063c0: 2020 5875 2c20 4d2e 2050 7974 6578 7463    Xu, M. Pytextc
-000063d0: 6c61 7373 6966 6965 723a 2054 6578 7420  lassifier: Text 
-000063e0: 636c 6173 7369 6669 6572 2074 6f6f 6c6b  classifier toolk
-000063f0: 6974 2066 6f72 204e 4c50 2028 5665 7273  it for NLP (Vers
-00006400: 696f 6e20 312e 322e 3029 205b 436f 6d70  ion 1.2.0) [Comp
-00006410: 7574 6572 2073 6f66 7477 6172 655d 2e20  uter software]. 
-00006420: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00006430: 6f6d 2f73 6869 6269 6e67 3632 342f 7079  om/shibing624/py
-00006440: 7465 7874 636c 6173 7369 6669 6572 0a20  textclassifier. 
-00006450: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
-00006460: 2020 200a 2020 2020 2020 2020 4269 6254     .        BibT
-00006470: 6558 3a0a 2020 2020 2020 2020 6060 606c  eX:.        ```l
-00006480: 6174 6578 0a20 2020 2020 2020 2040 6d69  atex.        @mi
-00006490: 7363 7b50 7974 6578 7463 6c61 7373 6966  sc{Pytextclassif
-000064a0: 6965 722c 0a20 2020 2020 2020 2020 2074  ier,.          t
-000064b0: 6974 6c65 3d7b 5079 7465 7874 636c 6173  itle={Pytextclas
-000064c0: 7369 6669 6572 3a20 5465 7874 2063 6c61  sifier: Text cla
-000064d0: 7373 6966 6965 7220 746f 6f6c 6b69 7420  ssifier toolkit 
-000064e0: 666f 7220 4e4c 507d 2c0a 2020 2020 2020  for NLP},.      
-000064f0: 2020 2020 6175 7468 6f72 3d7b 5875 204d      author={Xu M
-00006500: 696e 677d 2c0a 2020 2020 2020 2020 2020  ing},.          
-00006510: 7965 6172 3d7b 3230 3232 7d2c 0a20 2020  year={2022},.   
-00006520: 2020 2020 2020 2068 6f77 7075 626c 6973         howpublis
-00006530: 6865 643d 7b5c 7572 6c7b 6874 7470 733a  hed={\url{https:
-00006540: 2f2f 6769 7468 7562 2e63 6f6d 2f73 6869  //github.com/shi
-00006550: 6269 6e67 3632 342f 7079 7465 7874 636c  bing624/pytextcl
-00006560: 6173 7369 6669 6572 7d7d 2c0a 2020 2020  assifier}},.    
-00006570: 2020 2020 7d0a 2020 2020 2020 2020 6060      }.        ``
-00006580: 600a 2020 2020 2020 2020 0a20 2020 2020  `.        .     
-00006590: 2020 200a 2020 2020 2020 2020 2323 204c     .        ## L
-000065a0: 6963 656e 7365 0a20 2020 2020 2020 200a  icense.        .
-000065b0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-000065c0: 20e6 8e88 e69d 83e5 8d8f e8ae aee4 b8ba   ...............
-000065d0: 205b 5468 6520 4170 6163 6865 204c 6963   [The Apache Lic
-000065e0: 656e 7365 2032 2e30 5d28 4c49 4345 4e53  ense 2.0](LICENS
-000065f0: 4529 efbc 8ce5 8faf e585 8de8 b4b9 e794  E)..............
-00006600: a8e5 819a e595 86e4 b89a e794 a8e9 8094  ................
-00006610: e380 82e8 afb7 e59c a8e4 baa7 e593 81e8  ................
-00006620: afb4 e698 8ee4 b8ad e999 84e5 8aa0 2a2a  ..............**
-00006630: 7079 7465 7874 636c 6173 7369 6669 6572  pytextclassifier
-00006640: 2a2a e79a 84e9 93be e68e a5e5 928c e68e  **..............
-00006650: 88e6 9d83 e58d 8fe8 aeae e380 820a 2020  ..............  
-00006660: 2020 2020 2020 0a20 2020 2020 2020 200a        .        .
-00006670: 2020 2020 2020 2020 2323 2043 6f6e 7472          ## Contr
-00006680: 6962 7574 650a 2020 2020 2020 2020 e9a1  ibute.        ..
-00006690: b9e7 9bae e4bb a3e7 a081 e8bf 98e5 be88  ................
-000066a0: e7b2 97e7 b399 efbc 8ce5 a682 e69e 9ce5  ................
-000066b0: a4a7 e5ae b6e5 afb9 e4bb a3e7 a081 e69c  ................
-000066c0: 89e6 8980 e694 b9e8 bf9b efbc 8ce6 aca2  ................
-000066d0: e8bf 8ee6 8f90 e4ba a4e5 9b9e e69c ace9  ................
-000066e0: a1b9 e79b aeef bc8c e59c a8e6 8f90 e4ba  ................
-000066f0: a4e4 b98b e589 8def bc8c e6b3 a8e6 848f  ................
-00006700: e4bb a5e4 b88b e4b8 a4e7 82b9 efbc 9a0a  ................
-00006710: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00006720: 2020 2d20 e59c a860 7465 7374 7360 e6b7    - ...`tests`..
-00006730: bbe5 8aa0 e79b b8e5 ba94 e79a 84e5 8d95  ................
-00006740: e585 83e6 b58b e8af 950a 2020 2020 2020  ..........      
-00006750: 2020 202d 20e4 bdbf e794 a860 7079 7468     - ......`pyth
-00006760: 6f6e 2073 6574 7570 2e70 7920 7465 7374  on setup.py test
-00006770: 60e6 9da5 e8bf 90e8 a18c e689 80e6 9c89  `...............
-00006780: e58d 95e5 8583 e6b5 8be8 af95 efbc 8ce7  ................
-00006790: a1ae e4bf 9de6 8980 e69c 89e5 8d95 e6b5  ................
-000067a0: 8be9 83bd e698 afe9 809a e8bf 87e7 9a84  ................
-000067b0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-000067c0: 2020 e4b9 8be5 908e e58d b3e5 8faf e68f    ..............
-000067d0: 90e4 baa4 5052 e380 820a 2020 2020 2020  ....PR....      
-000067e0: 2020 0a20 2020 2020 2020 200a 4b65 7977    .        .Keyw
-000067f0: 6f72 6473 3a20 7079 7465 7874 636c 6173  ords: pytextclas
-00006800: 7369 6669 6572 2c74 6578 7463 6c61 7373  sifier,textclass
-00006810: 6966 6965 722c 636c 6173 7369 6669 6572  ifier,classifier
-00006820: 2c74 6578 7463 6c61 7373 6966 6963 6174  ,textclassificat
-00006830: 696f 6e0a 506c 6174 666f 726d 3a20 554e  ion.Platform: UN
-00006840: 4b4e 4f57 4e0a 436c 6173 7369 6669 6572  KNOWN.Classifier
-00006850: 3a20 496e 7465 6e64 6564 2041 7564 6965  : Intended Audie
-00006860: 6e63 6520 3a3a 2053 6369 656e 6365 2f52  nce :: Science/R
-00006870: 6573 6561 7263 680a 436c 6173 7369 6669  esearch.Classifi
-00006880: 6572 3a20 4f70 6572 6174 696e 6720 5379  er: Operating Sy
-00006890: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
-000068a0: 656e 6465 6e74 0a43 6c61 7373 6966 6965  endent.Classifie
-000068b0: 723a 204c 6963 656e 7365 203a 3a20 4f53  r: License :: OS
-000068c0: 4920 4170 7072 6f76 6564 203a 3a20 4170  I Approved :: Ap
-000068d0: 6163 6865 2053 6f66 7477 6172 6520 4c69  ache Software Li
-000068e0: 6365 6e73 650a 436c 6173 7369 6669 6572  cense.Classifier
-000068f0: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-00006900: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00006910: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-00006920: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00006930: 6520 3a3a 2050 7974 686f 6e20 3a3a 2032  e :: Python :: 2
-00006940: 2e37 0a43 6c61 7373 6966 6965 723a 2050  .7.Classifier: P
-00006950: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00006960: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00006970: 2033 0a43 6c61 7373 6966 6965 723a 2054   3.Classifier: T
-00006980: 6f70 6963 203a 3a20 5465 7874 2050 726f  opic :: Text Pro
-00006990: 6365 7373 696e 6720 3a3a 204c 696e 6775  cessing :: Lingu
-000069a0: 6973 7469 630a 436c 6173 7369 6669 6572  istic.Classifier
-000069b0: 3a20 546f 7069 6320 3a3a 2053 6369 656e  : Topic :: Scien
-000069c0: 7469 6669 632f 456e 6769 6e65 6572 696e  tific/Engineerin
-000069d0: 6720 3a3a 2041 7274 6966 6963 6961 6c20  g :: Artificial 
-000069e0: 496e 7465 6c6c 6967 656e 6365 0a44 6573  Intelligence.Des
-000069f0: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
-00006a00: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
-00006a10: 646f 776e 0a                             down.
+00003430: 7374 5f64 6174 6129 0a20 2020 2070 7269  st_data).    pri
+00003440: 6e74 2866 2761 6363 5f73 636f 7265 3a20  nt(f'acc_score: 
+00003450: 7b61 6363 5f73 636f 7265 7d27 290a 0a20  {acc_score}').. 
+00003460: 2020 2023 2074 7261 696e 206d 6f64 656c     # train model
+00003470: 2077 6974 6820 3177 2064 6174 6120 6669   with 1w data fi
+00003480: 6c65 2061 6e64 2031 3020 636c 6173 7365  le and 10 classe
+00003490: 730a 2020 2020 7072 696e 7428 272d 2720  s.    print('-' 
+000034a0: 2a20 3432 290a 2020 2020 6d20 3d20 4265  * 42).    m = Be
+000034b0: 7274 436c 6173 7369 6669 6572 286f 7574  rtClassifier(out
+000034c0: 7075 745f 6469 723d 276d 6f64 656c 732f  put_dir='models/
+000034d0: 6265 7274 2d63 6869 6e65 7365 272c 206e  bert-chinese', n
+000034e0: 756d 5f63 6c61 7373 6573 3d31 302c 0a20  um_classes=10,. 
+000034f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003500: 2020 2020 2020 6d6f 6465 6c5f 7479 7065        model_type
+00003510: 3d27 6265 7274 272c 206d 6f64 656c 5f6e  ='bert', model_n
+00003520: 616d 653d 2762 6572 742d 6261 7365 2d63  ame='bert-base-c
+00003530: 6869 6e65 7365 272c 206e 756d 5f65 706f  hinese', num_epo
+00003540: 6368 733d 322c 0a20 2020 2020 2020 2020  chs=2,.         
+00003550: 2020 2020 2020 2020 2020 2020 2020 6172                ar
+00003560: 6773 3d7b 226e 6f5f 6361 6368 6522 3a20  gs={"no_cache": 
+00003570: 5472 7565 2c20 226c 617a 795f 6c6f 6164  True, "lazy_load
+00003580: 696e 6722 3a20 5472 7565 2c20 226c 617a  ing": True, "laz
+00003590: 795f 7465 7874 5f63 6f6c 756d 6e22 3a20  y_text_column": 
+000035a0: 312c 2022 6c61 7a79 5f6c 6162 656c 735f  1, "lazy_labels_
+000035b0: 636f 6c75 6d6e 223a 2030 2c20 7d29 0a20  column": 0, }). 
+000035c0: 2020 2064 6174 615f 6669 6c65 203d 2027     data_file = '
+000035d0: 7468 7563 6e65 7773 5f74 7261 696e 5f31  thucnews_train_1
+000035e0: 772e 7478 7427 0a20 2020 2023 20e5 a682  w.txt'.    # ...
+000035f0: e69e 9ce8 aead e7bb 83e6 95b0 e68d aee8  ................
+00003600: b685 e8bf 87e7 99be e4b8 87e6 9da1 efbc  ................
+00003610: 8ce5 bbba e8ae aee4 bdbf e794 a86c 617a  .............laz
+00003620: 795f 6c6f 6164 696e 67e6 a8a1 e5bc 8fef  y_loading.......
+00003630: bc8c e587 8fe5 b091 e586 85e5 ad98 e58d  ................
+00003640: a0e7 94a8 0a20 2020 206d 2e74 7261 696e  .....    m.train
+00003650: 2864 6174 615f 6669 6c65 2c20 7465 7374  (data_file, test
+00003660: 5f73 697a 653d 302c 206e 616d 6573 3d28  _size=0, names=(
+00003670: 276c 6162 656c 7327 2c20 2774 6578 7427  'labels', 'text'
+00003680: 2929 0a20 2020 206d 2e6c 6f61 645f 6d6f  )).    m.load_mo
+00003690: 6465 6c28 290a 2020 2020 7072 6564 6963  del().    predic
+000036a0: 745f 6c61 6265 6c2c 2070 7265 6469 6374  t_label, predict
+000036b0: 5f70 726f 6261 203d 206d 2e70 7265 6469  _proba = m.predi
+000036c0: 6374 280a 2020 2020 2020 2020 5b27 e9a1  ct(.        ['..
+000036d0: bae4 b989 e58c 97e4 baac e88b 8fe6 b4bb  ................
+000036e0: 3838 e5b9 b3e7 b1b3 e8b5 b7e7 b2be e8a3  88..............
+000036f0: 85e6 88bf e59c a8e5 94ae 272c 0a20 2020  ..........',.   
+00003700: 2020 2020 2020 27e7 be8e 4542 2d35 e9a1        '...EB-5..
+00003710: b9e7 9bae e280 9c31 35e6 97a5 e5bf abe9  .......15.......
+00003720: 809f e7a7 bbe6 b091 e280 9de5 b086 e68e  ................
+00003730: a8e8 bf9f 272c 0a20 2020 2020 2020 2020  ....',.         
+00003740: 27e6 8192 e794 9f41 48e6 baa2 e68c 87e6  '......AH.......
+00003750: 94b6 e5b9 b320 41e8 82a1 e5af b948 e882  ..... A......H..
+00003760: a1e6 8a98 e4bb b731 2e39 3525 275d 290a  .......1.95%']).
+00003770: 2020 2020 7072 696e 7428 6627 7072 6564      print(f'pred
+00003780: 6963 745f 6c61 6265 6c3a 207b 7072 6564  ict_label: {pred
+00003790: 6963 745f 6c61 6265 6c7d 2c20 7072 6564  ict_label}, pred
+000037a0: 6963 745f 7072 6f62 613a 207b 7072 6564  ict_proba: {pred
+000037b0: 6963 745f 7072 6f62 617d 2729 0a60 6060  ict_proba}').```
+000037c0: 0a50 53ef bc9a e5a6 82e6 9e9c e8ae ade7  .PS.............
+000037d0: bb83 e695 b0e6 8dae e8b6 85e8 bf87 e799  ................
+000037e0: bee4 b887 e69d a1ef bc8c e5bb bae8 aeae  ................
+000037f0: e4bd bfe7 94a8 6c61 7a79 5f6c 6f61 6469  ......lazy_loadi
+00003800: 6e67 e6a8 a1e5 bc8f efbc 8ce5 878f e5b0  ng..............
+00003810: 91e5 8685 e5ad 98e5 8da0 e794 a80a 0a23  ...............#
+00003820: 2323 2320 e5a4 9ae6 a087 e7ad bee5 8886  ### ............
+00003830: e7b1 bbe6 a8a1 e59e 8b0a e588 86e7 b1bb  ................
+00003840: e58f afe4 bba5 e588 86e4 b8ba e5a4 9ae5  ................
+00003850: 8886 e7b1 bbe5 928c e5a4 9ae6 a087 e7ad  ................
+00003860: bee5 8886 e7b1 bbe3 8082 e5a4 9ae5 8886  ................
+00003870: e7b1 bbe7 9a84 e6a0 87e7 adbe e698 afe6  ................
+00003880: 8e92 e4bb 96e7 9a84 efbc 8ce8 808c e5a4  ................
+00003890: 9ae6 a087 e7ad bee5 8886 e7b1 bbe7 9a84  ................
+000038a0: e689 80e6 9c89 e6a0 87e7 adbe e698 afe4  ................
+000038b0: b88d e68e 92e4 bb96 e79a 84e3 8082 0a0a  ................
+000038c0: e5a4 9ae6 a087 e7ad bee5 8886 e7b1 bbe6  ................
+000038d0: af94 e8be 83e7 9bb4 e8a7 82e7 9a84 e790  ................
+000038e0: 86e8 a7a3 e698 afef bc8c e4b8 80e4 b8aa  ................
+000038f0: e6a0 b7e6 9cac e58f afe4 bba5 e590 8ce6  ................
+00003900: 97b6 e68b a5e6 9c89 e587 a0e4 b8aa e7b1  ................
+00003910: bbe5 88ab e6a0 87e7 adbe efbc 8c0a e6af  ................
+00003920: 94e5 a682 e4b8 80e9 a696 e6ad 8ce7 9a84  ................
+00003930: e6a0 87e7 adbe e58f afe4 bba5 e698 afe6  ................
+00003940: b581 e8a1 8ce3 8081 e8bd bbe5 bfab efbc  ................
+00003950: 8ce4 b880 e983 a8e7 94b5 e5bd b1e7 9a84  ................
+00003960: e6a0 87e7 adbe e58f afe4 bba5 e698 afe5  ................
+00003970: 8aa8 e4bd 9ce3 8081 e596 9ce5 89a7 e380  ................
+00003980: 81e6 909e e7ac 91e7 ad89 efbc 8ce8 bf99  ................
+00003990: e983 bde6 98af e5a4 9ae6 a087 e7ad bee5  ................
+000039a0: 8886 e7b1 bbe7 9a84 e683 85e5 86b5 e380  ................
+000039b0: 820a 0ae8 aead e7bb 83e5 928c e9a2 84e6  ................
+000039c0: b58b 6042 4552 5460 e5a4 9ae6 a087 e7ad  ..`BERT`........
+000039d0: bee5 8886 e7b1 bbe6 a8a1 e59e 8bef bc8c  ................
+000039e0: e7a4 bae4 be8b 5b65 7861 6d70 6c65 732f  ......[examples/
+000039f0: 6265 7274 5f6d 756c 7469 6c61 6265 6c5f  bert_multilabel_
+00003a00: 636c 6173 7369 6669 6361 7469 6f6e 5f7a  classification_z
+00003a10: 685f 6465 6d6f 2e70 792e 7079 5d28 6874  h_demo.py.py](ht
+00003a20: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00003a30: 2f73 6869 6269 6e67 3632 342f 7079 7465  /shibing624/pyte
+00003a40: 7874 636c 6173 7369 6669 6572 2f62 6c6f  xtclassifier/blo
+00003a50: 622f 6d61 7374 6572 2f65 7861 6d70 6c65  b/master/example
+00003a60: 732f 6265 7274 5f6d 756c 7469 6c61 6265  s/bert_multilabe
+00003a70: 6c5f 636c 6173 7369 6669 6361 7469 6f6e  l_classification
+00003a80: 5f7a 685f 6465 6d6f 2e70 7929 0a0a 6060  _zh_demo.py)..``
+00003a90: 6070 7974 686f 6e0a 696d 706f 7274 2073  `python.import s
+00003aa0: 7973 0a69 6d70 6f72 7420 7061 6e64 6173  ys.import pandas
+00003ab0: 2061 7320 7064 0a0a 7379 732e 7061 7468   as pd..sys.path
+00003ac0: 2e61 7070 656e 6428 272e 2e27 290a 6672  .append('..').fr
+00003ad0: 6f6d 2070 7974 6578 7463 6c61 7373 6966  om pytextclassif
+00003ae0: 6965 7220 696d 706f 7274 2042 6572 7443  ier import BertC
+00003af0: 6c61 7373 6966 6965 720a 0a0a 6465 6620  lassifier...def 
+00003b00: 6c6f 6164 5f6a 645f 6461 7461 2866 696c  load_jd_data(fil
+00003b10: 655f 7061 7468 293a 0a20 2020 2022 2222  e_path):.    """
+00003b20: 0a20 2020 204c 6f61 6420 6a64 2064 6174  .    Load jd dat
+00003b30: 6120 6672 6f6d 2066 696c 652e 0a20 2020  a from file..   
+00003b40: 2040 7061 7261 6d20 6669 6c65 5f70 6174   @param file_pat
+00003b50: 683a 200a 2020 2020 2020 2020 666f 726d  h: .        form
+00003b60: 6174 3a20 636f 6e74 656e 742c e585 b6e4  at: content,....
+00003b70: bb96 2ce4 ba92 e881 94e4 ba92 e980 9a2c  ..,............,
+00003b80: e4ba a7e5 9381 e58a 9fe8 8097 2ce6 bb91  ............,...
+00003b90: e8bd aee6 8f90 e689 8b2c e5a3 b0e9 9fb3  .........,......
+00003ba0: 2c41 5050 e693 8de6 8ea7 e680 a72c e591  ,APP.........,..
+00003bb0: bce5 90b8 e781 af2c e5a4 96e8 a782 2ce5  .......,......,.
+00003bc0: ba95 e5ba a72c e588 b6e7 83ad e88c 83e5  .....,..........
+00003bd0: 9bb4 2ce9 81a5 e68e a7e5 99a8 e794 b5e6  ..,.............
+00003be0: b1a0 2ce5 91b3 e981 932c e588 b6e7 83ad  ..,......,......
+00003bf0: e695 88e6 9e9c 2ce8 a1a3 e789 a9e7 8398  ......,.........
+00003c00: e5b9 b22c e4bd 93e7 a7af e5a4 a7e5 b08f  ...,............
+00003c10: 0a20 2020 2040 7265 7475 726e 3a20 0a20  .    @return: . 
+00003c20: 2020 2022 2222 0a20 2020 2064 6174 6120     """.    data 
+00003c30: 3d20 5b5d 0a20 2020 2077 6974 6820 6f70  = [].    with op
+00003c40: 656e 2866 696c 655f 7061 7468 2c20 2772  en(file_path, 'r
+00003c50: 272c 2065 6e63 6f64 696e 673d 2775 7466  ', encoding='utf
+00003c60: 2d38 2729 2061 7320 663a 0a20 2020 2020  -8') as f:.     
+00003c70: 2020 2066 6f72 206c 696e 6520 696e 2066     for line in f
+00003c80: 3a0a 2020 2020 2020 2020 2020 2020 6c69  :.            li
+00003c90: 6e65 203d 206c 696e 652e 7374 7269 7028  ne = line.strip(
+00003ca0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00003cb0: 206c 696e 652e 7374 6172 7473 7769 7468   line.startswith
+00003cc0: 2827 2327 293a 0a20 2020 2020 2020 2020  ('#'):.         
+00003cd0: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
+00003ce0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00003cf0: 6f74 206c 696e 653a 0a20 2020 2020 2020  ot line:.       
+00003d00: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
+00003d10: 650a 2020 2020 2020 2020 2020 2020 7465  e.            te
+00003d20: 726d 7320 3d20 6c69 6e65 2e73 706c 6974  rms = line.split
+00003d30: 2827 2c27 290a 2020 2020 2020 2020 2020  (',').          
+00003d40: 2020 6966 206c 656e 2874 6572 6d73 2920    if len(terms) 
+00003d50: 213d 2031 363a 0a20 2020 2020 2020 2020  != 16:.         
+00003d60: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
+00003d70: 2020 2020 2020 2020 2020 2020 7661 6c20              val 
+00003d80: 3d20 5b69 6e74 2869 2920 666f 7220 6920  = [int(i) for i 
+00003d90: 696e 2074 6572 6d73 5b31 3a5d 5d0a 2020  in terms[1:]].  
+00003da0: 2020 2020 2020 2020 2020 6461 7461 2e61            data.a
+00003db0: 7070 656e 6428 5b74 6572 6d73 5b30 5d2c  ppend([terms[0],
+00003dc0: 2076 616c 5d29 0a20 2020 2072 6574 7572   val]).    retur
+00003dd0: 6e20 6461 7461 0a0a 0a69 6620 5f5f 6e61  n data...if __na
+00003de0: 6d65 5f5f 203d 3d20 275f 5f6d 6169 6e5f  me__ == '__main_
+00003df0: 5f27 3a0a 2020 2020 2320 6d6f 6465 6c5f  _':.    # model_
+00003e00: 7479 7065 3a20 7375 7070 6f72 7420 2762  type: support 'b
+00003e10: 6572 7427 2c20 2761 6c62 6572 7427 2c20  ert', 'albert', 
+00003e20: 2772 6f62 6572 7461 272c 2027 786c 6e65  'roberta', 'xlne
+00003e30: 7427 0a20 2020 2023 206d 6f64 656c 5f6e  t'.    # model_n
+00003e40: 616d 653a 2073 7570 706f 7274 2027 6265  ame: support 'be
+00003e50: 7274 2d62 6173 652d 6368 696e 6573 6527  rt-base-chinese'
+00003e60: 2c20 2762 6572 742d 6261 7365 2d63 6173  , 'bert-base-cas
+00003e70: 6564 272c 2027 6265 7274 2d62 6173 652d  ed', 'bert-base-
+00003e80: 6d75 6c74 696c 696e 6775 616c 2d63 6173  multilingual-cas
+00003e90: 6564 2720 2e2e 2e0a 2020 2020 6d20 3d20  ed' ....    m = 
+00003ea0: 4265 7274 436c 6173 7369 6669 6572 286f  BertClassifier(o
+00003eb0: 7574 7075 745f 6469 723d 276d 6f64 656c  utput_dir='model
+00003ec0: 732f 6d75 6c74 696c 6162 656c 2d62 6572  s/multilabel-ber
+00003ed0: 742d 7a68 2d6d 6f64 656c 272c 206e 756d  t-zh-model', num
+00003ee0: 5f63 6c61 7373 6573 3d31 352c 0a20 2020  _classes=15,.   
+00003ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f00: 2020 2020 6d6f 6465 6c5f 7479 7065 3d27      model_type='
+00003f10: 6265 7274 272c 206d 6f64 656c 5f6e 616d  bert', model_nam
+00003f20: 653d 2762 6572 742d 6261 7365 2d63 6869  e='bert-base-chi
+00003f30: 6e65 7365 272c 206e 756d 5f65 706f 6368  nese', num_epoch
+00003f40: 733d 322c 206d 756c 7469 5f6c 6162 656c  s=2, multi_label
+00003f50: 3d54 7275 6529 0a20 2020 2023 2054 7261  =True).    # Tra
+00003f60: 696e 2061 6e64 2045 7661 6c75 6174 696f  in and Evaluatio
+00003f70: 6e20 6461 7461 206e 6565 6473 2074 6f20  n data needs to 
+00003f80: 6265 2069 6e20 6120 5061 6e64 6173 2044  be in a Pandas D
+00003f90: 6174 6166 7261 6d65 2063 6f6e 7461 696e  ataframe contain
+00003fa0: 696e 6720 6174 206c 6561 7374 2074 776f  ing at least two
+00003fb0: 2063 6f6c 756d 6e73 2c20 6120 2774 6578   columns, a 'tex
+00003fc0: 7427 2061 6e64 2061 2027 6c61 6265 6c73  t' and a 'labels
+00003fd0: 2720 636f 6c75 6d6e 2e20 5468 6520 606c  ' column. The `l
+00003fe0: 6162 656c 7360 2063 6f6c 756d 6e20 7368  abels` column sh
+00003ff0: 6f75 6c64 2063 6f6e 7461 696e 206d 756c  ould contain mul
+00004000: 7469 2d68 6f74 2065 6e63 6f64 6564 206c  ti-hot encoded l
+00004010: 6973 7473 2e0a 2020 2020 7472 6169 6e5f  ists..    train_
+00004020: 6461 7461 203d 205b 0a20 2020 2020 2020  data = [.       
+00004030: 205b 22e4 b880 e4b8 aae5 b08f e697 b6e6   [".............
+00004040: 88bf e997 b4e4 bb8d e784 b6e6 b2a1 e69a  ................
+00004050: 96e5 928c 222c 205b 302c 2030 2c20 302c  ....", [0, 0, 0,
+00004060: 2030 2c20 302c 2030 2c20 302c 2030 2c20   0, 0, 0, 0, 0, 
+00004070: 302c 2030 2c20 302c 2030 2c20 312c 2030  0, 0, 0, 0, 1, 0
+00004080: 2c20 305d 5d2c 0a20 2020 2020 2020 205b  , 0]],.        [
+00004090: 22e8 8097 e794 b5e6 8385 e586 b5ef bc9a  "...............
+000040a0: e8bf 99e4 b8aa e6b2 a1e6 9c89 e6b3 a8e6  ................
+000040b0: 848f 222c 205b 302c 2030 2c20 312c 2030  ..", [0, 0, 1, 0
+000040c0: 2c20 302c 2030 2c20 302c 2030 2c20 302c  , 0, 0, 0, 0, 0,
+000040d0: 2030 2c20 302c 2030 2c20 302c 2030 2c20   0, 0, 0, 0, 0, 
+000040e0: 305d 5d2c 0a20 2020 205d 0a20 2020 2064  0]],.    ].    d
+000040f0: 6174 6120 3d20 6c6f 6164 5f6a 645f 6461  ata = load_jd_da
+00004100: 7461 2827 6d75 6c74 696c 6162 656c 5f6a  ta('multilabel_j
+00004110: 645f 636f 6d6d 656e 7473 2e63 7376 2729  d_comments.csv')
+00004120: 0a20 2020 2074 7261 696e 5f64 6174 612e  .    train_data.
+00004130: 6578 7465 6e64 2864 6174 6129 0a20 2020  extend(data).   
+00004140: 2070 7269 6e74 2874 7261 696e 5f64 6174   print(train_dat
+00004150: 615b 3a35 5d29 0a20 2020 2074 7261 696e  a[:5]).    train
+00004160: 5f64 6620 3d20 7064 2e44 6174 6146 7261  _df = pd.DataFra
+00004170: 6d65 2874 7261 696e 5f64 6174 612c 2063  me(train_data, c
+00004180: 6f6c 756d 6e73 3d5b 2274 6578 7422 2c20  olumns=["text", 
+00004190: 226c 6162 656c 7322 5d29 0a0a 2020 2020  "labels"])..    
+000041a0: 7072 696e 7428 7472 6169 6e5f 6466 2e68  print(train_df.h
+000041b0: 6561 6428 2929 0a20 2020 206d 2e74 7261  ead()).    m.tra
+000041c0: 696e 2874 7261 696e 5f64 6629 0a20 2020  in(train_df).   
+000041d0: 2070 7269 6e74 286d 290a 2020 2020 2320   print(m).    # 
+000041e0: 4576 616c 7561 7465 2074 6865 206d 6f64  Evaluate the mod
+000041f0: 656c 0a20 2020 2061 6363 5f73 636f 7265  el.    acc_score
+00004200: 203d 206d 2e65 7661 6c75 6174 655f 6d6f   = m.evaluate_mo
+00004210: 6465 6c28 7472 6169 6e5f 6466 5b3a 3230  del(train_df[:20
+00004220: 5d29 0a20 2020 2070 7269 6e74 2866 2761  ]).    print(f'a
+00004230: 6363 5f73 636f 7265 3a20 7b61 6363 5f73  cc_score: {acc_s
+00004240: 636f 7265 7d27 290a 0a20 2020 2023 206c  core}')..    # l
+00004250: 6f61 6420 7472 6169 6e65 6420 6265 7374  oad trained best
+00004260: 206d 6f64 656c 2066 726f 6d20 6d6f 6465   model from mode
+00004270: 6c5f 6469 720a 2020 2020 6d2e 6c6f 6164  l_dir.    m.load
+00004280: 5f6d 6f64 656c 2829 0a20 2020 2070 7265  _model().    pre
+00004290: 6469 6374 5f6c 6162 656c 2c20 7072 6564  dict_label, pred
+000042a0: 6963 745f 7072 6f62 6120 3d20 6d2e 7072  ict_proba = m.pr
+000042b0: 6564 6963 7428 5b27 e4b8 80e4 b8aa e5b0  edict(['........
+000042c0: 8fe6 97b6 e688 bfe9 97b4 e4bb 8de7 84b6  ................
+000042d0: e6b2 a1e6 9a96 e592 8c27 2c20 27e8 8097  .........', '...
+000042e0: e794 b5e6 8385 e586 b5ef bc9a e8bf 99e4  ................
+000042f0: b8aa e6b2 a1e6 9c89 e6b3 a8e6 848f 275d  ..............']
+00004300: 290a 2020 2020 7072 696e 7428 6627 7072  ).    print(f'pr
+00004310: 6564 6963 745f 6c61 6265 6c3a 207b 7072  edict_label: {pr
+00004320: 6564 6963 745f 6c61 6265 6c7d 2c20 7072  edict_label}, pr
+00004330: 6564 6963 745f 7072 6f62 613a 207b 7072  edict_proba: {pr
+00004340: 6564 6963 745f 7072 6f62 617d 2729 0a60  edict_proba}').`
+00004350: 6060 0a0a 2323 2045 7661 6c75 6174 696f  ``..## Evaluatio
+00004360: 6e0a 0a23 2323 2044 6174 6173 6574 0a0a  n..### Dataset..
+00004370: 312e 2054 4855 434e 6577 73e4 b8ad e696  1. THUCNews.....
+00004380: 87e6 9687 e69c ace6 95b0 e68d aee9 9b86  ................
+00004390: efbc 8831 2e35 3647 42ef bc89 efbc 9ae5  ...1.56GB.......
+000043a0: ae98 e696 b95b e4b8 8be8 bdbd e59c b0e5  .....[..........
+000043b0: 9d80 5d28 6874 7470 3a2f 2f74 6875 6374  ..](http://thuct
+000043c0: 632e 7468 756e 6c70 2e6f 7267 2f29 efbc  c.thunlp.org/)..
+000043d0: 8ce6 8abd e6a0 b7e4 ba86 3130 e4b8 87e6  ..........10....
+000043e0: 9da1 5448 5543 4e65 7773 e4b8 ade6 9687  ..THUCNews......
+000043f0: e696 87e6 9cac 3130 e588 86e7 b1bb e695  ......10........
+00004400: b0e6 8dae e99b 86ef bc88 364d 42ef bc89  ..........6MB...
+00004410: efbc 8ce5 9cb0 e59d 80ef bc9a 5b65 7861  ............[exa
+00004420: 6d70 6c65 732f 7468 7563 6e65 7773 5f74  mples/thucnews_t
+00004430: 7261 696e 5f31 3077 2e74 7874 5d28 6874  rain_10w.txt](ht
+00004440: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00004450: 2f73 6869 6269 6e67 3632 342f 7079 7465  /shibing624/pyte
+00004460: 7874 636c 6173 7369 6669 6572 2f62 6c6f  xtclassifier/blo
+00004470: 622f 6d61 7374 6572 2f65 7861 6d70 6c65  b/master/example
+00004480: 732f 7468 7563 6e65 7773 5f74 7261 696e  s/thucnews_train
+00004490: 5f31 3077 2e74 7874 29e3 8082 0a32 2e20  _10w.txt)....2. 
+000044a0: 544e 4557 53e4 bb8a e697 a5e5 a4b4 e69d  TNEWS...........
+000044b0: a1e4 b8ad e696 87e6 96b0 e997 bbef bc88  ................
+000044c0: e79f ade6 9687 e69c acef bc89 e588 86e7  ................
+000044d0: b1bb 2053 686f 7274 2054 6578 7420 436c  .. Short Text Cl
+000044e0: 6173 7369 6669 6361 6974 6f6e 2066 6f72  assificaiton for
+000044f0: 204e 6577 73ef bc8c e8af a5e6 95b0 e68d   News...........
+00004500: aee9 9b86 2835 2e31 4d42 29e6 9da5 e887  ....(5.1MB).....
+00004510: aae4 bb8a e697 a5e5 a4b4 e69d a1e7 9a84  ................
+00004520: e696 b0e9 97bb e789 88e5 9d97 efbc 8ce5  ................
+00004530: 85b1 e68f 90e5 8f96 e4ba 8631 35e4 b8aa  ...........15...
+00004540: e7b1 bbe5 88ab e79a 84e6 96b0 e997 bbef  ................
+00004550: bc8c e58c 85e6 8bac e697 85e6 b8b8 efbc  ................
+00004560: 8ce6 9599 e882 b2ef bc8c e987 91e8 9e8d  ................
+00004570: efbc 8ce5 869b e4ba 8be7 ad89 efbc 8ce5  ................
+00004580: 9cb0 e59d 80ef bc9a 5b74 6e65 7773 5f70  ........[tnews_p
+00004590: 7562 6c69 632e 7a69 705d 2868 7474 7073  ublic.zip](https
+000045a0: 3a2f 2f73 746f 7261 6765 2e67 6f6f 676c  ://storage.googl
+000045b0: 6561 7069 732e 636f 6d2f 636c 7565 6265  eapis.com/cluebe
+000045c0: 6e63 686d 6172 6b2f 7461 736b 732f 746e  nchmark/tasks/tn
+000045d0: 6577 735f 7075 626c 6963 2e7a 6970 290a  ews_public.zip).
+000045e0: 0a23 2323 2045 7661 6c75 6174 696f 6e20  .### Evaluation 
+000045f0: 5265 7375 6c74 0ae5 9ca8 5448 5543 4e65  Result....THUCNe
+00004600: 7773 e4b8 ade6 9687 e696 87e6 9cac 3130  ws............10
+00004610: e588 86e7 b1bb e695 b0e6 8dae e99b 86ef  ................
+00004620: bc88 364d 42ef bc89 e4b8 8ae8 af84 e4bc  ..6MB...........
+00004630: b0ef bc8c e6a8 a1e5 9e8b e59c a8e6 b58b  ................
+00004640: e8af 95e9 9b86 2874 6573 7429 e8af 84e6  ......(test)....
+00004650: b58b e695 88e6 9e9c e5a6 82e4 b88b efbc  ................
+00004660: 9a0a 0ae6 a8a1 e59e 8b7c 6163 637c e8af  .........|acc|..
+00004670: b4e6 988e 0a2d 2d7c 2d2d 7c2d 2d0a 4c52  .....--|--|--.LR
+00004680: 7c30 2e38 3830 337c e980 bbe8 be91 e59b  |0.8803|........
+00004690: 9ee5 bd92 4c6f 6769 7374 6963 7320 5265  ....Logistics Re
+000046a0: 6772 6573 7369 6f6e 0a54 6578 7443 4e4e  gression.TextCNN
+000046b0: 7c30 2e38 3830 397c 4b69 6d20 3230 3134  |0.8809|Kim 2014
+000046c0: 20e7 bb8f e585 b8e7 9a84 434e 4ee6 9687   .........CNN...
+000046d0: e69c ace5 8886 e7b1 bb0a 5465 7874 524e  ..........TextRN
+000046e0: 4e5f 4174 747c 302e 3930 3232 7c42 694c  N_Att|0.9022|BiL
+000046f0: 5354 4d2b 4174 7465 6e74 696f 6e0a 4661  STM+Attention.Fa
+00004700: 7374 5465 7874 7c30 2e39 3137 377c 626f  stText|0.9177|bo
+00004710: 772b 6269 6772 616d 2b74 7269 6772 616d  w+bigram+trigram
+00004720: efbc 8c20 e695 88e6 9e9c e587 bae5 a587  ... ............
+00004730: e79a 84e5 a5bd 0a44 5043 4e4e 7c30 2e39  .......DPCNN|0.9
+00004740: 3132 357c e6b7 b1e5 b182 e987 91e5 ad97  125|............
+00004750: e5a1 9443 4e4e 0a54 7261 6e73 666f 726d  ...CNN.Transform
+00004760: 6572 7c30 2e38 3939 317c e695 88e6 9e9c  er|0.8991|......
+00004770: e8be 83e5 b7ae 0a42 4552 542d 6261 7365  .......BERT-base
+00004780: 7c2a 2a30 2e39 3438 332a 2a7c 6265 7274  |**0.9483**|bert
+00004790: 202b 2066 630a 4552 4e49 457c 302e 3934   + fc.ERNIE|0.94
+000047a0: 3631 7ce6 af94 6265 7274 e795 a5e5 b7ae  61|...bert......
+000047b0: 0a0a e59c a8e4 b8ad e696 87e6 96b0 e997  ................
+000047c0: bbe7 9fad e696 87e6 9cac e588 86e7 b1bb  ................
+000047d0: e695 b0e6 8dae e99b 8654 4e45 5753 e4b8  .........TNEWS..
+000047e0: 8ae8 af84 e4bc b0ef bc8c e6a8 a1e5 9e8b  ................
+000047f0: e59c a8e5 bc80 e58f 91e9 9b86 2864 6576  ............(dev
+00004800: 29e8 af84 e6b5 8be6 9588 e69e 9ce5 a682  )...............
+00004810: e4b8 8bef bc9a 0a0a e6a8 a1e5 9e8b 7c61  ..............|a
+00004820: 6363 7ce8 afb4 e698 8e0a 2d2d 7c2d 2d7c  cc|.......--|--|
+00004830: 2d2d 0a42 4552 542d 6261 7365 7c2a 2a30  --.BERT-base|**0
+00004840: 2e35 3636 302a 2a7c e69c ace9 a1b9 e79b  .5660**|........
+00004850: aee5 ae9e e78e b00a 4245 5254 2d62 6173  ........BERT-bas
+00004860: 657c 302e 3536 3039 7c43 4c55 4520 4265  e|0.5609|CLUE Be
+00004870: 6e63 686d 6172 6b20 4c65 6164 6572 626f  nchmark Leaderbo
+00004880: 6172 64e7 bb93 e69e 9c20 5b43 4c55 4562  ard...... [CLUEb
+00004890: 656e 6368 6d61 726b 5d28 6874 7470 733a  enchmark](https:
+000048a0: 2f2f 6769 7468 7562 2e63 6f6d 2f43 4c55  //github.com/CLU
+000048b0: 4562 656e 6368 6d61 726b 2f43 4c55 4529  Ebenchmark/CLUE)
+000048c0: 0a0a 2d20 e4bb a5e4 b88a e7bb 93e6 9e9c  ..- ............
+000048d0: e59d 87e4 b8ba e588 86e7 b1bb e79a 84e5  ................
+000048e0: 8786 e7a1 aee7 8e87 efbc 8861 6363 7572  ...........accur
+000048f0: 6163 79ef bc89 e7bb 93e6 9e9c 0a2d 2054  acy..........- T
+00004900: 4855 434e 6577 73e6 95b0 e68d aee9 9b86  HUCNews.........
+00004910: e8af 84e6 b58b e7bb 93e6 9e9c e58f afe4  ................
+00004920: bba5 e59f bae4 ba8e 6065 7861 6d70 6c65  ........`example
+00004930: 732f 7468 7563 6e65 7773 5f74 7261 696e  s/thucnews_train
+00004940: 5f31 3077 2e74 7874 60e6 95b0 e68d aee7  _10w.txt`.......
+00004950: 94a8 6065 7861 6d70 6c65 7360 e4b8 8be7  ..`examples`....
+00004960: 9a84 e590 84e6 a8a1 e59e 8b64 656d 6fe5  ...........demo.
+00004970: a48d e78e b00a 2d20 544e 4557 53e6 95b0  ......- TNEWS...
+00004980: e68d aee9 9b86 e8af 84e6 b58b e7bb 93e6  ................
+00004990: 9e9c e58f afe4 bba5 e4b8 8be8 bdbd 544e  ..............TN
+000049a0: 4557 53e6 95b0 e68d aee9 9b86 efbc 8ce8  EWS.............
+000049b0: bf90 e8a1 8c60 6578 616d 706c 6573 2f62  .....`examples/b
+000049c0: 6572 745f 636c 6173 7369 6669 6361 7469  ert_classificati
+000049d0: 6f6e 5f74 6e65 7773 5f64 656d 6f2e 7079  on_tnews_demo.py
+000049e0: 60e5 a48d e78e b00a 0a23 2323 20e5 91bd  `........### ...
+000049f0: e4bb a4e8 a18c e8b0 83e7 94a8 0a0a e68f  ................
+00004a00: 90e4 be9b e588 86e7 b1bb e6a8 a1e5 9e8b  ................
+00004a10: e591 bde4 bba4 e8a1 8ce8 b083 e794 a8e8  ................
+00004a20: 849a e69c acef bc8c e696 87e4 bbb6 e6a0  ................
+00004a30: 91ef bc9a 0a60 6060 6261 7368 0a70 7974  .....```bash.pyt
+00004a40: 6578 7463 6c61 7373 6966 6965 720a e294  extclassifier...
+00004a50: 9ce2 9480 e294 8020 6265 7274 5f63 6c61  ....... bert_cla
+00004a60: 7373 6966 6965 722e 7079 0ae2 949c e294  ssifier.py......
+00004a70: 80e2 9480 2066 6173 7474 6578 745f 636c  .... fasttext_cl
+00004a80: 6173 7369 6669 6572 2e70 790a e294 9ce2  assifier.py.....
+00004a90: 9480 e294 8020 636c 6173 7369 635f 636c  ..... classic_cl
+00004aa0: 6173 7369 6669 6572 2e70 790a e294 9ce2  assifier.py.....
+00004ab0: 9480 e294 8020 7465 7874 636e 6e5f 636c  ..... textcnn_cl
+00004ac0: 6173 7369 6669 6572 2e70 790a e294 94e2  assifier.py.....
+00004ad0: 9480 e294 8020 7465 7874 726e 6e5f 636c  ..... textrnn_cl
+00004ae0: 6173 7369 6669 6572 2e70 790a 6060 600a  assifier.py.```.
+00004af0: 0ae6 af8f e4b8 aae6 9687 e4bb b6e5 afb9  ................
+00004b00: e5ba 94e4 b880 e4b8 aae6 a8a1 e59e 8be6  ................
+00004b10: 96b9 e6b3 95ef bc8c e590 84e6 a8a1 e59e  ................
+00004b20: 8be5 ae8c e585 a8e7 8bac e7ab 8bef bc8c  ................
+00004b30: e58f afe4 bba5 e79b b4e6 8ea5 e8bf 90e8  ................
+00004b40: a18c efbc 8ce4 b99f e696 b9e4 bebf e4bf  ................
+00004b50: aee6 94b9 efbc 8ce6 94af e68c 81e9 809a  ................
+00004b60: e8bf 8760 6172 6770 6172 7365 6020 e4bf  ...`argparse` ..
+00004b70: aee6 94b9 602d 2d64 6174 615f 7061 7468  ....`--data_path
+00004b80: 60e7 ad89 e58f 82e6 95b0 e380 820a 0ae7  `...............
+00004b90: 9bb4 e68e a5e5 9ca8 e7bb 88e7 abaf e8b0  ................
+00004ba0: 83e7 94a8 6661 7374 7465 7874 e6a8 a1e5  ....fasttext....
+00004bb0: 9e8b e8ae ade7 bb83 efbc 9a0a 6060 6062  ............```b
+00004bc0: 6173 680a 7079 7468 6f6e 202d 6d20 7079  ash.python -m py
+00004bd0: 7465 7874 636c 6173 7369 6669 6572 2e66  textclassifier.f
+00004be0: 6173 7474 6578 745f 636c 6173 7369 6669  asttext_classifi
+00004bf0: 6572 202d 680a 6060 600a 0a23 2320 5465  er -h.```..## Te
+00004c00: 7874 2043 6c75 7374 6572 0a0a 0a54 6578  xt Cluster...Tex
+00004c10: 7420 636c 7573 7465 7269 6e67 2c20 666f  t clustering, fo
+00004c20: 7220 6578 616d 706c 6520 5b65 7861 6d70  r example [examp
+00004c30: 6c65 732f 636c 7573 7465 725f 6465 6d6f  les/cluster_demo
+00004c40: 2e70 795d 2868 7474 7073 3a2f 2f67 6974  .py](https://git
+00004c50: 6875 622e 636f 6d2f 7368 6962 696e 6736  hub.com/shibing6
+00004c60: 3234 2f70 7974 6578 7463 6c61 7373 6966  24/pytextclassif
+00004c70: 6965 722f 626c 6f62 2f6d 6173 7465 722f  ier/blob/master/
+00004c80: 6578 616d 706c 6573 2f63 6c75 7374 6572  examples/cluster
+00004c90: 5f64 656d 6f2e 7079 290a 0a60 6060 7079  _demo.py)..```py
+00004ca0: 7468 6f6e 0a69 6d70 6f72 7420 7379 730a  thon.import sys.
+00004cb0: 0a73 7973 2e70 6174 682e 6170 7065 6e64  .sys.path.append
+00004cc0: 2827 2e2e 2729 0a66 726f 6d20 7079 7465  ('..').from pyte
+00004cd0: 7874 636c 6173 7369 6669 6572 2e74 6578  xtclassifier.tex
+00004ce0: 7463 6c75 7374 6572 2069 6d70 6f72 7420  tcluster import 
+00004cf0: 5465 7874 436c 7573 7465 720a 0a69 6620  TextCluster..if 
+00004d00: 5f5f 6e61 6d65 5f5f 203d 3d20 275f 5f6d  __name__ == '__m
+00004d10: 6169 6e5f 5f27 3a0a 2020 2020 6d20 3d20  ain__':.    m = 
+00004d20: 5465 7874 436c 7573 7465 7228 6f75 7470  TextCluster(outp
+00004d30: 7574 5f64 6972 3d27 6d6f 6465 6c73 2f63  ut_dir='models/c
+00004d40: 6c75 7374 6572 2d74 6f79 272c 206e 5f63  luster-toy', n_c
+00004d50: 6c75 7374 6572 733d 3229 0a20 2020 2070  lusters=2).    p
+00004d60: 7269 6e74 286d 290a 2020 2020 6461 7461  rint(m).    data
+00004d70: 203d 205b 0a20 2020 2020 2020 2027 5374   = [.        'St
+00004d80: 7564 656e 7420 6465 6274 2074 6f20 636f  udent debt to co
+00004d90: 7374 2042 7269 7461 696e 2062 696c 6c69  st Britain billi
+00004da0: 6f6e 7320 7769 7468 696e 2064 6563 6164  ons within decad
+00004db0: 6573 272c 0a20 2020 2020 2020 2027 4368  es',.        'Ch
+00004dc0: 696e 6573 6520 6564 7563 6174 696f 6e20  inese education 
+00004dd0: 666f 7220 5456 2065 7870 6572 696d 656e  for TV experimen
+00004de0: 7427 2c0a 2020 2020 2020 2020 2741 6262  t',.        'Abb
+00004df0: 6f74 7420 676f 7665 726e 6d65 6e74 2073  ott government s
+00004e00: 7065 6e64 7320 2438 206d 696c 6c69 6f6e  pends $8 million
+00004e10: 206f 6e20 6869 6768 6572 2065 6475 6361   on higher educa
+00004e20: 7469 6f6e 272c 0a20 2020 2020 2020 2027  tion',.        '
+00004e30: 4d69 6464 6c65 2045 6173 7420 616e 6420  Middle East and 
+00004e40: 4173 6961 2062 6f6f 7374 2069 6e76 6573  Asia boost inves
+00004e50: 746d 656e 7420 696e 2074 6f70 206c 6576  tment in top lev
+00004e60: 656c 2073 706f 7274 7327 2c0a 2020 2020  el sports',.    
+00004e70: 2020 2020 2753 756d 6d69 7420 5365 7269      'Summit Seri
+00004e80: 6573 206c 6f6f 6b20 6c61 756e 6368 6573  es look launches
+00004e90: 2048 424f 2043 616e 6164 6120 7370 6f72   HBO Canada spor
+00004ea0: 7473 2064 6f63 2073 6572 6965 733a 204d  ts doc series: M
+00004eb0: 7564 6861 7227 0a20 2020 205d 0a20 2020  udhar'.    ].   
+00004ec0: 206d 2e74 7261 696e 2864 6174 6129 0a20   m.train(data). 
+00004ed0: 2020 206d 2e6c 6f61 645f 6d6f 6465 6c28     m.load_model(
+00004ee0: 290a 2020 2020 7220 3d20 6d2e 7072 6564  ).    r = m.pred
+00004ef0: 6963 7428 5b27 4162 626f 7474 2067 6f76  ict(['Abbott gov
+00004f00: 6572 6e6d 656e 7420 7370 656e 6473 2024  ernment spends $
+00004f10: 3820 6d69 6c6c 696f 6e20 6f6e 2068 6967  8 million on hig
+00004f20: 6865 7220 6564 7563 6174 696f 6e20 6d65  her education me
+00004f30: 6469 6120 626c 6974 7a27 2c0a 2020 2020  dia blitz',.    
+00004f40: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00004f50: 4d69 6464 6c65 2045 6173 7420 616e 6420  Middle East and 
+00004f60: 4173 6961 2062 6f6f 7374 2069 6e76 6573  Asia boost inves
+00004f70: 746d 656e 7420 696e 2074 6f70 206c 6576  tment in top lev
+00004f80: 656c 2073 706f 7274 7327 5d29 0a20 2020  el sports']).   
+00004f90: 2070 7269 6e74 2872 290a 0a20 2020 2023   print(r)..    #
+00004fa0: 2323 2323 2323 2323 2323 206c 6f61 6420  ########## load 
+00004fb0: 6368 696e 6573 6520 7472 6169 6e20 6461  chinese train da
+00004fc0: 7461 2066 726f 6d20 3177 2064 6174 6120  ta from 1w data 
+00004fd0: 6669 6c65 0a20 2020 2066 726f 6d20 736b  file.    from sk
+00004fe0: 6c65 6172 6e2e 6665 6174 7572 655f 6578  learn.feature_ex
+00004ff0: 7472 6163 7469 6f6e 2e74 6578 7420 696d  traction.text im
+00005000: 706f 7274 2054 6669 6466 5665 6374 6f72  port TfidfVector
+00005010: 697a 6572 0a0a 2020 2020 7463 6c75 7374  izer..    tclust
+00005020: 6572 203d 2054 6578 7443 6c75 7374 6572  er = TextCluster
+00005030: 286f 7574 7075 745f 6469 723d 276d 6f64  (output_dir='mod
+00005040: 656c 732f 636c 7573 7465 7227 2c20 6665  els/cluster', fe
+00005050: 6174 7572 653d 5466 6964 6656 6563 746f  ature=TfidfVecto
+00005060: 7269 7a65 7228 6e67 7261 6d5f 7261 6e67  rizer(ngram_rang
+00005070: 653d 2831 2c20 3229 292c 206e 5f63 6c75  e=(1, 2)), n_clu
+00005080: 7374 6572 733d 3130 290a 2020 2020 6461  sters=10).    da
+00005090: 7461 203d 2074 636c 7573 7465 722e 6c6f  ta = tcluster.lo
+000050a0: 6164 5f66 696c 655f 6461 7461 2827 7468  ad_file_data('th
+000050b0: 7563 6e65 7773 5f74 7261 696e 5f31 772e  ucnews_train_1w.
+000050c0: 7478 7427 2c20 7365 703d 275c 7427 2c20  txt', sep='\t', 
+000050d0: 7573 655f 636f 6c3d 3129 0a20 2020 2066  use_col=1).    f
+000050e0: 6561 7475 7265 2c20 6c61 6265 6c73 203d  eature, labels =
+000050f0: 2074 636c 7573 7465 722e 7472 6169 6e28   tcluster.train(
+00005100: 6461 7461 5b3a 3530 3030 5d29 0a20 2020  data[:5000]).   
+00005110: 2074 636c 7573 7465 722e 7368 6f77 5f63   tcluster.show_c
+00005120: 6c75 7374 6572 7328 6665 6174 7572 652c  lusters(feature,
+00005130: 206c 6162 656c 732c 2027 6d6f 6465 6c73   labels, 'models
+00005140: 2f63 6c75 7374 6572 2f63 6c75 7374 6572  /cluster/cluster
+00005150: 5f74 7261 696e 5f73 6567 5f73 616d 706c  _train_seg_sampl
+00005160: 6573 2e70 6e67 2729 0a20 2020 2072 203d  es.png').    r =
+00005170: 2074 636c 7573 7465 722e 7072 6564 6963   tcluster.predic
+00005180: 7428 6461 7461 5b3a 3330 5d29 0a20 2020  t(data[:30]).   
+00005190: 2070 7269 6e74 2872 290a 6060 600a 0a6f   print(r).```..o
+000051a0: 7574 7075 743a 0a0a 6060 600a 5465 7874  utput:..```.Text
+000051b0: 436c 7573 7465 7220 696e 7374 616e 6365  Cluster instance
+000051c0: 2028 4d69 6e69 4261 7463 684b 4d65 616e   (MiniBatchKMean
+000051d0: 7328 6e5f 636c 7573 7465 7273 3d32 2c20  s(n_clusters=2, 
+000051e0: 6e5f 696e 6974 3d31 3029 2c20 3c70 7974  n_init=10), <pyt
+000051f0: 6578 7463 6c61 7373 6966 6965 722e 7574  extclassifier.ut
+00005200: 696c 732e 746f 6b65 6e69 7a65 722e 546f  ils.tokenizer.To
+00005210: 6b65 6e69 7a65 7220 6f62 6a65 6374 2061  kenizer object a
+00005220: 7420 3078 3766 3830 6264 3436 3832 6230  t 0x7f80bd4682b0
+00005230: 3e2c 2054 6669 6466 5665 6374 6f72 697a  >, TfidfVectoriz
+00005240: 6572 286e 6772 616d 5f72 616e 6765 3d28  er(ngram_range=(
+00005250: 312c 2032 2929 290a 5b31 2031 2031 2031  1, 2))).[1 1 1 1
+00005260: 2031 2031 2031 2031 2031 2031 2031 2038   1 1 1 1 1 1 1 8
+00005270: 2031 2031 2031 2031 2031 2031 2031 2031   1 1 1 1 1 1 1 1
+00005280: 2031 2031 2039 2031 2031 2038 2031 2031   1 1 9 1 1 8 1 1
+00005290: 2039 2031 5d0a 6060 600a 636c 7573 7465   9 1].```.cluste
+000052a0: 7269 6e67 2070 6c6f 7420 696d 6167 653a  ring plot image:
+000052b0: 0a0a 215b 636c 7573 7465 725f 696d 6167  ..![cluster_imag
+000052c0: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
+000052d0: 622e 636f 6d2f 7368 6962 696e 6736 3234  b.com/shibing624
+000052e0: 2f70 7974 6578 7463 6c61 7373 6966 6965  /pytextclassifie
+000052f0: 722f 626c 6f62 2f6d 6173 7465 722f 646f  r/blob/master/do
+00005300: 6373 2f63 6c75 7374 6572 5f74 7261 696e  cs/cluster_train
+00005310: 5f73 6567 5f73 616d 706c 6573 2e70 6e67  _seg_samples.png
+00005320: 290a 0a0a 2323 2043 6f6e 7461 6374 0a0a  )...## Contact..
+00005330: 2d20 4973 7375 6528 e5bb bae8 aeae 29ef  - Issue(......).
+00005340: bc9a 5b21 5b47 6974 4875 6220 6973 7375  ..[![GitHub issu
+00005350: 6573 5d28 6874 7470 733a 2f2f 696d 672e  es](https://img.
+00005360: 7368 6965 6c64 732e 696f 2f67 6974 6875  shields.io/githu
+00005370: 622f 6973 7375 6573 2f73 6869 6269 6e67  b/issues/shibing
+00005380: 3632 342f 7079 7465 7874 636c 6173 7369  624/pytextclassi
+00005390: 6669 6572 2e73 7667 295d 2868 7474 7073  fier.svg)](https
+000053a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7368  ://github.com/sh
+000053b0: 6962 696e 6736 3234 2f70 7974 6578 7463  ibing624/pytextc
+000053c0: 6c61 7373 6966 6965 722f 6973 7375 6573  lassifier/issues
+000053d0: 290a 2d20 e982 aee4 bbb6 e688 91ef bc9a  ).- ............
+000053e0: 7875 6d69 6e67 3a20 7875 6d69 6e67 3632  xuming: xuming62
+000053f0: 3440 7171 2e63 6f6d 0a2d 20e5 beae e4bf  4@qq.com.- .....
+00005400: a1e6 8891 efbc 9ae5 8aa0 e688 912a e5be  .............*..
+00005410: aee4 bfa1 e58f b7ef bc9a 7875 6d69 6e67  ..........xuming
+00005420: 3632 342a 2c20 e8bf 9b50 7974 686f 6e2d  624*, ...Python-
+00005430: 4e4c 50e4 baa4 e6b5 81e7 bea4 efbc 8ce5  NLP.............
+00005440: a487 e6b3 a8ef bc9a 2ae5 a793 e590 8d2d  ........*......-
+00005450: e585 ace5 8fb8 e590 8d2d 4e4c 502a 0a3c  .........-NLP*.<
+00005460: 696d 6720 7372 633d 2264 6f63 732f 7765  img src="docs/we
+00005470: 6368 6174 2e6a 7065 6722 2077 6964 7468  chat.jpeg" width
+00005480: 3d22 3230 3022 202f 3e0a 0a0a 2323 2043  ="200" />...## C
+00005490: 6974 6174 696f 6e0a 0ae5 a682 e69e 9ce4  itation.........
+000054a0: bda0 e59c a8e7 a094 e7a9 b6e4 b8ad e4bd  ................
+000054b0: bfe7 94a8 e4ba 8670 7974 6578 7463 6c61  .......pytextcla
+000054c0: 7373 6966 6965 72ef bc8c e8af b7e6 8c89  ssifier.........
+000054d0: e5a6 82e4 b88b e6a0 bce5 bc8f e5bc 95e7  ................
+000054e0: 94a8 efbc 9a0a 0a41 5041 3a0a 6060 606c  .......APA:.```l
+000054f0: 6174 6578 0a58 752c 204d 2e20 5079 7465  atex.Xu, M. Pyte
+00005500: 7874 636c 6173 7369 6669 6572 3a20 5465  xtclassifier: Te
+00005510: 7874 2063 6c61 7373 6966 6965 7220 746f  xt classifier to
+00005520: 6f6c 6b69 7420 666f 7220 4e4c 5020 2856  olkit for NLP (V
+00005530: 6572 7369 6f6e 2031 2e32 2e30 2920 5b43  ersion 1.2.0) [C
+00005540: 6f6d 7075 7465 7220 736f 6674 7761 7265  omputer software
+00005550: 5d2e 2068 7474 7073 3a2f 2f67 6974 6875  ]. https://githu
+00005560: 622e 636f 6d2f 7368 6962 696e 6736 3234  b.com/shibing624
+00005570: 2f70 7974 6578 7463 6c61 7373 6966 6965  /pytextclassifie
+00005580: 720a 6060 600a 0a42 6962 5465 583a 0a60  r.```..BibTeX:.`
+00005590: 6060 6c61 7465 780a 406d 6973 637b 5079  ``latex.@misc{Py
+000055a0: 7465 7874 636c 6173 7369 6669 6572 2c0a  textclassifier,.
+000055b0: 2020 7469 746c 653d 7b50 7974 6578 7463    title={Pytextc
+000055c0: 6c61 7373 6966 6965 723a 2054 6578 7420  lassifier: Text 
+000055d0: 636c 6173 7369 6669 6572 2074 6f6f 6c6b  classifier toolk
+000055e0: 6974 2066 6f72 204e 4c50 7d2c 0a20 2061  it for NLP},.  a
+000055f0: 7574 686f 723d 7b58 7520 4d69 6e67 7d2c  uthor={Xu Ming},
+00005600: 0a20 2079 6561 723d 7b32 3032 327d 2c0a  .  year={2022},.
+00005610: 2020 686f 7770 7562 6c69 7368 6564 3d7b    howpublished={
+00005620: 5c75 726c 7b68 7474 7073 3a2f 2f67 6974  \url{https://git
+00005630: 6875 622e 636f 6d2f 7368 6962 696e 6736  hub.com/shibing6
+00005640: 3234 2f70 7974 6578 7463 6c61 7373 6966  24/pytextclassif
+00005650: 6965 727d 7d2c 0a7d 0a60 6060 0a0a 0a23  ier}},.}.```...#
+00005660: 2320 4c69 6365 6e73 650a 0a0a e68e 88e6  # License.......
+00005670: 9d83 e58d 8fe8 aeae e4b8 ba20 5b54 6865  ........... [The
+00005680: 2041 7061 6368 6520 4c69 6365 6e73 6520   Apache License 
+00005690: 322e 305d 284c 4943 454e 5345 29ef bc8c  2.0](LICENSE)...
+000056a0: e58f afe5 858d e8b4 b9e7 94a8 e581 9ae5  ................
+000056b0: 9586 e4b8 9ae7 94a8 e980 94e3 8082 e8af  ................
+000056c0: b7e5 9ca8 e4ba a7e5 9381 e8af b4e6 988e  ................
+000056d0: e4b8 ade9 9984 e58a a02a 2a70 7974 6578  .........**pytex
+000056e0: 7463 6c61 7373 6966 6965 722a 2ae7 9a84  tclassifier**...
+000056f0: e993 bee6 8ea5 e592 8ce6 8e88 e69d 83e5  ................
+00005700: 8d8f e8ae aee3 8082 0a0a 0a23 2320 436f  ...........## Co
+00005710: 6e74 7269 6275 7465 0ae9 a1b9 e79b aee4  ntribute........
+00005720: bba3 e7a0 81e8 bf98 e5be 88e7 b297 e7b3  ................
+00005730: 99ef bc8c e5a6 82e6 9e9c e5a4 a7e5 aeb6  ................
+00005740: e5af b9e4 bba3 e7a0 81e6 9c89 e689 80e6  ................
+00005750: 94b9 e8bf 9bef bc8c e6ac a2e8 bf8e e68f  ................
+00005760: 90e4 baa4 e59b 9ee6 9cac e9a1 b9e7 9bae  ................
+00005770: efbc 8ce5 9ca8 e68f 90e4 baa4 e4b9 8be5  ................
+00005780: 898d efbc 8ce6 b3a8 e684 8fe4 bba5 e4b8  ................
+00005790: 8be4 b8a4 e782 b9ef bc9a 0a0a 202d 20e5  ............ - .
+000057a0: 9ca8 6074 6573 7473 60e6 b7bb e58a a0e7  ..`tests`.......
+000057b0: 9bb8 e5ba 94e7 9a84 e58d 95e5 8583 e6b5  ................
+000057c0: 8be8 af95 0a20 2d20 e4bd bfe7 94a8 6070  ..... - ......`p
+000057d0: 7974 686f 6e20 7365 7475 702e 7079 2074  ython setup.py t
+000057e0: 6573 7460 e69d a5e8 bf90 e8a1 8ce6 8980  est`............
+000057f0: e69c 89e5 8d95 e585 83e6 b58b e8af 95ef  ................
+00005800: bc8c e7a1 aee4 bf9d e689 80e6 9c89 e58d  ................
+00005810: 95e6 b58b e983 bde6 98af e980 9ae8 bf87  ................
+00005820: e79a 840a 0ae4 b98b e590 8ee5 8db3 e58f  ................
+00005830: afe6 8f90 e4ba a450 52e3 8082 0a0a       .......PR.....
```

### Comparing `pytextclassifier-1.3.7/pytextclassifier.egg-info/SOURCES.txt` & `pytextclassifier-1.3.8/pytextclassifier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytextclassifier-1.3.7/setup.py` & `pytextclassifier-1.3.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 @author:XuMing(xuming624@qq.com)
 @description: 
 """
 from setuptools import setup, find_packages
 
-__version__ = '1.3.7'
+__version__ = '1.3.8'
 
 with open('README.md', 'r', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name='pytextclassifier',
     version=__version__,
```

