# Comparing `tmp/jusText-3.0.0.tar.gz` & `tmp/justext-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jusText-3.0.0.tar", last modified: Thu Oct 21 16:57:43 2021, max compression
+gzip compressed data, was "justext-3.0.1.tar", last modified: Thu May  9 15:49:49 2024, max compression
```

## Comparing `jusText-3.0.0.tar` & `justext-3.0.1.tar`

### file list

```diff
@@ -1,122 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-21 16:57:43.701112 jusText-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1903 2021-10-21 16:57:27.000000 jusText-3.0.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1339 2021-10-21 16:57:27.000000 jusText-3.0.0/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (121)       93 2021-10-21 16:57:27.000000 jusText-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6663 2021-10-21 16:57:43.701112 jusText-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3394 2021-10-21 16:57:27.000000 jusText-3.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-21 16:57:43.689112 jusText-3.0.0/jusText.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6663 2021-10-21 16:57:43.000000 jusText-3.0.0/jusText.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3439 2021-10-21 16:57:43.000000 jusText-3.0.0/jusText.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-21 16:57:43.000000 jusText-3.0.0/jusText.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       69 2021-10-21 16:57:43.000000 jusText-3.0.0/jusText.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-10-21 16:57:43.000000 jusText-3.0.0/jusText.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-21 16:57:43.689112 jusText-3.0.0/justext/
--rw-r--r--   0 runner    (1001) docker     (121)      269 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12600 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      802 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/_compat.py
--rw-r--r--   0 runner    (1001) docker     (121)    13177 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     1667 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/paragraph.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-21 16:57:43.701112 jusText-3.0.0/justext/stoplists/
--rw-r--r--   0 runner    (1001) docker     (121)     1205 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Afrikaans.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3424 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Albanian.txt
--rw-r--r--   0 runner    (1001) docker     (121)    30217 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Arabic.txt
--rw-r--r--   0 runner    (1001) docker     (121)      918 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Aragonese.txt
--rw-r--r--   0 runner    (1001) docker     (121)    45410 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Armenian.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3544 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Aromanian.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4379 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Asturian.txt
--rw-r--r--   0 runner    (1001) docker     (121)    33201 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Azerbaijani.txt
--rw-r--r--   0 runner    (1001) docker     (121)    17791 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Basque.txt
--rw-r--r--   0 runner    (1001) docker     (121)    65883 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Belarusian.txt
--rw-r--r--   0 runner    (1001) docker     (121)    62122 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Belarusian_Taraskievica.txt
--rw-r--r--   0 runner    (1001) docker     (121)    18721 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Bengali.txt
--rw-r--r--   0 runner    (1001) docker     (121)      950 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Bishnupriya_Manipuri.txt
--rw-r--r--   0 runner    (1001) docker     (121)    16143 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Bosnian.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1649 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Breton.txt
--rw-r--r--   0 runner    (1001) docker     (121)    15206 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Bulgarian.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1344 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Catalan.txt
--rw-r--r--   0 runner    (1001) docker     (121)       57 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Cebuano.txt
--rw-r--r--   0 runner    (1001) docker     (121)    35124 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Chuvash.txt
--rw-r--r--   0 runner    (1001) docker     (121)    17928 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Croatian.txt
--rw-r--r--   0 runner    (1001) docker     (121)    25564 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Czech.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3504 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Danish.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1756 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Dutch.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3123 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/English.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3657 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Esperanto.txt
--rw-r--r--   0 runner    (1001) docker     (121)    50849 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Estonian.txt
--rw-r--r--   0 runner    (1001) docker     (121)    66511 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Finnish.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2656 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/French.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2857 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Galician.txt
--rw-r--r--   0 runner    (1001) docker     (121)   128465 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Georgian.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4653 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/German.txt
--rw-r--r--   0 runner    (1001) docker     (121)     7796 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Greek.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6073 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Gujarati.txt
--rw-r--r--   0 runner    (1001) docker     (121)      175 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Haitian.txt
--rw-r--r--   0 runner    (1001) docker     (121)    45229 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Hebrew.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4944 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Hindi.txt
--rw-r--r--   0 runner    (1001) docker     (121)    29227 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Hungarian.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4813 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Icelandic.txt
--rw-r--r--   0 runner    (1001) docker     (121)      249 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Ido.txt
--rw-r--r--   0 runner    (1001) docker     (121)      733 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Igbo.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6758 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Indonesian.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1191 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Irish.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3715 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Italian.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4533 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Javanese.txt
--rw-r--r--   0 runner    (1001) docker     (121)   161220 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Kannada.txt
--rw-r--r--   0 runner    (1001) docker     (121)    52789 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Kazakh.txt
--rw-r--r--   0 runner    (1001) docker     (121)   131487 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Korean.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3530 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Kurdish.txt
--rw-r--r--   0 runner    (1001) docker     (121)    54729 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Kyrgyz.txt
--rw-r--r--   0 runner    (1001) docker     (121)    14282 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Latin.txt
--rw-r--r--   0 runner    (1001) docker     (121)    30561 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Latvian.txt
--rw-r--r--   0 runner    (1001) docker     (121)    43497 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Lithuanian.txt
--rw-r--r--   0 runner    (1001) docker     (121)      738 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Lombard.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1051 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Low_Saxon.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2374 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Luxembourgish.txt
--rw-r--r--   0 runner    (1001) docker     (121)    11982 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Macedonian.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6368 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Malay.txt
--rw-r--r--   0 runner    (1001) docker     (121)   309082 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Malayalam.txt
--rw-r--r--   0 runner    (1001) docker     (121)    11115 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Maltese.txt
--rw-r--r--   0 runner    (1001) docker     (121)    39588 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Marathi.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1749 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Neapolitan.txt
--rw-r--r--   0 runner    (1001) docker     (121)    26543 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Nepali.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1465 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Newar.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2850 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Norwegian_Bokmal.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2002 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Norwegian_Nynorsk.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3109 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Occitan.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4642 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Persian.txt
--rw-r--r--   0 runner    (1001) docker     (121)      419 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Piedmontese.txt
--rw-r--r--   0 runner    (1001) docker     (121)    29632 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Polish.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3261 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Portuguese.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2237 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Quechua.txt
--rw-r--r--   0 runner    (1001) docker     (121)     7067 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Romanian.txt
--rw-r--r--   0 runner    (1001) docker     (121)    77600 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Russian.txt
--rw-r--r--   0 runner    (1001) docker     (121)    14867 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Samogitian.txt
--rw-r--r--   0 runner    (1001) docker     (121)    21052 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Serbian.txt
--rw-r--r--   0 runner    (1001) docker     (121)    17311 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Serbo_Croatian.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3167 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Sicilian.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1567 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Simple_English.txt
--rw-r--r--   0 runner    (1001) docker     (121)    28930 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Slovak.txt
--rw-r--r--   0 runner    (1001) docker     (121)    17179 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Slovenian.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1851 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Spanish.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5971 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Sundanese.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2406 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Swahili.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4870 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Swedish.txt
--rw-r--r--   0 runner    (1001) docker     (121)      980 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Tagalog.txt
--rw-r--r--   0 runner    (1001) docker     (121)   154484 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Tamil.txt
--rw-r--r--   0 runner    (1001) docker     (121)    95849 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Telugu.txt
--rw-r--r--   0 runner    (1001) docker     (121)    25673 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Turkish.txt
--rw-r--r--   0 runner    (1001) docker     (121)    27602 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Turkmen.txt
--rw-r--r--   0 runner    (1001) docker     (121)    75370 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Ukrainian.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1900 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Urdu.txt
--rw-r--r--   0 runner    (1001) docker     (121)    51738 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Uzbek.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1769 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Vietnamese.txt
--rw-r--r--   0 runner    (1001) docker     (121)      533 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Volapuk.txt
--rw-r--r--   0 runner    (1001) docker     (121)      910 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Walloon.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Waray_Waray.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3338 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Welsh.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1353 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/West_Frisian.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2230 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Western_Panjabi.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1748 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/stoplists/Yoruba.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1965 2021-10-21 16:57:27.000000 jusText-3.0.0/justext/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      314 2021-10-21 16:57:43.705112 jusText-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2102 2021-10-21 16:57:27.000000 jusText-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:49:49.640720 justext-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-09 15:49:40.000000 justext-3.0.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-09 15:49:40.000000 justext-3.0.1/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-09 15:49:40.000000 justext-3.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-05-09 15:49:49.640720 justext-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-05-09 15:49:40.000000 justext-3.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:49:49.640720 justext-3.0.1/jusText.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-05-09 15:49:49.000000 justext-3.0.1/jusText.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-05-09 15:49:49.000000 justext-3.0.1/jusText.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 15:49:49.000000 justext-3.0.1/jusText.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-09 15:49:49.000000 justext-3.0.1/jusText.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-09 15:49:49.000000 justext-3.0.1/jusText.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:49:49.616720 justext-3.0.1/justext/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-09 15:49:40.000000 justext-3.0.1/justext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12600 2024-05-09 15:49:40.000000 justext-3.0.1/justext/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-09 15:49:40.000000 justext-3.0.1/justext/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13177 2024-05-09 15:49:40.000000 justext-3.0.1/justext/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-09 15:49:40.000000 justext-3.0.1/justext/paragraph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:49:49.636720 justext-3.0.1/justext/stoplists/
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Afrikaans.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Albanian.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    30217 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Arabic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Aragonese.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    45410 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Armenian.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Aromanian.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Asturian.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    33201 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Azerbaijani.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17791 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Basque.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    65883 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Belarusian.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    62122 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Belarusian_Taraskievica.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18721 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Bengali.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Bishnupriya_Manipuri.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16143 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Bosnian.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Breton.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15206 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Bulgarian.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Catalan.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Cebuano.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35124 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Chuvash.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17928 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Croatian.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    25564 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Czech.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Danish.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Dutch.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/English.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Esperanto.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    50849 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Estonian.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    66511 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Finnish.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/French.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Galician.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   128465 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Georgian.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/German.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7796 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Greek.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6073 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Gujarati.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Haitian.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    45229 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Hebrew.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Hindi.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    29227 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Hungarian.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Icelandic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Ido.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Igbo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Indonesian.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Irish.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Italian.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Javanese.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   161220 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Kannada.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    52789 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Kazakh.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   131487 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Korean.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Kurdish.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    54729 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Kyrgyz.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14282 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Latin.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    30561 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Latvian.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    43497 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Lithuanian.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Lombard.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Low_Saxon.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Luxembourgish.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11982 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Macedonian.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Malay.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   309082 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Malayalam.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11115 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Maltese.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    39588 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Marathi.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Neapolitan.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    26543 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Nepali.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Newar.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Norwegian_Bokmal.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Norwegian_Nynorsk.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Occitan.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Persian.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Piedmontese.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    29632 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Polish.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Portuguese.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Quechua.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7067 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Romanian.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    77600 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Russian.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14867 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Samogitian.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    21052 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Serbian.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17311 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Serbo_Croatian.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Sicilian.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Simple_English.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    28930 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Slovak.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17179 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Slovenian.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Spanish.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Sundanese.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Swahili.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Swedish.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Tagalog.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   154484 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Tamil.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    95849 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Telugu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    25673 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Turkish.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    27602 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Turkmen.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    75370 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Ukrainian.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Urdu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    51738 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Uzbek.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Vietnamese.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Volapuk.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Walloon.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Waray_Waray.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Welsh.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/West_Frisian.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Western_Panjabi.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-09 15:49:40.000000 justext-3.0.1/justext/stoplists/Yoruba.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-09 15:49:40.000000 justext-3.0.1/justext/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-09 15:49:49.640720 justext-3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-09 15:49:40.000000 justext-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:49:49.640720 justext-3.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-09 15:49:40.000000 justext-3.0.1/tests/test_classify_paragraphs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-09 15:49:40.000000 justext-3.0.1/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-09 15:49:40.000000 justext-3.0.1/tests/test_dom_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-05-09 15:49:40.000000 justext-3.0.1/tests/test_html_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-05-09 15:49:40.000000 justext-3.0.1/tests/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-05-09 15:49:40.000000 justext-3.0.1/tests/test_sax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-05-09 15:49:40.000000 justext-3.0.1/tests/test_utils.py
```

### Comparing `jusText-3.0.0/CHANGELOG.rst` & `justext-3.0.1/CHANGELOG.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 .. :changelog:
 
 Changelog for jusText
 =====================
 
