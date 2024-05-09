# Comparing `tmp/towalink_tlm-0.3.1.tar.gz` & `tmp/towalink_tlm-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "towalink_tlm-0.3.1.tar", last modified: Mon Apr 29 07:29:14 2024, max compression
+gzip compressed data, was "towalink_tlm-0.3.2.tar", last modified: Thu May  9 19:35:10 2024, max compression
```

## Comparing `towalink_tlm-0.3.1.tar` & `towalink_tlm-0.3.2.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.987734 towalink_tlm-0.3.1/
--rwxrw-r--   0 root         (0) root         (0)    34523 2020-08-22 10:31:22.000000 towalink_tlm-0.3.1/LICENSE
--rwxrw-r--   0 root         (0) root         (0)       92 2020-08-22 10:32:22.000000 towalink_tlm-0.3.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1703 2024-04-29 07:29:13.987734 towalink_tlm-0.3.1/PKG-INFO
--rwxrw-r--   0 root         (0) root         (0)      496 2023-06-03 20:36:23.000000 towalink_tlm-0.3.1/README.md
--rwxrw-r--   0 root         (0) root         (0)       97 2024-04-29 07:29:13.991734 towalink_tlm-0.3.1/setup.cfg
--rwxrw-r--   0 root         (0) root         (0)     1895 2024-04-25 18:32:46.000000 towalink_tlm-0.3.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.763737 towalink_tlm-0.3.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.827736 towalink_tlm-0.3.1/src/tlm/
--rwxrw-r--   0 root         (0) root         (0)    13045 2023-06-03 20:36:23.000000 towalink_tlm-0.3.1/src/tlm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.831736 towalink_tlm-0.3.1/src/tlm/ansible/
--rwxrw-r--   0 root         (0) root         (0)      312 2023-05-21 17:49:12.000000 towalink_tlm-0.3.1/src/tlm/ansible/node.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.755737 towalink_tlm-0.3.1/src/tlm/ansible/roles/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.739737 towalink_tlm-0.3.1/src/tlm/ansible/roles/bird/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.739737 towalink_tlm-0.3.1/src/tlm/ansible/roles/bird/files/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.847736 towalink_tlm-0.3.1/src/tlm/ansible/roles/bird/files/etc_apt_preferencesd/
--rwxrw-r--   0 root         (0) root         (0)      232 2020-09-08 12:46:36.000000 towalink_tlm-0.3.1/src/tlm/ansible/roles/bird/files/etc_apt_preferencesd/debian-testing
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.851736 towalink_tlm-0.3.1/src/tlm/ansible/roles/bird/tasks/
--rwxrw-r--   0 root         (0) root         (0)     2727 2022-07-06 20:50:24.000000 towalink_tlm-0.3.1/src/tlm/ansible/roles/bird/tasks/main.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.735737 towalink_tlm-0.3.1/src/tlm/ansible/roles/bird-lg-proxy/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.735737 towalink_tlm-0.3.1/src/tlm/ansible/roles/bird-lg-proxy/files/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.835736 towalink_tlm-0.3.1/src/tlm/ansible/roles/bird-lg-proxy/files/etc_initd/
--rwxrw-r--   0 root         (0) root         (0)      265 2023-06-11 07:52:39.000000 towalink_tlm-0.3.1/src/tlm/ansible/roles/bird-lg-proxy/files/etc_initd/towalink_bird-lg-proxy
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.839736 towalink_tlm-0.3.1/src/tlm/ansible/roles/bird-lg-proxy/files/etc_systemd_system/
--rwxrw-r--   0 root         (0) root         (0)      395 2023-06-11 07:53:03.000000 towalink_tlm-0.3.1/src/tlm/ansible/roles/bird-lg-proxy/files/etc_systemd_system/towalink_bird-lg-proxy.service
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.843736 towalink_tlm-0.3.1/src/tlm/ansible/roles/bird-lg-proxy/tasks/
--rwxrw-r--   0 root         (0) root         (0)     1262 2021-09-19 16:04:20.000000 towalink_tlm-0.3.1/src/tlm/ansible/roles/bird-lg-proxy/tasks/main.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.747737 towalink_tlm-0.3.1/src/tlm/ansible/roles/nodeconfig/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.743737 towalink_tlm-0.3.1/src/tlm/ansible/roles/nodeconfig/files/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.855736 towalink_tlm-0.3.1/src/tlm/ansible/roles/nodeconfig/files/opt_towalink_scripts/
--rwxrw-r--   0 root         (0) root         (0)      297 2020-09-07 15:14:20.000000 towalink_tlm-0.3.1/src/tlm/ansible/roles/nodeconfig/files/opt_towalink_scripts/rsync-nodecfg.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.859736 towalink_tlm-0.3.1/src/tlm/ansible/roles/nodeconfig/tasks/
--rwxrw-r--   0 root         (0) root         (0)     2336 2020-11-23 09:46:52.000000 towalink_tlm-0.3.1/src/tlm/ansible/roles/nodeconfig/tasks/main.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.755737 towalink_tlm-0.3.1/src/tlm/ansible/roles/startup/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.751737 towalink_tlm-0.3.1/src/tlm/ansible/roles/startup/files/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.867736 towalink_tlm-0.3.1/src/tlm/ansible/roles/startup/files/etc_initd/
--rwxrw-r--   0 root         (0) root         (0)      231 2023-11-19 11:13:30.000000 towalink_tlm-0.3.1/src/tlm/ansible/roles/startup/files/etc_initd/towalink_startup
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.871736 towalink_tlm-0.3.1/src/tlm/ansible/roles/startup/files/etc_systemd_system/
--rwxrw-r--   0 root         (0) root         (0)      330 2020-09-11 10:10:47.000000 towalink_tlm-0.3.1/src/tlm/ansible/roles/startup/files/etc_systemd_system/towalink_startup.service
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.875736 towalink_tlm-0.3.1/src/tlm/ansible/roles/startup/files/opt_towalink_startup/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.879736 towalink_tlm-0.3.1/src/tlm/ansible/roles/startup/files/opt_towalink_startup/scripts/
--rwxrw-r--   0 root         (0) root         (0)      317 2020-06-21 21:01:14.000000 towalink_tlm-0.3.1/src/tlm/ansible/roles/startup/files/opt_towalink_startup/scripts/wireguard
--rwxrw-r--   0 root         (0) root         (0)      250 2020-06-21 20:25:57.000000 towalink_tlm-0.3.1/src/tlm/ansible/roles/startup/files/opt_towalink_startup/towalink.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.883735 towalink_tlm-0.3.1/src/tlm/ansible/roles/startup/tasks/
--rwxrw-r--   0 root         (0) root         (0)     1115 2020-09-08 10:25:54.000000 towalink_tlm-0.3.1/src/tlm/ansible/roles/startup/tasks/main.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.759737 towalink_tlm-0.3.1/src/tlm/ansible/roles/system/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.759737 towalink_tlm-0.3.1/src/tlm/ansible/roles/system/files/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.887735 towalink_tlm-0.3.1/src/tlm/ansible/roles/system/files/unused_etc_sysctld/
--rwxrw-r--   0 root         (0) root         (0)      309 2020-09-10 17:23:27.000000 towalink_tlm-0.3.1/src/tlm/ansible/roles/system/files/unused_etc_sysctld/towalink.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.891735 towalink_tlm-0.3.1/src/tlm/ansible/roles/system/tasks/
--rwxrw-r--   0 root         (0) root         (0)      589 2020-09-11 14:09:00.000000 towalink_tlm-0.3.1/src/tlm/ansible/roles/system/tasks/main.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.895735 towalink_tlm-0.3.1/src/tlm/ansible/vars/
--rwxrw-r--   0 root         (0) root         (0)      137 2020-10-03 21:23:15.000000 towalink_tlm-0.3.1/src/tlm/ansible/vars/external_vars.yml
--rwxrw-r--   0 root         (0) root         (0)     4639 2021-06-16 18:55:44.000000 towalink_tlm-0.3.1/src/tlm/ansiblecaller.py
--rwxrw-r--   0 root         (0) root         (0)     1430 2020-06-02 19:29:15.000000 towalink_tlm-0.3.1/src/tlm/configfilecopier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.927735 towalink_tlm-0.3.1/src/tlm/configmanager/
--rwxrw-r--   0 root         (0) root         (0)        0 2020-06-15 18:25:35.000000 towalink_tlm-0.3.1/src/tlm/configmanager/__init__.py
--rwxrw-r--   0 root         (0) root         (0)     8372 2024-04-25 19:51:28.000000 towalink_tlm-0.3.1/src/tlm/configmanager/configmanager.py
--rwxrw-r--   0 root         (0) root         (0)     3943 2024-04-23 20:25:29.000000 towalink_tlm-0.3.1/src/tlm/configmanager/generatedconfig.py
--rwxrw-r--   0 root         (0) root         (0)     1688 2020-07-25 19:44:05.000000 towalink_tlm-0.3.1/src/tlm/configmanager/nodeconfig.py
--rwxrw-r--   0 root         (0) root         (0)     1503 2020-07-25 19:45:52.000000 towalink_tlm-0.3.1/src/tlm/configmanager/siteconfig.py
--rwxrw-r--   0 root         (0) root         (0)     6433 2020-09-17 19:42:31.000000 towalink_tlm-0.3.1/src/tlm/configmanager/tomlconfig.py
--rwxrw-r--   0 root         (0) root         (0)     4205 2021-05-27 20:26:40.000000 towalink_tlm-0.3.1/src/tlm/configmanager/tomlconfighierarchy.py
--rwxrw-r--   0 root         (0) root         (0)     2408 2024-04-23 19:52:45.000000 towalink_tlm-0.3.1/src/tlm/configmanager/wireguard.py
--rwxrw-r--   0 root         (0) root         (0)     5778 2020-07-12 20:32:32.000000 towalink_tlm-0.3.1/src/tlm/configmanager/yamlconfig.py
--rwxrw-r--   0 root         (0) root         (0)    18758 2024-04-26 20:04:14.000000 towalink_tlm-0.3.1/src/tlm/configorchestrator.py
--rwxrw-r--   0 root         (0) root         (0)     1330 2020-06-24 20:38:54.000000 towalink_tlm-0.3.1/src/tlm/directorycomparer.py
--rwxrw-r--   0 root         (0) root         (0)      891 2020-06-25 20:50:01.000000 towalink_tlm-0.3.1/src/tlm/exceptionlogger.py
--rwxrw-r--   0 root         (0) root         (0)     5170 2020-09-06 18:30:57.000000 towalink_tlm-0.3.1/src/tlm/exechelper.py
--rwxrw-r--   0 root         (0) root         (0)     2556 2024-04-26 20:02:14.000000 towalink_tlm-0.3.1/src/tlm/filesync.py
--rwxrw-r--   0 root         (0) root         (0)     3533 2023-06-09 16:27:34.000000 towalink_tlm-0.3.1/src/tlm/gitcaller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.935735 towalink_tlm-0.3.1/src/tlm/healthcheck/
--rwxrw-r--   0 root         (0) root         (0)        0 2023-06-03 20:36:25.000000 towalink_tlm-0.3.1/src/tlm/healthcheck/__init__.py
--rwxrw-r--   0 root         (0) root         (0)     1489 2023-06-03 20:36:25.000000 towalink_tlm-0.3.1/src/tlm/healthcheck/cmdexec.py
--rwxrw-r--   0 root         (0) root         (0)      831 2023-06-03 20:36:25.000000 towalink_tlm-0.3.1/src/tlm/healthcheck/ping.py
--rwxrw-r--   0 root         (0) root         (0)     3347 2020-07-12 20:29:48.000000 towalink_tlm-0.3.1/src/tlm/jinjatransformer.py
--rwxrw-r--   0 root         (0) root         (0)     3082 2023-06-09 15:57:54.000000 towalink_tlm-0.3.1/src/tlm/management_interface.py
--rwxrw-r--   0 root         (0) root         (0)    18840 2023-06-09 15:59:51.000000 towalink_tlm-0.3.1/src/tlm/nodeattacher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.963734 towalink_tlm-0.3.1/src/tlm/skeleton/
--rwxrw-r--   0 root         (0) root         (0)      160 2020-09-12 09:56:45.000000 towalink_tlm-0.3.1/src/tlm/skeleton/LICENSE
--rwxrw-r--   0 root         (0) root         (0)     2811 2023-06-03 20:36:24.000000 towalink_tlm-0.3.1/src/tlm/skeleton/bird.conf.jinja
--rwxrw-r--   0 root         (0) root         (0)      322 2023-06-03 20:36:24.000000 towalink_tlm-0.3.1/src/tlm/skeleton/bird_neighbors.conf.jinja
--rwxrw-r--   0 root         (0) root         (0)       46 2020-09-11 15:09:58.000000 towalink_tlm-0.3.1/src/tlm/skeleton/bird_site-template.conf.jinja
--rwxrw-r--   0 root         (0) root         (0)     1644 2020-09-27 20:09:05.000000 towalink_tlm-0.3.1/src/tlm/skeleton/config.toml
--rwxrw-r--   0 root         (0) root         (0)      330 2020-09-11 18:12:23.000000 towalink_tlm-0.3.1/src/tlm/skeleton/startup_loopback.jinja
--rwxrw-r--   0 root         (0) root         (0)      603 2024-04-23 20:31:58.000000 towalink_tlm-0.3.1/src/tlm/skeleton/tlwg.conf.jinja
--rwxrw-r--   0 root         (0) root         (0)    14437 2023-06-03 20:49:12.000000 towalink_tlm-0.3.1/src/tlm/towalinkmanager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.983734 towalink_tlm-0.3.1/src/towalink_tlm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1703 2024-04-29 07:29:13.000000 towalink_tlm-0.3.1/src/towalink_tlm.egg-info/PKG-INFO
--rwxrw-r--   0 root         (0) root         (0)     2264 2024-04-29 07:29:13.000000 towalink_tlm-0.3.1/src/towalink_tlm.egg-info/SOURCES.txt
--rwxrw-r--   0 root         (0) root         (0)        1 2024-04-29 07:29:13.000000 towalink_tlm-0.3.1/src/towalink_tlm.egg-info/dependency_links.txt
--rwxrw-r--   0 root         (0) root         (0)       33 2024-04-29 07:29:13.000000 towalink_tlm-0.3.1/src/towalink_tlm.egg-info/entry_points.txt
--rwxrw-r--   0 root         (0) root         (0)       72 2024-04-29 07:29:13.000000 towalink_tlm-0.3.1/src/towalink_tlm.egg-info/requires.txt
--rwxrw-r--   0 root         (0) root         (0)        4 2024-04-29 07:29:13.000000 towalink_tlm-0.3.1/src/towalink_tlm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 19:35:10.840650 towalink_tlm-0.3.2/
+-rwxrw-r--   0 root         (0) root         (0)    34523 2020-08-22 10:31:22.000000 towalink_tlm-0.3.2/LICENSE
+-rwxrw-r--   0 root         (0) root         (0)       92 2020-08-22 10:32:22.000000 towalink_tlm-0.3.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1703 2024-05-09 19:35:10.840650 towalink_tlm-0.3.2/PKG-INFO
+-rwxrw-r--   0 root         (0) root         (0)      496 2023-06-03 20:36:23.000000 towalink_tlm-0.3.2/README.md
+-rwxrw-r--   0 root         (0) root         (0)       97 2024-05-09 19:35:10.844650 towalink_tlm-0.3.2/setup.cfg
+-rwxrw-r--   0 root         (0) root         (0)     1895 2024-05-09 19:33:42.000000 towalink_tlm-0.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 19:35:09.636667 towalink_tlm-0.3.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 19:35:10.020662 towalink_tlm-0.3.2/src/tlm/
+-rwxrw-r--   0 root         (0) root         (0)    13045 2023-06-03 20:36:23.000000 towalink_tlm-0.3.2/src/tlm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 19:35:10.044661 towalink_tlm-0.3.2/src/tlm/ansible/
+-rwxrw-r--   0 root         (0) root         (0)      312 2023-05-21 17:49:12.000000 towalink_tlm-0.3.2/src/tlm/ansible/node.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 19:35:09.628667 towalink_tlm-0.3.2/src/tlm/ansible/roles/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 19:35:09.616667 towalink_tlm-0.3.2/src/tlm/ansible/roles/bird/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 19:35:09.612667 towalink_tlm-0.3.2/src/tlm/ansible/roles/bird/files/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 19:35:10.156660 towalink_tlm-0.3.2/src/tlm/ansible/roles/bird/files/etc_apt_preferencesd/
+-rwxrw-r--   0 root         (0) root         (0)      232 2020-09-08 12:46:36.000000 towalink_tlm-0.3.2/src/tlm/ansible/roles/bird/files/etc_apt_preferencesd/debian-testing
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 19:35:10.172659 towalink_tlm-0.3.2/src/tlm/ansible/roles/bird/tasks/
+-rwxrw-r--   0 root         (0) root         (0)     2727 2022-07-06 20:50:24.000000 towalink_tlm-0.3.2/src/tlm/ansible/roles/bird/tasks/main.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 19:35:09.612667 towalink_tlm-0.3.2/src/tlm/ansible/roles/bird-lg-proxy/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 19:35:09.608667 towalink_tlm-0.3.2/src/tlm/ansible/roles/bird-lg-proxy/files/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 19:35:10.052661 towalink_tlm-0.3.2/src/tlm/ansible/roles/bird-lg-proxy/files/etc_initd/
+-rwxrw-r--   0 root         (0) root         (0)      265 2023-06-11 07:52:39.000000 towalink_tlm-0.3.2/src/tlm/ansible/roles/bird-lg-proxy/files/etc_initd/towalink_bird-lg-proxy
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 19:35:10.064661 towalink_tlm-0.3.2/src/tlm/ansible/roles/bird-lg-proxy/files/etc_systemd_system/
+-rwxrw-r--   0 root         (0) root         (0)      395 2023-06-11 07:53:03.000000 towalink_tlm-0.3.2/src/tlm/ansible/roles/bird-lg-proxy/files/etc_systemd_system/towalink_bird-lg-proxy.service
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 19:35:10.092661 towalink_tlm-0.3.2/src/tlm/ansible/roles/bird-lg-proxy/tasks/
+-rwxrw-r--   0 root         (0) root         (0)     1262 2021-09-19 16:04:20.000000 towalink_tlm-0.3.2/src/tlm/ansible/roles/bird-lg-proxy/tasks/main.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 19:35:09.620667 towalink_tlm-0.3.2/src/tlm/ansible/roles/nodeconfig/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 19:35:09.620667 towalink_tlm-0.3.2/src/tlm/ansible/roles/nodeconfig/files/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 19:35:10.192659 towalink_tlm-0.3.2/src/tlm/ansible/roles/nodeconfig/files/opt_towalink_scripts/
+-rwxrw-r--   0 root         (0) root         (0)      297 2020-09-07 15:14:20.000000 towalink_tlm-0.3.2/src/tlm/ansible/roles/nodeconfig/files/opt_towalink_scripts/rsync-nodecfg.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 19:35:10.212659 towalink_tlm-0.3.2/src/tlm/ansible/roles/nodeconfig/tasks/
+-rwxrw-r--   0 root         (0) root         (0)     2336 2020-11-23 09:46:52.000000 towalink_tlm-0.3.2/src/tlm/ansible/roles/nodeconfig/tasks/main.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 19:35:09.628667 towalink_tlm-0.3.2/src/tlm/ansible/roles/startup/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 19:35:09.624667 towalink_tlm-0.3.2/src/tlm/ansible/roles/startup/files/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 19:35:10.236659 towalink_tlm-0.3.2/src/tlm/ansible/roles/startup/files/etc_initd/
+-rwxrw-r--   0 root         (0) root         (0)      231 2023-11-19 11:13:30.000000 towalink_tlm-0.3.2/src/tlm/ansible/roles/startup/files/etc_initd/towalink_startup
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 19:35:10.256658 towalink_tlm-0.3.2/src/tlm/ansible/roles/startup/files/etc_systemd_system/
+-rwxrw-r--   0 root         (0) root         (0)      330 2020-09-11 10:10:47.000000 towalink_tlm-0.3.2/src/tlm/ansible/roles/startup/files/etc_systemd_system/towalink_startup.service
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 19:35:10.288658 towalink_tlm-0.3.2/src/tlm/ansible/roles/startup/files/opt_towalink_startup/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 19:35:10.316658 towalink_tlm-0.3.2/src/tlm/ansible/roles/startup/files/opt_towalink_startup/scripts/
+-rwxrw-r--   0 root         (0) root         (0)      317 2020-06-21 21:01:14.000000 towalink_tlm-0.3.2/src/tlm/ansible/roles/startup/files/opt_towalink_startup/scripts/wireguard
+-rwxrw-r--   0 root         (0) root         (0)      250 2020-06-21 20:25:57.000000 towalink_tlm-0.3.2/src/tlm/ansible/roles/startup/files/opt_towalink_startup/towalink.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 19:35:10.340657 towalink_tlm-0.3.2/src/tlm/ansible/roles/startup/tasks/
+-rwxrw-r--   0 root         (0) root         (0)     1115 2020-09-08 10:25:54.000000 towalink_tlm-0.3.2/src/tlm/ansible/roles/startup/tasks/main.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 19:35:09.632667 towalink_tlm-0.3.2/src/tlm/ansible/roles/system/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 19:35:09.632667 towalink_tlm-0.3.2/src/tlm/ansible/roles/system/files/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 19:35:10.364657 towalink_tlm-0.3.2/src/tlm/ansible/roles/system/files/unused_etc_sysctld/
+-rwxrw-r--   0 root         (0) root         (0)      309 2020-09-10 17:23:27.000000 towalink_tlm-0.3.2/src/tlm/ansible/roles/system/files/unused_etc_sysctld/towalink.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 19:35:10.384657 towalink_tlm-0.3.2/src/tlm/ansible/roles/system/tasks/
+-rwxrw-r--   0 root         (0) root         (0)      589 2020-09-11 14:09:00.000000 towalink_tlm-0.3.2/src/tlm/ansible/roles/system/tasks/main.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 19:35:10.404656 towalink_tlm-0.3.2/src/tlm/ansible/vars/
+-rwxrw-r--   0 root         (0) root         (0)      137 2020-10-03 21:23:15.000000 towalink_tlm-0.3.2/src/tlm/ansible/vars/external_vars.yml
+-rwxrw-r--   0 root         (0) root         (0)     4639 2021-06-16 18:55:44.000000 towalink_tlm-0.3.2/src/tlm/ansiblecaller.py
+-rwxrw-r--   0 root         (0) root         (0)     1430 2020-06-02 19:29:15.000000 towalink_tlm-0.3.2/src/tlm/configfilecopier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 19:35:10.620653 towalink_tlm-0.3.2/src/tlm/configmanager/
+-rwxrw-r--   0 root         (0) root         (0)        0 2020-06-15 18:25:35.000000 towalink_tlm-0.3.2/src/tlm/configmanager/__init__.py
+-rwxrw-r--   0 root         (0) root         (0)     8372 2024-04-25 19:51:28.000000 towalink_tlm-0.3.2/src/tlm/configmanager/configmanager.py
+-rwxrw-r--   0 root         (0) root         (0)     3943 2024-04-23 20:25:29.000000 towalink_tlm-0.3.2/src/tlm/configmanager/generatedconfig.py
+-rwxrw-r--   0 root         (0) root         (0)     1688 2020-07-25 19:44:05.000000 towalink_tlm-0.3.2/src/tlm/configmanager/nodeconfig.py
+-rwxrw-r--   0 root         (0) root         (0)     1503 2020-07-25 19:45:52.000000 towalink_tlm-0.3.2/src/tlm/configmanager/siteconfig.py
+-rwxrw-r--   0 root         (0) root         (0)     6433 2020-09-17 19:42:31.000000 towalink_tlm-0.3.2/src/tlm/configmanager/tomlconfig.py
+-rwxrw-r--   0 root         (0) root         (0)     4205 2021-05-27 20:26:40.000000 towalink_tlm-0.3.2/src/tlm/configmanager/tomlconfighierarchy.py
+-rwxrw-r--   0 root         (0) root         (0)     2408 2024-04-23 19:52:45.000000 towalink_tlm-0.3.2/src/tlm/configmanager/wireguard.py
+-rwxrw-r--   0 root         (0) root         (0)     5778 2020-07-12 20:32:32.000000 towalink_tlm-0.3.2/src/tlm/configmanager/yamlconfig.py
+-rwxrw-r--   0 root         (0) root         (0)    18758 2024-04-26 20:04:14.000000 towalink_tlm-0.3.2/src/tlm/configorchestrator.py
+-rwxrw-r--   0 root         (0) root         (0)     1330 2020-06-24 20:38:54.000000 towalink_tlm-0.3.2/src/tlm/directorycomparer.py
+-rwxrw-r--   0 root         (0) root         (0)      891 2020-06-25 20:50:01.000000 towalink_tlm-0.3.2/src/tlm/exceptionlogger.py
+-rwxrw-r--   0 root         (0) root         (0)     5170 2020-09-06 18:30:57.000000 towalink_tlm-0.3.2/src/tlm/exechelper.py
+-rwxrw-r--   0 root         (0) root         (0)     2556 2024-04-26 20:02:14.000000 towalink_tlm-0.3.2/src/tlm/filesync.py
+-rwxrw-r--   0 root         (0) root         (0)     3533 2023-06-09 16:27:34.000000 towalink_tlm-0.3.2/src/tlm/gitcaller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 19:35:10.664653 towalink_tlm-0.3.2/src/tlm/healthcheck/
+-rwxrw-r--   0 root         (0) root         (0)        0 2023-06-03 20:36:25.000000 towalink_tlm-0.3.2/src/tlm/healthcheck/__init__.py
+-rwxrw-r--   0 root         (0) root         (0)     1489 2023-06-03 20:36:25.000000 towalink_tlm-0.3.2/src/tlm/healthcheck/cmdexec.py
+-rwxrw-r--   0 root         (0) root         (0)      831 2023-06-03 20:36:25.000000 towalink_tlm-0.3.2/src/tlm/healthcheck/ping.py
+-rwxrw-r--   0 root         (0) root         (0)     3347 2020-07-12 20:29:48.000000 towalink_tlm-0.3.2/src/tlm/jinjatransformer.py
+-rwxrw-r--   0 root         (0) root         (0)     3082 2023-06-09 15:57:54.000000 towalink_tlm-0.3.2/src/tlm/management_interface.py
+-rwxrw-r--   0 root         (0) root         (0)    18840 2023-06-09 15:59:51.000000 towalink_tlm-0.3.2/src/tlm/nodeattacher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 19:35:10.812651 towalink_tlm-0.3.2/src/tlm/skeleton/
+-rwxrw-r--   0 root         (0) root         (0)      160 2020-09-12 09:56:45.000000 towalink_tlm-0.3.2/src/tlm/skeleton/LICENSE
+-rwxrw-r--   0 root         (0) root         (0)     2811 2023-06-03 20:36:24.000000 towalink_tlm-0.3.2/src/tlm/skeleton/bird.conf.jinja
+-rwxrw-r--   0 root         (0) root         (0)      322 2023-06-03 20:36:24.000000 towalink_tlm-0.3.2/src/tlm/skeleton/bird_neighbors.conf.jinja
+-rwxrw-r--   0 root         (0) root         (0)       46 2020-09-11 15:09:58.000000 towalink_tlm-0.3.2/src/tlm/skeleton/bird_site-template.conf.jinja
+-rwxrw-r--   0 root         (0) root         (0)     1644 2020-09-27 20:09:05.000000 towalink_tlm-0.3.2/src/tlm/skeleton/config.toml
+-rwxrw-r--   0 root         (0) root         (0)      330 2020-09-11 18:12:23.000000 towalink_tlm-0.3.2/src/tlm/skeleton/startup_loopback.jinja
+-rwxrw-r--   0 root         (0) root         (0)      622 2024-05-09 19:31:30.000000 towalink_tlm-0.3.2/src/tlm/skeleton/tlwg.conf.jinja
+-rwxrw-r--   0 root         (0) root         (0)    14437 2023-06-03 20:49:12.000000 towalink_tlm-0.3.2/src/tlm/towalinkmanager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 19:35:10.836650 towalink_tlm-0.3.2/src/towalink_tlm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1703 2024-05-09 19:35:09.000000 towalink_tlm-0.3.2/src/towalink_tlm.egg-info/PKG-INFO
+-rwxrw-r--   0 root         (0) root         (0)     2264 2024-05-09 19:35:09.000000 towalink_tlm-0.3.2/src/towalink_tlm.egg-info/SOURCES.txt
+-rwxrw-r--   0 root         (0) root         (0)        1 2024-05-09 19:35:09.000000 towalink_tlm-0.3.2/src/towalink_tlm.egg-info/dependency_links.txt
+-rwxrw-r--   0 root         (0) root         (0)       33 2024-05-09 19:35:09.000000 towalink_tlm-0.3.2/src/towalink_tlm.egg-info/entry_points.txt
+-rwxrw-r--   0 root         (0) root         (0)       72 2024-05-09 19:35:09.000000 towalink_tlm-0.3.2/src/towalink_tlm.egg-info/requires.txt
+-rwxrw-r--   0 root         (0) root         (0)        4 2024-05-09 19:35:09.000000 towalink_tlm-0.3.2/src/towalink_tlm.egg-info/top_level.txt
```

### Comparing `towalink_tlm-0.3.1/LICENSE` & `towalink_tlm-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.3.1/PKG-INFO` & `towalink_tlm-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: towalink_tlm
-Version: 0.3.1
+Version: 0.3.2
 Summary: command line tool for configuring and managing a Towalink installation
 Home-page: https://www.towalink.net
 Author: The Towalink Project
 Author-email: pypi.tlm@towalink.net
 Project-URL: Project homepage, https://www.towalink.net
 Project-URL: Repository, https://www.github.com/towalink/tlm
 Project-URL: Documentation, https://towalink.readthedocs.io
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: towalink_tlm Version: 0.3.1 Summary: command line
+Metadata-Version: 2.1 Name: towalink_tlm Version: 0.3.2 Summary: command line
 tool for configuring and managing a Towalink installation Home-page: https://
 www.towalink.net Author: The Towalink Project Author-email:
 pypi.tlm@towalink.net Project-URL: Project homepage, https://www.towalink.net
 Project-URL: Repository, https://www.github.com/towalink/tlm Project-URL:
 Documentation, https://towalink.readthedocs.io Keywords: Towalink VPN SD-WAN
 WireGuard Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU Affero
