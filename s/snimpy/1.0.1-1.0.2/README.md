# Comparing `tmp/snimpy-1.0.1.tar.gz` & `tmp/snimpy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snimpy-1.0.1.tar", last modified: Fri Jun 30 06:51:27 2023, max compression
+gzip compressed data, was "snimpy-1.0.2.tar", last modified: Tue Dec 12 08:28:02 2023, max compression
```

## Comparing `snimpy-1.0.1.tar` & `snimpy-1.0.2.tar`

### file list

```diff
@@ -1,89 +1,90 @@
-drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-06-30 06:51:27.635898 snimpy-1.0.1/
-drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-06-30 06:51:27.631898 snimpy-1.0.1/.github/
--rw-r--r--   0 bernat     (500) users      (100)      157 2022-12-02 17:49:39.000000 snimpy-1.0.1/.github/dependabot.yml
-drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-06-30 06:51:27.631898 snimpy-1.0.1/.github/workflows/
--rw-r--r--   0 bernat     (500) users      (100)     1399 2023-06-24 22:17:32.000000 snimpy-1.0.1/.github/workflows/tests.yml
--rw-r--r--   0 bernat     (500) users      (100)      189 2022-12-14 10:15:32.000000 snimpy-1.0.1/.gitignore
--rw-r--r--   0 bernat     (500) users      (100)      108 2016-11-15 06:58:49.000000 snimpy-1.0.1/.gitmodules
--rw-r--r--   0 bernat     (500) users      (100)      132 2016-11-15 06:58:49.000000 snimpy-1.0.1/AUTHORS.rst
--rw-r--r--   0 bernat     (500) users      (100)     3089 2021-10-22 06:02:08.000000 snimpy-1.0.1/CONTRIBUTING.rst
--rw-r--r--   0 bernat     (500) users      (100)     3690 2023-06-30 06:47:54.000000 snimpy-1.0.1/HISTORY.rst
--rw-r--r--   0 bernat     (500) users      (100)      437 2016-11-15 06:58:49.000000 snimpy-1.0.1/MANIFEST.in
--rw-r--r--   0 bernat     (500) users      (100)     1474 2021-10-22 06:02:08.000000 snimpy-1.0.1/Makefile
--rw-r--r--   0 bernat     (500) users      (100)     6264 2023-06-30 06:51:27.635898 snimpy-1.0.1/PKG-INFO
--rw-r--r--   0 bernat     (500) users      (100)     1945 2021-05-29 15:40:24.000000 snimpy-1.0.1/README.rst
-drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-06-30 06:51:27.631898 snimpy-1.0.1/docs/
--rw-r--r--   0 bernat     (500) users      (100)     6777 2016-11-15 06:58:49.000000 snimpy-1.0.1/docs/Makefile
-drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-06-30 06:51:27.631898 snimpy-1.0.1/docs/_static/
--rw-r--r--   0 bernat     (500) users      (100)    12067 2016-11-15 06:58:49.000000 snimpy-1.0.1/docs/_static/snimpy.svg
-drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-06-30 06:51:27.631898 snimpy-1.0.1/docs/_themes/
--rw-r--r--   0 bernat     (500) users      (100)       22 2014-01-31 18:44:32.000000 snimpy-1.0.1/docs/_themes/.gitignore
--rw-r--r--   0 bernat     (500) users      (100)     1789 2014-01-31 18:44:32.000000 snimpy-1.0.1/docs/_themes/LICENSE
--rw-r--r--   0 bernat     (500) users      (100)     1093 2014-01-31 18:44:32.000000 snimpy-1.0.1/docs/_themes/README
-drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-06-30 06:51:27.631898 snimpy-1.0.1/docs/_themes/flask/
--rw-r--r--   0 bernat     (500) users      (100)      693 2014-01-31 18:45:14.000000 snimpy-1.0.1/docs/_themes/flask/layout.html
--rw-r--r--   0 bernat     (500) users      (100)      590 2014-01-31 18:45:14.000000 snimpy-1.0.1/docs/_themes/flask/relations.html
-drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-06-30 06:51:27.631898 snimpy-1.0.1/docs/_themes/flask/static/
--rw-r--r--   0 bernat     (500) users      (100)     9062 2014-01-31 18:45:16.000000 snimpy-1.0.1/docs/_themes/flask/static/flasky.css_t
--rw-r--r--   0 bernat     (500) users      (100)      164 2014-01-31 18:45:14.000000 snimpy-1.0.1/docs/_themes/flask/theme.conf
-drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-06-30 06:51:27.631898 snimpy-1.0.1/docs/_themes/flask_small/
--rw-r--r--   0 bernat     (500) users      (100)      683 2014-01-31 18:45:14.000000 snimpy-1.0.1/docs/_themes/flask_small/layout.html
-drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-06-30 06:51:27.631898 snimpy-1.0.1/docs/_themes/flask_small/static/
--rw-r--r--   0 bernat     (500) users      (100)     4609 2014-01-31 18:45:16.000000 snimpy-1.0.1/docs/_themes/flask_small/static/flasky.css_t
--rw-r--r--   0 bernat     (500) users      (100)      184 2014-01-31 18:45:14.000000 snimpy-1.0.1/docs/_themes/flask_small/theme.conf
--rw-r--r--   0 bernat     (500) users      (100)     3905 2023-06-30 06:50:57.000000 snimpy-1.0.1/docs/_themes/flask_theme_support.py
--rw-r--r--   0 bernat     (500) users      (100)      797 2016-11-15 06:58:49.000000 snimpy-1.0.1/docs/api.rst
--rwxr-xr-x   0 bernat     (500) users      (100)     1216 2023-06-30 06:51:10.000000 snimpy-1.0.1/docs/conf.py
--rw-r--r--   0 bernat     (500) users      (100)       32 2016-11-15 06:58:49.000000 snimpy-1.0.1/docs/contributing.rst
--rw-r--r--   0 bernat     (500) users      (100)       27 2016-11-15 06:58:49.000000 snimpy-1.0.1/docs/history.rst
--rw-r--r--   0 bernat     (500) users      (100)     2372 2023-06-27 20:20:26.000000 snimpy-1.0.1/docs/index.rst
--rw-r--r--   0 bernat     (500) users      (100)     1043 2016-11-15 06:58:49.000000 snimpy-1.0.1/docs/installation.rst
--rw-r--r--   0 bernat     (500) users      (100)      997 2016-11-15 06:58:49.000000 snimpy-1.0.1/docs/license.rst
--rw-r--r--   0 bernat     (500) users      (100)     6814 2021-04-09 20:14:39.000000 snimpy-1.0.1/docs/usage.rst
-drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-06-30 06:51:27.631898 snimpy-1.0.1/examples/
--rw-r--r--   0 bernat     (500) users      (100)     1234 2023-06-30 06:51:10.000000 snimpy-1.0.1/examples/add-vlan.py
--rw-r--r--   0 bernat     (500) users      (100)      531 2023-06-30 06:51:10.000000 snimpy-1.0.1/examples/disable-port-ingress-filtering.py
--rw-r--r--   0 bernat     (500) users      (100)     1769 2023-06-30 06:51:10.000000 snimpy-1.0.1/examples/enable-lldp.py
--rw-r--r--   0 bernat     (500) users      (100)      909 2023-06-30 06:51:10.000000 snimpy-1.0.1/examples/get-serial.py
--rw-r--r--   0 bernat     (500) users      (100)      114 2023-06-30 06:51:10.000000 snimpy-1.0.1/examples/list-interfaces.py
--rw-r--r--   0 bernat     (500) users      (100)      620 2023-06-30 06:51:10.000000 snimpy-1.0.1/examples/list-routes.py
--rw-r--r--   0 bernat     (500) users      (100)      585 2023-06-30 06:51:10.000000 snimpy-1.0.1/examples/rename-vlan.py
--rwxr-xr-x   0 bernat     (500) users      (100)     2178 2023-06-24 22:17:32.000000 snimpy-1.0.1/examples/set-syslog-ntp.py
--rw-r--r--   0 bernat     (500) users      (100)      630 2023-06-30 06:51:10.000000 snimpy-1.0.1/examples/vlan-and-interfaces.py
--rw-r--r--   0 bernat     (500) users      (100)      966 2022-12-14 10:01:45.000000 snimpy-1.0.1/flake.lock
--rw-r--r--   0 bernat     (500) users      (100)     1196 2023-06-27 20:38:13.000000 snimpy-1.0.1/flake.nix
-drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-06-30 06:51:27.635898 snimpy-1.0.1/man/
--rw-r--r--   0 bernat     (500) users      (100)     1015 2016-11-15 06:58:49.000000 snimpy-1.0.1/man/snimpy.1
--rw-r--r--   0 bernat     (500) users      (100)       38 2023-06-30 06:51:27.635898 snimpy-1.0.1/setup.cfg
--rw-r--r--   0 bernat     (500) users      (100)     2140 2023-06-30 06:51:10.000000 snimpy-1.0.1/setup.py
-drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-06-30 06:51:27.635898 snimpy-1.0.1/snimpy/
--rw-r--r--   0 bernat     (500) users      (100)      197 2023-06-30 06:51:10.000000 snimpy-1.0.1/snimpy/__init__.py
--rw-r--r--   0 bernat     (500) users      (100)      905 2023-06-30 06:51:10.000000 snimpy-1.0.1/snimpy/__main__.py
--rw-r--r--   0 bernat     (500) users      (100)      132 2023-06-30 06:51:27.000000 snimpy-1.0.1/snimpy/_version.py
--rw-r--r--   0 bernat     (500) users      (100)    29843 2023-06-30 06:51:10.000000 snimpy-1.0.1/snimpy/basictypes.py
--rw-r--r--   0 bernat     (500) users      (100)     1781 2023-06-30 06:51:10.000000 snimpy-1.0.1/snimpy/config.py
--rw-r--r--   0 bernat     (500) users      (100)     5810 2023-06-30 06:51:10.000000 snimpy-1.0.1/snimpy/main.py
--rw-r--r--   0 bernat     (500) users      (100)    20966 2023-06-30 06:51:10.000000 snimpy-1.0.1/snimpy/manager.py
--rw-r--r--   0 bernat     (500) users      (100)    23776 2023-06-30 06:51:10.000000 snimpy-1.0.1/snimpy/mib.py
--rw-r--r--   0 bernat     (500) users      (100)     5210 2023-06-30 06:51:10.000000 snimpy-1.0.1/snimpy/smi_build.py
--rw-r--r--   0 bernat     (500) users      (100)    16256 2023-06-30 06:51:10.000000 snimpy-1.0.1/snimpy/snmp.py
-drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-06-30 06:51:27.635898 snimpy-1.0.1/snimpy.egg-info/
--rw-r--r--   0 bernat     (500) users      (100)     6264 2023-06-30 06:51:27.000000 snimpy-1.0.1/snimpy.egg-info/PKG-INFO
--rw-r--r--   0 bernat     (500) users      (100)     1555 2023-06-30 06:51:27.000000 snimpy-1.0.1/snimpy.egg-info/SOURCES.txt
--rw-r--r--   0 bernat     (500) users      (100)        1 2023-06-30 06:51:27.000000 snimpy-1.0.1/snimpy.egg-info/dependency_links.txt
--rw-r--r--   0 bernat     (500) users      (100)       48 2023-06-30 06:51:27.000000 snimpy-1.0.1/snimpy.egg-info/entry_points.txt
--rw-r--r--   0 bernat     (500) users      (100)        1 2015-11-14 17:00:37.000000 snimpy-1.0.1/snimpy.egg-info/not-zip-safe
--rw-r--r--   0 bernat     (500) users      (100)       42 2023-06-30 06:51:27.000000 snimpy-1.0.1/snimpy.egg-info/requires.txt
--rw-r--r--   0 bernat     (500) users      (100)        7 2023-06-30 06:51:27.000000 snimpy-1.0.1/snimpy.egg-info/top_level.txt
-drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-06-30 06:51:27.635898 snimpy-1.0.1/tests/
--rw-r--r--   0 bernat     (500) users      (100)      624 2016-11-15 06:58:49.000000 snimpy-1.0.1/tests/SNIMPY-INVALID-MIB.mib
--rw-r--r--   0 bernat     (500) users      (100)    13822 2017-12-16 13:48:00.000000 snimpy-1.0.1/tests/SNIMPY-MIB.mib
--rw-r--r--   0 bernat     (500) users      (100)    18561 2023-06-30 06:51:10.000000 snimpy-1.0.1/tests/agent.py
--rw-r--r--   0 bernat     (500) users      (100)    26698 2023-06-30 06:51:10.000000 snimpy-1.0.1/tests/test_basictypes.py
--rw-r--r--   0 bernat     (500) users      (100)     1238 2023-06-30 06:51:10.000000 snimpy-1.0.1/tests/test_conf.py
--rw-r--r--   0 bernat     (500) users      (100)     1149 2023-06-30 06:51:10.000000 snimpy-1.0.1/tests/test_main.py
--rw-r--r--   0 bernat     (500) users      (100)    20324 2023-06-30 06:51:10.000000 snimpy-1.0.1/tests/test_manager.py
--rw-r--r--   0 bernat     (500) users      (100)    18875 2023-06-30 06:51:10.000000 snimpy-1.0.1/tests/test_mib.py
--rw-r--r--   0 bernat     (500) users      (100)    15585 2023-06-30 06:51:10.000000 snimpy-1.0.1/tests/test_snmp.py
--rw-r--r--   0 bernat     (500) users      (100)      744 2023-06-27 20:38:04.000000 snimpy-1.0.1/tox.ini
--rw-r--r--   0 bernat     (500) users      (100)       21 2023-06-30 06:51:27.000000 snimpy-1.0.1/version.txt
+drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-12-12 08:28:02.394754 snimpy-1.0.2/
+drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-12-12 08:28:02.390754 snimpy-1.0.2/.github/
+-rw-r--r--   0 bernat     (500) users      (100)       77 2023-07-02 15:55:20.000000 snimpy-1.0.2/.github/FUNDING.yml
+-rw-r--r--   0 bernat     (500) users      (100)      157 2022-12-02 17:49:39.000000 snimpy-1.0.2/.github/dependabot.yml
+drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-12-12 08:28:02.390754 snimpy-1.0.2/.github/workflows/
+-rw-r--r--   0 bernat     (500) users      (100)     1470 2023-11-01 12:54:09.000000 snimpy-1.0.2/.github/workflows/tests.yml
+-rw-r--r--   0 bernat     (500) users      (100)      189 2022-12-14 10:15:32.000000 snimpy-1.0.2/.gitignore
+-rw-r--r--   0 bernat     (500) users      (100)      108 2016-11-15 06:58:49.000000 snimpy-1.0.2/.gitmodules
+-rw-r--r--   0 bernat     (500) users      (100)      132 2016-11-15 06:58:49.000000 snimpy-1.0.2/AUTHORS.rst
+-rw-r--r--   0 bernat     (500) users      (100)     3089 2021-10-22 06:02:08.000000 snimpy-1.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 bernat     (500) users      (100)     3799 2023-12-12 08:27:40.000000 snimpy-1.0.2/HISTORY.rst
+-rw-r--r--   0 bernat     (500) users      (100)      437 2016-11-15 06:58:49.000000 snimpy-1.0.2/MANIFEST.in
+-rw-r--r--   0 bernat     (500) users      (100)     1474 2021-10-22 06:02:08.000000 snimpy-1.0.2/Makefile
+-rw-r--r--   0 bernat     (500) users      (100)     6373 2023-12-12 08:28:02.394754 snimpy-1.0.2/PKG-INFO
+-rw-r--r--   0 bernat     (500) users      (100)     1945 2021-05-29 15:40:24.000000 snimpy-1.0.2/README.rst
+drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-12-12 08:28:02.390754 snimpy-1.0.2/docs/
+-rw-r--r--   0 bernat     (500) users      (100)     6777 2016-11-15 06:58:49.000000 snimpy-1.0.2/docs/Makefile
+drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-12-12 08:28:02.390754 snimpy-1.0.2/docs/_static/
+-rw-r--r--   0 bernat     (500) users      (100)    12067 2016-11-15 06:58:49.000000 snimpy-1.0.2/docs/_static/snimpy.svg
+drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-12-12 08:28:02.390754 snimpy-1.0.2/docs/_themes/
+-rw-r--r--   0 bernat     (500) users      (100)       22 2014-01-31 18:44:32.000000 snimpy-1.0.2/docs/_themes/.gitignore
+-rw-r--r--   0 bernat     (500) users      (100)     1789 2014-01-31 18:44:32.000000 snimpy-1.0.2/docs/_themes/LICENSE
+-rw-r--r--   0 bernat     (500) users      (100)     1093 2014-01-31 18:44:32.000000 snimpy-1.0.2/docs/_themes/README
+drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-12-12 08:28:02.390754 snimpy-1.0.2/docs/_themes/flask/
+-rw-r--r--   0 bernat     (500) users      (100)      693 2014-01-31 18:45:14.000000 snimpy-1.0.2/docs/_themes/flask/layout.html
+-rw-r--r--   0 bernat     (500) users      (100)      590 2014-01-31 18:45:14.000000 snimpy-1.0.2/docs/_themes/flask/relations.html
+drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-12-12 08:28:02.390754 snimpy-1.0.2/docs/_themes/flask/static/
+-rw-r--r--   0 bernat     (500) users      (100)     9062 2014-01-31 18:45:16.000000 snimpy-1.0.2/docs/_themes/flask/static/flasky.css_t
+-rw-r--r--   0 bernat     (500) users      (100)      164 2014-01-31 18:45:14.000000 snimpy-1.0.2/docs/_themes/flask/theme.conf
+drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-12-12 08:28:02.390754 snimpy-1.0.2/docs/_themes/flask_small/
+-rw-r--r--   0 bernat     (500) users      (100)      683 2014-01-31 18:45:14.000000 snimpy-1.0.2/docs/_themes/flask_small/layout.html
+drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-12-12 08:28:02.390754 snimpy-1.0.2/docs/_themes/flask_small/static/
+-rw-r--r--   0 bernat     (500) users      (100)     4609 2014-01-31 18:45:16.000000 snimpy-1.0.2/docs/_themes/flask_small/static/flasky.css_t
+-rw-r--r--   0 bernat     (500) users      (100)      184 2014-01-31 18:45:14.000000 snimpy-1.0.2/docs/_themes/flask_small/theme.conf
+-rw-r--r--   0 bernat     (500) users      (100)     4875 2023-06-30 06:56:02.000000 snimpy-1.0.2/docs/_themes/flask_theme_support.py
+-rw-r--r--   0 bernat     (500) users      (100)      797 2016-11-15 06:58:49.000000 snimpy-1.0.2/docs/api.rst
+-rwxr-xr-x   0 bernat     (500) users      (100)     1216 2023-06-30 06:51:10.000000 snimpy-1.0.2/docs/conf.py
+-rw-r--r--   0 bernat     (500) users      (100)       32 2016-11-15 06:58:49.000000 snimpy-1.0.2/docs/contributing.rst
+-rw-r--r--   0 bernat     (500) users      (100)       27 2016-11-15 06:58:49.000000 snimpy-1.0.2/docs/history.rst
+-rw-r--r--   0 bernat     (500) users      (100)     2372 2023-06-27 20:20:26.000000 snimpy-1.0.2/docs/index.rst
+-rw-r--r--   0 bernat     (500) users      (100)     1209 2023-11-01 13:06:33.000000 snimpy-1.0.2/docs/installation.rst
+-rw-r--r--   0 bernat     (500) users      (100)      997 2016-11-15 06:58:49.000000 snimpy-1.0.2/docs/license.rst
+-rw-r--r--   0 bernat     (500) users      (100)     6814 2021-04-09 20:14:39.000000 snimpy-1.0.2/docs/usage.rst
+drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-12-12 08:28:02.390754 snimpy-1.0.2/examples/
+-rw-r--r--   0 bernat     (500) users      (100)     1234 2023-06-30 06:51:10.000000 snimpy-1.0.2/examples/add-vlan.py
+-rw-r--r--   0 bernat     (500) users      (100)      531 2023-06-30 06:51:10.000000 snimpy-1.0.2/examples/disable-port-ingress-filtering.py
+-rw-r--r--   0 bernat     (500) users      (100)     1769 2023-06-30 06:51:10.000000 snimpy-1.0.2/examples/enable-lldp.py
+-rw-r--r--   0 bernat     (500) users      (100)      909 2023-06-30 06:51:10.000000 snimpy-1.0.2/examples/get-serial.py
+-rw-r--r--   0 bernat     (500) users      (100)      114 2023-06-30 06:51:10.000000 snimpy-1.0.2/examples/list-interfaces.py
+-rw-r--r--   0 bernat     (500) users      (100)      620 2023-06-30 06:51:10.000000 snimpy-1.0.2/examples/list-routes.py
+-rw-r--r--   0 bernat     (500) users      (100)      585 2023-06-30 06:51:10.000000 snimpy-1.0.2/examples/rename-vlan.py
+-rwxr-xr-x   0 bernat     (500) users      (100)     2178 2023-06-24 22:17:32.000000 snimpy-1.0.2/examples/set-syslog-ntp.py
+-rw-r--r--   0 bernat     (500) users      (100)      630 2023-06-30 06:51:10.000000 snimpy-1.0.2/examples/vlan-and-interfaces.py
+-rw-r--r--   0 bernat     (500) users      (100)      966 2022-12-14 10:01:45.000000 snimpy-1.0.2/flake.lock
+-rw-r--r--   0 bernat     (500) users      (100)     1196 2023-06-27 20:38:13.000000 snimpy-1.0.2/flake.nix
+drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-12-12 08:28:02.394754 snimpy-1.0.2/man/
+-rw-r--r--   0 bernat     (500) users      (100)     1015 2016-11-15 06:58:49.000000 snimpy-1.0.2/man/snimpy.1
+-rw-r--r--   0 bernat     (500) users      (100)       38 2023-12-12 08:28:02.394754 snimpy-1.0.2/setup.cfg
+-rw-r--r--   0 bernat     (500) users      (100)     2152 2023-11-01 12:53:27.000000 snimpy-1.0.2/setup.py
+drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-12-12 08:28:02.394754 snimpy-1.0.2/snimpy/
+-rw-r--r--   0 bernat     (500) users      (100)      197 2023-06-30 06:51:10.000000 snimpy-1.0.2/snimpy/__init__.py
+-rw-r--r--   0 bernat     (500) users      (100)      905 2023-06-30 06:51:10.000000 snimpy-1.0.2/snimpy/__main__.py
+-rw-r--r--   0 bernat     (500) users      (100)      132 2023-12-12 08:28:02.000000 snimpy-1.0.2/snimpy/_version.py
+-rw-r--r--   0 bernat     (500) users      (100)    29843 2023-06-30 06:51:10.000000 snimpy-1.0.2/snimpy/basictypes.py
+-rw-r--r--   0 bernat     (500) users      (100)     1781 2023-06-30 06:51:10.000000 snimpy-1.0.2/snimpy/config.py
+-rw-r--r--   0 bernat     (500) users      (100)     5810 2023-06-30 06:51:10.000000 snimpy-1.0.2/snimpy/main.py
+-rw-r--r--   0 bernat     (500) users      (100)    20966 2023-06-30 06:51:10.000000 snimpy-1.0.2/snimpy/manager.py
+-rw-r--r--   0 bernat     (500) users      (100)    23776 2023-06-30 06:51:10.000000 snimpy-1.0.2/snimpy/mib.py
+-rw-r--r--   0 bernat     (500) users      (100)     5210 2023-06-30 06:51:10.000000 snimpy-1.0.2/snimpy/smi_build.py
+-rw-r--r--   0 bernat     (500) users      (100)    16256 2023-06-30 06:51:10.000000 snimpy-1.0.2/snimpy/snmp.py
+drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-12-12 08:28:02.394754 snimpy-1.0.2/snimpy.egg-info/
+-rw-r--r--   0 bernat     (500) users      (100)     6373 2023-12-12 08:28:02.000000 snimpy-1.0.2/snimpy.egg-info/PKG-INFO
+-rw-r--r--   0 bernat     (500) users      (100)     1575 2023-12-12 08:28:02.000000 snimpy-1.0.2/snimpy.egg-info/SOURCES.txt
+-rw-r--r--   0 bernat     (500) users      (100)        1 2023-12-12 08:28:02.000000 snimpy-1.0.2/snimpy.egg-info/dependency_links.txt
+-rw-r--r--   0 bernat     (500) users      (100)       48 2023-12-12 08:28:02.000000 snimpy-1.0.2/snimpy.egg-info/entry_points.txt
+-rw-r--r--   0 bernat     (500) users      (100)        1 2015-11-14 17:00:37.000000 snimpy-1.0.2/snimpy.egg-info/not-zip-safe
+-rw-r--r--   0 bernat     (500) users      (100)       82 2023-12-12 08:28:02.000000 snimpy-1.0.2/snimpy.egg-info/requires.txt
+-rw-r--r--   0 bernat     (500) users      (100)        7 2023-12-12 08:28:02.000000 snimpy-1.0.2/snimpy.egg-info/top_level.txt
+drwxr-xr-x   0 bernat     (500) users      (100)        0 2023-12-12 08:28:02.394754 snimpy-1.0.2/tests/
+-rw-r--r--   0 bernat     (500) users      (100)      624 2016-11-15 06:58:49.000000 snimpy-1.0.2/tests/SNIMPY-INVALID-MIB.mib
+-rw-r--r--   0 bernat     (500) users      (100)    13822 2017-12-16 13:48:00.000000 snimpy-1.0.2/tests/SNIMPY-MIB.mib
+-rw-r--r--   0 bernat     (500) users      (100)    18560 2023-12-02 18:08:36.000000 snimpy-1.0.2/tests/agent.py
+-rw-r--r--   0 bernat     (500) users      (100)    26698 2023-06-30 06:51:10.000000 snimpy-1.0.2/tests/test_basictypes.py
+-rw-r--r--   0 bernat     (500) users      (100)     1238 2023-06-30 06:51:10.000000 snimpy-1.0.2/tests/test_conf.py
+-rw-r--r--   0 bernat     (500) users      (100)     1149 2023-06-30 06:51:10.000000 snimpy-1.0.2/tests/test_main.py
+-rw-r--r--   0 bernat     (500) users      (100)    20324 2023-06-30 06:51:10.000000 snimpy-1.0.2/tests/test_manager.py
+-rw-r--r--   0 bernat     (500) users      (100)    18875 2023-06-30 06:51:10.000000 snimpy-1.0.2/tests/test_mib.py
+-rw-r--r--   0 bernat     (500) users      (100)    15585 2023-06-30 06:51:10.000000 snimpy-1.0.2/tests/test_snmp.py
+-rw-r--r--   0 bernat     (500) users      (100)      762 2023-11-01 12:47:41.000000 snimpy-1.0.2/tox.ini
+-rw-r--r--   0 bernat     (500) users      (100)       21 2023-12-12 08:28:02.000000 snimpy-1.0.2/version.txt
```

### Comparing `snimpy-1.0.1/.github/workflows/tests.yml` & `snimpy-1.0.2/.github/workflows/tests.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+---
 name: Tests
 on:
   push:
     branches:
       - master
     tags:
       - "*.*"
