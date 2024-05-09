# Comparing `tmp/sqlmap-1.8.4.tar.gz` & `tmp/sqlmap-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sqlmap-1.8.4.tar", last modified: Mon Apr  8 08:49:45 2024, max compression
+gzip compressed data, was "dist/sqlmap-1.8.5.tar", last modified: Thu May  9 14:15:02 2024, max compression
```

## Comparing `sqlmap-1.8.4.tar` & `sqlmap-1.8.5.tar`

### file list

```diff
@@ -1,781 +1,781 @@
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    29017 2024-04-08 08:49:36.000000 sqlmap-1.8.4/MANIFEST.in
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4946 2024-04-08 08:49:45.000000 sqlmap-1.8.4/PKG-INFO
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5302 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/README.md
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/thirdparty/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/thirdparty/wininetpton/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      319 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/wininetpton/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2775 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/wininetpton/win_inet_pton.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/thirdparty/clientform/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)   126727 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/clientform/clientform.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/clientform/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/thirdparty/multipart/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4513 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/multipart/multipartpost.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/multipart/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/thirdparty/socks/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    17437 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/socks/socks.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/socks/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1401 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/socks/LICENSE
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    10510 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/escsm.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3749 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/eucjpprober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2766 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/utf8prober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    11102 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/langturkishmodel.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5110 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/charsetprober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3413 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/mbcharsetprober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    13546 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/euckrfreq.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      242 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/version.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1754 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/gb2312prober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1855 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/cp949prober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     9411 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/chardistribution.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1661 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/enums.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    11345 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/langhebrewmodel.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    12688 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/langgreekmodel.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3950 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/escprober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3590 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/codingstatemachine.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    31621 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/euctwfreq.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5370 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/latin1prober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    12839 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/langbulgarianmodel.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    31254 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/big5freq.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1748 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/euckrprober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    25777 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/jisfreq.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1757 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/big5prober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    25481 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/mbcssm.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    12485 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/universaldetector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    20715 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/gb2312freq.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3774 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/sjisprober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1134 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/compat.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3546 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/sbcsgroupprober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1559 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3787 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/charsetgroupprober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    19643 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/jpcntx.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    17948 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/langcyrillicmodel.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    12592 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/langhungarianmodel.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1747 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/euctwprober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5657 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/sbcharsetprober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2012 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/mbcsgroupprober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    11290 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/langthaimodel.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    13838 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/chardet/hebrewprober.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/thirdparty/odict/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4283 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/odict/ordereddict.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      156 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/odict/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/thirdparty/keepalive/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      730 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/keepalive/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    22807 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/keepalive/keepalive.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/thirdparty/magic/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6723 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/magic/magic.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/magic/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/thirdparty/ansistrm/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5329 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/ansistrm/ansistrm.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/ansistrm/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/thirdparty/identywaf/
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)    25913 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/identywaf/identYwaf.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    61564 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/identywaf/data.json
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      270 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/identywaf/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1078 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/identywaf/LICENSE
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/thirdparty/prettyprint/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1357 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/prettyprint/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4215 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/prettyprint/prettyprint.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/thirdparty/bottle/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)   170898 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/bottle/bottle.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        5 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/bottle/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/thirdparty/fcrypt/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1356 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/fcrypt/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    26757 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/fcrypt/fcrypt.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/thirdparty/pydes/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    27500 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/pydes/pyDes.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      720 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/pydes/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/thirdparty/beautifulsoup/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    80038 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/beautifulsoup/beautifulsoup.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1673 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/beautifulsoup/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/thirdparty/six/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    34581 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/six/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/thirdparty/termcolor/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/termcolor/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5246 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/termcolor/termcolor.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/thirdparty/colorama/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2524 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/colorama/ansi.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2065 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/colorama/initialise.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6356 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/colorama/winterm.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      240 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/colorama/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    10243 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/colorama/ansitowin32.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5365 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/thirdparty/colorama/win32.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    16703 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/.pylintrc
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/procs/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/procs/mssqlserver/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      269 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/procs/mssqlserver/create_new_xp_cmdshell.sql
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      246 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/procs/mssqlserver/configure_openrowset.sql
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)       47 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/procs/mssqlserver/disable_xp_cmdshell_2000.sql
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)       70 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/procs/mssqlserver/enable_xp_cmdshell_2000.sql
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      163 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/procs/mssqlserver/activate_sp_oacreate.sql
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      333 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/procs/mssqlserver/run_statement_as_user.sql
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      197 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/procs/mssqlserver/dns_request.sql
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      236 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/procs/mssqlserver/configure_xp_cmdshell.sql
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      187 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/procs/README.txt
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/procs/postgresql/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      536 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/procs/postgresql/dns_request.sql
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/procs/mysql/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)       73 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/procs/mysql/write_file_limit.sql
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)       85 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/procs/mysql/dns_request.sql
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/procs/oracle/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2010 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/procs/oracle/read_file_export_extension.sql
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      397 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/procs/oracle/dns_request.sql
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      282 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/README.txt
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/9.1/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2693 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/9.1/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/9.0/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2633 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/9.0/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/9.5/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2633 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/9.5/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/9.3/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2693 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/9.3/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/12/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3257 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/12/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/11/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2633 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/11/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/8.4/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2563 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/8.4/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/8.2/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2561 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/8.2/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/8.3/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2562 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/8.3/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/9.4/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2693 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/9.4/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/10/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2632 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/10/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/9.2/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2693 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/9.2/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/9.6/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2632 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/9.6/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/9.1/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2652 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/9.1/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/9.0/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2729 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/9.0/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/9.5/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2639 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/9.5/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/9.3/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2652 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/9.3/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/11/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2640 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/11/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/8.4/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2020 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/8.4/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/8.2/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2018 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/8.2/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/8.3/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2016 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/8.3/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/9.4/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2652 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/9.4/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/10/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2639 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/10/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/9.2/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2652 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/9.2/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/9.6/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2640 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/9.6/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/windows/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/windows/32/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/windows/32/9.0/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4231 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/windows/32/9.0/lib_postgresqludf_sys.dll_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/windows/32/8.4/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4773 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/windows/32/8.4/lib_postgresqludf_sys.dll_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/windows/32/8.2/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4755 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/windows/32/8.2/lib_postgresqludf_sys.dll_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/windows/32/8.3/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4766 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/postgresql/windows/32/8.3/lib_postgresqludf_sys.dll_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/mysql/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/mysql/linux/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/mysql/linux/64/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3200 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/mysql/linux/64/lib_mysqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/mysql/linux/32/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2512 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/mysql/linux/32/lib_mysqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/mysql/windows/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/mysql/windows/64/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5267 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/mysql/windows/64/lib_mysqludf_sys.dll_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/udf/mysql/windows/32/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4549 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/udf/mysql/windows/32/lib_mysqludf_sys.dll_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/shell/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/shell/stagers/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      379 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/shell/stagers/stager.php_
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1201 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/shell/stagers/stager.asp_
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      529 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/shell/stagers/stager.aspx_
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1321 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/shell/stagers/stager.jsp_
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      686 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/shell/README.txt
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/shell/backdoors/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      243 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/shell/backdoors/backdoor.asp_
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      469 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/shell/backdoors/backdoor.php_
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      417 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/shell/backdoors/backdoor.aspx_
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      359 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/shell/backdoors/backdoor.jsp_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/txt/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    68896 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/txt/smalldict.txt
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18539 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/txt/common-outputs.txt
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    44074 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/txt/common-tables.txt
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)   399831 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/txt/user-agents.txt
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    61005 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/txt/sha256sums.txt
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    48329 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/txt/common-files.txt
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    14646 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/txt/keywords.txt
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    26013 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/txt/common-columns.txt
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)  6076425 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/txt/wordlist.tx_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/html/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5763 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/html/index.html
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/xml/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     9507 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/xml/errors.xml
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/xml/payloads/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    19304 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/xml/payloads/union_query.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5482 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/xml/payloads/inline_query.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    68050 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/xml/payloads/error_based.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    79693 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/xml/payloads/time_blind.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    24754 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/xml/payloads/stacked_queries.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    60087 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/xml/payloads/boolean_blind.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)   141162 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/xml/queries.xml
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/data/xml/banner/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      242 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/xml/banner/sharepoint.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1649 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/xml/banner/x-powered-by.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1448 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/xml/banner/set-cookie.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      233 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/xml/banner/x-aspnet-version.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)   101453 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/xml/banner/mssql.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      805 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/xml/banner/servlet-engine.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3897 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/xml/banner/generic.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      327 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/xml/banner/postgresql.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    31443 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/xml/banner/server.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      158 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/xml/banner/oracle.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2956 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/xml/banner/mysql.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    15092 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/data/xml/boundaries.xml
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/tamper/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1879 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/between.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      590 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/symboliclogical.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      955 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/misunion.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      753 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/schemasplit.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      906 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/dunion.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1127 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/least.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1211 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/substring2leftright.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1007 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/concat2concatws.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3046 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/luanginx.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      944 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/apostrophemask.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2589 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/space2mssqlblank.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      700 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/0eunion.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1197 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/randomcomments.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1802 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/plus2concat.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      963 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/varnish.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1314 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/multiplespaces.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1597 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/versionedkeywords.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      918 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/space2mssqlhash.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      639 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/informationschemacomment.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      559 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/ord2ascii.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1737 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/versionedmorekeywords.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      523 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/apostrophenullencode.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1413 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/percentage.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      825 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/sp_password.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      766 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/equaltorlike.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2250 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/plus2fnconcat.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1855 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/halfversionedmorekeywords.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1295 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/space2morecomment.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1201 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/modsecurityzeroversioned.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1135 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/greatest.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1290 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/bluecoat.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1065 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/uppercase.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1584 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/space2hash.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1455 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/overlongutf8more.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      680 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/decentities.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1264 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/space2dash.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1292 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/modsecurityversioned.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      715 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/hexentities.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1388 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/charencode.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      918 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/equaltolike.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1218 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/chardoubleencode.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      985 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/scientific.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1351 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/space2comment.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1306 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/unmagicquotes.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1285 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/xforwardedfor.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1282 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/space2plus.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1215 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/charunicodeescape.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      511 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/unionalltounion.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2218 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/space2morehash.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1744 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/ifnull2casewhenisnull.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      468 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/escapequotes.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1669 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/ifnull2ifisnull.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      758 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/commentbeforeparentheses.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      868 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/sleep2getlock.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1002 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/lowercase.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1225 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/commalessmid.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1646 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/charunicodeencode.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1168 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/space2mysqldash.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1377 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/hex2char.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1736 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/randomcase.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1000 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/appendnullbyte.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      519 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/base64encode.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1663 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/space2randomblank.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1295 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/binary.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2113 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/if2case.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1444 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/overlongutf8.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1977 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/space2mysqlblank.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      849 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/htmlencode.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      970 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/tamper/commalesslimit.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      258 2024-04-08 08:49:36.000000 sqlmap-1.8.4/sqlmap/__init__.py
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)    25734 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/sqlmap.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/doc/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    34109 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/CHANGELOG.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    25122 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/THANKS.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      190 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/AUTHORS
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/doc/translations/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3275 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-it-IT.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4221 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-uk-UA.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3289 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-ko-KR.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3143 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-rs-RS.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4882 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-in-HI.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3786 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-fa-IR.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4086 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-bg-BG.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4212 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-ru-RU.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3132 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-id-ID.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3326 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-fr-FR.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3169 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-pt-BR.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3174 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-hr-HR.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3161 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-nl-NL.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3234 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-sk-SK.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3555 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-vi-VN.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3220 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-pl-PL.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4242 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-gr-GR.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2951 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-zh-CN.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3603 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-ja-JP.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6020 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-ka-GE.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3023 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-tr-TR.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3178 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-de-DE.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3429 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/translations/README-es-MX.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    14763 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/doc/THIRD-PARTY.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    22364 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/sqlmap.conf
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18886 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/LICENSE
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/generic/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2654 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/generic/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2484 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/generic/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5055 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/generic/custom.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    30708 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/generic/entries.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    27907 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/generic/search.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1730 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/generic/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18208 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/generic/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    29216 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/generic/users.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1723 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/generic/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/generic/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6887 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/generic/misc.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    54885 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/generic/databases.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    12371 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/generic/filesystem.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/presto/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1701 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/presto/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2204 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/presto/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      678 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/presto/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      971 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/presto/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5279 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/presto/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      910 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/presto/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      671 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/presto/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/hsqldb/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1445 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/hsqldb/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2784 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/hsqldb/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      687 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/hsqldb/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      971 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/hsqldb/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5276 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/hsqldb/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      909 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/hsqldb/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2537 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/hsqldb/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mssqlserver/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18049 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mssqlserver/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2583 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mssqlserver/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      889 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mssqlserver/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6499 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mssqlserver/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6913 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mssqlserver/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      950 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mssqlserver/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    17312 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mssqlserver/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/access/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2525 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/access/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2130 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/access/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      670 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/access/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1011 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/access/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5843 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/access/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      919 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/access/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      691 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/access/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/raima/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2609 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/raima/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      520 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/raima/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      687 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/raima/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1035 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/raima/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2652 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/raima/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      899 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/raima/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      703 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/raima/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/derby/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1322 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/derby/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1830 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/derby/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      447 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/derby/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      995 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/derby/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2636 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/derby/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      907 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/derby/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/derby/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cache/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1356 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cache/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2397 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cache/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      735 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cache/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      967 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cache/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3135 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cache/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      900 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cache/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cache/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/vertica/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      459 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/vertica/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1920 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/vertica/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      689 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/vertica/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      975 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/vertica/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2992 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/vertica/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      920 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/vertica/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/vertica/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/firebird/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1080 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/firebird/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2260 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/firebird/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1151 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/firebird/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      979 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/firebird/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4990 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/firebird/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      929 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/firebird/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      675 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/firebird/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/monetdb/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1103 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/monetdb/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1894 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/monetdb/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      735 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/monetdb/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      975 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/monetdb/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2549 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/monetdb/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      920 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/monetdb/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/monetdb/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/maxdb/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     9202 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/maxdb/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      507 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/maxdb/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      447 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/maxdb/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      983 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/maxdb/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3792 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/maxdb/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      903 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/maxdb/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      678 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/maxdb/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mimersql/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      926 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mimersql/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1858 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mimersql/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      807 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mimersql/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      979 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mimersql/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2591 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mimersql/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      930 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mimersql/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mimersql/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/postgresql/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      428 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/postgresql/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2097 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/postgresql/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1016 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/postgresql/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5448 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/postgresql/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    10052 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/postgresql/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1304 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/postgresql/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3005 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/postgresql/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mysql/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      265 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mysql/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2095 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mysql/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1044 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mysql/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5124 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mysql/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    12785 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mysql/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1113 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mysql/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7731 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mysql/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/informix/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1022 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/informix/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1902 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/informix/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1272 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/informix/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      365 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/informix/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3284 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/informix/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      930 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/informix/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/informix/filesystem.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/altibase/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      589 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/altibase/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      506 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/altibase/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      678 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/altibase/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      979 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/altibase/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2657 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/altibase/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      930 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/altibase/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/altibase/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/extremedb/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2427 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/extremedb/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      507 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/extremedb/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      447 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/extremedb/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      983 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/extremedb/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2673 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/extremedb/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      939 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/extremedb/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      677 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/extremedb/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mckoi/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2371 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mckoi/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      503 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mckoi/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      447 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mckoi/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      967 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mckoi/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2590 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mckoi/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      899 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mckoi/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      669 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/mckoi/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/db2/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      615 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/db2/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1935 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/db2/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      678 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/db2/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      365 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/db2/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5871 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/db2/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      880 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/db2/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/db2/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cubrid/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      918 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cubrid/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1835 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cubrid/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      726 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cubrid/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      971 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cubrid/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2541 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cubrid/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      910 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cubrid/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cubrid/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/h2/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1580 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/h2/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      500 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/h2/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      687 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/h2/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      955 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/h2/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3324 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/h2/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      869 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/h2/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      663 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/h2/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/oracle/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6002 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/oracle/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2817 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/oracle/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      886 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/oracle/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1101 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/oracle/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3880 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/oracle/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      909 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/oracle/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2301 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/oracle/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cratedb/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      632 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cratedb/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2097 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cratedb/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      447 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cratedb/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      975 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cratedb/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2538 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cratedb/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      920 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cratedb/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/cratedb/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/sybase/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    11670 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/sybase/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2558 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/sybase/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      899 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/sybase/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      971 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/sybase/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3429 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/sybase/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      909 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/sybase/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      671 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/sybase/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/clickhouse/
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      638 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/clickhouse/enumeration.py
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      255 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/clickhouse/connector.py
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      687 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/clickhouse/syntax.py
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      987 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/clickhouse/takeover.py
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)     2627 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/clickhouse/fingerprint.py
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      950 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/clickhouse/__init__.py
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      679 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/clickhouse/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/sqlite/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2054 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/sqlite/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3083 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/sqlite/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      644 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/sqlite/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      971 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/sqlite/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3176 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/sqlite/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      909 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/sqlite/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      671 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/sqlite/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/virtuoso/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1541 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/virtuoso/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      506 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/virtuoso/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      678 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/virtuoso/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      979 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/virtuoso/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2517 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/virtuoso/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      929 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/virtuoso/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      675 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/virtuoso/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/frontbase/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      923 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/frontbase/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      507 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/frontbase/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      447 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/frontbase/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      983 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/frontbase/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2613 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/frontbase/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      939 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/frontbase/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      677 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/plugins/dbms/frontbase/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/lib/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/lib/controller/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     8896 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/controller/handler.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7233 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/controller/action.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    75900 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/controller/checks.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/controller/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    36817 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/controller/controller.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/lib/utils/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7984 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/utils/search.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4686 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/utils/httpd.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    48979 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/utils/hash.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2325 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/utils/getch.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5207 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/utils/sqlalchemy.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     8450 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/utils/hashdb.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2935 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/utils/xrange.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      926 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/utils/versioncheck.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3337 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/utils/progress.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2674 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/utils/purge.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    10977 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/utils/crawler.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     8030 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/utils/har.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    15901 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/utils/brute.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7369 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/utils/pivotdumptable.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/utils/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    34389 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/utils/api.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3190 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/utils/safe2bin.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1111 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/utils/timeout.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5564 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/utils/deps.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18275 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/utils/sgmllib.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/lib/request/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18899 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/request/basic.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6017 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/request/dns.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3229 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/request/direct.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     8399 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/request/redirecthandler.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      942 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/request/rangehandler.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      590 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/request/methodrequest.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5815 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/request/httpshandler.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/request/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      633 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/request/templates.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1384 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/request/basicauthhandler.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1566 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/request/chunkedhandler.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1158 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/request/pkihandler.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    24808 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/request/inject.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    80509 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/request/connect.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7788 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/request/comparison.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/lib/techniques/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/lib/techniques/error/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    21157 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/techniques/error/use.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/techniques/error/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/lib/techniques/dns/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5061 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/techniques/dns/use.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1125 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/techniques/dns/test.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/techniques/dns/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/lib/techniques/blind/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/techniques/blind/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    34684 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/techniques/blind/inference.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/techniques/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/lib/techniques/union/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    23147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/techniques/union/use.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18664 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/techniques/union/test.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/techniques/union/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/lib/core/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      728 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/data.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5865 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/patch.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1800 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/readlineng.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    28848 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/dump.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     8414 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/threads.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    13586 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/convert.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    13936 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/enums.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2634 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/decorators.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6032 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/bigarray.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    10052 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/gui.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1646 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/exception.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    15220 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/testing.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7536 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/optiondict.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    34190 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/target.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1980 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/session.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    59654 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/agent.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)   106570 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/option.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    45400 2024-04-08 08:49:36.000000 sqlmap-1.8.4/sqlmap/lib/core/settings.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     8986 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/compat.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5657 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/subprocessng.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1876 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/revision.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      885 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/profiling.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      559 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/defaults.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5489 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/log.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4956 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/shell.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    17637 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/dicts.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3201 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/wordlist.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      988 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/unescaper.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7468 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/update.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5046 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/replication.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6646 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/datatype.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)   195050 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/core/common.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/lib/takeover/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     8440 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/takeover/abstraction.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    13903 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/takeover/udf.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    28240 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/takeover/metasploit.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    11839 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/takeover/xp_cmdshell.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3838 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/takeover/registry.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18315 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/takeover/web.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/takeover/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4739 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/takeover/icmpsh.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/lib/parse/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    50151 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/parse/cmdline.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2703 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/parse/handler.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3578 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/parse/payloads.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3498 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/parse/configfile.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1460 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/parse/headers.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1805 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/parse/sitemap.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/parse/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3580 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/parse/banner.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3022 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/lib/parse/html.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6215 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/sqlmapapi.yaml
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/extra/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/extra/cloak/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2286 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/cloak/cloak.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      732 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/cloak/README.txt
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/cloak/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/extra/shutils/
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      305 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/shutils/modernize.sh
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      797 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/shutils/duplicates.py
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)     1368 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/shutils/precommit-hook.sh
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      332 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/shutils/pycodestyle.sh
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      660 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/shutils/drei.sh
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      255 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/shutils/blanks.sh
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      235 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/shutils/pylint.sh
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)     5855 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/shutils/pypi.sh
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      630 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/shutils/recloak.sh
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      903 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/shutils/newlines.py
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      869 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/shutils/strip.sh
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      245 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/shutils/junk.sh
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      311 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/shutils/autocompletion.sh
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      313 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/shutils/pydiatra.sh
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      875 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/shutils/postcommit-hook.sh
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      320 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/shutils/pyflakes.sh
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/extra/runcmd/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      193 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/runcmd/README.txt
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/extra/runcmd/src/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      883 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/runcmd/src/runcmd.sln
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      271 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/runcmd/src/README.txt
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/extra/runcmd/src/runcmd/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1348 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/runcmd/src/runcmd/runcmd.cpp
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      516 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/runcmd/src/runcmd/stdafx.h
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4508 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/runcmd/src/runcmd/runcmd.vcproj
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      293 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/runcmd/src/runcmd/stdafx.cpp
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    37206 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/runcmd/runcmd.exe_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/extra/beep/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2901 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/beep/beep.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/beep/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    46772 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/beep/beep.wav
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/extra/shellcodeexec/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/extra/shellcodeexec/linux/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1691 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/shellcodeexec/linux/shellcodeexec.x32_
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1927 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/shellcodeexec/linux/shellcodeexec.x64_
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      282 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/shellcodeexec/README.txt
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/extra/shellcodeexec/windows/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2758 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/shellcodeexec/windows/shellcodeexec.x32.exe_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/extra/icmpsh/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3965 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/icmpsh/icmpsh-m.c
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7009 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/icmpsh/icmpsh.exe_
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     9342 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/icmpsh/icmpsh-s.c
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1641 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/icmpsh/README.txt
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2136 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/icmpsh/icmpsh-m.pl
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      872 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/icmpsh/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4809 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/icmpsh/icmpsh_m.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/extra/dbgtool/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2475 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/dbgtool/dbgtool.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      549 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/dbgtool/README.txt
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/dbgtool/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap/extra/vulnserver/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     9127 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/vulnserver/vulnserver.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/extra/vulnserver/__init__.py
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)     4229 2024-04-08 08:11:36.000000 sqlmap-1.8.4/sqlmap/sqlmapapi.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)       38 2024-04-08 08:49:45.000000 sqlmap-1.8.4/setup.cfg
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3187 2024-04-08 08:49:36.000000 sqlmap-1.8.4/README.rst
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap.egg-info/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    24174 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap.egg-info/SOURCES.txt
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4946 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap.egg-info/PKG-INFO
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        7 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap.egg-info/top_level.txt
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        1 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap.egg-info/not-zip-safe
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)       47 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap.egg-info/entry_points.txt
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        1 2024-04-08 08:49:45.000000 sqlmap-1.8.4/sqlmap.egg-info/dependency_links.txt
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1549 2024-04-08 08:49:34.000000 sqlmap-1.8.4/setup.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    29017 2024-05-09 14:15:01.000000 sqlmap-1.8.5/MANIFEST.in
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4946 2024-05-09 14:15:02.000000 sqlmap-1.8.5/PKG-INFO
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5302 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/README.md
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/thirdparty/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/thirdparty/wininetpton/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      319 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/wininetpton/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2775 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/wininetpton/win_inet_pton.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/thirdparty/clientform/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)   126727 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/clientform/clientform.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/clientform/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/thirdparty/multipart/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4513 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/multipart/multipartpost.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/multipart/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/thirdparty/socks/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    17437 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/socks/socks.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/socks/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1401 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/socks/LICENSE
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/thirdparty/chardet/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    10510 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/chardet/escsm.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3749 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/chardet/eucjpprober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2766 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/chardet/utf8prober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    11102 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/chardet/langturkishmodel.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5110 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/chardet/charsetprober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3413 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/chardet/mbcharsetprober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    13546 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/chardet/euckrfreq.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      242 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/chardet/version.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1754 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/chardet/gb2312prober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1855 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/chardet/cp949prober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     9411 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/chardet/chardistribution.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1661 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/chardet/enums.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    11345 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/chardet/langhebrewmodel.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    12688 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/chardet/langgreekmodel.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3950 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/chardet/escprober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3590 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/chardet/codingstatemachine.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    31621 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/chardet/euctwfreq.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5370 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/chardet/latin1prober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    12839 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/chardet/langbulgarianmodel.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    31254 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/chardet/big5freq.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1748 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/chardet/euckrprober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    25777 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/chardet/jisfreq.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1757 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/chardet/big5prober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    25481 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/chardet/mbcssm.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    12485 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/chardet/universaldetector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    20715 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/chardet/gb2312freq.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3774 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/chardet/sjisprober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1134 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/chardet/compat.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3546 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/chardet/sbcsgroupprober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1559 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/chardet/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3787 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/chardet/charsetgroupprober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    19643 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/chardet/jpcntx.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    17948 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/chardet/langcyrillicmodel.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    12592 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/chardet/langhungarianmodel.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1747 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/chardet/euctwprober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5657 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/chardet/sbcharsetprober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2012 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/chardet/mbcsgroupprober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    11290 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/chardet/langthaimodel.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    13838 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/chardet/hebrewprober.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/thirdparty/odict/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4283 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/odict/ordereddict.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      156 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/odict/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/thirdparty/keepalive/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      730 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/keepalive/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    22807 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/keepalive/keepalive.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/thirdparty/magic/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6723 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/magic/magic.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/magic/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/thirdparty/ansistrm/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5329 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/ansistrm/ansistrm.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/ansistrm/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/thirdparty/identywaf/
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)    25913 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/identywaf/identYwaf.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    61564 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/identywaf/data.json
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      270 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/identywaf/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1078 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/identywaf/LICENSE
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/thirdparty/prettyprint/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1357 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/prettyprint/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4215 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/prettyprint/prettyprint.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/thirdparty/bottle/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)   170898 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/bottle/bottle.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        5 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/bottle/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/thirdparty/fcrypt/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1356 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/fcrypt/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    26757 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/fcrypt/fcrypt.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/thirdparty/pydes/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    27500 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/pydes/pyDes.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      720 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/pydes/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/thirdparty/beautifulsoup/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    80034 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/beautifulsoup/beautifulsoup.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1669 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/beautifulsoup/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/thirdparty/six/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    34581 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/six/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/thirdparty/termcolor/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/termcolor/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5246 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/termcolor/termcolor.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/thirdparty/colorama/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2524 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/colorama/ansi.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2065 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/colorama/initialise.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6356 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/colorama/winterm.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      240 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/colorama/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    10243 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/colorama/ansitowin32.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5365 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/thirdparty/colorama/win32.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    16703 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/.pylintrc
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/procs/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/procs/mssqlserver/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      269 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/procs/mssqlserver/create_new_xp_cmdshell.sql
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      246 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/procs/mssqlserver/configure_openrowset.sql
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)       47 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/procs/mssqlserver/disable_xp_cmdshell_2000.sql
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)       70 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/procs/mssqlserver/enable_xp_cmdshell_2000.sql
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      163 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/procs/mssqlserver/activate_sp_oacreate.sql
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      333 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/procs/mssqlserver/run_statement_as_user.sql
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      197 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/procs/mssqlserver/dns_request.sql
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      236 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/procs/mssqlserver/configure_xp_cmdshell.sql
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      187 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/procs/README.txt
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/procs/postgresql/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      536 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/procs/postgresql/dns_request.sql
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/procs/mysql/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)       73 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/procs/mysql/write_file_limit.sql
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)       85 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/procs/mysql/dns_request.sql
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/procs/oracle/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2010 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/procs/oracle/read_file_export_extension.sql
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      397 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/procs/oracle/dns_request.sql
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/udf/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      282 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/udf/README.txt
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/64/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/64/9.1/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2693 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/64/9.1/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/64/9.0/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2633 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/64/9.0/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/64/9.5/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2633 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/64/9.5/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/64/9.3/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2693 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/64/9.3/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/64/12/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3257 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/64/12/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/64/11/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2633 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/64/11/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/64/8.4/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2563 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/64/8.4/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/64/8.2/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2561 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/64/8.2/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/64/8.3/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2562 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/64/8.3/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/64/9.4/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2693 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/64/9.4/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/64/10/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2632 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/64/10/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/64/9.2/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2693 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/64/9.2/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/64/9.6/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2632 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/64/9.6/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/32/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/32/9.1/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2652 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/32/9.1/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/32/9.0/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2729 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/32/9.0/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/32/9.5/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2639 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/32/9.5/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/32/9.3/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2652 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/32/9.3/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/32/11/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2640 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/32/11/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/32/8.4/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2020 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/32/8.4/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/32/8.2/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2018 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/32/8.2/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/32/8.3/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2016 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/32/8.3/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/32/9.4/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2652 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/32/9.4/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/32/10/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2639 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/32/10/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/32/9.2/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2652 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/32/9.2/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/32/9.6/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2640 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/32/9.6/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/windows/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/windows/32/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/windows/32/9.0/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4231 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/windows/32/9.0/lib_postgresqludf_sys.dll_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/windows/32/8.4/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4773 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/windows/32/8.4/lib_postgresqludf_sys.dll_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/windows/32/8.2/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4755 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/windows/32/8.2/lib_postgresqludf_sys.dll_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/windows/32/8.3/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4766 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/udf/postgresql/windows/32/8.3/lib_postgresqludf_sys.dll_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/udf/mysql/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/udf/mysql/linux/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/udf/mysql/linux/64/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3200 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/udf/mysql/linux/64/lib_mysqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/udf/mysql/linux/32/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2512 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/udf/mysql/linux/32/lib_mysqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/udf/mysql/windows/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/udf/mysql/windows/64/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5267 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/udf/mysql/windows/64/lib_mysqludf_sys.dll_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/udf/mysql/windows/32/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4549 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/udf/mysql/windows/32/lib_mysqludf_sys.dll_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/shell/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/shell/stagers/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      379 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/shell/stagers/stager.php_
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1201 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/shell/stagers/stager.asp_
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      529 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/shell/stagers/stager.aspx_
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1321 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/shell/stagers/stager.jsp_
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      686 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/shell/README.txt
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/shell/backdoors/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      243 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/shell/backdoors/backdoor.asp_
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      469 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/shell/backdoors/backdoor.php_
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      417 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/shell/backdoors/backdoor.aspx_
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      359 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/shell/backdoors/backdoor.jsp_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/txt/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    68896 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/txt/smalldict.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18539 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/txt/common-outputs.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    44074 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/txt/common-tables.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)   399831 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/txt/user-agents.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    61005 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/txt/sha256sums.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    48329 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/txt/common-files.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    14646 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/txt/keywords.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    26013 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/txt/common-columns.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)  6076425 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/txt/wordlist.tx_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/html/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5763 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/html/index.html
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/xml/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     9507 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/xml/errors.xml
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/xml/payloads/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    19304 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/xml/payloads/union_query.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5482 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/xml/payloads/inline_query.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    68050 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/xml/payloads/error_based.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    79693 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/xml/payloads/time_blind.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    24754 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/xml/payloads/stacked_queries.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    60087 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/xml/payloads/boolean_blind.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)   141162 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/xml/queries.xml
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/data/xml/banner/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      242 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/xml/banner/sharepoint.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1649 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/xml/banner/x-powered-by.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1448 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/xml/banner/set-cookie.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      233 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/xml/banner/x-aspnet-version.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)   101453 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/xml/banner/mssql.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      805 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/xml/banner/servlet-engine.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3897 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/xml/banner/generic.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      327 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/xml/banner/postgresql.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    31443 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/xml/banner/server.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      158 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/xml/banner/oracle.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2956 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/xml/banner/mysql.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    15092 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/data/xml/boundaries.xml
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/tamper/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1879 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/between.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      590 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/symboliclogical.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      955 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/misunion.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      753 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/schemasplit.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      906 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/dunion.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1127 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/least.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1211 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/substring2leftright.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1007 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/concat2concatws.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3046 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/luanginx.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      944 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/apostrophemask.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2589 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/space2mssqlblank.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      700 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/0eunion.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1197 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/randomcomments.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1802 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/plus2concat.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      963 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/varnish.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1314 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/multiplespaces.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1597 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/versionedkeywords.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      918 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/space2mssqlhash.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      639 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/informationschemacomment.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      559 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/ord2ascii.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1737 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/versionedmorekeywords.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      523 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/apostrophenullencode.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1413 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/percentage.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      825 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/sp_password.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      766 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/equaltorlike.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2250 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/plus2fnconcat.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1855 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/halfversionedmorekeywords.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1295 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/space2morecomment.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1201 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/modsecurityzeroversioned.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1135 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/greatest.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1290 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/bluecoat.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1065 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/uppercase.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1584 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/space2hash.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1455 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/overlongutf8more.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      680 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/decentities.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1264 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/space2dash.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1292 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/modsecurityversioned.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      715 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/hexentities.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1388 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/charencode.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      918 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/equaltolike.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1218 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/chardoubleencode.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      985 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/scientific.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1351 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/space2comment.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1306 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/unmagicquotes.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1285 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/xforwardedfor.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1282 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/space2plus.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1215 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/charunicodeescape.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      511 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/unionalltounion.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2218 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/space2morehash.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1744 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/ifnull2casewhenisnull.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      468 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/escapequotes.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1669 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/ifnull2ifisnull.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      758 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/commentbeforeparentheses.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      868 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/sleep2getlock.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1002 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/lowercase.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1225 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/commalessmid.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1646 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/charunicodeencode.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1168 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/space2mysqldash.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1377 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/hex2char.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1736 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/randomcase.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1000 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/appendnullbyte.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      519 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/base64encode.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1663 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/space2randomblank.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1295 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/binary.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2113 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/if2case.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1444 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/overlongutf8.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1977 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/space2mysqlblank.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      849 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/htmlencode.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      970 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/tamper/commalesslimit.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      258 2024-05-09 14:15:01.000000 sqlmap-1.8.5/sqlmap/__init__.py
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)    25734 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/sqlmap.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/doc/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    34109 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/doc/CHANGELOG.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    25122 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/doc/THANKS.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      190 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/doc/AUTHORS
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/doc/translations/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3275 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/doc/translations/README-it-IT.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4221 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/doc/translations/README-uk-UA.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3289 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/doc/translations/README-ko-KR.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3143 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/doc/translations/README-rs-RS.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4882 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/doc/translations/README-in-HI.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3786 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/doc/translations/README-fa-IR.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4086 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/doc/translations/README-bg-BG.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4212 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/doc/translations/README-ru-RU.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3132 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/doc/translations/README-id-ID.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3326 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/doc/translations/README-fr-FR.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3169 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/doc/translations/README-pt-BR.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3174 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/doc/translations/README-hr-HR.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3161 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/doc/translations/README-nl-NL.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3234 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/doc/translations/README-sk-SK.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3555 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/doc/translations/README-vi-VN.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3220 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/doc/translations/README-pl-PL.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4242 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/doc/translations/README-gr-GR.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2951 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/doc/translations/README-zh-CN.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3603 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/doc/translations/README-ja-JP.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6020 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/doc/translations/README-ka-GE.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3023 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/doc/translations/README-tr-TR.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3178 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/doc/translations/README-de-DE.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3429 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/doc/translations/README-es-MX.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    14763 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/doc/THIRD-PARTY.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    22364 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/sqlmap.conf
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18886 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/LICENSE
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/plugins/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/plugins/generic/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2654 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/generic/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2484 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/generic/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5055 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/generic/custom.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    30708 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/generic/entries.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    27907 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/generic/search.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1730 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/generic/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18208 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/generic/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    29216 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/generic/users.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1723 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/generic/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/generic/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6887 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/generic/misc.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    54885 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/generic/databases.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    12371 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/generic/filesystem.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/presto/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1701 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/presto/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2204 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/presto/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      678 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/presto/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      971 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/presto/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5279 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/presto/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      910 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/presto/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      671 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/presto/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/hsqldb/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1445 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/hsqldb/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2784 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/hsqldb/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      687 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/hsqldb/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      971 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/hsqldb/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5276 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/hsqldb/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      909 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/hsqldb/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2537 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/hsqldb/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/mssqlserver/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18049 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/mssqlserver/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2583 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/mssqlserver/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      889 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/mssqlserver/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6499 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/mssqlserver/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6913 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/mssqlserver/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      950 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/mssqlserver/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    17312 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/mssqlserver/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/access/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2525 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/access/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2130 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/access/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      670 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/access/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1011 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/access/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5843 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/access/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      919 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/access/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      691 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/access/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/raima/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2609 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/raima/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      520 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/raima/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      687 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/raima/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1035 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/raima/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2652 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/raima/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      899 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/raima/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      703 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/raima/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/derby/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1322 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/derby/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1830 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/derby/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      447 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/derby/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      995 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/derby/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2636 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/derby/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      907 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/derby/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/derby/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/cache/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1356 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/cache/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2397 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/cache/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      735 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/cache/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      967 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/cache/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3135 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/cache/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      900 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/cache/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/cache/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/vertica/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      459 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/vertica/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1920 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/vertica/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      689 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/vertica/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      975 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/vertica/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2992 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/vertica/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      920 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/vertica/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/vertica/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/firebird/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1080 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/firebird/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2260 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/firebird/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1151 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/firebird/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      979 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/firebird/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4990 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/firebird/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      929 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/firebird/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      675 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/firebird/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/monetdb/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1103 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/monetdb/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1894 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/monetdb/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      735 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/monetdb/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      975 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/monetdb/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2549 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/monetdb/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      920 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/monetdb/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/monetdb/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/maxdb/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     9202 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/maxdb/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      507 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/maxdb/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      447 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/maxdb/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      983 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/maxdb/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3792 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/maxdb/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      903 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/maxdb/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      678 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/maxdb/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/mimersql/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      926 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/mimersql/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1858 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/mimersql/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      807 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/mimersql/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      979 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/mimersql/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2591 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/mimersql/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      930 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/mimersql/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/mimersql/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/postgresql/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      428 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/postgresql/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2097 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/postgresql/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1016 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/postgresql/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5448 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/postgresql/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    10052 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/postgresql/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1304 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/postgresql/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3005 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/postgresql/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/mysql/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      265 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/mysql/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2095 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/mysql/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1044 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/mysql/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5124 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/mysql/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    12826 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/mysql/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1113 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/mysql/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7731 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/mysql/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/informix/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1022 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/informix/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1902 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/informix/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1272 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/informix/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      365 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/informix/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3284 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/informix/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      930 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/informix/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/informix/filesystem.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/altibase/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      589 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/altibase/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      506 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/altibase/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      678 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/altibase/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      979 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/altibase/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2657 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/altibase/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      930 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/altibase/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/altibase/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/extremedb/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2427 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/extremedb/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      507 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/extremedb/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      447 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/extremedb/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      983 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/extremedb/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2673 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/extremedb/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      939 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/extremedb/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      677 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/extremedb/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/mckoi/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2371 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/mckoi/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      503 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/mckoi/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      447 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/mckoi/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      967 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/mckoi/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2590 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/mckoi/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      899 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/mckoi/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      669 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/mckoi/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/db2/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      615 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/db2/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1935 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/db2/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      678 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/db2/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      365 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/db2/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5871 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/db2/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      880 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/db2/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/db2/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/cubrid/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      918 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/cubrid/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1835 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/cubrid/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      726 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/cubrid/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      971 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/cubrid/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2541 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/cubrid/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      910 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/cubrid/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/cubrid/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/h2/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1580 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/h2/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      500 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/h2/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      687 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/h2/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      955 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/h2/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3324 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/h2/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      869 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/h2/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      663 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/h2/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/oracle/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6002 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/oracle/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2817 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/oracle/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      886 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/oracle/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1101 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/oracle/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3880 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/oracle/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      909 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/oracle/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2301 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/oracle/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/cratedb/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      632 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/cratedb/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2097 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/cratedb/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      447 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/cratedb/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      975 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/cratedb/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2538 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/cratedb/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      920 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/cratedb/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/cratedb/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/sybase/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    11670 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/sybase/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2558 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/sybase/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      899 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/sybase/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      971 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/sybase/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3429 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/sybase/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      909 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/sybase/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      671 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/sybase/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/clickhouse/
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      638 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/clickhouse/enumeration.py
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      255 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/clickhouse/connector.py
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      687 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/clickhouse/syntax.py
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      987 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/clickhouse/takeover.py
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)     2627 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/clickhouse/fingerprint.py
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      950 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/clickhouse/__init__.py
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      679 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/clickhouse/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/sqlite/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2054 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/sqlite/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3083 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/sqlite/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      644 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/sqlite/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      971 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/sqlite/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3176 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/sqlite/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      909 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/sqlite/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      671 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/sqlite/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/virtuoso/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1541 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/virtuoso/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      506 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/virtuoso/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      678 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/virtuoso/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      979 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/virtuoso/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2517 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/virtuoso/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      929 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/virtuoso/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      675 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/virtuoso/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/frontbase/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      923 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/frontbase/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      507 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/frontbase/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      447 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/frontbase/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      983 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/frontbase/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2613 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/frontbase/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      939 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/frontbase/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      677 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/plugins/dbms/frontbase/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/lib/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/lib/controller/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     8896 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/controller/handler.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7233 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/controller/action.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    75900 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/controller/checks.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/controller/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    36817 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/controller/controller.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/lib/utils/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7984 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/utils/search.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4686 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/utils/httpd.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    48979 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/utils/hash.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2325 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/utils/getch.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5207 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/utils/sqlalchemy.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     8450 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/utils/hashdb.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2935 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/utils/xrange.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      926 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/utils/versioncheck.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3337 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/utils/progress.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2674 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/utils/purge.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    10977 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/utils/crawler.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     8030 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/utils/har.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    15901 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/utils/brute.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7369 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/utils/pivotdumptable.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/utils/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    34389 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/utils/api.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3190 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/utils/safe2bin.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1111 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/utils/timeout.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5564 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/utils/deps.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18275 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/utils/sgmllib.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/lib/request/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18899 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/request/basic.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6017 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/request/dns.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3229 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/request/direct.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     8399 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/request/redirecthandler.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      942 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/request/rangehandler.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      590 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/request/methodrequest.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5815 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/request/httpshandler.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/request/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      633 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/request/templates.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1384 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/request/basicauthhandler.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1566 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/request/chunkedhandler.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1158 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/request/pkihandler.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    24808 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/request/inject.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    80515 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/request/connect.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7788 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/request/comparison.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/lib/techniques/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/lib/techniques/error/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    21157 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/techniques/error/use.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/techniques/error/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/lib/techniques/dns/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5061 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/techniques/dns/use.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1125 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/techniques/dns/test.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/techniques/dns/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/lib/techniques/blind/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/techniques/blind/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    34684 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/techniques/blind/inference.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/techniques/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/lib/techniques/union/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    23147 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/techniques/union/use.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18664 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/techniques/union/test.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/techniques/union/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/lib/core/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      728 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/core/data.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5865 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/core/patch.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1800 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/core/readlineng.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    28848 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/core/dump.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     8414 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/core/threads.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    13586 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/core/convert.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    13936 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/core/enums.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2634 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/core/decorators.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6032 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/core/bigarray.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    10052 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/core/gui.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1646 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/core/exception.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    15264 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/core/testing.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7536 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/core/optiondict.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    34190 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/core/target.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1980 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/core/session.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    59654 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/core/agent.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)   106570 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/core/option.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    45400 2024-05-09 14:15:01.000000 sqlmap-1.8.5/sqlmap/lib/core/settings.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     8986 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/core/compat.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/core/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5657 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/core/subprocessng.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1876 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/core/revision.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      885 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/core/profiling.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      559 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/core/defaults.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5489 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/core/log.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4956 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/core/shell.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    17637 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/core/dicts.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3201 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/core/wordlist.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      988 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/core/unescaper.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7468 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/core/update.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5046 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/core/replication.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6646 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/core/datatype.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)   195224 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/core/common.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/lib/takeover/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     8440 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/takeover/abstraction.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    13903 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/takeover/udf.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    28236 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/takeover/metasploit.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    11839 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/takeover/xp_cmdshell.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3838 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/takeover/registry.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18315 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/takeover/web.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/takeover/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4739 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/takeover/icmpsh.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/lib/parse/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    50151 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/parse/cmdline.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2703 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/parse/handler.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3578 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/parse/payloads.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3596 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/parse/configfile.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1460 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/parse/headers.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1805 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/parse/sitemap.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/parse/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3580 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/parse/banner.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3022 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/lib/parse/html.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6215 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/sqlmapapi.yaml
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/extra/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/extra/cloak/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2286 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/cloak/cloak.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      732 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/cloak/README.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/cloak/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/extra/shutils/
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      305 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/shutils/modernize.sh
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      797 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/shutils/duplicates.py
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)     1368 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/shutils/precommit-hook.sh
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      332 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/shutils/pycodestyle.sh
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      660 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/shutils/drei.sh
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      255 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/shutils/blanks.sh
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      235 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/shutils/pylint.sh
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)     5923 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/shutils/pypi.sh
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      630 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/shutils/recloak.sh
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      903 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/shutils/newlines.py
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      869 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/shutils/strip.sh
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      245 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/shutils/junk.sh
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      311 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/shutils/autocompletion.sh
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      313 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/shutils/pydiatra.sh
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      875 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/shutils/postcommit-hook.sh
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      320 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/shutils/pyflakes.sh
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/extra/runcmd/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      193 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/runcmd/README.txt
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/extra/runcmd/src/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      883 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/runcmd/src/runcmd.sln
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      271 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/runcmd/src/README.txt
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/extra/runcmd/src/runcmd/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1348 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/runcmd/src/runcmd/runcmd.cpp
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      516 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/runcmd/src/runcmd/stdafx.h
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4508 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/runcmd/src/runcmd/runcmd.vcproj
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      293 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/runcmd/src/runcmd/stdafx.cpp
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    37206 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/runcmd/runcmd.exe_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/extra/beep/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2901 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/beep/beep.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/beep/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    46772 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/beep/beep.wav
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/extra/shellcodeexec/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/extra/shellcodeexec/linux/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1691 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/shellcodeexec/linux/shellcodeexec.x32_
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1927 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/shellcodeexec/linux/shellcodeexec.x64_
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      282 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/shellcodeexec/README.txt
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/extra/shellcodeexec/windows/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2758 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/shellcodeexec/windows/shellcodeexec.x32.exe_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/extra/icmpsh/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3965 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/icmpsh/icmpsh-m.c
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7009 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/icmpsh/icmpsh.exe_
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     9342 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/icmpsh/icmpsh-s.c
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1641 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/icmpsh/README.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2136 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/icmpsh/icmpsh-m.pl
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      872 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/icmpsh/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4809 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/icmpsh/icmpsh_m.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/extra/dbgtool/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2475 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/dbgtool/dbgtool.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      549 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/dbgtool/README.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/dbgtool/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap/extra/vulnserver/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     9127 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/vulnserver/vulnserver.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/extra/vulnserver/__init__.py
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)     4225 2024-05-09 14:14:57.000000 sqlmap-1.8.5/sqlmap/sqlmapapi.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)       38 2024-05-09 14:15:02.000000 sqlmap-1.8.5/setup.cfg
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3187 2024-05-09 14:15:01.000000 sqlmap-1.8.5/README.rst
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2024-05-09 14:15:02.000000 sqlmap-1.8.5/sqlmap.egg-info/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    24174 2024-05-09 14:15:01.000000 sqlmap-1.8.5/sqlmap.egg-info/SOURCES.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4946 2024-05-09 14:15:01.000000 sqlmap-1.8.5/sqlmap.egg-info/PKG-INFO
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        7 2024-05-09 14:15:01.000000 sqlmap-1.8.5/sqlmap.egg-info/top_level.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        1 2024-05-09 14:15:01.000000 sqlmap-1.8.5/sqlmap.egg-info/not-zip-safe
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)       47 2024-05-09 14:15:01.000000 sqlmap-1.8.5/sqlmap.egg-info/entry_points.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        1 2024-05-09 14:15:01.000000 sqlmap-1.8.5/sqlmap.egg-info/dependency_links.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1549 2024-05-09 14:14:59.000000 sqlmap-1.8.5/setup.py
```

### Comparing `sqlmap-1.8.4/MANIFEST.in` & `sqlmap-1.8.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/PKG-INFO` & `sqlmap-1.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: sqlmap
-Version: 1.8.4
+Version: 1.8.5
 Summary: Automatic SQL injection and database takeover tool
 Home-page: https://sqlmap.org
 Author: Bernardo Damele Assumpcao Guimaraes, Miroslav Stampar
 Author-email: bernardo@sqlmap.org, miroslav@sqlmap.org
 License: GNU General Public License v2 (GPLv2)
