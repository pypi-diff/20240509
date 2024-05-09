# Comparing `tmp/networking-generic-switch-7.2.1.tar.gz` & `tmp/networking-generic-switch-7.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "networking-generic-switch-7.2.1.tar", last modified: Thu May  9 13:08:17 2024, max compression
+gzip compressed data, was "networking-generic-switch-7.3.0.tar", last modified: Mon Mar  4 09:56:23 2024, max compression
```

## Comparing `networking-generic-switch-7.2.1.tar` & `networking-generic-switch-7.3.0.tar`

### file list

```diff
@@ -1,188 +1,190 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-09 13:08:17.492974 networking-generic-switch-7.2.1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3029 2024-05-09 13:08:17.000000 networking-generic-switch-7.2.1/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2289 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13149 2024-05-09 13:08:17.000000 networking-generic-switch-7.2.1/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2591 2024-05-09 13:08:17.492974 networking-generic-switch-7.2.1/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1424 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-09 13:08:17.464972 networking-generic-switch-7.2.1/devstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4333 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/devstack/exercise.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1830 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/devstack/exercise.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11496 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/devstack/plugin.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/devstack/settings
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-09 13:08:17.464972 networking-generic-switch-7.2.1/devstack/upgrade/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1274 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/devstack/upgrade/resources.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/devstack/upgrade/settings
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2725 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/devstack/upgrade/upgrade.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-09 13:08:17.464972 networking-generic-switch-7.2.1/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      416 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-09 13:08:17.468973 networking-generic-switch-7.2.1/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2858 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16030 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/doc/source/configuration.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/doc/source/contributing.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-09 13:08:17.468973 networking-generic-switch-7.2.1/doc/source/dev/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3696 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/doc/source/dev/dev-quickstart.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-09 13:08:17.468973 networking-generic-switch-7.2.1/doc/source/include/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/doc/source/include/configure-neutron.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      350 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      376 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/doc/source/installation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      792 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/doc/source/supported-devices.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-09 13:08:17.460972 networking-generic-switch-7.2.1/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-09 13:08:17.460972 networking-generic-switch-7.2.1/etc/neutron/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-09 13:08:17.460972 networking-generic-switch-7.2.1/etc/neutron/plugins/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-09 13:08:17.468973 networking-generic-switch-7.2.1/etc/neutron/plugins/ml2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/etc/neutron/plugins/ml2/ml2_conf_genericswitch.ini.sample
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-09 13:08:17.468973 networking-generic-switch-7.2.1/networking_generic_switch/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      780 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/_i18n.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17169 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/batching.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1998 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/config.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-09 13:08:17.468973 networking-generic-switch-7.2.1/networking_generic_switch/devices/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8125 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/devices/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-09 13:08:17.472973 networking-generic-switch-7.2.1/networking_generic_switch/devices/netmiko_devices/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17314 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/devices/netmiko_devices/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1218 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/devices/netmiko_devices/arista.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1520 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/devices/netmiko_devices/aruba.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2381 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/devices/netmiko_devices/brocade.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2342 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/devices/netmiko_devices/cisco.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1374 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/devices/netmiko_devices/cisco300.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2474 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/devices/netmiko_devices/cumulus.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5353 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/devices/netmiko_devices/dell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1880 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/devices/netmiko_devices/fake.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1084 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/devices/netmiko_devices/hpe.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1172 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/devices/netmiko_devices/huawei.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1253 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/devices/netmiko_devices/huawei_vrpv8.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8057 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/devices/netmiko_devices/juniper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1163 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/devices/netmiko_devices/mellanox_mlnxos.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4249 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/devices/netmiko_devices/nokia.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1031 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/devices/netmiko_devices/ovs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1168 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/devices/netmiko_devices/pluribus.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1215 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/devices/netmiko_devices/ruijie.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2678 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/devices/netmiko_devices/sonic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2049 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/devices/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1985 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26449 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/generic_switch_mech.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2984 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/locking.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-09 13:08:17.472973 networking-generic-switch-7.2.1/networking_generic_switch/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-09 13:08:17.476973 networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-09 13:08:17.476973 networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/devices/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/devices/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2687 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/devices/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-09 13:08:17.480973 networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/netmiko/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/netmiko/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3630 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/netmiko/test_arista_eos.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5919 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/netmiko/test_aruba.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4036 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/netmiko/test_brocade_fastiron.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3468 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/netmiko/test_cisco_300.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3623 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/netmiko/test_cisco_ios.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4619 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/netmiko/test_cisco_nxos.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6911 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/netmiko/test_cumulus.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21116 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/netmiko/test_dell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3136 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/netmiko/test_huawei.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4493 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/netmiko/test_huawei_vrpv8.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15443 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/netmiko/test_juniper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20789 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/netmiko/test_netmiko_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6017 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/netmiko/test_nokia_srl.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3148 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/netmiko/test_ovs_linux.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2384 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/netmiko/test_pluribus.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4844 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/netmiko/test_sonic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16177 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/test_batching.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1966 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/test_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9236 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/test_devices.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    49926 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/test_generic_switch_mech.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3304 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/test_locking.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-09 13:08:17.468973 networking-generic-switch-7.2.1/networking_generic_switch.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2591 2024-05-09 13:08:17.000000 networking-generic-switch-7.2.1/networking_generic_switch.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7243 2024-05-09 13:08:17.000000 networking-generic-switch-7.2.1/networking_generic_switch.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-09 13:08:17.000000 networking-generic-switch-7.2.1/networking_generic_switch.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2132 2024-05-09 13:08:17.000000 networking-generic-switch-7.2.1/networking_generic_switch.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-09 13:08:17.000000 networking-generic-switch-7.2.1/networking_generic_switch.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-05-09 13:08:17.000000 networking-generic-switch-7.2.1/networking_generic_switch.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2024-05-09 13:08:17.000000 networking-generic-switch-7.2.1/networking_generic_switch.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       26 2024-05-09 13:08:17.000000 networking-generic-switch-7.2.1/networking_generic_switch.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-09 13:08:17.460972 networking-generic-switch-7.2.1/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-09 13:08:17.484973 networking-generic-switch-7.2.1/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/notes/add-aruba-support-463a90b0b150b9af.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/notes/add-cisco-nx-os-support-8046a33107e2a670.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/notes/add-cumulus-nclu-support-ddcffa604c3e1b18.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/notes/add-dellos10-support-c6426372f960ded4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      587 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/notes/add-initial-note-ae1c9f9709c2e66f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/notes/add-mellanox-mlnx-os-switch-support-a4bf0661cd27fec7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/notes/add-ngs_save_configuration-180c2145f08e54d2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      301 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/notes/add-ngs_ssh_disabled_algorithms-dfe3e805f480ce90.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/notes/add-sonic-os-switch-support-73fcaf3acdc8c1d0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/notes/add-switchmode-option-to-dell-powerconnect-87718a84430444ef.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      363 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/notes/add_alias_for_hpe_comware-0eb9a016f0c992df.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/notes/add_netmiko_hpe_comware_device-c39be5d96943c6fd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      488 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/notes/add_ngs_default_vlan-ab09e0f4fd7ce897.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/notes/batching-12d9005924fd9d74.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/notes/cumulus-802.3ad-da9bffe131995f98.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/notes/dell-powerconnect-5ce572b9fb2702d3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/notes/disable-inactive-ports-bd6c42ceb232aab2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/notes/drop-py-2-7-76d7a678dc042bd6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/notes/fix-junos-syntax-27bb18dc737d776b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      312 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/notes/fix-netmiko-and-ngs-33c79b55ff7e2fd7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/notes/fixes-netmiko-regression-binding-port-groups-af6978a199a381b1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      698 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/notes/juniper-92d75d3086cf78a2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/notes/junos-retry-warnings-f2b004fe99d7770d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      522 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/notes/log-unknown-ngs-options-8a385406055ccc98.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/notes/manage-vlans-c75e4c2e9b9b3403.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/notes/net-add-del-failure-f4ea1118bc1f9d28.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/notes/netmiko-session-logging-9834fcdb8d6e5bb3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      191 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/notes/network-name-format-075f5757d599ac92.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/notes/ngs-stress-78f9e993e62e2e36.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       60 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/notes/nokia-srl-support-52ea2a445f4b24d4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/notes/normalize-ngs-macaddr-1ff0b6be7a53087a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/notes/remove-del_network-transitional-2f5742f7cafa2276.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      106 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/notes/ruijie-netmiko-driver-14e521fc36ede897.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      425 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/notes/support-multiple-links-in-port-group-59a11c2c2da73065.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-09 13:08:17.488973 networking-generic-switch-7.2.1/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/source/2023.1.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-09 13:08:17.488973 networking-generic-switch-7.2.1/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-09 13:08:17.488973 networking-generic-switch-7.2.1/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9556 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      565 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3029 2024-05-09 13:08:17.492974 networking-generic-switch-7.2.1/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/setup.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-09 13:08:17.488973 networking-generic-switch-7.2.1/tempest_plugin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/tempest_plugin/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/tempest_plugin/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1734 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/tempest_plugin/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1504 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/tempest_plugin/plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-09 13:08:17.492974 networking-generic-switch-7.2.1/tempest_plugin/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/tempest_plugin/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-09 13:08:17.492974 networking-generic-switch-7.2.1/tempest_plugin/tests/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/tempest_plugin/tests/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1141 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/tempest_plugin/tests/common/ovs_lib.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-09 13:08:17.492974 networking-generic-switch-7.2.1/tempest_plugin/tests/scenario/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/tempest_plugin/tests/scenario/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5464 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/tempest_plugin/tests/scenario/test_ngs_basic_ops.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-09 13:08:17.492974 networking-generic-switch-7.2.1/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      477 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/tools/flake8wrap.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-09 13:08:17.492974 networking-generic-switch-7.2.1/tools/ngs-stress/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2277 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/tools/ngs-stress/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5653 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/tools/ngs-stress/ngs_stress.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1296 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/tools/run_bashate.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2999 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-09 13:08:17.492974 networking-generic-switch-7.2.1/zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1735 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/zuul.d/networking-generic-switch-jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1344 2024-05-09 13:07:52.000000 networking-generic-switch-7.2.1/zuul.d/project.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 09:56:23.464801 networking-generic-switch-7.3.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3189 2024-03-04 09:56:23.000000 networking-generic-switch-7.3.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2289 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13703 2024-03-04 09:56:23.000000 networking-generic-switch-7.3.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2591 2024-03-04 09:56:23.464801 networking-generic-switch-7.3.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1424 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 09:56:23.448801 networking-generic-switch-7.3.0/devstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4333 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/devstack/exercise.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1830 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/devstack/exercise.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11496 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/devstack/plugin.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/devstack/settings
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 09:56:23.448801 networking-generic-switch-7.3.0/devstack/upgrade/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1274 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/devstack/upgrade/resources.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/devstack/upgrade/settings
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2725 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/devstack/upgrade/upgrade.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 09:56:23.448801 networking-generic-switch-7.3.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      416 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 09:56:23.448801 networking-generic-switch-7.3.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2858 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16030 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/doc/source/configuration.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/doc/source/contributing.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 09:56:23.448801 networking-generic-switch-7.3.0/doc/source/dev/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3696 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/doc/source/dev/dev-quickstart.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 09:56:23.448801 networking-generic-switch-7.3.0/doc/source/include/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/doc/source/include/configure-neutron.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      350 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      376 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/doc/source/installation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      792 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/doc/source/supported-devices.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 09:56:23.448801 networking-generic-switch-7.3.0/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 09:56:23.448801 networking-generic-switch-7.3.0/etc/neutron/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 09:56:23.448801 networking-generic-switch-7.3.0/etc/neutron/plugins/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 09:56:23.452801 networking-generic-switch-7.3.0/etc/neutron/plugins/ml2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/etc/neutron/plugins/ml2/ml2_conf_genericswitch.ini.sample
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 09:56:23.452801 networking-generic-switch-7.3.0/networking_generic_switch/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      780 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/_i18n.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17169 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/batching.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2026 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/config.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 09:56:23.452801 networking-generic-switch-7.3.0/networking_generic_switch/devices/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8302 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/devices/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 09:56:23.452801 networking-generic-switch-7.3.0/networking_generic_switch/devices/netmiko_devices/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17314 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/devices/netmiko_devices/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1218 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/devices/netmiko_devices/arista.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1520 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/devices/netmiko_devices/aruba.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2381 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/devices/netmiko_devices/brocade.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2342 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/devices/netmiko_devices/cisco.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1374 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/devices/netmiko_devices/cisco300.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2474 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/devices/netmiko_devices/cumulus.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5353 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/devices/netmiko_devices/dell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3062 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/devices/netmiko_devices/fake.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1084 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/devices/netmiko_devices/hpe.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1172 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/devices/netmiko_devices/huawei.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1253 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/devices/netmiko_devices/huawei_vrpv8.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8057 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/devices/netmiko_devices/juniper.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1163 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/devices/netmiko_devices/mellanox_mlnxos.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4249 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/devices/netmiko_devices/nokia.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1031 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/devices/netmiko_devices/ovs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1168 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/devices/netmiko_devices/pluribus.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1215 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/devices/netmiko_devices/ruijie.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2678 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/devices/netmiko_devices/sonic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2049 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/devices/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1985 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26856 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/generic_switch_mech.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2984 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/locking.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 09:56:23.452801 networking-generic-switch-7.3.0/networking_generic_switch/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 09:56:23.452801 networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 09:56:23.452801 networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/devices/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/devices/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2687 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/devices/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 09:56:23.456801 networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/netmiko/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/netmiko/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3630 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/netmiko/test_arista_eos.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5919 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/netmiko/test_aruba.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4036 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/netmiko/test_brocade_fastiron.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3468 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/netmiko/test_cisco_300.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3623 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/netmiko/test_cisco_ios.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4619 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/netmiko/test_cisco_nxos.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6911 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/netmiko/test_cumulus.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21116 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/netmiko/test_dell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3136 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/netmiko/test_huawei.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4493 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/netmiko/test_huawei_vrpv8.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15443 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/netmiko/test_juniper.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20789 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/netmiko/test_netmiko_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6017 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/netmiko/test_nokia_srl.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3148 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/netmiko/test_ovs_linux.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2384 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/netmiko/test_pluribus.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4844 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/netmiko/test_sonic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16177 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/test_batching.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1966 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/test_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9236 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/test_devices.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    54687 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/test_generic_switch_mech.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3304 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/test_locking.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 09:56:23.452801 networking-generic-switch-7.3.0/networking_generic_switch.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2591 2024-03-04 09:56:23.000000 networking-generic-switch-7.3.0/networking_generic_switch.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7356 2024-03-04 09:56:23.000000 networking-generic-switch-7.3.0/networking_generic_switch.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-04 09:56:23.000000 networking-generic-switch-7.3.0/networking_generic_switch.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2132 2024-03-04 09:56:23.000000 networking-generic-switch-7.3.0/networking_generic_switch.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-04 09:56:23.000000 networking-generic-switch-7.3.0/networking_generic_switch.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-03-04 09:56:23.000000 networking-generic-switch-7.3.0/networking_generic_switch.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2024-03-04 09:56:23.000000 networking-generic-switch-7.3.0/networking_generic_switch.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       26 2024-03-04 09:56:23.000000 networking-generic-switch-7.3.0/networking_generic_switch.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 09:56:23.448801 networking-generic-switch-7.3.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 09:56:23.460801 networking-generic-switch-7.3.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/notes/add-aruba-support-463a90b0b150b9af.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/notes/add-cisco-nx-os-support-8046a33107e2a670.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/notes/add-cumulus-nclu-support-ddcffa604c3e1b18.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/notes/add-dellos10-support-c6426372f960ded4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      587 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/notes/add-initial-note-ae1c9f9709c2e66f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/notes/add-mellanox-mlnx-os-switch-support-a4bf0661cd27fec7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/notes/add-ngs_save_configuration-180c2145f08e54d2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      301 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/notes/add-ngs_ssh_disabled_algorithms-dfe3e805f480ce90.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/notes/add-sonic-os-switch-support-73fcaf3acdc8c1d0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/notes/add-switchmode-option-to-dell-powerconnect-87718a84430444ef.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      363 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/notes/add_alias_for_hpe_comware-0eb9a016f0c992df.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/notes/add_netmiko_hpe_comware_device-c39be5d96943c6fd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      488 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/notes/add_ngs_default_vlan-ab09e0f4fd7ce897.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/notes/batching-12d9005924fd9d74.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/notes/cumulus-802.3ad-da9bffe131995f98.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/notes/delete_network_postcommit-more-defensive-19929702ba7f19fb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/notes/dell-powerconnect-5ce572b9fb2702d3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/notes/disable-inactive-ports-bd6c42ceb232aab2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/notes/drop-py-2-7-76d7a678dc042bd6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/notes/fix-junos-syntax-27bb18dc737d776b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      312 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/notes/fix-netmiko-and-ngs-33c79b55ff7e2fd7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/notes/fixes-netmiko-regression-binding-port-groups-af6978a199a381b1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      698 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/notes/juniper-92d75d3086cf78a2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/notes/junos-retry-warnings-f2b004fe99d7770d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      522 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/notes/log-unknown-ngs-options-8a385406055ccc98.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/notes/manage-vlans-c75e4c2e9b9b3403.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/notes/net-add-del-failure-f4ea1118bc1f9d28.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/notes/netmiko-session-logging-9834fcdb8d6e5bb3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      191 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/notes/network-name-format-075f5757d599ac92.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/notes/ngs-stress-78f9e993e62e2e36.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       60 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/notes/nokia-srl-support-52ea2a445f4b24d4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/notes/normalize-ngs-macaddr-1ff0b6be7a53087a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/notes/remove-del_network-transitional-2f5742f7cafa2276.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      106 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/notes/ruijie-netmiko-driver-14e521fc36ede897.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      425 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/notes/support-multiple-links-in-port-group-59a11c2c2da73065.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 09:56:23.460801 networking-generic-switch-7.3.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/source/2023.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/source/2023.2.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 09:56:23.460801 networking-generic-switch-7.3.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 09:56:23.460801 networking-generic-switch-7.3.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9556 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      565 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3082 2024-03-04 09:56:23.464801 networking-generic-switch-7.3.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/setup.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 09:56:23.460801 networking-generic-switch-7.3.0/tempest_plugin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/tempest_plugin/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/tempest_plugin/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1734 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/tempest_plugin/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1504 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/tempest_plugin/plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 09:56:23.460801 networking-generic-switch-7.3.0/tempest_plugin/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/tempest_plugin/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 09:56:23.460801 networking-generic-switch-7.3.0/tempest_plugin/tests/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/tempest_plugin/tests/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1140 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/tempest_plugin/tests/common/ovs_lib.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 09:56:23.460801 networking-generic-switch-7.3.0/tempest_plugin/tests/scenario/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/tempest_plugin/tests/scenario/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5464 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/tempest_plugin/tests/scenario/test_ngs_basic_ops.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 09:56:23.464801 networking-generic-switch-7.3.0/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      477 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/tools/flake8wrap.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 09:56:23.464801 networking-generic-switch-7.3.0/tools/ngs-stress/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2277 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/tools/ngs-stress/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5653 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/tools/ngs-stress/ngs_stress.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1296 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/tools/run_bashate.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3264 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-04 09:56:23.464801 networking-generic-switch-7.3.0/zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1810 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/zuul.d/networking-generic-switch-jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1421 2024-03-04 09:55:56.000000 networking-generic-switch-7.3.0/zuul.d/project.yaml
```

### Comparing `networking-generic-switch-7.2.1/AUTHORS` & `networking-generic-switch-7.3.0/AUTHORS`

 * *Files 7% similar despite different names*

```diff
@@ -11,23 +11,25 @@
 Ghanshyam Mann <gmann@ghanshyammann.com>
 Graham Hayes <gr@ham.ie>
 Guang Yee <guang.yee@suse.com>
 Hangdong Zhang <hdzhang@fiberhome.com>
 Harald Jensas <hjensas@redhat.com>
 Harald Jensås <hjensas@redhat.com>
 Henry Gessau <gessau@gmail.com>
