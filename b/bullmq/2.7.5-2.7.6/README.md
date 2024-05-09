# Comparing `tmp/bullmq-2.7.5.tar.gz` & `tmp/bullmq-2.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bullmq-2.7.5.tar", last modified: Sun Apr 28 16:59:55 2024, max compression
+gzip compressed data, was "bullmq-2.7.6.tar", last modified: Thu May  9 04:40:07 2024, max compression
```

## Comparing `bullmq-2.7.5.tar` & `bullmq-2.7.6.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:59:55.072276 bullmq-2.7.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-28 16:59:55.072276 bullmq-2.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-28 16:58:55.000000 bullmq-2.7.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:59:55.060276 bullmq-2.7.5/bullmq/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-28 16:59:53.000000 bullmq-2.7.5/bullmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-28 16:58:55.000000 bullmq-2.7.5/bullmq/backoffs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:59:55.068276 bullmq-2.7.5/bullmq/commands/
--rw-r--r--   0 runner    (1001) docker     (127)    10913 2024-04-28 16:59:31.000000 bullmq-2.7.5/bullmq/commands/addDelayedJob-6.lua
--rw-r--r--   0 runner    (1001) docker     (127)    10334 2024-04-28 16:59:31.000000 bullmq-2.7.5/bullmq/commands/addParentJob-4.lua
--rw-r--r--   0 runner    (1001) docker     (127)    10691 2024-04-28 16:59:31.000000 bullmq-2.7.5/bullmq/commands/addPrioritizedJob-7.lua
--rw-r--r--   0 runner    (1001) docker     (127)    10780 2024-04-28 16:59:31.000000 bullmq-2.7.5/bullmq/commands/addStandardJob-7.lua
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-28 16:59:31.000000 bullmq-2.7.5/bullmq/commands/changeDelay-4.lua
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-28 16:59:31.000000 bullmq-2.7.5/bullmq/commands/changePriority-6.lua
--rw-r--r--   0 runner    (1001) docker     (127)     9965 2024-04-28 16:59:31.000000 bullmq-2.7.5/bullmq/commands/cleanJobsInSet-2.lua
--rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-28 16:59:31.000000 bullmq-2.7.5/bullmq/commands/drain-4.lua
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-28 16:59:31.000000 bullmq-2.7.5/bullmq/commands/extendLock-2.lua
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-28 16:59:31.000000 bullmq-2.7.5/bullmq/commands/getCounts-1.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-28 16:59:31.000000 bullmq-2.7.5/bullmq/commands/getRanges-1.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-28 16:59:31.000000 bullmq-2.7.5/bullmq/commands/getState-8.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-28 16:59:31.000000 bullmq-2.7.5/bullmq/commands/getStateV2-8.lua
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-28 16:59:31.000000 bullmq-2.7.5/bullmq/commands/isFinished-3.lua
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-28 16:59:31.000000 bullmq-2.7.5/bullmq/commands/isJobInList-1.lua
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-28 16:59:31.000000 bullmq-2.7.5/bullmq/commands/moveJobFromActiveToWait-10.lua
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-04-28 16:59:31.000000 bullmq-2.7.5/bullmq/commands/moveJobsToWait-7.lua
--rw-r--r--   0 runner    (1001) docker     (127)    18137 2024-04-28 16:59:31.000000 bullmq-2.7.5/bullmq/commands/moveStalledJobsToWait-9.lua
--rw-r--r--   0 runner    (1001) docker     (127)     7295 2024-04-28 16:59:31.000000 bullmq-2.7.5/bullmq/commands/moveToActive-11.lua
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-28 16:59:31.000000 bullmq-2.7.5/bullmq/commands/moveToDelayed-8.lua
--rw-r--r--   0 runner    (1001) docker     (127)    26012 2024-04-28 16:59:31.000000 bullmq-2.7.5/bullmq/commands/moveToFinished-14.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-28 16:59:31.000000 bullmq-2.7.5/bullmq/commands/moveToWaitingChildren-5.lua
--rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-04-28 16:59:31.000000 bullmq-2.7.5/bullmq/commands/obliterate-2.lua
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-04-28 16:59:31.000000 bullmq-2.7.5/bullmq/commands/paginate-1.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-28 16:59:31.000000 bullmq-2.7.5/bullmq/commands/pause-7.lua
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-04-28 16:59:31.000000 bullmq-2.7.5/bullmq/commands/promote-8.lua
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-28 16:59:31.000000 bullmq-2.7.5/bullmq/commands/releaseLock-1.lua
--rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-04-28 16:59:31.000000 bullmq-2.7.5/bullmq/commands/removeChildDependency-1.lua
--rw-r--r--   0 runner    (1001) docker     (127)     9216 2024-04-28 16:59:31.000000 bullmq-2.7.5/bullmq/commands/removeJob-1.lua
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-28 16:59:31.000000 bullmq-2.7.5/bullmq/commands/removeRepeatable-2.lua
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-28 16:59:31.000000 bullmq-2.7.5/bullmq/commands/reprocessJob-7.lua
--rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-04-28 16:59:31.000000 bullmq-2.7.5/bullmq/commands/retryJob-11.lua
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-28 16:59:31.000000 bullmq-2.7.5/bullmq/commands/saveStacktrace-1.lua
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-28 16:59:31.000000 bullmq-2.7.5/bullmq/commands/updateData-1.lua
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-28 16:59:31.000000 bullmq-2.7.5/bullmq/commands/updateProgress-3.lua
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:59:55.068276 bullmq-2.7.5/bullmq/custom_errors/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-28 16:58:55.000000 bullmq-2.7.5/bullmq/custom_errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-28 16:58:55.000000 bullmq-2.7.5/bullmq/custom_errors/waiting_children_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-28 16:58:55.000000 bullmq-2.7.5/bullmq/error_code.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-28 16:58:55.000000 bullmq-2.7.5/bullmq/event_emitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4621 2024-04-28 16:58:55.000000 bullmq-2.7.5/bullmq/flow_producer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10457 2024-04-28 16:58:55.000000 bullmq-2.7.5/bullmq/job.py
--rw-r--r--   0 runner    (1001) docker     (127)    10683 2024-04-28 16:58:55.000000 bullmq-2.7.5/bullmq/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-28 16:58:55.000000 bullmq-2.7.5/bullmq/queue_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-28 16:58:55.000000 bullmq-2.7.5/bullmq/redis_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    24462 2024-04-28 16:58:55.000000 bullmq-2.7.5/bullmq/scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-28 16:58:55.000000 bullmq-2.7.5/bullmq/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:59:55.068276 bullmq-2.7.5/bullmq/types/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-28 16:58:55.000000 bullmq-2.7.5/bullmq/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-28 16:58:55.000000 bullmq-2.7.5/bullmq/types/backoff_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-28 16:58:55.000000 bullmq-2.7.5/bullmq/types/job_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-28 16:58:55.000000 bullmq-2.7.5/bullmq/types/keep_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-28 16:58:55.000000 bullmq-2.7.5/bullmq/types/promote_jobs_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-28 16:58:55.000000 bullmq-2.7.5/bullmq/types/queue_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-28 16:58:55.000000 bullmq-2.7.5/bullmq/types/retry_jobs_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-28 16:58:55.000000 bullmq-2.7.5/bullmq/types/worker_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-28 16:58:55.000000 bullmq-2.7.5/bullmq/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10537 2024-04-28 16:58:55.000000 bullmq-2.7.5/bullmq/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:59:55.072276 bullmq-2.7.5/bullmq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-28 16:59:55.000000 bullmq-2.7.5/bullmq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-28 16:59:55.000000 bullmq-2.7.5/bullmq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 16:59:55.000000 bullmq-2.7.5/bullmq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-28 16:59:55.000000 bullmq-2.7.5/bullmq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-28 16:59:55.000000 bullmq-2.7.5/bullmq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-28 16:59:53.000000 bullmq-2.7.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 16:59:55.072276 bullmq-2.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-28 16:58:55.000000 bullmq-2.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:40:07.742522 bullmq-2.7.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-09 04:40:07.742522 bullmq-2.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-09 04:39:10.000000 bullmq-2.7.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:40:07.730522 bullmq-2.7.6/bullmq/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-09 04:40:05.000000 bullmq-2.7.6/bullmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-09 04:39:10.000000 bullmq-2.7.6/bullmq/backoffs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:40:07.738522 bullmq-2.7.6/bullmq/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)    10913 2024-05-09 04:39:44.000000 bullmq-2.7.6/bullmq/commands/addDelayedJob-6.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    10334 2024-05-09 04:39:44.000000 bullmq-2.7.6/bullmq/commands/addParentJob-4.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    10691 2024-05-09 04:39:44.000000 bullmq-2.7.6/bullmq/commands/addPrioritizedJob-7.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    10780 2024-05-09 04:39:44.000000 bullmq-2.7.6/bullmq/commands/addStandardJob-7.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-09 04:39:44.000000 bullmq-2.7.6/bullmq/commands/changeDelay-4.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-09 04:39:44.000000 bullmq-2.7.6/bullmq/commands/changePriority-6.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     9965 2024-05-09 04:39:44.000000 bullmq-2.7.6/bullmq/commands/cleanJobsInSet-2.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-05-09 04:39:44.000000 bullmq-2.7.6/bullmq/commands/drain-4.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-09 04:39:44.000000 bullmq-2.7.6/bullmq/commands/extendLock-2.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-09 04:39:44.000000 bullmq-2.7.6/bullmq/commands/getCounts-1.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-09 04:39:44.000000 bullmq-2.7.6/bullmq/commands/getRanges-1.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-09 04:39:44.000000 bullmq-2.7.6/bullmq/commands/getState-8.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-09 04:39:44.000000 bullmq-2.7.6/bullmq/commands/getStateV2-8.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-09 04:39:44.000000 bullmq-2.7.6/bullmq/commands/isFinished-3.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-09 04:39:44.000000 bullmq-2.7.6/bullmq/commands/isJobInList-1.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-09 04:39:44.000000 bullmq-2.7.6/bullmq/commands/moveJobFromActiveToWait-10.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-05-09 04:39:44.000000 bullmq-2.7.6/bullmq/commands/moveJobsToWait-7.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    18137 2024-05-09 04:39:44.000000 bullmq-2.7.6/bullmq/commands/moveStalledJobsToWait-9.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     7295 2024-05-09 04:39:44.000000 bullmq-2.7.6/bullmq/commands/moveToActive-11.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-05-09 04:39:44.000000 bullmq-2.7.6/bullmq/commands/moveToDelayed-8.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    26012 2024-05-09 04:39:44.000000 bullmq-2.7.6/bullmq/commands/moveToFinished-14.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-09 04:39:44.000000 bullmq-2.7.6/bullmq/commands/moveToWaitingChildren-5.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-05-09 04:39:44.000000 bullmq-2.7.6/bullmq/commands/obliterate-2.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-09 04:39:44.000000 bullmq-2.7.6/bullmq/commands/paginate-1.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-09 04:39:44.000000 bullmq-2.7.6/bullmq/commands/pause-7.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-05-09 04:39:44.000000 bullmq-2.7.6/bullmq/commands/promote-8.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-09 04:39:44.000000 bullmq-2.7.6/bullmq/commands/releaseLock-1.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-05-09 04:39:44.000000 bullmq-2.7.6/bullmq/commands/removeChildDependency-1.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     9216 2024-05-09 04:39:44.000000 bullmq-2.7.6/bullmq/commands/removeJob-1.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-09 04:39:44.000000 bullmq-2.7.6/bullmq/commands/removeRepeatable-2.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-09 04:39:44.000000 bullmq-2.7.6/bullmq/commands/reprocessJob-7.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-05-09 04:39:44.000000 bullmq-2.7.6/bullmq/commands/retryJob-11.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-09 04:39:44.000000 bullmq-2.7.6/bullmq/commands/saveStacktrace-1.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-09 04:39:44.000000 bullmq-2.7.6/bullmq/commands/updateData-1.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-09 04:39:44.000000 bullmq-2.7.6/bullmq/commands/updateProgress-3.lua
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:40:07.738522 bullmq-2.7.6/bullmq/custom_errors/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-09 04:39:10.000000 bullmq-2.7.6/bullmq/custom_errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-09 04:39:10.000000 bullmq-2.7.6/bullmq/custom_errors/waiting_children_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-09 04:39:10.000000 bullmq-2.7.6/bullmq/error_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-09 04:39:10.000000 bullmq-2.7.6/bullmq/event_emitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4621 2024-05-09 04:39:10.000000 bullmq-2.7.6/bullmq/flow_producer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10457 2024-05-09 04:39:10.000000 bullmq-2.7.6/bullmq/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10683 2024-05-09 04:39:10.000000 bullmq-2.7.6/bullmq/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-09 04:39:10.000000 bullmq-2.7.6/bullmq/queue_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-09 04:39:10.000000 bullmq-2.7.6/bullmq/redis_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24462 2024-05-09 04:39:10.000000 bullmq-2.7.6/bullmq/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-09 04:39:10.000000 bullmq-2.7.6/bullmq/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:40:07.738522 bullmq-2.7.6/bullmq/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-09 04:39:10.000000 bullmq-2.7.6/bullmq/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-09 04:39:10.000000 bullmq-2.7.6/bullmq/types/backoff_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-09 04:39:10.000000 bullmq-2.7.6/bullmq/types/job_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-09 04:39:10.000000 bullmq-2.7.6/bullmq/types/keep_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-09 04:39:10.000000 bullmq-2.7.6/bullmq/types/promote_jobs_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-09 04:39:10.000000 bullmq-2.7.6/bullmq/types/queue_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-09 04:39:10.000000 bullmq-2.7.6/bullmq/types/retry_jobs_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-09 04:39:10.000000 bullmq-2.7.6/bullmq/types/worker_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-09 04:39:10.000000 bullmq-2.7.6/bullmq/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10537 2024-05-09 04:39:10.000000 bullmq-2.7.6/bullmq/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:40:07.738522 bullmq-2.7.6/bullmq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-09 04:40:07.000000 bullmq-2.7.6/bullmq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-09 04:40:07.000000 bullmq-2.7.6/bullmq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 04:40:07.000000 bullmq-2.7.6/bullmq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-09 04:40:07.000000 bullmq-2.7.6/bullmq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-09 04:40:07.000000 bullmq-2.7.6/bullmq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-09 04:40:05.000000 bullmq-2.7.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 04:40:07.742522 bullmq-2.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-09 04:39:10.000000 bullmq-2.7.6/setup.py
```

### Comparing `bullmq-2.7.5/PKG-INFO` & `bullmq-2.7.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 2.7.5
+Version: 2.7.6
 Summary: BullMQ for Python
 Author-email: "Taskforce.sh Inc." <manast@taskforce.sh>
 Project-URL: Homepage, https://bullmq.io
 Project-URL: Bug Tracker, https://github.com/taskforcesh/bullmq/issues
 Keywords: python,bullmq,queues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bullmq-2.7.5/README.md` & `bullmq-2.7.6/README.md`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/bullmq/backoffs.py` & `bullmq-2.7.6/bullmq/backoffs.py`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/bullmq/commands/addDelayedJob-6.lua` & `bullmq-2.7.6/bullmq/commands/addDelayedJob-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/bullmq/commands/addParentJob-4.lua` & `bullmq-2.7.6/bullmq/commands/addParentJob-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/bullmq/commands/addPrioritizedJob-7.lua` & `bullmq-2.7.6/bullmq/commands/addPrioritizedJob-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/bullmq/commands/addStandardJob-7.lua` & `bullmq-2.7.6/bullmq/commands/addStandardJob-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/bullmq/commands/changeDelay-4.lua` & `bullmq-2.7.6/bullmq/commands/changeDelay-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/bullmq/commands/changePriority-6.lua` & `bullmq-2.7.6/bullmq/commands/changePriority-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/bullmq/commands/cleanJobsInSet-2.lua` & `bullmq-2.7.6/bullmq/commands/cleanJobsInSet-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/bullmq/commands/drain-4.lua` & `bullmq-2.7.6/bullmq/commands/drain-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/bullmq/commands/getCounts-1.lua` & `bullmq-2.7.6/bullmq/commands/getCounts-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/bullmq/commands/getRanges-1.lua` & `bullmq-2.7.6/bullmq/commands/getRanges-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/bullmq/commands/getState-8.lua` & `bullmq-2.7.6/bullmq/commands/getState-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/bullmq/commands/getStateV2-8.lua` & `bullmq-2.7.6/bullmq/commands/getStateV2-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/bullmq/commands/isFinished-3.lua` & `bullmq-2.7.6/bullmq/commands/isFinished-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/bullmq/commands/moveJobFromActiveToWait-10.lua` & `bullmq-2.7.6/bullmq/commands/moveJobFromActiveToWait-10.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/bullmq/commands/moveJobsToWait-7.lua` & `bullmq-2.7.6/bullmq/commands/moveJobsToWait-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/bullmq/commands/moveStalledJobsToWait-9.lua` & `bullmq-2.7.6/bullmq/commands/moveStalledJobsToWait-9.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/bullmq/commands/moveToActive-11.lua` & `bullmq-2.7.6/bullmq/commands/moveToActive-11.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/bullmq/commands/moveToDelayed-8.lua` & `bullmq-2.7.6/bullmq/commands/moveToDelayed-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/bullmq/commands/moveToFinished-14.lua` & `bullmq-2.7.6/bullmq/commands/moveToFinished-14.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/bullmq/commands/moveToWaitingChildren-5.lua` & `bullmq-2.7.6/bullmq/commands/moveToWaitingChildren-5.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/bullmq/commands/obliterate-2.lua` & `bullmq-2.7.6/bullmq/commands/obliterate-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/bullmq/commands/paginate-1.lua` & `bullmq-2.7.6/bullmq/commands/paginate-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/bullmq/commands/pause-7.lua` & `bullmq-2.7.6/bullmq/commands/pause-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/bullmq/commands/promote-8.lua` & `bullmq-2.7.6/bullmq/commands/promote-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/bullmq/commands/removeChildDependency-1.lua` & `bullmq-2.7.6/bullmq/commands/removeChildDependency-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/bullmq/commands/removeJob-1.lua` & `bullmq-2.7.6/bullmq/commands/removeJob-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/bullmq/commands/removeRepeatable-2.lua` & `bullmq-2.7.6/bullmq/commands/removeRepeatable-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/bullmq/commands/reprocessJob-7.lua` & `bullmq-2.7.6/bullmq/commands/reprocessJob-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/bullmq/commands/retryJob-11.lua` & `bullmq-2.7.6/bullmq/commands/retryJob-11.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/bullmq/commands/updateProgress-3.lua` & `bullmq-2.7.6/bullmq/commands/updateProgress-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/bullmq/event_emitter.py` & `bullmq-2.7.6/bullmq/event_emitter.py`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/bullmq/flow_producer.py` & `bullmq-2.7.6/bullmq/flow_producer.py`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/bullmq/job.py` & `bullmq-2.7.6/bullmq/job.py`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/bullmq/queue.py` & `bullmq-2.7.6/bullmq/queue.py`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/bullmq/queue_keys.py` & `bullmq-2.7.6/bullmq/queue_keys.py`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/bullmq/redis_connection.py` & `bullmq-2.7.6/bullmq/redis_connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import redis.asyncio as redis
 from redis.backoff import ExponentialBackoff
-from redis.retry import Retry
+from redis.asyncio.retry import Retry
 from redis.exceptions import (
    BusyLoadingError,
    ConnectionError,
    TimeoutError
 )
 import warnings
 from bullmq.utils import isRedisVersionLowerThan
```

