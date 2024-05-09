# Comparing `tmp/shadowsocks_manager-0.1.5.tar.gz` & `tmp/shadowsocks_manager-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shadowsocks_manager-0.1.5.tar", last modified: Mon May  6 05:00:24 2024, max compression
+gzip compressed data, was "shadowsocks_manager-0.1.6.tar", last modified: Thu May  9 15:53:32 2024, max compression
```

## Comparing `shadowsocks_manager-0.1.5.tar` & `shadowsocks_manager-0.1.6.tar`

### file list

```diff
@@ -1,123 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.388720 shadowsocks_manager-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    21139 2024-05-06 05:00:24.388720 shadowsocks_manager-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16718 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.372721 shadowsocks_manager-0.1.5/bin/
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/bin/ssm-dev-start
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/bin/ssm-dev-stop
--rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/bin/ssm-setup
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/bin/ssm-test
--rw-r--r--   0 runner    (1001) docker     (127)     6313 2024-05-06 05:00:20.000000 shadowsocks_manager-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-06 05:00:24.392721 shadowsocks_manager-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.372721 shadowsocks_manager-0.1.5/shadowsocks_manager/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.376721 shadowsocks_manager-0.1.5/shadowsocks_manager/args_formatter/
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/args_formatter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/args_formatter/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.376721 shadowsocks_manager-0.1.5/shadowsocks_manager/domain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/domain/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/domain/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.376721 shadowsocks_manager-0.1.5/shadowsocks_manager/domain/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/domain/fixtures/nameserver.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.376721 shadowsocks_manager-0.1.5/shadowsocks_manager/domain/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/domain/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8433 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/domain/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/domain/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/domain/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/domain/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/domain/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.376721 shadowsocks_manager-0.1.5/shadowsocks_manager/dynamicmethod/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/dynamicmethod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/dynamicmethod/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/dynamicmethod/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.380720 shadowsocks_manager-0.1.5/shadowsocks_manager/dynamicmethod/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/dynamicmethod/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/dynamicmethod/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/dynamicmethod/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/dynamicmethod/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.380720 shadowsocks_manager-0.1.5/shadowsocks_manager/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/fixtures/auth.group.json
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/fixtures/django_celery_beat.crontabschedule.json
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/fixtures/django_celery_beat.intervalschedule.json
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/fixtures/django_celery_beat.periodictask.json
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/fixtures/sites.site.json
--rwxr-xr-x   0 runner    (1001) docker     (127)      940 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.380720 shadowsocks_manager-0.1.5/shadowsocks_manager/notification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/notification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/notification/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/notification/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.380720 shadowsocks_manager-0.1.5/shadowsocks_manager/notification/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/notification/fixtures/template.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.380720 shadowsocks_manager-0.1.5/shadowsocks_manager/notification/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/notification/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/notification/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/notification/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/notification/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/notification/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/notification/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.380720 shadowsocks_manager-0.1.5/shadowsocks_manager/retry/
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/retry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/retry/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.384720 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6083 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.384720 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/fixtures/config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.384720 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.384720 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/management/commands/shadowsocks_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.384720 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36237 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)    21055 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.384720 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks_manager/celery.py
--rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks_manager/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks_manager/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks_manager/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.384720 shadowsocks_manager-0.1.5/shadowsocks_manager/singleton/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/singleton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/singleton/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/singleton/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.384720 shadowsocks_manager-0.1.5/shadowsocks_manager/singleton/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/singleton/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/singleton/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/singleton/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/singleton/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.388720 shadowsocks_manager-0.1.5/shadowsocks_manager/statistic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/statistic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/statistic/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/statistic/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.388720 shadowsocks_manager-0.1.5/shadowsocks_manager/statistic/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/statistic/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/statistic/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/statistic/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/statistic/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/statistic/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/statistic/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/statistic/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.388720 shadowsocks_manager-0.1.5/shadowsocks_manager/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/utils/celery.py
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/utils/createsuperuser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/utils/dotenv.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/utils/manage.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-06 05:00:08.000000 shadowsocks_manager-0.1.5/shadowsocks_manager/utils/uwsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:00:24.388720 shadowsocks_manager-0.1.5/shadowsocks_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21139 2024-05-06 05:00:24.000000 shadowsocks_manager-0.1.5/shadowsocks_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-06 05:00:24.000000 shadowsocks_manager-0.1.5/shadowsocks_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 05:00:24.000000 shadowsocks_manager-0.1.5/shadowsocks_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-06 05:00:24.000000 shadowsocks_manager-0.1.5/shadowsocks_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-06 05:00:24.000000 shadowsocks_manager-0.1.5/shadowsocks_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-06 05:00:24.000000 shadowsocks_manager-0.1.5/shadowsocks_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:53:32.529014 shadowsocks_manager-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    21317 2024-05-09 15:53:32.529014 shadowsocks_manager-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16896 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:53:32.513014 shadowsocks_manager-0.1.6/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/bin/ssm-dev-start
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/bin/ssm-dev-stop
+-rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/bin/ssm-setup
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/bin/ssm-test
+-rw-r--r--   0 runner    (1001) docker     (127)     6313 2024-05-09 15:53:25.000000 shadowsocks_manager-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-09 15:53:32.529014 shadowsocks_manager-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:53:32.513014 shadowsocks_manager-0.1.6/shadowsocks_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:53:32.513014 shadowsocks_manager-0.1.6/shadowsocks_manager/args_formatter/
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/args_formatter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/args_formatter/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:53:32.513014 shadowsocks_manager-0.1.6/shadowsocks_manager/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/domain/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/domain/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:53:32.513014 shadowsocks_manager-0.1.6/shadowsocks_manager/domain/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/domain/fixtures/nameserver.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:53:32.517014 shadowsocks_manager-0.1.6/shadowsocks_manager/domain/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/domain/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8433 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/domain/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/domain/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/domain/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/domain/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/domain/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:53:32.517014 shadowsocks_manager-0.1.6/shadowsocks_manager/dynamicmethod/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/dynamicmethod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/dynamicmethod/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/dynamicmethod/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:53:32.517014 shadowsocks_manager-0.1.6/shadowsocks_manager/dynamicmethod/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/dynamicmethod/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/dynamicmethod/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/dynamicmethod/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/dynamicmethod/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:53:32.517014 shadowsocks_manager-0.1.6/shadowsocks_manager/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/fixtures/auth.group.json
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/fixtures/django_celery_beat.crontabschedule.json
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/fixtures/django_celery_beat.intervalschedule.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/fixtures/django_celery_beat.periodictask.json
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/fixtures/sites.site.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)      940 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:53:32.517014 shadowsocks_manager-0.1.6/shadowsocks_manager/notification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/notification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/notification/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/notification/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:53:32.517014 shadowsocks_manager-0.1.6/shadowsocks_manager/notification/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/notification/fixtures/template-txt-to-json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/notification/fixtures/template.json
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/notification/fixtures/template.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:53:32.517014 shadowsocks_manager-0.1.6/shadowsocks_manager/notification/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/notification/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/notification/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/notification/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/notification/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/notification/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/notification/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:53:32.521014 shadowsocks_manager-0.1.6/shadowsocks_manager/retry/
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/retry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/retry/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:53:32.521014 shadowsocks_manager-0.1.6/shadowsocks_manager/shadowsocks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/shadowsocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/shadowsocks/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/shadowsocks/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:53:32.521014 shadowsocks_manager-0.1.6/shadowsocks_manager/shadowsocks/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/shadowsocks/fixtures/config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:53:32.521014 shadowsocks_manager-0.1.6/shadowsocks_manager/shadowsocks/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/shadowsocks/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:53:32.521014 shadowsocks_manager-0.1.6/shadowsocks_manager/shadowsocks/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/shadowsocks/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/shadowsocks/management/commands/shadowsocks_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:53:32.521014 shadowsocks_manager-0.1.6/shadowsocks_manager/shadowsocks/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/shadowsocks/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36237 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/shadowsocks/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/shadowsocks/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/shadowsocks/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21055 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/shadowsocks/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/shadowsocks/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/shadowsocks/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:53:32.521014 shadowsocks_manager-0.1.6/shadowsocks_manager/shadowsocks_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/shadowsocks_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/shadowsocks_manager/celery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/shadowsocks_manager/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/shadowsocks_manager/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/shadowsocks_manager/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:53:32.525014 shadowsocks_manager-0.1.6/shadowsocks_manager/singleton/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/singleton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/singleton/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/singleton/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:53:32.525014 shadowsocks_manager-0.1.6/shadowsocks_manager/singleton/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/singleton/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/singleton/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/singleton/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/singleton/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:53:32.525014 shadowsocks_manager-0.1.6/shadowsocks_manager/statistic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/statistic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/statistic/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/statistic/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:53:32.525014 shadowsocks_manager-0.1.6/shadowsocks_manager/statistic/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/statistic/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/statistic/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/statistic/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/statistic/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/statistic/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/statistic/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/statistic/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:53:32.525014 shadowsocks_manager-0.1.6/shadowsocks_manager/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/utils/celery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/utils/createsuperuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/utils/dotenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/utils/manage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-09 15:52:59.000000 shadowsocks_manager-0.1.6/shadowsocks_manager/utils/uwsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:53:32.525014 shadowsocks_manager-0.1.6/shadowsocks_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21317 2024-05-09 15:53:32.000000 shadowsocks_manager-0.1.6/shadowsocks_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-05-09 15:53:32.000000 shadowsocks_manager-0.1.6/shadowsocks_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 15:53:32.000000 shadowsocks_manager-0.1.6/shadowsocks_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-09 15:53:32.000000 shadowsocks_manager-0.1.6/shadowsocks_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-09 15:53:32.000000 shadowsocks_manager-0.1.6/shadowsocks_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-09 15:53:32.000000 shadowsocks_manager-0.1.6/shadowsocks_manager.egg-info/top_level.txt
```

### Comparing `shadowsocks_manager-0.1.5/LICENSE` & `shadowsocks_manager-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.5/PKG-INFO` & `shadowsocks_manager-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shadowsocks-manager
-Version: 0.1.5
+Version: 0.1.6
 Summary: A shadowsocks manager for multi-user and traffic statistics
 Home-page: https://github.com/alexzhangs/shadowsocks-manager
 Author: Alex
 Author-email: Alex <alexzhangs@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Alex Zhang
