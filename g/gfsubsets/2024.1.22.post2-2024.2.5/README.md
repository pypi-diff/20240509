# Comparing `tmp/gfsubsets-2024.1.22.post2.tar.gz` & `tmp/gfsubsets-2024.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gfsubsets-2024.1.22.post2.tar", last modified: Mon Jan 22 13:14:46 2024, max compression
+gzip compressed data, was "gfsubsets-2024.2.5.tar", last modified: Mon Feb  5 09:16:15 2024, max compression
```

## Comparing `gfsubsets-2024.1.22.post2.tar` & `gfsubsets-2024.2.5.tar`

### file list

```diff
@@ -1,380 +1,382 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 13:14:46.388010 gfsubsets-2024.1.22.post2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 13:14:46.316009 gfsubsets-2024.1.22.post2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 13:14:46.320009 gfsubsets-2024.1.22.post2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/.github/workflows/publish-release.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 13:14:46.316009 gfsubsets-2024.1.22.post2/Lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 13:14:46.320009 gfsubsets-2024.1.22.post2/Lib/gfsubsets/
--rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-01-22 13:14:46.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 13:14:46.348009 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/
--rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/adlam_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/ahom_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    20229 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/anatolian-hieroglyphs_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    63309 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/arabic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/armenian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/avestan_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/balinese_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    22478 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/bamum_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/bassa-vah_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/batak_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/bengali_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/bhaiksuki_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/brahmi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     8707 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/braille_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/buginese_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/buhid_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    25938 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/canadian-aboriginal_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/carian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/caucasian-albanian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/chakma_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/cham_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/cherokee_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    62229 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/chinese-hongkong_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    70904 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/chinese-simplified_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    52834 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/chinese-traditional_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/chorasmian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     7195 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/coptic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    46437 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/cuneiform_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/cypriot_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/cypro-minoan_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    14550 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/cyrillic-ext_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/cyrillic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/deseret_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/devanagari_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/dives-akuru_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/dogra_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/duployan_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    37878 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/egyptian-hieroglyphs_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/elbasan_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/elymaic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    15890 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/ethiopic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/georgian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/glagolitic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/gothic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/grantha_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    12690 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/greek-ext_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/greek_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/gujarati_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/gunjala-gondi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/gurmukhi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/hanifi-rohingya_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/hanunoo_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/hatran_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     4771 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/hebrew_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/imperial-aramaic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/indic-siyaq-numbers_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/inscriptional-pahlavi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/inscriptional-parthian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    60503 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/japanese_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/javanese_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/kaithi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/kannada_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/kawi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/kayah-li_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/kharoshthi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    20986 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/khitan-small-script_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/khmer_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/khojki_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/khudawadi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    94370 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/korean_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/lao_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    36014 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/latin-ext_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     7110 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/latin_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/lepcha_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/limbu_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    11187 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/linear-a_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     9423 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/linear-b_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/lisu_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/lycian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/lydian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/mahajani_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/makasar_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/malayalam_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/mandaic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/manichaean_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/marchen_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/masaram-gondi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    95384 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/math_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/mayan-numerals_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/medefaidrin_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/meetei-mayek_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     8806 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/mende-kikakui_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/meroitic-cursive_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/meroitic-hieroglyphs_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     5440 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/meroitic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/miao_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/modi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     7725 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/mongolian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/mro_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/multani_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    24758 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/music_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     7648 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/myanmar_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/nabataean_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/nag-mundari_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/nandinagari_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/new-tai-lue_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/newa_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/nko_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    14080 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/nushu_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/nyiakeng-puachue-hmong_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/ogham_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/ol-chiki_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/old-hungarian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/old-italic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/old-north-arabian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/old-permic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/old-persian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/old-sogdian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/old-south-arabian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/old-turkic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/old-uyghur_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/oriya_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/osage_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/osmanya_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/ottoman-siyaq-numbers_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/pahawh-hmong_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/palmyrene_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/pau-cin-hau_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/phags-pa_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/phoenician_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/psalter-pahlavi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/rejang_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/runic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/samaritan_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/saurashtra_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/sharada_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/shavian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/siddham_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    34050 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/signwriting_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/sinhala_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/sogdian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/sora-sompeng_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/soyombo_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/sundanese_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/syloti-nagri_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)   122024 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/symbols_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     4874 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/syriac_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/tagalog_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/tagbanwa_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/tai-le_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/tai-tham_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/tai-viet_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/takri_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/tamil-supplement_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/tamil_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/tangsa_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    77985 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/tangut_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/telugu_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/test.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/thaana_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/thai_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/tibetan_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/tifinagh_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/tirhuta_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/toto_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/ugaritic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/vai_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/vietnamese_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/vithkuqi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/wancho_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/warang-citi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/yezidi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    31152 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/yi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/zanabazar-square_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/Lib/gfsubsets/subsets.py
--rw-r--r--   0 runner    (1001) docker     (127)    15526 2024-01-22 13:14:46.388010 gfsubsets-2024.1.22.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 13:14:46.388010 gfsubsets-2024.1.22.post2/gfsubsets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15526 2024-01-22 13:14:46.000000 gfsubsets-2024.1.22.post2/gfsubsets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15973 2024-01-22 13:14:46.000000 gfsubsets-2024.1.22.post2/gfsubsets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-22 13:14:46.000000 gfsubsets-2024.1.22.post2/gfsubsets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-01-22 13:14:46.000000 gfsubsets-2024.1.22.post2/gfsubsets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-22 13:14:46.000000 gfsubsets-2024.1.22.post2/gfsubsets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 13:14:46.348009 gfsubsets-2024.1.22.post2/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/scripts/preprocess_namfile.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-22 13:14:46.388010 gfsubsets-2024.1.22.post2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 13:14:46.356009 gfsubsets-2024.1.22.post2/slices/
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/slices/README.md
--rw-r--r--   0 runner    (1001) docker     (127)  1087488 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/slices/hongkong-chinese_default.txt
--rw-r--r--   0 runner    (1001) docker     (127)   893039 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/slices/japanese_default.txt
--rw-r--r--   0 runner    (1001) docker     (127)   876086 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/slices/korean_default.txt
--rw-r--r--   0 runner    (1001) docker     (127)   889189 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/slices/simplified-chinese_default.txt
--rw-r--r--   0 runner    (1001) docker     (127)   904276 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/slices/traditional-chinese_default.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 13:14:46.384010 gfsubsets-2024.1.22.post2/subsets-input/
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/adlam_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/ahom_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/anatolian-hieroglyphs_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/arabic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/armenian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/avestan_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/balinese_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/bamum_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/bassa-vah_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/batak_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/bengali_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/bhaiksuki_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/brahmi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/braille_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/buginese_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/buhid_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/canadian-aboriginal_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/carian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/caucasian-albanian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/chakma_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/cham_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/cherokee_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)   283071 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/chinese-hongkong_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)   291627 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/chinese-simplified_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)   240250 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/chinese-traditional_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/chorasmian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/cjk_punctuation.nam
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/coptic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/cuneiform_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/cypriot_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/cypro-minoan_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/cyrillic-ext_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/cyrillic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/deseret_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/devanagari_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/dives-akuru_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/dogra_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/duployan_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/egyptian-hieroglyphs_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/elbasan_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/elymaic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/ethiopic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/georgian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/glagolitic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/gothic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/grantha_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/greek-ext_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/greek_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/gujarati_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/gunjala-gondi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/gurmukhi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/hanifi-rohingya_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/hanunoo_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/hatran_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/hebrew_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/imperial-aramaic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/indic-siyaq-numbers_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/inscriptional-pahlavi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/inscriptional-parthian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    82872 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/japanese_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/javanese_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/kaithi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/kannada_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/kawi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/kayah-li_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/kharoshthi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/khitan-small-script_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/khmer_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/khojki_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/khudawadi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/korean_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/lao_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/latin-ext_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/latin_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/lepcha_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/limbu_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/linear-a_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/linear-b_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/lisu_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/lycian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/lydian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/mahajani_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/makasar_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/malayalam_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/mandaic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/manichaean_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/marchen_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/masaram-gondi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/math_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/mayan-numerals_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/medefaidrin_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/meetei-mayek_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/mende-kikakui_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/meroitic-cursive_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/meroitic-hieroglyphs_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/meroitic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/miao_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/modi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/mongolian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/mro_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/multani_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/music_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/myanmar_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/nabataean_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/nag-mundari_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/nandinagari_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/new-tai-lue_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/newa_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/nko_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/nushu_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/nyiakeng-puachue-hmong_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/ogham_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/ol-chiki_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/old-hungarian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/old-italic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/old-north-arabian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/old-permic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/old-persian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/old-sogdian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/old-south-arabian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/old-turkic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/old-uyghur_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/oriya_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/osage_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/osmanya_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/ottoman-siyaq-numbers_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/pahawh-hmong_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/palmyrene_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/pau-cin-hau_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/phags-pa_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/phoenician_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/psalter-pahlavi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/rejang_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/runic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/samaritan_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/saurashtra_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/sharada_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/shavian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/siddham_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/signwriting_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/sinhala_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/sogdian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/sora-sompeng_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/soyombo_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/sundanese_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/syllabic.nam
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/syloti-nagri_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/symbols_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/syriac_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/tagalog_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/tagbanwa_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/tai-le_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/tai-tham_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/tai-viet_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/takri_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/tamil-supplement_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/tamil_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/tangsa_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/tangut_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/telugu_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/thaana_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/thai_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/tibetan_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/tifinagh_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/tirhuta_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/toto_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/ugaritic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/vai_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/vietnamese_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/vithkuqi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/wancho_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/warang-citi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/yezidi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/yi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-01-22 13:14:32.000000 gfsubsets-2024.1.22.post2/subsets-input/zanabazar-square_unique-glyphs.nam
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 09:16:15.457099 gfsubsets-2024.2.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 09:16:15.385099 gfsubsets-2024.2.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 09:16:15.385099 gfsubsets-2024.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/.github/workflows/publish-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 09:16:15.385099 gfsubsets-2024.2.5/Lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 09:16:15.385099 gfsubsets-2024.2.5/Lib/gfsubsets/
+-rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-02-05 09:16:15.000000 gfsubsets-2024.2.5/Lib/gfsubsets/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 09:16:15.417099 gfsubsets-2024.2.5/Lib/gfsubsets/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/adlam_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/ahom_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    20229 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/anatolian-hieroglyphs_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    63309 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/arabic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/armenian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/avestan_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/balinese_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    22478 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/bamum_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/bassa-vah_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/batak_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/bengali_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/bhaiksuki_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/brahmi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     8707 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/braille_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/buginese_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/buhid_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    25938 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/canadian-aboriginal_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/carian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/caucasian-albanian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/chakma_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/cham_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/cherokee_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    62229 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/chinese-hongkong_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    70904 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/chinese-simplified_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    52834 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/chinese-traditional_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/chorasmian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     7195 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/coptic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    46437 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/cuneiform_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/cypriot_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/cypro-minoan_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    14550 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/cyrillic-ext_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/cyrillic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/deseret_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/devanagari_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/dives-akuru_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/dogra_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/duployan_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    37878 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/egyptian-hieroglyphs_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/elbasan_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/elymaic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    15890 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/ethiopic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/georgian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/glagolitic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/gothic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/grantha_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    12690 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/greek-ext_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/greek_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/gujarati_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/gunjala-gondi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/gurmukhi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/hanifi-rohingya_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/hanunoo_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/hatran_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     4771 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/hebrew_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/imperial-aramaic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/indic-siyaq-numbers_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/inscriptional-pahlavi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/inscriptional-parthian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    60503 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/japanese_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/javanese_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/kaithi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/kannada_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/kawi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/kayah-li_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/kharoshthi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    20986 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/khitan-small-script_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/khmer_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/khojki_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/khudawadi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    94370 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/korean_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/lao_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    36014 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/latin-ext_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     7110 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/latin_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/lepcha_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/limbu_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    11187 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/linear-a_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     9423 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/linear-b_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/lisu_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/lycian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/lydian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/mahajani_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/makasar_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/malayalam_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/mandaic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/manichaean_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/marchen_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/masaram-gondi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    95384 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/math_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/mayan-numerals_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/medefaidrin_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/meetei-mayek_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     8806 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/mende-kikakui_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/meroitic-cursive_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/meroitic-hieroglyphs_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     5440 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/meroitic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/miao_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/modi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     7725 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/mongolian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/mro_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/multani_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    24758 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/music_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     7648 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/myanmar_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/nabataean_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/nag-mundari_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/nandinagari_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/new-tai-lue_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/newa_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/nko_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    14080 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/nushu_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/nyiakeng-puachue-hmong_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/ogham_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/ol-chiki_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/old-hungarian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/old-italic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/old-north-arabian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/old-permic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/old-persian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/old-sogdian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/old-south-arabian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/old-turkic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/old-uyghur_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/oriya_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/osage_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/osmanya_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/ottoman-siyaq-numbers_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/pahawh-hmong_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/palmyrene_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/pau-cin-hau_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/phags-pa_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/phoenician_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/psalter-pahlavi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/rejang_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/runic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/samaritan_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/saurashtra_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/sharada_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/shavian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/siddham_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    34050 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/signwriting_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/sinhala_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/sogdian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/sora-sompeng_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/soyombo_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/sundanese_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/syloti-nagri_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)   123099 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/symbols_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     4874 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/syriac_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/tagalog_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/tagbanwa_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/tai-le_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/tai-tham_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/tai-viet_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/takri_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/tamil-supplement_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/tamil_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/tangsa_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    77985 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/tangut_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/telugu_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/test.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/thaana_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/thai_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/tibetan_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/tifinagh_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/tirhuta_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/toto_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/ugaritic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/vai_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/vietnamese_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/vithkuqi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/wancho_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/warang-citi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/yezidi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    31152 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/yi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/zanabazar-square_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     8688 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/data/znamenny_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/Lib/gfsubsets/subsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15519 2024-02-05 09:16:15.457099 gfsubsets-2024.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 09:16:15.457099 gfsubsets-2024.2.5/gfsubsets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15519 2024-02-05 09:16:15.000000 gfsubsets-2024.2.5/gfsubsets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16060 2024-02-05 09:16:15.000000 gfsubsets-2024.2.5/gfsubsets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 09:16:15.000000 gfsubsets-2024.2.5/gfsubsets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-05 09:16:15.000000 gfsubsets-2024.2.5/gfsubsets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-05 09:16:15.000000 gfsubsets-2024.2.5/gfsubsets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 09:16:15.417099 gfsubsets-2024.2.5/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/scripts/preprocess_namfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-05 09:16:15.457099 gfsubsets-2024.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 09:16:15.425099 gfsubsets-2024.2.5/slices/
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/slices/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)  1087488 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/slices/hongkong-chinese_default.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   893039 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/slices/japanese_default.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   876086 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/slices/korean_default.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   889189 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/slices/simplified-chinese_default.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   904276 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/slices/traditional-chinese_default.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 09:16:15.457099 gfsubsets-2024.2.5/subsets-input/
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/adlam_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/ahom_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/anatolian-hieroglyphs_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/arabic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/armenian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/avestan_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/balinese_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/bamum_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/bassa-vah_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/batak_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/bengali_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/bhaiksuki_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/brahmi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/braille_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/buginese_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/buhid_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/canadian-aboriginal_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/carian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/caucasian-albanian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/chakma_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/cham_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/cherokee_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)   283071 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/chinese-hongkong_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)   291627 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/chinese-simplified_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)   240250 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/chinese-traditional_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/chorasmian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/cjk_punctuation.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/coptic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/cuneiform_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/cypriot_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/cypro-minoan_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/cyrillic-ext_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/cyrillic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/deseret_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/devanagari_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/dives-akuru_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/dogra_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/duployan_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/egyptian-hieroglyphs_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/elbasan_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/elymaic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/ethiopic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/georgian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/glagolitic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/gothic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/grantha_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/greek-ext_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/greek_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/gujarati_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/gunjala-gondi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/gurmukhi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/hanifi-rohingya_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/hanunoo_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/hatran_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/hebrew_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/imperial-aramaic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/indic-siyaq-numbers_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/inscriptional-pahlavi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/inscriptional-parthian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    82872 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/japanese_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/javanese_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/kaithi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/kannada_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/kawi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/kayah-li_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/kharoshthi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/khitan-small-script_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/khmer_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/khojki_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/khudawadi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/korean_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/lao_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/latin-ext_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/latin_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/lepcha_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/limbu_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/linear-a_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/linear-b_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/lisu_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/lycian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/lydian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/mahajani_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/makasar_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/malayalam_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/mandaic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/manichaean_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/marchen_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/masaram-gondi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/math_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/mayan-numerals_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/medefaidrin_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/meetei-mayek_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/mende-kikakui_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/meroitic-cursive_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/meroitic-hieroglyphs_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/meroitic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/miao_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/modi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/mongolian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/mro_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/multani_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/music_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/myanmar_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/nabataean_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/nag-mundari_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/nandinagari_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/new-tai-lue_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/newa_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/nko_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/nushu_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/nyiakeng-puachue-hmong_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/ogham_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/ol-chiki_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/old-hungarian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/old-italic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/old-north-arabian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/old-permic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/old-persian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/old-sogdian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/old-south-arabian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/old-turkic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/old-uyghur_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/oriya_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/osage_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/osmanya_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/ottoman-siyaq-numbers_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/pahawh-hmong_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/palmyrene_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/pau-cin-hau_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/phags-pa_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/phoenician_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/psalter-pahlavi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/rejang_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/runic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/samaritan_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/saurashtra_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/sharada_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/shavian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/siddham_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/signwriting_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/sinhala_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/sogdian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/sora-sompeng_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/soyombo_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/sundanese_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/syllabic.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/syloti-nagri_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     5802 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/symbols_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/syriac_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/tagalog_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/tagbanwa_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/tai-le_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/tai-tham_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/tai-viet_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/takri_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/tamil-supplement_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/tamil_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/tangsa_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/tangut_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/telugu_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/thaana_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/thai_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/tibetan_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/tifinagh_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/tirhuta_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/toto_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/ugaritic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/vai_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/vietnamese_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/vithkuqi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/wancho_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/warang-citi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/yezidi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/yi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/zanabazar-square_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-05 09:16:01.000000 gfsubsets-2024.2.5/subsets-input/znamenny_unique-glyphs.nam
```

### Comparing `gfsubsets-2024.1.22.post2/.github/workflows/publish-release.yml` & `gfsubsets-2024.2.5/.github/workflows/publish-release.yml`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/LICENSE` & `gfsubsets-2024.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/__init__.py` & `gfsubsets-2024.2.5/Lib/gfsubsets/__init__.py`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/adlam_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/adlam_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/ahom_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/ahom_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/anatolian-hieroglyphs_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/anatolian-hieroglyphs_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/arabic_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/arabic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/armenian_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/armenian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/avestan_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/avestan_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/balinese_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/balinese_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/bamum_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/bamum_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/bassa-vah_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/bassa-vah_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/batak_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/batak_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/bengali_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/bengali_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/bhaiksuki_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/bhaiksuki_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/brahmi_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/brahmi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/braille_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/braille_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/buginese_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/buginese_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/buhid_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/buhid_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/canadian-aboriginal_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/canadian-aboriginal_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/carian_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/carian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/caucasian-albanian_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/caucasian-albanian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/chakma_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/chakma_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/cham_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/cham_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/cherokee_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/cherokee_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/chinese-hongkong_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/chinese-hongkong_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/chinese-simplified_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/chinese-simplified_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/chinese-traditional_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/chinese-traditional_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/chorasmian_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/chorasmian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/coptic_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/coptic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/cuneiform_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/cuneiform_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/cypriot_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/cypriot_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/cypro-minoan_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/cypro-minoan_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/cyrillic-ext_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/cyrillic-ext_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/cyrillic_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/cyrillic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/deseret_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/deseret_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/devanagari_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/devanagari_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/dives-akuru_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/dives-akuru_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/dogra_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/dogra_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/duployan_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/duployan_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/egyptian-hieroglyphs_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/egyptian-hieroglyphs_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/elbasan_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/elbasan_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/elymaic_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/elymaic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/ethiopic_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/ethiopic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/georgian_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/georgian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/glagolitic_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/glagolitic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/gothic_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/gothic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/grantha_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/grantha_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/greek-ext_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/greek-ext_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/greek_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/greek_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/gujarati_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/gujarati_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/gunjala-gondi_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/gunjala-gondi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/gurmukhi_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/gurmukhi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/hanifi-rohingya_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/hanifi-rohingya_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/hanunoo_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/hanunoo_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/hatran_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/hatran_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/hebrew_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/hebrew_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/imperial-aramaic_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/imperial-aramaic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/indic-siyaq-numbers_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/indic-siyaq-numbers_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/inscriptional-pahlavi_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/inscriptional-pahlavi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/inscriptional-parthian_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/inscriptional-parthian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/japanese_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/japanese_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/javanese_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/javanese_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/kaithi_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/kaithi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/kannada_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/kannada_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/kawi_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/kawi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/kayah-li_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/kayah-li_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/kharoshthi_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/kharoshthi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/khitan-small-script_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/khitan-small-script_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/khmer_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/khmer_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/khojki_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/khojki_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/khudawadi_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/khudawadi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/korean_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/korean_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/lao_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/lao_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/latin-ext_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/latin-ext_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/latin_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/latin_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/lepcha_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/lepcha_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/limbu_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/limbu_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/linear-a_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/linear-a_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/linear-b_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/linear-b_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/lisu_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/lisu_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/lycian_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/lycian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/lydian_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/lydian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/mahajani_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/mahajani_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/makasar_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/makasar_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/malayalam_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/malayalam_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/mandaic_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/mandaic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/manichaean_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/manichaean_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/marchen_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/marchen_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/masaram-gondi_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/masaram-gondi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/math_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/math_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/mayan-numerals_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/mayan-numerals_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/medefaidrin_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/medefaidrin_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/meetei-mayek_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/meetei-mayek_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/mende-kikakui_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/mende-kikakui_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/meroitic-cursive_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/meroitic-cursive_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/meroitic-hieroglyphs_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/meroitic-hieroglyphs_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/meroitic_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/meroitic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/miao_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/miao_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/modi_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/modi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/mongolian_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/mongolian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/mro_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/mro_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/multani_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/multani_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/music_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/music_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/myanmar_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/myanmar_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/nabataean_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/nabataean_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/nag-mundari_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/nag-mundari_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/nandinagari_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/nandinagari_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/new-tai-lue_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/new-tai-lue_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/newa_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/newa_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/nko_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/nko_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/nushu_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/nushu_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/nyiakeng-puachue-hmong_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/nyiakeng-puachue-hmong_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/ogham_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/ogham_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/ol-chiki_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/ol-chiki_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/old-hungarian_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/old-hungarian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/old-italic_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/old-italic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/old-north-arabian_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/old-north-arabian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/old-permic_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/old-permic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/old-persian_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/old-persian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/old-sogdian_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/old-sogdian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/old-south-arabian_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/old-south-arabian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/old-turkic_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/old-turkic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/old-uyghur_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/old-uyghur_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/oriya_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/oriya_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/osage_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/osage_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/osmanya_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/osmanya_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/ottoman-siyaq-numbers_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/ottoman-siyaq-numbers_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/pahawh-hmong_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/pahawh-hmong_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/palmyrene_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/palmyrene_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/pau-cin-hau_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/pau-cin-hau_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/phags-pa_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/phags-pa_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/phoenician_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/phoenician_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/psalter-pahlavi_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/psalter-pahlavi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/rejang_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/rejang_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/runic_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/runic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/samaritan_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/samaritan_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/saurashtra_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/saurashtra_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/sharada_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/sharada_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/shavian_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/shavian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/siddham_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/siddham_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/signwriting_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/signwriting_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/sinhala_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/sinhala_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/sogdian_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/sogdian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/sora-sompeng_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/sora-sompeng_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/soyombo_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/soyombo_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/sundanese_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/sundanese_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/syloti-nagri_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/syloti-nagri_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/symbols_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/symbols_unique-glyphs.nam`

 * *Files 1% similar despite different names*

```diff
@@ -1835,14 +1835,34 @@
 0x10E78 RUMI NUMBER SEVEN HUNDRED
 0x10E79 RUMI NUMBER EIGHT HUNDRED
 0x10E7A RUMI NUMBER NINE HUNDRED
 0x10E7B RUMI FRACTION ONE HALF
 0x10E7C RUMI FRACTION ONE QUARTER
 0x10E7D RUMI FRACTION ONE THIRD
 0x10E7E RUMI FRACTION TWO THIRDS
