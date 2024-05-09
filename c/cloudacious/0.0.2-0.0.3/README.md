# Comparing `tmp/cloudacious-0.0.2.tar.gz` & `tmp/cloudacious-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "cloudacious-0.0.3.tar", max compression
```

## Comparing `cloudacious-0.0.2.tar` & `cloudacious-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,4 @@
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 cloudacious-0.0.2/.gitlab-ci.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudacious-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cloudacious-0.0.2/.pypirc
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 cloudacious-0.0.2/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudacious-0.0.2/config.cfg
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 cloudacious-0.0.2/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudacious-0.0.2/src/cloudacious/README.md
--rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 cloudacious-0.0.2/src/cloudacious/iac/ContainerImages.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudacious-0.0.2/src/cloudacious/iac/README.md
--rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 cloudacious-0.0.2/.gitignore
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 cloudacious-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 cloudacious-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      838 2024-05-09 19:05:25.275543 cloudacious-0.0.3/README.md
+-rw-r--r--   0        0        0      435 2024-05-09 19:13:59.641769 cloudacious-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1014 2024-05-08 04:21:55.701008 cloudacious-0.0.3/src/cloudacious/Dynamo.py
+-rw-r--r--   0        0        0     1246 1970-01-01 00:00:00.000000 cloudacious-0.0.3/PKG-INFO
```