+Hervé Beraud <hberaud@redhat.com>
 Hironori Shiina <shiina.hironori@jp.fujitsu.com>
 Ian Wienand <iwienand@redhat.com>
 Iury Gregory Melo Ferreira <imelofer@redhat.com>
 James Denton <james.denton@outlook.com>
 James Denton <james.denton@rackspace.com>
 James E. Blair <jeblair@redhat.com>
 Jay Faulkner <jay@jvf.cc>
 Jenkins <jenkins@cz7764.bud.mirantis.net>
 Jim Rollenhagen <jim@jimrollenhagen.com>
+John Garbutt <john.garbutt@gresearch.co.uk>
 John Garbutt <john.garbutt@stackhpc.com>
 John Garbutt <john@johngarbutt.com>
 John L. Villalovos <john.l.villalovos@intel.com>
 John L. Villalovos <openstack.org@sodarock.com>
 Julia Kreger <juliaashleykreger@gmail.com>
 Kaifeng Wang <kaifeng.w@gmail.com>
 Le Hou <houl7@chinaunicom.cn>
@@ -42,17 +44,19 @@
 Pierre Riteau <priteau@uchicago.edu>
 Piotr Parczewski <piotr@stackhpc.com>
 Riccardo Pittau <elfosardo@gmail.com>
 Ruby Loo <ruby.loo@intel.com>
 Sean McGinnis <sean.mcginnis@gmail.com>
 Sebastien Guay <sebastien.guay@nokia.com>
 Serge Kovaleff <serge.kovaleff@gmail.com>