+0x1D2C0 KAKTOVIK NUMERAL ZERO
+0x1D2C1 KAKTOVIK NUMERAL ONE
+0x1D2C2 KAKTOVIK NUMERAL TWO
+0x1D2C3 KAKTOVIK NUMERAL THREE
+0x1D2C4 KAKTOVIK NUMERAL FOUR
+0x1D2C5 KAKTOVIK NUMERAL FIVE
+0x1D2C6 KAKTOVIK NUMERAL SIX
+0x1D2C7 KAKTOVIK NUMERAL SEVEN
+0x1D2C8 KAKTOVIK NUMERAL EIGHT
+0x1D2C9 KAKTOVIK NUMERAL NINE
+0x1D2CA KAKTOVIK NUMERAL TEN
+0x1D2CB KAKTOVIK NUMERAL ELEVEN
+0x1D2CC KAKTOVIK NUMERAL TWELVE
+0x1D2CD KAKTOVIK NUMERAL THIRTEEN
+0x1D2CE KAKTOVIK NUMERAL FOURTEEN
+0x1D2CF KAKTOVIK NUMERAL FIFTEEN
+0x1D2D0 KAKTOVIK NUMERAL SIXTEEN
+0x1D2D1 KAKTOVIK NUMERAL SEVENTEEN
+0x1D2D2 KAKTOVIK NUMERAL EIGHTEEN
+0x1D2D3 KAKTOVIK NUMERAL NINETEEN
 0x1D2E0 MAYAN NUMERAL ZERO
 0x1D2E1 MAYAN NUMERAL ONE
 0x1D2E2 MAYAN NUMERAL TWO
 0x1D2E3 MAYAN NUMERAL THREE
 0x1D2E4 MAYAN NUMERAL FOUR
 0x1D2E5 MAYAN NUMERAL FIVE
 0x1D2E6 MAYAN NUMERAL SIX
