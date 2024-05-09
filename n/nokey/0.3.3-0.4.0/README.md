# Comparing `tmp/nokey-0.3.3.tar.gz` & `tmp/nokey-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nokey-0.3.3.tar", last modified: Sun Apr 28 00:56:01 2024, max compression
+gzip compressed data, was "nokey-0.4.0.tar", last modified: Thu May  9 00:37:27 2024, max compression
```

## Comparing `nokey-0.3.3.tar` & `nokey-0.4.0.tar`

### file list

```diff
@@ -1,89 +1,90 @@
-drwx------   0 root         (0) root         (0)        0 2024-04-28 00:56:01.695121 nokey-0.3.3/
--rw-------   0 root         (0) root         (0)     1068 2024-04-10 23:28:41.000000 nokey-0.3.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3742 2024-04-28 00:56:01.691121 nokey-0.3.3/PKG-INFO
--rw-------   0 root         (0) root         (0)     3164 2024-04-27 13:46:03.000000 nokey-0.3.3/README.md
-drwx------   0 root         (0) root         (0)        0 2024-04-28 00:56:01.391121 nokey-0.3.3/nokey/
--rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/__init__.py
-drwx------   0 root         (0) root         (0)        0 2024-04-28 00:56:01.415121 nokey-0.3.3/nokey/activities/
--rw-------   0 root         (0) root         (0)     5116 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/activities/bored_api.py
-drwx------   0 root         (0) root         (0)        0 2024-04-28 00:56:01.423121 nokey-0.3.3/nokey/animals/
--rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/animals/__init__.py
--rw-------   0 root         (0) root         (0)     2754 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/animals/dog_api.py
-drwx------   0 root         (0) root         (0)        0 2024-04-28 00:56:01.431121 nokey-0.3.3/nokey/art_and_images/
--rw-------   0 root         (0) root         (0)     7770 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/art_and_images/lorem_picsum.py
-drwx------   0 root         (0) root         (0)        0 2024-04-28 00:56:01.439121 nokey-0.3.3/nokey/books_and_literature/
--rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/books_and_literature/__init__.py
--rw-------   0 root         (0) root         (0)     6079 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/books_and_literature/gutendex.py
-drwx------   0 root         (0) root         (0)        0 2024-04-28 00:56:01.451121 nokey-0.3.3/nokey/calendar/
--rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/calendar/__init__.py
--rw-------   0 root         (0) root         (0)     4848 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/calendar/nager_date.py
-drwx------   0 root         (0) root         (0)        0 2024-04-28 00:56:01.459121 nokey-0.3.3/nokey/country_info/
--rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/country_info/__init__.py
--rw-------   0 root         (0) root         (0)     4740 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/country_info/rest_country.py
-drwx------   0 root         (0) root         (0)        0 2024-04-28 00:56:01.491121 nokey-0.3.3/nokey/developer_tools/
--rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/developer_tools/__init__.py
--rw-------   0 root         (0) root         (0)     3945 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/developer_tools/apis_guru.py
--rw-------   0 root         (0) root         (0)     3564 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/developer_tools/filter_lists.py
--rw-------   0 root         (0) root         (0)     2578 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/developer_tools/microlink.py
--rw-------   0 root         (0) root         (0)     7314 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/developer_tools/url_haus.py
--rw-------   0 root         (0) root         (0)     1621 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/developer_tools/url_shortener.py
-drwx------   0 root         (0) root         (0)        0 2024-04-28 00:56:01.503121 nokey-0.3.3/nokey/education/
--rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/education/__init__.py
--rw-------   0 root         (0) root         (0)     2348 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/education/university_domains_and_names.py
-drwx------   0 root         (0) root         (0)        0 2024-04-28 00:56:01.523121 nokey-0.3.3/nokey/finance_and_crypto/
--rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/finance_and_crypto/__init__.py
--rw-------   0 root         (0) root         (0)     5877 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/finance_and_crypto/coinmap.py
--rw-------   0 root         (0) root         (0)     2513 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/finance_and_crypto/exchange_api.py
--rw-------   0 root         (0) root         (0)     1127 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/finance_and_crypto/wall_street_bets.py
-drwx------   0 root         (0) root         (0)        0 2024-04-28 00:56:01.535121 nokey-0.3.3/nokey/food/
--rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/food/__init__.py
--rw-------   0 root         (0) root         (0)     3198 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/food/fruityvice.py
-drwx------   0 root         (0) root         (0)        0 2024-04-28 00:56:01.551121 nokey-0.3.3/nokey/games/
--rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/games/__init__.py
--rw-------   0 root         (0) root         (0)     6542 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/games/free_to_game.py
--rw-------   0 root         (0) root         (0)     5382 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/games/open_trivia_db.py
-drwx------   0 root         (0) root         (0)        0 2024-04-28 00:56:01.563121 nokey-0.3.3/nokey/geolocation/
--rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/geolocation/__init__.py
--rw-------   0 root         (0) root         (0)     1045 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/geolocation/ip_api.py
--rw-------   0 root         (0) root         (0)     1874 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/geolocation/zippopotamus.py
-drwx------   0 root         (0) root         (0)        0 2024-04-28 00:56:01.575121 nokey-0.3.3/nokey/government/
--rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/government/__init__.py
--rw-------   0 root         (0) root         (0)    10654 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/government/federal_register.py
-drwx------   0 root         (0) root         (0)        0 2024-04-28 00:56:01.595121 nokey-0.3.3/nokey/helperFuncs/
--rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/helperFuncs/__init__.py
--rw-------   0 root         (0) root         (0)      822 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/helperFuncs/get_api_list.py
--rw-------   0 root         (0) root         (0)     3234 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/helperFuncs/make_request.py
--rw-------   0 root         (0) root         (0)      954 2024-04-27 14:00:02.000000 nokey-0.3.3/nokey/helperFuncs/nokey_apis.py
-drwx------   0 root         (0) root         (0)        0 2024-04-28 00:56:01.603121 nokey-0.3.3/nokey/inspiration/
--rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/inspiration/__init__.py
--rw-------   0 root         (0) root         (0)     5925 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/inspiration/dictum.py
-drwx------   0 root         (0) root         (0)        0 2024-04-28 00:56:01.615121 nokey-0.3.3/nokey/jokes/
--rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/jokes/__init__.py
--rw-------   0 root         (0) root         (0)     3004 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/jokes/joke_api.py
-drwx------   0 root         (0) root         (0)        0 2024-04-28 00:56:01.623121 nokey-0.3.3/nokey/language/
--rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/language/__init__.py
--rw-------   0 root         (0) root         (0)     1185 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/language/free_dictionary.py
-drwx------   0 root         (0) root         (0)        0 2024-04-28 00:56:01.635121 nokey-0.3.3/nokey/random/
--rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/random/__init__.py
--rw-------   0 root         (0) root         (0)     1119 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/random/random_user.py
-drwx------   0 root         (0) root         (0)        0 2024-04-28 00:56:01.651121 nokey-0.3.3/nokey/science_and_nature/
--rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/science_and_nature/__init__.py
--rw-------   0 root         (0) root         (0)    50596 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/science_and_nature/integrated_taxonomic_information_system.py
--rw-------   0 root         (0) root         (0)     2948 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/science_and_nature/nobel_prize.py
-drwx------   0 root         (0) root         (0)        0 2024-04-28 00:56:01.659121 nokey-0.3.3/nokey/spaceflight/
--rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/spaceflight/__init__.py
--rw-------   0 root         (0) root         (0)     8784 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/spaceflight/spaceflight_news.py
-drwx------   0 root         (0) root         (0)        0 2024-04-28 00:56:01.671121 nokey-0.3.3/nokey/tv_and_film/
--rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/tv_and_film/__init__.py
--rw-------   0 root         (0) root         (0)    43523 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/tv_and_film/star_trek_api.py
-drwx------   0 root         (0) root         (0)        0 2024-04-28 00:56:01.683121 nokey-0.3.3/nokey/weather/
--rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/weather/__init__.py
--rw-------   0 root         (0) root         (0)    26115 2024-04-27 13:48:18.000000 nokey-0.3.3/nokey/weather/national_weather_service.py
-drwx------   0 root         (0) root         (0)        0 2024-04-28 00:56:01.687121 nokey-0.3.3/nokey.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3742 2024-04-28 00:56:01.000000 nokey-0.3.3/nokey.egg-info/PKG-INFO
--rw-------   0 root         (0) root         (0)     1946 2024-04-28 00:56:01.000000 nokey-0.3.3/nokey.egg-info/SOURCES.txt
--rw-------   0 root         (0) root         (0)        1 2024-04-28 00:56:01.000000 nokey-0.3.3/nokey.egg-info/dependency_links.txt
--rw-------   0 root         (0) root         (0)       27 2024-04-28 00:56:01.000000 nokey-0.3.3/nokey.egg-info/requires.txt
--rw-------   0 root         (0) root         (0)        6 2024-04-28 00:56:01.000000 nokey-0.3.3/nokey.egg-info/top_level.txt
--rw-------   0 root         (0) root         (0)      557 2024-04-28 00:55:31.000000 nokey-0.3.3/pyproject.toml
--rw-------   0 root         (0) root         (0)       38 2024-04-28 00:56:01.695121 nokey-0.3.3/setup.cfg
+drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.362013 nokey-0.4.0/
+-rw-------   0 root         (0) root         (0)     1068 2024-04-10 23:28:41.000000 nokey-0.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3756 2024-05-09 00:37:27.362013 nokey-0.4.0/PKG-INFO
+-rw-------   0 root         (0) root         (0)     3178 2024-05-09 00:35:34.000000 nokey-0.4.0/README.md
+drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.050013 nokey-0.4.0/nokey/
+-rw-------   0 root         (0) root         (0)        0 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/__init__.py
+drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.074013 nokey-0.4.0/nokey/activities/
+-rw-------   0 root         (0) root         (0)     5116 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/activities/bored_api.py
+drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.082013 nokey-0.4.0/nokey/animals/
+-rw-------   0 root         (0) root         (0)        0 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/animals/__init__.py
+-rw-------   0 root         (0) root         (0)     2754 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/animals/dog_api.py
+drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.086013 nokey-0.4.0/nokey/art_and_images/
+-rw-------   0 root         (0) root         (0)     7770 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/art_and_images/lorem_picsum.py
+drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.098013 nokey-0.4.0/nokey/books_and_literature/
+-rw-------   0 root         (0) root         (0)        0 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/books_and_literature/__init__.py
+-rw-------   0 root         (0) root         (0)     6079 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/books_and_literature/gutendex.py
+drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.106013 nokey-0.4.0/nokey/calendar/
+-rw-------   0 root         (0) root         (0)        0 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/calendar/__init__.py
+-rw-------   0 root         (0) root         (0)     4848 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/calendar/nager_date.py
+drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.118013 nokey-0.4.0/nokey/country_info/
+-rw-------   0 root         (0) root         (0)        0 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/country_info/__init__.py
+-rw-------   0 root         (0) root         (0)     4740 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/country_info/rest_country.py
+drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.150013 nokey-0.4.0/nokey/developer_tools/
+-rw-------   0 root         (0) root         (0)        0 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/developer_tools/__init__.py
+-rw-------   0 root         (0) root         (0)     3945 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/developer_tools/apis_guru.py
+-rw-------   0 root         (0) root         (0)     3564 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/developer_tools/filter_lists.py
+-rw-------   0 root         (0) root         (0)     2578 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/developer_tools/microlink.py
+-rw-------   0 root         (0) root         (0)     7314 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/developer_tools/url_haus.py
+-rw-------   0 root         (0) root         (0)     1621 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/developer_tools/url_shortener.py
+drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.158013 nokey-0.4.0/nokey/education/
+-rw-------   0 root         (0) root         (0)        0 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/education/__init__.py
+-rw-------   0 root         (0) root         (0)     2348 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/education/university_domains_and_names.py
+drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.186013 nokey-0.4.0/nokey/finance_and_crypto/
+-rw-------   0 root         (0) root         (0)        0 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/finance_and_crypto/__init__.py
+-rw-------   0 root         (0) root         (0)     5877 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/finance_and_crypto/coinmap.py
+-rw-------   0 root         (0) root         (0)     2513 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/finance_and_crypto/exchange_api.py
+-rw-------   0 root         (0) root         (0)     1127 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/finance_and_crypto/wall_street_bets.py
+drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.198013 nokey-0.4.0/nokey/food/
+-rw-------   0 root         (0) root         (0)        0 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/food/__init__.py
+-rw-------   0 root         (0) root         (0)     3198 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/food/fruityvice.py
+drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.210013 nokey-0.4.0/nokey/games/
+-rw-------   0 root         (0) root         (0)        0 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/games/__init__.py
+-rw-------   0 root         (0) root         (0)     6542 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/games/free_to_game.py
+-rw-------   0 root         (0) root         (0)     5382 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/games/open_trivia_db.py
+drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.226013 nokey-0.4.0/nokey/geolocation/
+-rw-------   0 root         (0) root         (0)        0 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/geolocation/__init__.py
+-rw-------   0 root         (0) root         (0)     1045 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/geolocation/ip_api.py
+-rw-------   0 root         (0) root         (0)     1874 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/geolocation/zippopotamus.py
+drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.242013 nokey-0.4.0/nokey/government/
+-rw-------   0 root         (0) root         (0)        0 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/government/__init__.py
+-rw-------   0 root         (0) root         (0)    10654 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/government/federal_register.py
+-rw-------   0 root         (0) root         (0)   157333 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/government/usa_spending.py
+drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.266013 nokey-0.4.0/nokey/helperFuncs/
+-rw-------   0 root         (0) root         (0)        0 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/helperFuncs/__init__.py
+-rw-------   0 root         (0) root         (0)      822 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/helperFuncs/get_api_list.py
+-rw-------   0 root         (0) root         (0)     5137 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/helperFuncs/make_request.py
+-rw-------   0 root         (0) root         (0)      970 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/helperFuncs/nokey_apis.py
+drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.274013 nokey-0.4.0/nokey/inspiration/
+-rw-------   0 root         (0) root         (0)        0 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/inspiration/__init__.py
+-rw-------   0 root         (0) root         (0)     5925 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/inspiration/dictum.py
+drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.286013 nokey-0.4.0/nokey/jokes/
+-rw-------   0 root         (0) root         (0)        0 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/jokes/__init__.py
+-rw-------   0 root         (0) root         (0)     3004 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/jokes/joke_api.py
+drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.294013 nokey-0.4.0/nokey/language/
+-rw-------   0 root         (0) root         (0)        0 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/language/__init__.py
+-rw-------   0 root         (0) root         (0)     1185 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/language/free_dictionary.py
+drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.306013 nokey-0.4.0/nokey/random/
+-rw-------   0 root         (0) root         (0)        0 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/random/__init__.py
+-rw-------   0 root         (0) root         (0)     1119 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/random/random_user.py
+drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.318013 nokey-0.4.0/nokey/science_and_nature/
+-rw-------   0 root         (0) root         (0)        0 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/science_and_nature/__init__.py
+-rw-------   0 root         (0) root         (0)    50596 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/science_and_nature/integrated_taxonomic_information_system.py
+-rw-------   0 root         (0) root         (0)     2948 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/science_and_nature/nobel_prize.py
+drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.330013 nokey-0.4.0/nokey/spaceflight/
+-rw-------   0 root         (0) root         (0)        0 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/spaceflight/__init__.py
+-rw-------   0 root         (0) root         (0)     8784 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/spaceflight/spaceflight_news.py
+drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.338013 nokey-0.4.0/nokey/tv_and_film/
+-rw-------   0 root         (0) root         (0)        0 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/tv_and_film/__init__.py
+-rw-------   0 root         (0) root         (0)    43523 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/tv_and_film/star_trek_api.py
+drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.350013 nokey-0.4.0/nokey/weather/
+-rw-------   0 root         (0) root         (0)        0 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/weather/__init__.py
+-rw-------   0 root         (0) root         (0)    26115 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/weather/national_weather_service.py
+drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.358013 nokey-0.4.0/nokey.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3756 2024-05-09 00:37:26.000000 nokey-0.4.0/nokey.egg-info/PKG-INFO
+-rw-------   0 root         (0) root         (0)     1979 2024-05-09 00:37:26.000000 nokey-0.4.0/nokey.egg-info/SOURCES.txt
+-rw-------   0 root         (0) root         (0)        1 2024-05-09 00:37:26.000000 nokey-0.4.0/nokey.egg-info/dependency_links.txt
+-rw-------   0 root         (0) root         (0)       27 2024-05-09 00:37:26.000000 nokey-0.4.0/nokey.egg-info/requires.txt
+-rw-------   0 root         (0) root         (0)        6 2024-05-09 00:37:26.000000 nokey-0.4.0/nokey.egg-info/top_level.txt
+-rw-------   0 root         (0) root         (0)      557 2024-05-09 00:36:14.000000 nokey-0.4.0/pyproject.toml
+-rw-------   0 root         (0) root         (0)       38 2024-05-09 00:37:27.366013 nokey-0.4.0/setup.cfg
```

### Comparing `nokey-0.3.3/LICENSE` & `nokey-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nokey-0.3.3/PKG-INFO` & `nokey-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nokey
-Version: 0.3.3
+Version: 0.4.0
 Summary: A python package for accessing APIs that require no key.
 Author-email: Spyder Rex <billyjohnsonauthor@gmail.com>
 Project-URL: Homepage, https://github.com/SpyderRex/nokey
 Project-URL: Issues, https://github.com/Spyder/nokey/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -48,17 +48,17 @@
 # Print the URL
 print(dog_image_url)
 ```
 
 Also, to print out a list of the APIs supported by nokey, simply run the following script:
 
 ```python
