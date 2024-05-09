# Comparing `tmp/metalsmith-2.1.0.tar.gz` & `tmp/metalsmith-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metalsmith-2.1.0.tar", last modified: Wed Nov 15 11:11:26 2023, max compression
+gzip compressed data, was "metalsmith-2.1.1.tar", last modified: Thu Feb 22 15:05:18 2024, max compression
```

## Comparing `metalsmith-2.1.0.tar` & `metalsmith-2.1.1.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-15 11:11:26.114216 metalsmith-2.1.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       38 2023-11-15 11:10:37.000000 metalsmith-2.1.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5814 2023-11-15 11:10:37.000000 metalsmith-2.1.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1013 2023-11-15 11:11:25.000000 metalsmith-2.1.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11543 2023-11-15 11:11:25.000000 metalsmith-2.1.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2023-11-15 11:10:37.000000 metalsmith-2.1.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2952 2023-11-15 11:11:26.114216 metalsmith-2.1.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1559 2023-11-15 11:10:37.000000 metalsmith-2.1.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-15 11:11:26.102216 metalsmith-2.1.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2023-11-15 11:10:37.000000 metalsmith-2.1.0/doc/joined-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2023-11-15 11:10:37.000000 metalsmith-2.1.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-15 11:11:26.102216 metalsmith-2.1.0/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-15 11:11:26.102216 metalsmith-2.1.0/doc/source/_exts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9068 2023-11-15 11:10:37.000000 metalsmith-2.1.0/doc/source/_exts/ansible-autodoc.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-15 11:11:26.102216 metalsmith-2.1.0/doc/source/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      803 2023-11-15 11:10:37.000000 metalsmith-2.1.0/doc/source/cli/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2889 2023-11-15 11:10:37.000000 metalsmith-2.1.0/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      471 2023-11-15 11:10:37.000000 metalsmith-2.1.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-15 11:11:26.102216 metalsmith-2.1.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2023-11-15 11:10:37.000000 metalsmith-2.1.0/doc/source/user/ansible.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-15 11:11:26.102216 metalsmith-2.1.0/metalsmith/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      772 2023-11-15 11:10:37.000000 metalsmith-2.1.0/metalsmith/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11069 2023-11-15 11:10:37.000000 metalsmith-2.1.0/metalsmith/_cmd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4122 2023-11-15 11:10:37.000000 metalsmith-2.1.0/metalsmith/_format.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5504 2023-11-15 11:10:37.000000 metalsmith-2.1.0/metalsmith/_instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3506 2023-11-15 11:10:37.000000 metalsmith-2.1.0/metalsmith/_network_metadata.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9141 2023-11-15 11:10:37.000000 metalsmith-2.1.0/metalsmith/_nics.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31736 2023-11-15 11:10:37.000000 metalsmith-2.1.0/metalsmith/_provisioner.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6097 2023-11-15 11:10:37.000000 metalsmith-2.1.0/metalsmith/_scheduler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4276 2023-11-15 11:10:37.000000 metalsmith-2.1.0/metalsmith/_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2955 2023-11-15 11:10:37.000000 metalsmith-2.1.0/metalsmith/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5717 2023-11-15 11:10:37.000000 metalsmith-2.1.0/metalsmith/instance_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13443 2023-11-15 11:10:37.000000 metalsmith-2.1.0/metalsmith/sources.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-15 11:11:26.106216 metalsmith-2.1.0/metalsmith/test/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-15 11:10:37.000000 metalsmith-2.1.0/metalsmith/test/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    33972 2023-11-15 11:10:37.000000 metalsmith-2.1.0/metalsmith/test/test_cmd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7069 2023-11-15 11:10:37.000000 metalsmith-2.1.0/metalsmith/test/test_instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5820 2023-11-15 11:10:37.000000 metalsmith-2.1.0/metalsmith/test/test_instance_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10431 2023-11-15 11:10:37.000000 metalsmith-2.1.0/metalsmith/test/test_metalsmith_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5206 2023-11-15 11:10:37.000000 metalsmith-2.1.0/metalsmith/test/test_network_metadata.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15050 2023-11-15 11:10:37.000000 metalsmith-2.1.0/metalsmith/test/test_nics.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   101043 2023-11-15 11:10:37.000000 metalsmith-2.1.0/metalsmith/test/test_provisioner.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5386 2023-11-15 11:10:37.000000 metalsmith-2.1.0/metalsmith/test/test_scheduler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9678 2023-11-15 11:10:37.000000 metalsmith-2.1.0/metalsmith/test/test_sources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3361 2023-11-15 11:10:37.000000 metalsmith-2.1.0/metalsmith/test/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      741 2023-11-15 11:10:37.000000 metalsmith-2.1.0/metalsmith/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-15 11:11:26.106216 metalsmith-2.1.0/metalsmith.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2952 2023-11-15 11:11:25.000000 metalsmith-2.1.0/metalsmith.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4331 2023-11-15 11:11:26.000000 metalsmith-2.1.0/metalsmith.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-11-15 11:11:25.000000 metalsmith-2.1.0/metalsmith.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2023-11-15 11:11:25.000000 metalsmith-2.1.0/metalsmith.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-11-15 11:11:25.000000 metalsmith-2.1.0/metalsmith.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-11-15 11:11:25.000000 metalsmith-2.1.0/metalsmith.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2023-11-15 11:11:25.000000 metalsmith-2.1.0/metalsmith.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2023-11-15 11:11:25.000000 metalsmith-2.1.0/metalsmith.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-15 11:11:26.098216 metalsmith-2.1.0/metalsmith_ansible/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-15 11:11:26.098216 metalsmith-2.1.0/metalsmith_ansible/ansible_plugins/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-15 11:11:26.106216 metalsmith-2.1.0/metalsmith_ansible/ansible_plugins/modules/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4457 2023-11-15 11:10:37.000000 metalsmith-2.1.0/metalsmith_ansible/ansible_plugins/modules/metalsmith_deployment_defaults.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15915 2023-11-15 11:10:37.000000 metalsmith-2.1.0/metalsmith_ansible/ansible_plugins/modules/metalsmith_instances.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-15 11:11:26.098216 metalsmith-2.1.0/metalsmith_ansible/roles/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-15 11:11:26.106216 metalsmith-2.1.0/metalsmith_ansible/roles/metalsmith_deployment/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7263 2023-11-15 11:10:37.000000 metalsmith-2.1.0/metalsmith_ansible/roles/metalsmith_deployment/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-15 11:11:26.106216 metalsmith-2.1.0/metalsmith_ansible/roles/metalsmith_deployment/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      515 2023-11-15 11:10:37.000000 metalsmith-2.1.0/metalsmith_ansible/roles/metalsmith_deployment/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-15 11:11:26.106216 metalsmith-2.1.0/metalsmith_ansible/roles/metalsmith_deployment/meta/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       23 2023-11-15 11:10:37.000000 metalsmith-2.1.0/metalsmith_ansible/roles/metalsmith_deployment/meta/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-15 11:11:26.106216 metalsmith-2.1.0/metalsmith_ansible/roles/metalsmith_deployment/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1462 2023-11-15 11:10:37.000000 metalsmith-2.1.0/metalsmith_ansible/roles/metalsmith_deployment/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-15 11:11:26.098216 metalsmith-2.1.0/playbooks/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-15 11:11:26.110216 metalsmith-2.1.0/playbooks/integration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4541 2023-11-15 11:10:37.000000 metalsmith-2.1.0/playbooks/integration/centos-image.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2614 2023-11-15 11:10:37.000000 metalsmith-2.1.0/playbooks/integration/centos8-image.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1251 2023-11-15 11:10:37.000000 metalsmith-2.1.0/playbooks/integration/centos8-integration.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2614 2023-11-15 11:10:37.000000 metalsmith-2.1.0/playbooks/integration/centos9-image.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1251 2023-11-15 11:10:37.000000 metalsmith-2.1.0/playbooks/integration/centos9-integration.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3790 2023-11-15 11:10:37.000000 metalsmith-2.1.0/playbooks/integration/cirros-image.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3688 2023-11-15 11:10:37.000000 metalsmith-2.1.0/playbooks/integration/exercise.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1092 2023-11-15 11:10:37.000000 metalsmith-2.1.0/playbooks/integration/initial-setup.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2023-11-15 11:10:37.000000 metalsmith-2.1.0/playbooks/integration/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1250 2023-11-15 11:10:37.000000 metalsmith-2.1.0/playbooks/integration/run.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2023-11-15 11:10:37.000000 metalsmith-2.1.0/playbooks/integration/ssh-key.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-15 11:11:26.098216 metalsmith-2.1.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-15 11:11:26.114216 metalsmith-2.1.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/notes/0.9-deprecations-f403ce4961b77fe1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/notes/allocation-hostname-f148e8adf0aee89a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/notes/allow-both-network-and-subnet-in-nic-info-af8b40a26d55828e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/notes/api-stein-8e5d165aa6d115cf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/notes/associated-993c26ac5dc0cfc0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/notes/config_drive-f59bb5d8e684b2ef.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/notes/deprecations-14-4292eaa456564782.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/notes/drop-py-2-7-3cd57c85e8eb8d2d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/notes/exceptions-395ae4f1ad4de6da.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/notes/file-checksum-d19370a8fde00a81.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      426 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/notes/fix-ip-allocation-deferred-causing-broken-network-metadata-9c3ccfab2c563466.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/notes/format-hostname-634a412ea933a966.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/notes/iinfo-2014b1de4dbeca2d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/notes/initial-5afe4a5f6a13fa8e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/notes/instance-config-c4ea6a169f782138.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/notes/keep-instance-info-3e7bb09244d5aaa6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      545 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/notes/network-metadata-ff0c3e80e5e0f53c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/notes/no-clean-up-03bfaee6bbb112fb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      546 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/notes/openstacksdk-9ad2298b84e34a5f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/notes/prettytable-1db78a96c1d921d0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      418 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/notes/raw_http_images-41007351896ff642.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/notes/reserve-hostname-85d02321156bde3b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/notes/resource-class-1957e83fa8235641.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/notes/source-detect-673ad8c3e98c3df1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      558 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/notes/states-79b593683c0783d5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/notes/stein-deprecation-6a4c9217a6ac4f13.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/notes/subnet-1c177e4b40cc607c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      336 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/notes/update-references-for-checksums-44206e710b0506fe.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/notes/whole-disk-root-gb-bd8ee3600de9ec8d.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-15 11:11:26.114216 metalsmith-2.1.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/source/2023.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/source/2023.2.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-15 11:11:26.114216 metalsmith-2.1.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-15 11:11:26.114216 metalsmith-2.1.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6627 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      214 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-11-15 11:10:37.000000 metalsmith-2.1.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2023-11-15 11:10:37.000000 metalsmith-2.1.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1125 2023-11-15 11:11:26.114216 metalsmith-2.1.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-11-15 11:10:37.000000 metalsmith-2.1.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2023-11-15 11:10:37.000000 metalsmith-2.1.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-15 11:11:26.114216 metalsmith-2.1.0/tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      276 2023-11-15 11:10:37.000000 metalsmith-2.1.0/tools/ansible-lint.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3305 2023-11-15 11:10:37.000000 metalsmith-2.1.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.484915 metalsmith-2.1.1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       38 2024-02-22 15:04:47.000000 metalsmith-2.1.1/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6272 2024-02-22 15:04:47.000000 metalsmith-2.1.1/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1049 2024-02-22 15:05:18.000000 metalsmith-2.1.1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11740 2024-02-22 15:05:18.000000 metalsmith-2.1.1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2024-02-22 15:04:47.000000 metalsmith-2.1.1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2952 2024-02-22 15:05:18.484915 metalsmith-2.1.1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1559 2024-02-22 15:04:47.000000 metalsmith-2.1.1/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.464915 metalsmith-2.1.1/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2024-02-22 15:04:47.000000 metalsmith-2.1.1/doc/joined-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2024-02-22 15:04:47.000000 metalsmith-2.1.1/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.464915 metalsmith-2.1.1/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.464915 metalsmith-2.1.1/doc/source/_exts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9068 2024-02-22 15:04:47.000000 metalsmith-2.1.1/doc/source/_exts/ansible-autodoc.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.468915 metalsmith-2.1.1/doc/source/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      803 2024-02-22 15:04:47.000000 metalsmith-2.1.1/doc/source/cli/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2889 2024-02-22 15:04:47.000000 metalsmith-2.1.1/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      471 2024-02-22 15:04:47.000000 metalsmith-2.1.1/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.468915 metalsmith-2.1.1/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2024-02-22 15:04:47.000000 metalsmith-2.1.1/doc/source/user/ansible.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.468915 metalsmith-2.1.1/metalsmith/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      772 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11069 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/_cmd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4122 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/_format.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5504 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/_instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3506 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/_network_metadata.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9141 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/_nics.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31736 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/_provisioner.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6097 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/_scheduler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4276 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2955 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5717 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/instance_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13443 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/sources.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.472915 metalsmith-2.1.1/metalsmith/test/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/test/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    33972 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/test/test_cmd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7069 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/test/test_instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5820 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/test/test_instance_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10431 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/test/test_metalsmith_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5206 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/test/test_network_metadata.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15050 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/test/test_nics.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   101043 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/test/test_provisioner.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5386 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/test/test_scheduler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9678 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/test/test_sources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3361 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/test/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      741 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.468915 metalsmith-2.1.1/metalsmith.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2952 2024-02-22 15:05:18.000000 metalsmith-2.1.1/metalsmith.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4331 2024-02-22 15:05:18.000000 metalsmith-2.1.1/metalsmith.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-02-22 15:05:18.000000 metalsmith-2.1.1/metalsmith.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2024-02-22 15:05:18.000000 metalsmith-2.1.1/metalsmith.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-02-22 15:05:18.000000 metalsmith-2.1.1/metalsmith.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-02-22 15:05:18.000000 metalsmith-2.1.1/metalsmith.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2024-02-22 15:05:18.000000 metalsmith-2.1.1/metalsmith.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2024-02-22 15:05:18.000000 metalsmith-2.1.1/metalsmith.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.460915 metalsmith-2.1.1/metalsmith_ansible/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.460915 metalsmith-2.1.1/metalsmith_ansible/ansible_plugins/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.472915 metalsmith-2.1.1/metalsmith_ansible/ansible_plugins/modules/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4457 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith_ansible/ansible_plugins/modules/metalsmith_deployment_defaults.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15915 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith_ansible/ansible_plugins/modules/metalsmith_instances.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.460915 metalsmith-2.1.1/metalsmith_ansible/roles/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.472915 metalsmith-2.1.1/metalsmith_ansible/roles/metalsmith_deployment/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7263 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith_ansible/roles/metalsmith_deployment/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.472915 metalsmith-2.1.1/metalsmith_ansible/roles/metalsmith_deployment/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      515 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith_ansible/roles/metalsmith_deployment/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.472915 metalsmith-2.1.1/metalsmith_ansible/roles/metalsmith_deployment/meta/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       23 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith_ansible/roles/metalsmith_deployment/meta/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.472915 metalsmith-2.1.1/metalsmith_ansible/roles/metalsmith_deployment/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1462 2024-02-22 15:04:47.000000 metalsmith-2.1.1/metalsmith_ansible/roles/metalsmith_deployment/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.464915 metalsmith-2.1.1/playbooks/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.476915 metalsmith-2.1.1/playbooks/integration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4541 2024-02-22 15:04:47.000000 metalsmith-2.1.1/playbooks/integration/centos-image.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2614 2024-02-22 15:04:47.000000 metalsmith-2.1.1/playbooks/integration/centos8-image.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1251 2024-02-22 15:04:47.000000 metalsmith-2.1.1/playbooks/integration/centos8-integration.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2614 2024-02-22 15:04:47.000000 metalsmith-2.1.1/playbooks/integration/centos9-image.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1251 2024-02-22 15:04:47.000000 metalsmith-2.1.1/playbooks/integration/centos9-integration.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3790 2024-02-22 15:04:47.000000 metalsmith-2.1.1/playbooks/integration/cirros-image.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3688 2024-02-22 15:04:47.000000 metalsmith-2.1.1/playbooks/integration/exercise.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1092 2024-02-22 15:04:47.000000 metalsmith-2.1.1/playbooks/integration/initial-setup.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2024-02-22 15:04:47.000000 metalsmith-2.1.1/playbooks/integration/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1250 2024-02-22 15:04:47.000000 metalsmith-2.1.1/playbooks/integration/run.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2024-02-22 15:04:47.000000 metalsmith-2.1.1/playbooks/integration/ssh-key.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.464915 metalsmith-2.1.1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.480915 metalsmith-2.1.1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/0.9-deprecations-f403ce4961b77fe1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/allocation-hostname-f148e8adf0aee89a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/allow-both-network-and-subnet-in-nic-info-af8b40a26d55828e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/api-stein-8e5d165aa6d115cf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/associated-993c26ac5dc0cfc0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/config_drive-f59bb5d8e684b2ef.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/deprecations-14-4292eaa456564782.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/drop-py-2-7-3cd57c85e8eb8d2d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/exceptions-395ae4f1ad4de6da.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/file-checksum-d19370a8fde00a81.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      426 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/fix-ip-allocation-deferred-causing-broken-network-metadata-9c3ccfab2c563466.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/format-hostname-634a412ea933a966.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/iinfo-2014b1de4dbeca2d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/initial-5afe4a5f6a13fa8e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/instance-config-c4ea6a169f782138.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/keep-instance-info-3e7bb09244d5aaa6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      545 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/network-metadata-ff0c3e80e5e0f53c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/no-clean-up-03bfaee6bbb112fb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      546 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/openstacksdk-9ad2298b84e34a5f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/prettytable-1db78a96c1d921d0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      418 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/raw_http_images-41007351896ff642.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/reserve-hostname-85d02321156bde3b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/resource-class-1957e83fa8235641.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/source-detect-673ad8c3e98c3df1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      558 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/states-79b593683c0783d5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/stein-deprecation-6a4c9217a6ac4f13.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/subnet-1c177e4b40cc607c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      336 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/update-references-for-checksums-44206e710b0506fe.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/notes/whole-disk-root-gb-bd8ee3600de9ec8d.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.484915 metalsmith-2.1.1/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/source/2023.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/source/2023.2.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.484915 metalsmith-2.1.1/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.484915 metalsmith-2.1.1/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6627 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      214 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-02-22 15:04:47.000000 metalsmith-2.1.1/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2024-02-22 15:04:47.000000 metalsmith-2.1.1/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1154 2024-02-22 15:05:18.484915 metalsmith-2.1.1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-02-22 15:04:47.000000 metalsmith-2.1.1/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2024-02-22 15:04:47.000000 metalsmith-2.1.1/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:05:18.484915 metalsmith-2.1.1/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      276 2024-02-22 15:04:47.000000 metalsmith-2.1.1/tools/ansible-lint.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3567 2024-02-22 15:04:47.000000 metalsmith-2.1.1/tox.ini
```

### Comparing `metalsmith-2.1.0/.zuul.yaml` & `metalsmith-2.1.1/.zuul.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -107,14 +107,19 @@
         IRONIC_VM_SPECS_RAM: 1024
         LIBVIRT_STORAGE_POOL_PATH: /opt/libvirt/images
         SWIFT_ENABLE_TEMPURLS: true
         SWIFT_HASH: 54bd5642300c4b45-846f8636a70a07d2
         SWIFT_START_ALL_SERVICES: false
         SWIFT_TEMPURL_KEY: 54bd5642300c4b45846f8636a70a07d2
         IRONIC_PXE_BOOT_RETRY_TIMEOUT: 600