@@ -3175,14 +3195,26 @@
 0x1F8A9 RIGHTWARDS BACK-TILTED SHADOWED WHITE ARROW
 0x1F8AA LEFTWARDS FRONT-TILTED SHADOWED WHITE ARROW
 0x1F8AB RIGHTWARDS FRONT-TILTED SHADOWED WHITE ARROW
 0x1F8AC WHITE ARROW SHAFT WIDTH ONE
 0x1F8AD WHITE ARROW SHAFT WIDTH TWO THIRDS
 0x1F8B0 ARROW POINTING UPWARDS THEN NORTH WEST
 0x1F8B1 ARROW POINTING RIGHTWARDS THEN CURVING SOUTH WEST
+0x1F900 CIRCLED CROSS FORMEE WITH FOUR DOTS
+0x1F901 CIRCLED CROSS FORMEE WITH TWO DOTS
+0x1F902 CIRCLED CROSS FORMEE
+0x1F903 LEFT HALF CIRCLE WITH FOUR DOTS
+0x1F904 LEFT HALF CIRCLE WITH THREE DOTS
+0x1F905 LEFT HALF CIRCLE WITH TWO DOTS
+0x1F906 LEFT HALF CIRCLE WITH DOT
+0x1F907 LEFT HALF CIRCLE
+0x1F908 DOWNWARD FACING HOOK
+0x1F909 DOWNWARD FACING NOTCHED HOOK
+0x1F90A DOWNWARD FACING HOOK WITH DOT
+0x1F90B DOWNWARD FACING NOTCHED HOOK WITH DOT
 0x1F93B MODERN PENTATHLON
 0x1F946 RIFLE
 0x1F984 UNICORN FACE
 0x1F996 T-REX
 0x1F9E9 JIGSAW PUZZLE PIECE
 0x1FA00 NEUTRAL CHESS KING
 0x1FA01 NEUTRAL CHESS QUEEN