+Sharpz7 <adam.mcarthur62@gmail.com>
 Steve Relf <s.relf@eschercloud.ai>
 Stig Telfer <stig.openstack@telfer.org>
 Sławek Kapłoński <skaplons@redhat.com>
+Takashi Kajinami <kajinamit@oss.nttdata.com>
 Tuan Do Anh <tuanda@vn.fujitsu.com>
 Vasyl Saienko <vsaienko@mirantis.com>
 Vieri <15050873171@163.com>
 Vlad Gridin <vladyslav.gridin@nuagenetworks.net>
 Vlad Sorokin <vvsorokin@us.ibm.com>
 Vladyslav Drok <vdrok@mirantis.com>
 Vu Cong Tuan <tuanvc@vn.fujitsu.com>
```

### Comparing `networking-generic-switch-7.2.1/CONTRIBUTING.rst` & `networking-generic-switch-7.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/ChangeLog` & `networking-generic-switch-7.3.0/ChangeLog`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,29 @@
 CHANGES
 =======
 
-7.2.1
+7.3.0
 -----
 
+* reno: Update master for unmaintained/yoga
+* [codespell] Adding CI target for Tox Codespell
+* [codespell] Adding Tox Target for Codespell
+* [codespell] Fixing Spelling Mistakes
+* Clean up removed services from devstack options
+* Revert "bump eventlet to latest version that support python 3.12"
+* bump eventlet to latest version that support python 3.12
+* [ngs\_coordination] backend\_url should be secret
+* Fix batching error due to outdated etcd3gw
 * Fix regression plugging 802.3ad port group
-* Honor ngs\_save\_configuration setting when using batch commands
+* Update master for stable/2023.2
 * CI fix: Use the un-deprecated v3 etcd API
-* Update TOX\_CONSTRAINTS\_FILE for stable/2023.2
-* Update .gitreview for stable/2023.2
+* Fix delete\_network\_postcommit KeyError
+* Do not make actual device changes in bind\_port()
+* Honor ngs\_save\_configuration setting when using batch commands
+* Fake: support adding a random sleep and injecting failures
 
 7.2.0
 -----
 
 * Bugs are now tracked in launchpad, fix docs
 * Fixes, updates for CI configuration
 * Update master for stable/2023.1
```

