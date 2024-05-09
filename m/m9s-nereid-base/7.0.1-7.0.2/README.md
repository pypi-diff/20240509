# Comparing `tmp/m9s_nereid_base-7.0.1.tar.gz` & `tmp/m9s_nereid_base-7.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m9s_nereid_base-7.0.1.tar", last modified: Thu Apr 25 14:14:33 2024, max compression
+gzip compressed data, was "m9s_nereid_base-7.0.2.tar", last modified: Thu May  9 09:32:51 2024, max compression
```

## Comparing `m9s_nereid_base-7.0.1.tar` & `m9s_nereid_base-7.0.2.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:14:33.892678 m9s_nereid_base-7.0.1/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       81 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.1/.coveragerc
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1875 2022-02-15 11:09:33.000000 m9s_nereid_base-7.0.1/.drone.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.1/.flake8
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.1/.gitlab-ci-m9s.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2217 2024-04-25 09:39:28.000000 m9s_nereid_base-7.0.1/.gitlab-ci.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.1/.isort.cfg
-drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:14:33.888678 m9s_nereid_base-7.0.1/.woodpecker/
--rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     1367 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.1/.woodpecker/mail_curl.sh
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      645 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.1/.woodpecker/report.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1302 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.1/.woodpecker/test.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      862 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.1/COPYRIGHT
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.1/INSTALL
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.1/LICENSE
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      121 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.1/MANIFEST.in
--rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     3204 2024-04-25 14:14:33.892678 m9s_nereid_base-7.0.1/PKG-INFO
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1042 2024-04-25 14:06:28.000000 m9s_nereid_base-7.0.1/README.md
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       38 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.1/README.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1088 2024-01-25 12:48:43.000000 m9s_nereid_base-7.0.1/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       16 2020-03-16 09:24:45.000000 m9s_nereid_base-7.0.1/babel.cfg
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4861 2024-01-24 19:18:39.000000 m9s_nereid_base-7.0.1/configuration.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1458 2024-01-25 11:36:59.000000 m9s_nereid_base-7.0.1/country.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      986 2024-01-24 19:10:30.000000 m9s_nereid_base-7.0.1/currency.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       86 2024-04-25 14:06:28.000000 m9s_nereid_base-7.0.1/dev_requirements.txt
-drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:14:33.892678 m9s_nereid_base-7.0.1/doc/
-drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:14:33.892678 m9s_nereid_base-7.0.1/doc/de/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       37 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.1/doc/de/index.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       38 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.1/doc/index.rst
-drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:14:33.888678 m9s_nereid_base-7.0.1/icons/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      296 2021-02-14 10:44:50.000000 m9s_nereid_base-7.0.1/icons/tryton-media.svg
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      989 2021-02-14 10:44:50.000000 m9s_nereid_base-7.0.1/icons/tryton-web.svg
-drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:14:33.888678 m9s_nereid_base-7.0.1/locale/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    12688 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.1/locale/ca.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    14142 2022-04-12 07:18:45.000000 m9s_nereid_base-7.0.1/locale/de.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    13174 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.1/locale/es.po
-drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:14:33.892678 m9s_nereid_base-7.0.1/m9s_nereid_base.egg-info/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3204 2024-04-25 14:14:33.000000 m9s_nereid_base-7.0.1/m9s_nereid_base.egg-info/PKG-INFO
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2598 2024-04-25 14:14:33.000000 m9s_nereid_base-7.0.1/m9s_nereid_base.egg-info/SOURCES.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2024-04-25 14:14:33.000000 m9s_nereid_base-7.0.1/m9s_nereid_base.egg-info/dependency_links.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       60 2024-04-25 14:14:33.000000 m9s_nereid_base-7.0.1/m9s_nereid_base.egg-info/entry_points.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2024-01-26 11:11:06.000000 m9s_nereid_base-7.0.1/m9s_nereid_base.egg-info/not-zip-safe
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      105 2024-04-25 14:14:33.000000 m9s_nereid_base-7.0.1/m9s_nereid_base.egg-info/requires.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        8 2024-04-25 14:14:33.000000 m9s_nereid_base-7.0.1/m9s_nereid_base.egg-info/top_level.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1311 2022-04-08 10:03:51.000000 m9s_nereid_base-7.0.1/message.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      646 2024-01-24 19:10:30.000000 m9s_nereid_base-7.0.1/model.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    12383 2024-01-26 20:14:57.000000 m9s_nereid_base-7.0.1/party.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3509 2022-03-29 15:04:46.000000 m9s_nereid_base-7.0.1/party.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.1/requirements.txt
--rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)       38 2024-04-25 14:14:33.892678 m9s_nereid_base-7.0.1/setup.cfg
--rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     4466 2024-01-26 19:58:30.000000 m9s_nereid_base-7.0.1/setup.py
--rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     8146 2024-04-25 09:34:16.000000 m9s_nereid_base-7.0.1/static_file.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3259 2022-03-25 09:26:04.000000 m9s_nereid_base-7.0.1/static_file.xml
-drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:14:33.892678 m9s_nereid_base-7.0.1/templates/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        0 2020-03-16 09:24:45.000000 m9s_nereid_base-7.0.1/templates/home.html
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        0 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.1/templates/new-password.jinja
-drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:14:33.892678 m9s_nereid_base-7.0.1/templates/tests/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      129 2020-03-16 09:24:45.000000 m9s_nereid_base-7.0.1/templates/tests/exists-both.html
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       12 2020-03-16 09:24:45.000000 m9s_nereid_base-7.0.1/templates/tests/from-module.html
-drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:14:33.888678 m9s_nereid_base-7.0.1/tests/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      115 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.1/tests/__init__.py
--rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)    14559 2024-04-25 09:39:28.000000 m9s_nereid_base-7.0.1/tests/address.py
--rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)    46720 2024-04-25 09:39:28.000000 m9s_nereid_base-7.0.1/tests/auth.py
--rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     3603 2024-04-25 09:39:28.000000 m9s_nereid_base-7.0.1/tests/common.py
--rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     4865 2024-04-25 09:39:28.000000 m9s_nereid_base-7.0.1/tests/country.py
--rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     5316 2024-04-25 09:39:28.000000 m9s_nereid_base-7.0.1/tests/currency.py
--rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)    10378 2024-04-25 09:39:28.000000 m9s_nereid_base-7.0.1/tests/i18n.py
--rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     9772 2024-04-25 09:39:28.000000 m9s_nereid_base-7.0.1/tests/routing.py
--rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     4442 2024-04-25 09:39:28.000000 m9s_nereid_base-7.0.1/tests/static_file.py
--rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     1011 2024-04-25 09:39:28.000000 m9s_nereid_base-7.0.1/tests/test_module.py
--rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)    14582 2024-04-25 09:39:28.000000 m9s_nereid_base-7.0.1/tests/translation.py
--rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     4390 2024-04-25 09:39:28.000000 m9s_nereid_base-7.0.1/tests/user.py
--rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     1435 2024-04-25 09:39:28.000000 m9s_nereid_base-7.0.1/tests/website.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      595 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.1/tox.ini
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    28638 2024-02-02 10:32:01.000000 m9s_nereid_base-7.0.1/translation.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      442 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.1/translation.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      156 2024-02-02 15:04:04.000000 m9s_nereid_base-7.0.1/tryton.cfg
--rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)    35790 2024-04-25 09:34:16.000000 m9s_nereid_base-7.0.1/user.py
-drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-25 14:14:33.888678 m9s_nereid_base-7.0.1/view/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      366 2022-03-29 15:04:46.000000 m9s_nereid_base-7.0.1/view/contact_mechanism_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      290 2022-03-29 15:04:46.000000 m9s_nereid_base-7.0.1/view/contact_mechanism_tree.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      290 2022-03-29 15:04:46.000000 m9s_nereid_base-7.0.1/view/contact_mechanism_tree_sequence.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      765 2021-05-14 10:34:06.000000 m9s_nereid_base-7.0.1/view/nereid_user_form2.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      265 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.1/view/nereid_user_tree.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      338 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.1/view/party_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      631 2021-03-16 09:13:55.000000 m9s_nereid_base-7.0.1/view/static_file_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      210 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.1/view/static_file_tree.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      459 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.1/view/static_folder_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      182 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.1/view/static_folder_tree.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      367 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.1/view/translation_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1007 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.1/view/website_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      322 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.1/view/website_locale_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      239 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.1/view/website_locale_tree.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      210 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.1/view/website_tree.xml
--rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)    14802 2024-03-28 10:37:04.000000 m9s_nereid_base-7.0.1/website.py
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-05-09 09:32:51.983208 m9s_nereid_base-7.0.2/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       81 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.2/.coveragerc
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1875 2022-02-15 11:09:33.000000 m9s_nereid_base-7.0.2/.drone.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.2/.flake8
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.2/.gitlab-ci-m9s.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2217 2024-04-25 09:39:28.000000 m9s_nereid_base-7.0.2/.gitlab-ci.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.2/.isort.cfg
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-05-09 09:32:51.979208 m9s_nereid_base-7.0.2/.woodpecker/
+-rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     1367 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.2/.woodpecker/mail_curl.sh
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      645 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.2/.woodpecker/report.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1302 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.2/.woodpecker/test.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      862 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.2/COPYRIGHT
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.2/INSTALL
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.2/LICENSE
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      121 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.2/MANIFEST.in
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     3204 2024-05-09 09:32:51.983208 m9s_nereid_base-7.0.2/PKG-INFO
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1042 2024-04-25 14:06:28.000000 m9s_nereid_base-7.0.2/README.md
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       38 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.2/README.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1088 2024-01-25 12:48:43.000000 m9s_nereid_base-7.0.2/__init__.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       16 2020-03-16 09:24:45.000000 m9s_nereid_base-7.0.2/babel.cfg
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4861 2024-01-24 19:18:39.000000 m9s_nereid_base-7.0.2/configuration.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1458 2024-01-25 11:36:59.000000 m9s_nereid_base-7.0.2/country.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      986 2024-01-24 19:10:30.000000 m9s_nereid_base-7.0.2/currency.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       86 2024-04-25 14:06:28.000000 m9s_nereid_base-7.0.2/dev_requirements.txt
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-05-09 09:32:51.979208 m9s_nereid_base-7.0.2/doc/
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-05-09 09:32:51.979208 m9s_nereid_base-7.0.2/doc/de/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       37 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.2/doc/de/index.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       38 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.2/doc/index.rst
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-05-09 09:32:51.971208 m9s_nereid_base-7.0.2/icons/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      296 2021-02-14 10:44:50.000000 m9s_nereid_base-7.0.2/icons/tryton-media.svg
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      989 2021-02-14 10:44:50.000000 m9s_nereid_base-7.0.2/icons/tryton-web.svg
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-05-09 09:32:51.971208 m9s_nereid_base-7.0.2/locale/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    12688 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.2/locale/ca.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    14142 2022-04-12 07:18:45.000000 m9s_nereid_base-7.0.2/locale/de.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    13174 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.2/locale/es.po
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-05-09 09:32:51.979208 m9s_nereid_base-7.0.2/m9s_nereid_base.egg-info/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3204 2024-05-09 09:32:51.000000 m9s_nereid_base-7.0.2/m9s_nereid_base.egg-info/PKG-INFO
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2598 2024-05-09 09:32:51.000000 m9s_nereid_base-7.0.2/m9s_nereid_base.egg-info/SOURCES.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2024-05-09 09:32:51.000000 m9s_nereid_base-7.0.2/m9s_nereid_base.egg-info/dependency_links.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       60 2024-05-09 09:32:51.000000 m9s_nereid_base-7.0.2/m9s_nereid_base.egg-info/entry_points.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2024-01-26 11:11:06.000000 m9s_nereid_base-7.0.2/m9s_nereid_base.egg-info/not-zip-safe
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      105 2024-05-09 09:32:51.000000 m9s_nereid_base-7.0.2/m9s_nereid_base.egg-info/requires.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        8 2024-05-09 09:32:51.000000 m9s_nereid_base-7.0.2/m9s_nereid_base.egg-info/top_level.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1311 2022-04-08 10:03:51.000000 m9s_nereid_base-7.0.2/message.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      646 2024-01-24 19:10:30.000000 m9s_nereid_base-7.0.2/model.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    12383 2024-01-26 20:14:57.000000 m9s_nereid_base-7.0.2/party.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3509 2022-03-29 15:04:46.000000 m9s_nereid_base-7.0.2/party.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.2/requirements.txt
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)       38 2024-05-09 09:32:51.983208 m9s_nereid_base-7.0.2/setup.cfg
+-rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     4466 2024-01-26 19:58:30.000000 m9s_nereid_base-7.0.2/setup.py
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     8172 2024-05-09 09:29:24.000000 m9s_nereid_base-7.0.2/static_file.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3259 2022-03-25 09:26:04.000000 m9s_nereid_base-7.0.2/static_file.xml
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-05-09 09:32:51.983208 m9s_nereid_base-7.0.2/templates/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        0 2020-03-16 09:24:45.000000 m9s_nereid_base-7.0.2/templates/home.html
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        0 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.2/templates/new-password.jinja
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-05-09 09:32:51.983208 m9s_nereid_base-7.0.2/templates/tests/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      129 2020-03-16 09:24:45.000000 m9s_nereid_base-7.0.2/templates/tests/exists-both.html
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       12 2020-03-16 09:24:45.000000 m9s_nereid_base-7.0.2/templates/tests/from-module.html
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-05-09 09:32:51.975208 m9s_nereid_base-7.0.2/tests/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      115 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.2/tests/__init__.py
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)    14559 2024-04-25 09:39:28.000000 m9s_nereid_base-7.0.2/tests/address.py
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)    46720 2024-04-25 09:39:28.000000 m9s_nereid_base-7.0.2/tests/auth.py
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     3603 2024-04-25 09:39:28.000000 m9s_nereid_base-7.0.2/tests/common.py
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     4865 2024-04-25 09:39:28.000000 m9s_nereid_base-7.0.2/tests/country.py
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     5316 2024-04-25 09:39:28.000000 m9s_nereid_base-7.0.2/tests/currency.py
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)    10378 2024-04-25 09:39:28.000000 m9s_nereid_base-7.0.2/tests/i18n.py
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     9772 2024-04-25 09:39:28.000000 m9s_nereid_base-7.0.2/tests/routing.py
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     4442 2024-04-25 09:39:28.000000 m9s_nereid_base-7.0.2/tests/static_file.py
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     1011 2024-04-25 09:39:28.000000 m9s_nereid_base-7.0.2/tests/test_module.py
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)    14582 2024-04-25 09:39:28.000000 m9s_nereid_base-7.0.2/tests/translation.py
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     4390 2024-04-25 09:39:28.000000 m9s_nereid_base-7.0.2/tests/user.py
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     1435 2024-04-25 09:39:28.000000 m9s_nereid_base-7.0.2/tests/website.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      595 2024-01-25 12:46:38.000000 m9s_nereid_base-7.0.2/tox.ini
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    28638 2024-02-02 10:32:01.000000 m9s_nereid_base-7.0.2/translation.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      442 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.2/translation.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      156 2024-04-25 14:14:41.000000 m9s_nereid_base-7.0.2/tryton.cfg
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)    35790 2024-04-25 09:34:16.000000 m9s_nereid_base-7.0.2/user.py
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-05-09 09:32:51.979208 m9s_nereid_base-7.0.2/view/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      366 2022-03-29 15:04:46.000000 m9s_nereid_base-7.0.2/view/contact_mechanism_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      290 2022-03-29 15:04:46.000000 m9s_nereid_base-7.0.2/view/contact_mechanism_tree.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      290 2022-03-29 15:04:46.000000 m9s_nereid_base-7.0.2/view/contact_mechanism_tree_sequence.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      765 2021-05-14 10:34:06.000000 m9s_nereid_base-7.0.2/view/nereid_user_form2.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      265 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.2/view/nereid_user_tree.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      338 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.2/view/party_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      631 2021-03-16 09:13:55.000000 m9s_nereid_base-7.0.2/view/static_file_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      210 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.2/view/static_file_tree.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      459 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.2/view/static_folder_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      182 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.2/view/static_folder_tree.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      367 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.2/view/translation_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1007 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.2/view/website_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      322 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.2/view/website_locale_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      239 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.2/view/website_locale_tree.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      210 2020-03-16 09:24:46.000000 m9s_nereid_base-7.0.2/view/website_tree.xml
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)    14802 2024-03-28 10:37:04.000000 m9s_nereid_base-7.0.2/website.py
```

### Comparing `m9s_nereid_base-7.0.1/.drone.yml` & `m9s_nereid_base-7.0.2/.drone.yml`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.1/.gitlab-ci.yml` & `m9s_nereid_base-7.0.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.1/.woodpecker/mail_curl.sh` & `m9s_nereid_base-7.0.2/.woodpecker/mail_curl.sh`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.1/.woodpecker/report.yml` & `m9s_nereid_base-7.0.2/.woodpecker/report.yml`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.1/.woodpecker/test.yml` & `m9s_nereid_base-7.0.2/.woodpecker/test.yml`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.1/COPYRIGHT` & `m9s_nereid_base-7.0.2/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.1/INSTALL` & `m9s_nereid_base-7.0.2/INSTALL`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.1/LICENSE` & `m9s_nereid_base-7.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.1/PKG-INFO` & `m9s_nereid_base-7.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m9s_nereid_base
-Version: 7.0.1
+Version: 7.0.2
 Summary: Tryton Nereid Base Module
 Home-page: https://www.m9s.biz/
 Download-URL: https://gitlab.com/m9s/nereid_base.git
 Author: MBSolutions
 Author-email: info@m9s.biz
 License: GPL-3
 Project-URL: Bug Tracker, https://support.m9s.biz/
```