@@ -9,25 +10,28 @@
   schedule:
     - cron: 30 7 2 * *
 jobs:
   tests:
     name: Run tests
     runs-on: ubuntu-latest
     strategy:
+      fail-fast: false
       matrix:
         python-version:
           - 3.7
           - 3.8
           - 3.9
           - "3.10"
           - "3.11"
+          - "3.12"
     steps:
-      - uses: actions/checkout@v1
+      - uses: actions/checkout@v4
         with:
           submodules: true
+          fetch-depth: 0
       - name: Setup Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install non-Python dependencies
         run: >
           sudo apt -qy update;
```

### Comparing `snimpy-1.0.1/CONTRIBUTING.rst` & `snimpy-1.0.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/HISTORY.rst` & `snimpy-1.0.2/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 .. :changelog:
 
 History
 -------
 
+1.0.2 (2023-12-12)
+++++++++++++++++++
+
+* Compatibility with Python 3.12 by adding dependency to pyasyncore.
+
 1.0.1 (2023-06-30)
 ++++++++++++++++++
 
 * Switch to pysnmp-lextudio, a maintained fork of PySNMP.
 
 1.0.0 (2021-05-29)
 ++++++++++++++++++
```

### Comparing `snimpy-1.0.1/Makefile` & `snimpy-1.0.2/Makefile`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/PKG-INFO` & `snimpy-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snimpy
-Version: 1.0.1
+Version: 1.0.2
 Summary: interactive SNMP tool
 Home-page: https://github.com/vincentbernat/snimpy
 Author: Vincent Bernat
 Author-email: bernat@luffy.cx
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
@@ -79,14 +79,19 @@
 
 
 
 
 History
 -------
 
+1.0.2 (2023-12-12)
+++++++++++++++++++
+
+* Compatibility with Python 3.12 by adding dependency to pyasyncore.
+
 1.0.1 (2023-06-30)
 ++++++++++++++++++
 
 * Switch to pysnmp-lextudio, a maintained fork of PySNMP.
 
 1.0.0 (2021-05-29)
 ++++++++++++++++++
```

