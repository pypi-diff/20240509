# Comparing `tmp/ocdsmerge-0.6.6.tar.gz` & `tmp/ocdsmerge-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ocdsmerge-0.6.6.tar", last modified: Sat Apr 10 22:32:24 2021, max compression
+gzip compressed data, was "ocdsmerge-0.7.0.tar", last modified: Thu May  9 01:28:31 2024, max compression
```

## Comparing `ocdsmerge-0.6.6.tar` & `ocdsmerge-0.7.0.tar`

### file list

```diff
@@ -1,138 +1,139 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2021-04-10 22:32:24.000000 ocdsmerge-0.6.6/
--rw-r--r--   0 james      (501) staff       (20)     2598 2021-04-10 22:32:24.000000 ocdsmerge-0.6.6/PKG-INFO
-drwxr-xr-x   0 james      (501) staff       (20)        0 2021-04-10 22:32:24.000000 ocdsmerge-0.6.6/ocdsmerge.egg-info/
--rw-r--r--   0 james      (501) staff       (20)     2598 2021-04-10 22:32:24.000000 ocdsmerge-0.6.6/ocdsmerge.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     5323 2021-04-10 22:32:24.000000 ocdsmerge-0.6.6/ocdsmerge.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)       75 2021-04-10 22:32:24.000000 ocdsmerge-0.6.6/ocdsmerge.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)       10 2021-04-10 22:32:24.000000 ocdsmerge-0.6.6/ocdsmerge.egg-info/top_level.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2021-04-10 22:32:24.000000 ocdsmerge-0.6.6/ocdsmerge.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)     1494 2017-08-16 14:22:52.000000 ocdsmerge-0.6.6/LICENSE
-drwxr-xr-x   0 james      (501) staff       (20)        0 2021-04-10 22:32:24.000000 ocdsmerge-0.6.6/tests/
--rw-r--r--   0 james      (501) staff       (20)      977 2020-01-01 02:57:08.000000 ocdsmerge-0.6.6/tests/test_flatten.py
--rw-r--r--   0 james      (501) staff       (20)      379 2019-12-30 18:26:33.000000 ocdsmerge-0.6.6/tests/conftest.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2021-04-10 22:32:24.000000 ocdsmerge-0.6.6/tests/cassettes/
--rw-r--r--   0 james      (501) staff       (20)   109677 2020-04-08 04:05:49.000000 ocdsmerge-0.6.6/tests/cassettes/test_warn.yaml
--rw-r--r--   0 james      (501) staff       (20)    79755 2020-04-08 04:05:49.000000 ocdsmerge-0.6.6/tests/cassettes/test_merge.yaml
--rw-r--r--   0 james      (501) staff       (20)      471 2019-12-30 03:31:37.000000 ocdsmerge-0.6.6/tests/__init__.py
--rw-r--r--   0 james      (501) staff       (20)      504 2020-04-08 04:49:26.000000 ocdsmerge-0.6.6/tests/test_util.py
--rw-r--r--   0 james      (501) staff       (20)     7755 2021-03-05 02:10:37.000000 ocdsmerge-0.6.6/tests/test_merge.py
--rw-r--r--   0 james      (501) staff       (20)     2999 2020-01-06 02:11:00.000000 ocdsmerge-0.6.6/tests/test_collisions.py
--rw-r--r--   0 james      (501) staff       (20)     2365 2020-10-02 18:46:13.000000 ocdsmerge-0.6.6/tests/test_fixtures.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2021-04-10 22:32:24.000000 ocdsmerge-0.6.6/tests/fixtures/
--rw-r--r--   0 james      (501) staff       (20)    87980 2019-07-29 15:57:59.000000 ocdsmerge-0.6.6/tests/fixtures/release-schema-1__1__4.json
-drwxr-xr-x   0 james      (501) staff       (20)        0 2021-04-10 22:32:24.000000 ocdsmerge-0.6.6/tests/fixtures/1.0/
--rw-r--r--   0 james      (501) staff       (20)      566 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/1.0/suppliers-versioned.json
--rw-r--r--   0 james      (501) staff       (20)      323 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/1.0/suppliers-compiled.json
--rw-r--r--   0 james      (501) staff       (20)      659 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/1.0/suppliers.json
-drwxr-xr-x   0 james      (501) staff       (20)        0 2021-04-10 22:32:24.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/
--rw-r--r--   0 james      (501) staff       (20)      466 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/simple.json
--rw-r--r--   0 james      (501) staff       (20)      230 2019-03-26 21:18:46.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/initial-null.json
--rw-r--r--   0 james      (501) staff       (20)      245 2019-03-27 16:15:22.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/empty-object-compiled.json
--rw-r--r--   0 james      (501) staff       (20)      171 2019-03-27 01:32:50.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/single-empty-object-compiled.json
--rw-r--r--   0 james      (501) staff       (20)      212 2019-03-27 01:33:37.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/single-empty-object-versioned.json
--rw-r--r--   0 james      (501) staff       (20)      664 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/string-list.json
--rw-r--r--   0 james      (501) staff       (20)      785 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/simple-versioned.json
--rw-r--r--   0 james      (501) staff       (20)      480 2019-03-27 15:59:04.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/single-empty-wholelistmerge-array-versioned.json
--rw-r--r--   0 james      (501) staff       (20)      243 2019-03-27 15:50:58.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/fill-identifiermerge-array-compiled.json
--rw-r--r--   0 james      (501) staff       (20)     2124 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/mergeid-versioned.json
--rw-r--r--   0 james      (501) staff       (20)      610 2019-03-26 21:20:39.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/initial-null-versioned.json
--rw-r--r--   0 james      (501) staff       (20)     1615 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/lists-versioned.json
--rw-r--r--   0 james      (501) staff       (20)      175 2019-03-27 15:50:58.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/single-empty-identifiermerge-array.json
--rw-r--r--   0 james      (501) staff       (20)      498 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/mergeid-compiled.json
--rw-r--r--   0 james      (501) staff       (20)      474 2019-03-27 16:15:41.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/empty-object-versioned.json
--rw-r--r--   0 james      (501) staff       (20)      304 2019-03-27 16:02:19.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/fill-wholelistmerge-array-compiled.json
--rw-r--r--   0 james      (501) staff       (20)      562 2019-03-27 15:43:10.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/empty-wholelistmerge-array.json
--rw-r--r--   0 james      (501) staff       (20)      419 2019-03-27 15:50:58.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/fill-identifiermerge-array.json
--rw-r--r--   0 james      (501) staff       (20)      204 2019-03-26 21:21:01.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/initial-null-compiled.json
--rw-r--r--   0 james      (501) staff       (20)      312 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/string-list-compiled.json
--rw-r--r--   0 james      (501) staff       (20)      758 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/contextual-compiled.json
--rw-r--r--   0 james      (501) staff       (20)      466 2019-03-27 15:50:58.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/empty-identifiermerge-array-versioned.json
--rw-r--r--   0 james      (501) staff       (20)      823 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/contextual.json
--rw-r--r--   0 james      (501) staff       (20)      845 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/mergeid.json
--rw-r--r--   0 james      (501) staff       (20)      725 2019-03-27 15:44:03.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/empty-wholelistmerge-array-versioned.json
--rw-r--r--   0 james      (501) staff       (20)      373 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/unit-compiled.json
--rw-r--r--   0 james      (501) staff       (20)      254 2019-03-27 15:56:22.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/single-empty-wholelistmerge-array.json
--rw-r--r--   0 james      (501) staff       (20)     1098 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/lists.json
--rw-r--r--   0 james      (501) staff       (20)      237 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/simple-compiled.json
--rw-r--r--   0 james      (501) staff       (20)      427 2019-03-27 16:15:09.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/empty-object.json
--rw-r--r--   0 james      (501) staff       (20)     1460 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/unit-versioned.json
--rw-r--r--   0 james      (501) staff       (20)      419 2019-03-27 15:50:58.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/empty-identifiermerge-array.json
--rw-r--r--   0 james      (501) staff       (20)      209 2019-03-27 15:50:58.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/single-empty-identifiermerge-array-versioned.json
--rw-r--r--   0 james      (501) staff       (20)      464 2019-03-26 21:03:58.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/null.json
--rw-r--r--   0 james      (501) staff       (20)      171 2019-03-27 15:50:58.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/single-empty-identifiermerge-array-compiled.json
--rw-r--r--   0 james      (501) staff       (20)      725 2019-03-27 16:02:05.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/fill-wholelistmerge-array-versioned.json
--rw-r--r--   0 james      (501) staff       (20)      255 2019-03-27 15:59:20.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/single-empty-wholelistmerge-array-compiled.json
--rw-r--r--   0 james      (501) staff       (20)      396 2019-03-27 01:39:14.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/fill-object.json
--rw-r--r--   0 james      (501) staff       (20)     2389 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/contextual-versioned.json
--rw-r--r--   0 james      (501) staff       (20)      504 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/lists-compiled.json
--rw-r--r--   0 james      (501) staff       (20)      783 2019-03-26 21:08:22.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/null-versioned.json
--rw-r--r--   0 james      (501) staff       (20)     1165 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/string-list-versioned.json
--rw-r--r--   0 james      (501) staff       (20)      255 2019-03-27 15:24:04.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/empty-wholelistmerge-array-compiled.json
--rw-r--r--   0 james      (501) staff       (20)      562 2019-03-27 16:01:12.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/fill-wholelistmerge-array.json
--rw-r--r--   0 james      (501) staff       (20)      740 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/unit.json
--rw-r--r--   0 james      (501) staff       (20)      204 2019-03-27 16:13:59.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/single-empty-object.json
--rw-r--r--   0 james      (501) staff       (20)      204 2019-03-26 21:08:53.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/null-compiled.json
--rw-r--r--   0 james      (501) staff       (20)      435 2019-03-27 01:39:06.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/fill-object-versioned.json
--rw-r--r--   0 james      (501) staff       (20)      472 2019-03-27 15:50:58.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/fill-identifiermerge-array-versioned.json
--rw-r--r--   0 james      (501) staff       (20)      218 2019-03-27 01:23:29.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/fill-object-compiled.json
--rw-r--r--   0 james      (501) staff       (20)      243 2019-03-27 15:50:58.000000 ocdsmerge-0.6.6/tests/fixtures/1.1/empty-identifiermerge-array-compiled.json
--rw-r--r--   0 james      (501) staff       (20)    65422 2019-07-29 15:57:50.000000 ocdsmerge-0.6.6/tests/fixtures/release-schema-1__0__3.json
--rw-r--r--   0 james      (501) staff       (20)     3087 2019-03-27 17:16:40.000000 ocdsmerge-0.6.6/tests/fixtures/README.md
-drwxr-xr-x   0 james      (501) staff       (20)        0 2021-04-10 22:32:24.000000 ocdsmerge-0.6.6/tests/fixtures/schema/
--rw-r--r--   0 james      (501) staff       (20)      445 2019-12-29 21:52:07.000000 ocdsmerge-0.6.6/tests/fixtures/schema/identifier-merge-duplicate-id-by-position.json
--rw-r--r--   0 james      (501) staff       (20)      576 2020-01-05 19:08:58.000000 ocdsmerge-0.6.6/tests/fixtures/schema/identifier-merge-duplicate-id-append.json
--rw-r--r--   0 james      (501) staff       (20)      215 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/schema/identifier-merge-collision-compiled.json
--rw-r--r--   0 james      (501) staff       (20)      667 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/schema/deep-whole-list-merge.json
--rw-r--r--   0 james      (501) staff       (20)      353 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/schema/whole-list-merge-no-id.json
--rw-r--r--   0 james      (501) staff       (20)      311 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/schema/whole-list-merge-object.json
--rw-r--r--   0 james      (501) staff       (20)      510 2019-12-29 21:52:07.000000 ocdsmerge-0.6.6/tests/fixtures/schema/identifier-merge-duplicate-id.json
--rw-r--r--   0 james      (501) staff       (20)      513 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/schema/no-top-level-id.json
--rw-r--r--   0 james      (501) staff       (20)      136 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/schema/omit-when-merged-array-of-non-objects.json
--rw-r--r--   0 james      (501) staff       (20)      361 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/schema/no-top-level-id-compiled.json
--rw-r--r--   0 james      (501) staff       (20)      398 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/schema/deep-identifier-merge-compiled.json
--rw-r--r--   0 james      (501) staff       (20)      355 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/schema/deep-whole-list-merge-compiled.json
--rw-r--r--   0 james      (501) staff       (20)      569 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/schema/version-id.json
--rw-r--r--   0 james      (501) staff       (20)      190 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/schema/deep-omit-when-merged.json
--rw-r--r--   0 james      (501) staff       (20)      315 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/schema/whole-list-merge-empty.json
--rw-r--r--   0 james      (501) staff       (20)      195 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/schema/deep-omit-when-merged-compiled.json
--rw-r--r--   0 james      (501) staff       (20)      235 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/schema/whole-list-merge-duplicate-id-compiled.json
--rw-r--r--   0 james      (501) staff       (20)      380 2019-12-29 21:52:07.000000 ocdsmerge-0.6.6/tests/fixtures/schema/identifier-merge-duplicate-id-compiled.json
--rw-r--r--   0 james      (501) staff       (20)      369 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/schema/merge-property-is-false.json
--rw-r--r--   0 james      (501) staff       (20)      282 2020-01-06 02:34:08.000000 ocdsmerge-0.6.6/tests/fixtures/schema/identifier-merge-no-id.json
--rw-r--r--   0 james      (501) staff       (20)      251 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/schema/merge-property-is-false-compiled.json
--rw-r--r--   0 james      (501) staff       (20)      201 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/schema/whole-list-merge-no-id-compiled.json
--rw-r--r--   0 james      (501) staff       (20)      209 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/schema/whole-list-merge-object-compiled.json
--rw-r--r--   0 james      (501) staff       (20)      201 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/schema/whole-list-merge-duplicate-id.json
--rw-r--r--   0 james      (501) staff       (20)      181 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/schema/identifier-merge-collision.json
--rw-r--r--   0 james      (501) staff       (20)      241 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/schema/omit-when-merged-shadowed-compiled.json
--rw-r--r--   0 james      (501) staff       (20)      203 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/schema/omit-when-merged-shadowed.json
--rw-r--r--   0 james      (501) staff       (20)      171 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/schema/whole-list-merge-empty-compiled.json
--rw-r--r--   0 james      (501) staff       (20)      574 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/schema/deep-identifier-merge.json
--rw-r--r--   0 james      (501) staff       (20)      141 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/schema/omit-when-merged-array-of-non-objects-compiled.json
--rw-r--r--   0 james      (501) staff       (20)      399 2020-01-06 02:34:09.000000 ocdsmerge-0.6.6/tests/fixtures/schema/identifier-merge-no-id-append.json
--rw-r--r--   0 james      (501) staff       (20)     1085 2019-01-22 21:08:42.000000 ocdsmerge-0.6.6/tests/fixtures/schema/version-id-versioned.json
--rw-r--r--   0 james      (501) staff       (20)    63895 2019-07-29 15:58:16.000000 ocdsmerge-0.6.6/tests/fixtures/versioned-release-validation-schema-1__0__3.json
--rw-r--r--   0 james      (501) staff       (20)     5385 2020-01-06 02:37:04.000000 ocdsmerge-0.6.6/tests/fixtures/schema.json
--rw-r--r--   0 james      (501) staff       (20)    73891 2019-07-29 15:58:25.000000 ocdsmerge-0.6.6/tests/fixtures/versioned-release-validation-schema-1__1__4.json
--rw-r--r--   0 james      (501) staff       (20)     2874 2019-12-29 21:52:07.000000 ocdsmerge-0.6.6/tests/test_rules.py
--rw-r--r--   0 james      (501) staff       (20)      225 2021-04-10 21:52:35.000000 ocdsmerge-0.6.6/MANIFEST.in
-drwxr-xr-x   0 james      (501) staff       (20)        0 2021-04-10 22:32:24.000000 ocdsmerge-0.6.6/docs/
--rw-r--r--   0 james      (501) staff       (20)     2202 2021-02-20 00:46:35.000000 ocdsmerge-0.6.6/docs/index.rst
--rw-r--r--   0 james      (501) staff       (20)     5577 2020-11-25 21:24:44.000000 ocdsmerge-0.6.6/docs/create-merged-releases.rst
--rw-r--r--   0 james      (501) staff       (20)      634 2020-03-13 04:03:43.000000 ocdsmerge-0.6.6/docs/Makefile
--rw-r--r--   0 james      (501) staff       (20)     2599 2021-04-10 21:43:18.000000 ocdsmerge-0.6.6/docs/conf.py
--rw-r--r--   0 james      (501) staff       (20)     3065 2020-11-25 21:24:52.000000 ocdsmerge-0.6.6/docs/update-merged-releases.rst
--rw-r--r--   0 james      (501) staff       (20)     3894 2020-11-25 21:24:47.000000 ocdsmerge-0.6.6/docs/handle-bad-data.rst
-drwxr-xr-x   0 james      (501) staff       (20)        0 2021-04-10 22:32:24.000000 ocdsmerge-0.6.6/docs/api/
--rw-r--r--   0 james      (501) staff       (20)      934 2021-03-05 02:21:05.000000 ocdsmerge-0.6.6/docs/api/index.rst
--rw-r--r--   0 james      (501) staff       (20)    10882 2021-04-10 22:16:33.000000 ocdsmerge-0.6.6/docs/changelog.rst
--rw-r--r--   0 james      (501) staff       (20)     1123 2021-04-10 21:45:38.000000 ocdsmerge-0.6.6/setup.py
--rw-r--r--   0 james      (501) staff       (20)       38 2021-04-10 22:32:24.000000 ocdsmerge-0.6.6/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)     1775 2021-02-20 02:02:41.000000 ocdsmerge-0.6.6/README.rst
-drwxr-xr-x   0 james      (501) staff       (20)        0 2021-04-10 22:32:24.000000 ocdsmerge-0.6.6/ocdsmerge/
--rw-r--r--   0 james      (501) staff       (20)     5145 2020-08-19 22:09:04.000000 ocdsmerge-0.6.6/ocdsmerge/merge.py
--rw-r--r--   0 james      (501) staff       (20)     8284 2021-03-05 02:22:24.000000 ocdsmerge-0.6.6/ocdsmerge/flatten.py
--rw-r--r--   0 james      (501) staff       (20)     2599 2020-04-08 04:49:10.000000 ocdsmerge-0.6.6/ocdsmerge/util.py
--rw-r--r--   0 james      (501) staff       (20)      136 2019-12-29 21:52:01.000000 ocdsmerge-0.6.6/ocdsmerge/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     3045 2019-12-30 04:24:06.000000 ocdsmerge-0.6.6/ocdsmerge/rules.py
--rw-r--r--   0 james      (501) staff       (20)     1256 2021-03-05 01:57:57.000000 ocdsmerge-0.6.6/ocdsmerge/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:28:31.213497 ocdsmerge-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-09 01:28:31.213497 ocdsmerge-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:28:31.193497 ocdsmerge-0.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:28:31.193497 ocdsmerge-0.7.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11174 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/docs/create-merged-releases.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/docs/handle-bad-data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/docs/update-merged-releases.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:28:31.193497 ocdsmerge-0.7.0/ocdsmerge/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/ocdsmerge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/ocdsmerge/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8735 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/ocdsmerge/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/ocdsmerge/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/ocdsmerge/rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/ocdsmerge/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:28:31.213497 ocdsmerge-0.7.0/ocdsmerge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-09 01:28:31.000000 ocdsmerge-0.7.0/ocdsmerge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-05-09 01:28:31.000000 ocdsmerge-0.7.0/ocdsmerge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 01:28:31.000000 ocdsmerge-0.7.0/ocdsmerge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-09 01:28:31.000000 ocdsmerge-0.7.0/ocdsmerge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 01:28:31.000000 ocdsmerge-0.7.0/ocdsmerge.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-09 01:28:31.213497 ocdsmerge-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:28:31.193497 ocdsmerge-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:28:31.197497 ocdsmerge-0.7.0/tests/cassettes/
+-rw-r--r--   0 runner    (1001) docker     (127)   545983 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/cassettes/test_merge.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   327224 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/cassettes/test_warn.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:28:31.197497 ocdsmerge-0.7.0/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:28:31.197497 ocdsmerge-0.7.0/tests/fixtures/1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.0/suppliers-compiled.json
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.0/suppliers-versioned.json
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.0/suppliers.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:28:31.205497 ocdsmerge-0.7.0/tests/fixtures/1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/contextual-compiled.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/contextual-versioned.json
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/contextual.json
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/empty-identifiermerge-array-compiled.json
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/empty-identifiermerge-array-versioned.json
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/empty-identifiermerge-array.json
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/empty-object-compiled.json
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/empty-object-versioned.json
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/empty-object.json
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/empty-wholelistmerge-array-compiled.json
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/empty-wholelistmerge-array-versioned.json
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/empty-wholelistmerge-array.json
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/fill-identifiermerge-array-compiled.json
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/fill-identifiermerge-array-versioned.json
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/fill-identifiermerge-array.json
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/fill-object-compiled.json
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/fill-object-versioned.json
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/fill-object.json
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/fill-wholelistmerge-array-compiled.json
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/fill-wholelistmerge-array-versioned.json
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/fill-wholelistmerge-array.json
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/initial-null-compiled.json
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/initial-null-versioned.json
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/initial-null.json
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/lists-compiled.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/lists-versioned.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/lists.json
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/mergeid-compiled.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/mergeid-versioned.json
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/mergeid.json
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/null-compiled.json
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/null-versioned.json
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/null.json
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/simple-compiled.json
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/simple-versioned.json
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/simple.json
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/single-empty-identifiermerge-array-compiled.json
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/single-empty-identifiermerge-array-versioned.json
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/single-empty-identifiermerge-array.json
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/single-empty-object-compiled.json
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/single-empty-object-versioned.json
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/single-empty-object.json
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/single-empty-wholelistmerge-array-compiled.json
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/single-empty-wholelistmerge-array-versioned.json
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/single-empty-wholelistmerge-array.json
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/string-list-compiled.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/string-list-versioned.json
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/string-list.json
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/unit-compiled.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/unit-versioned.json
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/1.1/unit.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    65422 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/release-schema-1__0__3.json
+-rw-r--r--   0 runner    (1001) docker     (127)    87980 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/release-schema-1__1__4.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:28:31.213497 ocdsmerge-0.7.0/tests/fixtures/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/schema/deep-identifier-merge-compiled.json
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/schema/deep-identifier-merge.json
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/schema/deep-omit-when-merged-compiled.json
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/schema/deep-omit-when-merged.json
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/schema/deep-whole-list-merge-compiled.json
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/schema/deep-whole-list-merge.json
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/schema/identifier-merge-collision-compiled.json
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/schema/identifier-merge-collision.json
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/schema/identifier-merge-duplicate-id-append.json
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/schema/identifier-merge-duplicate-id-by-position.json
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/schema/identifier-merge-duplicate-id-compiled.json
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/schema/identifier-merge-duplicate-id.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/schema/identifier-merge-no-id-append.json
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/schema/identifier-merge-no-id.json
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/schema/merge-property-is-false-compiled.json
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/schema/merge-property-is-false.json
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/schema/no-top-level-id-compiled.json
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/schema/no-top-level-id.json
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/schema/omit-when-merged-array-of-non-objects-compiled.json
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/schema/omit-when-merged-array-of-non-objects.json
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/schema/omit-when-merged-shadowed-compiled.json
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/schema/omit-when-merged-shadowed.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/schema/version-id-versioned.json
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/schema/version-id.json
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/schema/whole-list-merge-duplicate-id-compiled.json
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/schema/whole-list-merge-duplicate-id.json
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/schema/whole-list-merge-empty-compiled.json
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/schema/whole-list-merge-empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/schema/whole-list-merge-no-id-compiled.json
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/schema/whole-list-merge-no-id.json
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/schema/whole-list-merge-object-compiled.json
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/schema/whole-list-merge-object.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5385 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)    63895 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/versioned-release-validation-schema-1__0__3.json
+-rw-r--r--   0 runner    (1001) docker     (127)    73891 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/fixtures/versioned-release-validation-schema-1__1__4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/test_collisions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/test_flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7977 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/test_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/test_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-09 01:28:27.000000 ocdsmerge-0.7.0/tests/test_util.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ocdsmerge-0.6.6/PKG-INFO` & `ocdsmerge-0.7.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,46 @@
 Metadata-Version: 2.1
 Name: ocdsmerge