```

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/syriac_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/syriac_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/tagalog_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/tagalog_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/tagbanwa_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/tagbanwa_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/tai-le_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/tai-le_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/tai-tham_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/tai-tham_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/tai-viet_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/tai-viet_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/takri_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/takri_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/tamil-supplement_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/tamil-supplement_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/tamil_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/tamil_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/tangsa_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/tangsa_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/tangut_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/tangut_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/telugu_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/telugu_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/thaana_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/thaana_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/thai_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/thai_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/tibetan_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/tibetan_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/tifinagh_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/tifinagh_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/tirhuta_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/tirhuta_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/toto_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/toto_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/ugaritic_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/ugaritic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/vai_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/vai_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/vietnamese_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/vietnamese_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/vithkuqi_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/vithkuqi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/wancho_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/wancho_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/warang-citi_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/warang-citi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/yezidi_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/yezidi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/yi_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/yi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/data/zanabazar-square_unique-glyphs.nam` & `gfsubsets-2024.2.5/Lib/gfsubsets/data/zanabazar-square_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/Lib/gfsubsets/subsets.py` & `gfsubsets-2024.2.5/Lib/gfsubsets/subsets.py`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/PKG-INFO` & `gfsubsets-2024.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gfsubsets
-Version: 2024.1.22.post2
+Version: 2024.2.5
 Summary: Codepoint definitions for the Google Fonts subsetter
 Author-email: Dave Crossland <dave@lab6.com>, Lasse Fister <lasse@graphicore.de>, Marc Foley <m.foley.88@gmail.com>, Simon Cozens <simon@simon-cozens.org>, Garret Rieger <grieger@google.com>, Roderick Sheeter <rsheeter@google.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `gfsubsets-2024.1.22.post2/README.md` & `gfsubsets-2024.2.5/README.md`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/gfsubsets.egg-info/PKG-INFO` & `gfsubsets-2024.2.5/gfsubsets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gfsubsets