-Download-URL: https://github.com/sqlmapproject/sqlmap/archive/1.8.4.zip
+Download-URL: https://github.com/sqlmapproject/sqlmap/archive/1.8.5.zip
 Project-URL: Source, https://github.com/sqlmapproject/sqlmap/
 Project-URL: Documentation, https://github.com/sqlmapproject/sqlmap/wiki
 Project-URL: Tracker, https://github.com/sqlmapproject/sqlmap/issues
 Description: sqlmap
         ======
         
         |Python 2.6|2.7|3.x| |License| |Twitter|
```

### Comparing `sqlmap-1.8.4/sqlmap/README.md` & `sqlmap-1.8.5/sqlmap/README.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/wininetpton/win_inet_pton.py` & `sqlmap-1.8.5/sqlmap/thirdparty/wininetpton/win_inet_pton.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/clientform/clientform.py` & `sqlmap-1.8.5/sqlmap/thirdparty/clientform/clientform.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/multipart/multipartpost.py` & `sqlmap-1.8.5/sqlmap/thirdparty/multipart/multipartpost.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/socks/socks.py` & `sqlmap-1.8.5/sqlmap/thirdparty/socks/socks.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/socks/LICENSE` & `sqlmap-1.8.5/sqlmap/thirdparty/socks/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/chardet/escsm.py` & `sqlmap-1.8.5/sqlmap/thirdparty/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/chardet/eucjpprober.py` & `sqlmap-1.8.5/sqlmap/thirdparty/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/chardet/utf8prober.py` & `sqlmap-1.8.5/sqlmap/thirdparty/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/chardet/langturkishmodel.py` & `sqlmap-1.8.5/sqlmap/thirdparty/chardet/langturkishmodel.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/chardet/charsetprober.py` & `sqlmap-1.8.5/sqlmap/thirdparty/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/chardet/mbcharsetprober.py` & `sqlmap-1.8.5/sqlmap/thirdparty/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/chardet/euckrfreq.py` & `sqlmap-1.8.5/sqlmap/thirdparty/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/chardet/gb2312prober.py` & `sqlmap-1.8.5/sqlmap/thirdparty/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/chardet/cp949prober.py` & `sqlmap-1.8.5/sqlmap/thirdparty/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/chardet/chardistribution.py` & `sqlmap-1.8.5/sqlmap/thirdparty/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/chardet/enums.py` & `sqlmap-1.8.5/sqlmap/thirdparty/chardet/enums.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/chardet/langhebrewmodel.py` & `sqlmap-1.8.5/sqlmap/thirdparty/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/chardet/langgreekmodel.py` & `sqlmap-1.8.5/sqlmap/thirdparty/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/chardet/escprober.py` & `sqlmap-1.8.5/sqlmap/thirdparty/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/chardet/codingstatemachine.py` & `sqlmap-1.8.5/sqlmap/thirdparty/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/chardet/euctwfreq.py` & `sqlmap-1.8.5/sqlmap/thirdparty/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/chardet/latin1prober.py` & `sqlmap-1.8.5/sqlmap/thirdparty/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/chardet/langbulgarianmodel.py` & `sqlmap-1.8.5/sqlmap/thirdparty/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/chardet/big5freq.py` & `sqlmap-1.8.5/sqlmap/thirdparty/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/chardet/euckrprober.py` & `sqlmap-1.8.5/sqlmap/thirdparty/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/chardet/jisfreq.py` & `sqlmap-1.8.5/sqlmap/thirdparty/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/chardet/big5prober.py` & `sqlmap-1.8.5/sqlmap/thirdparty/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/chardet/mbcssm.py` & `sqlmap-1.8.5/sqlmap/thirdparty/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/chardet/universaldetector.py` & `sqlmap-1.8.5/sqlmap/thirdparty/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/chardet/gb2312freq.py` & `sqlmap-1.8.5/sqlmap/thirdparty/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/chardet/sjisprober.py` & `sqlmap-1.8.5/sqlmap/thirdparty/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/chardet/compat.py` & `sqlmap-1.8.5/sqlmap/thirdparty/chardet/compat.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/chardet/sbcsgroupprober.py` & `sqlmap-1.8.5/sqlmap/thirdparty/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/chardet/__init__.py` & `sqlmap-1.8.5/sqlmap/thirdparty/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/chardet/charsetgroupprober.py` & `sqlmap-1.8.5/sqlmap/thirdparty/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/chardet/jpcntx.py` & `sqlmap-1.8.5/sqlmap/thirdparty/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/chardet/langcyrillicmodel.py` & `sqlmap-1.8.5/sqlmap/thirdparty/chardet/langcyrillicmodel.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/chardet/langhungarianmodel.py` & `sqlmap-1.8.5/sqlmap/thirdparty/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/chardet/euctwprober.py` & `sqlmap-1.8.5/sqlmap/thirdparty/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/chardet/sbcharsetprober.py` & `sqlmap-1.8.5/sqlmap/thirdparty/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/chardet/mbcsgroupprober.py` & `sqlmap-1.8.5/sqlmap/thirdparty/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/chardet/langthaimodel.py` & `sqlmap-1.8.5/sqlmap/thirdparty/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/chardet/hebrewprober.py` & `sqlmap-1.8.5/sqlmap/thirdparty/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/odict/ordereddict.py` & `sqlmap-1.8.5/sqlmap/thirdparty/odict/ordereddict.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/keepalive/__init__.py` & `sqlmap-1.8.5/sqlmap/thirdparty/keepalive/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/keepalive/keepalive.py` & `sqlmap-1.8.5/sqlmap/thirdparty/keepalive/keepalive.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/magic/magic.py` & `sqlmap-1.8.5/sqlmap/thirdparty/magic/magic.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/ansistrm/ansistrm.py` & `sqlmap-1.8.5/sqlmap/thirdparty/ansistrm/ansistrm.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/identywaf/identYwaf.py` & `sqlmap-1.8.5/sqlmap/thirdparty/identywaf/identYwaf.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/identywaf/data.json` & `sqlmap-1.8.5/sqlmap/thirdparty/identywaf/data.json`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/identywaf/LICENSE` & `sqlmap-1.8.5/sqlmap/thirdparty/identywaf/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/prettyprint/__init__.py` & `sqlmap-1.8.5/sqlmap/thirdparty/prettyprint/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/prettyprint/prettyprint.py` & `sqlmap-1.8.5/sqlmap/thirdparty/prettyprint/prettyprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/bottle/bottle.py` & `sqlmap-1.8.5/sqlmap/thirdparty/bottle/bottle.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/fcrypt/__init__.py` & `sqlmap-1.8.5/sqlmap/thirdparty/fcrypt/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/fcrypt/fcrypt.py` & `sqlmap-1.8.5/sqlmap/thirdparty/fcrypt/fcrypt.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/pydes/pyDes.py` & `sqlmap-1.8.5/sqlmap/thirdparty/pydes/pyDes.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/pydes/__init__.py` & `sqlmap-1.8.5/sqlmap/thirdparty/pydes/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/beautifulsoup/beautifulsoup.py` & `sqlmap-1.8.5/sqlmap/thirdparty/beautifulsoup/beautifulsoup.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     notice, this list of conditions and the following disclaimer.
 
   * Redistributions in binary form must reproduce the above
     copyright notice, this list of conditions and the following
     disclaimer in the documentation and/or other materials provided
     with the distribution.
 
-  * Neither the name of the the Beautiful Soup Consortium and All
+  * Neither the name of the Beautiful Soup Consortium and All
     Night Kosher Bakery nor the names of its contributors may be
     used to endorse or promote products derived from this software
     without specific prior written permission.
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
 "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
 LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
```

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/beautifulsoup/__init__.py` & `sqlmap-1.8.5/sqlmap/thirdparty/beautifulsoup/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #     notice, this list of conditions and the following disclaimer.
 # 
 #   * Redistributions in binary form must reproduce the above
 #     copyright notice, this list of conditions and the following
 #     disclaimer in the documentation and/or other materials provided
 #     with the distribution.
 # 