+        # Tell devstack to set an owner project as metalsmith
+        # testing is executed with a devstack-admin OS_CLOUD
+        # which means all action use it, and with newer RBAC,
+        # the node cannot be seen in that case.
+        IRONIC_SET_NODE_OWNER: admin
       centos_glance_initramds_image: test-centos-initramfs
       centos_glance_kernel_image: test-centos-kernel
       centos_glance_root_image: test-centos-partition
       centos_glance_whole_disk_image: test-centos-wholedisk
       metalsmith_netboot: false
       metalsmith_root_size: 9
       metalsmith_python: python3
@@ -161,26 +166,35 @@
         Integration job using HTTP as image source and direct deploy.
     parent: metalsmith-integration-base
     run: playbooks/integration/run.yaml
     vars:
       metalsmith_precreate_port: true
       metalsmith_use_http: true
 
+- job:
+    name: metalsmith-tox-codespell
+    parent: openstack-tox
+    timeout: 7200
+    vars:
+      tox_envlist: codespell
+
 - project:
     templates:
       - check-requirements
       - openstack-python3-antelope-jobs
       - openstack-cover-jobs
       - publish-openstack-docs-pti
       - release-notes-jobs-python3
     check:
       jobs:
         - metalsmith-integration-glance-centos9-uefi
         - metalsmith-integration-glance-centos9-legacy
         - metalsmith-integration-http-cirros
         - openstack-tox-linters
