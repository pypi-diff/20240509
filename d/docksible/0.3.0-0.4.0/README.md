# Comparing `tmp/docksible-0.3.0.tar.gz` & `tmp/docksible-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docksible-0.3.0.tar", last modified: Mon Apr 22 18:32:58 2024, max compression
+gzip compressed data, was "docksible-0.4.0.tar", last modified: Thu May  9 16:13:41 2024, max compression
```

## Comparing `docksible-0.3.0.tar` & `docksible-0.4.0.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-22 18:32:58.077164 docksible-0.3.0/
--rw-rw-r--   0 brian     (1000) brian     (1000)       40 2024-04-22 18:30:44.000000 docksible-0.3.0/.gitignore
--rw-rw-r--   0 brian     (1000) brian     (1000)      603 2024-04-22 18:30:44.000000 docksible-0.3.0/LICENSE.txt
--rw-r--r--   0 brian     (1000) brian     (1000)     1225 2024-04-22 18:32:58.077164 docksible-0.3.0/PKG-INFO
--rw-rw-r--   0 brian     (1000) brian     (1000)      349 2024-04-22 18:30:44.000000 docksible-0.3.0/README.md
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-22 18:32:58.065164 docksible-0.3.0/_DEPRECATED_ansible/
--rw-rw-r--   0 brian     (1000) brian     (1000)      109 2024-04-22 18:30:44.000000 docksible-0.3.0/_DEPRECATED_ansible/django.yml
--rw-rw-r--   0 brian     (1000) brian     (1000)       73 2024-04-22 18:30:44.000000 docksible-0.3.0/_DEPRECATED_ansible/hosts
--rw-rw-r--   0 brian     (1000) brian     (1000)       68 2024-04-22 18:30:44.000000 docksible-0.3.0/_DEPRECATED_ansible/letsencrypt.yml
--rw-rw-r--   0 brian     (1000) brian     (1000)       93 2024-04-22 18:30:44.000000 docksible-0.3.0/_DEPRECATED_ansible/playbook.yml
--rw-rw-r--   0 brian     (1000) brian     (1000)      175 2024-04-22 18:30:44.000000 docksible-0.3.0/_DEPRECATED_ansible/readme.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)       86 2024-04-22 18:30:44.000000 docksible-0.3.0/_DEPRECATED_ansible/redmine.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-22 18:32:58.061164 docksible-0.3.0/_DEPRECATED_ansible/roles/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-22 18:32:58.061164 docksible-0.3.0/_DEPRECATED_ansible/roles/build-image/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-22 18:32:58.065164 docksible-0.3.0/_DEPRECATED_ansible/roles/build-image/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)      562 2024-04-22 18:30:44.000000 docksible-0.3.0/_DEPRECATED_ansible/roles/build-image/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-22 18:32:58.061164 docksible-0.3.0/_DEPRECATED_ansible/roles/django/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-22 18:32:58.065164 docksible-0.3.0/_DEPRECATED_ansible/roles/django/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)     1142 2024-04-22 18:30:44.000000 docksible-0.3.0/_DEPRECATED_ansible/roles/django/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-22 18:32:58.065164 docksible-0.3.0/_DEPRECATED_ansible/roles/django/templates/
--rw-rw-r--   0 brian     (1000) brian     (1000)      154 2024-04-22 18:30:44.000000 docksible-0.3.0/_DEPRECATED_ansible/roles/django/templates/.env
--rw-rw-r--   0 brian     (1000) brian     (1000)     1822 2024-04-22 18:30:44.000000 docksible-0.3.0/_DEPRECATED_ansible/roles/django/templates/docker-compose-django.yml.j2
--rw-rw-r--   0 brian     (1000) brian     (1000)      688 2024-04-22 18:30:44.000000 docksible-0.3.0/_DEPRECATED_ansible/roles/django/templates/nginx.conf.j2
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-22 18:32:58.061164 docksible-0.3.0/_DEPRECATED_ansible/roles/docker-compose/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-22 18:32:58.065164 docksible-0.3.0/_DEPRECATED_ansible/roles/docker-compose/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)     1608 2024-04-22 18:30:44.000000 docksible-0.3.0/_DEPRECATED_ansible/roles/docker-compose/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-22 18:32:58.065164 docksible-0.3.0/_DEPRECATED_ansible/roles/docker-compose/templates/
--rw-rw-r--   0 brian     (1000) brian     (1000)      126 2024-04-22 18:30:44.000000 docksible-0.3.0/_DEPRECATED_ansible/roles/docker-compose/templates/.env
--rw-rw-r--   0 brian     (1000) brian     (1000)     2222 2024-04-22 18:30:44.000000 docksible-0.3.0/_DEPRECATED_ansible/roles/docker-compose/templates/docker-compose.yml.j2
--rw-rw-r--   0 brian     (1000) brian     (1000)      389 2024-04-22 18:30:44.000000 docksible-0.3.0/_DEPRECATED_ansible/roles/docker-compose/templates/nginx.conf.j2
--rw-rw-r--   0 brian     (1000) brian     (1000)      795 2024-04-22 18:30:44.000000 docksible-0.3.0/_DEPRECATED_ansible/roles/docker-compose/templates/nginx.conf.j2.todo
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-22 18:32:58.061164 docksible-0.3.0/_DEPRECATED_ansible/roles/letsencrypt/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-22 18:32:58.065164 docksible-0.3.0/_DEPRECATED_ansible/roles/letsencrypt/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)     3296 2024-04-22 18:30:44.000000 docksible-0.3.0/_DEPRECATED_ansible/roles/letsencrypt/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-22 18:32:58.069164 docksible-0.3.0/_DEPRECATED_ansible/roles/letsencrypt/templates/
--rw-rw-r--   0 brian     (1000) brian     (1000)      984 2024-04-22 18:30:44.000000 docksible-0.3.0/_DEPRECATED_ansible/roles/letsencrypt/templates/docker-compose-certbot-django.yml.j2
--rw-rw-r--   0 brian     (1000) brian     (1000)      839 2024-04-22 18:30:44.000000 docksible-0.3.0/_DEPRECATED_ansible/roles/letsencrypt/templates/docker-compose-certbot-no-www.yml.j2
--rw-rw-r--   0 brian     (1000) brian     (1000)      859 2024-04-22 18:30:44.000000 docksible-0.3.0/_DEPRECATED_ansible/roles/letsencrypt/templates/docker-compose-certbot.yml.j2
--rw-rw-r--   0 brian     (1000) brian     (1000)      397 2024-04-22 18:30:44.000000 docksible-0.3.0/_DEPRECATED_ansible/roles/letsencrypt/templates/nginx.conf.1.j2
--rw-rw-r--   0 brian     (1000) brian     (1000)      990 2024-04-22 18:30:44.000000 docksible-0.3.0/_DEPRECATED_ansible/roles/letsencrypt/templates/nginx.conf.django.j2
--rw-rw-r--   0 brian     (1000) brian     (1000)      749 2024-04-22 18:30:44.000000 docksible-0.3.0/_DEPRECATED_ansible/roles/letsencrypt/templates/nginx.conf.j2
--rw-rw-r--   0 brian     (1000) brian     (1000)     5585 2024-04-22 18:30:44.000000 docksible-0.3.0/_DEPRECATED_ansible/roles/letsencrypt/templates/wp-config.php
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-22 18:32:58.061164 docksible-0.3.0/_DEPRECATED_ansible/roles/redmine/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-22 18:32:58.069164 docksible-0.3.0/_DEPRECATED_ansible/roles/redmine/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)     1027 2024-04-22 18:30:44.000000 docksible-0.3.0/_DEPRECATED_ansible/roles/redmine/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-22 18:32:58.069164 docksible-0.3.0/_DEPRECATED_ansible/roles/redmine/templates/
--rw-rw-r--   0 brian     (1000) brian     (1000)     1251 2024-04-22 18:30:44.000000 docksible-0.3.0/_DEPRECATED_ansible/roles/redmine/templates/docker-compose-redmine.yml.j2
--rw-rw-r--   0 brian     (1000) brian     (1000)      389 2024-04-22 18:30:44.000000 docksible-0.3.0/_DEPRECATED_ansible/roles/redmine/templates/nginx.conf.j2
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-22 18:32:58.061164 docksible-0.3.0/_DEPRECATED_ansible/roles/ssh-proxy/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-22 18:32:58.069164 docksible-0.3.0/_DEPRECATED_ansible/roles/ssh-proxy/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)      165 2024-04-22 18:30:44.000000 docksible-0.3.0/_DEPRECATED_ansible/roles/ssh-proxy/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-22 18:32:58.061164 docksible-0.3.0/_DEPRECATED_ansible/roles/ssl-selfsigned/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-22 18:32:58.069164 docksible-0.3.0/_DEPRECATED_ansible/roles/ssl-selfsigned/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)     2408 2024-04-22 18:30:44.000000 docksible-0.3.0/_DEPRECATED_ansible/roles/ssl-selfsigned/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-22 18:32:58.073164 docksible-0.3.0/_DEPRECATED_ansible/roles/ssl-selfsigned/templates/
--rw-rw-r--   0 brian     (1000) brian     (1000)      609 2024-04-22 18:30:44.000000 docksible-0.3.0/_DEPRECATED_ansible/roles/ssl-selfsigned/templates/nginx.conf.j2
--rw-rw-r--   0 brian     (1000) brian     (1000)      126 2024-04-22 18:30:44.000000 docksible-0.3.0/_DEPRECATED_ansible/roles/ssl-selfsigned/templates/self-signed.conf
--rw-rw-r--   0 brian     (1000) brian     (1000)      860 2024-04-22 18:30:44.000000 docksible-0.3.0/_DEPRECATED_ansible/roles/ssl-selfsigned/templates/ssl-params.conf
--rw-rw-r--   0 brian     (1000) brian     (1000)     5585 2024-04-22 18:30:44.000000 docksible-0.3.0/_DEPRECATED_ansible/roles/ssl-selfsigned/templates/wp-config.php
--rw-rw-r--   0 brian     (1000) brian     (1000)       71 2024-04-22 18:30:44.000000 docksible-0.3.0/_DEPRECATED_ansible/ssl-selfsigned.yml
--rw-rw-r--   0 brian     (1000) brian     (1000)    70933 2024-04-22 18:30:44.000000 docksible-0.3.0/_DEPRECATED_redmine_defaults.sql
--rw-rw-r--   0 brian     (1000) brian     (1000)     1169 2024-04-22 18:30:44.000000 docksible-0.3.0/pyproject.toml
--rw-rw-r--   0 brian     (1000) brian     (1000)       38 2024-04-22 18:32:58.077164 docksible-0.3.0/setup.cfg
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-22 18:32:58.061164 docksible-0.3.0/src/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-22 18:32:58.073164 docksible-0.3.0/src/docksible/
--rw-rw-r--   0 brian     (1000) brian     (1000)    10210 2024-04-22 18:30:44.000000 docksible-0.3.0/src/docksible/arg_validator.py
--rw-rw-r--   0 brian     (1000) brian     (1000)      231 2024-04-22 18:30:44.000000 docksible-0.3.0/src/docksible/constants.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    43534 2024-04-22 18:30:44.000000 docksible-0.3.0/src/docksible/docksible.py
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-22 18:32:58.077164 docksible-0.3.0/src/docksible/project/
--rw-rw-r--   0 brian     (1000) brian     (1000)       61 2024-04-22 18:30:44.000000 docksible-0.3.0/src/docksible/project/letsencrypt.yml
--rw-rw-r--   0 brian     (1000) brian     (1000)      115 2024-04-22 18:30:44.000000 docksible-0.3.0/src/docksible/project/redmine.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-22 18:32:58.061164 docksible-0.3.0/src/docksible/project/roles/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-22 18:32:58.061164 docksible-0.3.0/src/docksible/project/roles/letsencrypt/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-22 18:32:58.077164 docksible-0.3.0/src/docksible/project/roles/letsencrypt/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)     3260 2024-04-22 18:30:44.000000 docksible-0.3.0/src/docksible/project/roles/letsencrypt/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-22 18:32:58.077164 docksible-0.3.0/src/docksible/project/roles/letsencrypt/templates/
--rw-rw-r--   0 brian     (1000) brian     (1000)     1003 2024-04-22 18:30:44.000000 docksible-0.3.0/src/docksible/project/roles/letsencrypt/templates/docker-compose-certbot-django.yml.j2
--rw-rw-r--   0 brian     (1000) brian     (1000)      854 2024-04-22 18:30:44.000000 docksible-0.3.0/src/docksible/project/roles/letsencrypt/templates/docker-compose-certbot-no-www.yml.j2
--rw-rw-r--   0 brian     (1000) brian     (1000)      874 2024-04-22 18:30:44.000000 docksible-0.3.0/src/docksible/project/roles/letsencrypt/templates/docker-compose-certbot.yml.j2
--rw-rw-r--   0 brian     (1000) brian     (1000)      375 2024-04-22 18:30:44.000000 docksible-0.3.0/src/docksible/project/roles/letsencrypt/templates/nginx.conf.1.j2
--rw-rw-r--   0 brian     (1000) brian     (1000)      947 2024-04-22 18:30:44.000000 docksible-0.3.0/src/docksible/project/roles/letsencrypt/templates/nginx.conf.django.j2
--rw-rw-r--   0 brian     (1000) brian     (1000)      676 2024-04-22 18:30:44.000000 docksible-0.3.0/src/docksible/project/roles/letsencrypt/templates/nginx.conf.j2
--rw-rw-r--   0 brian     (1000) brian     (1000)     5646 2024-04-22 18:30:44.000000 docksible-0.3.0/src/docksible/project/roles/letsencrypt/templates/wp-config.php
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-22 18:32:58.061164 docksible-0.3.0/src/docksible/project/roles/redmine/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-22 18:32:58.077164 docksible-0.3.0/src/docksible/project/roles/redmine/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)     1056 2024-04-22 18:30:44.000000 docksible-0.3.0/src/docksible/project/roles/redmine/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-22 18:32:58.077164 docksible-0.3.0/src/docksible/project/roles/redmine/templates/
--rw-rw-r--   0 brian     (1000) brian     (1000)     1356 2024-04-22 18:30:44.000000 docksible-0.3.0/src/docksible/project/roles/redmine/templates/docker-compose-redmine.yml.j2
--rw-rw-r--   0 brian     (1000) brian     (1000)      386 2024-04-22 18:30:44.000000 docksible-0.3.0/src/docksible/project/roles/redmine/templates/nginx.conf.j2
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-22 18:32:58.061164 docksible-0.3.0/src/docksible/project/roles/setup-docker-compose/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-22 18:32:58.077164 docksible-0.3.0/src/docksible/project/roles/setup-docker-compose/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)     1171 2024-04-22 18:30:44.000000 docksible-0.3.0/src/docksible/project/roles/setup-docker-compose/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-22 18:32:58.061164 docksible-0.3.0/src/docksible/project/roles/ssh-proxy/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-22 18:32:58.077164 docksible-0.3.0/src/docksible/project/roles/ssh-proxy/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)      200 2024-04-22 18:30:44.000000 docksible-0.3.0/src/docksible/project/roles/ssh-proxy/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-22 18:32:58.065164 docksible-0.3.0/src/docksible/project/roles/wordpress/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-22 18:32:58.077164 docksible-0.3.0/src/docksible/project/roles/wordpress/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)     1068 2024-04-22 18:30:44.000000 docksible-0.3.0/src/docksible/project/roles/wordpress/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-22 18:32:58.077164 docksible-0.3.0/src/docksible/project/roles/wordpress/templates/
--rw-rw-r--   0 brian     (1000) brian     (1000)     1787 2024-04-22 18:30:44.000000 docksible-0.3.0/src/docksible/project/roles/wordpress/templates/docker-compose-wordpress.yml.j2
--rw-rw-r--   0 brian     (1000) brian     (1000)      386 2024-04-22 18:30:44.000000 docksible-0.3.0/src/docksible/project/roles/wordpress/templates/nginx.conf.j2
--rw-rw-r--   0 brian     (1000) brian     (1000)       85 2024-04-22 18:30:44.000000 docksible-0.3.0/src/docksible/project/setup-docker-compose.yml
--rw-rw-r--   0 brian     (1000) brian     (1000)      117 2024-04-22 18:30:44.000000 docksible-0.3.0/src/docksible/project/wordpress.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-22 18:32:58.077164 docksible-0.3.0/src/docksible.egg-info/
--rw-r--r--   0 brian     (1000) brian     (1000)     1225 2024-04-22 18:32:58.000000 docksible-0.3.0/src/docksible.egg-info/PKG-INFO
--rw-rw-r--   0 brian     (1000) brian     (1000)     3554 2024-04-22 18:32:58.000000 docksible-0.3.0/src/docksible.egg-info/SOURCES.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)        1 2024-04-22 18:32:58.000000 docksible-0.3.0/src/docksible.egg-info/dependency_links.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)       55 2024-04-22 18:32:58.000000 docksible-0.3.0/src/docksible.egg-info/entry_points.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)       33 2024-04-22 18:32:58.000000 docksible-0.3.0/src/docksible.egg-info/requires.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)       10 2024-04-22 18:32:58.000000 docksible-0.3.0/src/docksible.egg-info/top_level.txt
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-09 16:13:41.250191 docksible-0.4.0/
+-rw-rw-r--   0 brian     (1000) brian     (1000)       40 2024-05-09 16:11:35.000000 docksible-0.4.0/.gitignore
+-rw-rw-r--   0 brian     (1000) brian     (1000)      603 2024-05-09 16:11:35.000000 docksible-0.4.0/LICENSE.txt
+-rw-r--r--   0 brian     (1000) brian     (1000)     1225 2024-05-09 16:13:41.250191 docksible-0.4.0/PKG-INFO
+-rw-rw-r--   0 brian     (1000) brian     (1000)      349 2024-05-09 16:11:35.000000 docksible-0.4.0/README.md
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-09 16:13:41.238191 docksible-0.4.0/_DEPRECATED_ansible/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      109 2024-05-09 16:11:35.000000 docksible-0.4.0/_DEPRECATED_ansible/django.yml
+-rw-rw-r--   0 brian     (1000) brian     (1000)       73 2024-05-09 16:11:35.000000 docksible-0.4.0/_DEPRECATED_ansible/hosts
+-rw-rw-r--   0 brian     (1000) brian     (1000)       68 2024-05-09 16:11:35.000000 docksible-0.4.0/_DEPRECATED_ansible/letsencrypt.yml
+-rw-rw-r--   0 brian     (1000) brian     (1000)       93 2024-05-09 16:11:35.000000 docksible-0.4.0/_DEPRECATED_ansible/playbook.yml
+-rw-rw-r--   0 brian     (1000) brian     (1000)      175 2024-05-09 16:11:35.000000 docksible-0.4.0/_DEPRECATED_ansible/readme.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)       86 2024-05-09 16:11:35.000000 docksible-0.4.0/_DEPRECATED_ansible/redmine.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-09 16:13:41.234191 docksible-0.4.0/_DEPRECATED_ansible/roles/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-09 16:13:41.234191 docksible-0.4.0/_DEPRECATED_ansible/roles/build-image/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-09 16:13:41.238191 docksible-0.4.0/_DEPRECATED_ansible/roles/build-image/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      562 2024-05-09 16:11:35.000000 docksible-0.4.0/_DEPRECATED_ansible/roles/build-image/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-09 16:13:41.234191 docksible-0.4.0/_DEPRECATED_ansible/roles/django/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-09 16:13:41.238191 docksible-0.4.0/_DEPRECATED_ansible/roles/django/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1142 2024-05-09 16:11:35.000000 docksible-0.4.0/_DEPRECATED_ansible/roles/django/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-09 16:13:41.238191 docksible-0.4.0/_DEPRECATED_ansible/roles/django/templates/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      154 2024-05-09 16:11:35.000000 docksible-0.4.0/_DEPRECATED_ansible/roles/django/templates/.env
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1822 2024-05-09 16:11:35.000000 docksible-0.4.0/_DEPRECATED_ansible/roles/django/templates/docker-compose-django.yml.j2
+-rw-rw-r--   0 brian     (1000) brian     (1000)      688 2024-05-09 16:11:35.000000 docksible-0.4.0/_DEPRECATED_ansible/roles/django/templates/nginx.conf.j2
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-09 16:13:41.234191 docksible-0.4.0/_DEPRECATED_ansible/roles/docker-compose/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-09 16:13:41.242191 docksible-0.4.0/_DEPRECATED_ansible/roles/docker-compose/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1608 2024-05-09 16:11:35.000000 docksible-0.4.0/_DEPRECATED_ansible/roles/docker-compose/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-09 16:13:41.242191 docksible-0.4.0/_DEPRECATED_ansible/roles/docker-compose/templates/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      126 2024-05-09 16:11:35.000000 docksible-0.4.0/_DEPRECATED_ansible/roles/docker-compose/templates/.env
+-rw-rw-r--   0 brian     (1000) brian     (1000)     2222 2024-05-09 16:11:35.000000 docksible-0.4.0/_DEPRECATED_ansible/roles/docker-compose/templates/docker-compose.yml.j2
+-rw-rw-r--   0 brian     (1000) brian     (1000)      389 2024-05-09 16:11:35.000000 docksible-0.4.0/_DEPRECATED_ansible/roles/docker-compose/templates/nginx.conf.j2
+-rw-rw-r--   0 brian     (1000) brian     (1000)      795 2024-05-09 16:11:35.000000 docksible-0.4.0/_DEPRECATED_ansible/roles/docker-compose/templates/nginx.conf.j2.todo
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-09 16:13:41.234191 docksible-0.4.0/_DEPRECATED_ansible/roles/letsencrypt/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-09 16:13:41.242191 docksible-0.4.0/_DEPRECATED_ansible/roles/letsencrypt/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     3296 2024-05-09 16:11:35.000000 docksible-0.4.0/_DEPRECATED_ansible/roles/letsencrypt/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-09 16:13:41.242191 docksible-0.4.0/_DEPRECATED_ansible/roles/letsencrypt/templates/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      984 2024-05-09 16:11:35.000000 docksible-0.4.0/_DEPRECATED_ansible/roles/letsencrypt/templates/docker-compose-certbot-django.yml.j2
+-rw-rw-r--   0 brian     (1000) brian     (1000)      839 2024-05-09 16:11:35.000000 docksible-0.4.0/_DEPRECATED_ansible/roles/letsencrypt/templates/docker-compose-certbot-no-www.yml.j2
+-rw-rw-r--   0 brian     (1000) brian     (1000)      859 2024-05-09 16:11:35.000000 docksible-0.4.0/_DEPRECATED_ansible/roles/letsencrypt/templates/docker-compose-certbot.yml.j2
+-rw-rw-r--   0 brian     (1000) brian     (1000)      397 2024-05-09 16:11:35.000000 docksible-0.4.0/_DEPRECATED_ansible/roles/letsencrypt/templates/nginx.conf.1.j2
+-rw-rw-r--   0 brian     (1000) brian     (1000)      990 2024-05-09 16:11:35.000000 docksible-0.4.0/_DEPRECATED_ansible/roles/letsencrypt/templates/nginx.conf.django.j2
+-rw-rw-r--   0 brian     (1000) brian     (1000)      749 2024-05-09 16:11:35.000000 docksible-0.4.0/_DEPRECATED_ansible/roles/letsencrypt/templates/nginx.conf.j2
+-rw-rw-r--   0 brian     (1000) brian     (1000)     5585 2024-05-09 16:11:35.000000 docksible-0.4.0/_DEPRECATED_ansible/roles/letsencrypt/templates/wp-config.php
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-09 16:13:41.234191 docksible-0.4.0/_DEPRECATED_ansible/roles/redmine/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-09 16:13:41.242191 docksible-0.4.0/_DEPRECATED_ansible/roles/redmine/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1027 2024-05-09 16:11:35.000000 docksible-0.4.0/_DEPRECATED_ansible/roles/redmine/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-09 16:13:41.242191 docksible-0.4.0/_DEPRECATED_ansible/roles/redmine/templates/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1251 2024-05-09 16:11:35.000000 docksible-0.4.0/_DEPRECATED_ansible/roles/redmine/templates/docker-compose-redmine.yml.j2
+-rw-rw-r--   0 brian     (1000) brian     (1000)      389 2024-05-09 16:11:35.000000 docksible-0.4.0/_DEPRECATED_ansible/roles/redmine/templates/nginx.conf.j2
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-09 16:13:41.234191 docksible-0.4.0/_DEPRECATED_ansible/roles/ssh-proxy/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-09 16:13:41.242191 docksible-0.4.0/_DEPRECATED_ansible/roles/ssh-proxy/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      165 2024-05-09 16:11:35.000000 docksible-0.4.0/_DEPRECATED_ansible/roles/ssh-proxy/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-09 16:13:41.234191 docksible-0.4.0/_DEPRECATED_ansible/roles/ssl-selfsigned/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-09 16:13:41.242191 docksible-0.4.0/_DEPRECATED_ansible/roles/ssl-selfsigned/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     2408 2024-05-09 16:11:35.000000 docksible-0.4.0/_DEPRECATED_ansible/roles/ssl-selfsigned/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-09 16:13:41.242191 docksible-0.4.0/_DEPRECATED_ansible/roles/ssl-selfsigned/templates/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      609 2024-05-09 16:11:35.000000 docksible-0.4.0/_DEPRECATED_ansible/roles/ssl-selfsigned/templates/nginx.conf.j2
+-rw-rw-r--   0 brian     (1000) brian     (1000)      126 2024-05-09 16:11:35.000000 docksible-0.4.0/_DEPRECATED_ansible/roles/ssl-selfsigned/templates/self-signed.conf
+-rw-rw-r--   0 brian     (1000) brian     (1000)      860 2024-05-09 16:11:35.000000 docksible-0.4.0/_DEPRECATED_ansible/roles/ssl-selfsigned/templates/ssl-params.conf
+-rw-rw-r--   0 brian     (1000) brian     (1000)     5585 2024-05-09 16:11:35.000000 docksible-0.4.0/_DEPRECATED_ansible/roles/ssl-selfsigned/templates/wp-config.php
+-rw-rw-r--   0 brian     (1000) brian     (1000)       71 2024-05-09 16:11:35.000000 docksible-0.4.0/_DEPRECATED_ansible/ssl-selfsigned.yml
+-rw-rw-r--   0 brian     (1000) brian     (1000)    70933 2024-05-09 16:11:35.000000 docksible-0.4.0/_DEPRECATED_redmine_defaults.sql
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1169 2024-05-09 16:11:35.000000 docksible-0.4.0/pyproject.toml
+-rw-rw-r--   0 brian     (1000) brian     (1000)       38 2024-05-09 16:13:41.250191 docksible-0.4.0/setup.cfg
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-09 16:13:41.238191 docksible-0.4.0/src/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-09 16:13:41.242191 docksible-0.4.0/src/docksible/
+-rw-rw-r--   0 brian     (1000) brian     (1000)    10726 2024-05-09 16:11:35.000000 docksible-0.4.0/src/docksible/arg_validator.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)      303 2024-05-09 16:11:35.000000 docksible-0.4.0/src/docksible/constants.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    11164 2024-05-09 16:11:35.000000 docksible-0.4.0/src/docksible/docksible.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-09 16:13:41.246191 docksible-0.4.0/src/docksible/project/
+-rw-rw-r--   0 brian     (1000) brian     (1000)       61 2024-05-09 16:11:35.000000 docksible-0.4.0/src/docksible/project/letsencrypt.yml
+-rw-rw-r--   0 brian     (1000) brian     (1000)      115 2024-05-09 16:11:35.000000 docksible-0.4.0/src/docksible/project/redmine.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-09 16:13:41.238191 docksible-0.4.0/src/docksible/project/roles/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-09 16:13:41.238191 docksible-0.4.0/src/docksible/project/roles/letsencrypt/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-09 16:13:41.246191 docksible-0.4.0/src/docksible/project/roles/letsencrypt/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     3260 2024-05-09 16:11:35.000000 docksible-0.4.0/src/docksible/project/roles/letsencrypt/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-09 16:13:41.246191 docksible-0.4.0/src/docksible/project/roles/letsencrypt/templates/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1003 2024-05-09 16:11:35.000000 docksible-0.4.0/src/docksible/project/roles/letsencrypt/templates/docker-compose-certbot-django.yml.j2
+-rw-rw-r--   0 brian     (1000) brian     (1000)      854 2024-05-09 16:11:35.000000 docksible-0.4.0/src/docksible/project/roles/letsencrypt/templates/docker-compose-certbot-no-www.yml.j2
+-rw-rw-r--   0 brian     (1000) brian     (1000)      874 2024-05-09 16:11:35.000000 docksible-0.4.0/src/docksible/project/roles/letsencrypt/templates/docker-compose-certbot.yml.j2
+-rw-rw-r--   0 brian     (1000) brian     (1000)      427 2024-05-09 16:11:35.000000 docksible-0.4.0/src/docksible/project/roles/letsencrypt/templates/nginx.conf.1.j2
+-rw-rw-r--   0 brian     (1000) brian     (1000)      947 2024-05-09 16:11:35.000000 docksible-0.4.0/src/docksible/project/roles/letsencrypt/templates/nginx.conf.django.j2
+-rw-rw-r--   0 brian     (1000) brian     (1000)      728 2024-05-09 16:11:35.000000 docksible-0.4.0/src/docksible/project/roles/letsencrypt/templates/nginx.conf.j2
+-rw-rw-r--   0 brian     (1000) brian     (1000)     5646 2024-05-09 16:11:35.000000 docksible-0.4.0/src/docksible/project/roles/letsencrypt/templates/wp-config.php
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-09 16:13:41.238191 docksible-0.4.0/src/docksible/project/roles/redmine/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-09 16:13:41.246191 docksible-0.4.0/src/docksible/project/roles/redmine/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1056 2024-05-09 16:11:35.000000 docksible-0.4.0/src/docksible/project/roles/redmine/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-09 16:13:41.246191 docksible-0.4.0/src/docksible/project/roles/redmine/templates/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1353 2024-05-09 16:11:35.000000 docksible-0.4.0/src/docksible/project/roles/redmine/templates/docker-compose-redmine.yml.j2
+-rw-rw-r--   0 brian     (1000) brian     (1000)      386 2024-05-09 16:11:35.000000 docksible-0.4.0/src/docksible/project/roles/redmine/templates/nginx.conf.j2
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-09 16:13:41.238191 docksible-0.4.0/src/docksible/project/roles/setup-docker-compose/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-09 16:13:41.250191 docksible-0.4.0/src/docksible/project/roles/setup-docker-compose/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1171 2024-05-09 16:11:35.000000 docksible-0.4.0/src/docksible/project/roles/setup-docker-compose/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-09 16:13:41.238191 docksible-0.4.0/src/docksible/project/roles/ssh-proxy/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-09 16:13:41.250191 docksible-0.4.0/src/docksible/project/roles/ssh-proxy/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      200 2024-05-09 16:11:35.000000 docksible-0.4.0/src/docksible/project/roles/ssh-proxy/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-09 16:13:41.238191 docksible-0.4.0/src/docksible/project/roles/wordpress/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-09 16:13:41.250191 docksible-0.4.0/src/docksible/project/roles/wordpress/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1068 2024-05-09 16:11:35.000000 docksible-0.4.0/src/docksible/project/roles/wordpress/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-09 16:13:41.250191 docksible-0.4.0/src/docksible/project/roles/wordpress/templates/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1787 2024-05-09 16:11:35.000000 docksible-0.4.0/src/docksible/project/roles/wordpress/templates/docker-compose-wordpress.yml.j2
+-rw-rw-r--   0 brian     (1000) brian     (1000)      446 2024-05-09 16:11:35.000000 docksible-0.4.0/src/docksible/project/roles/wordpress/templates/nginx.conf.j2
+-rw-rw-r--   0 brian     (1000) brian     (1000)       85 2024-05-09 16:11:35.000000 docksible-0.4.0/src/docksible/project/setup-docker-compose.yml
+-rw-rw-r--   0 brian     (1000) brian     (1000)      117 2024-05-09 16:11:35.000000 docksible-0.4.0/src/docksible/project/wordpress.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-05-09 16:13:41.250191 docksible-0.4.0/src/docksible.egg-info/
+-rw-r--r--   0 brian     (1000) brian     (1000)     1225 2024-05-09 16:13:41.000000 docksible-0.4.0/src/docksible.egg-info/PKG-INFO
+-rw-rw-r--   0 brian     (1000) brian     (1000)     3554 2024-05-09 16:13:41.000000 docksible-0.4.0/src/docksible.egg-info/SOURCES.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)        1 2024-05-09 16:13:41.000000 docksible-0.4.0/src/docksible.egg-info/dependency_links.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)       55 2024-05-09 16:13:41.000000 docksible-0.4.0/src/docksible.egg-info/entry_points.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)       33 2024-05-09 16:13:41.000000 docksible-0.4.0/src/docksible.egg-info/requires.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)       10 2024-05-09 16:13:41.000000 docksible-0.4.0/src/docksible.egg-info/top_level.txt
```

### Comparing `docksible-0.3.0/LICENSE.txt` & `docksible-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `docksible-0.3.0/PKG-INFO` & `docksible-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docksible
-Version: 0.3.0
+Version: 0.4.0
 Summary: Deploy and set up Docker Compose based web apps with Ansible
 Author-email: "Brian St. Hilaire" <brian.st-hilaire@sanctus-tech.com>
 Project-URL: Homepage, https://github.com/saint-hilaire/docksible
 Project-URL: Issues, https://github.com/saint-hilaire/docksible/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Framework :: Ansible
```