+3.0.1 (2024-05-09)
+------------------
+- *BUG FIX:* Fix issue with new version of lxml `#48 <https://github.com/miso-belica/jusText/pull/48>`_.
+
 3.0.0 (2021-10-21)
 ------------------
 - *INCOMPATIBLE CHANGE:* Dropped support for Python 3.4 and below.
 - *BUG FIX:* Don't join words separated only by ``<br>`` tag.
 - *BUG FIX:* List available stop-lists alphabetically.
 
 2.2.0 (2016-03-06)
```

### Comparing `jusText-3.0.0/LICENSE.rst` & `justext-3.0.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/PKG-INFO` & `justext-3.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: jusText
-Version: 3.0.0
+Version: 3.0.1
 Summary: Heuristic based boilerplate removal tool
 Home-page: https://github.com/miso-belica/jusText
 Author: Jan Pomikálek
 Author-email: jan.pomikalek@gmail.com
 Maintainer: Michal Belica
 Maintainer-email: miso.belica@gmail.com
 License: The BSD 2-Clause License
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
@@ -26,14 +25,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Pre-processors
 Classifier: Topic :: Text Processing :: Filters
 Classifier: Topic :: Text Processing :: Markup :: HTML
 License-File: LICENSE.rst
+Requires-Dist: lxml[html_clean]>=4.4.2
+Requires-Dist: backports.functools-lru-cache; python_version < "3.2"
 
 .. _jusText: http://code.google.com/p/justext/
 .. _Python: http://www.python.org/
 .. _lxml: http://lxml.de/
 
 jusText
 =======