+        - metalsmith-tox-codespell:
+            voting: false
     gate:
       jobs:
         - metalsmith-integration-glance-centos9-uefi
         - metalsmith-integration-glance-centos9-legacy
         - metalsmith-integration-http-cirros
         - openstack-tox-linters
```

### Comparing `metalsmith-2.1.0/AUTHORS` & `metalsmith-2.1.1/AUTHORS`

 * *Files 15% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 Julia Kreger <juliaashleykreger@gmail.com>
 Kaifeng Wang <kaifeng.w@gmail.com>
 Lucas Alvares Gomes <lucasagomes@gmail.com>
 Mark Goddard <mark@stackhpc.com>
 OpenStack Release Bot <infra-root@openstack.org>
 Riccardo Pittau <elfosardo@gmail.com>
 Sean McGinnis <sean.mcginnis@gmail.com>
+Sharpz7 <adam.mcarthur62@gmail.com>
 Steve Baker <sbaker@redhat.com>
 Takashi Kajinami <tkajinam@redhat.com>
 Vieri <15050873171@163.com>
 Wander Way <wanderwayout@gmail.com>
 YuehuiLei <leiyuehui@inspur.com>
 caoyuan <cao.yuan@99cloud.net>
 jacky06 <zhang.min@99cloud.net>
```