### Comparing `docksible-0.3.0/_DEPRECATED_ansible/roles/build-image/tasks/main.yml` & `docksible-0.4.0/_DEPRECATED_ansible/roles/build-image/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `docksible-0.3.0/_DEPRECATED_ansible/roles/django/tasks/main.yml` & `docksible-0.4.0/_DEPRECATED_ansible/roles/django/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `docksible-0.3.0/_DEPRECATED_ansible/roles/django/templates/docker-compose-django.yml.j2` & `docksible-0.4.0/_DEPRECATED_ansible/roles/django/templates/docker-compose-django.yml.j2`

 * *Files identical despite different names*

### Comparing `docksible-0.3.0/_DEPRECATED_ansible/roles/django/templates/nginx.conf.j2` & `docksible-0.4.0/_DEPRECATED_ansible/roles/django/templates/nginx.conf.j2`

 * *Files identical despite different names*

### Comparing `docksible-0.3.0/_DEPRECATED_ansible/roles/docker-compose/tasks/main.yml` & `docksible-0.4.0/_DEPRECATED_ansible/roles/docker-compose/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `docksible-0.3.0/_DEPRECATED_ansible/roles/docker-compose/templates/docker-compose.yml.j2` & `docksible-0.4.0/_DEPRECATED_ansible/roles/docker-compose/templates/docker-compose.yml.j2`

 * *Files identical despite different names*