### Comparing `networking-generic-switch-7.2.1/LICENSE` & `networking-generic-switch-7.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/PKG-INFO` & `networking-generic-switch-7.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: networking-generic-switch
-Version: 7.2.1
+Version: 7.3.0
 Summary: Generic Switch ML2 Neutron Driver
 Home-page: https://github.com/openstack/networking-generic-switch
 Author: Mirantis
 Author-email: mos-ironic@mirantis.com
 License: UNKNOWN
 Description: ============================================
         Networking-generic-switch Neutron ML2 driver
```

### Comparing `networking-generic-switch-7.2.1/README.rst` & `networking-generic-switch-7.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/devstack/exercise.py` & `networking-generic-switch-7.3.0/devstack/exercise.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/devstack/exercise.sh` & `networking-generic-switch-7.3.0/devstack/exercise.sh`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/devstack/plugin.sh` & `networking-generic-switch-7.3.0/devstack/plugin.sh`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/devstack/upgrade/resources.sh` & `networking-generic-switch-7.3.0/devstack/upgrade/resources.sh`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/devstack/upgrade/upgrade.sh` & `networking-generic-switch-7.3.0/devstack/upgrade/upgrade.sh`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/doc/source/conf.py` & `networking-generic-switch-7.3.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/doc/source/configuration.rst` & `networking-generic-switch-7.3.0/doc/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/doc/source/dev/dev-quickstart.rst` & `networking-generic-switch-7.3.0/doc/source/dev/dev-quickstart.rst`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/doc/source/supported-devices.rst` & `networking-generic-switch-7.3.0/doc/source/supported-devices.rst`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/_i18n.py` & `networking-generic-switch-7.3.0/networking_generic_switch/_i18n.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/batching.py` & `networking-generic-switch-7.3.0/networking_generic_switch/batching.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/config.py` & `networking-generic-switch-7.3.0/networking_generic_switch/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from oslo_log import log as logging
 
 CONF = cfg.CONF
 LOG = logging.getLogger(__name__)
 
 coordination_opts = [
     cfg.StrOpt('backend_url',
+               secret=True,
                help='The backend URL to use for distributed coordination.'),
     cfg.IntOpt('acquire_timeout',
                min=0,
                default=60,
                help='Timeout in seconds after which an attempt to grab a lock '
                     'is failed. Value of 0 is forever.'),
 ]
```

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/devices/__init__.py` & `networking-generic-switch-7.3.0/networking_generic_switch/devices/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,14 +46,18 @@
     {'name': 'ngs_network_name_format', 'default': '{network_id}'},
     # If false, ngs will not add and delete VLANs from switches
     {'name': 'ngs_manage_vlans', 'default': True},
     # If False, ngs will skip saving configuration on devices
     {'name': 'ngs_save_configuration', 'default': True},
     # When true try to batch up in flight switch requests
     {'name': 'ngs_batch_requests', 'default': False},
+    # The following three are used in the Fake device driver.
+    {'name': 'ngs_fake_sleep_min_s'},
+    {'name': 'ngs_fake_sleep_max_s'},
+    {'name': 'ngs_fake_failure_prob'},
 ]
 
 
 def device_manager(device_cfg, device_name=""):
     device_type = device_cfg.get('device_type', '')
     try:
         mgr = stevedore.driver.DriverManager(
```

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/devices/netmiko_devices/__init__.py` & `networking-generic-switch-7.3.0/networking_generic_switch/devices/netmiko_devices/__init__.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/devices/netmiko_devices/arista.py` & `networking-generic-switch-7.3.0/networking_generic_switch/devices/netmiko_devices/arista.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/devices/netmiko_devices/aruba.py` & `networking-generic-switch-7.3.0/networking_generic_switch/devices/netmiko_devices/aruba.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/devices/netmiko_devices/brocade.py` & `networking-generic-switch-7.3.0/networking_generic_switch/devices/netmiko_devices/brocade.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/devices/netmiko_devices/cisco.py` & `networking-generic-switch-7.3.0/networking_generic_switch/devices/netmiko_devices/cisco.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/devices/netmiko_devices/cisco300.py` & `networking-generic-switch-7.3.0/networking_generic_switch/devices/netmiko_devices/cisco300.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/devices/netmiko_devices/cumulus.py` & `networking-generic-switch-7.3.0/networking_generic_switch/devices/netmiko_devices/cumulus.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/devices/netmiko_devices/dell.py` & `networking-generic-switch-7.3.0/networking_generic_switch/devices/netmiko_devices/dell.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/devices/netmiko_devices/hpe.py` & `networking-generic-switch-7.3.0/networking_generic_switch/devices/netmiko_devices/hpe.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/devices/netmiko_devices/huawei.py` & `networking-generic-switch-7.3.0/networking_generic_switch/devices/netmiko_devices/huawei.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/devices/netmiko_devices/huawei_vrpv8.py` & `networking-generic-switch-7.3.0/networking_generic_switch/devices/netmiko_devices/huawei_vrpv8.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/devices/netmiko_devices/juniper.py` & `networking-generic-switch-7.3.0/networking_generic_switch/devices/netmiko_devices/juniper.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/devices/netmiko_devices/mellanox_mlnxos.py` & `networking-generic-switch-7.3.0/networking_generic_switch/devices/netmiko_devices/mellanox_mlnxos.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/devices/netmiko_devices/nokia.py` & `networking-generic-switch-7.3.0/networking_generic_switch/devices/netmiko_devices/nokia.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/devices/netmiko_devices/ovs.py` & `networking-generic-switch-7.3.0/networking_generic_switch/devices/netmiko_devices/ovs.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/devices/netmiko_devices/pluribus.py` & `networking-generic-switch-7.3.0/networking_generic_switch/devices/netmiko_devices/pluribus.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/devices/netmiko_devices/ruijie.py` & `networking-generic-switch-7.3.0/networking_generic_switch/devices/netmiko_devices/ruijie.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/devices/netmiko_devices/sonic.py` & `networking-generic-switch-7.3.0/networking_generic_switch/devices/netmiko_devices/sonic.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/devices/utils.py` & `networking-generic-switch-7.3.0/networking_generic_switch/devices/utils.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/exceptions.py` & `networking-generic-switch-7.3.0/networking_generic_switch/exceptions.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/generic_switch_mech.py` & `networking-generic-switch-7.3.0/networking_generic_switch/generic_switch_mech.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 #    under the License.
 
 import sys
 
 from neutron.db import provisioning_blocks
 from neutron_lib.api.definitions import portbindings
 from neutron_lib.callbacks import resources
+from neutron_lib import constants as const
 from neutron_lib.plugins.ml2 import api
 from oslo_log import log as logging
 
 from networking_generic_switch import config as gsw_conf
 from networking_generic_switch import devices
 from networking_generic_switch.devices import utils as device_utils
 
@@ -75,17 +76,17 @@
         will block the entire process so care should be taken to not
         drastically affect performance. Raising an exception will
         cause the deletion of the resource.
         """
 
         network = context.current
         network_id = network['id']
-        provider_type = network['provider:network_type']
-        segmentation_id = network['provider:segmentation_id']
-        physnet = network['provider:physical_network']
+        provider_type = network.get('provider:network_type')
+        segmentation_id = network.get('provider:segmentation_id')
+        physnet = network.get('provider:physical_network')
 
         if provider_type == 'vlan' and segmentation_id:
             # Create vlan on all switches from this driver
             for switch_name, switch in self._get_devices_by_physnet(physnet):
                 try:
                     switch.add_network(segmentation_id, network_id)
                 except Exception as e:
@@ -160,17 +161,17 @@
         Called after the transaction commits. Call can block, though
         will block the entire process so care should be taken to not
         drastically affect performance. Runtime errors are not
         expected, and will not prevent the resource from being
         deleted.
         """
         network = context.current