### Comparing `snimpy-1.0.1/README.rst` & `snimpy-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/docs/Makefile` & `snimpy-1.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/docs/_static/snimpy.svg` & `snimpy-1.0.2/docs/_static/snimpy.svg`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/docs/_themes/LICENSE` & `snimpy-1.0.2/docs/_themes/LICENSE`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/docs/_themes/README` & `snimpy-1.0.2/docs/_themes/README`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/docs/_themes/flask/layout.html` & `snimpy-1.0.2/docs/_themes/flask/layout.html`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/docs/_themes/flask/relations.html` & `snimpy-1.0.2/docs/_themes/flask/relations.html`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/docs/_themes/flask/static/flasky.css_t` & `snimpy-1.0.2/docs/_themes/flask/static/flasky.css_t`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/docs/_themes/flask_small/layout.html` & `snimpy-1.0.2/docs/_themes/flask_small/layout.html`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/docs/_themes/flask_small/static/flasky.css_t` & `snimpy-1.0.2/docs/_themes/flask_small/static/flasky.css_t`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/docs/_themes/flask_theme_support.py` & `snimpy-1.0.2/docs/_themes/flask_theme_support.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,89 +1,86 @@
 # flasky extensions.  flasky pygments style based on tango style
 from pygments.style import Style
-from pygments.token import (
-    Keyword,
-    Name,
-    Comment,
-    String,
-    Error,
-    Number,
-    Operator,
-    Generic,
-    Whitespace,
-    Punctuation,
-    Other,
-    Literal,
-)
+from pygments.token import Keyword, Name, Comment, String, Error, \
+     Number, Operator, Generic, Whitespace, Punctuation, Other, Literal
 
 
 class FlaskyStyle(Style):
     background_color = "#f8f8f8"
     default_style = ""
 
     styles = {
         # No corresponding class for the following:
-        # Text:                     "", # class:  ''
-        Whitespace: "underline #f8f8f8",  # class: 'w'
-        Error: "#a40000 border:#ef2929",  # class: 'err'
-        Other: "#000000",  # class 'x'
-        Comment: "italic #8f5902",  # class: 'c'
-        Comment.Preproc: "noitalic",  # class: 'cp'
-        Keyword: "bold #004461",  # class: 'k'
-        Keyword.Constant: "bold #004461",  # class: 'kc'
-        Keyword.Declaration: "bold #004461",  # class: 'kd'
-        Keyword.Namespace: "bold #004461",  # class: 'kn'
-        Keyword.Pseudo: "bold #004461",  # class: 'kp'
-        Keyword.Reserved: "bold #004461",  # class: 'kr'
-        Keyword.Type: "bold #004461",  # class: 'kt'
-        Operator: "#582800",  # class: 'o'
-        Operator.Word: "bold #004461",  # class: 'ow' - like keywords
-        Punctuation: "bold #000000",  # class: 'p'
+        #Text:                     "", # class:  ''
+        Whitespace:                "underline #f8f8f8",      # class: 'w'
+        Error:                     "#a40000 border:#ef2929", # class: 'err'
+        Other:                     "#000000",                # class 'x'
+
+        Comment:                   "italic #8f5902", # class: 'c'
+        Comment.Preproc:           "noitalic",       # class: 'cp'
+
+        Keyword:                   "bold #004461",   # class: 'k'
+        Keyword.Constant:          "bold #004461",   # class: 'kc'
+        Keyword.Declaration:       "bold #004461",   # class: 'kd'
+        Keyword.Namespace:         "bold #004461",   # class: 'kn'
+        Keyword.Pseudo:            "bold #004461",   # class: 'kp'
+        Keyword.Reserved:          "bold #004461",   # class: 'kr'
+        Keyword.Type:              "bold #004461",   # class: 'kt'
+
+        Operator:                  "#582800",   # class: 'o'
+        Operator.Word:             "bold #004461",   # class: 'ow' - like keywords
+
+        Punctuation:               "bold #000000",   # class: 'p'
+
         # because special names such as Name.Class, Name.Function, etc.
         # are not recognized as such later in the parsing, we choose them
         # to look the same as ordinary variables.
-        Name: "#000000",  # class: 'n'
-        Name.Attribute: "#c4a000",  # class: 'na' - to be revised
-        Name.Builtin: "#004461",  # class: 'nb'
-        Name.Builtin.Pseudo: "#3465a4",  # class: 'bp'
-        Name.Class: "#000000",  # class: 'nc' - to be revised
-        Name.Constant: "#000000",  # class: 'no' - to be revised
-        Name.Decorator: "#888",  # class: 'nd' - to be revised
-        Name.Entity: "#ce5c00",  # class: 'ni'
-        Name.Exception: "bold #cc0000",  # class: 'ne'
-        Name.Function: "#000000",  # class: 'nf'
-        Name.Property: "#000000",  # class: 'py'
-        Name.Label: "#f57900",  # class: 'nl'
-        Name.Namespace: "#000000",  # class: 'nn' - to be revised
-        Name.Other: "#000000",  # class: 'nx'
-        Name.Tag: "bold #004461",  # class: 'nt' - like a keyword
-        Name.Variable: "#000000",  # class: 'nv' - to be revised
-        Name.Variable.Class: "#000000",  # class: 'vc' - to be revised
-        Name.Variable.Global: "#000000",  # class: 'vg' - to be revised
-        Name.Variable.Instance: "#000000",  # class: 'vi' - to be revised
-        Number: "#990000",  # class: 'm'
-        Literal: "#000000",  # class: 'l'
-        Literal.Date: "#000000",  # class: 'ld'
-        String: "#4e9a06",  # class: 's'
-        String.Backtick: "#4e9a06",  # class: 'sb'
-        String.Char: "#4e9a06",  # class: 'sc'
-        String.Doc: "italic #8f5902",  # class: 'sd' - like a comment
-        String.Double: "#4e9a06",  # class: 's2'
-        String.Escape: "#4e9a06",  # class: 'se'
-        String.Heredoc: "#4e9a06",  # class: 'sh'
-        String.Interpol: "#4e9a06",  # class: 'si'
-        String.Other: "#4e9a06",  # class: 'sx'
-        String.Regex: "#4e9a06",  # class: 'sr'
-        String.Single: "#4e9a06",  # class: 's1'
-        String.Symbol: "#4e9a06",  # class: 'ss'
-        Generic: "#000000",  # class: 'g'
-        Generic.Deleted: "#a40000",  # class: 'gd'
-        Generic.Emph: "italic #000000",  # class: 'ge'
-        Generic.Error: "#ef2929",  # class: 'gr'
-        Generic.Heading: "bold #000080",  # class: 'gh'
-        Generic.Inserted: "#00A000",  # class: 'gi'
-        Generic.Output: "#888",  # class: 'go'
-        Generic.Prompt: "#745334",  # class: 'gp'
-        Generic.Strong: "bold #000000",  # class: 'gs'
-        Generic.Subheading: "bold #800080",  # class: 'gu'
-        Generic.Traceback: "bold #a40000",  # class: 'gt'
+        Name:                      "#000000",        # class: 'n'
+        Name.Attribute:            "#c4a000",        # class: 'na' - to be revised
+        Name.Builtin:              "#004461",        # class: 'nb'
+        Name.Builtin.Pseudo:       "#3465a4",        # class: 'bp'
+        Name.Class:                "#000000",        # class: 'nc' - to be revised
+        Name.Constant:             "#000000",        # class: 'no' - to be revised
+        Name.Decorator:            "#888",           # class: 'nd' - to be revised
+        Name.Entity:               "#ce5c00",        # class: 'ni'
+        Name.Exception:            "bold #cc0000",   # class: 'ne'
+        Name.Function:             "#000000",        # class: 'nf'
+        Name.Property:             "#000000",        # class: 'py'
+        Name.Label:                "#f57900",        # class: 'nl'
+        Name.Namespace:            "#000000",        # class: 'nn' - to be revised
+        Name.Other:                "#000000",        # class: 'nx'
+        Name.Tag:                  "bold #004461",   # class: 'nt' - like a keyword
+        Name.Variable:             "#000000",        # class: 'nv' - to be revised
+        Name.Variable.Class:       "#000000",        # class: 'vc' - to be revised
+        Name.Variable.Global:      "#000000",        # class: 'vg' - to be revised
+        Name.Variable.Instance:    "#000000",        # class: 'vi' - to be revised
+
+        Number:                    "#990000",        # class: 'm'
+
+        Literal:                   "#000000",        # class: 'l'
+        Literal.Date:              "#000000",        # class: 'ld'
+
+        String:                    "#4e9a06",        # class: 's'
+        String.Backtick:           "#4e9a06",        # class: 'sb'
+        String.Char:               "#4e9a06",        # class: 'sc'
+        String.Doc:                "italic #8f5902", # class: 'sd' - like a comment
+        String.Double:             "#4e9a06",        # class: 's2'
+        String.Escape:             "#4e9a06",        # class: 'se'
+        String.Heredoc:            "#4e9a06",        # class: 'sh'
+        String.Interpol:           "#4e9a06",        # class: 'si'
+        String.Other:              "#4e9a06",        # class: 'sx'
+        String.Regex:              "#4e9a06",        # class: 'sr'
+        String.Single:             "#4e9a06",        # class: 's1'
+        String.Symbol:             "#4e9a06",        # class: 'ss'
+
+        Generic:                   "#000000",        # class: 'g'
+        Generic.Deleted:           "#a40000",        # class: 'gd'
+        Generic.Emph:              "italic #000000", # class: 'ge'
+        Generic.Error:             "#ef2929",        # class: 'gr'
+        Generic.Heading:           "bold #000080",   # class: 'gh'
+        Generic.Inserted:          "#00A000",        # class: 'gi'
+        Generic.Output:            "#888",           # class: 'go'
+        Generic.Prompt:            "#745334",        # class: 'gp'
+        Generic.Strong:            "bold #000000",   # class: 'gs'
+        Generic.Subheading:        "bold #800080",   # class: 'gu'
+        Generic.Traceback:         "bold #a40000",   # class: 'gt'
     }