### Comparing `docksible-0.3.0/_DEPRECATED_ansible/roles/docker-compose/templates/nginx.conf.j2.todo` & `docksible-0.4.0/_DEPRECATED_ansible/roles/docker-compose/templates/nginx.conf.j2.todo`

 * *Files identical despite different names*

### Comparing `docksible-0.3.0/_DEPRECATED_ansible/roles/letsencrypt/tasks/main.yml` & `docksible-0.4.0/_DEPRECATED_ansible/roles/letsencrypt/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `docksible-0.3.0/_DEPRECATED_ansible/roles/letsencrypt/templates/docker-compose-certbot-django.yml.j2` & `docksible-0.4.0/_DEPRECATED_ansible/roles/letsencrypt/templates/docker-compose-certbot-django.yml.j2`

 * *Files identical despite different names*

### Comparing `docksible-0.3.0/_DEPRECATED_ansible/roles/letsencrypt/templates/docker-compose-certbot-no-www.yml.j2` & `docksible-0.4.0/_DEPRECATED_ansible/roles/letsencrypt/templates/docker-compose-certbot-no-www.yml.j2`

 * *Files identical despite different names*

### Comparing `docksible-0.3.0/_DEPRECATED_ansible/roles/letsencrypt/templates/docker-compose-certbot.yml.j2` & `docksible-0.4.0/_DEPRECATED_ansible/roles/letsencrypt/templates/docker-compose-certbot.yml.j2`

 * *Files identical despite different names*