-from nokey.helperFuncs import get_api_list
+from nokey.helperFuncs.get_api_list import get_api_list
 
-api_list = get_api_list.get_api_list()
+api_list = get_api_list()
 
 print(api_list)
 ```
 
 Each API class has an "about" attribute that returns a short description of the API. To get the URL for the API documentation of any API, simply call the get_docs_url() method for the API class.
 
 ## Contributing
@@ -133,14 +133,16 @@
 
 ## calendar
 Nager.Date
 
 ## government
 Federal Register
 
+USA Spending
+
 ## tv_and_film
 Star Trek API
 
 ## books_and_literature
 Gutendex
 
 # Future Roadmap
```

### Comparing `nokey-0.3.3/README.md` & `nokey-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 # Print the URL
 print(dog_image_url)
 ```
 
 Also, to print out a list of the APIs supported by nokey, simply run the following script:
 
 ```python
-from nokey.helperFuncs import get_api_list
+from nokey.helperFuncs.get_api_list import get_api_list
 
-api_list = get_api_list.get_api_list()
+api_list = get_api_list()
 
 print(api_list)
 ```
 
 Each API class has an "about" attribute that returns a short description of the API. To get the URL for the API documentation of any API, simply call the get_docs_url() method for the API class.
 
 ## Contributing
@@ -117,14 +117,16 @@
 
 ## calendar
 Nager.Date
 
 ## government
 Federal Register
 
+USA Spending
+
 ## tv_and_film
 Star Trek API
 
 ## books_and_literature
 Gutendex
 
 # Future Roadmap
```