```

### Comparing `snimpy-1.0.1/docs/api.rst` & `snimpy-1.0.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/docs/conf.py` & `snimpy-1.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/docs/index.rst` & `snimpy-1.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/docs/installation.rst` & `snimpy-1.0.2/docs/installation.rst`

 * *Files 16% similar despite different names*

```diff
@@ -35,7 +35,11 @@
 .. _libsmi: http://www.ibr.cs.tu-bs.de/projects/libsmi/
 .. _homebrew: http://brew.sh
 
 On Debian and Ubuntu, *Snimpy* is also available as a package you can
 install with::
 
     $ sudo apt-get install snimpy
+
+If you plan to use custom MIBs, note that as snimpy relies on libsmi_ to
+find the MIBs, so you have to add the path to these MIBs in /etc/smi.conf or
+$HOME/.smirc .
```

### Comparing `snimpy-1.0.1/docs/license.rst` & `snimpy-1.0.2/docs/license.rst`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/docs/usage.rst` & `snimpy-1.0.2/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/examples/add-vlan.py` & `snimpy-1.0.2/examples/add-vlan.py`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/examples/disable-port-ingress-filtering.py` & `snimpy-1.0.2/examples/disable-port-ingress-filtering.py`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/examples/enable-lldp.py` & `snimpy-1.0.2/examples/enable-lldp.py`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/examples/get-serial.py` & `snimpy-1.0.2/examples/get-serial.py`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/examples/list-routes.py` & `snimpy-1.0.2/examples/list-routes.py`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/examples/rename-vlan.py` & `snimpy-1.0.2/examples/rename-vlan.py`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/examples/set-syslog-ntp.py` & `snimpy-1.0.2/examples/set-syslog-ntp.py`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/examples/vlan-and-interfaces.py` & `snimpy-1.0.2/examples/vlan-and-interfaces.py`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/flake.lock` & `snimpy-1.0.2/flake.lock`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/flake.nix` & `snimpy-1.0.2/flake.nix`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/man/snimpy.1` & `snimpy-1.0.2/man/snimpy.1`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/snimpy/__main__.py` & `snimpy-1.0.2/snimpy/__main__.py`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/snimpy/basictypes.py` & `snimpy-1.0.2/snimpy/basictypes.py`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/snimpy/config.py` & `snimpy-1.0.2/snimpy/config.py`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/snimpy/main.py` & `snimpy-1.0.2/snimpy/main.py`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/snimpy/manager.py` & `snimpy-1.0.2/snimpy/manager.py`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/snimpy/mib.py` & `snimpy-1.0.2/snimpy/mib.py`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/snimpy/smi_build.py` & `snimpy-1.0.2/snimpy/smi_build.py`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/snimpy/snmp.py` & `snimpy-1.0.2/snimpy/snmp.py`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/snimpy.egg-info/PKG-INFO` & `snimpy-1.0.2/snimpy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snimpy
-Version: 1.0.1
+Version: 1.0.2
 Summary: interactive SNMP tool
 Home-page: https://github.com/vincentbernat/snimpy
 Author: Vincent Bernat
 Author-email: bernat@luffy.cx
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
@@ -79,14 +79,19 @@
 
 
 
 
 History
 -------
 