### Comparing `docksible-0.3.0/_DEPRECATED_ansible/roles/letsencrypt/templates/nginx.conf.django.j2` & `docksible-0.4.0/_DEPRECATED_ansible/roles/letsencrypt/templates/nginx.conf.django.j2`

 * *Files identical despite different names*

### Comparing `docksible-0.3.0/_DEPRECATED_ansible/roles/letsencrypt/templates/nginx.conf.j2` & `docksible-0.4.0/_DEPRECATED_ansible/roles/letsencrypt/templates/nginx.conf.j2`

 * *Files identical despite different names*

### Comparing `docksible-0.3.0/_DEPRECATED_ansible/roles/letsencrypt/templates/wp-config.php` & `docksible-0.4.0/_DEPRECATED_ansible/roles/letsencrypt/templates/wp-config.php`

 * *Files identical despite different names*

### Comparing `docksible-0.3.0/_DEPRECATED_ansible/roles/redmine/tasks/main.yml` & `docksible-0.4.0/_DEPRECATED_ansible/roles/redmine/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `docksible-0.3.0/_DEPRECATED_ansible/roles/redmine/templates/docker-compose-redmine.yml.j2` & `docksible-0.4.0/_DEPRECATED_ansible/roles/redmine/templates/docker-compose-redmine.yml.j2`

 * *Files identical despite different names*