-#   * Neither the name of the the Beautiful Soup Consortium and All
+#   * Neither the name of the Beautiful Soup Consortium and All
 #     Night Kosher Bakery nor the names of its contributors may be
 #     used to endorse or promote products derived from this software
 #     without specific prior written permission.
 # 
 # THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
 # "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
 # LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
```

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/six/__init__.py` & `sqlmap-1.8.5/sqlmap/thirdparty/six/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/termcolor/termcolor.py` & `sqlmap-1.8.5/sqlmap/thirdparty/termcolor/termcolor.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/colorama/ansi.py` & `sqlmap-1.8.5/sqlmap/thirdparty/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/colorama/initialise.py` & `sqlmap-1.8.5/sqlmap/thirdparty/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/colorama/winterm.py` & `sqlmap-1.8.5/sqlmap/thirdparty/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/colorama/ansitowin32.py` & `sqlmap-1.8.5/sqlmap/thirdparty/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/thirdparty/colorama/win32.py` & `sqlmap-1.8.5/sqlmap/thirdparty/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/.pylintrc` & `sqlmap-1.8.5/sqlmap/.pylintrc`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/procs/postgresql/dns_request.sql` & `sqlmap-1.8.5/sqlmap/data/procs/postgresql/dns_request.sql`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/procs/oracle/read_file_export_extension.sql` & `sqlmap-1.8.5/sqlmap/data/procs/oracle/read_file_export_extension.sql`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/9.1/lib_postgresqludf_sys.so_` & `sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/64/9.1/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/9.0/lib_postgresqludf_sys.so_` & `sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/64/9.0/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/9.5/lib_postgresqludf_sys.so_` & `sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/64/9.5/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/9.3/lib_postgresqludf_sys.so_` & `sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/64/9.3/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/12/lib_postgresqludf_sys.so_` & `sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/64/12/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/11/lib_postgresqludf_sys.so_` & `sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/64/11/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/8.4/lib_postgresqludf_sys.so_` & `sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/64/8.4/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/8.2/lib_postgresqludf_sys.so_` & `sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/64/8.2/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/8.3/lib_postgresqludf_sys.so_` & `sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/64/8.3/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/9.4/lib_postgresqludf_sys.so_` & `sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/64/9.4/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/10/lib_postgresqludf_sys.so_` & `sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/64/10/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/9.2/lib_postgresqludf_sys.so_` & `sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/64/9.2/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/64/9.6/lib_postgresqludf_sys.so_` & `sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/64/9.6/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/9.1/lib_postgresqludf_sys.so_` & `sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/32/9.1/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/9.0/lib_postgresqludf_sys.so_` & `sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/32/9.0/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/9.5/lib_postgresqludf_sys.so_` & `sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/32/9.5/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/9.3/lib_postgresqludf_sys.so_` & `sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/32/9.3/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/11/lib_postgresqludf_sys.so_` & `sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/32/11/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/8.4/lib_postgresqludf_sys.so_` & `sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/32/8.4/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/8.2/lib_postgresqludf_sys.so_` & `sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/32/8.2/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/8.3/lib_postgresqludf_sys.so_` & `sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/32/8.3/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/9.4/lib_postgresqludf_sys.so_` & `sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/32/9.4/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/10/lib_postgresqludf_sys.so_` & `sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/32/10/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/9.2/lib_postgresqludf_sys.so_` & `sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/32/9.2/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/udf/postgresql/linux/32/9.6/lib_postgresqludf_sys.so_` & `sqlmap-1.8.5/sqlmap/data/udf/postgresql/linux/32/9.6/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/udf/postgresql/windows/32/9.0/lib_postgresqludf_sys.dll_` & `sqlmap-1.8.5/sqlmap/data/udf/postgresql/windows/32/9.0/lib_postgresqludf_sys.dll_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/udf/postgresql/windows/32/8.4/lib_postgresqludf_sys.dll_` & `sqlmap-1.8.5/sqlmap/data/udf/postgresql/windows/32/8.4/lib_postgresqludf_sys.dll_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/udf/postgresql/windows/32/8.2/lib_postgresqludf_sys.dll_` & `sqlmap-1.8.5/sqlmap/data/udf/postgresql/windows/32/8.2/lib_postgresqludf_sys.dll_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/udf/postgresql/windows/32/8.3/lib_postgresqludf_sys.dll_` & `sqlmap-1.8.5/sqlmap/data/udf/postgresql/windows/32/8.3/lib_postgresqludf_sys.dll_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/udf/mysql/linux/64/lib_mysqludf_sys.so_` & `sqlmap-1.8.5/sqlmap/data/udf/mysql/linux/64/lib_mysqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/udf/mysql/linux/32/lib_mysqludf_sys.so_` & `sqlmap-1.8.5/sqlmap/data/udf/mysql/linux/32/lib_mysqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/udf/mysql/windows/64/lib_mysqludf_sys.dll_` & `sqlmap-1.8.5/sqlmap/data/udf/mysql/windows/64/lib_mysqludf_sys.dll_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/udf/mysql/windows/32/lib_mysqludf_sys.dll_` & `sqlmap-1.8.5/sqlmap/data/udf/mysql/windows/32/lib_mysqludf_sys.dll_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/shell/stagers/stager.asp_` & `sqlmap-1.8.5/sqlmap/data/shell/stagers/stager.asp_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/shell/stagers/stager.aspx_` & `sqlmap-1.8.5/sqlmap/data/shell/stagers/stager.aspx_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/shell/stagers/stager.jsp_` & `sqlmap-1.8.5/sqlmap/data/shell/stagers/stager.jsp_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/shell/README.txt` & `sqlmap-1.8.5/sqlmap/data/shell/README.txt`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/txt/smalldict.txt` & `sqlmap-1.8.5/sqlmap/data/txt/smalldict.txt`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/txt/common-outputs.txt` & `sqlmap-1.8.5/sqlmap/data/txt/common-outputs.txt`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/txt/common-tables.txt` & `sqlmap-1.8.5/sqlmap/data/txt/common-tables.txt`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/txt/user-agents.txt` & `sqlmap-1.8.5/sqlmap/data/txt/user-agents.txt`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/txt/sha256sums.txt` & `sqlmap-1.8.5/sqlmap/data/txt/sha256sums.txt`

 * *Files 1% similar despite different names*

