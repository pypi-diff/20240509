# Comparing `tmp/dramatiq-1.8.1.tar.gz` & `tmp/dramatiq-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dramatiq-1.8.1.tar", last modified: Thu Feb  6 08:48:41 2020, max compression
+gzip compressed data, was "dist/dramatiq-1.9.0.tar", last modified: Mon Jun  8 09:40:16 2020, max compression
```

## Comparing `dramatiq-1.8.1.tar` & `dramatiq-1.9.0.tar`

### file list

```diff
@@ -1,78 +1,79 @@
-drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2020-02-06 08:48:41.000000 dramatiq-1.8.1/
--rw-r--r--   0 bogdan     (501) staff       (20)    35147 2020-01-14 07:13:59.000000 dramatiq-1.8.1/COPYING
--rw-r--r--   0 bogdan     (501) staff       (20)     7650 2020-01-14 07:13:59.000000 dramatiq-1.8.1/COPYING.LESSER
--rw-r--r--   0 bogdan     (501) staff       (20)      163 2020-01-14 07:13:59.000000 dramatiq-1.8.1/MANIFEST.in
--rw-r--r--   0 bogdan     (501) staff       (20)     3370 2020-02-06 08:48:41.000000 dramatiq-1.8.1/PKG-INFO
--rw-r--r--   0 bogdan     (501) staff       (20)     1991 2020-01-14 08:01:10.000000 dramatiq-1.8.1/README.md
-drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2020-02-06 08:48:41.000000 dramatiq-1.8.1/bin/
--rwxr-xr-x   0 bogdan     (501) staff       (20)      291 2020-01-14 07:13:59.000000 dramatiq-1.8.1/bin/dramatiq-gevent
-drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2020-02-06 08:48:41.000000 dramatiq-1.8.1/dramatiq/
--rw-r--r--   0 bogdan     (501) staff       (20)     1954 2020-02-06 08:48:15.000000 dramatiq-1.8.1/dramatiq/__init__.py
--rw-r--r--   0 bogdan     (501) staff       (20)      839 2020-01-14 07:13:59.000000 dramatiq-1.8.1/dramatiq/__main__.py
--rw-r--r--   0 bogdan     (501) staff       (20)     8233 2020-01-14 07:13:59.000000 dramatiq-1.8.1/dramatiq/actor.py
--rw-r--r--   0 bogdan     (501) staff       (20)    11159 2020-02-02 08:59:55.000000 dramatiq-1.8.1/dramatiq/broker.py
-drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2020-02-06 08:48:41.000000 dramatiq-1.8.1/dramatiq/brokers/
--rw-r--r--   0 bogdan     (501) staff       (20)      747 2020-01-14 07:13:59.000000 dramatiq-1.8.1/dramatiq/brokers/__init__.py
--rw-r--r--   0 bogdan     (501) staff       (20)    19725 2020-02-02 10:01:56.000000 dramatiq-1.8.1/dramatiq/brokers/rabbitmq.py
-drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2020-02-06 08:48:41.000000 dramatiq-1.8.1/dramatiq/brokers/redis/
--rw-r--r--   0 bogdan     (501) staff       (20)     8016 2020-01-21 08:52:32.000000 dramatiq-1.8.1/dramatiq/brokers/redis/dispatch.lua
--rw-r--r--   0 bogdan     (501) staff       (20)     1395 2020-01-21 08:52:32.000000 dramatiq-1.8.1/dramatiq/brokers/redis/maxstack.lua
--rw-r--r--   0 bogdan     (501) staff       (20)    13400 2020-02-02 10:01:56.000000 dramatiq-1.8.1/dramatiq/brokers/redis.py
--rw-r--r--   0 bogdan     (501) staff       (20)     6706 2020-01-14 08:01:10.000000 dramatiq-1.8.1/dramatiq/brokers/stub.py
--rw-r--r--   0 bogdan     (501) staff       (20)     2213 2020-02-05 18:45:08.000000 dramatiq-1.8.1/dramatiq/canteen.py
--rw-r--r--   0 bogdan     (501) staff       (20)    19714 2020-02-05 18:45:12.000000 dramatiq-1.8.1/dramatiq/cli.py
--rw-r--r--   0 bogdan     (501) staff       (20)     4174 2020-01-14 07:13:59.000000 dramatiq-1.8.1/dramatiq/common.py
--rw-r--r--   0 bogdan     (501) staff       (20)     2039 2020-01-14 07:13:59.000000 dramatiq-1.8.1/dramatiq/compat.py
--rw-r--r--   0 bogdan     (501) staff       (20)    11660 2020-02-02 10:13:06.000000 dramatiq-1.8.1/dramatiq/composition.py
--rw-r--r--   0 bogdan     (501) staff       (20)     1923 2020-01-14 07:13:59.000000 dramatiq-1.8.1/dramatiq/encoder.py
--rw-r--r--   0 bogdan     (501) staff       (20)     1893 2020-01-14 07:13:59.000000 dramatiq-1.8.1/dramatiq/errors.py
--rw-r--r--   0 bogdan     (501) staff       (20)     3718 2020-01-14 07:13:59.000000 dramatiq-1.8.1/dramatiq/generic.py
--rw-r--r--   0 bogdan     (501) staff       (20)     1006 2020-01-14 07:13:59.000000 dramatiq-1.8.1/dramatiq/logging.py
--rw-r--r--   0 bogdan     (501) staff       (20)     5345 2020-01-14 07:13:59.000000 dramatiq-1.8.1/dramatiq/message.py
-drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2020-02-06 08:48:41.000000 dramatiq-1.8.1/dramatiq/middleware/
--rw-r--r--   0 bogdan     (501) staff       (20)     1745 2020-02-05 17:06:14.000000 dramatiq-1.8.1/dramatiq/middleware/__init__.py
--rw-r--r--   0 bogdan     (501) staff       (20)     1762 2020-01-14 08:01:10.000000 dramatiq-1.8.1/dramatiq/middleware/age_limit.py
--rw-r--r--   0 bogdan     (501) staff       (20)     2040 2020-02-02 10:01:56.000000 dramatiq-1.8.1/dramatiq/middleware/callbacks.py
--rw-r--r--   0 bogdan     (501) staff       (20)     1710 2020-01-14 07:13:59.000000 dramatiq-1.8.1/dramatiq/middleware/current_message.py
--rw-r--r--   0 bogdan     (501) staff       (20)     1744 2020-02-02 10:13:06.000000 dramatiq-1.8.1/dramatiq/middleware/group_callbacks.py
--rw-r--r--   0 bogdan     (501) staff       (20)     5029 2020-02-02 10:01:56.000000 dramatiq-1.8.1/dramatiq/middleware/middleware.py
--rw-r--r--   0 bogdan     (501) staff       (20)     2186 2020-01-14 08:01:10.000000 dramatiq-1.8.1/dramatiq/middleware/pipelines.py
--rw-r--r--   0 bogdan     (501) staff       (20)     7136 2020-02-05 17:21:23.000000 dramatiq-1.8.1/dramatiq/middleware/prometheus.py
--rw-r--r--   0 bogdan     (501) staff       (20)     3731 2020-01-14 07:13:59.000000 dramatiq-1.8.1/dramatiq/middleware/retries.py
--rw-r--r--   0 bogdan     (501) staff       (20)     3405 2020-01-14 07:13:59.000000 dramatiq-1.8.1/dramatiq/middleware/shutdown.py
--rw-r--r--   0 bogdan     (501) staff       (20)     2748 2020-01-14 07:13:59.000000 dramatiq-1.8.1/dramatiq/middleware/threading.py
--rw-r--r--   0 bogdan     (501) staff       (20)     3663 2020-01-14 07:13:59.000000 dramatiq-1.8.1/dramatiq/middleware/time_limit.py
-drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2020-02-06 08:48:41.000000 dramatiq-1.8.1/dramatiq/rate_limits/
--rw-r--r--   0 bogdan     (501) staff       (20)     1155 2020-01-14 07:13:59.000000 dramatiq-1.8.1/dramatiq/rate_limits/__init__.py
--rw-r--r--   0 bogdan     (501) staff       (20)     3907 2020-01-14 07:13:59.000000 dramatiq-1.8.1/dramatiq/rate_limits/backend.py
-drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2020-02-06 08:48:41.000000 dramatiq-1.8.1/dramatiq/rate_limits/backends/
--rw-r--r--   0 bogdan     (501) staff       (20)     1361 2020-01-14 07:13:59.000000 dramatiq-1.8.1/dramatiq/rate_limits/backends/__init__.py
--rw-r--r--   0 bogdan     (501) staff       (20)     3117 2020-01-14 07:13:59.000000 dramatiq-1.8.1/dramatiq/rate_limits/backends/memcached.py
--rw-r--r--   0 bogdan     (501) staff       (20)     4246 2020-01-14 07:13:59.000000 dramatiq-1.8.1/dramatiq/rate_limits/backends/redis.py
--rw-r--r--   0 bogdan     (501) staff       (20)     2965 2020-01-14 07:13:59.000000 dramatiq-1.8.1/dramatiq/rate_limits/backends/stub.py
--rw-r--r--   0 bogdan     (501) staff       (20)     2993 2020-01-14 07:13:59.000000 dramatiq-1.8.1/dramatiq/rate_limits/barrier.py
--rw-r--r--   0 bogdan     (501) staff       (20)     2633 2020-01-14 07:13:59.000000 dramatiq-1.8.1/dramatiq/rate_limits/bucket.py
--rw-r--r--   0 bogdan     (501) staff       (20)     1805 2020-01-14 07:13:59.000000 dramatiq-1.8.1/dramatiq/rate_limits/concurrent.py
--rw-r--r--   0 bogdan     (501) staff       (20)     2505 2020-01-14 07:13:59.000000 dramatiq-1.8.1/dramatiq/rate_limits/rate_limiter.py
--rw-r--r--   0 bogdan     (501) staff       (20)     2207 2020-01-14 07:13:59.000000 dramatiq-1.8.1/dramatiq/rate_limits/window.py
-drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2020-02-06 08:48:41.000000 dramatiq-1.8.1/dramatiq/results/
--rw-r--r--   0 bogdan     (501) staff       (20)      986 2020-01-14 07:13:59.000000 dramatiq-1.8.1/dramatiq/results/__init__.py
--rw-r--r--   0 bogdan     (501) staff       (20)     4981 2020-01-14 07:13:59.000000 dramatiq-1.8.1/dramatiq/results/backend.py
-drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2020-02-06 08:48:41.000000 dramatiq-1.8.1/dramatiq/results/backends/
--rw-r--r--   0 bogdan     (501) staff       (20)     1360 2020-01-14 07:13:59.000000 dramatiq-1.8.1/dramatiq/results/backends/__init__.py
--rw-r--r--   0 bogdan     (501) staff       (20)     2239 2020-01-14 07:13:59.000000 dramatiq-1.8.1/dramatiq/results/backends/memcached.py
--rw-r--r--   0 bogdan     (501) staff       (20)     3576 2020-01-14 07:13:59.000000 dramatiq-1.8.1/dramatiq/results/backends/redis.py
--rw-r--r--   0 bogdan     (501) staff       (20)     1591 2020-01-14 07:13:59.000000 dramatiq-1.8.1/dramatiq/results/backends/stub.py
--rw-r--r--   0 bogdan     (501) staff       (20)     1047 2020-01-14 07:13:59.000000 dramatiq-1.8.1/dramatiq/results/errors.py
--rw-r--r--   0 bogdan     (501) staff       (20)     2660 2020-01-14 07:13:59.000000 dramatiq-1.8.1/dramatiq/results/middleware.py
--rw-r--r--   0 bogdan     (501) staff       (20)     1222 2020-01-14 07:13:59.000000 dramatiq-1.8.1/dramatiq/watcher.py
--rw-r--r--   0 bogdan     (501) staff       (20)    19707 2020-01-14 07:13:59.000000 dramatiq-1.8.1/dramatiq/worker.py
-drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2020-02-06 08:48:41.000000 dramatiq-1.8.1/dramatiq.egg-info/
--rw-r--r--   0 bogdan     (501) staff       (20)     3370 2020-02-06 08:48:41.000000 dramatiq-1.8.1/dramatiq.egg-info/PKG-INFO
--rw-r--r--   0 bogdan     (501) staff       (20)     1834 2020-02-06 08:48:41.000000 dramatiq-1.8.1/dramatiq.egg-info/SOURCES.txt
--rw-r--r--   0 bogdan     (501) staff       (20)        1 2020-02-06 08:48:41.000000 dramatiq-1.8.1/dramatiq.egg-info/dependency_links.txt
--rw-r--r--   0 bogdan     (501) staff       (20)       53 2020-02-06 08:48:41.000000 dramatiq-1.8.1/dramatiq.egg-info/entry_points.txt
--rw-r--r--   0 bogdan     (501) staff       (20)      517 2020-02-06 08:48:41.000000 dramatiq-1.8.1/dramatiq.egg-info/requires.txt
--rw-r--r--   0 bogdan     (501) staff       (20)        9 2020-02-06 08:48:41.000000 dramatiq-1.8.1/dramatiq.egg-info/top_level.txt
--rw-r--r--   0 bogdan     (501) staff       (20)      472 2020-02-06 08:48:41.000000 dramatiq-1.8.1/setup.cfg
--rw-r--r--   0 bogdan     (501) staff       (20)     3198 2020-01-14 08:01:10.000000 dramatiq-1.8.1/setup.py
+drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2020-06-08 09:40:16.000000 dramatiq-1.9.0/
+-rw-r--r--   0 bogdan     (501) staff       (20)    35147 2020-01-14 07:13:59.000000 dramatiq-1.9.0/COPYING
+-rw-r--r--   0 bogdan     (501) staff       (20)     7650 2020-01-14 07:13:59.000000 dramatiq-1.9.0/COPYING.LESSER
+-rw-r--r--   0 bogdan     (501) staff       (20)      163 2020-01-14 07:13:59.000000 dramatiq-1.9.0/MANIFEST.in
+-rw-r--r--   0 bogdan     (501) staff       (20)     3370 2020-06-08 09:40:16.000000 dramatiq-1.9.0/PKG-INFO
+-rw-r--r--   0 bogdan     (501) staff       (20)     1991 2020-01-14 08:01:10.000000 dramatiq-1.9.0/README.md
+drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2020-06-08 09:40:16.000000 dramatiq-1.9.0/bin/
+-rwxr-xr-x   0 bogdan     (501) staff       (20)      291 2020-01-14 07:13:59.000000 dramatiq-1.9.0/bin/dramatiq-gevent
+drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2020-06-08 09:40:16.000000 dramatiq-1.9.0/dramatiq/
+-rw-r--r--   0 bogdan     (501) staff       (20)     1970 2020-06-08 09:39:29.000000 dramatiq-1.9.0/dramatiq/__init__.py
+-rw-r--r--   0 bogdan     (501) staff       (20)      839 2020-01-14 07:13:59.000000 dramatiq-1.9.0/dramatiq/__main__.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     8702 2020-06-08 08:58:03.000000 dramatiq-1.9.0/dramatiq/actor.py
+-rw-r--r--   0 bogdan     (501) staff       (20)    11053 2020-03-29 09:54:03.000000 dramatiq-1.9.0/dramatiq/broker.py
+drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2020-06-08 09:40:16.000000 dramatiq-1.9.0/dramatiq/brokers/
+-rw-r--r--   0 bogdan     (501) staff       (20)      747 2020-01-14 07:13:59.000000 dramatiq-1.9.0/dramatiq/brokers/__init__.py
+-rw-r--r--   0 bogdan     (501) staff       (20)    19808 2020-06-08 09:06:29.000000 dramatiq-1.9.0/dramatiq/brokers/rabbitmq.py
+drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2020-06-08 09:40:16.000000 dramatiq-1.9.0/dramatiq/brokers/redis/
+-rw-r--r--   0 bogdan     (501) staff       (20)     8016 2020-01-21 08:52:32.000000 dramatiq-1.9.0/dramatiq/brokers/redis/dispatch.lua
+-rw-r--r--   0 bogdan     (501) staff       (20)     1395 2020-01-21 08:52:32.000000 dramatiq-1.9.0/dramatiq/brokers/redis/maxstack.lua
+-rw-r--r--   0 bogdan     (501) staff       (20)    13567 2020-06-08 08:52:50.000000 dramatiq-1.9.0/dramatiq/brokers/redis.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     6706 2020-01-14 08:01:10.000000 dramatiq-1.9.0/dramatiq/brokers/stub.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     2213 2020-02-05 18:45:08.000000 dramatiq-1.9.0/dramatiq/canteen.py
+-rw-r--r--   0 bogdan     (501) staff       (20)    20408 2020-06-08 09:28:30.000000 dramatiq-1.9.0/dramatiq/cli.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     4174 2020-01-14 07:13:59.000000 dramatiq-1.9.0/dramatiq/common.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     2140 2020-04-18 14:26:28.000000 dramatiq-1.9.0/dramatiq/compat.py
+-rw-r--r--   0 bogdan     (501) staff       (20)    11660 2020-02-02 10:13:06.000000 dramatiq-1.9.0/dramatiq/composition.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     1923 2020-01-14 07:13:59.000000 dramatiq-1.9.0/dramatiq/encoder.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     2440 2020-04-18 14:21:02.000000 dramatiq-1.9.0/dramatiq/errors.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     3718 2020-01-14 07:13:59.000000 dramatiq-1.9.0/dramatiq/generic.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     1006 2020-01-14 07:13:59.000000 dramatiq-1.9.0/dramatiq/logging.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     5345 2020-01-14 07:13:59.000000 dramatiq-1.9.0/dramatiq/message.py
+drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2020-06-08 09:40:16.000000 dramatiq-1.9.0/dramatiq/middleware/
+-rw-r--r--   0 bogdan     (501) staff       (20)     1745 2020-02-05 17:06:14.000000 dramatiq-1.9.0/dramatiq/middleware/__init__.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     1762 2020-01-14 08:01:10.000000 dramatiq-1.9.0/dramatiq/middleware/age_limit.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     2040 2020-02-02 10:01:56.000000 dramatiq-1.9.0/dramatiq/middleware/callbacks.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     1710 2020-01-14 07:13:59.000000 dramatiq-1.9.0/dramatiq/middleware/current_message.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     1744 2020-02-02 10:13:06.000000 dramatiq-1.9.0/dramatiq/middleware/group_callbacks.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     5029 2020-02-02 10:01:56.000000 dramatiq-1.9.0/dramatiq/middleware/middleware.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     2186 2020-01-14 08:01:10.000000 dramatiq-1.9.0/dramatiq/middleware/pipelines.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     7136 2020-02-05 17:21:23.000000 dramatiq-1.9.0/dramatiq/middleware/prometheus.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     4682 2020-04-26 09:33:23.000000 dramatiq-1.9.0/dramatiq/middleware/retries.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     3405 2020-01-14 07:13:59.000000 dramatiq-1.9.0/dramatiq/middleware/shutdown.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     2748 2020-01-14 07:13:59.000000 dramatiq-1.9.0/dramatiq/middleware/threading.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     3663 2020-01-14 07:13:59.000000 dramatiq-1.9.0/dramatiq/middleware/time_limit.py
+drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2020-06-08 09:40:16.000000 dramatiq-1.9.0/dramatiq/rate_limits/
+-rw-r--r--   0 bogdan     (501) staff       (20)     1155 2020-01-14 07:13:59.000000 dramatiq-1.9.0/dramatiq/rate_limits/__init__.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     3907 2020-01-14 07:13:59.000000 dramatiq-1.9.0/dramatiq/rate_limits/backend.py
+drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2020-06-08 09:40:16.000000 dramatiq-1.9.0/dramatiq/rate_limits/backends/
+-rw-r--r--   0 bogdan     (501) staff       (20)     1361 2020-01-14 07:13:59.000000 dramatiq-1.9.0/dramatiq/rate_limits/backends/__init__.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     3117 2020-01-14 07:13:59.000000 dramatiq-1.9.0/dramatiq/rate_limits/backends/memcached.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     4246 2020-01-14 07:13:59.000000 dramatiq-1.9.0/dramatiq/rate_limits/backends/redis.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     2965 2020-01-14 07:13:59.000000 dramatiq-1.9.0/dramatiq/rate_limits/backends/stub.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     2993 2020-01-14 07:13:59.000000 dramatiq-1.9.0/dramatiq/rate_limits/barrier.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     2633 2020-01-14 07:13:59.000000 dramatiq-1.9.0/dramatiq/rate_limits/bucket.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     1805 2020-01-14 07:13:59.000000 dramatiq-1.9.0/dramatiq/rate_limits/concurrent.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     2505 2020-01-14 07:13:59.000000 dramatiq-1.9.0/dramatiq/rate_limits/rate_limiter.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     2207 2020-01-14 07:13:59.000000 dramatiq-1.9.0/dramatiq/rate_limits/window.py
+drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2020-06-08 09:40:16.000000 dramatiq-1.9.0/dramatiq/results/
+-rw-r--r--   0 bogdan     (501) staff       (20)     1018 2020-03-29 09:54:03.000000 dramatiq-1.9.0/dramatiq/results/__init__.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     5523 2020-03-29 09:54:03.000000 dramatiq-1.9.0/dramatiq/results/backend.py
+drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2020-06-08 09:40:16.000000 dramatiq-1.9.0/dramatiq/results/backends/
+-rw-r--r--   0 bogdan     (501) staff       (20)     1360 2020-01-14 07:13:59.000000 dramatiq-1.9.0/dramatiq/results/backends/__init__.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     2239 2020-01-14 07:13:59.000000 dramatiq-1.9.0/dramatiq/results/backends/memcached.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     3627 2020-03-29 09:54:03.000000 dramatiq-1.9.0/dramatiq/results/backends/redis.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     1591 2020-01-14 07:13:59.000000 dramatiq-1.9.0/dramatiq/results/backends/stub.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     1345 2020-04-26 09:09:16.000000 dramatiq-1.9.0/dramatiq/results/errors.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     3587 2020-03-29 09:54:03.000000 dramatiq-1.9.0/dramatiq/results/middleware.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     1614 2020-04-26 09:09:16.000000 dramatiq-1.9.0/dramatiq/results/result.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     1222 2020-01-14 07:13:59.000000 dramatiq-1.9.0/dramatiq/watcher.py
+-rw-r--r--   0 bogdan     (501) staff       (20)    20076 2020-04-26 09:33:23.000000 dramatiq-1.9.0/dramatiq/worker.py
+drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2020-06-08 09:40:16.000000 dramatiq-1.9.0/dramatiq.egg-info/
+-rw-r--r--   0 bogdan     (501) staff       (20)     3370 2020-06-08 09:40:16.000000 dramatiq-1.9.0/dramatiq.egg-info/PKG-INFO
+-rw-r--r--   0 bogdan     (501) staff       (20)     1861 2020-06-08 09:40:16.000000 dramatiq-1.9.0/dramatiq.egg-info/SOURCES.txt
+-rw-r--r--   0 bogdan     (501) staff       (20)        1 2020-06-08 09:40:16.000000 dramatiq-1.9.0/dramatiq.egg-info/dependency_links.txt
+-rw-r--r--   0 bogdan     (501) staff       (20)       53 2020-06-08 09:40:16.000000 dramatiq-1.9.0/dramatiq.egg-info/entry_points.txt
+-rw-r--r--   0 bogdan     (501) staff       (20)      517 2020-06-08 09:40:16.000000 dramatiq-1.9.0/dramatiq.egg-info/requires.txt
+-rw-r--r--   0 bogdan     (501) staff       (20)        9 2020-06-08 09:40:16.000000 dramatiq-1.9.0/dramatiq.egg-info/top_level.txt
+-rw-r--r--   0 bogdan     (501) staff       (20)      477 2020-06-08 09:40:16.000000 dramatiq-1.9.0/setup.cfg
+-rw-r--r--   0 bogdan     (501) staff       (20)     3198 2020-01-14 08:01:10.000000 dramatiq-1.9.0/setup.py
```

### Comparing `dramatiq-1.8.1/COPYING` & `dramatiq-1.9.0/COPYING`

 * *Files identical despite different names*

### Comparing `dramatiq-1.8.1/COPYING.LESSER` & `dramatiq-1.9.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `dramatiq-1.8.1/PKG-INFO` & `dramatiq-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dramatiq
-Version: 1.8.1
+Version: 1.9.0
 Summary: Background Processing for Python 3.
 Home-page: UNKNOWN
 Author: Bogdan Popa
 Author-email: bogdan@cleartype.io
 License: UNKNOWN
 Description: <img src="https://dramatiq.io/_static/logo.png" align="right" width="131" />
```