### Comparing `docksible-0.3.0/_DEPRECATED_ansible/roles/ssl-selfsigned/tasks/main.yml` & `docksible-0.4.0/_DEPRECATED_ansible/roles/ssl-selfsigned/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `docksible-0.3.0/_DEPRECATED_ansible/roles/ssl-selfsigned/templates/nginx.conf.j2` & `docksible-0.4.0/_DEPRECATED_ansible/roles/ssl-selfsigned/templates/nginx.conf.j2`

 * *Files identical despite different names*

### Comparing `docksible-0.3.0/_DEPRECATED_ansible/roles/ssl-selfsigned/templates/ssl-params.conf` & `docksible-0.4.0/_DEPRECATED_ansible/roles/ssl-selfsigned/templates/ssl-params.conf`

 * *Files identical despite different names*

### Comparing `docksible-0.3.0/_DEPRECATED_ansible/roles/ssl-selfsigned/templates/wp-config.php` & `docksible-0.4.0/_DEPRECATED_ansible/roles/ssl-selfsigned/templates/wp-config.php`

 * *Files identical despite different names*

### Comparing `docksible-0.3.0/_DEPRECATED_redmine_defaults.sql` & `docksible-0.4.0/_DEPRECATED_redmine_defaults.sql`

 * *Files identical despite different names*