@@ -143,14 +144,18 @@
 
 
 .. :changelog:
 
 Changelog for jusText
 =====================
 
+3.0.1 (2024-05-09)
+------------------
+- *BUG FIX:* Fix issue with new version of lxml `#48 <https://github.com/miso-belica/jusText/pull/48>`_.
+
 3.0.0 (2021-10-21)
 ------------------
 - *INCOMPATIBLE CHANGE:* Dropped support for Python 3.4 and below.
 - *BUG FIX:* Don't join words separated only by ``<br>`` tag.
 - *BUG FIX:* List available stop-lists alphabetically.
 
 2.2.0 (2016-03-06)
@@ -187,9 +192,7 @@
 - *BUG FIX:* More robust parsing of meta tags containing the information about
   used charset.
 - *BUG FIX:* Corrected decoding of HTML entities &#128; to &#159;
 
 1.1.0 (2011-03-09)
 ------------------
 - First public release.
-
-
```

### Comparing `jusText-3.0.0/README.rst` & `justext-3.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/jusText.egg-info/PKG-INFO` & `justext-3.0.1/jusText.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: jusText
-Version: 3.0.0
+Version: 3.0.1
 Summary: Heuristic based boilerplate removal tool
 Home-page: https://github.com/miso-belica/jusText
 Author: Jan Pomikálek
 Author-email: jan.pomikalek@gmail.com
 Maintainer: Michal Belica
 Maintainer-email: miso.belica@gmail.com
 License: The BSD 2-Clause License
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
@@ -26,14 +25,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Pre-processors
 Classifier: Topic :: Text Processing :: Filters
 Classifier: Topic :: Text Processing :: Markup :: HTML
 License-File: LICENSE.rst