-Version: 0.6.6
+Version: 0.7.0
 Summary: A library and reference implementation for merging OCDS releases
 Home-page: https://github.com/open-contracting/ocds-merge
 Author: Open Contracting Partnership
 Author-email: data@open-contracting.org
 License: BSD
-Description: |PyPI Version| |Build Status| |Lint Status| |Coverage Status| |Python Version|
-        
-        This Python package creates records that conform to the `Open Contracting Data Standard <https://standard.open-contracting.org>`__. Specifically, it provides classes for merging OCDS releases with the same OCID into either a compiled release or a versioned release (collectively called "merged releases"), as described in the `OCDS documentation <https://standard.open-contracting.org/latest/en/schema/merging/>`__.
-        
-        Instead of using this library directly, it is easier to create merged releases using either:
-        
-        -  `OCDS Kit <https://ocdskit.readthedocs.io/>`__'s `compile <https://ocdskit.readthedocs.io/en/latest/cli/ocds.html#compile>`__ command-line tool
-        -  OCDS Kit's `merge <https://ocdskit.readthedocs.io/en/latest/api/combine.html#ocdskit.combine.merge>`__ Python function
-        -  `OCDS Toucan <https://toucan.open-contracting.org/>`__'s `compile releases <https://toucan.open-contracting.org/compile/>`__ web application
-        
-        If you are viewing this on GitHub or PyPi, open the `full documentation <https://ocds-merge.readthedocs.io/>`__ for additional details.
-        
-        .. |PyPI Version| image:: https://img.shields.io/pypi/v/ocdsmerge.svg
-           :target: https://pypi.org/project/ocdsmerge/
-        .. |Build Status| image:: https://github.com/open-contracting/ocds-merge/workflows/CI/badge.svg
-        .. |Lint Status| image:: https://github.com/open-contracting/ocds-merge/workflows/Lint/badge.svg
-        .. |Coverage Status| image:: https://coveralls.io/repos/github/open-contracting/ocds-merge/badge.svg?branch=main
-           :target: https://coveralls.io/github/open-contracting/ocds-merge?branch=main
-        .. |Python Version| image:: https://img.shields.io/pypi/pyversions/ocdsmerge.svg
-           :target: https://pypi.org/project/ocdsmerge/
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: jsonref
+Requires-Dist: requests
 Provides-Extra: test