### Comparing `docksible-0.3.0/pyproject.toml` & `docksible-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=69.0",
     "setuptools-scm>=8.0"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "docksible"
-version = "0.3.0"
+version = "0.4.0"
 authors = [
     {name="Brian St. Hilaire", email="brian.st-hilaire@sanctus-tech.com"}
 ]
 description = "Deploy and set up Docker Compose based web apps with Ansible"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
```

### Comparing `docksible-0.3.0/src/docksible/arg_validator.py` & `docksible-0.4.0/src/docksible/arg_validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,14 +221,28 @@
 
             self.args.database_root_password = self.get_pass_and_check(
                 'Please enter a database root password: ',
                 0,
                 True
             )
 
+        if self.args.action == 'backup':
+            self.handle_defaults([
+                {
+                    'arg_name': 'database_name',
+                    'cli_default_value': None,
+                    'override_default_value': DEFAULT_DATABASE_NAME,
+                },
+                {
+                    'arg_name': 'database_username',
+                    'cli_default_value': None,
+                    'override_default_value': DEFAULT_DATABASE_USERNAME,
+                },
+            ], True, True)
+
         if self.args.database_username and not self.args.database_password:
             self.args.database_password = self.get_pass_and_check(
                 'Please enter a database password: ',
                 0,
                 True
             )