### Comparing `nokey-0.3.3/nokey/activities/bored_api.py` & `nokey-0.4.0/nokey/activities/bored_api.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.3/nokey/animals/dog_api.py` & `nokey-0.4.0/nokey/animals/dog_api.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.3/nokey/art_and_images/lorem_picsum.py` & `nokey-0.4.0/nokey/art_and_images/lorem_picsum.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.3/nokey/books_and_literature/gutendex.py` & `nokey-0.4.0/nokey/books_and_literature/gutendex.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.3/nokey/calendar/nager_date.py` & `nokey-0.4.0/nokey/calendar/nager_date.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.3/nokey/country_info/rest_country.py` & `nokey-0.4.0/nokey/country_info/rest_country.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.3/nokey/developer_tools/apis_guru.py` & `nokey-0.4.0/nokey/developer_tools/apis_guru.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.3/nokey/developer_tools/filter_lists.py` & `nokey-0.4.0/nokey/developer_tools/filter_lists.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.3/nokey/developer_tools/microlink.py` & `nokey-0.4.0/nokey/developer_tools/microlink.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.3/nokey/developer_tools/url_haus.py` & `nokey-0.4.0/nokey/developer_tools/url_haus.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.3/nokey/developer_tools/url_shortener.py` & `nokey-0.4.0/nokey/developer_tools/url_shortener.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.3/nokey/education/university_domains_and_names.py` & `nokey-0.4.0/nokey/education/university_domains_and_names.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.3/nokey/finance_and_crypto/coinmap.py` & `nokey-0.4.0/nokey/finance_and_crypto/coinmap.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.3/nokey/finance_and_crypto/exchange_api.py` & `nokey-0.4.0/nokey/finance_and_crypto/exchange_api.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.3/nokey/finance_and_crypto/wall_street_bets.py` & `nokey-0.4.0/nokey/finance_and_crypto/wall_street_bets.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.3/nokey/food/fruityvice.py` & `nokey-0.4.0/nokey/food/fruityvice.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.3/nokey/games/free_to_game.py` & `nokey-0.4.0/nokey/games/free_to_game.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.3/nokey/games/open_trivia_db.py` & `nokey-0.4.0/nokey/games/open_trivia_db.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.3/nokey/geolocation/ip_api.py` & `nokey-0.4.0/nokey/geolocation/ip_api.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.3/nokey/geolocation/zippopotamus.py` & `nokey-0.4.0/nokey/geolocation/zippopotamus.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.3/nokey/government/federal_register.py` & `nokey-0.4.0/nokey/government/federal_register.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.3/nokey/helperFuncs/get_api_list.py` & `nokey-0.4.0/nokey/helperFuncs/get_api_list.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.3/nokey/helperFuncs/make_request.py` & `nokey-0.4.0/nokey/helperFuncs/make_request.py`

 * *Files 24% similar despite different names*