@@ -133,20 +133,26 @@
         * ~~Pre-installed, and have a builtin service manager.~~
         * No builtin service manager, you need to install it and start the service by yourself.
 
 Code in Python, base on Django, Django REST framework, Celery, and SQLite.
 
 The development status can be found at: [project home](https://github.com/alexzhangs/shadowsocks-manager/projects/1).
 
+
+## Screenshots
+
 Shadowsocks Node List:
 ![Home › Shadowsocks › Shadowsocks Nodes](https://www.0xbeta.com/shadowsocks-manager/assets/images/shadowsocks-node-list.png)
 
 Add Shadowsocks Node:
 ![Home › Shadowsocks › Shadowsocks Nodes](https://www.0xbeta.com/shadowsocks-manager/assets/images/shadowsocks-node-add.png)
 
+Add Shadowsocks Account:
+![Home › Shadowsocks › Shadowsocks Accounts](https://www.0xbeta.com/shadowsocks-manager/assets/images/shadowsocks-account-add.png)
+
 
 ## 1. Requirements
 
 * Python 2.7, Python 3.x
 * Django 1.11.x, Django 3.x
 * Docker
 * [Shadowsocks-libev 3.2.0 for Linux (multi-user API is required)](https://github.com/shadowsocks/shadowsocks-libev)
```

### Comparing `shadowsocks_manager-0.1.5/README.md` & `shadowsocks_manager-0.1.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -38,20 +38,26 @@
         * ~~Pre-installed, and have a builtin service manager.~~
         * No builtin service manager, you need to install it and start the service by yourself.
 
 Code in Python, base on Django, Django REST framework, Celery, and SQLite.
 
 The development status can be found at: [project home](https://github.com/alexzhangs/shadowsocks-manager/projects/1).
 
+
+## Screenshots
+
 Shadowsocks Node List:
 ![Home › Shadowsocks › Shadowsocks Nodes](https://www.0xbeta.com/shadowsocks-manager/assets/images/shadowsocks-node-list.png)
 
 Add Shadowsocks Node:
 ![Home › Shadowsocks › Shadowsocks Nodes](https://www.0xbeta.com/shadowsocks-manager/assets/images/shadowsocks-node-add.png)
 
+Add Shadowsocks Account:
+![Home › Shadowsocks › Shadowsocks Accounts](https://www.0xbeta.com/shadowsocks-manager/assets/images/shadowsocks-account-add.png)
+
 
 ## 1. Requirements
 
 * Python 2.7, Python 3.x
 * Django 1.11.x, Django 3.x
 * Docker
 * [Shadowsocks-libev 3.2.0 for Linux (multi-user API is required)](https://github.com/shadowsocks/shadowsocks-libev)
```

### Comparing `shadowsocks_manager-0.1.5/bin/ssm-dev-start` & `shadowsocks_manager-0.1.6/bin/ssm-dev-start`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.5/bin/ssm-setup` & `shadowsocks_manager-0.1.6/bin/ssm-setup`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.5/bin/ssm-test` & `shadowsocks_manager-0.1.6/bin/ssm-test`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.5/pyproject.toml` & `shadowsocks_manager-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "shadowsocks-manager"
-version = "0.1.5"
+version = "0.1.6"
 requires-python = ">=2.7"
 dependencies = [
     "future",
     "six",
     "boto3",
     "celery",
     "Django<4",
@@ -136,15 +136,15 @@
 [tool.setuptools.package-data]
 shadowsocks_manager = ["fixtures/*", "**/fixtures/*"]
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 [tool.bumpversion]
-current_version = "0.1.5"
+current_version = "0.1.6"
 parse = """
     (?P<major>\\d+)\\.
     (?P<minor>\\d+)\\.
     (?P<patch>\\d+)
     (
         \\-                         # separator
         (?P<suffix>[0-9]\\d*)       # suffix Number
```

### Comparing `shadowsocks_manager-0.1.5/setup.cfg` & `shadowsocks_manager-0.1.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = shadowsocks-manager
-version = 0.1.5
+version = 0.1.6
 description = A shadowsocks manager for multi-user and traffic statistics
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Alex
 author_email = alexzhangs@gmail.com
 url = https://github.com/alexzhangs/shadowsocks-manager
 license = MIT
```

### Comparing `shadowsocks_manager-0.1.5/shadowsocks_manager/__main__.py` & `shadowsocks_manager-0.1.6/shadowsocks_manager/__main__.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.5/shadowsocks_manager/args_formatter/__init__.py` & `shadowsocks_manager-0.1.6/shadowsocks_manager/args_formatter/__init__.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.5/shadowsocks_manager/args_formatter/tests.py` & `shadowsocks_manager-0.1.6/shadowsocks_manager/args_formatter/tests.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.5/shadowsocks_manager/domain/admin.py` & `shadowsocks_manager-0.1.6/shadowsocks_manager/domain/admin.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.5/shadowsocks_manager/domain/models.py` & `shadowsocks_manager-0.1.6/shadowsocks_manager/domain/models.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.5/shadowsocks_manager/domain/serializers.py` & `shadowsocks_manager-0.1.6/shadowsocks_manager/domain/serializers.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.5/shadowsocks_manager/domain/tests.py` & `shadowsocks_manager-0.1.6/shadowsocks_manager/domain/tests.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.5/shadowsocks_manager/domain/views.py` & `shadowsocks_manager-0.1.6/shadowsocks_manager/domain/views.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.5/shadowsocks_manager/dynamicmethod/models.py` & `shadowsocks_manager-0.1.6/shadowsocks_manager/dynamicmethod/models.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.5/shadowsocks_manager/fixtures/django_celery_beat.crontabschedule.json` & `shadowsocks_manager-0.1.6/shadowsocks_manager/fixtures/django_celery_beat.crontabschedule.json`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.5/shadowsocks_manager/fixtures/django_celery_beat.periodictask.json` & `shadowsocks_manager-0.1.6/shadowsocks_manager/fixtures/django_celery_beat.periodictask.json`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.5/shadowsocks_manager/manage.py` & `shadowsocks_manager-0.1.6/shadowsocks_manager/manage.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.5/shadowsocks_manager/notification/fixtures/template.json` & `shadowsocks_manager-0.1.6/shadowsocks_manager/notification/fixtures/template.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9833333333333334%*

 * *Differences: {'0': '{\'fields\': {\'content\': "Subject: CREDENTIAL: VPN Account (Shadowsocks)\\r\\nTo: {{ '*

 * *      'account.email }}\\r\\nDear {{ account.first_name }},\\r\\n\\r\\nYour VPN account is setup '*

 * *      'as below.\\r\\n\\r\\n* Port: {{ account.username }}\\r\\n* Password: {{ account.password '*

 * *      "}}\\r\\n\\r\\nIt's available on {{ node_accounts|length }} node(s):\\r\\n{% for obj in "*

 * *      'node_accounts %}\\r\\nNode #{{ forloop.counter }}:\\r\\n------\\r\\n{% ifchanged %}\\r\\n* '*

 * *      'VPN Server: {% i […]*

```diff
@@ -1,11 +1,11 @@
 [
     {
         "fields": {
-            "content": "Subject: CREDENTIAL: VPN Account (Shadowsocks)\r\nTo: {{ account.email }}\r\nDear {{ account.first_name }},\r\n\r\nYour VPN account is setup as below.\r\n\r\n* Port: {{ account.username }}\r\n* Password: {{ account.password }}\r\n\r\nIt's available on {{ node_accounts|length }} node(s):\r\n\r\n{% spaceless %}\r\n{% for obj in node_accounts %}\r\nNode #{{ forloop.counter }}:\r\n------\r\n{% spaceless %}\r\n{% ifchanged %}\r\n* VPN Server: {% if obj.node.domain %} {{ obj.node.domain }} {% else %} {{ obj.node.public_ip }} {% endif %}\r\n* Location: {{ obj.node.location }}\r\n* Encrypt: {{ obj.node.ssmanager.encrypt }}\r\n{% else %}\r\nThis node shares the same settings with above.\r\n{%endifchanged%}\r\n{% endspaceless %}\r\n{% endfor %}\r\n{% endspaceless %}\r\n{% if sender.get_full_name %} {{ sender.get_full_name }} {% else %} {{ '' }} {% endif %}",
+            "content": "Subject: CREDENTIAL: VPN Account (Shadowsocks)\r\nTo: {{ account.email }}\r\nDear {{ account.first_name }},\r\n\r\nYour VPN account is setup as below.\r\n\r\n* Port: {{ account.username }}\r\n* Password: {{ account.password }}\r\n\r\nIt's available on {{ node_accounts|length }} node(s):\r\n{% for obj in node_accounts %}\r\nNode #{{ forloop.counter }}:\r\n------\r\n{% ifchanged %}\r\n* VPN Server: {% if obj.node.record.fqdn %}{{ obj.node.record.fqdn }}{% else %}{{ obj.node.public_ip }}{% endif %}\r\n* Location: {{ obj.node.location }}\r\n* Encrypt: {{ obj.node.ssmanager.encrypt }}{% if obj.node.ssmanager.is_v2ray_enabled %}\r\n* V2Ray: Required\r\n    * Plugin: v2ray-plugin\r\n    * Plugin Options: tls;host={{ obj.node.record.fqdn }}\r\n    * Mode: Websocket (HTTPS){% endif %}\r\n{% else %}\r\nThis node shares the same settings with above.{%endifchanged%}{% endfor %}\r\n{% if sender.get_full_name %}\r\n{{ sender.get_full_name }}{% endif %}",
             "dt_created": "2019-05-12T15:37:42.356Z",
             "dt_updated": "2019-06-18T20:21:16.078Z",
             "is_active": true,
             "type": "account_created"
         },
         "model": "notification.template",
         "pk": 1
```

### Comparing `shadowsocks_manager-0.1.5/shadowsocks_manager/notification/models.py` & `shadowsocks_manager-0.1.6/shadowsocks_manager/notification/models.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.5/shadowsocks_manager/notification/tests.py` & `shadowsocks_manager-0.1.6/shadowsocks_manager/notification/tests.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.5/shadowsocks_manager/retry/__init__.py` & `shadowsocks_manager-0.1.6/shadowsocks_manager/retry/__init__.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.5/shadowsocks_manager/retry/tests.py` & `shadowsocks_manager-0.1.6/shadowsocks_manager/retry/tests.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/admin.py` & `shadowsocks_manager-0.1.6/shadowsocks_manager/shadowsocks/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 class SSManagerInline(admin.TabularInline):
     model = SSManager
     extra = 1
     max_num = 1
 
     fields = ('interface', 'port', 'encrypt', 'is_accessible',
               'server_edition', 'is_v2ray_enabled',)
-    readonly_fields = ('is_accessible', 'is_v2ray_enabled', 'dt_created', 'dt_updated')
+    readonly_fields = ('is_accessible', 'dt_created', 'dt_updated')
 
     def is_accessible(self, obj):
         return obj.is_accessible
 
     is_accessible.boolean = True
```

### Comparing `shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/management/commands/shadowsocks_config.py` & `shadowsocks_manager-0.1.6/shadowsocks_manager/shadowsocks/management/commands/shadowsocks_config.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/models.py` & `shadowsocks_manager-0.1.6/shadowsocks_manager/shadowsocks/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
         # set a default group
         obj = Group.objects.get(name='shadowsocks-clients')
         if obj not in self.groups.all():
             self.groups.add(obj)
 
         return ret
 
-    def notify(self, sender=None):
+    def notify(self, sender=User()):
         """
         Send account owner the account information by email.
         """
         if not self.email:
             raise ValidationError({'email': ["There's no Email address configured for %s." % self.get_full_name()]})
 
         if not self.is_active:
@@ -532,15 +532,15 @@
         LIBEV: "libev",
         PYTHON: "python",
     }
 
 
 class SSManager(models.Model):
     node = models.ForeignKey(Node, on_delete=models.CASCADE, related_name='ssmanagers')
-    interface = enum.EnumField(InterfaceList, default=InterfaceList.LOCALHOST,
+    interface = enum.EnumField(InterfaceList, default=InterfaceList.PRIVATE,
         help_text='Network interface bound to Manager API on the node, use an internal '
             'interface if possible.')
     port = models.PositiveIntegerField(default=6001,
         help_text='Port number bound to Manager API.')
     encrypt = models.CharField(max_length=32, default='aes-256-cfb',
         help_text='Encrypt method: rc4-md5, aes-128-gcm, aes-192-gcm, aes-256-gcm, '
             'aes-128-cfb, aes-192-cfb, aes-256-cfb, aes-128-ctr, aes-192-ctr, aes-256-ctr, '
```

### Comparing `shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/serializers.py` & `shadowsocks_manager-0.1.6/shadowsocks_manager/shadowsocks/serializers.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/tests.py` & `shadowsocks_manager-0.1.6/shadowsocks_manager/shadowsocks/tests.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/urls.py` & `shadowsocks_manager-0.1.6/shadowsocks_manager/shadowsocks/urls.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks/views.py` & `shadowsocks_manager-0.1.6/shadowsocks_manager/shadowsocks/views.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks_manager/celery.py` & `shadowsocks_manager-0.1.6/shadowsocks_manager/shadowsocks_manager/celery.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks_manager/settings.py` & `shadowsocks_manager-0.1.6/shadowsocks_manager/shadowsocks_manager/settings.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.5/shadowsocks_manager/shadowsocks_manager/urls.py` & `shadowsocks_manager-0.1.6/shadowsocks_manager/shadowsocks_manager/urls.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.5/shadowsocks_manager/singleton/models.py` & `shadowsocks_manager-0.1.6/shadowsocks_manager/singleton/models.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.5/shadowsocks_manager/statistic/admin.py` & `shadowsocks_manager-0.1.6/shadowsocks_manager/statistic/admin.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.5/shadowsocks_manager/statistic/models.py` & `shadowsocks_manager-0.1.6/shadowsocks_manager/statistic/models.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.5/shadowsocks_manager/statistic/serializers.py` & `shadowsocks_manager-0.1.6/shadowsocks_manager/statistic/serializers.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.5/shadowsocks_manager/statistic/tests.py` & `shadowsocks_manager-0.1.6/shadowsocks_manager/statistic/tests.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.5/shadowsocks_manager/statistic/views.py` & `shadowsocks_manager-0.1.6/shadowsocks_manager/statistic/views.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.5/shadowsocks_manager/utils/celery.py` & `shadowsocks_manager-0.1.6/shadowsocks_manager/utils/celery.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.5/shadowsocks_manager/utils/createsuperuser.py` & `shadowsocks_manager-0.1.6/shadowsocks_manager/utils/createsuperuser.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.5/shadowsocks_manager/utils/dotenv.py` & `shadowsocks_manager-0.1.6/shadowsocks_manager/utils/dotenv.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.5/shadowsocks_manager/utils/manage.py` & `shadowsocks_manager-0.1.6/shadowsocks_manager/utils/manage.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.5/shadowsocks_manager.egg-info/PKG-INFO` & `shadowsocks_manager-0.1.6/shadowsocks_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shadowsocks-manager
-Version: 0.1.5
+Version: 0.1.6
 Summary: A shadowsocks manager for multi-user and traffic statistics
 Home-page: https://github.com/alexzhangs/shadowsocks-manager
 Author: Alex
 Author-email: Alex <alexzhangs@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Alex Zhang
@@ -133,20 +133,26 @@
         * ~~Pre-installed, and have a builtin service manager.~~
         * No builtin service manager, you need to install it and start the service by yourself.
 
 Code in Python, base on Django, Django REST framework, Celery, and SQLite.
 
 The development status can be found at: [project home](https://github.com/alexzhangs/shadowsocks-manager/projects/1).
 
+
+## Screenshots
+
 Shadowsocks Node List:
 ![Home › Shadowsocks › Shadowsocks Nodes](https://www.0xbeta.com/shadowsocks-manager/assets/images/shadowsocks-node-list.png)
 
 Add Shadowsocks Node:
 ![Home › Shadowsocks › Shadowsocks Nodes](https://www.0xbeta.com/shadowsocks-manager/assets/images/shadowsocks-node-add.png)
 
+Add Shadowsocks Account:
+![Home › Shadowsocks › Shadowsocks Accounts](https://www.0xbeta.com/shadowsocks-manager/assets/images/shadowsocks-account-add.png)
+
 
 ## 1. Requirements
 
 * Python 2.7, Python 3.x
 * Django 1.11.x, Django 3.x
 * Docker
 * [Shadowsocks-libev 3.2.0 for Linux (multi-user API is required)](https://github.com/shadowsocks/shadowsocks-libev)
```

### Comparing `shadowsocks_manager-0.1.5/shadowsocks_manager.egg-info/SOURCES.txt` & `shadowsocks_manager-0.1.6/shadowsocks_manager.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,17 @@
 shadowsocks_manager/notification/admin.py
 shadowsocks_manager/notification/apps.py
 shadowsocks_manager/notification/models.py
 shadowsocks_manager/notification/serializers.py
 shadowsocks_manager/notification/tests.py
 shadowsocks_manager/notification/urls.py
 shadowsocks_manager/notification/views.py
+shadowsocks_manager/notification/fixtures/template-txt-to-json.py
 shadowsocks_manager/notification/fixtures/template.json
+shadowsocks_manager/notification/fixtures/template.txt
 shadowsocks_manager/notification/migrations/__init__.py
 shadowsocks_manager/retry/__init__.py
 shadowsocks_manager/retry/tests.py
 shadowsocks_manager/shadowsocks/__init__.py
 shadowsocks_manager/shadowsocks/admin.py
 shadowsocks_manager/shadowsocks/apps.py
 shadowsocks_manager/shadowsocks/models.py
```

### Comparing `shadowsocks_manager-0.1.5/shadowsocks_manager.egg-info/requires.txt` & `shadowsocks_manager-0.1.6/shadowsocks_manager.egg-info/requires.txt`

 * *Files identical despite different names*