+Requires-Dist: lxml[html_clean]>=4.4.2
+Requires-Dist: backports.functools-lru-cache; python_version < "3.2"
 
 .. _jusText: http://code.google.com/p/justext/
 .. _Python: http://www.python.org/
 .. _lxml: http://lxml.de/
 
 jusText
 =======
@@ -143,14 +144,18 @@
 
 
 .. :changelog:
 
 Changelog for jusText
 =====================
 
+3.0.1 (2024-05-09)
+------------------
+- *BUG FIX:* Fix issue with new version of lxml `#48 <https://github.com/miso-belica/jusText/pull/48>`_.
+
 3.0.0 (2021-10-21)
 ------------------
 - *INCOMPATIBLE CHANGE:* Dropped support for Python 3.4 and below.
 - *BUG FIX:* Don't join words separated only by ``<br>`` tag.
 - *BUG FIX:* List available stop-lists alphabetically.
 
 2.2.0 (2016-03-06)
@@ -187,9 +192,7 @@
 - *BUG FIX:* More robust parsing of meta tags containing the information about
   used charset.
 - *BUG FIX:* Corrected decoding of HTML entities &#128; to &#159;
 
 1.1.0 (2011-03-09)
 ------------------
 - First public release.
-
-
```

### Comparing `jusText-3.0.0/jusText.egg-info/SOURCES.txt` & `justext-3.0.1/jusText.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -110,8 +110,15 @@
 justext/stoplists/Vietnamese.txt
 justext/stoplists/Volapuk.txt
 justext/stoplists/Walloon.txt
 justext/stoplists/Waray_Waray.txt
 justext/stoplists/Welsh.txt
 justext/stoplists/West_Frisian.txt
 justext/stoplists/Western_Panjabi.txt