### Comparing `dramatiq-1.8.1/README.md` & `dramatiq-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `dramatiq-1.8.1/dramatiq/__init__.py` & `dramatiq-1.9.0/dramatiq/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from .actor import Actor, actor
 from .broker import Broker, Consumer, MessageProxy, get_broker, set_broker
 from .composition import group, pipeline
 from .encoder import Encoder, JSONEncoder, PickleEncoder
 from .errors import (
     ActorNotFound, BrokerError, ConnectionClosed, ConnectionError, ConnectionFailed, DramatiqError, QueueJoinTimeout,
-    QueueNotFound, RateLimitExceeded
+    QueueNotFound, RateLimitExceeded, Retry
 )
 from .generic import GenericActor
 from .logging import get_logger
 from .message import Message, get_encoder, set_encoder
 from .middleware import Middleware
 from .worker import Worker
 
@@ -43,23 +43,23 @@
     "Encoder", "JSONEncoder", "PickleEncoder",
 
     # Errors
     "DramatiqError",
     "BrokerError",
     "ActorNotFound", "QueueNotFound", "QueueJoinTimeout",
     "ConnectionError", "ConnectionClosed", "ConnectionFailed",
-    "RateLimitExceeded",
+    "RateLimitExceeded", "Retry",
 
     # Logging
     "get_logger",
 
     # Messages
     "Message", "get_encoder", "set_encoder",
 
     # Middlware
     "Middleware",
 
     # Workers
     "Worker",
 ]
 