```diff
@@ -149,27 +149,27 @@
 74fe683e94702bef6b8ea8eebb7fc47040e3ef5a03dec756e3cf4504a00c7839  extra/shutils/newlines.py
 fed05c468af662ba6ca6885baf8bf85fec1e58f438b3208f3819ad730a75a803  extra/shutils/postcommit-hook.sh
 dc35b51f5c9347eda8130106ee46bb051474fc0c5ed101f84abf3e546f729ceb  extra/shutils/precommit-hook.sh
 9a82c097f16a3062bd0e818bff12b4ec21b6f8f38b778604573a416589dfc450  extra/shutils/pycodestyle.sh
 fa1a42d189188770e82d536821d694626ca854438dadb9e08e143d3ece8c7e27  extra/shutils/pydiatra.sh
 5da7d1c86ca93313477d1deb0d6d4490798a2b63a2dd8729094184625b971e11  extra/shutils/pyflakes.sh
 c941be05376ba0a99d329e6de60e3b06b3fb261175070da6b1fc073d3afd5281  extra/shutils/pylint.sh
-bc2ceff560d11d696329bd976b14fbd8cddf428ad9f95eeb0a8f53e1afdc998b  extra/shutils/pypi.sh
+47b75c19b8c3dc6bca9e81918a838bd9261dac9c57366e75c4300c247dec2263  extra/shutils/pypi.sh
 df768bcb9838dc6c46dab9b4a877056cb4742bd6cfaaf438c4a3712c5cc0d264  extra/shutils/recloak.sh
 1972990a67caf2d0231eacf60e211acf545d9d0beeb3c145a49ba33d5d491b3f  extra/shutils/strip.sh
 99d0e94dd5fe60137abf48bfa051129fb251f5c40f0f7a270c89fbcb07323730  extra/vulnserver/__init__.py
 2ffe028b8b21306b6f528e62b214f43172fcf5bb59d317a13ba78e70155677ce  extra/vulnserver/vulnserver.py
 f9c96cd3fe99578bed9d49a8bdf8d76836d320a7c48c56eb0469f48b36775c35  lib/controller/action.py
 5d62d04edd432834df809707450a42778768ccc3c909eef6c6738ee780ffa884  lib/controller/checks.py
 34120f3ea85f4d69211642a263f963f08c97c20d47fd2ca082c23a5336d393f8  lib/controller/controller.py
 46d70b69cc7af0849242da5094a644568d7662a256a63e88ae485985b6dccf12  lib/controller/handler.py
 99d0e94dd5fe60137abf48bfa051129fb251f5c40f0f7a270c89fbcb07323730  lib/controller/__init__.py
 826c33f1105be4c0985e1bbe1d75bdb009c17815ad6552fc8d9bf39090d3c40f  lib/core/agent.py
 b2d69c99632da5c2acd0c0934e70d55862f1380a3f602cbe7456d617fb9c1fc9  lib/core/bigarray.py
-ba3f0002aa93f8f21f06dbea343573c590b9e6ec160fc6668c15e68a970cfb12  lib/core/common.py
+a4863238aba3a2d203c26127a4a7a6df873bd0c6f1cd798d4a7abcdc71a07cb6  lib/core/common.py
 5c26b0f308266bc3a9679ef837439e38d1dc7a69eac6bd3422280f49aaf114d2  lib/core/compat.py
 b60c96780cad4a257f91a0611b08cfcc52f242908c5d5ab2bf9034ef07869602  lib/core/convert.py
 5e381515873e71c395c77df00bf1dd8c4592afc6210a2f75cbc20daf384e539f  lib/core/data.py
 724b3f6f5bcd1479de19c7835577bcd8811f2ec72ccaebaf5b2dfdb8161a167d  lib/core/datatype.py
 55e7d63aae317763afcbdbea1c7731497c93bad14f6d032a0ccfffe72ffc121f  lib/core/decorators.py
 595c7dfde7c67cdb674fb019a24b07a501a9cdb6321e4f8ce3d3354cd9526eae  lib/core/defaults.py
 e8f6f1df8814b7b03c3eba22901837555083f66c99ee93b943911de785736bfa  lib/core/dicts.py
@@ -183,52 +183,52 @@
 33e0ec9ed38ae1ac74f1e2e3a1a246dee44c167723c9df69635793bfdbd971df  lib/core/option.py
 fdce95c552a097bf0dd44e5d6be2204c4c458d490e62c4d9d68fca5e2dc37c48  lib/core/patch.py
 bf77f9fc4296f239687297aee1fd6113b34f855965a6f690b52e26bd348cb353  lib/core/profiling.py
 4ccce0d53f467166d4084c9ef53a07f54cc352e75f785454a31c8a820511a84e  lib/core/readlineng.py
 4eff81c639a72b261c8ba1c876a01246e718e6626e8e77ae9cc6298b20a39355  lib/core/replication.py
 bbd1dcda835934728efc6d68686e9b0da72b09b3ee38f3c0ab78e8c18b0ba726  lib/core/revision.py
 eed6b0a21b3e69c5583133346b0639dc89937bd588887968ee85f8389d7c3c96  lib/core/session.py
-8c56685dbca6414a9b3c1dcc45249d41ab4677635edd8a5a68cc8ef5504d39da  lib/core/settings.py
+3f14500213dde69e2833c7f1e3c6c81695605f72ecc3ef0ebcc5df66a562231e  lib/core/settings.py
 2bec97d8a950f7b884e31dfe9410467f00d24f21b35672b95f8d68ed59685fd4  lib/core/shell.py
 e90a359b37a55c446c60e70ccd533f87276714d0b09e34f69b0740fd729ddbf8  lib/core/subprocessng.py
 54f7c70b4c7a9931f7ff3c1c12030180bde38e35a306d5e343ad6052919974cd  lib/core/target.py
-5941a7a641ea58b1d9e59ab3c9f4e9e40566ba08842e1cadb51ea8df9faf763f  lib/core/testing.py
+970b1c3e59481f11dd185bdde52f697f7d8dfc3152d24e3d336ec3fab59a857c  lib/core/testing.py
 8cb7424aa9d42d028a6780250effe4e719d9bb35558057f8ebe9e32408a6b80f  lib/core/threads.py
 ff39235aee7e33498c66132d17e6e86e7b8a29754e3fdecd880ca8356b17f791  lib/core/unescaper.py
 2984e4973868f586aa932f00da684bf31718c0331817c9f8721acd71fd661f89  lib/core/update.py
 ce65f9e8e1c726de3cec6abf31a2ffdbc16c251f772adcc14f67dee32d0f6b57  lib/core/wordlist.py
 99d0e94dd5fe60137abf48bfa051129fb251f5c40f0f7a270c89fbcb07323730  lib/__init__.py
 ba16fdd71fba31990dc92ff5a7388fb0ebac21ca905c314be6c8c2b868f94ab7  lib/parse/banner.py
 d757343f241b14e23aefb2177b6c2598f1bc06253fd93b0d8a28d4a55c267100  lib/parse/cmdline.py
-bcf0b32a730f1cdf097b00acf220eb216bc8eb4cb5d217a4a0d6ebe9f8086129  lib/parse/configfile.py
+d1fa3b9457f0e934600519309cbd3d84f9e6158a620866e7b352078c7c136f01  lib/parse/configfile.py
 9af4c86e41e50bd6055573a7b76e380a6658b355320c72dd6d2d5ddab14dc082  lib/parse/handler.py
 13b3ab678a2c422ce1dea9558668c05e562c0ec226f36053259a0be7280ebf92  lib/parse/headers.py
 b48edf3f30db127b18419f607894d5de46fc949d14c65fdc85ece524207d6dfd  lib/parse/html.py
 99d0e94dd5fe60137abf48bfa051129fb251f5c40f0f7a270c89fbcb07323730  lib/parse/__init__.py
 8743332261f8b0da52c94ca56510f0f2e856431c2bbe2164efdd3de605c2802b  lib/parse/payloads.py
 23adb7169e99554708062ff87ae795b90c6a284d1b5159eada974bf9f8d7583f  lib/parse/sitemap.py
 0acfa7da4b0dbc81652b018c3fdbb42512c8d7d5f01bbf9aef18e5ea7d38107a  lib/request/basicauthhandler.py
 c8446d4a50f06a50d7db18adc04c321e12cd2d0fa8b04bd58306511c89823316  lib/request/basic.py
 ead55e936dfc8941e512c8e8a4f644689387f331f4eed97854c558be3e227a91  lib/request/chunkedhandler.py
 06128c4e3e0e1fe34618de9d1fd5ee21292953dce4a3416567e200d2dfda79f2  lib/request/comparison.py
-00b23e22a65889829f4ffe65eea5e2bd5cf6ceab4f9b0f32b05047335b0b4a3e  lib/request/connect.py
+45f365239c48f2f6b8adc605b2f33b3522bda6e3248589dae909380434aaa0ad  lib/request/connect.py
 470e96857a7037a2d74b2c4b1c8c5d8379b76ea8cbdb1d8dd4367a7a852fa93c  lib/request/direct.py
 e802cc9099282764da0280172623600b6b9bb9fe1c87f352ade8be7a3f622585  lib/request/dns.py
 226226c2b8c906e0d0612ea68404c7f266e7a6685e0bf233e5456e10625b012d  lib/request/httpshandler.py
 99d0e94dd5fe60137abf48bfa051129fb251f5c40f0f7a270c89fbcb07323730  lib/request/__init__.py
 6944e07e5c061afea30494bcea5198c67b86dda1f291b80e75cb1f121490f1a7  lib/request/inject.py
 ba87a7bc91c1ec99a273284b9d0363358339aab0220651ff1ceddf3737ce2436  lib/request/methodrequest.py
 4ba939b6b9a130cd185e749c585afa2c4c8a5dbcbf8216ecc4f3199fe001b3e2  lib/request/pkihandler.py
 c6b222c0d34313cdea82fb39c8ead5d658400bf41e56aabd9640bdcf9bedc3a1  lib/request/rangehandler.py
 06bba7e3d77a3fb35e0b87420bb29bb1793f6dd7521fbfb063484575ac1c48e1  lib/request/redirecthandler.py
 9c5aab24a226acc093c62ca0b8c3736fb0dc2cf88ccbba85b323980a0f669d3e  lib/request/templates.py
 f07a4e40819dc2e7920f9291424761971a9769e4acfd34da223f24717563193c  lib/takeover/abstraction.py
 e775a0abe52c1a204c484ef212ff135c857cc8b7e2c94da23b5624c561ec4b9e  lib/takeover/icmpsh.py
 99d0e94dd5fe60137abf48bfa051129fb251f5c40f0f7a270c89fbcb07323730  lib/takeover/__init__.py
-d7ef25256e5f69b5a54569ad8b87ffa2045b5ed678e5bfbcea75136c0201b034  lib/takeover/metasploit.py
+c3d8c98a6d44d392f7b8572d3b35804f85838ddbc8e2a2f57af58f8e598af2f4  lib/takeover/metasploit.py
 a31b1bf60fcf58b7b735a64d73335212d5089e84051ff7883c14f6c73e055643  lib/takeover/registry.py
 90655344c9968e841eb809845e30da8cc60160390911345ac873be39d270467f  lib/takeover/udf.py
 145a9a8b7afb6504700faa1c61ca18eabab3253951788f29e7ee63c3ebff0e48  lib/takeover/web.py
 c4dc16a5ec302a504096f3caf0aa72e15c8b65bf03d9b62aa71bd4d384afec11  lib/takeover/xp_cmdshell.py
 6f87a9f4d9213363dd19bf687ff641ab76908e6ee67c79ec4b8fe831aad85e5d  lib/techniques/blind/inference.py
 99d0e94dd5fe60137abf48bfa051129fb251f5c40f0f7a270c89fbcb07323730  lib/techniques/blind/__init__.py
 99d0e94dd5fe60137abf48bfa051129fb251f5c40f0f7a270c89fbcb07323730  lib/techniques/dns/__init__.py
@@ -394,15 +394,15 @@
 88a613aa168a2ce241f8bf2233a1f00e6216aef17e469d0543b6c678d14e9ea1  plugins/dbms/mssqlserver/fingerprint.py
 376656382ddbfdbf0001cc92f09fc58692c7645fdaf40788b314130a01f99eb6  plugins/dbms/mssqlserver/__init__.py
 fdc3effe9320197795137dedb58e46c0409f19649889177443a2cbf58787c0dd  plugins/dbms/mssqlserver/syntax.py
 77ea4b1cd1491b3f1e2e98a8ff2e20ac300b693dd39b0c7330e0b29e233a00df  plugins/dbms/mssqlserver/takeover.py
 7f0165c085b0cb7d168d86acb790741c7ba12ad01ca9edf7972cfb184adb3ee9  plugins/dbms/mysql/connector.py
 05c4624b2729f13af2dd19286fc9276fc97c0f1ff19a31255785b7581fc232ae  plugins/dbms/mysql/enumeration.py
 9915fd436ea1783724b4fe12ea1d68fc3b838c37684a2c6dd01d53c739a1633f  plugins/dbms/mysql/filesystem.py
-ada995d6633ea737e8f12ba4a569ecb1bae9ffe7928c47ed0235f9de2d96f263  plugins/dbms/mysql/fingerprint.py
+bb5e22e286408100bcc0bd2d5f9d894ea0927c9300fa1635f4f6253590305b54  plugins/dbms/mysql/fingerprint.py
 ae824d447c1a59d055367aa9180acb42f7bb10df0006d4f99eeb12e43af563ae  plugins/dbms/mysql/__init__.py
 60fc1c647e31df191af2edfd26f99bf739fec53d3a8e1beb3bffdcf335c781fe  plugins/dbms/mysql/syntax.py
 784c31c2c0e19feb88bf5d21bfc7ae4bf04291922e40830da677577c5d5b4598  plugins/dbms/mysql/takeover.py
 6ae43c1d1a03f2e7a5c59890662f7609ebfd9ab7c26efb6ece85ae595335790e  plugins/dbms/oracle/connector.py
 ff648ca28dfbc9cbbd3f3c4ceb92ccaacfd0206e580629b7d22115c50ed7eb06  plugins/dbms/oracle/enumeration.py
 3a53b87decff154355b7c43742c0979323ae9ba3b34a6225a326ec787e85ce6d  plugins/dbms/oracle/filesystem.py
 f8c0c05b518dbcdb6b9a618e3fa33daefdb84bea6cb70521b7b58c7de9e6bf3a  plugins/dbms/oracle/fingerprint.py
@@ -469,15 +469,15 @@
 3c5f83d8c18443870ee0e1e61be2d65c175d9f02f0732885467e46a681bb9716  plugins/generic/misc.py
 83391b64fc6c16aba6ddc5cc2b737de35b2aa7b98f5eafe5d1ee2b067da50c64  plugins/generic/search.py
 978a495aaa3fc587e77572af96882a99aca7820f408fe1d4d0234a7ffb3972bb  plugins/generic/syntax.py
 fff84edc86b7d22dc01148fb10bb43d51cb9638dff21436fb94555db2a664766  plugins/generic/takeover.py
 0bc5c150e8cf4f892aba1ff15fc8938c387fb2a173b77329a0dc4cdb8b4bb4e2  plugins/generic/users.py
 99d0e94dd5fe60137abf48bfa051129fb251f5c40f0f7a270c89fbcb07323730  plugins/__init__.py
 d5b3243c2b048aa8074d2d828f74fbf8237286c3d00fd868f1b4090c267b78ef  README.md
-6cfaaf6534688cecda09433246d0a8518f98ce5cf6d6a8159f24d70502cfc14f  sqlmapapi.py
+78aafd53980096364f0c995c6283931bff505aed88fed1e7906fb06ee60e9c5b  sqlmapapi.py
 168309215af7dd5b0b71070e1770e72f1cbb29a3d8025143fb8aa0b88cd56b62  sqlmapapi.yaml
 5e172e315524845fe091aa0b7b29303c92ac8f67594c6d50f026d627e415b7ed  sqlmap.conf
 7800faa964d1fc06bbca856ca35bf21d68f5e044ae0bd5d7dea16d625d585adb  sqlmap.py
 adda508966db26c30b11390d6483c1fa25b092942a29730e739e1e50c403a21f  tamper/0eunion.py
 d38fe5ab97b401810612eae049325aa990c55143504b25cc9924810917511dee  tamper/apostrophemask.py
 8de713d1534d8cda171db4ceeb9f4324bcc030bbef21ffeaf60396c6bece31e4  tamper/apostrophenullencode.py
 661e45f350ecba30a030f09b921071f31061e21f3e961d10ce8f2fd182f4c1b2  tamper/appendnullbyte.py
@@ -545,16 +545,16 @@
 b4b03668061ba1a1dfc2e3a3db8ba500481da23f22b2bb1ebcbddada7479c3b0  tamper/uppercase.py
 3142a59cbcf2038bf9a50307576f3efea7a0dedf7701a4a4348ab47e9447fc34  tamper/varnish.py
 19ae32e01e44152d29b303eedfadb812bb216e7b4c37d42d8bd01fa02ea20864  tamper/versionedkeywords.py
 460988f86bcedf656dca61131b11d4926eb295c6affc8d36989435b4d21a74dd  tamper/versionedmorekeywords.py
 bd0fd06e24c3e05aecaccf5ba4c17d181e6cd35eee82c0efd6df5414fb0cb6f6  tamper/xforwardedfor.py
 55eaefc664bd8598329d535370612351ec8443c52465f0a37172ea46a97c458a  thirdparty/ansistrm/ansistrm.py
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  thirdparty/ansistrm/__init__.py
-82b6daf563d8c1933a8de655e04d6c8466d3db5c583c952e450d47ccc5c7c662  thirdparty/beautifulsoup/beautifulsoup.py
-bc92179cb2785712951fef05333290abf22e5b595e0a93d0168cc05132bc5f37  thirdparty/beautifulsoup/__init__.py
+e8f0ea4d982ef93c8c59c7165a1f39ccccddcb24b9fec1c2d2aa5bdb2373fdd5  thirdparty/beautifulsoup/beautifulsoup.py
+7d62c59f787f987cbce0de5375f604da8de0ba01742842fb2b3d12fcb92fcb63  thirdparty/beautifulsoup/__init__.py
 1b0f89e4713cc8cec4e4d824368a4eb9d3bdce7ddfc712326caac4feda1d7f69  thirdparty/bottle/bottle.py
 9f56e761d79bfdb34304a012586cb04d16b435ef6130091a97702e559260a2f2  thirdparty/bottle/__init__.py
 0ffccae46cb3a15b117acd0790b2738a5b45417d1b2822ceac57bdff10ef3bff  thirdparty/chardet/big5freq.py
 901c476dd7ad0693deef1ae56fe7bdf748a8b7ae20fde1922dddf6941eff8773  thirdparty/chardet/big5prober.py
 df0a164bad8aac6a282b2ab3e334129e315b2696ba57b834d9d68089b4f0725f  thirdparty/chardet/chardistribution.py
 e9b0eef1822246e49c5f871af4881bd14ebd4c0d8f1975c37a3e82738ffd90ee  thirdparty/chardet/charsetgroupprober.py
 2929b0244ae3ca9ca3d1b459982e45e5e33b73c61080b6088d95e29ed64db2d8  thirdparty/chardet/charsetprober.py
```