-justext/stoplists/Yoruba.txt
+justext/stoplists/Yoruba.txt
+tests/test_classify_paragraphs.py
+tests/test_core.py
+tests/test_dom_utils.py
+tests/test_html_encoding.py
+tests/test_paths.py
+tests/test_sax.py
+tests/test_utils.py
```

### Comparing `jusText-3.0.0/justext/__main__.py` & `justext-3.0.1/justext/__main__.py`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/_compat.py` & `justext-3.0.1/justext/_compat.py`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/core.py` & `justext-3.0.1/justext/core.py`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/paragraph.py` & `justext-3.0.1/justext/paragraph.py`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Afrikaans.txt` & `justext-3.0.1/justext/stoplists/Afrikaans.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Albanian.txt` & `justext-3.0.1/justext/stoplists/Albanian.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Arabic.txt` & `justext-3.0.1/justext/stoplists/Arabic.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Aragonese.txt` & `justext-3.0.1/justext/stoplists/Aragonese.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Armenian.txt` & `justext-3.0.1/justext/stoplists/Armenian.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Aromanian.txt` & `justext-3.0.1/justext/stoplists/Aromanian.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Asturian.txt` & `justext-3.0.1/justext/stoplists/Asturian.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Azerbaijani.txt` & `justext-3.0.1/justext/stoplists/Azerbaijani.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Basque.txt` & `justext-3.0.1/justext/stoplists/Basque.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Belarusian.txt` & `justext-3.0.1/justext/stoplists/Belarusian.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Belarusian_Taraskievica.txt` & `justext-3.0.1/justext/stoplists/Belarusian_Taraskievica.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Bengali.txt` & `justext-3.0.1/justext/stoplists/Bengali.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Bishnupriya_Manipuri.txt` & `justext-3.0.1/justext/stoplists/Bishnupriya_Manipuri.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Bosnian.txt` & `justext-3.0.1/justext/stoplists/Bosnian.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Breton.txt` & `justext-3.0.1/justext/stoplists/Breton.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Bulgarian.txt` & `justext-3.0.1/justext/stoplists/Bulgarian.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Catalan.txt` & `justext-3.0.1/justext/stoplists/Catalan.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Chuvash.txt` & `justext-3.0.1/justext/stoplists/Chuvash.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Croatian.txt` & `justext-3.0.1/justext/stoplists/Croatian.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Czech.txt` & `justext-3.0.1/justext/stoplists/Czech.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Danish.txt` & `justext-3.0.1/justext/stoplists/Danish.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Dutch.txt` & `justext-3.0.1/justext/stoplists/Dutch.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/English.txt` & `justext-3.0.1/justext/stoplists/English.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Esperanto.txt` & `justext-3.0.1/justext/stoplists/Esperanto.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Estonian.txt` & `justext-3.0.1/justext/stoplists/Estonian.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Finnish.txt` & `justext-3.0.1/justext/stoplists/Finnish.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/French.txt` & `justext-3.0.1/justext/stoplists/French.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Galician.txt` & `justext-3.0.1/justext/stoplists/Galician.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Georgian.txt` & `justext-3.0.1/justext/stoplists/Georgian.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/German.txt` & `justext-3.0.1/justext/stoplists/German.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Greek.txt` & `justext-3.0.1/justext/stoplists/Greek.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Gujarati.txt` & `justext-3.0.1/justext/stoplists/Gujarati.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Hebrew.txt` & `justext-3.0.1/justext/stoplists/Hebrew.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Hindi.txt` & `justext-3.0.1/justext/stoplists/Hindi.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Hungarian.txt` & `justext-3.0.1/justext/stoplists/Hungarian.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Icelandic.txt` & `justext-3.0.1/justext/stoplists/Icelandic.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Igbo.txt` & `justext-3.0.1/justext/stoplists/Igbo.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Indonesian.txt` & `justext-3.0.1/justext/stoplists/Indonesian.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Irish.txt` & `justext-3.0.1/justext/stoplists/Irish.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Italian.txt` & `justext-3.0.1/justext/stoplists/Italian.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Javanese.txt` & `justext-3.0.1/justext/stoplists/Javanese.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Kannada.txt` & `justext-3.0.1/justext/stoplists/Kannada.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Kazakh.txt` & `justext-3.0.1/justext/stoplists/Kazakh.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Korean.txt` & `justext-3.0.1/justext/stoplists/Korean.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Kurdish.txt` & `justext-3.0.1/justext/stoplists/Kurdish.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Kyrgyz.txt` & `justext-3.0.1/justext/stoplists/Kyrgyz.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Latin.txt` & `justext-3.0.1/justext/stoplists/Latin.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Latvian.txt` & `justext-3.0.1/justext/stoplists/Latvian.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Lithuanian.txt` & `justext-3.0.1/justext/stoplists/Lithuanian.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Lombard.txt` & `justext-3.0.1/justext/stoplists/Lombard.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Low_Saxon.txt` & `justext-3.0.1/justext/stoplists/Low_Saxon.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Luxembourgish.txt` & `justext-3.0.1/justext/stoplists/Luxembourgish.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Macedonian.txt` & `justext-3.0.1/justext/stoplists/Macedonian.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Malay.txt` & `justext-3.0.1/justext/stoplists/Malay.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Malayalam.txt` & `justext-3.0.1/justext/stoplists/Malayalam.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Maltese.txt` & `justext-3.0.1/justext/stoplists/Maltese.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Marathi.txt` & `justext-3.0.1/justext/stoplists/Marathi.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Neapolitan.txt` & `justext-3.0.1/justext/stoplists/Neapolitan.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Nepali.txt` & `justext-3.0.1/justext/stoplists/Nepali.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Newar.txt` & `justext-3.0.1/justext/stoplists/Newar.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Norwegian_Bokmal.txt` & `justext-3.0.1/justext/stoplists/Norwegian_Bokmal.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Norwegian_Nynorsk.txt` & `justext-3.0.1/justext/stoplists/Norwegian_Nynorsk.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Occitan.txt` & `justext-3.0.1/justext/stoplists/Occitan.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Persian.txt` & `justext-3.0.1/justext/stoplists/Persian.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Polish.txt` & `justext-3.0.1/justext/stoplists/Polish.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Portuguese.txt` & `justext-3.0.1/justext/stoplists/Portuguese.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Quechua.txt` & `justext-3.0.1/justext/stoplists/Quechua.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Romanian.txt` & `justext-3.0.1/justext/stoplists/Romanian.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Russian.txt` & `justext-3.0.1/justext/stoplists/Russian.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Samogitian.txt` & `justext-3.0.1/justext/stoplists/Samogitian.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Serbian.txt` & `justext-3.0.1/justext/stoplists/Serbian.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Serbo_Croatian.txt` & `justext-3.0.1/justext/stoplists/Serbo_Croatian.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Sicilian.txt` & `justext-3.0.1/justext/stoplists/Sicilian.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Simple_English.txt` & `justext-3.0.1/justext/stoplists/Simple_English.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Slovak.txt` & `justext-3.0.1/justext/stoplists/Slovak.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Slovenian.txt` & `justext-3.0.1/justext/stoplists/Slovenian.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Spanish.txt` & `justext-3.0.1/justext/stoplists/Spanish.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Sundanese.txt` & `justext-3.0.1/justext/stoplists/Sundanese.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Swahili.txt` & `justext-3.0.1/justext/stoplists/Swahili.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Swedish.txt` & `justext-3.0.1/justext/stoplists/Swedish.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Tagalog.txt` & `justext-3.0.1/justext/stoplists/Tagalog.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Tamil.txt` & `justext-3.0.1/justext/stoplists/Tamil.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Telugu.txt` & `justext-3.0.1/justext/stoplists/Telugu.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Turkish.txt` & `justext-3.0.1/justext/stoplists/Turkish.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Turkmen.txt` & `justext-3.0.1/justext/stoplists/Turkmen.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Ukrainian.txt` & `justext-3.0.1/justext/stoplists/Ukrainian.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Urdu.txt` & `justext-3.0.1/justext/stoplists/Urdu.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Uzbek.txt` & `justext-3.0.1/justext/stoplists/Uzbek.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Vietnamese.txt` & `justext-3.0.1/justext/stoplists/Vietnamese.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Volapuk.txt` & `justext-3.0.1/justext/stoplists/Volapuk.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Walloon.txt` & `justext-3.0.1/justext/stoplists/Walloon.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Welsh.txt` & `justext-3.0.1/justext/stoplists/Welsh.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/West_Frisian.txt` & `justext-3.0.1/justext/stoplists/West_Frisian.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Western_Panjabi.txt` & `justext-3.0.1/justext/stoplists/Western_Panjabi.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/stoplists/Yoruba.txt` & `justext-3.0.1/justext/stoplists/Yoruba.txt`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/justext/utils.py` & `justext-3.0.1/justext/utils.py`

 * *Files identical despite different names*

### Comparing `jusText-3.0.0/setup.py` & `justext-3.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,25 +17,25 @@
 with open("README.rst") as readme:
     with open("CHANGELOG.rst") as changelog:
         long_description = readme.read() + "\n\n" + changelog.read()
 
 
 setup(
     name="jusText",
-    version="3.0.0",
+    version="3.0.1",
     description="Heuristic based boilerplate removal tool",
     long_description=long_description,
     author="Jan Pomikálek",
     author_email="jan.pomikalek@gmail.com",
     maintainer="Michal Belica",
     maintainer_email="miso.belica@gmail.com",
     url="https://github.com/miso-belica/jusText",
     license="The BSD 2-Clause License",
     install_requires=[
-        'lxml >= 4.4.2',
+        'lxml[html_clean] >= 4.4.2',
         'backports.functools-lru-cache; python_version < "3.2"'
     ],
     tests_require=[
         "pytest",
         "pytest-cov",
         "coverage",
     ],
```