```

### Comparing `docksible-0.3.0/src/docksible/project/roles/letsencrypt/tasks/main.yml` & `docksible-0.4.0/src/docksible/project/roles/letsencrypt/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `docksible-0.3.0/src/docksible/project/roles/letsencrypt/templates/docker-compose-certbot-django.yml.j2` & `docksible-0.4.0/src/docksible/project/roles/letsencrypt/templates/docker-compose-certbot-django.yml.j2`

 * *Files identical despite different names*

### Comparing `docksible-0.3.0/src/docksible/project/roles/letsencrypt/templates/docker-compose-certbot-no-www.yml.j2` & `docksible-0.4.0/src/docksible/project/roles/letsencrypt/templates/docker-compose-certbot-no-www.yml.j2`

 * *Files identical despite different names*

### Comparing `docksible-0.3.0/src/docksible/project/roles/letsencrypt/templates/docker-compose-certbot.yml.j2` & `docksible-0.4.0/src/docksible/project/roles/letsencrypt/templates/docker-compose-certbot.yml.j2`

 * *Files identical despite different names*

### Comparing `docksible-0.3.0/src/docksible/project/roles/letsencrypt/templates/nginx.conf.django.j2` & `docksible-0.4.0/src/docksible/project/roles/letsencrypt/templates/nginx.conf.django.j2`

 * *Files identical despite different names*