-        provider_type = network['provider:network_type']
-        segmentation_id = network['provider:segmentation_id']
-        physnet = network['provider:physical_network']
+        provider_type = network.get('provider:network_type')
+        segmentation_id = network.get('provider:segmentation_id')
+        physnet = network.get('provider:physical_network')
 
         if provider_type == 'vlan' and segmentation_id:
             # Delete vlan on all switches from this driver
             exc_info = None
             for switch_name, switch in self._get_devices_by_physnet(physnet):
                 try:
                     switch.del_network(segmentation_id, network['id'])
@@ -336,28 +337,58 @@
         result in the deletion of the resource.
 
         update_port_postcommit is called for all changes to the port
         state. It is up to the mechanism driver to ignore state or
         state changes that it does not know or care about.
         """
         port = context.current
+        network = context.network.current
         if self._is_port_bound(port):
             binding_profile = port['binding:profile']
             local_link_information = binding_profile.get(
                 'local_link_information')
             if not local_link_information:
                 return
+            # Necessary because the "provisioning_complete" event triggers
+            # an additional call to update_port_postcommit().  We don't
+            # want to configure the port a second time.
+            if port['status'] == const.PORT_STATUS_ACTIVE:
+                LOG.debug("Port %(port_id)s is already active, "
+                          "not doing anything",
+                          {'port_id': port['id']})
+                return
+            # If binding has already succeeded, we should have valid links
+            # at this point, but check just in case.
+            if not self._is_link_valid(port, network):
+                return
+            is_802_3ad = self._is_802_3ad(port)
             for link in local_link_information:
+                port_id = link.get('port_id')
                 switch_info = link.get('switch_info')
                 switch_id = link.get('switch_id')
                 switch = device_utils.get_switch_device(
                     self.switches, switch_info=switch_info,
                     ngs_mac_address=switch_id)
-                if not switch:
-                    return
+
+                # If segmentation ID is None, set vlan 1
+                segmentation_id = network.get('provider:segmentation_id') or 1
+                LOG.debug("Putting switch port %(switch_port)s on "
+                          "%(switch_info)s in vlan %(segmentation_id)s",
+                          {'switch_port': port_id, 'switch_info': switch_info,
+                           'segmentation_id': segmentation_id})
+                # Move port to network
+                if is_802_3ad and hasattr(switch, 'plug_bond_to_network'):
+                    switch.plug_bond_to_network(port_id, segmentation_id)
+                else:
+                    switch.plug_port_to_network(port_id, segmentation_id)
+                LOG.info("Successfully plugged port %(port_id)s in segment "
+                         "%(segment_id)s on device %(device)s",
+                         {'port_id': port['id'], 'device': switch_info,
+                          'segment_id': segmentation_id})
+
             provisioning_blocks.provisioning_complete(
                 context._plugin_context, port['id'], resources.PORT,
                 GENERIC_SWITCH_ENTITY)
         elif self._is_port_bound(context.original):
             # The port has been unbound. This will cause the local link
             # information to be lost, so remove the port from the network on
             # the switch now while we have the required information.
@@ -442,40 +473,15 @@
 
         if self._is_port_supported(port) and local_link_information:
             # NOTE(jamesdenton): If any link of the port is invalid, none
             # of the links should be processed.
             if not self._is_link_valid(port, network):
                 return
 
-            is_802_3ad = self._is_802_3ad(port)
-            for link in local_link_information:
-                port_id = link.get('port_id')
-                switch_info = link.get('switch_info')
-                switch_id = link.get('switch_id')
-                switch = device_utils.get_switch_device(
-                    self.switches, switch_info=switch_info,
-                    ngs_mac_address=switch_id)
-
-                segments = context.segments_to_bind
-                # If segmentation ID is None, set vlan 1
-                segmentation_id = segments[0].get('segmentation_id') or 1
-                LOG.debug("Putting port %(port_id)s on %(switch_info)s "
-                          "to vlan: %(segmentation_id)s",
-                          {'port_id': port_id, 'switch_info': switch_info,
-                           'segmentation_id': segmentation_id})
-                # Move port to network
-                if is_802_3ad and hasattr(switch, 'plug_bond_to_network'):
-                    switch.plug_bond_to_network(port_id, segmentation_id)
-                else:
-                    switch.plug_port_to_network(port_id, segmentation_id)
-                LOG.info("Successfully bound port %(port_id)s in segment "
-                         "%(segment_id)s on device %(device)s",
-                         {'port_id': port['id'], 'device': switch_info,
-                          'segment_id': segmentation_id})
-
+            segments = context.segments_to_bind
             context.set_binding(segments[0][api.ID],
                                 portbindings.VIF_TYPE_OTHER, {})
             provisioning_blocks.add_provisioning_component(
                 context._plugin_context, port['id'], resources.PORT,
                 GENERIC_SWITCH_ENTITY)
 
     def _is_link_valid(self, port, network):
```

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/locking.py` & `networking-generic-switch-7.3.0/networking_generic_switch/locking.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/devices/test_utils.py` & `networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/devices/test_utils.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/netmiko/test_arista_eos.py` & `networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/netmiko/test_arista_eos.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/netmiko/test_aruba.py` & `networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/netmiko/test_aruba.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/netmiko/test_brocade_fastiron.py` & `networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/netmiko/test_brocade_fastiron.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/netmiko/test_cisco_300.py` & `networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/netmiko/test_cisco_300.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/netmiko/test_cisco_ios.py` & `networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/netmiko/test_cisco_ios.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/netmiko/test_cisco_nxos.py` & `networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/netmiko/test_cisco_nxos.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/netmiko/test_cumulus.py` & `networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/netmiko/test_cumulus.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/netmiko/test_dell.py` & `networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/netmiko/test_dell.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/netmiko/test_huawei.py` & `networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/netmiko/test_huawei.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/netmiko/test_huawei_vrpv8.py` & `networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/netmiko/test_huawei_vrpv8.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/netmiko/test_juniper.py` & `networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/netmiko/test_juniper.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/netmiko/test_netmiko_base.py` & `networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/netmiko/test_netmiko_base.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/netmiko/test_nokia_srl.py` & `networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/netmiko/test_nokia_srl.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/netmiko/test_ovs_linux.py` & `networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/netmiko/test_ovs_linux.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/netmiko/test_pluribus.py` & `networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/netmiko/test_pluribus.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/netmiko/test_sonic.py` & `networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/netmiko/test_sonic.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/test_batching.py` & `networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/test_batching.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/test_config.py` & `networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/test_devices.py` & `networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/test_devices.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/test_generic_switch_mech.py` & `networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/test_generic_switch_mech.py`

 * *Files 3% similar despite different names*

```diff
@@ -338,15 +338,15 @@
                                         'id': 'aaaa-bbbb-cccc'}
         mock_context.segments_to_bind = [mock_context.network.current]
 
         self.assertRaises(exceptions.GenericSwitchNetmikoMethodError,
                           driver.delete_port_postcommit,
                           mock_context)
 
-    def test_delete_port_potcommit_unknown_switch(self, m_list):
+    def test_delete_port_postcommit_unknown_switch(self, m_list):
         driver = gsm.GenericSwitchDriver()
         driver.initialize()
         mock_context = mock.create_autospec(driver_context.PortContext)
         mock_context.current = {'binding:profile':
                                 {'local_link_information':
                                     [
                                         {
@@ -404,20 +404,22 @@
                                             'switch_info': 'foo',
                                             'port_id': 2222
                                         }
                                     ]
                                  },
                                 'binding:vnic_type': 'baremetal',
                                 'id': '123',
-                                'binding:vif_type': 'unbound'}
+                                'binding:vif_type': 'unbound',
+                                'status': 'DOWN'}
         mock_context.original = {'binding:profile': {},
                                  'binding:vnic_type': 'baremetal',
                                  'id': '123',
                                  'binding:vif_type': 'unbound'}
         driver.update_port_postcommit(mock_context)
+        self.switch_mock.plug_port_to_network.assert_not_called()
         self.assertFalse(m_pc.called)
 
     @mock.patch.object(provisioning_blocks, 'provisioning_complete')
     def test_update_port_postcommit_not_baremetal(self, m_pc, m_list):
         driver = gsm.GenericSwitchDriver()
         driver.initialize()
         mock_context = mock.create_autospec(driver_context.PortContext)
@@ -429,37 +431,41 @@
                                             'switch_info': 'foo',
                                             'port_id': 2222
                                         }
                                     ]
                                  },
                                 'binding:vnic_type': 'mcvtap',
                                 'id': '123',
-                                'binding:vif_type': 'other'}
+                                'binding:vif_type': 'other',
+                                'status': 'DOWN'}
         mock_context.original = {'binding:profile': {},
                                  'binding:vnic_type': 'mcvtap',
                                  'id': '123',
                                  'binding:vif_type': 'unbound'}
         driver.update_port_postcommit(mock_context)
+        self.switch_mock.plug_port_to_network.assert_not_called()
         self.assertFalse(m_pc.called)
 
     @mock.patch.object(provisioning_blocks, 'provisioning_complete')
     def test_update_port_postcommit_no_llc(self, m_pc, m_list):
         driver = gsm.GenericSwitchDriver()
         driver.initialize()
         mock_context = mock.create_autospec(driver_context.PortContext)
         mock_context._plugin_context = mock.MagicMock()
         mock_context.current = {'binding:profile': {},
                                 'binding:vnic_type': 'baremetal',
                                 'id': '123',
-                                'binding:vif_type': 'other'}
+                                'binding:vif_type': 'other',
+                                'status': 'DOWN'}
         mock_context.original = {'binding:profile': {},
                                  'binding:vnic_type': 'baremetal',
                                  'id': '123',
                                  'binding:vif_type': 'unbound'}
         driver.update_port_postcommit(mock_context)
+        self.switch_mock.plug_port_to_network.assert_not_called()
         self.assertFalse(m_pc.called)
 
     @mock.patch.object(provisioning_blocks, 'provisioning_complete')
     def test_update_port_postcommit_not_managed_by_ngs(self, m_pc, m_list):
         driver = gsm.GenericSwitchDriver()
         driver.initialize()
         mock_context = mock.create_autospec(driver_context.PortContext)
@@ -471,20 +477,22 @@
                                             'switch_info': 'ughh',
                                             'port_id': 2222
                                         }
                                     ]
                                  },
                                 'binding:vnic_type': 'baremetal',
                                 'id': '123',
-                                'binding:vif_type': 'other'}
+                                'binding:vif_type': 'other',
+                                'status': 'DOWN'}
         mock_context.original = {'binding:profile': {},
                                  'binding:vnic_type': 'baremetal',
                                  'id': '123',
                                  'binding:vif_type': 'unbound'}
         driver.update_port_postcommit(mock_context)
+        self.switch_mock.plug_port_to_network.assert_not_called()
         self.assertFalse(m_pc.called)
 
     @mock.patch.object(provisioning_blocks, 'provisioning_complete')
     def test_update_port_postcommit_complete_provisioning(self, m_pc, m_list):
         driver = gsm.GenericSwitchDriver()
         driver.initialize()
         mock_context = mock.create_autospec(driver_context.PortContext)
@@ -496,21 +504,28 @@
                                             'switch_info': 'foo',
                                             'port_id': 2222
                                         }
                                     ]
                                  },
                                 'binding:vnic_type': 'baremetal',
                                 'id': '123',
-                                'binding:vif_type': 'other'}
+                                'binding:vif_type': 'other',
+                                'status': 'DOWN'}
         mock_context.original = {'binding:profile': {},
                                  'binding:vnic_type': 'baremetal',
                                  'id': '123',
                                  'binding:vif_type': 'unbound'}
+        mock_context.network = mock.Mock()
+        mock_context.network.current = {
+            'provider:segmentation_id': 42,
+            'provider:physical_network': 'physnet1'
+        }
         driver.update_port_postcommit(mock_context)
-        self.switch_mock.plug_port_to_network.assert_not_called()
+        self.switch_mock.plug_port_to_network.assert_called_once_with(
+            2222, 42)
         m_pc.assert_called_once_with(mock_context._plugin_context,
                                      mock_context.current['id'],
                                      resources.PORT,
                                      'GENERICSWITCH')
 
     @mock.patch.object(provisioning_blocks, 'provisioning_complete')
     def test_update_portgroup_postcommit_complete_provisioning(self,
@@ -531,21 +546,31 @@
                                             'switch_info': 'foo',
                                             'port_id': 3333
                                         },
                                     ]
                                  },
                                 'binding:vnic_type': 'baremetal',
                                 'id': '123',
-                                'binding:vif_type': 'other'}
+                                'binding:vif_type': 'other',
+                                'status': 'DOWN'}
         mock_context.original = {'binding:profile': {},
                                  'binding:vnic_type': 'baremetal',
                                  'id': '123',
                                  'binding:vif_type': 'unbound'}
+        mock_context.network = mock.Mock()
+        mock_context.network.current = {
+            'provider:segmentation_id': 42,
+            'provider:physical_network': 'physnet1'
+        }
         driver.update_port_postcommit(mock_context)
-        self.switch_mock.plug_port_to_network.assert_not_called()
+        self.switch_mock.plug_port_to_network.assert_has_calls(
+            [mock.call(2222, 42),
+             mock.call(3333, 42)]
+        )
+        self.switch_mock.plug_bond_to_network.assert_not_called()
         m_pc.assert_has_calls([mock.call(mock_context._plugin_context,
                                          mock_context.current['id'],
                                          resources.PORT,
                                          'GENERICSWITCH')])
 
     @mock.patch.object(provisioning_blocks, 'provisioning_complete')
     def test_update_portgroup_postcommit_complete_provisioning_802_3ad(self,
@@ -570,27 +595,106 @@
                                  'local_group_information':
                                     {
                                         'bond_mode': '802.3ad'
                                     }
                                  },
                                 'binding:vnic_type': 'baremetal',
                                 'id': '123',
-                                'binding:vif_type': 'other'}
+                                'binding:vif_type': 'other',
+                                'status': 'DOWN'}
         mock_context.original = {'binding:profile': {},
                                  'binding:vnic_type': 'baremetal',
                                  'id': '123',
                                  'binding:vif_type': 'unbound'}
+        mock_context.network = mock.Mock()
+        mock_context.network.current = {
+            'provider:segmentation_id': 42,
+            'provider:physical_network': 'physnet1'
+        }
         driver.update_port_postcommit(mock_context)
-        self.switch_mock.plug_bond_to_network.assert_not_called()
+        self.switch_mock.plug_bond_to_network.assert_has_calls(
+            [mock.call(2222, 42),
+             mock.call(3333, 42)]
+        )
+        self.switch_mock.plug_port_to_network.assert_not_called()
         m_pc.assert_has_calls([mock.call(mock_context._plugin_context,
                                          mock_context.current['id'],
                                          resources.PORT,
                                          'GENERICSWITCH')])
 
     @mock.patch.object(provisioning_blocks, 'provisioning_complete')
+    def test_update_port_postcommit_with_physnet(self, m_pc, m_list):
+        driver = gsm.GenericSwitchDriver()
+        driver.initialize()
+        mock_context = mock.create_autospec(driver_context.PortContext)
+        mock_context._plugin_context = mock.MagicMock()
+        mock_context.current = {'binding:profile':
+                                {'local_link_information':
+                                    [
+                                        {
+                                            'switch_info': 'foo',
+                                            'port_id': 2222
+                                        }
+                                    ]
+                                 },
+                                'binding:vnic_type': 'baremetal',
+                                'id': '123',
+                                'binding:vif_type': 'other',
+                                'status': 'DOWN'}
+        mock_context.original = {'binding:profile': {},
+                                 'binding:vnic_type': 'baremetal',
+                                 'id': '123',
+                                 'binding:vif_type': 'unbound'}
+        mock_context.network = mock.Mock()
+        mock_context.network.current = {
+            'provider:physical_network': 'physnet1'
+        }
+        self.switch_mock._get_physical_networks.return_value = ['physnet1']
+
+        driver.update_port_postcommit(mock_context)
+        self.switch_mock.plug_port_to_network.assert_called_once_with(
+            2222, 1)
+        m_pc.assert_called_once_with(mock_context._plugin_context,
+                                     mock_context.current['id'],
+                                     resources.PORT,
+                                     'GENERICSWITCH')
+
+    @mock.patch.object(provisioning_blocks, 'provisioning_complete')
+    def test_update_port_postcommit_with_different_physnet(self, m_pc, m_list):
+        driver = gsm.GenericSwitchDriver()
+        driver.initialize()
+        mock_context = mock.create_autospec(driver_context.PortContext)
+        mock_context._plugin_context = mock.MagicMock()
+        mock_context.current = {'binding:profile':
+                                {'local_link_information':
+                                    [
+                                        {
+                                            'switch_info': 'foo',
+                                            'port_id': 2222
+                                        }
+                                    ]
+                                 },
+                                'binding:vnic_type': 'baremetal',
+                                'id': '123',
+                                'binding:vif_type': 'other',
+                                'status': 'DOWN'}
+        mock_context.original = {'binding:profile': {},
+                                 'binding:vnic_type': 'baremetal',
+                                 'id': '123',
+                                 'binding:vif_type': 'unbound'}
+        mock_context.network.current = {
+            'provider:physical_network': 'physnet1'
+        }
+        self.switch_mock._get_physical_networks.return_value = ['physnet2']
+
+        driver.update_port_postcommit(mock_context)
+        self.switch_mock.plug_port_to_network.assert_not_called()
+        m_pc.assert_not_called()
+
+    @mock.patch.object(provisioning_blocks, 'provisioning_complete')
     def test_update_port_postcommit_unbind_not_bound(self, m_pc, m_list):
         driver = gsm.GenericSwitchDriver()
         driver.initialize()
         mock_context = mock.create_autospec(driver_context.PortContext)
         mock_context._plugin_context = mock.MagicMock()
         mock_context.current = {'binding:profile': {},
                                 'binding:vnic_type': 'baremetal',
@@ -771,21 +875,20 @@
             {
                 'segmentation_id': None,
                 'id': 123
             }
         ]
 
         driver.bind_port(mock_context)
-        self.switch_mock.plug_port_to_network.assert_called_once_with(
-            2222, 1)
         mock_context.set_binding.assert_called_with(123, 'other', {})
         m_apc.assert_called_once_with(mock_context._plugin_context,
                                       mock_context.current['id'],
                                       resources.PORT,
                                       'GENERICSWITCH')
+        self.switch_mock.plug_port_to_network.assert_not_called()
 
     @mock.patch.object(provisioning_blocks, 'add_provisioning_component')
     def test_bind_portgroup(self, m_apc, m_list):
         driver = gsm.GenericSwitchDriver()
         driver.initialize()
         mock_context = mock.create_autospec(driver_context.PortContext)
         mock_context._plugin_context = mock.MagicMock()
@@ -811,25 +914,22 @@
             {
                 'segmentation_id': None,
                 'id': 123
             }
         ]
 
         driver.bind_port(mock_context)
-        self.switch_mock.plug_port_to_network.assert_has_calls(
-            [mock.call(2222, 1),
-             mock.call(3333, 1)]
-        )
         mock_context.set_binding.assert_has_calls(
             [mock.call(123, 'other', {})]
         )
         m_apc.assert_has_calls([mock.call(mock_context._plugin_context,
                                           mock_context.current['id'],
                                           resources.PORT,
                                           'GENERICSWITCH')])
+        self.switch_mock.plug_port_to_network.assert_not_called()
 
     @mock.patch.object(provisioning_blocks, 'add_provisioning_component')
     def test_bind_portgroup_802_3ad(self, m_apc, m_list):
         driver = gsm.GenericSwitchDriver()
         driver.initialize()
         mock_context = mock.create_autospec(driver_context.PortContext)
         mock_context._plugin_context = mock.MagicMock()
@@ -859,25 +959,23 @@
             {
                 'segmentation_id': None,
                 'id': 123
             }
         ]
 
         driver.bind_port(mock_context)
-        self.switch_mock.plug_bond_to_network.assert_has_calls(
-            [mock.call(2222, 1),
-             mock.call(3333, 1)]
-        )
         mock_context.set_binding.assert_has_calls(
             [mock.call(123, 'other', {})]
         )
         m_apc.assert_has_calls([mock.call(mock_context._plugin_context,
                                           mock_context.current['id'],
                                           resources.PORT,
                                           'GENERICSWITCH')])
+        self.switch_mock.plug_port_to_network.assert_not_called()
+        self.switch_mock.plug_bond_to_network.assert_not_called()
 
     @mock.patch.object(provisioning_blocks, 'add_provisioning_component')
     def test_bind_port_with_physnet(self, m_apc, m_list):
         driver = gsm.GenericSwitchDriver()
         driver.initialize()
         mock_context = mock.create_autospec(driver_context.PortContext)
         mock_context._plugin_context = mock.MagicMock()
@@ -900,21 +998,20 @@
                 'segmentation_id': None,
                 'id': 123
             }
         ]
         self.switch_mock._get_physical_networks.return_value = ['physnet1']
 
         driver.bind_port(mock_context)
-        self.switch_mock.plug_port_to_network.assert_called_once_with(
-            2222, 1)
         mock_context.set_binding.assert_called_with(123, 'other', {})
         m_apc.assert_called_once_with(mock_context._plugin_context,
                                       mock_context.current['id'],
                                       resources.PORT,
                                       'GENERICSWITCH')
+        self.switch_mock.plug_port_to_network.assert_not_called()
 
     @mock.patch.object(provisioning_blocks, 'add_provisioning_component')
     def test_bind_port_unknown_switch(self, m_apc, m_list):
         driver = gsm.GenericSwitchDriver()
         driver.initialize()
         mock_context = mock.create_autospec(driver_context.PortContext)
         mock_context._plugin_context = mock.MagicMock()
```

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch/tests/unit/test_locking.py` & `networking-generic-switch-7.3.0/networking_generic_switch/tests/unit/test_locking.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch.egg-info/PKG-INFO` & `networking-generic-switch-7.3.0/networking_generic_switch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: networking-generic-switch
-Version: 7.2.1
+Version: 7.3.0
 Summary: Generic Switch ML2 Neutron Driver
 Home-page: https://github.com/openstack/networking-generic-switch
 Author: Mirantis
 Author-email: mos-ironic@mirantis.com
 License: UNKNOWN
 Description: ============================================
         Networking-generic-switch Neutron ML2 driver
```

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch.egg-info/SOURCES.txt` & `networking-generic-switch-7.3.0/networking_generic_switch.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,15 @@
 releasenotes/notes/add-sonic-os-switch-support-73fcaf3acdc8c1d0.yaml
 releasenotes/notes/add-switchmode-option-to-dell-powerconnect-87718a84430444ef.yaml
 releasenotes/notes/add_alias_for_hpe_comware-0eb9a016f0c992df.yaml
 releasenotes/notes/add_netmiko_hpe_comware_device-c39be5d96943c6fd.yaml
 releasenotes/notes/add_ngs_default_vlan-ab09e0f4fd7ce897.yaml
 releasenotes/notes/batching-12d9005924fd9d74.yaml
 releasenotes/notes/cumulus-802.3ad-da9bffe131995f98.yaml
+releasenotes/notes/delete_network_postcommit-more-defensive-19929702ba7f19fb.yaml
 releasenotes/notes/dell-powerconnect-5ce572b9fb2702d3.yaml
 releasenotes/notes/disable-inactive-ports-bd6c42ceb232aab2.yaml
 releasenotes/notes/drop-py-2-7-76d7a678dc042bd6.yaml
 releasenotes/notes/fix-junos-syntax-27bb18dc737d776b.yaml
 releasenotes/notes/fix-netmiko-and-ngs-33c79b55ff7e2fd7.yaml
 releasenotes/notes/fixes-netmiko-regression-binding-port-groups-af6978a199a381b1.yaml
 releasenotes/notes/juniper-92d75d3086cf78a2.yaml
@@ -120,14 +121,15 @@
 releasenotes/notes/ngs-stress-78f9e993e62e2e36.yaml
 releasenotes/notes/nokia-srl-support-52ea2a445f4b24d4.yaml
 releasenotes/notes/normalize-ngs-macaddr-1ff0b6be7a53087a.yaml
 releasenotes/notes/remove-del_network-transitional-2f5742f7cafa2276.yaml
 releasenotes/notes/ruijie-netmiko-driver-14e521fc36ede897.yaml
 releasenotes/notes/support-multiple-links-in-port-group-59a11c2c2da73065.yaml
 releasenotes/source/2023.1.rst
+releasenotes/source/2023.2.rst
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/queens.rst
 releasenotes/source/rocky.rst
 releasenotes/source/stein.rst
 releasenotes/source/train.rst
 releasenotes/source/unreleased.rst
```

### Comparing `networking-generic-switch-7.2.1/networking_generic_switch.egg-info/entry_points.txt` & `networking-generic-switch-7.3.0/networking_generic_switch.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/releasenotes/notes/add-initial-note-ae1c9f9709c2e66f.yaml` & `networking-generic-switch-7.3.0/releasenotes/notes/add-initial-note-ae1c9f9709c2e66f.yaml`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/releasenotes/notes/juniper-92d75d3086cf78a2.yaml` & `networking-generic-switch-7.3.0/releasenotes/notes/juniper-92d75d3086cf78a2.yaml`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/releasenotes/notes/log-unknown-ngs-options-8a385406055ccc98.yaml` & `networking-generic-switch-7.3.0/releasenotes/notes/log-unknown-ngs-options-8a385406055ccc98.yaml`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/releasenotes/source/conf.py` & `networking-generic-switch-7.3.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/requirements.txt` & `networking-generic-switch-7.3.0/requirements.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # The order of packages is significant, because pip processes them in the order
 # of appearance. Changing the order has an impact on the overall integration
 # process, which may cause wedges in the gate later.
-etcd3gw>=0.2.4 # Apache-2.0
+etcd3gw>=2.1.0 # Apache-2.0
 eventlet>=0.18.2 # Apache-2.0
 stevedore>=1.20.0 # Apache-2.0
 netmiko>=4.1.1 # MIT
 neutron>=13.0.0.0b1 # Apache-2.0
 neutron-lib>=1.18.0 # Apache-2.0
 oslo.config>=5.2.0 # Apache-2.0
 oslo.i18n>=3.15.3 # Apache-2.0
```

### Comparing `networking-generic-switch-7.2.1/setup.cfg` & `networking-generic-switch-7.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -50,11 +50,15 @@
 	netmiko_nokia_srl = networking_generic_switch.devices.netmiko_devices.nokia:NokiaSRL
 	netmiko_pluribus = networking_generic_switch.devices.netmiko_devices.pluribus:Pluribus
 	netmiko_aruba_os = networking_generic_switch.devices.netmiko_devices.aruba:ArubaOSCX
 	netmiko_fake = networking_generic_switch.devices.netmiko_devices.fake:Fake
 tempest.test_plugins = 
 	ngs_tests = tempest_plugin.plugin:NGSTempestPlugin
 
+[codespell]
+quiet-level = 4
+ignore-words-list = cna
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `networking-generic-switch-7.2.1/setup.py` & `networking-generic-switch-7.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/tempest_plugin/config.py` & `networking-generic-switch-7.3.0/tempest_plugin/config.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/tempest_plugin/plugin.py` & `networking-generic-switch-7.3.0/tempest_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/tempest_plugin/tests/common/ovs_lib.py` & `networking-generic-switch-7.3.0/tempest_plugin/tests/common/ovs_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 
-# I'd be happy to re-use ovs_lib from neutron.agent.common
+# I'd be happy to reuse ovs_lib from neutron.agent.common
 # but Tempest all_plugin run tries to import the module
 # and has an issue with importing CLI options
 # Current approach is to re-implement a small subset of ovsctl commands
 
 import json
 
 from tempest.lib.cli import base
```

### Comparing `networking-generic-switch-7.2.1/tempest_plugin/tests/scenario/test_ngs_basic_ops.py` & `networking-generic-switch-7.3.0/tempest_plugin/tests/scenario/test_ngs_basic_ops.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/tools/ngs-stress/README.rst` & `networking-generic-switch-7.3.0/tools/ngs-stress/README.rst`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/tools/ngs-stress/ngs_stress.py` & `networking-generic-switch-7.3.0/tools/ngs-stress/ngs_stress.py`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/tools/run_bashate.sh` & `networking-generic-switch-7.3.0/tools/run_bashate.sh`

 * *Files identical despite different names*

### Comparing `networking-generic-switch-7.2.1/tox.ini` & `networking-generic-switch-7.3.0/tox.ini`

 * *Files 23% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 setenv = VIRTUAL_ENV={envdir}
          PYTHONDONTWRITEBYTECODE = 1
          PYTHONWARNINGS=default::DeprecationWarning
          LANGUAGE=en_US
          LC_ALL=en_US.UTF-8
          TESTS_DIR=./networking_generic_switch/tests/unit/
 deps =
-    -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/2023.2}
+    -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
     -r{toxinidir}/requirements.txt
     -r{toxinidir}/test-requirements.txt
 passenv =
     http_proxy
     HTTP_PROXY
     https_proxy
     HTTPS_PROXY
@@ -44,15 +44,15 @@
   doc8 README.rst CONTRIBUTING.rst doc/source --ignore D001
 
 [testenv:docs]
 setenv = PYTHONHASHSEED=0
 sitepackages = False
 envdir = {toxworkdir}/venv
 deps =
-    -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/2023.2}
+    -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
     -r{toxinidir}/requirements.txt
     -r{toxinidir}/doc/requirements.txt
 commands =
   sphinx-build -W -b html doc/source doc/build/html
 
 [testenv:pdf-docs]
 allowlist_externals = make
@@ -62,23 +62,23 @@
 deps = {[testenv:docs]deps}
 commands =
   sphinx-build -b latex doc/source doc/build/pdf
   make -C doc/build/pdf
 
 [testenv:releasenotes]
 deps =
-    -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/2023.2}
+    -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
     -r{toxinidir}/doc/requirements.txt
 commands =
   sphinx-build -a -E -W -d releasenotes/build/doctrees -b html releasenotes/source releasenotes/build/html
 
 [testenv:venv]
 setenv = PYTHONHASHSEED=0
 deps =
-    -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/2023.2}
+    -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
     -r{toxinidir}/test-requirements.txt
     -r{toxinidir}/doc/requirements.txt
 commands = {posargs}
 
 [flake8]
 exclude =  .venv,.git,.tox,dist,doc,*lib/python*,*egg,build
 max-complexity=17
@@ -95,7 +95,17 @@
 commands =
     coverage erase
     coverage run --branch --include "networking_generic_switch*" -m unittest discover networking_generic_switch.tests.unit
     coverage report -m --fail-under 70
 
 [hacking]
 import_exceptions = networking_generic_switch._i18n
+
+[testenv:codespell]
+description =
+  Run codespell to check spelling
+deps = codespell
+# note(JayF): {posargs} lets us run `tox -ecodespell -- -w` to get codespell
+#             to correct spelling issues in our code it's aware of.
+commands =
+  codespell {posargs}
+
```

### Comparing `networking-generic-switch-7.2.1/zuul.d/project.yaml` & `networking-generic-switch-7.3.0/zuul.d/project.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -17,14 +17,16 @@
               - ^tools/.*$
               - ^tox.ini$
               - ^setup.cfg$
         # NOTE(rpittau): temp disabling job until all changes
         # for ussuri are completed
         - ironic-grenade-dsvm-multinode-multitenant:
             voting: false
+        - networking-generic-switch-tox-codespell:
+            voting: false
     gate:
       jobs:
         - networking-generic-switch-tempest-dlm
         - ironic-tempest-ipa-wholedisk-direct-tinyipa-multinode:
             irrelevant-files:
               - ^.*\.rst$
               - ^doc/.*$
```

