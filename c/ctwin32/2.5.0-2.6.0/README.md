# Comparing `tmp/ctwin32-2.5.0.tar.gz` & `tmp/ctwin32-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctwin32-2.5.0.tar", last modified: Mon Mar 11 15:55:08 2024, max compression
+gzip compressed data, was "ctwin32-2.6.0.tar", last modified: Thu May  9 05:30:15 2024, max compression
```

## Comparing `ctwin32-2.5.0.tar` & `ctwin32-2.6.0.tar`

### file list

```diff
@@ -1,73 +1,76 @@
-drwxrwxrwx   0        0        0        0 2024-03-11 15:55:08.526887 ctwin32-2.5.0/
--rw-rw-rw-   0        0        0     1057 2024-03-11 08:41:46.000000 ctwin32-2.5.0/LICENSE
--rw-rw-rw-   0        0        0       24 2023-10-24 06:50:38.000000 ctwin32-2.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2845 2024-03-11 15:55:08.524884 ctwin32-2.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     1916 2023-10-24 06:50:38.000000 ctwin32-2.5.0/README.md
--rw-rw-rw-   0        0        0     1641 2023-10-24 06:50:38.000000 ctwin32-2.5.0/bld.py
-drwxrwxrwx   0        0        0        0 2024-03-11 15:55:08.490874 ctwin32-2.5.0/ctwin32/
--rw-rw-rw-   0        0        0   223786 2024-03-11 15:50:12.000000 ctwin32-2.5.0/ctwin32/__init__.py
--rw-rw-rw-   0        0        0    44305 2024-03-11 08:41:46.000000 ctwin32-2.5.0/ctwin32/advapi.py
--rw-rw-rw-   0        0        0    17770 2024-03-11 08:41:46.000000 ctwin32-2.5.0/ctwin32/bcrypt.py
--rw-rw-rw-   0        0        0     6010 2024-03-11 08:41:46.000000 ctwin32-2.5.0/ctwin32/cfgmgr.py
--rw-rw-rw-   0        0        0     9079 2024-03-11 08:41:46.000000 ctwin32-2.5.0/ctwin32/comctl.py
--rw-rw-rw-   0        0        0     4352 2024-03-11 08:41:46.000000 ctwin32-2.5.0/ctwin32/gdi.py
--rw-rw-rw-   0        0        0    13791 2024-03-11 08:41:46.000000 ctwin32-2.5.0/ctwin32/iphlpapi.py
--rw-rw-rw-   0        0        0    52499 2024-03-11 11:14:05.000000 ctwin32-2.5.0/ctwin32/kernel.py
--rw-rw-rw-   0        0        0     7154 2024-03-11 08:41:46.000000 ctwin32-2.5.0/ctwin32/misc.py
--rw-rw-rw-   0        0        0     5174 2024-03-11 08:41:46.000000 ctwin32-2.5.0/ctwin32/msi.py
--rw-rw-rw-   0        0        0    19091 2024-03-11 08:41:46.000000 ctwin32-2.5.0/ctwin32/ntdll.py
--rw-rw-rw-   0        0        0     4182 2024-03-11 08:41:46.000000 ctwin32-2.5.0/ctwin32/psapi.py
--rw-rw-rw-   0        0        0     6236 2024-03-11 08:41:46.000000 ctwin32-2.5.0/ctwin32/secur.py
--rw-rw-rw-   0        0        0    17523 2024-03-11 08:41:46.000000 ctwin32-2.5.0/ctwin32/setupapi.py
--rw-rw-rw-   0        0        0     7921 2024-03-11 08:41:46.000000 ctwin32-2.5.0/ctwin32/shell.py
--rw-rw-rw-   0        0        0    13802 2024-03-11 08:41:46.000000 ctwin32-2.5.0/ctwin32/svc_util.py
--rw-rw-rw-   0        0        0    44326 2024-03-11 08:41:46.000000 ctwin32-2.5.0/ctwin32/user.py
--rw-rw-rw-   0        0        0     4923 2024-03-11 08:41:46.000000 ctwin32-2.5.0/ctwin32/version.py
--rw-rw-rw-   0        0        0     6877 2024-03-11 08:41:46.000000 ctwin32-2.5.0/ctwin32/virtdisk.py
--rw-rw-rw-   0        0        0    28593 2024-03-11 08:41:46.000000 ctwin32-2.5.0/ctwin32/wndcls.py
--rw-rw-rw-   0        0        0    15926 2024-03-11 08:41:46.000000 ctwin32-2.5.0/ctwin32/wtypes.py
-drwxrwxrwx   0        0        0        0 2024-03-11 15:55:08.524884 ctwin32-2.5.0/ctwin32.egg-info/
--rw-rw-rw-   0        0        0     2845 2024-03-11 15:55:08.000000 ctwin32-2.5.0/ctwin32.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1320 2024-03-11 15:55:08.000000 ctwin32-2.5.0/ctwin32.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-11 15:55:08.000000 ctwin32-2.5.0/ctwin32.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-03-11 15:55:08.000000 ctwin32-2.5.0/ctwin32.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-11 15:55:08.466863 ctwin32-2.5.0/doc/
-drwxrwxrwx   0        0        0        0 2024-03-11 15:55:08.494876 ctwin32-2.5.0/doc/images/
--rw-rw-rw-   0        0        0     7882 2023-10-24 06:50:38.000000 ctwin32-2.5.0/doc/images/ctwin32.ico
--rw-rw-rw-   0        0        0     3034 2024-03-11 08:41:46.000000 ctwin32-2.5.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-03-11 15:55:08.524884 ctwin32-2.5.0/samples/
--rw-rw-rw-   0        0        0        0 2023-10-24 06:50:38.000000 ctwin32-2.5.0/samples/__init__.py
--rw-rw-rw-   0        0        0     5738 2024-03-11 08:41:46.000000 ctwin32-2.5.0/samples/api_set.py
--rw-rw-rw-   0        0        0     2571 2024-03-11 08:41:46.000000 ctwin32-2.5.0/samples/arp_table.py
--rw-rw-rw-   0        0        0     2527 2024-03-11 08:41:46.000000 ctwin32-2.5.0/samples/atta_vdisk.py
--rw-rw-rw-   0        0        0     3999 2024-03-11 08:41:46.000000 ctwin32-2.5.0/samples/calendar.pyw
--rw-rw-rw-   0        0        0     7283 2024-03-11 08:41:46.000000 ctwin32-2.5.0/samples/dump_ver_res.py
--rw-rw-rw-   0        0        0     2754 2024-03-11 08:41:46.000000 ctwin32-2.5.0/samples/endis_bsl_usb.py
--rw-rw-rw-   0        0        0     2300 2024-03-11 08:41:46.000000 ctwin32-2.5.0/samples/exbinmsi.py
--rw-rw-rw-   0        0        0     7490 2024-03-11 08:41:46.000000 ctwin32-2.5.0/samples/extract_ico.py
--rw-rw-rw-   0        0        0     4693 2024-03-11 08:41:46.000000 ctwin32-2.5.0/samples/find_zombies.py
--rw-rw-rw-   0        0        0     2026 2024-03-11 08:41:46.000000 ctwin32-2.5.0/samples/fopa.py
--rw-rw-rw-   0        0        0     4124 2024-03-11 08:41:46.000000 ctwin32-2.5.0/samples/hello_wnd.pyw
--rw-rw-rw-   0        0        0     6777 2024-03-11 08:41:46.000000 ctwin32-2.5.0/samples/keyview.pyw
--rw-rw-rw-   0        0        0     1989 2024-03-11 08:41:46.000000 ctwin32-2.5.0/samples/listpipes.py
--rw-rw-rw-   0        0        0     3700 2024-03-11 08:41:46.000000 ctwin32-2.5.0/samples/logonsessions.py
--rw-rw-rw-   0        0        0     3222 2024-03-11 08:41:46.000000 ctwin32-2.5.0/samples/lsc.py
--rw-rw-rw-   0        0        0     1976 2024-03-11 08:41:46.000000 ctwin32-2.5.0/samples/netifaces.py
--rw-rw-rw-   0        0        0     2270 2024-03-11 08:41:46.000000 ctwin32-2.5.0/samples/np_dev.py
--rw-rw-rw-   0        0        0     8406 2024-03-11 08:41:46.000000 ctwin32-2.5.0/samples/power_requests.py
--rw-rw-rw-   0        0        0     5123 2024-03-11 08:41:46.000000 ctwin32-2.5.0/samples/print_reparse_points.py
--rw-rw-rw-   0        0        0     3172 2024-03-11 08:41:46.000000 ctwin32-2.5.0/samples/py_ver.py
--rw-rw-rw-   0        0        0     5138 2024-03-11 08:41:46.000000 ctwin32-2.5.0/samples/remove_drive_by_letter.py
--rw-rw-rw-   0        0        0     4316 2024-03-11 08:41:46.000000 ctwin32-2.5.0/samples/restart_usb_port.py
--rw-rw-rw-   0        0        0     6485 2024-03-11 08:41:46.000000 ctwin32-2.5.0/samples/rm_sign_tool.py
--rw-rw-rw-   0        0        0     5460 2024-03-11 08:41:46.000000 ctwin32-2.5.0/samples/senv.py
--rw-rw-rw-   0        0        0     4569 2024-03-11 08:41:46.000000 ctwin32-2.5.0/samples/simple_aes.py
--rw-rw-rw-   0        0        0     3373 2024-03-11 08:41:46.000000 ctwin32-2.5.0/samples/stopnow.py
--rw-rw-rw-   0        0        0     2253 2024-03-11 08:41:46.000000 ctwin32-2.5.0/samples/sua_enums.py
--rw-rw-rw-   0        0        0     2698 2024-03-11 08:41:46.000000 ctwin32-2.5.0/samples/test_sign_tool.py
--rw-rw-rw-   0        0        0     2054 2024-03-11 08:41:46.000000 ctwin32-2.5.0/samples/uptime_evt.py
--rw-rw-rw-   0        0        0     2658 2024-03-11 08:41:46.000000 ctwin32-2.5.0/samples/virt_term_seq.py
--rw-rw-rw-   0        0        0     3879 2024-03-11 08:41:46.000000 ctwin32-2.5.0/samples/volume_paths.py
--rw-rw-rw-   0        0        0     2789 2024-03-11 11:19:48.000000 ctwin32-2.5.0/samples/wait_for_job.py
--rw-rw-rw-   0        0        0       42 2024-03-11 15:55:08.526887 ctwin32-2.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1102 2023-10-24 06:50:38.000000 ctwin32-2.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 05:30:15.613857 ctwin32-2.6.0/
+-rw-rw-rw-   0        0        0     1057 2024-03-11 08:41:46.000000 ctwin32-2.6.0/LICENSE
+-rw-rw-rw-   0        0        0       24 2023-10-24 06:50:38.000000 ctwin32-2.6.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2986 2024-05-09 05:30:15.613857 ctwin32-2.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2004 2024-03-15 05:04:38.000000 ctwin32-2.6.0/README.md
+-rw-rw-rw-   0        0        0     1641 2023-10-24 06:50:38.000000 ctwin32-2.6.0/bld.py
+drwxrwxrwx   0        0        0        0 2024-05-09 05:30:15.563845 ctwin32-2.6.0/ctwin32/
+-rw-rw-rw-   0        0        0   224259 2024-05-09 05:28:35.000000 ctwin32-2.6.0/ctwin32/__init__.py
+-rw-rw-rw-   0        0        0    44043 2024-04-01 12:07:21.000000 ctwin32-2.6.0/ctwin32/advapi.py
+-rw-rw-rw-   0        0        0    17663 2024-04-01 12:09:09.000000 ctwin32-2.6.0/ctwin32/bcrypt.py
+-rw-rw-rw-   0        0        0     7544 2024-04-01 12:10:07.000000 ctwin32-2.6.0/ctwin32/cfgmgr.py
+-rw-rw-rw-   0        0        0     9079 2024-03-11 08:41:46.000000 ctwin32-2.6.0/ctwin32/comctl.py
+-rw-rw-rw-   0        0        0     5307 2024-03-26 05:08:52.000000 ctwin32-2.6.0/ctwin32/gdi.py
+-rw-rw-rw-   0        0        0    13781 2024-04-01 12:11:23.000000 ctwin32-2.6.0/ctwin32/iphlpapi.py
+-rw-rw-rw-   0        0        0    53100 2024-04-01 12:12:18.000000 ctwin32-2.6.0/ctwin32/kernel.py
+-rw-rw-rw-   0        0        0     7227 2024-04-01 12:13:31.000000 ctwin32-2.6.0/ctwin32/misc.py
+-rw-rw-rw-   0        0        0     5435 2024-04-01 12:14:30.000000 ctwin32-2.6.0/ctwin32/msi.py
+-rw-rw-rw-   0        0        0    20043 2024-04-01 12:15:41.000000 ctwin32-2.6.0/ctwin32/ntdll.py
+-rw-rw-rw-   0        0        0     4171 2024-04-01 12:31:33.000000 ctwin32-2.6.0/ctwin32/psapi.py
+-rw-rw-rw-   0        0        0     6236 2024-03-11 08:41:46.000000 ctwin32-2.6.0/ctwin32/secur.py
+-rw-rw-rw-   0        0        0    17513 2024-04-01 12:17:35.000000 ctwin32-2.6.0/ctwin32/setupapi.py
+-rw-rw-rw-   0        0        0     7925 2024-04-01 12:31:47.000000 ctwin32-2.6.0/ctwin32/shell.py
+-rw-rw-rw-   0        0        0    13802 2024-03-11 08:41:46.000000 ctwin32-2.6.0/ctwin32/svc_util.py
+-rw-rw-rw-   0        0        0    44339 2024-04-10 16:16:27.000000 ctwin32-2.6.0/ctwin32/user.py
+-rw-rw-rw-   0        0        0     4924 2024-04-01 12:32:11.000000 ctwin32-2.6.0/ctwin32/version.py
+-rw-rw-rw-   0        0        0     6877 2024-03-11 08:41:46.000000 ctwin32-2.6.0/ctwin32/virtdisk.py
+-rw-rw-rw-   0        0        0    28552 2024-04-01 12:32:24.000000 ctwin32-2.6.0/ctwin32/wndcls.py
+-rw-rw-rw-   0        0        0    16982 2024-04-02 02:58:09.000000 ctwin32-2.6.0/ctwin32/wtypes.py
+drwxrwxrwx   0        0        0        0 2024-05-09 05:30:15.611856 ctwin32-2.6.0/ctwin32.egg-info/
+-rw-rw-rw-   0        0        0     2986 2024-05-09 05:30:15.000000 ctwin32-2.6.0/ctwin32.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1382 2024-05-09 05:30:15.000000 ctwin32-2.6.0/ctwin32.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 05:30:15.000000 ctwin32-2.6.0/ctwin32.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-09 05:30:15.000000 ctwin32-2.6.0/ctwin32.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 05:30:15.539842 ctwin32-2.6.0/doc/
+drwxrwxrwx   0        0        0        0 2024-05-09 05:30:15.569846 ctwin32-2.6.0/doc/images/
+-rw-rw-rw-   0        0        0     7882 2023-10-24 06:50:38.000000 ctwin32-2.6.0/doc/images/ctwin32.ico
+-rw-rw-rw-   0        0        0     3232 2024-05-09 05:21:31.000000 ctwin32-2.6.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-09 05:30:15.611856 ctwin32-2.6.0/samples/
+-rw-rw-rw-   0        0        0        0 2023-10-24 06:50:38.000000 ctwin32-2.6.0/samples/__init__.py
+-rw-rw-rw-   0        0        0     5738 2024-03-11 08:41:46.000000 ctwin32-2.6.0/samples/api_set.py
+-rw-rw-rw-   0        0        0     2571 2024-03-11 08:41:46.000000 ctwin32-2.6.0/samples/arp_table.py
+-rw-rw-rw-   0        0        0     2527 2024-03-11 08:41:46.000000 ctwin32-2.6.0/samples/atta_vdisk.py
+-rw-rw-rw-   0        0        0     3999 2024-03-11 08:41:46.000000 ctwin32-2.6.0/samples/calendar.pyw
+-rw-rw-rw-   0        0        0     2995 2024-03-25 12:25:51.000000 ctwin32-2.6.0/samples/cnt_irq.py
+-rw-rw-rw-   0        0        0     2130 2024-03-29 06:31:54.000000 ctwin32-2.6.0/samples/dump_proc_env.py
+-rw-rw-rw-   0        0        0     7283 2024-03-11 08:41:46.000000 ctwin32-2.6.0/samples/dump_ver_res.py
+-rw-rw-rw-   0        0        0     2754 2024-03-11 08:41:46.000000 ctwin32-2.6.0/samples/endis_bsl_usb.py
+-rw-rw-rw-   0        0        0     2300 2024-03-11 08:41:46.000000 ctwin32-2.6.0/samples/exbinmsi.py
+-rw-rw-rw-   0        0        0     7490 2024-03-11 08:41:46.000000 ctwin32-2.6.0/samples/extract_ico.py
+-rw-rw-rw-   0        0        0     4693 2024-03-11 08:41:46.000000 ctwin32-2.6.0/samples/find_zombies.py
+-rw-rw-rw-   0        0        0     2026 2024-03-11 08:41:46.000000 ctwin32-2.6.0/samples/fopa.py
+-rw-rw-rw-   0        0        0     4124 2024-03-11 08:41:46.000000 ctwin32-2.6.0/samples/hello_wnd.pyw
+-rw-rw-rw-   0        0        0     6777 2024-03-11 08:41:46.000000 ctwin32-2.6.0/samples/keyview.pyw
+-rw-rw-rw-   0        0        0     1989 2024-03-11 08:41:46.000000 ctwin32-2.6.0/samples/listpipes.py
+-rw-rw-rw-   0        0        0     3700 2024-03-11 08:41:46.000000 ctwin32-2.6.0/samples/logonsessions.py
+-rw-rw-rw-   0        0        0     3222 2024-03-11 08:41:46.000000 ctwin32-2.6.0/samples/lsc.py
+-rw-rw-rw-   0        0        0     1976 2024-03-17 05:12:33.000000 ctwin32-2.6.0/samples/netifaces.py
+-rw-rw-rw-   0        0        0     2270 2024-03-11 08:41:46.000000 ctwin32-2.6.0/samples/np_dev.py
+-rw-rw-rw-   0        0        0     8406 2024-03-11 08:41:46.000000 ctwin32-2.6.0/samples/power_requests.py
+-rw-rw-rw-   0        0        0     5123 2024-03-11 08:41:46.000000 ctwin32-2.6.0/samples/print_reparse_points.py
+-rw-rw-rw-   0        0        0     3172 2024-03-11 08:41:46.000000 ctwin32-2.6.0/samples/py_ver.py
+-rw-rw-rw-   0        0        0     5138 2024-03-11 08:41:46.000000 ctwin32-2.6.0/samples/remove_drive_by_letter.py
+-rw-rw-rw-   0        0        0     4109 2024-03-25 12:25:51.000000 ctwin32-2.6.0/samples/restart_usb_port.py
+-rw-rw-rw-   0        0        0     6485 2024-03-11 08:41:46.000000 ctwin32-2.6.0/samples/rm_sign_tool.py
+-rw-rw-rw-   0        0        0     5464 2024-04-01 12:31:02.000000 ctwin32-2.6.0/samples/senv.py
+-rw-rw-rw-   0        0        0     4569 2024-03-11 08:41:46.000000 ctwin32-2.6.0/samples/simple_aes.py
+-rw-rw-rw-   0        0        0     3373 2024-03-11 08:41:46.000000 ctwin32-2.6.0/samples/stopnow.py
+-rw-rw-rw-   0        0        0     2253 2024-03-11 08:41:46.000000 ctwin32-2.6.0/samples/sua_enums.py
+-rw-rw-rw-   0        0        0     2698 2024-03-11 08:41:46.000000 ctwin32-2.6.0/samples/test_sign_tool.py
+-rw-rw-rw-   0        0        0     2802 2024-03-27 04:37:46.000000 ctwin32-2.6.0/samples/timeit.py
+-rw-rw-rw-   0        0        0     2054 2024-03-11 08:41:46.000000 ctwin32-2.6.0/samples/uptime_evt.py
+-rw-rw-rw-   0        0        0     2658 2024-03-11 08:41:46.000000 ctwin32-2.6.0/samples/virt_term_seq.py
+-rw-rw-rw-   0        0        0     3879 2024-03-11 08:41:46.000000 ctwin32-2.6.0/samples/volume_paths.py
+-rw-rw-rw-   0        0        0     2882 2024-03-13 13:41:34.000000 ctwin32-2.6.0/samples/wait_for_job.py
+-rw-rw-rw-   0        0        0       42 2024-05-09 05:30:15.613857 ctwin32-2.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1102 2023-10-24 06:50:38.000000 ctwin32-2.6.0/setup.py
```

### Comparing `ctwin32-2.5.0/LICENSE` & `ctwin32-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ctwin32-2.5.0/PKG-INFO` & `ctwin32-2.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctwin32
-Version: 2.5.0
+Version: 2.6.0
 Summary: Access selected win32 APIs through ctypes
 Author: Rocco Matano
 License: MIT License
 Project-URL: homepage, https://github.com/RoccoMatano/ctwin32
 Project-URL: changelog, https://github.com/RoccoMatano/ctwin32/blob/master/changelog.md
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -12,20 +12,22 @@
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ![logo](https://raw.githubusercontent.com/RoccoMatano/ctwin32/master/doc/images/ctwin32.ico) ctwin32
 
+[![winonly](https://img.shields.io/badge/Windows-0078D6?style=plastic&logo=windows)](.)
 [![PyPI - Version](https://img.shields.io/pypi/v/ctwin32.svg)](https://pypi.org/project/ctwin32)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ctwin32.svg)](https://pypi.org/project/ctwin32)
 [![License - MIT](https://img.shields.io/badge/license-MIT-green)](https://spdx.org/licenses/MIT.html)
 [![PyPI - Stats](https://img.shields.io/pypi/dm/ctwin32)](https://pypistats.org/packages/ctwin32)
 
 -----
```

### Comparing `ctwin32-2.5.0/README.md` & `ctwin32-2.6.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # ![logo](https://raw.githubusercontent.com/RoccoMatano/ctwin32/master/doc/images/ctwin32.ico) ctwin32
 
+[![winonly](https://img.shields.io/badge/Windows-0078D6?style=plastic&logo=windows)](.)
 [![PyPI - Version](https://img.shields.io/pypi/v/ctwin32.svg)](https://pypi.org/project/ctwin32)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ctwin32.svg)](https://pypi.org/project/ctwin32)
 [![License - MIT](https://img.shields.io/badge/license-MIT-green)](https://spdx.org/licenses/MIT.html)
 [![PyPI - Stats](https://img.shields.io/pypi/dm/ctwin32)](https://pypistats.org/packages/ctwin32)
 
 -----
```

### Comparing `ctwin32-2.5.0/bld.py` & `ctwin32-2.6.0/bld.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.5.0/ctwin32/__init__.py` & `ctwin32-2.6.0/ctwin32/__init__.py`

 * *Files identical despite different names*

```diff
@@ -32,15 +32,15 @@
     UINT,
     WCHAR_SIZE,
     )
 ref = ctypes.byref
 
 ################################################################################
 
-__version__ = "2.5.0"
+__version__ = "2.6.0"
 
 ################################################################################
 
 def raise_if(condition):
     if condition:
         raise ctypes.WinError()
 
@@ -86,15 +86,16 @@
     function.restype = signature[0]
     function.argtypes = signature[1:]
     return function
 
 ################################################################################
 
 def multi_str_from_str(_str):
-    _str = _str.rstrip("\0")
+    idx = _str.find("\0\0")
+    _str = _str[:idx] if idx != -1 else _str.rstrip("\0")
     return [] if not _str else _str.split("\0")
 
 ################################################################################
 
 def multi_str_from_addr(addr):
     end = addr
     while True:
@@ -140,16 +141,22 @@
         if need_qmark:
             parts.extend(bs_accu)
             parts.append('"')
     return "".join(parts)
 
 ################################################################################
 
-def ns_from_struct(cts):
-    return _namespace(**{f: getattr(cts, f) for f, *_ in cts._fields_})
+def ns_from_struct(ctypes_struct):
+    # hack the class name for nicer repr
+    class HackedClassName(_namespace):
+        pass
+    HackedClassName.__name__ = type(ctypes_struct).__name__
+    return HackedClassName(
+        **{f: getattr(ctypes_struct, f) for f, *_ in ctypes_struct._fields_}
+        )
 
 ################################################################################
 
 def _warn_win_ver():
     osve = OSVERSIONINFOEX()
     status = ctypes.WinDLL("ntdll.dll").RtlGetVersion(ref(osve))
     if status == 0 and osve.dwMajorVersion < 10:
@@ -6928,14 +6935,16 @@
 CM_ENUMERATE_CLASSES_INSTALLER = 0x00000000
 CM_ENUMERATE_CLASSES_INTERFACE = 0x00000001
 CM_ENUMERATE_CLASSES_BITS = 0x00000001
 CM_LOCATE_DEVNODE_NORMAL = 0x00000000
 CM_LOCATE_DEVNODE_PHANTOM = 0x00000001
 CM_LOCATE_DEVNODE_CANCELREMOVE = 0x00000002
 CM_LOCATE_DEVNODE_NOVALIDATION = 0x00000004
+CM_GET_DEVICE_INTERFACE_LIST_PRESENT = 0x00000000  # only live interfaces
+CM_GET_DEVICE_INTERFACE_LIST_ALL_DEVICES = 0x00000001  # all, live or not
 
 SPDRP_DEVICEDESC = 0x00000000  # DeviceDesc (R/W)
 SPDRP_HARDWAREID = 0x00000001  # HardwareID (R/W)
 SPDRP_COMPATIBLEIDS = 0x00000002  # CompatibleIDs (R/W)
 SPDRP_UNUSED0 = 0x00000003  # unused
 SPDRP_SERVICE = 0x00000004  # Service (R/W)
 SPDRP_UNUSED1 = 0x00000005  # unused
@@ -7636,14 +7645,17 @@
 ISOLATIONAWARE_MANIFEST_RESOURCE_ID = PWSTR(2)
 ISOLATIONAWARE_NOSTATICIMPORT_MANIFEST_RESOURCE_ID = PWSTR(3)
 ISOLATIONPOLICY_MANIFEST_RESOURCE_ID = PWSTR(4)
 ISOLATIONPOLICY_BROWSER_MANIFEST_RESOURCE_ID = PWSTR(5)
 MINIMUM_RESERVED_MANIFEST_RESOURCE_ID = PWSTR(1)
 MAXIMUM_RESERVED_MANIFEST_RESOURCE_ID = PWSTR(16)
 
+IMAGE_DOS_SIGNATURE = 0x5A4D
+IMAGE_NT_SIGNATURE = 0x00004550
+
 IMAGE_FILE_MACHINE_UNKNOWN = 0
 IMAGE_FILE_MACHINE_TARGET_HOST = 0x0001
 IMAGE_FILE_MACHINE_I386 = 0x014c
 IMAGE_FILE_MACHINE_R3000 = 0x0162
 IMAGE_FILE_MACHINE_R4000 = 0x0166
 IMAGE_FILE_MACHINE_R10000 = 0x0168
 IMAGE_FILE_MACHINE_WCEMIPSV2 = 0x0169
```

### Comparing `ctwin32-2.5.0/ctwin32/advapi.py` & `ctwin32-2.6.0/ctwin32/advapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 ################################################################################
 
 from types import SimpleNamespace as _namespace
 from datetime import datetime as _dt
 import ctypes
 
 from .wtypes import (
+    byte_buffer,
+    string_buffer,
     ArgcArgvFromArgs,
     BOOL,
     BYTE,
     DWORD,
     ENDIANNESS,
     FILETIME,
     HANDLE,
@@ -326,15 +328,15 @@
         PDWORD,
         PFILETIME
         )
     )
 
 def RegEnumKeyEx(key, index):
     name_len = DWORD(_MAX_KEY_LEN)
-    name = ctypes.create_unicode_buffer(_MAX_KEY_LEN)
+    name = string_buffer(_MAX_KEY_LEN)
     raise_on_err(
         _RegEnumKeyEx(
             key,
             index,
             name,
             ref(name_len),
             None,
@@ -371,16 +373,16 @@
         )
     )
 
 def RegEnumValue(key, index):
     info = RegQueryInfoKey(key)
     nlen = DWORD(info.max_value_name_len + 1)
     vlen = DWORD(info.max_value_len + 1)
-    name = ctypes.create_unicode_buffer(nlen.value)
-    value = ctypes.create_string_buffer(vlen.value)
+    name = string_buffer(nlen.value)
+    value = byte_buffer(vlen.value)
     typ = DWORD()
     while True:
         err = _RegEnumValue(
             key,
             index,
             name,
             ref(nlen),
@@ -389,15 +391,15 @@
             ctypes.cast(value, PBYTE),
             ref(vlen)
             )
         if err == 0:
             break
         elif err == ERROR_MORE_DATA:
             vlen = DWORD(vlen.value * 2)
-            value = ctypes.create_string_buffer(vlen.value)
+            value = byte_buffer(vlen.value)
         else:
             raise ctypes.WinError(err)
 
     return (name.value, *registry_to_py(typ.value, value.raw[:vlen.value]))
 
 ################################################################################
 
@@ -421,30 +423,30 @@
         PBYTE,
         PDWORD
         )
     )
 
 def RegQueryValueEx(key, name):
     vlen = DWORD(256)
-    value = ctypes.create_string_buffer(vlen.value)
+    value = byte_buffer(vlen.value)
     typ = DWORD()
     while True:
         err = _RegQueryValueEx(
             key,
             name,
             None,
             ref(typ),
             ctypes.cast(value, PBYTE),
             ref(vlen)
             )
         if err == 0:
             break
         elif err == ERROR_MORE_DATA:
             vlen = DWORD(vlen.value * 2)
-            value = ctypes.create_string_buffer(vlen.value)
+            value = byte_buffer(vlen.value)
         else:
             raise ctypes.WinError(err)
 
     return registry_to_py(typ.value, value[:vlen.value])
 
 ################################################################################
 
@@ -457,15 +459,15 @@
         DWORD,
         PVOID,
         DWORD,
         )
     )
 
 def RegSetValueEx(key, name, typ, data):
-    dta = ctypes.create_string_buffer(data)
+    dta = byte_buffer(data)
     raise_on_err(
         _RegSetValueEx(
             key,
             name,
             0,
             typ,
             ref(dta),
@@ -484,15 +486,15 @@
         DWORD,
         PVOID,
         DWORD,
         )
     )
 
 def RegSetKeyValue(parent, key_name, value_name, typ, data):
-    dta = ctypes.create_string_buffer(data)
+    dta = byte_buffer(data)
     raise_on_err(
         _RegSetKeyValue(
             parent,
             key_name,
             value_name,
             typ,
             ref(dta),
@@ -502,15 +504,15 @@
 
 ################################################################################
 
 def reg_set_str(key, name, string, typ=None):
     typ = REG_SZ if typ is None else typ
     if not is_registry_string(typ):
         raise ValueError(f"invalid registry type: {typ}")
-    value = ctypes.create_unicode_buffer(string, len(string))
+    value = string_buffer(string, len(string))
     raise_on_err(
         _RegSetValueEx(
             key,
             name,
             0,
             typ,
             ref(value),
@@ -567,15 +569,15 @@
 ################################################################################
 
 _ConvertSidToStringSid = fun_fact(
     _adv.ConvertSidToStringSidW, (BOOL, PVOID, PPWSTR)
     )
 
 def ConvertSidToStringSid(sid):
-    bin_sid = ctypes.create_string_buffer(sid)
+    bin_sid = byte_buffer(sid)
     str_sid = PWSTR()
     try:
         raise_on_zero(_ConvertSidToStringSid(ref(bin_sid), ref(str_sid)))
         return ctypes.wstring_at(str_sid)
     finally:
         LocalFree(str_sid)
 
@@ -588,15 +590,15 @@
         PVOID,
         PBOOL
         )
     )
 
 def CheckTokenMembership(token_handle, sid_to_check):
     res = BOOL()
-    sid = ctypes.create_string_buffer(sid_to_check)
+    sid = byte_buffer(sid_to_check)
     raise_on_zero(_CheckTokenMembership(token_handle, ref(sid), ref(res)))
     return res.value != 0
 
 ################################################################################
 
 def running_as_admin():
     # well known sid of aministrators group
@@ -647,15 +649,15 @@
     _adv.GetTokenInformation, (BOOL, HANDLE, INT, PVOID, DWORD, PDWORD)
     )
 
 def GetTokenInformation(hdl, cls):
     rlen = DWORD(256)
     while True:
         size = rlen.value
-        buf = ctypes.create_string_buffer(size)
+        buf = byte_buffer(size)
         if _GetTokenInformation(hdl, cls, buf, size, ref(rlen)):
             return buf.raw[:rlen.value]
         elif (err := GetLastError()) != ERROR_INSUFFICIENT_BUFFER:
             raise ctypes.WinError(err)
 
 ################################################################################
 
@@ -827,16 +829,16 @@
         )
     err = GetLastError()
     if ok:
         raise AssertionError("logic error in LookupAccountSid")
     if err != ERROR_INSUFFICIENT_BUFFER:
         raise ctypes.WinError(err)
 
-    name = ctypes.create_unicode_buffer(name_size.value)
-    domain = ctypes.create_unicode_buffer(domain_size.value)
+    name = string_buffer(name_size.value)
+    domain = string_buffer(domain_size.value)
     raise_on_zero(
         _LookupAccountSid(
             system_name,
             sid,
             name,
             ref(name_size),
             domain,
@@ -1106,15 +1108,15 @@
         binary_path_name,
         load_order_group=None,
         dependencies=None,
         service_start_name=None,
         password=None
         ):
     if dependencies is not None:
-        dependencies = ctypes.create_unicode_buffer("\x00".join(dependencies))
+        dependencies = string_buffer("\x00".join(dependencies))
     res = SC_HANDLE(
         _CreateService(
             scm,
             service_name,
             display_name,
             desired_acc,
             service_type,
@@ -1244,15 +1246,15 @@
         PDWORD,
         PWSTR
         )
     )
 
 def EnumServicesStatusEx(scm, stype, sstate, group_name=None):
     stat_size = ctypes.sizeof(ENUM_SERVICE_STATUS_PROCESS)
-    buf = ctypes.create_string_buffer(16 * 1024)
+    buf = byte_buffer(16 * 1024)
     needed = DWORD()
     num_ret = DWORD()
     resume = DWORD()
     result = []
     success = False
 
     while not success:
@@ -1272,15 +1274,15 @@
 
         for offs in range(0, num_ret.value * stat_size, stat_size):
             status = ENUM_SERVICE_STATUS_PROCESS.from_buffer(buf, offs)
             result.append(ns_from_struct(status))
 
         if success:
             break
-        buf = ctypes.create_string_buffer(needed.value)
+        buf = byte_buffer(needed.value)
 
     return result
 
 ################################################################################
 
 class QUERY_SERVICE_CONFIG(ctypes.Structure):
     _fields_ = (
@@ -1310,15 +1312,15 @@
     needed = DWORD()
     ok = _QueryServiceConfig(svc, None, 0, ref(needed))
     err = GetLastError()
     if ok:
         raise AssertionError("logic error in QueryServiceConfig")
     if err != ERROR_INSUFFICIENT_BUFFER:
         raise ctypes.WinError(err)
-    buf = ctypes.create_string_buffer(needed.value)
+    buf = byte_buffer(needed.value)
     pqsc = ctypes.cast(buf, PQUERY_SERVICE_CONFIG)
     raise_on_zero(_QueryServiceConfig(svc, pqsc, needed.value, ref(needed)))
     return ns_from_struct(pqsc.contents)
 
 ################################################################################
 
 SERVICE_MAIN_FUNCTION = ctypes.WINFUNCTYPE(None, DWORD, PPWSTR)
@@ -1613,15 +1615,15 @@
 
 def ReadEventLog(hdl, flags=None, offs=0, size=16384):
     if flags is None:
         flags = EVENTLOG_SEQUENTIAL_READ | EVENTLOG_BACKWARDS_READ
     want = DWORD(size)
     while True:
         got = DWORD()
-        buf = ctypes.create_string_buffer(want.value)
+        buf = byte_buffer(want.value)
         ok = _ReadEventLog(hdl, flags, offs, buf, want, ref(got), ref(want))
         got = got.value
         if not ok:
             err = GetLastError()
             if err == ERROR_HANDLE_EOF:
                 got = 0
                 break
```

### Comparing `ctwin32-2.5.0/ctwin32/bcrypt.py` & `ctwin32-2.6.0/ctwin32/bcrypt.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 #
 ################################################################################
 
 import ctypes
 from .wtypes import (
+    byte_buffer,
+    string_buffer,
     ENDIANNESS,
     HANDLE,
     NTSTATUS,
     PCHAR,
     PHANDLE,
     PULONG,
     PVOID,
@@ -208,15 +210,15 @@
         ULONG
         )
     )
 
 def BCryptGetProperty(obj, name):
     size = ULONG()
     raise_failed_status(_BCryptGetProperty(obj, name, None, 0, ref(size), 0))
-    buf = ctypes.create_string_buffer(size.value)
+    buf = byte_buffer(size.value)
     raise_failed_status(_BCryptGetProperty(obj, name, buf, size, ref(size), 0))
     return bytes(buf)
 
 def get_property_ulong(obj, name):
     _bytes = BCryptGetProperty(obj, name)
     if len(_bytes) != ctypes.sizeof(ULONG):
         raise ValueError(f"property size mismatch ({len(_bytes)})")
@@ -235,15 +237,15 @@
         )
     )
 
 def BCryptSetProperty(obj, name, value):
     if isinstance(value, int):
         buf = value.to_bytes(((value.bit_length() + 31) // 32) * 4, ENDIANNESS)
     elif isinstance(value, str):
-        buf = bytes(ctypes.create_unicode_buffer(value))
+        buf = bytes(string_buffer(value))
     else:
         buf = bytes(value)
     raise_failed_status(_BCryptSetProperty(obj, name, buf, len(buf), 0))
 
 ################################################################################
 
 _BCryptCreateHash = fun_fact(
@@ -287,15 +289,15 @@
 ################################################################################
 
 _BCryptFinishHash = fun_fact(
     _bcr.BCryptFinishHash, (NTSTATUS, HANDLE, PCHAR, ULONG, ULONG)
     )
 
 def BCryptFinishHash(bhash, dig_size):
-    buf = ctypes.create_string_buffer(dig_size)
+    buf = byte_buffer(dig_size)
     raise_failed_status(_BCryptFinishHash(bhash, buf, len(buf), 0))
     return bytes(buf)
 
 ################################################################################
 
 class BCryptHash:
     "standard python hash wrapper for a BCrypt hash"
@@ -306,15 +308,15 @@
         self.hash = None
         self.obj_buf = None
         self.balg = None
         try:
             self.balg = BCryptOpenAlgorithmProvider(alg)
             self.dig_size = get_property_ulong(self.balg, BCRYPT_HASH_LENGTH)
             obj_size = get_property_ulong(self.balg, BCRYPT_OBJECT_LENGTH)
-            self.obj_buf = ctypes.create_string_buffer(obj_size)
+            self.obj_buf = byte_buffer(obj_size)
             self.hash = BCryptCreateHash(self.balg, self.obj_buf)
         except OSError:
             self.close()
             raise
 
     def close(self):
         if self.hash is not None:
@@ -378,15 +380,15 @@
     )
 
 def BCryptExportKey(key, btype, exp_key=None):
     size = ULONG()
     raise_failed_status(
         _BCryptExportKey(key, exp_key, btype, None, 0, ref(size), 0)
         )
-    blob = ctypes.create_string_buffer(size.value)
+    blob = byte_buffer(size.value)
     raise_failed_status(
         _BCryptExportKey(key, exp_key, btype, blob, size, ref(size), 0)
         )
     return bytes(blob)
 
 ################################################################################
 
@@ -422,15 +424,15 @@
         ULONG
         )
     )
 
 def BCryptGenerateSymmetricKey(balg, secret):
     ksize = get_property_ulong(balg, BCRYPT_OBJECT_LENGTH)
     key = BCRYPT_KEY()
-    key.buf = ctypes.create_string_buffer(ksize)
+    key.buf = byte_buffer(ksize)
     raise_failed_status(
         _BCryptGenerateSymmetricKey(
             balg,
             ref(key),
             key.buf,
             len(key.buf),
             secret,
@@ -488,15 +490,15 @@
             len(digest),
             None,
             0,
             ref(size),
             flags
             )
         )
-    signature = ctypes.create_string_buffer(size.value)
+    signature = byte_buffer(size.value)
     raise_failed_status(
         _BCryptSignHash(
             key,
             None,
             digest,
             len(digest),
             signature,
@@ -566,15 +568,15 @@
             0 if iv is None else len(iv),
             None,
             0,
             ref(size),
             flags
             )
         )
-    output = ctypes.create_string_buffer(size.value)
+    output = byte_buffer(size.value)
     raise_failed_status(
         _BCryptEncrypt(
             key,
             input,
             len(input),
             None,
             iv,
@@ -617,15 +619,15 @@
             0 if iv is None else len(iv),
             None,
             0,
             ref(size),
             flags
             )
         )
-    output = ctypes.create_string_buffer(size.value)
+    output = byte_buffer(size.value)
     raise_failed_status(
         _BCryptDecrypt(
             key,
             input,
             len(input),
             None,
             iv,
```

### Comparing `ctwin32-2.5.0/ctwin32/cfgmgr.py` & `ctwin32-2.6.0/ctwin32/cfgmgr.py`

 * *Files 21% similar despite different names*

```diff
@@ -20,31 +20,36 @@
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 #
 ################################################################################
 
 import ctypes
 from .wtypes import (
+    byte_buffer,
+    string_buffer,
     DWORD,
     GUID,
     INT,
     PDWORD,
     PGUID,
     PINT,
     PVOID,
     PWSTR,
     PULONG,
     ULONG,
     )
 from . import (
     ref,
     fun_fact,
+    multi_str_from_str,
     MAX_DEVICE_ID_LEN,
     MAX_PATH,
+    CM_GET_DEVICE_INTERFACE_LIST_PRESENT,
     CM_LOCATE_DEVNODE_NORMAL,
+    CR_BUFFER_SMALL,
     CR_SUCCESS,
     ERROR_FLOPPY_UNKNOWN_ERROR,
     ERROR_CURRENT_DIRECTORY,
     )
 from .advapi import registry_to_py
 _cfg = ctypes.WinDLL("cfgmgr32.dll")
 
@@ -62,15 +67,15 @@
 
 _CM_Get_Device_ID = fun_fact(
     _cfg.CM_Get_Device_IDW,
     (DWORD, DWORD, PWSTR, ULONG, ULONG)
     )
 
 def CM_Get_Device_ID(devinst):
-    idstr = ctypes.create_unicode_buffer(MAX_DEVICE_ID_LEN)
+    idstr = string_buffer(MAX_DEVICE_ID_LEN)
     raise_on_cr(_CM_Get_Device_ID(devinst, idstr, MAX_DEVICE_ID_LEN, 0))
     return idstr.value
 
 ################################################################################
 
 _CM_Get_DevNode_Status = fun_fact(
     _cfg.CM_Get_DevNode_Status,
@@ -87,15 +92,15 @@
 
 _CM_Enumerate_Enumerators = fun_fact(
     _cfg.CM_Enumerate_EnumeratorsW,
     (DWORD, ULONG, PWSTR, PULONG, ULONG)
     )
 
 def CM_Enumerate_Enumerators(idx):
-    enum_str = ctypes.create_unicode_buffer(MAX_DEVICE_ID_LEN)
+    enum_str = string_buffer(MAX_DEVICE_ID_LEN)
     size = ULONG(MAX_DEVICE_ID_LEN)
     raise_on_cr(_CM_Enumerate_Enumerators(idx, enum_str, ref(size), 0))
     return enum_str.value
 
 ################################################################################
 
 _CM_Enumerate_Classes = fun_fact(
@@ -129,15 +134,15 @@
         ULONG,
         ULONG
         )
     )
 
 def CM_Request_Device_Eject(devinst):
     veto_type = INT()
-    veto_name = ctypes.create_unicode_buffer(MAX_PATH)
+    veto_name = string_buffer(MAX_PATH)
     err = _CM_Request_Device_Eject(
         devinst,
         ref(veto_type),
         veto_name,
         MAX_PATH,
         0
         )
@@ -180,21 +185,84 @@
         devinst,
         prop,
         ref(reg_type),
         None,
         ref(req_size),
         0
         )
-    buf = ctypes.create_string_buffer(req_size.value)
+    buf = byte_buffer(req_size.value)
     raise_on_cr(
         _CM_Get_DevNode_Registry_Property(
             devinst,
             prop,
             ref(reg_type),
             buf,
             ref(req_size),
             0
             )
         )
     return registry_to_py(reg_type.value, buf.raw[:req_size.value])
 
 ################################################################################
+
+_CM_Get_Device_Interface_List_Size = fun_fact(
+    _cfg.CM_Get_Device_Interface_List_SizeW, (
+        DWORD,
+        PULONG,
+        PGUID,
+        PWSTR,
+        ULONG
+        )
+    )
+
+def CM_Get_Device_Interface_List_Size(
+    guid,
+    didstr,
+    flags=CM_GET_DEVICE_INTERFACE_LIST_PRESENT
+    ):
+    size = ULONG()
+    raise_on_cr(
+        _CM_Get_Device_Interface_List_Size(
+            ref(size),
+            ref(guid),
+            didstr,
+            flags
+            )
+        )
+    return size.value
+
+################################################################################
+
+_CM_Get_Device_Interface_List = fun_fact(
+    _cfg.CM_Get_Device_Interface_ListW, (
+        DWORD,
+        PGUID,
+        PWSTR,
+        PWSTR,
+        ULONG,
+        ULONG
+        )
+    )
+
+def CM_Get_Device_Interface_List(
+    guid,
+    didstr,
+    flags=CM_GET_DEVICE_INTERFACE_LIST_PRESENT
+    ):
+    res = CR_BUFFER_SMALL
+    while res == CR_BUFFER_SMALL:
+        size = ULONG(CM_Get_Device_Interface_List_Size(guid, didstr, flags))
+        iface = string_buffer(size.value)
+        res = _CM_Get_Device_Interface_List(
+            ref(guid),
+            didstr,
+            iface,
+            size,
+            flags
+            )
+        if res == CR_SUCCESS:
+            return multi_str_from_str(iface.value)
+        if res != CR_BUFFER_SMALL:
+            raise_on_cr(res)
+    return []
+
+################################################################################
```

### Comparing `ctwin32-2.5.0/ctwin32/comctl.py` & `ctwin32-2.6.0/ctwin32/comctl.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.5.0/ctwin32/gdi.py` & `ctwin32-2.6.0/ctwin32/gdi.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,27 +22,32 @@
 #
 ################################################################################
 
 import ctypes
 from .wtypes import (
     BOOL,
     BYTE,
+    DWORD,
     HANDLE,
     INT,
     LONG,
+    PINT,
     PLOGFONT,
     POINTER,
+    PRECT,
     PWSTR,
+    UINT,
     WCHAR,
     )
 from . import (
     ref,
     raise_if,
     raise_on_zero,
     fun_fact,
+    ETO_OPAQUE,
     HGDI_ERROR,
     )
 
 _gdi = ctypes.WinDLL("gdi32.dll")
 
 ################################################################################
 
@@ -125,13 +130,42 @@
 def SetBkMode(hdc, mode):
     previous = _SetBkMode(hdc, mode)
     raise_on_zero(previous)
     return previous
 
 ################################################################################
 
+_SetBkColor = fun_fact(_gdi.SetBkColor, (DWORD, HANDLE, DWORD))
+
+def SetBkColor(hdc, colorref):
+    previous = _SetBkColor(hdc, colorref)
+    raise_on_zero(previous)
+    return previous
+
+################################################################################
+
 _TextOut = fun_fact(_gdi.TextOutW, (BOOL, HANDLE, INT, INT, PWSTR, INT))
 
 def TextOut(hdc, x, y, text):
     raise_on_zero(_TextOut(hdc, x, y, text, len(text)))
 
 ################################################################################
+
+_ExtTextOut = fun_fact(
+    _gdi.ExtTextOutW,
+    (BOOL, HANDLE, INT, INT, UINT, PRECT, PWSTR, UINT, PINT)
+    )
+
+def ExtTextOut(hdc, x, y, opt, rect, text, pDX=None):
+    span = len(text) if text else 0
+    raise_on_zero(
+        _ExtTextOut(hdc, x, y, opt, ref(rect), text, span, pDX)
+        )
+
+################################################################################
+
+def fill_solid_rect(hdc, rect, colorref):
+    oldclr = SetBkColor(hdc, colorref)
+    ExtTextOut(hdc, 0, 0, ETO_OPAQUE, rect, None, None)
+    SetBkColor(hdc, oldclr)
+
+################################################################################
```

### Comparing `ctwin32-2.5.0/ctwin32/iphlpapi.py` & `ctwin32-2.6.0/ctwin32/iphlpapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 
 import ipaddress as _iaddr
 from types import SimpleNamespace as _namespace
 from collections import defaultdict as _defdict
 
 import ctypes
 from .wtypes import (
+    byte_buffer,
+    string_buffer,
     BYTE,
     DWORD,
     GUID,
     INT,
     PCHAR,
     PGUID,
     POINTER,
@@ -309,15 +311,15 @@
         GAA_FLAG_INCLUDE_PREFIX |
         GAA_FLAG_SKIP_ANYCAST |
         GAA_FLAG_SKIP_MULTICAST
         )
     blen = ULONG(16 * 1024)
     error = ERROR_BUFFER_OVERFLOW
     while error == ERROR_BUFFER_OVERFLOW:
-        buffer = ctypes.create_string_buffer(blen.value)
+        buffer = byte_buffer(blen.value)
         p_addr = ctypes.cast(buffer, PIP_ADAPTER_ADDRESSES)
         error = _GetAdaptersAddresses(fam, flags, None, p_addr, ref(blen))
     raise_on_err(error)
 
     return _adapter_addresses_to_interfaces(p_addr, include_loopback)
 
 ################################################################################
@@ -406,26 +408,26 @@
     )
 
 IF_MAX_STRING_SIZE = 256
 
 def ConvertInterfaceLuidToAlias(luid):
     luid = ULONGLONG(luid)
     size = SIZE_T(IF_MAX_STRING_SIZE + 1)
-    alias = ctypes.create_unicode_buffer(size.value)
+    alias = string_buffer(size.value)
     raise_on_err(_ConvertInterfaceLuidToAlias(ref(luid), alias, size))
     return alias.value
 
 ################################################################################
 
 _ConvertInterfaceLuidToName = fun_fact(
     _iph.ConvertInterfaceLuidToNameW,
     (DWORD, PULONGLONG, PWSTR, SIZE_T)
     )
 
 def ConvertInterfaceLuidToName(luid):
     luid = ULONGLONG(luid)
     size = SIZE_T(IF_MAX_STRING_SIZE + 1)
-    name = ctypes.create_unicode_buffer(size.value)
+    name = string_buffer(size.value)
     raise_on_err(_ConvertInterfaceLuidToName(ref(luid), name, size))
     return name.value
 
 ################################################################################
```

### Comparing `ctwin32-2.5.0/ctwin32/kernel.py` & `ctwin32-2.6.0/ctwin32/kernel.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,23 +23,26 @@
 ################################################################################
 
 import collections as _collections
 from enum import IntEnum as _int_enum
 
 import ctypes
 from .wtypes import (
+    byte_buffer,
+    string_buffer,
     BOOL,
     BYTE,
     CallbackContext,
     CallbackContextPtr,
     CHAR,
     DWORD,
     FILETIME,
     HANDLE,
     INT,
+    LARGE_INTEGER,
     PBOOL,
     PBYTE,
     PDWORD,
     POINTER,
     PPWSTR,
     PSIZE_T,
     PULONG_PTR,
@@ -291,15 +294,15 @@
         iptr, ilen = None, 0
     else:
         iptr, ilen = ref(in_ctobj), ctypes.sizeof(in_ctobj)
 
     if out_len is None or out_len == 0:
         out, optr, olen = None, None, 0
     else:
-        out = ctypes.create_string_buffer(out_len)
+        out = byte_buffer(out_len)
         optr, olen = ref(out), out_len
 
     raise_on_zero(
         _DeviceIoControl(
             hdl,
             ioctl,
             iptr,
@@ -318,15 +321,14 @@
 
 _CreateIoCompletionPort = fun_fact(
     _k32.CreateIoCompletionPort,
     (KHANDLE, HANDLE, HANDLE, ULONG_PTR, DWORD)
     )
 
 def CreateIoCompletionPort(file, existing, key, num_threads):
-    print(f"{file=}, {existing=}, {key=}, {num_threads=}")
     ioport = _CreateIoCompletionPort(file, existing, key, num_threads)
     ioport.raise_on_invalid()
     return ioport
 
 def create_io_completion_port(file, key, num_threads=0, existing=None):
     return CreateIoCompletionPort(file, existing, key, num_threads)
 
@@ -386,15 +388,15 @@
     )
 
 def GetModuleFileName(hmod):
     size = 128
     res = size
     while res >= size:
         size *= 2
-        buf = ctypes.create_unicode_buffer(size)
+        buf = string_buffer(size)
         res = _GetModuleFileName(hmod, buf, size)
     raise_on_zero(res)
     return buf.value
 
 ################################################################################
 
 _WaitForSingleObject = fun_fact(
@@ -447,23 +449,23 @@
 
 _QueryDosDevice = fun_fact(
     _k32.QueryDosDeviceW, (DWORD, PWSTR, PWSTR, DWORD)
     )
 
 def QueryDosDevice(device_name):
     size = 512
-    buf = ctypes.create_unicode_buffer(size)
+    buf = string_buffer(size)
     while True:
         if res := _QueryDosDevice(device_name, buf, size):
             if device_name is None:
                 return multi_str_from_ubuf(buf, res)
             return buf.value[:res]
         raise_if(GetLastError() != ERROR_INSUFFICIENT_BUFFER)
         size *= 2
-        buf = ctypes.create_unicode_buffer(size)
+        buf = string_buffer(size)
 
 ################################################################################
 
 def GetSystemTime():
     st = SYSTEMTIME()
     _k32.GetSystemTime(ref(st))
     return st
@@ -587,36 +589,36 @@
 _GetPrivateProfileSectionNames = fun_fact(
     _k32.GetPrivateProfileSectionNamesW,
     (DWORD, PWSTR, DWORD, PWSTR)
     )
 
 def GetPrivateProfileSectionNames(filename):
     size = 512
-    buf = ctypes.create_unicode_buffer(size)
+    buf = string_buffer(size)
     res = _GetPrivateProfileSectionNames(buf, size, filename)
     while res == size - 2:
         size *= 2
-        buf = ctypes.create_unicode_buffer(size)
+        buf = string_buffer(size)
         res = _GetPrivateProfileSectionNames(buf, size, filename)
     return multi_str_from_ubuf(buf, res)
 
 ################################################################################
 
 _GetPrivateProfileSection = fun_fact(
     _k32.GetPrivateProfileSectionW,
     (DWORD, PWSTR, PWSTR, DWORD, PWSTR)
     )
 
 def GetPrivateProfileSection(secname, filename):
     size = 512
-    buf = ctypes.create_unicode_buffer(size)
+    buf = string_buffer(size)
     res = _GetPrivateProfileSection(secname, buf, size, filename)
     while res == size - 2:
         size *= 2
-        buf = ctypes.create_unicode_buffer(size)
+        buf = string_buffer(size)
         res = _GetPrivateProfileSection(secname, buf, size, filename)
     entries = multi_str_from_ubuf(buf, res)
     d = _collections.OrderedDict()
     for e in entries:
         k, v = e.split("=", 1)
         d[k] = v
     return d
@@ -640,28 +642,28 @@
             secdata = "\0\0"
     # quote from https://github.com/python/cpython/issues/76926 concerning
     # CPython versions up to 3.9:
     #   "PyUnicode_AsWideCharString was updated to raise ValueError for
     #    embedded nulls if the 'size' output parameter is NULL."
     # That's why we need to detour 'secdata' through a unicode buffer. Since
     # py310 that would no longer be necessary (ctypes was fixed).
-    buf = ctypes.create_unicode_buffer(secdata, len(secdata))
+    buf = string_buffer(secdata, len(secdata))
     raise_on_zero(_WritePrivateProfileSection(secname, buf, filename))
 
 ################################################################################
 
 _GetEnvironmentVariable = fun_fact(
     _k32.GetEnvironmentVariableW,
     (DWORD, PWSTR, PWSTR, DWORD)
     )
 
 def GetEnvironmentVariable(name):
     size = 512
     while True:
-        var = ctypes.create_unicode_buffer(size)
+        var = string_buffer(size)
         req = _GetEnvironmentVariable(name, var, size)
         raise_on_zero(req)
         if req <= size:
             break
         size = req
     return var.value
 
@@ -705,28 +707,28 @@
 _SetEnvironmentStrings = fun_fact(
     _k32.SetEnvironmentStringsW,
     (BOOL, PWSTR)
     )
 
 def SetEnvironmentStrings(strings):
     # see comment on PyUnicode_AsWideCharString above
-    buf = ctypes.create_unicode_buffer(strings, len(strings))
+    buf = string_buffer(strings, len(strings))
     raise_on_zero(_SetEnvironmentStrings(buf))
 
 ################################################################################
 
 _ExpandEnvironmentStrings = fun_fact(
     _k32.ExpandEnvironmentStringsW,
     (DWORD, PWSTR, PWSTR, DWORD)
     )
 
 def ExpandEnvironmentStrings(template):
     size = len(template)
     while True:
-        var = ctypes.create_unicode_buffer(size)
+        var = string_buffer(size)
         req = _ExpandEnvironmentStrings(template, var, size)
         raise_on_zero(req)
         if req <= size:
             break
         size = req
     return var.value
 
@@ -832,15 +834,15 @@
 
 ################################################################################
 
 class ProcThreadAttributeList:
     def __init__(self, attr_pairs):
         self.buf = None
         size = InitializeProcThreadAttributeList(None, len(attr_pairs), 0)
-        buf = ctypes.create_string_buffer(size)
+        buf = byte_buffer(size)
         InitializeProcThreadAttributeList(buf, 1, 0, size)
         try:
             for id, value in attr_pairs:
                 UpdateProcThreadAttribute(buf, 0, id, value)
         except OSError:
             DeleteProcThreadAttributeList(buf)
             raise
@@ -960,40 +962,71 @@
 
 class JOBOBJECT_ASSOCIATE_COMPLETION_PORT(ctypes.Structure):
     _fields_ = (
         ("CompletionKey", PVOID),
         ("CompletionPort", HANDLE),
         )
 
+class JOBOBJECT_BASIC_ACCOUNTING_INFORMATION(ctypes.Structure):
+    _fields_ = (
+        ("TotalUserTime", LARGE_INTEGER),
+        ("TotalKernelTime", LARGE_INTEGER),
+        ("ThisPeriodTotalUserTime", LARGE_INTEGER),
+        ("ThisPeriodTotalKernelTime", LARGE_INTEGER),
+        ("TotalPageFaultCount", DWORD),
+        ("TotalProcesses", DWORD),
+        ("ActiveProcesses", DWORD),
+        ("TotalTerminatedProcesses", DWORD),
+    )
+
 ################################################################################
 
 _SetInformationJobObject = fun_fact(
     _k32.SetInformationJobObject,
     (BOOL, HANDLE, INT, PVOID, DWORD)
     )
 
 def SetInformationJobObject(job, cls, ct_info):
     size = ctypes.sizeof(ct_info)
     raise_on_zero(_SetInformationJobObject(job, cls, ref(ct_info), size))
 
 ################################################################################
 
+_QueryInformationJobObject = fun_fact(
+    _k32.QueryInformationJobObject,
+    (BOOL, HANDLE, INT, PVOID, DWORD, PDWORD)
+    )
+
+def QueryInformationJobObject(job, cls, res_obj):
+    raise_on_zero(
+        _QueryInformationJobObject(
+            job,
+            cls,
+            ref(res_obj),
+            ctypes.sizeof(res_obj),
+            None
+            )
+        )
+    return res_obj
+
+################################################################################
+
 _ResumeThread = fun_fact(_k32.ResumeThread, (DWORD, HANDLE))
 
 def ResumeThread(thdl):
     scnt = _ResumeThread(thdl)
     raise_if(scnt == 0xffffffff)
     return scnt
 
 ################################################################################
 
 def _get_dir(func, order):
     buf_size = 256
     while True:
-        buf = ctypes.create_unicode_buffer(buf_size)
+        buf = string_buffer(buf_size)
         req_size = func(*((buf, buf_size) if order else (buf_size, buf)))
         if req_size <= buf_size:
             return buf.value
         buf_size = req_size
 
 ################################################################################
 
@@ -1089,15 +1122,15 @@
 ################################################################################
 
 _GlobalGetAtomName = fun_fact(_k32.GlobalGetAtomNameW, (UINT, WORD, PWSTR, INT))
 
 def GlobalGetAtomName(atom):
     size = 512
     while True:
-        var = ctypes.create_unicode_buffer(size)
+        var = string_buffer(size)
         req = _GlobalGetAtomName(atom, var, size)
         raise_on_zero(req)
         if req <= size:
             break
         size = req
     return var.value
 
@@ -1660,36 +1693,36 @@
 
 _GetLogicalDriveStrings = fun_fact(
     _k32.GetLogicalDriveStringsW, (DWORD, DWORD, PWSTR)
     )
 
 def GetLogicalDriveStrings():
     size = 256
-    buf = ctypes.create_unicode_buffer(size)
+    buf = string_buffer(size)
     raise_on_zero(res := _GetLogicalDriveStrings(size, buf))
     return multi_str_from_ubuf(buf, res)
 
 ################################################################################
 
 _FindFirstVolume = fun_fact(_k32.FindFirstVolumeW, (HANDLE, PWSTR, DWORD))
 
 def FindFirstVolume():
     size = 256
-    buf = ctypes.create_unicode_buffer(size)
+    buf = string_buffer(size)
     hdl = _FindFirstVolume(buf, size)
     raise_if(hdl == INVALID_HANDLE_VALUE)
     return hdl, buf.value
 
 ################################################################################
 
 _FindNextVolume = fun_fact(_k32.FindNextVolumeW, (BOOL, HANDLE, PWSTR, DWORD))
 
 def FindNextVolume(hdl):
     size = 256
-    buf = ctypes.create_unicode_buffer(size)
+    buf = string_buffer(size)
     raise_on_zero(_FindNextVolume(hdl, buf, size))
     return buf.value
 
 ################################################################################
 
 _FindVolumeClose = fun_fact(_k32.FindVolumeClose, (BOOL, HANDLE))
 
@@ -1715,30 +1748,30 @@
 _GetVolumePathNamesForVolumeName = fun_fact(
     _k32.GetVolumePathNamesForVolumeNameW, (BOOL, PWSTR, PWSTR, DWORD, PDWORD)
     )
 
 def GetVolumePathNamesForVolumeName(vol):
     size = DWORD(256)
     while True:
-        buf = ctypes.create_unicode_buffer(size.value)
+        buf = string_buffer(size.value)
         ok = _GetVolumePathNamesForVolumeName(vol, buf, size, ref(size))
         if ok:
             return multi_str_from_ubuf(buf, size.value)
         else:
             if (err := GetLastError()) != ERROR_MORE_DATA:
                 raise_on_err(err)
 
 ################################################################################
 
 _ReadProcessMemory = fun_fact(
     _k32.ReadProcessMemory, (BOOL, HANDLE, PVOID, PVOID, SIZE_T, PSIZE_T)
     )
 
 def ReadProcessMemory(hdl, addr, length):
-    buf = ctypes.create_string_buffer(length)
+    buf = byte_buffer(length)
     raise_on_zero(_ReadProcessMemory(hdl, addr, buf, length, None))
     return buf
 
 ################################################################################
 
 _WriteProcessMemory = fun_fact(
     _k32.WriteProcessMemory, (BOOL, HANDLE, PVOID, PVOID, SIZE_T, PSIZE_T)
```

### Comparing `ctwin32-2.5.0/ctwin32/misc.py` & `ctwin32-2.6.0/ctwin32/misc.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 #
 ################################################################################
 
 import ctypes
 from .wtypes import (
+    byte_buffer,
+    string_buffer,
     BOOL,
     BOOLEAN,
     DWORD,
     ENDIANNESS,
     HANDLE,
     LONG,
     PDWORD,
@@ -58,15 +60,15 @@
 _CallNtPowerInformation = fun_fact(
     _popro.CallNtPowerInformation,
     (LONG, LONG, PVOID, ULONG, PVOID, ULONG),
     )
 
 def CallNtPowerInformation(level, outsize=0, input=None):
     src, slen = (None, 0) if not input else (ref(input), ULONG(len(input)))
-    dst, dlen = ctypes.create_string_buffer(outsize), ULONG(outsize)
+    dst, dlen = byte_buffer(outsize), ULONG(outsize)
     raise_failed_status(_CallNtPowerInformation(level, src, slen, dst, dlen))
     return dst.raw
 
 ################################################################################
 
 def get_system_execution_state():
     bts = CallNtPowerInformation(SystemExecutionState, ctypes.sizeof(ULONG))
@@ -152,34 +154,34 @@
     _ue.DestroyEnvironmentBlock, (BOOL, PVOID)
     )
 
 _CreateEnvironmentBlock = fun_fact(
     _ue.CreateEnvironmentBlock, (BOOL, PPVOID, HANDLE, BOOL)
     )
 
-def _env_block_from_token(token):
+def _env_block_from_token(token, inherit):
     ptr = PVOID()
-    raise_on_zero(_CreateEnvironmentBlock(ref(ptr), token, False))
+    raise_on_zero(_CreateEnvironmentBlock(ref(ptr), token, inherit))
     try:
         return multi_str_from_addr(ptr.value)
     finally:
         raise_on_zero(_DestroyEnvironmentBlock(ptr))
 
-def CreateEnvironmentBlock(token=None):
+def CreateEnvironmentBlock(token=None, inherit=False):
     if token is None:
         with advapi.OpenProcessToken(
                 kernel.GetCurrentProcess(),
                 TOKEN_READ
                 ) as t:
-            return _env_block_from_token(t)
+            return _env_block_from_token(t, inherit)
     else:
-        return _env_block_from_token(token)
+        return _env_block_from_token(token, inherit)
 
-def create_env_block_as_dict(token=None):
-    return kernel.env_str_to_dict(CreateEnvironmentBlock(token))
+def create_env_block_as_dict(token=None, inherit=False):
+    return kernel.env_str_to_dict(CreateEnvironmentBlock(token, inherit))
 
 ################################################################################
 
 _dbghlp = ctypes.WinDLL("dbghelp.dll")
 
 UNDNAME_COMPLETE = 0x0000
 UNDNAME_NO_LEADING_UNDERSCORES = 0x0001
@@ -204,15 +206,15 @@
 _UnDecorateSymbolName = fun_fact(
     _dbghlp.UnDecorateSymbolNameW, (DWORD, PWSTR, PWSTR, DWORD, DWORD)
     )
 
 def UnDecorateSymbolName(sym_name, flags=UNDNAME_COMPLETE):
     size = 256
     while True:
-        buf = ctypes.create_unicode_buffer(size)
+        buf = string_buffer(size)
         result = _UnDecorateSymbolName(sym_name, buf, size, flags)
         raise_on_zero(result)
         if result <= size - 4:
             return buf.value
         size *= 2
 
 ################################################################################
```

### Comparing `ctwin32-2.5.0/ctwin32/msi.py` & `ctwin32-2.6.0/ctwin32/msi.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 #
 ################################################################################
 
 import ctypes
 from .wtypes import (
+    byte_buffer,
+    string_buffer,
     DWORD,
     PCHAR,
     PDWORD,
     POINTER,
     PWSTR,
     ScdToBeClosed,
     UINT,
@@ -116,29 +118,38 @@
     with suppress_winerr(ERROR_NO_MORE_ITEMS):
         while True:
             with MsiViewFetch(view) as record:
                 yield record
 
 ################################################################################
 
+_MsiRecordGetFieldCount = fun_fact(
+    _msi.MsiRecordGetFieldCount, (UINT, MSIHANDLE)
+    )
+
+def MsiRecordGetFieldCount(record):
+    return _MsiRecordGetFieldCount(record)
+
+################################################################################
+
 _MsiRecordGetString = fun_fact(
     _msi.MsiRecordGetStringW, (
         UINT,
         MSIHANDLE,
         UINT,
         PWSTR,
         PDWORD
         )
     )
 
 def MsiRecordGetString(record, field_idx):
     size = DWORD(512)
     err = ERROR_MORE_DATA
     while err == ERROR_MORE_DATA:
-        buf = ctypes.create_unicode_buffer(size.value)
+        buf = string_buffer(size.value)
         err = _MsiRecordGetString(record, field_idx, buf, ref(size))
     raise_on_err(err)
     return buf.value
 
 ################################################################################
 
 _MsiRecordReadStream = fun_fact(
@@ -148,15 +159,15 @@
         UINT,
         PCHAR,
         PDWORD
         )
     )
 
 def MsiRecordReadStream(record, field_idx, size):
-    res = ctypes.create_string_buffer(size)
+    res = byte_buffer(size)
     size = DWORD(size)
     raise_on_err(_MsiRecordReadStream(record, field_idx, res, ref(size)))
     return res.raw[:size.value]
 
 ################################################################################
 
 def record_read_stream_all(record, field_idx):
```

### Comparing `ctwin32-2.5.0/ctwin32/ntdll.py` & `ctwin32-2.6.0/ctwin32/ntdll.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,18 @@
 
 from enum import IntFlag as _int_flag
 from types import SimpleNamespace as _namespace
 from collections import defaultdict as _defdict
 
 import ctypes
 from .wtypes import (
+    byte_buffer,
+    string_buffer,
     BOOLEAN,
+    BYTE,
     FILETIME,
     HANDLE,
     LARGE_INTEGER,
     LONG,
     LONG_PTR,
     INT,
     NTSTATUS,
@@ -131,14 +134,43 @@
         ("HandleCount", ULONG),
         ("SessionId", ULONG),
         ("UniqueProcessKey", UINT_PTR),
         )
 
 ################################################################################
 
+class SYSTEM_BASIC_INFORMATION(ctypes.Structure):
+    _fields_ = (
+        ("Reserved", ULONG),
+        ("TimerResolution", ULONG),
+        ("PageSize", ULONG),
+        ("NumberOfPhysicalPages", ULONG),
+        ("LowestPhysicalPageNumber", ULONG),
+        ("HighestPhysicalPageNumber", ULONG),
+        ("AllocationGranularity", ULONG),
+        ("MinimumUserModeAddress", ULONG_PTR),
+        ("MaximumUserModeAddress", ULONG_PTR),
+        ("ActiveProcessorsAffinityMask", ULONG_PTR),
+        ("NumberOfProcessors", BYTE),
+        )
+
+################################################################################
+
+class SYSTEM_PROCESSOR_PERFORMANCE_INFORMATION(ctypes.Structure):
+    _fields_ = (
+        ("IdleTime", LARGE_INTEGER),
+        ("KernelTime", LARGE_INTEGER),
+        ("UserTime", LARGE_INTEGER),
+        ("DpcTime", LARGE_INTEGER),
+        ("InterruptTime", LARGE_INTEGER),
+        ("InterruptCount", ULONG),
+        )
+
+################################################################################
+
 class CLIENT_ID(ctypes.Structure):
     _fields_ = (
         ("UniqueProcess", LONG_PTR),
         ("UniqueThread", LONG_PTR)
         )
 
 ################################################################################
@@ -276,15 +308,15 @@
 
 def _var_size_proc_info(proc_handle, proc_info):
     # This works only for the few information classes that return variable
     # size items (50, 51, 60, 64, 85, 97). Those that deliver fixed size items
     # cannot be queried for the required size.
     size = ULONG(0)
     NtQueryInformationProcess(proc_handle, proc_info, 0, size, ref(size))
-    buff = ctypes.create_string_buffer(size.value)
+    buff = byte_buffer(size.value)
     raise_failed_status(
         NtQueryInformationProcess(proc_handle, proc_info, buff, size, ref(size))
         )
     return buff
 
 ################################################################################
 
@@ -306,15 +338,15 @@
             pid=pi.UniqueProcessId or 0
             )
 
     status = STATUS_INFO_LENGTH_MISMATCH
     while status == STATUS_INFO_LENGTH_MISMATCH:
         size = ULONG(0)
         NtQuerySystemInformation(SystemProcessInformation, 0, 0, ref(size))
-        buf = ctypes.create_string_buffer(size.value)
+        buf = byte_buffer(size.value)
         status = NtQuerySystemInformation(
             SystemProcessInformation,
             ref(buf),
             size,
             ref(size)
             )
     raise_failed_status(status)
@@ -349,15 +381,15 @@
 def proc_path_from_pid(pid):
 
     if pid == 0:
         return "idle"
     elif pid == 4:
         return "system"
 
-    buf = ctypes.create_unicode_buffer(512)
+    buf = string_buffer(512)
     size = ctypes.sizeof(SYSTEM_PROCESS_ID_INFORMATION)
     spii = SYSTEM_PROCESS_ID_INFORMATION()
     spii.ProcessId = ctypes.cast(pid, HANDLE)
     spii.ImageName.Length = 0
     spii.ImageName.MaximumLength = buf._length_
     spii.ImageName.Buffer = ctypes.addressof(buf)
 
@@ -368,15 +400,15 @@
             size,
             None
             )
         if status != STATUS_INFO_LENGTH_MISMATCH:
             break
 
         # Required length is stored in MaximumLength.
-        buf = ctypes.create_unicode_buffer(spii.ImageName.MaximumLength)
+        buf = string_buffer(spii.ImageName.MaximumLength)
         spii.ImageName.Buffer = ctypes.addressof(buf)
 
     raise_failed_status(status)
     return _resolve_device_prefix(str(spii.ImageName))
 
 ################################################################################
 
@@ -496,15 +528,15 @@
 
 ################################################################################
 
 def get_directory_info(hdir, restart_scan):
     iosb = IO_STATUS_BLOCK()
     bsize = 256
     while True:
-        buf = ctypes.create_string_buffer(bsize)
+        buf = byte_buffer(bsize)
         stat = _NtQueryDirectoryFile(
             hdir,
             None,
             None,
             None,
             ref(iosb),
             buf,
@@ -579,17 +611,17 @@
 def NtPowerInformation(pwr_info, in_bytes, out_len):
     if in_bytes is None:
         iptr, ilen = None, 0
     else:
         iptr, ilen = ref(in_bytes), len(in_bytes)
 
     if out_len is None or out_len == 0:
-        out, optr, olen = ctypes.create_string_buffer(0), None, 0
+        out, optr, olen = byte_buffer(0), None, 0
     else:
-        out = ctypes.create_string_buffer(out_len)
+        out = byte_buffer(out_len)
         optr, olen = ref(out), out_len
 
     raise_failed_status(_NtPowerInformation(pwr_info, iptr, ilen, optr, olen))
     return out
 
 ################################################################################
```

### Comparing `ctwin32-2.5.0/ctwin32/psapi.py` & `ctwin32-2.6.0/ctwin32/psapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 #
 ################################################################################
 
 import ctypes
 from .wtypes import (
+    string_buffer,
     BOOL,
     DWORD,
     HANDLE,
     HMODULE,
     PDWORD,
     POINTER,
     PVOID,
@@ -81,30 +82,30 @@
     )
 
 def GetMappedFileName(hdl, addr):
     size = 128
     length = size
     while length == size:
         size *= 2
-        name = ctypes.create_unicode_buffer(size)
+        name = string_buffer(size)
         length = _GetMappedFileName(hdl, addr, name, size)
     return ntdll._resolve_device_prefix(name.value)
 
 ################################################################################
 
 _GetModuleFileNameEx = fun_fact(
     _psa.GetModuleFileNameExW, (DWORD, HANDLE, PVOID, PWSTR, DWORD)
     )
 
 def GetModuleFileNameEx(hdl, mod):
     size = 128
     length = size
     while length == size:
         size *= 2
-        name = ctypes.create_unicode_buffer(size)
+        name = string_buffer(size)
         length = _GetModuleFileNameEx(hdl, mod, name, size)
         raise_on_zero(length)
     return name.value
 
 ################################################################################
 
 class MODULEINFO(ctypes.Structure):
```

### Comparing `ctwin32-2.5.0/ctwin32/secur.py` & `ctwin32-2.6.0/ctwin32/secur.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.5.0/ctwin32/setupapi.py` & `ctwin32-2.6.0/ctwin32/setupapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 # DEALINGS IN THE SOFTWARE.
 #
 ################################################################################
 
 import re
 import ctypes
 from .wtypes import (
+    byte_buffer,
+    string_buffer,
     BOOL,
     DWORD,
     GUID,
     HANDLE,
     HWND,
     PBYTE,
     PDWORD,
@@ -209,15 +211,15 @@
     (BOOL, PGUID, PWSTR, DWORD, PDWORD)
     )
 
 def SetupDiClassNameFromGuid(guid):
     guid = GUID(guid)  # need ctypes instance
     req_size = DWORD(0)
     _SetupDiClassNameFromGuid(ref(guid), None, 0, ref(req_size))
-    name = ctypes.create_unicode_buffer(req_size.value)
+    name = string_buffer(req_size.value)
     raise_on_zero(
         _SetupDiClassNameFromGuid(
             ref(guid),
             name,
             req_size.value,
             ref(req_size)
             )
@@ -252,15 +254,15 @@
     _sua.SetupDiGetDeviceInstanceIdW,
     (BOOL, HANDLE, PSP_DEVINFO_DATA, PWSTR, DWORD, PDWORD)
     )
 
 def SetupDiGetDeviceInstanceId(info_set, deinda):
     req_size = DWORD()
     _SetupDiGetDeviceInstanceId(info_set, deinda, None, 0, ref(req_size))
-    idstr = ctypes.create_unicode_buffer(req_size.value)
+    idstr = string_buffer(req_size.value)
     raise_on_zero(
         _SetupDiGetDeviceInstanceId(
             info_set,
             deinda,
             idstr,
             req_size.value,
             ref(req_size)
@@ -481,15 +483,15 @@
         deinda,
         prop,
         ref(reg_type),
         None,
         0,
         ref(req_size)
         )
-    buf = ctypes.create_string_buffer(req_size.value)
+    buf = byte_buffer(req_size.value)
     raise_on_zero(
         _SetupDiGetDeviceRegistryProperty(
             info_set,
             deinda,
             prop,
             ref(reg_type),
             ctypes.cast(buf, PBYTE),
```

### Comparing `ctwin32-2.5.0/ctwin32/shell.py` & `ctwin32-2.6.0/ctwin32/shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 #
 ################################################################################
 
 import ctypes
 from .wtypes import (
+    string_buffer,
     BOOL,
     DWORD,
     HANDLE,
     HINSTANCE,
     HRESULT,
     HWND,
     INT,
@@ -220,12 +221,12 @@
 ################################################################################
 
 _SHGetFolderPath = fun_fact(
     _sh.SHGetFolderPathW, (HRESULT, HWND, INT, HANDLE, DWORD, PWSTR)
     )
 
 def SHGetFolderPath(csidl, flags=0, token=None):
-    buf = ctypes.create_unicode_buffer(MAX_PATH)
+    buf = string_buffer(MAX_PATH)
     raise_on_hr(_SHGetFolderPath(None, csidl, token, flags, buf))
     return buf.value
 
 ################################################################################
```

### Comparing `ctwin32-2.5.0/ctwin32/svc_util.py` & `ctwin32-2.6.0/ctwin32/svc_util.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.5.0/ctwin32/user.py` & `ctwin32-2.6.0/ctwin32/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 #
 ################################################################################
 
 from types import SimpleNamespace as _namespace
 
 import ctypes
 from .wtypes import (
+    string_buffer,
     BOOL,
     BYTE,
     CallbackContext,
     CallbackContextPtr,
     DWORD,
     HANDLE,
     HINSTANCE,
@@ -116,15 +117,15 @@
 
 ################################################################################
 
 _GetWindowText = fun_fact(_usr.GetWindowTextW, (INT, HWND, PWSTR, INT))
 
 def GetWindowText(hwnd):
     slen = GetWindowTextLength(hwnd)
-    buf = ctypes.create_unicode_buffer(slen + 1)
+    buf = string_buffer(slen + 1)
     res = _GetWindowText(hwnd, buf, slen + 1)
     raise_if(res != slen)
     return buf.value
 
 ################################################################################
 
 _SetWindowText = fun_fact(_usr.SetWindowTextW, (BOOL, HWND, PWSTR))
@@ -138,15 +139,15 @@
     _usr.GetClassNameW, (INT, HWND, PWSTR, INT)
     )
 
 def GetClassName(hwnd):
     size = 32
     while True:
         size *= 2
-        buf = ctypes.create_unicode_buffer(size)
+        buf = string_buffer(size)
         res = _GetClassName(hwnd, buf, buf._length_)
         raise_on_zero(res)
         if res != size - 1:
             return buf.value
 
 ################################################################################
 
@@ -908,15 +909,15 @@
     )
 
 def GetDlgItemText(dlg, id):
     length = 128
     res = length
     while res >= length:
         length *= 2
-        buf = ctypes.create_unicode_buffer(length)
+        buf = string_buffer(length)
         kernel.SetLastError(0)
         res = _GetDlgItemText(dlg, id, buf, length)
         raise_on_err(kernel.GetLastError())
     return buf.value
 
 ################################################################################
 
@@ -1196,52 +1197,56 @@
 
 _GetClipboardFormatName = fun_fact(
     _usr.GetClipboardFormatNameW, (DWORD, DWORD, PWSTR, DWORD)
     )
 
 def GetClipboardFormatName(fmt_atom):
     bufsize = 1024
-    buf = ctypes.create_unicode_buffer(bufsize)
+    buf = string_buffer(bufsize)
     if _GetClipboardFormatName(fmt_atom, buf, bufsize) == 0:
         raise ctypes.WinError()
     return buf.value
 
 ################################################################################
 
 EnumClipboardFormats = fun_fact(_usr.EnumClipboardFormats, (DWORD, DWORD))
 
 ################################################################################
 
 def txt_to_clip(txt, hwnd=None):
-    buf = ctypes.create_unicode_buffer(txt)
+    buf = string_buffer(txt)
     size = ctypes.sizeof(buf)
     copied = False
     hcopy = kernel.GlobalAlloc(GMEM_MOVEABLE, size)
     try:
         ctypes.memmove(kernel.GlobalLock(hcopy), buf, size)
         kernel.GlobalUnlock(hcopy)
         OpenClipboard(hwnd)
-        EmptyClipboard()
-        SetClipboardData(CF_UNICODETEXT, hcopy)
-        copied = True
-        CloseClipboard()
+        try:
+            EmptyClipboard()
+            SetClipboardData(CF_UNICODETEXT, hcopy)
+            copied = True
+        finally:
+            CloseClipboard()
     finally:
         if not copied:
             kernel.GlobalFree(hcopy)
 
 ################################################################################
 
 def txt_from_clip(hwnd=None):
     if not IsClipboardFormatAvailable(CF_UNICODETEXT):
         raise OSError("no clipboard text available")
     OpenClipboard(hwnd)
-    hmem = GetClipboardData(CF_UNICODETEXT)
-    txt = ctypes.wstring_at(kernel.GlobalLock(hmem))
-    kernel.GlobalUnlock(hmem)
-    CloseClipboard()
+    try:
+        hmem = GetClipboardData(CF_UNICODETEXT)
+        txt = ctypes.wstring_at(kernel.GlobalLock(hmem))
+        kernel.GlobalUnlock(hmem)
+    finally:
+        CloseClipboard()
     return txt
 
 ################################################################################
 
 GetSystemMetrics = fun_fact(_usr.GetSystemMetrics, (INT, INT))
 
 ################################################################################
@@ -1259,15 +1264,15 @@
 
 _GetKeyNameText = fun_fact(_usr.GetKeyNameTextW, (INT, LONG, PWSTR, INT))
 
 def GetKeyNameText(lparam, expect_empty=False):
     size = ret = 32
     while ret >= size - 1:
         size *= 2
-        key_name = ctypes.create_unicode_buffer(size)
+        key_name = string_buffer(size)
         ret = _GetKeyNameText(lparam, key_name, size)
         raise_if(not ret and not expect_empty)
     return key_name.value
 
 ################################################################################
 
 _CreateIconFromResourceEx = fun_fact(
```

### Comparing `ctwin32-2.5.0/ctwin32/version.py` & `ctwin32-2.6.0/ctwin32/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 #
 ################################################################################
 
 import ctypes
 from .wtypes import (
+    byte_buffer,
     BOOL,
     DWORD,
     PDWORD,
     PPVOID,
     PUINT,
     PVOID,
     PWSTR,
@@ -81,15 +82,15 @@
 _GetFileVersionInfo = fun_fact(
     _ver.GetFileVersionInfoW, (BOOL, PWSTR, DWORD, DWORD, PVOID)
     )
 
 def GetFileVersionInfo(fname, size=0):
     if size == 0:
         size = GetFileVersionInfoSize(fname)
-    buf = ctypes.create_string_buffer(size)
+    buf = byte_buffer(size)
     raise_on_zero(_GetFileVersionInfo(fname, 0, size, buf))
     return buf.raw
 
 ################################################################################
 
 _VerQueryValue = fun_fact(
     _ver.VerQueryValueW, (BOOL, PVOID, PWSTR, PPVOID, PUINT)
```

### Comparing `ctwin32-2.5.0/ctwin32/virtdisk.py` & `ctwin32-2.6.0/ctwin32/virtdisk.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.5.0/ctwin32/wndcls.py` & `ctwin32-2.6.0/ctwin32/wndcls.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 import sys
 import traceback
 import lzma
 import base64
 
 import ctypes
 from .wtypes import (
+    string_buffer,
     HANDLE,
     HIWORD,
     HWND,
     LOWORD,
     LPARAM,
     POINT,
     PPOINT,
@@ -732,24 +733,24 @@
         title,
         cdata=None
         ):
     style |= WS_VISIBLE | WS_CHILD
     # bytes = template + class + title + creation data
     cls = (
         _std_classes.get(cls.lower(), None) or
-        bytes(ctypes.create_unicode_buffer(cls))
+        bytes(string_buffer(cls))
         )
     cdata = (
         bytes(WORD(0)) if cdata is None
         else bytes(WORD(len(cdata))) + cdata
         )
     bts = (
         bytes(user.DLGITEMTEMPLATE(style, 0, x, y, cx, cy, id)) +
         cls +
-        bytes(ctypes.create_unicode_buffer(title)) +
+        bytes(string_buffer(title)) +
         cdata
         )
     # align to DWORD for the following items
     bts += (-len(bts) % 4) * b"\0"
     assert len(bts) % 4 == 0
     return bts
 
@@ -769,17 +770,17 @@
     # bytes = template + menu + class + title + pointsize + typeface + items
     style |= DS_SETFONT  # always set font
     tmpl = user.DLGTEMPLATE(style, 0, len(items), x, y, cx, cy)
     bts = b"".join((
         bytes(tmpl),
         bytes(WORD(0)),     # no menu
         bytes(WORD(0)),     # default class
-        bytes(ctypes.create_unicode_buffer(title)),
+        bytes(string_buffer(title)),
         bytes(WORD(pointsize)),
-        bytes(ctypes.create_unicode_buffer(typeface))
+        bytes(string_buffer(typeface))
         ))
     return b"".join((
         bts,
         (-len(bts) % 4) * b"\0",  # align to DWORD for the following items
         *(dlg_item_template(*item) for item in items)
         ))
```

### Comparing `ctwin32-2.5.0/ctwin32/wtypes.py` & `ctwin32-2.6.0/ctwin32/wtypes.py`

 * *Files 7% similar despite different names*

```diff
@@ -72,14 +72,38 @@
 
 # handle types
 
 HANDLE = HINSTANCE = HMODULE = HWND = ctypes.c_void_p
 
 ################################################################################
 
+# byte and string buffers
+
+def byte_buffer(init, size=None):
+    if isinstance(init, bytes):
+        if size is None:
+            size = 1 + len(init)
+        (buf := (CHAR * size)()).value = init
+        return buf
+    elif isinstance(init, int):
+        return (CHAR * init)()
+    raise TypeError(init)
+
+def string_buffer(init, size=None):
+    if isinstance(init, str):
+        if size is None:
+            size = 1 + sum(2 if ord(c) > 0xFFFF else 1 for c in init)
+        (buf := (WCHAR * size)()).value = init
+        return buf
+    elif isinstance(init, int):
+        return (WCHAR * init)()
+    raise TypeError(init)
+
+################################################################################
+
 # some structure definitions
 
 class GUID(ULONG * 4):         # using ULONG for correct alignment
     def __init__(self, init=None):
         # init is None or str or GUID or UUID or something that can be
         # converted to bytes (like comtypes.GUID). If init is None we simply
         # keep the initial state of 'all bytes are zero'.
@@ -123,16 +147,28 @@
     def __init__(self, i64=0):
         self.dwLowDateTime = i64 & 0xffffffff
         self.dwHighDateTime = i64 >> 32
 
     def __int__(self):
         return self.dwLowDateTime | (self.dwHighDateTime << 32)
 
+    def __add__(self, other):
+        return self.__class__(int(self) + int(other))
+
+    def __sub__(self, other):
+        return self.__class__(int(self) - int(other))
+
     def __iadd__(self, other):
-        i64 = int(self) + other
+        i64 = int(self) + int(other)
+        self.dwLowDateTime = i64 & 0xffffffff
+        self.dwHighDateTime = i64 >> 32
+        return self
+
+    def __isub__(self, other):
+        i64 = int(self) - int(other)
         self.dwLowDateTime = i64 & 0xffffffff
         self.dwHighDateTime = i64 >> 32
         return self
 
     def __repr__(self):
         return f"{self.__class__.__name__}({int(self)})"
```

### Comparing `ctwin32-2.5.0/ctwin32.egg-info/PKG-INFO` & `ctwin32-2.6.0/ctwin32.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctwin32
-Version: 2.5.0
+Version: 2.6.0
 Summary: Access selected win32 APIs through ctypes
 Author: Rocco Matano
 License: MIT License
 Project-URL: homepage, https://github.com/RoccoMatano/ctwin32
 Project-URL: changelog, https://github.com/RoccoMatano/ctwin32/blob/master/changelog.md
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -12,20 +12,22 @@
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ![logo](https://raw.githubusercontent.com/RoccoMatano/ctwin32/master/doc/images/ctwin32.ico) ctwin32
 
+[![winonly](https://img.shields.io/badge/Windows-0078D6?style=plastic&logo=windows)](.)
 [![PyPI - Version](https://img.shields.io/pypi/v/ctwin32.svg)](https://pypi.org/project/ctwin32)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ctwin32.svg)](https://pypi.org/project/ctwin32)
 [![License - MIT](https://img.shields.io/badge/license-MIT-green)](https://spdx.org/licenses/MIT.html)
 [![PyPI - Stats](https://img.shields.io/pypi/dm/ctwin32)](https://pypistats.org/packages/ctwin32)
 
 -----
```

### Comparing `ctwin32-2.5.0/ctwin32.egg-info/SOURCES.txt` & `ctwin32-2.6.0/ctwin32.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -31,14 +31,16 @@
 ctwin32.egg-info/top_level.txt
 doc/images/ctwin32.ico
 samples/__init__.py
 samples/api_set.py
 samples/arp_table.py
 samples/atta_vdisk.py
 samples/calendar.pyw
+samples/cnt_irq.py
+samples/dump_proc_env.py
 samples/dump_ver_res.py
 samples/endis_bsl_usb.py
 samples/exbinmsi.py
 samples/extract_ico.py
 samples/find_zombies.py
 samples/fopa.py
 samples/hello_wnd.pyw
@@ -55,11 +57,12 @@
 samples/restart_usb_port.py
 samples/rm_sign_tool.py
 samples/senv.py
 samples/simple_aes.py
 samples/stopnow.py
 samples/sua_enums.py
 samples/test_sign_tool.py
+samples/timeit.py
 samples/uptime_evt.py
 samples/virt_term_seq.py
 samples/volume_paths.py
 samples/wait_for_job.py
```

### Comparing `ctwin32-2.5.0/doc/images/ctwin32.ico` & `ctwin32-2.6.0/doc/images/ctwin32.ico`

 * *Files identical despite different names*

### Comparing `ctwin32-2.5.0/pyproject.toml` & `ctwin32-2.6.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     "Environment :: Win32 (MS Windows)",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: 3.13",
     ]
 dynamic = ["version", "readme"]
 
 [project.urls]
 homepage = "https://github.com/RoccoMatano/ctwin32"
 changelog = "https://github.com/RoccoMatano/ctwin32/blob/master/changelog.md"
 
@@ -62,21 +63,24 @@
     "SIM",      # flake8-simplify
     "UP",       # pyupgrade
     "W",        # pycodestyle warnings
     "YTT",      # flake8-2020
     ]
 ignore = [
     "COM812",   # Trailing comma missing
+    "COM819",   # prohibited-trailing-comma
     "ISC003",   # Explicitly concatenated string should be implicitly concatenated
+    "PLW1510",  # `subprocess.run` without explicit `check` argument
     "PTH123",   # open() should be replaced by Path.open()
     "RSE102",   # Unnecessary parentheses on raised exception
     "RET505",   # Unnecessary {branch} after return statement
     "RET508",   # Unnecessary {branch} after break statement
     "SIM102",   # Use a single if statement instead of nested if statements
     "SIM117",   # Use a single instead of nested `with` statements
+    "UP015",    # redundant-open-modes
     "UP039",    # unnecessary-class-parentheses
     "RUF013",   # implicit-optional -> no f..g typing!!!
     ]
 
 ################################################################################
 
 [tool.flake8]
```

### Comparing `ctwin32-2.5.0/samples/api_set.py` & `ctwin32-2.6.0/samples/api_set.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.5.0/samples/arp_table.py` & `ctwin32-2.6.0/samples/arp_table.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.5.0/samples/atta_vdisk.py` & `ctwin32-2.6.0/samples/atta_vdisk.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.5.0/samples/calendar.pyw` & `ctwin32-2.6.0/samples/calendar.pyw`

 * *Files identical despite different names*

### Comparing `ctwin32-2.5.0/samples/dump_ver_res.py` & `ctwin32-2.6.0/samples/dump_ver_res.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.5.0/samples/endis_bsl_usb.py` & `ctwin32-2.6.0/samples/endis_bsl_usb.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.5.0/samples/exbinmsi.py` & `ctwin32-2.6.0/samples/exbinmsi.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.5.0/samples/extract_ico.py` & `ctwin32-2.6.0/samples/extract_ico.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.5.0/samples/find_zombies.py` & `ctwin32-2.6.0/samples/find_zombies.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.5.0/samples/fopa.py` & `ctwin32-2.6.0/samples/fopa.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.5.0/samples/hello_wnd.pyw` & `ctwin32-2.6.0/samples/hello_wnd.pyw`

 * *Files identical despite different names*

### Comparing `ctwin32-2.5.0/samples/keyview.pyw` & `ctwin32-2.6.0/samples/keyview.pyw`

 * *Files identical despite different names*

### Comparing `ctwin32-2.5.0/samples/listpipes.py` & `ctwin32-2.6.0/samples/listpipes.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.5.0/samples/logonsessions.py` & `ctwin32-2.6.0/samples/logonsessions.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.5.0/samples/lsc.py` & `ctwin32-2.6.0/samples/lsc.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.5.0/samples/netifaces.py` & `ctwin32-2.6.0/samples/netifaces.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.5.0/samples/np_dev.py` & `ctwin32-2.6.0/samples/np_dev.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.5.0/samples/power_requests.py` & `ctwin32-2.6.0/samples/power_requests.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.5.0/samples/print_reparse_points.py` & `ctwin32-2.6.0/samples/print_reparse_points.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.5.0/samples/py_ver.py` & `ctwin32-2.6.0/samples/py_ver.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.5.0/samples/remove_drive_by_letter.py` & `ctwin32-2.6.0/samples/remove_drive_by_letter.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.5.0/samples/restart_usb_port.py` & `ctwin32-2.6.0/samples/restart_usb_port.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,17 +30,15 @@
 import sys
 import ctypes
 from ctwin32 import (
     advapi,
     cfgmgr,
     kernel,
     ntdll,
-    setupapi,
     CTL_CODE,
-    ERROR_PATH_NOT_FOUND,
     FILE_ANY_ACCESS,
     FILE_DEVICE_UNKNOWN,
     METHOD_BUFFERED,
     SPDRP_LOCATION_INFORMATION,
     )
 from ctwin32.wtypes import (
     GUID,
@@ -71,22 +69,18 @@
     except ValueError as e:
         e.args = (f"{device_id} -> not a direct child of a hub",)
         raise
 
     # Step 3: the USB hub is the parent device
     hub = cfgmgr.CM_Get_Parent(devinst)
 
-    # Step 4: scan all USB hubs for this devinst to get its device path
+    # Step 4: request the USB hub's device interface
+    didstr = cfgmgr.CM_Get_Device_ID(hub)
     guid = GUID("f18a0e88-c30c-11d0-8815-00a0c906bed8")
-    for info_set, did in setupapi.enum_dev_interfaces(guid):
-        path, deinda = setupapi.SetupDiGetDeviceInterfaceDetail(info_set, did)
-        if deinda.DevInst == hub:
-            break
-    else:
-        raise ctypes.WinError(ERROR_PATH_NOT_FOUND)
+    path = cfgmgr.CM_Get_Device_Interface_List(guid, didstr)[0]
 
     # Step 5: open the hub
     with kernel.create_file(path) as hhub:
 
         # Step 6: call IOCTL_USB_HUB_CYCLE_PORT
         FILE_DEVICE_USB = FILE_DEVICE_UNKNOWN
         USB_HUB_CYCLE_PORT = 273
```

### Comparing `ctwin32-2.5.0/samples/rm_sign_tool.py` & `ctwin32-2.6.0/samples/rm_sign_tool.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.5.0/samples/senv.py` & `ctwin32-2.6.0/samples/senv.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 import sys
 import argparse
 from ctwin32 import (
     ctypes,
     user,
     advapi,
     shell,
+    wtypes,
     HWND_BROADCAST,
     WM_SETTINGCHANGE,
     SMTO_NORMAL,
     REG_SZ,
     REG_EXPAND_SZ,
     KEY_READ,
     KEY_WRITE,
@@ -64,15 +65,15 @@
             except OSError:
                 pass
             return result
 
 ################################################################################
 
 def broadcast_env_change():
-    estr = ctypes.create_unicode_buffer("Environment")
+    estr = wtypes.string_buffer("Environment")
     user.SendMessageTimeout(
         HWND_BROADCAST,
         WM_SETTINGCHANGE,
         0,
         ctypes.addressof(estr),
         SMTO_NORMAL,
         500
```

### Comparing `ctwin32-2.5.0/samples/simple_aes.py` & `ctwin32-2.6.0/samples/simple_aes.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.5.0/samples/stopnow.py` & `ctwin32-2.6.0/samples/stopnow.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.5.0/samples/sua_enums.py` & `ctwin32-2.6.0/samples/sua_enums.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.5.0/samples/test_sign_tool.py` & `ctwin32-2.6.0/samples/test_sign_tool.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.5.0/samples/uptime_evt.py` & `ctwin32-2.6.0/samples/uptime_evt.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.5.0/samples/virt_term_seq.py` & `ctwin32-2.6.0/samples/virt_term_seq.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.5.0/samples/volume_paths.py` & `ctwin32-2.6.0/samples/volume_paths.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.5.0/samples/wait_for_job.py` & `ctwin32-2.6.0/samples/wait_for_job.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,29 +18,31 @@
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 #
 ################################################################################
 
+# This example shows how to wait for a job object. I.e. waiting until all
+# processes in this job stopped executing.
+
 import sys
 from ctwin32 import (
     kernel,
     CREATE_SUSPENDED,
     INFINITE,
     INVALID_HANDLE_VALUE,
     JobObjectAssociateCompletionPortInformation,
     JOB_OBJECT_MSG_ACTIVE_PROCESS_ZERO
     )
 
 ################################################################################
 
 def create_job(arglist):
     arglist = ["cmd", "/c", *arglist] if sys.stdout is not None else arglist
-    print(f"{arglist=}")
     job = kernel.CreateJobObject()
     with kernel.create_process(arglist, CREATE_SUSPENDED) as proc_info:
         kernel.AssignProcessToJobObject(job, proc_info.hProcess)
         io_port = kernel.create_io_completion_port(INVALID_HANDLE_VALUE, 0)
         joacp = kernel.JOBOBJECT_ASSOCIATE_COMPLETION_PORT(job, io_port)
         kernel.SetInformationJobObject(
             job,
```

### Comparing `ctwin32-2.5.0/setup.py` & `ctwin32-2.6.0/setup.py`

 * *Files identical despite different names*