### Comparing `docksible-0.3.0/src/docksible/project/roles/letsencrypt/templates/nginx.conf.j2` & `docksible-0.4.0/src/docksible/project/roles/letsencrypt/templates/nginx.conf.j2`

 * *Files 14% similar despite different names*

```diff
@@ -15,9 +15,10 @@
     }
     ssl_certificate /etc/letsencrypt/live/{{ domain }}/fullchain.pem;
     ssl_certificate_key /etc/letsencrypt/live/{{ domain }}/privkey.pem;
     location / {
         proxy_pass  http://docksible_{{ service_to_encrypt }}:{{ port_to_encrypt }};
         proxy_set_header Host      $host;
         proxy_set_header X-Real-IP $remote_addr;
+        proxy_set_header X-Forwarded-Proto $scheme;
     }
 }
```

### Comparing `docksible-0.3.0/src/docksible/project/roles/letsencrypt/templates/wp-config.php` & `docksible-0.4.0/src/docksible/project/roles/letsencrypt/templates/wp-config.php`

 * *Files identical despite different names*

### Comparing `docksible-0.3.0/src/docksible/project/roles/redmine/tasks/main.yml` & `docksible-0.4.0/src/docksible/project/roles/redmine/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `docksible-0.3.0/src/docksible/project/roles/redmine/templates/docker-compose-redmine.yml.j2` & `docksible-0.4.0/src/docksible/project/roles/redmine/templates/docker-compose-redmine.yml.j2`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     environment:
       REDMINE_DB_MYSQL: docksible_db
       REDMINE_DB_PASSWORD: "{{ database_root_password }}"
     security_opt:
       - seccomp:unconfined
 
   docksible_db:
-    image: mysql:latest
+    image: mysql:8.3
     container_name: docksible_db
     restart: always
     environment:
       MYSQL_ROOT_PASSWORD: "{{ database_root_password }}"
       MYSQL_DATABASE: redmine
     volumes:
       - "$HOME/docksible-volumes/db_data:/var/lib/mysql"
```

### Comparing `docksible-0.3.0/src/docksible/project/roles/setup-docker-compose/tasks/main.yml` & `docksible-0.4.0/src/docksible/project/roles/setup-docker-compose/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `docksible-0.3.0/src/docksible/project/roles/wordpress/tasks/main.yml` & `docksible-0.4.0/src/docksible/project/roles/wordpress/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `docksible-0.3.0/src/docksible/project/roles/wordpress/templates/docker-compose-wordpress.yml.j2` & `docksible-0.4.0/src/docksible/project/roles/wordpress/templates/docker-compose-wordpress.yml.j2`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 version: "3.3"
     
 services:
 
   docksible_db:
-    image: mysql:8.0
+    image: mysql:8.3
     container_name: docksible_db
     volumes:
       - "$HOME/docksible-volumes/db_data:/var/lib/mysql"
     restart: unless-stopped
     environment:
       - "MYSQL_ROOT_PASSWORD={{ database_root_password }}"
       - "MYSQL_USER={{ database_username }}"
```

### Comparing `docksible-0.3.0/src/docksible.egg-info/PKG-INFO` & `docksible-0.4.0/src/docksible.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docksible
-Version: 0.3.0
+Version: 0.4.0
 Summary: Deploy and set up Docker Compose based web apps with Ansible
 Author-email: "Brian St. Hilaire" <brian.st-hilaire@sanctus-tech.com>
 Project-URL: Homepage, https://github.com/saint-hilaire/docksible
 Project-URL: Issues, https://github.com/saint-hilaire/docksible/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Framework :: Ansible
```

### Comparing `docksible-0.3.0/src/docksible.egg-info/SOURCES.txt` & `docksible-0.4.0/src/docksible.egg-info/SOURCES.txt`

 * *Files identical despite different names*