-Version: 2024.1.22.post2
+Version: 2024.2.5
 Summary: Codepoint definitions for the Google Fonts subsetter
 Author-email: Dave Crossland <dave@lab6.com>, Lasse Fister <lasse@graphicore.de>, Marc Foley <m.foley.88@gmail.com>, Simon Cozens <simon@simon-cozens.org>, Garret Rieger <grieger@google.com>, Roderick Sheeter <rsheeter@google.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `gfsubsets-2024.1.22.post2/gfsubsets.egg-info/SOURCES.txt` & `gfsubsets-2024.2.5/gfsubsets.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -175,14 +175,15 @@
 Lib/gfsubsets/data/vietnamese_unique-glyphs.nam
 Lib/gfsubsets/data/vithkuqi_unique-glyphs.nam
 Lib/gfsubsets/data/wancho_unique-glyphs.nam
 Lib/gfsubsets/data/warang-citi_unique-glyphs.nam
 Lib/gfsubsets/data/yezidi_unique-glyphs.nam
 Lib/gfsubsets/data/yi_unique-glyphs.nam
 Lib/gfsubsets/data/zanabazar-square_unique-glyphs.nam
+Lib/gfsubsets/data/znamenny_unique-glyphs.nam
 gfsubsets.egg-info/PKG-INFO
 gfsubsets.egg-info/SOURCES.txt
 gfsubsets.egg-info/dependency_links.txt
 gfsubsets.egg-info/requires.txt
 gfsubsets.egg-info/top_level.txt
 scripts/preprocess_namfile.py
 slices/README.md
@@ -361,8 +362,9 @@
 subsets-input/vai_unique-glyphs.nam
 subsets-input/vietnamese_unique-glyphs.nam
 subsets-input/vithkuqi_unique-glyphs.nam
 subsets-input/wancho_unique-glyphs.nam
 subsets-input/warang-citi_unique-glyphs.nam
 subsets-input/yezidi_unique-glyphs.nam
 subsets-input/yi_unique-glyphs.nam
-subsets-input/zanabazar-square_unique-glyphs.nam
+subsets-input/zanabazar-square_unique-glyphs.nam
+subsets-input/znamenny_unique-glyphs.nam
```