### Comparing `metalsmith-2.1.0/ChangeLog` & `metalsmith-2.1.1/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 CHANGES
 =======
 
+2.1.1
+-----
+
+* reno: Update master for unmaintained/yoga
+* [codespell] Adding CI target for Tox Codespell
+* [codespell] Adding Tox Target for Codespell
+* CI: Ask ironic devstack to set node owner
+
 2.1.0
 -----
 
 * Document LP as official bugtracker
 * Metalsmith in maintenance mode
 * Update master for stable/2023.2
 * Set role default metalsmith\_provisioning\_timeout
```

### Comparing `metalsmith-2.1.0/LICENSE` & `metalsmith-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/PKG-INFO` & `metalsmith-2.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: metalsmith
-Version: 2.1.0
+Version: 2.1.1
 Summary: Deployment and Scheduling tool for Bare Metal
 Home-page: https://opendev.org/openstack/metalsmith
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache-2
 Description: Deployment and Scheduling tool for Bare Metal
         =============================================
```

### Comparing `metalsmith-2.1.0/README.rst` & `metalsmith-2.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/doc/source/_exts/ansible-autodoc.py` & `metalsmith-2.1.1/doc/source/_exts/ansible-autodoc.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/doc/source/cli/index.rst` & `metalsmith-2.1.1/doc/source/cli/index.rst`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/doc/source/conf.py` & `metalsmith-2.1.1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/metalsmith/__init__.py` & `metalsmith-2.1.1/metalsmith/__init__.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/metalsmith/_cmd.py` & `metalsmith-2.1.1/metalsmith/_cmd.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/metalsmith/_format.py` & `metalsmith-2.1.1/metalsmith/_format.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/metalsmith/_instance.py` & `metalsmith-2.1.1/metalsmith/_instance.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/metalsmith/_network_metadata.py` & `metalsmith-2.1.1/metalsmith/_network_metadata.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/metalsmith/_nics.py` & `metalsmith-2.1.1/metalsmith/_nics.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/metalsmith/_provisioner.py` & `metalsmith-2.1.1/metalsmith/_provisioner.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/metalsmith/_scheduler.py` & `metalsmith-2.1.1/metalsmith/_scheduler.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/metalsmith/_utils.py` & `metalsmith-2.1.1/metalsmith/_utils.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/metalsmith/exceptions.py` & `metalsmith-2.1.1/metalsmith/exceptions.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/metalsmith/instance_config.py` & `metalsmith-2.1.1/metalsmith/instance_config.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/metalsmith/sources.py` & `metalsmith-2.1.1/metalsmith/sources.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/metalsmith/test/test_cmd.py` & `metalsmith-2.1.1/metalsmith/test/test_cmd.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/metalsmith/test/test_instance.py` & `metalsmith-2.1.1/metalsmith/test/test_instance.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/metalsmith/test/test_instance_config.py` & `metalsmith-2.1.1/metalsmith/test/test_instance_config.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/metalsmith/test/test_metalsmith_instances.py` & `metalsmith-2.1.1/metalsmith/test/test_metalsmith_instances.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/metalsmith/test/test_network_metadata.py` & `metalsmith-2.1.1/metalsmith/test/test_network_metadata.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/metalsmith/test/test_nics.py` & `metalsmith-2.1.1/metalsmith/test/test_nics.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/metalsmith/test/test_provisioner.py` & `metalsmith-2.1.1/metalsmith/test/test_provisioner.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/metalsmith/test/test_scheduler.py` & `metalsmith-2.1.1/metalsmith/test/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/metalsmith/test/test_sources.py` & `metalsmith-2.1.1/metalsmith/test/test_sources.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/metalsmith/test/test_utils.py` & `metalsmith-2.1.1/metalsmith/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/metalsmith/version.py` & `metalsmith-2.1.1/metalsmith/version.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/metalsmith.egg-info/PKG-INFO` & `metalsmith-2.1.1/metalsmith.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: metalsmith
-Version: 2.1.0
+Version: 2.1.1
 Summary: Deployment and Scheduling tool for Bare Metal
 Home-page: https://opendev.org/openstack/metalsmith
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache-2
 Description: Deployment and Scheduling tool for Bare Metal
         =============================================
```