```diff
@@ -82,9 +82,65 @@
         return {"error": "Request timed out."}
     except RequestException as req_err:
         # Handle other request exceptions
         return {"error": f"Request exception occurred: {req_err}"}
     except Exception as err:
         # Handle any other unexpected errors
         return {"error": f"An unexpected error occurred: {err}"}
+        
+def make_request_with_post_and_data(url, data):
+    """
+    Make a request to an API if the API using the POST method.
+    
+    Args:
+    - url (str): The url of the API.
+    - data (dict): The data to be included in the request.
+    
+    Returns:
+    - dict: A dictionary containing either the response data or an error message.
+    """
+    try:
+        response = requests.post(url, data=data)
+        return response.json()
+    except HTTPError as http_err:
+        # Handle HTTP error
+        return {"error": f"HTTP error occurred: {http_err}"}
+    except Timeout:
+        # Handle timeout error
+        return {"error": "Request timed out."}
+    except RequestException as req_err:
+        # Handle other request exceptions
+        return {"error": f"Request exception occurred: {req_err}"}
+    except Exception as err:
+        # Handle any other unexpected errors
+        return {"error": f"An unexpected error occurred: {err}"}
+        
+def make_request_with_post_and_json(url, json):
+    """
+    Make a request to an API if the API using the POST method.
+    
+    Args:
+    - url (str): The url of the API.
+    - data (dict): The data to be included in the request.
+    
+    Returns:
+    - dict: A dictionary containing either the response data or an error message.
+    """
+    try:
+        response = requests.post(url, json=json)
+        return response.json()
+    except HTTPError as http_err:
+        # Handle HTTP error
+        return {"error": f"HTTP error occurred: {http_err}"}
+    except Timeout:
+        # Handle timeout error
+        return {"error": "Request timed out."}
+    except RequestException as req_err:
+        # Handle other request exceptions
+        return {"error": f"Request exception occurred: {req_err}"}
+    except Exception as err:
+        # Handle any other unexpected errors
+        return {"error": f"An unexpected error occurred: {err}"}
+   
+
```