+Requires-Dist: coveralls; extra == "test"
+Requires-Dist: jsonschema; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+
+|PyPI Version| |Build Status| |Coverage Status| |Python Version|
+
+This Python package creates records that conform to the `Open Contracting Data Standard <https://standard.open-contracting.org>`__. Specifically, it provides classes for merging OCDS releases with the same OCID into either a compiled release or a versioned release (collectively called "merged releases"), as described in the `OCDS documentation <https://standard.open-contracting.org/latest/en/schema/merging/>`__.
+
+Instead of using this library directly, it is easier to create merged releases using either:
+
+-  `OCDS Kit <https://ocdskit.readthedocs.io/>`__'s `compile <https://ocdskit.readthedocs.io/en/latest/cli/ocds.html#compile>`__ command-line tool
+-  OCDS Kit's `merge <https://ocdskit.readthedocs.io/en/latest/api/combine.html#ocdskit.combine.merge>`__ Python function
+
+If you are viewing this on GitHub or PyPI, open the `full documentation <https://ocds-merge.readthedocs.io/>`__ for additional details.
+
+.. |PyPI Version| image:: https://img.shields.io/pypi/v/ocdsmerge.svg
+   :target: https://pypi.org/project/ocdsmerge/
+.. |Build Status| image:: https://github.com/open-contracting/ocds-merge/actions/workflows/ci.yml/badge.svg
+   :target: https://github.com/open-contracting/ocds-merge/actions/workflows/ci.yml
+.. |Coverage Status| image:: https://coveralls.io/repos/github/open-contracting/ocds-merge/badge.svg?branch=main
+   :target: https://coveralls.io/github/open-contracting/ocds-merge?branch=main
+.. |Python Version| image:: https://img.shields.io/pypi/pyversions/ocdsmerge.svg
+   :target: https://pypi.org/project/ocdsmerge/
```

### Comparing `ocdsmerge-0.6.6/ocdsmerge.egg-info/PKG-INFO` & `ocdsmerge-0.7.0/ocdsmerge.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,46 @@
 Metadata-Version: 2.1
 Name: ocdsmerge
-Version: 0.6.6
+Version: 0.7.0
 Summary: A library and reference implementation for merging OCDS releases
 Home-page: https://github.com/open-contracting/ocds-merge
 Author: Open Contracting Partnership
 Author-email: data@open-contracting.org
 License: BSD
-Description: |PyPI Version| |Build Status| |Lint Status| |Coverage Status| |Python Version|
-        
-        This Python package creates records that conform to the `Open Contracting Data Standard <https://standard.open-contracting.org>`__. Specifically, it provides classes for merging OCDS releases with the same OCID into either a compiled release or a versioned release (collectively called "merged releases"), as described in the `OCDS documentation <https://standard.open-contracting.org/latest/en/schema/merging/>`__.
-        
-        Instead of using this library directly, it is easier to create merged releases using either:
-        
-        -  `OCDS Kit <https://ocdskit.readthedocs.io/>`__'s `compile <https://ocdskit.readthedocs.io/en/latest/cli/ocds.html#compile>`__ command-line tool
-        -  OCDS Kit's `merge <https://ocdskit.readthedocs.io/en/latest/api/combine.html#ocdskit.combine.merge>`__ Python function
-        -  `OCDS Toucan <https://toucan.open-contracting.org/>`__'s `compile releases <https://toucan.open-contracting.org/compile/>`__ web application
-        
-        If you are viewing this on GitHub or PyPi, open the `full documentation <https://ocds-merge.readthedocs.io/>`__ for additional details.
-        
-        .. |PyPI Version| image:: https://img.shields.io/pypi/v/ocdsmerge.svg
-           :target: https://pypi.org/project/ocdsmerge/
-        .. |Build Status| image:: https://github.com/open-contracting/ocds-merge/workflows/CI/badge.svg
-        .. |Lint Status| image:: https://github.com/open-contracting/ocds-merge/workflows/Lint/badge.svg
-        .. |Coverage Status| image:: https://coveralls.io/repos/github/open-contracting/ocds-merge/badge.svg?branch=main
-           :target: https://coveralls.io/github/open-contracting/ocds-merge?branch=main
-        .. |Python Version| image:: https://img.shields.io/pypi/pyversions/ocdsmerge.svg
-           :target: https://pypi.org/project/ocdsmerge/
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: jsonref
+Requires-Dist: requests
 Provides-Extra: test
+Requires-Dist: coveralls; extra == "test"
+Requires-Dist: jsonschema; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+
+|PyPI Version| |Build Status| |Coverage Status| |Python Version|
+
+This Python package creates records that conform to the `Open Contracting Data Standard <https://standard.open-contracting.org>`__. Specifically, it provides classes for merging OCDS releases with the same OCID into either a compiled release or a versioned release (collectively called "merged releases"), as described in the `OCDS documentation <https://standard.open-contracting.org/latest/en/schema/merging/>`__.
+
+Instead of using this library directly, it is easier to create merged releases using either:
+
+-  `OCDS Kit <https://ocdskit.readthedocs.io/>`__'s `compile <https://ocdskit.readthedocs.io/en/latest/cli/ocds.html#compile>`__ command-line tool
+-  OCDS Kit's `merge <https://ocdskit.readthedocs.io/en/latest/api/combine.html#ocdskit.combine.merge>`__ Python function
+
+If you are viewing this on GitHub or PyPI, open the `full documentation <https://ocds-merge.readthedocs.io/>`__ for additional details.
+
+.. |PyPI Version| image:: https://img.shields.io/pypi/v/ocdsmerge.svg
+   :target: https://pypi.org/project/ocdsmerge/
+.. |Build Status| image:: https://github.com/open-contracting/ocds-merge/actions/workflows/ci.yml/badge.svg
+   :target: https://github.com/open-contracting/ocds-merge/actions/workflows/ci.yml
+.. |Coverage Status| image:: https://coveralls.io/repos/github/open-contracting/ocds-merge/badge.svg?branch=main
+   :target: https://coveralls.io/github/open-contracting/ocds-merge?branch=main
+.. |Python Version| image:: https://img.shields.io/pypi/pyversions/ocdsmerge.svg
+   :target: https://pypi.org/project/ocdsmerge/
```

### Comparing `ocdsmerge-0.6.6/ocdsmerge.egg-info/SOURCES.txt` & `ocdsmerge-0.7.0/ocdsmerge.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 LICENSE
 MANIFEST.in
 README.rst
-setup.py
+pyproject.toml
+setup.cfg
 docs/Makefile
 docs/changelog.rst
 docs/conf.py
 docs/create-merged-releases.rst
 docs/handle-bad-data.rst
 docs/index.rst
+docs/requirements.txt
 docs/update-merged-releases.rst
 docs/api/index.rst
 ocdsmerge/__init__.py
 ocdsmerge/exceptions.py
 ocdsmerge/flatten.py
 ocdsmerge/merge.py
 ocdsmerge/rules.py
```

### Comparing `ocdsmerge-0.6.6/LICENSE` & `ocdsmerge-0.7.0/LICENSE`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,29 @@
-Copyright (c) 2015, Open Data Services Coop
+BSD 3-Clause License
+
+Copyright (c) 2015, Open Contracting Partnership
 All rights reserved.
 
-Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
 
-1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+* Redistributions of source code must retain the above copyright notice, this
+  list of conditions and the following disclaimer.
 
-2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+* Redistributions in binary form must reproduce the above copyright notice,
+  this list of conditions and the following disclaimer in the documentation
+  and/or other materials provided with the distribution.
 
-3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+* Neither the name of the copyright holder nor the names of its
+  contributors may be used to endorse or promote products derived from
+  this software without specific prior written permission.
 
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `ocdsmerge-0.6.6/tests/test_flatten.py` & `ocdsmerge-0.7.0/tests/test_flatten.py`

 * *Files identical despite different names*

### Comparing `ocdsmerge-0.6.6/tests/test_merge.py` & `ocdsmerge-0.7.0/tests/test_merge.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,56 +1,67 @@
 import json
 import os.path
 import re
+import warnings
 from copy import deepcopy
 from glob import glob
 
 import pytest
 
 from ocdsmerge import CompiledRelease, Merger, VersionedRelease
-from ocdsmerge.exceptions import (InconsistentTypeError, MissingDateKeyError, NonObjectReleaseError,
-                                  NonStringDateValueError, NullDateValueError)
+from ocdsmerge.exceptions import (
+    DuplicateIdValueWarning,
+    InconsistentTypeError,
+    MissingDateKeyError,
+    NonObjectReleaseError,
+    NonStringDateValueError,
+    NullDateValueError,
+)
 from tests import load, path, schema_url, tags
 
-simple_schema = path('schema.json')
 