### Comparing `metalsmith-2.1.0/metalsmith.egg-info/SOURCES.txt` & `metalsmith-2.1.1/metalsmith.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/metalsmith_ansible/ansible_plugins/modules/metalsmith_deployment_defaults.py` & `metalsmith-2.1.1/metalsmith_ansible/ansible_plugins/modules/metalsmith_deployment_defaults.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/metalsmith_ansible/ansible_plugins/modules/metalsmith_instances.py` & `metalsmith-2.1.1/metalsmith_ansible/ansible_plugins/modules/metalsmith_instances.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/metalsmith_ansible/roles/metalsmith_deployment/README.rst` & `metalsmith-2.1.1/metalsmith_ansible/roles/metalsmith_deployment/README.rst`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/metalsmith_ansible/roles/metalsmith_deployment/defaults/main.yml` & `metalsmith-2.1.1/metalsmith_ansible/roles/metalsmith_deployment/defaults/main.yml`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/metalsmith_ansible/roles/metalsmith_deployment/tasks/main.yml` & `metalsmith-2.1.1/metalsmith_ansible/roles/metalsmith_deployment/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/playbooks/integration/centos-image.yaml` & `metalsmith-2.1.1/playbooks/integration/centos-image.yaml`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/playbooks/integration/centos8-image.yaml` & `metalsmith-2.1.1/playbooks/integration/centos8-image.yaml`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/playbooks/integration/centos8-integration.yaml` & `metalsmith-2.1.1/playbooks/integration/centos8-integration.yaml`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/playbooks/integration/centos9-image.yaml` & `metalsmith-2.1.1/playbooks/integration/centos9-image.yaml`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/playbooks/integration/centos9-integration.yaml` & `metalsmith-2.1.1/playbooks/integration/centos9-integration.yaml`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/playbooks/integration/cirros-image.yaml` & `metalsmith-2.1.1/playbooks/integration/cirros-image.yaml`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/playbooks/integration/exercise.yaml` & `metalsmith-2.1.1/playbooks/integration/exercise.yaml`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/playbooks/integration/initial-setup.yaml` & `metalsmith-2.1.1/playbooks/integration/initial-setup.yaml`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/playbooks/integration/run.yaml` & `metalsmith-2.1.1/playbooks/integration/run.yaml`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/releasenotes/notes/network-metadata-ff0c3e80e5e0f53c.yaml` & `metalsmith-2.1.1/releasenotes/notes/network-metadata-ff0c3e80e5e0f53c.yaml`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/releasenotes/notes/openstacksdk-9ad2298b84e34a5f.yaml` & `metalsmith-2.1.1/releasenotes/notes/openstacksdk-9ad2298b84e34a5f.yaml`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/releasenotes/notes/states-79b593683c0783d5.yaml` & `metalsmith-2.1.1/releasenotes/notes/states-79b593683c0783d5.yaml`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/releasenotes/source/conf.py` & `metalsmith-2.1.1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/setup.cfg` & `metalsmith-2.1.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -30,11 +30,14 @@
 	share/ansible/roles/ = metalsmith_ansible/roles/*
 	share/ansible/plugins/ = metalsmith_ansible/ansible_plugins/*
 
 [entry_points]
 console_scripts = 
 	metalsmith = metalsmith._cmd:main
 
+[codespell]
+quiet-level = 4
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `metalsmith-2.1.0/setup.py` & `metalsmith-2.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `metalsmith-2.1.0/tox.ini` & `metalsmith-2.1.1/tox.ini`

 * *Files 22% similar despite different names*

```diff
@@ -13,15 +13,15 @@
          PYTHONDONTWRITEBYTECODE=1
 deps =
     -c{env:TOX_CONSTRAINTS_FILE:https://opendev.org/openstack/requirements/raw/branch/master/upper-constraints.txt}
     -r{toxinidir}/requirements.txt
     -r{toxinidir}/test-requirements.txt
 commands =
     stestr run {posargs}
-passenv = 
+passenv =
     http_proxy
     HTTP_PROXY
     https_proxy
     HTTPS_PROXY
     no_proxy
     NO_PROXY
 
@@ -115,7 +115,16 @@
 usedevelop = False
 allowlist_externals = bash
 deps =
   ansible>=5,<6
   ansible-lint>=5,<6
 commands =
     bash tools/ansible-lint.sh
+
+[testenv:codespell]
+description =
+  Run codespell to check spelling
+deps = codespell
+# note(JayF): {posargs} lets us run `tox -ecodespell -- -w` to get codespell
+#             to correct spelling issues in our code it's aware of.
+commands =
+  codespell {posargs}
```