-__version__ = "1.8.1"
+__version__ = "1.9.0"
```

### Comparing `dramatiq-1.8.1/dramatiq/__main__.py` & `dramatiq-1.9.0/dramatiq/__main__.py`

 * *Files identical despite different names*

### Comparing `dramatiq-1.8.1/dramatiq/actor.py` & `dramatiq-1.9.0/dramatiq/actor.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,15 +138,23 @@
 
         Returns:
           Whatever the underlying function backing this actor returns.
         """
         try:
             self.logger.debug("Received args=%r kwargs=%r.", args, kwargs)
             start = time.perf_counter()
-            return self.fn(*args, **kwargs)
+            result = self.fn(*args, **kwargs)
+            if result is not None and not self.options.get("store_results", False):
+                self.logger.warning(
+                    "Actor '%s' returns a value that is not None, and you haven't added the "
+                    "Results middleware to the broker, which means the return value will be silently dropped. "
+                    "Consider adding the Results middleware to your broker." % self.actor_name
+                )
+
+            return result
         finally:
             delta = time.perf_counter() - start
             self.logger.debug("Completed after %.02fms.", delta * 1000)
 
     def __repr__(self):
         return "Actor(%(fn)r, queue_name=%(queue_name)r, actor_name=%(actor_name)r)" % vars(self)
```

### Comparing `dramatiq-1.8.1/dramatiq/broker.py` & `dramatiq-1.9.0/dramatiq/broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -318,17 +318,15 @@
 
     def __init__(self, message):
         self.failed = False
         self._message = message
         self._exception = None
 
     def stuff_exception(self, exception):
-        """Stuff an exception into this message.  Currently, this is
-        used by the stub broker to known why a particular message has
-        failed.
+        """Stuff an exception into this message.
         """
         self._exception = exception
 
     def fail(self):
         """Mark this message for rejection.
         """
         self.failed = True