### Comparing `m9s_nereid_base-7.0.1/README.md` & `m9s_nereid_base-7.0.2/README.md`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.1/__init__.py` & `m9s_nereid_base-7.0.2/__init__.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.1/configuration.xml` & `m9s_nereid_base-7.0.2/configuration.xml`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.1/country.py` & `m9s_nereid_base-7.0.2/country.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.1/currency.py` & `m9s_nereid_base-7.0.2/currency.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.1/icons/tryton-web.svg` & `m9s_nereid_base-7.0.2/icons/tryton-web.svg`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.1/locale/ca.po` & `m9s_nereid_base-7.0.2/locale/ca.po`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.1/locale/de.po` & `m9s_nereid_base-7.0.2/locale/de.po`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.1/locale/es.po` & `m9s_nereid_base-7.0.2/locale/es.po`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.1/m9s_nereid_base.egg-info/PKG-INFO` & `m9s_nereid_base-7.0.2/m9s_nereid_base.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m9s-nereid-base
-Version: 7.0.1
+Version: 7.0.2
 Summary: Tryton Nereid Base Module
 Home-page: https://www.m9s.biz/
 Download-URL: https://gitlab.com/m9s/nereid_base.git
 Author: MBSolutions
 Author-email: info@m9s.biz
 License: GPL-3
 Project-URL: Bug Tracker, https://support.m9s.biz/