### Comparing `gfsubsets-2024.1.22.post2/pyproject.toml` & `gfsubsets-2024.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/scripts/preprocess_namfile.py` & `gfsubsets-2024.2.5/scripts/preprocess_namfile.py`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/slices/README.md` & `gfsubsets-2024.2.5/slices/README.md`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/slices/hongkong-chinese_default.txt` & `gfsubsets-2024.2.5/slices/hongkong-chinese_default.txt`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/slices/japanese_default.txt` & `gfsubsets-2024.2.5/slices/japanese_default.txt`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/slices/korean_default.txt` & `gfsubsets-2024.2.5/slices/korean_default.txt`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/slices/simplified-chinese_default.txt` & `gfsubsets-2024.2.5/slices/simplified-chinese_default.txt`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/slices/traditional-chinese_default.txt` & `gfsubsets-2024.2.5/slices/traditional-chinese_default.txt`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/subsets-input/adlam_unique-glyphs.nam` & `gfsubsets-2024.2.5/subsets-input/adlam_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/subsets-input/caucasian-albanian_unique-glyphs.nam` & `gfsubsets-2024.2.5/subsets-input/caucasian-albanian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/subsets-input/chinese-hongkong_unique-glyphs.nam` & `gfsubsets-2024.2.5/subsets-input/chinese-hongkong_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/subsets-input/chinese-simplified_unique-glyphs.nam` & `gfsubsets-2024.2.5/subsets-input/chinese-simplified_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/subsets-input/chinese-traditional_unique-glyphs.nam` & `gfsubsets-2024.2.5/subsets-input/chinese-traditional_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/subsets-input/cjk_punctuation.nam` & `gfsubsets-2024.2.5/subsets-input/cjk_punctuation.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/subsets-input/coptic_unique-glyphs.nam` & `gfsubsets-2024.2.5/subsets-input/coptic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/subsets-input/gunjala-gondi_unique-glyphs.nam` & `gfsubsets-2024.2.5/subsets-input/gunjala-gondi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/subsets-input/japanese_unique-glyphs.nam` & `gfsubsets-2024.2.5/subsets-input/japanese_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/subsets-input/latin-ext_unique-glyphs.nam` & `gfsubsets-2024.2.5/subsets-input/latin-ext_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/subsets-input/latin_unique-glyphs.nam` & `gfsubsets-2024.2.5/subsets-input/latin_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/subsets-input/masaram-gondi_unique-glyphs.nam` & `gfsubsets-2024.2.5/subsets-input/masaram-gondi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/subsets-input/math_unique-glyphs.nam` & `gfsubsets-2024.2.5/subsets-input/math_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/subsets-input/mongolian_unique-glyphs.nam` & `gfsubsets-2024.2.5/subsets-input/mongolian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/subsets-input/symbols_unique-glyphs.nam` & `gfsubsets-2024.2.5/subsets-input/symbols_unique-glyphs.nam`

 * *Files 2% similar despite different names*