-test_merge_argvalues = []
-for minor_version, schema in (('1.1', None), ('1.1', schema_url), ('1.0', schema_url), ('schema', simple_schema)):
-    if schema and schema.startswith('http'):
-        schema = schema.format(tags[minor_version])
-    for suffix in ('compiled', 'versioned'):
-        filenames = glob(path(os.path.join(minor_version, '*-{}.json'.format(suffix))))
-        assert len(filenames), '{} fixtures not found'.format(suffix)
-        test_merge_argvalues += [(filename, schema) for filename in filenames]
+def get_test_cases():
+    test_merge_argvalues = []
+
+    simple_schema = path('schema.json')
+
+    for minor_version, schema in (('1.1', None), ('1.1', schema_url), ('1.0', schema_url), ('schema', simple_schema)):
+        if schema and schema.startswith('http'):
+            schema = schema.format(tags[minor_version])
+        for suffix in ('compiled', 'versioned'):
+            filenames = glob(path(os.path.join(minor_version, f'*-{suffix}.json')))
+            assert len(filenames), f'{suffix} fixtures not found'
+            test_merge_argvalues += [(filename, schema) for filename in filenames]
+
+    return test_merge_argvalues
 
 
-@pytest.mark.vcr()
 @pytest.mark.parametrize('error, data', [
     (MissingDateKeyError, {}),
     (NullDateValueError, {'date': None}),
     (NonStringDateValueError, {'date': {}}),
     (NonObjectReleaseError, '{}'),
     (NonObjectReleaseError, b'{}'),
     (NonObjectReleaseError, []),
-    (NonObjectReleaseError, tuple()),
+    (NonObjectReleaseError, ()),
     (NonObjectReleaseError, set()),
 ])
 def test_errors(error, data, empty_merger):
     for infix in ('compiled', 'versioned'):
         with pytest.raises(error):
-            getattr(empty_merger, 'create_{}_release'.format(infix))([{'date': '2010-01-01'}, data])
+            getattr(empty_merger, f'create_{infix}_release')([{'date': '2010-01-01'}, data])
 
     if not isinstance(data, dict):
         with pytest.raises(error):
             empty_merger.create_compiled_release([data])
     else:
         release = deepcopy(data)
 
         expected = {
-            'id': 'None-{}'.format(data.get('date')),
+            'id': f"None-{data.get('date')}",
             'tag': ['compiled'],
         }
 
         if data.get('date') is not None:
             expected['date'] = data['date']
 
         assert empty_merger.create_compiled_release([release]) == expected
@@ -70,82 +81,84 @@
                 'value': 'tender',
             }],
         }
 
         assert empty_merger.create_versioned_release([release]) == expected
 
 
-@pytest.mark.vcr()
 def test_key_error(empty_merger):
     with pytest.raises(KeyError) as excinfo:
         empty_merger.create_compiled_release([{'date': '2010-01-01'}, {}])
 
     message = 'The `date` field of at least one release is missing.'
 
     assert excinfo.value.key == 'date'
     assert excinfo.value.message == message
     assert str(excinfo.value) == message
 
 
-@pytest.mark.vcr()
-@pytest.mark.parametrize('filename,schema', test_merge_argvalues)
+@pytest.mark.parametrize('filename,schema', get_test_cases())
 def test_merge(filename, schema):
     merger = Merger(schema)
 
     if filename.endswith('-compiled.json'):
         infix = 'compiled'
     else:
         infix = 'versioned'
 
     with open(filename) as f:
         expected = json.load(f)
     with open(re.sub(r'-(?:compiled|versioned)', '', filename)) as f:
         releases = json.load(f)
 
     original = deepcopy(releases)
-    actual = getattr(merger, 'create_{}_release'.format(infix))(releases)
+
+    with warnings.catch_warnings():
+        warnings.simplefilter('error')  # no unexpected warnings
+        if filename == os.path.join('tests', 'fixtures', 'schema', 'identifier-merge-duplicate-id-compiled.json'):
+            warnings.filterwarnings('ignore', category=DuplicateIdValueWarning)
+
+        actual = getattr(merger, f'create_{infix}_release')(releases)
 
     assert releases == original
     assert actual == expected, filename + '\n' + json.dumps(actual)
 
 
-@pytest.mark.vcr()
 @pytest.mark.parametrize('infix,cls', [('compiled', CompiledRelease), ('versioned', VersionedRelease)])
 def test_extend(infix, cls, empty_merger):
-    expected = load(os.path.join('1.1', 'lists-{}.json'.format(infix)))
+    expected = load(os.path.join('1.1', f'lists-{infix}.json'))
     releases = load(os.path.join('1.1', 'lists.json'))
 
-    merged_release = getattr(empty_merger, 'create_{}_release'.format(infix))(releases[:1])
+    merged_release = getattr(empty_merger, f'create_{infix}_release')(releases[:1])
 
     merger = cls(merged_release, merge_rules=empty_merger.merge_rules)
     merger.extend(releases[1:])
 
     assert merger.asdict() == expected
 
     merger = cls(merged_release, schema={})
     merger.extend(releases[1:])
 
     assert merger.asdict() == expected
 
 
-@pytest.mark.vcr()
 @pytest.mark.parametrize('infix,cls', [('compiled', CompiledRelease), ('versioned', VersionedRelease)])
 def test_append(infix, cls, empty_merger):
-    expected = load(os.path.join('1.1', 'lists-{}.json'.format(infix)))
+    expected = load(os.path.join('1.1', f'lists-{infix}.json'))
     releases = load(os.path.join('1.1', 'lists.json'))
 
-    merged_release = getattr(empty_merger, 'create_{}_release'.format(infix))(releases[:1])
+    merged_release = getattr(empty_merger, f'create_{infix}_release')(releases[:1])
 
     merger = cls(merged_release, merge_rules=empty_merger.merge_rules)
     merger.append(releases[1])
 
     assert merger.asdict() == expected
 
     merger = cls(merged_release, schema={})