```

### Comparing `dramatiq-1.8.1/dramatiq/brokers/__init__.py` & `dramatiq-1.9.0/dramatiq/brokers/__init__.py`

 * *Files identical despite different names*

### Comparing `dramatiq-1.8.1/dramatiq/brokers/rabbitmq.py` & `dramatiq-1.9.0/dramatiq/brokers/rabbitmq.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,18 @@
         self.connections = set()
         self.channels = set()
         self.queues = set()
         self.queues_pending = set()
         self.state = local()
 
     @property
+    def consumer_class(self):
+        return _RabbitmqConsumer
+
+    @property
     def connection(self):
         """The :class:`pika.BlockingConnection` for the current
         thread.  This property may change without notice.
         """
         connection = getattr(self.state, "connection", None)
         if connection is None:
             connection = self.state.connection = pika.BlockingConnection(
@@ -185,15 +189,15 @@
           prefetch(int): The number of messages to prefetch.
           timeout(int): The idle timeout in milliseconds.
 
         Returns:
           Consumer: A consumer that retrieves messages from RabbitMQ.
         """
         self.declare_queue(queue_name, ensure=True)
-        return _RabbitmqConsumer(self.parameters, queue_name, prefetch, timeout)
+        return self.consumer_class(self.parameters, queue_name, prefetch, timeout)
 
     def declare_queue(self, queue_name, *, ensure=False):
         """Declare a queue.  Has no effect if a queue with the given
         name already exists.
 
         Parameters:
           queue_name(str): The name of the new queue.
@@ -280,19 +284,14 @@
         Raises:
           ConnectionClosed: If the underlying channel or connection
             has been closed.
         """
         queue_name = message.queue_name
         self.declare_queue(queue_name, ensure=True)
 
-        properties = pika.BasicProperties(
-            delivery_mode=2,
-            priority=message.options.get("broker_priority"),
-        )
-
         if delay is not None:
             queue_name = dq_name(queue_name)
             message_eta = current_millis() + delay
             message = message.copy(
                 queue_name=queue_name,
                 options={
                     "eta": message_eta,
@@ -304,15 +303,18 @@
             try:
                 self.logger.debug("Enqueueing message %r on queue %r.", message.message_id, queue_name)
                 self.emit_before("enqueue", message, delay)
                 self.channel.basic_publish(
                     exchange="",
                     routing_key=queue_name,
                     body=message.encode(),
-                    properties=properties,
+                    properties=pika.BasicProperties(
+                        delivery_mode=2,
+                        priority=message.options.get("broker_priority"),
+                    ),
                 )
                 self.emit_after("enqueue", message, delay)
                 return message
 
             except (pika.exceptions.AMQPConnectionError,
                     pika.exceptions.AMQPChannelError) as e:
                 # Delete the channel and the connection so that the
```

### Comparing `dramatiq-1.8.1/dramatiq/brokers/redis/dispatch.lua` & `dramatiq-1.9.0/dramatiq/brokers/redis/dispatch.lua`

 * *Files identical despite different names*

### Comparing `dramatiq-1.8.1/dramatiq/brokers/redis/maxstack.lua` & `dramatiq-1.9.0/dramatiq/brokers/redis/maxstack.lua`

 * *Files identical despite different names*

### Comparing `dramatiq-1.8.1/dramatiq/brokers/redis.py` & `dramatiq-1.9.0/dramatiq/brokers/redis.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,28 +73,30 @@
       heartbeat_timeout(int): The amount of time (in ms) that has to
         pass without a heartbeat for a broker process to be considered
         offline.
       dead_message_ttl(int): The amount of time (in ms) that
         dead-lettered messages are kept in Redis for.
       requeue_deadline(int): Deprecated.  Does nothing.
       requeue_interval(int): Deprecated.  Does nothing.
+      client(redis.StrictRedis): A redis client to use.
       **parameters(dict): Connection parameters are passed directly
         to :class:`redis.Redis`.
 
     .. _Redis: http://redis-py.readthedocs.io/en/latest/#redis.Redis
     """
 
     def __init__(
             self, *,
             url=None, middleware=None, namespace="dramatiq",
             maintenance_chance=DEFAULT_MAINTENANCE_CHANCE,
             heartbeat_timeout=DEFAULT_HEARTBEAT_TIMEOUT,
             dead_message_ttl=DEFAULT_DEAD_MESSAGE_TTL,
             requeue_deadline=None,
             requeue_interval=None,
+            client=None,
             **parameters
     ):
         super().__init__(middleware=middleware)
 
         if url:
             parameters["connection_pool"] = redis.ConnectionPool.from_url(url)
 
@@ -105,29 +107,33 @@
         self.broker_id = str(uuid4())
         self.namespace = namespace
         self.maintenance_chance = maintenance_chance
         self.heartbeat_timeout = heartbeat_timeout
         self.dead_message_ttl = dead_message_ttl
         self.queues = set()
         # TODO: Replace usages of StrictRedis (redis-py 2.x) with Redis in Dramatiq 2.0.
-        self.client = client = redis.StrictRedis(**parameters)
-        self.scripts = {name: client.register_script(script) for name, script in _scripts.items()}
+        self.client = client or redis.StrictRedis(**parameters)
+        self.scripts = {name: self.client.register_script(script) for name, script in _scripts.items()}
+
+    @property
+    def consumer_class(self):
+        return _RedisConsumer
 
     def consume(self, queue_name, prefetch=1, timeout=5000):
         """Create a new consumer for a queue.
 
         Parameters:
           queue_name(str): The queue to consume.
           prefetch(int): The number of messages to prefetch.
           timeout(int): The idle timeout in milliseconds.
 
         Returns:
           Consumer: A consumer that retrieves messages from Redis.
         """
-        return _RedisConsumer(self, queue_name, prefetch, timeout)
+        return self.consumer_class(self, queue_name, prefetch, timeout)
 
     def declare_queue(self, queue_name):
         """Declare a queue.  Has no effect if a queue with the given
         name has already been declared.
 
         Parameters:
           queue_name(str): The name of the new queue.
```

### Comparing `dramatiq-1.8.1/dramatiq/brokers/stub.py` & `dramatiq-1.9.0/dramatiq/brokers/stub.py`

 * *Files identical despite different names*

### Comparing `dramatiq-1.8.1/dramatiq/canteen.py` & `dramatiq-1.9.0/dramatiq/canteen.py`

 * *Files identical despite different names*

### Comparing `dramatiq-1.8.1/dramatiq/cli.py` & `dramatiq-1.9.0/dramatiq/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import multiprocessing
 import os
 import random
 import signal
 import sys
 import time
 from itertools import chain
-from threading import Thread
+from threading import Event, Thread
 
 from dramatiq import Broker, ConnectionError, Worker, __version__, get_broker, get_logger
 from dramatiq.canteen import Canteen, canteen_add, canteen_get, canteen_try_init
 from dramatiq.compat import StreamablePipe, file_or_stderr
 
 try:
     from .watcher import setup_file_watcher
@@ -277,17 +277,17 @@
     return setup_logging
 
 
 setup_worker_logging = make_logging_setup("WorkerProcess")
 setup_fork_logging = make_logging_setup("ForkProcess")
 
 
-def watch_logs(log_filename, pipes):
+def watch_logs(log_filename, pipes, stop):
     with file_or_stderr(log_filename, mode="a", encoding="utf-8") as log_file:
-        while pipes:
+        while pipes and not stop.is_set():
             try:
                 events = multiprocessing.connection.wait(pipes, timeout=1)
                 for event in events:
                     try:
                         while event.poll():
                             # StreamHandler writes newlines into the pipe separately
                             # from the actual log entry; to avoid back-to-back newlines
@@ -297,15 +297,15 @@
                                 data = event.recv_bytes()
                             except EOFError:
                                 event.close()
                                 raise
 
                             data = data.decode("utf-8", errors="replace").rstrip("\n")
                             if not data:
-                                break
+                                continue
 
                             log_file.write(data + "\n")
                             log_file.flush()
                     except BrokenPipeError:
                         event.close()
                         raise
             # If one of the worker processes is killed, its handle will be
@@ -314,15 +314,15 @@
             # is closed, and event.poll() raises BrokenPipeError when
             # its pipe is closed.  When any of these events happen, we
             # just take the closed pipes out of the waitlist.
             except (EOFError, OSError):
                 pipes = [p for p in pipes if not p.closed]
 
 
-def worker_process(args, worker_id, logging_pipe, canteen):
+def worker_process(args, worker_id, logging_pipe, canteen, event):
     try:
         # Re-seed the random number generator from urandom on
         # supported platforms.  This should make it so that worker
         # processes don't all follow the same sequence.
         random.seed()
 
         logger = setup_worker_logging(args, worker_id, logging_pipe)
@@ -347,14 +347,19 @@
         worker.start()
     except ImportError:
         logger.exception("Failed to import module.")
         return sys.exit(RET_IMPORT)
     except ConnectionError:
         logger.exception("Broker connection failed.")
         return sys.exit(RET_CONNECT)
+    finally:
+        # Signal to the master process that this process has booted,
+        # regardless of whether it failed or not.  If it did fail, the
+        # worker process will realize that soon enough.
+        event.set()
 
     def termhandler(signum, frame):
         nonlocal running
         if running:
             logger.info("Stopping worker process...")
             running = False
         else:
@@ -432,39 +437,50 @@
             logger = setup_parent_logging(args, stream=stream)
             logger.critical(e)
             return RET_PIDFILE
 
     canteen = multiprocessing.Value(Canteen)
     worker_pipes = []
     worker_processes = []
+    worker_process_events = []
     for worker_id in range(args.processes):
-        read_pipe, write_pipe = multiprocessing.Pipe()
+        read_pipe, write_pipe = multiprocessing.Pipe(duplex=False)
+        event = multiprocessing.Event()
         proc = multiprocessing.Process(
             target=worker_process,
-            args=(args, worker_id, StreamablePipe(write_pipe), canteen),
-            daemon=True,
+            args=(args, worker_id, StreamablePipe(write_pipe), canteen, event),
+            daemon=False,
         )
         proc.start()
         worker_pipes.append(read_pipe)
         worker_processes.append(proc)
+        worker_process_events.append(event)
+
+    # Wait for all worker processes to come online before starting the
+    # fork processes.  This is required to avoid race conditions like
+    # in #297.
+    for event in worker_process_events:
+        if proc.is_alive():
+            if not event.wait(timeout=30):
+                break
 
     fork_pipes = []
     fork_processes = []
     for fork_id, fork_path in enumerate(chain(args.forks, canteen_get(canteen))):
-        read_pipe, write_pipe = multiprocessing.Pipe()
+        read_pipe, write_pipe = multiprocessing.Pipe(duplex=False)
         proc = multiprocessing.Process(
             target=fork_process,
             args=(args, fork_id, fork_path, StreamablePipe(write_pipe)),
             daemon=True,
         )
         proc.start()
         fork_pipes.append(read_pipe)
         fork_processes.append(proc)
 
-    parent_read_pipe, parent_write_pipe = multiprocessing.Pipe()
+    parent_read_pipe, parent_write_pipe = multiprocessing.Pipe(duplex=False)
     logger = setup_parent_logging(args, stream=StreamablePipe(parent_write_pipe))
     logger.info("Dramatiq %r is booting up." % __version__)
     if args.pid_file:
         atexit.register(remove_pidfile, args.pid_file, logger)
 
     running, reload_process = True, False
 
@@ -478,17 +494,18 @@
             signal.SIG_BLOCK,
             {signal.SIGINT, signal.SIGTERM, signal.SIGHUP},
         )
 
     if HAS_WATCHDOG and args.watch:
         file_watcher = setup_file_watcher(args.watch, args.watch_use_polling)
 
+    log_watcher_stop_event = Event()
     log_watcher = Thread(
         target=watch_logs,
-        args=(args.log_file, [parent_read_pipe, *worker_pipes, *fork_pipes]),
+        args=(args.log_file, [parent_read_pipe, *worker_pipes, *fork_pipes], log_watcher_stop_event),
         daemon=False,
     )
     log_watcher.start()
 
     def stop_subprocesses(signum):
         nonlocal running
         running = False
@@ -522,41 +539,38 @@
     signal.signal(signal.SIGTERM, sighandler)
     if hasattr(signal, "SIGHUP"):
         signal.signal(signal.SIGHUP, sighandler)
     if hasattr(signal, "SIGBREAK"):
         signal.signal(signal.SIGBREAK, sighandler)
 
     # Wait for all workers to terminate.  If any of the processes
-    # terminates unexpectedly, then shut down the rest as well.
-    while any(p.exitcode is None for p in worker_processes):
+    # terminates unexpectedly, then shut down the rest as well.  The
+    # use of `waited' here avoids a race condition where the processes
+    # could potentially exit before we even get a chance to wait on
+    # them.
+    waited = False
+    while not waited or any(p.exitcode is None for p in worker_processes):
+        waited = True
         for proc in worker_processes:
             proc.join(timeout=1)
             if proc.exitcode is None:
                 continue
 
             if running:  # pragma: no cover
                 logger.critical("Worker with PID %r exited unexpectedly (code %r). Shutting down...", proc.pid, proc.exitcode)
                 stop_subprocesses(signal.SIGTERM)
                 retcode = proc.exitcode
                 break
 
             else:
                 retcode = max(retcode, proc.exitcode)
 
-    for pipe in [parent_read_pipe, parent_write_pipe, *worker_pipes, *fork_pipes]:
-        try:
-            pipe.close()
-        # If the worker process was killed, the handle may already be
-        # closed.
-        except (EOFError, OSError):
-            pass
-
-    # The log watcher can't be a daemon in case we log to a file.  So
-    # we have to wait for it to complete on exit.  Closing all the
-    # pipes above is what should trigger said exit.
+    # The log watcher can't be a daemon in case we log to a file so we
+    # have to wait for it to complete on exit.
+    log_watcher_stop_event.set()
     log_watcher.join()
 
     if HAS_WATCHDOG and args.watch:
         file_watcher.stop()
         file_watcher.join()
 
     if reload_process:
```

### Comparing `dramatiq-1.8.1/dramatiq/common.py` & `dramatiq-1.9.0/dramatiq/common.py`

 * *Files identical despite different names*

### Comparing `dramatiq-1.8.1/dramatiq/compat.py` & `dramatiq-1.9.0/dramatiq/compat.py`

 * *Files 13% similar despite different names*

```diff
@@ -32,14 +32,20 @@
         parent.
     """
 
     def __init__(self, pipe, *, encoding="utf-8"):
         self.encoding = encoding
         self.pipe = pipe
 
+    def fileno(self):
+        return self.pipe.fileno()
+
+    def isatty(self):
+        return False
+
     def flush(self):
         pass
 
     def close(self):
         self.pipe.close()
 
     def read(self):  # pragma: no cover
```

### Comparing `dramatiq-1.8.1/dramatiq/composition.py` & `dramatiq-1.9.0/dramatiq/composition.py`

 * *Files identical despite different names*

### Comparing `dramatiq-1.8.1/dramatiq/encoder.py` & `dramatiq-1.9.0/dramatiq/encoder.py`

 * *Files identical despite different names*

### Comparing `dramatiq-1.8.1/dramatiq/errors.py` & `dramatiq-1.9.0/dramatiq/errors.py`

 * *Files 10% similar despite different names*

```diff
@@ -62,7 +62,22 @@
     """Raised when a broker connection is suddenly closed.
     """
 
 
 class RateLimitExceeded(DramatiqError):
     """Raised when a rate limit has been exceeded.
     """
+
+
+class Retry(DramatiqError):
+    """Actors may raise this error when they should be retried.  This
+    behaves just like any other exception from the perspective of the
+    :class:`Retries<dramatiq.middleware.Retries>` middleware, the only
+    difference is it doesn't get logged as an error.
+
+    If the ``delay`` argument is provided, then the message will be
+    retried after at least that amount of time (in milliseconds).
+    """
+
+    def __init__(self, message="", delay=None):
+        super().__init__(message)
+        self.delay = delay
```

### Comparing `dramatiq-1.8.1/dramatiq/generic.py` & `dramatiq-1.9.0/dramatiq/generic.py`

 * *Files identical despite different names*

### Comparing `dramatiq-1.8.1/dramatiq/logging.py` & `dramatiq-1.9.0/dramatiq/logging.py`

 * *Files identical despite different names*

### Comparing `dramatiq-1.8.1/dramatiq/message.py` & `dramatiq-1.9.0/dramatiq/message.py`

 * *Files identical despite different names*

### Comparing `dramatiq-1.8.1/dramatiq/middleware/__init__.py` & `dramatiq-1.9.0/dramatiq/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `dramatiq-1.8.1/dramatiq/middleware/age_limit.py` & `dramatiq-1.9.0/dramatiq/middleware/age_limit.py`

 * *Files identical despite different names*

### Comparing `dramatiq-1.8.1/dramatiq/middleware/callbacks.py` & `dramatiq-1.9.0/dramatiq/middleware/callbacks.py`

 * *Files identical despite different names*

### Comparing `dramatiq-1.8.1/dramatiq/middleware/current_message.py` & `dramatiq-1.9.0/dramatiq/middleware/current_message.py`

 * *Files identical despite different names*

### Comparing `dramatiq-1.8.1/dramatiq/middleware/group_callbacks.py` & `dramatiq-1.9.0/dramatiq/middleware/group_callbacks.py`

 * *Files identical despite different names*

### Comparing `dramatiq-1.8.1/dramatiq/middleware/middleware.py` & `dramatiq-1.9.0/dramatiq/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `dramatiq-1.8.1/dramatiq/middleware/pipelines.py` & `dramatiq-1.9.0/dramatiq/middleware/pipelines.py`

 * *Files identical despite different names*

### Comparing `dramatiq-1.8.1/dramatiq/middleware/prometheus.py` & `dramatiq-1.9.0/dramatiq/middleware/prometheus.py`

 * *Files identical despite different names*

### Comparing `dramatiq-1.8.1/dramatiq/middleware/shutdown.py` & `dramatiq-1.9.0/dramatiq/middleware/shutdown.py`

 * *Files identical despite different names*

### Comparing `dramatiq-1.8.1/dramatiq/middleware/threading.py` & `dramatiq-1.9.0/dramatiq/middleware/threading.py`

 * *Files identical despite different names*

### Comparing `dramatiq-1.8.1/dramatiq/middleware/time_limit.py` & `dramatiq-1.9.0/dramatiq/middleware/time_limit.py`

 * *Files identical despite different names*

### Comparing `dramatiq-1.8.1/dramatiq/rate_limits/__init__.py` & `dramatiq-1.9.0/dramatiq/rate_limits/__init__.py`

 * *Files identical despite different names*

### Comparing `dramatiq-1.8.1/dramatiq/rate_limits/backend.py` & `dramatiq-1.9.0/dramatiq/rate_limits/backend.py`

 * *Files identical despite different names*

### Comparing `dramatiq-1.8.1/dramatiq/rate_limits/backends/__init__.py` & `dramatiq-1.9.0/dramatiq/rate_limits/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `dramatiq-1.8.1/dramatiq/rate_limits/backends/memcached.py` & `dramatiq-1.9.0/dramatiq/rate_limits/backends/memcached.py`

 * *Files identical despite different names*

### Comparing `dramatiq-1.8.1/dramatiq/rate_limits/backends/redis.py` & `dramatiq-1.9.0/dramatiq/rate_limits/backends/redis.py`

 * *Files identical despite different names*

### Comparing `dramatiq-1.8.1/dramatiq/rate_limits/backends/stub.py` & `dramatiq-1.9.0/dramatiq/rate_limits/backends/stub.py`

 * *Files identical despite different names*

### Comparing `dramatiq-1.8.1/dramatiq/rate_limits/barrier.py` & `dramatiq-1.9.0/dramatiq/rate_limits/barrier.py`

 * *Files identical despite different names*

### Comparing `dramatiq-1.8.1/dramatiq/rate_limits/bucket.py` & `dramatiq-1.9.0/dramatiq/rate_limits/bucket.py`

 * *Files identical despite different names*

### Comparing `dramatiq-1.8.1/dramatiq/rate_limits/concurrent.py` & `dramatiq-1.9.0/dramatiq/rate_limits/concurrent.py`

 * *Files identical despite different names*

### Comparing `dramatiq-1.8.1/dramatiq/rate_limits/rate_limiter.py` & `dramatiq-1.9.0/dramatiq/rate_limits/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `dramatiq-1.8.1/dramatiq/rate_limits/window.py` & `dramatiq-1.9.0/dramatiq/rate_limits/window.py`

 * *Files identical despite different names*

### Comparing `dramatiq-1.8.1/dramatiq/results/__init__.py` & `dramatiq-1.9.0/dramatiq/results/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,11 +12,11 @@
 # FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public
 # License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from .backend import Missing, ResultBackend
-from .errors import ResultError, ResultMissing, ResultTimeout
+from .errors import ResultError, ResultFailure, ResultMissing, ResultTimeout
 from .middleware import Results
 
-__all__ = ["Missing", "ResultBackend", "ResultError", "ResultTimeout", "ResultMissing", "Results"]
+__all__ = ["Missing", "ResultBackend", "ResultError", "ResultFailure", "ResultTimeout", "ResultMissing", "Results"]
```

### Comparing `dramatiq-1.8.1/dramatiq/results/backend.py` & `dramatiq-1.9.0/dramatiq/results/backend.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import hashlib
 import time
 import typing
 
 from ..common import compute_backoff, q_name
 from ..encoder import Encoder
 from .errors import ResultMissing, ResultTimeout
+from .result import unwrap_result, wrap_exception, wrap_result
 
 #: The default timeout for blocking get operations in milliseconds.
 DEFAULT_TIMEOUT = 10000
 
 #: The minimum amount of time in ms to wait between polls.
 BACKOFF_FACTOR = 100
 
@@ -89,27 +90,39 @@
                 time.sleep(delay)
                 continue
 
             elif result is Missing:
                 raise ResultMissing(message)
 
             else:
-                return result
+                return unwrap_result(result)
 
     def store_result(self, message, result: Result, ttl: int) -> None:
         """Store a result in the backend.
 
         Parameters:
           message(Message)
           result(object): Must be serializable.
           ttl(int): The maximum amount of time the result may be
             stored in the backend for.
         """
         message_key = self.build_message_key(message)
-        return self._store(message_key, result, ttl)
+        return self._store(message_key, wrap_result(result), ttl)
+
+    def store_exception(self, message, exception: Exception, ttl: int) -> None:
+        """Store an exception in the backend.
+
+        Parameters:
+          message(Message)
+          exception(Exception)
+          ttl(int): The maximum amount of time the exception may be
+            stored in the backend for.
+        """
+        message_key = self.build_message_key(message)
+        return self._store(message_key, wrap_exception(exception), ttl)
 
     def build_message_key(self, message) -> str:
         """Given a message, return its globally-unique key.
 
         Parameters:
           message(Message)
```

### Comparing `dramatiq-1.8.1/dramatiq/results/backends/__init__.py` & `dramatiq-1.9.0/dramatiq/results/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `dramatiq-1.8.1/dramatiq/results/backends/memcached.py` & `dramatiq-1.9.0/dramatiq/results/backends/memcached.py`

 * *Files identical despite different names*

### Comparing `dramatiq-1.8.1/dramatiq/results/backends/redis.py` & `dramatiq-1.9.0/dramatiq/results/backends/redis.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,28 +14,29 @@
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import redis
 
 from ..backend import DEFAULT_TIMEOUT, ResultBackend, ResultMissing, ResultTimeout
+from ..result import unwrap_result
 
 
 class RedisBackend(ResultBackend):
     """A result backend for Redis_.  This is the recommended result
     backend as waiting for a result is resource efficient.
 
     Parameters:
       namespace(str): A string with which to prefix result keys.
       encoder(Encoder): The encoder to use when storing and retrieving
         result data.  Defaults to :class:`.JSONEncoder`.
       client(Redis): An optional client.  If this is passed,
         then all other parameters are ignored.
       url(str): An optional connection URL.  If both a URL and
-        connection paramters are provided, the URL is used.
+        connection parameters are provided, the URL is used.
       **parameters(dict): Connection parameters are passed directly
         to :class:`redis.Redis`.
 
     .. _redis: https://redis.io
     """
 
     def __init__(self, *, namespace="dramatiq-results", encoder=None, client=None, url=None, **parameters):
@@ -81,15 +82,15 @@
                 raise ResultTimeout(message)
 
         else:
             data = self.client.lindex(message_key, 0)
             if data is None:
                 raise ResultMissing(message)
 
-        return self.encoder.decode(data)
+        return unwrap_result(self.encoder.decode(data))
 
     def _store(self, message_key, result, ttl):
         with self.client.pipeline() as pipe:
             pipe.delete(message_key)
             pipe.lpush(message_key, self.encoder.encode(result))
             pipe.pexpire(message_key, ttl)
             pipe.execute()
```

### Comparing `dramatiq-1.8.1/dramatiq/results/backends/stub.py` & `dramatiq-1.9.0/dramatiq/results/backends/stub.py`

 * *Files identical despite different names*

### Comparing `dramatiq-1.8.1/dramatiq/watcher.py` & `dramatiq-1.9.0/dramatiq/watcher.py`

 * *Files identical despite different names*

### Comparing `dramatiq-1.8.1/dramatiq/worker.py` & `dramatiq-1.9.0/dramatiq/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import time
 from collections import defaultdict
 from itertools import chain
 from queue import Empty, PriorityQueue
 from threading import Event, Thread
 
 from .common import current_millis, iter_queue, join_all, q_name
-from .errors import ActorNotFound, ConnectionError, RateLimitExceeded
+from .errors import ActorNotFound, ConnectionError, RateLimitExceeded, Retry
 from .logging import get_logger
 from .middleware import Middleware, SkipMessage
 
 #: The number of milliseconds to wait before restarting consumers
 #: after a connection error.
 CONSUMER_RESTART_DELAY = int(os.getenv("dramatiq_restart_delay", 3000))
 CONSUMER_RESTART_DELAY_SECS = CONSUMER_RESTART_DELAY / 1000
@@ -474,20 +474,24 @@
         except SkipMessage:
             self.logger.warning("Message %s was skipped.", message)
             self.broker.emit_after("skip_message", message)
 
         except BaseException as e:
             # Stuff the exception into the message [proxy] so that it
             # may be used by the stub broker to provide a nicer
-            # testing experience.
+            # testing experience.  Also used by the results middleware
+            # to pass exceptions into results.
             message.stuff_exception(e)
 
+            throws = message.options.get("throws") or actor.options.get("throws")
             if isinstance(e, RateLimitExceeded):
-                self.logger.error("Rate limit exceeded in message %s: %s.", message, e)
-            else:
+                self.logger.debug("Rate limit exceeded in message %s: %s.", message, e)
+            elif throws and isinstance(e, throws):
+                self.logger.info("Failed to process message %s with expected exception %s.", message, type(e).__name__)
+            elif not isinstance(e, Retry):
                 self.logger.error("Failed to process message %s with unhandled exception.", message, exc_info=True)
 
             self.broker.emit_after("process_message", message, exception=e)
 
         finally:
             # NOTE: There is no race here as any message that was
             # processed must have come off of a consumer.  Therefore,
```

### Comparing `dramatiq-1.8.1/dramatiq.egg-info/PKG-INFO` & `dramatiq-1.9.0/dramatiq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dramatiq
-Version: 1.8.1
+Version: 1.9.0
 Summary: Background Processing for Python 3.
 Home-page: UNKNOWN
 Author: Bogdan Popa
 Author-email: bogdan@cleartype.io
 License: UNKNOWN
 Description: <img src="https://dramatiq.io/_static/logo.png" align="right" width="131" />
```

### Comparing `dramatiq-1.8.1/dramatiq.egg-info/SOURCES.txt` & `dramatiq-1.9.0/dramatiq.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -56,11 +56,12 @@
 dramatiq/rate_limits/backends/memcached.py
 dramatiq/rate_limits/backends/redis.py
 dramatiq/rate_limits/backends/stub.py
 dramatiq/results/__init__.py
 dramatiq/results/backend.py
 dramatiq/results/errors.py
 dramatiq/results/middleware.py
+dramatiq/results/result.py
 dramatiq/results/backends/__init__.py
 dramatiq/results/backends/memcached.py
 dramatiq/results/backends/redis.py
 dramatiq/results/backends/stub.py
```

### Comparing `dramatiq-1.8.1/dramatiq.egg-info/requires.txt` & `dramatiq-1.9.0/dramatiq.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 prometheus-client>=0.2
 
 [all]
 watchdog_gevent==0.1
 watchdog<0.9,>=0.8
 pylibmc<2.0,>=1.5
-redis<4.0,>=2.0
 pika<2.0,>=1.0
+redis<4.0,>=2.0
 
 [dev]
 watchdog_gevent==0.1
 watchdog<0.9,>=0.8
 pylibmc<2.0,>=1.5
-redis<4.0,>=2.0
 pika<2.0,>=1.0
+redis<4.0,>=2.0
 alabaster
 sphinx<1.8
 sphinxcontrib-napoleon
 flake8
 flake8-bugbear
 flake8-quotes
 isort
```

### Comparing `dramatiq-1.8.1/setup.py` & `dramatiq-1.9.0/setup.py`

 * *Files identical despite different names*

