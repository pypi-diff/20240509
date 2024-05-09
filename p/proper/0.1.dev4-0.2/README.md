# Comparing `tmp/proper-0.1.dev4.tar.gz` & `tmp/proper-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/proper-0.1.dev4.tar", last modified: Fri Sep 10 20:41:21 2021, max compression
+gzip compressed data, was "proper-0.2.tar", last modified: Thu May  9 20:45:46 2024, max compression
```

## Comparing `proper-0.1.dev4.tar` & `proper-0.2.tar`

### file list

```diff
@@ -1,337 +1,224 @@
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.369338 proper-0.1.dev4/
--rw-r--r--   0 jps        (501) staff       (20)      104 2021-07-22 22:24:27.000000 proper-0.1.dev4/MANIFEST.in
--rw-r--r--   0 jps        (501) staff       (20)     1063 2021-06-18 22:51:22.000000 proper-0.1.dev4/MIT-LICENSE
--rw-r--r--   0 jps        (501) staff       (20)     3179 2021-09-10 20:41:21.369693 proper-0.1.dev4/PKG-INFO
--rw-r--r--   0 jps        (501) staff       (20)     1971 2020-12-13 02:49:43.000000 proper-0.1.dev4/README.md
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.129122 proper-0.1.dev4/blueprints/
--rw-r--r--   0 jps        (501) staff       (20)     6148 2021-09-06 21:02:09.000000 proper-0.1.dev4/blueprints/.DS_Store
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.131442 proper-0.1.dev4/blueprints/controller/
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.100595 proper-0.1.dev4/blueprints/controller/[[ app_name ]]/
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.133378 proper-0.1.dev4/blueprints/controller/[[ app_name ]]/controllers/
--rw-r--r--   0 jps        (501) staff       (20)      199 2021-09-03 22:24:09.000000 proper-0.1.dev4/blueprints/controller/[[ app_name ]]/controllers/[[ snake_name ]].tmpl.py
--rw-r--r--   0 jps        (501) staff       (20)       45 2021-09-03 22:24:04.000000 proper-0.1.dev4/blueprints/controller/[[ app_name ]]/controllers/__init__.append.py
--rw-r--r--   0 jps        (501) staff       (20)      141 2021-09-03 22:23:59.000000 proper-0.1.dev4/blueprints/controller/routes.tmpl.py
--rw-r--r--   0 jps        (501) staff       (20)      112 2021-09-03 22:23:51.000000 proper-0.1.dev4/blueprints/controller/template.tmpl.html.jinja
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.100897 proper-0.1.dev4/blueprints/model/
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.101005 proper-0.1.dev4/blueprints/model/[[ app_name ]]/
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.135326 proper-0.1.dev4/blueprints/model/[[ app_name ]]/models/
--rw-r--r--   0 jps        (501) staff       (20)      301 2021-09-06 03:09:24.000000 proper-0.1.dev4/blueprints/model/[[ app_name ]]/models/[[ snake_name ]].tmpl.py
--rw-r--r--   0 jps        (501) staff       (20)       45 2021-09-03 22:23:35.000000 proper-0.1.dev4/blueprints/model/[[ app_name ]]/models/__init__.append.py
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.145661 proper-0.1.dev4/blueprints/project/
--rw-r--r--   0 jps        (501) staff       (20)    10244 2021-09-06 21:02:09.000000 proper-0.1.dev4/blueprints/project/.DS_Store
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.146714 proper-0.1.dev4/blueprints/project/.well-known/
--rw-r--r--   0 jps        (501) staff       (20)        0 2021-09-02 17:41:54.000000 proper-0.1.dev4/blueprints/project/.well-known/.keep
--rw-r--r--   0 jps        (501) staff       (20)      368 2021-09-02 17:14:59.000000 proper-0.1.dev4/blueprints/project/Dockerfile.tmpl
--rwxr-xr-x   0 jps        (501) staff       (20)      638 2021-09-03 22:26:36.000000 proper-0.1.dev4/blueprints/project/Makefile.tmpl
--rwxr-xr-x   0 jps        (501) staff       (20)     1254 2021-09-02 17:20:11.000000 proper-0.1.dev4/blueprints/project/README.tmpl.md
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.150870 proper-0.1.dev4/blueprints/project/[[ app_name ]]/
--rw-r--r--   0 jps        (501) staff       (20)     8196 2021-09-06 21:02:15.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/.DS_Store
--rw-r--r--   0 jps        (501) staff       (20)       35 2020-11-14 19:58:15.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/__init__.py
--rwxr-xr-x   0 jps        (501) staff       (20)      305 2021-09-03 03:00:23.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/app.tmpl.py
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.157451 proper-0.1.dev4/blueprints/project/[[ app_name ]]/config/
--rw-r--r--   0 jps        (501) staff       (20)      683 2021-08-01 03:16:28.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/config/__init__.py
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.164559 proper-0.1.dev4/blueprints/project/[[ app_name ]]/config/__pycache__/
--rw-r--r--   0 jps        (501) staff       (20)      881 2021-08-28 04:04:26.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/config/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)      352 2021-07-30 23:43:12.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/config/__pycache__/development.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)      323 2021-07-27 16:16:47.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/config/__pycache__/production.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)      929 2021-08-29 22:39:25.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/config/__pycache__/shared.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)      214 2021-07-27 16:16:47.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/config/__pycache__/staging.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)      373 2021-07-30 23:42:44.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/config/__pycache__/testing.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)      284 2021-09-03 03:07:47.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/config/development.tmpl.py
--rw-r--r--   0 jps        (501) staff       (20)      144 2021-09-03 03:07:40.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/config/production.py
--rw-r--r--   0 jps        (501) staff       (20)      651 2021-09-04 02:53:28.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/config/shared.tmpl.py
--rw-r--r--   0 jps        (501) staff       (20)      104 2021-06-24 18:21:38.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/config/staging.py
--rw-r--r--   0 jps        (501) staff       (20)      247 2021-09-03 03:08:07.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/config/testing.tmpl.py
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.169086 proper-0.1.dev4/blueprints/project/[[ app_name ]]/controllers/
--rw-r--r--   0 jps        (501) staff       (20)     6148 2021-09-06 21:05:39.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/controllers/.DS_Store
--rwxr-xr-x   0 jps        (501) staff       (20)      114 2021-09-06 21:21:16.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/controllers/__init__.py
--rwxr-xr-x   0 jps        (501) staff       (20)     2662 2021-09-06 04:23:54.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/controllers/application.py
--rwxr-xr-x   0 jps        (501) staff       (20)     2590 2021-09-06 22:55:14.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/controllers/auth.py
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.171758 proper-0.1.dev4/blueprints/project/[[ app_name ]]/controllers/forms/
--rw-r--r--   0 jps        (501) staff       (20)        0 2021-09-06 20:51:40.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/controllers/forms/__init__.py
--rwxr-xr-x   0 jps        (501) staff       (20)     1694 2021-09-06 22:43:36.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/controllers/forms/auth.tmpl.py
--rw-r--r--   0 jps        (501) staff       (20)      807 2021-09-06 20:55:05.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/controllers/forms/pwned.py
--rwxr-xr-x   0 jps        (501) staff       (20)      193 2021-09-03 22:15:33.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/controllers/pages.py
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.173337 proper-0.1.dev4/blueprints/project/[[ app_name ]]/mailers/
--rw-r--r--   0 jps        (501) staff       (20)       28 2020-11-14 19:58:15.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/mailers/__init__.py
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.175531 proper-0.1.dev4/blueprints/project/[[ app_name ]]/mailers/__pycache__/
--rw-r--r--   0 jps        (501) staff       (20)      138 2021-07-27 16:16:48.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/mailers/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)      835 2021-07-27 16:16:48.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/mailers/__pycache__/auth.cpython-39.pyc
--rwxr-xr-x   0 jps        (501) staff       (20)      706 2021-09-03 22:18:00.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/mailers/auth.py
--rwxr-xr-x   0 jps        (501) staff       (20)      676 2021-09-06 22:39:54.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/main.py
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.177868 proper-0.1.dev4/blueprints/project/[[ app_name ]]/models/
--rwxr-xr-x   0 jps        (501) staff       (20)      101 2021-09-06 21:21:20.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/models/__init__.py
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.184174 proper-0.1.dev4/blueprints/project/[[ app_name ]]/models/__pycache__/
--rw-r--r--   0 jps        (501) staff       (20)      261 2021-07-27 16:16:47.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/models/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     1034 2021-08-29 22:39:26.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/models/__pycache__/base.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     2641 2021-07-27 16:16:47.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/models/__pycache__/post.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)      685 2021-07-27 16:16:48.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/models/__pycache__/relation.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     1336 2021-07-27 16:16:48.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/models/__pycache__/topic.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)      781 2021-07-27 16:16:48.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/models/__pycache__/user.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)      613 2021-09-06 22:39:46.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/models/base.py
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.186890 proper-0.1.dev4/blueprints/project/[[ app_name ]]/models/mixins/
--rwxr-xr-x   0 jps        (501) staff       (20)       94 2021-06-23 22:08:42.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/models/mixins/__init__.py
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.189748 proper-0.1.dev4/blueprints/project/[[ app_name ]]/models/mixins/__pycache__/
--rw-r--r--   0 jps        (501) staff       (20)      221 2021-07-27 16:16:47.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/models/mixins/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     2244 2021-07-27 16:16:47.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/models/mixins/__pycache__/authenticable.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)      543 2021-07-27 16:16:48.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/models/mixins/__pycache__/timestamped.cpython-39.pyc
--rwxr-xr-x   0 jps        (501) staff       (20)     1474 2021-09-06 22:44:03.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/models/mixins/authenticable.tmpl.py
--rw-r--r--   0 jps        (501) staff       (20)      363 2021-06-23 15:45:53.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/models/mixins/timestamped.py
--rwxr-xr-x   0 jps        (501) staff       (20)      200 2021-09-06 04:18:49.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/models/user.py
--rwxr-xr-x   0 jps        (501) staff       (20)     1070 2021-09-04 03:53:59.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/routes.py
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.191166 proper-0.1.dev4/blueprints/project/[[ app_name ]]/services/
--rw-r--r--   0 jps        (501) staff       (20)        0 2021-06-23 22:06:34.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/services/__init__.py
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.193939 proper-0.1.dev4/blueprints/project/[[ app_name ]]/services/__pycache__/
--rw-r--r--   0 jps        (501) staff       (20)      118 2021-07-27 16:16:47.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/services/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     1923 2021-07-30 21:22:12.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/services/__pycache__/auth_services.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     1482 2021-07-27 16:19:08.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/services/__pycache__/posts_services.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     1811 2021-09-03 22:18:54.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/services/auth_services.py
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.194988 proper-0.1.dev4/blueprints/project/[[ app_name ]]/templates/
--rw-r--r--   0 jps        (501) staff       (20)     6148 2021-09-06 21:02:02.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/templates/.DS_Store
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.199898 proper-0.1.dev4/blueprints/project/[[ app_name ]]/templates/auth/
--rwxr-xr-x   0 jps        (501) staff       (20)     1446 2021-09-06 21:29:14.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/templates/auth/password_change.html.jinja
--rwxr-xr-x   0 jps        (501) staff       (20)     1130 2021-09-06 21:29:08.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/templates/auth/reset.html.jinja
--rwxr-xr-x   0 jps        (501) staff       (20)      532 2021-02-19 03:36:58.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/templates/auth/reset_invalid.html.jinja
--rwxr-xr-x   0 jps        (501) staff       (20)      658 2021-02-19 03:36:58.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/templates/auth/reset_sent.html.jinja
--rwxr-xr-x   0 jps        (501) staff       (20)     1526 2021-09-06 21:28:59.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/templates/auth/sign_in.html.jinja
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.200589 proper-0.1.dev4/blueprints/project/[[ app_name ]]/templates/common/
--rw-r--r--   0 jps        (501) staff       (20)      283 2021-05-18 02:53:25.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/templates/common/Button.html.jinja
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.201604 proper-0.1.dev4/blueprints/project/[[ app_name ]]/templates/emails/
--rwxr-xr-x   0 jps        (501) staff       (20)      491 2021-09-03 22:10:03.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/templates/emails/password_reset.html.jinja
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.204706 proper-0.1.dev4/blueprints/project/[[ app_name ]]/templates/layouts/
--rwxr-xr-x   0 jps        (501) staff       (20)      604 2021-09-03 22:12:15.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/templates/layouts/application.html.jinja
--rwxr-xr-x   0 jps        (501) staff       (20)      772 2021-09-03 22:13:01.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/templates/layouts/auth.html.jinja
--rwxr-xr-x   0 jps        (501) staff       (20)      283 2021-09-03 22:13:10.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/templates/layouts/email.html.jinja
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.207819 proper-0.1.dev4/blueprints/project/[[ app_name ]]/templates/pages/
--rwxr-xr-x   0 jps        (501) staff       (20)      641 2021-09-03 22:13:51.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/templates/pages/error.html.jinja
--rwxr-xr-x   0 jps        (501) staff       (20)      136 2021-09-03 22:14:47.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/templates/pages/index.html.jinja
--rwxr-xr-x   0 jps        (501) staff       (20)      747 2021-09-03 22:14:53.000000 proper-0.1.dev4/blueprints/project/[[ app_name ]]/templates/pages/not_found.html.jinja
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.208838 proper-0.1.dev4/blueprints/project/db/
--rw-r--r--   0 jps        (501) staff       (20)     6148 2021-09-06 21:02:02.000000 proper-0.1.dev4/blueprints/project/db/.DS_Store
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.210683 proper-0.1.dev4/blueprints/project/db/migrations/
--rw-r--r--   0 jps        (501) staff       (20)        0 2021-02-22 18:34:20.000000 proper-0.1.dev4/blueprints/project/db/migrations/__init__.py
--rw-r--r--   0 jps        (501) staff       (20)      494 2021-07-04 03:08:09.000000 proper-0.1.dev4/blueprints/project/db/migrations/script.py.mako
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.212884 proper-0.1.dev4/blueprints/project/deploy/
--rw-r--r--   0 jps        (501) staff       (20)      885 2021-09-02 17:42:04.000000 proper-0.1.dev4/blueprints/project/deploy/nginx.tmpl.conf
--rw-r--r--   0 jps        (501) staff       (20)      720 2021-09-02 17:34:12.000000 proper-0.1.dev4/blueprints/project/deploy/uwsgi.tmpl.ini
--rw-r--r--   0 jps        (501) staff       (20)      414 2021-09-02 17:17:39.000000 proper-0.1.dev4/blueprints/project/docker-compose.tmpl.yml
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.213965 proper-0.1.dev4/blueprints/project/logs/
--rw-r--r--   0 jps        (501) staff       (20)        0 2021-05-07 20:16:59.000000 proper-0.1.dev4/blueprints/project/logs/.keep
--rwxr-xr-x   0 jps        (501) staff       (20)      979 2021-09-06 22:49:35.000000 proper-0.1.dev4/blueprints/project/manage.tmpl.py
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.217590 proper-0.1.dev4/blueprints/project/requirements/
--rw-r--r--   0 jps        (501) staff       (20)       51 2021-09-02 17:09:05.000000 proper-0.1.dev4/blueprints/project/requirements/dev-requirements.ini
--rw-r--r--   0 jps        (501) staff       (20)       29 2021-09-02 17:09:28.000000 proper-0.1.dev4/blueprints/project/requirements/prod-requirements.ini
--rw-r--r--   0 jps        (501) staff       (20)      326 2021-09-04 03:20:48.000000 proper-0.1.dev4/blueprints/project/requirements/requirements.ini
--rw-r--r--   0 jps        (501) staff       (20)       85 2021-09-02 17:08:34.000000 proper-0.1.dev4/blueprints/project/requirements/test-requirements.ini
--rw-r--r--   0 jps        (501) staff       (20)       38 2020-11-07 17:38:45.000000 proper-0.1.dev4/blueprints/project/setup.py
--rwxr-xr-x   0 jps        (501) staff       (20)      804 2021-09-06 20:58:41.000000 proper-0.1.dev4/blueprints/project/setup.tmpl.cfg
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.223590 proper-0.1.dev4/blueprints/project/static/
--rw-r--r--   0 jps        (501) staff       (20)     6148 2021-09-06 21:02:02.000000 proper-0.1.dev4/blueprints/project/static/.DS_Store
--rw-r--r--   0 jps        (501) staff       (20)      537 2020-11-14 19:58:15.000000 proper-0.1.dev4/blueprints/project/static/.eslintrc.js
--rw-r--r--   0 jps        (501) staff       (20)      978 2021-09-03 22:22:04.000000 proper-0.1.dev4/blueprints/project/static/package.json
--rw-r--r--   0 jps        (501) staff       (20)      246 2021-09-02 17:43:55.000000 proper-0.1.dev4/blueprints/project/static/postcss.config.js
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.225799 proper-0.1.dev4/blueprints/project/static/public/
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.226571 proper-0.1.dev4/blueprints/project/static/public/css/
--rw-r--r--   0 jps        (501) staff       (20)        0 2021-09-02 17:49:13.000000 proper-0.1.dev4/blueprints/project/static/public/css/.keep
--rw-r--r--   0 jps        (501) staff       (20)     4286 2020-11-14 19:58:15.000000 proper-0.1.dev4/blueprints/project/static/public/favicon.ico
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.227001 proper-0.1.dev4/blueprints/project/static/public/fonts/
--rw-r--r--   0 jps        (501) staff       (20)        0 2021-09-03 02:29:25.000000 proper-0.1.dev4/blueprints/project/static/public/fonts/.keep
--rw-r--r--   0 jps        (501) staff       (20)        0 2021-09-02 17:48:53.000000 proper-0.1.dev4/blueprints/project/static/public/humans.txt
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.227458 proper-0.1.dev4/blueprints/project/static/public/images/
--rw-r--r--   0 jps        (501) staff       (20)        0 2021-09-02 17:48:44.000000 proper-0.1.dev4/blueprints/project/static/public/images/.keep
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.227914 proper-0.1.dev4/blueprints/project/static/public/js/
--rw-r--r--   0 jps        (501) staff       (20)        0 2021-09-02 17:49:33.000000 proper-0.1.dev4/blueprints/project/static/public/js/.keep
--rw-r--r--   0 jps        (501) staff       (20)       27 2020-11-14 19:58:15.000000 proper-0.1.dev4/blueprints/project/static/public/robots.txt
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.228376 proper-0.1.dev4/blueprints/project/static/public/vendor/
--rw-r--r--   0 jps        (501) staff       (20)        0 2021-09-03 02:29:47.000000 proper-0.1.dev4/blueprints/project/static/public/vendor/.keep
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.111932 proper-0.1.dev4/blueprints/project/static/src/
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.234011 proper-0.1.dev4/blueprints/project/static/src/css/
--rw-r--r--   0 jps        (501) staff       (20)       83 2021-09-04 03:15:01.000000 proper-0.1.dev4/blueprints/project/static/src/css/_base.css
--rw-r--r--   0 jps        (501) staff       (20)     1498 2021-09-04 03:19:27.000000 proper-0.1.dev4/blueprints/project/static/src/css/_buttons.css
--rw-r--r--   0 jps        (501) staff       (20)      213 2021-09-04 03:17:25.000000 proper-0.1.dev4/blueprints/project/static/src/css/_components.css
--rw-r--r--   0 jps        (501) staff       (20)     2860 2021-03-21 03:07:49.000000 proper-0.1.dev4/blueprints/project/static/src/css/_forms.css
--rw-r--r--   0 jps        (501) staff       (20)       34 2021-03-21 03:07:49.000000 proper-0.1.dev4/blueprints/project/static/src/css/_utilities.css
--rw-r--r--   0 jps        (501) staff       (20)       27 2020-11-14 19:58:15.000000 proper-0.1.dev4/blueprints/project/static/src/css/email.css
--rw-r--r--   0 jps        (501) staff       (20)       80 2021-09-03 22:19:25.000000 proper-0.1.dev4/blueprints/project/static/src/css/styles.css
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.234856 proper-0.1.dev4/blueprints/project/static/src/js/
--rw-r--r--   0 jps        (501) staff       (20)        0 2021-09-02 17:45:07.000000 proper-0.1.dev4/blueprints/project/static/src/js/scripts.js
--rw-r--r--   0 jps        (501) staff       (20)      115 2021-09-02 17:44:49.000000 proper-0.1.dev4/blueprints/project/static/tailwind.config.tmpl.js
--rw-r--r--   0 jps        (501) staff       (20)      295 2021-01-19 03:43:09.000000 proper-0.1.dev4/blueprints/project/static/webpack.config.js
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.235285 proper-0.1.dev4/blueprints/project/tests/
--rw-r--r--   0 jps        (501) staff       (20)       53 2020-11-14 19:58:15.000000 proper-0.1.dev4/blueprints/project/tests/conftest.py
--rw-r--r--   0 jps        (501) staff       (20)      369 2021-08-29 22:24:50.000000 proper-0.1.dev4/blueprints/project/uwsgi-dev.ini
--rw-r--r--   0 jps        (501) staff       (20)       83 2021-09-02 17:01:52.000000 proper-0.1.dev4/blueprints/project/wsgi.tmpl.py
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.236101 proper-0.1.dev4/blueprints/resource/
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.113531 proper-0.1.dev4/blueprints/resource/[[ app_name ]]/
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.237797 proper-0.1.dev4/blueprints/resource/[[ app_name ]]/controllers/
--rw-r--r--   0 jps        (501) staff       (20)      357 2021-09-03 22:23:08.000000 proper-0.1.dev4/blueprints/resource/[[ app_name ]]/controllers/[[ snake_name ]].tmpl.py
--rw-r--r--   0 jps        (501) staff       (20)       45 2021-09-03 22:23:03.000000 proper-0.1.dev4/blueprints/resource/[[ app_name ]]/controllers/__init__.append.py
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.113749 proper-0.1.dev4/blueprints/resource/[[ app_name ]]/templates/
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.241448 proper-0.1.dev4/blueprints/resource/[[ app_name ]]/templates/[[ snake_name ]]/
--rw-r--r--   0 jps        (501) staff       (20)      112 2021-02-11 02:39:25.000000 proper-0.1.dev4/blueprints/resource/[[ app_name ]]/templates/[[ snake_name ]]/edit.html.jinja
--rw-r--r--   0 jps        (501) staff       (20)      112 2021-02-11 02:39:25.000000 proper-0.1.dev4/blueprints/resource/[[ app_name ]]/templates/[[ snake_name ]]/index.html.jinja
--rw-r--r--   0 jps        (501) staff       (20)      112 2021-02-11 02:39:25.000000 proper-0.1.dev4/blueprints/resource/[[ app_name ]]/templates/[[ snake_name ]]/new.html.jinja
--rw-r--r--   0 jps        (501) staff       (20)      112 2021-02-11 02:39:25.000000 proper-0.1.dev4/blueprints/resource/[[ app_name ]]/templates/[[ snake_name ]]/show.html.jinja
--rw-r--r--   0 jps        (501) staff       (20)      104 2021-09-03 22:22:46.000000 proper-0.1.dev4/blueprints/resource/routes.tmpl.py
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.248876 proper-0.1.dev4/proper/
--rw-r--r--   0 jps        (501) staff       (20)     8196 2021-09-06 21:02:02.000000 proper-0.1.dev4/proper/.DS_Store
--rw-r--r--   0 jps        (501) staff       (20)      245 2021-08-29 16:49:51.000000 proper-0.1.dev4/proper/__init__.py
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.260835 proper-0.1.dev4/proper/__pycache__/
--rw-r--r--   0 jps        (501) staff       (20)      286 2021-09-04 02:03:27.000000 proper-0.1.dev4/proper/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     7064 2021-09-04 02:03:28.000000 proper-0.1.dev4/proper/__pycache__/auth.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)      319 2021-09-04 02:03:27.000000 proper-0.1.dev4/proper/__pycache__/constants.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)    15526 2021-09-04 02:03:27.000000 proper-0.1.dev4/proper/__pycache__/errors.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     2710 2021-09-04 02:03:27.000000 proper-0.1.dev4/proper/__pycache__/local.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)    11516 2021-09-04 02:03:27.000000 proper-0.1.dev4/proper/__pycache__/request.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)    11097 2021-09-04 02:03:27.000000 proper-0.1.dev4/proper/__pycache__/response.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     4193 2021-09-04 02:03:28.000000 proper-0.1.dev4/proper/__pycache__/static.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     4126 2021-09-04 02:03:27.000000 proper-0.1.dev4/proper/__pycache__/status.cpython-39.pyc
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.267759 proper-0.1.dev4/proper/app/
--rw-r--r--   0 jps        (501) staff       (20)       27 2020-08-14 21:45:00.000000 proper-0.1.dev4/proper/app/__init__.py
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.275031 proper-0.1.dev4/proper/app/__pycache__/
--rw-r--r--   0 jps        (501) staff       (20)      156 2021-09-04 02:03:27.000000 proper-0.1.dev4/proper/app/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     2919 2021-09-04 02:03:27.000000 proper-0.1.dev4/proper/app/__pycache__/app.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     4173 2021-09-06 04:13:32.000000 proper-0.1.dev4/proper/app/__pycache__/cli.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     1399 2021-09-04 02:03:28.000000 proper-0.1.dev4/proper/app/__pycache__/cli_run.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)      535 2021-09-04 02:03:28.000000 proper-0.1.dev4/proper/app/__pycache__/default_config.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     2708 2021-09-04 02:03:27.000000 proper-0.1.dev4/proper/app/__pycache__/error_handlers.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     3172 2021-09-04 02:03:27.000000 proper-0.1.dev4/proper/app/__pycache__/errors_mixin.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     5683 2021-09-04 02:03:27.000000 proper-0.1.dev4/proper/app/__pycache__/setup_mixin.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     3317 2021-07-29 02:24:00.000000 proper-0.1.dev4/proper/app/app.py
--rw-r--r--   0 jps        (501) staff       (20)     3468 2021-09-06 04:13:11.000000 proper-0.1.dev4/proper/app/cli.py
--rw-r--r--   0 jps        (501) staff       (20)     1291 2021-09-03 02:49:29.000000 proper-0.1.dev4/proper/app/cli_run.py
--rw-r--r--   0 jps        (501) staff       (20)     1030 2021-01-23 15:07:44.000000 proper-0.1.dev4/proper/app/default_config.py
--rw-r--r--   0 jps        (501) staff       (20)     2324 2021-07-22 22:21:55.000000 proper-0.1.dev4/proper/app/error_handlers.py
--rw-r--r--   0 jps        (501) staff       (20)     3060 2021-07-28 17:03:51.000000 proper-0.1.dev4/proper/app/errors_mixin.py
--rw-r--r--   0 jps        (501) staff       (20)     5127 2021-07-28 16:53:03.000000 proper-0.1.dev4/proper/app/setup_mixin.py
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.286660 proper-0.1.dev4/proper/app/templates/
--rw-r--r--   0 jps        (501) staff       (20)     1036 2020-08-14 21:45:00.000000 proper-0.1.dev4/proper/app/templates/_context.html.jinja
--rw-r--r--   0 jps        (501) staff       (20)     1481 2020-08-14 21:45:00.000000 proper-0.1.dev4/proper/app/templates/_debug-styles.css
--rw-r--r--   0 jps        (501) staff       (20)     4260 2020-08-14 21:45:00.000000 proper-0.1.dev4/proper/app/templates/_prism.css
--rw-r--r--   0 jps        (501) staff       (20)     8483 2020-08-14 21:45:00.000000 proper-0.1.dev4/proper/app/templates/_prism.js
--rw-r--r--   0 jps        (501) staff       (20)      326 2020-08-14 21:45:00.000000 proper-0.1.dev4/proper/app/templates/debug-error.html.jinja
--rw-r--r--   0 jps        (501) staff       (20)     1351 2021-02-04 02:37:47.000000 proper-0.1.dev4/proper/app/templates/debug-not-found.html.jinja
--rw-r--r--   0 jps        (501) staff       (20)      909 2020-11-20 03:03:44.000000 proper-0.1.dev4/proper/app/templates/fallback-error.html
--rw-r--r--   0 jps        (501) staff       (20)     2347 2020-08-14 21:45:00.000000 proper-0.1.dev4/proper/app/templates/fallback-forbidden.html
--rw-r--r--   0 jps        (501) staff       (20)      940 2020-11-20 03:03:44.000000 proper-0.1.dev4/proper/app/templates/fallback-not-found.html
--rw-r--r--   0 jps        (501) staff       (20)      469 2020-08-14 21:45:00.000000 proper-0.1.dev4/proper/app/templates/layout.html.jinja
--rwxr-xr-x   0 jps        (501) staff       (20)     9403 2021-06-24 17:21:52.000000 proper-0.1.dev4/proper/auth.py
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.288100 proper-0.1.dev4/proper/cli/
--rw-r--r--   0 jps        (501) staff       (20)      605 2021-09-04 02:36:59.000000 proper-0.1.dev4/proper/cli/__init__.py
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.289641 proper-0.1.dev4/proper/cli/__pycache__/
--rw-r--r--   0 jps        (501) staff       (20)      882 2021-09-04 02:37:02.000000 proper-0.1.dev4/proper/cli/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     1574 2021-09-04 02:03:28.000000 proper-0.1.dev4/proper/cli/__pycache__/welcome.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     1400 2021-08-29 22:28:16.000000 proper-0.1.dev4/proper/cli/welcome.py
--rw-r--r--   0 jps        (501) staff       (20)      206 2020-08-14 21:45:00.000000 proper-0.1.dev4/proper/constants.py
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.292206 proper-0.1.dev4/proper/controller/
--rw-r--r--   0 jps        (501) staff       (20)       39 2021-02-27 23:04:58.000000 proper-0.1.dev4/proper/controller/__init__.py
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.294849 proper-0.1.dev4/proper/controller/__pycache__/
--rw-r--r--   0 jps        (501) staff       (20)      175 2021-09-04 02:03:28.000000 proper-0.1.dev4/proper/controller/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     1280 2021-09-04 02:03:28.000000 proper-0.1.dev4/proper/controller/__pycache__/base_channel.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     2528 2021-09-04 02:03:28.000000 proper-0.1.dev4/proper/controller/__pycache__/base_controller.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)      421 2020-08-14 21:45:00.000000 proper-0.1.dev4/proper/controller/base_channel.py
--rw-r--r--   0 jps        (501) staff       (20)     2108 2021-07-29 03:47:29.000000 proper-0.1.dev4/proper/controller/base_controller.py
--rw-r--r--   0 jps        (501) staff       (20)    12214 2020-08-14 21:45:00.000000 proper-0.1.dev4/proper/errors.py
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.300784 proper-0.1.dev4/proper/generators/
--rw-r--r--   0 jps        (501) staff       (20)      168 2021-09-04 02:00:04.000000 proper-0.1.dev4/proper/generators/__init__.py
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.308852 proper-0.1.dev4/proper/generators/__pycache__/
--rw-r--r--   0 jps        (501) staff       (20)      319 2021-09-04 02:03:28.000000 proper-0.1.dev4/proper/generators/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     1625 2021-09-04 03:29:51.000000 proper-0.1.dev4/proper/generators/__pycache__/controller.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)      351 2021-09-06 03:10:16.000000 proper-0.1.dev4/proper/generators/__pycache__/mailer.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     7251 2021-09-06 03:59:23.000000 proper-0.1.dev4/proper/generators/__pycache__/model.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     2590 2021-09-04 02:35:52.000000 proper-0.1.dev4/proper/generators/__pycache__/project.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     2748 2021-09-04 03:29:51.000000 proper-0.1.dev4/proper/generators/__pycache__/resource.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     1672 2021-09-04 03:29:29.000000 proper-0.1.dev4/proper/generators/controller.py
--rw-r--r--   0 jps        (501) staff       (20)      149 2021-09-04 03:29:18.000000 proper-0.1.dev4/proper/generators/mailer.py
--rw-r--r--   0 jps        (501) staff       (20)     7309 2021-09-06 03:59:16.000000 proper-0.1.dev4/proper/generators/model.py
--rw-r--r--   0 jps        (501) staff       (20)     2297 2021-09-04 02:35:19.000000 proper-0.1.dev4/proper/generators/project.py
--rw-r--r--   0 jps        (501) staff       (20)     2693 2021-09-04 03:29:08.000000 proper-0.1.dev4/proper/generators/resource.py
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.318854 proper-0.1.dev4/proper/helpers/
--rw-r--r--   0 jps        (501) staff       (20)      384 2021-07-28 16:55:25.000000 proper-0.1.dev4/proper/helpers/__init__.py
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.332817 proper-0.1.dev4/proper/helpers/__pycache__/
--rw-r--r--   0 jps        (501) staff       (20)      385 2021-09-04 02:03:27.000000 proper-0.1.dev4/proper/helpers/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     4911 2021-09-04 02:03:27.000000 proper-0.1.dev4/proper/helpers/__pycache__/cookies.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     1316 2021-09-04 02:03:27.000000 proper-0.1.dev4/proper/helpers/__pycache__/digestor.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     3590 2021-09-04 02:03:27.000000 proper-0.1.dev4/proper/helpers/__pycache__/dot.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)      957 2021-09-04 02:03:27.000000 proper-0.1.dev4/proper/helpers/__pycache__/encoding.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     2569 2021-09-04 02:03:27.000000 proper-0.1.dev4/proper/helpers/__pycache__/frozendict.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)      650 2021-09-04 02:03:27.000000 proper-0.1.dev4/proper/helpers/__pycache__/headersdict.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)      362 2021-09-04 02:03:27.000000 proper-0.1.dev4/proper/helpers/__pycache__/iterable.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     4104 2021-09-04 02:03:27.000000 proper-0.1.dev4/proper/helpers/__pycache__/multidict.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     9879 2021-09-04 02:03:27.000000 proper-0.1.dev4/proper/helpers/__pycache__/paginator.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     6755 2021-09-04 02:08:14.000000 proper-0.1.dev4/proper/helpers/__pycache__/render.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     1323 2021-09-04 02:03:27.000000 proper-0.1.dev4/proper/helpers/__pycache__/serializer.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     1734 2021-09-10 20:38:25.000000 proper-0.1.dev4/proper/helpers/__pycache__/slugify.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     5321 2020-11-27 02:33:54.000000 proper-0.1.dev4/proper/helpers/cookies.py
--rw-r--r--   0 jps        (501) staff       (20)      809 2021-01-10 02:45:48.000000 proper-0.1.dev4/proper/helpers/digestor.py
--rw-r--r--   0 jps        (501) staff       (20)     2784 2020-11-02 02:31:32.000000 proper-0.1.dev4/proper/helpers/dot.py
--rw-r--r--   0 jps        (501) staff       (20)      721 2020-11-02 02:31:32.000000 proper-0.1.dev4/proper/helpers/encoding.py
--rw-r--r--   0 jps        (501) staff       (20)     1421 2021-02-07 16:01:10.000000 proper-0.1.dev4/proper/helpers/frozendict.py
--rw-r--r--   0 jps        (501) staff       (20)      276 2020-11-02 02:31:32.000000 proper-0.1.dev4/proper/helpers/headersdict.py
--rw-r--r--   0 jps        (501) staff       (20)      158 2021-02-07 16:01:10.000000 proper-0.1.dev4/proper/helpers/iterable.py
--rw-r--r--   0 jps        (501) staff       (20)     3780 2020-11-02 02:31:32.000000 proper-0.1.dev4/proper/helpers/multidict.py
--rw-r--r--   0 jps        (501) staff       (20)     9974 2020-11-14 19:13:23.000000 proper-0.1.dev4/proper/helpers/paginator.py
--rw-r--r--   0 jps        (501) staff       (20)     6885 2021-09-04 02:08:11.000000 proper-0.1.dev4/proper/helpers/render.py
--rw-r--r--   0 jps        (501) staff       (20)     1107 2021-03-25 03:11:50.000000 proper-0.1.dev4/proper/helpers/serializer.py
--rw-r--r--   0 jps        (501) staff       (20)     1687 2021-09-08 21:17:45.000000 proper-0.1.dev4/proper/helpers/slugify.py
--rw-r--r--   0 jps        (501) staff       (20)     2218 2020-11-21 15:19:59.000000 proper-0.1.dev4/proper/local.py
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.339104 proper-0.1.dev4/proper/middleware/
--rw-r--r--   0 jps        (501) staff       (20)      345 2020-08-14 21:45:00.000000 proper-0.1.dev4/proper/middleware/README.md
--rw-r--r--   0 jps        (501) staff       (20)      235 2020-08-14 21:45:00.000000 proper-0.1.dev4/proper/middleware/__init__.py
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.346139 proper-0.1.dev4/proper/middleware/__pycache__/
--rw-r--r--   0 jps        (501) staff       (20)      299 2021-09-04 02:03:27.000000 proper-0.1.dev4/proper/middleware/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     1435 2021-09-04 02:03:27.000000 proper-0.1.dev4/proper/middleware/__pycache__/dispatch.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)      645 2021-09-04 02:03:27.000000 proper-0.1.dev4/proper/middleware/__pycache__/head.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)      526 2021-09-04 02:03:27.000000 proper-0.1.dev4/proper/middleware/__pycache__/match.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)      863 2021-09-04 02:03:27.000000 proper-0.1.dev4/proper/middleware/__pycache__/method_override.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     1852 2021-09-04 02:03:27.000000 proper-0.1.dev4/proper/middleware/__pycache__/protect_from_forgery.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)      608 2021-09-04 02:03:27.000000 proper-0.1.dev4/proper/middleware/__pycache__/redirect.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     1738 2021-09-04 02:03:27.000000 proper-0.1.dev4/proper/middleware/__pycache__/session.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     1459 2021-07-29 02:06:23.000000 proper-0.1.dev4/proper/middleware/dispatch.py
--rw-r--r--   0 jps        (501) staff       (20)      427 2021-07-28 03:25:12.000000 proper-0.1.dev4/proper/middleware/head.py
--rw-r--r--   0 jps        (501) staff       (20)      386 2021-07-28 03:25:19.000000 proper-0.1.dev4/proper/middleware/match.py
--rw-r--r--   0 jps        (501) staff       (20)      729 2021-07-28 03:25:26.000000 proper-0.1.dev4/proper/middleware/method_override.py
--rw-r--r--   0 jps        (501) staff       (20)     1766 2021-07-28 03:25:32.000000 proper-0.1.dev4/proper/middleware/protect_from_forgery.py
--rw-r--r--   0 jps        (501) staff       (20)      484 2021-07-28 03:26:14.000000 proper-0.1.dev4/proper/middleware/redirect.py
--rw-r--r--   0 jps        (501) staff       (20)     1817 2021-03-25 03:03:48.000000 proper-0.1.dev4/proper/middleware/session.py
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.349680 proper-0.1.dev4/proper/parsers/
--rw-r--r--   0 jps        (501) staff       (20)      202 2020-11-26 02:31:37.000000 proper-0.1.dev4/proper/parsers/__init__.py
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.355022 proper-0.1.dev4/proper/parsers/__pycache__/
--rw-r--r--   0 jps        (501) staff       (20)      287 2021-09-04 02:03:27.000000 proper-0.1.dev4/proper/parsers/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)      445 2021-09-04 02:03:27.000000 proper-0.1.dev4/proper/parsers/__pycache__/parse_comma_separated.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)      599 2021-09-04 02:03:27.000000 proper-0.1.dev4/proper/parsers/__pycache__/parse_cookies.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     3277 2021-09-04 02:03:27.000000 proper-0.1.dev4/proper/parsers/__pycache__/parse_form_data.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)      488 2021-09-04 02:03:27.000000 proper-0.1.dev4/proper/parsers/__pycache__/parse_http_date.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     1471 2021-09-04 02:03:27.000000 proper-0.1.dev4/proper/parsers/__pycache__/parse_query_string.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)      237 2020-11-28 15:09:37.000000 proper-0.1.dev4/proper/parsers/parse_comma_separated.py
--rw-r--r--   0 jps        (501) staff       (20)      494 2020-08-14 21:45:00.000000 proper-0.1.dev4/proper/parsers/parse_cookies.py
--rw-r--r--   0 jps        (501) staff       (20)     3555 2021-03-25 03:04:33.000000 proper-0.1.dev4/proper/parsers/parse_form_data.py
--rw-r--r--   0 jps        (501) staff       (20)      334 2020-11-26 02:47:01.000000 proper-0.1.dev4/proper/parsers/parse_http_date.py
--rw-r--r--   0 jps        (501) staff       (20)     1236 2020-11-02 02:31:32.000000 proper-0.1.dev4/proper/parsers/parse_query_string.py
--rw-r--r--   0 jps        (501) staff       (20)    11475 2021-08-17 04:14:59.000000 proper-0.1.dev4/proper/request.py
--rw-r--r--   0 jps        (501) staff       (20)    11497 2021-07-29 04:24:53.000000 proper-0.1.dev4/proper/response.py
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.361341 proper-0.1.dev4/proper/router/
--rw-r--r--   0 jps        (501) staff       (20)      148 2021-07-28 21:49:27.000000 proper-0.1.dev4/proper/router/__init__.py
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.368606 proper-0.1.dev4/proper/router/__pycache__/
--rw-r--r--   0 jps        (501) staff       (20)      232 2021-09-04 02:03:27.000000 proper-0.1.dev4/proper/router/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     4834 2021-09-04 02:03:27.000000 proper-0.1.dev4/proper/router/__pycache__/base.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     3858 2021-09-04 02:03:27.000000 proper-0.1.dev4/proper/router/__pycache__/resource.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     5572 2021-09-04 03:36:28.000000 proper-0.1.dev4/proper/router/__pycache__/route.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     3552 2021-09-04 02:03:27.000000 proper-0.1.dev4/proper/router/__pycache__/router.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     2889 2021-09-04 02:03:27.000000 proper-0.1.dev4/proper/router/__pycache__/scope.cpython-39.pyc
--rw-r--r--   0 jps        (501) staff       (20)     4393 2021-07-28 22:19:32.000000 proper-0.1.dev4/proper/router/base.py
--rw-r--r--   0 jps        (501) staff       (20)     3787 2021-07-29 02:17:47.000000 proper-0.1.dev4/proper/router/resource.py
--rw-r--r--   0 jps        (501) staff       (20)     4599 2021-09-04 03:36:01.000000 proper-0.1.dev4/proper/router/route.py
--rw-r--r--   0 jps        (501) staff       (20)     3317 2021-07-29 02:22:36.000000 proper-0.1.dev4/proper/router/router.py
--rw-r--r--   0 jps        (501) staff       (20)     2440 2021-07-29 02:19:28.000000 proper-0.1.dev4/proper/router/scope.py
--rw-r--r--   0 jps        (501) staff       (20)     4128 2021-09-03 02:49:26.000000 proper-0.1.dev4/proper/static.py
--rw-r--r--   0 jps        (501) staff       (20)     4303 2020-11-14 19:23:24.000000 proper-0.1.dev4/proper/status.py
-drwxr-xr-x   0 jps        (501) staff       (20)        0 2021-09-10 20:41:21.252266 proper-0.1.dev4/proper.egg-info/
--rw-r--r--   0 jps        (501) staff       (20)     3179 2021-09-10 20:41:20.000000 proper-0.1.dev4/proper.egg-info/PKG-INFO
--rw-r--r--   0 jps        (501) staff       (20)    12213 2021-09-10 20:41:20.000000 proper-0.1.dev4/proper.egg-info/SOURCES.txt
--rw-r--r--   0 jps        (501) staff       (20)        1 2021-09-10 20:41:20.000000 proper-0.1.dev4/proper.egg-info/dependency_links.txt
--rw-r--r--   0 jps        (501) staff       (20)       43 2021-09-10 20:41:20.000000 proper-0.1.dev4/proper.egg-info/entry_points.txt
--rw-r--r--   0 jps        (501) staff       (20)      332 2021-09-10 20:41:20.000000 proper-0.1.dev4/proper.egg-info/requires.txt
--rw-r--r--   0 jps        (501) staff       (20)        7 2021-09-10 20:41:20.000000 proper-0.1.dev4/proper.egg-info/top_level.txt
--rw-r--r--   0 jps        (501) staff       (20)     1888 2021-09-10 20:41:21.371625 proper-0.1.dev4/setup.cfg
--rw-r--r--   0 jps        (501) staff       (20)       83 2021-01-09 15:46:42.000000 proper-0.1.dev4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.436938 proper-0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-09 20:45:37.000000 proper-0.2/MIT-LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-09 20:45:46.436938 proper-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-09 20:45:37.000000 proper-0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-05-09 20:45:37.000000 proper-0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 20:45:46.436938 proper-0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.400938 proper-0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.400938 proper-0.2/src/blueprints/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.404938 proper-0.2/src/blueprints/app/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.404938 proper-0.2/src/blueprints/app/[[ app_name ]]/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/app/[[ app_name ]]/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      141 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/app/[[ app_name ]]/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.404938 proper-0.2/src/blueprints/app/[[ app_name ]]/cl/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/app/[[ app_name ]]/cl/__init__.tt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.408938 proper-0.2/src/blueprints/app/[[ app_name ]]/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/app/[[ app_name ]]/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/app/[[ app_name ]]/config/app.tt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/app/[[ app_name ]]/config/database.tt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/app/[[ app_name ]]/config/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/app/[[ app_name ]]/config/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.408938 proper-0.2/src/blueprints/app/[[ app_name ]]/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/app/[[ app_name ]]/initializers/1_app.tt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/app/[[ app_name ]]/initializers/2_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/app/[[ app_name ]]/initializers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      554 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/app/[[ app_name ]]/initializers/error_handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.408938 proper-0.2/src/blueprints/app/[[ app_name ]]/mailers/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/app/[[ app_name ]]/mailers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/app/[[ app_name ]]/mailers/mailer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.408938 proper-0.2/src/blueprints/app/[[ app_name ]]/models/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      194 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/app/[[ app_name ]]/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/app/[[ app_name ]]/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.408938 proper-0.2/src/blueprints/app/[[ app_name ]]/models/concerns/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/app/[[ app_name ]]/models/concerns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/app/[[ app_name ]]/models/concerns/timestamped.tt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      805 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/app/[[ app_name ]]/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.408938 proper-0.2/src/blueprints/app/[[ app_name ]]/views/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      716 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/app/[[ app_name ]]/views/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      283 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/app/[[ app_name ]]/views/app.tt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.408938 proper-0.2/src/blueprints/app/[[ app_name ]]/views/concerns/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/app/[[ app_name ]]/views/concerns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/app/[[ app_name ]]/views/concerns/db_connection.tt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/app/[[ app_name ]]/views/concerns/security_headers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      243 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/app/[[ app_name ]]/views/page.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.408938 proper-0.2/src/blueprints/app/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/app/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/app/wsgi.tt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.408938 proper-0.2/src/blueprints/auth/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.408938 proper-0.2/src/blueprints/auth/[[ app_name ]]/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/auth/[[ app_name ]]/app.append.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.412938 proper-0.2/src/blueprints/auth/[[ app_name ]]/cl/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/auth/[[ app_name ]]/cl/__init__.append.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/auth/[[ app_name ]]/cl/auth.tt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.412938 proper-0.2/src/blueprints/auth/[[ app_name ]]/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/auth/[[ app_name ]]/config/app.append.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/auth/[[ app_name ]]/config/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.412938 proper-0.2/src/blueprints/auth/[[ app_name ]]/mailers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      714 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/auth/[[ app_name ]]/mailers/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.412938 proper-0.2/src/blueprints/auth/[[ app_name ]]/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/auth/[[ app_name ]]/models/__init__.append.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.412938 proper-0.2/src/blueprints/auth/[[ app_name ]]/models/concerns/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4145 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/auth/[[ app_name ]]/models/concerns/authenticable.tt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      229 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/auth/[[ app_name ]]/models/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.412938 proper-0.2/src/blueprints/auth/[[ app_name ]]/views/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/auth/[[ app_name ]]/views/app.append.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/auth/[[ app_name ]]/views/app.prepend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.412938 proper-0.2/src/blueprints/auth/[[ app_name ]]/views/concerns/
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/auth/[[ app_name ]]/views/concerns/load_user.tt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/auth/[[ app_name ]]/views/concerns/require_login.tt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.412938 proper-0.2/src/blueprints/auth/[[ app_name ]]/views/password/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/auth/[[ app_name ]]/views/password/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      813 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/auth/[[ app_name ]]/views/password/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/auth/[[ app_name ]]/views/password/pwned.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/auth/[[ app_name ]]/views/password/reset.tt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/auth/[[ app_name ]]/views/password/validators.tt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.412938 proper-0.2/src/blueprints/auth/[[ app_name ]]/views/session/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/auth/[[ app_name ]]/views/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/auth/[[ app_name ]]/views/session/forms.tt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/auth/[[ app_name ]]/views/session/session.tt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/auth/routes.tt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.400938 proper-0.2/src/blueprints/i18n/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.400938 proper-0.2/src/blueprints/i18n/[[ app_name ]]/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.412938 proper-0.2/src/blueprints/i18n/[[ app_name ]]/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/i18n/[[ app_name ]]/initializers/i18n.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.412938 proper-0.2/src/blueprints/i18n/[[ app_name ]]/views/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/i18n/[[ app_name ]]/views/app.prepend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.416938 proper-0.2/src/blueprints/i18n/[[ app_name ]]/views/concerns/
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/i18n/[[ app_name ]]/views/concerns/set_locale.tt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.400938 proper-0.2/src/blueprints/model/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.400938 proper-0.2/src/blueprints/model/[[ app_name ]]/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.416938 proper-0.2/src/blueprints/model/[[ app_name ]]/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/model/[[ app_name ]]/models/[[ singular_snake ]].tt.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/model/[[ app_name ]]/models/__init__.append.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.416938 proper-0.2/src/blueprints/resource/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.400938 proper-0.2/src/blueprints/resource/[[ app_name ]]/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.400938 proper-0.2/src/blueprints/resource/[[ app_name ]]/views/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.416938 proper-0.2/src/blueprints/resource/[[ app_name ]]/views/[[ view_snake ]]/
+-rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/resource/[[ app_name ]]/views/[[ view_snake ]]/[[ view_snake ]].tt.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/resource/[[ app_name ]]/views/[[ view_snake ]]/__init__.tt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/resource/[[ app_name ]]/views/[[ view_snake ]]/forms.tt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/resource/routes.tt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.416938 proper-0.2/src/blueprints/storage/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.400938 proper-0.2/src/blueprints/storage/[[ app_name ]]/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.416938 proper-0.2/src/blueprints/storage/[[ app_name ]]/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/storage/[[ app_name ]]/config/app.append.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/storage/[[ app_name ]]/config/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.416938 proper-0.2/src/blueprints/storage/[[ app_name ]]/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/storage/[[ app_name ]]/models/__init__.append.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/storage/[[ app_name ]]/models/attachment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.416938 proper-0.2/src/blueprints/storage/[[ app_name ]]/views/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/storage/[[ app_name ]]/views/storage.tt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/storage/routes.tt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.416938 proper-0.2/src/blueprints/view/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.400938 proper-0.2/src/blueprints/view/[[ app_name ]]/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.416938 proper-0.2/src/blueprints/view/[[ app_name ]]/views/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/view/[[ app_name ]]/views/[[ plural_snake ]].tt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-09 20:45:37.000000 proper-0.2/src/blueprints/view/routes.tt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.420938 proper-0.2/src/proper/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-09 20:45:37.000000 proper-0.2/src/proper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.420938 proper-0.2/src/proper/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-09 20:45:37.000000 proper-0.2/src/proper/auth/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9773 2024-05-09 20:45:37.000000 proper-0.2/src/proper/auth/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-09 20:45:37.000000 proper-0.2/src/proper/auth/install.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.420938 proper-0.2/src/proper/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-09 20:45:37.000000 proper-0.2/src/proper/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-09 20:45:37.000000 proper-0.2/src/proper/cache/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-05-09 20:45:37.000000 proper-0.2/src/proper/cache/sqlite_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.420938 proper-0.2/src/proper/cl/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-09 20:45:37.000000 proper-0.2/src/proper/cl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-05-09 20:45:37.000000 proper-0.2/src/proper/cl/app_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-09 20:45:37.000000 proper-0.2/src/proper/cl/db_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-09 20:45:37.000000 proper-0.2/src/proper/cl/proper_cl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.420938 proper-0.2/src/proper/concerns/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-09 20:45:37.000000 proper-0.2/src/proper/concerns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-05-09 20:45:37.000000 proper-0.2/src/proper/concerns/request_forgery_protection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-09 20:45:37.000000 proper-0.2/src/proper/concerns/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-09 20:45:37.000000 proper-0.2/src/proper/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.424938 proper-0.2/src/proper/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-09 20:45:37.000000 proper-0.2/src/proper/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15261 2024-05-09 20:45:37.000000 proper-0.2/src/proper/core/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8552 2024-05-09 20:45:37.000000 proper-0.2/src/proper/core/app_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-09 20:45:37.000000 proper-0.2/src/proper/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-05-09 20:45:37.000000 proper-0.2/src/proper/core/error_handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.424938 proper-0.2/src/proper/core/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-09 20:45:37.000000 proper-0.2/src/proper/core/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-09 20:45:37.000000 proper-0.2/src/proper/core/pipeline/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-09 20:45:37.000000 proper-0.2/src/proper/core/pipeline/head.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-09 20:45:37.000000 proper-0.2/src/proper/core/pipeline/match.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-09 20:45:37.000000 proper-0.2/src/proper/core/pipeline/method_override.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-09 20:45:37.000000 proper-0.2/src/proper/core/pipeline/redirect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-09 20:45:37.000000 proper-0.2/src/proper/current.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14960 2024-05-09 20:45:37.000000 proper-0.2/src/proper/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.424938 proper-0.2/src/proper/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-09 20:45:37.000000 proper-0.2/src/proper/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-05-09 20:45:37.000000 proper-0.2/src/proper/generators/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-05-09 20:45:37.000000 proper-0.2/src/proper/generators/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6730 2024-05-09 20:45:37.000000 proper-0.2/src/proper/generators/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-09 20:45:37.000000 proper-0.2/src/proper/generators/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.428938 proper-0.2/src/proper/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-09 20:45:37.000000 proper-0.2/src/proper/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-09 20:45:37.000000 proper-0.2/src/proper/helpers/digestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-09 20:45:37.000000 proper-0.2/src/proper/helpers/dotdict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-09 20:45:37.000000 proper-0.2/src/proper/helpers/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-09 20:45:37.000000 proper-0.2/src/proper/helpers/jsonplus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-09 20:45:37.000000 proper-0.2/src/proper/helpers/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4881 2024-05-09 20:45:37.000000 proper-0.2/src/proper/helpers/multidict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-09 20:45:37.000000 proper-0.2/src/proper/helpers/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10103 2024-05-09 20:45:37.000000 proper-0.2/src/proper/helpers/render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-09 20:45:37.000000 proper-0.2/src/proper/helpers/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8214 2024-05-09 20:45:37.000000 proper-0.2/src/proper/helpers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.428938 proper-0.2/src/proper/i18n/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-09 20:45:37.000000 proper-0.2/src/proper/i18n/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10031 2024-05-09 20:45:37.000000 proper-0.2/src/proper/i18n/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-09 20:45:37.000000 proper-0.2/src/proper/i18n/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42542 2024-05-09 20:45:37.000000 proper-0.2/src/proper/i18n/plural_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-09 20:45:37.000000 proper-0.2/src/proper/i18n/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:37.000000 proper-0.2/src/proper/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.428938 proper-0.2/src/proper/request/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-09 20:45:37.000000 proper-0.2/src/proper/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-05-09 20:45:37.000000 proper-0.2/src/proper/request/forwarded.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15818 2024-05-09 20:45:37.000000 proper-0.2/src/proper/request/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-09 20:45:37.000000 proper-0.2/src/proper/request/make_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13375 2024-05-09 20:45:37.000000 proper-0.2/src/proper/request/multipart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-05-09 20:45:37.000000 proper-0.2/src/proper/request/parse_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10245 2024-05-09 20:45:37.000000 proper-0.2/src/proper/request/request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.428938 proper-0.2/src/proper/response/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-09 20:45:37.000000 proper-0.2/src/proper/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-05-09 20:45:37.000000 proper-0.2/src/proper/response/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-09 20:45:37.000000 proper-0.2/src/proper/response/file_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-09 20:45:37.000000 proper-0.2/src/proper/response/flash_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19265 2024-05-09 20:45:37.000000 proper-0.2/src/proper/response/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9750 2024-05-09 20:45:37.000000 proper-0.2/src/proper/response/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.432938 proper-0.2/src/proper/router/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-09 20:45:37.000000 proper-0.2/src/proper/router/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-05-09 20:45:37.000000 proper-0.2/src/proper/router/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27011 2024-05-09 20:45:37.000000 proper-0.2/src/proper/router/route.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-05-09 20:45:37.000000 proper-0.2/src/proper/router/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-09 20:45:37.000000 proper-0.2/src/proper/router/scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-09 20:45:37.000000 proper-0.2/src/proper/router/static.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-05-09 20:45:37.000000 proper-0.2/src/proper/status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.432938 proper-0.2/src/proper/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-09 20:45:37.000000 proper-0.2/src/proper/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-09 20:45:37.000000 proper-0.2/src/proper/storage/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-09 20:45:37.000000 proper-0.2/src/proper/storage/install.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.432938 proper-0.2/src/proper/storage/services/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-09 20:45:37.000000 proper-0.2/src/proper/storage/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-09 20:45:37.000000 proper-0.2/src/proper/storage/services/disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-09 20:45:37.000000 proper-0.2/src/proper/storage/services/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-09 20:45:37.000000 proper-0.2/src/proper/storage/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-09 20:45:37.000000 proper-0.2/src/proper/storage/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-09 20:45:37.000000 proper-0.2/src/proper/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5564 2024-05-09 20:45:37.000000 proper-0.2/src/proper/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.432938 proper-0.2/src/proper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-09 20:45:46.000000 proper-0.2/src/proper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6482 2024-05-09 20:45:46.000000 proper-0.2/src/proper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 20:45:46.000000 proper-0.2/src/proper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-09 20:45:46.000000 proper-0.2/src/proper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-09 20:45:46.000000 proper-0.2/src/proper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-09 20:45:46.000000 proper-0.2/src/proper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:45:46.432938 proper-0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-05-09 20:45:38.000000 proper-0.2/tests/test_e2e_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-09 20:45:38.000000 proper-0.2/tests/test_e2e_hello.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-09 20:45:38.000000 proper-0.2/tests/test_e2e_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-09 20:45:38.000000 proper-0.2/tests/test_e2e_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-05-09 20:45:38.000000 proper-0.2/tests/test_e2e_router.py
```

### Comparing `proper-0.1.dev4/MIT-LICENSE` & `proper-0.2/MIT-LICENSE`

 * *Files identical despite different names*

### Comparing `proper-0.1.dev4/README.md` & `proper-0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Proper
 
 A web framework optimized for programmer happiness.
 
 
 ### Requirements
 