```diff
@@ -227,16 +227,20 @@
 0x1F6FB PICKUP TRUCK
 0x1F6FC ROLLER SKATE
 
 @block(Alchemical Symbols)
 @block(Geometric Shapes Extended)
 @block(Supplemental Arrows-C)
 
+0x1F900..0x1F90B
+
 0x1F93B MODERN PENTATHLON
 0x1F946 RIFLE
 0x1F984 UNICORN FACE
 0x1F996 T-REX
 0x1F9E9 JIGSAW PUZZLE PIECE
 
 @block(Chess Symbols)
 @block(Symbols and Pictographs Extended-A)
 @block(Symbols for Legacy Computing)
+@block(Kaktovik Numerals)
+
```

### Comparing `gfsubsets-2024.1.22.post2/subsets-input/syriac_unique-glyphs.nam` & `gfsubsets-2024.2.5/subsets-input/syriac_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/subsets-input/thaana_unique-glyphs.nam` & `gfsubsets-2024.2.5/subsets-input/thaana_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/subsets-input/vietnamese_unique-glyphs.nam` & `gfsubsets-2024.2.5/subsets-input/vietnamese_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gfsubsets-2024.1.22.post2/subsets-input/yi_unique-glyphs.nam` & `gfsubsets-2024.2.5/subsets-input/yi_unique-glyphs.nam`

 * *Files identical despite different names*