```

### Comparing `towalink_tlm-0.3.1/setup.py` & `towalink_tlm-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup_kwargs = {
     'name': 'towalink_tlm',
-    'version': '0.3.1',
+    'version': '0.3.2',
     'author': 'The Towalink Project',
     'author_email': 'pypi.tlm@towalink.net',
     'description': 'command line tool for configuring and managing a Towalink installation',
     'long_description': long_description,
     'long_description_content_type': 'text/markdown',
     'url': 'https://www.towalink.net',
     'packages': setuptools.find_namespace_packages('src'),
```

### Comparing `towalink_tlm-0.3.1/src/tlm/__init__.py` & `towalink_tlm-0.3.2/src/tlm/__init__.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.3.1/src/tlm/ansible/roles/bird/tasks/main.yml` & `towalink_tlm-0.3.2/src/tlm/ansible/roles/bird/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.3.1/src/tlm/ansible/roles/bird-lg-proxy/tasks/main.yml` & `towalink_tlm-0.3.2/src/tlm/ansible/roles/bird-lg-proxy/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.3.1/src/tlm/ansible/roles/nodeconfig/tasks/main.yml` & `towalink_tlm-0.3.2/src/tlm/ansible/roles/nodeconfig/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.3.1/src/tlm/ansible/roles/startup/tasks/main.yml` & `towalink_tlm-0.3.2/src/tlm/ansible/roles/startup/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.3.1/src/tlm/ansible/roles/system/tasks/main.yml` & `towalink_tlm-0.3.2/src/tlm/ansible/roles/system/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.3.1/src/tlm/ansiblecaller.py` & `towalink_tlm-0.3.2/src/tlm/ansiblecaller.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.3.1/src/tlm/configfilecopier.py` & `towalink_tlm-0.3.2/src/tlm/configfilecopier.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.3.1/src/tlm/configmanager/configmanager.py` & `towalink_tlm-0.3.2/src/tlm/configmanager/configmanager.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.3.1/src/tlm/configmanager/generatedconfig.py` & `towalink_tlm-0.3.2/src/tlm/configmanager/generatedconfig.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.3.1/src/tlm/configmanager/nodeconfig.py` & `towalink_tlm-0.3.2/src/tlm/configmanager/nodeconfig.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.3.1/src/tlm/configmanager/siteconfig.py` & `towalink_tlm-0.3.2/src/tlm/configmanager/siteconfig.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.3.1/src/tlm/configmanager/tomlconfig.py` & `towalink_tlm-0.3.2/src/tlm/configmanager/tomlconfig.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.3.1/src/tlm/configmanager/tomlconfighierarchy.py` & `towalink_tlm-0.3.2/src/tlm/configmanager/tomlconfighierarchy.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.3.1/src/tlm/configmanager/wireguard.py` & `towalink_tlm-0.3.2/src/tlm/configmanager/wireguard.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.3.1/src/tlm/configmanager/yamlconfig.py` & `towalink_tlm-0.3.2/src/tlm/configmanager/yamlconfig.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.3.1/src/tlm/configorchestrator.py` & `towalink_tlm-0.3.2/src/tlm/configorchestrator.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.3.1/src/tlm/directorycomparer.py` & `towalink_tlm-0.3.2/src/tlm/directorycomparer.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.3.1/src/tlm/exceptionlogger.py` & `towalink_tlm-0.3.2/src/tlm/exceptionlogger.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.3.1/src/tlm/exechelper.py` & `towalink_tlm-0.3.2/src/tlm/exechelper.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.3.1/src/tlm/filesync.py` & `towalink_tlm-0.3.2/src/tlm/filesync.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.3.1/src/tlm/gitcaller.py` & `towalink_tlm-0.3.2/src/tlm/gitcaller.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.3.1/src/tlm/healthcheck/cmdexec.py` & `towalink_tlm-0.3.2/src/tlm/healthcheck/cmdexec.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.3.1/src/tlm/healthcheck/ping.py` & `towalink_tlm-0.3.2/src/tlm/healthcheck/ping.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.3.1/src/tlm/jinjatransformer.py` & `towalink_tlm-0.3.2/src/tlm/jinjatransformer.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.3.1/src/tlm/management_interface.py` & `towalink_tlm-0.3.2/src/tlm/management_interface.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.3.1/src/tlm/nodeattacher.py` & `towalink_tlm-0.3.2/src/tlm/nodeattacher.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.3.1/src/tlm/skeleton/bird.conf.jinja` & `towalink_tlm-0.3.2/src/tlm/skeleton/bird.conf.jinja`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.3.1/src/tlm/skeleton/config.toml` & `towalink_tlm-0.3.2/src/tlm/skeleton/config.toml`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.3.1/src/tlm/skeleton/tlwg.conf.jinja` & `towalink_tlm-0.3.2/src/tlm/skeleton/tlwg.conf.jinja`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [Interface]
 ListenPort = {{wg_listenport}}
 PrivateKey = {{wg_private}}
 Address = {{wg_addresses|join(', ')}}
 {%- if wg_peer_address_ipv4 is defined %}
 Postup = ip addr add {{wg_address_ipv4}} peer {{wg_peer_address_ipv4}} dev {{wg_ifname}}
 {%- endif %}
-{%- if wg_mtu is defined %}
+{%- if wg_mtu is defined wg_mtu is not none %}
 Mtu = {{wg_mtu}}
 {%- endif %}
 Table = off
 
 [Peer]
 Endpoint = {{wg_peer_endpoint}}
 PublicKey = {{wg_peer_public}}
```

### Comparing `towalink_tlm-0.3.1/src/tlm/towalinkmanager.py` & `towalink_tlm-0.3.2/src/tlm/towalinkmanager.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.3.1/src/towalink_tlm.egg-info/PKG-INFO` & `towalink_tlm-0.3.2/src/towalink_tlm.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: towalink-tlm
-Version: 0.3.1
+Version: 0.3.2
 Summary: command line tool for configuring and managing a Towalink installation
 Home-page: https://www.towalink.net
 Author: The Towalink Project
 Author-email: pypi.tlm@towalink.net
 Project-URL: Project homepage, https://www.towalink.net
 Project-URL: Repository, https://www.github.com/towalink/tlm
 Project-URL: Documentation, https://towalink.readthedocs.io
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: towalink-tlm Version: 0.3.1 Summary: command line
+Metadata-Version: 2.1 Name: towalink-tlm Version: 0.3.2 Summary: command line
 tool for configuring and managing a Towalink installation Home-page: https://
 www.towalink.net Author: The Towalink Project Author-email:
 pypi.tlm@towalink.net Project-URL: Project homepage, https://www.towalink.net
 Project-URL: Repository, https://www.github.com/towalink/tlm Project-URL:
 Documentation, https://towalink.readthedocs.io Keywords: Towalink VPN SD-WAN
 WireGuard Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU Affero
```

### Comparing `towalink_tlm-0.3.1/src/towalink_tlm.egg-info/SOURCES.txt` & `towalink_tlm-0.3.2/src/towalink_tlm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