### Comparing `bullmq-2.7.5/bullmq/scripts.py` & `bullmq-2.7.6/bullmq/scripts.py`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/bullmq/timer.py` & `bullmq-2.7.6/bullmq/timer.py`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/bullmq/types/job_options.py` & `bullmq-2.7.6/bullmq/types/job_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/bullmq/types/worker_options.py` & `bullmq-2.7.6/bullmq/types/worker_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/bullmq/utils.py` & `bullmq-2.7.6/bullmq/utils.py`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/bullmq/worker.py` & `bullmq-2.7.6/bullmq/worker.py`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/bullmq.egg-info/PKG-INFO` & `bullmq-2.7.6/bullmq.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 2.7.5
+Version: 2.7.6
 Summary: BullMQ for Python
 Author-email: "Taskforce.sh Inc." <manast@taskforce.sh>
 Project-URL: Homepage, https://bullmq.io
 Project-URL: Bug Tracker, https://github.com/taskforcesh/bullmq/issues
 Keywords: python,bullmq,queues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bullmq-2.7.5/bullmq.egg-info/SOURCES.txt` & `bullmq-2.7.6/bullmq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.5/pyproject.toml` & `bullmq-2.7.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bullmq"
-version = "2.7.5"
+version = "2.7.6"
 description='BullMQ for Python'
 readme="README.md"
 authors = [
     {name = "Taskforce.sh Inc.", email = "manast@taskforce.sh"},
 ]
 requires-python = ">=3.10.0"
 classifiers=[
```