-    merger.extend(releases[1:])
+    merger.append(releases[1])
 
     assert merger.asdict() == expected
 
 
 def test_inconsistent_type(empty_merger):
     data = [{
         "date": "2000-01-01T00:00:00Z",
@@ -199,15 +212,15 @@
     actual = deepcopy(data)
     expected = deepcopy(output)
     del actual[i]['mixedArray'][j]
     if i == 1:
         del expected['mixedArray'][j]
 
     assert simple_merger.create_compiled_release(actual) == expected, \
-        'removed item index {} from release index {}'.format(j, i)
+        f'removed item index {j} from release index {i}'
 
 
 @pytest.mark.parametrize('i,j', [(0, 0), (0, 1), (1, 0), (1, 1)])
 def test_merge_when_array_is_mixed_without_schema(i, j, empty_merger):
     data = [{
         'ocid': 'ocds-213czf-A',
         "id": "1",
@@ -243,12 +256,12 @@
     expected = deepcopy(output)
     del actual[i]['mixedArray'][j]
     if i == 1:
         del expected['mixedArray'][j]
 
     if j == 0:
         assert empty_merger.create_compiled_release(actual) == expected, \
-            'removed item index {} from release index {}'.format(j, i)
+            f'removed item index {j} from release index {i}'
     else:
         with pytest.raises(AssertionError):
             assert empty_merger.create_compiled_release(actual) == expected, \
-                'removed item index {} from release index {}'.format(j, i)
+                f'removed item index {j} from release index {i}'
```

### Comparing `ocdsmerge-0.6.6/tests/test_collisions.py` & `ocdsmerge-0.7.0/tests/test_collisions.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,82 +6,81 @@
 from ocdsmerge import APPEND, MERGE_BY_POSITION, Merger
 from ocdsmerge.exceptions import DuplicateIdValueWarning
 from tests import load
 
 releases = load(os.path.join('schema', 'identifier-merge-duplicate-id.json'))
 
 
-@pytest.mark.vcr()
 def test_warn(empty_merger):
     fields = ['identifierMerge', 'array']
     string = "Multiple objects have the `id` value '1' in the `nested.{}` array"
 
     with pytest.warns(DuplicateIdValueWarning) as records:
         empty_merger.create_compiled_release(releases)
 
     assert len(records) == 2
 
     for i, record in enumerate(records):
-        message = string.format(fields[i])
+        assert str(record.message) == string.format(fields[i])
 
-        assert record.message.path == ('nested', fields[i],)
-        assert record.message.id == '1'
-        assert record.message.message == message
-        assert str(record.message) == message
 
-
-@pytest.mark.vcr()
 def test_raise(empty_merger):
     with pytest.raises(DuplicateIdValueWarning) as excinfo:
         with warnings.catch_warnings():
             warnings.filterwarnings('error', category=DuplicateIdValueWarning)
             empty_merger.create_compiled_release(releases)
 
-    message = "Multiple objects have the `id` value '1' in the `nested.identifierMerge` array"
-
-    assert excinfo.value.path == ('nested', 'identifierMerge',)
-    assert excinfo.value.id == '1'
-    assert excinfo.value.message == message
-    assert str(excinfo.value) == message
+    assert str(excinfo.value) == "Multiple objects have the `id` value '1' in the `nested.identifierMerge` array"
 
 
-@pytest.mark.vcr()
 def test_ignore(empty_merger):
-    with pytest.warns(None) as records:
-        with warnings.catch_warnings():
-            warnings.filterwarnings('ignore', category=DuplicateIdValueWarning)
-            empty_merger.create_compiled_release(releases)
+    with warnings.catch_warnings():
+        warnings.simplefilter('error')  # no unexpected warnings
 
-    assert not records, 'unexpected warning: {}'.format(records[0].message)
+        warnings.filterwarnings('ignore', category=DuplicateIdValueWarning)
+        empty_merger.create_compiled_release(releases)
 
 
-@pytest.mark.vcr()
 def test_merge_by_position():
+    fields = ['identifierMerge', 'array', 'identifierMerge', 'array']
+    string = "Multiple objects have the `id` value '1' in the `nested.{}` array"
+
     merger = Merger(rule_overrides={('nested', 'array',): MERGE_BY_POSITION})
 
-    with pytest.warns(DuplicateIdValueWarning):
+    with pytest.warns(DuplicateIdValueWarning) as records:
         compiled_release = merger.create_compiled_release(releases + releases)
 
     assert compiled_release == load(os.path.join('schema', 'identifier-merge-duplicate-id-by-position.json'))
 
+    assert len(records) == 4
+
+    for i, record in enumerate(records):
+        assert str(record.message) == string.format(fields[i])
+
 
-@pytest.mark.vcr()
 def test_append():
+    fields = ['identifierMerge', 'array', 'identifierMerge', 'array']
+    string = "Multiple objects have the `id` value '1' in the `nested.{}` array"
+
     merger = Merger(rule_overrides={('nested', 'array',): APPEND})
 
-    with pytest.warns(DuplicateIdValueWarning):
+    with pytest.warns(DuplicateIdValueWarning) as records:
         compiled_release = merger.create_compiled_release(releases + releases)
 
     assert compiled_release == load(os.path.join('schema', 'identifier-merge-duplicate-id-append.json'))
 
+    assert len(records) == 4
+
+    for i, record in enumerate(records):
+        assert str(record.message) == string.format(fields[i])
+
 
-@pytest.mark.vcr()
 def test_append_no_id():
     merger = Merger(rule_overrides={('nested', 'array',): APPEND})
     data = load(os.path.join('schema', 'identifier-merge-no-id.json'))
 
-    with pytest.warns(None) as records:
-        with warnings.catch_warnings():
-            compiled_release = merger.create_compiled_release(data + data)
+    with warnings.catch_warnings():
+        warnings.simplefilter('error')  # no unexpected warnings
+
+        compiled_release = merger.create_compiled_release(data + data)
 
     assert compiled_release == load(os.path.join('schema', 'identifier-merge-no-id-append.json'))
-    assert not records, 'unexpected warning: {}'.format(records[0].message)
```

### Comparing `ocdsmerge-0.6.6/tests/test_fixtures.py` & `ocdsmerge-0.7.0/tests/test_fixtures.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,44 +17,49 @@
 
 import pytest
 from jsonschema import FormatChecker
 from jsonschema.validators import Draft4Validator as validator
 
 from tests import load, path, tags
 
-release_schema_path = 'release-schema-{}.json'
-versioned_release_schema_path = 'versioned-release-validation-schema-{}.json'
-
-test_valid_argvalues = []
-for minor_version, patch_tag in tags.items():
-    filenames = glob(path(os.path.join(minor_version, '*.json')))
-    assert len(filenames), 'ocds fixtures not found'
-    for versioned, schema_path in ((False, release_schema_path), (True, versioned_release_schema_path)):
-        schema = load(schema_path.format(patch_tag))
-        for filename in filenames:
-            if not versioned ^ filename.endswith('-versioned.json'):
-                test_valid_argvalues.append((filename, schema))
-
 
 def custom_warning_formatter(message, category, filename, lineno, line=None):
     return str(message).replace(os.getcwd() + os.sep, '')
 
 
 warnings.formatwarning = custom_warning_formatter
 
 
-@pytest.mark.parametrize('filename,schema', test_valid_argvalues)
+def get_test_cases():
+    test_valid_argvalues = []
+
+    release_schema_path = 'release-schema-{}.json'
+    versioned_release_schema_path = 'versioned-release-validation-schema-{}.json'
+
+    for minor_version, patch_tag in tags.items():
+        filenames = glob(path(os.path.join(minor_version, '*.json')))
+        assert len(filenames), 'ocds fixtures not found'
+        for versioned, schema_path in ((False, release_schema_path), (True, versioned_release_schema_path)):
+            schema = load(schema_path.format(patch_tag))
+            for filename in filenames:
+                if not versioned ^ filename.endswith('-versioned.json'):
+                    test_valid_argvalues.append((filename, schema))
+
+    return test_valid_argvalues
+
+
+@pytest.mark.parametrize('filename,schema', get_test_cases())
 def test_valid(filename, schema):
     errors = 0
 
     with open(filename) as f:
         data = json.load(f)
     if filename.endswith('-versioned.json') or filename.endswith('-compiled.json'):
         data = [data]
 
     for datum in data:
         for error in validator(schema, format_checker=FormatChecker()).iter_errors(datum):
             errors += 1
             warnings.warn(json.dumps(error.instance, indent=2))
-            warnings.warn('{} ({})\n'.format(error.message, '/'.join(error.absolute_schema_path)))
+            warnings.warn(f"{error.message} ({'/'.join(error.absolute_schema_path)})\n")
 
-    assert errors == 0, '{} is invalid. See warnings below.'.format(filename)
+    assert errors == 0, f'{filename} is invalid. See warnings below.'
```

### Comparing `ocdsmerge-0.6.6/tests/fixtures/release-schema-1__1__4.json` & `ocdsmerge-0.7.0/tests/fixtures/release-schema-1__1__4.json`

 * *Files identical despite different names*

### Comparing `ocdsmerge-0.6.6/tests/fixtures/1.0/suppliers-versioned.json` & `ocdsmerge-0.7.0/tests/fixtures/1.0/suppliers-versioned.json`

 * *Files identical despite different names*

### Comparing `ocdsmerge-0.6.6/tests/fixtures/1.0/suppliers.json` & `ocdsmerge-0.7.0/tests/fixtures/1.0/suppliers.json`

 * *Files identical despite different names*

### Comparing `ocdsmerge-0.6.6/tests/fixtures/1.1/string-list.json` & `ocdsmerge-0.7.0/tests/fixtures/1.1/string-list.json`

 * *Files identical despite different names*

### Comparing `ocdsmerge-0.6.6/tests/fixtures/1.1/simple-versioned.json` & `ocdsmerge-0.7.0/tests/fixtures/1.1/simple-versioned.json`

 * *Files identical despite different names*

### Comparing `ocdsmerge-0.6.6/tests/fixtures/1.1/mergeid-versioned.json` & `ocdsmerge-0.7.0/tests/fixtures/1.1/mergeid-versioned.json`

 * *Files identical despite different names*

### Comparing `ocdsmerge-0.6.6/tests/fixtures/1.1/initial-null-versioned.json` & `ocdsmerge-0.7.0/tests/fixtures/1.1/initial-null-versioned.json`

 * *Files identical despite different names*

### Comparing `ocdsmerge-0.6.6/tests/fixtures/1.1/lists-versioned.json` & `ocdsmerge-0.7.0/tests/fixtures/1.1/lists-versioned.json`

 * *Files identical despite different names*

### Comparing `ocdsmerge-0.6.6/tests/fixtures/1.1/empty-wholelistmerge-array.json` & `ocdsmerge-0.7.0/tests/fixtures/1.1/empty-wholelistmerge-array.json`

 * *Files identical despite different names*

### Comparing `ocdsmerge-0.6.6/tests/fixtures/1.1/contextual-compiled.json` & `ocdsmerge-0.7.0/tests/fixtures/1.1/contextual-compiled.json`

 * *Files identical despite different names*

### Comparing `ocdsmerge-0.6.6/tests/fixtures/1.1/contextual.json` & `ocdsmerge-0.7.0/tests/fixtures/1.1/contextual.json`

 * *Files identical despite different names*

### Comparing `ocdsmerge-0.6.6/tests/fixtures/1.1/mergeid.json` & `ocdsmerge-0.7.0/tests/fixtures/1.1/mergeid.json`

 * *Files identical despite different names*

### Comparing `ocdsmerge-0.6.6/tests/fixtures/1.1/empty-wholelistmerge-array-versioned.json` & `ocdsmerge-0.7.0/tests/fixtures/1.1/empty-wholelistmerge-array-versioned.json`

 * *Files identical despite different names*

### Comparing `ocdsmerge-0.6.6/tests/fixtures/1.1/lists.json` & `ocdsmerge-0.7.0/tests/fixtures/1.1/lists.json`

 * *Files identical despite different names*

### Comparing `ocdsmerge-0.6.6/tests/fixtures/1.1/unit-versioned.json` & `ocdsmerge-0.7.0/tests/fixtures/1.1/unit-versioned.json`

 * *Files identical despite different names*

### Comparing `ocdsmerge-0.6.6/tests/fixtures/1.1/fill-wholelistmerge-array-versioned.json` & `ocdsmerge-0.7.0/tests/fixtures/1.1/fill-wholelistmerge-array-versioned.json`

 * *Files identical despite different names*

### Comparing `ocdsmerge-0.6.6/tests/fixtures/1.1/contextual-versioned.json` & `ocdsmerge-0.7.0/tests/fixtures/1.1/contextual-versioned.json`

 * *Files identical despite different names*

### Comparing `ocdsmerge-0.6.6/tests/fixtures/1.1/null-versioned.json` & `ocdsmerge-0.7.0/tests/fixtures/1.1/null-versioned.json`

 * *Files identical despite different names*

### Comparing `ocdsmerge-0.6.6/tests/fixtures/1.1/string-list-versioned.json` & `ocdsmerge-0.7.0/tests/fixtures/1.1/string-list-versioned.json`

 * *Files identical despite different names*

### Comparing `ocdsmerge-0.6.6/tests/fixtures/1.1/fill-wholelistmerge-array.json` & `ocdsmerge-0.7.0/tests/fixtures/1.1/fill-wholelistmerge-array.json`

 * *Files identical despite different names*

### Comparing `ocdsmerge-0.6.6/tests/fixtures/1.1/unit.json` & `ocdsmerge-0.7.0/tests/fixtures/1.1/unit.json`

 * *Files identical despite different names*

### Comparing `ocdsmerge-0.6.6/tests/fixtures/release-schema-1__0__3.json` & `ocdsmerge-0.7.0/tests/fixtures/release-schema-1__0__3.json`

 * *Files identical despite different names*

### Comparing `ocdsmerge-0.6.6/tests/fixtures/README.md` & `ocdsmerge-0.7.0/tests/fixtures/README.md`

 * *Files identical despite different names*

### Comparing `ocdsmerge-0.6.6/tests/fixtures/schema/identifier-merge-duplicate-id-append.json` & `ocdsmerge-0.7.0/tests/fixtures/schema/identifier-merge-duplicate-id-append.json`

 * *Files identical despite different names*

### Comparing `ocdsmerge-0.6.6/tests/fixtures/schema/deep-whole-list-merge.json` & `ocdsmerge-0.7.0/tests/fixtures/schema/deep-whole-list-merge.json`

 * *Files identical despite different names*

### Comparing `ocdsmerge-0.6.6/tests/fixtures/schema/no-top-level-id.json` & `ocdsmerge-0.7.0/tests/fixtures/schema/no-top-level-id.json`

 * *Files identical despite different names*

### Comparing `ocdsmerge-0.6.6/tests/fixtures/schema/version-id.json` & `ocdsmerge-0.7.0/tests/fixtures/schema/version-id.json`

 * *Files identical despite different names*

### Comparing `ocdsmerge-0.6.6/tests/fixtures/schema/deep-identifier-merge.json` & `ocdsmerge-0.7.0/tests/fixtures/schema/deep-identifier-merge.json`

 * *Files identical despite different names*

### Comparing `ocdsmerge-0.6.6/tests/fixtures/schema/version-id-versioned.json` & `ocdsmerge-0.7.0/tests/fixtures/schema/version-id-versioned.json`

 * *Files identical despite different names*

### Comparing `ocdsmerge-0.6.6/tests/fixtures/versioned-release-validation-schema-1__0__3.json` & `ocdsmerge-0.7.0/tests/fixtures/versioned-release-validation-schema-1__0__3.json`

 * *Files identical despite different names*

### Comparing `ocdsmerge-0.6.6/tests/fixtures/schema.json` & `ocdsmerge-0.7.0/tests/fixtures/schema.json`

 * *Files identical despite different names*

### Comparing `ocdsmerge-0.6.6/tests/fixtures/versioned-release-validation-schema-1__1__4.json` & `ocdsmerge-0.7.0/tests/fixtures/versioned-release-validation-schema-1__1__4.json`

 * *Files identical despite different names*

### Comparing `ocdsmerge-0.6.6/tests/test_rules.py` & `ocdsmerge-0.7.0/tests/test_rules.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 from ocdsmerge.rules import get_merge_rules
 from tests import schema_url, tags
 
 
 def test_get_merge_rules_1_1():
     assert get_merge_rules(schema_url.format(tags['1.1'])) == {
-        ('awards', 'items', 'additionalClassifications'): {'wholeListMerge'},
-        ('contracts', 'items', 'additionalClassifications'): {'wholeListMerge'},
-        ('contracts', 'relatedProcesses', 'relationship'): {'wholeListMerge'},
-        ('date',): {'omitWhenMerged'},
-        ('id',): {'omitWhenMerged'},
-        ('parties', 'additionalIdentifiers'): {'wholeListMerge'},
-        ('parties', 'roles'): {'wholeListMerge'},
-        ('relatedProcesses', 'relationship'): {'wholeListMerge'},
-        ('tag',): {'omitWhenMerged'},
-        ('tender', 'additionalProcurementCategories'): {'wholeListMerge'},
-        ('tender', 'items', 'additionalClassifications'): {'wholeListMerge'},
-        ('tender', 'submissionMethod'): {'wholeListMerge'},
+        ('awards', 'items', 'additionalClassifications'): 'wholeListMerge',
+        ('contracts', 'items', 'additionalClassifications'): 'wholeListMerge',
+        ('contracts', 'relatedProcesses', 'relationship'): 'wholeListMerge',
+        ('date',): 'omitWhenMerged',
+        ('id',): 'omitWhenMerged',
+        ('parties', 'additionalIdentifiers'): 'wholeListMerge',
+        ('parties', 'roles'): 'wholeListMerge',
+        ('relatedProcesses', 'relationship'): 'wholeListMerge',
+        ('tag',): 'omitWhenMerged',
+        ('tender', 'additionalProcurementCategories'): 'wholeListMerge',
+        ('tender', 'items', 'additionalClassifications'): 'wholeListMerge',
+        ('tender', 'submissionMethod'): 'wholeListMerge',
 
         # Deprecated
-        ('awards', 'amendment', 'changes'): {'wholeListMerge'},
-        ('awards', 'amendments', 'changes'): {'wholeListMerge'},
-        ('awards', 'suppliers', 'additionalIdentifiers'): {'wholeListMerge'},
-        ('buyer', 'additionalIdentifiers'): {'wholeListMerge'},
-        ('contracts', 'amendment', 'changes'): {'wholeListMerge'},
-        ('contracts', 'amendments', 'changes'): {'wholeListMerge'},
-        ('contracts', 'implementation', 'transactions', 'payee', 'additionalIdentifiers'): {'wholeListMerge'},
-        ('contracts', 'implementation', 'transactions', 'payer', 'additionalIdentifiers'): {'wholeListMerge'},
-        ('tender', 'amendment', 'changes'): {'wholeListMerge'},
-        ('tender', 'amendments', 'changes'): {'wholeListMerge'},
-        ('tender', 'procuringEntity', 'additionalIdentifiers'): {'wholeListMerge'},
-        ('tender', 'tenderers', 'additionalIdentifiers'): {'wholeListMerge'},
+        ('awards', 'amendment', 'changes'): 'wholeListMerge',
+        ('awards', 'amendments', 'changes'): 'wholeListMerge',
+        ('awards', 'suppliers', 'additionalIdentifiers'): 'wholeListMerge',
+        ('buyer', 'additionalIdentifiers'): 'wholeListMerge',
+        ('contracts', 'amendment', 'changes'): 'wholeListMerge',
+        ('contracts', 'amendments', 'changes'): 'wholeListMerge',
+        ('contracts', 'implementation', 'transactions', 'payee', 'additionalIdentifiers'): 'wholeListMerge',
+        ('contracts', 'implementation', 'transactions', 'payer', 'additionalIdentifiers'): 'wholeListMerge',
+        ('tender', 'amendment', 'changes'): 'wholeListMerge',
+        ('tender', 'amendments', 'changes'): 'wholeListMerge',
+        ('tender', 'procuringEntity', 'additionalIdentifiers'): 'wholeListMerge',
+        ('tender', 'tenderers', 'additionalIdentifiers'): 'wholeListMerge',
     }
 
 
 def test_get_merge_rules_1_0():
     assert get_merge_rules(schema_url.format(tags['1.0'])) == {
-        ('awards', 'amendment', 'changes'): {'wholeListMerge'},
-        ('awards', 'items', 'additionalClassifications'): {'wholeListMerge'},
-        ('awards', 'suppliers'): {'wholeListMerge'},
-        ('buyer', 'additionalIdentifiers'): {'wholeListMerge'},
-        ('contracts', 'amendment', 'changes'): {'wholeListMerge'},
-        ('contracts', 'items', 'additionalClassifications'): {'wholeListMerge'},
-        ('date',): {'omitWhenMerged'},
-        ('id',): {'omitWhenMerged'},
-        ('ocid',): {'omitWhenMerged'},
-        ('tag',): {'omitWhenMerged'},
-        ('tender', 'amendment', 'changes'): {'wholeListMerge'},
-        ('tender', 'items', 'additionalClassifications'): {'wholeListMerge'},
-        ('tender', 'procuringEntity', 'additionalIdentifiers'): {'wholeListMerge'},
-        ('tender', 'submissionMethod'): {'wholeListMerge'},
-        ('tender', 'tenderers'): {'wholeListMerge'},
+        ('awards', 'amendment', 'changes'): 'wholeListMerge',
+        ('awards', 'items', 'additionalClassifications'): 'wholeListMerge',
+        ('awards', 'suppliers'): 'wholeListMerge',
+        ('buyer', 'additionalIdentifiers'): 'wholeListMerge',
+        ('contracts', 'amendment', 'changes'): 'wholeListMerge',
+        ('contracts', 'items', 'additionalClassifications'): 'wholeListMerge',
+        ('date',): 'omitWhenMerged',
+        ('id',): 'omitWhenMerged',
+        ('ocid',): 'omitWhenMerged',
+        ('tag',): 'omitWhenMerged',
+        ('tender', 'amendment', 'changes'): 'wholeListMerge',
+        ('tender', 'items', 'additionalClassifications'): 'wholeListMerge',
+        ('tender', 'procuringEntity', 'additionalIdentifiers'): 'wholeListMerge',
+        ('tender', 'submissionMethod'): 'wholeListMerge',
+        ('tender', 'tenderers'): 'wholeListMerge',
     }
```

### Comparing `ocdsmerge-0.6.6/docs/index.rst` & `ocdsmerge-0.7.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ocdsmerge-0.6.6/docs/create-merged-releases.rst` & `ocdsmerge-0.7.0/docs/create-merged-releases.rst`

 * *Files identical despite different names*

### Comparing `ocdsmerge-0.6.6/docs/Makefile` & `ocdsmerge-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ocdsmerge-0.6.6/docs/conf.py` & `ocdsmerge-0.7.0/docs/conf.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,70 +12,67 @@
 #
 # import os
 # import sys
 # sys.path.insert(0, os.path.abspath('.'))
 import os
 import sys
 
-sys.path.insert(0, os.path.abspath('..'))
+sys.path.insert(0, os.path.abspath(".."))
 
 
 # -- Project information -----------------------------------------------------
 
-project = 'OCDS Merge'
-copyright = '2019, Open Contracting Partnership'
-author = 'Open Contracting Partnership'
+project = "OCDS Merge"
+copyright = "2019, Open Contracting Partnership"
+author = "Open Contracting Partnership"
 
 # The short X.Y version
-version = '0.6.6'
+version = "0.7.0"
 # The full version, including alpha/beta/rc tags
 release = version
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
-    'sphinx.ext.autodoc',
-    'sphinx.ext.viewcode',
+    "sphinx.ext.autodoc",
+    "sphinx.ext.intersphinx",
+    "sphinx.ext.viewcode",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'default'
+html_theme = "furo"
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = []
 
 
 # -- Extension configuration -------------------------------------------------
 
-# Needed for ReadTheDocs (Sphinx 1.8).
-master_doc = 'index'
-
 autodoc_default_options = {
-    'members': None,
+    "members": None,
+    "member-order": "bysource",
 }
-autodoc_member_order = 'bysource'
-
-on_rtd = os.environ.get('READTHEDOCS', None) == 'True'
+autodoc_typehints = "description"
+autodoc_type_aliases = {}
 
-if not on_rtd:  # only import and set the theme if we're building docs locally
-    import sphinx_rtd_theme
-    html_theme = 'sphinx_rtd_theme'
-    html_theme_path = [sphinx_rtd_theme.get_html_theme_path()]
+intersphinx_mapping = {
+    "python": ("https://docs.python.org/3", None),
+}
```

### Comparing `ocdsmerge-0.6.6/docs/update-merged-releases.rst` & `ocdsmerge-0.7.0/docs/update-merged-releases.rst`

 * *Files identical despite different names*

### Comparing `ocdsmerge-0.6.6/docs/handle-bad-data.rst` & `ocdsmerge-0.7.0/docs/handle-bad-data.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Handle Bad Data
 ===============
 
 The merge routine merges multiple individual releases into either a compiled release or a versioned release. Across the individual releases, it merges objects in arrays based on their ``id`` values, as described in the `OCDS documentation <https://standard.open-contracting.org/latest/en/schema/merging/>`__. This allows a publisher to, for example, disclose an upcoming milestone in one release, and set the date on which it was met in another release.
 
 However, if objects that correspond to different things re-use ``id`` values, then only the last object is retained in the merged release, by default. (To be clear, such data has structural errors.) For example, if a publisher creates a release for each award notice in a procurement procedure, and restarts the numbering of award objects in each release from '1', then the later releases will overwrite the award objects of the earlier releases.
 
-Similarly, if, in a single release, objects in the same array share an ``id`` value, then only the last object is retained. If so, this package issues a :code:`DuplicateIdValueWarning` warning. You can turn the warning into an exception or ignore the warning using a `warning filter <https://docs.python.org/3.8/library/warnings.html>`__. For example:
+Similarly, if, in a single release, objects in the same array share an ``id`` value, then only the last object is retained. If so, this package issues a :code:`DuplicateIdValueWarning` warning. You can turn the warning into an exception or ignore the warning using a `warning filter <https://docs.python.org/3/library/warnings.html>`__. For example:
 
 .. code-block:: python
 
    import warnings
 
    import ocdsmerge
    from ocdsmerge.exceptions import DuplicateIdValueWarning
@@ -24,15 +24,15 @@
        compiled_release = merger.create_compiled_release(releases)
 
    # Ignore the warning, instead.
    with warnings.catch_warnings():
        warnings.filterwarnings('ignore', category=DuplicateIdValueWarning)
        compiled_release = merger.create_compiled_release(releases)
 
-  # {'tag': ['compiled'], 'id': 'None-None', 'awards': [{'id': '1'}]}
+   # {'tag': ['compiled'], 'id': 'None-None', 'awards': [{'id': '1'}]}
 
 If you know in advance that the individual releases have structural errors as described above, you can change the behavior of the merge routine by setting a :code:`rule_overrides` argument on a per-field basis:
 
 -  :code:`ocdsmerge.MERGE_BY_POSITION`: merge objects in the given array based on their array index, instead of their ``id`` value.
 
    - This is appropriate if the publisher always re-publishes all prior objects in a given array, and puts them in a consistent order.
```

### Comparing `ocdsmerge-0.6.6/docs/api/index.rst` & `ocdsmerge-0.7.0/docs/api/index.rst`

 * *Files identical despite different names*

### Comparing `ocdsmerge-0.6.6/docs/changelog.rst` & `ocdsmerge-0.7.0/docs/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,25 @@
 Changelog
 =========
 
+0.7.0 (2024-05-08)
+------------------
+
+Changed
+~~~~~~~
+
+-  :func:`ocdsmerge.util.get_tags` raises an error if it encounters an HTTP error.
+-  :exc:`ocdsmerge.exceptions.DuplicateIdValueWarning` has no custom attributes.
+-  Drop support for Python 3.6 and 3.7.
+
+Added
+~~~~~
+
+-  Add PyPy support.
+
 0.6.6 (2021-04-10)
 ------------------
 
 Added
 ~~~~~
 
 -  Add Python wheels distribution.
@@ -86,15 +101,15 @@
 0.5.10.post3 (2019-11-28)
 -------------------------
 
 Changed
 ~~~~~~~
 
 -  The collision behavior is changed to always warn.
--  Remove the ``collision_behavior`` argument. Use a `warning filter <https://docs.python.org/3.8/library/warnings.html>`__ instead.
+-  Remove the ``collision_behavior`` argument. Use a `warning filter <https://docs.python.org/3/library/warnings.html>`__ instead.
 -  Add ``path`` and ``id`` properties to ``DuplicateIdValueWarning`` to store the ``path`` at which, and the ``id`` on which, the collision occurred.
 
 0.5.10.post2 (2019-11-22)
 -------------------------
 
 Changed
 ~~~~~~~
@@ -125,15 +140,15 @@
 
 Changed
 ~~~~~~~
 
 -  Warn if multiple objects in an array have the same ``id`` value.
 -  Add a ``collision_behavior`` argument to ``merge``, ``merge_versioned``, ``add_release_to_compiled_release`` and ``add_release_to_versioned_release``, which can be set to:
 
-   -  ``ocdsmerge.WARN``: issue a ``DuplicateIdValueWarning`` `warning <https://docs.python.org/3.8/library/warnings.html>`__ (default)
+   -  ``ocdsmerge.WARN``: issue a ``DuplicateIdValueWarning`` `warning <https://docs.python.org/3/library/warnings.html>`__ (default)
    -  ``ocdsmerge.RAISE``: raise a ``DuplicateIdValueError`` exception
    -  ``ocdsmerge.IGNORE``: silently ignore the collision
 
 0.5.9 (2019-11-20)
 ------------------
 
 Fixed
```

### Comparing `ocdsmerge-0.6.6/README.rst` & `ocdsmerge-0.7.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-|PyPI Version| |Build Status| |Lint Status| |Coverage Status| |Python Version|
+|PyPI Version| |Build Status| |Coverage Status| |Python Version|
 
 This Python package creates records that conform to the `Open Contracting Data Standard <https://standard.open-contracting.org>`__. Specifically, it provides classes for merging OCDS releases with the same OCID into either a compiled release or a versioned release (collectively called "merged releases"), as described in the `OCDS documentation <https://standard.open-contracting.org/latest/en/schema/merging/>`__.
 
 Instead of using this library directly, it is easier to create merged releases using either:
 
 -  `OCDS Kit <https://ocdskit.readthedocs.io/>`__'s `compile <https://ocdskit.readthedocs.io/en/latest/cli/ocds.html#compile>`__ command-line tool
 -  OCDS Kit's `merge <https://ocdskit.readthedocs.io/en/latest/api/combine.html#ocdskit.combine.merge>`__ Python function
--  `OCDS Toucan <https://toucan.open-contracting.org/>`__'s `compile releases <https://toucan.open-contracting.org/compile/>`__ web application
 
-If you are viewing this on GitHub or PyPi, open the `full documentation <https://ocds-merge.readthedocs.io/>`__ for additional details.
+If you are viewing this on GitHub or PyPI, open the `full documentation <https://ocds-merge.readthedocs.io/>`__ for additional details.
 
 .. |PyPI Version| image:: https://img.shields.io/pypi/v/ocdsmerge.svg
    :target: https://pypi.org/project/ocdsmerge/
-.. |Build Status| image:: https://github.com/open-contracting/ocds-merge/workflows/CI/badge.svg
-.. |Lint Status| image:: https://github.com/open-contracting/ocds-merge/workflows/Lint/badge.svg
+.. |Build Status| image:: https://github.com/open-contracting/ocds-merge/actions/workflows/ci.yml/badge.svg
+   :target: https://github.com/open-contracting/ocds-merge/actions/workflows/ci.yml
 .. |Coverage Status| image:: https://coveralls.io/repos/github/open-contracting/ocds-merge/badge.svg?branch=main
    :target: https://coveralls.io/github/open-contracting/ocds-merge?branch=main
 .. |Python Version| image:: https://img.shields.io/pypi/pyversions/ocdsmerge.svg
    :target: https://pypi.org/project/ocdsmerge/
```

### Comparing `ocdsmerge-0.6.6/ocdsmerge/merge.py` & `ocdsmerge-0.7.0/ocdsmerge/merge.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,63 +1,76 @@
-from ocdsmerge.flatten import flatten, unflatten
-from ocdsmerge.rules import get_merge_rules
+from typing import Any, Dict, List, Optional, Type
+
+from ocdsmerge.flatten import Flattened, RuleOverrides, flatten, unflatten
+from ocdsmerge.rules import MergeRules, Schema, get_merge_rules
 from ocdsmerge.util import sorted_releases
 
 
 class Merger:
-    def __init__(self, schema=None, merge_rules=None, rule_overrides=None):
+    def __init__(
+        self,
+        schema: Schema = None,
+        merge_rules: Optional[MergeRules] = None,
+        rule_overrides: Optional[RuleOverrides] = None,
+    ):
         """
         Initializes a reusable ``Merger`` instance for creating merged releases.
 
         :param schema: the release schema (if not provided, will default to the latest version of OCDS)
-        :param dict merge_rules: the merge rules (if not provided, will determine the rules from the ``schema``)
-        :param dict rule_overrides: any rule overrides, in which keys are field paths as tuples, and values are either
+        :param merge_rules: the merge rules (if not provided, will determine the rules from the ``schema``)
+        :param rule_overrides: any rule overrides, in which keys are field paths as tuples, and values are either
             ``ocdsmerge.APPEND`` or ``ocdsmerge.MERGE_BY_POSITION``
         :type schema: dict or str
         """
         if merge_rules is None:
             merge_rules = get_merge_rules(schema)
         if rule_overrides is None:
             rule_overrides = {}
 
         self.merge_rules = merge_rules
         self.rule_overrides = rule_overrides
 
-    def create_compiled_release(self, releases):
+    def create_compiled_release(self, releases: List[Dict[str, Any]]) -> Dict[str, Any]:
         """
         Merges a list of releases into a compiled release.
         """
         return self._create_merged_release(CompiledRelease, releases)
 
-    def create_versioned_release(self, releases):
+    def create_versioned_release(self, releases: List[Dict[str, Any]]) -> Dict[str, Any]:
         """
         Merges a list of releases into a versioned release.
         """
         return self._create_merged_release(VersionedRelease, releases)
 
-    def _create_merged_release(self, cls, releases):
+    def _create_merged_release(self, cls: Type["MergedRelease"], releases: List[Dict[str, Any]]) -> Dict[str, Any]:
         merged_release = cls(merge_rules=self.merge_rules, rule_overrides=self.rule_overrides)
         merged_release.extend(releases)
         return merged_release.asdict()
 
 
 class MergedRelease:
     """
     Whether the class is for merging versioned releases.
     """
-    versioned = None
+    versioned: Optional[bool] = None
 
-    def __init__(self, data=None, schema=None, merge_rules=None, rule_overrides=None):
+    def __init__(
+        self,
+        data: Optional[Dict[str, Any]] = None,
+        schema: Schema = None,
+        merge_rules: Optional[MergeRules] = None,
+        rule_overrides: Optional[RuleOverrides] = None,
+    ):
         """
         Initializes a merged release.
 
-        :param dict data: the latest copy of the merged release, if any
+        :param data: the latest copy of the merged release, if any
         :param schema: the release schema (if not provided, will default to the latest version of OCDS)
-        :param dict merge_rules: the merge rules (if not provided, will determine the rules from the ``schema``)
-        :param dict rule_overrides: any rule overrides, in which keys are field paths as tuples, and values are either
+        :param merge_rules: the merge rules (if not provided, will determine the rules from the ``schema``)
+        :param rule_overrides: any rule overrides, in which keys are field paths as tuples, and values are either
             ``ocdsmerge.APPEND`` or ``ocdsmerge.MERGE_BY_POSITION``
         :type schema: dict or str
         """
         if merge_rules is None:
             merge_rules = get_merge_rules(schema)
         if rule_overrides is None:
             rule_overrides = {}
@@ -66,28 +79,28 @@
         self.rule_overrides = rule_overrides
 
         if data is None:
             self.data = {}
         else:
             self.data = flatten(data, self.merge_rules, self.rule_overrides, flattened={}, versioned=self.versioned)
 
-    def asdict(self):
+    def asdict(self) -> Dict[str, Any]:
         """
         Returns the merged release as a dictionary.
         """
         return unflatten(self.data)
 
-    def extend(self, releases):
+    def extend(self, releases: List[Dict[str, Any]]) -> None:
         """
         Sorts and merges many releases into the merged release.
         """
         for release in sorted_releases(releases):
             self.append(release)
 
-    def append(self, release):
+    def append(self, release: Dict[str, Any]) -> None:
         """
         Merges one release into the merged release.
         """
         release = release.copy()
 
         # Store the values of fields that set "omitWhenMerged": true.
         ocid = release.get('ocid')
@@ -95,39 +108,45 @@
         date = release.get('date')
         # Prior to OCDS 1.1.4, `tag` didn't set "omitWhenMerged": true.
         tag = release.pop('tag', None)
 
         flat = flatten(release, self.merge_rules, self.rule_overrides, flattened={})
         self.flat_append(flat, ocid, release_id, date, tag)
 
-    def flat_append(self, flat, ocid, release_id, date, tag):
+    def flat_append(
+        self, flat: Flattened, ocid: Optional[str], release_id: Optional[str], date: Optional[str], tag: Optional[str]
+    ) -> None:
         raise NotImplementedError('subclasses must implement flat_append()')
 
 
 class CompiledRelease(MergedRelease):
     versioned = False
 
-    def __init__(self, data=None, **kwargs):
+    def __init__(self, data: Optional[Dict[str, Any]] = None, **kwargs):
         super().__init__(data, **kwargs)
         self.data[('tag',)] = ['compiled']
 
-    def flat_append(self, flat, ocid, release_id, date, tag):
+    def flat_append(
+        self, flat: Flattened, ocid: Optional[str], release_id: Optional[str], date: Optional[str], tag: Optional[str]
+    ) -> None:
         # Add an `id` and `date`.
-        self.data[('id',)] = '{}-{}'.format(ocid, date)
+        self.data[('id',)] = f'{ocid}-{date}'
         self.data[('date',)] = date
         # In OCDS 1.0, `ocid` incorrectly sets "mergeStrategy": "ocdsOmit".
         self.data[('ocid',)] = ocid
 
         self.data.update(flat)
 
 
 class VersionedRelease(MergedRelease):
     versioned = True
 
-    def flat_append(self, flat, ocid, release_id, date, tag):
+    def flat_append(
+        self, flat: Flattened, ocid: Optional[str], release_id: Optional[str], date: Optional[str], tag: Optional[str]
+    ) -> None:
         # Don't version the OCID.
         flat.pop(('ocid',), None)
         self.data[('ocid',)] = ocid
 
         for key, value in flat.items():
             # If key is not versioned, continue. If the value is unchanged, don't add it to the history.
             if key in self.data and (type(self.data[key]) is not list or value == self.data[key][-1]['value']):
```

### Comparing `ocdsmerge-0.6.6/ocdsmerge/flatten.py` & `ocdsmerge-0.7.0/ocdsmerge/flatten.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,68 +1,69 @@
 import uuid
 import warnings
 from enum import Enum, auto, unique
+from typing import Any, Dict, Generator, List, Optional, Tuple, Union
 
 from ocdsmerge.exceptions import DuplicateIdValueWarning, InconsistentTypeError
+from ocdsmerge.rules import MergeRules
 
 VERSIONED_VALUE_KEYS = frozenset(['releaseID', 'releaseDate', 'releaseTag', 'value'])
 
 
 @unique
 class MergeStrategy(Enum):
     APPEND = auto()
     MERGE_BY_POSITION = auto()
 
 
 globals().update(MergeStrategy.__members__)
 
+Identifier = Union[int, str]
+Flattened = Dict[Tuple[Identifier, ...], Any]
+RuleOverrides = Dict[Tuple[str, ...], MergeStrategy]
+
 
 class IdValue(str):
     """
     A string with ``identifier`` and ``original_value`` properties.
     """
-    def __init__(self, identifier):
+    def __init__(self, identifier: Identifier):
         self.identifier = identifier
         str.__init__(identifier)
 
     @property
-    def original_value(self):
+    def original_value(self) -> Optional[Identifier]:
         return self._original_value
 
     @original_value.setter
-    def original_value(self, original_value):
+    def original_value(self, original_value: Optional[Identifier]) -> None:
         self._original_value = original_value
 
 
-class IdDict(dict):
-    """
-    A dictionary with an ``identifier`` property.
-    """
-    @property
-    def identifier(self):
-        return self._identifier
-
-    @identifier.setter
-    def identifier(self, identifier):
-        self._identifier = identifier
-
-
-def is_versioned_value(value):
+def is_versioned_value(value: Dict[str, Any]) -> bool:
     """
     Returns whether the value is a versioned value.
     """
     return len(value) == 4 and VERSIONED_VALUE_KEYS.issuperset(value)
 
 
-def flatten(obj, merge_rules, rule_overrides, flattened, path=(), rule_path=(), versioned=False):
+def flatten(
+    obj: Union[List[Dict[str, Any]], Dict[str, Any]],
+    merge_rules: MergeRules,
+    rule_overrides: RuleOverrides,
+    flattened: Flattened,
+    path: Tuple[Identifier, ...] = (),
+    rule_path: Tuple[str, ...] = (),
+    versioned: Optional[bool] = False
+) -> Flattened:
     """
     Flattens a JSON object into key-value pairs, in which the key is the JSON path as a tuple. For example:
 
     Replaces numbers in JSON paths (representing positions in arrays) with special objects. This ensures that objects
-    in arrays with different `id` values have different JSON paths – and makes it easy to identify such arrays.
+    in arrays with different `id` values have different JSON paths – and makes it easy to identify such arrays.
 
     .. code:: json
 
        {
            "a": "I am a",
            "b": ["A", "list"],
            "c": [
@@ -94,65 +95,69 @@
         is_dict = True
         iterable = obj.items()
 
     for key, value in iterable:
         if is_dict:
             new_rule_path = rule_path + (key,)
 
-        new_path_merge_rules = merge_rules.get(new_rule_path, set())
+        new_path_merge_rules = merge_rules.get(new_rule_path, None)
 
-        if 'omitWhenMerged' in new_path_merge_rules:
+        if new_path_merge_rules == 'omitWhenMerged':
             continue
         # If it's `wholeListMerge`, if it's neither an object nor an array, if it's an array containing non-objects
         # (even if `wholeListMerge` is `false`), or if it's versioned values, use the whole list merge strategy.
         # Note: Behavior is undefined and inconsistent if the array is not in the schema and contains objects in some
         # cases but not in others.
         # See https://standard.open-contracting.org/1.1/en/schema/merging/#whole-list-merge
         # See https://standard.open-contracting.org/1.1/en/schema/merging/#objects
-        elif 'wholeListMerge' in new_path_merge_rules or not isinstance(value, (dict, list)) or \
+        elif new_path_merge_rules == 'wholeListMerge' or not isinstance(value, (dict, list)) or \
                 type(value) is list and any(not isinstance(item, dict) for item in value) or \
                 versioned and value and all(is_versioned_value(item) for item in value):
             flattened[path + (key,)] = value
         # Recurse into non-empty objects, and arrays of objects that aren't `wholeListMerge`.
         elif value:
             flatten(value, merge_rules, rule_overrides, flattened, path + (key,), new_rule_path, versioned)
 
     return flattened
 
 
-def _enumerate(obj, path, rule_path, rule):
+def _enumerate(
+    obj: List[Dict[str, Any]], path: Tuple[Identifier, ...], rule_path: Tuple[str, ...], rule: Optional[MergeStrategy]
+) -> Generator[Tuple[IdValue, Any], None, None]:
     # This tracks the identifiers of objects in an array, to warn about collisions.
     identifiers = {}
 
     for key, value in enumerate(obj):
         new_key, default_key = _id_value(key, value, rule)
 
         # Check whether the identifier is used by other objects in the array.
         default_path = path + (default_key,)
         if default_path not in identifiers:
             identifiers[default_path] = key
         elif identifiers[default_path] != key:
-            warnings.warn(DuplicateIdValueWarning(rule_path, default_key, 'Multiple objects have the `id` '
-                          'value {!r} in the `{}` array'.format(default_key, '.'.join(map(str, rule_path)))))
+            warnings.warn(
+                f'Multiple objects have the `id` value {default_key!r} in the `{".".join(map(str, rule_path))}` array',
+                category=DuplicateIdValueWarning,
+            )
 
         yield new_key, value
 
 
-def _id_value(key, value, rule):
+def _id_value(key: int, value: Dict[str, Any], rule: Optional[MergeStrategy]) -> Tuple[IdValue, IdValue]:
     # If it is an array of objects, get the `id` value to apply the identifier merge strategy.
     # https://standard.open-contracting.org/latest/en/schema/merging/#identifier-merge
     if 'id' in value:
         id_value = value['id']
         identifier = id_value
     # If the object contained no top-level `id` value, set a unique value.
     else:
         id_value = None
         identifier = str(uuid.uuid1(1))  # use 1 instead of MAC address
 
-    # Calculate the default key for the warning.
+    # Calculate the key for the warning, which checks for collisions using the default merge strategy.
     default_key = IdValue(identifier)
 
     if rule == MergeStrategy.APPEND:
         if 'id' in value:
             new_key = IdValue(str(uuid.uuid1(1)))
         else:  # avoid creating an extra UUID
             new_key = default_key
@@ -163,72 +168,67 @@
 
     # Save the original value. (If the value is an integer, this avoids coercing it to a string.)
     new_key.original_value = id_value
 
     return new_key, default_key
 
 
-def unflatten(flattened):
+def unflatten(flattened: Flattened) -> Dict[str, Any]:
     """
     Unflattens a flattened object into a JSON object.
     """
-    unflattened = {}
+    unflattened: Dict[str, Any] = {}
 
-    identifiers = {}
+    identifiers: Dict[Tuple[Identifier, ...], Dict] = {}
 
     for key in flattened:
         current_node = unflattened
 
         for end, part in enumerate(key, 1):
+            # When running mypy, uncomment these lines:
+            # if TYPE_CHECKING:
+            #     assert type(part) is str
+
             # If this is a path to an item of an array.
             # See https://standard.open-contracting.org/1.1/en/schema/merging/#identifier-merge
             if type(part) is IdValue:
-                path = key[:end]
-
-                # If the `id` of an object in the array matches, change into it.
-                id_path = path + (part.identifier,)
-                if id_path in identifiers:
-                    current_node = identifiers[id_path]
-
-                # Otherwise, append a new object, and change into it.
-                else:
-                    new_node = IdDict()
-                    new_node.identifier = part.identifier
+                # If no `id` of an object in the array matches, append a new object.
+                id_path = key[:end - 1] + (part.identifier,)
+                if id_path not in identifiers:
+                    new_node = {}
 
                     # If the original object had an `id` value, set it.
                     if part.original_value is not None:
                         new_node['id'] = part.original_value
 
                     # Cache which identifiers appear in which arrays.
-                    identifiers[path + (new_node.identifier,)] = new_node
+                    identifiers[id_path] = new_node
 
                     current_node.append(new_node)
-                    current_node = new_node
 
-                continue
+                # Change into it.
+                current_node = identifiers[id_path]
 
-            if not isinstance(current_node, dict):
+            elif not isinstance(current_node, dict):
                 message = 'An earlier release had the literal {!r} for /{}, but the current release has an object with a {!r} key'  # noqa: E501
                 raise InconsistentTypeError(message.format(current_node, '/'.join(key[:end - 1]), part))
 
             # Otherwise, this is a path to a property of an object. If this is a path to a node we visited before,
             # change into it. If it's an `id` field, it's already been set to its original value.
-            if part in current_node:
+            elif part in current_node:
                 current_node = current_node[part]
-                continue
 
-            if end < len(key):
+            elif end < len(key):
                 # If the path is to a new array, start a new array, and change into it.
                 if type(key[end]) is IdValue:
                     current_node[part] = []
                 # If the path is to a new object, start a new object, and change into it.
                 else:
                     current_node[part] = {}
 
                 current_node = current_node[part]
-                continue
 
             # If this is a full path, copy the data, omitting null'ed fields.
-            if flattened[key] is not None:
+            elif flattened[key] is not None:
                 current_node[part] = flattened[key]
 
     return unflattened
```

### Comparing `ocdsmerge-0.6.6/ocdsmerge/util.py` & `ocdsmerge-0.7.0/ocdsmerge/util.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,43 @@
 import re
 from functools import lru_cache
+from typing import Any, Dict, List
 
 import requests
 
-from ocdsmerge.exceptions import (MissingDateKeyError, NonObjectReleaseError, NonStringDateValueError,
-                                  NullDateValueError)
+from ocdsmerge.exceptions import (
+    MissingDateKeyError,
+    NonObjectReleaseError,
+    NonStringDateValueError,
+    NullDateValueError,
+)
 
 
-@lru_cache()
-def get_tags():
+@lru_cache
+def get_tags() -> List[str]:
     """
     Returns the tags of all versions of OCDS in alphabetical order.
     """
-    return re.findall(r'"(\d+__\d+__\d+)/', requests.get('https://standard.open-contracting.org/schema/').text)
+    # response = requests.get('https://api.github.com/repos/open-contracting/standard/tags')
+    # response.raise_for_status()
+    # return [tag['name'] for tag in response.text()]
+    response = requests.get('https://standard.open-contracting.org/schema/')
+    response.raise_for_status()
+    return re.findall(r'"(\d+__\d+__\d+)/', response.text)
 
 
-def get_release_schema_url(tag):
+def get_release_schema_url(tag: str) -> str:
     """
     Returns the URL of the release schema in the given version of OCDS.
     """
-    return 'https://standard.open-contracting.org/schema/{}/release-schema.json'.format(tag)
+    return f'https://standard.open-contracting.org/schema/{tag}/release-schema.json'
 
 
 # If we need a method to get dates from releases, see https://github.com/open-contracting/ocds-merge/issues/25
-def sorted_releases(releases):
+def sorted_releases(releases: List[Dict[str, Any]]) -> List[Dict[str, Any]]:
     """
     Sorts a list of releases by date.
     """
     # Avoids an error if sorting a single compiled release.
     if isinstance(releases, list) and len(releases) == 1 and isinstance(releases[0], dict):
         return releases
     try:
@@ -36,21 +46,23 @@
         raise MissingDateKeyError('date', 'The `date` field of at least one release is missing.')
     except TypeError as e:
         if ' not supported between instances of ' in e.args[0]:
             if 'NoneType' in e.args[0]:
                 raise NullDateValueError('The `date` field of at least one release is null.')
             else:
                 raise NonStringDateValueError('The `date` field of at least one release is not a string.')
-        elif e.args[0] == 'string indices must be integers':
+        elif e.args[0] in ('string indices must be integers', "string indices must be integers, not 'str'",
+                           'string index indices must be integers or slices, not str'):
             raise NonObjectReleaseError('At least one release is a string, not a dict. Use `json.loads` to parse the '
                                         'string as JSON.')
         elif e.args[0] == 'byte indices must be integers or slices, not str':
             raise NonObjectReleaseError('At least one release is a byte-string, not a dict. Use `json.loads` to parse '
                                         'the byte-string as JSON.')
         elif e.args[0] == 'list indices must be integers or slices, not str':
             raise NonObjectReleaseError('At least one release is a list, not a dict.')
         elif e.args[0] == 'tuple indices must be integers or slices, not str':
             raise NonObjectReleaseError('At least one release is a tuple, not a dict.')
-        elif e.args[0] == "'set' object is not subscriptable":
+        elif e.args[0] in ("'set' object is not subscriptable",
+                           "'set' object is not subscriptable (key 'date')"):
             raise NonObjectReleaseError('At least one release is a set, not a dict.')
         else:
             raise
```

### Comparing `ocdsmerge-0.6.6/ocdsmerge/exceptions.py` & `ocdsmerge-0.7.0/ocdsmerge/exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 class OCDSMergeError(Exception):
     """Base class for exceptions from within this package"""
 
 
 class MissingDateKeyError(OCDSMergeError, KeyError):
     """Raised when a release is missing a 'date' key"""
 
-    def __init__(self, key, message):
+    def __init__(self, key: str, message: str):
         self.key = key
         self.message = message
 
-    def __str__(self):
+    def __str__(self) -> str:
         return str(self.message)
 
 
 class NonObjectReleaseError(OCDSMergeError, TypeError):
     """Raised when a release is not an object"""
 
 
@@ -31,15 +31,7 @@
 
 class OCDSMergeWarning(UserWarning):
     """Base class for warnings from within this package"""
 
 
 class DuplicateIdValueWarning(OCDSMergeWarning):
     """Used when at least two objects in the same array have the same value for the 'id' field"""
-
-    def __init__(self, path, id, message):
-        self.path = path
-        self.id = id
-        self.message = message
-
-    def __str__(self):
-        return str(self.message)
```