+1.0.2 (2023-12-12)
+++++++++++++++++++
+
+* Compatibility with Python 3.12 by adding dependency to pyasyncore.
+
 1.0.1 (2023-06-30)
 ++++++++++++++++++
 
 * Switch to pysnmp-lextudio, a maintained fork of PySNMP.
 
 1.0.0 (2021-05-29)
 ++++++++++++++++++
```

### Comparing `snimpy-1.0.1/snimpy.egg-info/SOURCES.txt` & `snimpy-1.0.2/snimpy.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 Makefile
 README.rst
 flake.lock
 flake.nix
 setup.py
 tox.ini
 version.txt
+.github/FUNDING.yml
 .github/dependabot.yml
 .github/workflows/tests.yml
 docs/Makefile
 docs/api.rst
 docs/conf.py
 docs/contributing.rst
 docs/history.rst
```

### Comparing `snimpy-1.0.1/tests/SNIMPY-INVALID-MIB.mib` & `snimpy-1.0.2/tests/SNIMPY-INVALID-MIB.mib`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/tests/SNIMPY-MIB.mib` & `snimpy-1.0.2/tests/SNIMPY-MIB.mib`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/tests/agent.py` & `snimpy-1.0.2/tests/agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from multiprocessing import Process, Queue
 import random
 
 from pysnmp.entity import engine, config
 from pysnmp.entity.rfc3413 import cmdrsp, context