-- Python 3.6+
+- Python 3.10+
 
 
 ### Installation
 
 	pip install proper
 
 
@@ -37,19 +37,14 @@
 - Regular WSGI is great.
 
 
 # Sources of inspirations
 
 ## From Elixir/Phoenix
 
-### Pipelines in the routes.
-
-You don't need to have a framework for APIs and other for full-fletched apps, you can just deactivate cookie sessions, flash messages and other things yoi don't need for specific sections of your sites.
-And is super easy to add things too like admin-only sections just by composing multiple pipelines, after all, there are just lists of callables.
-
 ### App-code over framework-code.
 
 You can make it clean and straightforward or you can make it configurable.
 But if you put the code in the application, thanks to a standarized project skeleton,
 you can have both!
 
 
@@ -57,12 +52,15 @@
 
 ### Convention over configuration.
 
 ### Optimize for developer happiness.
 
 ### The application code must be beatiful.
 
-- Empty class-based controllers that works!
-- Class-based controllers allows several tricks that make the experience much better:
+- Empty class-based views that works!
+- Class-based views allows several tricks that make the experience much better:
 	- A configurable and plugganle render and view functions.
 	- Class based views a-la Django, but simpler and completely obvious because is your application code (see (App-code over framework-code)
-	- Saving context varaibles in your controller instance looks much cleaner that building a dictionary and manually calling render and the end of each controller.
+	- Saving context varaibles in your view instance looks much cleaner that building a dictionary and manually calling render and the end of each view.
+
+
+![Visualization of the codebase](./diagram.svg)
```

### Comparing `proper-0.1.dev4/blueprints/project/[[ app_name ]]/controllers/auth.py` & `proper-0.2/src/blueprints/auth/[[ app_name ]]/views/password/reset.tt.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,85 +1,61 @@
-from ..app import app
-from ..mailers import send_password_reset_email
-from ..models import User
-from ..services import auth_services
+from proper.status import unprocessable
 
-from .application import ApplicationController, REDIRECT_AFTER_LOGIN_KEY
-from .forms.auth import PasswordChangeForm, PasswordResetForm, SignInForm
+from [[ app_name ]].app import config
+from [[ app_name ]].mailers import send_password_reset_email
+from [[ app_name ]].models import User
 
+from ..app import AppView
+from ..concerns.require_login import REDIRECT_AFTER_LOGIN_KEY
+from .forms import PasswordResetModel, PasswordChangeModel
 
-class Auth(ApplicationController):
 
-    def sign_in(self):
-        if self.req.user:
-            return go_forward(self.resp)
+class PasswordReset(AppView):
+    def new(self):
+        self.form = PasswordResetModel.as_form()
+        return self.render("PasswordReset.New")
 
-        self.form = form = SignInForm(self.req.form)
-        if not self.req.is_post or not form.validate():
-            return
+    def create(self):
+        self.form = PasswordResetModel.as_form(self.params)
+        if self.form.is_invalid:
+            return self.render("PasswordReset.New", status=unprocessable)
 
-        credentials = form.save()
-        user = auth_services.authenticate(User, **credentials)
-        if not user:
-            # msg = "We didn’t recognize that password."
-            msg = "Wrong username and/or password"
-            form.password.error = msg
-            return
-
-        auth_services.sign_in(user, req=self.req, resp=self.resp)
-        self.resp.flash("Welcome back!")
-        return go_forward(self.resp)
-
-    def sign_out(self):
-        if self.req.user:
-            auth_services.sign_out(self.req.user, req=self.req, resp=self.resp)
-        return self.resp.redirect_to("/")
-
-    def reset(self):
-        self.form = form = PasswordResetForm(self.req.form)
-        if not self.req.is_post:
-            return
-
-        if not form.validate():
-            return
-
-        login = form.save()["login"]
-        user = User.by_login(login)
+        login = self.form.save()["login"]
+        user = User.get_by_login(login)
         send_password_reset_email(user)
         self.email = user.email
-        self.resp.template = "auth/reset_sent"
+        return self.render("PasswordReset.Create")
 
-    def reset_validate(self, token):
-        user = auth_services.authenticate_timestamped_token(User, token)
+    def edit(self):
+        self.pk = self.params.get("pk")
+        user = User.authenticate_timestamped_token(self.pk)
         if not user:
-            self.resp.template = "auth/reset_invalid"
-            return
+            return self.render("PasswordReset.Invalid", status=unprocessable)
 
-        auth_services.sign_in(user, req=self.req, resp=self.resp)
-        self.resp.redirect_to(app.url_for("Auth.password_change"))
+        self.login = user.login
+        self.form = PasswordChangeModel.as_form()
+        self.password_minlen = config.AUTH_PASSWORD_MINLEN
+        return self.render("PasswordReset.Edit")
+
+    def update(self):
+        self.pk = self.params.get("pk")
+        user = User.authenticate_timestamped_token(self.pk)
+        if not user:
+            return self.render("PasswordReset.Invalid", status=unprocessable)
 
-    def password_change(self):
-        if not self.req.user:
-            return self.resp.redirect_to(app.url_for("Auth.sign_in"))
-
-        self.form = form = PasswordChangeForm(self.req.form)
-        self.password_minlen = app.config.auth_password_minlen
-
-        if not self.req.is_post:
-            return
-
-        if not form.validate():
-            return
-
-        new_password = form.save()["password"][0]
-        auth_services.set_new_password(
-            self.req.user,
-            new_password,
-            req=self.req,
-            resp=self._appresp,
-        )
-        go_forward(self.resp)
-
-
-def go_forward(resp):
-    next_url = resp.session.pop(REDIRECT_AFTER_LOGIN_KEY, None) or "/"
-    resp.redirect_to(next_url)
+        self.form = PasswordChangeModel.as_form(self.params)
+        if self.form.is_invalid:
+            self.login = user.login
+            self.password_minlen = config.AUTH_PASSWORD_MINLEN
+            return self.render("PasswordReset.Edit", status=unprocessable)
+
+        new_password = self.form.save()["password1"]
+        user.set_password(new_password)
+        user.save()
+        user.sign_in()
+        self._go_forward(flash="Password updated")
+
+    # Private
+
+    def _go_forward(self, flash=None):
+        next_url = self.response.session.pop(REDIRECT_AFTER_LOGIN_KEY, None) or "/"
+        self.response.redirect_to(next_url, flash=flash)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `proper-0.1.dev4/blueprints/project/[[ app_name ]]/controllers/forms/pwned.py` & `proper-0.2/src/blueprints/auth/[[ app_name ]]/views/password/pwned.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 API_URL = "https://api.pwnedpasswords.com/range/"
 HTTP_OK = 200
 
 
 def query_api(hprefix):
     url = f"{API_URL}{hprefix}"
     try:
-        req = urllib.request.urlopen(url, timeout=1)
+        resp = urllib.request.urlopen(url, timeout=1)
     except HTTPException:
         return []
-    if req.status != HTTP_OK:
+    if resp.status != HTTP_OK:
         return []
-    return req.read().decode("utf8").split("\r\n")
+    return resp.read().decode("utf8").split("\r\n")
 
 
 def get_pwned_count(passw):
     hash = sha1(passw.encode("utf8")).hexdigest().upper()
     hprefix = hash[:5]
     hsuffix = hash[5:]
     resp = query_api(hprefix)
```

### Comparing `proper-0.1.dev4/blueprints/project/[[ app_name ]]/mailers/auth.py` & `proper-0.2/src/blueprints/auth/[[ app_name ]]/mailers/auth.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from ..app import app, send_email
-from ..config import config
+from ..app import app, auth, config
+from .mailer import send_email
 
 
 __all__ = (
     "render_password_reset_email",
     "send_password_reset_email",
 )
 
 
 def render_password_reset_email(user):
-    token = user.get_timestamped_token()
-    validate_url = app.url_for("Auth.reset_validate", token=token)
-    reset_url = app.url_for("Auth.reset")
-    return app.render(
-        "emails/password_reset.html.jinja",
-        validate_url=f"{config.host}{validate_url}",
-        reset_url=f"{config.host}{reset_url}",
+    token = auth.get_timestamped_token(user)
+    validate_url = app.url_for("PasswordReset.edit", pk=token)
+    reset_url = app.url_for("PasswordReset.new")
+    return app.catalog.render(
+        "Emails.PasswordReset",
+        validate_url=f"{config.HOST}{validate_url}",
+        reset_url=f"{config.HOST}{reset_url}",
     )
 
 
 def send_password_reset_email(user):
     kw = {
         "to": user.email,
         "subject": "Reset your password",
```

### Comparing `proper-0.1.dev4/blueprints/project/manage.tmpl.py` & `proper-0.2/src/blueprints/auth/[[ app_name ]]/cl/auth.tt.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,57 @@
-#!/usr/bin/env python
-from pyceo import Cli
+from proper_cli import Cli
 
-from [[ app_name ]].main import app
-from [[ app_name ]].models import User, alembic, dbs
+from [[ app_name ]].app import app
 
 
-class AuthCli(Cli):
-    def user(self, login, password):
+class AuthCL(Cli):
+    def user(self, login: str, password: str) -> None:
         """
         Adds an user.
 
         Arguments:
-          - login:    Username
-          - password: Plain-text password (will be encrypted)
+
+        - login:
+            Username
+
+        - password:
+            Plain-text password (will be encrypted)
+
         """
-        dbs.create(User, login=login, password=password)
-        dbs.commit()
+        from [[ app_name ]].models.user import User
+
+        try:
+            User.create(login=login, password=password)
+        except Exception as e:
+            print("ERROR:", e)
+            return
         print("User added")
 
-    def password(self, login, password):
+    def password(self, login: str, password: str) -> None:
         """
-        Set the password of a user.
+        Set the password of a user
 
         Arguments:
-          - login:    Username
-          - password: Plain-text password (will be encrypted)
+
+        - login:
+            Username
+
+        - password:
+            Plain-text password (will be encrypted)
+
         """
-        user = User.by_login(login)
+        from [[ app_name ]].models.user import User
+
+        user = User.get_by_login(login)
         if not user:
-            print ("User not found")
+            print("User not found")
+            return
+        try:
+            user.set_password(password)
+            user.save()
+        except Exception as e:
+            print("ERROR:", e)
             return
-        user.password = password
-        dbs.commit()
         print("Password updated")
 
 
-app.cli.auth = AuthCli
-app.cli.db = alembic.get_pyceo_cli()
-
-
-if __name__ == "__main__":
-    app.cli()
+app.CL.auth = AuthCL
```

### Comparing `proper-0.1.dev4/proper/errors.py` & `proper-0.2/src/proper/errors.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,116 @@
+import typing as t
+
+import itsdangerous
+
 from . import status
 
 
+class BadSecretKey(Exception):
+    pass
+
+
+class MissingRouteParameter(Exception):
+    def __init__(self, name: str, path: str) -> None:
+        msg = f"missing value for {name} in {path}"
+        super().__init__(msg)
+
+
+class BadRoutePlaceholder(Exception):
+    def __init__(self, name: str, path: str, rx: str) -> None:
+        msg = f"placeholder {name} doesn't have the expected format <{rx}> in {path}"
+        super().__init__(msg)
+
+
+class DuplicatedRoutePlaceholder(Exception):
+    def __init__(self, name: str, path: str) -> None:
+        msg = f"placeholder {name} declared more than once in {path}"
+        super().__init__(msg)
+
+
+class BadRouteFormat(Exception):
+    pass
+
+
+class RouteNotFound(Exception):
+    pass
+
+
+class WrongHashAlgorithm(Exception):
+    pass
+
+
+class BadSignature(itsdangerous.BadSignature):
+    def __init__(self, message: str = "Bad signtaure", payload: t.Any = None):
+        super().__init__(message, payload)
+
+
+class TranslationsNotFound(Exception):
+    def __init__(self, locale: str) -> None:
+        if "_" in locale:
+            lang = locale.split("_")[0]
+            msg = f"No translations found for the '{locale}' or '{lang}' locales"
+        else:
+            msg = f"No translations found for the '{locale}' locale"
+        super().__init__(msg)
+
+
 class HTTPError(Exception):
     """A generic HTTP error.
 
     Arguments are:
 
-        msg (str):
-            Description of the error.
+    - msg (str):
+        Description of the error.
 
-        status (str):
-            HTTP status line, e.g. '200 OK' or '725 It works on my machine'.
+    - status (str):
+        HTTP status line, e.g. '200 OK' or '725 It works on my machine'.
 
-        **headers (dict):
-            Optional headers to attach to the response
+    - **headers (dict):
+        Optional headers to attach to the response
 
     """
 
-    __slots__ = ("msg", "status_code", "headers")
+    __slots__ = ("msg", "status", "headers")
 
-    def __init__(self, msg="", status_code=None, **headers):
+    def __init__(
+        self,
+        msg: str = "",
+        status: str = "500 Error",
+        **headers: list[str],
+    ):
         self.msg = msg
-        self.status_code = getattr(self, "status_code", status_code)
+        self.status = getattr(self, "status", status)
         self.headers = headers
 
     def __str__(self):
         return self.msg
 
     def __repr__(self):
         return f'{self.__class__.__name__}("{self.msg}")'
 
+    @property
+    def status_code(self) -> int:
+        return int(self.status.split(" ", 1)[0])
+
+    @property
+    def description(self) -> str:
+        return self.__doc__ or ""
+
 
 class BadRequest(HTTPError):
     """400 Bad Request.
 
     The server cannot or will not process the request due to something
     that is perceived to be a client error (e.g., malformed request
     syntax, invalid request message framing, or deceptive request
     routing).
     """
 
-    status_code = status.bad_request
+    status = status.bad_request
 
 
 class InvalidHeader(BadRequest):
     """400 Bad Request.
 
     One of the headers in the request is invalid.
     """
@@ -53,21 +119,42 @@
 class ClientDisconnected(BadRequest):
     """400 Bad Request.
 
     The request was interrupted.
     """
 
 
+class MultipartError(BadRequest):
+    """400 Bad Request.
+
+    The form data cannot be parsed..
+    """
+
+
 class MissingHeader(BadRequest):
     """400 Bad Request.
 
     One of the headers in the request is missing.
     """
 
 
+class BadRequestKeyError(BadRequest, KeyError):
+    """An exception that is used to signal both a KeyError and a
+    BadRequest.
+    """
+
+    def __init__(self, key: str | None = None, *args: t.Any, **kwargs: t.Any):
+        super().__init__(*args, **kwargs)
+
+        if key is None:
+            KeyError.__init__(self)
+        else:
+            KeyError.__init__(self, key)
+
+
 class Unauthorized(HTTPError):
     """401 Unauthorized.
 
     The request has not been applied because it lacks valid
     authentication credentials for the target resource.
 
     The server generating a 401 response MUST send a WWW-Authenticate
@@ -80,15 +167,15 @@
     replaced Authorization header field. If the 401 response contains
     the same challenge as the prior response, and the user agent has
     already attempted authentication at least once, then the user agent
     SHOULD present the enclosed representation to the user, since it
     usually contains relevant diagnostic information.
     """
 
-    status_code = status.unauthorized
+    status = status.unauthorized
 
 
 class Forbidden(HTTPError):
     """403 Forbidden.
 
     The server understood the request but refuses to authorize it.
     A server that wishes to make public why the request has been
@@ -101,15 +188,15 @@
     credentials. However, a request might be forbidden for reasons
     unrelated to the credentials.
 
     An server that wishes to hide the existence of a forbidden target
     resource MAY instead respond with a status code of '404 Not Found'.
     """
 
-    status_code = status.forbidden
+    status = status.forbidden
 
 
 class MissingCSRFToken(Forbidden):
     """403 Forbidden.
 
     We couldn't find a CSRF token in the request.
     """
@@ -130,15 +217,15 @@
 
     A 404 status code does not indicate whether this lack of
     representation is temporary or permanent; the 410 Gone status code
     is preferred over 404 if the origin server knows that the condition
     is likely to be permanent.
     """
 
-    status_code = status.not_found
+    status = status.not_found
 
 
 class MatchNotFound(NotFound):
     """404 Not Found.
 
     We couldn't found a matching route for the requested URL.
 
@@ -154,31 +241,31 @@
     server but not supported by the target resource.
 
     The origin server MUST generate an Allow header field in a 405
     response containing a list of the target resource's currently
     supported methods.
     """
 
-    status_code = status.method_not_allowed
+    status = status.method_not_allowed
 
     def __init__(self, msg, allowed, **headers):
         headers.setdefault("Allow", ", ".join(allowed))
-        super().__init__(msg, status_code=self.status_code, **headers)
+        super().__init__(msg, status=self.status, **headers)
 
 
 class NotAcceptable(HTTPError):
     """406 Not Acceptable.
 
     The target resource does not have a current representation that
     would be acceptable to the user agent, according to the proactive
     negotiation header fields received in the request, and the server
     is unwilling to supply a default representation.
     """
 
-    status_code = status.not_acceptable
+    status = status.not_acceptable
 
 
 class Conflict(HTTPError):
     """409 Conflict.
 
     The request could not be completed due to a conflict with the
     current state of the target resource. This code is used in
@@ -193,15 +280,15 @@
     PUT included changes to a resource that conflict with those made by
     an earlier (third-party) request, the origin server might use a 409
     response to indicate that it can't complete the request. In this
     case, the response representation would likely contain information
     useful for merging the differences based on the revision history.
     """
 
-    status_code = status.conflict
+    status = status.conflict
 
 
 class Gone(HTTPError):
     """410 Gone.
 
     The target resource is no longer available at the origin server and
     this condition is likely to be permanent.
@@ -212,102 +299,125 @@
 
     The 410 response is primarily intended to assist the task of web
     maintenance by notifying the recipient that the resource is
     intentionally unavailable and that the server owners desire that
     remote links to that resource be removed.
     """
 
-    status_code = status.gone
+    status = status.gone
 
 
 class LengthRequired(HTTPError):
     """411 Length Required.
 
     The server refuses to accept the request without a defined Content-
     Length.
     """
 
-    status_code = status.length_required
+    status = status.length_required
 
 
 class PreconditionFailed(HTTPError):
     """412 Precondition Failed.
 
     One or more conditions given in the request header fields evaluated
     to false when tested on the server.
 
     This response code allows the client to place preconditions on the
     current resource state (its current representations and metadata)
     and, thus, prevent the request method from being applied if the
     target resource is in an unexpected state.
     """
 
-    status_code = status.precondition_failed
+    status = status.precondition_failed
 
 
 class RequestEntityTooLarge(HTTPError):
     """413 Request Entity Too Large.
 
     The server is refusing to process a request because the request
     payload is larger than the server is willing or able to process.
     """
 
-    status_code = status.request_entity_too_large
+    status = status.request_entity_too_large
 
 
 class UriTooLong(HTTPError):
     """414 URI Too Long.
 
     The server is refusing to service the request because the request-
     target is longer than the server is willing to interpret.
 
     This rare condition is only likely to occur from a client error
     or an attack attempt by a client.
     """
 
-    status_code = status.request_uri_too_long
+    status = status.request_uri_too_long
 
 
 class UnsupportedMediaType(HTTPError):
     """415 Unsupported Media Type.
 
     The origin server is refusing to service the request because the
     payload is in a format not supported by this method on the target
     resource.
 
     The format problem might be due to the request's indicated Content-
     Type or Content-Encoding, or as a result of inspecting the data
     directly.
     """
 
-    status_code = status.unsupported_media_type
+    status = status.unsupported_media_type
+
+
+class RangeNotSatisfiable(HTTPError):
+    """416 Range Not Satisfiable.
+
+    The server cannot serve the requested ranges. The most likely reason is
+    that the document doesn't contain such ranges, or that the Range header
+    value, though syntactically correct, doesn't make sense.
+
+    The format problem might be due to the request's indicated Content-
+    Type or Content-Encoding, or as a result of inspecting the data
+    directly.
+
+    The 416 response message contains a Content-Range with
+    the current length of the resource, that you need to provide
+    to raise thie exception.
+    """
+
+    status = status.range_not_satisfiable
+
+    def __init__(self, msg, length: int | str = "*", **headers):
+        headers.setdefault("Content-Range", f"bytes */{length}")
+        super().__init__(msg, status=self.status, **headers)
 
 
 class UnprocessableEntity(HTTPError):
     """422 Unprocessable Entity.
 
     The server understands the content type of the request entity (hence
     a 415 Unsupported Media Type status code is inappropriate), and the
     syntax of the request entity is correct (thus a 400 Bad Request
     status code is inappropriate) but was unable to process the
     contained instructions.
     """
 
-    status_code = status.unprocessable_entity
+    status = status.unprocessable_entity
 
 
 class FailedDependency(HTTPError):
     """424 Failed Dependency.
 
     The 424 (Failed Dependency) status code means that the method could
     not be performed on the resource because the requested action
     depended on another action and that action failed.
     """
 
-    status_code = status.failed_dependency
+    status = status.failed_dependency
 
 
 class PreconditionRequired(HTTPError):
     """428 Precondition Required.
 
     The 428 status code indicates that the origin server requires the
     request to be conditional.
@@ -315,53 +425,53 @@
     Its typical use is to avoid the 'lost update' problem, where a client
     GETs a resource's state, modifies it, and PUTs it back to the server,
     when meanwhile a third party has modified the state on the server,
     leading to a conflict.  By requiring requests to be conditional, the
     server can assure that clients are working with the correct copies.
     """
 
-    status_code = status.precondition_required
+    status = status.precondition_required
 
 
 class TooManyRequests(HTTPError):
     """429 Too Many Requests.
 
     The user has sent too many requests in a given amount of time ('rate
     limiting').
     The response representations SHOULD include details explaining the
     condition, and MAY include a Retry-After header indicating how long
     to wait before making a new request.
     """
 
-    status_code = status.too_many_requests
+    status = status.too_many_requests
 
 
 class UnavailableForLegalReasons(HTTPError):
     """451 Unavailable For Legal Reasons.
 
     The server is denying access to the resource as a consequence of a
     legal demand.
 
     Responses using this status code SHOULD include an explanation, in
     the response body, of the details of the legal demand: the party
     making it, the applicable legislation or regulation, and what
     classes of person and resource it applies to.
     """
 
-    status_code = status.unavailable_for_legal_reasons
+    status = status.unavailable_for_legal_reasons
 
 
 class InternalServerError(HTTPError):
     """500 Internal Server Error.
 
     The server encountered an unexpected condition that prevented it
     from fulfilling the request.
     """
 
-    status_code = status.internal_server_error
+    status = status.internal_server_error
 
 
 ServerError = InternalServerError
 Error = InternalServerError
 
 
 class NotImplemented(HTTPError):
@@ -369,33 +479,33 @@
 
     The 501 (Not Implemented) status code indicates that the server does
     not support the functionality required to fulfill the request.  This
     is the appropriate response when the server does not recognize the
     request method and is not capable of supporting it for any resource.
     """
 
-    status_code = status.not_implemented
+    status = status.not_implemented
 
 
 class InsufficientStorage(HTTPError):
     """507 Insufficient Storage.
 
     The 507 (Insufficient Storage) status code means the method could not
     be performed on the resource because the server is unable to store
     the representation needed to successfully complete the request. This
     condition is considered to be temporary. If the request that
     received this status code was the result of a user action, the
     request MUST NOT be repeated until it is requested by a separate user
     action.
     """
 
-    status_code = status.insufficient_storage
+    status = status.insufficient_storage
 
 
 class NetworkAuthenticationRequired(HTTPError):
     """511 Network Authentication Required.
 
     The 511 status code indicates that the client needs to authenticate
     to gain network access.
     """
 
-    status_code = status.network_authentication_required
+    status = status.network_authentication_required
```

### Comparing `proper-0.1.dev4/proper/generators/controller.py` & `proper-0.2/src/proper/generators/view.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,68 @@
 from pathlib import Path
+from typing import TYPE_CHECKING
 
 import inflection
 
-from proper.helpers.render import BLUEPRINTS, BlueprintRender, append_routes
+from ..helpers.render import BLUEPRINTS, BlueprintRender, append_routes, save_file
 
 
-CONTROLLER_BLUEPRINT = BLUEPRINTS / "controller"
-ROUTES_TMPL = "routes.tmpl.py"
-TEMPLATE_TMPL = "template.tmpl.html.jinja"
+if TYPE_CHECKING:
+    from proper import App
 
 
-def gen_controller(app, class_name, *actions):
-    """Stubs out a new controller and its templates.
+VIEW_BLUEPRINT = BLUEPRINTS / "view"
+COMPONENT_TT = "component.jinja"
+ROUTES_TT = "routes.tt.py"
 
-        ./manage.py g controller NAME [action ...]
+
+def gen_view(app: "App", name: str, *actions: str) -> None:
+    """Stubs out a new view and its components.
+
+        proper g view NAME [action ...]
 
     Arguments:
 
-    - class_name: The PascalCased controller class name (in plural).
-    - actions: Optional list of actions.
+    - name:
+        The PascalCased view class name, in plural.
+
+    - actions:
+        Optional list of actions.
 
     Example:
 
-        ./manage.py g controller Articles index show
+        proper g view Articles index show
 
     """
-    class_name = inflection.camelize(inflection.pluralize(class_name))
-    snake_name = inflection.underscore(class_name)
-    actions = [inflection.underscore(action) for action in actions] or ["index"]
+    plural_name = inflection.pluralize(name)
+    plural_pascal = inflection.camelize(plural_name)
+    plural_snake = inflection.underscore(plural_name)
+    actions = tuple([inflection.underscore(action) for action in actions] or ["index"])
+    root_path = Path(app.root_path.parent)
 
     bp = BlueprintRender(
-        CONTROLLER_BLUEPRINT,
-        app.root_path.parent,
+        VIEW_BLUEPRINT,
+        root_path,
         context={
             "app_name": app.root_path.name,
-            "class_name": class_name,
-            "snake_name": snake_name,
+            "plural_pascal": plural_pascal,
+            "plural_snake": plural_snake,
+            "snake_name": plural_snake,
             "actions": actions,
         },
-        ignore=[ROUTES_TMPL, TEMPLATE_TMPL]
+        ignore=[ROUTES_TT, COMPONENT_TT],
     )
     bp()
 
-    template_tmpl = CONTROLLER_BLUEPRINT / TEMPLATE_TMPL
-    content = bp.render.string(template_tmpl.read_text())
-
-    (app.root_path / "templates" / snake_name).mkdir(parents=False, exist_ok=True)
-    folder = Path(app.root_path.name) / "templates" / snake_name
+    component_tt = VIEW_BLUEPRINT / COMPONENT_TT
+    content = component_tt.read_text()
     for action in actions:
-        dst_relpath = folder / f"{action}.html.jinja"
-        bp.save_file(content, dst_relpath)
+        action_pascal = inflection.camelize(action)
+        save_file(
+            root_path,
+            f"{app.root_path.name}/components/{plural_pascal}/{action_pascal}.jinja",
+            content
+        )
 
-    routes_tmpl = CONTROLLER_BLUEPRINT / ROUTES_TMPL
-    new_routes = bp.render.string(routes_tmpl.read_text())
+    routes_tt = VIEW_BLUEPRINT / ROUTES_TT
+    new_routes = bp.render.string(routes_tt.read_text())
     append_routes(app, new_routes)
```

### Comparing `proper-0.1.dev4/proper/helpers/digestor.py` & `proper-0.2/src/proper/helpers/digestor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import shutil
 from hashlib import md5
+from pathlib import Path
+from typing import Dict
 
 
-__all__ = ("Digestor", )
+__all__ = ("Digestor",)
 
 
 class Digestor:
-    def __init__(self, root, *, length=12):
+    def __init__(self, root: "Path", *, length: int = 12) -> None:
         self.root = root
         self.length = length
-        self.manifest = {}
+        self.manifest: Dict[str, str] = {}
 
-    def digest(self, path):
+    def digest(self, path: "Path") -> str:
         hash = self.get_hash(path)
         new_path = path.with_suffix(f".{hash}{path.suffix}")
         shutil.copyfile(path, new_path)
         rel_path = str(path.relative_to(self.root))
         rel_new_path = str(new_path.relative_to(self.root))
         self.manifest[rel_path] = rel_new_path
         return rel_new_path
 
-    def get_hash(self, path):
+    def get_hash(self, path: "Path") -> str:
         md5_hash = md5()
         with open(path, "rb") as f:
             for byte_block in iter(lambda: f.read(4096), b""):
                 md5_hash.update(byte_block)
-        return md5_hash.hexdigest()[:self.length]
+        return md5_hash.hexdigest()[: self.length]
```

### Comparing `proper-0.1.dev4/proper/helpers/dot.py` & `proper-0.2/src/proper/helpers/dotdict.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,98 +1,70 @@
 import copy
+import typing as t
 
 
-__all__ = ("Dot", )
+__all__ = ("DotDict",)
 
 
-class Dot(dict):
+class DotDict(dict):
     """A dict that:
 
     1. Allows `obj.foo` in addition to `obj['foo']` and
        `obj.foo.bar` in addition to `obj['foo']['bar']`.
     2. Can normalize keys with the optional methods `_key_encode`.
     3. Improved `update()` method for deep updating and key normalization.
+    """
 
-    Examples:
+    def __init__(
+        self,
+        *args,
+        **kwargs
+    ) -> None:
+        super().__init__()
+        self.update(*args, **kwargs)
 
-    >>> d = Dot({'a': 1, 'b': 2, 'foo': {'b': {'a': 'r'}} })
-    >>> d.a
-    1
-    >>> d.foo
-    {'b': {'a': 'r'}}
-    >>> d.foo.b.a
-    'r'
+    def __setattr__(self, name: str, value: t.Any) -> None:
+        if name.startswith("__"):
+            return super().__setattr__(name, value)
 
-    """
+        return self.__setitem__(name, value)
 
-    def __init__(self, dict_or_iter=None, **kwargs):
-        super().__init__()
-        self.update(dict_or_iter, **kwargs)
+    def __getattr__(self, name: str) -> t.Any:
+        if name.startswith("__"):
+            return super().__getattribute__(name)
 
-    def _key_encode(self, key):
-        return key
+        return self.__getitem__(name)
 
-    def __setattr__(self, key, value):
-        if key.startswith("_"):
-            return super().__setattr__(key, value)
-        raise AttributeError(
-            """Use the obj[key] = value notation to set or update values."""
-        )
-
-    def __getattr__(self, key):
-        return self.__getitem__(key)
-
-    def __getitem__(self, key):
-        key = self._key_encode(key)
-        value = super().__getitem__(key)
+    def __setitem__(self, key: object, value: t.Any) -> None:
         if isinstance(value, dict):
-            return self.__class__(value)
-        return value
-
-    def __setitem__(self, key, value):
-        key = self._key_encode(key)
+            value = self.__class__(value)
         super().__setitem__(key, value)
 
-    def __delitem__(self, key):
-        key = self._key_encode(key)
-        super().__delitem__(key)
-
-    def __contains__(self, key):
-        return self._key_encode(key) in super().keys()
-
-    def keys(self):
-        return (self._key_encode(key) for key in super().keys())
-
-    def setdefault(self, key, default=None):
-        key = self._key_encode(key)
-        return super().setdefault(key, default)
-
-    def get(self, key, default=None):
-        key = self._key_encode(key)
-        value = super().get(key, default)
-        if isinstance(value, dict):
-            return self.__class__(value)
-        return value
+    def copy(self) -> "DotDict":
+        return self.__class__(super().copy())
 
-    def update(self, src=None, **kwargs):
-        if src is None:
-            return
-        if not hasattr(src, "items"):
-            src = dict(src)
-        self._deepupdate(self, src)
+    def update(self, *args, **kwargs) -> None:  # type: ignore
+        if args:
+            self._update(src=dict(*args), target=self)
+        if kwargs:
+            self._update(src=kwargs, target=self)
 
-    def _deepupdate(self, target, src):
+    def _update(self, src: dict, target: dict) -> None:
         """Deep update target dict with src.
 
         For each k,v in src: if k doesn't exist in target, it is deep copied from
         src to target. Otherwise, if v is a dict, recursively deep-update it.
 
         """
+        if not src:
+            return
         for key, value in src.items():
-            key = self._key_encode(key)
-            if isinstance(value, dict):
-                if key not in target:
-                    dict.__setitem__(target, key, copy.deepcopy(value))
+            if key not in target:
+                if isinstance(value, dict):
+                    target[key] = copy.deepcopy(value)
                 else:
-                    self._deepupdate(dict.__getitem__(target, key), value)
+                    target[key] = copy.copy(value)
             else:
-                dict.__setitem__(target, key, copy.copy(value))
+                if isinstance(target[key], dict) and isinstance(value, dict):
+                    self._update(src=value, target=target[key])
+                else:
+                    target[key] = copy.copy(value)
```

### Comparing `proper-0.1.dev4/proper/request.py` & `proper-0.2/src/proper/request/request.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,384 +1,333 @@
-"""
-Request class.
-"""
-from datetime import datetime
-from typing import Any, Dict, List, Optional, Tuple, Union
+import typing as t
+from io import BytesIO
+
+import itsdangerous
 
-from . import errors
-from .constants import DELETE, FLASHES_SESSION_KEY, GET, HEAD, PATCH, POST, PUT
-from .helpers import HeadersDict, MultiDict, tunnel_decode, tunnel_encode
-from .parsers import (
-    parse_comma_separated,
-    parse_cookies,
-    parse_form_data,
-    parse_http_date,
-    parse_query_string,
-)
-from .router import Route
+from proper import current
+from proper.constants import FLASHES_SESSION_KEY, GET, HEAD
+from proper.errors import BadSignature
+from proper.helpers import DotDict, MultiDict, Undefined, split_locale
+from proper.router import Route
 
+from .headers import RequestHeadersMixin
+from .make_env import make_test_env
+from .parse_form import parse_form, parse_query_string
 
-__all__ = ("Request", "make_test_environ")
 
-DEFAULT_HTTP_PORT = 80
-DEFAULT_HTTPS_PORT = 443
+__all__ = ("Request", )
 
 
-class Request:
+class Request(RequestHeadersMixin):
     """An HTTP request.
 
-    Arguments are:
+    Arguments:
 
-    encoding:
-        Default encoding.
+        encoding:
+            Default encoding.
 
-    config:
-        Extra options
+        max_content_length:
+            Maximum content length in bytes.
 
-    **environ:
-        A WSGI environment dict passed in from the server (See also PEP-3333).
+        max_query_size:
+            Maximum query string size in bytes.
 
+        **env:
+            A WSGI environment dict passed in from the server (See also PEP-3333).
 
     Attributes:
 
-    environ:
-        The WSGI environment dict passed in from the server.
+        env:
+            The WSGI environment dict passed in from the server,
+        with keys normalized to lower-case
 
-    scheme:
-        The request scheme as an string (either "http" or "https").
+        locale:
+            Set in the `SetLocale` concern
 
-    host:
-        The requested host.
+        language:
+            Just the language part of the locale. So `en_US` -> `en`.
 
-    host_with_port:
-        A host:port string for this request. The port is not included
-        if its the default for the scheme.
+        body:
+            The request body as a bytes stream.
 
-    method:
-        The uppercased request method, example: "GET".
+        accept:
+            Indicates which content types, expressed as MIME types,
+        the client is able to understand.
 
-    path:
-        Requested path without the leading or trailing slash.
+        accept_encoding:
+            Indicates the content encoding (usually a compression algorithm) that
+        the client can understand.
 
-    query:
-        Parsed args from the URL.
+        accept_language:
+            Indicates the natural language and locale that the client prefers.
 
-    form:
-        A :class:`MultiDict` object containing the parsed body data, like the
-        one sent by a HTML form with a POST, **including** the files.
+        content_length:
+            The length in bytes, as an integer, of the content
+            sent by the client.
 
-    remote_addr:
-        IP address of the closest client or proxy to the WSGI server.
+        content_type:
+            The MIME content type of the incoming request.
 
-        If your application is behind one or more reverse proxies,
-        and it doesn't pass forward the IP address of the client,
-        you can use the `access_route` attribute to retrieve the real
-        IP address of the client.
-
-    root_path:
-        The root path of the script (SCRIPT_NAME).
-        Note: The router does **NOT** uses this value for `url_for()`, but the
-        one from `app.config.root_path`.
-        A :class:`MultiDict` object containing the query string data.
-
-    cookies:
-        All cookies transmitted with the request.
-
-    xhr:
-        True if current request is an XHR request.
-
-    secure:
-        Whether the current request was made via a SSL connection.
-
-    content_type:
-        The MIME content type of the incoming request.
-
-    content_length:
-        The length in bytes, as an integer, of the content sent by the client.
-
-    stream:
-        Returns the contents of the incoming HTTP entity body.
-
-    flashes:
-        The flashed messages stored in the session cookie.
-        By reading this value it will be stored in the request but
-        deleted form the session.
-
-    if_none_match:
-        Value of the If-None-Match header, as a parsed list of strings,
-        or an empty list if the header is missing or its value is blank.
-
-    if_modified_since:
-        Value of the If-Modified-Since header, or an empty string if the header
-        is missing or the date cannot be parsed.
+        cookies:
+            A dict with the cookies sent with the request.
 
-    """
+        date:
+            The date and time at which the message originated.
 
-    encoding: str
-    config: Dict[str, Any]
-    environ: Dict[str, Any]
-    method: str
-    real_method: str
-    path: str
-    content_type: str
-    scheme: str
-    host: str
-    port: int
-
-    matched_route: Optional[Route]
-    matched_params: Optional[Dict[str, Any]]
-    user: Optional[Any]
-    csrf_token: Optional[str]
+        default_port:
+            Returns the default port (80 for HTTP, 443 for HTTPS)
 
-    _session: Dict[str, Any]
+        encoding:
+            From the arguments.
 
-    def __init__(
-        self,
-        *,
-        encoding: str = "utf8",
-        config: Optional[Dict[str, Any]] = None,
-        **environ,
-    ) -> None:
-        self.encoding = encoding
-        self.config = config or {}
-        environ = environ or make_test_environ()
-        self.environ = environ
+        flashes:
+            The flashed messages stored in the session cookie.
+            By reading this value it will be stored in the request but
+            deleted form the session.
 
-        self.method = environ.get("REQUEST_METHOD", "GET").upper()
-        self.real_method = self.method
+        form:
+            A `MultiDict` object containing the parsed body data, like the
+            one sent by a HTML form with a POST, **including** the files.
 
-        # PATH_INFO is always "bytes tunneled as latin-1" and must be decoded back.
-        # Read the docstring on `support/encoding.py` for more details.
-        self.path = "/" + tunnel_decode(environ.get("PATH_INFO", "").strip("/"))
+        format:
+            Computed based on the value of the "Accept" header, with "html"
+        as a fallback.
 
-        self.content_type = self.environ.get("CONTENT_TYPE", "")
+        forwarded:
+            A comma-separated list of forwarding information from the client
+            to the server on its way through proxies.
 
-        self.scheme = self.environ.get("HTTP_X_FORWARDED_PROTO") or self.environ.get(
-            "wsgi.url_scheme"
-        )
-        self.host, self.port = self._parse_host(self.environ.get("HTTP_HOST"))
+        host, protocol, port, path, and query_string:
+            Components of the URL used for the request, based on the pattern:
+            `protocol://host:port/path?query_string`.
 
-        self.matched_route = None
-        self.matched_params = None
-        self.user = None
-        self.csrf_token = None
-        self._session = {}
-
-        self._content_length = None
-        self._cookies = None
-        self._form = None
-        self._headers = None
-        self._query = None
-        self._remote_addr = None
-        self._if_none_match = None
-        self._if_modified_since = None
+        host_with_port:
+            A host:port string for this request. The port is not included
+            if its the default for the protocol.
 
-    def __repr__(self) -> str:
-        return f"<Request {self.method} “{self.path}”>"
+        if_none_match:
+            A list of ETags provided by the client.
 
-    def _parse_host(self, host: str) -> Tuple[str, int]:
-        _defport = DEFAULT_HTTPS_PORT if self.scheme == "https" else DEFAULT_HTTP_PORT
-        if not host:
-            return "", _defport
-
-        sport: str = ""
-
-        if "]:" in host:
-            host, sport = host.split("]:", 1)
-            host = host[1:]
-        elif host[0] == "[":
-            host = host[1:-1]
-        elif ":" in host:
-            host, sport = host.rsplit(":", 1)
+        if_modified_since:
+            The date and time at which the client last modified the resource.
 
-        port = int(sport) if sport and sport.isdecimal() else _defport
-        return host, port
+        is_get, is_head, is_post, is_put, is_patch, and is_delete:
+            Return True or False based on the request method.
 
-    @property
-    def port_is_default(self) -> bool:
-        return (self.port == DEFAULT_HTTPS_PORT and self.scheme == "https") or (
-            self.port == DEFAULT_HTTP_PORT
-        )
+        is_ssl:
+            Whether the current request was made via a SSL connection.
 
-    @property
-    def host_with_port(self) -> str:
-        """Returns a host:port string for this request, such as “example.com” or
-        “example.com:8080”.
-        Port is only included if it is not a default port (80 or 443)
-        """
-        if self.port_is_default:
-            return self.host
-        return f"{self.host}:{self.port}"
+        is_xhr:
+            True if current request is an XHR request.
 
-    @property
-    def url(self) -> str:
-        """Returns the current URL."""
-        url_ = f"{self.host_with_port}{self.path}"
-        query_string = self.environ.get("QUERY_STRING", "")
-        if query_string:
-            url_ = f"{url_}?{query_string}"
-        return url_
+        max_content_length:
+            From the arguments.
 
-    @property
-    def content_length(self) -> int:
-        """The content_length value as an integer."""
-        if self._content_length is None:
-            length = self.environ.get("CONTENT_LENGTH", "0")
-            self._content_length = self._validate_content_length(length)
-        return self._content_length
+        max_query_size:
+            From the arguments.
 
-    def _validate_content_length(self, length: Union[int, str]) -> int:
-        try:
-            ilength = int(length)
-        except ValueError:
-            raise errors.InvalidHeader("The Content-Length header must be a number.")
-        if ilength < 0:
-            raise errors.InvalidHeader(
-                "The value of the Content-Length header must be a positive number."
-            )
-        return ilength
+        request_method:
+            The uppercased request method, like: "GET".
 
-    @property
-    def cookies(self) -> Dict[str, Any]:
-        if self._cookies is None:
-            self._cookies = parse_cookies(self.environ.get("HTTP_COOKIE"))
-        return self._cookies
+        method:
+            Returns the same value as `request_method` except for HEAD,
+            which it returns as GET; or for POST if it has been overrided
+            by PATCH, PUT, or DELETE (see `Method override`).
 
-    @property
-    def flashes(self) -> List[Dict[str, Any]]:
-        return self._session.get(FLASHES_SESSION_KEY, [])
+        port_is_default:
+            Returns True or False, depending if the port is the default for
+            the protocol.
 
-    @property
-    def form(self) -> MultiDict:
-        if self._form is None:
-            # GET and HEAD can't have form data.
-            if self.method in (GET, HEAD):
-                self._form = MultiDict()
-            else:
-                self._form = parse_form_data(
-                    self.stream,
-                    self.content_type,
-                    self.content_length,
-                    self.encoding,
-                    self.config,
-                )
-        return self._form
+        port_string:
+            A `:port` string for the request if the port is not the default for
+            the protocol.
 
-    @property
-    def headers(self) -> HeadersDict:
-        if self._headers is None:
-            headers = HeadersDict()
-            for name, value in self.environ.items():
-                name = name.upper()
-                if name.startswith(("HTTP_", "HTTP-")):
-                    headers[name[5:]] = value
-                headers[name] = value
-            self._headers = headers
-        return self._headers
+        query:
+            A `MultiDict` object containing the query string data.
 
-    @property
-    def is_get(self) -> bool:
-        return self.method == GET
+        remote_ip:
+            IP address of the closest client or proxy to the WSGI server.
+            If your application is behind one or more reverse proxies,
+            and it doesn't pass forward the IP address of the client,
+            you can use the `access_route` attribute to retrieve the real
+            IP address of the client.
 
-    @property
-    def is_head(self) -> bool:
-        return self.real_method == HEAD
+        request_id:
+            Parse the `x-request-id` header for a value that uniquely
+            identify a request.
 
-    @property
-    def is_post(self) -> bool:
-        return self.method == POST
+        session:
+            The session data sent with the request.
 
-    @property
-    def is_put(self) -> bool:
-        return self.method == PUT
+        url:
+            Returns the full URL used for the request.
+
+        matched_route, matched_params, and matched_action:
+            Added when the request match a route.
+
+        csrf_token:
+            A CSRF (Cross-Site Request Forgery) token.
+
+        user:
+            Added when the request comes from a logged-in user.
+
+    """
+
+    method: str
+    path: str
+
+    matched_route: Route | None = None
+    matched_params: dict | None = None
+    matched_action: str | None = None
+    csrf_token: str = ""
+    user: t.Any = None
+    session: DotDict
+    locale: str | None = None
+
+    # Cache attrs
+    _form: MultiDict | None = None
+    _query: MultiDict | None = None
+
+    def __init__(
+        self,
+        *,
+        encoding: str = "utf8",
+        max_content_length: int = -1,
+        max_query_size: int | None = None,
+        **env,
+    ) -> None:
+        self.encoding = encoding
+        self.max_content_length = max_content_length
+        self.max_query_size = max_query_size
+        self.session = DotDict()
+
+        env = env or make_test_env()
+        super().__init__(env)
+
+    def __repr__(self) -> str:
+        return f"<Request {self.method} “{self.path}”>"
 
     @property
-    def is_patch(self) -> bool:
-        return self.method == PATCH
+    def language(self) -> str | None:
+        if self.locale:
+            return split_locale(self.locale)[0]
 
     @property
-    def is_delete(self) -> bool:
-        return self.method == DELETE
+    def body(self) -> BytesIO:
+        """The request body as a BytesIO stream."""
+        return self.env.get("wsgi.input") or BytesIO()
 
     @property
-    def query(self) -> MultiDict:
-        if self._query is None:
-            query_string = self.environ.get("QUERY_STRING", "")
-            self._query = parse_query_string(query_string, self.config)
-        return self._query
+    def flashes(self) -> dict:
+        """The flashed messages stored in the session cookie."""
+        return self.session.get(FLASHES_SESSION_KEY, {})
 
     @property
-    def remote_addr(self) -> str:
-        """Passed-forward IP address of the client or IP address of the
-        closest proxy to the WSGI server.
+    def form(self) -> MultiDict:
+        """A `MultiDict` object containing the parsed body data, like the
+        one sent by a HTML form with a POST, **including** the files.
         """
-        if self._remote_addr is None:
-            addr = None
-            if "HTTP_X_FORWARDED_FOR" in self.environ:
-                addr = self.environ["HTTP_X_FORWARDED_FOR"]
-            if "HTTP_X_REAL_IP" in self.environ:
-                addr = self.environ["HTTP_X_REAL_IP"]
-            elif "REMOTE_ADDR" in self.environ:
-                addr = self.environ["REMOTE_ADDR"]
-            addr = addr or "127.0.0.1"
-            self._remote_addr = addr
-        return self._remote_addr
+        if self._form is None:
+            self._form = self._parse_form()
+        return self._form
 
-    @property
-    def root_path(self) -> str:
-        return self.environ.get("SCRIPT_NAME")
+    def _parse_form(self) -> MultiDict:
+        # GET and HEAD can't have form data.
+        if self.method in (GET, HEAD):
+            return MultiDict()
+
+        return parse_form(
+            self.body,
+            self.content_type,
+            self.content_length,
+            encoding=self.encoding,
+            max_content_length=self.max_content_length,
+        )
 
     @property
-    def secure(self) -> bool:
-        return self.scheme == "https"
+    def query(self) -> MultiDict:
+        """A `MultiDict` object containing the query string data."""
+        if self._query is None:
+            self._query = self._parse_query()
+        return self._query
 
-    @property
-    def session(self) -> Dict[str, Any]:
-        return self._session
+    def _parse_query(self) -> MultiDict:
+        return parse_query_string(
+            self.query_string,
+            encoding=self.encoding,
+            max_query_size=self.max_query_size,
+        )
 
     @property
-    def stream(self) -> Any:
-        return self.environ["wsgi.input"]
+    def query_string(self) -> str:
+        """Returns the query string."""
+        return self.env.get("query_string", "")
 
     @property
-    def xhr(self) -> bool:
-        if "HTTP_X_REQUESTED_WITH" in self.environ:
-            return self.environ["HTTP_X_REQUESTED_WITH"] == "XMLHttpRequest"
-        return False
-
-    def must_check_csrf(self) -> bool:
-        """Return wether the CSRF token in this request must be checked
-        for validity."""
-        return self.method in (POST, PUT, DELETE, PATCH)
+    def url(self) -> str:
+        """Returns the current URL."""
+        return self.get_url()
 
-    @property
-    def if_none_match(self) -> List[str]:
-        """Value of the If-None-Match header, as a parsed list of strings,
-        or an empty list if the header is missing or its value is blank.
+    def get_url(self, include_query: bool = True) -> str:
+        """Returns the current URL, optionally including the query string"""
+        url = self.path
+        if include_query and self.query_string:
+            url = f"{url}?{self.query_string}"
+        return url
+
+    def get_signed_cookie(
+            self,
+            name: str,
+            default: t.Any = Undefined,
+            *,
+            salt: str = "",
+            max_age: int | None = None,
+        ) -> str | t.Any:
         """
-        if self._if_none_match is None:
-            header = self.environ.get("HTTP_IF_NONE_MATCH", "")
-            self._if_none_match = parse_comma_separated(header)
-        return self._if_none_match
+        Returns a cookie value for a signed cookie, or raises a `ValueError` if
+        there is no cookie with that name, or a `proper.errors.BadSignature`
+        exception if the signature is no longer valid.
+
+        If you provide the `default` argument the exceptions will be suppressed and
+        that default value will be returned instead.
+
+        The optional salt argument can be used to provide extra protection against
+        brute force attacks on your secret key. If supplied, the `max_age` argument
+        will be checked against the signed timestamp attached to the cookie value
+        to ensure the cookie is not older than `max_age` seconds.
+
+        For example:
+
+        $ request.get_signed_cookie("name")
+        'Jon'
+        $ request.get_signed_cookie("name", salt="name-salt")
+        'Jon' # assuming cookie was set using the same salt
+        $ request.get_signed_cookie("nonexistent-cookie")
+        KeyError: 'nonexistent-cookie'
+        $ request.get_signed_cookie("nonexistent-cookie", False)
+        False
+        $ request.get_signed_cookie("cookie-that-was-tampered-with")
+        BadSignature: ...
+        $ request.get_signed_cookie("name", max_age=60)
+        SignatureExpired: Signature age 1677.3839159 > 60 seconds
+        $ request.get_signed_cookie("name", False, max_age=60)
+        False
+"""
+        signer = current.app.get_signer(salt)
+        signed_value = self.cookies.get(name)
+        if not signed_value:
+            if default is not Undefined:
+                return default
+            else:
+                raise ValueError("Cookie not set")
 
-    @property
-    def if_modified_since(self) -> Union[datetime, str]:
-        if self._if_modified_since is None:
-            header = self.environ.get("HTTP_IF_MODIFIED_SINCE", "")
-            self._if_modified_since = parse_http_date(header) or ""
-        return self._if_modified_since
-
-
-def make_test_environ(path: str = None, **kwargs: Dict[str, Any]) -> Dict[str, str]:
-    from wsgiref.util import setup_testing_defaults
-
-    environ = {"REMOTE_ADDR": "127.0.0.1"}
-    setup_testing_defaults(environ)
-
-    if path:
-        if "?" in path:
-            path, query = path.rsplit("?", 1)
-            environ["QUERY_STRING"] = query
-        environ["PATH_INFO"] = tunnel_encode(path.strip())
+        try:
+            value = signer.unsign(signed_value, max_age=max_age)
+            if isinstance(value, bytes):
+                return value.decode()
+            else:
+                return value
 
-    environ.update(**{key: str(value) for key, value in kwargs.items()})
-    return environ
+        except itsdangerous.BadSignature as err:
+            if default is not Undefined:
+                return default
+            raise BadSignature() from err
```

### Comparing `proper-0.1.dev4/proper/router/router.py` & `proper-0.2/src/proper/router/scope.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,117 +1,113 @@
-"""Router object that holds all routes and match them to urls.
-"""
-from typing import Any, Dict, Iterable, List, Optional, Tuple
+import typing as t
 
-from proper.errors import MatchNotFound, MethodNotAllowed
 from .route import Route
-from .scope import flatten
 
 
-__all__ = ("Router", "NameNotFound")
+__all__ = (
+    "Scope",
+    "scope",
+)
+
+
+def flatten(ll: t.Iterable) -> list:
+    """
+    Flatten a list of lists and items into a list of items, without sublists
+    Examples:
+
+    >>> flatten([[1, 2, 3], 4, [5]])
+    [1, 2, 3, 4, 5]
+    >>> flatten([1, 2, 3, 4, 5])
+    [1, 2, 3, 4, 5]
+    >>> flatten([[1, 2, 3, 4, 5]])
+    [1, 2, 3, 4, 5]
+    >>> flatten([[], 1])
+    [1]
+    >>> flatten([[1, [2, 3]], 4, [5]])
+    [1, 2, 3, 4, 5]
+
+    """
+    result = []
+    for item in ll:
+        if isinstance(item, list):
+            result += flatten(item)
+        else:
+            result.append(item)
+    return result
+
+
+class Scope:
+    r"""
+    A Scope is a convenient shortcut to set a prefix and a host to a group
+    of routes.
+
+    Arguments are:
+
+    mount (str):
+        Prefix for all routes under this scope. Can contain placeholders
+        like `:name` or `:name<format>` where "format" can be:
+
+        - nothing, for matching anything except slashes
+        - `int` or `float`, for matching numbers
+        - `path`, for matching anything *including* slashes
+        - a regular expression
+
+        Note that declaring a format doesn't make type conversions, **all values
+        are passed to the view as strings**.
+
+        Examples:
 
+        - `docs/:lang<en|es|pt>`
+        - `questions/:uuid`
+        - `:year<int>/:month<int>`
+        - `:year<\d{4}>/:month<\d{2}>`
 
-class NameNotFound(Exception):
-    pass
+    host (str):
+        Optional. Host for all routes under this scope, including any subdomain
+        and an optional port. Examples: "www.example.com", "localhost:5000".
 
+        Like `mount`, it can contain placeholders like `:name` or `:name<format>`
+        with the same format rules.
 
-class Router:
-    _debug: bool
-    _routes: List
-    _routes_by_name = Dict[str, Route]
-
-    def __init__(self, *, _debug: bool = False) -> None:
-        self._routes = []
-        self._routes_by_name = {}
-        self._debug = _debug
-
-    def match(
-        self,
-        method: str,
-        path: str,
-        host: Optional[str] = None,
-    ) -> Tuple[Route, Dict[str, Any]]:
-        """Takes a method and a path, that came from an URL,
-        and tries to match them to a existing route
-
-        Arguments are:
-
-        method:
-            Usualy, one of the HTTP methods: "get", "post", "put", "delete",
-            "options", or "patch"; but it could also be another
-            application-specific value.
-
-        path:
-            The path of this route
-
-        host:
-            Optional. Host for this route, including any subdomain
-            and an optional port. Examples: "www.example.com", "localhost:5000".
-
-        Returns a matched `(route, params)`
-        """
-        # If the path match but the method do not, we need to return
-        # a list of the allowed methods with the 405 response.
-        allowed = set()
-        for route in self.routes:
-            if route.host is not None and route.host != host:
-                continue
-            match = route.match(path)
-            if not match:
-                continue
-            if route.method != method:
-                allowed.add(route.method)
-                continue
-
-            if not (route.to or route.redirect):
-                # build-only route
-                continue
-
-            params = route.defaults.copy() or {}
-            params.update(match.groupdict())
-
-            return route, params
-
-        if allowed:
-            msg = f"`{path}` does not accept a `{method}`."
-            raise MethodNotAllowed(msg, allowed=allowed)
+        Examples:
+
+        - :lang<en|es|pt>.example.com
+        - :username.localhost:5000
+
+    """
+    __slots__ = (
+        "mount",
+        "host",
+    )
+
+    mount: str
+    host: str | None
+
+    def __init__(self, mount: str, *, host: str | None = None) -> None:
+        self.mount = "/" + mount.strip("/")
+        self.host = host
+
+    def __call__(self, *routes) -> list[Route]:
+        _routes = []
+        for route in flatten(routes):
+            self._mount_route(route)
+            _routes.append(route)
+
+        return _routes
+
+    def _mount_route(self, route: Route) -> None:
+        assert isinstance(
+            route, Route
+        ), "A scope only can work over instances of `route`."
+        if route.path == "/":
+            route.path = self.mount
         else:
-            msg = f"{method} `{path}` does not match."
-            raise MatchNotFound(msg)
+            route.path = self.mount.rstrip("/") + route.path
+        route.host = self.host or route.host
+
+    def __repr__(self) -> str:
+        return (
+            f"<scope {self.mount}" + (f" host={ self.host}" if self.host else "") + ">"
+        )
 
-    @property
-    def routes(self) -> List[Route]:
-        return self._routes
-
-    @routes.setter
-    def routes(self, values: Iterable) -> None:
-        _routes = flatten(values)
-        if self._debug:
-            assert all(
-                [isinstance(x, Route) for x in _routes]
-            ), "All routes must be instances of `Route`."
-        for route in _routes:
-            route.compile_path()
-        self._routes = _routes
-        self._routes_by_name = {route.name: route for route in _routes}
-
-    def url_for(
-        self,
-        name: str,
-        object: Optional[Any] = None,
-        *,
-        _anchor: Optional[str] = None,
-        **kwargs: Dict[str, Any]
-    ) -> str:
-        route = self._routes_by_name.get(name)
-        if not route:
-            raise NameNotFound(name)
-
-        if object is not None:
-            for key in route.path_placeholders:
-                kwargs.setdefault(key, getattr(object, key))
-
-        url = route.format(**kwargs)
-        if _anchor:
-            url += "#" + _anchor
 
-        return url
+scope = Scope
```