```

### Comparing `m9s_nereid_base-7.0.1/m9s_nereid_base.egg-info/SOURCES.txt` & `m9s_nereid_base-7.0.2/m9s_nereid_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.1/message.xml` & `m9s_nereid_base-7.0.2/message.xml`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.1/model.py` & `m9s_nereid_base-7.0.2/model.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.1/party.py` & `m9s_nereid_base-7.0.2/party.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.1/party.xml` & `m9s_nereid_base-7.0.2/party.xml`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.1/setup.py` & `m9s_nereid_base-7.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.1/static_file.py` & `m9s_nereid_base-7.0.2/static_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,15 +179,16 @@
         Setter for the functional binary field.
 
         :param files: Records
         :param name: Ignored
         :param value: The file buffer
         """
         for static_file in files:
-            static_file._set_file_binary(value)
+            if value:
+                static_file._set_file_binary(value)
 
     def get_file_binary(self, name):
         '''
         Getter for the binary_file field. This fetches the file from the
         file system, coverts it to buffer and returns it.
 
         :param name: Field name
```

### Comparing `m9s_nereid_base-7.0.1/static_file.xml` & `m9s_nereid_base-7.0.2/static_file.xml`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.1/tests/address.py` & `m9s_nereid_base-7.0.2/tests/address.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.1/tests/auth.py` & `m9s_nereid_base-7.0.2/tests/auth.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.1/tests/common.py` & `m9s_nereid_base-7.0.2/tests/common.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.1/tests/country.py` & `m9s_nereid_base-7.0.2/tests/country.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.1/tests/currency.py` & `m9s_nereid_base-7.0.2/tests/currency.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.1/tests/i18n.py` & `m9s_nereid_base-7.0.2/tests/i18n.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.1/tests/routing.py` & `m9s_nereid_base-7.0.2/tests/routing.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.1/tests/static_file.py` & `m9s_nereid_base-7.0.2/tests/static_file.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.1/tests/test_module.py` & `m9s_nereid_base-7.0.2/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.1/tests/translation.py` & `m9s_nereid_base-7.0.2/tests/translation.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.1/tests/user.py` & `m9s_nereid_base-7.0.2/tests/user.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.1/tests/website.py` & `m9s_nereid_base-7.0.2/tests/website.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.1/tox.ini` & `m9s_nereid_base-7.0.2/tox.ini`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.1/translation.py` & `m9s_nereid_base-7.0.2/translation.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.1/user.py` & `m9s_nereid_base-7.0.2/user.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.1/view/nereid_user_form2.xml` & `m9s_nereid_base-7.0.2/view/nereid_user_form2.xml`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.1/view/static_file_form.xml` & `m9s_nereid_base-7.0.2/view/static_file_form.xml`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.1/view/website_form.xml` & `m9s_nereid_base-7.0.2/view/website_form.xml`

 * *Files identical despite different names*

### Comparing `m9s_nereid_base-7.0.1/website.py` & `m9s_nereid_base-7.0.2/website.py`

 * *Files identical despite different names*