### Comparing `sqlmap-1.8.4/sqlmap/data/txt/common-files.txt` & `sqlmap-1.8.5/sqlmap/data/txt/common-files.txt`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/txt/keywords.txt` & `sqlmap-1.8.5/sqlmap/data/txt/keywords.txt`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/txt/common-columns.txt` & `sqlmap-1.8.5/sqlmap/data/txt/common-columns.txt`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/txt/wordlist.tx_` & `sqlmap-1.8.5/sqlmap/data/txt/wordlist.tx_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/html/index.html` & `sqlmap-1.8.5/sqlmap/data/html/index.html`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/xml/errors.xml` & `sqlmap-1.8.5/sqlmap/data/xml/errors.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/xml/payloads/union_query.xml` & `sqlmap-1.8.5/sqlmap/data/xml/payloads/union_query.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/xml/payloads/inline_query.xml` & `sqlmap-1.8.5/sqlmap/data/xml/payloads/inline_query.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/xml/payloads/error_based.xml` & `sqlmap-1.8.5/sqlmap/data/xml/payloads/error_based.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/xml/payloads/time_blind.xml` & `sqlmap-1.8.5/sqlmap/data/xml/payloads/time_blind.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/xml/payloads/stacked_queries.xml` & `sqlmap-1.8.5/sqlmap/data/xml/payloads/stacked_queries.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/xml/payloads/boolean_blind.xml` & `sqlmap-1.8.5/sqlmap/data/xml/payloads/boolean_blind.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/xml/queries.xml` & `sqlmap-1.8.5/sqlmap/data/xml/queries.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/xml/banner/x-powered-by.xml` & `sqlmap-1.8.5/sqlmap/data/xml/banner/x-powered-by.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/xml/banner/set-cookie.xml` & `sqlmap-1.8.5/sqlmap/data/xml/banner/set-cookie.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/xml/banner/mssql.xml` & `sqlmap-1.8.5/sqlmap/data/xml/banner/mssql.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/xml/banner/servlet-engine.xml` & `sqlmap-1.8.5/sqlmap/data/xml/banner/servlet-engine.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/xml/banner/generic.xml` & `sqlmap-1.8.5/sqlmap/data/xml/banner/generic.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/xml/banner/server.xml` & `sqlmap-1.8.5/sqlmap/data/xml/banner/server.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/xml/banner/mysql.xml` & `sqlmap-1.8.5/sqlmap/data/xml/banner/mysql.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/data/xml/boundaries.xml` & `sqlmap-1.8.5/sqlmap/data/xml/boundaries.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/between.py` & `sqlmap-1.8.5/sqlmap/tamper/between.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/symboliclogical.py` & `sqlmap-1.8.5/sqlmap/tamper/symboliclogical.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/misunion.py` & `sqlmap-1.8.5/sqlmap/tamper/misunion.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/schemasplit.py` & `sqlmap-1.8.5/sqlmap/tamper/schemasplit.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/dunion.py` & `sqlmap-1.8.5/sqlmap/tamper/dunion.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/least.py` & `sqlmap-1.8.5/sqlmap/tamper/least.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/substring2leftright.py` & `sqlmap-1.8.5/sqlmap/tamper/substring2leftright.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/concat2concatws.py` & `sqlmap-1.8.5/sqlmap/tamper/concat2concatws.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/luanginx.py` & `sqlmap-1.8.5/sqlmap/tamper/luanginx.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/apostrophemask.py` & `sqlmap-1.8.5/sqlmap/tamper/apostrophemask.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/space2mssqlblank.py` & `sqlmap-1.8.5/sqlmap/tamper/space2mssqlblank.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/0eunion.py` & `sqlmap-1.8.5/sqlmap/tamper/0eunion.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/randomcomments.py` & `sqlmap-1.8.5/sqlmap/tamper/randomcomments.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/plus2concat.py` & `sqlmap-1.8.5/sqlmap/tamper/plus2concat.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/varnish.py` & `sqlmap-1.8.5/sqlmap/tamper/varnish.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/multiplespaces.py` & `sqlmap-1.8.5/sqlmap/tamper/multiplespaces.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/versionedkeywords.py` & `sqlmap-1.8.5/sqlmap/tamper/versionedkeywords.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/space2mssqlhash.py` & `sqlmap-1.8.5/sqlmap/tamper/space2mssqlhash.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/informationschemacomment.py` & `sqlmap-1.8.5/sqlmap/tamper/informationschemacomment.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/ord2ascii.py` & `sqlmap-1.8.5/sqlmap/tamper/ord2ascii.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/versionedmorekeywords.py` & `sqlmap-1.8.5/sqlmap/tamper/versionedmorekeywords.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/apostrophenullencode.py` & `sqlmap-1.8.5/sqlmap/tamper/apostrophenullencode.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/percentage.py` & `sqlmap-1.8.5/sqlmap/tamper/percentage.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/sp_password.py` & `sqlmap-1.8.5/sqlmap/tamper/sp_password.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/equaltorlike.py` & `sqlmap-1.8.5/sqlmap/tamper/equaltorlike.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/plus2fnconcat.py` & `sqlmap-1.8.5/sqlmap/tamper/plus2fnconcat.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/halfversionedmorekeywords.py` & `sqlmap-1.8.5/sqlmap/tamper/halfversionedmorekeywords.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/space2morecomment.py` & `sqlmap-1.8.5/sqlmap/tamper/space2morecomment.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/modsecurityzeroversioned.py` & `sqlmap-1.8.5/sqlmap/tamper/modsecurityzeroversioned.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/greatest.py` & `sqlmap-1.8.5/sqlmap/tamper/greatest.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/bluecoat.py` & `sqlmap-1.8.5/sqlmap/tamper/bluecoat.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/uppercase.py` & `sqlmap-1.8.5/sqlmap/tamper/uppercase.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/space2hash.py` & `sqlmap-1.8.5/sqlmap/tamper/space2hash.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/overlongutf8more.py` & `sqlmap-1.8.5/sqlmap/tamper/overlongutf8more.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/decentities.py` & `sqlmap-1.8.5/sqlmap/tamper/decentities.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/space2dash.py` & `sqlmap-1.8.5/sqlmap/tamper/space2dash.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/modsecurityversioned.py` & `sqlmap-1.8.5/sqlmap/tamper/modsecurityversioned.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/hexentities.py` & `sqlmap-1.8.5/sqlmap/tamper/hexentities.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/charencode.py` & `sqlmap-1.8.5/sqlmap/tamper/charencode.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/equaltolike.py` & `sqlmap-1.8.5/sqlmap/tamper/equaltolike.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/chardoubleencode.py` & `sqlmap-1.8.5/sqlmap/tamper/chardoubleencode.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/scientific.py` & `sqlmap-1.8.5/sqlmap/tamper/scientific.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/space2comment.py` & `sqlmap-1.8.5/sqlmap/tamper/space2comment.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/unmagicquotes.py` & `sqlmap-1.8.5/sqlmap/tamper/unmagicquotes.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/xforwardedfor.py` & `sqlmap-1.8.5/sqlmap/tamper/xforwardedfor.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/space2plus.py` & `sqlmap-1.8.5/sqlmap/tamper/space2plus.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/charunicodeescape.py` & `sqlmap-1.8.5/sqlmap/tamper/charunicodeescape.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/space2morehash.py` & `sqlmap-1.8.5/sqlmap/tamper/space2morehash.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/ifnull2casewhenisnull.py` & `sqlmap-1.8.5/sqlmap/tamper/ifnull2casewhenisnull.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/ifnull2ifisnull.py` & `sqlmap-1.8.5/sqlmap/tamper/ifnull2ifisnull.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/commentbeforeparentheses.py` & `sqlmap-1.8.5/sqlmap/tamper/commentbeforeparentheses.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/sleep2getlock.py` & `sqlmap-1.8.5/sqlmap/tamper/sleep2getlock.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/lowercase.py` & `sqlmap-1.8.5/sqlmap/tamper/lowercase.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/commalessmid.py` & `sqlmap-1.8.5/sqlmap/tamper/commalessmid.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/charunicodeencode.py` & `sqlmap-1.8.5/sqlmap/tamper/charunicodeencode.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/space2mysqldash.py` & `sqlmap-1.8.5/sqlmap/tamper/space2mysqldash.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/hex2char.py` & `sqlmap-1.8.5/sqlmap/tamper/hex2char.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/randomcase.py` & `sqlmap-1.8.5/sqlmap/tamper/randomcase.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/appendnullbyte.py` & `sqlmap-1.8.5/sqlmap/tamper/appendnullbyte.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/base64encode.py` & `sqlmap-1.8.5/sqlmap/tamper/base64encode.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/space2randomblank.py` & `sqlmap-1.8.5/sqlmap/tamper/space2randomblank.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/binary.py` & `sqlmap-1.8.5/sqlmap/tamper/binary.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/if2case.py` & `sqlmap-1.8.5/sqlmap/tamper/if2case.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/overlongutf8.py` & `sqlmap-1.8.5/sqlmap/tamper/overlongutf8.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/space2mysqlblank.py` & `sqlmap-1.8.5/sqlmap/tamper/space2mysqlblank.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/htmlencode.py` & `sqlmap-1.8.5/sqlmap/tamper/htmlencode.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/tamper/commalesslimit.py` & `sqlmap-1.8.5/sqlmap/tamper/commalesslimit.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/sqlmap.py` & `sqlmap-1.8.5/sqlmap/sqlmap.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/doc/CHANGELOG.md` & `sqlmap-1.8.5/sqlmap/doc/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/doc/THANKS.md` & `sqlmap-1.8.5/sqlmap/doc/THANKS.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/doc/translations/README-it-IT.md` & `sqlmap-1.8.5/sqlmap/doc/translations/README-it-IT.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/doc/translations/README-uk-UA.md` & `sqlmap-1.8.5/sqlmap/doc/translations/README-uk-UA.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/doc/translations/README-ko-KR.md` & `sqlmap-1.8.5/sqlmap/doc/translations/README-ko-KR.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/doc/translations/README-rs-RS.md` & `sqlmap-1.8.5/sqlmap/doc/translations/README-rs-RS.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/doc/translations/README-in-HI.md` & `sqlmap-1.8.5/sqlmap/doc/translations/README-in-HI.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/doc/translations/README-fa-IR.md` & `sqlmap-1.8.5/sqlmap/doc/translations/README-fa-IR.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/doc/translations/README-bg-BG.md` & `sqlmap-1.8.5/sqlmap/doc/translations/README-bg-BG.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/doc/translations/README-ru-RU.md` & `sqlmap-1.8.5/sqlmap/doc/translations/README-ru-RU.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/doc/translations/README-id-ID.md` & `sqlmap-1.8.5/sqlmap/doc/translations/README-id-ID.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/doc/translations/README-fr-FR.md` & `sqlmap-1.8.5/sqlmap/doc/translations/README-fr-FR.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/doc/translations/README-pt-BR.md` & `sqlmap-1.8.5/sqlmap/doc/translations/README-pt-BR.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/doc/translations/README-hr-HR.md` & `sqlmap-1.8.5/sqlmap/doc/translations/README-hr-HR.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/doc/translations/README-nl-NL.md` & `sqlmap-1.8.5/sqlmap/doc/translations/README-nl-NL.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/doc/translations/README-sk-SK.md` & `sqlmap-1.8.5/sqlmap/doc/translations/README-sk-SK.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/doc/translations/README-vi-VN.md` & `sqlmap-1.8.5/sqlmap/doc/translations/README-vi-VN.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/doc/translations/README-pl-PL.md` & `sqlmap-1.8.5/sqlmap/doc/translations/README-pl-PL.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/doc/translations/README-gr-GR.md` & `sqlmap-1.8.5/sqlmap/doc/translations/README-gr-GR.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/doc/translations/README-zh-CN.md` & `sqlmap-1.8.5/sqlmap/doc/translations/README-zh-CN.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/doc/translations/README-ja-JP.md` & `sqlmap-1.8.5/sqlmap/doc/translations/README-ja-JP.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/doc/translations/README-ka-GE.md` & `sqlmap-1.8.5/sqlmap/doc/translations/README-ka-GE.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/doc/translations/README-tr-TR.md` & `sqlmap-1.8.5/sqlmap/doc/translations/README-tr-TR.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/doc/translations/README-de-DE.md` & `sqlmap-1.8.5/sqlmap/doc/translations/README-de-DE.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/doc/translations/README-es-MX.md` & `sqlmap-1.8.5/sqlmap/doc/translations/README-es-MX.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/doc/THIRD-PARTY.md` & `sqlmap-1.8.5/sqlmap/doc/THIRD-PARTY.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/sqlmap.conf` & `sqlmap-1.8.5/sqlmap/sqlmap.conf`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/LICENSE` & `sqlmap-1.8.5/sqlmap/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/generic/enumeration.py` & `sqlmap-1.8.5/sqlmap/plugins/generic/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/generic/connector.py` & `sqlmap-1.8.5/sqlmap/plugins/generic/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/generic/custom.py` & `sqlmap-1.8.5/sqlmap/plugins/generic/custom.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/generic/entries.py` & `sqlmap-1.8.5/sqlmap/plugins/generic/entries.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/generic/search.py` & `sqlmap-1.8.5/sqlmap/plugins/generic/search.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/generic/syntax.py` & `sqlmap-1.8.5/sqlmap/plugins/generic/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/generic/takeover.py` & `sqlmap-1.8.5/sqlmap/plugins/generic/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/generic/users.py` & `sqlmap-1.8.5/sqlmap/plugins/generic/users.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/generic/fingerprint.py` & `sqlmap-1.8.5/sqlmap/plugins/generic/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/generic/misc.py` & `sqlmap-1.8.5/sqlmap/plugins/generic/misc.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/generic/databases.py` & `sqlmap-1.8.5/sqlmap/plugins/generic/databases.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/generic/filesystem.py` & `sqlmap-1.8.5/sqlmap/plugins/generic/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/presto/enumeration.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/presto/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/presto/connector.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/presto/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/presto/syntax.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/presto/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/presto/takeover.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/presto/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/presto/fingerprint.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/presto/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/presto/__init__.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/presto/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/presto/filesystem.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/presto/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/hsqldb/enumeration.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/hsqldb/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/hsqldb/connector.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/hsqldb/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/hsqldb/syntax.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/hsqldb/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/hsqldb/takeover.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/hsqldb/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/hsqldb/fingerprint.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/hsqldb/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/hsqldb/__init__.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/hsqldb/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/hsqldb/filesystem.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/hsqldb/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/mssqlserver/enumeration.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/mssqlserver/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/mssqlserver/connector.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/mssqlserver/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/mssqlserver/syntax.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/mssqlserver/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/mssqlserver/takeover.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/mssqlserver/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/mssqlserver/fingerprint.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/mssqlserver/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/mssqlserver/__init__.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/mssqlserver/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/mssqlserver/filesystem.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/mssqlserver/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/access/enumeration.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/access/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/access/connector.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/access/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/access/syntax.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/access/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/access/takeover.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/access/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/access/fingerprint.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/access/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/access/__init__.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/access/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/access/filesystem.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/access/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/raima/enumeration.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/raima/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/raima/connector.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/raima/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/raima/syntax.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/raima/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/raima/takeover.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/raima/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/raima/fingerprint.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/raima/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/raima/__init__.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/raima/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/raima/filesystem.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/raima/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/derby/enumeration.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/derby/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/derby/connector.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/derby/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/derby/takeover.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/derby/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/derby/fingerprint.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/derby/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/derby/__init__.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/derby/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/cache/enumeration.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/cache/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/cache/connector.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/cache/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/cache/syntax.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/cache/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/cache/takeover.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/cache/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/cache/fingerprint.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/cache/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/cache/__init__.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/vertica/connector.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/vertica/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/vertica/syntax.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/vertica/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/vertica/takeover.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/vertica/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/vertica/fingerprint.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/vertica/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/vertica/__init__.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/vertica/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/firebird/enumeration.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/firebird/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/firebird/connector.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/firebird/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/firebird/syntax.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/firebird/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/firebird/takeover.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/firebird/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/firebird/fingerprint.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/firebird/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/firebird/__init__.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/firebird/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/firebird/filesystem.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/firebird/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/monetdb/enumeration.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/monetdb/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/monetdb/connector.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/monetdb/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/monetdb/syntax.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/monetdb/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/monetdb/takeover.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/monetdb/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/monetdb/fingerprint.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/monetdb/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/monetdb/__init__.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/monetdb/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/maxdb/enumeration.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/maxdb/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/maxdb/takeover.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/maxdb/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/maxdb/fingerprint.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/maxdb/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/maxdb/__init__.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/maxdb/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/maxdb/filesystem.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/maxdb/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/mimersql/enumeration.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/mimersql/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/mimersql/connector.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/mimersql/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/mimersql/syntax.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/mimersql/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/mimersql/takeover.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/mimersql/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/mimersql/fingerprint.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/mimersql/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/mimersql/__init__.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/mimersql/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/postgresql/connector.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/postgresql/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/postgresql/syntax.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/postgresql/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/postgresql/takeover.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/postgresql/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/postgresql/fingerprint.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/postgresql/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/postgresql/__init__.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/postgresql/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/postgresql/filesystem.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/postgresql/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/mysql/connector.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/mysql/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/mysql/syntax.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/mysql/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/mysql/takeover.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/mysql/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/mysql/fingerprint.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/mysql/fingerprint.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,18 +41,19 @@
 
             return None
 
         # Reference: https://downloads.mysql.com/archives/community/
         # Reference: https://dev.mysql.com/doc/relnotes/mysql/<major>.<minor>/en/
 
         versions = (
+            (80200, 80202),  # MySQL 8.2
             (80100, 80102),  # MySQL 8.1
-            (80000, 80035),  # MySQL 8.0
+            (80000, 80036),  # MySQL 8.0
             (60000, 60014),  # MySQL 6.0
-            (50700, 50744),  # MySQL 5.7
+            (50700, 50745),  # MySQL 5.7
             (50600, 50652),  # MySQL 5.6
             (50500, 50563),  # MySQL 5.5
             (50400, 50404),  # MySQL 5.4
             (50100, 50174),  # MySQL 5.1
             (50000, 50097),  # MySQL 5.0
             (40100, 40131),  # MySQL 4.1
             (40000, 40032),  # MySQL 4.0
```

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/mysql/__init__.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/mysql/filesystem.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/mysql/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/informix/enumeration.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/informix/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/informix/connector.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/informix/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/informix/syntax.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/informix/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/informix/fingerprint.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/informix/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/informix/__init__.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/informix/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/altibase/enumeration.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/altibase/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/altibase/syntax.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/altibase/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/altibase/takeover.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/altibase/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/altibase/fingerprint.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/altibase/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/altibase/__init__.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/altibase/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/extremedb/enumeration.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/extremedb/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/extremedb/takeover.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/extremedb/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/extremedb/fingerprint.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/extremedb/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/extremedb/__init__.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/extremedb/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/extremedb/filesystem.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/extremedb/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/mckoi/enumeration.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/mckoi/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/mckoi/takeover.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/mckoi/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/mckoi/fingerprint.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/mckoi/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/mckoi/__init__.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/mckoi/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/mckoi/filesystem.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/mckoi/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/db2/enumeration.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/db2/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/db2/connector.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/db2/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/db2/syntax.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/db2/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/db2/fingerprint.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/db2/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/db2/__init__.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/db2/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/cubrid/enumeration.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/cubrid/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/cubrid/connector.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/cubrid/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/cubrid/syntax.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/cubrid/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/cubrid/takeover.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/cubrid/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/cubrid/fingerprint.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/cubrid/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/cubrid/__init__.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/cubrid/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/h2/enumeration.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/h2/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/h2/syntax.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/h2/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/h2/takeover.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/h2/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/h2/fingerprint.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/h2/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/h2/__init__.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/h2/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/h2/filesystem.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/h2/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/oracle/enumeration.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/oracle/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/oracle/connector.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/oracle/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/oracle/syntax.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/oracle/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/oracle/takeover.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/oracle/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/oracle/fingerprint.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/oracle/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/oracle/__init__.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/oracle/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/oracle/filesystem.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/oracle/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/cratedb/enumeration.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/cratedb/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/cratedb/connector.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/cratedb/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/cratedb/takeover.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/cratedb/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/cratedb/fingerprint.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/cratedb/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/cratedb/__init__.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/cratedb/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/sybase/enumeration.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/sybase/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/sybase/connector.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/sybase/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/sybase/syntax.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/sybase/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/sybase/takeover.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/sybase/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/sybase/fingerprint.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/sybase/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/sybase/__init__.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/sybase/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/sybase/filesystem.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/sybase/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/clickhouse/enumeration.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/clickhouse/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/clickhouse/syntax.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/clickhouse/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/clickhouse/takeover.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/clickhouse/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/clickhouse/fingerprint.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/clickhouse/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/clickhouse/__init__.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/clickhouse/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/clickhouse/filesystem.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/clickhouse/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/sqlite/enumeration.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/sqlite/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/sqlite/connector.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/sqlite/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/sqlite/syntax.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/sqlite/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/sqlite/takeover.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/sqlite/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/sqlite/fingerprint.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/sqlite/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/sqlite/__init__.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/sqlite/filesystem.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/sqlite/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/virtuoso/enumeration.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/virtuoso/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/virtuoso/syntax.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/virtuoso/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/virtuoso/takeover.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/virtuoso/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/virtuoso/fingerprint.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/virtuoso/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/virtuoso/__init__.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/virtuoso/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/virtuoso/filesystem.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/virtuoso/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/frontbase/enumeration.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/frontbase/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/frontbase/takeover.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/frontbase/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/frontbase/fingerprint.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/frontbase/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/frontbase/__init__.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/frontbase/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/plugins/dbms/frontbase/filesystem.py` & `sqlmap-1.8.5/sqlmap/plugins/dbms/frontbase/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/controller/handler.py` & `sqlmap-1.8.5/sqlmap/lib/controller/handler.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/controller/action.py` & `sqlmap-1.8.5/sqlmap/lib/controller/action.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/controller/checks.py` & `sqlmap-1.8.5/sqlmap/lib/controller/checks.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/controller/controller.py` & `sqlmap-1.8.5/sqlmap/lib/controller/controller.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/utils/search.py` & `sqlmap-1.8.5/sqlmap/lib/utils/search.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/utils/httpd.py` & `sqlmap-1.8.5/sqlmap/lib/utils/httpd.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/utils/hash.py` & `sqlmap-1.8.5/sqlmap/lib/utils/hash.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/utils/getch.py` & `sqlmap-1.8.5/sqlmap/lib/utils/getch.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/utils/sqlalchemy.py` & `sqlmap-1.8.5/sqlmap/lib/utils/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/utils/hashdb.py` & `sqlmap-1.8.5/sqlmap/lib/utils/hashdb.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/utils/xrange.py` & `sqlmap-1.8.5/sqlmap/lib/utils/xrange.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/utils/versioncheck.py` & `sqlmap-1.8.5/sqlmap/lib/utils/versioncheck.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/utils/progress.py` & `sqlmap-1.8.5/sqlmap/lib/utils/progress.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/utils/purge.py` & `sqlmap-1.8.5/sqlmap/lib/utils/purge.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/utils/crawler.py` & `sqlmap-1.8.5/sqlmap/lib/utils/crawler.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/utils/har.py` & `sqlmap-1.8.5/sqlmap/lib/utils/har.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/utils/brute.py` & `sqlmap-1.8.5/sqlmap/lib/utils/brute.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/utils/pivotdumptable.py` & `sqlmap-1.8.5/sqlmap/lib/utils/pivotdumptable.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/utils/api.py` & `sqlmap-1.8.5/sqlmap/lib/utils/api.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/utils/safe2bin.py` & `sqlmap-1.8.5/sqlmap/lib/utils/safe2bin.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/utils/timeout.py` & `sqlmap-1.8.5/sqlmap/lib/utils/timeout.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/utils/deps.py` & `sqlmap-1.8.5/sqlmap/lib/utils/deps.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/utils/sgmllib.py` & `sqlmap-1.8.5/sqlmap/lib/utils/sgmllib.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/request/basic.py` & `sqlmap-1.8.5/sqlmap/lib/request/basic.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/request/dns.py` & `sqlmap-1.8.5/sqlmap/lib/request/dns.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/request/direct.py` & `sqlmap-1.8.5/sqlmap/lib/request/direct.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/request/redirecthandler.py` & `sqlmap-1.8.5/sqlmap/lib/request/redirecthandler.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/request/rangehandler.py` & `sqlmap-1.8.5/sqlmap/lib/request/rangehandler.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/request/methodrequest.py` & `sqlmap-1.8.5/sqlmap/lib/request/methodrequest.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/request/httpshandler.py` & `sqlmap-1.8.5/sqlmap/lib/request/httpshandler.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/request/templates.py` & `sqlmap-1.8.5/sqlmap/lib/request/templates.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/request/basicauthhandler.py` & `sqlmap-1.8.5/sqlmap/lib/request/basicauthhandler.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/request/chunkedhandler.py` & `sqlmap-1.8.5/sqlmap/lib/request/chunkedhandler.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/request/pkihandler.py` & `sqlmap-1.8.5/sqlmap/lib/request/pkihandler.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/request/inject.py` & `sqlmap-1.8.5/sqlmap/lib/request/inject.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/request/connect.py` & `sqlmap-1.8.5/sqlmap/lib/request/connect.py`

 * *Files 0% similar despite different names*

```diff
@@ -910,28 +910,28 @@
             elif kb.testMode or kb.multiThreadMode:
                 logger.critical(warnMsg)
                 return None, None, None
             else:
                 raise SqlmapConnectionException(warnMsg)
 
         finally:
-            if isinstance(page, six.binary_type):
-                if HTTP_HEADER.CONTENT_TYPE in (responseHeaders or {}) and not re.search(TEXT_CONTENT_TYPE_REGEX, responseHeaders[HTTP_HEADER.CONTENT_TYPE]):
-                    page = six.text_type(page, errors="ignore")
-                else:
-                    page = getUnicode(page)
-
             for function in kb.postprocessFunctions:
                 try:
                     page, responseHeaders, code = function(page, responseHeaders, code)
                 except Exception as ex:
                     errMsg = "error occurred while running postprocess "
                     errMsg += "function '%s' ('%s')" % (function.__name__, getSafeExString(ex))
                     raise SqlmapGenericException(errMsg)
 
+            if isinstance(page, six.binary_type):
+                if HTTP_HEADER.CONTENT_TYPE in (responseHeaders or {}) and not re.search(TEXT_CONTENT_TYPE_REGEX, responseHeaders[HTTP_HEADER.CONTENT_TYPE]):
+                    page = six.text_type(page, errors="ignore")
+                else:
+                    page = getUnicode(page)
+
             for _ in (getattr(conn, "redcode", None), code):
                 if _ is not None and _ in conf.abortCode:
                     errMsg = "aborting due to detected HTTP code '%d'" % _
                     singleTimeLogMessage(errMsg, logging.CRITICAL)
                     raise SystemExit
 
             threadData.lastPage = page
@@ -1179,15 +1179,15 @@
                 if urlencode(parameter) in paramString:
                     parameter = urlencode(parameter)
 
                 match = re.search(r"%s=[^&]*" % re.escape(parameter), paramString, re.I)
                 if match:
                     retVal = re.sub(r"(?i)%s" % re.escape(match.group(0)), ("%s=%s" % (parameter, newValue)).replace('\\', r'\\'), paramString)
                 else:
-                    match = re.search(r"(%s[\"']:[\"'])([^\"']+)" % re.escape(parameter), paramString, re.I)
+                    match = re.search(r"(%s[\"']\s*:\s*[\"'])([^\"']*)" % re.escape(parameter), paramString, re.I)
                     if match:
                         retVal = re.sub(r"(?i)%s" % re.escape(match.group(0)), "%s%s" % (match.group(1), newValue), paramString)
 
                 return retVal
 
             for attempt in xrange(conf.csrfRetries + 1):
                 if token:
```

### Comparing `sqlmap-1.8.4/sqlmap/lib/request/comparison.py` & `sqlmap-1.8.5/sqlmap/lib/request/comparison.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/techniques/error/use.py` & `sqlmap-1.8.5/sqlmap/lib/techniques/error/use.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/techniques/dns/use.py` & `sqlmap-1.8.5/sqlmap/lib/techniques/dns/use.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/techniques/dns/test.py` & `sqlmap-1.8.5/sqlmap/lib/techniques/dns/test.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/techniques/blind/inference.py` & `sqlmap-1.8.5/sqlmap/lib/techniques/blind/inference.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/techniques/union/use.py` & `sqlmap-1.8.5/sqlmap/lib/techniques/union/use.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/techniques/union/test.py` & `sqlmap-1.8.5/sqlmap/lib/techniques/union/test.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/core/data.py` & `sqlmap-1.8.5/sqlmap/lib/core/data.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/core/patch.py` & `sqlmap-1.8.5/sqlmap/lib/core/patch.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/core/readlineng.py` & `sqlmap-1.8.5/sqlmap/lib/core/readlineng.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/core/dump.py` & `sqlmap-1.8.5/sqlmap/lib/core/dump.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/core/threads.py` & `sqlmap-1.8.5/sqlmap/lib/core/threads.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/core/convert.py` & `sqlmap-1.8.5/sqlmap/lib/core/convert.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/core/enums.py` & `sqlmap-1.8.5/sqlmap/lib/core/enums.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/core/decorators.py` & `sqlmap-1.8.5/sqlmap/lib/core/decorators.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/core/bigarray.py` & `sqlmap-1.8.5/sqlmap/lib/core/bigarray.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/core/gui.py` & `sqlmap-1.8.5/sqlmap/lib/core/gui.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/core/exception.py` & `sqlmap-1.8.5/sqlmap/lib/core/exception.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/core/testing.py` & `sqlmap-1.8.5/sqlmap/lib/core/testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,15 +158,17 @@
         f.flush()
 
     base = "http://%s:%d/" % (address, port)
     url = "%s?id=1" % base
     direct = "sqlite3://%s" % database
     tmpdir = tempfile.mkdtemp()
 
-    content = open(os.path.abspath(os.path.join(os.path.dirname(__file__), "..", "..", "sqlmap.conf"))).read().replace("url =", "url = %s" % url)
+    with open(os.path.abspath(os.path.join(os.path.dirname(__file__), "..", "..", "sqlmap.conf"))) as f:
+        content = f.read().replace("url =", "url = %s" % url)
+
     with open(config, "w+") as f:
         f.write(content)
         f.flush()
 
     content = "%s?%s=%d\n%s?%s=%d\n%s&%s=1" % (base, randomStr(), randomInt(), base, randomStr(), randomInt(), url, randomStr())
     with open(multiple, "w+") as f:
         f.write(content)
@@ -210,15 +212,17 @@
 def smokeTest():
     """
     Runs the basic smoke testing of a program
     """
 
     unisonRandom()
 
-    content = open(paths.ERRORS_XML, "r").read()
+    with open(paths.ERRORS_XML, "r") as f:
+        content = f.read()
+
     for regex in re.findall(r'<error regexp="(.+?)"/>', content):
         try:
             re.compile(regex)
         except re.error:
             errMsg = "smoke test failed at compiling '%s'" % regex
             logger.error(errMsg)
             return False
```

### Comparing `sqlmap-1.8.4/sqlmap/lib/core/optiondict.py` & `sqlmap-1.8.5/sqlmap/lib/core/optiondict.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/core/target.py` & `sqlmap-1.8.5/sqlmap/lib/core/target.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/core/session.py` & `sqlmap-1.8.5/sqlmap/lib/core/session.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/core/agent.py` & `sqlmap-1.8.5/sqlmap/lib/core/agent.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/core/option.py` & `sqlmap-1.8.5/sqlmap/lib/core/option.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/core/settings.py` & `sqlmap-1.8.5/sqlmap/lib/core/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from lib.core.enums import DBMS
 from lib.core.enums import DBMS_DIRECTORY_NAME
 from lib.core.enums import OS
 from thirdparty import six
 from thirdparty.six import unichr as _unichr
 
 # sqlmap version (<major>.<minor>.<month>.<monthly commit>)
-VERSION = "1.8.4"
+VERSION = "1.8.5"
 TYPE = "pip"
 TYPE_COLORS = {"dev": 33, "stable": 90, "pip": 34}
 VERSION_STRING = "sqlmap/%s#%s" % ('.'.join(VERSION.split('.')[:-1]) if VERSION.count('.') > 2 and VERSION.split('.')[-1] == '0' else VERSION, TYPE)
 DESCRIPTION = "automatic SQL injection and database takeover tool"
 SITE = "https://sqlmap.org"
 DEFAULT_USER_AGENT = "%s (%s)" % (VERSION_STRING, SITE)
 DEV_EMAIL_ADDRESS = "dev@sqlmap.org"
```

### Comparing `sqlmap-1.8.4/sqlmap/lib/core/compat.py` & `sqlmap-1.8.5/sqlmap/lib/core/compat.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/core/subprocessng.py` & `sqlmap-1.8.5/sqlmap/lib/core/subprocessng.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/core/revision.py` & `sqlmap-1.8.5/sqlmap/lib/core/revision.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/core/profiling.py` & `sqlmap-1.8.5/sqlmap/lib/core/profiling.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/core/defaults.py` & `sqlmap-1.8.5/sqlmap/lib/core/defaults.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/core/log.py` & `sqlmap-1.8.5/sqlmap/lib/core/log.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/core/shell.py` & `sqlmap-1.8.5/sqlmap/lib/core/shell.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/core/dicts.py` & `sqlmap-1.8.5/sqlmap/lib/core/dicts.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/core/wordlist.py` & `sqlmap-1.8.5/sqlmap/lib/core/wordlist.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/core/unescaper.py` & `sqlmap-1.8.5/sqlmap/lib/core/unescaper.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/core/update.py` & `sqlmap-1.8.5/sqlmap/lib/core/update.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/core/replication.py` & `sqlmap-1.8.5/sqlmap/lib/core/replication.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/core/datatype.py` & `sqlmap-1.8.5/sqlmap/lib/core/datatype.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/core/common.py` & `sqlmap-1.8.5/sqlmap/lib/core/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -1329,15 +1329,18 @@
 
     >>> isZipFile(paths.WORDLIST)
     True
     """
 
     checkFile(filename)
 
-    return openFile(filename, "rb", encoding=None).read(len(ZIP_HEADER)) == ZIP_HEADER
+    with openFile(filename, "rb", encoding=None) as f:
+        header = f.read(len(ZIP_HEADER))
+
+    return header == ZIP_HEADER
 
 def isDigit(value):
     """
     Checks if provided (string) value consists of digits (Note: Python's isdigit() is problematic)
 
     >>> u'\xb2'.isdigit()
     True
@@ -2529,29 +2532,30 @@
     >>> initCommonOutputs(); "information_schema" in kb.commonOutputs["Databases"]
     True
     """
 
     kb.commonOutputs = {}
     key = None
 
-    for line in openFile(paths.COMMON_OUTPUTS, 'r'):
-        if line.find('#') != -1:
-            line = line[:line.find('#')]
-
-        line = line.strip()
-
-        if len(line) > 1:
-            if line.startswith('[') and line.endswith(']'):
-                key = line[1:-1]
-            elif key:
-                if key not in kb.commonOutputs:
-                    kb.commonOutputs[key] = set()
+    with openFile(paths.COMMON_OUTPUTS, 'r') as f:
+        for line in f:
+            if line.find('#') != -1:
+                line = line[:line.find('#')]
+
+            line = line.strip()
+
+            if len(line) > 1:
+                if line.startswith('[') and line.endswith(']'):
+                    key = line[1:-1]
+                elif key:
+                    if key not in kb.commonOutputs:
+                        kb.commonOutputs[key] = set()
 
-                if line not in kb.commonOutputs[key]:
-                    kb.commonOutputs[key].add(line)
+                    if line not in kb.commonOutputs[key]:
+                        kb.commonOutputs[key].add(line)
 
 def getFileItems(filename, commentPrefix='#', unicoded=True, lowercase=False, unique=False):
     """
     Returns newline delimited items contained inside file
 
     >>> "SELECT" in getFileItems(paths.SQL_KEYWORDS)
     True
@@ -5590,12 +5594,14 @@
     if paths.get("DIGEST_FILE"):
         for entry in getFileItems(paths.DIGEST_FILE):
             match = re.search(r"([0-9a-f]+)\s+([^\s]+)", entry)
             if match:
                 expected, filename = match.groups()
                 filepath = os.path.join(paths.SQLMAP_ROOT_PATH, filename).replace('/', os.path.sep)
                 checkFile(filepath)
-                if not hashlib.sha256(open(filepath, "rb").read()).hexdigest() == expected:
+                with open(filepath, "rb") as f:
+                    content = f.read()
+                if not hashlib.sha256(content).hexdigest() == expected:
                     retVal &= False
                     break
 
     return retVal
```

### Comparing `sqlmap-1.8.4/sqlmap/lib/takeover/abstraction.py` & `sqlmap-1.8.5/sqlmap/lib/takeover/abstraction.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/takeover/udf.py` & `sqlmap-1.8.5/sqlmap/lib/takeover/udf.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/takeover/metasploit.py` & `sqlmap-1.8.5/sqlmap/lib/takeover/metasploit.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,15 +192,15 @@
             _payloadStr = self._skeletonSelection("payload", self._msfPayloadsList)
 
         if _payloadStr == "windows/vncinject":
             choose = False
 
             if Backend.isDbms(DBMS.MYSQL):
                 debugMsg = "by default MySQL on Windows runs as SYSTEM "
-                debugMsg += "user, it is likely that the the VNC "
+                debugMsg += "user, it is likely that the VNC "
                 debugMsg += "injection will be successful"
                 logger.debug(debugMsg)
 
             elif Backend.isDbms(DBMS.PGSQL):
                 choose = True
 
                 warnMsg = "by default PostgreSQL on Windows runs as "
```

### Comparing `sqlmap-1.8.4/sqlmap/lib/takeover/xp_cmdshell.py` & `sqlmap-1.8.5/sqlmap/lib/takeover/xp_cmdshell.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/takeover/registry.py` & `sqlmap-1.8.5/sqlmap/lib/takeover/registry.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/takeover/web.py` & `sqlmap-1.8.5/sqlmap/lib/takeover/web.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/takeover/icmpsh.py` & `sqlmap-1.8.5/sqlmap/lib/takeover/icmpsh.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/parse/cmdline.py` & `sqlmap-1.8.5/sqlmap/lib/parse/cmdline.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/parse/handler.py` & `sqlmap-1.8.5/sqlmap/lib/parse/handler.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/parse/payloads.py` & `sqlmap-1.8.5/sqlmap/lib/parse/payloads.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/parse/configfile.py` & `sqlmap-1.8.5/sqlmap/lib/parse/configfile.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,15 +64,18 @@
     logger.debug(debugMsg)
 
     checkFile(configFile)
     configFP = openFile(configFile, "rb")
 
     try:
         config = UnicodeRawConfigParser()
-        config.readfp(configFP)
+        if hasattr(config, "read_file"):
+            config.read_file(configFP)
+        else:
+            config.readfp(configFP)
     except Exception as ex:
         errMsg = "you have provided an invalid and/or unreadable configuration file ('%s')" % getSafeExString(ex)
         raise SqlmapSyntaxException(errMsg)
 
     if not config.has_section("Target"):
         errMsg = "missing a mandatory section 'Target' in the configuration file"
         raise SqlmapMissingMandatoryOptionException(errMsg)
```

### Comparing `sqlmap-1.8.4/sqlmap/lib/parse/headers.py` & `sqlmap-1.8.5/sqlmap/lib/parse/headers.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/parse/sitemap.py` & `sqlmap-1.8.5/sqlmap/lib/parse/sitemap.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/parse/banner.py` & `sqlmap-1.8.5/sqlmap/lib/parse/banner.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/lib/parse/html.py` & `sqlmap-1.8.5/sqlmap/lib/parse/html.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/sqlmapapi.yaml` & `sqlmap-1.8.5/sqlmap/sqlmapapi.yaml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/extra/cloak/cloak.py` & `sqlmap-1.8.5/sqlmap/extra/cloak/cloak.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/extra/cloak/README.txt` & `sqlmap-1.8.5/sqlmap/extra/cloak/README.txt`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/extra/shutils/duplicates.py` & `sqlmap-1.8.5/sqlmap/extra/shutils/duplicates.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/extra/shutils/precommit-hook.sh` & `sqlmap-1.8.5/sqlmap/extra/shutils/precommit-hook.sh`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/extra/shutils/drei.sh` & `sqlmap-1.8.5/sqlmap/extra/shutils/drei.sh`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/extra/shutils/pypi.sh` & `sqlmap-1.8.5/sqlmap/extra/shutils/pypi.sh`

 * *Files 1% similar despite different names*

```diff
@@ -172,9 +172,11 @@
 
 .. pandoc --from=markdown --to=rst --output=README.rst sqlmap/README.md
 .. http://rst.ninjs.org/
 EOF
 sed -i "s/^VERSION =.*/VERSION = \"$VERSION\"/g" sqlmap/lib/core/settings.py
 sed -i "s/^TYPE =.*/TYPE = \"$TYPE\"/g" sqlmap/lib/core/settings.py
 for file in $(find sqlmap -type f | grep -v -E "\.(git|yml)"); do echo include $file >> MANIFEST.in; done
-python setup.py sdist upload
+python setup.py sdist bdist_wheel
+twine check dist/*
+twine upload --config-file=~/.pypirc dist/*
 rm -rf $TMP_DIR
```

### Comparing `sqlmap-1.8.4/sqlmap/extra/shutils/recloak.sh` & `sqlmap-1.8.5/sqlmap/extra/shutils/recloak.sh`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/extra/shutils/newlines.py` & `sqlmap-1.8.5/sqlmap/extra/shutils/newlines.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/extra/shutils/strip.sh` & `sqlmap-1.8.5/sqlmap/extra/shutils/strip.sh`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/extra/shutils/postcommit-hook.sh` & `sqlmap-1.8.5/sqlmap/extra/shutils/postcommit-hook.sh`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/extra/runcmd/src/runcmd.sln` & `sqlmap-1.8.5/sqlmap/extra/runcmd/src/runcmd.sln`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/extra/runcmd/src/runcmd/runcmd.cpp` & `sqlmap-1.8.5/sqlmap/extra/runcmd/src/runcmd/runcmd.cpp`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/extra/runcmd/src/runcmd/stdafx.h` & `sqlmap-1.8.5/sqlmap/extra/runcmd/src/runcmd/stdafx.h`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/extra/runcmd/src/runcmd/runcmd.vcproj` & `sqlmap-1.8.5/sqlmap/extra/runcmd/src/runcmd/runcmd.vcproj`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/extra/runcmd/runcmd.exe_` & `sqlmap-1.8.5/sqlmap/extra/runcmd/runcmd.exe_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/extra/beep/beep.py` & `sqlmap-1.8.5/sqlmap/extra/beep/beep.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/extra/beep/beep.wav` & `sqlmap-1.8.5/sqlmap/extra/beep/beep.wav`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/extra/shellcodeexec/linux/shellcodeexec.x32_` & `sqlmap-1.8.5/sqlmap/extra/shellcodeexec/linux/shellcodeexec.x32_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/extra/shellcodeexec/linux/shellcodeexec.x64_` & `sqlmap-1.8.5/sqlmap/extra/shellcodeexec/linux/shellcodeexec.x64_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/extra/shellcodeexec/windows/shellcodeexec.x32.exe_` & `sqlmap-1.8.5/sqlmap/extra/shellcodeexec/windows/shellcodeexec.x32.exe_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/extra/icmpsh/icmpsh-m.c` & `sqlmap-1.8.5/sqlmap/extra/icmpsh/icmpsh-m.c`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/extra/icmpsh/icmpsh.exe_` & `sqlmap-1.8.5/sqlmap/extra/icmpsh/icmpsh.exe_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/extra/icmpsh/icmpsh-s.c` & `sqlmap-1.8.5/sqlmap/extra/icmpsh/icmpsh-s.c`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/extra/icmpsh/README.txt` & `sqlmap-1.8.5/sqlmap/extra/icmpsh/README.txt`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/extra/icmpsh/icmpsh-m.pl` & `sqlmap-1.8.5/sqlmap/extra/icmpsh/icmpsh-m.pl`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/extra/icmpsh/__init__.py` & `sqlmap-1.8.5/sqlmap/extra/icmpsh/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/extra/icmpsh/icmpsh_m.py` & `sqlmap-1.8.5/sqlmap/extra/icmpsh/icmpsh_m.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/extra/dbgtool/dbgtool.py` & `sqlmap-1.8.5/sqlmap/extra/dbgtool/dbgtool.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/extra/dbgtool/README.txt` & `sqlmap-1.8.5/sqlmap/extra/dbgtool/README.txt`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/extra/vulnserver/vulnserver.py` & `sqlmap-1.8.5/sqlmap/extra/vulnserver/vulnserver.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap/sqlmapapi.py` & `sqlmap-1.8.5/sqlmap/sqlmapapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     setPaths(modulePath())
 
     # Parse command line options
     apiparser = ArgumentParser()
     apiparser.add_argument("-s", "--server", help="Run as a REST-JSON API server", action="store_true")
     apiparser.add_argument("-c", "--client", help="Run as a REST-JSON API client", action="store_true")
     apiparser.add_argument("-H", "--host", help="Host of the REST-JSON API server (default \"%s\")" % RESTAPI_DEFAULT_ADDRESS, default=RESTAPI_DEFAULT_ADDRESS)
-    apiparser.add_argument("-p", "--port", help="Port of the the REST-JSON API server (default %d)" % RESTAPI_DEFAULT_PORT, default=RESTAPI_DEFAULT_PORT, type=int)
+    apiparser.add_argument("-p", "--port", help="Port of the REST-JSON API server (default %d)" % RESTAPI_DEFAULT_PORT, default=RESTAPI_DEFAULT_PORT, type=int)
     apiparser.add_argument("--adapter", help="Server (bottle) adapter to use (default \"%s\")" % RESTAPI_DEFAULT_ADAPTER, default=RESTAPI_DEFAULT_ADAPTER)
     apiparser.add_argument("--database", help="Set IPC database filepath (optional)")
     apiparser.add_argument("--username", help="Basic authentication username (optional)")
     apiparser.add_argument("--password", help="Basic authentication password (optional)")
     (args, _) = apiparser.parse_known_args() if hasattr(apiparser, "parse_known_args") else apiparser.parse_args()
```

### Comparing `sqlmap-1.8.4/README.rst` & `sqlmap-1.8.5/README.rst`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap.egg-info/SOURCES.txt` & `sqlmap-1.8.5/sqlmap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqlmap-1.8.4/sqlmap.egg-info/PKG-INFO` & `sqlmap-1.8.5/sqlmap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: sqlmap
-Version: 1.8.4
+Version: 1.8.5
 Summary: Automatic SQL injection and database takeover tool
 Home-page: https://sqlmap.org
 Author: Bernardo Damele Assumpcao Guimaraes, Miroslav Stampar
 Author-email: bernardo@sqlmap.org, miroslav@sqlmap.org
 License: GNU General Public License v2 (GPLv2)
-Download-URL: https://github.com/sqlmapproject/sqlmap/archive/1.8.4.zip
+Download-URL: https://github.com/sqlmapproject/sqlmap/archive/1.8.5.zip
 Project-URL: Source, https://github.com/sqlmapproject/sqlmap/
 Project-URL: Documentation, https://github.com/sqlmapproject/sqlmap/wiki
 Project-URL: Tracker, https://github.com/sqlmapproject/sqlmap/issues
 Description: sqlmap
         ======
         
         |Python 2.6|2.7|3.x| |License| |Twitter|
```

### Comparing `sqlmap-1.8.4/setup.py` & `sqlmap-1.8.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 See the file 'LICENSE' for copying permission
 """
 
 from setuptools import setup, find_packages
 
 setup(
     name='sqlmap',
-    version='1.8.4',
+    version='1.8.5',
     description='Automatic SQL injection and database takeover tool',
     long_description=open('README.rst').read(),
     long_description_content_type='text/x-rst',
     author='Bernardo Damele Assumpcao Guimaraes, Miroslav Stampar',
     author_email='bernardo@sqlmap.org, miroslav@sqlmap.org',
     url='https://sqlmap.org',
     project_urls={
         'Documentation': 'https://github.com/sqlmapproject/sqlmap/wiki',
         'Source': 'https://github.com/sqlmapproject/sqlmap/',
         'Tracker': 'https://github.com/sqlmapproject/sqlmap/issues',
     },
-    download_url='https://github.com/sqlmapproject/sqlmap/archive/1.8.4.zip',
+    download_url='https://github.com/sqlmapproject/sqlmap/archive/1.8.5.zip',
     license='GNU General Public License v2 (GPLv2)',
     packages=find_packages(),
     include_package_data=True,
     zip_safe=False,
     # https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         'Development Status :: 5 - Production/Stable',
```