### Comparing `nokey-0.3.3/nokey/helperFuncs/nokey_apis.py` & `nokey-0.4.0/nokey/helperFuncs/nokey_apis.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,12 +12,12 @@
     "weather": ["National Weather Service API"],
     "developer_tools": ["URL Shortener", "URLHaus", "APIsGuru", "Microlink", "FilterLists"],
     "inspiration": ["Dictum"],
     "language": ["Free Dictionary"],
     "games": ["Free To Game", "Open Trivia Database"],
     "activities": ["Bored API"],
     "calendar": ["Nager.Date"],
-    "government": ["Federal Register"],
+    "government": ["Federal Register", "USA Spending"],
     "art_and_images": ["Lorem Picsum"],
     "tv_and_film": ["Star Trek API"],
     "books": ["Gutendex"]
 }
```

### Comparing `nokey-0.3.3/nokey/inspiration/dictum.py` & `nokey-0.4.0/nokey/inspiration/dictum.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.3/nokey/jokes/joke_api.py` & `nokey-0.4.0/nokey/jokes/joke_api.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.3/nokey/language/free_dictionary.py` & `nokey-0.4.0/nokey/language/free_dictionary.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.3/nokey/random/random_user.py` & `nokey-0.4.0/nokey/random/random_user.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.3/nokey/science_and_nature/integrated_taxonomic_information_system.py` & `nokey-0.4.0/nokey/science_and_nature/integrated_taxonomic_information_system.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.3/nokey/science_and_nature/nobel_prize.py` & `nokey-0.4.0/nokey/science_and_nature/nobel_prize.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.3/nokey/spaceflight/spaceflight_news.py` & `nokey-0.4.0/nokey/spaceflight/spaceflight_news.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.3/nokey/tv_and_film/star_trek_api.py` & `nokey-0.4.0/nokey/tv_and_film/star_trek_api.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.3/nokey/weather/national_weather_service.py` & `nokey-0.4.0/nokey/weather/national_weather_service.py`

 * *Files identical despite different names*

### Comparing `nokey-0.3.3/nokey.egg-info/PKG-INFO` & `nokey-0.4.0/nokey.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nokey
-Version: 0.3.3
+Version: 0.4.0
 Summary: A python package for accessing APIs that require no key.
 Author-email: Spyder Rex <billyjohnsonauthor@gmail.com>
 Project-URL: Homepage, https://github.com/SpyderRex/nokey
 Project-URL: Issues, https://github.com/Spyder/nokey/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -48,17 +48,17 @@
 # Print the URL
 print(dog_image_url)
 ```
 
 Also, to print out a list of the APIs supported by nokey, simply run the following script:
 
 ```python