-from pysnmp.carrier.asynsock.dgram import udp, udp6
+from pysnmp.carrier.asyncio.dgram import udp, udp6
 from pysnmp.proto.api import v2c
 
 
 class TestAgent:
 
     next_port = [random.randint(22000, 32000)]
```

### Comparing `snimpy-1.0.1/tests/test_basictypes.py` & `snimpy-1.0.2/tests/test_basictypes.py`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/tests/test_conf.py` & `snimpy-1.0.2/tests/test_conf.py`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/tests/test_main.py` & `snimpy-1.0.2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/tests/test_manager.py` & `snimpy-1.0.2/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/tests/test_mib.py` & `snimpy-1.0.2/tests/test_mib.py`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/tests/test_snmp.py` & `snimpy-1.0.2/tests/test_snmp.py`

 * *Files identical despite different names*

### Comparing `snimpy-1.0.1/tox.ini` & `snimpy-1.0.2/tox.ini`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [tox]
-envlist = py{34,35,36,37,38,39,310,311}{,-ipython},lint,doc
+envlist = py{34,35,36,37,38,39,310,311,312}{,-ipython},lint,doc
 skip_missing_interpreters = True
 
 [gh-actions]
 python =
   3.6: py36
   3.7: py37
   3.8: py38, lint, doc
   3.9: py39
   3.10: py310
   3.11: py311
+  3.12: py312
 
 [testenv]
 allowlist_externals = make
 deps =
     coverage
     ipython: ipython
     pytest
```

