# Comparing `tmp/django-easy-faq-1.7.tar.gz` & `tmp/django_easy_faq-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-easy-faq-1.7.tar", last modified: Sun Dec 24 19:02:26 2023, max compression
+gzip compressed data, was "django_easy_faq-1.8.tar", last modified: Thu May  9 01:25:33 2024, max compression
```

## Comparing `django-easy-faq-1.7.tar` & `django_easy_faq-1.8.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-12-24 19:02:26.402460 django-easy-faq-1.7/
--rw-rw-rw-   0        0        0     1083 2023-12-24 18:38:09.000000 django-easy-faq-1.7/LICENSE.txt
--rw-rw-rw-   0        0        0      108 2023-02-14 02:47:58.000000 django-easy-faq-1.7/MANIFEST.in
--rw-rw-rw-   0        0        0    15354 2023-12-24 19:02:26.401023 django-easy-faq-1.7/PKG-INFO
--rw-rw-rw-   0        0        0    14340 2023-12-24 18:36:12.000000 django-easy-faq-1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-12-24 19:02:26.400027 django-easy-faq-1.7/django_easy_faq.egg-info/
--rw-rw-rw-   0        0        0    15354 2023-12-24 19:02:26.000000 django-easy-faq-1.7/django_easy_faq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1080 2023-12-24 19:02:26.000000 django-easy-faq-1.7/django_easy_faq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-24 19:02:26.000000 django-easy-faq-1.7/django_easy_faq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-12-24 19:02:26.000000 django-easy-faq-1.7/django_easy_faq.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-12-24 19:02:26.000000 django-easy-faq-1.7/django_easy_faq.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-12-24 19:02:26.375018 django-easy-faq-1.7/faq/
--rw-rw-rw-   0        0        0       41 2023-02-14 02:47:58.000000 django-easy-faq-1.7/faq/__init__.py
--rw-rw-rw-   0        0        0     2429 2023-05-05 20:03:31.000000 django-easy-faq-1.7/faq/admin.py
--rw-rw-rw-   0        0        0      170 2023-02-14 02:47:58.000000 django-easy-faq-1.7/faq/apps.py
--rw-rw-rw-   0        0        0      270 2023-05-05 19:44:23.000000 django-easy-faq-1.7/faq/forms.py
-drwxrwxrwx   0        0        0        0 2023-12-24 19:02:26.382020 django-easy-faq-1.7/faq/migrations/
--rw-rw-rw-   0        0        0     4220 2023-02-14 02:47:58.000000 django-easy-faq-1.7/faq/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     1543 2023-02-14 02:47:58.000000 django-easy-faq-1.7/faq/migrations/0002_alter_answer_id_alter_answerhelpful_id_and_more.py
--rw-rw-rw-   0        0        0      455 2023-02-14 02:47:58.000000 django-easy-faq-1.7/faq/migrations/0003_auto_20220619_0939.py
--rw-rw-rw-   0        0        0      576 2023-02-14 02:47:58.000000 django-easy-faq-1.7/faq/migrations/0004_alter_answer_slug_alter_category_slug.py
--rw-rw-rw-   0        0        0      409 2023-05-05 20:01:24.000000 django-easy-faq-1.7/faq/migrations/0005_rename_description_category__description.py
--rw-rw-rw-   0        0        0        0 2023-02-14 02:47:58.000000 django-easy-faq-1.7/faq/migrations/__init__.py
--rw-rw-rw-   0        0        0     4957 2023-12-24 18:34:45.000000 django-easy-faq-1.7/faq/models.py
--rw-rw-rw-   0        0        0      346 2023-02-14 02:47:58.000000 django-easy-faq-1.7/faq/path_converters.py
--rw-rw-rw-   0        0        0     2476 2023-02-14 02:47:58.000000 django-easy-faq-1.7/faq/snippets.py
-drwxrwxrwx   0        0        0        0 2023-12-24 19:02:26.324695 django-easy-faq-1.7/faq/templates/
-drwxrwxrwx   0        0        0        0 2023-12-24 19:02:26.397028 django-easy-faq-1.7/faq/templates/faq/
--rw-rw-rw-   0        0        0      342 2023-02-14 02:47:58.000000 django-easy-faq-1.7/faq/templates/faq/answer_form.html
--rw-rw-rw-   0        0        0      242 2023-02-14 02:47:58.000000 django-easy-faq-1.7/faq/templates/faq/base.html
--rw-rw-rw-   0        0        0      421 2023-02-14 02:47:58.000000 django-easy-faq-1.7/faq/templates/faq/categories_list.html
--rw-rw-rw-   0        0        0      633 2023-02-14 02:47:58.000000 django-easy-faq-1.7/faq/templates/faq/category_detail.html
--rw-rw-rw-   0        0        0      281 2023-02-14 02:47:58.000000 django-easy-faq-1.7/faq/templates/faq/comment_form.html
--rw-rw-rw-   0        0        0      758 2023-02-14 02:47:58.000000 django-easy-faq-1.7/faq/templates/faq/comments.html
--rw-rw-rw-   0        0        0     1264 2023-02-14 02:47:58.000000 django-easy-faq-1.7/faq/templates/faq/question_base.html
--rw-rw-rw-   0        0        0     2877 2023-02-14 02:47:58.000000 django-easy-faq-1.7/faq/templates/faq/question_detail.html
--rw-rw-rw-   0        0        0      264 2023-02-14 02:47:58.000000 django-easy-faq-1.7/faq/templates/faq/question_form.html
--rw-rw-rw-   0        0        0      434 2023-02-14 02:47:58.000000 django-easy-faq-1.7/faq/templates/faq/questions_list.html
--rw-rw-rw-   0        0        0      262 2023-02-14 02:47:58.000000 django-easy-faq-1.7/faq/templates/faq/vote_form.html
--rw-rw-rw-   0        0        0     7715 2023-12-24 18:56:46.000000 django-easy-faq-1.7/faq/tests.py
--rw-rw-rw-   0        0        0     2964 2023-02-14 03:22:49.000000 django-easy-faq-1.7/faq/urls.py
--rw-rw-rw-   0        0        0    13091 2023-05-05 22:13:32.000000 django-easy-faq-1.7/faq/views.py
--rw-rw-rw-   0        0        0      993 2023-12-24 19:02:26.408984 django-easy-faq-1.7/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-02-14 02:47:58.000000 django-easy-faq-1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:25:33.007723 django_easy_faq-1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-09 01:25:29.000000 django_easy_faq-1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-09 01:25:29.000000 django_easy_faq-1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16054 2024-05-09 01:25:33.007723 django_easy_faq-1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15246 2024-05-09 01:25:29.000000 django_easy_faq-1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:25:33.003723 django_easy_faq-1.8/django_easy_faq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16054 2024-05-09 01:25:32.000000 django_easy_faq-1.8/django_easy_faq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-09 01:25:32.000000 django_easy_faq-1.8/django_easy_faq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 01:25:32.000000 django_easy_faq-1.8/django_easy_faq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-09 01:25:32.000000 django_easy_faq-1.8/django_easy_faq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-09 01:25:32.000000 django_easy_faq-1.8/django_easy_faq.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:25:33.003723 django_easy_faq-1.8/faq/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:25:33.003723 django_easy_faq-1.8/faq/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/migrations/0002_alter_answer_id_alter_answerhelpful_id_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/migrations/0003_auto_20220619_0939.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/migrations/0004_alter_answer_slug_alter_category_slug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/migrations/0005_rename_description_category__description.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/migrations/0006_answer_is_rich_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/path_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/snippets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:25:32.999723 django_easy_faq-1.8/faq/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:25:33.003723 django_easy_faq-1.8/faq/templates/faq/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/templates/faq/answer_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/templates/faq/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/templates/faq/categories_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/templates/faq/category_detail.html
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/templates/faq/comment_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/templates/faq/comments.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/templates/faq/question_base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/templates/faq/question_detail.html
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/templates/faq/question_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/templates/faq/questions_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/templates/faq/vote_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12843 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 01:25:33.007723 django_easy_faq-1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-09 01:25:29.000000 django_easy_faq-1.8/setup.py
```

### Comparing `django-easy-faq-1.7/LICENSE.txt` & `django_easy_faq-1.8/LICENSE`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 smark-1
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2024 smark-1
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `django-easy-faq-1.7/PKG-INFO` & `django_easy_faq-1.8/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,960 +1,953 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310d 0a4e 616d 653a 2064 6a61  : 2.1..Name: dja
-00000020: 6e67 6f2d 6561 7379 2d66 6171 0d0a 5665  ngo-easy-faq..Ve
-00000030: 7273 696f 6e3a 2031 2e37 0d0a 5375 6d6d  rsion: 1.7..Summ
-00000040: 6172 793a 2041 2044 6a61 6e67 6f20 6170  ary: A Django ap
-00000050: 7020 746f 2061 6464 2067 7265 6174 2066  p to add great f
-00000060: 6171 2066 756e 6374 696f 6e61 6c69 7479  aq functionality
-00000070: 2074 6f20 7765 6273 6974 652e 0d0a 486f   to website...Ho
-00000080: 6d65 2d70 6167 653a 2068 7474 7073 3a2f  me-page: https:/
-00000090: 2f67 6974 6875 622e 636f 6d2f 6472 6167  /github.com/drag
-000000a0: 6f6e 636f 6d6d 6974 732f 646a 616e 676f  oncommits/django
-000000b0: 2d65 6173 792d 6661 710d 0a4c 6963 656e  -easy-faq..Licen
-000000c0: 7365 3a20 4253 442d 332d 436c 6175 7365  se: BSD-3-Clause
-000000d0: 0d0a 436c 6173 7369 6669 6572 3a20 456e  ..Classifier: En
-000000e0: 7669 726f 6e6d 656e 7420 3a3a 2057 6562  vironment :: Web
-000000f0: 2045 6e76 6972 6f6e 6d65 6e74 0d0a 436c   Environment..Cl
-00000100: 6173 7369 6669 6572 3a20 4672 616d 6577  assifier: Framew
-00000110: 6f72 6b20 3a3a 2044 6a61 6e67 6f0d 0a43  ork :: Django..C
-00000120: 6c61 7373 6966 6965 723a 2049 6e74 656e  lassifier: Inten
-00000130: 6465 6420 4175 6469 656e 6365 203a 3a20  ded Audience :: 
-00000140: 4465 7665 6c6f 7065 7273 0d0a 436c 6173  Developers..Clas
-00000150: 7369 6669 6572 3a20 4c69 6365 6e73 6520  sifier: License 
-00000160: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
-00000170: 3a3a 2042 5344 204c 6963 656e 7365 0d0a  :: BSD License..
-00000180: 436c 6173 7369 6669 6572 3a20 4f70 6572  Classifier: Oper
-00000190: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
-000001a0: 4f53 2049 6e64 6570 656e 6465 6e74 0d0a  OS Independent..
-000001b0: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
-000001c0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-000001d0: 203a 3a20 5079 7468 6f6e 0d0a 436c 6173   :: Python..Clas
-000001e0: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-000001f0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000200: 5079 7468 6f6e 203a 3a20 332e 370d 0a43  Python :: 3.7..C
-00000210: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-00000220: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000230: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e38  :: Python :: 3.8
-00000240: 0d0a 436c 6173 7369 6669 6572 3a20 5072  ..Classifier: Pr
-00000250: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000260: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000270: 332e 390d 0a43 6c61 7373 6966 6965 723a  3.9..Classifier:
-00000280: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-00000290: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-000002a0: 3a3a 2033 2e31 300d 0a43 6c61 7373 6966  :: 3.10..Classif
-000002b0: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-000002c0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-000002d0: 686f 6e20 3a3a 2033 2e31 310d 0a43 6c61  hon :: 3.11..Cla
-000002e0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-000002f0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000300: 2050 7974 686f 6e20 3a3a 2033 2e31 320d   Python :: 3.12.
-00000310: 0a43 6c61 7373 6966 6965 723a 2054 6f70  .Classifier: Top
-00000320: 6963 203a 3a20 496e 7465 726e 6574 203a  ic :: Internet :
-00000330: 3a20 5757 572f 4854 5450 0d0a 436c 6173  : WWW/HTTP..Clas
-00000340: 7369 6669 6572 3a20 546f 7069 6320 3a3a  sifier: Topic ::
-00000350: 2049 6e74 6572 6e65 7420 3a3a 2057 5757   Internet :: WWW
-00000360: 2f48 5454 5020 3a3a 2044 796e 616d 6963  /HTTP :: Dynamic
-00000370: 2043 6f6e 7465 6e74 0d0a 5265 7175 6972   Content..Requir
-00000380: 6573 2d50 7974 686f 6e3a 203e 3d33 2e37  es-Python: >=3.7
-00000390: 0d0a 4465 7363 7269 7074 696f 6e2d 436f  ..Description-Co
-000003a0: 6e74 656e 742d 5479 7065 3a20 7465 7874  ntent-Type: text
-000003b0: 2f6d 6172 6b64 6f77 6e0d 0a4c 6963 656e  /markdown..Licen
-000003c0: 7365 2d46 696c 653a 204c 4943 454e 5345  se-File: LICENSE
-000003d0: 2e74 7874 0d0a 5265 7175 6972 6573 2d44  .txt..Requires-D
-000003e0: 6973 743a 2044 6a61 6e67 6f3e 3d33 2e32  ist: Django>=3.2
-000003f0: 0d0a 0d0a 2320 646a 616e 676f 2d65 6173  ....# django-eas
-00000400: 792d 6661 710d 0a0d 0a64 6a61 6e67 6f2d  y-faq....django-
-00000410: 6561 7379 2d66 6171 2069 7320 6120 446a  easy-faq is a Dj
-00000420: 616e 676f 2061 7070 2074 6f20 616c 6c6f  ango app to allo
-00000430: 7720 666f 7220 6120 7369 6d70 6c65 2079  w for a simple y
-00000440: 6574 2066 6561 7475 7265 2072 6963 6820  et feature rich 
-00000450: 6661 7120 6170 702e 2077 6974 6820 6361  faq app. with ca
-00000460: 7465 676f 7269 6573 2c20 636f 6d6d 656e  tegories, commen
-00000470: 7469 6e67 2076 6f74 696e 6720 6f66 2071  ting voting of q
-00000480: 7565 7374 696f 6e73 2061 6e64 2061 6e73  uestions and ans
-00000490: 7765 7273 2061 6c6c 2061 7320 616e 206f  wers all as an o
-000004a0: 7074 696f 6e61 6c20 7061 7274 206f 6620  ptional part of 
-000004b0: 7468 6520 6170 702e 2054 6f20 7365 6520  the app. To see 
-000004c0: 7363 7265 656e 7368 6f74 7320 6f66 2077  screenshots of w
-000004d0: 6861 7420 7468 6973 2064 6a61 6e67 6f2d  hat this django-
-000004e0: 6561 7379 2d66 6171 2063 6f75 6c64 206c  easy-faq could l
-000004f0: 6f6f 6b20 6c69 6b65 2077 6974 6820 626f  ook like with bo
-00000500: 6f74 7374 7261 7020 3520 7374 796c 696e  otstrap 5 stylin
-00000510: 6720 5b63 6c69 636b 2068 6572 655d 2864  g [click here](d
-00000520: 656d 6f2f 6465 6d6f 2e6d 6429 2e0d 0a0d  emo/demo.md)....
-00000530: 0a0d 0a23 2320 5175 6963 6b20 7374 6172  ...## Quick star
-00000540: 740d 0a0d 0a31 2e20 7069 7020 696e 7374  t....1. pip inst
-00000550: 616c 6c3a 0d0a 0d0a 2020 2020 6070 6970  all:....    `pip
-00000560: 2069 6e73 7461 6c6c 2064 6a61 6e67 6f2d   install django-
-00000570: 6561 7379 2d66 6171 600d 0a0d 0a32 2e20  easy-faq`....2. 
-00000580: 4164 6420 2266 6171 2220 746f 2079 6f75  Add "faq" to you
-00000590: 7220 494e 5354 414c 4c45 445f 4150 5053  r INSTALLED_APPS
-000005a0: 2073 6574 7469 6e67 206c 696b 6520 7468   setting like th
-000005b0: 6973 3a0d 0a0d 0a20 2020 2060 6060 7079  is:....    ```py
-000005c0: 7468 6f6e 0d0a 2020 2020 494e 5354 414c  thon..    INSTAL
-000005d0: 4c45 445f 4150 5053 203d 205b 0d0a 2020  LED_APPS = [..  
-000005e0: 2020 2020 2020 2e2e 2e0d 0a20 2020 2020        .....     
-000005f0: 2020 2027 6661 7127 2c5d 0d0a 2020 2020     'faq',]..    
-00000600: 6060 600d 0a0d 0a33 2e20 496e 636c 7564  ```....3. Includ
-00000610: 6520 7468 6520 6561 7379 2d66 6171 2055  e the easy-faq U
-00000620: 524c 636f 6e66 2069 6e20 796f 7572 2070  RLconf in your p
-00000630: 726f 6a65 6374 2075 726c 732e 7079 206c  roject urls.py l
-00000640: 696b 6520 7468 6973 3a3a 0d0a 0d0a 2020  ike this::....  
-00000650: 2020 6060 6070 7974 686f 6e0d 0a20 2020    ```python..   
-00000660: 2023 e280 a60d 0a20 2020 2070 6174 6828   #.....    path(
-00000670: 2766 6171 2f27 2c20 696e 636c 7564 6528  'faq/', include(
-00000680: 2766 6171 2e75 726c 7327 2929 2c0d 0a20  'faq.urls')),.. 
-00000690: 2020 2023 e280 a60d 0a20 2020 2060 6060     #.....    ```
-000006a0: 0d0a 0d0a 342e 2041 6464 2060 4641 515f  ....4. Add `FAQ_
-000006b0: 5345 5454 494e 4753 203d 205b 5d60 2074  SETTINGS = []` t
-000006c0: 6f20 796f 7572 2060 7365 7474 696e 6773  o your `settings
-000006d0: 2e70 7960 0d0a 352e 2052 756e 2060 6070  .py`..5. Run ``p
-000006e0: 7974 686f 6e20 6d61 6e61 6765 2e70 7920  ython manage.py 
-000006f0: 6d61 6b65 6d69 6772 6174 696f 6e73 6060  makemigrations``
-00000700: 2074 6f20 6372 6561 7465 2074 6865 2066   to create the f
-00000710: 6171 206d 6f64 656c 7320 6d69 6772 6174  aq models migrat
-00000720: 696f 6e73 2e0d 0a36 2e20 5275 6e20 6060  ions...6. Run ``
-00000730: 7079 7468 6f6e 206d 616e 6167 652e 7079  python manage.py
-00000740: 206d 6967 7261 7465 6060 2074 6f20 6372   migrate`` to cr
-00000750: 6561 7465 2074 6865 2066 6171 206d 6f64  eate the faq mod
-00000760: 656c 732e 0d0a 0d0a 372e 2053 7461 7274  els.....7. Start
-00000770: 2074 6865 2064 6576 656c 6f70 6d65 6e74   the development
-00000780: 2073 6572 7665 7220 616e 6420 7669 7369   server and visi
-00000790: 7420 6874 7470 3a2f 2f31 3237 2e30 2e30  t http://127.0.0
-000007a0: 2e31 3a38 3030 302f 6164 6d69 6e2f 0d0a  .1:8000/admin/..
-000007b0: 2020 2074 6f20 6372 6561 7465 2061 2063     to create a c
-000007c0: 6174 6567 6f72 7920 2879 6f75 276c 6c20  ategory (you'll 
-000007d0: 6e65 6564 2074 6865 2041 646d 696e 2061  need the Admin a
-000007e0: 7070 2065 6e61 626c 6564 292e 2863 6174  pp enabled).(cat
-000007f0: 6567 6f72 6965 7320 7061 7274 206f 6620  egories part of 
-00000800: 7468 6520 6170 7020 6361 6e20 6265 2064  the app can be d
-00000810: 6973 6162 6c65 6429 0d0a 0d0a 382e 2056  isabled)....8. V
-00000820: 6973 6974 2068 7474 703a 2f2f 3132 372e  isit http://127.
-00000830: 302e 302e 313a 3830 3030 2f66 6171 2f20  0.0.1:8000/faq/ 
-00000840: 746f 2073 6565 2074 6865 2063 6174 6567  to see the categ
-00000850: 6f72 6965 732e 0d0a 0d0a 2323 2053 6574  ories.....## Set
-00000860: 7469 6e67 730d 0a0d 0a79 6f75 2063 616e  tings....you can
-00000870: 2063 6861 6e67 6520 6d6f 7374 2074 6869   change most thi
-00000880: 6e67 7320 696e 2073 6574 7469 6e67 7320  ngs in settings 
-00000890: 6265 6c6f 7720 6973 2061 206c 6973 7420  below is a list 
-000008a0: 6f66 2061 6c6c 2073 6574 7469 6e67 730d  of all settings.
-000008b0: 0a61 6464 2061 6e79 206f 7220 616c 6c20  .add any or all 
-000008c0: 746f 2063 6861 6e67 6520 746f 2064 6573  to change to des
-000008d0: 6972 6564 2062 6568 6176 696f 723a 3a0d  ired behavior::.
-000008e0: 0a0d 0a0d 0a20 2020 2046 4151 5f53 4554  .....    FAQ_SET
-000008f0: 5449 4e47 5320 3d20 5b27 796f 7572 5f73  TINGS = ['your_s
-00000900: 6574 7469 6e67 735f 6865 7265 272c 5d0d  ettings_here',].
-00000910: 0a0d 0a0d 0a31 2e20 6e6f 5f63 6174 6567  .....1. no_categ
-00000920: 6f72 795f 6465 7363 7269 7074 696f 6e20  ory_description 
-00000930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000940: 202d 2061 6464 2069 6620 7573 696e 6720   - add if using 
-00000950: 6361 7465 676f 7269 6573 2062 7574 2064  categories but d
-00000960: 6f6e 2774 2077 616e 7420 6465 7363 7269  on't want descri
-00000970: 7074 696f 6e73 2066 6f72 2074 6865 6d0d  ptions for them.
-00000980: 0a32 2e20 6e6f 5f63 6174 6567 6f72 7920  .2. no_category 
-00000990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009a0: 2020 2020 2020 2020 2020 2020 202d 2061               - a
-000009b0: 6464 2069 6620 646f 6e27 7420 7761 6e74  dd if don't want
-000009c0: 2074 6f20 7573 6520 6361 7465 676f 7269   to use categori
-000009d0: 6573 0d0a 332e 206c 6f67 6765 645f 696e  es..3. logged_in
-000009e0: 5f75 7365 7273 5f63 616e 5f61 6464 5f71  _users_can_add_q
-000009f0: 7565 7374 696f 6e20 2020 2020 2020 2020  uestion         
-00000a00: 2d20 6164 6420 6966 2079 6f75 2077 616e  - add if you wan
-00000a10: 7420 616e 7920 6c6f 6767 6564 2069 6e20  t any logged in 
-00000a20: 7573 6572 2074 6f20 6265 2061 626c 6520  user to be able 
-00000a30: 746f 2061 736b 2061 2071 7565 7374 696f  to ask a questio
-00000a40: 6e0d 0a34 2e20 6c6f 6767 6564 5f69 6e5f  n..4. logged_in_
-00000a50: 7573 6572 735f 6361 6e5f 616e 7377 6572  users_can_answer
-00000a60: 5f71 7565 7374 696f 6e20 2020 2020 202d  _question      -
-00000a70: 2061 6464 2069 6620 796f 7520 7761 6e74   add if you want
-00000a80: 2061 6e79 206c 6f67 6765 6420 696e 2075   any logged in u
-00000a90: 7365 7220 746f 2062 6520 6162 6c65 2074  ser to be able t
-00000aa0: 6f20 616e 7377 6572 2061 2071 7565 7374  o answer a quest
-00000ab0: 696f 6e0d 0a35 2e20 616c 6c6f 775f 6d75  ion..5. allow_mu
-00000ac0: 6c74 6970 6c65 5f61 6e73 7765 7273 2020  ltiple_answers  
-00000ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ae0: 202d 2061 6464 2069 6620 796f 7520 7761   - add if you wa
-00000af0: 6e74 2061 2071 7565 7374 696f 6e20 746f  nt a question to
-00000b00: 2062 6520 6162 6c65 2074 6f20 6265 2061   be able to be a
-00000b10: 6e73 7765 7265 6420 6d75 6c74 6970 6c65  nswered multiple
-00000b20: 2074 696d 6573 0d0a 362e 206e 6f5f 636f   times..6. no_co
-00000b30: 6d6d 656e 7473 2020 2020 2020 2020 2020  mments          
-00000b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b50: 2020 2020 2d20 6164 6420 6966 2064 6f6e      - add if don
-00000b60: 2774 2077 616e 7420 746f 2075 7365 2063  't want to use c
-00000b70: 6f6d 6d65 6e74 730d 0a37 2e20 616e 6f6e  omments..7. anon
-00000b80: 796d 6f75 735f 7573 6572 5f63 616e 5f63  ymous_user_can_c
-00000b90: 6f6d 6d65 6e74 2020 2020 2020 2020 2020  omment          
-00000ba0: 2020 2020 202d 2061 6464 2069 6620 796f       - add if yo
-00000bb0: 7520 7761 6e74 2061 6e79 2075 7365 7220  u want any user 
-00000bc0: 746f 2062 6520 6162 6c65 2074 6f20 636f  to be able to co
-00000bd0: 6d6d 656e 7420 696e 636c 7564 696e 6720  mment including 
-00000be0: 616e 6f6e 796d 6f75 7320 7573 6572 730d  anonymous users.
-00000bf0: 0a38 2e20 7669 6577 5f6f 6e6c 795f 636f  .8. view_only_co
-00000c00: 6d6d 656e 7473 2020 2020 2020 2020 2020  mments          
-00000c10: 2020 2020 2020 2020 2020 2020 202d 2061               - a
-00000c20: 6464 2069 6620 796f 7520 7761 6e74 2075  dd if you want u
-00000c30: 7365 7273 2074 6f20 7365 6520 706f 7374  sers to see post
-00000c40: 6564 2063 6f6d 6d65 6e74 7320 6275 7420  ed comments but 
-00000c50: 6e6f 7420 6265 2061 626c 6520 746f 2061  not be able to a
-00000c60: 6464 2061 6e79 206d 6f72 650d 0a39 2e20  dd any more..9. 
-00000c70: 6e6f 5f76 6f74 6573 2020 2020 2020 2020  no_votes        
-00000c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c90: 2020 2020 2020 2020 202d 2061 6464 2069           - add i
-00000ca0: 6620 646f 6e27 7420 7761 6e74 2061 6e79  f don't want any
-00000cb0: 2076 6f74 696e 6720 666f 7220 7573 6566   voting for usef
-00000cc0: 756c 2071 7565 7374 696f 6e73 206f 7220  ul questions or 
-00000cd0: 616e 7377 6572 730d 0a31 302e 206e 6f5f  answers..10. no_
-00000ce0: 616e 7377 6572 5f76 6f74 6573 2020 2020  answer_votes    
-00000cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d00: 2020 2020 202d 2061 6464 2069 6620 6f6e       - add if on
-00000d10: 6c79 2077 616e 7420 7175 6573 7469 6f6e  ly want question
-00000d20: 2076 6f74 696e 670d 0a31 312e 206e 6f5f   voting..11. no_
-00000d30: 7175 6573 7469 6f6e 5f76 6f74 6573 2020  question_votes  
-00000d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d50: 2020 2020 202d 2061 6464 2069 6620 6f6e       - add if on
-00000d60: 6c79 2077 616e 7420 616e 7377 6572 2076  ly want answer v
-00000d70: 6f74 696e 670d 0a31 322e 2061 6c6c 6f77  oting..12. allow
-00000d80: 5f75 6e69 636f 6465 2020 2020 2020 2020  _unicode        
-00000d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000da0: 2020 202d 2061 6464 2069 6620 796f 7520     - add if you 
-00000db0: 7761 6e74 2074 6f20 616c 6c6f 7720 756e  want to allow un
-00000dc0: 6963 6f64 6520 736c 7567 730d 0a31 332e  icode slugs..13.
-00000dd0: 206c 6f67 696e 5f72 6571 7569 7265 6420   login_required 
-00000de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000df0: 2020 2020 2020 2020 202d 2061 6464 2069           - add i
-00000e00: 6620 796f 7520 7761 6e74 2074 6f20 6f6e  f you want to on
-00000e10: 6c79 206c 6574 206c 6f67 6765 6420 696e  ly let logged in
-00000e20: 2075 7365 7273 2073 6565 2046 4151 2773   users see FAQ's
-00000e30: 0d0a 0d0a 2323 2054 656d 706c 6174 6573  ....## Templates
-00000e40: 0d0a 0d0a 616c 6c20 6f66 2074 6865 2074  ....all of the t
-00000e50: 656d 706c 6174 6573 2061 7265 206d 6561  emplates are mea
-00000e60: 6e74 2074 6f20 6265 206f 7665 7277 7269  nt to be overwri
-00000e70: 7474 656e 0d0a 746f 206f 7665 7277 7269  tten..to overwri
-00000e80: 7465 2074 6865 6d20 6372 6561 7465 2061  te them create a
-00000e90: 2066 6171 2064 6972 6563 746f 7279 2069   faq directory i
-00000ea0: 6e73 6964 6520 6f66 2074 6865 2074 656d  nside of the tem
-00000eb0: 706c 6174 6573 2064 6972 6563 746f 7279  plates directory
-00000ec0: 2061 6e64 2061 6464 2061 2068 746d 6c20   and add a html 
-00000ed0: 6669 6c65 2077 6974 6820 7468 6520 7361  file with the sa
-00000ee0: 6d65 206e 616d 6520 746f 2069 740d 0a0d  me name to it...
-00000ef0: 0a69 6620 7468 6973 2064 6f65 736e 2774  .if this doesn't
-00000f00: 2077 6f72 6b20 6d61 6b65 2073 7572 6520   work make sure 
-00000f10: 7468 6174 2074 6865 2074 656d 706c 6174  that the templat
-00000f20: 6573 2073 6574 7469 6e67 2068 6173 2027  es setting has '
-00000f30: 4449 5253 273a 205b 2774 656d 706c 6174  DIRS': ['templat
-00000f40: 6573 275d 2c20 696e 2069 743a 3a0d 0a0d  es'], in it::...
-00000f50: 0a20 2020 2054 454d 504c 4154 4553 203d  .    TEMPLATES =
-00000f60: 205b 0d0a 2020 2020 2020 2020 7b0d 0a20   [..        {.. 
-00000f70: 2020 2020 2020 2020 2020 202e 2e2e 0d0a             .....
-00000f80: 2020 2020 2020 2020 2020 2020 2744 4952              'DIR
-00000f90: 5327 3a20 5b27 7465 6d70 6c61 7465 7327  S': ['templates'
-00000fa0: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
-00000fb0: 2e2e 2e0d 0a20 2020 2020 2020 207d 2c0d  .....        },.
-00000fc0: 0a20 2020 205d 0d0a 0d0a 6865 7265 2069  .    ]....here i
-00000fd0: 7320 6120 6c69 7374 206f 6620 7465 6d70  s a list of temp
-00000fe0: 6c61 7465 7320 616e 6420 7468 6572 6520  lates and there 
-00000ff0: 6465 6661 756c 7420 7465 6d70 6c61 7465  default template
-00001000: 2020 796f 7520 6361 6e20 6f76 6572 7772    you can overwr
-00001010: 6974 650d 0a0d 0a31 2e20 6361 7465 676f  ite....1. catego
-00001020: 7269 6573 5f6c 6973 742e 6874 6d6c 202d  ries_list.html -
-00001030: 2066 6171 206d 6169 6e20 7669 6577 2069   faq main view i
-00001040: 6620 7573 696e 6720 6361 7465 676f 7269  f using categori
-00001050: 6573 3a3a 0d0a 0d0a 0d0a 2020 2020 2020  es::......      
-00001060: 2020 3c68 313e 7365 6c65 6374 2061 2046    <h1>select a F
-00001070: 4151 2063 6174 6567 6f72 793c 2f68 313e  AQ category</h1>
-00001080: 0d0a 2020 2020 2020 2020 7b25 2066 6f72  ..        {% for
-00001090: 2063 6174 6567 6f72 7920 696e 2063 6174   category in cat
-000010a0: 6567 6f72 6965 7320 257d 0d0a 2020 2020  egories %}..    
-000010b0: 2020 2020 2020 2020 3c68 333e 3c61 2068          <h3><a h
-000010c0: 7265 663d 227b 2520 7572 6c20 2766 6171  ref="{% url 'faq
-000010d0: 3a63 6174 6567 6f72 795f 6465 7461 696c  :category_detail
-000010e0: 2720 6361 7465 676f 7279 2e73 6c75 6720  ' category.slug 
-000010f0: 257d 223e 7b7b 6361 7465 676f 7279 2e6e  %}">{{category.n
-00001100: 616d 657d 7d3c 2f61 3e3c 2f68 333e 0d0a  ame}}</a></h3>..
-00001110: 2020 2020 2020 2020 2020 2020 7b25 2069              {% i
-00001120: 6620 6361 7465 676f 7279 2e64 6573 6372  f category.descr
-00001130: 6970 7469 6f6e 2025 7d0d 0a20 2020 2020  iption %}..     
-00001140: 2020 2020 2020 2020 2020 203c 703e 7b7b             <p>{{
-00001150: 6361 7465 676f 7279 2e64 6573 6372 6970  category.descrip
-00001160: 7469 6f6e 7d7d 3c2f 703e 0d0a 2020 2020  tion}}</p>..    
-00001170: 2020 2020 2020 2020 7b25 2065 6e64 6966          {% endif
-00001180: 2025 7d0d 0a20 2020 2020 2020 2020 2020   %}..           
-00001190: 203c 6872 3e0d 0a20 2020 2020 2020 207b   <hr>..        {
-000011a0: 2520 656e 6466 6f72 2025 7d0d 0a0d 0a0d  % endfor %}.....
-000011b0: 0a32 2e20 6361 7465 676f 7279 5f64 6574  .2. category_det
-000011c0: 6169 6c2e 6874 6d6c 202d 2066 6171 2063  ail.html - faq c
-000011d0: 6174 6567 6f72 7920 6465 7461 696c 2076  ategory detail v
-000011e0: 6965 7720 6966 2075 7369 6e67 2063 6174  iew if using cat
-000011f0: 6567 6f72 6965 733a 3a0d 0a0d 0a0d 0a20  egories::...... 
-00001200: 2020 2020 2020 203c 6831 3e63 686f 6f73         <h1>choos
-00001210: 6520 6120 4641 5120 5175 6573 7469 6f6e  e a FAQ Question
-00001220: 3c2f 6831 3e0d 0a20 2020 2020 2020 203c  </h1>..        <
-00001230: 6832 3e7b 7b63 6174 6567 6f72 797d 7d3c  h2>{{category}}<
-00001240: 2f68 323e 0d0a 2020 2020 2020 2020 7b25  /h2>..        {%
-00001250: 2069 6620 6361 7465 676f 7279 2e64 6573   if category.des
-00001260: 6372 6970 7469 6f6e 2025 7d0d 0a20 2020  cription %}..   
-00001270: 2020 2020 203c 703e 7b7b 6361 7465 676f       <p>{{catego
-00001280: 7279 2e64 6573 6372 6970 7469 6f6e 7d7d  ry.description}}
-00001290: 3c2f 703e 0d0a 2020 2020 2020 2020 7b25  </p>..        {%
-000012a0: 2065 6e64 6966 2025 7d0d 0a20 2020 2020   endif %}..     
-000012b0: 2020 203c 6872 3e0d 0a20 2020 2020 2020     <hr>..       
-000012c0: 207b 2520 666f 7220 7175 6573 7469 6f6e   {% for question
-000012d0: 2069 6e20 6361 7465 676f 7279 2e71 7565   in category.que
-000012e0: 7374 696f 6e5f 7365 742e 616c 6c20 257d  stion_set.all %}
-000012f0: 0d0a 2020 2020 2020 2020 2020 2020 3c68  ..            <h
-00001300: 333e 3c61 2068 7265 663d 227b 2520 7572  3><a href="{% ur
-00001310: 6c20 2766 6171 3a71 7565 7374 696f 6e5f  l 'faq:question_
-00001320: 6465 7461 696c 2720 6361 7465 676f 7279  detail' category
-00001330: 2e73 6c75 6720 7175 6573 7469 6f6e 2e73  .slug question.s
-00001340: 6c75 6720 257d 223e 7b7b 7175 6573 7469  lug %}">{{questi
-00001350: 6f6e 2e71 7565 7374 696f 6e7d 7d3c 2f61  on.question}}</a
-00001360: 3e3c 2f68 333e 0d0a 2020 2020 2020 2020  ></h3>..        
-00001370: 7b25 2065 6e64 666f 7220 257d 0d0a 2020  {% endfor %}..  
-00001380: 2020 2020 2020 3c68 723e 0d0a 2020 2020        <hr>..    
-00001390: 2020 2020 3c61 2068 7265 663d 227b 2520      <a href="{% 
-000013a0: 7572 6c20 2766 6171 3a69 6e64 6578 5f76  url 'faq:index_v
-000013b0: 6965 7727 2025 7d22 3e62 6163 6b3c 2f61  iew' %}">back</a
-000013c0: 3e0d 0a20 2020 2020 2020 207b 2520 6966  >..        {% if
-000013d0: 2063 616e 5f61 6464 5f71 7565 7374 696f   can_add_questio
-000013e0: 6e20 257d 0d0a 2020 2020 2020 2020 2020  n %}..          
-000013f0: 2020 3c61 2068 7265 663d 227b 2520 7572    <a href="{% ur
-00001400: 6c20 2766 6171 3a61 6464 5f71 7565 7374  l 'faq:add_quest
-00001410: 696f 6e27 2063 6174 6567 6f72 792e 736c  ion' category.sl
-00001420: 7567 2025 7d22 3e61 6464 2071 7565 7374  ug %}">add quest
-00001430: 696f 6e3c 2f61 3e0d 0a20 2020 2020 2020  ion</a>..       
-00001440: 207b 2520 656e 6469 6620 257d 0d0a 0d0a   {% endif %}....
-00001450: 0d0a 332e 2071 7565 7374 696f 6e73 5f6c  ..3. questions_l
-00001460: 6973 742e 6874 6d6c 202d 206c 6973 7473  ist.html - lists
-00001470: 2061 6c6c 2071 7565 7374 696f 6e73 2069   all questions i
-00001480: 6620 6e6f 7420 7573 696e 6720 6361 7465  f not using cate
-00001490: 676f 7269 6573 3a3a 0d0a 0d0a 0d0a 2020  gories::......  
-000014a0: 2020 2020 2020 3c68 313e 6368 6f6f 7365        <h1>choose
-000014b0: 2061 2046 4151 2051 7565 7374 696f 6e3c   a FAQ Question<
-000014c0: 2f68 313e 0d0a 2020 2020 2020 2020 7b25  /h1>..        {%
-000014d0: 2066 6f72 2071 7565 7374 696f 6e20 696e   for question in
-000014e0: 2071 7565 7374 696f 6e73 2025 7d0d 0a20   questions %}.. 
-000014f0: 2020 2020 2020 2020 2020 203c 6833 3e3c             <h3><
-00001500: 6120 6872 6566 3d22 7b25 2075 726c 2027  a href="{% url '
-00001510: 6661 713a 7175 6573 7469 6f6e 5f64 6574  faq:question_det
-00001520: 6169 6c27 2071 7565 7374 696f 6e2e 736c  ail' question.sl
-00001530: 7567 2025 7d22 3e7b 7b71 7565 7374 696f  ug %}">{{questio
-00001540: 6e2e 7175 6573 7469 6f6e 7d7d 3c2f 613e  n.question}}</a>
-00001550: 3c2f 6833 3e0d 0a20 2020 2020 2020 207b  </h3>..        {
-00001560: 2520 656e 6466 6f72 2025 7d0d 0a20 2020  % endfor %}..   
-00001570: 200d 0a20 2020 2020 2020 207b 2520 6966   ..        {% if
-00001580: 2063 616e 5f61 6464 5f71 7565 7374 696f   can_add_questio
-00001590: 6e20 257d 0d0a 2020 2020 2020 2020 2020  n %}..          
-000015a0: 2020 3c68 723e 0d0a 2020 2020 2020 2020    <hr>..        
-000015b0: 2020 2020 3c61 2068 7265 663d 227b 2520      <a href="{% 
-000015c0: 7572 6c20 2766 6171 3a61 6464 5f71 7565  url 'faq:add_que
-000015d0: 7374 696f 6e27 2025 7d22 3e61 6464 2071  stion' %}">add q
-000015e0: 7565 7374 696f 6e3c 2f61 3e0d 0a20 2020  uestion</a>..   
-000015f0: 2020 2020 207b 2520 656e 6469 6620 257d       {% endif %}
-00001600: 0d0a 0d0a 0d0a 342e 2071 7565 7374 696f  ......4. questio
-00001610: 6e5f 6465 7461 696c 2e68 746d 6c20 2d20  n_detail.html - 
-00001620: 7468 6520 7175 6573 7469 6f6e 2064 6574  the question det
-00001630: 6169 6c20 7061 6765 3a3a 0d0a 0d0a 0d0a  ail page::......
-00001640: 2020 2020 2020 2020 7b25 2065 7874 656e          {% exten
-00001650: 6473 2027 6661 712f 7175 6573 7469 6f6e  ds 'faq/question
-00001660: 5f62 6173 652e 6874 6d6c 2720 257d 0d0a  _base.html' %}..
-00001670: 2020 2020 0d0a 2020 2020 2020 2020 7b25      ..        {%
-00001680: 2062 6c6f 636b 2071 7565 7374 696f 6e5f   block question_
-00001690: 636f 6e74 656e 7420 257d 0d0a 2020 2020  content %}..    
-000016a0: 2020 2020 7b25 2069 6620 616c 6c6f 775f      {% if allow_
-000016b0: 6d75 6c74 6970 6c65 5f61 6e73 7765 7273  multiple_answers
-000016c0: 2025 7d0d 0a20 2020 2020 2020 203c 6833   %}..        <h3
-000016d0: 3e61 6e73 7765 7273 3c2f 6833 3e0d 0a20  >answers</h3>.. 
-000016e0: 2020 2020 2020 203c 756c 3e0d 0a20 2020         <ul>..   
-000016f0: 2020 2020 2020 2020 207b 2520 666f 7220           {% for 
-00001700: 616e 7377 6572 2069 6e20 7175 6573 7469  answer in questi
-00001710: 6f6e 2e61 6e73 7765 725f 7365 742e 616c  on.answer_set.al
-00001720: 6c20 257d 0d0a 2020 2020 2020 2020 2020  l %}..          
-00001730: 2020 2020 2020 3c6c 693e 3c62 3e7b 7b61        <li><b>{{a
-00001740: 6e73 7765 722e 616e 7377 6572 7d7d 3c2f  nswer.answer}}</
-00001750: 623e 0d0a 2020 2020 2020 2020 2020 2020  b>..            
-00001760: 2020 2020 2020 2020 7b25 2069 6620 6361          {% if ca
-00001770: 6e5f 766f 7465 5f61 6e73 7765 7220 257d  n_vote_answer %}
-00001780: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001790: 2020 2020 2020 207c 2066 6f75 6e64 2074         | found t
-000017a0: 6869 7320 616e 7377 6572 2068 656c 7066  his answer helpf
-000017b0: 756c 3f0d 0a20 2020 2020 2020 2020 2020  ul?..           
-000017c0: 2020 2020 2020 2020 203c 666f 726d 2073           <form s
-000017d0: 7479 6c65 3d22 6469 7370 6c61 793a 2069  tyle="display: i
-000017e0: 6e6c 696e 653b 2220 6163 7469 6f6e 3d22  nline;" action="
-000017f0: 7b25 2069 6620 6361 7465 676f 7279 5f65  {% if category_e
-00001800: 6e61 626c 6564 2025 7d7b 2520 7572 6c20  nabled %}{% url 
-00001810: 2766 6171 3a76 6f74 655f 616e 7377 6572  'faq:vote_answer
-00001820: 2720 7175 6573 7469 6f6e 2e63 6174 6567  ' question.categ
-00001830: 6f72 792e 736c 7567 2071 7565 7374 696f  ory.slug questio
-00001840: 6e2e 736c 7567 2061 6e73 7765 722e 736c  n.slug answer.sl
-00001850: 7567 2025 7d7b 2520 656c 7365 2025 7d7b  ug %}{% else %}{
-00001860: 2520 7572 6c20 2766 6171 3a76 6f74 655f  % url 'faq:vote_
-00001870: 616e 7377 6572 2720 7175 6573 7469 6f6e  answer' question
-00001880: 2e73 6c75 6720 616e 7377 6572 2e73 6c75  .slug answer.slu
-00001890: 6720 257d 7b25 2065 6e64 6966 2025 7d22  g %}{% endif %}"
-000018a0: 206d 6574 686f 643d 2270 6f73 7422 3e0d   method="post">.
-000018b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000018c0: 2020 2020 2020 2020 207b 2520 6373 7266           {% csrf
-000018d0: 5f74 6f6b 656e 2025 7d0d 0a20 2020 2020  _token %}..     
-000018e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000018f0: 2020 203c 696e 7075 7420 7479 7065 3d22     <input type="
-00001900: 6869 6464 656e 2220 7661 6c75 653d 5472  hidden" value=Tr
-00001910: 7565 206e 616d 653d 2276 6f74 6522 3e0d  ue name="vote">.
-00001920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001930: 2020 2020 2020 2020 203c 6275 7474 6f6e           <button
-00001940: 2074 7970 653d 2273 7562 6d69 7422 3e79   type="submit">y
-00001950: 6573 287b 7b61 6e73 7765 722e 6865 6c70  es({{answer.help
-00001960: 6675 6c7d 7d29 3c2f 6275 7474 6f6e 3e0d  ful}})</button>.
-00001970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001980: 2020 2020 203c 2f66 6f72 6d3e 0d0a 2020       </form>..  
-00001990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019a0: 2020 3c66 6f72 6d20 7374 796c 653d 2264    <form style="d
-000019b0: 6973 706c 6179 3a20 696e 6c69 6e65 3b22  isplay: inline;"
-000019c0: 2061 6374 696f 6e3d 227b 2520 6966 2063   action="{% if c
-000019d0: 6174 6567 6f72 795f 656e 6162 6c65 6420  ategory_enabled 
-000019e0: 257d 7b25 2075 726c 2027 6661 713a 766f  %}{% url 'faq:vo
-000019f0: 7465 5f61 6e73 7765 7227 2071 7565 7374  te_answer' quest
-00001a00: 696f 6e2e 6361 7465 676f 7279 2e73 6c75  ion.category.slu
-00001a10: 6720 7175 6573 7469 6f6e 2e73 6c75 6720  g question.slug 
-00001a20: 616e 7377 6572 2e73 6c75 6720 257d 7b25  answer.slug %}{%
-00001a30: 2065 6c73 6520 257d 7b25 2075 726c 2027   else %}{% url '
-00001a40: 6661 713a 766f 7465 5f61 6e73 7765 7227  faq:vote_answer'
-00001a50: 2071 7565 7374 696f 6e2e 736c 7567 2061   question.slug a
-00001a60: 6e73 7765 722e 736c 7567 2025 7d7b 2520  nswer.slug %}{% 
-00001a70: 656e 6469 6620 257d 2220 6d65 7468 6f64  endif %}" method
-00001a80: 3d22 706f 7374 223e 0d0a 2020 2020 2020  ="post">..      
-00001a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001aa0: 2020 7b25 2063 7372 665f 746f 6b65 6e20    {% csrf_token 
-00001ab0: 257d 0d0a 2020 2020 2020 2020 2020 2020  %}..            
-00001ac0: 2020 2020 2020 2020 2020 2020 3c69 6e70              <inp
-00001ad0: 7574 2074 7970 653d 2268 6964 6465 6e22  ut type="hidden"
-00001ae0: 2076 616c 7565 3d46 616c 7365 206e 616d   value=False nam
-00001af0: 653d 2276 6f74 6522 3e0d 0a20 2020 2020  e="vote">..     
-00001b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b10: 2020 203c 6275 7474 6f6e 2074 7970 653d     <button type=
-00001b20: 2273 7562 6d69 7422 3e6e 6f28 7b7b 616e  "submit">no({{an
-00001b30: 7377 6572 2e6e 6f74 5f68 656c 7066 756c  swer.not_helpful
-00001b40: 7d7d 293c 2f62 7574 746f 6e3e 0d0a 2020  }})</button>..  
-00001b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b60: 2020 3c2f 666f 726d 3e0d 0a20 2020 2020    </form>..     
-00001b70: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00001b80: 2520 656e 6469 6620 257d 0d0a 2020 2020  % endif %}..    
-00001b90: 2020 2020 2020 2020 2020 2020 3c2f 6c69              </li
-00001ba0: 3e0d 0a20 2020 2020 2020 2020 2020 207b  >..            {
-00001bb0: 2520 656e 6466 6f72 2025 7d0d 0a20 2020  % endfor %}..   
-00001bc0: 2020 2020 203c 2f75 6c3e 0d0a 2020 2020       </ul>..    
-00001bd0: 0d0a 2020 2020 2020 2020 7b25 2065 6c73  ..        {% els
-00001be0: 6520 257d 0d0a 2020 2020 2020 2020 2020  e %}..          
-00001bf0: 2020 7b25 2069 6620 7175 6573 7469 6f6e    {% if question
-00001c00: 2e61 6e73 7765 725f 7365 742e 6578 6973  .answer_set.exis
-00001c10: 7473 2025 7d0d 0a20 2020 2020 2020 2020  ts %}..         
-00001c20: 2020 2020 2020 203c 703e 616e 7377 6572         <p>answer
-00001c30: 3a3c 2f70 3e0d 0a20 2020 2020 2020 2020  :</p>..         
-00001c40: 2020 2020 2020 203c 6833 3e7b 7b71 7565         <h3>{{que
-00001c50: 7374 696f 6e2e 616e 7377 6572 5f73 6574  stion.answer_set
-00001c60: 2e66 6972 7374 2e61 6e73 7765 727d 7d3c  .first.answer}}<
-00001c70: 2f68 333e 0d0a 2020 2020 2020 2020 2020  /h3>..          
-00001c80: 2020 2020 2020 7b25 2069 6620 6361 6e5f        {% if can_
-00001c90: 766f 7465 5f61 6e73 7765 7220 257d 0d0a  vote_answer %}..
-00001ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001cb0: 2066 6f75 6e64 2074 6869 7320 616e 7377   found this answ
-00001cc0: 6572 2068 656c 7066 756c 3f0d 0a20 2020  er helpful?..   
-00001cd0: 2020 2020 2020 2020 2020 2020 203c 666f               <fo
-00001ce0: 726d 2073 7479 6c65 3d22 6469 7370 6c61  rm style="displa
-00001cf0: 793a 2069 6e6c 696e 653b 2220 6163 7469  y: inline;" acti
-00001d00: 6f6e 3d22 7b25 2069 6620 6361 7465 676f  on="{% if catego
-00001d10: 7279 5f65 6e61 626c 6564 2025 7d7b 2520  ry_enabled %}{% 
-00001d20: 7572 6c20 2766 6171 3a76 6f74 655f 616e  url 'faq:vote_an
-00001d30: 7377 6572 2720 7175 6573 7469 6f6e 2e63  swer' question.c
-00001d40: 6174 6567 6f72 792e 736c 7567 2071 7565  ategory.slug que
-00001d50: 7374 696f 6e2e 736c 7567 2071 7565 7374  stion.slug quest
-00001d60: 696f 6e2e 616e 7377 6572 5f73 6574 2e66  ion.answer_set.f
-00001d70: 6972 7374 2e73 6c75 6720 257d 7b25 2065  irst.slug %}{% e
-00001d80: 6c73 6520 257d 7b25 2075 726c 2027 6661  lse %}{% url 'fa
-00001d90: 713a 766f 7465 5f61 6e73 7765 7227 2071  q:vote_answer' q
-00001da0: 7565 7374 696f 6e2e 736c 7567 2071 7565  uestion.slug que
-00001db0: 7374 696f 6e2e 616e 7377 6572 5f73 6574  stion.answer_set
-00001dc0: 2e66 6972 7374 2e73 6c75 6720 257d 7b25  .first.slug %}{%
-00001dd0: 2065 6e64 6966 2025 7d22 206d 6574 686f   endif %}" metho
-00001de0: 643d 2270 6f73 7422 3e0d 0a20 2020 2020  d="post">..     
-00001df0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00001e00: 2520 6373 7266 5f74 6f6b 656e 2025 7d0d  % csrf_token %}.
-00001e10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001e20: 2020 2020 203c 696e 7075 7420 7479 7065       <input type
-00001e30: 3d22 6869 6464 656e 2220 7661 6c75 653d  ="hidden" value=
-00001e40: 5472 7565 206e 616d 653d 2276 6f74 6522  True name="vote"
-00001e50: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
-00001e60: 2020 2020 2020 203c 6275 7474 6f6e 2074         <button t
-00001e70: 7970 653d 2273 7562 6d69 7422 3e79 6573  ype="submit">yes
-00001e80: 287b 7b71 7565 7374 696f 6e2e 616e 7377  ({{question.answ
-00001e90: 6572 5f73 6574 2e66 6972 7374 2e68 656c  er_set.first.hel
-00001ea0: 7066 756c 7d7d 293c 2f62 7574 746f 6e3e  pful}})</button>
-00001eb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001ec0: 2020 3c2f 666f 726d 3e0d 0a20 2020 2020    </form>..     
-00001ed0: 2020 2020 2020 2020 2020 203c 666f 726d             <form
-00001ee0: 2073 7479 6c65 3d22 6469 7370 6c61 793a   style="display:
-00001ef0: 2069 6e6c 696e 653b 2220 6163 7469 6f6e   inline;" action
-00001f00: 3d22 7b25 2069 6620 6361 7465 676f 7279  ="{% if category
-00001f10: 5f65 6e61 626c 6564 2025 7d7b 2520 7572  _enabled %}{% ur
-00001f20: 6c20 2766 6171 3a76 6f74 655f 616e 7377  l 'faq:vote_answ
-00001f30: 6572 2720 7175 6573 7469 6f6e 2e63 6174  er' question.cat
-00001f40: 6567 6f72 792e 736c 7567 2071 7565 7374  egory.slug quest
-00001f50: 696f 6e2e 736c 7567 2071 7565 7374 696f  ion.slug questio
-00001f60: 6e2e 616e 7377 6572 5f73 6574 2e66 6972  n.answer_set.fir
-00001f70: 7374 2e73 6c75 6720 257d 7b25 2065 6c73  st.slug %}{% els
-00001f80: 6520 257d 7b25 2075 726c 2027 6661 713a  e %}{% url 'faq:
-00001f90: 766f 7465 5f61 6e73 7765 7227 2071 7565  vote_answer' que
-00001fa0: 7374 696f 6e2e 736c 7567 2071 7565 7374  stion.slug quest
-00001fb0: 696f 6e2e 616e 7377 6572 5f73 6574 2e66  ion.answer_set.f
-00001fc0: 6972 7374 2e73 6c75 6720 257d 7b25 2065  irst.slug %}{% e
-00001fd0: 6e64 6966 2025 7d22 206d 6574 686f 643d  ndif %}" method=
-00001fe0: 2270 6f73 7422 3e0d 0a20 2020 2020 2020  "post">..       
-00001ff0: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
-00002000: 6373 7266 5f74 6f6b 656e 2025 7d0d 0a20  csrf_token %}.. 
-00002010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002020: 2020 203c 696e 7075 7420 7479 7065 3d22     <input type="
-00002030: 6869 6464 656e 2220 7661 6c75 653d 4661  hidden" value=Fa
-00002040: 6c73 6520 6e61 6d65 3d22 766f 7465 223e  lse name="vote">
-00002050: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002060: 2020 2020 2020 3c62 7574 746f 6e20 7479        <button ty
-00002070: 7065 3d22 7375 626d 6974 223e 6e6f 287b  pe="submit">no({
-00002080: 7b71 7565 7374 696f 6e2e 616e 7377 6572  {question.answer
-00002090: 5f73 6574 2e66 6972 7374 2e6e 6f74 5f68  _set.first.not_h
-000020a0: 656c 7066 756c 7d7d 293c 2f62 7574 746f  elpful}})</butto
-000020b0: 6e3e 0d0a 2020 2020 2020 2020 2020 2020  n>..            
-000020c0: 2020 2020 3c2f 666f 726d 3e0d 0a20 2020      </form>..   
-000020d0: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
-000020e0: 656e 6469 6620 257d 0d0a 2020 2020 2020  endif %}..      
-000020f0: 2020 2020 2020 7b25 2065 6c73 6520 257d        {% else %}
-00002100: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002110: 2020 6e6f 2061 6e73 7765 7273 2079 6574    no answers yet
-00002120: 0d0a 2020 2020 2020 2020 2020 2020 7b25  ..            {%
-00002130: 2065 6e64 6966 2025 7d0d 0a20 2020 2020   endif %}..     
-00002140: 2020 207b 2520 656e 6469 6620 257d 0d0a     {% endif %}..
-00002150: 2020 2020 0d0a 2020 2020 0d0a 2020 2020      ..    ..    
-00002160: 2020 2020 7b25 2069 6620 6361 6e5f 616e      {% if can_an
-00002170: 7377 6572 5f71 7565 7374 696f 6e20 257d  swer_question %}
-00002180: 0d0a 2020 2020 2020 2020 2020 2020 7b25  ..            {%
-00002190: 2069 6620 6361 7465 676f 7279 5f65 6e61   if category_ena
-000021a0: 626c 6564 2025 7d0d 0a20 2020 2020 2020  bled %}..       
-000021b0: 2020 2020 2020 2020 203c 6120 6872 6566           <a href
-000021c0: 3d22 7b25 2075 726c 2027 6661 713a 616e  ="{% url 'faq:an
-000021d0: 7377 6572 5f71 7565 7374 696f 6e27 2071  swer_question' q
-000021e0: 7565 7374 696f 6e2e 6361 7465 676f 7279  uestion.category
-000021f0: 2e73 6c75 6720 7175 6573 7469 6f6e 2e73  .slug question.s
-00002200: 6c75 6720 257d 223e 616e 7377 6572 2071  lug %}">answer q
-00002210: 7565 7374 696f 6e3c 2f61 3e0d 0a20 2020  uestion</a>..   
-00002220: 2020 2020 2020 2020 207b 2520 656c 7365           {% else
-00002230: 2025 7d0d 0a20 2020 2020 2020 2020 2020   %}..           
-00002240: 2020 2020 203c 6120 6872 6566 3d22 7b25       <a href="{%
-00002250: 2075 726c 2027 6661 713a 616e 7377 6572   url 'faq:answer
-00002260: 5f71 7565 7374 696f 6e27 2071 7565 7374  _question' quest
-00002270: 696f 6e2e 736c 7567 2025 7d22 3e61 6e73  ion.slug %}">ans
-00002280: 7765 7220 7175 6573 7469 6f6e 3c2f 613e  wer question</a>
-00002290: 0d0a 2020 2020 2020 2020 2020 2020 7b25  ..            {%
-000022a0: 2065 6e64 6966 2025 7d0d 0a20 2020 2020   endif %}..     
-000022b0: 2020 207b 2520 656e 6469 6620 257d 0d0a     {% endif %}..
-000022c0: 2020 2020 2020 2020 3c68 723e 0d0a 2020          <hr>..  
-000022d0: 2020 2020 2020 7b25 2069 6620 636f 6d6d        {% if comm
-000022e0: 656e 7473 5f61 6c6c 6f77 6564 2025 7d0d  ents_allowed %}.
-000022f0: 0a20 2020 2020 2020 2020 2020 207b 2520  .            {% 
-00002300: 696e 636c 7564 6520 2766 6171 2f63 6f6d  include 'faq/com
-00002310: 6d65 6e74 732e 6874 6d6c 2720 257d 0d0a  ments.html' %}..
-00002320: 2020 2020 2020 2020 7b25 2065 6e64 6966          {% endif
-00002330: 2025 7d0d 0a20 2020 200d 0a20 2020 2020   %}..    ..     
-00002340: 2020 207b 2520 656e 6462 6c6f 636b 2025     {% endblock %
-00002350: 7d0d 0a0d 0a35 2e20 616e 7377 6572 5f66  }....5. answer_f
-00002360: 6f72 6d2e 6874 6d6c 202d 2066 6f72 6d20  orm.html - form 
-00002370: 746f 2061 6464 2061 6e73 7765 7220 746f  to add answer to
-00002380: 2071 7565 7374 696f 6e3a 3a0d 0a0d 0a0d   question::.....
-00002390: 0a20 2020 2020 2020 203c 6831 3e41 6e73  .        <h1>Ans
-000023a0: 7765 7220 5175 6573 7469 6f6e 3c2f 6831  wer Question</h1
-000023b0: 3e0d 0a20 2020 2020 2020 203c 6120 6872  >..        <a hr
-000023c0: 6566 3d22 7b7b 7175 6573 7469 6f6e 2e67  ef="{{question.g
-000023d0: 6574 5f61 6273 6f6c 7574 655f 7572 6c7d  et_absolute_url}
-000023e0: 7d22 3e3c 6833 3e7b 7b71 7565 7374 696f  }"><h3>{{questio
-000023f0: 6e2e 7175 6573 7469 6f6e 7d7d 3c2f 6833  n.question}}</h3
-00002400: 3e3c 2f61 3e0d 0a20 2020 2020 2020 203c  ></a>..        <
-00002410: 666f 726d 206d 6574 686f 643d 2270 6f73  form method="pos
-00002420: 7422 3e0d 0a20 2020 2020 2020 2020 2020  t">..           
-00002430: 207b 2520 6373 7266 5f74 6f6b 656e 2025   {% csrf_token %
-00002440: 7d0d 0a20 2020 2020 2020 2020 2020 207b  }..            {
-00002450: 7b66 6f72 6d7d 7d0d 0a20 2020 2020 2020  {form}}..       
-00002460: 2020 2020 203c 696e 7075 7420 7479 7065       <input type
-00002470: 3d22 7375 626d 6974 223e 0d0a 2020 2020  ="submit">..    
-00002480: 2020 2020 3c2f 666f 726d 3e0d 0a0d 0a36      </form>....6
-00002490: 2e20 636f 6d6d 656e 745f 666f 726d 2e68  . comment_form.h
-000024a0: 746d 6c20 2d20 666f 726d 2074 6f20 6164  tml - form to ad
-000024b0: 6420 636f 6d6d 656e 7473 2074 6f20 7175  d comments to qu
-000024c0: 6573 7469 6f6e 2028 6f6e 6c79 2073 686f  estion (only sho
-000024d0: 7773 2075 7020 7768 656e 2066 6f72 6d20  ws up when form 
-000024e0: 6861 7320 6572 726f 7220 6265 6361 7573  has error becaus
-000024f0: 6520 7669 6577 206f 6e6c 7920 6765 7473  e view only gets
-00002500: 2070 6f73 7465 6420 746f 293a 3a0d 0a0d   posted to)::...
-00002510: 0a0d 0a20 2020 2020 2020 203c 6831 3e50  ...        <h1>P
-00002520: 6f73 7420 4120 436f 6d6d 656e 743c 2f68  ost A Comment</h
-00002530: 313e 0d0a 2020 2020 2020 2020 3c61 2068  1>..        <a h
-00002540: 7265 663d 227b 7b71 7565 7374 696f 6e2e  ref="{{question.
-00002550: 6765 745f 6162 736f 6c75 7465 5f75 726c  get_absolute_url
-00002560: 7d7d 223e 3c68 333e 7b7b 7175 6573 7469  }}"><h3>{{questi
-00002570: 6f6e 2e71 7565 7374 696f 6e7d 7d3c 2f68  on.question}}</h
-00002580: 333e 3c2f 613e 0d0a 2020 2020 2020 2020  3></a>..        
-00002590: 3c66 6f72 6d20 6d65 7468 6f64 3d22 706f  <form method="po
-000025a0: 7374 223e 0d0a 2020 2020 2020 2020 2020  st">..          
-000025b0: 2020 7b25 2063 7372 665f 746f 6b65 6e20    {% csrf_token 
-000025c0: 257d 0d0a 2020 2020 2020 2020 2020 2020  %}..            
-000025d0: 7b7b 666f 726d 7d7d 0d0a 2020 2020 2020  {{form}}..      
-000025e0: 2020 2020 2020 3c69 6e70 7574 2074 7970        <input typ
-000025f0: 653d 2273 7562 6d69 7422 3e0d 0a20 2020  e="submit">..   
-00002600: 2020 2020 203c 2f66 6f72 6d3e 0d0a 0d0a       </form>....
-00002610: 372e 2071 7565 7374 696f 6e5f 666f 726d  7. question_form
-00002620: 2e68 746d 6c20 2d20 666f 726d 2074 6f20  .html - form to 
-00002630: 6164 6420 6120 6e65 7720 7175 6573 7469  add a new questi
-00002640: 6f6e 3a3a 0d0a 0d0a 0d0a 2020 2020 2020  on::......      
-00002650: 2020 3c68 313e 4164 6420 596f 7572 2051    <h1>Add Your Q
-00002660: 7565 7374 696f 6e3c 2f68 313e 0d0a 2020  uestion</h1>..  
-00002670: 2020 2020 2020 3c66 6f72 6d20 6d65 7468        <form meth
-00002680: 6f64 3d22 706f 7374 223e 0d0a 2020 2020  od="post">..    
-00002690: 2020 2020 2020 2020 7b25 2063 7372 665f          {% csrf_
-000026a0: 746f 6b65 6e20 257d 0d0a 2020 2020 2020  token %}..      
-000026b0: 2020 2020 2020 7b7b 666f 726d 7d7d 0d0a        {{form}}..
-000026c0: 2020 2020 2020 2020 2020 2020 3c69 6e70              <inp
-000026d0: 7574 2074 7970 653d 2273 7562 6d69 7422  ut type="submit"
-000026e0: 3e0d 0a20 2020 2020 2020 203c 2f66 6f72  >..        </for
-000026f0: 6d3e 0d0a 0d0a 382e 2076 6f74 655f 666f  m>....8. vote_fo
-00002700: 726d 2e68 746d 6c20 2d20 666f 726d 2066  rm.html - form f
-00002710: 6f72 2076 6f74 696e 6720 7175 6573 7469  or voting questi
-00002720: 6f6e 7320 616e 6420 616e 7377 6572 7320  ons and answers 
-00002730: 286f 6e6c 7920 7368 6f77 7320 7570 2077  (only shows up w
-00002740: 6865 6e20 666f 726d 2068 6173 2065 7272  hen form has err
-00002750: 6f72 2062 6563 6175 7365 2076 6965 7720  or because view 
-00002760: 6f6e 6c79 2067 6574 7320 706f 7374 6564  only gets posted
-00002770: 2074 6f29 3a3a 0d0a 0d0a 0d0a 2020 2020   to)::......    
-00002780: 2020 2020 3c68 313e 766f 7465 3c2f 6831      <h1>vote</h1
-00002790: 3e0d 0a20 2020 2020 2020 203c 666f 726d  >..        <form
-000027a0: 206d 6574 686f 643d 2270 6f73 7422 3e0d   method="post">.
-000027b0: 0a20 2020 2020 2020 2020 2020 207b 2520  .            {% 
-000027c0: 6373 7266 5f74 6f6b 656e 2025 7d0d 0a20  csrf_token %}.. 
-000027d0: 2020 2020 2020 2020 2020 207b 7b66 6f72             {{for
-000027e0: 6d7d 7d0d 0a20 2020 2020 2020 2020 2020  m}}..           
-000027f0: 203c 696e 7075 7420 7479 7065 3d22 7375   <input type="su
-00002800: 626d 6974 223e 0d0a 2020 2020 2020 2020  bmit">..        
-00002810: 3c2f 666f 726d 3e0d 0a0d 0a39 2e20 636f  </form>....9. co
-00002820: 6d6d 656e 7473 2e68 746d 6c20 2d20 6966  mments.html - if
-00002830: 2063 6f6d 6d65 6e74 7320 6172 6520 616c   comments are al
-00002840: 6c6f 7765 6420 7468 6973 2074 656d 706c  lowed this templ
-00002850: 6174 6520 6973 2069 6e63 6c75 6465 6420  ate is included 
-00002860: 696e 2074 6865 2071 7565 7374 696f 6e20  in the question 
-00002870: 6465 7461 696c 2e68 746d 6c3a 3a0d 0a0d  detail.html::...
-00002880: 0a0d 0a20 2020 2020 2020 203c 6833 3e63  ...        <h3>c
-00002890: 6f6d 6d65 6e74 733c 2f68 333e 0d0a 2020  omments</h3>..  
-000028a0: 2020 2020 2020 3c75 6c3e 0d0a 2020 2020        <ul>..    
-000028b0: 2020 2020 2020 2020 7b25 2066 6f72 2063          {% for c
-000028c0: 6f6d 6d65 6e74 2069 6e20 7175 6573 7469  omment in questi
-000028d0: 6f6e 2e66 6171 636f 6d6d 656e 745f 7365  on.faqcomment_se
-000028e0: 742e 616c 6c20 257d 0d0a 2020 2020 2020  t.all %}..      
-000028f0: 2020 2020 2020 2020 2020 3c6c 693e 3c68            <li><h
-00002900: 343e 7b7b 636f 6d6d 656e 742e 636f 6d6d  4>{{comment.comm
-00002910: 656e 747d 7d3c 2f68 343e 0d0a 2020 2020  ent}}</h4>..    
-00002920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002930: 706f 7374 6564 2062 7920 7b25 2069 6620  posted by {% if 
-00002940: 636f 6d6d 656e 742e 7573 6572 257d 7b7b  comment.user%}{{
-00002950: 636f 6d6d 656e 742e 7573 6572 7d7d 7b25  comment.user}}{%
-00002960: 2065 6c73 6520 257d 616e 6f6e 796d 6f75   else %}anonymou
-00002970: 737b 2520 656e 6469 6620 257d 207b 7b63  s{% endif %} {{c
-00002980: 6f6d 6d65 6e74 2e70 6f73 745f 7469 6d65  omment.post_time
-00002990: 7c74 696d 6573 696e 6365 7d7d 2061 676f  |timesince}} ago
-000029a0: 3c2f 6c69 3e0d 0a20 2020 2020 2020 2020  </li>..         
-000029b0: 2020 207b 2520 656e 6466 6f72 2025 7d0d     {% endfor %}.
-000029c0: 0a20 2020 2020 2020 203c 2f75 6c3e 0d0a  .        </ul>..
-000029d0: 2020 2020 2020 2020 7b25 2069 6620 6164          {% if ad
-000029e0: 645f 6e65 775f 636f 6d6d 656e 745f 616c  d_new_comment_al
-000029f0: 6c6f 7765 6420 257d 0d0a 2020 2020 2020  lowed %}..      
-00002a00: 2020 2020 2020 7b25 2069 6620 6361 7465        {% if cate
-00002a10: 676f 7279 5f65 6e61 626c 6564 2025 7d0d  gory_enabled %}.
-00002a20: 0a20 2020 2020 2020 2020 2020 203c 666f  .            <fo
-00002a30: 726d 206d 6574 686f 643d 2270 6f73 7422  rm method="post"
-00002a40: 2061 6374 696f 6e3d 227b 2520 7572 6c20   action="{% url 
-00002a50: 2766 6171 3a61 6464 5f63 6f6d 6d65 6e74  'faq:add_comment
-00002a60: 2720 7175 6573 7469 6f6e 2e63 6174 6567  ' question.categ
-00002a70: 6f72 792e 736c 7567 2071 7565 7374 696f  ory.slug questio
-00002a80: 6e2e 736c 7567 2025 7d22 3e0d 0a20 2020  n.slug %}">..   
-00002a90: 2020 2020 2020 2020 207b 2520 656c 7365           {% else
-00002aa0: 2025 7d0d 0a20 2020 2020 2020 2020 2020   %}..           
-00002ab0: 203c 666f 726d 206d 6574 686f 643d 2270   <form method="p
-00002ac0: 6f73 7422 2061 6374 696f 6e3d 227b 2520  ost" action="{% 
-00002ad0: 7572 6c20 2766 6171 3a61 6464 5f63 6f6d  url 'faq:add_com
-00002ae0: 6d65 6e74 2720 7175 6573 7469 6f6e 2e73  ment' question.s
-00002af0: 6c75 6720 257d 223e 0d0a 2020 2020 2020  lug %}">..      
-00002b00: 2020 2020 2020 7b25 2065 6e64 6966 2025        {% endif %
-00002b10: 7d0d 0a20 2020 2020 2020 2020 2020 203c  }..            <
-00002b20: 6669 656c 6473 6574 3e0d 0a20 2020 2020  fieldset>..     
-00002b30: 2020 2020 2020 2020 2020 203c 6c65 6765             <lege
-00002b40: 6e64 3e50 6f73 7420 596f 7572 2043 6f6d  nd>Post Your Com
-00002b50: 6d65 6e74 2048 6572 653a 3c2f 6c65 6765  ment Here:</lege
-00002b60: 6e64 3e0d 0a20 2020 2020 2020 2020 2020  nd>..           
-00002b70: 2020 2020 207b 2520 6373 7266 5f74 6f6b       {% csrf_tok
-00002b80: 656e 2025 7d0d 0a20 2020 2020 2020 2020  en %}..         
-00002b90: 2020 2020 2020 207b 7b63 6f6d 6d65 6e74         {{comment
-00002ba0: 5f66 6f72 6d7d 7d0d 0a20 2020 2020 2020  _form}}..       
-00002bb0: 2020 2020 2020 2020 203c 696e 7075 7420           <input 
-00002bc0: 7479 7065 3d22 7375 626d 6974 2220 6e61  type="submit" na
-00002bd0: 6d65 3d22 706f 7374 223e 0d0a 2020 2020  me="post">..    
-00002be0: 2020 2020 2020 2020 3c2f 6669 656c 6473          </fields
-00002bf0: 6574 3e0d 0a20 2020 2020 2020 2020 2020  et>..           
-00002c00: 203c 2f66 6f72 6d3e 0d0a 2020 2020 2020   </form>..      
-00002c10: 2020 7b25 2065 6e64 6966 2025 7d0d 0a0d    {% endif %}...
-00002c20: 0a23 2320 5465 6d70 6c61 7465 2056 6172  .## Template Var
-00002c30: 6961 626c 6573 0d0a 0d0a 312e 2063 6174  iables....1. cat
-00002c40: 6567 6f72 6965 735f 6c69 7374 2e68 746d  egories_list.htm
-00002c50: 6c0d 0a20 2020 2063 6174 6567 6f72 6965  l..    categorie
-00002c60: 7320 2d20 616c 6c20 7468 6520 6361 7465  s - all the cate
-00002c70: 676f 7269 6573 2028 6361 7465 676f 7279  gories (category
-00002c80: 2071 7565 7279 7365 7429 0d0a 0d0a 322e   queryset)....2.
-00002c90: 2063 6174 6567 6f72 6965 735f 6465 7461   categories_deta
-00002ca0: 696c 2e68 746d 6c0d 0a20 2020 2063 6174  il.html..    cat
-00002cb0: 6567 6f72 7920 2d20 7468 6520 6361 7465  egory - the cate
-00002cc0: 676f 7279 2063 686f 7365 6e20 2863 6174  gory chosen (cat
-00002cd0: 6567 6f72 7920 6f62 6a65 6374 290d 0a20  egory object).. 
-00002ce0: 2020 2063 616e 5f61 6464 5f71 7565 7374     can_add_quest
-00002cf0: 696f 6e20 2d20 626f 6f6c 2069 6620 7468  ion - bool if th
-00002d00: 6520 7573 6572 2063 616e 2061 6464 2061  e user can add a
-00002d10: 2071 7565 7374 696f 6e20 2864 6570 656e   question (depen
-00002d20: 6473 206f 6e20 7468 6520 7365 7474 696e  ds on the settin
-00002d30: 6773 290d 0a33 2e20 7175 6573 7469 6f6e  gs)..3. question
-00002d40: 735f 6c69 7374 2e68 746d 6c0d 0a20 2020  s_list.html..   
-00002d50: 2071 7565 7374 696f 6e73 202d 2061 6c6c   questions - all
-00002d60: 2074 6865 2071 7565 7374 696f 6e73 2028   the questions (
-00002d70: 7175 6573 7469 6f6e 2071 7565 7279 7365  question queryse
-00002d80: 7429 0d0a 2020 2020 6361 6e5f 6164 645f  t)..    can_add_
-00002d90: 7175 6573 7469 6f6e 202d 2062 6f6f 6c20  question - bool 
-00002da0: 6966 2074 6865 2075 7365 7220 6361 6e20  if the user can 
-00002db0: 6164 6420 6120 7175 6573 7469 6f6e 2028  add a question (
-00002dc0: 6465 7065 6e64 7320 6f6e 2074 6865 2073  depends on the s
-00002dd0: 6574 7469 6e67 7329 0d0a 342e 2071 7565  ettings)..4. que
-00002de0: 7374 696f 6e5f 6465 7461 696c 2e68 746d  stion_detail.htm
-00002df0: 6c0d 0a20 2020 2071 7565 7374 696f 6e20  l..    question 
-00002e00: 2d20 7468 6520 7175 6573 7469 6f6e 2063  - the question c
-00002e10: 686f 7365 6e20 2871 7565 7374 696f 6e20  hosen (question 
-00002e20: 6f62 6a65 6374 290d 0a20 2020 2063 616e  object)..    can
-00002e30: 5f76 6f74 655f 7175 6573 7469 6f6e 202d  _vote_question -
-00002e40: 2062 6f6f 6c20 6966 2074 6865 2075 7365   bool if the use
-00002e50: 7220 6361 6e20 766f 7465 2061 2071 7565  r can vote a que
-00002e60: 7374 696f 6e20 2864 6570 656e 6473 206f  stion (depends o
-00002e70: 6e20 7468 6520 7365 7474 696e 6773 290d  n the settings).
-00002e80: 0a20 2020 2063 6174 6567 6f72 795f 656e  .    category_en
-00002e90: 6162 6c65 6420 2d20 626f 6f6c 2069 6620  abled - bool if 
-00002ea0: 6361 7465 676f 7279 2065 6e61 626c 6564  category enabled
-00002eb0: 2069 6e20 7365 7474 696e 6773 0d0a 2020   in settings..  
-00002ec0: 2020 616c 6c6f 775f 6d75 6c74 6970 6c65    allow_multiple
-00002ed0: 5f61 6e73 7765 7273 202d 2062 6f6f 6c20  _answers - bool 
-00002ee0: 6966 206d 756c 7469 706c 6520 616e 7377  if multiple answ
-00002ef0: 6572 7320 616c 6c6f 7765 6420 696e 2073  ers allowed in s
-00002f00: 6574 7469 6e67 730d 0a20 2020 2063 616e  ettings..    can
-00002f10: 5f76 6f74 655f 616e 7377 6572 202d 2062  _vote_answer - b
-00002f20: 6f6f 6c20 6966 2074 6865 2075 7365 7220  ool if the user 
-00002f30: 6361 6e20 766f 7465 2061 6e20 616e 7377  can vote an answ
-00002f40: 6572 2028 6465 7065 6e64 7320 6f6e 2074  er (depends on t
-00002f50: 6865 2073 6574 7469 6e67 7329 0d0a 2020  he settings)..  
-00002f60: 2020 6361 6e5f 616e 7377 6572 5f71 7565    can_answer_que
-00002f70: 7374 696f 6e20 2d20 626f 6f6c 2069 6620  stion - bool if 
-00002f80: 6375 7272 656e 7420 7573 6572 2063 616e  current user can
-00002f90: 2061 6e73 7765 7220 7175 6573 7469 6f6e   answer question
-00002fa0: 2028 6465 7065 6e64 7320 6f6e 2074 6865   (depends on the
-00002fb0: 2073 6574 7469 6e67 7329 0d0a 2020 2020   settings)..    
-00002fc0: 636f 6d6d 656e 7473 5f61 6c6c 6f77 6564  comments_allowed
-00002fd0: 202d 2062 6f6f 6c20 6966 2075 7369 6e67   - bool if using
-00002fe0: 2063 6f6d 6d65 6e74 7320 696e 2073 6574   comments in set
-00002ff0: 7469 6e67 730d 0a20 2020 2061 6464 5f6e  tings..    add_n
-00003000: 6577 5f63 6f6d 6d65 6e74 5f61 6c6c 6f77  ew_comment_allow
-00003010: 6564 202d 2062 6f6f 6c20 6966 2063 7572  ed - bool if cur
-00003020: 7265 6e74 2075 7365 7220 6361 6e20 6164  rent user can ad
-00003030: 6420 636f 6d6d 656e 7420 2864 6570 656e  d comment (depen
-00003040: 6473 206f 6e20 7468 6520 7365 7474 696e  ds on the settin
-00003050: 6773 290d 0a20 2020 2063 6f6d 6d65 6e74  gs)..    comment
-00003060: 5f66 6f72 6d20 2d20 666f 726d 2074 6f20  _form - form to 
-00003070: 7375 626d 6974 2061 206e 6577 2063 6f6d  submit a new com
-00003080: 6d65 6e74 0d0a 352e 2061 6e73 7765 725f  ment..5. answer_
-00003090: 666f 726d 2e68 746d 6c0d 0a20 2020 2071  form.html..    q
-000030a0: 7565 7374 696f 6e20 2d20 7468 6520 7175  uestion - the qu
-000030b0: 6573 7469 6f6e 2074 6f20 6164 6420 616e  estion to add an
-000030c0: 7377 6572 2074 6f20 2871 7565 7374 696f  swer to (questio
-000030d0: 6e20 6f62 6a65 6374 290d 0a20 2020 2066  n object)..    f
-000030e0: 6f72 6d20 2d20 666f 726d 2074 6f20 6164  orm - form to ad
-000030f0: 6420 6e65 7720 616e 7377 6572 0d0a 362e  d new answer..6.
-00003100: 2063 6f6d 6d65 6e74 5f66 6f72 6d2e 6874   comment_form.ht
-00003110: 6d6c 0d0a 2020 2020 7175 6573 7469 6f6e  ml..    question
-00003120: 202d 2074 6865 2071 7565 7374 696f 6e20   - the question 
-00003130: 746f 2061 6464 2063 6f6d 6d65 6e74 2074  to add comment t
-00003140: 6f20 2871 7565 7374 696f 6e20 6f62 6a65  o (question obje
-00003150: 6374 290d 0a20 2020 2066 6f72 6d20 2d20  ct)..    form - 
-00003160: 666f 726d 2074 6f20 6164 6420 6e65 7720  form to add new 
-00003170: 636f 6d6d 656e 740d 0a37 2e20 7175 6573  comment..7. ques
-00003180: 7469 6f6e 5f66 6f72 6d2e 6874 6d6c 0d0a  tion_form.html..
-00003190: 2020 2020 666f 726d 202d 2066 6f72 6d20      form - form 
-000031a0: 746f 2061 6464 206e 6577 2071 7565 7374  to add new quest
-000031b0: 696f 6e0d 0a38 2e20 766f 7465 5f66 6f72  ion..8. vote_for
-000031c0: 6d2e 6874 6d6c 0d0a 2020 2020 666f 726d  m.html..    form
-000031d0: 202d 2066 6f72 6d20 746f 2076 6f74 6520   - form to vote 
-000031e0: 666f 7220 6120 7175 6573 7469 6f6e 206f  for a question o
-000031f0: 7220 616e 7377 6572 0d0a 0d0a 2323 2055  r answer....## U
-00003200: 726c 730d 0a0d 0a61 6c6c 206f 6620 7468  rls....all of th
-00003210: 6520 666f 6c6c 6f77 696e 6720 7572 6c73  e following urls
-00003220: 2061 7265 2062 7920 6e61 6d65 2074 6865   are by name the
-00003230: 6e20 6164 6469 7469 6f6e 616c 0d0a 7468  n additional..th
-00003240: 6520 6170 7020 6e61 6d65 2066 6f72 2074  e app name for t
-00003250: 6865 2075 726c 7320 6973 2060 6027 6661  he urls is ``'fa
-00003260: 7127 6060 0d0a 0d0a 2a20 696e 6465 785f  q'``....* index_
-00003270: 7669 6577 0d0a 2020 2020 2a20 6e6f 2061  view..    * no a
-00003280: 7267 756d 656e 7473 0d0a 2020 2020 2a20  rguments..    * 
-00003290: 6469 7370 6c61 7973 2061 6c6c 2074 6865  displays all the
-000032a0: 2063 6174 6567 6f72 6965 7320 6966 2063   categories if c
-000032b0: 6174 6567 6f72 6965 7320 6172 6520 656e  ategories are en
-000032c0: 6162 6c65 6420 6f74 6865 7277 6973 6520  abled otherwise 
-000032d0: 7368 6f77 7320 7175 6573 7469 6f6e 730d  shows questions.
-000032e0: 0a2a 2063 6174 6567 6f72 795f 6465 7461  .* category_deta
-000032f0: 696c 0d0a 2020 2020 2a20 6e65 6564 7320  il..    * needs 
-00003300: 6361 7465 676f 7279 2073 6c75 6720 6173  category slug as
-00003310: 2073 6c75 670d 0a20 2020 202a 2064 6973   slug..    * dis
-00003320: 706c 6179 7320 616c 6c20 7468 6520 7175  plays all the qu
-00003330: 6573 7469 6f6e 7320 6769 7665 6e20 7468  estions given th
-00003340: 6520 6361 7465 676f 7279 2077 6865 6e20  e category when 
-00003350: 6361 7465 676f 7269 6573 2061 7265 2065  categories are e
-00003360: 6e61 626c 6564 0d0a 2a20 6164 645f 7175  nabled..* add_qu
-00003370: 6573 7469 6f6e 0d0a 2020 2020 2a20 6966  estion..    * if
-00003380: 2063 6174 6567 6f72 6965 7320 6172 6520   categories are 
-00003390: 656e 6162 6c65 6420 6e65 6564 7320 6361  enabled needs ca
-000033a0: 7465 676f 7279 2073 6c75 6720 6173 2073  tegory slug as s
-000033b0: 6c75 670d 0a20 2020 202a 2069 6620 6c6f  lug..    * if lo
-000033c0: 6767 6564 5f69 6e5f 7573 6572 735f 6361  gged_in_users_ca
-000033d0: 6e5f 6164 645f 7175 6573 7469 6f6e 2074  n_add_question t
-000033e0: 6865 6e20 6469 7370 6c61 7973 2066 6f72  hen displays for
-000033f0: 6d20 666f 7220 6c6f 6767 6564 2069 6e20  m for logged in 
-00003400: 7573 6572 7320 746f 2061 736b 2061 206e  users to ask a n
-00003410: 6577 2071 7565 7374 696f 6e0d 0a2a 2071  ew question..* q
-00003420: 7565 7374 696f 6e5f 6465 7461 696c 0d0a  uestion_detail..
-00003430: 2020 2020 2a20 6e65 6564 7320 7175 6573      * needs ques
-00003440: 7469 6f6e 2073 6c75 6720 6173 2071 7565  tion slug as que
-00003450: 7374 696f 6e20 7c20 6966 2063 6174 6567  stion | if categ
-00003460: 6f72 6965 7320 6172 6520 656e 6162 6c65  ories are enable
-00003470: 6420 6e65 6564 7320 6361 7465 676f 7279  d needs category
-00003480: 2073 6c75 6720 6173 2073 6c75 670d 0a20   slug as slug.. 
-00003490: 2020 202a 2064 6973 706c 6179 7320 7468     * displays th
-000034a0: 6520 6d61 696e 2046 4151 2070 6167 6520  e main FAQ page 
-000034b0: 7769 7468 2074 6865 2071 7565 7374 696f  with the questio
-000034c0: 6e20 616c 6c20 7468 6520 636f 6d6d 656e  n all the commen
-000034d0: 7473 2061 6e64 2061 6e73 7765 7273 0d0a  ts and answers..
-000034e0: 2a20 616e 7377 6572 5f71 7565 7374 696f  * answer_questio
-000034f0: 6e0d 0a20 2020 202a 206e 6565 6473 2071  n..    * needs q
-00003500: 7565 7374 696f 6e20 736c 7567 2061 7320  uestion slug as 
-00003510: 7175 6573 7469 6f6e 207c 2069 6620 6361  question | if ca
-00003520: 7465 676f 7269 6573 2061 7265 2065 6e61  tegories are ena
-00003530: 626c 6564 206e 6565 6473 2063 6174 6567  bled needs categ
-00003540: 6f72 7920 736c 7567 2061 7320 6361 7465  ory slug as cate
-00003550: 676f 7279 0d0a 2020 2020 2a20 6469 7370  gory..    * disp
-00003560: 6c61 7973 2074 6865 2061 6e73 7765 7220  lays the answer 
-00003570: 7175 6573 7469 6f6e 2066 6f72 6d0d 0a2a  question form..*
-00003580: 2061 6464 5f63 6f6d 6d65 6e74 0d0a 2020   add_comment..  
-00003590: 2020 2a20 6e65 6564 7320 7175 6573 7469    * needs questi
-000035a0: 6f6e 2073 6c75 6720 6173 2071 7565 7374  on slug as quest
-000035b0: 696f 6e20 7c20 6966 2063 6174 6567 6f72  ion | if categor
-000035c0: 6965 7320 6172 6520 656e 6162 6c65 6420  ies are enabled 
-000035d0: 6e65 6564 7320 6361 7465 676f 7279 2073  needs category s
-000035e0: 6c75 6720 6173 2063 6174 6567 6f72 790d  lug as category.
-000035f0: 0a20 2020 202a 206f 6e6c 7920 776f 726b  .    * only work
-00003600: 7320 6966 2075 7369 6e67 2063 6f6d 6d65  s if using comme
-00003610: 6e74 730d 0a20 2020 202a 2075 7365 6420  nts..    * used 
-00003620: 746f 2070 6f73 7420 636f 6d6d 656e 7420  to post comment 
-00003630: 666f 726d 2066 726f 6d20 7175 6573 7469  form from questi
-00003640: 6f6e 5f64 6574 6169 6c20 746f 2064 6174  on_detail to dat
-00003650: 6162 6173 650d 0a2a 2076 6f74 655f 616e  abase..* vote_an
-00003660: 7377 6572 0d0a 2020 2020 2a20 6e65 6564  swer..    * need
-00003670: 7320 7175 6573 7469 6f6e 2073 6c75 6720  s question slug 
-00003680: 6173 2071 7565 7374 696f 6e20 7c20 6e65  as question | ne
-00003690: 6564 7320 616e 7377 6572 2073 6c75 6720  eds answer slug 
-000036a0: 6173 2061 6e73 7765 7220 7c20 6966 2063  as answer | if c
-000036b0: 6174 6567 6f72 6965 7320 6172 6520 656e  ategories are en
-000036c0: 6162 6c65 6420 6e65 6564 7320 6361 7465  abled needs cate
-000036d0: 676f 7279 2073 6c75 6720 6173 2063 6174  gory slug as cat
-000036e0: 6567 6f72 790d 0a20 2020 202a 206f 6e6c  egory..    * onl
-000036f0: 7920 776f 726b 7320 6966 2075 7369 6e67  y works if using
-00003700: 2061 6e73 7765 7220 766f 7469 6e67 0d0a   answer voting..
-00003710: 2020 2020 2a20 7573 6564 2074 6f20 706f      * used to po
-00003720: 7374 2068 6964 6465 6e20 696e 7075 7420  st hidden input 
-00003730: 766f 7465 203d 2031 206f 7220 766f 7465  vote = 1 or vote
-00003740: 203d 2030 2064 6570 656e 6469 6e67 206f   = 0 depending o
-00003750: 6e20 766f 7465 2075 7020 6f72 2064 6f77  n vote up or dow
-00003760: 6e0d 0a2a 2076 6f74 655f 7175 6573 7469  n..* vote_questi
-00003770: 6f6e 0d0a 2020 2020 2a20 6e65 6564 7320  on..    * needs 
-00003780: 7175 6573 7469 6f6e 2073 6c75 6720 6173  question slug as
-00003790: 2071 7565 7374 696f 6e20 7c20 6966 2063   question | if c
-000037a0: 6174 6567 6f72 6965 7320 6172 6520 656e  ategories are en
-000037b0: 6162 6c65 6420 6e65 6564 7320 6361 7465  abled needs cate
-000037c0: 676f 7279 2073 6c75 6720 6173 2063 6174  gory slug as cat
-000037d0: 6567 6f72 790d 0a20 2020 202a 206f 6e6c  egory..    * onl
-000037e0: 7920 776f 726b 7320 6966 2075 7369 6e67  y works if using
-000037f0: 2071 7565 7374 696f 6e20 766f 7469 6e67   question voting
-00003800: 0d0a 2020 2020 2a20 7573 6564 2074 6f20  ..    * used to 
-00003810: 706f 7374 2068 6964 6465 6e20 696e 7075  post hidden inpu
-00003820: 7420 766f 7465 203d 2031 206f 7220 766f  t vote = 1 or vo
-00003830: 7465 203d 2030 2064 6570 656e 6469 6e67  te = 0 depending
-00003840: 206f 6e20 766f 7465 2075 7020 6f72 2064   on vote up or d
-00003850: 6f77 6e0d 0a0d 0a23 2320 436f 6e74 7269  own....## Contri
-00003860: 6275 7469 6e67 0d0a 0d0a 646a 616e 676f  buting....django
-00003870: 2d65 6173 792d 6661 7120 6169 6d73 2074  -easy-faq aims t
-00003880: 6f20 6265 2074 6865 2062 6573 7420 6661  o be the best fa
-00003890: 7120 6170 7020 666f 7220 646a 616e 676f  q app for django
-000038a0: 2e20 4974 2077 656c 636f 6d65 7320 2063  . It welcomes  c
-000038b0: 6f6e 7472 6962 7574 696f 6e73 206f 6620  ontributions of 
-000038c0: 616c 6c20 7479 7065 7320 2d20 6973 7375  all types - issu
-000038d0: 6573 2c20 6275 6773 2c20 6665 6174 7572  es, bugs, featur
-000038e0: 6520 7265 7175 6573 7473 2c20 646f 6375  e requests, docu
-000038f0: 6d65 6e74 6174 696f 6e20 7570 6461 7465  mentation update
-00003900: 732c 2074 6573 7473 2061 6e64 2070 756c  s, tests and pul
-00003910: 6c20 7265 7175 6573 7473 0d0a 0d0a 2323  l requests....##
-00003920: 2063 6861 6e67 6520 6c6f 670d 0a30 2e34   change log..0.4
-00003930: 2066 6978 6564 2062 7567 2074 6861 7420   fixed bug that 
-00003940: 6c6f 6767 6564 206f 7574 2075 7365 7273  logged out users
-00003950: 2063 616e 2076 6f74 6520 2d20 7768 6963   can vote - whic
-00003960: 6820 7468 656e 2072 6169 7365 7320 6578  h then raises ex
-00003970: 6365 7074 696f 6e73 0d0a 0d0a 302e 3520  ceptions....0.5 
-00003980: 6669 7865 6420 6d69 6772 6174 696f 6e73  fixed migrations
-00003990: 0d0a 0d0a 312e 3020 6164 6465 6420 7079  ....1.0 added py
-000039a0: 7069 2064 6973 7472 6962 7574 696f 6e0d  pi distribution.
-000039b0: 0a0d 0a31 2e31 2061 6464 6564 206d 6f72  ...1.1 added mor
-000039c0: 6520 7465 6d70 6c61 7465 7320 746f 206f  e templates to o
-000039d0: 7665 7272 6964 6520 6561 7369 6c79 0d0a  verride easily..
-000039e0: 0d0a 312e 3220 6669 7865 6420 6275 6720  ..1.2 fixed bug 
-000039f0: 696e 2070 7970 6920 6469 7374 726f 206e  in pypi distro n
-00003a00: 6f74 2069 6e63 6c75 6469 6e67 2066 6171  ot including faq
-00003a10: 2061 7070 0d0a 0d0a 312e 3320 6669 7865   app....1.3 fixe
-00003a20: 6420 6275 6720 7768 6572 6520 6120 736c  d bug where a sl
-00003a30: 7567 206d 7573 7420 6265 2066 696c 6c65  ug must be fille
-00003a40: 6420 6f75 7420 696e 2061 646d 696e 2065  d out in admin e
-00003a50: 7665 6e20 7468 6f75 6768 2073 6c75 6720  ven though slug 
-00003a60: 6765 7473 2061 7574 6f20 6765 6e65 7261  gets auto genera
-00003a70: 7465 6420 746f 2073 6176 6520 666f 7220  ted to save for 
-00003a80: 7175 6573 7469 6f6e 732c 2061 6e73 7765  questions, answe
-00003a90: 7273 2c20 616e 6420 6361 7465 676f 7269  rs, and categori
-00003aa0: 6573 2e20 6d61 6465 2071 7565 7374 696f  es. made questio
-00003ab0: 6e73 2c20 616e 7377 6572 732c 2063 6174  ns, answers, cat
-00003ac0: 6567 6f72 6965 7320 736c 7567 7320 7265  egories slugs re
-00003ad0: 6164 6f6e 6c79 2069 6e20 6164 6d69 6e0d  adonly in admin.
-00003ae0: 0a0d 0a31 2e34 2061 6464 6564 2075 6e69  ...1.4 added uni
-00003af0: 636f 6465 206f 7074 696f 6e20 746f 2061  code option to a
-00003b00: 6464 2075 6e69 636f 6465 2073 6c75 6773  dd unicode slugs
-00003b10: 0d0a 0d0a 312e 3520 6164 6465 6420 6c6f  ....1.5 added lo
-00003b20: 6769 6e5f 7265 7175 6972 6564 2073 6574  gin_required set
-00003b30: 7469 6e67 2074 6f20 616c 6c6f 7720 6661  ting to allow fa
-00003b40: 7120 6170 7020 746f 2062 6520 6176 6169  q app to be avai
-00003b50: 6c61 626c 6520 746f 206f 6e6c 7920 6c6f  lable to only lo
-00003b60: 6767 6564 2069 6e20 7573 6572 730d 0a0d  gged in users...
-00003b70: 0a31 2e36 2066 6978 6564 2062 7567 2077  .1.6 fixed bug w
-00003b80: 6865 7265 206e 6f5f 6361 7465 676f 7279  here no_category
-00003b90: 5f64 6573 6372 6970 7469 6f6e 2064 6964  _description did
-00003ba0: 206e 6f74 2064 6f20 7265 6d6f 7665 2074   not do remove t
-00003bb0: 6865 2063 6174 6567 6f72 7920 6465 7363  he category desc
-00003bc0: 7269 7074 696f 6e20 696e 2074 6865 2061  ription in the a
-00003bd0: 646d 696e 0d0a 0d0a 312e 3720 6164 6465  dmin....1.7 adde
-00003be0: 6420 7375 7070 6f72 7420 666f 7220 646a  d support for dj
-00003bf0: 616e 676f 2035 2e30 0d0a                 ango 5.0..
+00000000: 2320 646a 616e 676f 2d65 6173 792d 6661  # django-easy-fa
+00000010: 710a 0a64 6a61 6e67 6f2d 6561 7379 2d66  q..django-easy-f
+00000020: 6171 2069 7320 6120 446a 616e 676f 2061  aq is a Django a
+00000030: 7070 2074 6f20 616c 6c6f 7720 666f 7220  pp to allow for 
+00000040: 6120 7369 6d70 6c65 2079 6574 2066 6561  a simple yet fea
+00000050: 7475 7265 2072 6963 6820 6661 7120 6170  ture rich faq ap
+00000060: 702e 2077 6974 6820 6361 7465 676f 7269  p. with categori
+00000070: 6573 2c20 636f 6d6d 656e 7469 6e67 2076  es, commenting v
+00000080: 6f74 696e 6720 6f66 2071 7565 7374 696f  oting of questio
+00000090: 6e73 2061 6e64 2061 6e73 7765 7273 2061  ns and answers a
+000000a0: 6c6c 2061 7320 616e 206f 7074 696f 6e61  ll as an optiona
+000000b0: 6c20 7061 7274 206f 6620 7468 6520 6170  l part of the ap
+000000c0: 702e 2054 6f20 7365 6520 7363 7265 656e  p. To see screen
+000000d0: 7368 6f74 7320 6f66 2077 6861 7420 7468  shots of what th
+000000e0: 6973 2064 6a61 6e67 6f2d 6561 7379 2d66  is django-easy-f
+000000f0: 6171 2063 6f75 6c64 206c 6f6f 6b20 6c69  aq could look li
+00000100: 6b65 2077 6974 6820 626f 6f74 7374 7261  ke with bootstra
+00000110: 7020 3520 7374 796c 696e 6720 5b63 6c69  p 5 styling [cli
+00000120: 636b 2068 6572 655d 2864 656d 6f2f 6465  ck here](demo/de
+00000130: 6d6f 2e6d 6429 2e0a 0a0a 2323 2051 7569  mo.md)....## Qui
+00000140: 636b 2073 7461 7274 0a0a 312e 2070 6970  ck start..1. pip
+00000150: 2069 6e73 7461 6c6c 3a0a 0a20 2020 2060   install:..    `
+00000160: 7069 7020 696e 7374 616c 6c20 646a 616e  pip install djan
+00000170: 676f 2d65 6173 792d 6661 7160 0a0a 322e  go-easy-faq`..2.
+00000180: 2041 6464 2022 6661 7122 2074 6f20 796f   Add "faq" to yo
+00000190: 7572 2049 4e53 5441 4c4c 4544 5f41 5050  ur INSTALLED_APP
+000001a0: 5320 7365 7474 696e 6720 6c69 6b65 2074  S setting like t
+000001b0: 6869 733a 0a0a 2020 2020 6060 6070 7974  his:..    ```pyt
+000001c0: 686f 6e0a 2020 2020 494e 5354 414c 4c45  hon.    INSTALLE
+000001d0: 445f 4150 5053 203d 205b 0a20 2020 2020  D_APPS = [.     
+000001e0: 2020 202e 2e2e 0a20 2020 2020 2020 2027     ....        '
+000001f0: 6661 7127 2c5d 0a20 2020 2060 6060 0a0a  faq',].    ```..
+00000200: 332e 2049 6e63 6c75 6465 2074 6865 2065  3. Include the e
+00000210: 6173 792d 6661 7120 5552 4c63 6f6e 6620  asy-faq URLconf 
+00000220: 696e 2079 6f75 7220 7072 6f6a 6563 7420  in your project 
+00000230: 7572 6c73 2e70 7920 6c69 6b65 2074 6869  urls.py like thi
+00000240: 733a 3a0a 0a20 2020 2060 6060 7079 7468  s::..    ```pyth
+00000250: 6f6e 0a20 2020 2023 e280 a60a 2020 2020  on.    #....    
+00000260: 7061 7468 2827 6661 712f 272c 2069 6e63  path('faq/', inc
+00000270: 6c75 6465 2827 6661 712e 7572 6c73 2729  lude('faq.urls')
+00000280: 292c 0a20 2020 2023 e280 a60a 2020 2020  ),.    #....    
+00000290: 6060 600a 0a34 2e20 4164 6420 6046 4151  ```..4. Add `FAQ
+000002a0: 5f53 4554 5449 4e47 5320 3d20 5b5d 6020  _SETTINGS = []` 
+000002b0: 746f 2079 6f75 7220 6073 6574 7469 6e67  to your `setting
+000002c0: 732e 7079 600a 352e 2052 756e 2060 6070  s.py`.5. Run ``p
+000002d0: 7974 686f 6e20 6d61 6e61 6765 2e70 7920  ython manage.py 
+000002e0: 6d61 6b65 6d69 6772 6174 696f 6e73 6060  makemigrations``
+000002f0: 2074 6f20 6372 6561 7465 2074 6865 2066   to create the f
+00000300: 6171 206d 6f64 656c 7320 6d69 6772 6174  aq models migrat
+00000310: 696f 6e73 2e0a 362e 2052 756e 2060 6070  ions..6. Run ``p
+00000320: 7974 686f 6e20 6d61 6e61 6765 2e70 7920  ython manage.py 
+00000330: 6d69 6772 6174 6560 6020 746f 2063 7265  migrate`` to cre
+00000340: 6174 6520 7468 6520 6661 7120 6d6f 6465  ate the faq mode
+00000350: 6c73 2e0a 0a37 2e20 5374 6172 7420 7468  ls...7. Start th
+00000360: 6520 6465 7665 6c6f 706d 656e 7420 7365  e development se
+00000370: 7276 6572 2061 6e64 2076 6973 6974 2068  rver and visit h
+00000380: 7474 703a 2f2f 3132 372e 302e 302e 313a  ttp://127.0.0.1:
+00000390: 3830 3030 2f61 646d 696e 2f0a 2020 2074  8000/admin/.   t
+000003a0: 6f20 6372 6561 7465 2061 2063 6174 6567  o create a categ
+000003b0: 6f72 7920 2879 6f75 276c 6c20 6e65 6564  ory (you'll need
+000003c0: 2074 6865 2041 646d 696e 2061 7070 2065   the Admin app e
+000003d0: 6e61 626c 6564 292e 2863 6174 6567 6f72  nabled).(categor
+000003e0: 6965 7320 7061 7274 206f 6620 7468 6520  ies part of the 
+000003f0: 6170 7020 6361 6e20 6265 2064 6973 6162  app can be disab
+00000400: 6c65 6429 0a0a 382e 2056 6973 6974 2068  led)..8. Visit h
+00000410: 7474 703a 2f2f 3132 372e 302e 302e 313a  ttp://127.0.0.1:
+00000420: 3830 3030 2f66 6171 2f20 746f 2073 6565  8000/faq/ to see
+00000430: 2074 6865 2063 6174 6567 6f72 6965 732e   the categories.
+00000440: 0a0a 2323 2053 6574 7469 6e67 730a 0a79  ..## Settings..y
+00000450: 6f75 2063 616e 2063 6861 6e67 6520 6d6f  ou can change mo
+00000460: 7374 2074 6869 6e67 7320 696e 2073 6574  st things in set
+00000470: 7469 6e67 7320 6265 6c6f 7720 6973 2061  tings below is a
+00000480: 206c 6973 7420 6f66 2061 6c6c 2073 6574   list of all set
+00000490: 7469 6e67 730a 6164 6420 616e 7920 6f72  tings.add any or
+000004a0: 2061 6c6c 2074 6f20 6368 616e 6765 2074   all to change t
+000004b0: 6f20 6465 7369 7265 6420 6265 6861 7669  o desired behavi
+000004c0: 6f72 3a3a 0a0a 0a20 2020 2046 4151 5f53  or::...    FAQ_S
+000004d0: 4554 5449 4e47 5320 3d20 5b27 796f 7572  ETTINGS = ['your
+000004e0: 5f73 6574 7469 6e67 735f 6865 7265 272c  _settings_here',
+000004f0: 5d0a 0a0a 312e 206e 6f5f 6361 7465 676f  ]...1. no_catego
+00000500: 7279 5f64 6573 6372 6970 7469 6f6e 2020  ry_description  
+00000510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000520: 2d20 6164 6420 6966 2075 7369 6e67 2063  - add if using c
+00000530: 6174 6567 6f72 6965 7320 6275 7420 646f  ategories but do
+00000540: 6e27 7420 7761 6e74 2064 6573 6372 6970  n't want descrip
+00000550: 7469 6f6e 7320 666f 7220 7468 656d 0a32  tions for them.2
+00000560: 2e20 6e6f 5f63 6174 6567 6f72 7920 2020  . no_category   
+00000570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000580: 2020 2020 2020 2020 2020 202d 2061 6464             - add
+00000590: 2069 6620 646f 6e27 7420 7761 6e74 2074   if don't want t
+000005a0: 6f20 7573 6520 6361 7465 676f 7269 6573  o use categories
+000005b0: 0a33 2e20 6c6f 6767 6564 5f69 6e5f 7573  .3. logged_in_us
+000005c0: 6572 735f 6361 6e5f 6164 645f 7175 6573  ers_can_add_ques
+000005d0: 7469 6f6e 2020 2020 2020 2020 202d 2061  tion         - a
+000005e0: 6464 2069 6620 796f 7520 7761 6e74 2061  dd if you want a
+000005f0: 6e79 206c 6f67 6765 6420 696e 2075 7365  ny logged in use
+00000600: 7220 746f 2062 6520 6162 6c65 2074 6f20  r to be able to 
+00000610: 6173 6b20 6120 7175 6573 7469 6f6e 0a34  ask a question.4
+00000620: 2e20 6c6f 6767 6564 5f69 6e5f 7573 6572  . logged_in_user
+00000630: 735f 6361 6e5f 616e 7377 6572 5f71 7565  s_can_answer_que
+00000640: 7374 696f 6e20 2020 2020 202d 2061 6464  stion      - add
+00000650: 2069 6620 796f 7520 7761 6e74 2061 6e79   if you want any
+00000660: 206c 6f67 6765 6420 696e 2075 7365 7220   logged in user 
+00000670: 746f 2062 6520 6162 6c65 2074 6f20 616e  to be able to an
+00000680: 7377 6572 2061 2071 7565 7374 696f 6e0a  swer a question.
+00000690: 352e 2061 6c6c 6f77 5f6d 756c 7469 706c  5. allow_multipl
+000006a0: 655f 616e 7377 6572 7320 2020 2020 2020  e_answers       
+000006b0: 2020 2020 2020 2020 2020 2020 2d20 6164              - ad
+000006c0: 6420 6966 2079 6f75 2077 616e 7420 6120  d if you want a 
+000006d0: 7175 6573 7469 6f6e 2074 6f20 6265 2061  question to be a
+000006e0: 626c 6520 746f 2062 6520 616e 7377 6572  ble to be answer
+000006f0: 6564 206d 756c 7469 706c 6520 7469 6d65  ed multiple time
+00000700: 730a 362e 206e 6f5f 636f 6d6d 656e 7473  s.6. no_comments
+00000710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000720: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
+00000730: 6164 6420 6966 2064 6f6e 2774 2077 616e  add if don't wan
+00000740: 7420 746f 2075 7365 2063 6f6d 6d65 6e74  t to use comment
+00000750: 730a 372e 2061 6e6f 6e79 6d6f 7573 5f75  s.7. anonymous_u
+00000760: 7365 725f 6361 6e5f 636f 6d6d 656e 7420  ser_can_comment 
+00000770: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
+00000780: 6164 6420 6966 2079 6f75 2077 616e 7420  add if you want 
+00000790: 616e 7920 7573 6572 2074 6f20 6265 2061  any user to be a
+000007a0: 626c 6520 746f 2063 6f6d 6d65 6e74 2069  ble to comment i
+000007b0: 6e63 6c75 6469 6e67 2061 6e6f 6e79 6d6f  ncluding anonymo
+000007c0: 7573 2075 7365 7273 0a38 2e20 7669 6577  us users.8. view
+000007d0: 5f6f 6e6c 795f 636f 6d6d 656e 7473 2020  _only_comments  
+000007e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000007f0: 2020 2020 202d 2061 6464 2069 6620 796f       - add if yo
+00000800: 7520 7761 6e74 2075 7365 7273 2074 6f20  u want users to 
+00000810: 7365 6520 706f 7374 6564 2063 6f6d 6d65  see posted comme
+00000820: 6e74 7320 6275 7420 6e6f 7420 6265 2061  nts but not be a
+00000830: 626c 6520 746f 2061 6464 2061 6e79 206d  ble to add any m
+00000840: 6f72 650a 392e 206e 6f5f 766f 7465 7320  ore.9. no_votes 
+00000850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000870: 2d20 6164 6420 6966 2064 6f6e 2774 2077  - add if don't w
+00000880: 616e 7420 616e 7920 766f 7469 6e67 2066  ant any voting f
+00000890: 6f72 2075 7365 6675 6c20 7175 6573 7469  or useful questi
+000008a0: 6f6e 7320 6f72 2061 6e73 7765 7273 0a31  ons or answers.1
+000008b0: 302e 206e 6f5f 616e 7377 6572 5f76 6f74  0. no_answer_vot
+000008c0: 6573 2020 2020 2020 2020 2020 2020 2020  es              
+000008d0: 2020 2020 2020 2020 2020 202d 2061 6464             - add
+000008e0: 2069 6620 6f6e 6c79 2077 616e 7420 7175   if only want qu
+000008f0: 6573 7469 6f6e 2076 6f74 696e 670a 3131  estion voting.11
+00000900: 2e20 6e6f 5f71 7565 7374 696f 6e5f 766f  . no_question_vo
+00000910: 7465 7320 2020 2020 2020 2020 2020 2020  tes             
+00000920: 2020 2020 2020 2020 2020 2d20 6164 6420            - add 
+00000930: 6966 206f 6e6c 7920 7761 6e74 2061 6e73  if only want ans
+00000940: 7765 7220 766f 7469 6e67 0a31 322e 2061  wer voting.12. a
+00000950: 6c6c 6f77 5f75 6e69 636f 6465 2020 2020  llow_unicode    
+00000960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000970: 2020 2020 2020 202d 2061 6464 2069 6620         - add if 
+00000980: 796f 7520 7761 6e74 2074 6f20 616c 6c6f  you want to allo
+00000990: 7720 756e 6963 6f64 6520 736c 7567 730a  w unicode slugs.
+000009a0: 3133 2e20 6c6f 6769 6e5f 7265 7175 6972  13. login_requir
+000009b0: 6564 2020 2020 2020 2020 2020 2020 2020  ed              
+000009c0: 2020 2020 2020 2020 2020 2020 2d20 6164              - ad
+000009d0: 6420 6966 2079 6f75 2077 616e 7420 746f  d if you want to
+000009e0: 206f 6e6c 7920 6c65 7420 6c6f 6767 6564   only let logged
+000009f0: 2069 6e20 7573 6572 7320 7365 6520 4641   in users see FA
+00000a00: 5127 730a 3134 2e20 7269 6368 5f74 6578  Q's.14. rich_tex
+00000a10: 745f 616e 7377 6572 7320 2020 2020 2020  t_answers       
+00000a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a30: 2d20 6164 6420 6966 2079 6f75 2077 616e  - add if you wan
+00000a40: 7420 746f 2075 7365 2072 6963 6820 7465  t to use rich te
+00000a50: 7874 2066 6f72 2061 6e73 7765 7273 2e20  xt for answers. 
+00000a60: 5468 6973 2072 6571 7569 7265 7320 7468  This requires th
+00000a70: 6520 646a 616e 676f 2d74 696e 796d 6365  e django-tinymce
+00000a80: 2070 6163 6b61 6765 2074 6f20 6265 2069   package to be i
+00000a90: 6e73 7461 6c6c 6564 0a0a 2323 2054 656d  nstalled..## Tem
+00000aa0: 706c 6174 6573 0a0a 616c 6c20 6f66 2074  plates..all of t
+00000ab0: 6865 2074 656d 706c 6174 6573 2061 7265  he templates are
+00000ac0: 206d 6561 6e74 2074 6f20 6265 206f 7665   meant to be ove
+00000ad0: 7277 7269 7474 656e 0a74 6f20 6f76 6572  rwritten.to over
+00000ae0: 7772 6974 6520 7468 656d 2063 7265 6174  write them creat
+00000af0: 6520 6120 6661 7120 6469 7265 6374 6f72  e a faq director
+00000b00: 7920 696e 7369 6465 206f 6620 7468 6520  y inside of the 
+00000b10: 7465 6d70 6c61 7465 7320 6469 7265 6374  templates direct
+00000b20: 6f72 7920 616e 6420 6164 6420 6120 6874  ory and add a ht
+00000b30: 6d6c 2066 696c 6520 7769 7468 2074 6865  ml file with the
+00000b40: 2073 616d 6520 6e61 6d65 2074 6f20 6974   same name to it
+00000b50: 0a0a 6966 2074 6869 7320 646f 6573 6e27  ..if this doesn'
+00000b60: 7420 776f 726b 206d 616b 6520 7375 7265  t work make sure
+00000b70: 2074 6861 7420 7468 6520 7465 6d70 6c61   that the templa
+00000b80: 7465 7320 7365 7474 696e 6720 6861 7320  tes setting has 
+00000b90: 2744 4952 5327 3a20 5b27 7465 6d70 6c61  'DIRS': ['templa
+00000ba0: 7465 7327 5d2c 2069 6e20 6974 3a3a 0a0a  tes'], in it::..
+00000bb0: 2020 2020 5445 4d50 4c41 5445 5320 3d20      TEMPLATES = 
+00000bc0: 5b0a 2020 2020 2020 2020 7b0a 2020 2020  [.        {.    
+00000bd0: 2020 2020 2020 2020 2e2e 2e0a 2020 2020          ....    
+00000be0: 2020 2020 2020 2020 2744 4952 5327 3a20          'DIRS': 
+00000bf0: 5b27 7465 6d70 6c61 7465 7327 5d2c 0a20  ['templates'],. 
+00000c00: 2020 2020 2020 2020 2020 202e 2e2e 0a20             .... 
+00000c10: 2020 2020 2020 207d 2c0a 2020 2020 5d0a         },.    ].
+00000c20: 0a68 6572 6520 6973 2061 206c 6973 7420  .here is a list 
+00000c30: 6f66 2074 656d 706c 6174 6573 2061 6e64  of templates and
+00000c40: 2074 6865 7265 2064 6566 6175 6c74 2074   there default t
+00000c50: 656d 706c 6174 6520 2079 6f75 2063 616e  emplate  you can
+00000c60: 206f 7665 7277 7269 7465 0a0a 312e 2063   overwrite..1. c
+00000c70: 6174 6567 6f72 6965 735f 6c69 7374 2e68  ategories_list.h
+00000c80: 746d 6c20 2d20 6661 7120 6d61 696e 2076  tml - faq main v
+00000c90: 6965 7720 6966 2075 7369 6e67 2063 6174  iew if using cat
+00000ca0: 6567 6f72 6965 733a 3a0a 0a0a 2020 2020  egories::...    
+00000cb0: 2020 2020 3c68 313e 7365 6c65 6374 2061      <h1>select a
+00000cc0: 2046 4151 2063 6174 6567 6f72 793c 2f68   FAQ category</h
+00000cd0: 313e 0a20 2020 2020 2020 207b 2520 666f  1>.        {% fo
+00000ce0: 7220 6361 7465 676f 7279 2069 6e20 6361  r category in ca
+00000cf0: 7465 676f 7269 6573 2025 7d0a 2020 2020  tegories %}.    
+00000d00: 2020 2020 2020 2020 3c68 333e 3c61 2068          <h3><a h
+00000d10: 7265 663d 227b 2520 7572 6c20 2766 6171  ref="{% url 'faq
+00000d20: 3a63 6174 6567 6f72 795f 6465 7461 696c  :category_detail
+00000d30: 2720 6361 7465 676f 7279 2e73 6c75 6720  ' category.slug 
+00000d40: 257d 223e 7b7b 6361 7465 676f 7279 2e6e  %}">{{category.n
+00000d50: 616d 657d 7d3c 2f61 3e3c 2f68 333e 0a20  ame}}</a></h3>. 
+00000d60: 2020 2020 2020 2020 2020 207b 2520 6966             {% if
+00000d70: 2063 6174 6567 6f72 792e 6465 7363 7269   category.descri
+00000d80: 7074 696f 6e20 257d 0a20 2020 2020 2020  ption %}.       
+00000d90: 2020 2020 2020 2020 203c 703e 7b7b 6361           <p>{{ca
+00000da0: 7465 676f 7279 2e64 6573 6372 6970 7469  tegory.descripti
+00000db0: 6f6e 7d7d 3c2f 703e 0a20 2020 2020 2020  on}}</p>.       
+00000dc0: 2020 2020 207b 2520 656e 6469 6620 257d       {% endif %}
+00000dd0: 0a20 2020 2020 2020 2020 2020 203c 6872  .            <hr
+00000de0: 3e0a 2020 2020 2020 2020 7b25 2065 6e64  >.        {% end
+00000df0: 666f 7220 257d 0a0a 0a32 2e20 6361 7465  for %}...2. cate
+00000e00: 676f 7279 5f64 6574 6169 6c2e 6874 6d6c  gory_detail.html
+00000e10: 202d 2066 6171 2063 6174 6567 6f72 7920   - faq category 
+00000e20: 6465 7461 696c 2076 6965 7720 6966 2075  detail view if u
+00000e30: 7369 6e67 2063 6174 6567 6f72 6965 733a  sing categories:
+00000e40: 3a0a 0a0a 2020 2020 2020 2020 3c68 313e  :...        <h1>
+00000e50: 6368 6f6f 7365 2061 2046 4151 2051 7565  choose a FAQ Que
+00000e60: 7374 696f 6e3c 2f68 313e 0a20 2020 2020  stion</h1>.     
+00000e70: 2020 203c 6832 3e7b 7b63 6174 6567 6f72     <h2>{{categor
+00000e80: 797d 7d3c 2f68 323e 0a20 2020 2020 2020  y}}</h2>.       
+00000e90: 207b 2520 6966 2063 6174 6567 6f72 792e   {% if category.
+00000ea0: 6465 7363 7269 7074 696f 6e20 257d 0a20  description %}. 
+00000eb0: 2020 2020 2020 203c 703e 7b7b 6361 7465         <p>{{cate
+00000ec0: 676f 7279 2e64 6573 6372 6970 7469 6f6e  gory.description
+00000ed0: 7d7d 3c2f 703e 0a20 2020 2020 2020 207b  }}</p>.        {
+00000ee0: 2520 656e 6469 6620 257d 0a20 2020 2020  % endif %}.     
+00000ef0: 2020 203c 6872 3e0a 2020 2020 2020 2020     <hr>.        
+00000f00: 7b25 2066 6f72 2071 7565 7374 696f 6e20  {% for question 
+00000f10: 696e 2063 6174 6567 6f72 792e 7175 6573  in category.ques
+00000f20: 7469 6f6e 5f73 6574 2e61 6c6c 2025 7d0a  tion_set.all %}.
+00000f30: 2020 2020 2020 2020 2020 2020 3c68 333e              <h3>
+00000f40: 3c61 2068 7265 663d 227b 2520 7572 6c20  <a href="{% url 
+00000f50: 2766 6171 3a71 7565 7374 696f 6e5f 6465  'faq:question_de
+00000f60: 7461 696c 2720 6361 7465 676f 7279 2e73  tail' category.s
+00000f70: 6c75 6720 7175 6573 7469 6f6e 2e73 6c75  lug question.slu
+00000f80: 6720 257d 223e 7b7b 7175 6573 7469 6f6e  g %}">{{question
+00000f90: 2e71 7565 7374 696f 6e7d 7d3c 2f61 3e3c  .question}}</a><
+00000fa0: 2f68 333e 0a20 2020 2020 2020 207b 2520  /h3>.        {% 
+00000fb0: 656e 6466 6f72 2025 7d0a 2020 2020 2020  endfor %}.      
+00000fc0: 2020 3c68 723e 0a20 2020 2020 2020 203c    <hr>.        <
+00000fd0: 6120 6872 6566 3d22 7b25 2075 726c 2027  a href="{% url '
+00000fe0: 6661 713a 696e 6465 785f 7669 6577 2720  faq:index_view' 
+00000ff0: 257d 223e 6261 636b 3c2f 613e 0a20 2020  %}">back</a>.   
+00001000: 2020 2020 207b 2520 6966 2063 616e 5f61       {% if can_a
+00001010: 6464 5f71 7565 7374 696f 6e20 257d 0a20  dd_question %}. 
+00001020: 2020 2020 2020 2020 2020 203c 6120 6872             <a hr
+00001030: 6566 3d22 7b25 2075 726c 2027 6661 713a  ef="{% url 'faq:
+00001040: 6164 645f 7175 6573 7469 6f6e 2720 6361  add_question' ca
+00001050: 7465 676f 7279 2e73 6c75 6720 257d 223e  tegory.slug %}">
+00001060: 6164 6420 7175 6573 7469 6f6e 3c2f 613e  add question</a>
+00001070: 0a20 2020 2020 2020 207b 2520 656e 6469  .        {% endi
+00001080: 6620 257d 0a0a 0a33 2e20 7175 6573 7469  f %}...3. questi
+00001090: 6f6e 735f 6c69 7374 2e68 746d 6c20 2d20  ons_list.html - 
+000010a0: 6c69 7374 7320 616c 6c20 7175 6573 7469  lists all questi
+000010b0: 6f6e 7320 6966 206e 6f74 2075 7369 6e67  ons if not using
+000010c0: 2063 6174 6567 6f72 6965 733a 3a0a 0a0a   categories::...
+000010d0: 2020 2020 2020 2020 3c68 313e 6368 6f6f          <h1>choo
+000010e0: 7365 2061 2046 4151 2051 7565 7374 696f  se a FAQ Questio
+000010f0: 6e3c 2f68 313e 0a20 2020 2020 2020 207b  n</h1>.        {
+00001100: 2520 666f 7220 7175 6573 7469 6f6e 2069  % for question i
+00001110: 6e20 7175 6573 7469 6f6e 7320 257d 0a20  n questions %}. 
+00001120: 2020 2020 2020 2020 2020 203c 6833 3e3c             <h3><
+00001130: 6120 6872 6566 3d22 7b25 2075 726c 2027  a href="{% url '
+00001140: 6661 713a 7175 6573 7469 6f6e 5f64 6574  faq:question_det
+00001150: 6169 6c27 2071 7565 7374 696f 6e2e 736c  ail' question.sl
+00001160: 7567 2025 7d22 3e7b 7b71 7565 7374 696f  ug %}">{{questio
+00001170: 6e2e 7175 6573 7469 6f6e 7d7d 3c2f 613e  n.question}}</a>
+00001180: 3c2f 6833 3e0a 2020 2020 2020 2020 7b25  </h3>.        {%
+00001190: 2065 6e64 666f 7220 257d 0a20 2020 200a   endfor %}.    .
+000011a0: 2020 2020 2020 2020 7b25 2069 6620 6361          {% if ca
+000011b0: 6e5f 6164 645f 7175 6573 7469 6f6e 2025  n_add_question %
+000011c0: 7d0a 2020 2020 2020 2020 2020 2020 3c68  }.            <h
+000011d0: 723e 0a20 2020 2020 2020 2020 2020 203c  r>.            <
+000011e0: 6120 6872 6566 3d22 7b25 2075 726c 2027  a href="{% url '
+000011f0: 6661 713a 6164 645f 7175 6573 7469 6f6e  faq:add_question
+00001200: 2720 257d 223e 6164 6420 7175 6573 7469  ' %}">add questi
+00001210: 6f6e 3c2f 613e 0a20 2020 2020 2020 207b  on</a>.        {
+00001220: 2520 656e 6469 6620 257d 0a0a 0a34 2e20  % endif %}...4. 
+00001230: 7175 6573 7469 6f6e 5f64 6574 6169 6c2e  question_detail.
+00001240: 6874 6d6c 202d 2074 6865 2071 7565 7374  html - the quest
+00001250: 696f 6e20 6465 7461 696c 2070 6167 653a  ion detail page:
+00001260: 3a0a 0a0a 2020 2020 2020 2020 7b25 2065  :...        {% e
+00001270: 7874 656e 6473 2027 6661 712f 7175 6573  xtends 'faq/ques
+00001280: 7469 6f6e 5f62 6173 652e 6874 6d6c 2720  tion_base.html' 
+00001290: 257d 0a20 2020 200a 2020 2020 2020 2020  %}.    .        
+000012a0: 7b25 2062 6c6f 636b 2071 7565 7374 696f  {% block questio
+000012b0: 6e5f 636f 6e74 656e 7420 257d 0a20 2020  n_content %}.   
+000012c0: 2020 2020 207b 2520 6966 2061 6c6c 6f77       {% if allow
+000012d0: 5f6d 756c 7469 706c 655f 616e 7377 6572  _multiple_answer
+000012e0: 7320 257d 0a20 2020 2020 2020 203c 6833  s %}.        <h3
+000012f0: 3e61 6e73 7765 7273 3c2f 6833 3e0a 2020  >answers</h3>.  
+00001300: 2020 2020 2020 3c75 6c3e 0a20 2020 2020        <ul>.     
+00001310: 2020 2020 2020 207b 2520 666f 7220 616e         {% for an
+00001320: 7377 6572 2069 6e20 7175 6573 7469 6f6e  swer in question
+00001330: 2e61 6e73 7765 725f 7365 742e 616c 6c20  .answer_set.all 
+00001340: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+00001350: 2020 203c 6c69 3e3c 623e 7b7b 616e 7377     <li><b>{{answ
+00001360: 6572 2e61 6e73 7765 727d 7d3c 2f62 3e0a  er.answer}}</b>.
+00001370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001380: 2020 2020 7b25 2069 6620 6361 6e5f 766f      {% if can_vo
+00001390: 7465 5f61 6e73 7765 7220 257d 0a20 2020  te_answer %}.   
+000013a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013b0: 2020 7c20 666f 756e 6420 7468 6973 2061    | found this a
+000013c0: 6e73 7765 7220 6865 6c70 6675 6c3f 0a20  nswer helpful?. 
+000013d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013e0: 2020 203c 666f 726d 2073 7479 6c65 3d22     <form style="
+000013f0: 6469 7370 6c61 793a 2069 6e6c 696e 653b  display: inline;
+00001400: 2220 6163 7469 6f6e 3d22 7b25 2069 6620  " action="{% if 
+00001410: 6361 7465 676f 7279 5f65 6e61 626c 6564  category_enabled
+00001420: 2025 7d7b 2520 7572 6c20 2766 6171 3a76   %}{% url 'faq:v
+00001430: 6f74 655f 616e 7377 6572 2720 7175 6573  ote_answer' ques
+00001440: 7469 6f6e 2e63 6174 6567 6f72 792e 736c  tion.category.sl
+00001450: 7567 2071 7565 7374 696f 6e2e 736c 7567  ug question.slug
+00001460: 2061 6e73 7765 722e 736c 7567 2025 7d7b   answer.slug %}{
+00001470: 2520 656c 7365 2025 7d7b 2520 7572 6c20  % else %}{% url 
+00001480: 2766 6171 3a76 6f74 655f 616e 7377 6572  'faq:vote_answer
+00001490: 2720 7175 6573 7469 6f6e 2e73 6c75 6720  ' question.slug 
+000014a0: 616e 7377 6572 2e73 6c75 6720 257d 7b25  answer.slug %}{%
+000014b0: 2065 6e64 6966 2025 7d22 206d 6574 686f   endif %}" metho
+000014c0: 643d 2270 6f73 7422 3e0a 2020 2020 2020  d="post">.      
+000014d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014e0: 2020 7b25 2063 7372 665f 746f 6b65 6e20    {% csrf_token 
+000014f0: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+00001500: 2020 2020 2020 2020 2020 203c 696e 7075             <inpu
+00001510: 7420 7479 7065 3d22 6869 6464 656e 2220  t type="hidden" 
+00001520: 7661 6c75 653d 5472 7565 206e 616d 653d  value=True name=
+00001530: 2276 6f74 6522 3e0a 2020 2020 2020 2020  "vote">.        
+00001540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001550: 3c62 7574 746f 6e20 7479 7065 3d22 7375  <button type="su
+00001560: 626d 6974 223e 7965 7328 7b7b 616e 7377  bmit">yes({{answ
+00001570: 6572 2e68 656c 7066 756c 7d7d 293c 2f62  er.helpful}})</b
+00001580: 7574 746f 6e3e 0a20 2020 2020 2020 2020  utton>.         
+00001590: 2020 2020 2020 2020 2020 203c 2f66 6f72             </for
+000015a0: 6d3e 0a20 2020 2020 2020 2020 2020 2020  m>.             
+000015b0: 2020 2020 2020 203c 666f 726d 2073 7479         <form sty
+000015c0: 6c65 3d22 6469 7370 6c61 793a 2069 6e6c  le="display: inl
+000015d0: 696e 653b 2220 6163 7469 6f6e 3d22 7b25  ine;" action="{%
+000015e0: 2069 6620 6361 7465 676f 7279 5f65 6e61   if category_ena
+000015f0: 626c 6564 2025 7d7b 2520 7572 6c20 2766  bled %}{% url 'f
+00001600: 6171 3a76 6f74 655f 616e 7377 6572 2720  aq:vote_answer' 
+00001610: 7175 6573 7469 6f6e 2e63 6174 6567 6f72  question.categor
+00001620: 792e 736c 7567 2071 7565 7374 696f 6e2e  y.slug question.
+00001630: 736c 7567 2061 6e73 7765 722e 736c 7567  slug answer.slug
+00001640: 2025 7d7b 2520 656c 7365 2025 7d7b 2520   %}{% else %}{% 
+00001650: 7572 6c20 2766 6171 3a76 6f74 655f 616e  url 'faq:vote_an
+00001660: 7377 6572 2720 7175 6573 7469 6f6e 2e73  swer' question.s
+00001670: 6c75 6720 616e 7377 6572 2e73 6c75 6720  lug answer.slug 
+00001680: 257d 7b25 2065 6e64 6966 2025 7d22 206d  %}{% endif %}" m
+00001690: 6574 686f 643d 2270 6f73 7422 3e0a 2020  ethod="post">.  
+000016a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000016b0: 2020 2020 2020 7b25 2063 7372 665f 746f        {% csrf_to
+000016c0: 6b65 6e20 257d 0a20 2020 2020 2020 2020  ken %}.         
+000016d0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000016e0: 696e 7075 7420 7479 7065 3d22 6869 6464  input type="hidd
+000016f0: 656e 2220 7661 6c75 653d 4661 6c73 6520  en" value=False 
+00001700: 6e61 6d65 3d22 766f 7465 223e 0a20 2020  name="vote">.   
+00001710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001720: 2020 2020 203c 6275 7474 6f6e 2074 7970       <button typ
+00001730: 653d 2273 7562 6d69 7422 3e6e 6f28 7b7b  e="submit">no({{
+00001740: 616e 7377 6572 2e6e 6f74 5f68 656c 7066  answer.not_helpf
+00001750: 756c 7d7d 293c 2f62 7574 746f 6e3e 0a20  ul}})</button>. 
+00001760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001770: 2020 203c 2f66 6f72 6d3e 0a20 2020 2020     </form>.     
+00001780: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00001790: 2520 656e 6469 6620 257d 0a20 2020 2020  % endif %}.     
+000017a0: 2020 2020 2020 2020 2020 203c 2f6c 693e             </li>
+000017b0: 0a20 2020 2020 2020 2020 2020 207b 2520  .            {% 
+000017c0: 656e 6466 6f72 2025 7d0a 2020 2020 2020  endfor %}.      
+000017d0: 2020 3c2f 756c 3e0a 2020 2020 0a20 2020    </ul>.    .   
+000017e0: 2020 2020 207b 2520 656c 7365 2025 7d0a       {% else %}.
+000017f0: 2020 2020 2020 2020 2020 2020 7b25 2069              {% i
+00001800: 6620 7175 6573 7469 6f6e 2e61 6e73 7765  f question.answe
+00001810: 725f 7365 742e 6578 6973 7473 2025 7d0a  r_set.exists %}.
+00001820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001830: 3c70 3e61 6e73 7765 723a 3c2f 703e 0a20  <p>answer:</p>. 
+00001840: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00001850: 6833 3e7b 7b71 7565 7374 696f 6e2e 616e  h3>{{question.an
+00001860: 7377 6572 5f73 6574 2e66 6972 7374 2e61  swer_set.first.a
+00001870: 6e73 7765 727d 7d3c 2f68 333e 0a20 2020  nswer}}</h3>.   
+00001880: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
+00001890: 6966 2063 616e 5f76 6f74 655f 616e 7377  if can_vote_answ
+000018a0: 6572 2025 7d0a 2020 2020 2020 2020 2020  er %}.          
+000018b0: 2020 2020 2020 2066 6f75 6e64 2074 6869         found thi
+000018c0: 7320 616e 7377 6572 2068 656c 7066 756c  s answer helpful
+000018d0: 3f0a 2020 2020 2020 2020 2020 2020 2020  ?.              
+000018e0: 2020 3c66 6f72 6d20 7374 796c 653d 2264    <form style="d
+000018f0: 6973 706c 6179 3a20 696e 6c69 6e65 3b22  isplay: inline;"
+00001900: 2061 6374 696f 6e3d 227b 2520 6966 2063   action="{% if c
+00001910: 6174 6567 6f72 795f 656e 6162 6c65 6420  ategory_enabled 
+00001920: 257d 7b25 2075 726c 2027 6661 713a 766f  %}{% url 'faq:vo
+00001930: 7465 5f61 6e73 7765 7227 2071 7565 7374  te_answer' quest
+00001940: 696f 6e2e 6361 7465 676f 7279 2e73 6c75  ion.category.slu
+00001950: 6720 7175 6573 7469 6f6e 2e73 6c75 6720  g question.slug 
+00001960: 7175 6573 7469 6f6e 2e61 6e73 7765 725f  question.answer_
+00001970: 7365 742e 6669 7273 742e 736c 7567 2025  set.first.slug %
+00001980: 7d7b 2520 656c 7365 2025 7d7b 2520 7572  }{% else %}{% ur
+00001990: 6c20 2766 6171 3a76 6f74 655f 616e 7377  l 'faq:vote_answ
+000019a0: 6572 2720 7175 6573 7469 6f6e 2e73 6c75  er' question.slu
+000019b0: 6720 7175 6573 7469 6f6e 2e61 6e73 7765  g question.answe
+000019c0: 725f 7365 742e 6669 7273 742e 736c 7567  r_set.first.slug
+000019d0: 2025 7d7b 2520 656e 6469 6620 257d 2220   %}{% endif %}" 
+000019e0: 6d65 7468 6f64 3d22 706f 7374 223e 0a20  method="post">. 
+000019f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a00: 2020 207b 2520 6373 7266 5f74 6f6b 656e     {% csrf_token
+00001a10: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+00001a20: 2020 2020 2020 2020 3c69 6e70 7574 2074          <input t
+00001a30: 7970 653d 2268 6964 6465 6e22 2076 616c  ype="hidden" val
+00001a40: 7565 3d54 7275 6520 6e61 6d65 3d22 766f  ue=True name="vo
+00001a50: 7465 223e 0a20 2020 2020 2020 2020 2020  te">.           
+00001a60: 2020 2020 2020 2020 203c 6275 7474 6f6e           <button
+00001a70: 2074 7970 653d 2273 7562 6d69 7422 3e79   type="submit">y
+00001a80: 6573 287b 7b71 7565 7374 696f 6e2e 616e  es({{question.an
+00001a90: 7377 6572 5f73 6574 2e66 6972 7374 2e68  swer_set.first.h
+00001aa0: 656c 7066 756c 7d7d 293c 2f62 7574 746f  elpful}})</butto
+00001ab0: 6e3e 0a20 2020 2020 2020 2020 2020 2020  n>.             
+00001ac0: 2020 203c 2f66 6f72 6d3e 0a20 2020 2020     </form>.     
+00001ad0: 2020 2020 2020 2020 2020 203c 666f 726d             <form
+00001ae0: 2073 7479 6c65 3d22 6469 7370 6c61 793a   style="display:
+00001af0: 2069 6e6c 696e 653b 2220 6163 7469 6f6e   inline;" action
+00001b00: 3d22 7b25 2069 6620 6361 7465 676f 7279  ="{% if category
+00001b10: 5f65 6e61 626c 6564 2025 7d7b 2520 7572  _enabled %}{% ur
+00001b20: 6c20 2766 6171 3a76 6f74 655f 616e 7377  l 'faq:vote_answ
+00001b30: 6572 2720 7175 6573 7469 6f6e 2e63 6174  er' question.cat
+00001b40: 6567 6f72 792e 736c 7567 2071 7565 7374  egory.slug quest
+00001b50: 696f 6e2e 736c 7567 2071 7565 7374 696f  ion.slug questio
+00001b60: 6e2e 616e 7377 6572 5f73 6574 2e66 6972  n.answer_set.fir
+00001b70: 7374 2e73 6c75 6720 257d 7b25 2065 6c73  st.slug %}{% els
+00001b80: 6520 257d 7b25 2075 726c 2027 6661 713a  e %}{% url 'faq:
+00001b90: 766f 7465 5f61 6e73 7765 7227 2071 7565  vote_answer' que
+00001ba0: 7374 696f 6e2e 736c 7567 2071 7565 7374  stion.slug quest
+00001bb0: 696f 6e2e 616e 7377 6572 5f73 6574 2e66  ion.answer_set.f
+00001bc0: 6972 7374 2e73 6c75 6720 257d 7b25 2065  irst.slug %}{% e
+00001bd0: 6e64 6966 2025 7d22 206d 6574 686f 643d  ndif %}" method=
+00001be0: 2270 6f73 7422 3e0a 2020 2020 2020 2020  "post">.        
+00001bf0: 2020 2020 2020 2020 2020 2020 7b25 2063              {% c
+00001c00: 7372 665f 746f 6b65 6e20 257d 0a20 2020  srf_token %}.   
+00001c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c20: 203c 696e 7075 7420 7479 7065 3d22 6869   <input type="hi
+00001c30: 6464 656e 2220 7661 6c75 653d 4661 6c73  dden" value=Fals
+00001c40: 6520 6e61 6d65 3d22 766f 7465 223e 0a20  e name="vote">. 
+00001c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c60: 2020 203c 6275 7474 6f6e 2074 7970 653d     <button type=
+00001c70: 2273 7562 6d69 7422 3e6e 6f28 7b7b 7175  "submit">no({{qu
+00001c80: 6573 7469 6f6e 2e61 6e73 7765 725f 7365  estion.answer_se
+00001c90: 742e 6669 7273 742e 6e6f 745f 6865 6c70  t.first.not_help
+00001ca0: 6675 6c7d 7d29 3c2f 6275 7474 6f6e 3e0a  ful}})</button>.
+00001cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001cc0: 3c2f 666f 726d 3e0a 2020 2020 2020 2020  </form>.        
+00001cd0: 2020 2020 2020 2020 7b25 2065 6e64 6966          {% endif
+00001ce0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+00001cf0: 7b25 2065 6c73 6520 257d 0a20 2020 2020  {% else %}.     
+00001d00: 2020 2020 2020 2020 2020 206e 6f20 616e             no an
+00001d10: 7377 6572 7320 7965 740a 2020 2020 2020  swers yet.      
+00001d20: 2020 2020 2020 7b25 2065 6e64 6966 2025        {% endif %
+00001d30: 7d0a 2020 2020 2020 2020 7b25 2065 6e64  }.        {% end
+00001d40: 6966 2025 7d0a 2020 2020 0a20 2020 200a  if %}.    .    .
+00001d50: 2020 2020 2020 2020 7b25 2069 6620 6361          {% if ca
+00001d60: 6e5f 616e 7377 6572 5f71 7565 7374 696f  n_answer_questio
+00001d70: 6e20 257d 0a20 2020 2020 2020 2020 2020  n %}.           
+00001d80: 207b 2520 6966 2063 6174 6567 6f72 795f   {% if category_
+00001d90: 656e 6162 6c65 6420 257d 0a20 2020 2020  enabled %}.     
+00001da0: 2020 2020 2020 2020 2020 203c 6120 6872             <a hr
+00001db0: 6566 3d22 7b25 2075 726c 2027 6661 713a  ef="{% url 'faq:
+00001dc0: 616e 7377 6572 5f71 7565 7374 696f 6e27  answer_question'
+00001dd0: 2071 7565 7374 696f 6e2e 6361 7465 676f   question.catego
+00001de0: 7279 2e73 6c75 6720 7175 6573 7469 6f6e  ry.slug question
+00001df0: 2e73 6c75 6720 257d 223e 616e 7377 6572  .slug %}">answer
+00001e00: 2071 7565 7374 696f 6e3c 2f61 3e0a 2020   question</a>.  
+00001e10: 2020 2020 2020 2020 2020 7b25 2065 6c73            {% els
+00001e20: 6520 257d 0a20 2020 2020 2020 2020 2020  e %}.           
+00001e30: 2020 2020 203c 6120 6872 6566 3d22 7b25       <a href="{%
+00001e40: 2075 726c 2027 6661 713a 616e 7377 6572   url 'faq:answer
+00001e50: 5f71 7565 7374 696f 6e27 2071 7565 7374  _question' quest
+00001e60: 696f 6e2e 736c 7567 2025 7d22 3e61 6e73  ion.slug %}">ans
+00001e70: 7765 7220 7175 6573 7469 6f6e 3c2f 613e  wer question</a>
+00001e80: 0a20 2020 2020 2020 2020 2020 207b 2520  .            {% 
+00001e90: 656e 6469 6620 257d 0a20 2020 2020 2020  endif %}.       
+00001ea0: 207b 2520 656e 6469 6620 257d 0a20 2020   {% endif %}.   
+00001eb0: 2020 2020 203c 6872 3e0a 2020 2020 2020       <hr>.      
+00001ec0: 2020 7b25 2069 6620 636f 6d6d 656e 7473    {% if comments
+00001ed0: 5f61 6c6c 6f77 6564 2025 7d0a 2020 2020  _allowed %}.    
+00001ee0: 2020 2020 2020 2020 7b25 2069 6e63 6c75          {% inclu
+00001ef0: 6465 2027 6661 712f 636f 6d6d 656e 7473  de 'faq/comments
+00001f00: 2e68 746d 6c27 2025 7d0a 2020 2020 2020  .html' %}.      
+00001f10: 2020 7b25 2065 6e64 6966 2025 7d0a 2020    {% endif %}.  
+00001f20: 2020 0a20 2020 2020 2020 207b 2520 656e    .        {% en
+00001f30: 6462 6c6f 636b 2025 7d0a 0a35 2e20 616e  dblock %}..5. an
+00001f40: 7377 6572 5f66 6f72 6d2e 6874 6d6c 202d  swer_form.html -
+00001f50: 2066 6f72 6d20 746f 2061 6464 2061 6e73   form to add ans
+00001f60: 7765 7220 746f 2071 7565 7374 696f 6e3a  wer to question:
+00001f70: 3a0a 0a0a 2020 2020 2020 2020 3c68 313e  :...        <h1>
+00001f80: 416e 7377 6572 2051 7565 7374 696f 6e3c  Answer Question<
+00001f90: 2f68 313e 0a20 2020 2020 2020 203c 6120  /h1>.        <a 
+00001fa0: 6872 6566 3d22 7b7b 7175 6573 7469 6f6e  href="{{question
+00001fb0: 2e67 6574 5f61 6273 6f6c 7574 655f 7572  .get_absolute_ur
+00001fc0: 6c7d 7d22 3e3c 6833 3e7b 7b71 7565 7374  l}}"><h3>{{quest
+00001fd0: 696f 6e2e 7175 6573 7469 6f6e 7d7d 3c2f  ion.question}}</
+00001fe0: 6833 3e3c 2f61 3e0a 2020 2020 2020 2020  h3></a>.        
+00001ff0: 3c66 6f72 6d20 6d65 7468 6f64 3d22 706f  <form method="po
+00002000: 7374 223e 0a20 2020 2020 2020 2020 2020  st">.           
+00002010: 207b 2520 6373 7266 5f74 6f6b 656e 2025   {% csrf_token %
+00002020: 7d0a 2020 2020 2020 2020 2020 2020 7b7b  }.            {{
+00002030: 666f 726d 7d7d 0a20 2020 2020 2020 2020  form}}.         
+00002040: 2020 203c 696e 7075 7420 7479 7065 3d22     <input type="
+00002050: 7375 626d 6974 223e 0a20 2020 2020 2020  submit">.       
+00002060: 203c 2f66 6f72 6d3e 0a0a 362e 2063 6f6d   </form>..6. com
+00002070: 6d65 6e74 5f66 6f72 6d2e 6874 6d6c 202d  ment_form.html -
+00002080: 2066 6f72 6d20 746f 2061 6464 2063 6f6d   form to add com
+00002090: 6d65 6e74 7320 746f 2071 7565 7374 696f  ments to questio
+000020a0: 6e20 286f 6e6c 7920 7368 6f77 7320 7570  n (only shows up
+000020b0: 2077 6865 6e20 666f 726d 2068 6173 2065   when form has e
+000020c0: 7272 6f72 2062 6563 6175 7365 2076 6965  rror because vie
+000020d0: 7720 6f6e 6c79 2067 6574 7320 706f 7374  w only gets post
+000020e0: 6564 2074 6f29 3a3a 0a0a 0a20 2020 2020  ed to)::...     
+000020f0: 2020 203c 6831 3e50 6f73 7420 4120 436f     <h1>Post A Co
+00002100: 6d6d 656e 743c 2f68 313e 0a20 2020 2020  mment</h1>.     
+00002110: 2020 203c 6120 6872 6566 3d22 7b7b 7175     <a href="{{qu
+00002120: 6573 7469 6f6e 2e67 6574 5f61 6273 6f6c  estion.get_absol
+00002130: 7574 655f 7572 6c7d 7d22 3e3c 6833 3e7b  ute_url}}"><h3>{
+00002140: 7b71 7565 7374 696f 6e2e 7175 6573 7469  {question.questi
+00002150: 6f6e 7d7d 3c2f 6833 3e3c 2f61 3e0a 2020  on}}</h3></a>.  
+00002160: 2020 2020 2020 3c66 6f72 6d20 6d65 7468        <form meth
+00002170: 6f64 3d22 706f 7374 223e 0a20 2020 2020  od="post">.     
+00002180: 2020 2020 2020 207b 2520 6373 7266 5f74         {% csrf_t
+00002190: 6f6b 656e 2025 7d0a 2020 2020 2020 2020  oken %}.        
+000021a0: 2020 2020 7b7b 666f 726d 7d7d 0a20 2020      {{form}}.   
+000021b0: 2020 2020 2020 2020 203c 696e 7075 7420           <input 
+000021c0: 7479 7065 3d22 7375 626d 6974 223e 0a20  type="submit">. 
+000021d0: 2020 2020 2020 203c 2f66 6f72 6d3e 0a0a         </form>..
+000021e0: 372e 2071 7565 7374 696f 6e5f 666f 726d  7. question_form
+000021f0: 2e68 746d 6c20 2d20 666f 726d 2074 6f20  .html - form to 
+00002200: 6164 6420 6120 6e65 7720 7175 6573 7469  add a new questi
+00002210: 6f6e 3a3a 0a0a 0a20 2020 2020 2020 203c  on::...        <
+00002220: 6831 3e41 6464 2059 6f75 7220 5175 6573  h1>Add Your Ques
+00002230: 7469 6f6e 3c2f 6831 3e0a 2020 2020 2020  tion</h1>.      
+00002240: 2020 3c66 6f72 6d20 6d65 7468 6f64 3d22    <form method="
+00002250: 706f 7374 223e 0a20 2020 2020 2020 2020  post">.         
+00002260: 2020 207b 2520 6373 7266 5f74 6f6b 656e     {% csrf_token
+00002270: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+00002280: 7b7b 666f 726d 7d7d 0a20 2020 2020 2020  {{form}}.       
+00002290: 2020 2020 203c 696e 7075 7420 7479 7065       <input type
+000022a0: 3d22 7375 626d 6974 223e 0a20 2020 2020  ="submit">.     
+000022b0: 2020 203c 2f66 6f72 6d3e 0a0a 382e 2076     </form>..8. v
+000022c0: 6f74 655f 666f 726d 2e68 746d 6c20 2d20  ote_form.html - 
+000022d0: 666f 726d 2066 6f72 2076 6f74 696e 6720  form for voting 
+000022e0: 7175 6573 7469 6f6e 7320 616e 6420 616e  questions and an
+000022f0: 7377 6572 7320 286f 6e6c 7920 7368 6f77  swers (only show
+00002300: 7320 7570 2077 6865 6e20 666f 726d 2068  s up when form h
+00002310: 6173 2065 7272 6f72 2062 6563 6175 7365  as error because
+00002320: 2076 6965 7720 6f6e 6c79 2067 6574 7320   view only gets 
+00002330: 706f 7374 6564 2074 6f29 3a3a 0a0a 0a20  posted to)::... 
+00002340: 2020 2020 2020 203c 6831 3e76 6f74 653c         <h1>vote<
+00002350: 2f68 313e 0a20 2020 2020 2020 203c 666f  /h1>.        <fo
+00002360: 726d 206d 6574 686f 643d 2270 6f73 7422  rm method="post"
+00002370: 3e0a 2020 2020 2020 2020 2020 2020 7b25  >.            {%
+00002380: 2063 7372 665f 746f 6b65 6e20 257d 0a20   csrf_token %}. 
+00002390: 2020 2020 2020 2020 2020 207b 7b66 6f72             {{for
+000023a0: 6d7d 7d0a 2020 2020 2020 2020 2020 2020  m}}.            
+000023b0: 3c69 6e70 7574 2074 7970 653d 2273 7562  <input type="sub
+000023c0: 6d69 7422 3e0a 2020 2020 2020 2020 3c2f  mit">.        </
+000023d0: 666f 726d 3e0a 0a39 2e20 636f 6d6d 656e  form>..9. commen
+000023e0: 7473 2e68 746d 6c20 2d20 6966 2063 6f6d  ts.html - if com
+000023f0: 6d65 6e74 7320 6172 6520 616c 6c6f 7765  ments are allowe
+00002400: 6420 7468 6973 2074 656d 706c 6174 6520  d this template 
+00002410: 6973 2069 6e63 6c75 6465 6420 696e 2074  is included in t
+00002420: 6865 2071 7565 7374 696f 6e20 6465 7461  he question deta
+00002430: 696c 2e68 746d 6c3a 3a0a 0a0a 2020 2020  il.html::...    
+00002440: 2020 2020 3c68 333e 636f 6d6d 656e 7473      <h3>comments
+00002450: 3c2f 6833 3e0a 2020 2020 2020 2020 3c75  </h3>.        <u
+00002460: 6c3e 0a20 2020 2020 2020 2020 2020 207b  l>.            {
+00002470: 2520 666f 7220 636f 6d6d 656e 7420 696e  % for comment in
+00002480: 2071 7565 7374 696f 6e2e 6661 7163 6f6d   question.faqcom
+00002490: 6d65 6e74 5f73 6574 2e61 6c6c 2025 7d0a  ment_set.all %}.
+000024a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024b0: 3c6c 693e 3c68 343e 7b7b 636f 6d6d 656e  <li><h4>{{commen
+000024c0: 742e 636f 6d6d 656e 747d 7d3c 2f68 343e  t.comment}}</h4>
+000024d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000024e0: 2020 2020 2070 6f73 7465 6420 6279 207b       posted by {
+000024f0: 2520 6966 2063 6f6d 6d65 6e74 2e75 7365  % if comment.use
+00002500: 7225 7d7b 7b63 6f6d 6d65 6e74 2e75 7365  r%}{{comment.use
+00002510: 727d 7d7b 2520 656c 7365 2025 7d61 6e6f  r}}{% else %}ano
+00002520: 6e79 6d6f 7573 7b25 2065 6e64 6966 2025  nymous{% endif %
+00002530: 7d20 7b7b 636f 6d6d 656e 742e 706f 7374  } {{comment.post
+00002540: 5f74 696d 657c 7469 6d65 7369 6e63 657d  _time|timesince}
+00002550: 7d20 6167 6f3c 2f6c 693e 0a20 2020 2020  } ago</li>.     
+00002560: 2020 2020 2020 207b 2520 656e 6466 6f72         {% endfor
+00002570: 2025 7d0a 2020 2020 2020 2020 3c2f 756c   %}.        </ul
+00002580: 3e0a 2020 2020 2020 2020 7b25 2069 6620  >.        {% if 
+00002590: 6164 645f 6e65 775f 636f 6d6d 656e 745f  add_new_comment_
+000025a0: 616c 6c6f 7765 6420 257d 0a20 2020 2020  allowed %}.     
+000025b0: 2020 2020 2020 207b 2520 6966 2063 6174         {% if cat
+000025c0: 6567 6f72 795f 656e 6162 6c65 6420 257d  egory_enabled %}
+000025d0: 0a20 2020 2020 2020 2020 2020 203c 666f  .            <fo
+000025e0: 726d 206d 6574 686f 643d 2270 6f73 7422  rm method="post"
+000025f0: 2061 6374 696f 6e3d 227b 2520 7572 6c20   action="{% url 
+00002600: 2766 6171 3a61 6464 5f63 6f6d 6d65 6e74  'faq:add_comment
+00002610: 2720 7175 6573 7469 6f6e 2e63 6174 6567  ' question.categ
+00002620: 6f72 792e 736c 7567 2071 7565 7374 696f  ory.slug questio
+00002630: 6e2e 736c 7567 2025 7d22 3e0a 2020 2020  n.slug %}">.    
+00002640: 2020 2020 2020 2020 7b25 2065 6c73 6520          {% else 
+00002650: 257d 0a20 2020 2020 2020 2020 2020 203c  %}.            <
+00002660: 666f 726d 206d 6574 686f 643d 2270 6f73  form method="pos
+00002670: 7422 2061 6374 696f 6e3d 227b 2520 7572  t" action="{% ur
+00002680: 6c20 2766 6171 3a61 6464 5f63 6f6d 6d65  l 'faq:add_comme
+00002690: 6e74 2720 7175 6573 7469 6f6e 2e73 6c75  nt' question.slu
+000026a0: 6720 257d 223e 0a20 2020 2020 2020 2020  g %}">.         
+000026b0: 2020 207b 2520 656e 6469 6620 257d 0a20     {% endif %}. 
+000026c0: 2020 2020 2020 2020 2020 203c 6669 656c             <fiel
+000026d0: 6473 6574 3e0a 2020 2020 2020 2020 2020  dset>.          
+000026e0: 2020 2020 2020 3c6c 6567 656e 643e 506f        <legend>Po
+000026f0: 7374 2059 6f75 7220 436f 6d6d 656e 7420  st Your Comment 
+00002700: 4865 7265 3a3c 2f6c 6567 656e 643e 0a20  Here:</legend>. 
+00002710: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00002720: 2520 6373 7266 5f74 6f6b 656e 2025 7d0a  % csrf_token %}.
+00002730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002740: 7b7b 636f 6d6d 656e 745f 666f 726d 7d7d  {{comment_form}}
+00002750: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002760: 203c 696e 7075 7420 7479 7065 3d22 7375   <input type="su
+00002770: 626d 6974 2220 6e61 6d65 3d22 706f 7374  bmit" name="post
+00002780: 223e 0a20 2020 2020 2020 2020 2020 203c  ">.            <
+00002790: 2f66 6965 6c64 7365 743e 0a20 2020 2020  /fieldset>.     
+000027a0: 2020 2020 2020 203c 2f66 6f72 6d3e 0a20         </form>. 
+000027b0: 2020 2020 2020 207b 2520 656e 6469 6620         {% endif 
+000027c0: 257d 0a0a 2323 2054 656d 706c 6174 6520  %}..## Template 
+000027d0: 5661 7269 6162 6c65 730a 0a31 2e20 6361  Variables..1. ca
+000027e0: 7465 676f 7269 6573 5f6c 6973 742e 6874  tegories_list.ht
+000027f0: 6d6c 0a20 2020 2063 6174 6567 6f72 6965  ml.    categorie
+00002800: 7320 2d20 616c 6c20 7468 6520 6361 7465  s - all the cate
+00002810: 676f 7269 6573 2028 6361 7465 676f 7279  gories (category
+00002820: 2071 7565 7279 7365 7429 0a0a 322e 2063   queryset)..2. c
+00002830: 6174 6567 6f72 6965 735f 6465 7461 696c  ategories_detail
+00002840: 2e68 746d 6c0a 2020 2020 6361 7465 676f  .html.    catego
+00002850: 7279 202d 2074 6865 2063 6174 6567 6f72  ry - the categor
+00002860: 7920 6368 6f73 656e 2028 6361 7465 676f  y chosen (catego
+00002870: 7279 206f 626a 6563 7429 0a20 2020 2063  ry object).    c
+00002880: 616e 5f61 6464 5f71 7565 7374 696f 6e20  an_add_question 
+00002890: 2d20 626f 6f6c 2069 6620 7468 6520 7573  - bool if the us
+000028a0: 6572 2063 616e 2061 6464 2061 2071 7565  er can add a que
+000028b0: 7374 696f 6e20 2864 6570 656e 6473 206f  stion (depends o
+000028c0: 6e20 7468 6520 7365 7474 696e 6773 290a  n the settings).
+000028d0: 332e 2071 7565 7374 696f 6e73 5f6c 6973  3. questions_lis
+000028e0: 742e 6874 6d6c 0a20 2020 2071 7565 7374  t.html.    quest
+000028f0: 696f 6e73 202d 2061 6c6c 2074 6865 2071  ions - all the q
+00002900: 7565 7374 696f 6e73 2028 7175 6573 7469  uestions (questi
+00002910: 6f6e 2071 7565 7279 7365 7429 0a20 2020  on queryset).   
+00002920: 2063 616e 5f61 6464 5f71 7565 7374 696f   can_add_questio
+00002930: 6e20 2d20 626f 6f6c 2069 6620 7468 6520  n - bool if the 
+00002940: 7573 6572 2063 616e 2061 6464 2061 2071  user can add a q
+00002950: 7565 7374 696f 6e20 2864 6570 656e 6473  uestion (depends
+00002960: 206f 6e20 7468 6520 7365 7474 696e 6773   on the settings
+00002970: 290a 342e 2071 7565 7374 696f 6e5f 6465  ).4. question_de
+00002980: 7461 696c 2e68 746d 6c0a 2020 2020 7175  tail.html.    qu
+00002990: 6573 7469 6f6e 202d 2074 6865 2071 7565  estion - the que
+000029a0: 7374 696f 6e20 6368 6f73 656e 2028 7175  stion chosen (qu
+000029b0: 6573 7469 6f6e 206f 626a 6563 7429 0a20  estion object). 
+000029c0: 2020 2063 616e 5f76 6f74 655f 7175 6573     can_vote_ques
+000029d0: 7469 6f6e 202d 2062 6f6f 6c20 6966 2074  tion - bool if t
+000029e0: 6865 2075 7365 7220 6361 6e20 766f 7465  he user can vote
+000029f0: 2061 2071 7565 7374 696f 6e20 2864 6570   a question (dep
+00002a00: 656e 6473 206f 6e20 7468 6520 7365 7474  ends on the sett
+00002a10: 696e 6773 290a 2020 2020 6361 7465 676f  ings).    catego
+00002a20: 7279 5f65 6e61 626c 6564 202d 2062 6f6f  ry_enabled - boo
+00002a30: 6c20 6966 2063 6174 6567 6f72 7920 656e  l if category en
+00002a40: 6162 6c65 6420 696e 2073 6574 7469 6e67  abled in setting
+00002a50: 730a 2020 2020 616c 6c6f 775f 6d75 6c74  s.    allow_mult
+00002a60: 6970 6c65 5f61 6e73 7765 7273 202d 2062  iple_answers - b
+00002a70: 6f6f 6c20 6966 206d 756c 7469 706c 6520  ool if multiple 
+00002a80: 616e 7377 6572 7320 616c 6c6f 7765 6420  answers allowed 
+00002a90: 696e 2073 6574 7469 6e67 730a 2020 2020  in settings.    
+00002aa0: 6361 6e5f 766f 7465 5f61 6e73 7765 7220  can_vote_answer 
+00002ab0: 2d20 626f 6f6c 2069 6620 7468 6520 7573  - bool if the us
+00002ac0: 6572 2063 616e 2076 6f74 6520 616e 2061  er can vote an a
+00002ad0: 6e73 7765 7220 2864 6570 656e 6473 206f  nswer (depends o
+00002ae0: 6e20 7468 6520 7365 7474 696e 6773 290a  n the settings).
+00002af0: 2020 2020 6361 6e5f 616e 7377 6572 5f71      can_answer_q
+00002b00: 7565 7374 696f 6e20 2d20 626f 6f6c 2069  uestion - bool i
+00002b10: 6620 6375 7272 656e 7420 7573 6572 2063  f current user c
+00002b20: 616e 2061 6e73 7765 7220 7175 6573 7469  an answer questi
+00002b30: 6f6e 2028 6465 7065 6e64 7320 6f6e 2074  on (depends on t
+00002b40: 6865 2073 6574 7469 6e67 7329 0a20 2020  he settings).   
+00002b50: 2063 6f6d 6d65 6e74 735f 616c 6c6f 7765   comments_allowe
+00002b60: 6420 2d20 626f 6f6c 2069 6620 7573 696e  d - bool if usin
+00002b70: 6720 636f 6d6d 656e 7473 2069 6e20 7365  g comments in se
+00002b80: 7474 696e 6773 0a20 2020 2061 6464 5f6e  ttings.    add_n
+00002b90: 6577 5f63 6f6d 6d65 6e74 5f61 6c6c 6f77  ew_comment_allow
+00002ba0: 6564 202d 2062 6f6f 6c20 6966 2063 7572  ed - bool if cur
+00002bb0: 7265 6e74 2075 7365 7220 6361 6e20 6164  rent user can ad
+00002bc0: 6420 636f 6d6d 656e 7420 2864 6570 656e  d comment (depen
+00002bd0: 6473 206f 6e20 7468 6520 7365 7474 696e  ds on the settin
+00002be0: 6773 290a 2020 2020 636f 6d6d 656e 745f  gs).    comment_
+00002bf0: 666f 726d 202d 2066 6f72 6d20 746f 2073  form - form to s
+00002c00: 7562 6d69 7420 6120 6e65 7720 636f 6d6d  ubmit a new comm
+00002c10: 656e 740a 352e 2061 6e73 7765 725f 666f  ent.5. answer_fo
+00002c20: 726d 2e68 746d 6c0a 2020 2020 7175 6573  rm.html.    ques
+00002c30: 7469 6f6e 202d 2074 6865 2071 7565 7374  tion - the quest
+00002c40: 696f 6e20 746f 2061 6464 2061 6e73 7765  ion to add answe
+00002c50: 7220 746f 2028 7175 6573 7469 6f6e 206f  r to (question o
+00002c60: 626a 6563 7429 0a20 2020 2066 6f72 6d20  bject).    form 
+00002c70: 2d20 666f 726d 2074 6f20 6164 6420 6e65  - form to add ne
+00002c80: 7720 616e 7377 6572 0a36 2e20 636f 6d6d  w answer.6. comm
+00002c90: 656e 745f 666f 726d 2e68 746d 6c0a 2020  ent_form.html.  
+00002ca0: 2020 7175 6573 7469 6f6e 202d 2074 6865    question - the
+00002cb0: 2071 7565 7374 696f 6e20 746f 2061 6464   question to add
+00002cc0: 2063 6f6d 6d65 6e74 2074 6f20 2871 7565   comment to (que
+00002cd0: 7374 696f 6e20 6f62 6a65 6374 290a 2020  stion object).  
+00002ce0: 2020 666f 726d 202d 2066 6f72 6d20 746f    form - form to
+00002cf0: 2061 6464 206e 6577 2063 6f6d 6d65 6e74   add new comment
+00002d00: 0a37 2e20 7175 6573 7469 6f6e 5f66 6f72  .7. question_for
+00002d10: 6d2e 6874 6d6c 0a20 2020 2066 6f72 6d20  m.html.    form 
+00002d20: 2d20 666f 726d 2074 6f20 6164 6420 6e65  - form to add ne
+00002d30: 7720 7175 6573 7469 6f6e 0a38 2e20 766f  w question.8. vo
+00002d40: 7465 5f66 6f72 6d2e 6874 6d6c 0a20 2020  te_form.html.   
+00002d50: 2066 6f72 6d20 2d20 666f 726d 2074 6f20   form - form to 
+00002d60: 766f 7465 2066 6f72 2061 2071 7565 7374  vote for a quest
+00002d70: 696f 6e20 6f72 2061 6e73 7765 720a 0a23  ion or answer..#
+00002d80: 2320 5572 6c73 0a0a 616c 6c20 6f66 2074  # Urls..all of t
+00002d90: 6865 2066 6f6c 6c6f 7769 6e67 2075 726c  he following url
+00002da0: 7320 6172 6520 6279 206e 616d 6520 7468  s are by name th
+00002db0: 656e 2061 6464 6974 696f 6e61 6c0a 7468  en additional.th
+00002dc0: 6520 6170 7020 6e61 6d65 2066 6f72 2074  e app name for t
+00002dd0: 6865 2075 726c 7320 6973 2060 6027 6661  he urls is ``'fa
+00002de0: 7127 6060 0a0a 2a20 696e 6465 785f 7669  q'``..* index_vi
+00002df0: 6577 0a20 2020 202a 206e 6f20 6172 6775  ew.    * no argu
+00002e00: 6d65 6e74 730a 2020 2020 2a20 6469 7370  ments.    * disp
+00002e10: 6c61 7973 2061 6c6c 2074 6865 2063 6174  lays all the cat
+00002e20: 6567 6f72 6965 7320 6966 2063 6174 6567  egories if categ
+00002e30: 6f72 6965 7320 6172 6520 656e 6162 6c65  ories are enable
+00002e40: 6420 6f74 6865 7277 6973 6520 7368 6f77  d otherwise show
+00002e50: 7320 7175 6573 7469 6f6e 730a 2a20 6361  s questions.* ca
+00002e60: 7465 676f 7279 5f64 6574 6169 6c0a 2020  tegory_detail.  
+00002e70: 2020 2a20 6e65 6564 7320 6361 7465 676f    * needs catego
+00002e80: 7279 2073 6c75 6720 6173 2073 6c75 670a  ry slug as slug.
+00002e90: 2020 2020 2a20 6469 7370 6c61 7973 2061      * displays a
+00002ea0: 6c6c 2074 6865 2071 7565 7374 696f 6e73  ll the questions
+00002eb0: 2067 6976 656e 2074 6865 2063 6174 6567   given the categ
+00002ec0: 6f72 7920 7768 656e 2063 6174 6567 6f72  ory when categor
+00002ed0: 6965 7320 6172 6520 656e 6162 6c65 640a  ies are enabled.
+00002ee0: 2a20 6164 645f 7175 6573 7469 6f6e 0a20  * add_question. 
+00002ef0: 2020 202a 2069 6620 6361 7465 676f 7269     * if categori
+00002f00: 6573 2061 7265 2065 6e61 626c 6564 206e  es are enabled n
+00002f10: 6565 6473 2063 6174 6567 6f72 7920 736c  eeds category sl
+00002f20: 7567 2061 7320 736c 7567 0a20 2020 202a  ug as slug.    *
+00002f30: 2069 6620 6c6f 6767 6564 5f69 6e5f 7573   if logged_in_us
+00002f40: 6572 735f 6361 6e5f 6164 645f 7175 6573  ers_can_add_ques
+00002f50: 7469 6f6e 2074 6865 6e20 6469 7370 6c61  tion then displa
+00002f60: 7973 2066 6f72 6d20 666f 7220 6c6f 6767  ys form for logg
+00002f70: 6564 2069 6e20 7573 6572 7320 746f 2061  ed in users to a
+00002f80: 736b 2061 206e 6577 2071 7565 7374 696f  sk a new questio
+00002f90: 6e0a 2a20 7175 6573 7469 6f6e 5f64 6574  n.* question_det
+00002fa0: 6169 6c0a 2020 2020 2a20 6e65 6564 7320  ail.    * needs 
+00002fb0: 7175 6573 7469 6f6e 2073 6c75 6720 6173  question slug as
+00002fc0: 2071 7565 7374 696f 6e20 7c20 6966 2063   question | if c
+00002fd0: 6174 6567 6f72 6965 7320 6172 6520 656e  ategories are en
+00002fe0: 6162 6c65 6420 6e65 6564 7320 6361 7465  abled needs cate
+00002ff0: 676f 7279 2073 6c75 6720 6173 2073 6c75  gory slug as slu
+00003000: 670a 2020 2020 2a20 6469 7370 6c61 7973  g.    * displays
+00003010: 2074 6865 206d 6169 6e20 4641 5120 7061   the main FAQ pa
+00003020: 6765 2077 6974 6820 7468 6520 7175 6573  ge with the ques
+00003030: 7469 6f6e 2061 6c6c 2074 6865 2063 6f6d  tion all the com
+00003040: 6d65 6e74 7320 616e 6420 616e 7377 6572  ments and answer
+00003050: 730a 2a20 616e 7377 6572 5f71 7565 7374  s.* answer_quest
+00003060: 696f 6e0a 2020 2020 2a20 6e65 6564 7320  ion.    * needs 
+00003070: 7175 6573 7469 6f6e 2073 6c75 6720 6173  question slug as
+00003080: 2071 7565 7374 696f 6e20 7c20 6966 2063   question | if c
+00003090: 6174 6567 6f72 6965 7320 6172 6520 656e  ategories are en
+000030a0: 6162 6c65 6420 6e65 6564 7320 6361 7465  abled needs cate
+000030b0: 676f 7279 2073 6c75 6720 6173 2063 6174  gory slug as cat
+000030c0: 6567 6f72 790a 2020 2020 2a20 6469 7370  egory.    * disp
+000030d0: 6c61 7973 2074 6865 2061 6e73 7765 7220  lays the answer 
+000030e0: 7175 6573 7469 6f6e 2066 6f72 6d0a 2a20  question form.* 
+000030f0: 6164 645f 636f 6d6d 656e 740a 2020 2020  add_comment.    
+00003100: 2a20 6e65 6564 7320 7175 6573 7469 6f6e  * needs question
+00003110: 2073 6c75 6720 6173 2071 7565 7374 696f   slug as questio
+00003120: 6e20 7c20 6966 2063 6174 6567 6f72 6965  n | if categorie
+00003130: 7320 6172 6520 656e 6162 6c65 6420 6e65  s are enabled ne
+00003140: 6564 7320 6361 7465 676f 7279 2073 6c75  eds category slu
+00003150: 6720 6173 2063 6174 6567 6f72 790a 2020  g as category.  
+00003160: 2020 2a20 6f6e 6c79 2077 6f72 6b73 2069    * only works i
+00003170: 6620 7573 696e 6720 636f 6d6d 656e 7473  f using comments
+00003180: 0a20 2020 202a 2075 7365 6420 746f 2070  .    * used to p
+00003190: 6f73 7420 636f 6d6d 656e 7420 666f 726d  ost comment form
+000031a0: 2066 726f 6d20 7175 6573 7469 6f6e 5f64   from question_d
+000031b0: 6574 6169 6c20 746f 2064 6174 6162 6173  etail to databas
+000031c0: 650a 2a20 766f 7465 5f61 6e73 7765 720a  e.* vote_answer.
+000031d0: 2020 2020 2a20 6e65 6564 7320 7175 6573      * needs ques
+000031e0: 7469 6f6e 2073 6c75 6720 6173 2071 7565  tion slug as que
+000031f0: 7374 696f 6e20 7c20 6e65 6564 7320 616e  stion | needs an
+00003200: 7377 6572 2073 6c75 6720 6173 2061 6e73  swer slug as ans
+00003210: 7765 7220 7c20 6966 2063 6174 6567 6f72  wer | if categor
+00003220: 6965 7320 6172 6520 656e 6162 6c65 6420  ies are enabled 
+00003230: 6e65 6564 7320 6361 7465 676f 7279 2073  needs category s
+00003240: 6c75 6720 6173 2063 6174 6567 6f72 790a  lug as category.
+00003250: 2020 2020 2a20 6f6e 6c79 2077 6f72 6b73      * only works
+00003260: 2069 6620 7573 696e 6720 616e 7377 6572   if using answer
+00003270: 2076 6f74 696e 670a 2020 2020 2a20 7573   voting.    * us
+00003280: 6564 2074 6f20 706f 7374 2068 6964 6465  ed to post hidde
+00003290: 6e20 696e 7075 7420 766f 7465 203d 2031  n input vote = 1
+000032a0: 206f 7220 766f 7465 203d 2030 2064 6570   or vote = 0 dep
+000032b0: 656e 6469 6e67 206f 6e20 766f 7465 2075  ending on vote u
+000032c0: 7020 6f72 2064 6f77 6e0a 2a20 766f 7465  p or down.* vote
+000032d0: 5f71 7565 7374 696f 6e0a 2020 2020 2a20  _question.    * 
+000032e0: 6e65 6564 7320 7175 6573 7469 6f6e 2073  needs question s
+000032f0: 6c75 6720 6173 2071 7565 7374 696f 6e20  lug as question 
+00003300: 7c20 6966 2063 6174 6567 6f72 6965 7320  | if categories 
+00003310: 6172 6520 656e 6162 6c65 6420 6e65 6564  are enabled need
+00003320: 7320 6361 7465 676f 7279 2073 6c75 6720  s category slug 
+00003330: 6173 2063 6174 6567 6f72 790a 2020 2020  as category.    
+00003340: 2a20 6f6e 6c79 2077 6f72 6b73 2069 6620  * only works if 
+00003350: 7573 696e 6720 7175 6573 7469 6f6e 2076  using question v
+00003360: 6f74 696e 670a 2020 2020 2a20 7573 6564  oting.    * used
+00003370: 2074 6f20 706f 7374 2068 6964 6465 6e20   to post hidden 
+00003380: 696e 7075 7420 766f 7465 203d 2031 206f  input vote = 1 o
+00003390: 7220 766f 7465 203d 2030 2064 6570 656e  r vote = 0 depen
+000033a0: 6469 6e67 206f 6e20 766f 7465 2075 7020  ding on vote up 
+000033b0: 6f72 2064 6f77 6e0a 0a23 2320 646a 616e  or down..## djan
+000033c0: 676f 2d74 696e 796d 6365 0a49 6620 796f  go-tinymce.If yo
+000033d0: 7520 7761 6e74 2074 6f20 7573 6520 7269  u want to use ri
+000033e0: 6368 2074 6578 7420 616e 7377 6572 7320  ch text answers 
+000033f0: 796f 7520 7769 6c6c 206e 6565 6420 746f  you will need to
+00003400: 205b 696e 7374 616c 6c20 646a 616e 676f   [install django
+00003410: 2d74 696e 796d 6365 5d28 6874 7470 733a  -tinymce](https:
+00003420: 2f2f 646a 616e 676f 2d74 696e 796d 6365  //django-tinymce
+00003430: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00003440: 656e 2f6c 6174 6573 742f 696e 7374 616c  en/latest/instal
+00003450: 6c61 7469 6f6e 2e68 746d 6c23 6964 3229  lation.html#id2)
+00003460: 0a0a 4d61 6b65 2073 7572 6520 746f 2069  ..Make sure to i
+00003470: 6e63 6c75 6465 2069 6e20 7468 6520 7465  nclude in the te
+00003480: 6d70 6c61 7465 2074 6865 2060 7b7b 2066  mplate the `{{ f
+00003490: 6f72 6d2e 6d65 6469 6120 7d7d 6020 746f  orm.media }}` to
+000034a0: 2069 6e63 6c75 6465 2074 6865 2074 696e   include the tin
+000034b0: 796d 6365 206a 6176 6173 6372 6970 7420  ymce javascript 
+000034c0: 616e 6420 6373 7320 6669 6c65 732e 0a3e  and css files..>
+000034d0: 205b 2157 4152 4e49 4e47 5d20 200a 3e20   [!WARNING]  .> 
+000034e0: 4661 696c 696e 6720 746f 2066 6f6c 6c6f  Failing to follo
+000034f0: 7720 7468 6520 666f 6c6c 6f77 696e 6720  w the following 
+00003500: 7374 6570 7320 7769 6c6c 2072 6573 756c  steps will resul
+00003510: 7420 696e 2061 2078 7373 2076 756c 6e65  t in a xss vulne
+00003520: 7261 6269 6c69 7479 2069 6e20 796f 7572  rability in your
+00003530: 2073 6974 652e 0a0a 546f 2061 6c6c 6f77   site...To allow
+00003540: 2074 6865 2072 6963 6820 7465 7874 2061   the rich text a
+00003550: 6e73 7765 7273 2074 6f20 6265 2072 656e  nswers to be ren
+00003560: 6465 7265 6420 7072 6f70 6572 6c79 2079  dered properly y
+00003570: 6f75 2077 696c 6c20 6e65 6564 2074 6f20  ou will need to 
+00003580: 7573 6520 7468 6520 7361 6665 2066 696c  use the safe fil
+00003590: 7465 7220 696e 2079 6f75 7220 7465 6d70  ter in your temp
+000035a0: 6c61 7465 732e 0a57 6869 6c65 2064 6a61  lates..While dja
+000035b0: 6e67 6f2d 7469 6e79 6d63 6520 646f 6573  ngo-tinymce does
+000035c0: 2065 7363 6170 6520 7468 6520 6874 6d6c   escape the html
+000035d0: 2074 6865 2061 6e73 7765 7273 2074 6861   the answers tha
+000035e0: 7420 7765 7265 2063 7265 6174 6564 2077  t were created w
+000035f0: 6865 6e20 7468 6520 7269 6368 2074 6578  hen the rich tex
+00003600: 7420 6564 6974 6f72 2077 6173 206e 6f74  t editor was not
+00003610: 2065 6e61 626c 6564 202a 2a68 6173 206e   enabled **has n
+00003620: 6f74 2062 6565 6e20 6573 6361 7065 6420  ot been escaped 
+00003630: 616e 6420 6973 206e 6f74 2073 6166 652a  and is not safe*
+00003640: 2a2e 0a53 6f20 7468 6573 6520 616e 7377  *..So these answ
+00003650: 6572 7320 6361 6e6e 6f74 2062 6520 7265  ers cannot be re
+00003660: 6e64 6572 6564 2077 6974 6820 7468 6520  ndered with the 
+00003670: 7361 6665 2066 696c 7465 722e 2053 6f20  safe filter. So 
+00003680: 6120 666c 6167 2077 6173 2061 6464 6564  a flag was added
+00003690: 2074 6f20 7468 6520 616e 7377 6572 206d   to the answer m
+000036a0: 6f64 656c 2027 6973 5f72 6963 685f 7465  odel 'is_rich_te
+000036b0: 7874 2720 7468 6174 2069 7320 7365 7420  xt' that is set 
+000036c0: 746f 2054 7275 6520 7768 656e 2074 6865  to True when the
+000036d0: 2061 6e73 7765 7220 6973 2063 7265 6174   answer is creat
+000036e0: 6564 2077 6974 6820 7468 6520 7269 6368  ed with the rich
+000036f0: 2074 6578 7420 6564 6974 6f72 2e0a 496e   text editor..In
+00003700: 2074 6865 2074 656d 706c 6174 6520 796f   the template yo
+00003710: 7520 6361 6e20 7573 6520 7468 6520 666f  u can use the fo
+00003720: 6c6c 6f77 696e 6720 636f 6465 2074 6f20  llowing code to 
+00003730: 7265 6e64 6572 2074 6865 2061 6e73 7765  render the answe
+00003740: 7220 7072 6f70 6572 6c79 3a3a 0a0a 2020  r properly::..  
+00003750: 2020 7b25 2069 6620 616e 7377 6572 2e69    {% if answer.i
+00003760: 735f 7269 6368 5f74 6578 7420 257d 0a20  s_rich_text %}. 
+00003770: 2020 2020 2020 207b 7b61 6e73 7765 722e         {{answer.
+00003780: 616e 7377 6572 7c73 6166 657d 7d0a 2020  answer|safe}}.  
+00003790: 2020 7b25 2065 6c73 6520 257d 0a20 2020    {% else %}.   
+000037a0: 2020 2020 207b 7b61 6e73 7765 722e 616e       {{answer.an
+000037b0: 7377 6572 7d7d 0a20 2020 207b 2520 656e  swer}}.    {% en
+000037c0: 6469 6620 257d 0a0a 2323 2043 6f6e 7472  dif %}..## Contr
+000037d0: 6962 7574 696e 670a 0a64 6a61 6e67 6f2d  ibuting..django-
+000037e0: 6561 7379 2d66 6171 2061 696d 7320 746f  easy-faq aims to
+000037f0: 2062 6520 7468 6520 6265 7374 2066 6171   be the best faq
+00003800: 2061 7070 2066 6f72 2064 6a61 6e67 6f2e   app for django.
+00003810: 2049 7420 7765 6c63 6f6d 6573 2020 636f   It welcomes  co
+00003820: 6e74 7269 6275 7469 6f6e 7320 6f66 2061  ntributions of a
+00003830: 6c6c 2074 7970 6573 202d 2069 7373 7565  ll types - issue
+00003840: 732c 2062 7567 732c 2066 6561 7475 7265  s, bugs, feature
+00003850: 2072 6571 7565 7374 732c 2064 6f63 756d   requests, docum
+00003860: 656e 7461 7469 6f6e 2075 7064 6174 6573  entation updates
+00003870: 2c20 7465 7374 7320 616e 6420 7075 6c6c  , tests and pull
+00003880: 2072 6571 7565 7374 730a 0a23 2320 6368   requests..## ch
+00003890: 616e 6765 206c 6f67 0a30 2e34 2066 6978  ange log.0.4 fix
+000038a0: 6564 2062 7567 2074 6861 7420 6c6f 6767  ed bug that logg
+000038b0: 6564 206f 7574 2075 7365 7273 2063 616e  ed out users can
+000038c0: 2076 6f74 6520 2d20 7768 6963 6820 7468   vote - which th
+000038d0: 656e 2072 6169 7365 7320 6578 6365 7074  en raises except
+000038e0: 696f 6e73 0a0a 302e 3520 6669 7865 6420  ions..0.5 fixed 
+000038f0: 6d69 6772 6174 696f 6e73 0a0a 312e 3020  migrations..1.0 
+00003900: 6164 6465 6420 7079 7069 2064 6973 7472  added pypi distr
+00003910: 6962 7574 696f 6e0a 0a31 2e31 2061 6464  ibution..1.1 add
+00003920: 6564 206d 6f72 6520 7465 6d70 6c61 7465  ed more template
+00003930: 7320 746f 206f 7665 7272 6964 6520 6561  s to override ea
+00003940: 7369 6c79 0a0a 312e 3220 6669 7865 6420  sily..1.2 fixed 
+00003950: 6275 6720 696e 2070 7970 6920 6469 7374  bug in pypi dist
+00003960: 726f 206e 6f74 2069 6e63 6c75 6469 6e67  ro not including
+00003970: 2066 6171 2061 7070 0a0a 312e 3320 6669   faq app..1.3 fi
+00003980: 7865 6420 6275 6720 7768 6572 6520 6120  xed bug where a 
+00003990: 736c 7567 206d 7573 7420 6265 2066 696c  slug must be fil
+000039a0: 6c65 6420 6f75 7420 696e 2061 646d 696e  led out in admin
+000039b0: 2065 7665 6e20 7468 6f75 6768 2073 6c75   even though slu
+000039c0: 6720 6765 7473 2061 7574 6f20 6765 6e65  g gets auto gene
+000039d0: 7261 7465 6420 746f 2073 6176 6520 666f  rated to save fo
+000039e0: 7220 7175 6573 7469 6f6e 732c 2061 6e73  r questions, ans
+000039f0: 7765 7273 2c20 616e 6420 6361 7465 676f  wers, and catego
+00003a00: 7269 6573 2e20 6d61 6465 2071 7565 7374  ries. made quest
+00003a10: 696f 6e73 2c20 616e 7377 6572 732c 2063  ions, answers, c
+00003a20: 6174 6567 6f72 6965 7320 736c 7567 7320  ategories slugs 
+00003a30: 7265 6164 6f6e 6c79 2069 6e20 6164 6d69  readonly in admi
+00003a40: 6e0a 0a31 2e34 2061 6464 6564 2075 6e69  n..1.4 added uni
+00003a50: 636f 6465 206f 7074 696f 6e20 746f 2061  code option to a
+00003a60: 6464 2075 6e69 636f 6465 2073 6c75 6773  dd unicode slugs
+00003a70: 0a0a 312e 3520 6164 6465 6420 6c6f 6769  ..1.5 added logi
+00003a80: 6e5f 7265 7175 6972 6564 2073 6574 7469  n_required setti
+00003a90: 6e67 2074 6f20 616c 6c6f 7720 6661 7120  ng to allow faq 
+00003aa0: 6170 7020 746f 2062 6520 6176 6169 6c61  app to be availa
+00003ab0: 626c 6520 746f 206f 6e6c 7920 6c6f 6767  ble to only logg
+00003ac0: 6564 2069 6e20 7573 6572 730a 0a31 2e36  ed in users..1.6
+00003ad0: 2066 6978 6564 2062 7567 2077 6865 7265   fixed bug where
+00003ae0: 206e 6f5f 6361 7465 676f 7279 5f64 6573   no_category_des
+00003af0: 6372 6970 7469 6f6e 2064 6964 206e 6f74  cription did not
+00003b00: 2064 6f20 7265 6d6f 7665 2074 6865 2063   do remove the c
+00003b10: 6174 6567 6f72 7920 6465 7363 7269 7074  ategory descript
+00003b20: 696f 6e20 696e 2074 6865 2061 646d 696e  ion in the admin
+00003b30: 0a0a 312e 3720 6164 6465 6420 7375 7070  ..1.7 added supp
+00003b40: 6f72 7420 666f 7220 646a 616e 676f 2035  ort for django 5
+00003b50: 2e30 0a0a 312e 3820 6164 6465 6420 7375  .0..1.8 added su
+00003b60: 7070 6f72 7420 666f 7220 7269 6368 7465  pport for richte
+00003b70: 7874 2061 6e73 7765 7273 2077 6974 6820  xt answers with 
+00003b80: 646a 616e 676f 2d74 696e 796d 6365       django-tinymce
```

### Comparing `django-easy-faq-1.7/README.md` & `django_easy_faq-1.8/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,897 +1,1004 @@
-00000000: 2320 646a 616e 676f 2d65 6173 792d 6661  # django-easy-fa
-00000010: 710d 0a0d 0a64 6a61 6e67 6f2d 6561 7379  q....django-easy
-00000020: 2d66 6171 2069 7320 6120 446a 616e 676f  -faq is a Django
-00000030: 2061 7070 2074 6f20 616c 6c6f 7720 666f   app to allow fo
-00000040: 7220 6120 7369 6d70 6c65 2079 6574 2066  r a simple yet f
-00000050: 6561 7475 7265 2072 6963 6820 6661 7120  eature rich faq 
-00000060: 6170 702e 2077 6974 6820 6361 7465 676f  app. with catego
-00000070: 7269 6573 2c20 636f 6d6d 656e 7469 6e67  ries, commenting
-00000080: 2076 6f74 696e 6720 6f66 2071 7565 7374   voting of quest
-00000090: 696f 6e73 2061 6e64 2061 6e73 7765 7273  ions and answers
-000000a0: 2061 6c6c 2061 7320 616e 206f 7074 696f   all as an optio
-000000b0: 6e61 6c20 7061 7274 206f 6620 7468 6520  nal part of the 
-000000c0: 6170 702e 2054 6f20 7365 6520 7363 7265  app. To see scre
-000000d0: 656e 7368 6f74 7320 6f66 2077 6861 7420  enshots of what 
-000000e0: 7468 6973 2064 6a61 6e67 6f2d 6561 7379  this django-easy
-000000f0: 2d66 6171 2063 6f75 6c64 206c 6f6f 6b20  -faq could look 
-00000100: 6c69 6b65 2077 6974 6820 626f 6f74 7374  like with bootst
-00000110: 7261 7020 3520 7374 796c 696e 6720 5b63  rap 5 styling [c
-00000120: 6c69 636b 2068 6572 655d 2864 656d 6f2f  lick here](demo/
-00000130: 6465 6d6f 2e6d 6429 2e0d 0a0d 0a0d 0a23  demo.md).......#
-00000140: 2320 5175 6963 6b20 7374 6172 740d 0a0d  # Quick start...
-00000150: 0a31 2e20 7069 7020 696e 7374 616c 6c3a  .1. pip install:
-00000160: 0d0a 0d0a 2020 2020 6070 6970 2069 6e73  ....    `pip ins
-00000170: 7461 6c6c 2064 6a61 6e67 6f2d 6561 7379  tall django-easy
-00000180: 2d66 6171 600d 0a0d 0a32 2e20 4164 6420  -faq`....2. Add 
-00000190: 2266 6171 2220 746f 2079 6f75 7220 494e  "faq" to your IN
-000001a0: 5354 414c 4c45 445f 4150 5053 2073 6574  STALLED_APPS set
-000001b0: 7469 6e67 206c 696b 6520 7468 6973 3a0d  ting like this:.
-000001c0: 0a0d 0a20 2020 2060 6060 7079 7468 6f6e  ...    ```python
-000001d0: 0d0a 2020 2020 494e 5354 414c 4c45 445f  ..    INSTALLED_
-000001e0: 4150 5053 203d 205b 0d0a 2020 2020 2020  APPS = [..      
-000001f0: 2020 2e2e 2e0d 0a20 2020 2020 2020 2027    .....        '
-00000200: 6661 7127 2c5d 0d0a 2020 2020 6060 600d  faq',]..    ```.
-00000210: 0a0d 0a33 2e20 496e 636c 7564 6520 7468  ...3. Include th
-00000220: 6520 6561 7379 2d66 6171 2055 524c 636f  e easy-faq URLco
-00000230: 6e66 2069 6e20 796f 7572 2070 726f 6a65  nf in your proje
-00000240: 6374 2075 726c 732e 7079 206c 696b 6520  ct urls.py like 
-00000250: 7468 6973 3a3a 0d0a 0d0a 2020 2020 6060  this::....    ``
-00000260: 6070 7974 686f 6e0d 0a20 2020 2023 e280  `python..    #..
-00000270: a60d 0a20 2020 2070 6174 6828 2766 6171  ...    path('faq
-00000280: 2f27 2c20 696e 636c 7564 6528 2766 6171  /', include('faq
-00000290: 2e75 726c 7327 2929 2c0d 0a20 2020 2023  .urls')),..    #
-000002a0: e280 a60d 0a20 2020 2060 6060 0d0a 0d0a  .....    ```....
-000002b0: 342e 2041 6464 2060 4641 515f 5345 5454  4. Add `FAQ_SETT
-000002c0: 494e 4753 203d 205b 5d60 2074 6f20 796f  INGS = []` to yo
-000002d0: 7572 2060 7365 7474 696e 6773 2e70 7960  ur `settings.py`
-000002e0: 0d0a 352e 2052 756e 2060 6070 7974 686f  ..5. Run ``pytho
-000002f0: 6e20 6d61 6e61 6765 2e70 7920 6d61 6b65  n manage.py make
-00000300: 6d69 6772 6174 696f 6e73 6060 2074 6f20  migrations`` to 
-00000310: 6372 6561 7465 2074 6865 2066 6171 206d  create the faq m
-00000320: 6f64 656c 7320 6d69 6772 6174 696f 6e73  odels migrations
-00000330: 2e0d 0a36 2e20 5275 6e20 6060 7079 7468  ...6. Run ``pyth
-00000340: 6f6e 206d 616e 6167 652e 7079 206d 6967  on manage.py mig
-00000350: 7261 7465 6060 2074 6f20 6372 6561 7465  rate`` to create
-00000360: 2074 6865 2066 6171 206d 6f64 656c 732e   the faq models.
-00000370: 0d0a 0d0a 372e 2053 7461 7274 2074 6865  ....7. Start the
-00000380: 2064 6576 656c 6f70 6d65 6e74 2073 6572   development ser
-00000390: 7665 7220 616e 6420 7669 7369 7420 6874  ver and visit ht
-000003a0: 7470 3a2f 2f31 3237 2e30 2e30 2e31 3a38  tp://127.0.0.1:8
-000003b0: 3030 302f 6164 6d69 6e2f 0d0a 2020 2074  000/admin/..   t
-000003c0: 6f20 6372 6561 7465 2061 2063 6174 6567  o create a categ
-000003d0: 6f72 7920 2879 6f75 276c 6c20 6e65 6564  ory (you'll need
-000003e0: 2074 6865 2041 646d 696e 2061 7070 2065   the Admin app e
-000003f0: 6e61 626c 6564 292e 2863 6174 6567 6f72  nabled).(categor
-00000400: 6965 7320 7061 7274 206f 6620 7468 6520  ies part of the 
-00000410: 6170 7020 6361 6e20 6265 2064 6973 6162  app can be disab
-00000420: 6c65 6429 0d0a 0d0a 382e 2056 6973 6974  led)....8. Visit
-00000430: 2068 7474 703a 2f2f 3132 372e 302e 302e   http://127.0.0.
-00000440: 313a 3830 3030 2f66 6171 2f20 746f 2073  1:8000/faq/ to s
-00000450: 6565 2074 6865 2063 6174 6567 6f72 6965  ee the categorie
-00000460: 732e 0d0a 0d0a 2323 2053 6574 7469 6e67  s.....## Setting
-00000470: 730d 0a0d 0a79 6f75 2063 616e 2063 6861  s....you can cha
-00000480: 6e67 6520 6d6f 7374 2074 6869 6e67 7320  nge most things 
-00000490: 696e 2073 6574 7469 6e67 7320 6265 6c6f  in settings belo
-000004a0: 7720 6973 2061 206c 6973 7420 6f66 2061  w is a list of a
-000004b0: 6c6c 2073 6574 7469 6e67 730d 0a61 6464  ll settings..add
-000004c0: 2061 6e79 206f 7220 616c 6c20 746f 2063   any or all to c
-000004d0: 6861 6e67 6520 746f 2064 6573 6972 6564  hange to desired
-000004e0: 2062 6568 6176 696f 723a 3a0d 0a0d 0a0d   behavior::.....
-000004f0: 0a20 2020 2046 4151 5f53 4554 5449 4e47  .    FAQ_SETTING
-00000500: 5320 3d20 5b27 796f 7572 5f73 6574 7469  S = ['your_setti
-00000510: 6e67 735f 6865 7265 272c 5d0d 0a0d 0a0d  ngs_here',].....
-00000520: 0a31 2e20 6e6f 5f63 6174 6567 6f72 795f  .1. no_category_
-00000530: 6465 7363 7269 7074 696f 6e20 2020 2020  description     
-00000540: 2020 2020 2020 2020 2020 2020 202d 2061               - a
-00000550: 6464 2069 6620 7573 696e 6720 6361 7465  dd if using cate
-00000560: 676f 7269 6573 2062 7574 2064 6f6e 2774  gories but don't
-00000570: 2077 616e 7420 6465 7363 7269 7074 696f   want descriptio
-00000580: 6e73 2066 6f72 2074 6865 6d0d 0a32 2e20  ns for them..2. 
-00000590: 6e6f 5f63 6174 6567 6f72 7920 2020 2020  no_category     
-000005a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005b0: 2020 2020 2020 2020 202d 2061 6464 2069           - add i
-000005c0: 6620 646f 6e27 7420 7761 6e74 2074 6f20  f don't want to 
-000005d0: 7573 6520 6361 7465 676f 7269 6573 0d0a  use categories..
-000005e0: 332e 206c 6f67 6765 645f 696e 5f75 7365  3. logged_in_use
-000005f0: 7273 5f63 616e 5f61 6464 5f71 7565 7374  rs_can_add_quest
-00000600: 696f 6e20 2020 2020 2020 2020 2d20 6164  ion         - ad
-00000610: 6420 6966 2079 6f75 2077 616e 7420 616e  d if you want an
-00000620: 7920 6c6f 6767 6564 2069 6e20 7573 6572  y logged in user
-00000630: 2074 6f20 6265 2061 626c 6520 746f 2061   to be able to a
-00000640: 736b 2061 2071 7565 7374 696f 6e0d 0a34  sk a question..4
-00000650: 2e20 6c6f 6767 6564 5f69 6e5f 7573 6572  . logged_in_user
-00000660: 735f 6361 6e5f 616e 7377 6572 5f71 7565  s_can_answer_que
-00000670: 7374 696f 6e20 2020 2020 202d 2061 6464  stion      - add
-00000680: 2069 6620 796f 7520 7761 6e74 2061 6e79   if you want any
-00000690: 206c 6f67 6765 6420 696e 2075 7365 7220   logged in user 
-000006a0: 746f 2062 6520 6162 6c65 2074 6f20 616e  to be able to an
-000006b0: 7377 6572 2061 2071 7565 7374 696f 6e0d  swer a question.
-000006c0: 0a35 2e20 616c 6c6f 775f 6d75 6c74 6970  .5. allow_multip
-000006d0: 6c65 5f61 6e73 7765 7273 2020 2020 2020  le_answers      
-000006e0: 2020 2020 2020 2020 2020 2020 202d 2061               - a
-000006f0: 6464 2069 6620 796f 7520 7761 6e74 2061  dd if you want a
-00000700: 2071 7565 7374 696f 6e20 746f 2062 6520   question to be 
-00000710: 6162 6c65 2074 6f20 6265 2061 6e73 7765  able to be answe
-00000720: 7265 6420 6d75 6c74 6970 6c65 2074 696d  red multiple tim
-00000730: 6573 0d0a 362e 206e 6f5f 636f 6d6d 656e  es..6. no_commen
-00000740: 7473 2020 2020 2020 2020 2020 2020 2020  ts              
-00000750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000760: 2d20 6164 6420 6966 2064 6f6e 2774 2077  - add if don't w
-00000770: 616e 7420 746f 2075 7365 2063 6f6d 6d65  ant to use comme
-00000780: 6e74 730d 0a37 2e20 616e 6f6e 796d 6f75  nts..7. anonymou
-00000790: 735f 7573 6572 5f63 616e 5f63 6f6d 6d65  s_user_can_comme
-000007a0: 6e74 2020 2020 2020 2020 2020 2020 2020  nt              
-000007b0: 202d 2061 6464 2069 6620 796f 7520 7761   - add if you wa
-000007c0: 6e74 2061 6e79 2075 7365 7220 746f 2062  nt any user to b
-000007d0: 6520 6162 6c65 2074 6f20 636f 6d6d 656e  e able to commen
-000007e0: 7420 696e 636c 7564 696e 6720 616e 6f6e  t including anon
-000007f0: 796d 6f75 7320 7573 6572 730d 0a38 2e20  ymous users..8. 
-00000800: 7669 6577 5f6f 6e6c 795f 636f 6d6d 656e  view_only_commen
-00000810: 7473 2020 2020 2020 2020 2020 2020 2020  ts              
-00000820: 2020 2020 2020 2020 202d 2061 6464 2069           - add i
-00000830: 6620 796f 7520 7761 6e74 2075 7365 7273  f you want users
-00000840: 2074 6f20 7365 6520 706f 7374 6564 2063   to see posted c
-00000850: 6f6d 6d65 6e74 7320 6275 7420 6e6f 7420  omments but not 
-00000860: 6265 2061 626c 6520 746f 2061 6464 2061  be able to add a
-00000870: 6e79 206d 6f72 650d 0a39 2e20 6e6f 5f76  ny more..9. no_v
-00000880: 6f74 6573 2020 2020 2020 2020 2020 2020  otes            
-00000890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008a0: 2020 2020 202d 2061 6464 2069 6620 646f       - add if do
-000008b0: 6e27 7420 7761 6e74 2061 6e79 2076 6f74  n't want any vot
-000008c0: 696e 6720 666f 7220 7573 6566 756c 2071  ing for useful q
-000008d0: 7565 7374 696f 6e73 206f 7220 616e 7377  uestions or answ
-000008e0: 6572 730d 0a31 302e 206e 6f5f 616e 7377  ers..10. no_answ
-000008f0: 6572 5f76 6f74 6573 2020 2020 2020 2020  er_votes        
-00000900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000910: 202d 2061 6464 2069 6620 6f6e 6c79 2077   - add if only w
-00000920: 616e 7420 7175 6573 7469 6f6e 2076 6f74  ant question vot
-00000930: 696e 670d 0a31 312e 206e 6f5f 7175 6573  ing..11. no_ques
-00000940: 7469 6f6e 5f76 6f74 6573 2020 2020 2020  tion_votes      
-00000950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000960: 202d 2061 6464 2069 6620 6f6e 6c79 2077   - add if only w
-00000970: 616e 7420 616e 7377 6572 2076 6f74 696e  ant answer votin
-00000980: 670d 0a31 322e 2061 6c6c 6f77 5f75 6e69  g..12. allow_uni
-00000990: 636f 6465 2020 2020 2020 2020 2020 2020  code            
-000009a0: 2020 2020 2020 2020 2020 2020 2020 202d                 -
-000009b0: 2061 6464 2069 6620 796f 7520 7761 6e74   add if you want
-000009c0: 2074 6f20 616c 6c6f 7720 756e 6963 6f64   to allow unicod
-000009d0: 6520 736c 7567 730d 0a31 332e 206c 6f67  e slugs..13. log
-000009e0: 696e 5f72 6571 7569 7265 6420 2020 2020  in_required     
-000009f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a00: 2020 2020 202d 2061 6464 2069 6620 796f       - add if yo
-00000a10: 7520 7761 6e74 2074 6f20 6f6e 6c79 206c  u want to only l
-00000a20: 6574 206c 6f67 6765 6420 696e 2075 7365  et logged in use
-00000a30: 7273 2073 6565 2046 4151 2773 0d0a 0d0a  rs see FAQ's....
-00000a40: 2323 2054 656d 706c 6174 6573 0d0a 0d0a  ## Templates....
-00000a50: 616c 6c20 6f66 2074 6865 2074 656d 706c  all of the templ
-00000a60: 6174 6573 2061 7265 206d 6561 6e74 2074  ates are meant t
-00000a70: 6f20 6265 206f 7665 7277 7269 7474 656e  o be overwritten
-00000a80: 0d0a 746f 206f 7665 7277 7269 7465 2074  ..to overwrite t
-00000a90: 6865 6d20 6372 6561 7465 2061 2066 6171  hem create a faq
-00000aa0: 2064 6972 6563 746f 7279 2069 6e73 6964   directory insid
-00000ab0: 6520 6f66 2074 6865 2074 656d 706c 6174  e of the templat
-00000ac0: 6573 2064 6972 6563 746f 7279 2061 6e64  es directory and
-00000ad0: 2061 6464 2061 2068 746d 6c20 6669 6c65   add a html file
-00000ae0: 2077 6974 6820 7468 6520 7361 6d65 206e   with the same n
-00000af0: 616d 6520 746f 2069 740d 0a0d 0a69 6620  ame to it....if 
-00000b00: 7468 6973 2064 6f65 736e 2774 2077 6f72  this doesn't wor
-00000b10: 6b20 6d61 6b65 2073 7572 6520 7468 6174  k make sure that
-00000b20: 2074 6865 2074 656d 706c 6174 6573 2073   the templates s
-00000b30: 6574 7469 6e67 2068 6173 2027 4449 5253  etting has 'DIRS
-00000b40: 273a 205b 2774 656d 706c 6174 6573 275d  ': ['templates']
-00000b50: 2c20 696e 2069 743a 3a0d 0a0d 0a20 2020  , in it::....   
-00000b60: 2054 454d 504c 4154 4553 203d 205b 0d0a   TEMPLATES = [..
-00000b70: 2020 2020 2020 2020 7b0d 0a20 2020 2020          {..     
-00000b80: 2020 2020 2020 202e 2e2e 0d0a 2020 2020         .....    
-00000b90: 2020 2020 2020 2020 2744 4952 5327 3a20          'DIRS': 
-00000ba0: 5b27 7465 6d70 6c61 7465 7327 5d2c 0d0a  ['templates'],..
-00000bb0: 2020 2020 2020 2020 2020 2020 2e2e 2e0d              ....
-00000bc0: 0a20 2020 2020 2020 207d 2c0d 0a20 2020  .        },..   
-00000bd0: 205d 0d0a 0d0a 6865 7265 2069 7320 6120   ]....here is a 
-00000be0: 6c69 7374 206f 6620 7465 6d70 6c61 7465  list of template
-00000bf0: 7320 616e 6420 7468 6572 6520 6465 6661  s and there defa
-00000c00: 756c 7420 7465 6d70 6c61 7465 2020 796f  ult template  yo
-00000c10: 7520 6361 6e20 6f76 6572 7772 6974 650d  u can overwrite.
-00000c20: 0a0d 0a31 2e20 6361 7465 676f 7269 6573  ...1. categories
-00000c30: 5f6c 6973 742e 6874 6d6c 202d 2066 6171  _list.html - faq
-00000c40: 206d 6169 6e20 7669 6577 2069 6620 7573   main view if us
-00000c50: 696e 6720 6361 7465 676f 7269 6573 3a3a  ing categories::
-00000c60: 0d0a 0d0a 0d0a 2020 2020 2020 2020 3c68  ......        <h
-00000c70: 313e 7365 6c65 6374 2061 2046 4151 2063  1>select a FAQ c
-00000c80: 6174 6567 6f72 793c 2f68 313e 0d0a 2020  ategory</h1>..  
-00000c90: 2020 2020 2020 7b25 2066 6f72 2063 6174        {% for cat
-00000ca0: 6567 6f72 7920 696e 2063 6174 6567 6f72  egory in categor
-00000cb0: 6965 7320 257d 0d0a 2020 2020 2020 2020  ies %}..        
-00000cc0: 2020 2020 3c68 333e 3c61 2068 7265 663d      <h3><a href=
-00000cd0: 227b 2520 7572 6c20 2766 6171 3a63 6174  "{% url 'faq:cat
-00000ce0: 6567 6f72 795f 6465 7461 696c 2720 6361  egory_detail' ca
-00000cf0: 7465 676f 7279 2e73 6c75 6720 257d 223e  tegory.slug %}">
-00000d00: 7b7b 6361 7465 676f 7279 2e6e 616d 657d  {{category.name}
-00000d10: 7d3c 2f61 3e3c 2f68 333e 0d0a 2020 2020  }</a></h3>..    
-00000d20: 2020 2020 2020 2020 7b25 2069 6620 6361          {% if ca
-00000d30: 7465 676f 7279 2e64 6573 6372 6970 7469  tegory.descripti
-00000d40: 6f6e 2025 7d0d 0a20 2020 2020 2020 2020  on %}..         
-00000d50: 2020 2020 2020 203c 703e 7b7b 6361 7465         <p>{{cate
-00000d60: 676f 7279 2e64 6573 6372 6970 7469 6f6e  gory.description
-00000d70: 7d7d 3c2f 703e 0d0a 2020 2020 2020 2020  }}</p>..        
-00000d80: 2020 2020 7b25 2065 6e64 6966 2025 7d0d      {% endif %}.
-00000d90: 0a20 2020 2020 2020 2020 2020 203c 6872  .            <hr
-00000da0: 3e0d 0a20 2020 2020 2020 207b 2520 656e  >..        {% en
-00000db0: 6466 6f72 2025 7d0d 0a0d 0a0d 0a32 2e20  dfor %}......2. 
-00000dc0: 6361 7465 676f 7279 5f64 6574 6169 6c2e  category_detail.
-00000dd0: 6874 6d6c 202d 2066 6171 2063 6174 6567  html - faq categ
-00000de0: 6f72 7920 6465 7461 696c 2076 6965 7720  ory detail view 
-00000df0: 6966 2075 7369 6e67 2063 6174 6567 6f72  if using categor
-00000e00: 6965 733a 3a0d 0a0d 0a0d 0a20 2020 2020  ies::......     
-00000e10: 2020 203c 6831 3e63 686f 6f73 6520 6120     <h1>choose a 
-00000e20: 4641 5120 5175 6573 7469 6f6e 3c2f 6831  FAQ Question</h1
-00000e30: 3e0d 0a20 2020 2020 2020 203c 6832 3e7b  >..        <h2>{
-00000e40: 7b63 6174 6567 6f72 797d 7d3c 2f68 323e  {category}}</h2>
-00000e50: 0d0a 2020 2020 2020 2020 7b25 2069 6620  ..        {% if 
-00000e60: 6361 7465 676f 7279 2e64 6573 6372 6970  category.descrip
-00000e70: 7469 6f6e 2025 7d0d 0a20 2020 2020 2020  tion %}..       
-00000e80: 203c 703e 7b7b 6361 7465 676f 7279 2e64   <p>{{category.d
-00000e90: 6573 6372 6970 7469 6f6e 7d7d 3c2f 703e  escription}}</p>
-00000ea0: 0d0a 2020 2020 2020 2020 7b25 2065 6e64  ..        {% end
-00000eb0: 6966 2025 7d0d 0a20 2020 2020 2020 203c  if %}..        <
-00000ec0: 6872 3e0d 0a20 2020 2020 2020 207b 2520  hr>..        {% 
-00000ed0: 666f 7220 7175 6573 7469 6f6e 2069 6e20  for question in 
-00000ee0: 6361 7465 676f 7279 2e71 7565 7374 696f  category.questio
-00000ef0: 6e5f 7365 742e 616c 6c20 257d 0d0a 2020  n_set.all %}..  
-00000f00: 2020 2020 2020 2020 2020 3c68 333e 3c61            <h3><a
-00000f10: 2068 7265 663d 227b 2520 7572 6c20 2766   href="{% url 'f
-00000f20: 6171 3a71 7565 7374 696f 6e5f 6465 7461  aq:question_deta
-00000f30: 696c 2720 6361 7465 676f 7279 2e73 6c75  il' category.slu
-00000f40: 6720 7175 6573 7469 6f6e 2e73 6c75 6720  g question.slug 
-00000f50: 257d 223e 7b7b 7175 6573 7469 6f6e 2e71  %}">{{question.q
-00000f60: 7565 7374 696f 6e7d 7d3c 2f61 3e3c 2f68  uestion}}</a></h
-00000f70: 333e 0d0a 2020 2020 2020 2020 7b25 2065  3>..        {% e
-00000f80: 6e64 666f 7220 257d 0d0a 2020 2020 2020  ndfor %}..      
-00000f90: 2020 3c68 723e 0d0a 2020 2020 2020 2020    <hr>..        
-00000fa0: 3c61 2068 7265 663d 227b 2520 7572 6c20  <a href="{% url 
-00000fb0: 2766 6171 3a69 6e64 6578 5f76 6965 7727  'faq:index_view'
-00000fc0: 2025 7d22 3e62 6163 6b3c 2f61 3e0d 0a20   %}">back</a>.. 
-00000fd0: 2020 2020 2020 207b 2520 6966 2063 616e         {% if can
-00000fe0: 5f61 6464 5f71 7565 7374 696f 6e20 257d  _add_question %}
-00000ff0: 0d0a 2020 2020 2020 2020 2020 2020 3c61  ..            <a
-00001000: 2068 7265 663d 227b 2520 7572 6c20 2766   href="{% url 'f
-00001010: 6171 3a61 6464 5f71 7565 7374 696f 6e27  aq:add_question'
-00001020: 2063 6174 6567 6f72 792e 736c 7567 2025   category.slug %
-00001030: 7d22 3e61 6464 2071 7565 7374 696f 6e3c  }">add question<
-00001040: 2f61 3e0d 0a20 2020 2020 2020 207b 2520  /a>..        {% 
-00001050: 656e 6469 6620 257d 0d0a 0d0a 0d0a 332e  endif %}......3.
-00001060: 2071 7565 7374 696f 6e73 5f6c 6973 742e   questions_list.
-00001070: 6874 6d6c 202d 206c 6973 7473 2061 6c6c  html - lists all
-00001080: 2071 7565 7374 696f 6e73 2069 6620 6e6f   questions if no
-00001090: 7420 7573 696e 6720 6361 7465 676f 7269  t using categori
-000010a0: 6573 3a3a 0d0a 0d0a 0d0a 2020 2020 2020  es::......      
-000010b0: 2020 3c68 313e 6368 6f6f 7365 2061 2046    <h1>choose a F
-000010c0: 4151 2051 7565 7374 696f 6e3c 2f68 313e  AQ Question</h1>
-000010d0: 0d0a 2020 2020 2020 2020 7b25 2066 6f72  ..        {% for
-000010e0: 2071 7565 7374 696f 6e20 696e 2071 7565   question in que
-000010f0: 7374 696f 6e73 2025 7d0d 0a20 2020 2020  stions %}..     
-00001100: 2020 2020 2020 203c 6833 3e3c 6120 6872         <h3><a hr
-00001110: 6566 3d22 7b25 2075 726c 2027 6661 713a  ef="{% url 'faq:
-00001120: 7175 6573 7469 6f6e 5f64 6574 6169 6c27  question_detail'
-00001130: 2071 7565 7374 696f 6e2e 736c 7567 2025   question.slug %
-00001140: 7d22 3e7b 7b71 7565 7374 696f 6e2e 7175  }">{{question.qu
-00001150: 6573 7469 6f6e 7d7d 3c2f 613e 3c2f 6833  estion}}</a></h3
-00001160: 3e0d 0a20 2020 2020 2020 207b 2520 656e  >..        {% en
-00001170: 6466 6f72 2025 7d0d 0a20 2020 200d 0a20  dfor %}..    .. 
-00001180: 2020 2020 2020 207b 2520 6966 2063 616e         {% if can
-00001190: 5f61 6464 5f71 7565 7374 696f 6e20 257d  _add_question %}
-000011a0: 0d0a 2020 2020 2020 2020 2020 2020 3c68  ..            <h
-000011b0: 723e 0d0a 2020 2020 2020 2020 2020 2020  r>..            
-000011c0: 3c61 2068 7265 663d 227b 2520 7572 6c20  <a href="{% url 
-000011d0: 2766 6171 3a61 6464 5f71 7565 7374 696f  'faq:add_questio
-000011e0: 6e27 2025 7d22 3e61 6464 2071 7565 7374  n' %}">add quest
-000011f0: 696f 6e3c 2f61 3e0d 0a20 2020 2020 2020  ion</a>..       
-00001200: 207b 2520 656e 6469 6620 257d 0d0a 0d0a   {% endif %}....
-00001210: 0d0a 342e 2071 7565 7374 696f 6e5f 6465  ..4. question_de
-00001220: 7461 696c 2e68 746d 6c20 2d20 7468 6520  tail.html - the 
-00001230: 7175 6573 7469 6f6e 2064 6574 6169 6c20  question detail 
-00001240: 7061 6765 3a3a 0d0a 0d0a 0d0a 2020 2020  page::......    
-00001250: 2020 2020 7b25 2065 7874 656e 6473 2027      {% extends '
-00001260: 6661 712f 7175 6573 7469 6f6e 5f62 6173  faq/question_bas
-00001270: 652e 6874 6d6c 2720 257d 0d0a 2020 2020  e.html' %}..    
-00001280: 0d0a 2020 2020 2020 2020 7b25 2062 6c6f  ..        {% blo
-00001290: 636b 2071 7565 7374 696f 6e5f 636f 6e74  ck question_cont
-000012a0: 656e 7420 257d 0d0a 2020 2020 2020 2020  ent %}..        
-000012b0: 7b25 2069 6620 616c 6c6f 775f 6d75 6c74  {% if allow_mult
-000012c0: 6970 6c65 5f61 6e73 7765 7273 2025 7d0d  iple_answers %}.
-000012d0: 0a20 2020 2020 2020 203c 6833 3e61 6e73  .        <h3>ans
-000012e0: 7765 7273 3c2f 6833 3e0d 0a20 2020 2020  wers</h3>..     
-000012f0: 2020 203c 756c 3e0d 0a20 2020 2020 2020     <ul>..       
-00001300: 2020 2020 207b 2520 666f 7220 616e 7377       {% for answ
-00001310: 6572 2069 6e20 7175 6573 7469 6f6e 2e61  er in question.a
-00001320: 6e73 7765 725f 7365 742e 616c 6c20 257d  nswer_set.all %}
-00001330: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001340: 2020 3c6c 693e 3c62 3e7b 7b61 6e73 7765    <li><b>{{answe
-00001350: 722e 616e 7377 6572 7d7d 3c2f 623e 0d0a  r.answer}}</b>..
-00001360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001370: 2020 2020 7b25 2069 6620 6361 6e5f 766f      {% if can_vo
-00001380: 7465 5f61 6e73 7765 7220 257d 0d0a 2020  te_answer %}..  
-00001390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000013a0: 2020 207c 2066 6f75 6e64 2074 6869 7320     | found this 
-000013b0: 616e 7377 6572 2068 656c 7066 756c 3f0d  answer helpful?.
-000013c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000013d0: 2020 2020 203c 666f 726d 2073 7479 6c65       <form style
-000013e0: 3d22 6469 7370 6c61 793a 2069 6e6c 696e  ="display: inlin
-000013f0: 653b 2220 6163 7469 6f6e 3d22 7b25 2069  e;" action="{% i
-00001400: 6620 6361 7465 676f 7279 5f65 6e61 626c  f category_enabl
-00001410: 6564 2025 7d7b 2520 7572 6c20 2766 6171  ed %}{% url 'faq
-00001420: 3a76 6f74 655f 616e 7377 6572 2720 7175  :vote_answer' qu
-00001430: 6573 7469 6f6e 2e63 6174 6567 6f72 792e  estion.category.
-00001440: 736c 7567 2071 7565 7374 696f 6e2e 736c  slug question.sl
-00001450: 7567 2061 6e73 7765 722e 736c 7567 2025  ug answer.slug %
-00001460: 7d7b 2520 656c 7365 2025 7d7b 2520 7572  }{% else %}{% ur
-00001470: 6c20 2766 6171 3a76 6f74 655f 616e 7377  l 'faq:vote_answ
-00001480: 6572 2720 7175 6573 7469 6f6e 2e73 6c75  er' question.slu
-00001490: 6720 616e 7377 6572 2e73 6c75 6720 257d  g answer.slug %}
-000014a0: 7b25 2065 6e64 6966 2025 7d22 206d 6574  {% endif %}" met
-000014b0: 686f 643d 2270 6f73 7422 3e0d 0a20 2020  hod="post">..   
-000014c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000014d0: 2020 2020 207b 2520 6373 7266 5f74 6f6b       {% csrf_tok
-000014e0: 656e 2025 7d0d 0a20 2020 2020 2020 2020  en %}..         
-000014f0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00001500: 696e 7075 7420 7479 7065 3d22 6869 6464  input type="hidd
-00001510: 656e 2220 7661 6c75 653d 5472 7565 206e  en" value=True n
-00001520: 616d 653d 2276 6f74 6522 3e0d 0a20 2020  ame="vote">..   
-00001530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001540: 2020 2020 203c 6275 7474 6f6e 2074 7970       <button typ
-00001550: 653d 2273 7562 6d69 7422 3e79 6573 287b  e="submit">yes({
-00001560: 7b61 6e73 7765 722e 6865 6c70 6675 6c7d  {answer.helpful}
-00001570: 7d29 3c2f 6275 7474 6f6e 3e0d 0a20 2020  })</button>..   
-00001580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001590: 203c 2f66 6f72 6d3e 0d0a 2020 2020 2020   </form>..      
-000015a0: 2020 2020 2020 2020 2020 2020 2020 3c66                <f
-000015b0: 6f72 6d20 7374 796c 653d 2264 6973 706c  orm style="displ
-000015c0: 6179 3a20 696e 6c69 6e65 3b22 2061 6374  ay: inline;" act
-000015d0: 696f 6e3d 227b 2520 6966 2063 6174 6567  ion="{% if categ
-000015e0: 6f72 795f 656e 6162 6c65 6420 257d 7b25  ory_enabled %}{%
-000015f0: 2075 726c 2027 6661 713a 766f 7465 5f61   url 'faq:vote_a
-00001600: 6e73 7765 7227 2071 7565 7374 696f 6e2e  nswer' question.
-00001610: 6361 7465 676f 7279 2e73 6c75 6720 7175  category.slug qu
-00001620: 6573 7469 6f6e 2e73 6c75 6720 616e 7377  estion.slug answ
-00001630: 6572 2e73 6c75 6720 257d 7b25 2065 6c73  er.slug %}{% els
-00001640: 6520 257d 7b25 2075 726c 2027 6661 713a  e %}{% url 'faq:
-00001650: 766f 7465 5f61 6e73 7765 7227 2071 7565  vote_answer' que
-00001660: 7374 696f 6e2e 736c 7567 2061 6e73 7765  stion.slug answe
-00001670: 722e 736c 7567 2025 7d7b 2520 656e 6469  r.slug %}{% endi
-00001680: 6620 257d 2220 6d65 7468 6f64 3d22 706f  f %}" method="po
-00001690: 7374 223e 0d0a 2020 2020 2020 2020 2020  st">..          
-000016a0: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-000016b0: 2063 7372 665f 746f 6b65 6e20 257d 0d0a   csrf_token %}..
-000016c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016d0: 2020 2020 2020 2020 3c69 6e70 7574 2074          <input t
-000016e0: 7970 653d 2268 6964 6465 6e22 2076 616c  ype="hidden" val
-000016f0: 7565 3d46 616c 7365 206e 616d 653d 2276  ue=False name="v
-00001700: 6f74 6522 3e0d 0a20 2020 2020 2020 2020  ote">..         
-00001710: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00001720: 6275 7474 6f6e 2074 7970 653d 2273 7562  button type="sub
-00001730: 6d69 7422 3e6e 6f28 7b7b 616e 7377 6572  mit">no({{answer
-00001740: 2e6e 6f74 5f68 656c 7066 756c 7d7d 293c  .not_helpful}})<
-00001750: 2f62 7574 746f 6e3e 0d0a 2020 2020 2020  /button>..      
-00001760: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00001770: 666f 726d 3e0d 0a20 2020 2020 2020 2020  form>..         
-00001780: 2020 2020 2020 2020 2020 207b 2520 656e             {% en
-00001790: 6469 6620 257d 0d0a 2020 2020 2020 2020  dif %}..        
-000017a0: 2020 2020 2020 2020 3c2f 6c69 3e0d 0a20          </li>.. 
-000017b0: 2020 2020 2020 2020 2020 207b 2520 656e             {% en
-000017c0: 6466 6f72 2025 7d0d 0a20 2020 2020 2020  dfor %}..       
-000017d0: 203c 2f75 6c3e 0d0a 2020 2020 0d0a 2020   </ul>..    ..  
-000017e0: 2020 2020 2020 7b25 2065 6c73 6520 257d        {% else %}
-000017f0: 0d0a 2020 2020 2020 2020 2020 2020 7b25  ..            {%
-00001800: 2069 6620 7175 6573 7469 6f6e 2e61 6e73   if question.ans
-00001810: 7765 725f 7365 742e 6578 6973 7473 2025  wer_set.exists %
-00001820: 7d0d 0a20 2020 2020 2020 2020 2020 2020  }..             
-00001830: 2020 203c 703e 616e 7377 6572 3a3c 2f70     <p>answer:</p
-00001840: 3e0d 0a20 2020 2020 2020 2020 2020 2020  >..             
-00001850: 2020 203c 6833 3e7b 7b71 7565 7374 696f     <h3>{{questio
-00001860: 6e2e 616e 7377 6572 5f73 6574 2e66 6972  n.answer_set.fir
-00001870: 7374 2e61 6e73 7765 727d 7d3c 2f68 333e  st.answer}}</h3>
-00001880: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001890: 2020 7b25 2069 6620 6361 6e5f 766f 7465    {% if can_vote
-000018a0: 5f61 6e73 7765 7220 257d 0d0a 2020 2020  _answer %}..    
-000018b0: 2020 2020 2020 2020 2020 2020 2066 6f75               fou
-000018c0: 6e64 2074 6869 7320 616e 7377 6572 2068  nd this answer h
-000018d0: 656c 7066 756c 3f0d 0a20 2020 2020 2020  elpful?..       
-000018e0: 2020 2020 2020 2020 203c 666f 726d 2073           <form s
-000018f0: 7479 6c65 3d22 6469 7370 6c61 793a 2069  tyle="display: i
-00001900: 6e6c 696e 653b 2220 6163 7469 6f6e 3d22  nline;" action="
-00001910: 7b25 2069 6620 6361 7465 676f 7279 5f65  {% if category_e
-00001920: 6e61 626c 6564 2025 7d7b 2520 7572 6c20  nabled %}{% url 
-00001930: 2766 6171 3a76 6f74 655f 616e 7377 6572  'faq:vote_answer
-00001940: 2720 7175 6573 7469 6f6e 2e63 6174 6567  ' question.categ
-00001950: 6f72 792e 736c 7567 2071 7565 7374 696f  ory.slug questio
-00001960: 6e2e 736c 7567 2071 7565 7374 696f 6e2e  n.slug question.
-00001970: 616e 7377 6572 5f73 6574 2e66 6972 7374  answer_set.first
-00001980: 2e73 6c75 6720 257d 7b25 2065 6c73 6520  .slug %}{% else 
-00001990: 257d 7b25 2075 726c 2027 6661 713a 766f  %}{% url 'faq:vo
-000019a0: 7465 5f61 6e73 7765 7227 2071 7565 7374  te_answer' quest
-000019b0: 696f 6e2e 736c 7567 2071 7565 7374 696f  ion.slug questio
-000019c0: 6e2e 616e 7377 6572 5f73 6574 2e66 6972  n.answer_set.fir
-000019d0: 7374 2e73 6c75 6720 257d 7b25 2065 6e64  st.slug %}{% end
-000019e0: 6966 2025 7d22 206d 6574 686f 643d 2270  if %}" method="p
-000019f0: 6f73 7422 3e0d 0a20 2020 2020 2020 2020  ost">..         
-00001a00: 2020 2020 2020 2020 2020 207b 2520 6373             {% cs
-00001a10: 7266 5f74 6f6b 656e 2025 7d0d 0a20 2020  rf_token %}..   
-00001a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a30: 203c 696e 7075 7420 7479 7065 3d22 6869   <input type="hi
-00001a40: 6464 656e 2220 7661 6c75 653d 5472 7565  dden" value=True
-00001a50: 206e 616d 653d 2276 6f74 6522 3e0d 0a20   name="vote">.. 
-00001a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a70: 2020 203c 6275 7474 6f6e 2074 7970 653d     <button type=
-00001a80: 2273 7562 6d69 7422 3e79 6573 287b 7b71  "submit">yes({{q
-00001a90: 7565 7374 696f 6e2e 616e 7377 6572 5f73  uestion.answer_s
-00001aa0: 6574 2e66 6972 7374 2e68 656c 7066 756c  et.first.helpful
-00001ab0: 7d7d 293c 2f62 7574 746f 6e3e 0d0a 2020  }})</button>..  
-00001ac0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00001ad0: 666f 726d 3e0d 0a20 2020 2020 2020 2020  form>..         
-00001ae0: 2020 2020 2020 203c 666f 726d 2073 7479         <form sty
-00001af0: 6c65 3d22 6469 7370 6c61 793a 2069 6e6c  le="display: inl
-00001b00: 696e 653b 2220 6163 7469 6f6e 3d22 7b25  ine;" action="{%
-00001b10: 2069 6620 6361 7465 676f 7279 5f65 6e61   if category_ena
-00001b20: 626c 6564 2025 7d7b 2520 7572 6c20 2766  bled %}{% url 'f
-00001b30: 6171 3a76 6f74 655f 616e 7377 6572 2720  aq:vote_answer' 
-00001b40: 7175 6573 7469 6f6e 2e63 6174 6567 6f72  question.categor
-00001b50: 792e 736c 7567 2071 7565 7374 696f 6e2e  y.slug question.
-00001b60: 736c 7567 2071 7565 7374 696f 6e2e 616e  slug question.an
-00001b70: 7377 6572 5f73 6574 2e66 6972 7374 2e73  swer_set.first.s
-00001b80: 6c75 6720 257d 7b25 2065 6c73 6520 257d  lug %}{% else %}
-00001b90: 7b25 2075 726c 2027 6661 713a 766f 7465  {% url 'faq:vote
-00001ba0: 5f61 6e73 7765 7227 2071 7565 7374 696f  _answer' questio
-00001bb0: 6e2e 736c 7567 2071 7565 7374 696f 6e2e  n.slug question.
-00001bc0: 616e 7377 6572 5f73 6574 2e66 6972 7374  answer_set.first
-00001bd0: 2e73 6c75 6720 257d 7b25 2065 6e64 6966  .slug %}{% endif
-00001be0: 2025 7d22 206d 6574 686f 643d 2270 6f73   %}" method="pos
-00001bf0: 7422 3e0d 0a20 2020 2020 2020 2020 2020  t">..           
-00001c00: 2020 2020 2020 2020 207b 2520 6373 7266           {% csrf
-00001c10: 5f74 6f6b 656e 2025 7d0d 0a20 2020 2020  _token %}..     
-00001c20: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00001c30: 696e 7075 7420 7479 7065 3d22 6869 6464  input type="hidd
-00001c40: 656e 2220 7661 6c75 653d 4661 6c73 6520  en" value=False 
-00001c50: 6e61 6d65 3d22 766f 7465 223e 0d0a 2020  name="vote">..  
-00001c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c70: 2020 3c62 7574 746f 6e20 7479 7065 3d22    <button type="
-00001c80: 7375 626d 6974 223e 6e6f 287b 7b71 7565  submit">no({{que
-00001c90: 7374 696f 6e2e 616e 7377 6572 5f73 6574  stion.answer_set
-00001ca0: 2e66 6972 7374 2e6e 6f74 5f68 656c 7066  .first.not_helpf
-00001cb0: 756c 7d7d 293c 2f62 7574 746f 6e3e 0d0a  ul}})</button>..
-00001cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001cd0: 3c2f 666f 726d 3e0d 0a20 2020 2020 2020  </form>..       
-00001ce0: 2020 2020 2020 2020 207b 2520 656e 6469           {% endi
-00001cf0: 6620 257d 0d0a 2020 2020 2020 2020 2020  f %}..          
-00001d00: 2020 7b25 2065 6c73 6520 257d 0d0a 2020    {% else %}..  
-00001d10: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
-00001d20: 2061 6e73 7765 7273 2079 6574 0d0a 2020   answers yet..  
-00001d30: 2020 2020 2020 2020 2020 7b25 2065 6e64            {% end
-00001d40: 6966 2025 7d0d 0a20 2020 2020 2020 207b  if %}..        {
-00001d50: 2520 656e 6469 6620 257d 0d0a 2020 2020  % endif %}..    
-00001d60: 0d0a 2020 2020 0d0a 2020 2020 2020 2020  ..    ..        
-00001d70: 7b25 2069 6620 6361 6e5f 616e 7377 6572  {% if can_answer
-00001d80: 5f71 7565 7374 696f 6e20 257d 0d0a 2020  _question %}..  
-00001d90: 2020 2020 2020 2020 2020 7b25 2069 6620            {% if 
-00001da0: 6361 7465 676f 7279 5f65 6e61 626c 6564  category_enabled
-00001db0: 2025 7d0d 0a20 2020 2020 2020 2020 2020   %}..           
-00001dc0: 2020 2020 203c 6120 6872 6566 3d22 7b25       <a href="{%
-00001dd0: 2075 726c 2027 6661 713a 616e 7377 6572   url 'faq:answer
-00001de0: 5f71 7565 7374 696f 6e27 2071 7565 7374  _question' quest
-00001df0: 696f 6e2e 6361 7465 676f 7279 2e73 6c75  ion.category.slu
-00001e00: 6720 7175 6573 7469 6f6e 2e73 6c75 6720  g question.slug 
-00001e10: 257d 223e 616e 7377 6572 2071 7565 7374  %}">answer quest
-00001e20: 696f 6e3c 2f61 3e0d 0a20 2020 2020 2020  ion</a>..       
-00001e30: 2020 2020 207b 2520 656c 7365 2025 7d0d       {% else %}.
-00001e40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001e50: 203c 6120 6872 6566 3d22 7b25 2075 726c   <a href="{% url
-00001e60: 2027 6661 713a 616e 7377 6572 5f71 7565   'faq:answer_que
-00001e70: 7374 696f 6e27 2071 7565 7374 696f 6e2e  stion' question.
-00001e80: 736c 7567 2025 7d22 3e61 6e73 7765 7220  slug %}">answer 
-00001e90: 7175 6573 7469 6f6e 3c2f 613e 0d0a 2020  question</a>..  
-00001ea0: 2020 2020 2020 2020 2020 7b25 2065 6e64            {% end
-00001eb0: 6966 2025 7d0d 0a20 2020 2020 2020 207b  if %}..        {
-00001ec0: 2520 656e 6469 6620 257d 0d0a 2020 2020  % endif %}..    
-00001ed0: 2020 2020 3c68 723e 0d0a 2020 2020 2020      <hr>..      
-00001ee0: 2020 7b25 2069 6620 636f 6d6d 656e 7473    {% if comments
-00001ef0: 5f61 6c6c 6f77 6564 2025 7d0d 0a20 2020  _allowed %}..   
-00001f00: 2020 2020 2020 2020 207b 2520 696e 636c           {% incl
-00001f10: 7564 6520 2766 6171 2f63 6f6d 6d65 6e74  ude 'faq/comment
-00001f20: 732e 6874 6d6c 2720 257d 0d0a 2020 2020  s.html' %}..    
-00001f30: 2020 2020 7b25 2065 6e64 6966 2025 7d0d      {% endif %}.
-00001f40: 0a20 2020 200d 0a20 2020 2020 2020 207b  .    ..        {
-00001f50: 2520 656e 6462 6c6f 636b 2025 7d0d 0a0d  % endblock %}...
-00001f60: 0a35 2e20 616e 7377 6572 5f66 6f72 6d2e  .5. answer_form.
-00001f70: 6874 6d6c 202d 2066 6f72 6d20 746f 2061  html - form to a
-00001f80: 6464 2061 6e73 7765 7220 746f 2071 7565  dd answer to que
-00001f90: 7374 696f 6e3a 3a0d 0a0d 0a0d 0a20 2020  stion::......   
-00001fa0: 2020 2020 203c 6831 3e41 6e73 7765 7220       <h1>Answer 
-00001fb0: 5175 6573 7469 6f6e 3c2f 6831 3e0d 0a20  Question</h1>.. 
-00001fc0: 2020 2020 2020 203c 6120 6872 6566 3d22         <a href="
-00001fd0: 7b7b 7175 6573 7469 6f6e 2e67 6574 5f61  {{question.get_a
-00001fe0: 6273 6f6c 7574 655f 7572 6c7d 7d22 3e3c  bsolute_url}}"><
-00001ff0: 6833 3e7b 7b71 7565 7374 696f 6e2e 7175  h3>{{question.qu
-00002000: 6573 7469 6f6e 7d7d 3c2f 6833 3e3c 2f61  estion}}</h3></a
-00002010: 3e0d 0a20 2020 2020 2020 203c 666f 726d  >..        <form
-00002020: 206d 6574 686f 643d 2270 6f73 7422 3e0d   method="post">.
-00002030: 0a20 2020 2020 2020 2020 2020 207b 2520  .            {% 
-00002040: 6373 7266 5f74 6f6b 656e 2025 7d0d 0a20  csrf_token %}.. 
-00002050: 2020 2020 2020 2020 2020 207b 7b66 6f72             {{for
-00002060: 6d7d 7d0d 0a20 2020 2020 2020 2020 2020  m}}..           
-00002070: 203c 696e 7075 7420 7479 7065 3d22 7375   <input type="su
-00002080: 626d 6974 223e 0d0a 2020 2020 2020 2020  bmit">..        
-00002090: 3c2f 666f 726d 3e0d 0a0d 0a36 2e20 636f  </form>....6. co
-000020a0: 6d6d 656e 745f 666f 726d 2e68 746d 6c20  mment_form.html 
-000020b0: 2d20 666f 726d 2074 6f20 6164 6420 636f  - form to add co
-000020c0: 6d6d 656e 7473 2074 6f20 7175 6573 7469  mments to questi
-000020d0: 6f6e 2028 6f6e 6c79 2073 686f 7773 2075  on (only shows u
-000020e0: 7020 7768 656e 2066 6f72 6d20 6861 7320  p when form has 
-000020f0: 6572 726f 7220 6265 6361 7573 6520 7669  error because vi
-00002100: 6577 206f 6e6c 7920 6765 7473 2070 6f73  ew only gets pos
-00002110: 7465 6420 746f 293a 3a0d 0a0d 0a0d 0a20  ted to)::...... 
-00002120: 2020 2020 2020 203c 6831 3e50 6f73 7420         <h1>Post 
-00002130: 4120 436f 6d6d 656e 743c 2f68 313e 0d0a  A Comment</h1>..
-00002140: 2020 2020 2020 2020 3c61 2068 7265 663d          <a href=
-00002150: 227b 7b71 7565 7374 696f 6e2e 6765 745f  "{{question.get_
-00002160: 6162 736f 6c75 7465 5f75 726c 7d7d 223e  absolute_url}}">
-00002170: 3c68 333e 7b7b 7175 6573 7469 6f6e 2e71  <h3>{{question.q
-00002180: 7565 7374 696f 6e7d 7d3c 2f68 333e 3c2f  uestion}}</h3></
-00002190: 613e 0d0a 2020 2020 2020 2020 3c66 6f72  a>..        <for
-000021a0: 6d20 6d65 7468 6f64 3d22 706f 7374 223e  m method="post">
-000021b0: 0d0a 2020 2020 2020 2020 2020 2020 7b25  ..            {%
-000021c0: 2063 7372 665f 746f 6b65 6e20 257d 0d0a   csrf_token %}..
-000021d0: 2020 2020 2020 2020 2020 2020 7b7b 666f              {{fo
-000021e0: 726d 7d7d 0d0a 2020 2020 2020 2020 2020  rm}}..          
-000021f0: 2020 3c69 6e70 7574 2074 7970 653d 2273    <input type="s
-00002200: 7562 6d69 7422 3e0d 0a20 2020 2020 2020  ubmit">..       
-00002210: 203c 2f66 6f72 6d3e 0d0a 0d0a 372e 2071   </form>....7. q
-00002220: 7565 7374 696f 6e5f 666f 726d 2e68 746d  uestion_form.htm
-00002230: 6c20 2d20 666f 726d 2074 6f20 6164 6420  l - form to add 
-00002240: 6120 6e65 7720 7175 6573 7469 6f6e 3a3a  a new question::
-00002250: 0d0a 0d0a 0d0a 2020 2020 2020 2020 3c68  ......        <h
-00002260: 313e 4164 6420 596f 7572 2051 7565 7374  1>Add Your Quest
-00002270: 696f 6e3c 2f68 313e 0d0a 2020 2020 2020  ion</h1>..      
-00002280: 2020 3c66 6f72 6d20 6d65 7468 6f64 3d22    <form method="
-00002290: 706f 7374 223e 0d0a 2020 2020 2020 2020  post">..        
-000022a0: 2020 2020 7b25 2063 7372 665f 746f 6b65      {% csrf_toke
-000022b0: 6e20 257d 0d0a 2020 2020 2020 2020 2020  n %}..          
-000022c0: 2020 7b7b 666f 726d 7d7d 0d0a 2020 2020    {{form}}..    
-000022d0: 2020 2020 2020 2020 3c69 6e70 7574 2074          <input t
-000022e0: 7970 653d 2273 7562 6d69 7422 3e0d 0a20  ype="submit">.. 
-000022f0: 2020 2020 2020 203c 2f66 6f72 6d3e 0d0a         </form>..
-00002300: 0d0a 382e 2076 6f74 655f 666f 726d 2e68  ..8. vote_form.h
-00002310: 746d 6c20 2d20 666f 726d 2066 6f72 2076  tml - form for v
-00002320: 6f74 696e 6720 7175 6573 7469 6f6e 7320  oting questions 
-00002330: 616e 6420 616e 7377 6572 7320 286f 6e6c  and answers (onl
-00002340: 7920 7368 6f77 7320 7570 2077 6865 6e20  y shows up when 
-00002350: 666f 726d 2068 6173 2065 7272 6f72 2062  form has error b
-00002360: 6563 6175 7365 2076 6965 7720 6f6e 6c79  ecause view only
-00002370: 2067 6574 7320 706f 7374 6564 2074 6f29   gets posted to)
-00002380: 3a3a 0d0a 0d0a 0d0a 2020 2020 2020 2020  ::......        
-00002390: 3c68 313e 766f 7465 3c2f 6831 3e0d 0a20  <h1>vote</h1>.. 
-000023a0: 2020 2020 2020 203c 666f 726d 206d 6574         <form met
-000023b0: 686f 643d 2270 6f73 7422 3e0d 0a20 2020  hod="post">..   
-000023c0: 2020 2020 2020 2020 207b 2520 6373 7266           {% csrf
-000023d0: 5f74 6f6b 656e 2025 7d0d 0a20 2020 2020  _token %}..     
-000023e0: 2020 2020 2020 207b 7b66 6f72 6d7d 7d0d         {{form}}.
-000023f0: 0a20 2020 2020 2020 2020 2020 203c 696e  .            <in
-00002400: 7075 7420 7479 7065 3d22 7375 626d 6974  put type="submit
-00002410: 223e 0d0a 2020 2020 2020 2020 3c2f 666f  ">..        </fo
-00002420: 726d 3e0d 0a0d 0a39 2e20 636f 6d6d 656e  rm>....9. commen
-00002430: 7473 2e68 746d 6c20 2d20 6966 2063 6f6d  ts.html - if com
-00002440: 6d65 6e74 7320 6172 6520 616c 6c6f 7765  ments are allowe
-00002450: 6420 7468 6973 2074 656d 706c 6174 6520  d this template 
-00002460: 6973 2069 6e63 6c75 6465 6420 696e 2074  is included in t
-00002470: 6865 2071 7565 7374 696f 6e20 6465 7461  he question deta
-00002480: 696c 2e68 746d 6c3a 3a0d 0a0d 0a0d 0a20  il.html::...... 
-00002490: 2020 2020 2020 203c 6833 3e63 6f6d 6d65         <h3>comme
-000024a0: 6e74 733c 2f68 333e 0d0a 2020 2020 2020  nts</h3>..      
-000024b0: 2020 3c75 6c3e 0d0a 2020 2020 2020 2020    <ul>..        
-000024c0: 2020 2020 7b25 2066 6f72 2063 6f6d 6d65      {% for comme
-000024d0: 6e74 2069 6e20 7175 6573 7469 6f6e 2e66  nt in question.f
-000024e0: 6171 636f 6d6d 656e 745f 7365 742e 616c  aqcomment_set.al
-000024f0: 6c20 257d 0d0a 2020 2020 2020 2020 2020  l %}..          
-00002500: 2020 2020 2020 3c6c 693e 3c68 343e 7b7b        <li><h4>{{
-00002510: 636f 6d6d 656e 742e 636f 6d6d 656e 747d  comment.comment}
-00002520: 7d3c 2f68 343e 0d0a 2020 2020 2020 2020  }</h4>..        
-00002530: 2020 2020 2020 2020 2020 2020 706f 7374              post
-00002540: 6564 2062 7920 7b25 2069 6620 636f 6d6d  ed by {% if comm
-00002550: 656e 742e 7573 6572 257d 7b7b 636f 6d6d  ent.user%}{{comm
-00002560: 656e 742e 7573 6572 7d7d 7b25 2065 6c73  ent.user}}{% els
-00002570: 6520 257d 616e 6f6e 796d 6f75 737b 2520  e %}anonymous{% 
-00002580: 656e 6469 6620 257d 207b 7b63 6f6d 6d65  endif %} {{comme
-00002590: 6e74 2e70 6f73 745f 7469 6d65 7c74 696d  nt.post_time|tim
-000025a0: 6573 696e 6365 7d7d 2061 676f 3c2f 6c69  esince}} ago</li
-000025b0: 3e0d 0a20 2020 2020 2020 2020 2020 207b  >..            {
-000025c0: 2520 656e 6466 6f72 2025 7d0d 0a20 2020  % endfor %}..   
-000025d0: 2020 2020 203c 2f75 6c3e 0d0a 2020 2020       </ul>..    
-000025e0: 2020 2020 7b25 2069 6620 6164 645f 6e65      {% if add_ne
-000025f0: 775f 636f 6d6d 656e 745f 616c 6c6f 7765  w_comment_allowe
-00002600: 6420 257d 0d0a 2020 2020 2020 2020 2020  d %}..          
-00002610: 2020 7b25 2069 6620 6361 7465 676f 7279    {% if category
-00002620: 5f65 6e61 626c 6564 2025 7d0d 0a20 2020  _enabled %}..   
-00002630: 2020 2020 2020 2020 203c 666f 726d 206d           <form m
-00002640: 6574 686f 643d 2270 6f73 7422 2061 6374  ethod="post" act
-00002650: 696f 6e3d 227b 2520 7572 6c20 2766 6171  ion="{% url 'faq
-00002660: 3a61 6464 5f63 6f6d 6d65 6e74 2720 7175  :add_comment' qu
-00002670: 6573 7469 6f6e 2e63 6174 6567 6f72 792e  estion.category.
-00002680: 736c 7567 2071 7565 7374 696f 6e2e 736c  slug question.sl
-00002690: 7567 2025 7d22 3e0d 0a20 2020 2020 2020  ug %}">..       
-000026a0: 2020 2020 207b 2520 656c 7365 2025 7d0d       {% else %}.
-000026b0: 0a20 2020 2020 2020 2020 2020 203c 666f  .            <fo
-000026c0: 726d 206d 6574 686f 643d 2270 6f73 7422  rm method="post"
-000026d0: 2061 6374 696f 6e3d 227b 2520 7572 6c20   action="{% url 
-000026e0: 2766 6171 3a61 6464 5f63 6f6d 6d65 6e74  'faq:add_comment
-000026f0: 2720 7175 6573 7469 6f6e 2e73 6c75 6720  ' question.slug 
-00002700: 257d 223e 0d0a 2020 2020 2020 2020 2020  %}">..          
-00002710: 2020 7b25 2065 6e64 6966 2025 7d0d 0a20    {% endif %}.. 
-00002720: 2020 2020 2020 2020 2020 203c 6669 656c             <fiel
-00002730: 6473 6574 3e0d 0a20 2020 2020 2020 2020  dset>..         
-00002740: 2020 2020 2020 203c 6c65 6765 6e64 3e50         <legend>P
-00002750: 6f73 7420 596f 7572 2043 6f6d 6d65 6e74  ost Your Comment
-00002760: 2048 6572 653a 3c2f 6c65 6765 6e64 3e0d   Here:</legend>.
-00002770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002780: 207b 2520 6373 7266 5f74 6f6b 656e 2025   {% csrf_token %
-00002790: 7d0d 0a20 2020 2020 2020 2020 2020 2020  }..             
-000027a0: 2020 207b 7b63 6f6d 6d65 6e74 5f66 6f72     {{comment_for
-000027b0: 6d7d 7d0d 0a20 2020 2020 2020 2020 2020  m}}..           
-000027c0: 2020 2020 203c 696e 7075 7420 7479 7065       <input type
-000027d0: 3d22 7375 626d 6974 2220 6e61 6d65 3d22  ="submit" name="
-000027e0: 706f 7374 223e 0d0a 2020 2020 2020 2020  post">..        
-000027f0: 2020 2020 3c2f 6669 656c 6473 6574 3e0d      </fieldset>.
-00002800: 0a20 2020 2020 2020 2020 2020 203c 2f66  .            </f
-00002810: 6f72 6d3e 0d0a 2020 2020 2020 2020 7b25  orm>..        {%
-00002820: 2065 6e64 6966 2025 7d0d 0a0d 0a23 2320   endif %}....## 
-00002830: 5465 6d70 6c61 7465 2056 6172 6961 626c  Template Variabl
-00002840: 6573 0d0a 0d0a 312e 2063 6174 6567 6f72  es....1. categor
-00002850: 6965 735f 6c69 7374 2e68 746d 6c0d 0a20  ies_list.html.. 
-00002860: 2020 2063 6174 6567 6f72 6965 7320 2d20     categories - 
-00002870: 616c 6c20 7468 6520 6361 7465 676f 7269  all the categori
-00002880: 6573 2028 6361 7465 676f 7279 2071 7565  es (category que
-00002890: 7279 7365 7429 0d0a 0d0a 322e 2063 6174  ryset)....2. cat
-000028a0: 6567 6f72 6965 735f 6465 7461 696c 2e68  egories_detail.h
-000028b0: 746d 6c0d 0a20 2020 2063 6174 6567 6f72  tml..    categor
-000028c0: 7920 2d20 7468 6520 6361 7465 676f 7279  y - the category
-000028d0: 2063 686f 7365 6e20 2863 6174 6567 6f72   chosen (categor
-000028e0: 7920 6f62 6a65 6374 290d 0a20 2020 2063  y object)..    c
-000028f0: 616e 5f61 6464 5f71 7565 7374 696f 6e20  an_add_question 
-00002900: 2d20 626f 6f6c 2069 6620 7468 6520 7573  - bool if the us
-00002910: 6572 2063 616e 2061 6464 2061 2071 7565  er can add a que
-00002920: 7374 696f 6e20 2864 6570 656e 6473 206f  stion (depends o
-00002930: 6e20 7468 6520 7365 7474 696e 6773 290d  n the settings).
-00002940: 0a33 2e20 7175 6573 7469 6f6e 735f 6c69  .3. questions_li
-00002950: 7374 2e68 746d 6c0d 0a20 2020 2071 7565  st.html..    que
-00002960: 7374 696f 6e73 202d 2061 6c6c 2074 6865  stions - all the
-00002970: 2071 7565 7374 696f 6e73 2028 7175 6573   questions (ques
-00002980: 7469 6f6e 2071 7565 7279 7365 7429 0d0a  tion queryset)..
-00002990: 2020 2020 6361 6e5f 6164 645f 7175 6573      can_add_ques
-000029a0: 7469 6f6e 202d 2062 6f6f 6c20 6966 2074  tion - bool if t
-000029b0: 6865 2075 7365 7220 6361 6e20 6164 6420  he user can add 
-000029c0: 6120 7175 6573 7469 6f6e 2028 6465 7065  a question (depe
-000029d0: 6e64 7320 6f6e 2074 6865 2073 6574 7469  nds on the setti
-000029e0: 6e67 7329 0d0a 342e 2071 7565 7374 696f  ngs)..4. questio
-000029f0: 6e5f 6465 7461 696c 2e68 746d 6c0d 0a20  n_detail.html.. 
-00002a00: 2020 2071 7565 7374 696f 6e20 2d20 7468     question - th
-00002a10: 6520 7175 6573 7469 6f6e 2063 686f 7365  e question chose
-00002a20: 6e20 2871 7565 7374 696f 6e20 6f62 6a65  n (question obje
-00002a30: 6374 290d 0a20 2020 2063 616e 5f76 6f74  ct)..    can_vot
-00002a40: 655f 7175 6573 7469 6f6e 202d 2062 6f6f  e_question - boo
-00002a50: 6c20 6966 2074 6865 2075 7365 7220 6361  l if the user ca
-00002a60: 6e20 766f 7465 2061 2071 7565 7374 696f  n vote a questio
-00002a70: 6e20 2864 6570 656e 6473 206f 6e20 7468  n (depends on th
-00002a80: 6520 7365 7474 696e 6773 290d 0a20 2020  e settings)..   
-00002a90: 2063 6174 6567 6f72 795f 656e 6162 6c65   category_enable
-00002aa0: 6420 2d20 626f 6f6c 2069 6620 6361 7465  d - bool if cate
-00002ab0: 676f 7279 2065 6e61 626c 6564 2069 6e20  gory enabled in 
-00002ac0: 7365 7474 696e 6773 0d0a 2020 2020 616c  settings..    al
-00002ad0: 6c6f 775f 6d75 6c74 6970 6c65 5f61 6e73  low_multiple_ans
-00002ae0: 7765 7273 202d 2062 6f6f 6c20 6966 206d  wers - bool if m
-00002af0: 756c 7469 706c 6520 616e 7377 6572 7320  ultiple answers 
-00002b00: 616c 6c6f 7765 6420 696e 2073 6574 7469  allowed in setti
-00002b10: 6e67 730d 0a20 2020 2063 616e 5f76 6f74  ngs..    can_vot
-00002b20: 655f 616e 7377 6572 202d 2062 6f6f 6c20  e_answer - bool 
-00002b30: 6966 2074 6865 2075 7365 7220 6361 6e20  if the user can 
-00002b40: 766f 7465 2061 6e20 616e 7377 6572 2028  vote an answer (
-00002b50: 6465 7065 6e64 7320 6f6e 2074 6865 2073  depends on the s
-00002b60: 6574 7469 6e67 7329 0d0a 2020 2020 6361  ettings)..    ca
-00002b70: 6e5f 616e 7377 6572 5f71 7565 7374 696f  n_answer_questio
-00002b80: 6e20 2d20 626f 6f6c 2069 6620 6375 7272  n - bool if curr
-00002b90: 656e 7420 7573 6572 2063 616e 2061 6e73  ent user can ans
-00002ba0: 7765 7220 7175 6573 7469 6f6e 2028 6465  wer question (de
-00002bb0: 7065 6e64 7320 6f6e 2074 6865 2073 6574  pends on the set
-00002bc0: 7469 6e67 7329 0d0a 2020 2020 636f 6d6d  tings)..    comm
-00002bd0: 656e 7473 5f61 6c6c 6f77 6564 202d 2062  ents_allowed - b
-00002be0: 6f6f 6c20 6966 2075 7369 6e67 2063 6f6d  ool if using com
-00002bf0: 6d65 6e74 7320 696e 2073 6574 7469 6e67  ments in setting
-00002c00: 730d 0a20 2020 2061 6464 5f6e 6577 5f63  s..    add_new_c
-00002c10: 6f6d 6d65 6e74 5f61 6c6c 6f77 6564 202d  omment_allowed -
-00002c20: 2062 6f6f 6c20 6966 2063 7572 7265 6e74   bool if current
-00002c30: 2075 7365 7220 6361 6e20 6164 6420 636f   user can add co
-00002c40: 6d6d 656e 7420 2864 6570 656e 6473 206f  mment (depends o
-00002c50: 6e20 7468 6520 7365 7474 696e 6773 290d  n the settings).
-00002c60: 0a20 2020 2063 6f6d 6d65 6e74 5f66 6f72  .    comment_for
-00002c70: 6d20 2d20 666f 726d 2074 6f20 7375 626d  m - form to subm
-00002c80: 6974 2061 206e 6577 2063 6f6d 6d65 6e74  it a new comment
-00002c90: 0d0a 352e 2061 6e73 7765 725f 666f 726d  ..5. answer_form
-00002ca0: 2e68 746d 6c0d 0a20 2020 2071 7565 7374  .html..    quest
-00002cb0: 696f 6e20 2d20 7468 6520 7175 6573 7469  ion - the questi
-00002cc0: 6f6e 2074 6f20 6164 6420 616e 7377 6572  on to add answer
-00002cd0: 2074 6f20 2871 7565 7374 696f 6e20 6f62   to (question ob
-00002ce0: 6a65 6374 290d 0a20 2020 2066 6f72 6d20  ject)..    form 
-00002cf0: 2d20 666f 726d 2074 6f20 6164 6420 6e65  - form to add ne
-00002d00: 7720 616e 7377 6572 0d0a 362e 2063 6f6d  w answer..6. com
-00002d10: 6d65 6e74 5f66 6f72 6d2e 6874 6d6c 0d0a  ment_form.html..
-00002d20: 2020 2020 7175 6573 7469 6f6e 202d 2074      question - t
-00002d30: 6865 2071 7565 7374 696f 6e20 746f 2061  he question to a
-00002d40: 6464 2063 6f6d 6d65 6e74 2074 6f20 2871  dd comment to (q
-00002d50: 7565 7374 696f 6e20 6f62 6a65 6374 290d  uestion object).
-00002d60: 0a20 2020 2066 6f72 6d20 2d20 666f 726d  .    form - form
-00002d70: 2074 6f20 6164 6420 6e65 7720 636f 6d6d   to add new comm
-00002d80: 656e 740d 0a37 2e20 7175 6573 7469 6f6e  ent..7. question
-00002d90: 5f66 6f72 6d2e 6874 6d6c 0d0a 2020 2020  _form.html..    
-00002da0: 666f 726d 202d 2066 6f72 6d20 746f 2061  form - form to a
-00002db0: 6464 206e 6577 2071 7565 7374 696f 6e0d  dd new question.
-00002dc0: 0a38 2e20 766f 7465 5f66 6f72 6d2e 6874  .8. vote_form.ht
-00002dd0: 6d6c 0d0a 2020 2020 666f 726d 202d 2066  ml..    form - f
-00002de0: 6f72 6d20 746f 2076 6f74 6520 666f 7220  orm to vote for 
-00002df0: 6120 7175 6573 7469 6f6e 206f 7220 616e  a question or an
-00002e00: 7377 6572 0d0a 0d0a 2323 2055 726c 730d  swer....## Urls.
-00002e10: 0a0d 0a61 6c6c 206f 6620 7468 6520 666f  ...all of the fo
-00002e20: 6c6c 6f77 696e 6720 7572 6c73 2061 7265  llowing urls are
-00002e30: 2062 7920 6e61 6d65 2074 6865 6e20 6164   by name then ad
-00002e40: 6469 7469 6f6e 616c 0d0a 7468 6520 6170  ditional..the ap
-00002e50: 7020 6e61 6d65 2066 6f72 2074 6865 2075  p name for the u
-00002e60: 726c 7320 6973 2060 6027 6661 7127 6060  rls is ``'faq'``
-00002e70: 0d0a 0d0a 2a20 696e 6465 785f 7669 6577  ....* index_view
-00002e80: 0d0a 2020 2020 2a20 6e6f 2061 7267 756d  ..    * no argum
-00002e90: 656e 7473 0d0a 2020 2020 2a20 6469 7370  ents..    * disp
-00002ea0: 6c61 7973 2061 6c6c 2074 6865 2063 6174  lays all the cat
-00002eb0: 6567 6f72 6965 7320 6966 2063 6174 6567  egories if categ
-00002ec0: 6f72 6965 7320 6172 6520 656e 6162 6c65  ories are enable
-00002ed0: 6420 6f74 6865 7277 6973 6520 7368 6f77  d otherwise show
-00002ee0: 7320 7175 6573 7469 6f6e 730d 0a2a 2063  s questions..* c
-00002ef0: 6174 6567 6f72 795f 6465 7461 696c 0d0a  ategory_detail..
-00002f00: 2020 2020 2a20 6e65 6564 7320 6361 7465      * needs cate
-00002f10: 676f 7279 2073 6c75 6720 6173 2073 6c75  gory slug as slu
-00002f20: 670d 0a20 2020 202a 2064 6973 706c 6179  g..    * display
-00002f30: 7320 616c 6c20 7468 6520 7175 6573 7469  s all the questi
-00002f40: 6f6e 7320 6769 7665 6e20 7468 6520 6361  ons given the ca
-00002f50: 7465 676f 7279 2077 6865 6e20 6361 7465  tegory when cate
-00002f60: 676f 7269 6573 2061 7265 2065 6e61 626c  gories are enabl
-00002f70: 6564 0d0a 2a20 6164 645f 7175 6573 7469  ed..* add_questi
-00002f80: 6f6e 0d0a 2020 2020 2a20 6966 2063 6174  on..    * if cat
-00002f90: 6567 6f72 6965 7320 6172 6520 656e 6162  egories are enab
-00002fa0: 6c65 6420 6e65 6564 7320 6361 7465 676f  led needs catego
-00002fb0: 7279 2073 6c75 6720 6173 2073 6c75 670d  ry slug as slug.
-00002fc0: 0a20 2020 202a 2069 6620 6c6f 6767 6564  .    * if logged
-00002fd0: 5f69 6e5f 7573 6572 735f 6361 6e5f 6164  _in_users_can_ad
-00002fe0: 645f 7175 6573 7469 6f6e 2074 6865 6e20  d_question then 
-00002ff0: 6469 7370 6c61 7973 2066 6f72 6d20 666f  displays form fo
-00003000: 7220 6c6f 6767 6564 2069 6e20 7573 6572  r logged in user
-00003010: 7320 746f 2061 736b 2061 206e 6577 2071  s to ask a new q
-00003020: 7565 7374 696f 6e0d 0a2a 2071 7565 7374  uestion..* quest
-00003030: 696f 6e5f 6465 7461 696c 0d0a 2020 2020  ion_detail..    
-00003040: 2a20 6e65 6564 7320 7175 6573 7469 6f6e  * needs question
-00003050: 2073 6c75 6720 6173 2071 7565 7374 696f   slug as questio
-00003060: 6e20 7c20 6966 2063 6174 6567 6f72 6965  n | if categorie
-00003070: 7320 6172 6520 656e 6162 6c65 6420 6e65  s are enabled ne
-00003080: 6564 7320 6361 7465 676f 7279 2073 6c75  eds category slu
-00003090: 6720 6173 2073 6c75 670d 0a20 2020 202a  g as slug..    *
-000030a0: 2064 6973 706c 6179 7320 7468 6520 6d61   displays the ma
-000030b0: 696e 2046 4151 2070 6167 6520 7769 7468  in FAQ page with
-000030c0: 2074 6865 2071 7565 7374 696f 6e20 616c   the question al
-000030d0: 6c20 7468 6520 636f 6d6d 656e 7473 2061  l the comments a
-000030e0: 6e64 2061 6e73 7765 7273 0d0a 2a20 616e  nd answers..* an
-000030f0: 7377 6572 5f71 7565 7374 696f 6e0d 0a20  swer_question.. 
-00003100: 2020 202a 206e 6565 6473 2071 7565 7374     * needs quest
-00003110: 696f 6e20 736c 7567 2061 7320 7175 6573  ion slug as ques
-00003120: 7469 6f6e 207c 2069 6620 6361 7465 676f  tion | if catego
-00003130: 7269 6573 2061 7265 2065 6e61 626c 6564  ries are enabled
-00003140: 206e 6565 6473 2063 6174 6567 6f72 7920   needs category 
-00003150: 736c 7567 2061 7320 6361 7465 676f 7279  slug as category
-00003160: 0d0a 2020 2020 2a20 6469 7370 6c61 7973  ..    * displays
-00003170: 2074 6865 2061 6e73 7765 7220 7175 6573   the answer ques
-00003180: 7469 6f6e 2066 6f72 6d0d 0a2a 2061 6464  tion form..* add
-00003190: 5f63 6f6d 6d65 6e74 0d0a 2020 2020 2a20  _comment..    * 
-000031a0: 6e65 6564 7320 7175 6573 7469 6f6e 2073  needs question s
-000031b0: 6c75 6720 6173 2071 7565 7374 696f 6e20  lug as question 
-000031c0: 7c20 6966 2063 6174 6567 6f72 6965 7320  | if categories 
-000031d0: 6172 6520 656e 6162 6c65 6420 6e65 6564  are enabled need
-000031e0: 7320 6361 7465 676f 7279 2073 6c75 6720  s category slug 
-000031f0: 6173 2063 6174 6567 6f72 790d 0a20 2020  as category..   
-00003200: 202a 206f 6e6c 7920 776f 726b 7320 6966   * only works if
-00003210: 2075 7369 6e67 2063 6f6d 6d65 6e74 730d   using comments.
-00003220: 0a20 2020 202a 2075 7365 6420 746f 2070  .    * used to p
-00003230: 6f73 7420 636f 6d6d 656e 7420 666f 726d  ost comment form
-00003240: 2066 726f 6d20 7175 6573 7469 6f6e 5f64   from question_d
-00003250: 6574 6169 6c20 746f 2064 6174 6162 6173  etail to databas
-00003260: 650d 0a2a 2076 6f74 655f 616e 7377 6572  e..* vote_answer
-00003270: 0d0a 2020 2020 2a20 6e65 6564 7320 7175  ..    * needs qu
-00003280: 6573 7469 6f6e 2073 6c75 6720 6173 2071  estion slug as q
-00003290: 7565 7374 696f 6e20 7c20 6e65 6564 7320  uestion | needs 
-000032a0: 616e 7377 6572 2073 6c75 6720 6173 2061  answer slug as a
-000032b0: 6e73 7765 7220 7c20 6966 2063 6174 6567  nswer | if categ
-000032c0: 6f72 6965 7320 6172 6520 656e 6162 6c65  ories are enable
-000032d0: 6420 6e65 6564 7320 6361 7465 676f 7279  d needs category
-000032e0: 2073 6c75 6720 6173 2063 6174 6567 6f72   slug as categor
-000032f0: 790d 0a20 2020 202a 206f 6e6c 7920 776f  y..    * only wo
-00003300: 726b 7320 6966 2075 7369 6e67 2061 6e73  rks if using ans
-00003310: 7765 7220 766f 7469 6e67 0d0a 2020 2020  wer voting..    
-00003320: 2a20 7573 6564 2074 6f20 706f 7374 2068  * used to post h
-00003330: 6964 6465 6e20 696e 7075 7420 766f 7465  idden input vote
-00003340: 203d 2031 206f 7220 766f 7465 203d 2030   = 1 or vote = 0
-00003350: 2064 6570 656e 6469 6e67 206f 6e20 766f   depending on vo
-00003360: 7465 2075 7020 6f72 2064 6f77 6e0d 0a2a  te up or down..*
-00003370: 2076 6f74 655f 7175 6573 7469 6f6e 0d0a   vote_question..
-00003380: 2020 2020 2a20 6e65 6564 7320 7175 6573      * needs ques
-00003390: 7469 6f6e 2073 6c75 6720 6173 2071 7565  tion slug as que
-000033a0: 7374 696f 6e20 7c20 6966 2063 6174 6567  stion | if categ
-000033b0: 6f72 6965 7320 6172 6520 656e 6162 6c65  ories are enable
-000033c0: 6420 6e65 6564 7320 6361 7465 676f 7279  d needs category
-000033d0: 2073 6c75 6720 6173 2063 6174 6567 6f72   slug as categor
-000033e0: 790d 0a20 2020 202a 206f 6e6c 7920 776f  y..    * only wo
-000033f0: 726b 7320 6966 2075 7369 6e67 2071 7565  rks if using que
-00003400: 7374 696f 6e20 766f 7469 6e67 0d0a 2020  stion voting..  
-00003410: 2020 2a20 7573 6564 2074 6f20 706f 7374    * used to post
-00003420: 2068 6964 6465 6e20 696e 7075 7420 766f   hidden input vo
-00003430: 7465 203d 2031 206f 7220 766f 7465 203d  te = 1 or vote =
-00003440: 2030 2064 6570 656e 6469 6e67 206f 6e20   0 depending on 
-00003450: 766f 7465 2075 7020 6f72 2064 6f77 6e0d  vote up or down.
-00003460: 0a0d 0a23 2320 436f 6e74 7269 6275 7469  ...## Contributi
-00003470: 6e67 0d0a 0d0a 646a 616e 676f 2d65 6173  ng....django-eas
-00003480: 792d 6661 7120 6169 6d73 2074 6f20 6265  y-faq aims to be
-00003490: 2074 6865 2062 6573 7420 6661 7120 6170   the best faq ap
-000034a0: 7020 666f 7220 646a 616e 676f 2e20 4974  p for django. It
-000034b0: 2077 656c 636f 6d65 7320 2063 6f6e 7472   welcomes  contr
-000034c0: 6962 7574 696f 6e73 206f 6620 616c 6c20  ibutions of all 
-000034d0: 7479 7065 7320 2d20 6973 7375 6573 2c20  types - issues, 
-000034e0: 6275 6773 2c20 6665 6174 7572 6520 7265  bugs, feature re
-000034f0: 7175 6573 7473 2c20 646f 6375 6d65 6e74  quests, document
-00003500: 6174 696f 6e20 7570 6461 7465 732c 2074  ation updates, t
-00003510: 6573 7473 2061 6e64 2070 756c 6c20 7265  ests and pull re
-00003520: 7175 6573 7473 0d0a 0d0a 2323 2063 6861  quests....## cha
-00003530: 6e67 6520 6c6f 670d 0a30 2e34 2066 6978  nge log..0.4 fix
-00003540: 6564 2062 7567 2074 6861 7420 6c6f 6767  ed bug that logg
-00003550: 6564 206f 7574 2075 7365 7273 2063 616e  ed out users can
-00003560: 2076 6f74 6520 2d20 7768 6963 6820 7468   vote - which th
-00003570: 656e 2072 6169 7365 7320 6578 6365 7074  en raises except
-00003580: 696f 6e73 0d0a 0d0a 302e 3520 6669 7865  ions....0.5 fixe
-00003590: 6420 6d69 6772 6174 696f 6e73 0d0a 0d0a  d migrations....
-000035a0: 312e 3020 6164 6465 6420 7079 7069 2064  1.0 added pypi d
-000035b0: 6973 7472 6962 7574 696f 6e0d 0a0d 0a31  istribution....1
-000035c0: 2e31 2061 6464 6564 206d 6f72 6520 7465  .1 added more te
-000035d0: 6d70 6c61 7465 7320 746f 206f 7665 7272  mplates to overr
-000035e0: 6964 6520 6561 7369 6c79 0d0a 0d0a 312e  ide easily....1.
-000035f0: 3220 6669 7865 6420 6275 6720 696e 2070  2 fixed bug in p
-00003600: 7970 6920 6469 7374 726f 206e 6f74 2069  ypi distro not i
-00003610: 6e63 6c75 6469 6e67 2066 6171 2061 7070  ncluding faq app
-00003620: 0d0a 0d0a 312e 3320 6669 7865 6420 6275  ....1.3 fixed bu
-00003630: 6720 7768 6572 6520 6120 736c 7567 206d  g where a slug m
-00003640: 7573 7420 6265 2066 696c 6c65 6420 6f75  ust be filled ou
-00003650: 7420 696e 2061 646d 696e 2065 7665 6e20  t in admin even 
-00003660: 7468 6f75 6768 2073 6c75 6720 6765 7473  though slug gets
-00003670: 2061 7574 6f20 6765 6e65 7261 7465 6420   auto generated 
-00003680: 746f 2073 6176 6520 666f 7220 7175 6573  to save for ques
-00003690: 7469 6f6e 732c 2061 6e73 7765 7273 2c20  tions, answers, 
-000036a0: 616e 6420 6361 7465 676f 7269 6573 2e20  and categories. 
-000036b0: 6d61 6465 2071 7565 7374 696f 6e73 2c20  made questions, 
-000036c0: 616e 7377 6572 732c 2063 6174 6567 6f72  answers, categor
-000036d0: 6965 7320 736c 7567 7320 7265 6164 6f6e  ies slugs readon
-000036e0: 6c79 2069 6e20 6164 6d69 6e0d 0a0d 0a31  ly in admin....1
-000036f0: 2e34 2061 6464 6564 2075 6e69 636f 6465  .4 added unicode
-00003700: 206f 7074 696f 6e20 746f 2061 6464 2075   option to add u
-00003710: 6e69 636f 6465 2073 6c75 6773 0d0a 0d0a  nicode slugs....
-00003720: 312e 3520 6164 6465 6420 6c6f 6769 6e5f  1.5 added login_
-00003730: 7265 7175 6972 6564 2073 6574 7469 6e67  required setting
-00003740: 2074 6f20 616c 6c6f 7720 6661 7120 6170   to allow faq ap
-00003750: 7020 746f 2062 6520 6176 6169 6c61 626c  p to be availabl
-00003760: 6520 746f 206f 6e6c 7920 6c6f 6767 6564  e to only logged
-00003770: 2069 6e20 7573 6572 730d 0a0d 0a31 2e36   in users....1.6
-00003780: 2066 6978 6564 2062 7567 2077 6865 7265   fixed bug where
-00003790: 206e 6f5f 6361 7465 676f 7279 5f64 6573   no_category_des
-000037a0: 6372 6970 7469 6f6e 2064 6964 206e 6f74  cription did not
-000037b0: 2064 6f20 7265 6d6f 7665 2074 6865 2063   do remove the c
-000037c0: 6174 6567 6f72 7920 6465 7363 7269 7074  ategory descript
-000037d0: 696f 6e20 696e 2074 6865 2061 646d 696e  ion in the admin
-000037e0: 0d0a 0d0a 312e 3720 6164 6465 6420 7375  ....1.7 added su
-000037f0: 7070 6f72 7420 666f 7220 646a 616e 676f  pport for django
-00003800: 2035 2e30                                 5.0
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 646a 616e  : 2.1.Name: djan
+00000020: 676f 2d65 6173 792d 6661 710a 5665 7273  go-easy-faq.Vers
+00000030: 696f 6e3a 2031 2e38 0a53 756d 6d61 7279  ion: 1.8.Summary
+00000040: 3a20 4120 446a 616e 676f 2061 7070 2074  : A Django app t
+00000050: 6f20 6164 6420 6772 6561 7420 4641 5120  o add great FAQ 
+00000060: 6675 6e63 7469 6f6e 616c 6974 7920 746f  functionality to
+00000070: 2077 6562 7369 7465 0a48 6f6d 652d 7061   website.Home-pa
+00000080: 6765 3a20 6874 7470 733a 2f2f 6769 7468  ge: https://gith
+00000090: 7562 2e63 6f6d 2f73 6d61 726b 2d31 2f64  ub.com/smark-1/d
+000000a0: 6a61 6e67 6f2d 6561 7379 2d66 6171 2f0a  jango-easy-faq/.
+000000b0: 446f 776e 6c6f 6164 2d55 524c 3a20 6874  Download-URL: ht
+000000c0: 7470 733a 2f2f 7079 7069 2e70 7974 686f  tps://pypi.pytho
+000000d0: 6e2e 6f72 672f 7079 7069 2f64 6a61 6e67  n.org/pypi/djang
+000000e0: 6f2d 6561 7379 2d66 6171 0a4c 6963 656e  o-easy-faq.Licen
+000000f0: 7365 3a20 4d49 540a 4b65 7977 6f72 6473  se: MIT.Keywords
+00000100: 3a20 646a 616e 676f 2c66 6171 0a43 6c61  : django,faq.Cla
+00000110: 7373 6966 6965 723a 2049 6e74 656e 6465  ssifier: Intende
+00000120: 6420 4175 6469 656e 6365 203a 3a20 4465  d Audience :: De
+00000130: 7665 6c6f 7065 7273 0a43 6c61 7373 6966  velopers.Classif
+00000140: 6965 723a 204c 6963 656e 7365 203a 3a20  ier: License :: 
+00000150: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
+00000160: 4d49 5420 4c69 6365 6e73 650a 436c 6173  MIT License.Clas
+00000170: 7369 6669 6572 3a20 4f70 6572 6174 696e  sifier: Operatin
+00000180: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
+00000190: 6e64 6570 656e 6465 6e74 0a43 6c61 7373  ndependent.Class
+000001a0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+000001b0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000001c0: 7974 686f 6e20 3a3a 2033 0a43 6c61 7373  ython :: 3.Class
+000001d0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+000001e0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000001f0: 7974 686f 6e20 3a3a 2033 2e39 0a43 6c61  ython :: 3.9.Cla
+00000200: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+00000210: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000220: 2050 7974 686f 6e20 3a3a 2033 2e31 300a   Python :: 3.10.
+00000230: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+00000240: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000250: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000260: 3131 0a43 6c61 7373 6966 6965 723a 2050  11.Classifier: P
+00000270: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000280: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000290: 2033 2e31 320a 436c 6173 7369 6669 6572   3.12.Classifier
+000002a0: 3a20 4672 616d 6577 6f72 6b20 3a3a 2044  : Framework :: D
+000002b0: 6a61 6e67 6f0a 5265 7175 6972 6573 2d50  jango.Requires-P
+000002c0: 7974 686f 6e3a 203e 3d33 2e39 0a44 6573  ython: >=3.9.Des
+000002d0: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
+000002e0: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
+000002f0: 646f 776e 0a4c 6963 656e 7365 2d46 696c  down.License-Fil
+00000300: 653a 204c 4943 454e 5345 0a52 6571 7569  e: LICENSE.Requi
+00000310: 7265 732d 4469 7374 3a20 446a 616e 676f  res-Dist: Django
+00000320: 3e3d 332e 320a 0a23 2064 6a61 6e67 6f2d  >=3.2..# django-
+00000330: 6561 7379 2d66 6171 0a0a 646a 616e 676f  easy-faq..django
+00000340: 2d65 6173 792d 6661 7120 6973 2061 2044  -easy-faq is a D
+00000350: 6a61 6e67 6f20 6170 7020 746f 2061 6c6c  jango app to all
+00000360: 6f77 2066 6f72 2061 2073 696d 706c 6520  ow for a simple 
+00000370: 7965 7420 6665 6174 7572 6520 7269 6368  yet feature rich
+00000380: 2066 6171 2061 7070 2e20 7769 7468 2063   faq app. with c
+00000390: 6174 6567 6f72 6965 732c 2063 6f6d 6d65  ategories, comme
+000003a0: 6e74 696e 6720 766f 7469 6e67 206f 6620  nting voting of 
+000003b0: 7175 6573 7469 6f6e 7320 616e 6420 616e  questions and an
+000003c0: 7377 6572 7320 616c 6c20 6173 2061 6e20  swers all as an 
+000003d0: 6f70 7469 6f6e 616c 2070 6172 7420 6f66  optional part of
+000003e0: 2074 6865 2061 7070 2e20 546f 2073 6565   the app. To see
+000003f0: 2073 6372 6565 6e73 686f 7473 206f 6620   screenshots of 
+00000400: 7768 6174 2074 6869 7320 646a 616e 676f  what this django
+00000410: 2d65 6173 792d 6661 7120 636f 756c 6420  -easy-faq could 
+00000420: 6c6f 6f6b 206c 696b 6520 7769 7468 2062  look like with b
+00000430: 6f6f 7473 7472 6170 2035 2073 7479 6c69  ootstrap 5 styli
+00000440: 6e67 205b 636c 6963 6b20 6865 7265 5d28  ng [click here](
+00000450: 6465 6d6f 2f64 656d 6f2e 6d64 292e 0a0a  demo/demo.md)...
+00000460: 0a23 2320 5175 6963 6b20 7374 6172 740a  .## Quick start.
+00000470: 0a31 2e20 7069 7020 696e 7374 616c 6c3a  .1. pip install:
+00000480: 0a0a 2020 2020 6070 6970 2069 6e73 7461  ..    `pip insta
+00000490: 6c6c 2064 6a61 6e67 6f2d 6561 7379 2d66  ll django-easy-f
+000004a0: 6171 600a 0a32 2e20 4164 6420 2266 6171  aq`..2. Add "faq
+000004b0: 2220 746f 2079 6f75 7220 494e 5354 414c  " to your INSTAL
+000004c0: 4c45 445f 4150 5053 2073 6574 7469 6e67  LED_APPS setting
+000004d0: 206c 696b 6520 7468 6973 3a0a 0a20 2020   like this:..   
+000004e0: 2060 6060 7079 7468 6f6e 0a20 2020 2049   ```python.    I
+000004f0: 4e53 5441 4c4c 4544 5f41 5050 5320 3d20  NSTALLED_APPS = 
+00000500: 5b0a 2020 2020 2020 2020 2e2e 2e0a 2020  [.        ....  
+00000510: 2020 2020 2020 2766 6171 272c 5d0a 2020        'faq',].  
+00000520: 2020 6060 600a 0a33 2e20 496e 636c 7564    ```..3. Includ
+00000530: 6520 7468 6520 6561 7379 2d66 6171 2055  e the easy-faq U
+00000540: 524c 636f 6e66 2069 6e20 796f 7572 2070  RLconf in your p
+00000550: 726f 6a65 6374 2075 726c 732e 7079 206c  roject urls.py l
+00000560: 696b 6520 7468 6973 3a3a 0a0a 2020 2020  ike this::..    
+00000570: 6060 6070 7974 686f 6e0a 2020 2020 23e2  ```python.    #.
+00000580: 80a6 0a20 2020 2070 6174 6828 2766 6171  ...    path('faq
+00000590: 2f27 2c20 696e 636c 7564 6528 2766 6171  /', include('faq
+000005a0: 2e75 726c 7327 2929 2c0a 2020 2020 23e2  .urls')),.    #.
+000005b0: 80a6 0a20 2020 2060 6060 0a0a 342e 2041  ...    ```..4. A
+000005c0: 6464 2060 4641 515f 5345 5454 494e 4753  dd `FAQ_SETTINGS
+000005d0: 203d 205b 5d60 2074 6f20 796f 7572 2060   = []` to your `
+000005e0: 7365 7474 696e 6773 2e70 7960 0a35 2e20  settings.py`.5. 
+000005f0: 5275 6e20 6060 7079 7468 6f6e 206d 616e  Run ``python man
+00000600: 6167 652e 7079 206d 616b 656d 6967 7261  age.py makemigra
+00000610: 7469 6f6e 7360 6020 746f 2063 7265 6174  tions`` to creat
+00000620: 6520 7468 6520 6661 7120 6d6f 6465 6c73  e the faq models
+00000630: 206d 6967 7261 7469 6f6e 732e 0a36 2e20   migrations..6. 
+00000640: 5275 6e20 6060 7079 7468 6f6e 206d 616e  Run ``python man
+00000650: 6167 652e 7079 206d 6967 7261 7465 6060  age.py migrate``
+00000660: 2074 6f20 6372 6561 7465 2074 6865 2066   to create the f
+00000670: 6171 206d 6f64 656c 732e 0a0a 372e 2053  aq models...7. S
+00000680: 7461 7274 2074 6865 2064 6576 656c 6f70  tart the develop
+00000690: 6d65 6e74 2073 6572 7665 7220 616e 6420  ment server and 
+000006a0: 7669 7369 7420 6874 7470 3a2f 2f31 3237  visit http://127
+000006b0: 2e30 2e30 2e31 3a38 3030 302f 6164 6d69  .0.0.1:8000/admi
+000006c0: 6e2f 0a20 2020 746f 2063 7265 6174 6520  n/.   to create 
+000006d0: 6120 6361 7465 676f 7279 2028 796f 7527  a category (you'
+000006e0: 6c6c 206e 6565 6420 7468 6520 4164 6d69  ll need the Admi
+000006f0: 6e20 6170 7020 656e 6162 6c65 6429 2e28  n app enabled).(
+00000700: 6361 7465 676f 7269 6573 2070 6172 7420  categories part 
+00000710: 6f66 2074 6865 2061 7070 2063 616e 2062  of the app can b
+00000720: 6520 6469 7361 626c 6564 290a 0a38 2e20  e disabled)..8. 
+00000730: 5669 7369 7420 6874 7470 3a2f 2f31 3237  Visit http://127
+00000740: 2e30 2e30 2e31 3a38 3030 302f 6661 712f  .0.0.1:8000/faq/
+00000750: 2074 6f20 7365 6520 7468 6520 6361 7465   to see the cate
+00000760: 676f 7269 6573 2e0a 0a23 2320 5365 7474  gories...## Sett
+00000770: 696e 6773 0a0a 796f 7520 6361 6e20 6368  ings..you can ch
+00000780: 616e 6765 206d 6f73 7420 7468 696e 6773  ange most things
+00000790: 2069 6e20 7365 7474 696e 6773 2062 656c   in settings bel
+000007a0: 6f77 2069 7320 6120 6c69 7374 206f 6620  ow is a list of 
+000007b0: 616c 6c20 7365 7474 696e 6773 0a61 6464  all settings.add
+000007c0: 2061 6e79 206f 7220 616c 6c20 746f 2063   any or all to c
+000007d0: 6861 6e67 6520 746f 2064 6573 6972 6564  hange to desired
+000007e0: 2062 6568 6176 696f 723a 3a0a 0a0a 2020   behavior::...  
+000007f0: 2020 4641 515f 5345 5454 494e 4753 203d    FAQ_SETTINGS =
+00000800: 205b 2779 6f75 725f 7365 7474 696e 6773   ['your_settings
+00000810: 5f68 6572 6527 2c5d 0a0a 0a31 2e20 6e6f  _here',]...1. no
+00000820: 5f63 6174 6567 6f72 795f 6465 7363 7269  _category_descri
+00000830: 7074 696f 6e20 2020 2020 2020 2020 2020  ption           
+00000840: 2020 2020 2020 202d 2061 6464 2069 6620         - add if 
+00000850: 7573 696e 6720 6361 7465 676f 7269 6573  using categories
+00000860: 2062 7574 2064 6f6e 2774 2077 616e 7420   but don't want 
+00000870: 6465 7363 7269 7074 696f 6e73 2066 6f72  descriptions for
+00000880: 2074 6865 6d0a 322e 206e 6f5f 6361 7465   them.2. no_cate
+00000890: 676f 7279 2020 2020 2020 2020 2020 2020  gory            
+000008a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008b0: 2020 2d20 6164 6420 6966 2064 6f6e 2774    - add if don't
+000008c0: 2077 616e 7420 746f 2075 7365 2063 6174   want to use cat
+000008d0: 6567 6f72 6965 730a 332e 206c 6f67 6765  egories.3. logge
+000008e0: 645f 696e 5f75 7365 7273 5f63 616e 5f61  d_in_users_can_a
+000008f0: 6464 5f71 7565 7374 696f 6e20 2020 2020  dd_question     
+00000900: 2020 2020 2d20 6164 6420 6966 2079 6f75      - add if you
+00000910: 2077 616e 7420 616e 7920 6c6f 6767 6564   want any logged
+00000920: 2069 6e20 7573 6572 2074 6f20 6265 2061   in user to be a
+00000930: 626c 6520 746f 2061 736b 2061 2071 7565  ble to ask a que
+00000940: 7374 696f 6e0a 342e 206c 6f67 6765 645f  stion.4. logged_
+00000950: 696e 5f75 7365 7273 5f63 616e 5f61 6e73  in_users_can_ans
+00000960: 7765 725f 7175 6573 7469 6f6e 2020 2020  wer_question    
+00000970: 2020 2d20 6164 6420 6966 2079 6f75 2077    - add if you w
+00000980: 616e 7420 616e 7920 6c6f 6767 6564 2069  ant any logged i
+00000990: 6e20 7573 6572 2074 6f20 6265 2061 626c  n user to be abl
+000009a0: 6520 746f 2061 6e73 7765 7220 6120 7175  e to answer a qu
+000009b0: 6573 7469 6f6e 0a35 2e20 616c 6c6f 775f  estion.5. allow_
+000009c0: 6d75 6c74 6970 6c65 5f61 6e73 7765 7273  multiple_answers
+000009d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009e0: 2020 202d 2061 6464 2069 6620 796f 7520     - add if you 
+000009f0: 7761 6e74 2061 2071 7565 7374 696f 6e20  want a question 
+00000a00: 746f 2062 6520 6162 6c65 2074 6f20 6265  to be able to be
+00000a10: 2061 6e73 7765 7265 6420 6d75 6c74 6970   answered multip
+00000a20: 6c65 2074 696d 6573 0a36 2e20 6e6f 5f63  le times.6. no_c
+00000a30: 6f6d 6d65 6e74 7320 2020 2020 2020 2020  omments         
+00000a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a50: 2020 2020 202d 2061 6464 2069 6620 646f       - add if do
+00000a60: 6e27 7420 7761 6e74 2074 6f20 7573 6520  n't want to use 
+00000a70: 636f 6d6d 656e 7473 0a37 2e20 616e 6f6e  comments.7. anon
+00000a80: 796d 6f75 735f 7573 6572 5f63 616e 5f63  ymous_user_can_c
+00000a90: 6f6d 6d65 6e74 2020 2020 2020 2020 2020  omment          
+00000aa0: 2020 2020 202d 2061 6464 2069 6620 796f       - add if yo
+00000ab0: 7520 7761 6e74 2061 6e79 2075 7365 7220  u want any user 
+00000ac0: 746f 2062 6520 6162 6c65 2074 6f20 636f  to be able to co
+00000ad0: 6d6d 656e 7420 696e 636c 7564 696e 6720  mment including 
+00000ae0: 616e 6f6e 796d 6f75 7320 7573 6572 730a  anonymous users.
+00000af0: 382e 2076 6965 775f 6f6e 6c79 5f63 6f6d  8. view_only_com
+00000b00: 6d65 6e74 7320 2020 2020 2020 2020 2020  ments           
+00000b10: 2020 2020 2020 2020 2020 2020 2d20 6164              - ad
+00000b20: 6420 6966 2079 6f75 2077 616e 7420 7573  d if you want us
+00000b30: 6572 7320 746f 2073 6565 2070 6f73 7465  ers to see poste
+00000b40: 6420 636f 6d6d 656e 7473 2062 7574 206e  d comments but n
+00000b50: 6f74 2062 6520 6162 6c65 2074 6f20 6164  ot be able to ad
+00000b60: 6420 616e 7920 6d6f 7265 0a39 2e20 6e6f  d any more.9. no
+00000b70: 5f76 6f74 6573 2020 2020 2020 2020 2020  _votes          
+00000b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b90: 2020 2020 2020 202d 2061 6464 2069 6620         - add if 
+00000ba0: 646f 6e27 7420 7761 6e74 2061 6e79 2076  don't want any v
+00000bb0: 6f74 696e 6720 666f 7220 7573 6566 756c  oting for useful
+00000bc0: 2071 7565 7374 696f 6e73 206f 7220 616e   questions or an
+00000bd0: 7377 6572 730a 3130 2e20 6e6f 5f61 6e73  swers.10. no_ans
+00000be0: 7765 725f 766f 7465 7320 2020 2020 2020  wer_votes       
+00000bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c00: 2020 2d20 6164 6420 6966 206f 6e6c 7920    - add if only 
+00000c10: 7761 6e74 2071 7565 7374 696f 6e20 766f  want question vo
+00000c20: 7469 6e67 0a31 312e 206e 6f5f 7175 6573  ting.11. no_ques
+00000c30: 7469 6f6e 5f76 6f74 6573 2020 2020 2020  tion_votes      
+00000c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c50: 202d 2061 6464 2069 6620 6f6e 6c79 2077   - add if only w
+00000c60: 616e 7420 616e 7377 6572 2076 6f74 696e  ant answer votin
+00000c70: 670a 3132 2e20 616c 6c6f 775f 756e 6963  g.12. allow_unic
+00000c80: 6f64 6520 2020 2020 2020 2020 2020 2020  ode             
+00000c90: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
+00000ca0: 6164 6420 6966 2079 6f75 2077 616e 7420  add if you want 
+00000cb0: 746f 2061 6c6c 6f77 2075 6e69 636f 6465  to allow unicode
+00000cc0: 2073 6c75 6773 0a31 332e 206c 6f67 696e   slugs.13. login
+00000cd0: 5f72 6571 7569 7265 6420 2020 2020 2020  _required       
+00000ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000cf0: 2020 202d 2061 6464 2069 6620 796f 7520     - add if you 
+00000d00: 7761 6e74 2074 6f20 6f6e 6c79 206c 6574  want to only let
+00000d10: 206c 6f67 6765 6420 696e 2075 7365 7273   logged in users
+00000d20: 2073 6565 2046 4151 2773 0a31 342e 2072   see FAQ's.14. r
+00000d30: 6963 685f 7465 7874 5f61 6e73 7765 7273  ich_text_answers
+00000d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d50: 2020 2020 2020 202d 2061 6464 2069 6620         - add if 
+00000d60: 796f 7520 7761 6e74 2074 6f20 7573 6520  you want to use 
+00000d70: 7269 6368 2074 6578 7420 666f 7220 616e  rich text for an
+00000d80: 7377 6572 732e 2054 6869 7320 7265 7175  swers. This requ
+00000d90: 6972 6573 2074 6865 2064 6a61 6e67 6f2d  ires the django-
+00000da0: 7469 6e79 6d63 6520 7061 636b 6167 6520  tinymce package 
+00000db0: 746f 2062 6520 696e 7374 616c 6c65 640a  to be installed.
+00000dc0: 0a23 2320 5465 6d70 6c61 7465 730a 0a61  .## Templates..a
+00000dd0: 6c6c 206f 6620 7468 6520 7465 6d70 6c61  ll of the templa
+00000de0: 7465 7320 6172 6520 6d65 616e 7420 746f  tes are meant to
+00000df0: 2062 6520 6f76 6572 7772 6974 7465 6e0a   be overwritten.
+00000e00: 746f 206f 7665 7277 7269 7465 2074 6865  to overwrite the
+00000e10: 6d20 6372 6561 7465 2061 2066 6171 2064  m create a faq d
+00000e20: 6972 6563 746f 7279 2069 6e73 6964 6520  irectory inside 
+00000e30: 6f66 2074 6865 2074 656d 706c 6174 6573  of the templates
+00000e40: 2064 6972 6563 746f 7279 2061 6e64 2061   directory and a
+00000e50: 6464 2061 2068 746d 6c20 6669 6c65 2077  dd a html file w
+00000e60: 6974 6820 7468 6520 7361 6d65 206e 616d  ith the same nam
+00000e70: 6520 746f 2069 740a 0a69 6620 7468 6973  e to it..if this
+00000e80: 2064 6f65 736e 2774 2077 6f72 6b20 6d61   doesn't work ma
+00000e90: 6b65 2073 7572 6520 7468 6174 2074 6865  ke sure that the
+00000ea0: 2074 656d 706c 6174 6573 2073 6574 7469   templates setti
+00000eb0: 6e67 2068 6173 2027 4449 5253 273a 205b  ng has 'DIRS': [
+00000ec0: 2774 656d 706c 6174 6573 275d 2c20 696e  'templates'], in
+00000ed0: 2069 743a 3a0a 0a20 2020 2054 454d 504c   it::..    TEMPL
+00000ee0: 4154 4553 203d 205b 0a20 2020 2020 2020  ATES = [.       
+00000ef0: 207b 0a20 2020 2020 2020 2020 2020 202e   {.            .
+00000f00: 2e2e 0a20 2020 2020 2020 2020 2020 2027  ...            '
+00000f10: 4449 5253 273a 205b 2774 656d 706c 6174  DIRS': ['templat
+00000f20: 6573 275d 2c0a 2020 2020 2020 2020 2020  es'],.          
+00000f30: 2020 2e2e 2e0a 2020 2020 2020 2020 7d2c    ....        },
+00000f40: 0a20 2020 205d 0a0a 6865 7265 2069 7320  .    ]..here is 
+00000f50: 6120 6c69 7374 206f 6620 7465 6d70 6c61  a list of templa
+00000f60: 7465 7320 616e 6420 7468 6572 6520 6465  tes and there de
+00000f70: 6661 756c 7420 7465 6d70 6c61 7465 2020  fault template  
+00000f80: 796f 7520 6361 6e20 6f76 6572 7772 6974  you can overwrit
+00000f90: 650a 0a31 2e20 6361 7465 676f 7269 6573  e..1. categories
+00000fa0: 5f6c 6973 742e 6874 6d6c 202d 2066 6171  _list.html - faq
+00000fb0: 206d 6169 6e20 7669 6577 2069 6620 7573   main view if us
+00000fc0: 696e 6720 6361 7465 676f 7269 6573 3a3a  ing categories::
+00000fd0: 0a0a 0a20 2020 2020 2020 203c 6831 3e73  ...        <h1>s
+00000fe0: 656c 6563 7420 6120 4641 5120 6361 7465  elect a FAQ cate
+00000ff0: 676f 7279 3c2f 6831 3e0a 2020 2020 2020  gory</h1>.      
+00001000: 2020 7b25 2066 6f72 2063 6174 6567 6f72    {% for categor
+00001010: 7920 696e 2063 6174 6567 6f72 6965 7320  y in categories 
+00001020: 257d 0a20 2020 2020 2020 2020 2020 203c  %}.            <
+00001030: 6833 3e3c 6120 6872 6566 3d22 7b25 2075  h3><a href="{% u
+00001040: 726c 2027 6661 713a 6361 7465 676f 7279  rl 'faq:category
+00001050: 5f64 6574 6169 6c27 2063 6174 6567 6f72  _detail' categor
+00001060: 792e 736c 7567 2025 7d22 3e7b 7b63 6174  y.slug %}">{{cat
+00001070: 6567 6f72 792e 6e61 6d65 7d7d 3c2f 613e  egory.name}}</a>
+00001080: 3c2f 6833 3e0a 2020 2020 2020 2020 2020  </h3>.          
+00001090: 2020 7b25 2069 6620 6361 7465 676f 7279    {% if category
+000010a0: 2e64 6573 6372 6970 7469 6f6e 2025 7d0a  .description %}.
+000010b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000010c0: 3c70 3e7b 7b63 6174 6567 6f72 792e 6465  <p>{{category.de
+000010d0: 7363 7269 7074 696f 6e7d 7d3c 2f70 3e0a  scription}}</p>.
+000010e0: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
+000010f0: 6e64 6966 2025 7d0a 2020 2020 2020 2020  ndif %}.        
+00001100: 2020 2020 3c68 723e 0a20 2020 2020 2020      <hr>.       
+00001110: 207b 2520 656e 6466 6f72 2025 7d0a 0a0a   {% endfor %}...
+00001120: 322e 2063 6174 6567 6f72 795f 6465 7461  2. category_deta
+00001130: 696c 2e68 746d 6c20 2d20 6661 7120 6361  il.html - faq ca
+00001140: 7465 676f 7279 2064 6574 6169 6c20 7669  tegory detail vi
+00001150: 6577 2069 6620 7573 696e 6720 6361 7465  ew if using cate
+00001160: 676f 7269 6573 3a3a 0a0a 0a20 2020 2020  gories::...     
+00001170: 2020 203c 6831 3e63 686f 6f73 6520 6120     <h1>choose a 
+00001180: 4641 5120 5175 6573 7469 6f6e 3c2f 6831  FAQ Question</h1
+00001190: 3e0a 2020 2020 2020 2020 3c68 323e 7b7b  >.        <h2>{{
+000011a0: 6361 7465 676f 7279 7d7d 3c2f 6832 3e0a  category}}</h2>.
+000011b0: 2020 2020 2020 2020 7b25 2069 6620 6361          {% if ca
+000011c0: 7465 676f 7279 2e64 6573 6372 6970 7469  tegory.descripti
+000011d0: 6f6e 2025 7d0a 2020 2020 2020 2020 3c70  on %}.        <p
+000011e0: 3e7b 7b63 6174 6567 6f72 792e 6465 7363  >{{category.desc
+000011f0: 7269 7074 696f 6e7d 7d3c 2f70 3e0a 2020  ription}}</p>.  
+00001200: 2020 2020 2020 7b25 2065 6e64 6966 2025        {% endif %
+00001210: 7d0a 2020 2020 2020 2020 3c68 723e 0a20  }.        <hr>. 
+00001220: 2020 2020 2020 207b 2520 666f 7220 7175         {% for qu
+00001230: 6573 7469 6f6e 2069 6e20 6361 7465 676f  estion in catego
+00001240: 7279 2e71 7565 7374 696f 6e5f 7365 742e  ry.question_set.
+00001250: 616c 6c20 257d 0a20 2020 2020 2020 2020  all %}.         
+00001260: 2020 203c 6833 3e3c 6120 6872 6566 3d22     <h3><a href="
+00001270: 7b25 2075 726c 2027 6661 713a 7175 6573  {% url 'faq:ques
+00001280: 7469 6f6e 5f64 6574 6169 6c27 2063 6174  tion_detail' cat
+00001290: 6567 6f72 792e 736c 7567 2071 7565 7374  egory.slug quest
+000012a0: 696f 6e2e 736c 7567 2025 7d22 3e7b 7b71  ion.slug %}">{{q
+000012b0: 7565 7374 696f 6e2e 7175 6573 7469 6f6e  uestion.question
+000012c0: 7d7d 3c2f 613e 3c2f 6833 3e0a 2020 2020  }}</a></h3>.    
+000012d0: 2020 2020 7b25 2065 6e64 666f 7220 257d      {% endfor %}
+000012e0: 0a20 2020 2020 2020 203c 6872 3e0a 2020  .        <hr>.  
+000012f0: 2020 2020 2020 3c61 2068 7265 663d 227b        <a href="{
+00001300: 2520 7572 6c20 2766 6171 3a69 6e64 6578  % url 'faq:index
+00001310: 5f76 6965 7727 2025 7d22 3e62 6163 6b3c  _view' %}">back<
+00001320: 2f61 3e0a 2020 2020 2020 2020 7b25 2069  /a>.        {% i
+00001330: 6620 6361 6e5f 6164 645f 7175 6573 7469  f can_add_questi
+00001340: 6f6e 2025 7d0a 2020 2020 2020 2020 2020  on %}.          
+00001350: 2020 3c61 2068 7265 663d 227b 2520 7572    <a href="{% ur
+00001360: 6c20 2766 6171 3a61 6464 5f71 7565 7374  l 'faq:add_quest
+00001370: 696f 6e27 2063 6174 6567 6f72 792e 736c  ion' category.sl
+00001380: 7567 2025 7d22 3e61 6464 2071 7565 7374  ug %}">add quest
+00001390: 696f 6e3c 2f61 3e0a 2020 2020 2020 2020  ion</a>.        
+000013a0: 7b25 2065 6e64 6966 2025 7d0a 0a0a 332e  {% endif %}...3.
+000013b0: 2071 7565 7374 696f 6e73 5f6c 6973 742e   questions_list.
+000013c0: 6874 6d6c 202d 206c 6973 7473 2061 6c6c  html - lists all
+000013d0: 2071 7565 7374 696f 6e73 2069 6620 6e6f   questions if no
+000013e0: 7420 7573 696e 6720 6361 7465 676f 7269  t using categori
+000013f0: 6573 3a3a 0a0a 0a20 2020 2020 2020 203c  es::...        <
+00001400: 6831 3e63 686f 6f73 6520 6120 4641 5120  h1>choose a FAQ 
+00001410: 5175 6573 7469 6f6e 3c2f 6831 3e0a 2020  Question</h1>.  
+00001420: 2020 2020 2020 7b25 2066 6f72 2071 7565        {% for que
+00001430: 7374 696f 6e20 696e 2071 7565 7374 696f  stion in questio
+00001440: 6e73 2025 7d0a 2020 2020 2020 2020 2020  ns %}.          
+00001450: 2020 3c68 333e 3c61 2068 7265 663d 227b    <h3><a href="{
+00001460: 2520 7572 6c20 2766 6171 3a71 7565 7374  % url 'faq:quest
+00001470: 696f 6e5f 6465 7461 696c 2720 7175 6573  ion_detail' ques
+00001480: 7469 6f6e 2e73 6c75 6720 257d 223e 7b7b  tion.slug %}">{{
+00001490: 7175 6573 7469 6f6e 2e71 7565 7374 696f  question.questio
+000014a0: 6e7d 7d3c 2f61 3e3c 2f68 333e 0a20 2020  n}}</a></h3>.   
+000014b0: 2020 2020 207b 2520 656e 6466 6f72 2025       {% endfor %
+000014c0: 7d0a 2020 2020 0a20 2020 2020 2020 207b  }.    .        {
+000014d0: 2520 6966 2063 616e 5f61 6464 5f71 7565  % if can_add_que
+000014e0: 7374 696f 6e20 257d 0a20 2020 2020 2020  stion %}.       
+000014f0: 2020 2020 203c 6872 3e0a 2020 2020 2020       <hr>.      
+00001500: 2020 2020 2020 3c61 2068 7265 663d 227b        <a href="{
+00001510: 2520 7572 6c20 2766 6171 3a61 6464 5f71  % url 'faq:add_q
+00001520: 7565 7374 696f 6e27 2025 7d22 3e61 6464  uestion' %}">add
+00001530: 2071 7565 7374 696f 6e3c 2f61 3e0a 2020   question</a>.  
+00001540: 2020 2020 2020 7b25 2065 6e64 6966 2025        {% endif %
+00001550: 7d0a 0a0a 342e 2071 7565 7374 696f 6e5f  }...4. question_
+00001560: 6465 7461 696c 2e68 746d 6c20 2d20 7468  detail.html - th
+00001570: 6520 7175 6573 7469 6f6e 2064 6574 6169  e question detai
+00001580: 6c20 7061 6765 3a3a 0a0a 0a20 2020 2020  l page::...     
+00001590: 2020 207b 2520 6578 7465 6e64 7320 2766     {% extends 'f
+000015a0: 6171 2f71 7565 7374 696f 6e5f 6261 7365  aq/question_base
+000015b0: 2e68 746d 6c27 2025 7d0a 2020 2020 0a20  .html' %}.    . 
+000015c0: 2020 2020 2020 207b 2520 626c 6f63 6b20         {% block 
+000015d0: 7175 6573 7469 6f6e 5f63 6f6e 7465 6e74  question_content
+000015e0: 2025 7d0a 2020 2020 2020 2020 7b25 2069   %}.        {% i
+000015f0: 6620 616c 6c6f 775f 6d75 6c74 6970 6c65  f allow_multiple
+00001600: 5f61 6e73 7765 7273 2025 7d0a 2020 2020  _answers %}.    
+00001610: 2020 2020 3c68 333e 616e 7377 6572 733c      <h3>answers<
+00001620: 2f68 333e 0a20 2020 2020 2020 203c 756c  /h3>.        <ul
+00001630: 3e0a 2020 2020 2020 2020 2020 2020 7b25  >.            {%
+00001640: 2066 6f72 2061 6e73 7765 7220 696e 2071   for answer in q
+00001650: 7565 7374 696f 6e2e 616e 7377 6572 5f73  uestion.answer_s
+00001660: 6574 2e61 6c6c 2025 7d0a 2020 2020 2020  et.all %}.      
+00001670: 2020 2020 2020 2020 2020 3c6c 693e 3c62            <li><b
+00001680: 3e7b 7b61 6e73 7765 722e 616e 7377 6572  >{{answer.answer
+00001690: 7d7d 3c2f 623e 0a20 2020 2020 2020 2020  }}</b>.         
+000016a0: 2020 2020 2020 2020 2020 207b 2520 6966             {% if
+000016b0: 2063 616e 5f76 6f74 655f 616e 7377 6572   can_vote_answer
+000016c0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+000016d0: 2020 2020 2020 2020 207c 2066 6f75 6e64           | found
+000016e0: 2074 6869 7320 616e 7377 6572 2068 656c   this answer hel
+000016f0: 7066 756c 3f0a 2020 2020 2020 2020 2020  pful?.          
+00001700: 2020 2020 2020 2020 2020 3c66 6f72 6d20            <form 
+00001710: 7374 796c 653d 2264 6973 706c 6179 3a20  style="display: 
+00001720: 696e 6c69 6e65 3b22 2061 6374 696f 6e3d  inline;" action=
+00001730: 227b 2520 6966 2063 6174 6567 6f72 795f  "{% if category_
+00001740: 656e 6162 6c65 6420 257d 7b25 2075 726c  enabled %}{% url
+00001750: 2027 6661 713a 766f 7465 5f61 6e73 7765   'faq:vote_answe
+00001760: 7227 2071 7565 7374 696f 6e2e 6361 7465  r' question.cate
+00001770: 676f 7279 2e73 6c75 6720 7175 6573 7469  gory.slug questi
+00001780: 6f6e 2e73 6c75 6720 616e 7377 6572 2e73  on.slug answer.s
+00001790: 6c75 6720 257d 7b25 2065 6c73 6520 257d  lug %}{% else %}
+000017a0: 7b25 2075 726c 2027 6661 713a 766f 7465  {% url 'faq:vote
+000017b0: 5f61 6e73 7765 7227 2071 7565 7374 696f  _answer' questio
+000017c0: 6e2e 736c 7567 2061 6e73 7765 722e 736c  n.slug answer.sl
+000017d0: 7567 2025 7d7b 2520 656e 6469 6620 257d  ug %}{% endif %}
+000017e0: 2220 6d65 7468 6f64 3d22 706f 7374 223e  " method="post">
+000017f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001800: 2020 2020 2020 2020 207b 2520 6373 7266           {% csrf
+00001810: 5f74 6f6b 656e 2025 7d0a 2020 2020 2020  _token %}.      
+00001820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001830: 2020 3c69 6e70 7574 2074 7970 653d 2268    <input type="h
+00001840: 6964 6465 6e22 2076 616c 7565 3d54 7275  idden" value=Tru
+00001850: 6520 6e61 6d65 3d22 766f 7465 223e 0a20  e name="vote">. 
+00001860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001870: 2020 2020 2020 203c 6275 7474 6f6e 2074         <button t
+00001880: 7970 653d 2273 7562 6d69 7422 3e79 6573  ype="submit">yes
+00001890: 287b 7b61 6e73 7765 722e 6865 6c70 6675  ({{answer.helpfu
+000018a0: 6c7d 7d29 3c2f 6275 7474 6f6e 3e0a 2020  l}})</button>.  
+000018b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018c0: 2020 3c2f 666f 726d 3e0a 2020 2020 2020    </form>.      
+000018d0: 2020 2020 2020 2020 2020 2020 2020 3c66                <f
+000018e0: 6f72 6d20 7374 796c 653d 2264 6973 706c  orm style="displ
+000018f0: 6179 3a20 696e 6c69 6e65 3b22 2061 6374  ay: inline;" act
+00001900: 696f 6e3d 227b 2520 6966 2063 6174 6567  ion="{% if categ
+00001910: 6f72 795f 656e 6162 6c65 6420 257d 7b25  ory_enabled %}{%
+00001920: 2075 726c 2027 6661 713a 766f 7465 5f61   url 'faq:vote_a
+00001930: 6e73 7765 7227 2071 7565 7374 696f 6e2e  nswer' question.
+00001940: 6361 7465 676f 7279 2e73 6c75 6720 7175  category.slug qu
+00001950: 6573 7469 6f6e 2e73 6c75 6720 616e 7377  estion.slug answ
+00001960: 6572 2e73 6c75 6720 257d 7b25 2065 6c73  er.slug %}{% els
+00001970: 6520 257d 7b25 2075 726c 2027 6661 713a  e %}{% url 'faq:
+00001980: 766f 7465 5f61 6e73 7765 7227 2071 7565  vote_answer' que
+00001990: 7374 696f 6e2e 736c 7567 2061 6e73 7765  stion.slug answe
+000019a0: 722e 736c 7567 2025 7d7b 2520 656e 6469  r.slug %}{% endi
+000019b0: 6620 257d 2220 6d65 7468 6f64 3d22 706f  f %}" method="po
+000019c0: 7374 223e 0a20 2020 2020 2020 2020 2020  st">.           
+000019d0: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
+000019e0: 6373 7266 5f74 6f6b 656e 2025 7d0a 2020  csrf_token %}.  
+000019f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a00: 2020 2020 2020 3c69 6e70 7574 2074 7970        <input typ
+00001a10: 653d 2268 6964 6465 6e22 2076 616c 7565  e="hidden" value
+00001a20: 3d46 616c 7365 206e 616d 653d 2276 6f74  =False name="vot
+00001a30: 6522 3e0a 2020 2020 2020 2020 2020 2020  e">.            
+00001a40: 2020 2020 2020 2020 2020 2020 3c62 7574              <but
+00001a50: 746f 6e20 7479 7065 3d22 7375 626d 6974  ton type="submit
+00001a60: 223e 6e6f 287b 7b61 6e73 7765 722e 6e6f  ">no({{answer.no
+00001a70: 745f 6865 6c70 6675 6c7d 7d29 3c2f 6275  t_helpful}})</bu
+00001a80: 7474 6f6e 3e0a 2020 2020 2020 2020 2020  tton>.          
+00001a90: 2020 2020 2020 2020 2020 3c2f 666f 726d            </form
+00001aa0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00001ab0: 2020 2020 2020 7b25 2065 6e64 6966 2025        {% endif %
+00001ac0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00001ad0: 2020 3c2f 6c69 3e0a 2020 2020 2020 2020    </li>.        
+00001ae0: 2020 2020 7b25 2065 6e64 666f 7220 257d      {% endfor %}
+00001af0: 0a20 2020 2020 2020 203c 2f75 6c3e 0a20  .        </ul>. 
+00001b00: 2020 200a 2020 2020 2020 2020 7b25 2065     .        {% e
+00001b10: 6c73 6520 257d 0a20 2020 2020 2020 2020  lse %}.         
+00001b20: 2020 207b 2520 6966 2071 7565 7374 696f     {% if questio
+00001b30: 6e2e 616e 7377 6572 5f73 6574 2e65 7869  n.answer_set.exi
+00001b40: 7374 7320 257d 0a20 2020 2020 2020 2020  sts %}.         
+00001b50: 2020 2020 2020 203c 703e 616e 7377 6572         <p>answer
+00001b60: 3a3c 2f70 3e0a 2020 2020 2020 2020 2020  :</p>.          
+00001b70: 2020 2020 2020 3c68 333e 7b7b 7175 6573        <h3>{{ques
+00001b80: 7469 6f6e 2e61 6e73 7765 725f 7365 742e  tion.answer_set.
+00001b90: 6669 7273 742e 616e 7377 6572 7d7d 3c2f  first.answer}}</
+00001ba0: 6833 3e0a 2020 2020 2020 2020 2020 2020  h3>.            
+00001bb0: 2020 2020 7b25 2069 6620 6361 6e5f 766f      {% if can_vo
+00001bc0: 7465 5f61 6e73 7765 7220 257d 0a20 2020  te_answer %}.   
+00001bd0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00001be0: 756e 6420 7468 6973 2061 6e73 7765 7220  und this answer 
+00001bf0: 6865 6c70 6675 6c3f 0a20 2020 2020 2020  helpful?.       
+00001c00: 2020 2020 2020 2020 203c 666f 726d 2073           <form s
+00001c10: 7479 6c65 3d22 6469 7370 6c61 793a 2069  tyle="display: i
+00001c20: 6e6c 696e 653b 2220 6163 7469 6f6e 3d22  nline;" action="
+00001c30: 7b25 2069 6620 6361 7465 676f 7279 5f65  {% if category_e
+00001c40: 6e61 626c 6564 2025 7d7b 2520 7572 6c20  nabled %}{% url 
+00001c50: 2766 6171 3a76 6f74 655f 616e 7377 6572  'faq:vote_answer
+00001c60: 2720 7175 6573 7469 6f6e 2e63 6174 6567  ' question.categ
+00001c70: 6f72 792e 736c 7567 2071 7565 7374 696f  ory.slug questio
+00001c80: 6e2e 736c 7567 2071 7565 7374 696f 6e2e  n.slug question.
+00001c90: 616e 7377 6572 5f73 6574 2e66 6972 7374  answer_set.first
+00001ca0: 2e73 6c75 6720 257d 7b25 2065 6c73 6520  .slug %}{% else 
+00001cb0: 257d 7b25 2075 726c 2027 6661 713a 766f  %}{% url 'faq:vo
+00001cc0: 7465 5f61 6e73 7765 7227 2071 7565 7374  te_answer' quest
+00001cd0: 696f 6e2e 736c 7567 2071 7565 7374 696f  ion.slug questio
+00001ce0: 6e2e 616e 7377 6572 5f73 6574 2e66 6972  n.answer_set.fir
+00001cf0: 7374 2e73 6c75 6720 257d 7b25 2065 6e64  st.slug %}{% end
+00001d00: 6966 2025 7d22 206d 6574 686f 643d 2270  if %}" method="p
+00001d10: 6f73 7422 3e0a 2020 2020 2020 2020 2020  ost">.          
+00001d20: 2020 2020 2020 2020 2020 7b25 2063 7372            {% csr
+00001d30: 665f 746f 6b65 6e20 257d 0a20 2020 2020  f_token %}.     
+00001d40: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00001d50: 696e 7075 7420 7479 7065 3d22 6869 6464  input type="hidd
+00001d60: 656e 2220 7661 6c75 653d 5472 7565 206e  en" value=True n
+00001d70: 616d 653d 2276 6f74 6522 3e0a 2020 2020  ame="vote">.    
+00001d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d90: 3c62 7574 746f 6e20 7479 7065 3d22 7375  <button type="su
+00001da0: 626d 6974 223e 7965 7328 7b7b 7175 6573  bmit">yes({{ques
+00001db0: 7469 6f6e 2e61 6e73 7765 725f 7365 742e  tion.answer_set.
+00001dc0: 6669 7273 742e 6865 6c70 6675 6c7d 7d29  first.helpful}})
+00001dd0: 3c2f 6275 7474 6f6e 3e0a 2020 2020 2020  </button>.      
+00001de0: 2020 2020 2020 2020 2020 3c2f 666f 726d            </form
+00001df0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00001e00: 2020 3c66 6f72 6d20 7374 796c 653d 2264    <form style="d
+00001e10: 6973 706c 6179 3a20 696e 6c69 6e65 3b22  isplay: inline;"
+00001e20: 2061 6374 696f 6e3d 227b 2520 6966 2063   action="{% if c
+00001e30: 6174 6567 6f72 795f 656e 6162 6c65 6420  ategory_enabled 
+00001e40: 257d 7b25 2075 726c 2027 6661 713a 766f  %}{% url 'faq:vo
+00001e50: 7465 5f61 6e73 7765 7227 2071 7565 7374  te_answer' quest
+00001e60: 696f 6e2e 6361 7465 676f 7279 2e73 6c75  ion.category.slu
+00001e70: 6720 7175 6573 7469 6f6e 2e73 6c75 6720  g question.slug 
+00001e80: 7175 6573 7469 6f6e 2e61 6e73 7765 725f  question.answer_
+00001e90: 7365 742e 6669 7273 742e 736c 7567 2025  set.first.slug %
+00001ea0: 7d7b 2520 656c 7365 2025 7d7b 2520 7572  }{% else %}{% ur
+00001eb0: 6c20 2766 6171 3a76 6f74 655f 616e 7377  l 'faq:vote_answ
+00001ec0: 6572 2720 7175 6573 7469 6f6e 2e73 6c75  er' question.slu
+00001ed0: 6720 7175 6573 7469 6f6e 2e61 6e73 7765  g question.answe
+00001ee0: 725f 7365 742e 6669 7273 742e 736c 7567  r_set.first.slug
+00001ef0: 2025 7d7b 2520 656e 6469 6620 257d 2220   %}{% endif %}" 
+00001f00: 6d65 7468 6f64 3d22 706f 7374 223e 0a20  method="post">. 
+00001f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f20: 2020 207b 2520 6373 7266 5f74 6f6b 656e     {% csrf_token
+00001f30: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+00001f40: 2020 2020 2020 2020 3c69 6e70 7574 2074          <input t
+00001f50: 7970 653d 2268 6964 6465 6e22 2076 616c  ype="hidden" val
+00001f60: 7565 3d46 616c 7365 206e 616d 653d 2276  ue=False name="v
+00001f70: 6f74 6522 3e0a 2020 2020 2020 2020 2020  ote">.          
+00001f80: 2020 2020 2020 2020 2020 3c62 7574 746f            <butto
+00001f90: 6e20 7479 7065 3d22 7375 626d 6974 223e  n type="submit">
+00001fa0: 6e6f 287b 7b71 7565 7374 696f 6e2e 616e  no({{question.an
+00001fb0: 7377 6572 5f73 6574 2e66 6972 7374 2e6e  swer_set.first.n
+00001fc0: 6f74 5f68 656c 7066 756c 7d7d 293c 2f62  ot_helpful}})</b
+00001fd0: 7574 746f 6e3e 0a20 2020 2020 2020 2020  utton>.         
+00001fe0: 2020 2020 2020 203c 2f66 6f72 6d3e 0a20         </form>. 
+00001ff0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00002000: 2520 656e 6469 6620 257d 0a20 2020 2020  % endif %}.     
+00002010: 2020 2020 2020 207b 2520 656c 7365 2025         {% else %
+00002020: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00002030: 2020 6e6f 2061 6e73 7765 7273 2079 6574    no answers yet
+00002040: 0a20 2020 2020 2020 2020 2020 207b 2520  .            {% 
+00002050: 656e 6469 6620 257d 0a20 2020 2020 2020  endif %}.       
+00002060: 207b 2520 656e 6469 6620 257d 0a20 2020   {% endif %}.   
+00002070: 200a 2020 2020 0a20 2020 2020 2020 207b   .    .        {
+00002080: 2520 6966 2063 616e 5f61 6e73 7765 725f  % if can_answer_
+00002090: 7175 6573 7469 6f6e 2025 7d0a 2020 2020  question %}.    
+000020a0: 2020 2020 2020 2020 7b25 2069 6620 6361          {% if ca
+000020b0: 7465 676f 7279 5f65 6e61 626c 6564 2025  tegory_enabled %
+000020c0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+000020d0: 2020 3c61 2068 7265 663d 227b 2520 7572    <a href="{% ur
+000020e0: 6c20 2766 6171 3a61 6e73 7765 725f 7175  l 'faq:answer_qu
+000020f0: 6573 7469 6f6e 2720 7175 6573 7469 6f6e  estion' question
+00002100: 2e63 6174 6567 6f72 792e 736c 7567 2071  .category.slug q
+00002110: 7565 7374 696f 6e2e 736c 7567 2025 7d22  uestion.slug %}"
+00002120: 3e61 6e73 7765 7220 7175 6573 7469 6f6e  >answer question
+00002130: 3c2f 613e 0a20 2020 2020 2020 2020 2020  </a>.           
+00002140: 207b 2520 656c 7365 2025 7d0a 2020 2020   {% else %}.    
+00002150: 2020 2020 2020 2020 2020 2020 3c61 2068              <a h
+00002160: 7265 663d 227b 2520 7572 6c20 2766 6171  ref="{% url 'faq
+00002170: 3a61 6e73 7765 725f 7175 6573 7469 6f6e  :answer_question
+00002180: 2720 7175 6573 7469 6f6e 2e73 6c75 6720  ' question.slug 
+00002190: 257d 223e 616e 7377 6572 2071 7565 7374  %}">answer quest
+000021a0: 696f 6e3c 2f61 3e0a 2020 2020 2020 2020  ion</a>.        
+000021b0: 2020 2020 7b25 2065 6e64 6966 2025 7d0a      {% endif %}.
+000021c0: 2020 2020 2020 2020 7b25 2065 6e64 6966          {% endif
+000021d0: 2025 7d0a 2020 2020 2020 2020 3c68 723e   %}.        <hr>
+000021e0: 0a20 2020 2020 2020 207b 2520 6966 2063  .        {% if c
+000021f0: 6f6d 6d65 6e74 735f 616c 6c6f 7765 6420  omments_allowed 
+00002200: 257d 0a20 2020 2020 2020 2020 2020 207b  %}.            {
+00002210: 2520 696e 636c 7564 6520 2766 6171 2f63  % include 'faq/c
+00002220: 6f6d 6d65 6e74 732e 6874 6d6c 2720 257d  omments.html' %}
+00002230: 0a20 2020 2020 2020 207b 2520 656e 6469  .        {% endi
+00002240: 6620 257d 0a20 2020 200a 2020 2020 2020  f %}.    .      
+00002250: 2020 7b25 2065 6e64 626c 6f63 6b20 257d    {% endblock %}
+00002260: 0a0a 352e 2061 6e73 7765 725f 666f 726d  ..5. answer_form
+00002270: 2e68 746d 6c20 2d20 666f 726d 2074 6f20  .html - form to 
+00002280: 6164 6420 616e 7377 6572 2074 6f20 7175  add answer to qu
+00002290: 6573 7469 6f6e 3a3a 0a0a 0a20 2020 2020  estion::...     
+000022a0: 2020 203c 6831 3e41 6e73 7765 7220 5175     <h1>Answer Qu
+000022b0: 6573 7469 6f6e 3c2f 6831 3e0a 2020 2020  estion</h1>.    
+000022c0: 2020 2020 3c61 2068 7265 663d 227b 7b71      <a href="{{q
+000022d0: 7565 7374 696f 6e2e 6765 745f 6162 736f  uestion.get_abso
+000022e0: 6c75 7465 5f75 726c 7d7d 223e 3c68 333e  lute_url}}"><h3>
+000022f0: 7b7b 7175 6573 7469 6f6e 2e71 7565 7374  {{question.quest
+00002300: 696f 6e7d 7d3c 2f68 333e 3c2f 613e 0a20  ion}}</h3></a>. 
+00002310: 2020 2020 2020 203c 666f 726d 206d 6574         <form met
+00002320: 686f 643d 2270 6f73 7422 3e0a 2020 2020  hod="post">.    
+00002330: 2020 2020 2020 2020 7b25 2063 7372 665f          {% csrf_
+00002340: 746f 6b65 6e20 257d 0a20 2020 2020 2020  token %}.       
+00002350: 2020 2020 207b 7b66 6f72 6d7d 7d0a 2020       {{form}}.  
+00002360: 2020 2020 2020 2020 2020 3c69 6e70 7574            <input
+00002370: 2074 7970 653d 2273 7562 6d69 7422 3e0a   type="submit">.
+00002380: 2020 2020 2020 2020 3c2f 666f 726d 3e0a          </form>.
+00002390: 0a36 2e20 636f 6d6d 656e 745f 666f 726d  .6. comment_form
+000023a0: 2e68 746d 6c20 2d20 666f 726d 2074 6f20  .html - form to 
+000023b0: 6164 6420 636f 6d6d 656e 7473 2074 6f20  add comments to 
+000023c0: 7175 6573 7469 6f6e 2028 6f6e 6c79 2073  question (only s
+000023d0: 686f 7773 2075 7020 7768 656e 2066 6f72  hows up when for
+000023e0: 6d20 6861 7320 6572 726f 7220 6265 6361  m has error beca
+000023f0: 7573 6520 7669 6577 206f 6e6c 7920 6765  use view only ge
+00002400: 7473 2070 6f73 7465 6420 746f 293a 3a0a  ts posted to)::.
+00002410: 0a0a 2020 2020 2020 2020 3c68 313e 506f  ..        <h1>Po
+00002420: 7374 2041 2043 6f6d 6d65 6e74 3c2f 6831  st A Comment</h1
+00002430: 3e0a 2020 2020 2020 2020 3c61 2068 7265  >.        <a hre
+00002440: 663d 227b 7b71 7565 7374 696f 6e2e 6765  f="{{question.ge
+00002450: 745f 6162 736f 6c75 7465 5f75 726c 7d7d  t_absolute_url}}
+00002460: 223e 3c68 333e 7b7b 7175 6573 7469 6f6e  "><h3>{{question
+00002470: 2e71 7565 7374 696f 6e7d 7d3c 2f68 333e  .question}}</h3>
+00002480: 3c2f 613e 0a20 2020 2020 2020 203c 666f  </a>.        <fo
+00002490: 726d 206d 6574 686f 643d 2270 6f73 7422  rm method="post"
+000024a0: 3e0a 2020 2020 2020 2020 2020 2020 7b25  >.            {%
+000024b0: 2063 7372 665f 746f 6b65 6e20 257d 0a20   csrf_token %}. 
+000024c0: 2020 2020 2020 2020 2020 207b 7b66 6f72             {{for
+000024d0: 6d7d 7d0a 2020 2020 2020 2020 2020 2020  m}}.            
+000024e0: 3c69 6e70 7574 2074 7970 653d 2273 7562  <input type="sub
+000024f0: 6d69 7422 3e0a 2020 2020 2020 2020 3c2f  mit">.        </
+00002500: 666f 726d 3e0a 0a37 2e20 7175 6573 7469  form>..7. questi
+00002510: 6f6e 5f66 6f72 6d2e 6874 6d6c 202d 2066  on_form.html - f
+00002520: 6f72 6d20 746f 2061 6464 2061 206e 6577  orm to add a new
+00002530: 2071 7565 7374 696f 6e3a 3a0a 0a0a 2020   question::...  
+00002540: 2020 2020 2020 3c68 313e 4164 6420 596f        <h1>Add Yo
+00002550: 7572 2051 7565 7374 696f 6e3c 2f68 313e  ur Question</h1>
+00002560: 0a20 2020 2020 2020 203c 666f 726d 206d  .        <form m
+00002570: 6574 686f 643d 2270 6f73 7422 3e0a 2020  ethod="post">.  
+00002580: 2020 2020 2020 2020 2020 7b25 2063 7372            {% csr
+00002590: 665f 746f 6b65 6e20 257d 0a20 2020 2020  f_token %}.     
+000025a0: 2020 2020 2020 207b 7b66 6f72 6d7d 7d0a         {{form}}.
+000025b0: 2020 2020 2020 2020 2020 2020 3c69 6e70              <inp
+000025c0: 7574 2074 7970 653d 2273 7562 6d69 7422  ut type="submit"
+000025d0: 3e0a 2020 2020 2020 2020 3c2f 666f 726d  >.        </form
+000025e0: 3e0a 0a38 2e20 766f 7465 5f66 6f72 6d2e  >..8. vote_form.
+000025f0: 6874 6d6c 202d 2066 6f72 6d20 666f 7220  html - form for 
+00002600: 766f 7469 6e67 2071 7565 7374 696f 6e73  voting questions
+00002610: 2061 6e64 2061 6e73 7765 7273 2028 6f6e   and answers (on
+00002620: 6c79 2073 686f 7773 2075 7020 7768 656e  ly shows up when
+00002630: 2066 6f72 6d20 6861 7320 6572 726f 7220   form has error 
+00002640: 6265 6361 7573 6520 7669 6577 206f 6e6c  because view onl
+00002650: 7920 6765 7473 2070 6f73 7465 6420 746f  y gets posted to
+00002660: 293a 3a0a 0a0a 2020 2020 2020 2020 3c68  )::...        <h
+00002670: 313e 766f 7465 3c2f 6831 3e0a 2020 2020  1>vote</h1>.    
+00002680: 2020 2020 3c66 6f72 6d20 6d65 7468 6f64      <form method
+00002690: 3d22 706f 7374 223e 0a20 2020 2020 2020  ="post">.       
+000026a0: 2020 2020 207b 2520 6373 7266 5f74 6f6b       {% csrf_tok
+000026b0: 656e 2025 7d0a 2020 2020 2020 2020 2020  en %}.          
+000026c0: 2020 7b7b 666f 726d 7d7d 0a20 2020 2020    {{form}}.     
+000026d0: 2020 2020 2020 203c 696e 7075 7420 7479         <input ty
+000026e0: 7065 3d22 7375 626d 6974 223e 0a20 2020  pe="submit">.   
+000026f0: 2020 2020 203c 2f66 6f72 6d3e 0a0a 392e       </form>..9.
+00002700: 2063 6f6d 6d65 6e74 732e 6874 6d6c 202d   comments.html -
+00002710: 2069 6620 636f 6d6d 656e 7473 2061 7265   if comments are
+00002720: 2061 6c6c 6f77 6564 2074 6869 7320 7465   allowed this te
+00002730: 6d70 6c61 7465 2069 7320 696e 636c 7564  mplate is includ
+00002740: 6564 2069 6e20 7468 6520 7175 6573 7469  ed in the questi
+00002750: 6f6e 2064 6574 6169 6c2e 6874 6d6c 3a3a  on detail.html::
+00002760: 0a0a 0a20 2020 2020 2020 203c 6833 3e63  ...        <h3>c
+00002770: 6f6d 6d65 6e74 733c 2f68 333e 0a20 2020  omments</h3>.   
+00002780: 2020 2020 203c 756c 3e0a 2020 2020 2020       <ul>.      
+00002790: 2020 2020 2020 7b25 2066 6f72 2063 6f6d        {% for com
+000027a0: 6d65 6e74 2069 6e20 7175 6573 7469 6f6e  ment in question
+000027b0: 2e66 6171 636f 6d6d 656e 745f 7365 742e  .faqcomment_set.
+000027c0: 616c 6c20 257d 0a20 2020 2020 2020 2020  all %}.         
+000027d0: 2020 2020 2020 203c 6c69 3e3c 6834 3e7b         <li><h4>{
+000027e0: 7b63 6f6d 6d65 6e74 2e63 6f6d 6d65 6e74  {comment.comment
+000027f0: 7d7d 3c2f 6834 3e0a 2020 2020 2020 2020  }}</h4>.        
+00002800: 2020 2020 2020 2020 2020 2020 706f 7374              post
+00002810: 6564 2062 7920 7b25 2069 6620 636f 6d6d  ed by {% if comm
+00002820: 656e 742e 7573 6572 257d 7b7b 636f 6d6d  ent.user%}{{comm
+00002830: 656e 742e 7573 6572 7d7d 7b25 2065 6c73  ent.user}}{% els
+00002840: 6520 257d 616e 6f6e 796d 6f75 737b 2520  e %}anonymous{% 
+00002850: 656e 6469 6620 257d 207b 7b63 6f6d 6d65  endif %} {{comme
+00002860: 6e74 2e70 6f73 745f 7469 6d65 7c74 696d  nt.post_time|tim
+00002870: 6573 696e 6365 7d7d 2061 676f 3c2f 6c69  esince}} ago</li
+00002880: 3e0a 2020 2020 2020 2020 2020 2020 7b25  >.            {%
+00002890: 2065 6e64 666f 7220 257d 0a20 2020 2020   endfor %}.     
+000028a0: 2020 203c 2f75 6c3e 0a20 2020 2020 2020     </ul>.       
+000028b0: 207b 2520 6966 2061 6464 5f6e 6577 5f63   {% if add_new_c
+000028c0: 6f6d 6d65 6e74 5f61 6c6c 6f77 6564 2025  omment_allowed %
+000028d0: 7d0a 2020 2020 2020 2020 2020 2020 7b25  }.            {%
+000028e0: 2069 6620 6361 7465 676f 7279 5f65 6e61   if category_ena
+000028f0: 626c 6564 2025 7d0a 2020 2020 2020 2020  bled %}.        
+00002900: 2020 2020 3c66 6f72 6d20 6d65 7468 6f64      <form method
+00002910: 3d22 706f 7374 2220 6163 7469 6f6e 3d22  ="post" action="
+00002920: 7b25 2075 726c 2027 6661 713a 6164 645f  {% url 'faq:add_
+00002930: 636f 6d6d 656e 7427 2071 7565 7374 696f  comment' questio
+00002940: 6e2e 6361 7465 676f 7279 2e73 6c75 6720  n.category.slug 
+00002950: 7175 6573 7469 6f6e 2e73 6c75 6720 257d  question.slug %}
+00002960: 223e 0a20 2020 2020 2020 2020 2020 207b  ">.            {
+00002970: 2520 656c 7365 2025 7d0a 2020 2020 2020  % else %}.      
+00002980: 2020 2020 2020 3c66 6f72 6d20 6d65 7468        <form meth
+00002990: 6f64 3d22 706f 7374 2220 6163 7469 6f6e  od="post" action
+000029a0: 3d22 7b25 2075 726c 2027 6661 713a 6164  ="{% url 'faq:ad
+000029b0: 645f 636f 6d6d 656e 7427 2071 7565 7374  d_comment' quest
+000029c0: 696f 6e2e 736c 7567 2025 7d22 3e0a 2020  ion.slug %}">.  
+000029d0: 2020 2020 2020 2020 2020 7b25 2065 6e64            {% end
+000029e0: 6966 2025 7d0a 2020 2020 2020 2020 2020  if %}.          
+000029f0: 2020 3c66 6965 6c64 7365 743e 0a20 2020    <fieldset>.   
+00002a00: 2020 2020 2020 2020 2020 2020 203c 6c65               <le
+00002a10: 6765 6e64 3e50 6f73 7420 596f 7572 2043  gend>Post Your C
+00002a20: 6f6d 6d65 6e74 2048 6572 653a 3c2f 6c65  omment Here:</le
+00002a30: 6765 6e64 3e0a 2020 2020 2020 2020 2020  gend>.          
+00002a40: 2020 2020 2020 7b25 2063 7372 665f 746f        {% csrf_to
+00002a50: 6b65 6e20 257d 0a20 2020 2020 2020 2020  ken %}.         
+00002a60: 2020 2020 2020 207b 7b63 6f6d 6d65 6e74         {{comment
+00002a70: 5f66 6f72 6d7d 7d0a 2020 2020 2020 2020  _form}}.        
+00002a80: 2020 2020 2020 2020 3c69 6e70 7574 2074          <input t
+00002a90: 7970 653d 2273 7562 6d69 7422 206e 616d  ype="submit" nam
+00002aa0: 653d 2270 6f73 7422 3e0a 2020 2020 2020  e="post">.      
+00002ab0: 2020 2020 2020 3c2f 6669 656c 6473 6574        </fieldset
+00002ac0: 3e0a 2020 2020 2020 2020 2020 2020 3c2f  >.            </
+00002ad0: 666f 726d 3e0a 2020 2020 2020 2020 7b25  form>.        {%
+00002ae0: 2065 6e64 6966 2025 7d0a 0a23 2320 5465   endif %}..## Te
+00002af0: 6d70 6c61 7465 2056 6172 6961 626c 6573  mplate Variables
+00002b00: 0a0a 312e 2063 6174 6567 6f72 6965 735f  ..1. categories_
+00002b10: 6c69 7374 2e68 746d 6c0a 2020 2020 6361  list.html.    ca
+00002b20: 7465 676f 7269 6573 202d 2061 6c6c 2074  tegories - all t
+00002b30: 6865 2063 6174 6567 6f72 6965 7320 2863  he categories (c
+00002b40: 6174 6567 6f72 7920 7175 6572 7973 6574  ategory queryset
+00002b50: 290a 0a32 2e20 6361 7465 676f 7269 6573  )..2. categories
+00002b60: 5f64 6574 6169 6c2e 6874 6d6c 0a20 2020  _detail.html.   
+00002b70: 2063 6174 6567 6f72 7920 2d20 7468 6520   category - the 
+00002b80: 6361 7465 676f 7279 2063 686f 7365 6e20  category chosen 
+00002b90: 2863 6174 6567 6f72 7920 6f62 6a65 6374  (category object
+00002ba0: 290a 2020 2020 6361 6e5f 6164 645f 7175  ).    can_add_qu
+00002bb0: 6573 7469 6f6e 202d 2062 6f6f 6c20 6966  estion - bool if
+00002bc0: 2074 6865 2075 7365 7220 6361 6e20 6164   the user can ad
+00002bd0: 6420 6120 7175 6573 7469 6f6e 2028 6465  d a question (de
+00002be0: 7065 6e64 7320 6f6e 2074 6865 2073 6574  pends on the set
+00002bf0: 7469 6e67 7329 0a33 2e20 7175 6573 7469  tings).3. questi
+00002c00: 6f6e 735f 6c69 7374 2e68 746d 6c0a 2020  ons_list.html.  
+00002c10: 2020 7175 6573 7469 6f6e 7320 2d20 616c    questions - al
+00002c20: 6c20 7468 6520 7175 6573 7469 6f6e 7320  l the questions 
+00002c30: 2871 7565 7374 696f 6e20 7175 6572 7973  (question querys
+00002c40: 6574 290a 2020 2020 6361 6e5f 6164 645f  et).    can_add_
+00002c50: 7175 6573 7469 6f6e 202d 2062 6f6f 6c20  question - bool 
+00002c60: 6966 2074 6865 2075 7365 7220 6361 6e20  if the user can 
+00002c70: 6164 6420 6120 7175 6573 7469 6f6e 2028  add a question (
+00002c80: 6465 7065 6e64 7320 6f6e 2074 6865 2073  depends on the s
+00002c90: 6574 7469 6e67 7329 0a34 2e20 7175 6573  ettings).4. ques
+00002ca0: 7469 6f6e 5f64 6574 6169 6c2e 6874 6d6c  tion_detail.html
+00002cb0: 0a20 2020 2071 7565 7374 696f 6e20 2d20  .    question - 
+00002cc0: 7468 6520 7175 6573 7469 6f6e 2063 686f  the question cho
+00002cd0: 7365 6e20 2871 7565 7374 696f 6e20 6f62  sen (question ob
+00002ce0: 6a65 6374 290a 2020 2020 6361 6e5f 766f  ject).    can_vo
+00002cf0: 7465 5f71 7565 7374 696f 6e20 2d20 626f  te_question - bo
+00002d00: 6f6c 2069 6620 7468 6520 7573 6572 2063  ol if the user c
+00002d10: 616e 2076 6f74 6520 6120 7175 6573 7469  an vote a questi
+00002d20: 6f6e 2028 6465 7065 6e64 7320 6f6e 2074  on (depends on t
+00002d30: 6865 2073 6574 7469 6e67 7329 0a20 2020  he settings).   
+00002d40: 2063 6174 6567 6f72 795f 656e 6162 6c65   category_enable
+00002d50: 6420 2d20 626f 6f6c 2069 6620 6361 7465  d - bool if cate
+00002d60: 676f 7279 2065 6e61 626c 6564 2069 6e20  gory enabled in 
+00002d70: 7365 7474 696e 6773 0a20 2020 2061 6c6c  settings.    all
+00002d80: 6f77 5f6d 756c 7469 706c 655f 616e 7377  ow_multiple_answ
+00002d90: 6572 7320 2d20 626f 6f6c 2069 6620 6d75  ers - bool if mu
+00002da0: 6c74 6970 6c65 2061 6e73 7765 7273 2061  ltiple answers a
+00002db0: 6c6c 6f77 6564 2069 6e20 7365 7474 696e  llowed in settin
+00002dc0: 6773 0a20 2020 2063 616e 5f76 6f74 655f  gs.    can_vote_
+00002dd0: 616e 7377 6572 202d 2062 6f6f 6c20 6966  answer - bool if
+00002de0: 2074 6865 2075 7365 7220 6361 6e20 766f   the user can vo
+00002df0: 7465 2061 6e20 616e 7377 6572 2028 6465  te an answer (de
+00002e00: 7065 6e64 7320 6f6e 2074 6865 2073 6574  pends on the set
+00002e10: 7469 6e67 7329 0a20 2020 2063 616e 5f61  tings).    can_a
+00002e20: 6e73 7765 725f 7175 6573 7469 6f6e 202d  nswer_question -
+00002e30: 2062 6f6f 6c20 6966 2063 7572 7265 6e74   bool if current
+00002e40: 2075 7365 7220 6361 6e20 616e 7377 6572   user can answer
+00002e50: 2071 7565 7374 696f 6e20 2864 6570 656e   question (depen
+00002e60: 6473 206f 6e20 7468 6520 7365 7474 696e  ds on the settin
+00002e70: 6773 290a 2020 2020 636f 6d6d 656e 7473  gs).    comments
+00002e80: 5f61 6c6c 6f77 6564 202d 2062 6f6f 6c20  _allowed - bool 
+00002e90: 6966 2075 7369 6e67 2063 6f6d 6d65 6e74  if using comment
+00002ea0: 7320 696e 2073 6574 7469 6e67 730a 2020  s in settings.  
+00002eb0: 2020 6164 645f 6e65 775f 636f 6d6d 656e    add_new_commen
+00002ec0: 745f 616c 6c6f 7765 6420 2d20 626f 6f6c  t_allowed - bool
+00002ed0: 2069 6620 6375 7272 656e 7420 7573 6572   if current user
+00002ee0: 2063 616e 2061 6464 2063 6f6d 6d65 6e74   can add comment
+00002ef0: 2028 6465 7065 6e64 7320 6f6e 2074 6865   (depends on the
+00002f00: 2073 6574 7469 6e67 7329 0a20 2020 2063   settings).    c
+00002f10: 6f6d 6d65 6e74 5f66 6f72 6d20 2d20 666f  omment_form - fo
+00002f20: 726d 2074 6f20 7375 626d 6974 2061 206e  rm to submit a n
+00002f30: 6577 2063 6f6d 6d65 6e74 0a35 2e20 616e  ew comment.5. an
+00002f40: 7377 6572 5f66 6f72 6d2e 6874 6d6c 0a20  swer_form.html. 
+00002f50: 2020 2071 7565 7374 696f 6e20 2d20 7468     question - th
+00002f60: 6520 7175 6573 7469 6f6e 2074 6f20 6164  e question to ad
+00002f70: 6420 616e 7377 6572 2074 6f20 2871 7565  d answer to (que
+00002f80: 7374 696f 6e20 6f62 6a65 6374 290a 2020  stion object).  
+00002f90: 2020 666f 726d 202d 2066 6f72 6d20 746f    form - form to
+00002fa0: 2061 6464 206e 6577 2061 6e73 7765 720a   add new answer.
+00002fb0: 362e 2063 6f6d 6d65 6e74 5f66 6f72 6d2e  6. comment_form.
+00002fc0: 6874 6d6c 0a20 2020 2071 7565 7374 696f  html.    questio
+00002fd0: 6e20 2d20 7468 6520 7175 6573 7469 6f6e  n - the question
+00002fe0: 2074 6f20 6164 6420 636f 6d6d 656e 7420   to add comment 
+00002ff0: 746f 2028 7175 6573 7469 6f6e 206f 626a  to (question obj
+00003000: 6563 7429 0a20 2020 2066 6f72 6d20 2d20  ect).    form - 
+00003010: 666f 726d 2074 6f20 6164 6420 6e65 7720  form to add new 
+00003020: 636f 6d6d 656e 740a 372e 2071 7565 7374  comment.7. quest
+00003030: 696f 6e5f 666f 726d 2e68 746d 6c0a 2020  ion_form.html.  
+00003040: 2020 666f 726d 202d 2066 6f72 6d20 746f    form - form to
+00003050: 2061 6464 206e 6577 2071 7565 7374 696f   add new questio
+00003060: 6e0a 382e 2076 6f74 655f 666f 726d 2e68  n.8. vote_form.h
+00003070: 746d 6c0a 2020 2020 666f 726d 202d 2066  tml.    form - f
+00003080: 6f72 6d20 746f 2076 6f74 6520 666f 7220  orm to vote for 
+00003090: 6120 7175 6573 7469 6f6e 206f 7220 616e  a question or an
+000030a0: 7377 6572 0a0a 2323 2055 726c 730a 0a61  swer..## Urls..a
+000030b0: 6c6c 206f 6620 7468 6520 666f 6c6c 6f77  ll of the follow
+000030c0: 696e 6720 7572 6c73 2061 7265 2062 7920  ing urls are by 
+000030d0: 6e61 6d65 2074 6865 6e20 6164 6469 7469  name then additi
+000030e0: 6f6e 616c 0a74 6865 2061 7070 206e 616d  onal.the app nam
+000030f0: 6520 666f 7220 7468 6520 7572 6c73 2069  e for the urls i
+00003100: 7320 6060 2766 6171 2760 600a 0a2a 2069  s ``'faq'``..* i
+00003110: 6e64 6578 5f76 6965 770a 2020 2020 2a20  ndex_view.    * 
+00003120: 6e6f 2061 7267 756d 656e 7473 0a20 2020  no arguments.   
+00003130: 202a 2064 6973 706c 6179 7320 616c 6c20   * displays all 
+00003140: 7468 6520 6361 7465 676f 7269 6573 2069  the categories i
+00003150: 6620 6361 7465 676f 7269 6573 2061 7265  f categories are
+00003160: 2065 6e61 626c 6564 206f 7468 6572 7769   enabled otherwi
+00003170: 7365 2073 686f 7773 2071 7565 7374 696f  se shows questio
+00003180: 6e73 0a2a 2063 6174 6567 6f72 795f 6465  ns.* category_de
+00003190: 7461 696c 0a20 2020 202a 206e 6565 6473  tail.    * needs
+000031a0: 2063 6174 6567 6f72 7920 736c 7567 2061   category slug a
+000031b0: 7320 736c 7567 0a20 2020 202a 2064 6973  s slug.    * dis
+000031c0: 706c 6179 7320 616c 6c20 7468 6520 7175  plays all the qu
+000031d0: 6573 7469 6f6e 7320 6769 7665 6e20 7468  estions given th
+000031e0: 6520 6361 7465 676f 7279 2077 6865 6e20  e category when 
+000031f0: 6361 7465 676f 7269 6573 2061 7265 2065  categories are e
+00003200: 6e61 626c 6564 0a2a 2061 6464 5f71 7565  nabled.* add_que
+00003210: 7374 696f 6e0a 2020 2020 2a20 6966 2063  stion.    * if c
+00003220: 6174 6567 6f72 6965 7320 6172 6520 656e  ategories are en
+00003230: 6162 6c65 6420 6e65 6564 7320 6361 7465  abled needs cate
+00003240: 676f 7279 2073 6c75 6720 6173 2073 6c75  gory slug as slu
+00003250: 670a 2020 2020 2a20 6966 206c 6f67 6765  g.    * if logge
+00003260: 645f 696e 5f75 7365 7273 5f63 616e 5f61  d_in_users_can_a
+00003270: 6464 5f71 7565 7374 696f 6e20 7468 656e  dd_question then
+00003280: 2064 6973 706c 6179 7320 666f 726d 2066   displays form f
+00003290: 6f72 206c 6f67 6765 6420 696e 2075 7365  or logged in use
+000032a0: 7273 2074 6f20 6173 6b20 6120 6e65 7720  rs to ask a new 
+000032b0: 7175 6573 7469 6f6e 0a2a 2071 7565 7374  question.* quest
+000032c0: 696f 6e5f 6465 7461 696c 0a20 2020 202a  ion_detail.    *
+000032d0: 206e 6565 6473 2071 7565 7374 696f 6e20   needs question 
+000032e0: 736c 7567 2061 7320 7175 6573 7469 6f6e  slug as question
+000032f0: 207c 2069 6620 6361 7465 676f 7269 6573   | if categories
+00003300: 2061 7265 2065 6e61 626c 6564 206e 6565   are enabled nee
+00003310: 6473 2063 6174 6567 6f72 7920 736c 7567  ds category slug
+00003320: 2061 7320 736c 7567 0a20 2020 202a 2064   as slug.    * d
+00003330: 6973 706c 6179 7320 7468 6520 6d61 696e  isplays the main
+00003340: 2046 4151 2070 6167 6520 7769 7468 2074   FAQ page with t
+00003350: 6865 2071 7565 7374 696f 6e20 616c 6c20  he question all 
+00003360: 7468 6520 636f 6d6d 656e 7473 2061 6e64  the comments and
+00003370: 2061 6e73 7765 7273 0a2a 2061 6e73 7765   answers.* answe
+00003380: 725f 7175 6573 7469 6f6e 0a20 2020 202a  r_question.    *
+00003390: 206e 6565 6473 2071 7565 7374 696f 6e20   needs question 
+000033a0: 736c 7567 2061 7320 7175 6573 7469 6f6e  slug as question
+000033b0: 207c 2069 6620 6361 7465 676f 7269 6573   | if categories
+000033c0: 2061 7265 2065 6e61 626c 6564 206e 6565   are enabled nee
+000033d0: 6473 2063 6174 6567 6f72 7920 736c 7567  ds category slug
+000033e0: 2061 7320 6361 7465 676f 7279 0a20 2020   as category.   
+000033f0: 202a 2064 6973 706c 6179 7320 7468 6520   * displays the 
+00003400: 616e 7377 6572 2071 7565 7374 696f 6e20  answer question 
+00003410: 666f 726d 0a2a 2061 6464 5f63 6f6d 6d65  form.* add_comme
+00003420: 6e74 0a20 2020 202a 206e 6565 6473 2071  nt.    * needs q
+00003430: 7565 7374 696f 6e20 736c 7567 2061 7320  uestion slug as 
+00003440: 7175 6573 7469 6f6e 207c 2069 6620 6361  question | if ca
+00003450: 7465 676f 7269 6573 2061 7265 2065 6e61  tegories are ena
+00003460: 626c 6564 206e 6565 6473 2063 6174 6567  bled needs categ
+00003470: 6f72 7920 736c 7567 2061 7320 6361 7465  ory slug as cate
+00003480: 676f 7279 0a20 2020 202a 206f 6e6c 7920  gory.    * only 
+00003490: 776f 726b 7320 6966 2075 7369 6e67 2063  works if using c
+000034a0: 6f6d 6d65 6e74 730a 2020 2020 2a20 7573  omments.    * us
+000034b0: 6564 2074 6f20 706f 7374 2063 6f6d 6d65  ed to post comme
+000034c0: 6e74 2066 6f72 6d20 6672 6f6d 2071 7565  nt form from que
+000034d0: 7374 696f 6e5f 6465 7461 696c 2074 6f20  stion_detail to 
+000034e0: 6461 7461 6261 7365 0a2a 2076 6f74 655f  database.* vote_
+000034f0: 616e 7377 6572 0a20 2020 202a 206e 6565  answer.    * nee
+00003500: 6473 2071 7565 7374 696f 6e20 736c 7567  ds question slug
+00003510: 2061 7320 7175 6573 7469 6f6e 207c 206e   as question | n
+00003520: 6565 6473 2061 6e73 7765 7220 736c 7567  eeds answer slug
+00003530: 2061 7320 616e 7377 6572 207c 2069 6620   as answer | if 
+00003540: 6361 7465 676f 7269 6573 2061 7265 2065  categories are e
+00003550: 6e61 626c 6564 206e 6565 6473 2063 6174  nabled needs cat
+00003560: 6567 6f72 7920 736c 7567 2061 7320 6361  egory slug as ca
+00003570: 7465 676f 7279 0a20 2020 202a 206f 6e6c  tegory.    * onl
+00003580: 7920 776f 726b 7320 6966 2075 7369 6e67  y works if using
+00003590: 2061 6e73 7765 7220 766f 7469 6e67 0a20   answer voting. 
+000035a0: 2020 202a 2075 7365 6420 746f 2070 6f73     * used to pos
+000035b0: 7420 6869 6464 656e 2069 6e70 7574 2076  t hidden input v
+000035c0: 6f74 6520 3d20 3120 6f72 2076 6f74 6520  ote = 1 or vote 
+000035d0: 3d20 3020 6465 7065 6e64 696e 6720 6f6e  = 0 depending on
+000035e0: 2076 6f74 6520 7570 206f 7220 646f 776e   vote up or down
+000035f0: 0a2a 2076 6f74 655f 7175 6573 7469 6f6e  .* vote_question
+00003600: 0a20 2020 202a 206e 6565 6473 2071 7565  .    * needs que
+00003610: 7374 696f 6e20 736c 7567 2061 7320 7175  stion slug as qu
+00003620: 6573 7469 6f6e 207c 2069 6620 6361 7465  estion | if cate
+00003630: 676f 7269 6573 2061 7265 2065 6e61 626c  gories are enabl
+00003640: 6564 206e 6565 6473 2063 6174 6567 6f72  ed needs categor
+00003650: 7920 736c 7567 2061 7320 6361 7465 676f  y slug as catego
+00003660: 7279 0a20 2020 202a 206f 6e6c 7920 776f  ry.    * only wo
+00003670: 726b 7320 6966 2075 7369 6e67 2071 7565  rks if using que
+00003680: 7374 696f 6e20 766f 7469 6e67 0a20 2020  stion voting.   
+00003690: 202a 2075 7365 6420 746f 2070 6f73 7420   * used to post 
+000036a0: 6869 6464 656e 2069 6e70 7574 2076 6f74  hidden input vot
+000036b0: 6520 3d20 3120 6f72 2076 6f74 6520 3d20  e = 1 or vote = 
+000036c0: 3020 6465 7065 6e64 696e 6720 6f6e 2076  0 depending on v
+000036d0: 6f74 6520 7570 206f 7220 646f 776e 0a0a  ote up or down..
+000036e0: 2323 2064 6a61 6e67 6f2d 7469 6e79 6d63  ## django-tinymc
+000036f0: 650a 4966 2079 6f75 2077 616e 7420 746f  e.If you want to
+00003700: 2075 7365 2072 6963 6820 7465 7874 2061   use rich text a
+00003710: 6e73 7765 7273 2079 6f75 2077 696c 6c20  nswers you will 
+00003720: 6e65 6564 2074 6f20 5b69 6e73 7461 6c6c  need to [install
+00003730: 2064 6a61 6e67 6f2d 7469 6e79 6d63 655d   django-tinymce]
+00003740: 2868 7474 7073 3a2f 2f64 6a61 6e67 6f2d  (https://django-
+00003750: 7469 6e79 6d63 652e 7265 6164 7468 6564  tinymce.readthed
+00003760: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+00003770: 2f69 6e73 7461 6c6c 6174 696f 6e2e 6874  /installation.ht
+00003780: 6d6c 2369 6432 290a 0a4d 616b 6520 7375  ml#id2)..Make su
+00003790: 7265 2074 6f20 696e 636c 7564 6520 696e  re to include in
+000037a0: 2074 6865 2074 656d 706c 6174 6520 7468   the template th
+000037b0: 6520 607b 7b20 666f 726d 2e6d 6564 6961  e `{{ form.media
+000037c0: 207d 7d60 2074 6f20 696e 636c 7564 6520   }}` to include 
+000037d0: 7468 6520 7469 6e79 6d63 6520 6a61 7661  the tinymce java
+000037e0: 7363 7269 7074 2061 6e64 2063 7373 2066  script and css f
+000037f0: 696c 6573 2e0a 3e20 5b21 5741 524e 494e  iles..> [!WARNIN
+00003800: 475d 2020 0a3e 2046 6169 6c69 6e67 2074  G]  .> Failing t
+00003810: 6f20 666f 6c6c 6f77 2074 6865 2066 6f6c  o follow the fol
+00003820: 6c6f 7769 6e67 2073 7465 7073 2077 696c  lowing steps wil
+00003830: 6c20 7265 7375 6c74 2069 6e20 6120 7873  l result in a xs
+00003840: 7320 7675 6c6e 6572 6162 696c 6974 7920  s vulnerability 
+00003850: 696e 2079 6f75 7220 7369 7465 2e0a 0a54  in your site...T
+00003860: 6f20 616c 6c6f 7720 7468 6520 7269 6368  o allow the rich
+00003870: 2074 6578 7420 616e 7377 6572 7320 746f   text answers to
+00003880: 2062 6520 7265 6e64 6572 6564 2070 726f   be rendered pro
+00003890: 7065 726c 7920 796f 7520 7769 6c6c 206e  perly you will n
+000038a0: 6565 6420 746f 2075 7365 2074 6865 2073  eed to use the s
+000038b0: 6166 6520 6669 6c74 6572 2069 6e20 796f  afe filter in yo
+000038c0: 7572 2074 656d 706c 6174 6573 2e0a 5768  ur templates..Wh
+000038d0: 696c 6520 646a 616e 676f 2d74 696e 796d  ile django-tinym
+000038e0: 6365 2064 6f65 7320 6573 6361 7065 2074  ce does escape t
+000038f0: 6865 2068 746d 6c20 7468 6520 616e 7377  he html the answ
+00003900: 6572 7320 7468 6174 2077 6572 6520 6372  ers that were cr
+00003910: 6561 7465 6420 7768 656e 2074 6865 2072  eated when the r
+00003920: 6963 6820 7465 7874 2065 6469 746f 7220  ich text editor 
+00003930: 7761 7320 6e6f 7420 656e 6162 6c65 6420  was not enabled 
+00003940: 2a2a 6861 7320 6e6f 7420 6265 656e 2065  **has not been e
+00003950: 7363 6170 6564 2061 6e64 2069 7320 6e6f  scaped and is no
+00003960: 7420 7361 6665 2a2a 2e0a 536f 2074 6865  t safe**..So the
+00003970: 7365 2061 6e73 7765 7273 2063 616e 6e6f  se answers canno
+00003980: 7420 6265 2072 656e 6465 7265 6420 7769  t be rendered wi
+00003990: 7468 2074 6865 2073 6166 6520 6669 6c74  th the safe filt
+000039a0: 6572 2e20 536f 2061 2066 6c61 6720 7761  er. So a flag wa
+000039b0: 7320 6164 6465 6420 746f 2074 6865 2061  s added to the a
+000039c0: 6e73 7765 7220 6d6f 6465 6c20 2769 735f  nswer model 'is_
+000039d0: 7269 6368 5f74 6578 7427 2074 6861 7420  rich_text' that 
+000039e0: 6973 2073 6574 2074 6f20 5472 7565 2077  is set to True w
+000039f0: 6865 6e20 7468 6520 616e 7377 6572 2069  hen the answer i
+00003a00: 7320 6372 6561 7465 6420 7769 7468 2074  s created with t
+00003a10: 6865 2072 6963 6820 7465 7874 2065 6469  he rich text edi
+00003a20: 746f 722e 0a49 6e20 7468 6520 7465 6d70  tor..In the temp
+00003a30: 6c61 7465 2079 6f75 2063 616e 2075 7365  late you can use
+00003a40: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
+00003a50: 6f64 6520 746f 2072 656e 6465 7220 7468  ode to render th
+00003a60: 6520 616e 7377 6572 2070 726f 7065 726c  e answer properl
+00003a70: 793a 3a0a 0a20 2020 207b 2520 6966 2061  y::..    {% if a
+00003a80: 6e73 7765 722e 6973 5f72 6963 685f 7465  nswer.is_rich_te
+00003a90: 7874 2025 7d0a 2020 2020 2020 2020 7b7b  xt %}.        {{
+00003aa0: 616e 7377 6572 2e61 6e73 7765 727c 7361  answer.answer|sa
+00003ab0: 6665 7d7d 0a20 2020 207b 2520 656c 7365  fe}}.    {% else
+00003ac0: 2025 7d0a 2020 2020 2020 2020 7b7b 616e   %}.        {{an
+00003ad0: 7377 6572 2e61 6e73 7765 727d 7d0a 2020  swer.answer}}.  
+00003ae0: 2020 7b25 2065 6e64 6966 2025 7d0a 0a23    {% endif %}..#
+00003af0: 2320 436f 6e74 7269 6275 7469 6e67 0a0a  # Contributing..
+00003b00: 646a 616e 676f 2d65 6173 792d 6661 7120  django-easy-faq 
+00003b10: 6169 6d73 2074 6f20 6265 2074 6865 2062  aims to be the b
+00003b20: 6573 7420 6661 7120 6170 7020 666f 7220  est faq app for 
+00003b30: 646a 616e 676f 2e20 4974 2077 656c 636f  django. It welco
+00003b40: 6d65 7320 2063 6f6e 7472 6962 7574 696f  mes  contributio
+00003b50: 6e73 206f 6620 616c 6c20 7479 7065 7320  ns of all types 
+00003b60: 2d20 6973 7375 6573 2c20 6275 6773 2c20  - issues, bugs, 
+00003b70: 6665 6174 7572 6520 7265 7175 6573 7473  feature requests
+00003b80: 2c20 646f 6375 6d65 6e74 6174 696f 6e20  , documentation 
+00003b90: 7570 6461 7465 732c 2074 6573 7473 2061  updates, tests a
+00003ba0: 6e64 2070 756c 6c20 7265 7175 6573 7473  nd pull requests
+00003bb0: 0a0a 2323 2063 6861 6e67 6520 6c6f 670a  ..## change log.
+00003bc0: 302e 3420 6669 7865 6420 6275 6720 7468  0.4 fixed bug th
+00003bd0: 6174 206c 6f67 6765 6420 6f75 7420 7573  at logged out us
+00003be0: 6572 7320 6361 6e20 766f 7465 202d 2077  ers can vote - w
+00003bf0: 6869 6368 2074 6865 6e20 7261 6973 6573  hich then raises
+00003c00: 2065 7863 6570 7469 6f6e 730a 0a30 2e35   exceptions..0.5
+00003c10: 2066 6978 6564 206d 6967 7261 7469 6f6e   fixed migration
+00003c20: 730a 0a31 2e30 2061 6464 6564 2070 7970  s..1.0 added pyp
+00003c30: 6920 6469 7374 7269 6275 7469 6f6e 0a0a  i distribution..
+00003c40: 312e 3120 6164 6465 6420 6d6f 7265 2074  1.1 added more t
+00003c50: 656d 706c 6174 6573 2074 6f20 6f76 6572  emplates to over
+00003c60: 7269 6465 2065 6173 696c 790a 0a31 2e32  ride easily..1.2
+00003c70: 2066 6978 6564 2062 7567 2069 6e20 7079   fixed bug in py
+00003c80: 7069 2064 6973 7472 6f20 6e6f 7420 696e  pi distro not in
+00003c90: 636c 7564 696e 6720 6661 7120 6170 700a  cluding faq app.
+00003ca0: 0a31 2e33 2066 6978 6564 2062 7567 2077  .1.3 fixed bug w
+00003cb0: 6865 7265 2061 2073 6c75 6720 6d75 7374  here a slug must
+00003cc0: 2062 6520 6669 6c6c 6564 206f 7574 2069   be filled out i
+00003cd0: 6e20 6164 6d69 6e20 6576 656e 2074 686f  n admin even tho
+00003ce0: 7567 6820 736c 7567 2067 6574 7320 6175  ugh slug gets au
+00003cf0: 746f 2067 656e 6572 6174 6564 2074 6f20  to generated to 
+00003d00: 7361 7665 2066 6f72 2071 7565 7374 696f  save for questio
+00003d10: 6e73 2c20 616e 7377 6572 732c 2061 6e64  ns, answers, and
+00003d20: 2063 6174 6567 6f72 6965 732e 206d 6164   categories. mad
+00003d30: 6520 7175 6573 7469 6f6e 732c 2061 6e73  e questions, ans
+00003d40: 7765 7273 2c20 6361 7465 676f 7269 6573  wers, categories
+00003d50: 2073 6c75 6773 2072 6561 646f 6e6c 7920   slugs readonly 
+00003d60: 696e 2061 646d 696e 0a0a 312e 3420 6164  in admin..1.4 ad
+00003d70: 6465 6420 756e 6963 6f64 6520 6f70 7469  ded unicode opti
+00003d80: 6f6e 2074 6f20 6164 6420 756e 6963 6f64  on to add unicod
+00003d90: 6520 736c 7567 730a 0a31 2e35 2061 6464  e slugs..1.5 add
+00003da0: 6564 206c 6f67 696e 5f72 6571 7569 7265  ed login_require
+00003db0: 6420 7365 7474 696e 6720 746f 2061 6c6c  d setting to all
+00003dc0: 6f77 2066 6171 2061 7070 2074 6f20 6265  ow faq app to be
+00003dd0: 2061 7661 696c 6162 6c65 2074 6f20 6f6e   available to on
+00003de0: 6c79 206c 6f67 6765 6420 696e 2075 7365  ly logged in use
+00003df0: 7273 0a0a 312e 3620 6669 7865 6420 6275  rs..1.6 fixed bu
+00003e00: 6720 7768 6572 6520 6e6f 5f63 6174 6567  g where no_categ
+00003e10: 6f72 795f 6465 7363 7269 7074 696f 6e20  ory_description 
+00003e20: 6469 6420 6e6f 7420 646f 2072 656d 6f76  did not do remov
+00003e30: 6520 7468 6520 6361 7465 676f 7279 2064  e the category d
+00003e40: 6573 6372 6970 7469 6f6e 2069 6e20 7468  escription in th
+00003e50: 6520 6164 6d69 6e0a 0a31 2e37 2061 6464  e admin..1.7 add
+00003e60: 6564 2073 7570 706f 7274 2066 6f72 2064  ed support for d
+00003e70: 6a61 6e67 6f20 352e 300a 0a31 2e38 2061  jango 5.0..1.8 a
+00003e80: 6464 6564 2073 7570 706f 7274 2066 6f72  dded support for
+00003e90: 2072 6963 6874 6578 7420 616e 7377 6572   richtext answer
+00003ea0: 7320 7769 7468 2064 6a61 6e67 6f2d 7469  s with django-ti
+00003eb0: 6e79 6d63 650a                           nymce.
```

### Comparing `django-easy-faq-1.7/django_easy_faq.egg-info/PKG-INFO` & `django_easy_faq-1.8/django_easy_faq.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,368 +1,386 @@
-Metadata-Version: 2.1
-Name: django-easy-faq
-Version: 1.7
-Summary: A Django app to add great faq functionality to website.
-Home-page: https://github.com/dragoncommits/django-easy-faq
-License: BSD-3-Clause
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: Django>=3.2
-
-# django-easy-faq
-
-django-easy-faq is a Django app to allow for a simple yet feature rich faq app. with categories, commenting voting of questions and answers all as an optional part of the app. To see screenshots of what this django-easy-faq could look like with bootstrap 5 styling [click here](demo/demo.md).
-
-
-## Quick start
-
-1. pip install:
-
-    `pip install django-easy-faq`
-
-2. Add "faq" to your INSTALLED_APPS setting like this:
-
-    ```python
-    INSTALLED_APPS = [
-        ...
-        'faq',]
-    ```
-
-3. Include the easy-faq URLconf in your project urls.py like this::
-
-    ```python
-    #…
-    path('faq/', include('faq.urls')),
-    #…
-    ```
-
-4. Add `FAQ_SETTINGS = []` to your `settings.py`
-5. Run ``python manage.py makemigrations`` to create the faq models migrations.
-6. Run ``python manage.py migrate`` to create the faq models.
-
-7. Start the development server and visit http://127.0.0.1:8000/admin/
-   to create a category (you'll need the Admin app enabled).(categories part of the app can be disabled)
-
-8. Visit http://127.0.0.1:8000/faq/ to see the categories.
-
-## Settings
-
-you can change most things in settings below is a list of all settings
-add any or all to change to desired behavior::
-
-
-    FAQ_SETTINGS = ['your_settings_here',]
-
-
-1. no_category_description                  - add if using categories but don't want descriptions for them
-2. no_category                              - add if don't want to use categories
-3. logged_in_users_can_add_question         - add if you want any logged in user to be able to ask a question
-4. logged_in_users_can_answer_question      - add if you want any logged in user to be able to answer a question
-5. allow_multiple_answers                   - add if you want a question to be able to be answered multiple times
-6. no_comments                              - add if don't want to use comments
-7. anonymous_user_can_comment               - add if you want any user to be able to comment including anonymous users
-8. view_only_comments                       - add if you want users to see posted comments but not be able to add any more
-9. no_votes                                 - add if don't want any voting for useful questions or answers
-10. no_answer_votes                         - add if only want question voting
-11. no_question_votes                       - add if only want answer voting
-12. allow_unicode                           - add if you want to allow unicode slugs
-13. login_required                          - add if you want to only let logged in users see FAQ's
-
-## Templates
-
-all of the templates are meant to be overwritten
-to overwrite them create a faq directory inside of the templates directory and add a html file with the same name to it
-
-if this doesn't work make sure that the templates setting has 'DIRS': ['templates'], in it::
-
-    TEMPLATES = [
-        {
-            ...
-            'DIRS': ['templates'],
-            ...
-        },
-    ]
-
-here is a list of templates and there default template  you can overwrite
-
-1. categories_list.html - faq main view if using categories::
-
-
-        <h1>select a FAQ category</h1>
-        {% for category in categories %}
-            <h3><a href="{% url 'faq:category_detail' category.slug %}">{{category.name}}</a></h3>
-            {% if category.description %}
-                <p>{{category.description}}</p>
-            {% endif %}
-            <hr>
-        {% endfor %}
-
-
-2. category_detail.html - faq category detail view if using categories::
-
-
-        <h1>choose a FAQ Question</h1>
-        <h2>{{category}}</h2>
-        {% if category.description %}
-        <p>{{category.description}}</p>
-        {% endif %}
-        <hr>
-        {% for question in category.question_set.all %}
-            <h3><a href="{% url 'faq:question_detail' category.slug question.slug %}">{{question.question}}</a></h3>
-        {% endfor %}
-        <hr>
-        <a href="{% url 'faq:index_view' %}">back</a>
-        {% if can_add_question %}
-            <a href="{% url 'faq:add_question' category.slug %}">add question</a>
-        {% endif %}
-
-
-3. questions_list.html - lists all questions if not using categories::
-
-
-        <h1>choose a FAQ Question</h1>
-        {% for question in questions %}
-            <h3><a href="{% url 'faq:question_detail' question.slug %}">{{question.question}}</a></h3>
-        {% endfor %}
-    
-        {% if can_add_question %}
-            <hr>
-            <a href="{% url 'faq:add_question' %}">add question</a>
-        {% endif %}
-
-
-4. question_detail.html - the question detail page::
-
-
-        {% extends 'faq/question_base.html' %}
-    
-        {% block question_content %}
-        {% if allow_multiple_answers %}
-        <h3>answers</h3>
-        <ul>
-            {% for answer in question.answer_set.all %}
-                <li><b>{{answer.answer}}</b>
-                    {% if can_vote_answer %}
-                     | found this answer helpful?
-                    <form style="display: inline;" action="{% if category_enabled %}{% url 'faq:vote_answer' question.category.slug question.slug answer.slug %}{% else %}{% url 'faq:vote_answer' question.slug answer.slug %}{% endif %}" method="post">
-                        {% csrf_token %}
-                        <input type="hidden" value=True name="vote">
-                        <button type="submit">yes({{answer.helpful}})</button>
-                    </form>
-                    <form style="display: inline;" action="{% if category_enabled %}{% url 'faq:vote_answer' question.category.slug question.slug answer.slug %}{% else %}{% url 'faq:vote_answer' question.slug answer.slug %}{% endif %}" method="post">
-                        {% csrf_token %}
-                        <input type="hidden" value=False name="vote">
-                        <button type="submit">no({{answer.not_helpful}})</button>
-                    </form>
-                    {% endif %}
-                </li>
-            {% endfor %}
-        </ul>
-    
-        {% else %}
-            {% if question.answer_set.exists %}
-                <p>answer:</p>
-                <h3>{{question.answer_set.first.answer}}</h3>
-                {% if can_vote_answer %}
-                 found this answer helpful?
-                <form style="display: inline;" action="{% if category_enabled %}{% url 'faq:vote_answer' question.category.slug question.slug question.answer_set.first.slug %}{% else %}{% url 'faq:vote_answer' question.slug question.answer_set.first.slug %}{% endif %}" method="post">
-                    {% csrf_token %}
-                    <input type="hidden" value=True name="vote">
-                    <button type="submit">yes({{question.answer_set.first.helpful}})</button>
-                </form>
-                <form style="display: inline;" action="{% if category_enabled %}{% url 'faq:vote_answer' question.category.slug question.slug question.answer_set.first.slug %}{% else %}{% url 'faq:vote_answer' question.slug question.answer_set.first.slug %}{% endif %}" method="post">
-                    {% csrf_token %}
-                    <input type="hidden" value=False name="vote">
-                    <button type="submit">no({{question.answer_set.first.not_helpful}})</button>
-                </form>
-                {% endif %}
-            {% else %}
-                no answers yet
-            {% endif %}
-        {% endif %}
-    
-    
-        {% if can_answer_question %}
-            {% if category_enabled %}
-                <a href="{% url 'faq:answer_question' question.category.slug question.slug %}">answer question</a>
-            {% else %}
-                <a href="{% url 'faq:answer_question' question.slug %}">answer question</a>
-            {% endif %}
-        {% endif %}
-        <hr>
-        {% if comments_allowed %}
-            {% include 'faq/comments.html' %}
-        {% endif %}
-    
-        {% endblock %}
-
-5. answer_form.html - form to add answer to question::
-
-
-        <h1>Answer Question</h1>
-        <a href="{{question.get_absolute_url}}"><h3>{{question.question}}</h3></a>
-        <form method="post">
-            {% csrf_token %}
-            {{form}}
-            <input type="submit">
-        </form>
-
-6. comment_form.html - form to add comments to question (only shows up when form has error because view only gets posted to)::
-
-
-        <h1>Post A Comment</h1>
-        <a href="{{question.get_absolute_url}}"><h3>{{question.question}}</h3></a>
-        <form method="post">
-            {% csrf_token %}
-            {{form}}
-            <input type="submit">
-        </form>
-
-7. question_form.html - form to add a new question::
-
-
-        <h1>Add Your Question</h1>
-        <form method="post">
-            {% csrf_token %}
-            {{form}}
-            <input type="submit">
-        </form>
-
-8. vote_form.html - form for voting questions and answers (only shows up when form has error because view only gets posted to)::
-
-
-        <h1>vote</h1>
-        <form method="post">
-            {% csrf_token %}
-            {{form}}
-            <input type="submit">
-        </form>
-
-9. comments.html - if comments are allowed this template is included in the question detail.html::
-
-
-        <h3>comments</h3>
-        <ul>
-            {% for comment in question.faqcomment_set.all %}
-                <li><h4>{{comment.comment}}</h4>
-                    posted by {% if comment.user%}{{comment.user}}{% else %}anonymous{% endif %} {{comment.post_time|timesince}} ago</li>
-            {% endfor %}
-        </ul>
-        {% if add_new_comment_allowed %}
-            {% if category_enabled %}
-            <form method="post" action="{% url 'faq:add_comment' question.category.slug question.slug %}">
-            {% else %}
-            <form method="post" action="{% url 'faq:add_comment' question.slug %}">
-            {% endif %}
-            <fieldset>
-                <legend>Post Your Comment Here:</legend>
-                {% csrf_token %}
-                {{comment_form}}
-                <input type="submit" name="post">
-            </fieldset>
-            </form>
-        {% endif %}
-
-## Template Variables
-
-1. categories_list.html
-    categories - all the categories (category queryset)
-
-2. categories_detail.html
-    category - the category chosen (category object)
-    can_add_question - bool if the user can add a question (depends on the settings)
-3. questions_list.html
-    questions - all the questions (question queryset)
-    can_add_question - bool if the user can add a question (depends on the settings)
-4. question_detail.html
-    question - the question chosen (question object)
-    can_vote_question - bool if the user can vote a question (depends on the settings)
-    category_enabled - bool if category enabled in settings
-    allow_multiple_answers - bool if multiple answers allowed in settings
-    can_vote_answer - bool if the user can vote an answer (depends on the settings)
-    can_answer_question - bool if current user can answer question (depends on the settings)
-    comments_allowed - bool if using comments in settings
-    add_new_comment_allowed - bool if current user can add comment (depends on the settings)
-    comment_form - form to submit a new comment
-5. answer_form.html
-    question - the question to add answer to (question object)
-    form - form to add new answer
-6. comment_form.html
-    question - the question to add comment to (question object)
-    form - form to add new comment
-7. question_form.html
-    form - form to add new question
-8. vote_form.html
-    form - form to vote for a question or answer
-
-## Urls
-
-all of the following urls are by name then additional
-the app name for the urls is ``'faq'``
-
-* index_view
-    * no arguments
-    * displays all the categories if categories are enabled otherwise shows questions
-* category_detail
-    * needs category slug as slug
-    * displays all the questions given the category when categories are enabled
-* add_question
-    * if categories are enabled needs category slug as slug
-    * if logged_in_users_can_add_question then displays form for logged in users to ask a new question
-* question_detail
-    * needs question slug as question | if categories are enabled needs category slug as slug
-    * displays the main FAQ page with the question all the comments and answers
-* answer_question
-    * needs question slug as question | if categories are enabled needs category slug as category
-    * displays the answer question form
-* add_comment
-    * needs question slug as question | if categories are enabled needs category slug as category
-    * only works if using comments
-    * used to post comment form from question_detail to database
-* vote_answer
-    * needs question slug as question | needs answer slug as answer | if categories are enabled needs category slug as category
-    * only works if using answer voting
-    * used to post hidden input vote = 1 or vote = 0 depending on vote up or down
-* vote_question
-    * needs question slug as question | if categories are enabled needs category slug as category
-    * only works if using question voting
-    * used to post hidden input vote = 1 or vote = 0 depending on vote up or down
-
-## Contributing
-
-django-easy-faq aims to be the best faq app for django. It welcomes  contributions of all types - issues, bugs, feature requests, documentation updates, tests and pull requests
-
-## change log
-0.4 fixed bug that logged out users can vote - which then raises exceptions
-
-0.5 fixed migrations
-
-1.0 added pypi distribution
-
-1.1 added more templates to override easily
-
-1.2 fixed bug in pypi distro not including faq app
-
-1.3 fixed bug where a slug must be filled out in admin even though slug gets auto generated to save for questions, answers, and categories. made questions, answers, categories slugs readonly in admin
-
-1.4 added unicode option to add unicode slugs
-
-1.5 added login_required setting to allow faq app to be available to only logged in users
-
-1.6 fixed bug where no_category_description did not do remove the category description in the admin
-
-1.7 added support for django 5.0
+Metadata-Version: 2.1
+Name: django-easy-faq
+Version: 1.8
+Summary: A Django app to add great FAQ functionality to website
+Home-page: https://github.com/smark-1/django-easy-faq/
+Download-URL: https://pypi.python.org/pypi/django-easy-faq
+License: MIT
+Keywords: django,faq
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Framework :: Django
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: Django>=3.2
+
+# django-easy-faq
+
+django-easy-faq is a Django app to allow for a simple yet feature rich faq app. with categories, commenting voting of questions and answers all as an optional part of the app. To see screenshots of what this django-easy-faq could look like with bootstrap 5 styling [click here](demo/demo.md).
+
+
+## Quick start
+
+1. pip install:
+
+    `pip install django-easy-faq`
+
+2. Add "faq" to your INSTALLED_APPS setting like this:
+
+    ```python
+    INSTALLED_APPS = [
+        ...
+        'faq',]
+    ```
+
+3. Include the easy-faq URLconf in your project urls.py like this::
+
+    ```python
+    #…
+    path('faq/', include('faq.urls')),
+    #…
+    ```
+
+4. Add `FAQ_SETTINGS = []` to your `settings.py`
+5. Run ``python manage.py makemigrations`` to create the faq models migrations.
+6. Run ``python manage.py migrate`` to create the faq models.
+
+7. Start the development server and visit http://127.0.0.1:8000/admin/
+   to create a category (you'll need the Admin app enabled).(categories part of the app can be disabled)
+
+8. Visit http://127.0.0.1:8000/faq/ to see the categories.
+
+## Settings
+
+you can change most things in settings below is a list of all settings
+add any or all to change to desired behavior::
+
+
+    FAQ_SETTINGS = ['your_settings_here',]
+
+
+1. no_category_description                  - add if using categories but don't want descriptions for them
+2. no_category                              - add if don't want to use categories
+3. logged_in_users_can_add_question         - add if you want any logged in user to be able to ask a question
+4. logged_in_users_can_answer_question      - add if you want any logged in user to be able to answer a question
+5. allow_multiple_answers                   - add if you want a question to be able to be answered multiple times
+6. no_comments                              - add if don't want to use comments
+7. anonymous_user_can_comment               - add if you want any user to be able to comment including anonymous users
+8. view_only_comments                       - add if you want users to see posted comments but not be able to add any more
+9. no_votes                                 - add if don't want any voting for useful questions or answers
+10. no_answer_votes                         - add if only want question voting
+11. no_question_votes                       - add if only want answer voting
+12. allow_unicode                           - add if you want to allow unicode slugs
+13. login_required                          - add if you want to only let logged in users see FAQ's
+14. rich_text_answers                       - add if you want to use rich text for answers. This requires the django-tinymce package to be installed
+
+## Templates
+
+all of the templates are meant to be overwritten
+to overwrite them create a faq directory inside of the templates directory and add a html file with the same name to it
+
+if this doesn't work make sure that the templates setting has 'DIRS': ['templates'], in it::
+
+    TEMPLATES = [
+        {
+            ...
+            'DIRS': ['templates'],
+            ...
+        },
+    ]
+
+here is a list of templates and there default template  you can overwrite
+
+1. categories_list.html - faq main view if using categories::
+
+
+        <h1>select a FAQ category</h1>
+        {% for category in categories %}
+            <h3><a href="{% url 'faq:category_detail' category.slug %}">{{category.name}}</a></h3>
+            {% if category.description %}
+                <p>{{category.description}}</p>
+            {% endif %}
+            <hr>
+        {% endfor %}
+
+
+2. category_detail.html - faq category detail view if using categories::
+
+
+        <h1>choose a FAQ Question</h1>
+        <h2>{{category}}</h2>
+        {% if category.description %}
+        <p>{{category.description}}</p>
+        {% endif %}
+        <hr>
+        {% for question in category.question_set.all %}
+            <h3><a href="{% url 'faq:question_detail' category.slug question.slug %}">{{question.question}}</a></h3>
+        {% endfor %}
+        <hr>
+        <a href="{% url 'faq:index_view' %}">back</a>
+        {% if can_add_question %}
+            <a href="{% url 'faq:add_question' category.slug %}">add question</a>
+        {% endif %}
+
+
+3. questions_list.html - lists all questions if not using categories::
+
+
+        <h1>choose a FAQ Question</h1>
+        {% for question in questions %}
+            <h3><a href="{% url 'faq:question_detail' question.slug %}">{{question.question}}</a></h3>
+        {% endfor %}
+    
+        {% if can_add_question %}
+            <hr>
+            <a href="{% url 'faq:add_question' %}">add question</a>
+        {% endif %}
+
+
+4. question_detail.html - the question detail page::
+
+
+        {% extends 'faq/question_base.html' %}
+    
+        {% block question_content %}
+        {% if allow_multiple_answers %}
+        <h3>answers</h3>
+        <ul>
+            {% for answer in question.answer_set.all %}
+                <li><b>{{answer.answer}}</b>
+                    {% if can_vote_answer %}
+                     | found this answer helpful?
+                    <form style="display: inline;" action="{% if category_enabled %}{% url 'faq:vote_answer' question.category.slug question.slug answer.slug %}{% else %}{% url 'faq:vote_answer' question.slug answer.slug %}{% endif %}" method="post">
+                        {% csrf_token %}
+                        <input type="hidden" value=True name="vote">
+                        <button type="submit">yes({{answer.helpful}})</button>
+                    </form>
+                    <form style="display: inline;" action="{% if category_enabled %}{% url 'faq:vote_answer' question.category.slug question.slug answer.slug %}{% else %}{% url 'faq:vote_answer' question.slug answer.slug %}{% endif %}" method="post">
+                        {% csrf_token %}
+                        <input type="hidden" value=False name="vote">
+                        <button type="submit">no({{answer.not_helpful}})</button>
+                    </form>
+                    {% endif %}
+                </li>
+            {% endfor %}
+        </ul>
+    
+        {% else %}
+            {% if question.answer_set.exists %}
+                <p>answer:</p>
+                <h3>{{question.answer_set.first.answer}}</h3>
+                {% if can_vote_answer %}
+                 found this answer helpful?
+                <form style="display: inline;" action="{% if category_enabled %}{% url 'faq:vote_answer' question.category.slug question.slug question.answer_set.first.slug %}{% else %}{% url 'faq:vote_answer' question.slug question.answer_set.first.slug %}{% endif %}" method="post">
+                    {% csrf_token %}
+                    <input type="hidden" value=True name="vote">
+                    <button type="submit">yes({{question.answer_set.first.helpful}})</button>
+                </form>
+                <form style="display: inline;" action="{% if category_enabled %}{% url 'faq:vote_answer' question.category.slug question.slug question.answer_set.first.slug %}{% else %}{% url 'faq:vote_answer' question.slug question.answer_set.first.slug %}{% endif %}" method="post">
+                    {% csrf_token %}
+                    <input type="hidden" value=False name="vote">
+                    <button type="submit">no({{question.answer_set.first.not_helpful}})</button>
+                </form>
+                {% endif %}
+            {% else %}
+                no answers yet
+            {% endif %}
+        {% endif %}
+    
+    
+        {% if can_answer_question %}
+            {% if category_enabled %}
+                <a href="{% url 'faq:answer_question' question.category.slug question.slug %}">answer question</a>
+            {% else %}
+                <a href="{% url 'faq:answer_question' question.slug %}">answer question</a>
+            {% endif %}
+        {% endif %}
+        <hr>
+        {% if comments_allowed %}
+            {% include 'faq/comments.html' %}
+        {% endif %}
+    
+        {% endblock %}
+
+5. answer_form.html - form to add answer to question::
+
+
+        <h1>Answer Question</h1>
+        <a href="{{question.get_absolute_url}}"><h3>{{question.question}}</h3></a>
+        <form method="post">
+            {% csrf_token %}
+            {{form}}
+            <input type="submit">
+        </form>
+
+6. comment_form.html - form to add comments to question (only shows up when form has error because view only gets posted to)::
+
+
+        <h1>Post A Comment</h1>
+        <a href="{{question.get_absolute_url}}"><h3>{{question.question}}</h3></a>
+        <form method="post">
+            {% csrf_token %}
+            {{form}}
+            <input type="submit">
+        </form>
+
+7. question_form.html - form to add a new question::
+
+
+        <h1>Add Your Question</h1>
+        <form method="post">
+            {% csrf_token %}
+            {{form}}
+            <input type="submit">
+        </form>
+
+8. vote_form.html - form for voting questions and answers (only shows up when form has error because view only gets posted to)::
+
+
+        <h1>vote</h1>
+        <form method="post">
+            {% csrf_token %}
+            {{form}}
+            <input type="submit">
+        </form>
+
+9. comments.html - if comments are allowed this template is included in the question detail.html::
+
+
+        <h3>comments</h3>
+        <ul>
+            {% for comment in question.faqcomment_set.all %}
+                <li><h4>{{comment.comment}}</h4>
+                    posted by {% if comment.user%}{{comment.user}}{% else %}anonymous{% endif %} {{comment.post_time|timesince}} ago</li>
+            {% endfor %}
+        </ul>
+        {% if add_new_comment_allowed %}
+            {% if category_enabled %}
+            <form method="post" action="{% url 'faq:add_comment' question.category.slug question.slug %}">
+            {% else %}
+            <form method="post" action="{% url 'faq:add_comment' question.slug %}">
+            {% endif %}
+            <fieldset>
+                <legend>Post Your Comment Here:</legend>
+                {% csrf_token %}
+                {{comment_form}}
+                <input type="submit" name="post">
+            </fieldset>
+            </form>
+        {% endif %}
+
+## Template Variables
+
+1. categories_list.html
+    categories - all the categories (category queryset)
+
+2. categories_detail.html
+    category - the category chosen (category object)
+    can_add_question - bool if the user can add a question (depends on the settings)
+3. questions_list.html
+    questions - all the questions (question queryset)
+    can_add_question - bool if the user can add a question (depends on the settings)
+4. question_detail.html
+    question - the question chosen (question object)
+    can_vote_question - bool if the user can vote a question (depends on the settings)
+    category_enabled - bool if category enabled in settings
+    allow_multiple_answers - bool if multiple answers allowed in settings
+    can_vote_answer - bool if the user can vote an answer (depends on the settings)
+    can_answer_question - bool if current user can answer question (depends on the settings)
+    comments_allowed - bool if using comments in settings
+    add_new_comment_allowed - bool if current user can add comment (depends on the settings)
+    comment_form - form to submit a new comment
+5. answer_form.html
+    question - the question to add answer to (question object)
+    form - form to add new answer
+6. comment_form.html
+    question - the question to add comment to (question object)
+    form - form to add new comment
+7. question_form.html
+    form - form to add new question
+8. vote_form.html
+    form - form to vote for a question or answer
+
+## Urls
+
+all of the following urls are by name then additional
+the app name for the urls is ``'faq'``
+
+* index_view
+    * no arguments
+    * displays all the categories if categories are enabled otherwise shows questions
+* category_detail
+    * needs category slug as slug
+    * displays all the questions given the category when categories are enabled
+* add_question
+    * if categories are enabled needs category slug as slug
+    * if logged_in_users_can_add_question then displays form for logged in users to ask a new question
+* question_detail
+    * needs question slug as question | if categories are enabled needs category slug as slug
+    * displays the main FAQ page with the question all the comments and answers
+* answer_question
+    * needs question slug as question | if categories are enabled needs category slug as category
+    * displays the answer question form
+* add_comment
+    * needs question slug as question | if categories are enabled needs category slug as category
+    * only works if using comments
+    * used to post comment form from question_detail to database
+* vote_answer
+    * needs question slug as question | needs answer slug as answer | if categories are enabled needs category slug as category
+    * only works if using answer voting
+    * used to post hidden input vote = 1 or vote = 0 depending on vote up or down
+* vote_question
+    * needs question slug as question | if categories are enabled needs category slug as category
+    * only works if using question voting
+    * used to post hidden input vote = 1 or vote = 0 depending on vote up or down
+
+## django-tinymce
+If you want to use rich text answers you will need to [install django-tinymce](https://django-tinymce.readthedocs.io/en/latest/installation.html#id2)
+
+Make sure to include in the template the `{{ form.media }}` to include the tinymce javascript and css files.
+> [!WARNING]  
+> Failing to follow the following steps will result in a xss vulnerability in your site.
+
+To allow the rich text answers to be rendered properly you will need to use the safe filter in your templates.
+While django-tinymce does escape the html the answers that were created when the rich text editor was not enabled **has not been escaped and is not safe**.
+So these answers cannot be rendered with the safe filter. So a flag was added to the answer model 'is_rich_text' that is set to True when the answer is created with the rich text editor.
+In the template you can use the following code to render the answer properly::
+
+    {% if answer.is_rich_text %}
+        {{answer.answer|safe}}
+    {% else %}
+        {{answer.answer}}
+    {% endif %}
+
+## Contributing
+
+django-easy-faq aims to be the best faq app for django. It welcomes  contributions of all types - issues, bugs, feature requests, documentation updates, tests and pull requests
+
+## change log
+0.4 fixed bug that logged out users can vote - which then raises exceptions
+
+0.5 fixed migrations
+
+1.0 added pypi distribution
+
+1.1 added more templates to override easily
+
+1.2 fixed bug in pypi distro not including faq app
+
+1.3 fixed bug where a slug must be filled out in admin even though slug gets auto generated to save for questions, answers, and categories. made questions, answers, categories slugs readonly in admin
+
+1.4 added unicode option to add unicode slugs
+
+1.5 added login_required setting to allow faq app to be available to only logged in users
+
+1.6 fixed bug where no_category_description did not do remove the category description in the admin
+
+1.7 added support for django 5.0
+
+1.8 added support for richtext answers with django-tinymce
```

### Comparing `django-easy-faq-1.7/django_easy_faq.egg-info/SOURCES.txt` & `django_easy_faq-1.8/django_easy_faq.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-LICENSE.txt
+LICENSE
 MANIFEST.in
 README.md
-setup.cfg
 setup.py
 django_easy_faq.egg-info/PKG-INFO
 django_easy_faq.egg-info/SOURCES.txt
 django_easy_faq.egg-info/dependency_links.txt
 django_easy_faq.egg-info/requires.txt
 django_easy_faq.egg-info/top_level.txt
 faq/__init__.py
@@ -19,14 +18,15 @@
 faq/urls.py
 faq/views.py
 faq/migrations/0001_initial.py
 faq/migrations/0002_alter_answer_id_alter_answerhelpful_id_and_more.py
 faq/migrations/0003_auto_20220619_0939.py
 faq/migrations/0004_alter_answer_slug_alter_category_slug.py
 faq/migrations/0005_rename_description_category__description.py
+faq/migrations/0006_answer_is_rich_text.py
 faq/migrations/__init__.py
 faq/templates/faq/answer_form.html
 faq/templates/faq/base.html
 faq/templates/faq/categories_list.html
 faq/templates/faq/category_detail.html
 faq/templates/faq/comment_form.html
 faq/templates/faq/comments.html
```

### Comparing `django-easy-faq-1.7/faq/admin.py` & `django_easy_faq-1.8/faq/admin.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-from django.contrib import admin
-from .models import *
-from django.conf import settings
-
-# Register your models here.
-
-class AnswerHelpfulAdmin(admin.ModelAdmin):
-    list_display = ("vote", "answer", "user")
-    list_filter = ('vote',)
-    search_fields = ['answer', "user"]
-
-
-class QuestionHelpfulAdmin(admin.ModelAdmin):
-    list_display = ("vote", "question", "user")
-    list_filter = ('vote',)
-    search_fields = ['question', "user"]
-
-
-class AnswerAdmin(admin.ModelAdmin):
-    list_display = ("answer", "question", "helpful", "not_helpful")
-    list_filter = ('helpful', "not_helpful")
-    search_fields = ['answer', "question"]
-    readonly_fields = ('helpful', "not_helpful", 'slug')
-
-
-class CategoryAdmin(admin.ModelAdmin):
-    search_fields = ['name', "_description"]
-    readonly_fields = ("slug",)
-
-    def get_list_display(self, request):
-        if "no_category_description" not in settings.FAQ_SETTINGS:
-            return ["name", "slug", "description"]
-        return ['name', 'slug']
-
-    def get_exclude(self, request, obj=None):
-        if "no_category_description" in settings.FAQ_SETTINGS:
-            return ['_description']
-        else:
-            return None
-
-class CommentAdmin(admin.ModelAdmin):
-    list_display = ("comment", "question", "user", "post_time")
-    list_filter = ('question', "post_time")
-    search_fields = ['comment', "question"]
-
-
-class QuestionAdmin(admin.ModelAdmin):
-    list_display = ("question", "category", "slug", "helpful", "not_helpful")
-    list_filter = ('helpful', "not_helpful", "category")
-    search_fields = ["question"]
-    readonly_fields = ('helpful', "not_helpful", "slug")
-
-
-admin.site.register(Question, QuestionAdmin)
-admin.site.register(Answer, AnswerAdmin)
-
-# if category enabled
-if "no_category" not in settings.FAQ_SETTINGS:
-    admin.site.register(Category, CategoryAdmin)
-
-# if comments are enabled
-if "no_comments" not in settings.FAQ_SETTINGS:
-    admin.site.register(FAQComment, CommentAdmin)
-
-# if votes are enabled
-if "no_votes" not in settings.FAQ_SETTINGS:
-    # if answer votes are enabled
-    if "no_answer_votes" not in settings.FAQ_SETTINGS:
-        admin.site.register(AnswerHelpful, AnswerHelpfulAdmin)
-
-    # if question votes are enabled
-    if "no_question_votes" not in settings.FAQ_SETTINGS:
-        admin.site.register(QuestionHelpful, QuestionHelpfulAdmin)
+from django.contrib import admin
+from .models import *
+from django.conf import settings
+
+# Register your models here.
+
+class AnswerHelpfulAdmin(admin.ModelAdmin):
+    list_display = ("vote", "answer", "user")
+    list_filter = ('vote',)
+    search_fields = ['answer', "user"]
+
+
+class QuestionHelpfulAdmin(admin.ModelAdmin):
+    list_display = ("vote", "question", "user")
+    list_filter = ('vote',)
+    search_fields = ['question', "user"]
+
+
+class AnswerAdmin(admin.ModelAdmin):
+    list_display = ("answer", "question", "helpful", "not_helpful",'is_rich_text')
+    list_filter = ('helpful', "not_helpful",'is_rich_text')
+    search_fields = ['answer', "question"]
+    readonly_fields = ('helpful', "not_helpful", 'slug','is_rich_text')
+
+
+class CategoryAdmin(admin.ModelAdmin):
+    search_fields = ['name', "_description"]
+    readonly_fields = ("slug",)
+
+    def get_list_display(self, request):
+        if "no_category_description" not in settings.FAQ_SETTINGS:
+            return ["name", "slug", "description"]
+        return ['name', 'slug']
+
+    def get_exclude(self, request, obj=None):
+        if "no_category_description" in settings.FAQ_SETTINGS:
+            return ['_description']
+        else:
+            return None
+
+class CommentAdmin(admin.ModelAdmin):
+    list_display = ("comment", "question", "user", "post_time")
+    list_filter = ('question', "post_time")
+    search_fields = ['comment', "question"]
+
+
+class QuestionAdmin(admin.ModelAdmin):
+    list_display = ("question", "category", "slug", "helpful", "not_helpful")
+    list_filter = ('helpful', "not_helpful", "category")
+    search_fields = ["question"]
+    readonly_fields = ('helpful', "not_helpful", "slug")
+
+
+admin.site.register(Question, QuestionAdmin)
+admin.site.register(Answer, AnswerAdmin)
+
+# if category enabled
+if "no_category" not in settings.FAQ_SETTINGS:
+    admin.site.register(Category, CategoryAdmin)
+
+# if comments are enabled
+if "no_comments" not in settings.FAQ_SETTINGS:
+    admin.site.register(FAQComment, CommentAdmin)
+
+# if votes are enabled
+if "no_votes" not in settings.FAQ_SETTINGS:
+    # if answer votes are enabled
+    if "no_answer_votes" not in settings.FAQ_SETTINGS:
+        admin.site.register(AnswerHelpful, AnswerHelpfulAdmin)
+
+    # if question votes are enabled
+    if "no_question_votes" not in settings.FAQ_SETTINGS:
+        admin.site.register(QuestionHelpful, QuestionHelpfulAdmin)
```

### Comparing `django-easy-faq-1.7/faq/migrations/0002_alter_answer_id_alter_answerhelpful_id_and_more.py` & `django_easy_faq-1.8/faq/migrations/0002_alter_answer_id_alter_answerhelpful_id_and_more.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-# Generated by Django 4.0 on 2021-12-19 14:31
-
-from django.db import migrations, models
-
-
-class Migration(migrations.Migration):
-
-    dependencies = [
-        ('faq', '0001_initial'),
-    ]
-
-    operations = [
-        migrations.AlterField(
-            model_name='answer',
-            name='id',
-            field=models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID'),
-        ),
-        migrations.AlterField(
-            model_name='answerhelpful',
-            name='id',
-            field=models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID'),
-        ),
-        migrations.AlterField(
-            model_name='category',
-            name='id',
-            field=models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID'),
-        ),
-        migrations.AlterField(
-            model_name='faqcomment',
-            name='id',
-            field=models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID'),
-        ),
-        migrations.AlterField(
-            model_name='question',
-            name='id',
-            field=models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID'),
-        ),
-        migrations.AlterField(
-            model_name='questionhelpful',
-            name='id',
-            field=models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID'),
-        ),
-    ]
+# Generated by Django 4.0 on 2021-12-19 14:31
+
+from django.db import migrations, models
+
+
+class Migration(migrations.Migration):
+
+    dependencies = [
+        ('faq', '0001_initial'),
+    ]
+
+    operations = [
+        migrations.AlterField(
+            model_name='answer',
+            name='id',
+            field=models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID'),
+        ),
+        migrations.AlterField(
+            model_name='answerhelpful',
+            name='id',
+            field=models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID'),
+        ),
+        migrations.AlterField(
+            model_name='category',
+            name='id',
+            field=models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID'),
+        ),
+        migrations.AlterField(
+            model_name='faqcomment',
+            name='id',
+            field=models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID'),
+        ),
+        migrations.AlterField(
+            model_name='question',
+            name='id',
+            field=models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID'),
+        ),
+        migrations.AlterField(
+            model_name='questionhelpful',
+            name='id',
+            field=models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID'),
+        ),
+    ]
```

### Comparing `django-easy-faq-1.7/faq/migrations/0004_alter_answer_slug_alter_category_slug.py` & `django_easy_faq-1.8/faq/migrations/0004_alter_answer_slug_alter_category_slug.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# Generated by Django 4.0 on 2022-06-19 16:09
-
-from django.db import migrations, models
-
-
-class Migration(migrations.Migration):
-
-    dependencies = [
-        ('faq', '0003_auto_20220619_0939'),
-    ]
-
-    operations = [
-        migrations.AlterField(
-            model_name='answer',
-            name='slug',
-            field=models.SlugField(blank=True, max_length=10),
-        ),
-        migrations.AlterField(
-            model_name='category',
-            name='slug',
-            field=models.SlugField(blank=True, unique=True),
-        ),
-    ]
+# Generated by Django 4.0 on 2022-06-19 16:09
+
+from django.db import migrations, models
+
+
+class Migration(migrations.Migration):
+
+    dependencies = [
+        ('faq', '0003_auto_20220619_0939'),
+    ]
+
+    operations = [
+        migrations.AlterField(
+            model_name='answer',
+            name='slug',
+            field=models.SlugField(blank=True, max_length=10),
+        ),
+        migrations.AlterField(
+            model_name='category',
+            name='slug',
+            field=models.SlugField(blank=True, unique=True),
+        ),
+    ]
```

### Comparing `django-easy-faq-1.7/faq/models.py` & `django_easy_faq-1.8/faq/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,152 +1,153 @@
-from django.conf import settings
-from django.db import models
-from django.utils.text import slugify
-from django.shortcuts import reverse
-
-from . import snippets
-
-
-# Create your models here.
-class Question(models.Model):
-    category = models.ForeignKey("category", on_delete=models.SET_NULL, null=True, blank=True)
-    question = models.CharField(max_length=150, unique=True)
-    slug = models.SlugField(max_length=150, unique=True, blank=True)
-    helpful = models.IntegerField(default=0)
-    not_helpful = models.IntegerField(default=0)
-
-    def get_helpful(self):
-        return QuestionHelpful.objects.filter(question=self, vote=True).count()
-
-    def get_not_helpful(self):
-        return QuestionHelpful.objects.filter(question=self, vote=False).count()
-
-    def __str__(self):
-        return self.question
-
-    def save(self, *args, **kwargs):
-        self.slug = slugify(self.question, allow_unicode='allow_unicode' in settings.FAQ_SETTINGS)[:150]
-        # if question already exists
-        if self.pk:
-            self.helpful = self.get_helpful()
-            self.not_helpful = self.get_not_helpful()
-        return super().save(*args, **kwargs)
-
-    def get_absolute_url(self):
-        # if using categories
-        if "no_category" not in settings.FAQ_SETTINGS:
-            return reverse("faq:question_detail", args=(self.category.slug, self.slug))
-        else:
-            return reverse("faq:question_detail", args=(self.slug,))
-
-
-    class Meta:
-        app_label = 'faq'
-
-
-class Answer(models.Model):
-    question = models.ForeignKey(Question, on_delete=models.CASCADE)
-    answer = models.TextField()
-    slug = models.SlugField(max_length=10, blank=True)
-    helpful = models.IntegerField(default=0)
-    not_helpful = models.IntegerField(default=0)
-
-    def get_helpful(self):
-        return AnswerHelpful.objects.filter(answer=self, vote=True).count()
-
-    def get_not_helpful(self):
-        return AnswerHelpful.objects.filter(answer=self, vote=False).count()
-
-    def __str__(self):
-        return self.answer
-
-    class Meta:
-        order_with_respect_to = 'question'
-        app_label = 'faq'
-
-    def save(self, *args, **kwargs):
-        # if first time saving add a new slug
-        if not self.pk or not self.slug:
-            new_slug = snippets.create_random_slug(5)
-            while Answer.objects.filter(slug=new_slug, answer=self.answer).exists():
-                new_slug = snippets.create_random_slug()
-            self.slug = new_slug
-        # if answer is not new
-        if self.pk:
-            self.helpful = self.get_helpful()
-            self.not_helpful = self.get_not_helpful()
-        super().save(*args, **kwargs)
-
-
-class Category(models.Model):
-    name = models.CharField(max_length=50, unique=True)
-    _description = models.TextField()
-    slug = models.SlugField(max_length=50, unique=True, blank=True)
-
-    def __str__(self):
-        return self.name
-
-    class Meta:
-        verbose_name_plural = "categories"
-        app_label = 'faq'
-
-    @property
-    def description(self):
-        """only show the description is categories have descriptions"""
-        if "no_category_description" in settings.FAQ_SETTINGS:
-            return None
-        else:
-            return self._description
-
-    def save(self, *args, **kwargs):
-        self.slug = slugify(self.name, allow_unicode='allow_unicode' in settings.FAQ_SETTINGS)[:50]
-        return super().save(*args, **kwargs)
-
-
-class FAQComment(models.Model):
-    user = models.ForeignKey(settings.AUTH_USER_MODEL, on_delete=models.CASCADE, null=True)
-    comment = models.TextField()
-    question = models.ForeignKey(Question, on_delete=models.CASCADE)
-    post_time = models.DateTimeField(auto_now_add=True)
-
-    def __str__(self):
-        return self.comment
-
-    class Meta:
-        ordering = ['question', '-post_time']
-        app_label = 'faq'
-
-
-class AnswerHelpful(models.Model):
-    user = models.ForeignKey(settings.AUTH_USER_MODEL, on_delete=models.CASCADE)
-    answer = models.ForeignKey(Answer, on_delete=models.CASCADE)
-    vote = models.BooleanField()
-
-    def __str__(self):
-        if self.vote:
-            vote_var = 'like'
-        else:
-            vote_var = 'dislike'
-
-        return str(self.answer) + '- ' + vote_var
-
-    class Meta:
-        ordering = ['answer', 'vote']
-        app_label = 'faq'
-
-
-class QuestionHelpful(models.Model):
-    user = models.ForeignKey(settings.AUTH_USER_MODEL, on_delete=models.CASCADE)
-    question = models.ForeignKey(Question, on_delete=models.CASCADE)
-    vote = models.BooleanField()
-
-    def __str__(self):
-        if self.vote:
-            vote_var = 'like'
-        else:
-            vote_var = 'dislike'
-
-        return str(self.question) + '- ' + vote_var
-
-    class Meta:
-        ordering = ['question', 'vote']
-        app_label = 'faq'
+from django.conf import settings
+from django.db import models
+from django.utils.text import slugify
+from django.shortcuts import reverse
+
+from . import snippets
+
+
+# Create your models here.
+class Question(models.Model):
+    category = models.ForeignKey("category", on_delete=models.SET_NULL, null=True, blank=True)
+    question = models.CharField(max_length=150, unique=True)
+    slug = models.SlugField(max_length=150, unique=True, blank=True)
+    helpful = models.IntegerField(default=0)
+    not_helpful = models.IntegerField(default=0)
+
+    def get_helpful(self):
+        return QuestionHelpful.objects.filter(question=self, vote=True).count()
+
+    def get_not_helpful(self):
+        return QuestionHelpful.objects.filter(question=self, vote=False).count()
+
+    def __str__(self):
+        return self.question
+
+    def save(self, *args, **kwargs):
+        self.slug = slugify(self.question, allow_unicode='allow_unicode' in settings.FAQ_SETTINGS)[:150]
+        # if question already exists
+        if self.pk:
+            self.helpful = self.get_helpful()
+            self.not_helpful = self.get_not_helpful()
+        return super().save(*args, **kwargs)
+
+    def get_absolute_url(self):
+        # if using categories
+        if "no_category" not in settings.FAQ_SETTINGS:
+            return reverse("faq:question_detail", args=(self.category.slug, self.slug))
+        else:
+            return reverse("faq:question_detail", args=(self.slug,))
+
+
+    class Meta:
+        app_label = 'faq'
+
+
+class Answer(models.Model):
+    question = models.ForeignKey(Question, on_delete=models.CASCADE)
+    answer = models.TextField()
+    slug = models.SlugField(max_length=10, blank=True)
+    helpful = models.IntegerField(default=0)
+    not_helpful = models.IntegerField(default=0)
+    is_rich_text = models.BooleanField(default=False)
+
+    def get_helpful(self):
+        return AnswerHelpful.objects.filter(answer=self, vote=True).count()
+
+    def get_not_helpful(self):
+        return AnswerHelpful.objects.filter(answer=self, vote=False).count()
+
+    def __str__(self):
+        return self.answer
+
+    class Meta:
+        order_with_respect_to = 'question'
+        app_label = 'faq'
+
+    def save(self, *args, **kwargs):
+        # if first time saving add a new slug
+        if not self.pk or not self.slug:
+            new_slug = snippets.create_random_slug(5)
+            while Answer.objects.filter(slug=new_slug, answer=self.answer).exists():
+                new_slug = snippets.create_random_slug()
+            self.slug = new_slug
+        # if answer is not new
+        if self.pk:
+            self.helpful = self.get_helpful()
+            self.not_helpful = self.get_not_helpful()
+        super().save(*args, **kwargs)
+
+
+class Category(models.Model):
+    name = models.CharField(max_length=50, unique=True)
+    _description = models.TextField()
+    slug = models.SlugField(max_length=50, unique=True, blank=True)
+
+    def __str__(self):
+        return self.name
+
+    class Meta:
+        verbose_name_plural = "categories"
+        app_label = 'faq'
+
+    @property
+    def description(self):
+        """only show the description is categories have descriptions"""
+        if "no_category_description" in settings.FAQ_SETTINGS:
+            return None
+        else:
+            return self._description
+
+    def save(self, *args, **kwargs):
+        self.slug = slugify(self.name, allow_unicode='allow_unicode' in settings.FAQ_SETTINGS)[:50]
+        return super().save(*args, **kwargs)
+
+
+class FAQComment(models.Model):
+    user = models.ForeignKey(settings.AUTH_USER_MODEL, on_delete=models.CASCADE, null=True)
+    comment = models.TextField()
+    question = models.ForeignKey(Question, on_delete=models.CASCADE)
+    post_time = models.DateTimeField(auto_now_add=True)
+
+    def __str__(self):
+        return self.comment
+
+    class Meta:
+        ordering = ['question', '-post_time']
+        app_label = 'faq'
+
+
+class AnswerHelpful(models.Model):
+    user = models.ForeignKey(settings.AUTH_USER_MODEL, on_delete=models.CASCADE)
+    answer = models.ForeignKey(Answer, on_delete=models.CASCADE)
+    vote = models.BooleanField()
+
+    def __str__(self):
+        if self.vote:
+            vote_var = 'like'
+        else:
+            vote_var = 'dislike'
+
+        return str(self.answer) + '- ' + vote_var
+
+    class Meta:
+        ordering = ['answer', 'vote']
+        app_label = 'faq'
+
+
+class QuestionHelpful(models.Model):
+    user = models.ForeignKey(settings.AUTH_USER_MODEL, on_delete=models.CASCADE)
+    question = models.ForeignKey(Question, on_delete=models.CASCADE)
+    vote = models.BooleanField()
+
+    def __str__(self):
+        if self.vote:
+            vote_var = 'like'
+        else:
+            vote_var = 'dislike'
+
+        return str(self.question) + '- ' + vote_var
+
+    class Meta:
+        ordering = ['question', 'vote']
+        app_label = 'faq'
```

### Comparing `django-easy-faq-1.7/faq/snippets.py` & `django_easy_faq-1.8/faq/snippets.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-import secrets
-from django.conf import settings
-
-ALL_URL_CHARS = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789"
-
-
-def create_random_slug(size=10):
-    """amount of characters you want generated for random_slug"""
-    res = ''.join(secrets.choice(ALL_URL_CHARS) for _ in range(size))
-    return str(res)
-
-
-def get_template_settings(request):
-    """returns most of the settings to be added into get_context_data method"""
-    context = {}
-    # if using categories
-    if "no_category" not in settings.FAQ_SETTINGS:
-        context['category_enabled'] = True
-    else:
-        context['category_enabled'] = False
-
-    if "allow_multiple_answers" in settings.FAQ_SETTINGS:
-        context['allow_multiple_answers'] = True
-    else:
-        context['allow_multiple_answers'] = False
-
-    # if using comments
-    if "no_comments" not in settings.FAQ_SETTINGS:
-        context["comments_allowed"] = True
-        if "anonymous_user_can_comment" in settings.FAQ_SETTINGS:
-            context['add_new_comment_allowed'] = True
-        else:
-            if request.user.is_authenticated:
-                context['add_new_comment_allowed'] = True
-            else:
-                context['add_new_comment_allowed'] = False
-
-        if "view_only_comments" in settings.FAQ_SETTINGS:
-            context['add_new_comment_allowed'] = False
-    else:
-        context["comments_allowed"] = False
-
-    # if can vote on answers
-    if "no_votes" not in settings.FAQ_SETTINGS:
-        # if can vote answer
-        if "no_answer_votes" not in settings.FAQ_SETTINGS:
-            if request.user.is_authenticated:
-                context["can_vote_answer"] = True
-            else:
-                context["can_vote_answer"] = False
-        else:
-
-            context["can_vote_answer"] = False
-
-        if "no_question_votes" not in settings.FAQ_SETTINGS:
-            if request.user.is_authenticated:
-                context["can_vote_question"] = True
-            else:
-                context["can_vote_question"] = False
-        else:
-
-            context["can_vote_question"] = False
-    else:
-        context["can_vote_answer"] = False
-        context["can_vote_question"] = False
-
-    context["can_add_question"] = False
-    if "logged_in_users_can_add_question" in settings.FAQ_SETTINGS:
-        if request.user.is_authenticated:
-            context["can_add_question"] = True
-
-    return context
+import secrets
+from django.conf import settings
+
+ALL_URL_CHARS = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789"
+
+
+def create_random_slug(size=10):
+    """amount of characters you want generated for random_slug"""
+    res = ''.join(secrets.choice(ALL_URL_CHARS) for _ in range(size))
+    return str(res)
+
+
+def get_template_settings(request):
+    """returns most of the settings to be added into get_context_data method"""
+    context = {}
+    # if using categories
+    if "no_category" not in settings.FAQ_SETTINGS:
+        context['category_enabled'] = True
+    else:
+        context['category_enabled'] = False
+
+    if "allow_multiple_answers" in settings.FAQ_SETTINGS:
+        context['allow_multiple_answers'] = True
+    else:
+        context['allow_multiple_answers'] = False
+
+    # if using comments
+    if "no_comments" not in settings.FAQ_SETTINGS:
+        context["comments_allowed"] = True
+        if "anonymous_user_can_comment" in settings.FAQ_SETTINGS:
+            context['add_new_comment_allowed'] = True
+        else:
+            if request.user.is_authenticated:
+                context['add_new_comment_allowed'] = True
+            else:
+                context['add_new_comment_allowed'] = False
+
+        if "view_only_comments" in settings.FAQ_SETTINGS:
+            context['add_new_comment_allowed'] = False
+    else:
+        context["comments_allowed"] = False
+
+    # if can vote on answers
+    if "no_votes" not in settings.FAQ_SETTINGS:
+        # if can vote answer
+        if "no_answer_votes" not in settings.FAQ_SETTINGS:
+            if request.user.is_authenticated:
+                context["can_vote_answer"] = True
+            else:
+                context["can_vote_answer"] = False
+        else:
+
+            context["can_vote_answer"] = False
+
+        if "no_question_votes" not in settings.FAQ_SETTINGS:
+            if request.user.is_authenticated:
+                context["can_vote_question"] = True
+            else:
+                context["can_vote_question"] = False
+        else:
+
+            context["can_vote_question"] = False
+    else:
+        context["can_vote_answer"] = False
+        context["can_vote_question"] = False
+
+    context["can_add_question"] = False
+    if "logged_in_users_can_add_question" in settings.FAQ_SETTINGS:
+        if request.user.is_authenticated:
+            context["can_add_question"] = True
+
+    return context
```

### Comparing `django-easy-faq-1.7/faq/templates/faq/question_base.html` & `django_easy_faq-1.8/faq/templates/faq/question_base.html`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-{% extends 'faq/base.html' %}
-{% block title %}FAQ | {{question.question|title}}{% endblock %}
-{% block heading %}{{question.question|title}}{% endblock %}
-
-{% block content %}
-{% if can_vote_question %}
-    found this question helpful?
-    <form style="display: inline;" action="{% if category_enabled %}{% url 'faq:vote_question' question.category.slug question.slug %}{% else %}{% url 'faq:vote_question' question.slug %}{% endif %}" method="post">
-        {% csrf_token %}
-        <input type="hidden" value=True name="vote">
-        <button type="submit">yes({{question.helpful}})</button>
-    </form>
-    <form style="display: inline;" action="{% if category_enabled %}{% url 'faq:vote_question' question.category.slug question.slug %}{% else %}{% url 'faq:vote_question' question.slug %}{% endif %}" method="post">
-        {% csrf_token %}
-        <input type="hidden" value=False name="vote">
-         <button type="submit">no({{question.not_helpful}})</button>
-    </form>
-{% endif %}
-{% if question.category and category_enabled %}
-    <p>category - <a href="{% url 'faq:category_detail' question.category.slug %}">{{question.category.name}}</a></p>
-{% endif %}
-<hr/>
-
-{% block question_content %}
-{% endblock %}
-
+{% extends 'faq/base.html' %}
+{% block title %}FAQ | {{question.question|title}}{% endblock %}
+{% block heading %}{{question.question|title}}{% endblock %}
+
+{% block content %}
+{% if can_vote_question %}
+    found this question helpful?
+    <form style="display: inline;" action="{% if category_enabled %}{% url 'faq:vote_question' question.category.slug question.slug %}{% else %}{% url 'faq:vote_question' question.slug %}{% endif %}" method="post">
+        {% csrf_token %}
+        <input type="hidden" value=True name="vote">
+        <button type="submit">yes({{question.helpful}})</button>
+    </form>
+    <form style="display: inline;" action="{% if category_enabled %}{% url 'faq:vote_question' question.category.slug question.slug %}{% else %}{% url 'faq:vote_question' question.slug %}{% endif %}" method="post">
+        {% csrf_token %}
+        <input type="hidden" value=False name="vote">
+         <button type="submit">no({{question.not_helpful}})</button>
+    </form>
+{% endif %}
+{% if question.category and category_enabled %}
+    <p>category - <a href="{% url 'faq:category_detail' question.category.slug %}">{{question.category.name}}</a></p>
+{% endif %}
+<hr/>
+
+{% block question_content %}
+{% endblock %}
+
 {% endblock %}
```

### Comparing `django-easy-faq-1.7/faq/templates/faq/question_detail.html` & `django_easy_faq-1.8/faq/templates/faq/question_detail.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,61 +1,70 @@
-{% extends 'faq/question_base.html' %}
-
-{% block question_content %}
-{% if allow_multiple_answers %}
-<h3>answers</h3>
-<ul>
-    {% for answer in question.answer_set.all %}
-        <li><b>{{answer.answer}}</b>
-            {% if can_vote_answer %}
-             | found this answer helpful?
-            <form style="display: inline;" action="{% if category_enabled %}{% url 'faq:vote_answer' question.category.slug question.slug answer.slug %}{% else %}{% url 'faq:vote_answer' question.slug answer.slug %}{% endif %}" method="post">
-                {% csrf_token %}
-                <input type="hidden" value=True name="vote">
-                <button type="submit">yes({{answer.helpful}})</button>
-            </form>
-            <form style="display: inline;" action="{% if category_enabled %}{% url 'faq:vote_answer' question.category.slug question.slug answer.slug %}{% else %}{% url 'faq:vote_answer' question.slug answer.slug %}{% endif %}" method="post">
-                {% csrf_token %}
-                <input type="hidden" value=False name="vote">
-                <button type="submit">no({{answer.not_helpful}})</button>
-            </form>
-            {% endif %}
-        </li>
-    {% endfor %}
-</ul>
-
-{% else %}
-    {% if question.answer_set.exists %}
-        <p>answer:</p>
-        <h3>{{question.answer_set.first.answer}}</h3>
-        {% if can_vote_answer %}
-         found this answer helpful?
-        <form style="display: inline;" action="{% if category_enabled %}{% url 'faq:vote_answer' question.category.slug question.slug question.answer_set.first.slug %}{% else %}{% url 'faq:vote_answer' question.slug question.answer_set.first.slug %}{% endif %}" method="post">
-            {% csrf_token %}
-            <input type="hidden" value=True name="vote">
-            <button type="submit">yes({{question.answer_set.first.helpful}})</button>
-        </form>
-        <form style="display: inline;" action="{% if category_enabled %}{% url 'faq:vote_answer' question.category.slug question.slug question.answer_set.first.slug %}{% else %}{% url 'faq:vote_answer' question.slug question.answer_set.first.slug %}{% endif %}" method="post">
-            {% csrf_token %}
-            <input type="hidden" value=False name="vote">
-            <button type="submit">no({{question.answer_set.first.not_helpful}})</button>
-        </form>
-        {% endif %}
-    {% else %}
-        no answers yet
-    {% endif %}
-{% endif %}
-
-
-{% if can_answer_question %}
-    {% if category_enabled %}
-        <a href="{% url 'faq:answer_question' question.category.slug question.slug %}">answer question</a>
-    {% else %}
-        <a href="{% url 'faq:answer_question' question.slug %}">answer question</a>
-    {% endif %}
-{% endif %}
-<hr>
-{% if comments_allowed %}
-    {% include 'faq/comments.html' %}
-{% endif %}
-
+{% extends 'faq/question_base.html' %}
+
+{% block question_content %}
+{% if allow_multiple_answers %}
+<h3>answers</h3>
+<ul>
+    {% for answer in question.answer_set.all %}
+        <li>
+        {% if answer.is_rich_text %}
+            {{ answer.answer|safe }}
+        {% else %}
+            <b>{{answer.answer}}</b>
+        {% endif %}
+            {% if can_vote_answer %}
+             | found this answer helpful?
+            <form style="display: inline;" action="{% if category_enabled %}{% url 'faq:vote_answer' question.category.slug question.slug answer.slug %}{% else %}{% url 'faq:vote_answer' question.slug answer.slug %}{% endif %}" method="post">
+                {% csrf_token %}
+                <input type="hidden" value=True name="vote">
+                <button type="submit">yes({{answer.helpful}})</button>
+            </form>
+            <form style="display: inline;" action="{% if category_enabled %}{% url 'faq:vote_answer' question.category.slug question.slug answer.slug %}{% else %}{% url 'faq:vote_answer' question.slug answer.slug %}{% endif %}" method="post">
+                {% csrf_token %}
+                <input type="hidden" value=False name="vote">
+                <button type="submit">no({{answer.not_helpful}})</button>
+            </form>
+            {% endif %}
+        </li>
+    {% endfor %}
+</ul>
+
+{% else %}
+    {% if question.answer_set.exists %}
+        <p>answer:</p>
+        {% if question.answer_set.first.is_rich_text %}
+            <p>{{question.answer_set.first.answer|safe}}</p>
+        {% else %}
+            <h3>{{question.answer_set.first.answer}}</h3>
+        {% endif %}
+        {% if can_vote_answer %}
+         found this answer helpful?
+        <form style="display: inline;" action="{% if category_enabled %}{% url 'faq:vote_answer' question.category.slug question.slug question.answer_set.first.slug %}{% else %}{% url 'faq:vote_answer' question.slug question.answer_set.first.slug %}{% endif %}" method="post">
+            {% csrf_token %}
+            <input type="hidden" value=True name="vote">
+            <button type="submit">yes({{question.answer_set.first.helpful}})</button>
+        </form>
+        <form style="display: inline;" action="{% if category_enabled %}{% url 'faq:vote_answer' question.category.slug question.slug question.answer_set.first.slug %}{% else %}{% url 'faq:vote_answer' question.slug question.answer_set.first.slug %}{% endif %}" method="post">
+            {% csrf_token %}
+            <input type="hidden" value=False name="vote">
+            <button type="submit">no({{question.answer_set.first.not_helpful}})</button>
+        </form>
+        {% endif %}
+    {% else %}
+        no answers yet
+    {% endif %}
+{% endif %}
+
+
+{% if can_answer_question %}
+    {% if category_enabled %}
+        <a href="{% url 'faq:answer_question' question.category.slug question.slug %}">answer question</a>
+    {% else %}
+        <a href="{% url 'faq:answer_question' question.slug %}">answer question</a>
+    {% endif %}
+{% endif %}
+<hr>
+{% if comments_allowed %}
+    {% include 'faq/comments.html' %}
+{% endif %}
+
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,20 +1,25 @@
 {% extends 'faq/question_base.html' %} {% block question_content %} {% if
 allow_multiple_answers %}
 ******** aannsswweerrss ********
     * {% for answer in question.answer_set.all %}
-    * {{{{aannsswweerr..aannsswweerr}}}} {% if can_vote_answer %} | found this answer helpful?
+    * {% if answer.is_rich_text %} {{ answer.answer|safe }} {% else %} {{
+      {{aannsswweerr..aannsswweerr}}}} {% endif %} {% if can_vote_answer %} | found this answer
+      helpful?
       {% csrf_token %} yes({{answer.helpful}})
       {% csrf_token %} no({{answer.not_helpful}})
       {% endif %}
     * {% endfor %}
 {% else %} {% if question.answer_set.exists %}
 answer:
+{% if question.answer_set.first.is_rich_text %}
+{{question.answer_set.first.answer|safe}}
+{% else %}
 ******** {{{{qquueessttiioonn..aannsswweerr__sseett..ffiirrsstt..aannsswweerr}}}} ********
-{% if can_vote_answer %} found this answer helpful?
+{% endif %} {% if can_vote_answer %} found this answer helpful?
 {% csrf_token %} yes({{question.answer_set.first.helpful}})
 {% csrf_token %} no({{question.answer_set.first.not_helpful}})
 {% endif %} {% else %} no answers yet {% endif %} {% endif %} {% if
 can_answer_question %} {% if category_enabled %} _a_n_s_w_e_r_ _q_u_e_s_t_i_o_n {% else %}
 _a_n_s_w_e_r_ _q_u_e_s_t_i_o_n {% endif %} {% endif %}
 ===============================================================================
 {% if comments_allowed %} {% include 'faq/comments.html' %} {% endif %} {%
```

### Comparing `django-easy-faq-1.7/faq/tests.py` & `django_easy_faq-1.8/faq/tests.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,176 +1,176 @@
-from django.test import TestCase, RequestFactory, override_settings
-from django.shortcuts import reverse
-from faq.views import IndexView, CategoryDetail, QuestionDetail
-from faq import models
-from django.contrib.auth.models import User, AnonymousUser
-
-
-# Create your tests here.
-
-class IndexViewTestCase(TestCase):
-
-    @override_settings(FAQ_SETTINGS=["no_category"])
-    def test_get_template_names_no_categories(self):
-        """gets correct template when not using categories"""
-        request = RequestFactory().get(reverse("faq:index_view"))
-        view = IndexView()
-        view.setup(request)
-
-        self.assertEqual(view.get_template_names(), "faq/questions_list.html")
-        self.assertNotEqual(view.get_template_names(), "faq/categories_list.html")
-
-    @override_settings(FAQ_SETTINGS=[])
-    def test_get_template_names_categories(self):
-        """gets correct template when not using categories"""
-        request = RequestFactory().get(reverse("faq:index_view"))
-        view = IndexView()
-        view.setup(request)
-
-        self.assertNotEqual(view.get_template_names(), "faq/questions_list.html")
-        self.assertEqual(view.get_template_names(), "faq/categories_list.html")
-
-
-    @override_settings(FAQ_SETTINGS=["no_category"])
-    def test_get_queryset_no_categories(self):
-        """gets correct query set when not using categories"""
-        request = RequestFactory().get(reverse("faq:index_view"))
-        view = IndexView()
-        view.setup(request)
-
-        models.Question.objects.create(question="?")
-        models.Question.objects.create(question="the?")
-        view.get_queryset()
-
-        self.assertEqual(view.get_queryset().first(), models.Question.objects.first())
-        self.assertNotEqual(view.get_queryset().first(), models.Question.objects.last())
-        self.assertNotEqual(view.get_queryset().first(), models.Category.objects.first())
-
-    @override_settings(FAQ_SETTINGS=[])
-    def test_get_queryset_categories(self):
-        """gets correct query set when using categories"""
-        request = RequestFactory().get(reverse("faq:index_view"))
-        view = IndexView()
-        view.setup(request)
-
-        category = models.Category.objects.create(name="category", _description="this is a category")
-        models.Category.objects.create(name="category 2", _description="this is a category")
-        models.Question.objects.create(question="category question", category=category)
-        models.Question.objects.create(question="category question 2", category=category)
-        models.Question.objects.create(question="question not in category")
-
-        self.assertEqual(view.get_queryset().first(), models.Category.objects.first())
-        self.assertNotEqual(view.get_queryset().first(), models.Question.objects.first())
-        self.assertNotEqual(view.get_queryset().first(), models.Category.objects.last())
-
-    @override_settings(FAQ_SETTINGS=[])
-    def test_get_context_object_name_categories(self):
-        """gets correct template variable when using categories"""
-        request = RequestFactory().get(reverse("faq:index_view"))
-        view = IndexView()
-        view.setup(request)
-
-        self.assertEqual(view.get_context_object_name([]), "categories")
-        self.assertNotEqual(view.get_context_object_name([]), "questions")
-
-    @override_settings(FAQ_SETTINGS=["no_category"])
-    def test_get_context_object_name_no_categories(self):
-        """gets correct template variable when not using categories"""
-        request = RequestFactory().get(reverse("faq:index_view"))
-        view = IndexView()
-        view.setup(request)
-
-        self.assertEqual(view.get_context_object_name([]), "questions")
-        self.assertNotEqual(view.get_context_object_name([]), "categories")
-
-    @override_settings(FAQ_SETTINGS=["no_category"])
-    def test_get_context_data_not_using_categories(self):
-        """gets context data correctly when not using categories"""
-        request = RequestFactory().get(reverse("faq:index_view"))
-        request.user = AnonymousUser()
-        view = IndexView()
-        view.object_list = view.get_queryset()
-        view.setup(request)
-
-        self.assertIn("can_add_question", view.get_context_data())
-
-    @override_settings(FAQ_SETTINGS=[])
-    def test_get_context_data_using_categories(self):
-        """gets context data correctly when using categories"""
-        request = RequestFactory().get(reverse("faq:index_view"))
-        request.user = AnonymousUser()
-        view = IndexView()
-        view.object_list = view.get_queryset()
-        view.setup(request)
-
-        self.assertEqual(view.get_context_data()['can_add_question'],False)
-
-    @override_settings(FAQ_SETTINGS=["no_category", "logged_in_users_can_add_question"])
-    def test_get_context_data_not_using_categories_logged_in_can_add(self):
-        """gets context data correctly when not using categories and logged_in_users_can_add_question"""
-        request = RequestFactory()
-        request = request.get(reverse("faq:index_view"))
-        request.user = User.objects.create_user(username="jim", password="the")
-        view = IndexView()
-        view.object_list = view.get_queryset()
-        view.setup(request)
-
-        self.assertIn("can_add_question", view.get_context_data())
-
-
-class CategoryDetailTestCase(TestCase):
-    def setUp(self):
-        models.Category.objects.create(name="cat1", _description="descript")
-        models.Category.objects.create(name="cat2", _description="descript2")
-        models.Category.objects.create(name="cat3")
-
-
-class QuestionViewTestCase(TestCase):
-    def setUp(self):
-        category = models.Category.objects.create(name="cat1", _description="descript")
-
-        models.Question.objects.create(category=category, question="great question")
-
-    @override_settings(FAQ_SETTINGS=[])
-    def test_anonymous_user_cant_vote(self):
-        """a user doesn't get a link to vote"""
-
-        question = models.Question.objects.first()
-        response = self.client.get(reverse("faq:question_detail", args=(question.category.slug, question.slug,)))
-
-        self.assertEqual(response.context['can_vote_question'], False)
-        self.assertEqual(response.context['can_vote_answer'], False)
-
-
-class VoteQuestionTestCase(TestCase):
-    def setUp(self):
-        category = models.Category.objects.create(name="cat1", _description="descript")
-
-        models.Question.objects.create(category=category, question="great question")
-
-    @override_settings(FAQ_SETTINGS=[])
-    def test_anonymous_user_cant_vote(self):
-        """redirects logged out users to login page"""
-
-        question = models.Question.objects.first()
-        response = self.client.post(reverse("faq:vote_question", args=(question.category.slug, question.slug,)))
-
-        self.assertEqual(response.status_code, 302)
-
-
-class VoteanswerTestCase(TestCase):
-    def setUp(self):
-        category = models.Category.objects.create(name="cat1", _description="descript")
-
-        question = models.Question.objects.create(category=category, question="great question")
-
-        self.answer = models.Answer.objects.create(question=question, answer="because")
-
-    @override_settings(FAQ_SETTINGS=[])
-    def test_anonymous_user_cant_vote(self):
-        """redirects logged out users to login page"""
-
-        question = models.Question.objects.first()
-        response = self.client.post(
-                reverse("faq:vote_answer", args=(question.category.slug, question.slug, self.answer.slug)))
-
-        self.assertEqual(response.status_code, 302)
+from django.test import TestCase, RequestFactory, override_settings
+from django.shortcuts import reverse
+from faq.views import IndexView, CategoryDetail, QuestionDetail
+from faq import models
+from django.contrib.auth.models import User, AnonymousUser
+
+
+# Create your tests here.
+
+class IndexViewTestCase(TestCase):
+
+    @override_settings(FAQ_SETTINGS=["no_category"])
+    def test_get_template_names_no_categories(self):
+        """gets correct template when not using categories"""
+        request = RequestFactory().get(reverse("faq:index_view"))
+        view = IndexView()
+        view.setup(request)
+
+        self.assertEqual(view.get_template_names(), "faq/questions_list.html")
+        self.assertNotEqual(view.get_template_names(), "faq/categories_list.html")
+
+    @override_settings(FAQ_SETTINGS=[])
+    def test_get_template_names_categories(self):
+        """gets correct template when not using categories"""
+        request = RequestFactory().get(reverse("faq:index_view"))
+        view = IndexView()
+        view.setup(request)
+
+        self.assertNotEqual(view.get_template_names(), "faq/questions_list.html")
+        self.assertEqual(view.get_template_names(), "faq/categories_list.html")
+
+
+    @override_settings(FAQ_SETTINGS=["no_category"])
+    def test_get_queryset_no_categories(self):
+        """gets correct query set when not using categories"""
+        request = RequestFactory().get(reverse("faq:index_view"))
+        view = IndexView()
+        view.setup(request)
+
+        models.Question.objects.create(question="?")
+        models.Question.objects.create(question="the?")
+        view.get_queryset()
+
+        self.assertEqual(view.get_queryset().first(), models.Question.objects.first())
+        self.assertNotEqual(view.get_queryset().first(), models.Question.objects.last())
+        self.assertNotEqual(view.get_queryset().first(), models.Category.objects.first())
+
+    @override_settings(FAQ_SETTINGS=[])
+    def test_get_queryset_categories(self):
+        """gets correct query set when using categories"""
+        request = RequestFactory().get(reverse("faq:index_view"))
+        view = IndexView()
+        view.setup(request)
+
+        category = models.Category.objects.create(name="category", _description="this is a category")
+        models.Category.objects.create(name="category 2", _description="this is a category")
+        models.Question.objects.create(question="category question", category=category)
+        models.Question.objects.create(question="category question 2", category=category)
+        models.Question.objects.create(question="question not in category")
+
+        self.assertEqual(view.get_queryset().first(), models.Category.objects.first())
+        self.assertNotEqual(view.get_queryset().first(), models.Question.objects.first())
+        self.assertNotEqual(view.get_queryset().first(), models.Category.objects.last())
+
+    @override_settings(FAQ_SETTINGS=[])
+    def test_get_context_object_name_categories(self):
+        """gets correct template variable when using categories"""
+        request = RequestFactory().get(reverse("faq:index_view"))
+        view = IndexView()
+        view.setup(request)
+
+        self.assertEqual(view.get_context_object_name([]), "categories")
+        self.assertNotEqual(view.get_context_object_name([]), "questions")
+
+    @override_settings(FAQ_SETTINGS=["no_category"])
+    def test_get_context_object_name_no_categories(self):
+        """gets correct template variable when not using categories"""
+        request = RequestFactory().get(reverse("faq:index_view"))
+        view = IndexView()
+        view.setup(request)
+
+        self.assertEqual(view.get_context_object_name([]), "questions")
+        self.assertNotEqual(view.get_context_object_name([]), "categories")
+
+    @override_settings(FAQ_SETTINGS=["no_category"])
+    def test_get_context_data_not_using_categories(self):
+        """gets context data correctly when not using categories"""
+        request = RequestFactory().get(reverse("faq:index_view"))
+        request.user = AnonymousUser()
+        view = IndexView()
+        view.object_list = view.get_queryset()
+        view.setup(request)
+
+        self.assertIn("can_add_question", view.get_context_data())
+
+    @override_settings(FAQ_SETTINGS=[])
+    def test_get_context_data_using_categories(self):
+        """gets context data correctly when using categories"""
+        request = RequestFactory().get(reverse("faq:index_view"))
+        request.user = AnonymousUser()
+        view = IndexView()
+        view.object_list = view.get_queryset()
+        view.setup(request)
+
+        self.assertEqual(view.get_context_data()['can_add_question'],False)
+
+    @override_settings(FAQ_SETTINGS=["no_category", "logged_in_users_can_add_question"])
+    def test_get_context_data_not_using_categories_logged_in_can_add(self):
+        """gets context data correctly when not using categories and logged_in_users_can_add_question"""
+        request = RequestFactory()
+        request = request.get(reverse("faq:index_view"))
+        request.user = User.objects.create_user(username="jim", password="the")
+        view = IndexView()
+        view.object_list = view.get_queryset()
+        view.setup(request)
+
+        self.assertIn("can_add_question", view.get_context_data())
+
+
+class CategoryDetailTestCase(TestCase):
+    def setUp(self):
+        models.Category.objects.create(name="cat1", _description="descript")
+        models.Category.objects.create(name="cat2", _description="descript2")
+        models.Category.objects.create(name="cat3")
+
+
+class QuestionViewTestCase(TestCase):
+    def setUp(self):
+        category = models.Category.objects.create(name="cat1", _description="descript")
+
+        models.Question.objects.create(category=category, question="great question")
+
+    @override_settings(FAQ_SETTINGS=[])
+    def test_anonymous_user_cant_vote(self):
+        """a user doesn't get a link to vote"""
+
+        question = models.Question.objects.first()
+        response = self.client.get(reverse("faq:question_detail", args=(question.category.slug, question.slug,)))
+
+        self.assertEqual(response.context['can_vote_question'], False)
+        self.assertEqual(response.context['can_vote_answer'], False)
+
+
+class VoteQuestionTestCase(TestCase):
+    def setUp(self):
+        category = models.Category.objects.create(name="cat1", _description="descript")
+
+        models.Question.objects.create(category=category, question="great question")
+
+    @override_settings(FAQ_SETTINGS=[])
+    def test_anonymous_user_cant_vote(self):
+        """redirects logged out users to login page"""
+
+        question = models.Question.objects.first()
+        response = self.client.post(reverse("faq:vote_question", args=(question.category.slug, question.slug,)))
+
+        self.assertEqual(response.status_code, 302)
+
+
+class VoteanswerTestCase(TestCase):
+    def setUp(self):
+        category = models.Category.objects.create(name="cat1", _description="descript")
+
+        question = models.Question.objects.create(category=category, question="great question")
+
+        self.answer = models.Answer.objects.create(question=question, answer="because")
+
+    @override_settings(FAQ_SETTINGS=[])
+    def test_anonymous_user_cant_vote(self):
+        """redirects logged out users to login page"""
+
+        question = models.Question.objects.first()
+        response = self.client.post(
+                reverse("faq:vote_answer", args=(question.category.slug, question.slug, self.answer.slug)))
+
+        self.assertEqual(response.status_code, 302)
```

### Comparing `django-easy-faq-1.7/faq/views.py` & `django_easy_faq-1.8/faq/views.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,326 +1,327 @@
-from django.core.exceptions import PermissionDenied
-from django.shortcuts import reverse
-from django.views import generic
-from django.contrib.auth.mixins import UserPassesTestMixin
-from django.conf import settings
-from . import models
-from . import forms
-from .snippets import get_template_settings
-
-
-# Create your views here.
-class IndexView(generic.ListView):
-    """
-    this view depending on settings either displays all the categories as a list if the categories is enabled using the categories_list.html template
-
-    if categories are not enabled it will then show a list of all the questions using questions_list.html template
-    """
-
-    def get_template_names(self):
-        """if "no_category" render questions_list.html
-            else render categories_list.html"""
-        if "no_category" in settings.FAQ_SETTINGS:
-            return "faq/questions_list.html"
-        return "faq/categories_list.html"
-
-    def get_queryset(self):
-        if "no_category" in settings.FAQ_SETTINGS:
-            return models.Question.objects.all()
-        return models.Category.objects.all()
-
-    def get_context_object_name(self, object_list):
-        if "no_category" in settings.FAQ_SETTINGS:
-            return "questions"
-        return "categories"
-
-    def get_context_data(self, **kwargs):
-        context = super().get_context_data(**kwargs)
-        context.update(get_template_settings(self.request))  # add in all settings into templates
-        return context
-
-
-class CategoryDetail(generic.DetailView):
-    """
-    this view only runs when categories are enabled
-    this view shows all the questions related to this category
-    """
-    model = models.Category
-    template_name = "faq/category_detail.html"
-
-    def get_context_data(self, *, object_list=None, **kwargs):
-        context = super().get_context_data()
-        context.update(get_template_settings(self.request))  # add in all settings into templates
-        return context
-
-
-class AddQuestion(UserPassesTestMixin, generic.CreateView):
-    """
-    this view is for a user to add a question to the faq questions
-    if the using categories then this will also add the current category to it
-    the default setting is only to allow the superuser to add new questions
-    to change this:
-        A) override the testfunc method
-        B) set staff_can_add_question in the FAQ_SETTINGS to True (allows any staff user to add a question)
-        C) set authenticated_user_can_add_question in the FAQ_SETTINGS to True (allows any authenticated user to add a question)
-    """
-    model = models.Question
-    fields = ['question']
-
-    def test_func(self):
-        # when authenticated_user_can_add_question in the FAQ_SETTINGS is set to True
-        if "logged_in_users_can_add_question" in settings.FAQ_SETTINGS:
-            if self.request.user.is_authenticated:
-                return True
-        return False
-
-    def get_success_url(self):
-        return self.question_url
-
-    def form_valid(self, form):
-        # if using categories
-        if "no_category" not in settings.FAQ_SETTINGS:
-            form = form.save(commit=False)
-            form.category = models.Category.objects.get(slug=self.kwargs["slug"])
-            form.save()
-            self.question_url = form.get_absolute_url()
-            return super().form_valid(form)
-        else:
-            form = form.save()
-            self.question_url = form.get_absolute_url()
-            return super().form_valid(form)
-
-    def get_context_data(self, **kwargs):
-        context = super().get_context_data(**kwargs)
-
-        if "no_category" not in settings.FAQ_SETTINGS:
-            context['category'] = models.Category.objects.get(slug=self.kwargs["slug"])
-        return context
-
-
-class QuestionDetail(generic.DetailView):
-    model = models.Question
-    template_name = "faq/question_detail.html"
-    context_object_name = "question"
-
-    def get_object(self, queryset=None):
-        # if using categories
-        if "no_category" not in settings.FAQ_SETTINGS:
-            return self.model.objects.get(category__slug=self.kwargs["slug"], slug=self.kwargs["question"])
-        else:
-            return self.model.objects.get(slug=self.kwargs["slug"])
-
-    def get_context_data(self, **kwargs):
-        context = super().get_context_data()
-        context.update(get_template_settings(self.request))  # add in all settings into templates
-
-        # check if logged in users are allowed to answer questions
-        if "logged_in_users_can_answer_question" in settings.FAQ_SETTINGS:
-            # check if user is logged in
-            if self.request.user.is_authenticated:
-                if "allow_multiple_answers" in settings.FAQ_SETTINGS:
-                    context['can_answer_question'] = True
-                else:
-                    # if there is already one answer
-                    if self.get_object().answer_set.count() > 0:
-                        context['can_answer_question'] = False
-                    else:
-                        context['can_answer_question'] = True
-            else:
-                context['can_answer_question'] = False
-        else:
-            context['can_answer_question'] = False
-
-        context["comment_form"] = forms.CommentForm()
-        return context
-
-
-class AddAnswer(UserPassesTestMixin, generic.CreateView):
-    model = models.Answer
-    fields = ["answer"]
-    template_name = "faq/answer_form.html"
-
-    def test_func(self):
-        # when authenticated_user_can_add_question in the FAQ_SETTINGS is set to True
-        if "logged_in_users_can_answer_question" in settings.FAQ_SETTINGS:
-            if self.request.user.is_authenticated:
-                if "allow_multiple_answers" in settings.FAQ_SETTINGS:
-                    return True
-                else:
-
-                    # if using categories
-                    if "no_category" not in settings.FAQ_SETTINGS:
-                        question = models.Question.objects.get(category__slug=self.kwargs['category'],
-                                                               slug=self.kwargs['question'])
-                    else:
-                        question = models.Question.objects.get(slug=self.kwargs['question'])
-
-                    # if there is already one answer don't allow user to add answer
-                    if question.answer_set.count() > 0:
-                        return False
-                    else:
-                        return True
-        return False
-
-    def get_success_url(self):
-        # if using categories
-        if "no_category" not in settings.FAQ_SETTINGS:
-            return reverse("faq:question_detail", args=(self.kwargs['category'], self.kwargs['question']))
-        else:
-            return reverse("faq:question_detail", args=(self.kwargs['question'],))
-
-    def get_context_data(self, **kwargs):
-        context = super().get_context_data()
-        context.update(get_template_settings(self.request))  # add in all settings into templates
-
-        # if using categories
-        if "no_category" not in settings.FAQ_SETTINGS:
-            question = models.Question.objects.get(category__slug=self.kwargs['category'], slug=self.kwargs['question'])
-        else:
-            question = models.Question.objects.get(slug=self.kwargs['question'])
-
-        context["question"] = question
-        return context
-
-    def form_valid(self, form):
-        form = form.save(commit=False)
-
-        # if using categories
-        if "no_category" not in settings.FAQ_SETTINGS:
-            question = models.Question.objects.get(category__slug=self.kwargs['category'], slug=self.kwargs['question'])
-        else:
-            question = models.Question.objects.get(slug=self.kwargs['question'])
-
-        form.question = question
-        form.save()
-        return super().form_valid(form)
-
-
-class AddComment(generic.CreateView):
-    model = models.FAQComment
-    form_class = forms.CommentForm
-    template_name = "faq/comment_form.html"
-
-    def get_question(self):
-        # if using categories
-        if "no_category" not in settings.FAQ_SETTINGS:
-            question = models.Question.objects.get(category__slug=self.kwargs['category'], slug=self.kwargs['question'])
-        else:
-            question = models.Question.objects.get(slug=self.kwargs['question'])
-
-        return question
-
-    def get_success_url(self):
-        return self.get_question().get_absolute_url()
-
-    def get_context_data(self, **kwargs):
-        context = super().get_context_data()
-        context.update(get_template_settings(self.request))  # add in all settings into templates
-        context["question"] = self.get_question()
-        return context
-
-    def form_valid(self, form):
-        form = form.save(commit=False)
-        form.question = self.get_question()
-        if self.request.user.is_authenticated:
-            form.user = self.request.user
-        form.save()
-        return super().form_valid(form)
-
-    def get(self, *args, **kwargs):
-        if "view_only_comments" in settings.FAQ_SETTINGS:
-            raise PermissionDenied("comments are view only at this time")
-        if self.request.user.is_authenticated:
-            pass
-        else:
-            if not "anonymous_user_can_comment" in settings.FAQ_SETTINGS:
-                raise PermissionDenied("have to be logged in to comment")
-        return super().get(*args, **kwargs)
-
-    def post(self, *args, **kwargs):
-        if "view_only_comments" in settings.FAQ_SETTINGS:
-            raise PermissionDenied("comments are view only at this time")
-        if self.request.user.is_authenticated:
-            pass
-        else:
-            if not "anonymous_user_can_comment" in settings.FAQ_SETTINGS:
-                raise PermissionDenied("have to be logged in to comment")
-        return super().post(*args, **kwargs)
-
-
-class VoteAnswerHelpful(UserPassesTestMixin, generic.FormView):
-    form_class = forms.VoteForm
-    template_name = "faq/vote_form.html"
-
-    def get_success_url(self):
-        return self.get_question().get_absolute_url()
-
-    def get_question(self):
-        # if using categories
-        if "no_category" not in settings.FAQ_SETTINGS:
-            question = models.Question.objects.get(category__slug=self.kwargs['category'], slug=self.kwargs['question'])
-        else:
-            question = models.Question.objects.get(slug=self.kwargs['question'])
-
-        return question
-
-    def get_answer(self):
-        return models.Answer.objects.get(question=self.get_question(), slug=self.kwargs['answer'])
-
-    def form_valid(self, form):
-        # if already voted get vote otherwise create it
-        if models.AnswerHelpful.objects.filter(answer=self.get_answer(), user=self.request.user).exists():
-            helpful = models.AnswerHelpful.objects.get(answer=self.get_answer(), user=self.request.user)
-        else:
-            helpful = models.AnswerHelpful(answer=self.get_answer(), user=self.request.user)
-
-        helpful.vote = form.cleaned_data['vote']
-        helpful.save()
-        self.get_answer().save()
-        return super().form_valid(form)
-
-    def test_func(self):
-        if "no_answer_votes" in settings.FAQ_SETTINGS:
-            return False
-        elif "no_votes" in settings.FAQ_SETTINGS:
-            return False
-        if not self.request.user.is_authenticated:
-            return False
-        return True
-
-
-class VoteQuestionHelpful(UserPassesTestMixin, generic.FormView):
-    form_class = forms.VoteForm
-    template_name = "faq/vote_form.html"
-
-    def get_success_url(self):
-        return self.get_question().get_absolute_url()
-
-    def get_question(self):
-        # if using categories
-        if "no_category" not in settings.FAQ_SETTINGS:
-            question = models.Question.objects.get(category__slug=self.kwargs['category'], slug=self.kwargs['question'])
-        else:
-            question = models.Question.objects.get(slug=self.kwargs['question'])
-
-        return question
-
-    def form_valid(self, form):
-        # if already voted get vote otherwise create it
-        if models.QuestionHelpful.objects.filter(question=self.get_question(), user=self.request.user).exists():
-            helpful = models.QuestionHelpful.objects.get(question=self.get_question(), user=self.request.user)
-        else:
-            helpful = models.QuestionHelpful(question=self.get_question(), user=self.request.user)
-
-        helpful.vote = form.cleaned_data['vote']
-        helpful.save()
-        self.get_question().save()
-        return super().form_valid(form)
-
-    def test_func(self):
-        if "no_question_votes" in settings.FAQ_SETTINGS:
-            return False
-        elif "no_votes" in settings.FAQ_SETTINGS:
-            return False
-        if not self.request.user.is_authenticated:
-            return False
-        return True
+from django.core.exceptions import PermissionDenied
+from django.shortcuts import reverse
+from django.views import generic
+from django.contrib.auth.mixins import UserPassesTestMixin
+from django.conf import settings
+from . import models
+from . import forms
+from .snippets import get_template_settings
+
+
+# Create your views here.
+class IndexView(generic.ListView):
+    """
+    this view depending on settings either displays all the categories as a list if the categories is enabled using the categories_list.html template
+
+    if categories are not enabled it will then show a list of all the questions using questions_list.html template
+    """
+
+    def get_template_names(self):
+        """if "no_category" render questions_list.html
+            else render categories_list.html"""
+        if "no_category" in settings.FAQ_SETTINGS:
+            return "faq/questions_list.html"
+        return "faq/categories_list.html"
+
+    def get_queryset(self):
+        if "no_category" in settings.FAQ_SETTINGS:
+            return models.Question.objects.all()
+        return models.Category.objects.all()
+
+    def get_context_object_name(self, object_list):
+        if "no_category" in settings.FAQ_SETTINGS:
+            return "questions"
+        return "categories"
+
+    def get_context_data(self, **kwargs):
+        context = super().get_context_data(**kwargs)
+        context.update(get_template_settings(self.request))  # add in all settings into templates
+        return context
+
+
+class CategoryDetail(generic.DetailView):
+    """
+    this view only runs when categories are enabled
+    this view shows all the questions related to this category
+    """
+    model = models.Category
+    template_name = "faq/category_detail.html"
+
+    def get_context_data(self, *, object_list=None, **kwargs):
+        context = super().get_context_data()
+        context.update(get_template_settings(self.request))  # add in all settings into templates
+        return context
+
+
+class AddQuestion(UserPassesTestMixin, generic.CreateView):
+    """
+    this view is for a user to add a question to the faq questions
+    if the using categories then this will also add the current category to it
+    the default setting is only to allow the superuser to add new questions
+    to change this:
+        A) override the testfunc method
+        B) set staff_can_add_question in the FAQ_SETTINGS to True (allows any staff user to add a question)
+        C) set authenticated_user_can_add_question in the FAQ_SETTINGS to True (allows any authenticated user to add a question)
+    """
+    model = models.Question
+    fields = ['question']
+
+    def test_func(self):
+        # when authenticated_user_can_add_question in the FAQ_SETTINGS is set to True
+        if "logged_in_users_can_add_question" in settings.FAQ_SETTINGS:
+            if self.request.user.is_authenticated:
+                return True
+        return False
+
+    def get_success_url(self):
+        return self.question_url
+
+    def form_valid(self, form):
+        # if using categories
+        if "no_category" not in settings.FAQ_SETTINGS:
+            form = form.save(commit=False)
+            form.category = models.Category.objects.get(slug=self.kwargs["slug"])
+            form.save()
+            self.question_url = form.get_absolute_url()
+            return super().form_valid(form)
+        else:
+            form = form.save()
+            self.question_url = form.get_absolute_url()
+            return super().form_valid(form)
+
+    def get_context_data(self, **kwargs):
+        context = super().get_context_data(**kwargs)
+
+        if "no_category" not in settings.FAQ_SETTINGS:
+            context['category'] = models.Category.objects.get(slug=self.kwargs["slug"])
+        return context
+
+
+class QuestionDetail(generic.DetailView):
+    model = models.Question
+    template_name = "faq/question_detail.html"
+    context_object_name = "question"
+
+    def get_object(self, queryset=None):
+        # if using categories
+        if "no_category" not in settings.FAQ_SETTINGS:
+            return self.model.objects.get(category__slug=self.kwargs["slug"], slug=self.kwargs["question"])
+        else:
+            return self.model.objects.get(slug=self.kwargs["slug"])
+
+    def get_context_data(self, **kwargs):
+        context = super().get_context_data()
+        context.update(get_template_settings(self.request))  # add in all settings into templates
+
+        # check if logged in users are allowed to answer questions
+        if "logged_in_users_can_answer_question" in settings.FAQ_SETTINGS:
+            # check if user is logged in
+            if self.request.user.is_authenticated:
+                if "allow_multiple_answers" in settings.FAQ_SETTINGS:
+                    context['can_answer_question'] = True
+                else:
+                    # if there is already one answer
+                    if self.get_object().answer_set.count() > 0:
+                        context['can_answer_question'] = False
+                    else:
+                        context['can_answer_question'] = True
+            else:
+                context['can_answer_question'] = False
+        else:
+            context['can_answer_question'] = False
+
+        context["comment_form"] = forms.CommentForm()
+        return context
+
+
+class AddAnswer(UserPassesTestMixin, generic.CreateView):
+    template_name = "faq/answer_form.html"
+    form_class = forms.AnswerForm
+
+    def test_func(self):
+        # when authenticated_user_can_add_question in the FAQ_SETTINGS is set to True
+        if "logged_in_users_can_answer_question" in settings.FAQ_SETTINGS:
+            if self.request.user.is_authenticated:
+                if "allow_multiple_answers" in settings.FAQ_SETTINGS:
+                    return True
+                else:
+
+                    # if using categories
+                    if "no_category" not in settings.FAQ_SETTINGS:
+                        question = models.Question.objects.get(category__slug=self.kwargs['category'],
+                                                               slug=self.kwargs['question'])
+                    else:
+                        question = models.Question.objects.get(slug=self.kwargs['question'])
+
+                    # if there is already one answer don't allow user to add answer
+                    if question.answer_set.count() > 0:
+                        return False
+                    else:
+                        return True
+        return False
+
+    def get_success_url(self):
+        # if using categories
+        if "no_category" not in settings.FAQ_SETTINGS:
+            return reverse("faq:question_detail", args=(self.kwargs['category'], self.kwargs['question']))
+        else:
+            return reverse("faq:question_detail", args=(self.kwargs['question'],))
+
+    def get_context_data(self, **kwargs):
+        context = super().get_context_data()
+        context.update(get_template_settings(self.request))  # add in all settings into templates
+
+        # if using categories
+        if "no_category" not in settings.FAQ_SETTINGS:
+            question = models.Question.objects.get(category__slug=self.kwargs['category'], slug=self.kwargs['question'])
+        else:
+            question = models.Question.objects.get(slug=self.kwargs['question'])
+
+        context["question"] = question
+        return context
+
+    def form_valid(self, form):
+        form = form.save(commit=False)
+
+        # if using categories
+        if "no_category" not in settings.FAQ_SETTINGS:
+            question = models.Question.objects.get(category__slug=self.kwargs['category'], slug=self.kwargs['question'])
+        else:
+            question = models.Question.objects.get(slug=self.kwargs['question'])
+
+        form.question = question
+        if "rich_text_answers" in settings.FAQ_SETTINGS:
+            form.is_rich_text = True
+        form.save()
+        return super().form_valid(form)
+
+
+class AddComment(generic.CreateView):
+    model = models.FAQComment
+    form_class = forms.CommentForm
+    template_name = "faq/comment_form.html"
+
+    def get_question(self):
+        # if using categories
+        if "no_category" not in settings.FAQ_SETTINGS:
+            question = models.Question.objects.get(category__slug=self.kwargs['category'], slug=self.kwargs['question'])
+        else:
+            question = models.Question.objects.get(slug=self.kwargs['question'])
+
+        return question
+
+    def get_success_url(self):
+        return self.get_question().get_absolute_url()
+
+    def get_context_data(self, **kwargs):
+        context = super().get_context_data()
+        context.update(get_template_settings(self.request))  # add in all settings into templates
+        context["question"] = self.get_question()
+        return context
+
+    def form_valid(self, form):
+        form = form.save(commit=False)
+        form.question = self.get_question()
+        if self.request.user.is_authenticated:
+            form.user = self.request.user
+        form.save()
+        return super().form_valid(form)
+
+    def get(self, *args, **kwargs):
+        if "view_only_comments" in settings.FAQ_SETTINGS:
+            raise PermissionDenied("comments are view only at this time")
+        if self.request.user.is_authenticated:
+            pass
+        else:
+            if not "anonymous_user_can_comment" in settings.FAQ_SETTINGS:
+                raise PermissionDenied("have to be logged in to comment")
+        return super().get(*args, **kwargs)
+
+    def post(self, *args, **kwargs):
+        if "view_only_comments" in settings.FAQ_SETTINGS:
+            raise PermissionDenied("comments are view only at this time")
+        if self.request.user.is_authenticated:
+            pass
+        else:
+            if not "anonymous_user_can_comment" in settings.FAQ_SETTINGS:
+                raise PermissionDenied("have to be logged in to comment")
+        return super().post(*args, **kwargs)
+
+
+class VoteAnswerHelpful(UserPassesTestMixin, generic.FormView):
+    form_class = forms.VoteForm
+    template_name = "faq/vote_form.html"
+
+    def get_success_url(self):
+        return self.get_question().get_absolute_url()
+
+    def get_question(self):
+        # if using categories
+        if "no_category" not in settings.FAQ_SETTINGS:
+            question = models.Question.objects.get(category__slug=self.kwargs['category'], slug=self.kwargs['question'])
+        else:
+            question = models.Question.objects.get(slug=self.kwargs['question'])
+
+        return question
+
+    def get_answer(self):
+        return models.Answer.objects.get(question=self.get_question(), slug=self.kwargs['answer'])
+
+    def form_valid(self, form):
+        # if already voted get vote otherwise create it
+        if models.AnswerHelpful.objects.filter(answer=self.get_answer(), user=self.request.user).exists():
+            helpful = models.AnswerHelpful.objects.get(answer=self.get_answer(), user=self.request.user)
+        else:
+            helpful = models.AnswerHelpful(answer=self.get_answer(), user=self.request.user)
+
+        helpful.vote = form.cleaned_data['vote']
+        helpful.save()
+        self.get_answer().save()
+        return super().form_valid(form)
+
+    def test_func(self):
+        if "no_answer_votes" in settings.FAQ_SETTINGS:
+            return False
+        elif "no_votes" in settings.FAQ_SETTINGS:
+            return False
+        if not self.request.user.is_authenticated:
+            return False
+        return True
+
+
+class VoteQuestionHelpful(UserPassesTestMixin, generic.FormView):
+    form_class = forms.VoteForm
+    template_name = "faq/vote_form.html"
+
+    def get_success_url(self):
+        return self.get_question().get_absolute_url()
+
+    def get_question(self):
+        # if using categories
+        if "no_category" not in settings.FAQ_SETTINGS:
+            question = models.Question.objects.get(category__slug=self.kwargs['category'], slug=self.kwargs['question'])
+        else:
+            question = models.Question.objects.get(slug=self.kwargs['question'])
+
+        return question
+
+    def form_valid(self, form):
+        # if already voted get vote otherwise create it
+        if models.QuestionHelpful.objects.filter(question=self.get_question(), user=self.request.user).exists():
+            helpful = models.QuestionHelpful.objects.get(question=self.get_question(), user=self.request.user)
+        else:
+            helpful = models.QuestionHelpful(question=self.get_question(), user=self.request.user)
+
+        helpful.vote = form.cleaned_data['vote']
+        helpful.save()
+        self.get_question().save()
+        return super().form_valid(form)
+
+    def test_func(self):
+        if "no_question_votes" in settings.FAQ_SETTINGS:
+            return False
+        elif "no_votes" in settings.FAQ_SETTINGS:
+            return False
+        if not self.request.user.is_authenticated:
+            return False
+        return True
```