-from nokey.helperFuncs import get_api_list
+from nokey.helperFuncs.get_api_list import get_api_list
 
-api_list = get_api_list.get_api_list()
+api_list = get_api_list()
 
 print(api_list)
 ```
 
 Each API class has an "about" attribute that returns a short description of the API. To get the URL for the API documentation of any API, simply call the get_docs_url() method for the API class.
 
 ## Contributing
@@ -133,14 +133,16 @@
 
 ## calendar
 Nager.Date
 
 ## government
 Federal Register
 
+USA Spending
+
 ## tv_and_film
 Star Trek API
 
 ## books_and_literature
 Gutendex
 
 # Future Roadmap
```

### Comparing `nokey-0.3.3/nokey.egg-info/SOURCES.txt` & `nokey-0.4.0/nokey.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 nokey/games/free_to_game.py
 nokey/games/open_trivia_db.py
 nokey/geolocation/__init__.py
 nokey/geolocation/ip_api.py
 nokey/geolocation/zippopotamus.py
 nokey/government/__init__.py
 nokey/government/federal_register.py
+nokey/government/usa_spending.py
 nokey/helperFuncs/__init__.py
 nokey/helperFuncs/get_api_list.py
 nokey/helperFuncs/make_request.py
 nokey/helperFuncs/nokey_apis.py
 nokey/inspiration/__init__.py
 nokey/inspiration/dictum.py
 nokey/jokes/__init__.py
```

### Comparing `nokey-0.3.3/pyproject.toml` & `nokey-0.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nokey"
-version = "0.3.3"
+version = "0.4.0"
 authors = [
   { name="Spyder Rex", email="billyjohnsonauthor@gmail.com" },
 ]
 description = "A python package for accessing APIs that require no key."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

