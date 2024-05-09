# Comparing `tmp/punkweb_bb-0.1.3.tar.gz` & `tmp/punkweb_bb-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "punkweb_bb-0.1.3.tar", last modified: Tue May  7 06:28:58 2024, max compression
+gzip compressed data, was "punkweb_bb-0.1.4.tar", last modified: Thu May  9 06:04:30 2024, max compression
```

## Comparing `punkweb_bb-0.1.3.tar` & `punkweb_bb-0.1.4.tar`

### file list

```diff
@@ -1,261 +1,263 @@
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.333790 punkweb_bb-0.1.3/
--rw-r--r--   0 pork      (1000) pork      (1000)     1507 2024-04-09 06:08:41.000000 punkweb_bb-0.1.3/LICENSE
--rw-r--r--   0 pork      (1000) pork      (1000)       64 2024-04-09 05:47:19.000000 punkweb_bb-0.1.3/MANIFEST.in
--rw-r--r--   0 pork      (1000) pork      (1000)     4843 2024-05-07 06:28:58.333790 punkweb_bb-0.1.3/PKG-INFO
--rw-r--r--   0 pork      (1000) pork      (1000)     4189 2024-05-07 06:14:42.000000 punkweb_bb-0.1.3/README.md
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.321790 punkweb_bb-0.1.3/punkweb_bb/
--rw-r--r--   0 pork      (1000) pork      (1000)        0 2023-08-20 16:04:51.000000 punkweb_bb-0.1.3/punkweb_bb/__init__.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.321790 punkweb_bb-0.1.3/punkweb_bb/__pycache__/
--rw-r--r--   0 pork      (1000) pork      (1000)      161 2024-04-09 05:48:25.000000 punkweb_bb-0.1.3/punkweb_bb/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     3679 2024-04-09 05:48:25.000000 punkweb_bb-0.1.3/punkweb_bb/__pycache__/admin.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     2980 2024-04-09 05:48:25.000000 punkweb_bb-0.1.3/punkweb_bb/__pycache__/admin_forms.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      730 2024-04-09 06:55:15.000000 punkweb_bb-0.1.3/punkweb_bb/__pycache__/apps.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     8534 2024-04-09 06:32:38.000000 punkweb_bb-0.1.3/punkweb_bb/__pycache__/bbcode_tags.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      392 2024-04-09 06:44:27.000000 punkweb_bb-0.1.3/punkweb_bb/__pycache__/context_processors.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     4680 2024-04-09 05:48:25.000000 punkweb_bb-0.1.3/punkweb_bb/__pycache__/forms.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     1249 2024-04-09 05:48:25.000000 punkweb_bb-0.1.3/punkweb_bb/__pycache__/middleware.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     1478 2024-04-09 05:48:25.000000 punkweb_bb-0.1.3/punkweb_bb/__pycache__/mixins.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)    12308 2024-05-07 05:16:02.000000 punkweb_bb-0.1.3/punkweb_bb/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      990 2024-04-09 05:48:25.000000 punkweb_bb-0.1.3/punkweb_bb/__pycache__/pagination.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     5335 2024-04-09 07:07:59.000000 punkweb_bb-0.1.3/punkweb_bb/__pycache__/parsers.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      448 2024-04-09 05:48:25.000000 punkweb_bb-0.1.3/punkweb_bb/__pycache__/response.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      665 2024-05-07 02:14:22.000000 punkweb_bb-0.1.3/punkweb_bb/__pycache__/settings.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      864 2024-04-09 05:48:25.000000 punkweb_bb-0.1.3/punkweb_bb/__pycache__/signals.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)    50877 2024-05-07 06:13:11.000000 punkweb_bb-0.1.3/punkweb_bb/__pycache__/tests.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     2304 2024-04-09 05:48:25.000000 punkweb_bb-0.1.3/punkweb_bb/__pycache__/urls.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)    15592 2024-05-07 06:13:06.000000 punkweb_bb-0.1.3/punkweb_bb/__pycache__/views.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     1552 2024-04-09 05:48:25.000000 punkweb_bb-0.1.3/punkweb_bb/__pycache__/widgets.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     2493 2024-04-05 21:20:18.000000 punkweb_bb-0.1.3/punkweb_bb/admin.py
--rw-r--r--   0 pork      (1000) pork      (1000)     1128 2024-04-03 19:18:44.000000 punkweb_bb-0.1.3/punkweb_bb/admin_forms.py
--rw-r--r--   0 pork      (1000) pork      (1000)      207 2024-04-09 06:52:38.000000 punkweb_bb-0.1.3/punkweb_bb/apps.py
--rw-r--r--   0 pork      (1000) pork      (1000)     4419 2024-04-09 06:31:31.000000 punkweb_bb-0.1.3/punkweb_bb/bbcode_tags.py
--rw-r--r--   0 pork      (1000) pork      (1000)      146 2024-04-09 04:54:41.000000 punkweb_bb-0.1.3/punkweb_bb/context_processors.py
--rw-r--r--   0 pork      (1000) pork      (1000)     1977 2024-04-03 19:20:08.000000 punkweb_bb-0.1.3/punkweb_bb/forms.py
--rw-r--r--   0 pork      (1000) pork      (1000)      456 2024-04-05 21:11:30.000000 punkweb_bb-0.1.3/punkweb_bb/middleware.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.321790 punkweb_bb-0.1.3/punkweb_bb/migrations/
--rw-r--r--   0 pork      (1000) pork      (1000)     8950 2024-04-09 07:09:02.000000 punkweb_bb-0.1.3/punkweb_bb/migrations/0001_initial.py
--rw-r--r--   0 pork      (1000) pork      (1000)      388 2024-05-07 04:24:13.000000 punkweb_bb-0.1.3/punkweb_bb/migrations/0002_thread_view_count.py
--rw-r--r--   0 pork      (1000) pork      (1000)        0 2023-08-20 16:04:51.000000 punkweb_bb-0.1.3/punkweb_bb/migrations/__init__.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.321790 punkweb_bb-0.1.3/punkweb_bb/migrations/__pycache__/
--rw-r--r--   0 pork      (1000) pork      (1000)     6456 2024-04-09 07:09:10.000000 punkweb_bb-0.1.3/punkweb_bb/migrations/__pycache__/0001_initial.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      815 2024-05-07 04:24:16.000000 punkweb_bb-0.1.3/punkweb_bb/migrations/__pycache__/0002_thread_view_count.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      172 2024-04-09 05:48:25.000000 punkweb_bb-0.1.3/punkweb_bb/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      395 2024-04-03 19:16:01.000000 punkweb_bb-0.1.3/punkweb_bb/mixins.py
--rw-r--r--   0 pork      (1000) pork      (1000)     5519 2024-05-07 05:16:01.000000 punkweb_bb-0.1.3/punkweb_bb/models.py
--rw-r--r--   0 pork      (1000) pork      (1000)      409 2024-04-06 08:06:22.000000 punkweb_bb-0.1.3/punkweb_bb/pagination.py
--rw-r--r--   0 pork      (1000) pork      (1000)     2732 2024-04-09 07:07:58.000000 punkweb_bb-0.1.3/punkweb_bb/parsers.py
--rw-r--r--   0 pork      (1000) pork      (1000)      130 2024-04-03 19:15:29.000000 punkweb_bb-0.1.3/punkweb_bb/response.py
--rw-r--r--   0 pork      (1000) pork      (1000)      312 2024-05-07 02:14:21.000000 punkweb_bb-0.1.3/punkweb_bb/settings.py
--rw-r--r--   0 pork      (1000) pork      (1000)      365 2024-04-03 19:18:44.000000 punkweb_bb-0.1.3/punkweb_bb/signals.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.317790 punkweb_bb-0.1.3/punkweb_bb/static/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.321790 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.321790 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/
--rw-r--r--   0 pork      (1000) pork      (1000)     1455 2024-04-06 07:32:15.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/defaults.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1331 2024-04-06 07:48:47.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/index.css
--rw-r--r--   0 pork      (1000) pork      (1000)      234 2024-04-03 22:23:23.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/login.css
--rw-r--r--   0 pork      (1000) pork      (1000)      395 2024-04-08 22:57:27.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/members.css
--rw-r--r--   0 pork      (1000) pork      (1000)      321 2024-04-03 21:47:53.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/post-form.css
--rw-r--r--   0 pork      (1000) pork      (1000)      916 2024-05-07 01:46:57.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/profile.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1296 2024-04-05 22:11:56.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/punkweb-modal.css
--rw-r--r--   0 pork      (1000) pork      (1000)    11284 2024-04-08 22:28:14.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/punkweb.css
--rw-r--r--   0 pork      (1000) pork      (1000)      308 2024-04-06 07:53:29.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/settings.css
--rw-r--r--   0 pork      (1000) pork      (1000)      333 2024-04-08 23:25:45.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/shoutbox.css
--rw-r--r--   0 pork      (1000) pork      (1000)      536 2024-04-06 07:48:52.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/subcategory.css
--rw-r--r--   0 pork      (1000) pork      (1000)      329 2024-04-03 19:20:08.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/thread-form.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1508 2024-04-06 07:53:50.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/thread.css
--rw-r--r--   0 pork      (1000) pork      (1000)      448 2024-04-05 15:05:58.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/typography.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1154 2024-04-05 19:38:35.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/variables.css
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.321790 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/editor/
--rw-r--r--   0 pork      (1000) pork      (1000)     1466 2024-04-06 07:32:28.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-content.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1624 2024-04-03 19:20:08.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-tags.js
--rw-r--r--   0 pork      (1000) pork      (1000)        0 2024-04-03 19:20:08.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.css
--rw-r--r--   0 pork      (1000) pork      (1000)      606 2024-04-08 22:10:44.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.js
--rw-r--r--   0 pork      (1000) pork      (1000)      318 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/favicon.ico
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.325790 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/img/
--rw-r--r--   0 pork      (1000) pork      (1000)    60475 2024-04-03 19:20:08.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/img/default-profile-image.png
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.325790 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/js/
--rw-r--r--   0 pork      (1000) pork      (1000)      179 2024-04-03 19:20:08.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/js/punkweb-modal.js
--rw-r--r--   0 pork      (1000) pork      (1000)      142 2024-04-08 20:20:47.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/js/shoutbox.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.325790 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/
--rw-r--r--   0 pork      (1000) pork      (1000)    44307 2024-04-03 19:17:23.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/htmx-1.9.4.min.js
--rw-r--r--   0 pork      (1000) pork      (1000)    87461 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/jquery-3.7.0.min.js
--rw-r--r--   0 pork      (1000) pork      (1000)    10331 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/open-color.css
--rw-r--r--   0 pork      (1000) pork      (1000)     3948 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/prism.css
--rw-r--r--   0 pork      (1000) pork      (1000)   576492 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/prism.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.325790 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/
--rw-r--r--   0 pork      (1000) pork      (1000)     4129 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/README.md
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.325790 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.325790 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/
--rw-r--r--   0 pork      (1000) pork      (1000)    61679 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/bbcode.js
--rw-r--r--   0 pork      (1000) pork      (1000)    26086 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/xhtml.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.325790 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/
--rw-r--r--   0 pork      (1000) pork      (1000)    11260 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/material.js
--rw-r--r--   0 pork      (1000) pork      (1000)    15873 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/monocons.js
--rw-r--r--   0 pork      (1000) pork      (1000)   312959 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.bbcode.js
--rw-r--r--   0 pork      (1000) pork      (1000)   251279 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.js
--rw-r--r--   0 pork      (1000) pork      (1000)   277366 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.xhtml.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.325790 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/
--rw-r--r--   0 pork      (1000) pork      (1000)     3446 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/alternative-lists.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2571 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autosave.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2791 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autoyoutube.js
--rw-r--r--   0 pork      (1000) pork      (1000)     6306 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/dragdrop.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2528 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/format.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2059 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/plaintext.js
--rw-r--r--   0 pork      (1000) pork      (1000)     9375 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/undo.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2067 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/v1compat.js
--rw-r--r--   0 pork      (1000) pork      (1000)   249123 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/sceditor.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.325790 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.325790 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/
--rw-r--r--   0 pork      (1000) pork      (1000)     1476 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/default.css
--rw-r--r--   0 pork      (1000) pork      (1000)    11194 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/default.css
--rw-r--r--   0 pork      (1000) pork      (1000)    11500 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/defaultdark.css
--rw-r--r--   0 pork      (1000) pork      (1000)     4583 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/famfamfam.png
--rw-r--r--   0 pork      (1000) pork      (1000)    12943 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/modern.css
--rw-r--r--   0 pork      (1000) pork      (1000)    13431 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office-toolbar.css
--rw-r--r--   0 pork      (1000) pork      (1000)    14124 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office.css
--rw-r--r--   0 pork      (1000) pork      (1000)    13183 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/square.css
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.329790 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/
--rw-r--r--   0 pork      (1000) pork      (1000)      756 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/alien.png
--rw-r--r--   0 pork      (1000) pork      (1000)     1182 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angel.png
--rw-r--r--   0 pork      (1000) pork      (1000)      781 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angry.png
--rw-r--r--   0 pork      (1000) pork      (1000)      972 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blink.png
--rw-r--r--   0 pork      (1000) pork      (1000)      865 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blush.png
--rw-r--r--   0 pork      (1000) pork      (1000)      753 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cheerful.png
--rw-r--r--   0 pork      (1000) pork      (1000)      965 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cool.png
--rw-r--r--   0 pork      (1000) pork      (1000)      421 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/credits.txt
--rw-r--r--   0 pork      (1000) pork      (1000)      877 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cwy.png
--rw-r--r--   0 pork      (1000) pork      (1000)     1012 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/devil.png
--rw-r--r--   0 pork      (1000) pork      (1000)      991 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/dizzy.png
--rw-r--r--   0 pork      (1000) pork      (1000)      983 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ermm.png
--rw-r--r--   0 pork      (1000) pork      (1000)      793 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/face.png
--rw-r--r--   0 pork      (1000) pork      (1000)      792 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/getlost.png
--rw-r--r--   0 pork      (1000) pork      (1000)      867 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/grin.png
--rw-r--r--   0 pork      (1000) pork      (1000)      792 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/happy.png
--rw-r--r--   0 pork      (1000) pork      (1000)      572 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/heart.png
--rw-r--r--   0 pork      (1000) pork      (1000)      793 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/kissing.png
--rw-r--r--   0 pork      (1000) pork      (1000)      912 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/laughing.png
--rw-r--r--   0 pork      (1000) pork      (1000)      694 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ninja.png
--rw-r--r--   0 pork      (1000) pork      (1000)      804 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pinch.png
--rw-r--r--   0 pork      (1000) pork      (1000)      799 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pouty.png
--rw-r--r--   0 pork      (1000) pork      (1000)      789 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sad.png
--rw-r--r--   0 pork      (1000) pork      (1000)      780 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/shocked.png
--rw-r--r--   0 pork      (1000) pork      (1000)      783 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sick.png
--rw-r--r--   0 pork      (1000) pork      (1000)      788 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sideways.png
--rw-r--r--   0 pork      (1000) pork      (1000)      930 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/silly.png
--rw-r--r--   0 pork      (1000) pork      (1000)     1039 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sleeping.png
--rw-r--r--   0 pork      (1000) pork      (1000)      983 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/smile.png
--rw-r--r--   0 pork      (1000) pork      (1000)      981 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/tongue.png
--rw-r--r--   0 pork      (1000) pork      (1000)      763 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/unsure.png
--rw-r--r--   0 pork      (1000) pork      (1000)      718 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/w00t.png
--rw-r--r--   0 pork      (1000) pork      (1000)      810 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wassat.png
--rw-r--r--   0 pork      (1000) pork      (1000)     1072 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/whistling.png
--rw-r--r--   0 pork      (1000) pork      (1000)      791 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wink.png
--rw-r--r--   0 pork      (1000) pork      (1000)     1010 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wub.png
--rw-r--r--   0 pork      (1000) pork      (1000)     2237 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/example.html
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.329790 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/
--rw-r--r--   0 pork      (1000) pork      (1000)     3235 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ar.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2803 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ca.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2543 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cn.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2879 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cs.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2504 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/de.js
--rw-r--r--   0 pork      (1000) pork      (1000)     4020 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/el.js
--rw-r--r--   0 pork      (1000) pork      (1000)      102 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/en-US.js
--rw-r--r--   0 pork      (1000) pork      (1000)      250 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/en.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2831 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/es.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2018 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/et.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3577 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fa.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2813 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fi.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2906 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fr.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2802 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/gl.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2956 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/hu.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2718 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/id.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2981 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/it.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3259 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ja.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3141 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/lt.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2797 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nb.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2903 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nl.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2745 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pl.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2739 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt-BR.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2810 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3192 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ru.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3017 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sk.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2210 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sv.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2122 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/template.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2772 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tr.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2557 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tw.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3102 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/uk.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2913 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/vi.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.329790 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.329790 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/
--rw-r--r--   0 pork      (1000) pork      (1000)    17567 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/bbcode.js
--rw-r--r--   0 pork      (1000) pork      (1000)     8873 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/xhtml.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.329790 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/
--rw-r--r--   0 pork      (1000) pork      (1000)     9203 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/material.js
--rw-r--r--   0 pork      (1000) pork      (1000)    14779 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/monocons.js
--rw-r--r--   0 pork      (1000) pork      (1000)    91043 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.bbcode.min.js
--rw-r--r--   0 pork      (1000) pork      (1000)    73632 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.min.js
--rw-r--r--   0 pork      (1000) pork      (1000)    82349 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.xhtml.min.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.329790 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/
--rw-r--r--   0 pork      (1000) pork      (1000)     1417 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/alternative-lists.js
--rw-r--r--   0 pork      (1000) pork      (1000)     1259 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autosave.js
--rw-r--r--   0 pork      (1000) pork      (1000)     1107 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autoyoutube.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3667 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/dragdrop.js
--rw-r--r--   0 pork      (1000) pork      (1000)     1088 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/format.js
--rw-r--r--   0 pork      (1000) pork      (1000)      775 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/plaintext.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2760 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/undo.js
--rw-r--r--   0 pork      (1000) pork      (1000)      934 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/v1compat.js
--rw-r--r--   0 pork      (1000) pork      (1000)    73296 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/sceditor.min.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.329790 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.329790 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/
--rw-r--r--   0 pork      (1000) pork      (1000)     1016 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/default.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)     9307 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/default.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)     9570 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/defaultdark.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)     4583 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/famfamfam.png
--rw-r--r--   0 pork      (1000) pork      (1000)    10656 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/modern.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)    12604 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office-toolbar.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)    13148 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)    10710 2024-04-03 19:11:51.000000 punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/square.min.css
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.317790 punkweb_bb-0.1.3/punkweb_bb/templates/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.333790 punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/
--rw-r--r--   0 pork      (1000) pork      (1000)     4037 2024-05-07 02:13:59.000000 punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/base.html
--rw-r--r--   0 pork      (1000) pork      (1000)      460 2024-04-05 19:59:05.000000 punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/base_modal.html
--rw-r--r--   0 pork      (1000) pork      (1000)      396 2024-04-06 07:23:56.000000 punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/bbcode.html
--rw-r--r--   0 pork      (1000) pork      (1000)     8127 2024-04-09 06:45:08.000000 punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/index.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1087 2024-04-06 02:06:29.000000 punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/login.html
--rw-r--r--   0 pork      (1000) pork      (1000)     2729 2024-04-08 23:13:19.000000 punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/members.html
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.333790 punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/partials/
--rw-r--r--   0 pork      (1000) pork      (1000)      417 2024-04-06 02:06:29.000000 punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/partials/post_delete.html
--rw-r--r--   0 pork      (1000) pork      (1000)      565 2024-04-06 02:06:29.000000 punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/partials/post_update.html
--rw-r--r--   0 pork      (1000) pork      (1000)      425 2024-04-06 02:06:29.000000 punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/partials/thread_delete.html
--rw-r--r--   0 pork      (1000) pork      (1000)     2948 2024-04-08 23:26:38.000000 punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/profile.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1994 2024-04-07 22:46:43.000000 punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/settings.html
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.333790 punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/shoutbox/
--rw-r--r--   0 pork      (1000) pork      (1000)      312 2024-04-08 23:26:13.000000 punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/shoutbox/shout_list.html
--rw-r--r--   0 pork      (1000) pork      (1000)      672 2024-04-08 23:49:26.000000 punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/shoutbox/shoutbox.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1167 2024-04-06 02:06:29.000000 punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/signup.html
--rw-r--r--   0 pork      (1000) pork      (1000)     4950 2024-05-07 04:34:46.000000 punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/subcategory.html
--rw-r--r--   0 pork      (1000) pork      (1000)     7595 2024-05-07 04:36:10.000000 punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/thread.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1537 2024-05-07 04:34:23.000000 punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/thread_create.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1730 2024-05-07 04:35:30.000000 punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/thread_update.html
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.333790 punkweb_bb-0.1.3/punkweb_bb/templatetags/
--rw-r--r--   0 pork      (1000) pork      (1000)        0 2024-05-07 04:31:09.000000 punkweb_bb-0.1.3/punkweb_bb/templatetags/__init__.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.333790 punkweb_bb-0.1.3/punkweb_bb/templatetags/__pycache__/
--rw-r--r--   0 pork      (1000) pork      (1000)      174 2024-05-07 04:31:10.000000 punkweb_bb-0.1.3/punkweb_bb/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      621 2024-05-07 04:30:58.000000 punkweb_bb-0.1.3/punkweb_bb/templatetags/__pycache__/humanize_count.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      619 2024-05-07 04:31:10.000000 punkweb_bb-0.1.3/punkweb_bb/templatetags/__pycache__/humanize_int.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      833 2024-04-09 07:07:10.000000 punkweb_bb-0.1.3/punkweb_bb/templatetags/__pycache__/shoutbox_bbcode.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      248 2024-05-07 04:31:08.000000 punkweb_bb-0.1.3/punkweb_bb/templatetags/humanize_int.py
--rw-r--r--   0 pork      (1000) pork      (1000)      310 2024-04-09 07:07:08.000000 punkweb_bb-0.1.3/punkweb_bb/templatetags/shoutbox_bbcode.py
--rw-r--r--   0 pork      (1000) pork      (1000)    25989 2024-05-07 06:12:50.000000 punkweb_bb-0.1.3/punkweb_bb/tests.py
--rw-r--r--   0 pork      (1000) pork      (1000)     1538 2024-04-08 22:43:34.000000 punkweb_bb-0.1.3/punkweb_bb/urls.py
--rw-r--r--   0 pork      (1000) pork      (1000)    10723 2024-05-07 06:13:06.000000 punkweb_bb-0.1.3/punkweb_bb/views.py
--rw-r--r--   0 pork      (1000) pork      (1000)      840 2024-04-03 19:20:08.000000 punkweb_bb-0.1.3/punkweb_bb/widgets.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-07 06:28:58.321790 punkweb_bb-0.1.3/punkweb_bb.egg-info/
--rw-r--r--   0 pork      (1000) pork      (1000)     4843 2024-05-07 06:28:58.000000 punkweb_bb-0.1.3/punkweb_bb.egg-info/PKG-INFO
--rw-r--r--   0 pork      (1000) pork      (1000)    13346 2024-05-07 06:28:58.000000 punkweb_bb-0.1.3/punkweb_bb.egg-info/SOURCES.txt
--rw-r--r--   0 pork      (1000) pork      (1000)        1 2024-05-07 06:28:58.000000 punkweb_bb-0.1.3/punkweb_bb.egg-info/dependency_links.txt
--rw-r--r--   0 pork      (1000) pork      (1000)        1 2024-04-09 07:09:59.000000 punkweb_bb-0.1.3/punkweb_bb.egg-info/not-zip-safe
--rw-r--r--   0 pork      (1000) pork      (1000)       41 2024-05-07 06:28:58.000000 punkweb_bb-0.1.3/punkweb_bb.egg-info/requires.txt
--rw-r--r--   0 pork      (1000) pork      (1000)       11 2024-05-07 06:28:58.000000 punkweb_bb-0.1.3/punkweb_bb.egg-info/top_level.txt
--rw-r--r--   0 pork      (1000) pork      (1000)       38 2024-05-07 06:28:58.333790 punkweb_bb-0.1.3/setup.cfg
--rw-r--r--   0 pork      (1000) pork      (1000)      986 2024-05-07 06:28:57.000000 punkweb_bb-0.1.3/setup.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.064355 punkweb_bb-0.1.4/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1507 2024-04-09 06:08:41.000000 punkweb_bb-0.1.4/LICENSE
+-rw-r--r--   0 pork      (1000) pork      (1000)       64 2024-04-09 05:47:19.000000 punkweb_bb-0.1.4/MANIFEST.in
+-rw-r--r--   0 pork      (1000) pork      (1000)     4992 2024-05-09 06:04:30.064355 punkweb_bb-0.1.4/PKG-INFO
+-rw-r--r--   0 pork      (1000) pork      (1000)     4338 2024-05-09 05:30:29.000000 punkweb_bb-0.1.4/README.md
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.048355 punkweb_bb-0.1.4/punkweb_bb/
+-rw-r--r--   0 pork      (1000) pork      (1000)        0 2023-08-20 16:04:51.000000 punkweb_bb-0.1.4/punkweb_bb/__init__.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.048355 punkweb_bb-0.1.4/punkweb_bb/__pycache__/
+-rw-r--r--   0 pork      (1000) pork      (1000)      161 2024-04-09 05:48:25.000000 punkweb_bb-0.1.4/punkweb_bb/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     3679 2024-04-09 05:48:25.000000 punkweb_bb-0.1.4/punkweb_bb/__pycache__/admin.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     2980 2024-04-09 05:48:25.000000 punkweb_bb-0.1.4/punkweb_bb/__pycache__/admin_forms.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      730 2024-04-09 06:55:15.000000 punkweb_bb-0.1.4/punkweb_bb/__pycache__/apps.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     8534 2024-04-09 06:32:38.000000 punkweb_bb-0.1.4/punkweb_bb/__pycache__/bbcode_tags.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      392 2024-04-09 06:44:27.000000 punkweb_bb-0.1.4/punkweb_bb/__pycache__/context_processors.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     4680 2024-04-09 05:48:25.000000 punkweb_bb-0.1.4/punkweb_bb/__pycache__/forms.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1581 2024-05-09 05:36:59.000000 punkweb_bb-0.1.4/punkweb_bb/__pycache__/guests.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1560 2024-05-09 05:37:45.000000 punkweb_bb-0.1.4/punkweb_bb/__pycache__/middleware.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1478 2024-04-09 05:48:25.000000 punkweb_bb-0.1.4/punkweb_bb/__pycache__/mixins.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)    12308 2024-05-07 05:16:02.000000 punkweb_bb-0.1.4/punkweb_bb/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      990 2024-04-09 05:48:25.000000 punkweb_bb-0.1.4/punkweb_bb/__pycache__/pagination.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     5335 2024-04-09 07:07:59.000000 punkweb_bb-0.1.4/punkweb_bb/__pycache__/parsers.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      448 2024-04-09 05:48:25.000000 punkweb_bb-0.1.4/punkweb_bb/__pycache__/response.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      947 2024-05-09 05:27:51.000000 punkweb_bb-0.1.4/punkweb_bb/__pycache__/settings.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      864 2024-04-09 05:48:25.000000 punkweb_bb-0.1.4/punkweb_bb/__pycache__/signals.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)    51829 2024-05-09 05:55:07.000000 punkweb_bb-0.1.4/punkweb_bb/__pycache__/tests.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     2304 2024-04-09 05:48:25.000000 punkweb_bb-0.1.4/punkweb_bb/__pycache__/urls.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)    16108 2024-05-09 05:54:18.000000 punkweb_bb-0.1.4/punkweb_bb/__pycache__/views.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1552 2024-04-09 05:48:25.000000 punkweb_bb-0.1.4/punkweb_bb/__pycache__/widgets.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     2493 2024-04-05 21:20:18.000000 punkweb_bb-0.1.4/punkweb_bb/admin.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     1128 2024-04-03 19:18:44.000000 punkweb_bb-0.1.4/punkweb_bb/admin_forms.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      207 2024-04-09 06:52:38.000000 punkweb_bb-0.1.4/punkweb_bb/apps.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     4419 2024-04-09 06:31:31.000000 punkweb_bb-0.1.4/punkweb_bb/bbcode_tags.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      146 2024-04-09 04:54:41.000000 punkweb_bb-0.1.4/punkweb_bb/context_processors.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     1977 2024-04-03 19:20:08.000000 punkweb_bb-0.1.4/punkweb_bb/forms.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      467 2024-05-09 05:36:58.000000 punkweb_bb-0.1.4/punkweb_bb/guests.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      628 2024-05-09 05:37:44.000000 punkweb_bb-0.1.4/punkweb_bb/middleware.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.048355 punkweb_bb-0.1.4/punkweb_bb/migrations/
+-rw-r--r--   0 pork      (1000) pork      (1000)     8950 2024-04-09 07:09:02.000000 punkweb_bb-0.1.4/punkweb_bb/migrations/0001_initial.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      388 2024-05-07 04:24:13.000000 punkweb_bb-0.1.4/punkweb_bb/migrations/0002_thread_view_count.py
+-rw-r--r--   0 pork      (1000) pork      (1000)        0 2023-08-20 16:04:51.000000 punkweb_bb-0.1.4/punkweb_bb/migrations/__init__.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.052355 punkweb_bb-0.1.4/punkweb_bb/migrations/__pycache__/
+-rw-r--r--   0 pork      (1000) pork      (1000)     6456 2024-04-09 07:09:10.000000 punkweb_bb-0.1.4/punkweb_bb/migrations/__pycache__/0001_initial.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      815 2024-05-07 04:24:16.000000 punkweb_bb-0.1.4/punkweb_bb/migrations/__pycache__/0002_thread_view_count.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      172 2024-04-09 05:48:25.000000 punkweb_bb-0.1.4/punkweb_bb/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      395 2024-04-03 19:16:01.000000 punkweb_bb-0.1.4/punkweb_bb/mixins.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     5519 2024-05-07 05:16:01.000000 punkweb_bb-0.1.4/punkweb_bb/models.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      409 2024-04-06 08:06:22.000000 punkweb_bb-0.1.4/punkweb_bb/pagination.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     2732 2024-04-09 07:07:58.000000 punkweb_bb-0.1.4/punkweb_bb/parsers.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      130 2024-04-03 19:15:29.000000 punkweb_bb-0.1.4/punkweb_bb/response.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      517 2024-05-09 05:27:49.000000 punkweb_bb-0.1.4/punkweb_bb/settings.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      365 2024-04-03 19:18:44.000000 punkweb_bb-0.1.4/punkweb_bb/signals.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.048355 punkweb_bb-0.1.4/punkweb_bb/static/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.052355 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.052355 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1455 2024-04-06 07:32:15.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/defaults.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1331 2024-04-06 07:48:47.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/index.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      234 2024-04-03 22:23:23.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/login.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      395 2024-04-08 22:57:27.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/members.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      321 2024-04-03 21:47:53.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/post-form.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      916 2024-05-07 01:46:57.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/profile.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1296 2024-04-05 22:11:56.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/punkweb-modal.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    11745 2024-05-09 05:20:26.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/punkweb.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      308 2024-04-06 07:53:29.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/settings.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      333 2024-04-08 23:25:45.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/shoutbox.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      536 2024-04-06 07:48:52.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/subcategory.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      329 2024-04-03 19:20:08.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/thread-form.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1508 2024-04-06 07:53:50.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/thread.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      448 2024-04-05 15:05:58.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/typography.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1154 2024-04-05 19:38:35.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/variables.css
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.052355 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/editor/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1466 2024-04-06 07:32:28.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-content.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1624 2024-04-03 19:20:08.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-tags.js
+-rw-r--r--   0 pork      (1000) pork      (1000)        0 2024-04-03 19:20:08.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      606 2024-04-08 22:10:44.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      318 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/favicon.ico
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.052355 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/img/
+-rw-r--r--   0 pork      (1000) pork      (1000)    60475 2024-04-03 19:20:08.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/img/default-profile-image.png
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.052355 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/js/
+-rw-r--r--   0 pork      (1000) pork      (1000)      179 2024-04-03 19:20:08.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/js/punkweb-modal.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      142 2024-04-08 20:20:47.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/js/shoutbox.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.052355 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/
+-rw-r--r--   0 pork      (1000) pork      (1000)    44307 2024-04-03 19:17:23.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/htmx-1.9.4.min.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    87461 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/jquery-3.7.0.min.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    10331 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/open-color.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     3948 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/prism.css
+-rw-r--r--   0 pork      (1000) pork      (1000)   576492 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/prism.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.052355 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/
+-rw-r--r--   0 pork      (1000) pork      (1000)     4129 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/README.md
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.052355 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.052355 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/
+-rw-r--r--   0 pork      (1000) pork      (1000)    61679 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/bbcode.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    26086 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/xhtml.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.052355 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/
+-rw-r--r--   0 pork      (1000) pork      (1000)    11260 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/material.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    15873 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/monocons.js
+-rw-r--r--   0 pork      (1000) pork      (1000)   312959 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.bbcode.js
+-rw-r--r--   0 pork      (1000) pork      (1000)   251279 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.js
+-rw-r--r--   0 pork      (1000) pork      (1000)   277366 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.xhtml.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.056355 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/
+-rw-r--r--   0 pork      (1000) pork      (1000)     3446 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/alternative-lists.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2571 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autosave.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2791 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autoyoutube.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     6306 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/dragdrop.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2528 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/format.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2059 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/plaintext.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     9375 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/undo.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2067 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/v1compat.js
+-rw-r--r--   0 pork      (1000) pork      (1000)   249123 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/sceditor.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.056355 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.056355 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1476 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/default.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    11194 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/default.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    11500 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/defaultdark.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     4583 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/famfamfam.png
+-rw-r--r--   0 pork      (1000) pork      (1000)    12943 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/modern.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    13431 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office-toolbar.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    14124 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    13183 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/square.css
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.056355 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/
+-rw-r--r--   0 pork      (1000) pork      (1000)      756 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/alien.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     1182 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angel.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      781 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angry.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      972 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blink.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      865 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blush.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      753 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cheerful.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      965 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cool.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      421 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/credits.txt
+-rw-r--r--   0 pork      (1000) pork      (1000)      877 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cwy.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     1012 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/devil.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      991 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/dizzy.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      983 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ermm.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      793 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/face.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      792 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/getlost.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      867 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/grin.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      792 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/happy.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      572 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/heart.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      793 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/kissing.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      912 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/laughing.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      694 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ninja.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      804 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pinch.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      799 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pouty.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      789 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sad.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      780 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/shocked.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      783 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sick.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      788 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sideways.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      930 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/silly.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     1039 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sleeping.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      983 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/smile.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      981 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/tongue.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      763 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/unsure.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      718 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/w00t.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      810 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wassat.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     1072 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/whistling.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      791 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wink.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     1010 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wub.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     2237 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/example.html
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.060355 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/
+-rw-r--r--   0 pork      (1000) pork      (1000)     3235 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ar.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2803 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ca.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2543 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cn.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2879 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cs.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2504 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/de.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     4020 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/el.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      102 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/en-US.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      250 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/en.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2831 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/es.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2018 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/et.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3577 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fa.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2813 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fi.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2906 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fr.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2802 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/gl.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2956 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/hu.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2718 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/id.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2981 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/it.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3259 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ja.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3141 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/lt.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2797 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nb.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2903 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nl.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2745 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pl.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2739 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt-BR.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2810 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3192 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ru.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3017 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sk.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2210 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sv.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2122 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/template.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2772 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tr.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2557 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tw.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3102 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/uk.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2913 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/vi.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.060355 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.060355 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/
+-rw-r--r--   0 pork      (1000) pork      (1000)    17567 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/bbcode.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     8873 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/xhtml.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.060355 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/
+-rw-r--r--   0 pork      (1000) pork      (1000)     9203 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/material.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    14779 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/monocons.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    91043 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.bbcode.min.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    73632 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.min.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    82349 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.xhtml.min.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.060355 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1417 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/alternative-lists.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     1259 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autosave.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     1107 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autoyoutube.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3667 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/dragdrop.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     1088 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/format.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      775 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/plaintext.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2760 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/undo.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      934 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/v1compat.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    73296 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/sceditor.min.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.060355 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.060355 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1016 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/default.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     9307 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/default.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     9570 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/defaultdark.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     4583 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/famfamfam.png
+-rw-r--r--   0 pork      (1000) pork      (1000)    10656 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/modern.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    12604 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office-toolbar.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    13148 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    10710 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/square.min.css
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.048355 punkweb_bb-0.1.4/punkweb_bb/templates/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.064355 punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/
+-rw-r--r--   0 pork      (1000) pork      (1000)     4037 2024-05-07 02:13:59.000000 punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/base.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      460 2024-04-05 19:59:05.000000 punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/base_modal.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      396 2024-04-06 07:23:56.000000 punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/bbcode.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     8703 2024-05-09 05:55:01.000000 punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/index.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1087 2024-04-06 02:06:29.000000 punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/login.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     2729 2024-04-08 23:13:19.000000 punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/members.html
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.064355 punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/partials/
+-rw-r--r--   0 pork      (1000) pork      (1000)      417 2024-04-06 02:06:29.000000 punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/partials/post_delete.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      565 2024-04-06 02:06:29.000000 punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/partials/post_update.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      425 2024-04-06 02:06:29.000000 punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/partials/thread_delete.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     2948 2024-04-08 23:26:38.000000 punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/profile.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1994 2024-04-07 22:46:43.000000 punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/settings.html
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.064355 punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/shoutbox/
+-rw-r--r--   0 pork      (1000) pork      (1000)      312 2024-04-08 23:26:13.000000 punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/shoutbox/shout_list.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      672 2024-04-08 23:49:26.000000 punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/shoutbox/shoutbox.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1167 2024-04-06 02:06:29.000000 punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/signup.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     4950 2024-05-07 04:34:46.000000 punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/subcategory.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     7595 2024-05-07 04:36:10.000000 punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/thread.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1537 2024-05-07 04:34:23.000000 punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/thread_create.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1730 2024-05-07 04:35:30.000000 punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/thread_update.html
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.064355 punkweb_bb-0.1.4/punkweb_bb/templatetags/
+-rw-r--r--   0 pork      (1000) pork      (1000)        0 2024-05-07 04:31:09.000000 punkweb_bb-0.1.4/punkweb_bb/templatetags/__init__.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.064355 punkweb_bb-0.1.4/punkweb_bb/templatetags/__pycache__/
+-rw-r--r--   0 pork      (1000) pork      (1000)      174 2024-05-07 04:31:10.000000 punkweb_bb-0.1.4/punkweb_bb/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      621 2024-05-07 04:30:58.000000 punkweb_bb-0.1.4/punkweb_bb/templatetags/__pycache__/humanize_count.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      619 2024-05-07 04:31:10.000000 punkweb_bb-0.1.4/punkweb_bb/templatetags/__pycache__/humanize_int.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      833 2024-04-09 07:07:10.000000 punkweb_bb-0.1.4/punkweb_bb/templatetags/__pycache__/shoutbox_bbcode.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      248 2024-05-07 04:31:08.000000 punkweb_bb-0.1.4/punkweb_bb/templatetags/humanize_int.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      310 2024-04-09 07:07:08.000000 punkweb_bb-0.1.4/punkweb_bb/templatetags/shoutbox_bbcode.py
+-rw-r--r--   0 pork      (1000) pork      (1000)    26368 2024-05-09 05:54:51.000000 punkweb_bb-0.1.4/punkweb_bb/tests.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     1538 2024-04-08 22:43:34.000000 punkweb_bb-0.1.4/punkweb_bb/urls.py
+-rw-r--r--   0 pork      (1000) pork      (1000)    11036 2024-05-09 05:54:18.000000 punkweb_bb-0.1.4/punkweb_bb/views.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      840 2024-04-03 19:20:08.000000 punkweb_bb-0.1.4/punkweb_bb/widgets.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.048355 punkweb_bb-0.1.4/punkweb_bb.egg-info/
+-rw-r--r--   0 pork      (1000) pork      (1000)     4992 2024-05-09 06:04:30.000000 punkweb_bb-0.1.4/punkweb_bb.egg-info/PKG-INFO
+-rw-r--r--   0 pork      (1000) pork      (1000)    13413 2024-05-09 06:04:30.000000 punkweb_bb-0.1.4/punkweb_bb.egg-info/SOURCES.txt
+-rw-r--r--   0 pork      (1000) pork      (1000)        1 2024-05-09 06:04:30.000000 punkweb_bb-0.1.4/punkweb_bb.egg-info/dependency_links.txt
+-rw-r--r--   0 pork      (1000) pork      (1000)        1 2024-04-09 07:09:59.000000 punkweb_bb-0.1.4/punkweb_bb.egg-info/not-zip-safe
+-rw-r--r--   0 pork      (1000) pork      (1000)       54 2024-05-09 06:04:30.000000 punkweb_bb-0.1.4/punkweb_bb.egg-info/requires.txt
+-rw-r--r--   0 pork      (1000) pork      (1000)       11 2024-05-09 06:04:30.000000 punkweb_bb-0.1.4/punkweb_bb.egg-info/top_level.txt
+-rw-r--r--   0 pork      (1000) pork      (1000)       38 2024-05-09 06:04:30.064355 punkweb_bb-0.1.4/setup.cfg
+-rw-r--r--   0 pork      (1000) pork      (1000)     1010 2024-05-09 06:02:08.000000 punkweb_bb-0.1.4/setup.py
```

### Comparing `punkweb_bb-0.1.3/LICENSE` & `punkweb_bb-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/PKG-INFO` & `punkweb_bb-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: punkweb_bb
-Version: 0.1.3
+Version: 0.1.4
 Summary: Django application that provides a simple and modern forum board software for your Django website.
 Home-page: https://github.com/Punkweb/PunkwebBB
 Author: Punkweb
 Author-email: punkwebnet@gmail.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -108,14 +108,17 @@
 
 ```python
 PUNKWEB_BB = {
   "SITE_NAME": "PUNKWEB",
   "SITE_TITLE": "PunkwebBB",
   "FAVICON": "punkweb_bb/favicon.ico",
   "SHOUTBOX_ENABLED": True,
+  "DISCORD_WIDGET_ENABLED": False,
+  "DISCORD_WIDGET_THEME": "dark",
+  "DISCORD_SERVER_ID": None, # Found under Server Settings > Widget > Server ID
 }
 ```
 
 ## Testing
 
 Report:
```

### Comparing `punkweb_bb-0.1.3/README.md` & `punkweb_bb-0.1.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -90,14 +90,17 @@
 
 ```python
 PUNKWEB_BB = {
   "SITE_NAME": "PUNKWEB",
   "SITE_TITLE": "PunkwebBB",
   "FAVICON": "punkweb_bb/favicon.ico",
   "SHOUTBOX_ENABLED": True,
+  "DISCORD_WIDGET_ENABLED": False,
+  "DISCORD_WIDGET_THEME": "dark",
+  "DISCORD_SERVER_ID": None, # Found under Server Settings > Widget > Server ID
 }
 ```
 
 ## Testing
 
 Report:
```

### Comparing `punkweb_bb-0.1.3/punkweb_bb/__pycache__/admin.cpython-311.pyc` & `punkweb_bb-0.1.4/punkweb_bb/__pycache__/admin.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/__pycache__/admin_forms.cpython-311.pyc` & `punkweb_bb-0.1.4/punkweb_bb/__pycache__/admin_forms.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/__pycache__/apps.cpython-311.pyc` & `punkweb_bb-0.1.4/punkweb_bb/__pycache__/apps.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/__pycache__/bbcode_tags.cpython-311.pyc` & `punkweb_bb-0.1.4/punkweb_bb/__pycache__/bbcode_tags.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/__pycache__/forms.cpython-311.pyc` & `punkweb_bb-0.1.4/punkweb_bb/__pycache__/forms.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/__pycache__/middleware.cpython-311.pyc` & `punkweb_bb-0.1.4/punkweb_bb/__pycache__/middleware.cpython-311.pyc`

 * *Files 25% similar despite different names*

#### Python bytecode

```diff
@@ -1,18 +1,19 @@
 magic:    0xa70d0d0a
-moddate:  0x02691066 (Fri Apr  5 21:11:30 2024 UTC)
-files sz: 456
+moddate:  0x28613c66 (Thu May  9 05:37:44 2024 UTC)
+files sz: 628
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
-      0x9700640064016c006d015a010100640064026c026d035a030100020047
-      00640384006404a6020000ab0200000000000000005a0464055300
+      0x9700640064016c006d015a010100640064026c026d035a030100640064
+      036c046d055a05010002004700640484006405a6020000ab020000000000
+      0000005a0664065300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('cache',))
                  6 IMPORT_NAME              0 (django.core.cache)
                  8 IMPORT_FROM              1 (cache)
                 10 STORE_NAME               1 (cache)
@@ -21,147 +22,182 @@
      2          14 LOAD_CONST               0 (0)
                 16 LOAD_CONST               2 (('timezone',))
                 18 IMPORT_NAME              2 (django.utils)
                 20 IMPORT_FROM              3 (timezone)
                 22 STORE_NAME               3 (timezone)
                 24 POP_TOP
    
-     5          26 PUSH_NULL
-                28 LOAD_BUILD_CLASS
-                30 LOAD_CONST               3 (<code object ProfileOnlineCacheMiddleware, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/middleware.py", line 5>)
-                32 MAKE_FUNCTION            0
-                34 LOAD_CONST               4 ('ProfileOnlineCacheMiddleware')
-                36 PRECALL                  2
-                40 CALL                     2
-                50 STORE_NAME               4 (ProfileOnlineCacheMiddleware)
-                52 LOAD_CONST               5 (None)
-                54 RETURN_VALUE
+     4          26 LOAD_CONST               0 (0)
+                28 LOAD_CONST               3 (('guest_list',))
+                30 IMPORT_NAME              4 (punkweb_bb.guests)
+                32 IMPORT_FROM              5 (guest_list)
+                34 STORE_NAME               5 (guest_list)
+                36 POP_TOP
+   
+     7          38 PUSH_NULL
+                40 LOAD_BUILD_CLASS
+                42 LOAD_CONST               4 (<code object ProfileOnlineCacheMiddleware, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/middleware.py", line 7>)
+                44 MAKE_FUNCTION            0
+                46 LOAD_CONST               5 ('ProfileOnlineCacheMiddleware')
+                48 PRECALL                  2
+                52 CALL                     2
+                62 STORE_NAME               6 (ProfileOnlineCacheMiddleware)
+                64 LOAD_CONST               6 (None)
+                66 RETURN_VALUE
    consts
       0
       ('cache',)
       ('timezone',)
+      ('guest_list',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a03640284005a0464035300
-           5           0 RESUME                   0
+           7           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ProfileOnlineCacheMiddleware')
                        8 STORE_NAME               2 (__qualname__)
          
-           6          10 LOAD_CONST               1 (<code object __init__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/middleware.py", line 6>)
+           8          10 LOAD_CONST               1 (<code object __init__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/middleware.py", line 8>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (__init__)
          
-           9          16 LOAD_CONST               2 (<code object __call__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/middleware.py", line 9>)
+          11          16 LOAD_CONST               2 (<code object __call__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/middleware.py", line 11>)
                       18 MAKE_FUNCTION            0
                       20 STORE_NAME               4 (__call__)
                       22 LOAD_CONST               3 (None)
                       24 RETURN_VALUE
          consts
             'ProfileOnlineCacheMiddleware'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code 0x97007c017c005f00000000000000000064005300
-                 6           0 RESUME                   0
+                 8           0 RESUME                   0
                
-                 7           2 LOAD_FAST                1 (get_response)
+                 9           2 LOAD_FAST                1 (get_response)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (get_response)
                             16 LOAD_CONST               0 (None)
                             18 RETURN_VALUE
                consts
                   None
                names      ('get_response',)
                varnames   ('self', 'get_response')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/middleware.py'
                name       '__init__'
-               firstlineno 6
+               firstlineno 8
                lnotab 0x0201
             code
                argcount  : 2
-               nlocals   : 3
+               nlocals   : 4
                stacksize : 5
                flags     : 3
                code
-                  0x97007c016a0000000000000000006a0100000000000000007239740500
+                  0x97007c016a0000000000000000006a010000000000000000723a740500
                   0000000000000000006a03000000000000000064017c016a000000000000
                   0000006a0400000000000000006a0500000000000000009b009d02740d00
                   0000000000000000006a070000000000000000a6000000ab000000000000
-                  0000006402a6030000ab03000000000000000001007c00a0080000000000
-                  0000000000000000000000000000007c01a6010000ab0100000000000000
-                  007d027c025300
-                 9           0 RESUME                   0
+                  0000006402a6030000ab03000000000000000001006e2e7c016a08000000
+                  0000000000a00900000000000000000000000000000000000000006403a6
+                  010000ab0100000000000000007d027415000000000000000000006a0b00
+                  000000000000007c02a6010000ab01000000000000000001007415000000
+                  000000000000006a0c0000000000000000a6000000ab0000000000000000
+                  0001007c00a00d00000000000000000000000000000000000000007c01a6
+                  010000ab0100000000000000007d037c035300
+                11           0 RESUME                   0
                
-                10           2 LOAD_FAST                1 (request)
+                12           2 LOAD_FAST                1 (request)
                              4 LOAD_ATTR                0 (user)
                             14 LOAD_ATTR                1 (is_authenticated)
-                            24 POP_JUMP_FORWARD_IF_FALSE    57 (to 140)
+                            24 POP_JUMP_FORWARD_IF_FALSE    58 (to 142)
                
-                11          26 LOAD_GLOBAL              5 (NULL + cache)
+                13          26 LOAD_GLOBAL              5 (NULL + cache)
                             38 LOAD_ATTR                3 (set)
                
-                12          48 LOAD_CONST               1 ('profile_online_')
+                14          48 LOAD_CONST               1 ('profile_online_')
                             50 LOAD_FAST                1 (request)
                             52 LOAD_ATTR                0 (user)
                             62 LOAD_ATTR                4 (profile)
                             72 LOAD_ATTR                5 (id)
                             82 FORMAT_VALUE             0
                             84 BUILD_STRING             2
                             86 LOAD_GLOBAL             13 (NULL + timezone)
                             98 LOAD_ATTR                7 (now)
                            108 PRECALL                  0
                            112 CALL                     0
                            122 LOAD_CONST               2 (300)
                
-                11         124 PRECALL                  3
+                13         124 PRECALL                  3
                            128 CALL                     3
                            138 POP_TOP
+                           140 JUMP_FORWARD            46 (to 234)
                
-                15     >>  140 LOAD_FAST                0 (self)
-                           142 LOAD_METHOD              8 (get_response)
-                           164 LOAD_FAST                1 (request)
-                           166 PRECALL                  1
-                           170 CALL                     1
-                           180 STORE_FAST               2 (response)
+                17     >>  142 LOAD_FAST                1 (request)
+                           144 LOAD_ATTR                8 (META)
+                           154 LOAD_METHOD              9 (get)
+                           176 LOAD_CONST               3 ('REMOTE_ADDR')
+                           178 PRECALL                  1
+                           182 CALL                     1
+                           192 STORE_FAST               2 (ip)
+               
+                18         194 LOAD_GLOBAL             21 (NULL + guest_list)
+                           206 LOAD_ATTR               11 (add)
+                           216 LOAD_FAST                2 (ip)
+                           218 PRECALL                  1
+                           222 CALL                     1
+                           232 POP_TOP
+               
+                20     >>  234 LOAD_GLOBAL             21 (NULL + guest_list)
+                           246 LOAD_ATTR               12 (clear_expired)
+                           256 PRECALL                  0
+                           260 CALL                     0
+                           270 POP_TOP
+               
+                22         272 LOAD_FAST                0 (self)
+                           274 LOAD_METHOD             13 (get_response)
+                           296 LOAD_FAST                1 (request)
+                           298 PRECALL                  1
+                           302 CALL                     1
+                           312 STORE_FAST               3 (response)
                
-                17         182 LOAD_FAST                2 (response)
-                           184 RETURN_VALUE
+                24         314 LOAD_FAST                3 (response)
+                           316 RETURN_VALUE
                consts
                   None
                   'profile_online_'
                   300
-               names      ('user', 'is_authenticated', 'cache', 'set', 'profile', 'id', 'timezone', 'now', 'get_response')
-               varnames   ('self', 'request', 'response')
+                  'REMOTE_ADDR'
+               names      ('user', 'is_authenticated', 'cache', 'set', 'profile', 'id', 'timezone', 'now', 'META', 'get', 'guest_list', 'add', 'clear_expired', 'get_response')
+               varnames   ('self', 'request', 'ip', 'response')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/middleware.py'
                name       '__call__'
-               firstlineno 9
-               lnotab 0x0201180116014cff10042a02
+               firstlineno 11
+               lnotab 0x0201180116014cff12043401280226022a02
             None
          names      ('__name__', '__module__', '__qualname__', '__init__', '__call__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/middleware.py'
          name       'ProfileOnlineCacheMiddleware'
-         firstlineno 5
+         firstlineno 7
          lnotab 0x0a010603
       'ProfileOnlineCacheMiddleware'
       None
-   names      ('django.core.cache', 'cache', 'django.utils', 'timezone', 'ProfileOnlineCacheMiddleware')
+   names      ('django.core.cache', 'cache', 'django.utils', 'timezone', 'punkweb_bb.guests', 'guest_list', 'ProfileOnlineCacheMiddleware')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/middleware.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c010c03
+   lnotab 0x00ff02010c010c020c03
```

### Comparing `punkweb_bb-0.1.3/punkweb_bb/__pycache__/mixins.cpython-311.pyc` & `punkweb_bb-0.1.4/punkweb_bb/__pycache__/mixins.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/__pycache__/models.cpython-311.pyc` & `punkweb_bb-0.1.4/punkweb_bb/__pycache__/models.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/__pycache__/pagination.cpython-311.pyc` & `punkweb_bb-0.1.4/punkweb_bb/__pycache__/pagination.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/__pycache__/parsers.cpython-311.pyc` & `punkweb_bb-0.1.4/punkweb_bb/__pycache__/parsers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/__pycache__/signals.cpython-311.pyc` & `punkweb_bb-0.1.4/punkweb_bb/__pycache__/signals.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/__pycache__/tests.cpython-311.pyc` & `punkweb_bb-0.1.4/punkweb_bb/__pycache__/tests.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x62c63966 (Tue May  7 06:12:50 2024 UTC)
-files sz: 25989
+moddate:  0x2b653c66 (Thu May  9 05:54:51 2024 UTC)
+files sz: 26368
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a020100640064036c036d
@@ -188,127 +188,127 @@
                352 MAKE_FUNCTION            0
                354 LOAD_CONST              25 ('IndexViewTestCase')
                356 LOAD_NAME                9 (TestCase)
                358 PRECALL                  3
                362 CALL                     3
                372 STORE_NAME              31 (IndexViewTestCase)
    
-   329         374 PUSH_NULL
+   340         374 PUSH_NULL
                376 LOAD_BUILD_CLASS
-               378 LOAD_CONST              26 (<code object LoginViewTestCase, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 329>)
+               378 LOAD_CONST              26 (<code object LoginViewTestCase, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 340>)
                380 MAKE_FUNCTION            0
                382 LOAD_CONST              27 ('LoginViewTestCase')
                384 LOAD_NAME                9 (TestCase)
                386 PRECALL                  3
                390 CALL                     3
                400 STORE_NAME              32 (LoginViewTestCase)
    
-   350         402 PUSH_NULL
+   361         402 PUSH_NULL
                404 LOAD_BUILD_CLASS
-               406 LOAD_CONST              28 (<code object LogoutViewTestCase, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 350>)
+               406 LOAD_CONST              28 (<code object LogoutViewTestCase, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 361>)
                408 MAKE_FUNCTION            0
                410 LOAD_CONST              29 ('LogoutViewTestCase')
                412 LOAD_NAME                9 (TestCase)
                414 PRECALL                  3
                418 CALL                     3
                428 STORE_NAME              33 (LogoutViewTestCase)
    
-   364         430 PUSH_NULL
+   375         430 PUSH_NULL
                432 LOAD_BUILD_CLASS
-               434 LOAD_CONST              30 (<code object SignupViewTestCase, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 364>)
+               434 LOAD_CONST              30 (<code object SignupViewTestCase, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 375>)
                436 MAKE_FUNCTION            0
                438 LOAD_CONST              31 ('SignupViewTestCase')
                440 LOAD_NAME                9 (TestCase)
                442 PRECALL                  3
                446 CALL                     3
                456 STORE_NAME              34 (SignupViewTestCase)
    
-   389         458 PUSH_NULL
+   400         458 PUSH_NULL
                460 LOAD_BUILD_CLASS
-               462 LOAD_CONST              32 (<code object SettingsViewTestCase, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 389>)
+               462 LOAD_CONST              32 (<code object SettingsViewTestCase, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 400>)
                464 MAKE_FUNCTION            0
                466 LOAD_CONST              33 ('SettingsViewTestCase')
                468 LOAD_NAME                9 (TestCase)
                470 PRECALL                  3
                474 CALL                     3
                484 STORE_NAME              35 (SettingsViewTestCase)
    
-   419         486 PUSH_NULL
+   430         486 PUSH_NULL
                488 LOAD_BUILD_CLASS
-               490 LOAD_CONST              34 (<code object ThreadCreateViewTestCase, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 419>)
+               490 LOAD_CONST              34 (<code object ThreadCreateViewTestCase, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 430>)
                492 MAKE_FUNCTION            0
                494 LOAD_CONST              35 ('ThreadCreateViewTestCase')
                496 LOAD_NAME                9 (TestCase)
                498 PRECALL                  3
                502 CALL                     3
                512 STORE_NAME              36 (ThreadCreateViewTestCase)
    
-   469         514 PUSH_NULL
+   480         514 PUSH_NULL
                516 LOAD_BUILD_CLASS
-               518 LOAD_CONST              36 (<code object ThreadViewTestCase, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 469>)
+               518 LOAD_CONST              36 (<code object ThreadViewTestCase, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 480>)
                520 MAKE_FUNCTION            0
                522 LOAD_CONST              37 ('ThreadViewTestCase')
                524 LOAD_NAME                9 (TestCase)
                526 PRECALL                  3
                530 CALL                     3
                540 STORE_NAME              37 (ThreadViewTestCase)
    
-   492         542 PUSH_NULL
+   503         542 PUSH_NULL
                544 LOAD_BUILD_CLASS
-               546 LOAD_CONST              38 (<code object ThreadUpdateViewTestCase, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 492>)
+               546 LOAD_CONST              38 (<code object ThreadUpdateViewTestCase, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 503>)
                548 MAKE_FUNCTION            0
                550 LOAD_CONST              39 ('ThreadUpdateViewTestCase')
                552 LOAD_NAME                9 (TestCase)
                554 PRECALL                  3
                558 CALL                     3
                568 STORE_NAME              38 (ThreadUpdateViewTestCase)
    
-   541         570 PUSH_NULL
+   552         570 PUSH_NULL
                572 LOAD_BUILD_CLASS
-               574 LOAD_CONST              40 (<code object ThreadDeleteViewTestCase, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 541>)
+               574 LOAD_CONST              40 (<code object ThreadDeleteViewTestCase, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 552>)
                576 MAKE_FUNCTION            0
                578 LOAD_CONST              41 ('ThreadDeleteViewTestCase')
                580 LOAD_NAME                9 (TestCase)
                582 PRECALL                  3
                586 CALL                     3
                596 STORE_NAME              39 (ThreadDeleteViewTestCase)
    
-   583         598 PUSH_NULL
+   594         598 PUSH_NULL
                600 LOAD_BUILD_CLASS
-               602 LOAD_CONST              42 (<code object PostCreateViewTestCase, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 583>)
+               602 LOAD_CONST              42 (<code object PostCreateViewTestCase, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 594>)
                604 MAKE_FUNCTION            0
                606 LOAD_CONST              43 ('PostCreateViewTestCase')
                608 LOAD_NAME                9 (TestCase)
                610 PRECALL                  3
                614 CALL                     3
                624 STORE_NAME              40 (PostCreateViewTestCase)
    
-   620         626 PUSH_NULL
+   631         626 PUSH_NULL
                628 LOAD_BUILD_CLASS
-               630 LOAD_CONST              44 (<code object PostUpdateViewTestCase, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 620>)
+               630 LOAD_CONST              44 (<code object PostUpdateViewTestCase, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 631>)
                632 MAKE_FUNCTION            0
                634 LOAD_CONST              45 ('PostUpdateViewTestCase')
                636 LOAD_NAME                9 (TestCase)
                638 PRECALL                  3
                642 CALL                     3
                652 STORE_NAME              41 (PostUpdateViewTestCase)
    
-   670         654 PUSH_NULL
+   681         654 PUSH_NULL
                656 LOAD_BUILD_CLASS
-               658 LOAD_CONST              46 (<code object PostDeleteViewTestCase, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 670>)
+               658 LOAD_CONST              46 (<code object PostDeleteViewTestCase, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 681>)
                660 MAKE_FUNCTION            0
                662 LOAD_CONST              47 ('PostDeleteViewTestCase')
                664 LOAD_NAME                9 (TestCase)
                666 PRECALL                  3
                670 CALL                     3
                680 STORE_NAME              42 (PostDeleteViewTestCase)
    
-   715         682 PUSH_NULL
+   726         682 PUSH_NULL
                684 LOAD_BUILD_CLASS
-               686 LOAD_CONST              48 (<code object ShoutCreateViewTestCase, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 715>)
+               686 LOAD_CONST              48 (<code object ShoutCreateViewTestCase, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 726>)
                688 MAKE_FUNCTION            0
                690 LOAD_CONST              49 ('ShoutCreateViewTestCase')
                692 LOAD_NAME                9 (TestCase)
                694 PRECALL                  3
                698 CALL                     3
                708 STORE_NAME              43 (ShoutCreateViewTestCase)
                710 LOAD_CONST               1 (None)
@@ -2832,42 +2832,50 @@
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a02640184005a03640284005a04640384005a0564
-            0484005a06640584005a0764065300
+            0484005a06640584005a07640684005a08640784005a0964085300
          293           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('IndexViewTestCase')
                        8 STORE_NAME               2 (__qualname__)
          
          294          10 LOAD_CONST               1 (<code object setUp, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 294>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (setUp)
          
-         302          16 LOAD_CONST               2 (<code object test_users_online, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 302>)
+         302          16 LOAD_CONST               2 (<code object test_members_online, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 302>)
                       18 MAKE_FUNCTION            0
-                      20 STORE_NAME               4 (test_users_online)
+                      20 STORE_NAME               4 (test_members_online)
          
          311          22 LOAD_CONST               3 (<code object test_staff_online, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 311>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               5 (test_staff_online)
          
-         320          28 LOAD_CONST               4 (<code object test_newest_user, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 320>)
+         320          28 LOAD_CONST               4 (<code object test_guests_online, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 320>)
                       30 MAKE_FUNCTION            0
-                      32 STORE_NAME               6 (test_newest_user)
+                      32 STORE_NAME               6 (test_guests_online)
          
-         324          34 LOAD_CONST               5 (<code object test_users_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 324>)
+         324          34 LOAD_CONST               5 (<code object test_total_online, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 324>)
                       36 MAKE_FUNCTION            0
-                      38 STORE_NAME               7 (test_users_count)
-                      40 LOAD_CONST               6 (None)
-                      42 RETURN_VALUE
+                      38 STORE_NAME               7 (test_total_online)
+         
+         331          40 LOAD_CONST               6 (<code object test_newest_user, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 331>)
+                      42 MAKE_FUNCTION            0
+                      44 STORE_NAME               8 (test_newest_user)
+         
+         335          46 LOAD_CONST               7 (<code object test_users_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 335>)
+                      48 MAKE_FUNCTION            0
+                      50 STORE_NAME               9 (test_users_count)
+                      52 LOAD_CONST               8 (None)
+                      54 RETURN_VALUE
          consts
             'IndexViewTestCase'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 5
                flags     : 3
@@ -2968,15 +2976,15 @@
                             62 STORE_FAST               1 (response)
                
                304          64 LOAD_FAST                0 (self)
                             66 LOAD_METHOD              3 (assertEqual)
                             88 LOAD_GLOBAL              9 (NULL + len)
                            100 LOAD_FAST                1 (response)
                            102 LOAD_ATTR                5 (context)
-                           112 LOAD_CONST               1 ('users_online')
+                           112 LOAD_CONST               1 ('members_online')
                            114 BINARY_SUBSCR
                            124 PRECALL                  1
                            128 CALL                     1
                            138 LOAD_CONST               2 (0)
                            140 PRECALL                  2
                            144 CALL                     2
                            154 POP_TOP
@@ -3000,35 +3008,35 @@
                            278 STORE_FAST               1 (response)
                
                309         280 LOAD_FAST                0 (self)
                            282 LOAD_METHOD              3 (assertEqual)
                            304 LOAD_GLOBAL              9 (NULL + len)
                            316 LOAD_FAST                1 (response)
                            318 LOAD_ATTR                5 (context)
-                           328 LOAD_CONST               1 ('users_online')
+                           328 LOAD_CONST               1 ('members_online')
                            330 BINARY_SUBSCR
                            340 PRECALL                  1
                            344 CALL                     1
                            354 LOAD_CONST               3 (1)
                            356 PRECALL                  2
                            360 CALL                     2
                            370 POP_TOP
                            372 LOAD_CONST               0 (None)
                            374 RETURN_VALUE
                consts
                   None
-                  'users_online'
+                  'members_online'
                   0
                   1
                names      ('client', 'get', 'url', 'assertEqual', 'len', 'context', 'force_login', 'user')
                varnames   ('self', 'response')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
-               name       'test_users_online'
+               name       'test_members_online'
                firstlineno 302
                lnotab 0x02013e015c023e013e02
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 6
                flags     : 3
@@ -3122,16 +3130,16 @@
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c006a020000000000000000a6010000ab010000000000
                   0000007d017c00a00300000000000000000000000000000000000000007c
-                  016a0400000000000000006401190000000000000000007c006a05000000
-                  0000000000a6020000ab020000000000000000010064005300
+                  016a0400000000000000006401190000000000000000006402a6020000ab
+                  020000000000000000010064005300
                320           0 RESUME                   0
                
                321           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (client)
                             14 LOAD_METHOD              1 (get)
                             36 LOAD_FAST                0 (self)
                             38 LOAD_ATTR                2 (url)
@@ -3139,14 +3147,128 @@
                             52 CALL                     1
                             62 STORE_FAST               1 (response)
                
                322          64 LOAD_FAST                0 (self)
                             66 LOAD_METHOD              3 (assertEqual)
                             88 LOAD_FAST                1 (response)
                             90 LOAD_ATTR                4 (context)
+                           100 LOAD_CONST               1 ('guests_online')
+                           102 BINARY_SUBSCR
+                           112 LOAD_CONST               2 (1)
+                           114 PRECALL                  2
+                           118 CALL                     2
+                           128 POP_TOP
+                           130 LOAD_CONST               0 (None)
+                           132 RETURN_VALUE
+               consts
+                  None
+                  'guests_online'
+                  1
+               names      ('client', 'get', 'url', 'assertEqual', 'context')
+               varnames   ('self', 'response')
+               freevars   ()
+               cellvars   ()
+               filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
+               name       'test_guests_online'
+               firstlineno 320
+               lnotab 0x02013e01
+            code
+               argcount  : 1
+               nlocals   : 2
+               stacksize : 4
+               flags     : 3
+               code
+                  0x97007c006a000000000000000000a00100000000000000000000000000
+                  000000000000007c006a020000000000000000a6010000ab010000000000
+                  0000007d017c006a000000000000000000a0030000000000000000000000
+                  0000000000000000007c006a040000000000000000a6010000ab01000000
+                  000000000001007c006a000000000000000000a001000000000000000000
+                  00000000000000000000007c006a020000000000000000a6010000ab0100
+                  000000000000007d017c00a0050000000000000000000000000000000000
+                  0000007c016a0600000000000000006401190000000000000000006402a6
+                  020000ab020000000000000000010064005300
+               324           0 RESUME                   0
+               
+               325           2 LOAD_FAST                0 (self)
+                             4 LOAD_ATTR                0 (client)
+                            14 LOAD_METHOD              1 (get)
+                            36 LOAD_FAST                0 (self)
+                            38 LOAD_ATTR                2 (url)
+                            48 PRECALL                  1
+                            52 CALL                     1
+                            62 STORE_FAST               1 (response)
+               
+               326          64 LOAD_FAST                0 (self)
+                            66 LOAD_ATTR                0 (client)
+                            76 LOAD_METHOD              3 (force_login)
+                            98 LOAD_FAST                0 (self)
+                           100 LOAD_ATTR                4 (user)
+                           110 PRECALL                  1
+                           114 CALL                     1
+                           124 POP_TOP
+               
+               327         126 LOAD_FAST                0 (self)
+                           128 LOAD_ATTR                0 (client)
+                           138 LOAD_METHOD              1 (get)
+                           160 LOAD_FAST                0 (self)
+                           162 LOAD_ATTR                2 (url)
+                           172 PRECALL                  1
+                           176 CALL                     1
+                           186 STORE_FAST               1 (response)
+               
+               329         188 LOAD_FAST                0 (self)
+                           190 LOAD_METHOD              5 (assertEqual)
+                           212 LOAD_FAST                1 (response)
+                           214 LOAD_ATTR                6 (context)
+                           224 LOAD_CONST               1 ('total_online')
+                           226 BINARY_SUBSCR
+                           236 LOAD_CONST               2 (2)
+                           238 PRECALL                  2
+                           242 CALL                     2
+                           252 POP_TOP
+                           254 LOAD_CONST               0 (None)
+                           256 RETURN_VALUE
+               consts
+                  None
+                  'total_online'
+                  2
+               names      ('client', 'get', 'url', 'force_login', 'user', 'assertEqual', 'context')
+               varnames   ('self', 'response')
+               freevars   ()
+               cellvars   ()
+               filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
+               name       'test_total_online'
+               firstlineno 324
+               lnotab 0x02013e013e013e02
+            code
+               argcount  : 1
+               nlocals   : 2
+               stacksize : 4
+               flags     : 3
+               code
+                  0x97007c006a000000000000000000a00100000000000000000000000000
+                  000000000000007c006a020000000000000000a6010000ab010000000000
+                  0000007d017c00a00300000000000000000000000000000000000000007c
+                  016a0400000000000000006401190000000000000000007c006a05000000
+                  0000000000a6020000ab020000000000000000010064005300
+               331           0 RESUME                   0
+               
+               332           2 LOAD_FAST                0 (self)
+                             4 LOAD_ATTR                0 (client)
+                            14 LOAD_METHOD              1 (get)
+                            36 LOAD_FAST                0 (self)
+                            38 LOAD_ATTR                2 (url)
+                            48 PRECALL                  1
+                            52 CALL                     1
+                            62 STORE_FAST               1 (response)
+               
+               333          64 LOAD_FAST                0 (self)
+                            66 LOAD_METHOD              3 (assertEqual)
+                            88 LOAD_FAST                1 (response)
+                            90 LOAD_ATTR                4 (context)
                            100 LOAD_CONST               1 ('newest_user')
                            102 BINARY_SUBSCR
                            112 LOAD_FAST                0 (self)
                            114 LOAD_ATTR                5 (staff_user)
                            124 PRECALL                  2
                            128 CALL                     2
                            138 POP_TOP
@@ -3157,40 +3279,40 @@
                   'newest_user'
                names      ('client', 'get', 'url', 'assertEqual', 'context', 'staff_user')
                varnames   ('self', 'response')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'test_newest_user'
-               firstlineno 320
+               firstlineno 331
                lnotab 0x02013e01
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c006a020000000000000000a6010000ab010000000000
                   0000007d017c00a00300000000000000000000000000000000000000007c
                   016a040000000000000000640119000000000000000000a0050000000000
                   000000000000000000000000000000a6000000ab00000000000000000064
                   02a6020000ab020000000000000000010064005300
-               324           0 RESUME                   0
+               335           0 RESUME                   0
                
-               325           2 LOAD_FAST                0 (self)
+               336           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (client)
                             14 LOAD_METHOD              1 (get)
                             36 LOAD_FAST                0 (self)
                             38 LOAD_ATTR                2 (url)
                             48 PRECALL                  1
                             52 CALL                     1
                             62 STORE_FAST               1 (response)
                
-               326          64 LOAD_FAST                0 (self)
+               337          64 LOAD_FAST                0 (self)
                             66 LOAD_METHOD              3 (assertEqual)
                             88 LOAD_FAST                1 (response)
                             90 LOAD_ATTR                4 (context)
                            100 LOAD_CONST               1 ('users')
                            102 BINARY_SUBSCR
                            112 LOAD_METHOD              5 (count)
                            134 PRECALL                  0
@@ -3207,49 +3329,49 @@
                   2
                names      ('client', 'get', 'url', 'assertEqual', 'context', 'count')
                varnames   ('self', 'response')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'test_users_count'
-               firstlineno 324
+               firstlineno 335
                lnotab 0x02013e01
             None
-         names      ('__name__', '__module__', '__qualname__', 'setUp', 'test_users_online', 'test_staff_online', 'test_newest_user', 'test_users_count')
+         names      ('__name__', '__module__', '__qualname__', 'setUp', 'test_members_online', 'test_staff_online', 'test_guests_online', 'test_total_online', 'test_newest_user', 'test_users_count')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
          name       'IndexViewTestCase'
          firstlineno 293
-         lnotab 0x0a010608060906090604
+         lnotab 0x0a01060806090609060406070604
       'IndexViewTestCase'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a02640184005a03640284005a04640384005a0564
             045300
-         329           0 RESUME                   0
+         340           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('LoginViewTestCase')
                        8 STORE_NAME               2 (__qualname__)
          
-         330          10 LOAD_CONST               1 (<code object setUp, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 330>)
+         341          10 LOAD_CONST               1 (<code object setUp, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 341>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (setUp)
          
-         335          16 LOAD_CONST               2 (<code object test_redirect_authenticated_user, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 335>)
+         346          16 LOAD_CONST               2 (<code object test_redirect_authenticated_user, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 346>)
                       18 MAKE_FUNCTION            0
                       20 STORE_NAME               4 (test_redirect_authenticated_user)
          
-         341          22 LOAD_CONST               3 (<code object test_login, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 341>)
+         352          22 LOAD_CONST               3 (<code object test_login, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 352>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               5 (test_login)
                       28 LOAD_CONST               4 (None)
                       30 RETURN_VALUE
          consts
             'LoginViewTestCase'
             code
@@ -3260,30 +3382,30 @@
                code
                   0x9700740100000000000000000000a6000000ab0000000000000000007c
                   005f0100000000000000007405000000000000000000006401a6010000ab
                   0100000000000000007c005f030000000000000000740800000000000000
                   0000006a050000000000000000a006000000000000000000000000000000
                   000000000064026402ac03a6020000ab0200000000000000007c005f0700
                   0000000000000064005300
-               330           0 RESUME                   0
+               341           0 RESUME                   0
                
-               331           2 LOAD_GLOBAL              1 (NULL + Client)
+               342           2 LOAD_GLOBAL              1 (NULL + Client)
                             14 PRECALL                  0
                             18 CALL                     0
                             28 LOAD_FAST                0 (self)
                             30 STORE_ATTR               1 (client)
                
-               332          40 LOAD_GLOBAL              5 (NULL + reverse)
+               343          40 LOAD_GLOBAL              5 (NULL + reverse)
                             52 LOAD_CONST               1 ('punkweb_bb:login')
                             54 PRECALL                  1
                             58 CALL                     1
                             68 LOAD_FAST                0 (self)
                             70 STORE_ATTR               3 (url)
                
-               333          80 LOAD_GLOBAL              8 (User)
+               344          80 LOAD_GLOBAL              8 (User)
                             92 LOAD_ATTR                5 (objects)
                            102 LOAD_METHOD              6 (create_user)
                            124 LOAD_CONST               2 ('test')
                            126 LOAD_CONST               2 ('test')
                            128 KW_NAMES                 3
                            130 PRECALL                  2
                            134 CALL                     2
@@ -3298,50 +3420,50 @@
                   ('username', 'password')
                names      ('Client', 'client', 'reverse', 'url', 'User', 'objects', 'create_user', 'user')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'setUp'
-               firstlineno 330
+               firstlineno 341
                lnotab 0x020126012801
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 6
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c006a020000000000000000a6010000ab010000000000
                   00000001007c006a000000000000000000a0030000000000000000000000
                   0000000000000000007c006a040000000000000000a6010000ab01000000
                   00000000007d017c00a00500000000000000000000000000000000000000
                   007c01740d000000000000000000006401a6010000ab0100000000000000
                   00a6020000ab020000000000000000010064005300
-               335           0 RESUME                   0
+               346           0 RESUME                   0
                
-               336           2 LOAD_FAST                0 (self)
+               347           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (client)
                             14 LOAD_METHOD              1 (force_login)
                             36 LOAD_FAST                0 (self)
                             38 LOAD_ATTR                2 (user)
                             48 PRECALL                  1
                             52 CALL                     1
                             62 POP_TOP
                
-               337          64 LOAD_FAST                0 (self)
+               348          64 LOAD_FAST                0 (self)
                             66 LOAD_ATTR                0 (client)
                             76 LOAD_METHOD              3 (get)
                             98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                4 (url)
                            110 PRECALL                  1
                            114 CALL                     1
                            124 STORE_FAST               1 (response)
                
-               339         126 LOAD_FAST                0 (self)
+               350         126 LOAD_FAST                0 (self)
                            128 LOAD_METHOD              5 (assertRedirects)
                            150 LOAD_FAST                1 (response)
                            152 LOAD_GLOBAL             13 (NULL + reverse)
                            164 LOAD_CONST               1 ('punkweb_bb:index')
                            166 PRECALL                  1
                            170 CALL                     1
                            180 PRECALL                  2
@@ -3354,15 +3476,15 @@
                   'punkweb_bb:index'
                names      ('client', 'force_login', 'user', 'get', 'url', 'assertRedirects', 'reverse')
                varnames   ('self', 'response')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'test_redirect_authenticated_user'
-               firstlineno 335
+               firstlineno 346
                lnotab 0x02013e013e02
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 6
                flags     : 3
                code
@@ -3370,45 +3492,45 @@
                   000000000000007c006a0200000000000000006401640164029c026403ac
                   04a6030000ab0300000000000000007d017c00a003000000000000000000
                   00000000000000000000007c017409000000000000000000006405a60100
                   00ab010000000000000000a6020000ab02000000000000000001007c00a0
                   0500000000000000000000000000000000000000007c016a060000000000
                   0000006406190000000000000000006a070000000000000000a6010000ab
                   010000000000000000010064005300
-               341           0 RESUME                   0
+               352           0 RESUME                   0
                
-               342           2 LOAD_FAST                0 (self)
+               353           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (client)
                             14 LOAD_METHOD              1 (post)
                
-               343          36 LOAD_FAST                0 (self)
+               354          36 LOAD_FAST                0 (self)
                             38 LOAD_ATTR                2 (url)
                             48 LOAD_CONST               1 ('test')
                             50 LOAD_CONST               1 ('test')
                             52 LOAD_CONST               2 (('username', 'password'))
                             54 BUILD_CONST_KEY_MAP      2
                             56 LOAD_CONST               3 (True)
                
-               342          58 KW_NAMES                 4
+               353          58 KW_NAMES                 4
                             60 PRECALL                  3
                             64 CALL                     3
                             74 STORE_FAST               1 (response)
                
-               346          76 LOAD_FAST                0 (self)
+               357          76 LOAD_FAST                0 (self)
                             78 LOAD_METHOD              3 (assertRedirects)
                            100 LOAD_FAST                1 (response)
                            102 LOAD_GLOBAL              9 (NULL + reverse)
                            114 LOAD_CONST               5 ('punkweb_bb:index')
                            116 PRECALL                  1
                            120 CALL                     1
                            130 PRECALL                  2
                            134 CALL                     2
                            144 POP_TOP
                
-               347         146 LOAD_FAST                0 (self)
+               358         146 LOAD_FAST                0 (self)
                            148 LOAD_METHOD              5 (assertTrue)
                            170 LOAD_FAST                1 (response)
                            172 LOAD_ATTR                6 (context)
                            182 LOAD_CONST               6 ('user')
                            184 BINARY_SUBSCR
                            194 LOAD_ATTR                7 (is_authenticated)
                            204 PRECALL                  1
@@ -3426,43 +3548,43 @@
                   'user'
                names      ('client', 'post', 'url', 'assertRedirects', 'reverse', 'assertTrue', 'context', 'is_authenticated')
                varnames   ('self', 'response')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'test_login'
-               firstlineno 341
+               firstlineno 352
                lnotab 0x0201220116ff12044601
             None
          names      ('__name__', '__module__', '__qualname__', 'setUp', 'test_redirect_authenticated_user', 'test_login')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
          name       'LoginViewTestCase'
-         firstlineno 329
+         firstlineno 340
          lnotab 0x0a0106050606
       'LoginViewTestCase'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a03640284005a0464035300
-         350           0 RESUME                   0
+         361           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('LogoutViewTestCase')
                        8 STORE_NAME               2 (__qualname__)
          
-         351          10 LOAD_CONST               1 (<code object setUp, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 351>)
+         362          10 LOAD_CONST               1 (<code object setUp, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 362>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (setUp)
          
-         356          16 LOAD_CONST               2 (<code object test_logout, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 356>)
+         367          16 LOAD_CONST               2 (<code object test_logout, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 367>)
                       18 MAKE_FUNCTION            0
                       20 STORE_NAME               4 (test_logout)
                       22 LOAD_CONST               3 (None)
                       24 RETURN_VALUE
          consts
             'LogoutViewTestCase'
             code
@@ -3473,30 +3595,30 @@
                code
                   0x9700740100000000000000000000a6000000ab0000000000000000007c
                   005f0100000000000000007405000000000000000000006401a6010000ab
                   0100000000000000007c005f030000000000000000740800000000000000
                   0000006a050000000000000000a006000000000000000000000000000000
                   000000000064026402ac03a6020000ab0200000000000000007c005f0700
                   0000000000000064005300
-               351           0 RESUME                   0
+               362           0 RESUME                   0
                
-               352           2 LOAD_GLOBAL              1 (NULL + Client)
+               363           2 LOAD_GLOBAL              1 (NULL + Client)
                             14 PRECALL                  0
                             18 CALL                     0
                             28 LOAD_FAST                0 (self)
                             30 STORE_ATTR               1 (client)
                
-               353          40 LOAD_GLOBAL              5 (NULL + reverse)
+               364          40 LOAD_GLOBAL              5 (NULL + reverse)
                             52 LOAD_CONST               1 ('punkweb_bb:logout')
                             54 PRECALL                  1
                             58 CALL                     1
                             68 LOAD_FAST                0 (self)
                             70 STORE_ATTR               3 (url)
                
-               354          80 LOAD_GLOBAL              8 (User)
+               365          80 LOAD_GLOBAL              8 (User)
                             92 LOAD_ATTR                5 (objects)
                            102 LOAD_METHOD              6 (create_user)
                            124 LOAD_CONST               2 ('test')
                            126 LOAD_CONST               2 ('test')
                            128 KW_NAMES                 3
                            130 PRECALL                  2
                            134 CALL                     2
@@ -3511,15 +3633,15 @@
                   ('username', 'password')
                names      ('Client', 'client', 'reverse', 'url', 'User', 'objects', 'create_user', 'user')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'setUp'
-               firstlineno 351
+               firstlineno 362
                lnotab 0x020126012801
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 6
                flags     : 3
                code
@@ -3529,48 +3651,48 @@
                   0000000000000000007c006a0400000000000000006401ac02a6020000ab
                   0200000000000000007d017c00a005000000000000000000000000000000
                   00000000007c01740d000000000000000000006403a6010000ab01000000
                   0000000000a6020000ab02000000000000000001007c00a0070000000000
                   0000000000000000000000000000007c016a080000000000000000640419
                   0000000000000000006a090000000000000000a6010000ab010000000000
                   000000010064005300
-               356           0 RESUME                   0
+               367           0 RESUME                   0
                
-               357           2 LOAD_FAST                0 (self)
+               368           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (client)
                             14 LOAD_METHOD              1 (force_login)
                             36 LOAD_FAST                0 (self)
                             38 LOAD_ATTR                2 (user)
                             48 PRECALL                  1
                             52 CALL                     1
                             62 POP_TOP
                
-               358          64 LOAD_FAST                0 (self)
+               369          64 LOAD_FAST                0 (self)
                             66 LOAD_ATTR                0 (client)
                             76 LOAD_METHOD              3 (get)
                             98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                4 (url)
                            110 LOAD_CONST               1 (True)
                            112 KW_NAMES                 2
                            114 PRECALL                  2
                            118 CALL                     2
                            128 STORE_FAST               1 (response)
                
-               360         130 LOAD_FAST                0 (self)
+               371         130 LOAD_FAST                0 (self)
                            132 LOAD_METHOD              5 (assertRedirects)
                            154 LOAD_FAST                1 (response)
                            156 LOAD_GLOBAL             13 (NULL + reverse)
                            168 LOAD_CONST               3 ('punkweb_bb:login')
                            170 PRECALL                  1
                            174 CALL                     1
                            184 PRECALL                  2
                            188 CALL                     2
                            198 POP_TOP
                
-               361         200 LOAD_FAST                0 (self)
+               372         200 LOAD_FAST                0 (self)
                            202 LOAD_METHOD              7 (assertFalse)
                            224 LOAD_FAST                1 (response)
                            226 LOAD_ATTR                8 (context)
                            236 LOAD_CONST               4 ('user')
                            238 BINARY_SUBSCR
                            248 LOAD_ATTR                9 (is_authenticated)
                            258 PRECALL                  1
@@ -3586,49 +3708,49 @@
                   'user'
                names      ('client', 'force_login', 'user', 'get', 'url', 'assertRedirects', 'reverse', 'assertFalse', 'context', 'is_authenticated')
                varnames   ('self', 'response')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'test_logout'
-               firstlineno 356
+               firstlineno 367
                lnotab 0x02013e0142024601
             None
          names      ('__name__', '__module__', '__qualname__', 'setUp', 'test_logout')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
          name       'LogoutViewTestCase'
-         firstlineno 350
+         firstlineno 361
          lnotab 0x0a010605
       'LogoutViewTestCase'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a02640184005a03640284005a04640384005a0564
             045300
-         364           0 RESUME                   0
+         375           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('SignupViewTestCase')
                        8 STORE_NAME               2 (__qualname__)
          
-         365          10 LOAD_CONST               1 (<code object setUp, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 365>)
+         376          10 LOAD_CONST               1 (<code object setUp, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 376>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (setUp)
          
-         370          16 LOAD_CONST               2 (<code object test_redirect_authenticated_user, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 370>)
+         381          16 LOAD_CONST               2 (<code object test_redirect_authenticated_user, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 381>)
                       18 MAKE_FUNCTION            0
                       20 STORE_NAME               4 (test_redirect_authenticated_user)
          
-         376          22 LOAD_CONST               3 (<code object test_signup, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 376>)
+         387          22 LOAD_CONST               3 (<code object test_signup, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 387>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               5 (test_signup)
                       28 LOAD_CONST               4 (None)
                       30 RETURN_VALUE
          consts
             'SignupViewTestCase'
             code
@@ -3639,30 +3761,30 @@
                code
                   0x9700740100000000000000000000a6000000ab0000000000000000007c
                   005f0100000000000000007405000000000000000000006401a6010000ab
                   0100000000000000007c005f030000000000000000740800000000000000
                   0000006a050000000000000000a006000000000000000000000000000000
                   000000000064026403ac04a6020000ab0200000000000000007c005f0700
                   0000000000000064005300
-               365           0 RESUME                   0
+               376           0 RESUME                   0
                
-               366           2 LOAD_GLOBAL              1 (NULL + Client)
+               377           2 LOAD_GLOBAL              1 (NULL + Client)
                             14 PRECALL                  0
                             18 CALL                     0
                             28 LOAD_FAST                0 (self)
                             30 STORE_ATTR               1 (client)
                
-               367          40 LOAD_GLOBAL              5 (NULL + reverse)
+               378          40 LOAD_GLOBAL              5 (NULL + reverse)
                             52 LOAD_CONST               1 ('punkweb_bb:signup')
                             54 PRECALL                  1
                             58 CALL                     1
                             68 LOAD_FAST                0 (self)
                             70 STORE_ATTR               3 (url)
                
-               368          80 LOAD_GLOBAL              8 (User)
+               379          80 LOAD_GLOBAL              8 (User)
                             92 LOAD_ATTR                5 (objects)
                            102 LOAD_METHOD              6 (create_user)
                            124 LOAD_CONST               2 ('test1')
                            126 LOAD_CONST               3 ('test')
                            128 KW_NAMES                 4
                            130 PRECALL                  2
                            134 CALL                     2
@@ -3678,50 +3800,50 @@
                   ('username', 'password')
                names      ('Client', 'client', 'reverse', 'url', 'User', 'objects', 'create_user', 'user')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'setUp'
-               firstlineno 365
+               firstlineno 376
                lnotab 0x020126012801
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 6
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c006a020000000000000000a6010000ab010000000000
                   00000001007c006a000000000000000000a0030000000000000000000000
                   0000000000000000007c006a040000000000000000a6010000ab01000000
                   00000000007d017c00a00500000000000000000000000000000000000000
                   007c01740d000000000000000000006401a6010000ab0100000000000000
                   00a6020000ab020000000000000000010064005300
-               370           0 RESUME                   0
+               381           0 RESUME                   0
                
-               371           2 LOAD_FAST                0 (self)
+               382           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (client)
                             14 LOAD_METHOD              1 (force_login)
                             36 LOAD_FAST                0 (self)
                             38 LOAD_ATTR                2 (user)
                             48 PRECALL                  1
                             52 CALL                     1
                             62 POP_TOP
                
-               372          64 LOAD_FAST                0 (self)
+               383          64 LOAD_FAST                0 (self)
                             66 LOAD_ATTR                0 (client)
                             76 LOAD_METHOD              3 (get)
                             98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                4 (url)
                            110 PRECALL                  1
                            114 CALL                     1
                            124 STORE_FAST               1 (response)
                
-               374         126 LOAD_FAST                0 (self)
+               385         126 LOAD_FAST                0 (self)
                            128 LOAD_METHOD              5 (assertRedirects)
                            150 LOAD_FAST                1 (response)
                            152 LOAD_GLOBAL             13 (NULL + reverse)
                            164 LOAD_CONST               1 ('punkweb_bb:index')
                            166 PRECALL                  1
                            170 CALL                     1
                            180 PRECALL                  2
@@ -3734,50 +3856,50 @@
                   'punkweb_bb:index'
                names      ('client', 'force_login', 'user', 'get', 'url', 'assertRedirects', 'reverse')
                varnames   ('self', 'response')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'test_redirect_authenticated_user'
-               firstlineno 370
+               firstlineno 381
                lnotab 0x02013e013e02
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 7
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c006a02000000000000000064016402640264039c03a6
                   020000ab0200000000000000007d017c00a0030000000000000000000000
                   0000000000000000007c017409000000000000000000006404a6010000ab
                   010000000000000000a6020000ab020000000000000000010064005300
-               376           0 RESUME                   0
+               387           0 RESUME                   0
                
-               377           2 LOAD_FAST                0 (self)
+               388           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (client)
                             14 LOAD_METHOD              1 (post)
                
-               378          36 LOAD_FAST                0 (self)
+               389          36 LOAD_FAST                0 (self)
                             38 LOAD_ATTR                2 (url)
                
-               380          48 LOAD_CONST               1 ('test2')
+               391          48 LOAD_CONST               1 ('test2')
                
-               381          50 LOAD_CONST               2 ('needsmorecomplexity')
+               392          50 LOAD_CONST               2 ('needsmorecomplexity')
                
-               382          52 LOAD_CONST               2 ('needsmorecomplexity')
+               393          52 LOAD_CONST               2 ('needsmorecomplexity')
                
-               379          54 LOAD_CONST               3 (('username', 'password1', 'password2'))
+               390          54 LOAD_CONST               3 (('username', 'password1', 'password2'))
                             56 BUILD_CONST_KEY_MAP      3
                
-               377          58 PRECALL                  2
+               388          58 PRECALL                  2
                             62 CALL                     2
                             72 STORE_FAST               1 (response)
                
-               386          74 LOAD_FAST                0 (self)
+               397          74 LOAD_FAST                0 (self)
                             76 LOAD_METHOD              3 (assertRedirects)
                             98 LOAD_FAST                1 (response)
                            100 LOAD_GLOBAL              9 (NULL + reverse)
                            112 LOAD_CONST               4 ('punkweb_bb:login')
                            114 PRECALL                  1
                            118 CALL                     1
                            128 PRECALL                  2
@@ -3793,49 +3915,49 @@
                   'punkweb_bb:login'
                names      ('client', 'post', 'url', 'assertRedirects', 'reverse')
                varnames   ('self', 'response')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'test_signup'
-               firstlineno 376
+               firstlineno 387
                lnotab 0x020122010c020201020102fd04fe1009
             None
          names      ('__name__', '__module__', '__qualname__', 'setUp', 'test_redirect_authenticated_user', 'test_signup')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
          name       'SignupViewTestCase'
-         firstlineno 364
+         firstlineno 375
          lnotab 0x0a0106050606
       'SignupViewTestCase'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a02640184005a03640284005a04640384005a0564
             045300
-         389           0 RESUME                   0
+         400           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('SettingsViewTestCase')
                        8 STORE_NAME               2 (__qualname__)
          
-         390          10 LOAD_CONST               1 (<code object setUp, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 390>)
+         401          10 LOAD_CONST               1 (<code object setUp, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 401>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (setUp)
          
-         395          16 LOAD_CONST               2 (<code object test_redirect_unauthenticated_user, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 395>)
+         406          16 LOAD_CONST               2 (<code object test_redirect_unauthenticated_user, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 406>)
                       18 MAKE_FUNCTION            0
                       20 STORE_NAME               4 (test_redirect_unauthenticated_user)
          
-         400          22 LOAD_CONST               3 (<code object test_settings, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 400>)
+         411          22 LOAD_CONST               3 (<code object test_settings, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 411>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               5 (test_settings)
                       28 LOAD_CONST               4 (None)
                       30 RETURN_VALUE
          consts
             'SettingsViewTestCase'
             code
@@ -3846,30 +3968,30 @@
                code
                   0x9700740100000000000000000000a6000000ab0000000000000000007c
                   005f0100000000000000007405000000000000000000006401a6010000ab
                   0100000000000000007c005f030000000000000000740800000000000000
                   0000006a050000000000000000a006000000000000000000000000000000
                   000000000064026402ac03a6020000ab0200000000000000007c005f0700
                   0000000000000064005300
-               390           0 RESUME                   0
+               401           0 RESUME                   0
                
-               391           2 LOAD_GLOBAL              1 (NULL + Client)
+               402           2 LOAD_GLOBAL              1 (NULL + Client)
                             14 PRECALL                  0
                             18 CALL                     0
                             28 LOAD_FAST                0 (self)
                             30 STORE_ATTR               1 (client)
                
-               392          40 LOAD_GLOBAL              5 (NULL + reverse)
+               403          40 LOAD_GLOBAL              5 (NULL + reverse)
                             52 LOAD_CONST               1 ('punkweb_bb:settings')
                             54 PRECALL                  1
                             58 CALL                     1
                             68 LOAD_FAST                0 (self)
                             70 STORE_ATTR               3 (url)
                
-               393          80 LOAD_GLOBAL              8 (User)
+               404          80 LOAD_GLOBAL              8 (User)
                             92 LOAD_ATTR                5 (objects)
                            102 LOAD_METHOD              6 (create_user)
                            124 LOAD_CONST               2 ('test')
                            126 LOAD_CONST               2 ('test')
                            128 KW_NAMES                 3
                            130 PRECALL                  2
                            134 CALL                     2
@@ -3884,40 +4006,40 @@
                   ('username', 'password')
                names      ('Client', 'client', 'reverse', 'url', 'User', 'objects', 'create_user', 'user')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'setUp'
-               firstlineno 390
+               firstlineno 401
                lnotab 0x020126012801
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 6
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c006a020000000000000000a6010000ab010000000000
                   0000007d017c00a00300000000000000000000000000000000000000007c
                   017409000000000000000000006401a6010000ab0100000000000000009b
                   0064027c006a0200000000000000009b009d03a6020000ab020000000000
                   000000010064005300
-               395           0 RESUME                   0
+               406           0 RESUME                   0
                
-               396           2 LOAD_FAST                0 (self)
+               407           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (client)
                             14 LOAD_METHOD              1 (get)
                             36 LOAD_FAST                0 (self)
                             38 LOAD_ATTR                2 (url)
                             48 PRECALL                  1
                             52 CALL                     1
                             62 STORE_FAST               1 (response)
                
-               398          64 LOAD_FAST                0 (self)
+               409          64 LOAD_FAST                0 (self)
                             66 LOAD_METHOD              3 (assertRedirects)
                             88 LOAD_FAST                1 (response)
                             90 LOAD_GLOBAL              9 (NULL + reverse)
                            102 LOAD_CONST               1 ('punkweb_bb:login')
                            104 PRECALL                  1
                            108 CALL                     1
                            118 FORMAT_VALUE             0
@@ -3937,15 +4059,15 @@
                   '?next='
                names      ('client', 'get', 'url', 'assertRedirects', 'reverse')
                varnames   ('self', 'response')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'test_redirect_unauthenticated_user'
-               firstlineno 395
+               firstlineno 406
                lnotab 0x02013e02
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
@@ -3960,79 +4082,79 @@
                   0000000000000001007c006a0200000000000000006a0800000000000000
                   00a0090000000000000000000000000000000000000000a6000000ab0000
                   0000000000000001007c00a0050000000000000000000000000000000000
                   0000007c006a0200000000000000006a0800000000000000006a0a000000
                   00000000006404a6020000ab02000000000000000001007c00a005000000
                   00000000000000000000000000000000007c016a06000000000000000064
                   01a6020000ab020000000000000000010064005300
-               400           0 RESUME                   0
+               411           0 RESUME                   0
                
-               401           2 LOAD_FAST                0 (self)
+               412           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (client)
                             14 LOAD_METHOD              1 (force_login)
                             36 LOAD_FAST                0 (self)
                             38 LOAD_ATTR                2 (user)
                             48 PRECALL                  1
                             52 CALL                     1
                             62 POP_TOP
                
-               402          64 LOAD_FAST                0 (self)
+               413          64 LOAD_FAST                0 (self)
                             66 LOAD_ATTR                0 (client)
                             76 LOAD_METHOD              3 (get)
                             98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                4 (url)
                            110 PRECALL                  1
                            114 CALL                     1
                            124 STORE_FAST               1 (response)
                
-               404         126 LOAD_FAST                0 (self)
+               415         126 LOAD_FAST                0 (self)
                            128 LOAD_METHOD              5 (assertEqual)
                            150 LOAD_FAST                1 (response)
                            152 LOAD_ATTR                6 (status_code)
                            162 LOAD_CONST               1 (200)
                            164 PRECALL                  2
                            168 CALL                     2
                            178 POP_TOP
                
-               406         180 LOAD_FAST                0 (self)
+               417         180 LOAD_FAST                0 (self)
                            182 LOAD_ATTR                0 (client)
                            192 LOAD_METHOD              7 (post)
                
-               407         214 LOAD_FAST                0 (self)
+               418         214 LOAD_FAST                0 (self)
                            216 LOAD_ATTR                4 (url)
                
-               409         226 LOAD_CONST               2 ('signature')
+               420         226 LOAD_CONST               2 ('signature')
                            228 LOAD_CONST               3 ('[b]test[/b]')
                
-               408         230 BUILD_MAP                1
+               419         230 BUILD_MAP                1
                
-               406         232 PRECALL                  2
+               417         232 PRECALL                  2
                            236 CALL                     2
                            246 POP_TOP
                
-               413         248 LOAD_FAST                0 (self)
+               424         248 LOAD_FAST                0 (self)
                            250 LOAD_ATTR                2 (user)
                            260 LOAD_ATTR                8 (profile)
                            270 LOAD_METHOD              9 (refresh_from_db)
                            292 PRECALL                  0
                            296 CALL                     0
                            306 POP_TOP
                
-               414         308 LOAD_FAST                0 (self)
+               425         308 LOAD_FAST                0 (self)
                            310 LOAD_METHOD              5 (assertEqual)
                            332 LOAD_FAST                0 (self)
                            334 LOAD_ATTR                2 (user)
                            344 LOAD_ATTR                8 (profile)
                            354 LOAD_ATTR               10 (_signature_rendered)
                            364 LOAD_CONST               4 ('<strong>test</strong>')
                            366 PRECALL                  2
                            370 CALL                     2
                            380 POP_TOP
                
-               416         382 LOAD_FAST                0 (self)
+               427         382 LOAD_FAST                0 (self)
                            384 LOAD_METHOD              5 (assertEqual)
                            406 LOAD_FAST                1 (response)
                            408 LOAD_ATTR                6 (status_code)
                            418 LOAD_CONST               1 (200)
                            420 PRECALL                  2
                            424 CALL                     2
                            434 POP_TOP
@@ -4046,53 +4168,53 @@
                   '<strong>test</strong>'
                names      ('client', 'force_login', 'user', 'get', 'url', 'assertEqual', 'status_code', 'post', 'profile', 'refresh_from_db', '_signature_rendered')
                varnames   ('self', 'response')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'test_settings'
-               firstlineno 400
+               firstlineno 411
                lnotab 0x02013e013e02360222010c0204ff02fe10073c014a02
             None
          names      ('__name__', '__module__', '__qualname__', 'setUp', 'test_redirect_unauthenticated_user', 'test_settings')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
          name       'SettingsViewTestCase'
-         firstlineno 389
+         firstlineno 400
          lnotab 0x0a0106050605
       'SettingsViewTestCase'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a02640184005a03640284005a04640384005a0564
             0484005a0664055300
-         419           0 RESUME                   0
+         430           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ThreadCreateViewTestCase')
                        8 STORE_NAME               2 (__qualname__)
          
-         420          10 LOAD_CONST               1 (<code object setUp, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 420>)
+         431          10 LOAD_CONST               1 (<code object setUp, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 431>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (setUp)
          
-         435          16 LOAD_CONST               2 (<code object test_redirect_unauthenticated_user, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 435>)
+         446          16 LOAD_CONST               2 (<code object test_redirect_unauthenticated_user, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 446>)
                       18 MAKE_FUNCTION            0
                       20 STORE_NAME               4 (test_redirect_unauthenticated_user)
          
-         440          22 LOAD_CONST               3 (<code object test_thread_create, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 440>)
+         451          22 LOAD_CONST               3 (<code object test_thread_create, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 451>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               5 (test_thread_create)
          
-         462          28 LOAD_CONST               4 (<code object test_thread_create_staff_post_only, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 462>)
+         473          28 LOAD_CONST               4 (<code object test_thread_create_staff_post_only, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 473>)
                       30 MAKE_FUNCTION            0
                       32 STORE_NAME               6 (test_thread_create_staff_post_only)
                       34 LOAD_CONST               5 (None)
                       36 RETURN_VALUE
          consts
             'ThreadCreateViewTestCase'
             code
@@ -4114,95 +4236,95 @@
                   00a007000000000000000000000000000000000000000064057c006a0800
                   0000000000000064056406ac07a6040000ab0400000000000000007c005f
                   0b000000000000000074190000000000000000000064087c006a0a000000
                   00000000006a0d00000000000000006701ac09a6020000ab020000000000
                   0000007c005f0e000000000000000074190000000000000000000064087c
                   006a0b00000000000000006a0d00000000000000006701ac09a6020000ab
                   0200000000000000007c005f0f000000000000000064005300
-               420           0 RESUME                   0
+               431           0 RESUME                   0
                
-               421           2 LOAD_GLOBAL              1 (NULL + Client)
+               432           2 LOAD_GLOBAL              1 (NULL + Client)
                             14 PRECALL                  0
                             18 CALL                     0
                             28 LOAD_FAST                0 (self)
                             30 STORE_ATTR               1 (client)
                
-               422          40 LOAD_GLOBAL              4 (User)
+               433          40 LOAD_GLOBAL              4 (User)
                             52 LOAD_ATTR                3 (objects)
                             62 LOAD_METHOD              4 (create_user)
                             84 LOAD_CONST               1 ('test')
                             86 LOAD_CONST               1 ('test')
                             88 KW_NAMES                 2
                             90 PRECALL                  2
                             94 CALL                     2
                            104 LOAD_FAST                0 (self)
                            106 STORE_ATTR               5 (user)
                
-               423         116 LOAD_GLOBAL             12 (Category)
+               434         116 LOAD_GLOBAL             12 (Category)
                            128 LOAD_ATTR                3 (objects)
                            138 LOAD_METHOD              7 (create)
                            160 LOAD_CONST               1 ('test')
                            162 KW_NAMES                 3
                            164 PRECALL                  1
                            168 CALL                     1
                            178 LOAD_FAST                0 (self)
                            180 STORE_ATTR               8 (category)
                
-               424         190 LOAD_GLOBAL             18 (Subcategory)
+               435         190 LOAD_GLOBAL             18 (Subcategory)
                            202 LOAD_ATTR                3 (objects)
                            212 LOAD_METHOD              7 (create)
                
-               425         234 LOAD_CONST               1 ('test')
+               436         234 LOAD_CONST               1 ('test')
                            236 LOAD_FAST                0 (self)
                            238 LOAD_ATTR                8 (category)
                            248 LOAD_CONST               1 ('test')
                
-               424         250 KW_NAMES                 4
+               435         250 KW_NAMES                 4
                            252 PRECALL                  3
                            256 CALL                     3
                            266 LOAD_FAST                0 (self)
                            268 STORE_ATTR              10 (subcategory)
                
-               427         278 LOAD_GLOBAL             18 (Subcategory)
+               438         278 LOAD_GLOBAL             18 (Subcategory)
                            290 LOAD_ATTR                3 (objects)
                            300 LOAD_METHOD              7 (create)
                
-               428         322 LOAD_CONST               5 ('staff')
+               439         322 LOAD_CONST               5 ('staff')
                            324 LOAD_FAST                0 (self)
                            326 LOAD_ATTR                8 (category)
                            336 LOAD_CONST               5 ('staff')
                            338 LOAD_CONST               6 (True)
                
-               427         340 KW_NAMES                 7
+               438         340 KW_NAMES                 7
                            342 PRECALL                  4
                            346 CALL                     4
                            356 LOAD_FAST                0 (self)
                            358 STORE_ATTR              11 (staff_subcategory)
                
-               430         368 LOAD_GLOBAL             25 (NULL + reverse)
+               441         368 LOAD_GLOBAL             25 (NULL + reverse)
                            380 LOAD_CONST               8 ('punkweb_bb:thread_create')
                            382 LOAD_FAST                0 (self)
                            384 LOAD_ATTR               10 (subcategory)
                            394 LOAD_ATTR               13 (slug)
                            404 BUILD_LIST               1
                            406 KW_NAMES                 9
                            408 PRECALL                  2
                            412 CALL                     2
                            422 LOAD_FAST                0 (self)
                            424 STORE_ATTR              14 (url)
                
-               431         434 LOAD_GLOBAL             25 (NULL + reverse)
+               442         434 LOAD_GLOBAL             25 (NULL + reverse)
                
-               432         446 LOAD_CONST               8 ('punkweb_bb:thread_create')
+               443         446 LOAD_CONST               8 ('punkweb_bb:thread_create')
                            448 LOAD_FAST                0 (self)
                            450 LOAD_ATTR               11 (staff_subcategory)
                            460 LOAD_ATTR               13 (slug)
                            470 BUILD_LIST               1
                
-               431         472 KW_NAMES                 9
+               442         472 KW_NAMES                 9
                            474 PRECALL                  2
                            478 CALL                     2
                            488 LOAD_FAST                0 (self)
                            490 STORE_ATTR              15 (staff_only_url)
                            500 LOAD_CONST               0 (None)
                            502 RETURN_VALUE
                consts
@@ -4218,40 +4340,40 @@
                   ('args',)
                names      ('Client', 'client', 'User', 'objects', 'create_user', 'user', 'Category', 'create', 'category', 'Subcategory', 'subcategory', 'staff_subcategory', 'reverse', 'slug', 'url', 'staff_only_url')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'setUp'
-               firstlineno 420
+               firstlineno 431
                lnotab 0x020126014c014a012c0110ff1c032c0112ff1c0342010c011aff
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 6
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c006a020000000000000000a6010000ab010000000000
                   0000007d017c00a00300000000000000000000000000000000000000007c
                   017409000000000000000000006401a6010000ab0100000000000000009b
                   0064027c006a0200000000000000009b009d03a6020000ab020000000000
                   000000010064005300
-               435           0 RESUME                   0
+               446           0 RESUME                   0
                
-               436           2 LOAD_FAST                0 (self)
+               447           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (client)
                             14 LOAD_METHOD              1 (get)
                             36 LOAD_FAST                0 (self)
                             38 LOAD_ATTR                2 (url)
                             48 PRECALL                  1
                             52 CALL                     1
                             62 STORE_FAST               1 (response)
                
-               438          64 LOAD_FAST                0 (self)
+               449          64 LOAD_FAST                0 (self)
                             66 LOAD_METHOD              3 (assertRedirects)
                             88 LOAD_FAST                1 (response)
                             90 LOAD_GLOBAL              9 (NULL + reverse)
                            102 LOAD_CONST               1 ('punkweb_bb:login')
                            104 PRECALL                  1
                            108 CALL                     1
                            118 FORMAT_VALUE             0
@@ -4271,15 +4393,15 @@
                   '?next='
                names      ('client', 'get', 'url', 'assertRedirects', 'reverse')
                varnames   ('self', 'response')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'test_redirect_unauthenticated_user'
-               firstlineno 435
+               firstlineno 446
                lnotab 0x02013e02
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 6
                flags     : 3
                code
@@ -4300,105 +4422,105 @@
                   10000000000000000000006a090000000000000000a00d00000000000000
                   00000000000000000000000000a6000000ab0000000000000000006406a6
                   020000ab02000000000000000001007c00a0050000000000000000000000
                   0000000000000000007c026a0200000000000000007c006a020000000000
                   000000a6020000ab02000000000000000001007c00a00500000000000000
                   000000000000000000000000007c026a0e00000000000000007c006a0e00
                   00000000000000a6020000ab020000000000000000010064005300
-               440           0 RESUME                   0
+               451           0 RESUME                   0
                
-               441           2 LOAD_FAST                0 (self)
+               452           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (client)
                             14 LOAD_METHOD              1 (force_login)
                             36 LOAD_FAST                0 (self)
                             38 LOAD_ATTR                2 (user)
                             48 PRECALL                  1
                             52 CALL                     1
                             62 POP_TOP
                
-               442          64 LOAD_FAST                0 (self)
+               453          64 LOAD_FAST                0 (self)
                             66 LOAD_ATTR                0 (client)
                             76 LOAD_METHOD              3 (get)
                             98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                4 (url)
                            110 PRECALL                  1
                            114 CALL                     1
                            124 STORE_FAST               1 (response)
                
-               444         126 LOAD_FAST                0 (self)
+               455         126 LOAD_FAST                0 (self)
                            128 LOAD_METHOD              5 (assertEqual)
                            150 LOAD_FAST                1 (response)
                            152 LOAD_ATTR                6 (status_code)
                            162 LOAD_CONST               1 (200)
                            164 PRECALL                  2
                            168 CALL                     2
                            178 POP_TOP
                
-               446         180 LOAD_FAST                0 (self)
+               457         180 LOAD_FAST                0 (self)
                            182 LOAD_ATTR                0 (client)
                            192 LOAD_METHOD              7 (post)
                
-               447         214 LOAD_FAST                0 (self)
+               458         214 LOAD_FAST                0 (self)
                            216 LOAD_ATTR                4 (url)
                
-               449         226 LOAD_CONST               2 ('test')
+               460         226 LOAD_CONST               2 ('test')
                
-               450         228 LOAD_CONST               2 ('test')
+               461         228 LOAD_CONST               2 ('test')
                
-               448         230 LOAD_CONST               3 (('title', 'content'))
+               459         230 LOAD_CONST               3 (('title', 'content'))
                            232 BUILD_CONST_KEY_MAP      2
                
-               452         234 LOAD_CONST               4 (True)
+               463         234 LOAD_CONST               4 (True)
                
-               446         236 KW_NAMES                 5
+               457         236 KW_NAMES                 5
                            238 PRECALL                  3
                            242 CALL                     3
                            252 STORE_FAST               1 (response)
                
-               455         254 LOAD_GLOBAL             16 (Thread)
+               466         254 LOAD_GLOBAL             16 (Thread)
                            266 LOAD_ATTR                9 (objects)
                            276 LOAD_METHOD             10 (first)
                            298 PRECALL                  0
                            302 CALL                     0
                            312 STORE_FAST               2 (new_thread)
                
-               457         314 LOAD_FAST                0 (self)
+               468         314 LOAD_FAST                0 (self)
                            316 LOAD_METHOD             11 (assertRedirects)
                            338 LOAD_FAST                1 (response)
                            340 LOAD_FAST                2 (new_thread)
                            342 LOAD_METHOD             12 (get_absolute_url)
                            364 PRECALL                  0
                            368 CALL                     0
                            378 PRECALL                  2
                            382 CALL                     2
                            392 POP_TOP
                
-               458         394 LOAD_FAST                0 (self)
+               469         394 LOAD_FAST                0 (self)
                            396 LOAD_METHOD              5 (assertEqual)
                            418 LOAD_GLOBAL             16 (Thread)
                            430 LOAD_ATTR                9 (objects)
                            440 LOAD_METHOD             13 (count)
                            462 PRECALL                  0
                            466 CALL                     0
                            476 LOAD_CONST               6 (1)
                            478 PRECALL                  2
                            482 CALL                     2
                            492 POP_TOP
                
-               459         494 LOAD_FAST                0 (self)
+               470         494 LOAD_FAST                0 (self)
                            496 LOAD_METHOD              5 (assertEqual)
                            518 LOAD_FAST                2 (new_thread)
                            520 LOAD_ATTR                2 (user)
                            530 LOAD_FAST                0 (self)
                            532 LOAD_ATTR                2 (user)
                            542 PRECALL                  2
                            546 CALL                     2
                            556 POP_TOP
                
-               460         558 LOAD_FAST                0 (self)
+               471         558 LOAD_FAST                0 (self)
                            560 LOAD_METHOD              5 (assertEqual)
                            582 LOAD_FAST                2 (new_thread)
                            584 LOAD_ATTR               14 (subcategory)
                            594 LOAD_FAST                0 (self)
                            596 LOAD_ATTR               14 (subcategory)
                            606 PRECALL                  2
                            610 CALL                     2
@@ -4415,15 +4537,15 @@
                   1
                names      ('client', 'force_login', 'user', 'get', 'url', 'assertEqual', 'status_code', 'post', 'Thread', 'objects', 'first', 'assertRedirects', 'get_absolute_url', 'count', 'subcategory')
                varnames   ('self', 'response', 'new_thread')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'test_thread_create'
-               firstlineno 440
+               firstlineno 451
                lnotab
                   0x02013e013e02360222010c02020102fe040402fa12093c025001640140
                   01
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
@@ -4433,35 +4555,35 @@
                   000000000000007c006a020000000000000000a6010000ab010000000000
                   00000001007c006a000000000000000000a0030000000000000000000000
                   0000000000000000007c006a040000000000000000a6010000ab01000000
                   00000000007d017c00a00500000000000000000000000000000000000000
                   007c017c006a060000000000000000a00700000000000000000000000000
                   00000000000000a6000000ab000000000000000000a6020000ab02000000
                   0000000000010064005300
-               462           0 RESUME                   0
+               473           0 RESUME                   0
                
-               463           2 LOAD_FAST                0 (self)
+               474           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (client)
                             14 LOAD_METHOD              1 (force_login)
                             36 LOAD_FAST                0 (self)
                             38 LOAD_ATTR                2 (user)
                             48 PRECALL                  1
                             52 CALL                     1
                             62 POP_TOP
                
-               464          64 LOAD_FAST                0 (self)
+               475          64 LOAD_FAST                0 (self)
                             66 LOAD_ATTR                0 (client)
                             76 LOAD_METHOD              3 (get)
                             98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                4 (staff_only_url)
                            110 PRECALL                  1
                            114 CALL                     1
                            124 STORE_FAST               1 (response)
                
-               466         126 LOAD_FAST                0 (self)
+               477         126 LOAD_FAST                0 (self)
                            128 LOAD_METHOD              5 (assertRedirects)
                            150 LOAD_FAST                1 (response)
                            152 LOAD_FAST                0 (self)
                            154 LOAD_ATTR                6 (staff_subcategory)
                            164 LOAD_METHOD              7 (get_absolute_url)
                            186 PRECALL                  0
                            190 CALL                     0
@@ -4474,43 +4596,43 @@
                   None
                names      ('client', 'force_login', 'user', 'get', 'staff_only_url', 'assertRedirects', 'staff_subcategory', 'get_absolute_url')
                varnames   ('self', 'response')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'test_thread_create_staff_post_only'
-               firstlineno 462
+               firstlineno 473
                lnotab 0x02013e013e02
             None
          names      ('__name__', '__module__', '__qualname__', 'setUp', 'test_redirect_unauthenticated_user', 'test_thread_create', 'test_thread_create_staff_post_only')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
          name       'ThreadCreateViewTestCase'
-         firstlineno 419
+         firstlineno 430
          lnotab 0x0a01060f06050616
       'ThreadCreateViewTestCase'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a03640284005a0464035300
-         469           0 RESUME                   0
+         480           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ThreadViewTestCase')
                        8 STORE_NAME               2 (__qualname__)
          
-         470          10 LOAD_CONST               1 (<code object setUp, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 470>)
+         481          10 LOAD_CONST               1 (<code object setUp, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 481>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (setUp)
          
-         482          16 LOAD_CONST               2 (<code object test_view_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 482>)
+         493          16 LOAD_CONST               2 (<code object test_view_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 493>)
                       18 MAKE_FUNCTION            0
                       20 STORE_NAME               4 (test_view_count)
                       22 LOAD_CONST               3 (None)
                       24 RETURN_VALUE
          consts
             'ThreadViewTestCase'
             code
@@ -4530,76 +4652,76 @@
                   0800000000000000006401ac04a6030000ab0300000000000000007c005f
                   0a00000000000000007416000000000000000000006a0300000000000000
                   00a00700000000000000000000000000000000000000007c006a0a000000
                   00000000007c006a05000000000000000064016401ac05a6040000ab0400
                   000000000000007c005f0c0000000000000000741b000000000000000000
                   0064067c006a0c00000000000000006a0e00000000000000006701ac07a6
                   020000ab0200000000000000007c005f0f000000000000000064005300
-               470           0 RESUME                   0
+               481           0 RESUME                   0
                
-               471           2 LOAD_GLOBAL              1 (NULL + Client)
+               482           2 LOAD_GLOBAL              1 (NULL + Client)
                             14 PRECALL                  0
                             18 CALL                     0
                             28 LOAD_FAST                0 (self)
                             30 STORE_ATTR               1 (client)
                
-               472          40 LOAD_GLOBAL              4 (User)
+               483          40 LOAD_GLOBAL              4 (User)
                             52 LOAD_ATTR                3 (objects)
                             62 LOAD_METHOD              4 (create_user)
                             84 LOAD_CONST               1 ('test')
                             86 LOAD_CONST               1 ('test')
                             88 KW_NAMES                 2
                             90 PRECALL                  2
                             94 CALL                     2
                            104 LOAD_FAST                0 (self)
                            106 STORE_ATTR               5 (user)
                
-               473         116 LOAD_GLOBAL             12 (Category)
+               484         116 LOAD_GLOBAL             12 (Category)
                            128 LOAD_ATTR                3 (objects)
                            138 LOAD_METHOD              7 (create)
                            160 LOAD_CONST               1 ('test')
                            162 KW_NAMES                 3
                            164 PRECALL                  1
                            168 CALL                     1
                            178 LOAD_FAST                0 (self)
                            180 STORE_ATTR               8 (category)
                
-               474         190 LOAD_GLOBAL             18 (Subcategory)
+               485         190 LOAD_GLOBAL             18 (Subcategory)
                            202 LOAD_ATTR                3 (objects)
                            212 LOAD_METHOD              7 (create)
                
-               475         234 LOAD_CONST               1 ('test')
+               486         234 LOAD_CONST               1 ('test')
                            236 LOAD_FAST                0 (self)
                            238 LOAD_ATTR                8 (category)
                            248 LOAD_CONST               1 ('test')
                
-               474         250 KW_NAMES                 4
+               485         250 KW_NAMES                 4
                            252 PRECALL                  3
                            256 CALL                     3
                            266 LOAD_FAST                0 (self)
                            268 STORE_ATTR              10 (subcategory)
                
-               477         278 LOAD_GLOBAL             22 (Thread)
+               488         278 LOAD_GLOBAL             22 (Thread)
                            290 LOAD_ATTR                3 (objects)
                            300 LOAD_METHOD              7 (create)
                
-               478         322 LOAD_FAST                0 (self)
+               489         322 LOAD_FAST                0 (self)
                            324 LOAD_ATTR               10 (subcategory)
                            334 LOAD_FAST                0 (self)
                            336 LOAD_ATTR                5 (user)
                            346 LOAD_CONST               1 ('test')
                            348 LOAD_CONST               1 ('test')
                
-               477         350 KW_NAMES                 5
+               488         350 KW_NAMES                 5
                            352 PRECALL                  4
                            356 CALL                     4
                            366 LOAD_FAST                0 (self)
                            368 STORE_ATTR              12 (thread)
                
-               480         378 LOAD_GLOBAL             27 (NULL + reverse)
+               491         378 LOAD_GLOBAL             27 (NULL + reverse)
                            390 LOAD_CONST               6 ('punkweb_bb:thread')
                            392 LOAD_FAST                0 (self)
                            394 LOAD_ATTR               12 (thread)
                            404 LOAD_ATTR               14 (id)
                            414 BUILD_LIST               1
                            416 KW_NAMES                 7
                            418 PRECALL                  2
@@ -4619,15 +4741,15 @@
                   ('args',)
                names      ('Client', 'client', 'User', 'objects', 'create_user', 'user', 'Category', 'create', 'category', 'Subcategory', 'subcategory', 'Thread', 'thread', 'reverse', 'id', 'url')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'setUp'
-               firstlineno 470
+               firstlineno 481
                lnotab 0x020126014c014a012c0110ff1c032c011cff1c03
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
@@ -4637,47 +4759,47 @@
                   016a0400000000000000006401190000000000000000006a050000000000
                   0000006402a6020000ab02000000000000000001007c006a000000000000
                   000000a00100000000000000000000000000000000000000007c006a0200
                   00000000000000a6010000ab0100000000000000007d017c00a003000000
                   00000000000000000000000000000000007c016a04000000000000000064
                   01190000000000000000006a0500000000000000006402a6020000ab0200
                   00000000000000010064005300
-               482           0 RESUME                   0
+               493           0 RESUME                   0
                
-               483           2 LOAD_FAST                0 (self)
+               494           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (client)
                             14 LOAD_METHOD              1 (get)
                             36 LOAD_FAST                0 (self)
                             38 LOAD_ATTR                2 (url)
                             48 PRECALL                  1
                             52 CALL                     1
                             62 STORE_FAST               1 (response)
                
-               484          64 LOAD_FAST                0 (self)
+               495          64 LOAD_FAST                0 (self)
                             66 LOAD_METHOD              3 (assertEqual)
                             88 LOAD_FAST                1 (response)
                             90 LOAD_ATTR                4 (context)
                            100 LOAD_CONST               1 ('thread')
                            102 BINARY_SUBSCR
                            112 LOAD_ATTR                5 (view_count)
                            122 LOAD_CONST               2 (1)
                            124 PRECALL                  2
                            128 CALL                     2
                            138 POP_TOP
                
-               488         140 LOAD_FAST                0 (self)
+               499         140 LOAD_FAST                0 (self)
                            142 LOAD_ATTR                0 (client)
                            152 LOAD_METHOD              1 (get)
                            174 LOAD_FAST                0 (self)
                            176 LOAD_ATTR                2 (url)
                            186 PRECALL                  1
                            190 CALL                     1
                            200 STORE_FAST               1 (response)
                
-               489         202 LOAD_FAST                0 (self)
+               500         202 LOAD_FAST                0 (self)
                            204 LOAD_METHOD              3 (assertEqual)
                            226 LOAD_FAST                1 (response)
                            228 LOAD_ATTR                4 (context)
                            238 LOAD_CONST               1 ('thread')
                            240 BINARY_SUBSCR
                            250 LOAD_ATTR                5 (view_count)
                            260 LOAD_CONST               2 (1)
@@ -4692,53 +4814,53 @@
                   1
                names      ('client', 'get', 'url', 'assertEqual', 'context', 'view_count')
                varnames   ('self', 'response')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'test_view_count'
-               firstlineno 482
+               firstlineno 493
                lnotab 0x02013e014c043e01
             None
          names      ('__name__', '__module__', '__qualname__', 'setUp', 'test_view_count')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
          name       'ThreadViewTestCase'
-         firstlineno 469
+         firstlineno 480
          lnotab 0x0a01060c
       'ThreadViewTestCase'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a02640184005a03640284005a04640384005a0564
             0484005a0664055300
-         492           0 RESUME                   0
+         503           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ThreadUpdateViewTestCase')
                        8 STORE_NAME               2 (__qualname__)
          
-         493          10 LOAD_CONST               1 (<code object setUp, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 493>)
+         504          10 LOAD_CONST               1 (<code object setUp, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 504>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (setUp)
          
-         506          16 LOAD_CONST               2 (<code object test_redirect_unauthenticated_user, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 506>)
+         517          16 LOAD_CONST               2 (<code object test_redirect_unauthenticated_user, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 517>)
                       18 MAKE_FUNCTION            0
                       20 STORE_NAME               4 (test_redirect_unauthenticated_user)
          
-         511          22 LOAD_CONST               3 (<code object test_is_author, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 511>)
+         522          22 LOAD_CONST               3 (<code object test_is_author, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 522>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               5 (test_is_author)
          
-         520          28 LOAD_CONST               4 (<code object test_thread_update, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 520>)
+         531          28 LOAD_CONST               4 (<code object test_thread_update, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 531>)
                       30 MAKE_FUNCTION            0
                       32 STORE_NAME               6 (test_thread_update)
                       34 LOAD_CONST               5 (None)
                       36 RETURN_VALUE
          consts
             'ThreadUpdateViewTestCase'
             code
@@ -4761,87 +4883,87 @@
                   030000ab0300000000000000007c005f0b00000000000000007418000000
                   000000000000006a030000000000000000a0080000000000000000000000
                   0000000000000000007c006a0b00000000000000007c006a050000000000
                   00000064016401ac06a6040000ab0400000000000000007c005f0d000000
                   0000000000741d0000000000000000000064077c006a0d00000000000000
                   006a0f00000000000000006701ac08a6020000ab0200000000000000007c
                   005f10000000000000000064005300
-               493           0 RESUME                   0
+               504           0 RESUME                   0
                
-               494           2 LOAD_GLOBAL              1 (NULL + Client)
+               505           2 LOAD_GLOBAL              1 (NULL + Client)
                             14 PRECALL                  0
                             18 CALL                     0
                             28 LOAD_FAST                0 (self)
                             30 STORE_ATTR               1 (client)
                
-               495          40 LOAD_GLOBAL              4 (User)
+               506          40 LOAD_GLOBAL              4 (User)
                             52 LOAD_ATTR                3 (objects)
                             62 LOAD_METHOD              4 (create_user)
                             84 LOAD_CONST               1 ('test')
                             86 LOAD_CONST               1 ('test')
                             88 KW_NAMES                 2
                             90 PRECALL                  2
                             94 CALL                     2
                            104 LOAD_FAST                0 (self)
                            106 STORE_ATTR               5 (user)
                
-               496         116 LOAD_GLOBAL              4 (User)
+               507         116 LOAD_GLOBAL              4 (User)
                            128 LOAD_ATTR                3 (objects)
                            138 LOAD_METHOD              4 (create_user)
                            160 LOAD_CONST               3 ('other')
                            162 LOAD_CONST               3 ('other')
                            164 KW_NAMES                 2
                            166 PRECALL                  2
                            170 CALL                     2
                            180 LOAD_FAST                0 (self)
                            182 STORE_ATTR               6 (other_user)
                
-               497         192 LOAD_GLOBAL             14 (Category)
+               508         192 LOAD_GLOBAL             14 (Category)
                            204 LOAD_ATTR                3 (objects)
                            214 LOAD_METHOD              8 (create)
                            236 LOAD_CONST               1 ('test')
                            238 KW_NAMES                 4
                            240 PRECALL                  1
                            244 CALL                     1
                            254 LOAD_FAST                0 (self)
                            256 STORE_ATTR               9 (category)
                
-               498         266 LOAD_GLOBAL             20 (Subcategory)
+               509         266 LOAD_GLOBAL             20 (Subcategory)
                            278 LOAD_ATTR                3 (objects)
                            288 LOAD_METHOD              8 (create)
                
-               499         310 LOAD_CONST               1 ('test')
+               510         310 LOAD_CONST               1 ('test')
                            312 LOAD_FAST                0 (self)
                            314 LOAD_ATTR                9 (category)
                            324 LOAD_CONST               1 ('test')
                
-               498         326 KW_NAMES                 5
+               509         326 KW_NAMES                 5
                            328 PRECALL                  3
                            332 CALL                     3
                            342 LOAD_FAST                0 (self)
                            344 STORE_ATTR              11 (subcategory)
                
-               501         354 LOAD_GLOBAL             24 (Thread)
+               512         354 LOAD_GLOBAL             24 (Thread)
                            366 LOAD_ATTR                3 (objects)
                            376 LOAD_METHOD              8 (create)
                
-               502         398 LOAD_FAST                0 (self)
+               513         398 LOAD_FAST                0 (self)
                            400 LOAD_ATTR               11 (subcategory)
                            410 LOAD_FAST                0 (self)
                            412 LOAD_ATTR                5 (user)
                            422 LOAD_CONST               1 ('test')
                            424 LOAD_CONST               1 ('test')
                
-               501         426 KW_NAMES                 6
+               512         426 KW_NAMES                 6
                            428 PRECALL                  4
                            432 CALL                     4
                            442 LOAD_FAST                0 (self)
                            444 STORE_ATTR              13 (thread)
                
-               504         454 LOAD_GLOBAL             29 (NULL + reverse)
+               515         454 LOAD_GLOBAL             29 (NULL + reverse)
                            466 LOAD_CONST               7 ('punkweb_bb:thread_update')
                            468 LOAD_FAST                0 (self)
                            470 LOAD_ATTR               13 (thread)
                            480 LOAD_ATTR               15 (id)
                            490 BUILD_LIST               1
                            492 KW_NAMES                 8
                            494 PRECALL                  2
@@ -4862,40 +4984,40 @@
                   ('args',)
                names      ('Client', 'client', 'User', 'objects', 'create_user', 'user', 'other_user', 'Category', 'create', 'category', 'Subcategory', 'subcategory', 'Thread', 'thread', 'reverse', 'id', 'url')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'setUp'
-               firstlineno 493
+               firstlineno 504
                lnotab 0x020126014c014c014a012c0110ff1c032c011cff1c03
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 6
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c006a020000000000000000a6010000ab010000000000
                   0000007d017c00a00300000000000000000000000000000000000000007c
                   017409000000000000000000006401a6010000ab0100000000000000009b
                   0064027c006a0200000000000000009b009d03a6020000ab020000000000
                   000000010064005300
-               506           0 RESUME                   0
+               517           0 RESUME                   0
                
-               507           2 LOAD_FAST                0 (self)
+               518           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (client)
                             14 LOAD_METHOD              1 (get)
                             36 LOAD_FAST                0 (self)
                             38 LOAD_ATTR                2 (url)
                             48 PRECALL                  1
                             52 CALL                     1
                             62 STORE_FAST               1 (response)
                
-               509          64 LOAD_FAST                0 (self)
+               520          64 LOAD_FAST                0 (self)
                             66 LOAD_METHOD              3 (assertRedirects)
                             88 LOAD_FAST                1 (response)
                             90 LOAD_GLOBAL              9 (NULL + reverse)
                            102 LOAD_CONST               1 ('punkweb_bb:login')
                            104 PRECALL                  1
                            108 CALL                     1
                            118 FORMAT_VALUE             0
@@ -4915,15 +5037,15 @@
                   '?next='
                names      ('client', 'get', 'url', 'assertRedirects', 'reverse')
                varnames   ('self', 'response')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'test_redirect_unauthenticated_user'
-               firstlineno 506
+               firstlineno 517
                lnotab 0x02013e02
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
@@ -4936,62 +5058,62 @@
                   007c006a000000000000000000a001000000000000000000000000000000
                   00000000007c006a070000000000000000a6010000ab0100000000000000
                   0001007c006a000000000000000000a00300000000000000000000000000
                   000000000000007c006a040000000000000000a6010000ab010000000000
                   0000007d017c00a00500000000000000000000000000000000000000007c
                   016a0600000000000000006402a6020000ab020000000000000000010064
                   005300
-               511           0 RESUME                   0
+               522           0 RESUME                   0
                
-               512           2 LOAD_FAST                0 (self)
+               523           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (client)
                             14 LOAD_METHOD              1 (force_login)
                             36 LOAD_FAST                0 (self)
                             38 LOAD_ATTR                2 (other_user)
                             48 PRECALL                  1
                             52 CALL                     1
                             62 POP_TOP
                
-               513          64 LOAD_FAST                0 (self)
+               524          64 LOAD_FAST                0 (self)
                             66 LOAD_ATTR                0 (client)
                             76 LOAD_METHOD              3 (get)
                             98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                4 (url)
                            110 PRECALL                  1
                            114 CALL                     1
                            124 STORE_FAST               1 (response)
                
-               514         126 LOAD_FAST                0 (self)
+               525         126 LOAD_FAST                0 (self)
                            128 LOAD_METHOD              5 (assertEqual)
                            150 LOAD_FAST                1 (response)
                            152 LOAD_ATTR                6 (status_code)
                            162 LOAD_CONST               1 (404)
                            164 PRECALL                  2
                            168 CALL                     2
                            178 POP_TOP
                
-               516         180 LOAD_FAST                0 (self)
+               527         180 LOAD_FAST                0 (self)
                            182 LOAD_ATTR                0 (client)
                            192 LOAD_METHOD              1 (force_login)
                            214 LOAD_FAST                0 (self)
                            216 LOAD_ATTR                7 (user)
                            226 PRECALL                  1
                            230 CALL                     1
                            240 POP_TOP
                
-               517         242 LOAD_FAST                0 (self)
+               528         242 LOAD_FAST                0 (self)
                            244 LOAD_ATTR                0 (client)
                            254 LOAD_METHOD              3 (get)
                            276 LOAD_FAST                0 (self)
                            278 LOAD_ATTR                4 (url)
                            288 PRECALL                  1
                            292 CALL                     1
                            302 STORE_FAST               1 (response)
                
-               518         304 LOAD_FAST                0 (self)
+               529         304 LOAD_FAST                0 (self)
                            306 LOAD_METHOD              5 (assertEqual)
                            328 LOAD_FAST                1 (response)
                            330 LOAD_ATTR                6 (status_code)
                            340 LOAD_CONST               2 (200)
                            342 PRECALL                  2
                            346 CALL                     2
                            356 POP_TOP
@@ -5003,15 +5125,15 @@
                   200
                names      ('client', 'force_login', 'other_user', 'get', 'url', 'assertEqual', 'status_code', 'user')
                varnames   ('self', 'response')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'test_is_author'
-               firstlineno 511
+               firstlineno 522
                lnotab 0x02013e013e0136023e013e01
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 6
                flags     : 3
                code
@@ -5029,94 +5151,94 @@
                   020000ab02000000000000000001007c006a090000000000000000a00b00
                   00000000000000000000000000000000000000a6000000ab000000000000
                   00000001007c00a00500000000000000000000000000000000000000007c
                   006a0900000000000000006a0c00000000000000006402a6020000ab0200
                   0000000000000001007c00a0050000000000000000000000000000000000
                   0000007c006a0900000000000000006a0d00000000000000006402a60200
                   00ab020000000000000000010064005300
-               520           0 RESUME                   0
+               531           0 RESUME                   0
                
-               521           2 LOAD_FAST                0 (self)
+               532           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (client)
                             14 LOAD_METHOD              1 (force_login)
                             36 LOAD_FAST                0 (self)
                             38 LOAD_ATTR                2 (user)
                             48 PRECALL                  1
                             52 CALL                     1
                             62 POP_TOP
                
-               522          64 LOAD_FAST                0 (self)
+               533          64 LOAD_FAST                0 (self)
                             66 LOAD_ATTR                0 (client)
                             76 LOAD_METHOD              3 (get)
                             98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                4 (url)
                            110 PRECALL                  1
                            114 CALL                     1
                            124 STORE_FAST               1 (response)
                
-               524         126 LOAD_FAST                0 (self)
+               535         126 LOAD_FAST                0 (self)
                            128 LOAD_METHOD              5 (assertEqual)
                            150 LOAD_FAST                1 (response)
                            152 LOAD_ATTR                6 (status_code)
                            162 LOAD_CONST               1 (200)
                            164 PRECALL                  2
                            168 CALL                     2
                            178 POP_TOP
                
-               526         180 LOAD_FAST                0 (self)
+               537         180 LOAD_FAST                0 (self)
                            182 LOAD_ATTR                0 (client)
                            192 LOAD_METHOD              7 (post)
                
-               527         214 LOAD_FAST                0 (self)
+               538         214 LOAD_FAST                0 (self)
                            216 LOAD_ATTR                4 (url)
                
-               529         226 LOAD_CONST               2 ('edit')
+               540         226 LOAD_CONST               2 ('edit')
                
-               530         228 LOAD_CONST               2 ('edit')
+               541         228 LOAD_CONST               2 ('edit')
                
-               528         230 LOAD_CONST               3 (('title', 'content'))
+               539         230 LOAD_CONST               3 (('title', 'content'))
                            232 BUILD_CONST_KEY_MAP      2
                
-               532         234 LOAD_CONST               4 (True)
+               543         234 LOAD_CONST               4 (True)
                
-               526         236 KW_NAMES                 5
+               537         236 KW_NAMES                 5
                            238 PRECALL                  3
                            242 CALL                     3
                            252 STORE_FAST               1 (response)
                
-               535         254 LOAD_FAST                0 (self)
+               546         254 LOAD_FAST                0 (self)
                            256 LOAD_METHOD              8 (assertRedirects)
                            278 LOAD_FAST                1 (response)
                            280 LOAD_FAST                0 (self)
                            282 LOAD_ATTR                9 (thread)
                            292 LOAD_METHOD             10 (get_absolute_url)
                            314 PRECALL                  0
                            318 CALL                     0
                            328 PRECALL                  2
                            332 CALL                     2
                            342 POP_TOP
                
-               536         344 LOAD_FAST                0 (self)
+               547         344 LOAD_FAST                0 (self)
                            346 LOAD_ATTR                9 (thread)
                            356 LOAD_METHOD             11 (refresh_from_db)
                            378 PRECALL                  0
                            382 CALL                     0
                            392 POP_TOP
                
-               537         394 LOAD_FAST                0 (self)
+               548         394 LOAD_FAST                0 (self)
                            396 LOAD_METHOD              5 (assertEqual)
                            418 LOAD_FAST                0 (self)
                            420 LOAD_ATTR                9 (thread)
                            430 LOAD_ATTR               12 (title)
                            440 LOAD_CONST               2 ('edit')
                            442 PRECALL                  2
                            446 CALL                     2
                            456 POP_TOP
                
-               538         458 LOAD_FAST                0 (self)
+               549         458 LOAD_FAST                0 (self)
                            460 LOAD_METHOD              5 (assertEqual)
                            482 LOAD_FAST                0 (self)
                            484 LOAD_ATTR                9 (thread)
                            494 LOAD_ATTR               13 (_content_rendered)
                            504 LOAD_CONST               2 ('edit')
                            506 PRECALL                  2
                            510 CALL                     2
@@ -5132,53 +5254,53 @@
                   ('follow',)
                names      ('client', 'force_login', 'user', 'get', 'url', 'assertEqual', 'status_code', 'post', 'assertRedirects', 'thread', 'get_absolute_url', 'refresh_from_db', 'title', '_content_rendered')
                varnames   ('self', 'response')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'test_thread_update'
-               firstlineno 520
+               firstlineno 531
                lnotab 0x02013e013e02360222010c02020102fe040402fa12095a0132014001
             None
          names      ('__name__', '__module__', '__qualname__', 'setUp', 'test_redirect_unauthenticated_user', 'test_is_author', 'test_thread_update')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
          name       'ThreadUpdateViewTestCase'
-         firstlineno 492
+         firstlineno 503
          lnotab 0x0a01060d06050609
       'ThreadUpdateViewTestCase'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a02640184005a03640284005a04640384005a0564
             0484005a0664055300
-         541           0 RESUME                   0
+         552           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ThreadDeleteViewTestCase')
                        8 STORE_NAME               2 (__qualname__)
          
-         542          10 LOAD_CONST               1 (<code object setUp, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 542>)
+         553          10 LOAD_CONST               1 (<code object setUp, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 553>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (setUp)
          
-         555          16 LOAD_CONST               2 (<code object test_redirect_unauthenticated_user, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 555>)
+         566          16 LOAD_CONST               2 (<code object test_redirect_unauthenticated_user, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 566>)
                       18 MAKE_FUNCTION            0
                       20 STORE_NAME               4 (test_redirect_unauthenticated_user)
          
-         560          22 LOAD_CONST               3 (<code object test_is_author, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 560>)
+         571          22 LOAD_CONST               3 (<code object test_is_author, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 571>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               5 (test_is_author)
          
-         569          28 LOAD_CONST               4 (<code object test_thread_delete, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 569>)
+         580          28 LOAD_CONST               4 (<code object test_thread_delete, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 580>)
                       30 MAKE_FUNCTION            0
                       32 STORE_NAME               6 (test_thread_delete)
                       34 LOAD_CONST               5 (None)
                       36 RETURN_VALUE
          consts
             'ThreadDeleteViewTestCase'
             code
@@ -5201,87 +5323,87 @@
                   030000ab0300000000000000007c005f0b00000000000000007418000000
                   000000000000006a030000000000000000a0080000000000000000000000
                   0000000000000000007c006a0b00000000000000007c006a050000000000
                   00000064016401ac06a6040000ab0400000000000000007c005f0d000000
                   0000000000741d0000000000000000000064077c006a0d00000000000000
                   006a0f00000000000000006701ac08a6020000ab0200000000000000007c
                   005f10000000000000000064005300
-               542           0 RESUME                   0
+               553           0 RESUME                   0
                
-               543           2 LOAD_GLOBAL              1 (NULL + Client)
+               554           2 LOAD_GLOBAL              1 (NULL + Client)
                             14 PRECALL                  0
                             18 CALL                     0
                             28 LOAD_FAST                0 (self)
                             30 STORE_ATTR               1 (client)
                
-               544          40 LOAD_GLOBAL              4 (User)
+               555          40 LOAD_GLOBAL              4 (User)
                             52 LOAD_ATTR                3 (objects)
                             62 LOAD_METHOD              4 (create_user)
                             84 LOAD_CONST               1 ('test')
                             86 LOAD_CONST               1 ('test')
                             88 KW_NAMES                 2
                             90 PRECALL                  2
                             94 CALL                     2
                            104 LOAD_FAST                0 (self)
                            106 STORE_ATTR               5 (user)
                
-               545         116 LOAD_GLOBAL              4 (User)
+               556         116 LOAD_GLOBAL              4 (User)
                            128 LOAD_ATTR                3 (objects)
                            138 LOAD_METHOD              4 (create_user)
                            160 LOAD_CONST               3 ('other')
                            162 LOAD_CONST               3 ('other')
                            164 KW_NAMES                 2
                            166 PRECALL                  2
                            170 CALL                     2
                            180 LOAD_FAST                0 (self)
                            182 STORE_ATTR               6 (other_user)
                
-               546         192 LOAD_GLOBAL             14 (Category)
+               557         192 LOAD_GLOBAL             14 (Category)
                            204 LOAD_ATTR                3 (objects)
                            214 LOAD_METHOD              8 (create)
                            236 LOAD_CONST               1 ('test')
                            238 KW_NAMES                 4
                            240 PRECALL                  1
                            244 CALL                     1
                            254 LOAD_FAST                0 (self)
                            256 STORE_ATTR               9 (category)
                
-               547         266 LOAD_GLOBAL             20 (Subcategory)
+               558         266 LOAD_GLOBAL             20 (Subcategory)
                            278 LOAD_ATTR                3 (objects)
                            288 LOAD_METHOD              8 (create)
                
-               548         310 LOAD_CONST               1 ('test')
+               559         310 LOAD_CONST               1 ('test')
                            312 LOAD_FAST                0 (self)
                            314 LOAD_ATTR                9 (category)
                            324 LOAD_CONST               1 ('test')
                
-               547         326 KW_NAMES                 5
+               558         326 KW_NAMES                 5
                            328 PRECALL                  3
                            332 CALL                     3
                            342 LOAD_FAST                0 (self)
                            344 STORE_ATTR              11 (subcategory)
                
-               550         354 LOAD_GLOBAL             24 (Thread)
+               561         354 LOAD_GLOBAL             24 (Thread)
                            366 LOAD_ATTR                3 (objects)
                            376 LOAD_METHOD              8 (create)
                
-               551         398 LOAD_FAST                0 (self)
+               562         398 LOAD_FAST                0 (self)
                            400 LOAD_ATTR               11 (subcategory)
                            410 LOAD_FAST                0 (self)
                            412 LOAD_ATTR                5 (user)
                            422 LOAD_CONST               1 ('test')
                            424 LOAD_CONST               1 ('test')
                
-               550         426 KW_NAMES                 6
+               561         426 KW_NAMES                 6
                            428 PRECALL                  4
                            432 CALL                     4
                            442 LOAD_FAST                0 (self)
                            444 STORE_ATTR              13 (thread)
                
-               553         454 LOAD_GLOBAL             29 (NULL + reverse)
+               564         454 LOAD_GLOBAL             29 (NULL + reverse)
                            466 LOAD_CONST               7 ('punkweb_bb:thread_delete')
                            468 LOAD_FAST                0 (self)
                            470 LOAD_ATTR               13 (thread)
                            480 LOAD_ATTR               15 (id)
                            490 BUILD_LIST               1
                            492 KW_NAMES                 8
                            494 PRECALL                  2
@@ -5302,40 +5424,40 @@
                   ('args',)
                names      ('Client', 'client', 'User', 'objects', 'create_user', 'user', 'other_user', 'Category', 'create', 'category', 'Subcategory', 'subcategory', 'Thread', 'thread', 'reverse', 'id', 'url')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'setUp'
-               firstlineno 542
+               firstlineno 553
                lnotab 0x020126014c014c014a012c0110ff1c032c011cff1c03
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 6
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c006a020000000000000000a6010000ab010000000000
                   0000007d017c00a00300000000000000000000000000000000000000007c
                   017409000000000000000000006401a6010000ab0100000000000000009b
                   0064027c006a0200000000000000009b009d03a6020000ab020000000000
                   000000010064005300
-               555           0 RESUME                   0
+               566           0 RESUME                   0
                
-               556           2 LOAD_FAST                0 (self)
+               567           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (client)
                             14 LOAD_METHOD              1 (get)
                             36 LOAD_FAST                0 (self)
                             38 LOAD_ATTR                2 (url)
                             48 PRECALL                  1
                             52 CALL                     1
                             62 STORE_FAST               1 (response)
                
-               558          64 LOAD_FAST                0 (self)
+               569          64 LOAD_FAST                0 (self)
                             66 LOAD_METHOD              3 (assertRedirects)
                             88 LOAD_FAST                1 (response)
                             90 LOAD_GLOBAL              9 (NULL + reverse)
                            102 LOAD_CONST               1 ('punkweb_bb:login')
                            104 PRECALL                  1
                            108 CALL                     1
                            118 FORMAT_VALUE             0
@@ -5355,15 +5477,15 @@
                   '?next='
                names      ('client', 'get', 'url', 'assertRedirects', 'reverse')
                varnames   ('self', 'response')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'test_redirect_unauthenticated_user'
-               firstlineno 555
+               firstlineno 566
                lnotab 0x02013e02
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
@@ -5376,62 +5498,62 @@
                   007c006a000000000000000000a001000000000000000000000000000000
                   00000000007c006a070000000000000000a6010000ab0100000000000000
                   0001007c006a000000000000000000a00300000000000000000000000000
                   000000000000007c006a040000000000000000a6010000ab010000000000
                   0000007d017c00a00500000000000000000000000000000000000000007c
                   016a0600000000000000006402a6020000ab020000000000000000010064
                   005300
-               560           0 RESUME                   0
+               571           0 RESUME                   0
                
-               561           2 LOAD_FAST                0 (self)
+               572           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (client)
                             14 LOAD_METHOD              1 (force_login)
                             36 LOAD_FAST                0 (self)
                             38 LOAD_ATTR                2 (other_user)
                             48 PRECALL                  1
                             52 CALL                     1
                             62 POP_TOP
                
-               562          64 LOAD_FAST                0 (self)
+               573          64 LOAD_FAST                0 (self)
                             66 LOAD_ATTR                0 (client)
                             76 LOAD_METHOD              3 (get)
                             98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                4 (url)
                            110 PRECALL                  1
                            114 CALL                     1
                            124 STORE_FAST               1 (response)
                
-               563         126 LOAD_FAST                0 (self)
+               574         126 LOAD_FAST                0 (self)
                            128 LOAD_METHOD              5 (assertEqual)
                            150 LOAD_FAST                1 (response)
                            152 LOAD_ATTR                6 (status_code)
                            162 LOAD_CONST               1 (404)
                            164 PRECALL                  2
                            168 CALL                     2
                            178 POP_TOP
                
-               565         180 LOAD_FAST                0 (self)
+               576         180 LOAD_FAST                0 (self)
                            182 LOAD_ATTR                0 (client)
                            192 LOAD_METHOD              1 (force_login)
                            214 LOAD_FAST                0 (self)
                            216 LOAD_ATTR                7 (user)
                            226 PRECALL                  1
                            230 CALL                     1
                            240 POP_TOP
                
-               566         242 LOAD_FAST                0 (self)
+               577         242 LOAD_FAST                0 (self)
                            244 LOAD_ATTR                0 (client)
                            254 LOAD_METHOD              3 (get)
                            276 LOAD_FAST                0 (self)
                            278 LOAD_ATTR                4 (url)
                            288 PRECALL                  1
                            292 CALL                     1
                            302 STORE_FAST               1 (response)
                
-               567         304 LOAD_FAST                0 (self)
+               578         304 LOAD_FAST                0 (self)
                            306 LOAD_METHOD              5 (assertEqual)
                            328 LOAD_FAST                1 (response)
                            330 LOAD_ATTR                6 (status_code)
                            340 LOAD_CONST               2 (200)
                            342 PRECALL                  2
                            346 CALL                     2
                            356 POP_TOP
@@ -5443,15 +5565,15 @@
                   200
                names      ('client', 'force_login', 'other_user', 'get', 'url', 'assertEqual', 'status_code', 'user')
                varnames   ('self', 'response')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'test_is_author'
-               firstlineno 560
+               firstlineno 571
                lnotab 0x02013e013e0136023e013e01
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
@@ -5467,72 +5589,72 @@
                   007c016a0800000000000000006404190000000000000000007c006a0900
                   00000000000000a00a0000000000000000000000000000000000000000a6
                   000000ab000000000000000000a6020000ab02000000000000000001007c
                   00a005000000000000000000000000000000000000000074160000000000
                   00000000006a0c0000000000000000a00d00000000000000000000000000
                   00000000000000a6000000ab0000000000000000006405a6020000ab0200
                   00000000000000010064005300
-               569           0 RESUME                   0
+               580           0 RESUME                   0
                
-               570           2 LOAD_FAST                0 (self)
+               581           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (client)
                             14 LOAD_METHOD              1 (force_login)
                             36 LOAD_FAST                0 (self)
                             38 LOAD_ATTR                2 (user)
                             48 PRECALL                  1
                             52 CALL                     1
                             62 POP_TOP
                
-               571          64 LOAD_FAST                0 (self)
+               582          64 LOAD_FAST                0 (self)
                             66 LOAD_ATTR                0 (client)
                             76 LOAD_METHOD              3 (get)
                             98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                4 (url)
                            110 PRECALL                  1
                            114 CALL                     1
                            124 STORE_FAST               1 (response)
                
-               573         126 LOAD_FAST                0 (self)
+               584         126 LOAD_FAST                0 (self)
                            128 LOAD_METHOD              5 (assertEqual)
                            150 LOAD_FAST                1 (response)
                            152 LOAD_ATTR                6 (status_code)
                            162 LOAD_CONST               1 (200)
                            164 PRECALL                  2
                            168 CALL                     2
                            178 POP_TOP
                
-               575         180 LOAD_FAST                0 (self)
+               586         180 LOAD_FAST                0 (self)
                            182 LOAD_ATTR                0 (client)
                            192 LOAD_METHOD              7 (delete)
                            214 LOAD_FAST                0 (self)
                            216 LOAD_ATTR                4 (url)
                            226 LOAD_CONST               2 (True)
                            228 KW_NAMES                 3
                            230 PRECALL                  2
                            234 CALL                     2
                            244 STORE_FAST               1 (response)
                
-               577         246 LOAD_FAST                0 (self)
+               588         246 LOAD_FAST                0 (self)
                            248 LOAD_METHOD              5 (assertEqual)
                
-               578         270 LOAD_FAST                1 (response)
+               589         270 LOAD_FAST                1 (response)
                            272 LOAD_ATTR                8 (headers)
                            282 LOAD_CONST               4 ('HX-Redirect')
                            284 BINARY_SUBSCR
                            294 LOAD_FAST                0 (self)
                            296 LOAD_ATTR                9 (subcategory)
                            306 LOAD_METHOD             10 (get_absolute_url)
                            328 PRECALL                  0
                            332 CALL                     0
                
-               577         342 PRECALL                  2
+               588         342 PRECALL                  2
                            346 CALL                     2
                            356 POP_TOP
                
-               580         358 LOAD_FAST                0 (self)
+               591         358 LOAD_FAST                0 (self)
                            360 LOAD_METHOD              5 (assertEqual)
                            382 LOAD_GLOBAL             22 (Thread)
                            394 LOAD_ATTR               12 (objects)
                            404 LOAD_METHOD             13 (count)
                            426 PRECALL                  0
                            430 CALL                     0
                            440 LOAD_CONST               5 (0)
@@ -5550,49 +5672,49 @@
                   0
                names      ('client', 'force_login', 'user', 'get', 'url', 'assertEqual', 'status_code', 'delete', 'headers', 'subcategory', 'get_absolute_url', 'Thread', 'objects', 'count')
                varnames   ('self', 'response')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'test_thread_delete'
-               firstlineno 569
+               firstlineno 580
                lnotab 0x02013e013e0236024202180148ff1003
             None
          names      ('__name__', '__module__', '__qualname__', 'setUp', 'test_redirect_unauthenticated_user', 'test_is_author', 'test_thread_delete')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
          name       'ThreadDeleteViewTestCase'
-         firstlineno 541
+         firstlineno 552
          lnotab 0x0a01060d06050609
       'ThreadDeleteViewTestCase'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a02640184005a03640284005a04640384005a0564
             045300
-         583           0 RESUME                   0
+         594           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('PostCreateViewTestCase')
                        8 STORE_NAME               2 (__qualname__)
          
-         584          10 LOAD_CONST               1 (<code object setUp, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 584>)
+         595          10 LOAD_CONST               1 (<code object setUp, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 595>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (setUp)
          
-         596          16 LOAD_CONST               2 (<code object test_redirect_unauthenticated_user, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 596>)
+         607          16 LOAD_CONST               2 (<code object test_redirect_unauthenticated_user, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 607>)
                       18 MAKE_FUNCTION            0
                       20 STORE_NAME               4 (test_redirect_unauthenticated_user)
          
-         601          22 LOAD_CONST               3 (<code object test_post_create, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 601>)
+         612          22 LOAD_CONST               3 (<code object test_post_create, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 612>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               5 (test_post_create)
                       28 LOAD_CONST               4 (None)
                       30 RETURN_VALUE
          consts
             'PostCreateViewTestCase'
             code
@@ -5612,76 +5734,76 @@
                   0800000000000000006401ac04a6030000ab0300000000000000007c005f
                   0a00000000000000007416000000000000000000006a0300000000000000
                   00a00700000000000000000000000000000000000000007c006a0a000000
                   00000000007c006a05000000000000000064016401ac05a6040000ab0400
                   000000000000007c005f0c0000000000000000741b000000000000000000
                   0064067c006a0c00000000000000006a0e00000000000000006701ac07a6
                   020000ab0200000000000000007c005f0f000000000000000064005300
-               584           0 RESUME                   0
+               595           0 RESUME                   0
                
-               585           2 LOAD_GLOBAL              1 (NULL + Client)
+               596           2 LOAD_GLOBAL              1 (NULL + Client)
                             14 PRECALL                  0
                             18 CALL                     0
                             28 LOAD_FAST                0 (self)
                             30 STORE_ATTR               1 (client)
                
-               586          40 LOAD_GLOBAL              4 (User)
+               597          40 LOAD_GLOBAL              4 (User)
                             52 LOAD_ATTR                3 (objects)
                             62 LOAD_METHOD              4 (create_user)
                             84 LOAD_CONST               1 ('test')
                             86 LOAD_CONST               1 ('test')
                             88 KW_NAMES                 2
                             90 PRECALL                  2
                             94 CALL                     2
                            104 LOAD_FAST                0 (self)
                            106 STORE_ATTR               5 (user)
                
-               587         116 LOAD_GLOBAL             12 (Category)
+               598         116 LOAD_GLOBAL             12 (Category)
                            128 LOAD_ATTR                3 (objects)
                            138 LOAD_METHOD              7 (create)
                            160 LOAD_CONST               1 ('test')
                            162 KW_NAMES                 3
                            164 PRECALL                  1
                            168 CALL                     1
                            178 LOAD_FAST                0 (self)
                            180 STORE_ATTR               8 (category)
                
-               588         190 LOAD_GLOBAL             18 (Subcategory)
+               599         190 LOAD_GLOBAL             18 (Subcategory)
                            202 LOAD_ATTR                3 (objects)
                            212 LOAD_METHOD              7 (create)
                
-               589         234 LOAD_CONST               1 ('test')
+               600         234 LOAD_CONST               1 ('test')
                            236 LOAD_FAST                0 (self)
                            238 LOAD_ATTR                8 (category)
                            248 LOAD_CONST               1 ('test')
                
-               588         250 KW_NAMES                 4
+               599         250 KW_NAMES                 4
                            252 PRECALL                  3
                            256 CALL                     3
                            266 LOAD_FAST                0 (self)
                            268 STORE_ATTR              10 (subcategory)
                
-               591         278 LOAD_GLOBAL             22 (Thread)
+               602         278 LOAD_GLOBAL             22 (Thread)
                            290 LOAD_ATTR                3 (objects)
                            300 LOAD_METHOD              7 (create)
                
-               592         322 LOAD_FAST                0 (self)
+               603         322 LOAD_FAST                0 (self)
                            324 LOAD_ATTR               10 (subcategory)
                            334 LOAD_FAST                0 (self)
                            336 LOAD_ATTR                5 (user)
                            346 LOAD_CONST               1 ('test')
                            348 LOAD_CONST               1 ('test')
                
-               591         350 KW_NAMES                 5
+               602         350 KW_NAMES                 5
                            352 PRECALL                  4
                            356 CALL                     4
                            366 LOAD_FAST                0 (self)
                            368 STORE_ATTR              12 (thread)
                
-               594         378 LOAD_GLOBAL             27 (NULL + reverse)
+               605         378 LOAD_GLOBAL             27 (NULL + reverse)
                            390 LOAD_CONST               6 ('punkweb_bb:post_create')
                            392 LOAD_FAST                0 (self)
                            394 LOAD_ATTR               12 (thread)
                            404 LOAD_ATTR               14 (id)
                            414 BUILD_LIST               1
                            416 KW_NAMES                 7
                            418 PRECALL                  2
@@ -5701,40 +5823,40 @@
                   ('args',)
                names      ('Client', 'client', 'User', 'objects', 'create_user', 'user', 'Category', 'create', 'category', 'Subcategory', 'subcategory', 'Thread', 'thread', 'reverse', 'id', 'url')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'setUp'
-               firstlineno 584
+               firstlineno 595
                lnotab 0x020126014c014a012c0110ff1c032c011cff1c03
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 6
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c006a020000000000000000a6010000ab010000000000
                   0000007d017c00a00300000000000000000000000000000000000000007c
                   017409000000000000000000006401a6010000ab0100000000000000009b
                   0064027c006a0200000000000000009b009d03a6020000ab020000000000
                   000000010064005300
-               596           0 RESUME                   0
+               607           0 RESUME                   0
                
-               597           2 LOAD_FAST                0 (self)
+               608           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (client)
                             14 LOAD_METHOD              1 (get)
                             36 LOAD_FAST                0 (self)
                             38 LOAD_ATTR                2 (url)
                             48 PRECALL                  1
                             52 CALL                     1
                             62 STORE_FAST               1 (response)
                
-               599          64 LOAD_FAST                0 (self)
+               610          64 LOAD_FAST                0 (self)
                             66 LOAD_METHOD              3 (assertRedirects)
                             88 LOAD_FAST                1 (response)
                             90 LOAD_GLOBAL              9 (NULL + reverse)
                            102 LOAD_CONST               1 ('punkweb_bb:login')
                            104 PRECALL                  1
                            108 CALL                     1
                            118 FORMAT_VALUE             0
@@ -5754,15 +5876,15 @@
                   '?next='
                names      ('client', 'get', 'url', 'assertRedirects', 'reverse')
                varnames   ('self', 'response')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'test_redirect_unauthenticated_user'
-               firstlineno 596
+               firstlineno 607
                lnotab 0x02013e02
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 5
                flags     : 3
                code
@@ -5779,85 +5901,85 @@
                   00740a000000000000000000006a060000000000000000a00b0000000000
                   000000000000000000000000000000a6000000ab00000000000000000064
                   05a6020000ab02000000000000000001007c00a00a000000000000000000
                   00000000000000000000007c026a0200000000000000007c006a02000000
                   0000000000a6020000ab02000000000000000001007c00a00a0000000000
                   0000000000000000000000000000007c026a0c00000000000000007c006a
                   0c0000000000000000a6020000ab020000000000000000010064005300
-               601           0 RESUME                   0
+               612           0 RESUME                   0
                
-               602           2 LOAD_FAST                0 (self)
+               613           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (client)
                             14 LOAD_METHOD              1 (force_login)
                             36 LOAD_FAST                0 (self)
                             38 LOAD_ATTR                2 (user)
                             48 PRECALL                  1
                             52 CALL                     1
                             62 POP_TOP
                
-               604          64 LOAD_FAST                0 (self)
+               615          64 LOAD_FAST                0 (self)
                             66 LOAD_ATTR                0 (client)
                             76 LOAD_METHOD              3 (post)
                
-               605          98 LOAD_FAST                0 (self)
+               616          98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                4 (url)
                
-               607         110 LOAD_CONST               1 ('content')
+               618         110 LOAD_CONST               1 ('content')
                            112 LOAD_CONST               2 ('test')
                
-               606         114 BUILD_MAP                1
+               617         114 BUILD_MAP                1
                
-               609         116 LOAD_CONST               3 (True)
+               620         116 LOAD_CONST               3 (True)
                
-               604         118 KW_NAMES                 4
+               615         118 KW_NAMES                 4
                            120 PRECALL                  3
                            124 CALL                     3
                            134 STORE_FAST               1 (response)
                
-               612         136 LOAD_GLOBAL             10 (Post)
+               623         136 LOAD_GLOBAL             10 (Post)
                            148 LOAD_ATTR                6 (objects)
                            158 LOAD_METHOD              7 (first)
                            180 PRECALL                  0
                            184 CALL                     0
                            194 STORE_FAST               2 (new_post)
                
-               614         196 LOAD_FAST                0 (self)
+               625         196 LOAD_FAST                0 (self)
                            198 LOAD_METHOD              8 (assertRedirects)
                            220 LOAD_FAST                1 (response)
                            222 LOAD_FAST                2 (new_post)
                            224 LOAD_METHOD              9 (get_absolute_url)
                            246 PRECALL                  0
                            250 CALL                     0
                            260 PRECALL                  2
                            264 CALL                     2
                            274 POP_TOP
                
-               615         276 LOAD_FAST                0 (self)
+               626         276 LOAD_FAST                0 (self)
                            278 LOAD_METHOD             10 (assertEqual)
                            300 LOAD_GLOBAL             10 (Post)
                            312 LOAD_ATTR                6 (objects)
                            322 LOAD_METHOD             11 (count)
                            344 PRECALL                  0
                            348 CALL                     0
                            358 LOAD_CONST               5 (1)
                            360 PRECALL                  2
                            364 CALL                     2
                            374 POP_TOP
                
-               616         376 LOAD_FAST                0 (self)
+               627         376 LOAD_FAST                0 (self)
                            378 LOAD_METHOD             10 (assertEqual)
                            400 LOAD_FAST                2 (new_post)
                            402 LOAD_ATTR                2 (user)
                            412 LOAD_FAST                0 (self)
                            414 LOAD_ATTR                2 (user)
                            424 PRECALL                  2
                            428 CALL                     2
                            438 POP_TOP
                
-               617         440 LOAD_FAST                0 (self)
+               628         440 LOAD_FAST                0 (self)
                            442 LOAD_METHOD             10 (assertEqual)
                            464 LOAD_FAST                2 (new_post)
                            466 LOAD_ATTR               12 (thread)
                            476 LOAD_FAST                0 (self)
                            478 LOAD_ATTR               12 (thread)
                            488 PRECALL                  2
                            492 CALL                     2
@@ -5873,53 +5995,53 @@
                   1
                names      ('client', 'force_login', 'user', 'post', 'url', 'Post', 'objects', 'first', 'assertRedirects', 'get_absolute_url', 'assertEqual', 'count', 'thread')
                varnames   ('self', 'response', 'new_post')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'test_post_create'
-               firstlineno 601
+               firstlineno 612
                lnotab 0x02013e0222010c0204ff020302fb12083c02500164014001
             None
          names      ('__name__', '__module__', '__qualname__', 'setUp', 'test_redirect_unauthenticated_user', 'test_post_create')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
          name       'PostCreateViewTestCase'
-         firstlineno 583
+         firstlineno 594
          lnotab 0x0a01060c0605
       'PostCreateViewTestCase'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a02640184005a03640284005a04640384005a0564
             0484005a0664055300
-         620           0 RESUME                   0
+         631           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('PostUpdateViewTestCase')
                        8 STORE_NAME               2 (__qualname__)
          
-         621          10 LOAD_CONST               1 (<code object setUp, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 621>)
+         632          10 LOAD_CONST               1 (<code object setUp, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 632>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (setUp)
          
-         637          16 LOAD_CONST               2 (<code object test_redirect_unauthenticated_user, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 637>)
+         648          16 LOAD_CONST               2 (<code object test_redirect_unauthenticated_user, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 648>)
                       18 MAKE_FUNCTION            0
                       20 STORE_NAME               4 (test_redirect_unauthenticated_user)
          
-         642          22 LOAD_CONST               3 (<code object test_is_author, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 642>)
+         653          22 LOAD_CONST               3 (<code object test_is_author, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 653>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               5 (test_is_author)
          
-         651          28 LOAD_CONST               4 (<code object test_post_update, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 651>)
+         662          28 LOAD_CONST               4 (<code object test_post_update, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 662>)
                       30 MAKE_FUNCTION            0
                       32 STORE_NAME               6 (test_post_update)
                       34 LOAD_CONST               5 (None)
                       36 RETURN_VALUE
          consts
             'PostUpdateViewTestCase'
             code
@@ -5945,103 +6067,103 @@
                   00000064016401ac06a6040000ab0400000000000000007c005f0d000000
                   0000000000741c000000000000000000006a030000000000000000a00800
                   000000000000000000000000000000000000007c006a0d00000000000000
                   007c006a0500000000000000006401ac07a6030000ab0300000000000000
                   007c005f0f000000000000000074210000000000000000000064087c006a
                   0f00000000000000006a1100000000000000006701ac09a6020000ab0200
                   000000000000007c005f12000000000000000064005300
-               621           0 RESUME                   0
+               632           0 RESUME                   0
                
-               622           2 LOAD_GLOBAL              1 (NULL + Client)
+               633           2 LOAD_GLOBAL              1 (NULL + Client)
                             14 PRECALL                  0
                             18 CALL                     0
                             28 LOAD_FAST                0 (self)
                             30 STORE_ATTR               1 (client)
                
-               623          40 LOAD_GLOBAL              4 (User)
+               634          40 LOAD_GLOBAL              4 (User)
                             52 LOAD_ATTR                3 (objects)
                             62 LOAD_METHOD              4 (create_user)
                             84 LOAD_CONST               1 ('test')
                             86 LOAD_CONST               1 ('test')
                             88 KW_NAMES                 2
                             90 PRECALL                  2
                             94 CALL                     2
                            104 LOAD_FAST                0 (self)
                            106 STORE_ATTR               5 (user)
                
-               624         116 LOAD_GLOBAL              4 (User)
+               635         116 LOAD_GLOBAL              4 (User)
                            128 LOAD_ATTR                3 (objects)
                            138 LOAD_METHOD              4 (create_user)
                            160 LOAD_CONST               3 ('other')
                            162 LOAD_CONST               3 ('other')
                            164 KW_NAMES                 2
                            166 PRECALL                  2
                            170 CALL                     2
                            180 LOAD_FAST                0 (self)
                            182 STORE_ATTR               6 (other_user)
                
-               625         192 LOAD_GLOBAL             14 (Category)
+               636         192 LOAD_GLOBAL             14 (Category)
                            204 LOAD_ATTR                3 (objects)
                            214 LOAD_METHOD              8 (create)
                            236 LOAD_CONST               1 ('test')
                            238 KW_NAMES                 4
                            240 PRECALL                  1
                            244 CALL                     1
                            254 LOAD_FAST                0 (self)
                            256 STORE_ATTR               9 (category)
                
-               626         266 LOAD_GLOBAL             20 (Subcategory)
+               637         266 LOAD_GLOBAL             20 (Subcategory)
                            278 LOAD_ATTR                3 (objects)
                            288 LOAD_METHOD              8 (create)
                
-               627         310 LOAD_CONST               1 ('test')
+               638         310 LOAD_CONST               1 ('test')
                            312 LOAD_FAST                0 (self)
                            314 LOAD_ATTR                9 (category)
                            324 LOAD_CONST               1 ('test')
                
-               626         326 KW_NAMES                 5
+               637         326 KW_NAMES                 5
                            328 PRECALL                  3
                            332 CALL                     3
                            342 LOAD_FAST                0 (self)
                            344 STORE_ATTR              11 (subcategory)
                
-               629         354 LOAD_GLOBAL             24 (Thread)
+               640         354 LOAD_GLOBAL             24 (Thread)
                            366 LOAD_ATTR                3 (objects)
                            376 LOAD_METHOD              8 (create)
                
-               630         398 LOAD_FAST                0 (self)
+               641         398 LOAD_FAST                0 (self)
                            400 LOAD_ATTR               11 (subcategory)
                            410 LOAD_FAST                0 (self)
                            412 LOAD_ATTR                5 (user)
                            422 LOAD_CONST               1 ('test')
                            424 LOAD_CONST               1 ('test')
                
-               629         426 KW_NAMES                 6
+               640         426 KW_NAMES                 6
                            428 PRECALL                  4
                            432 CALL                     4
                            442 LOAD_FAST                0 (self)
                            444 STORE_ATTR              13 (thread)
                
-               632         454 LOAD_GLOBAL             28 (Post)
+               643         454 LOAD_GLOBAL             28 (Post)
                            466 LOAD_ATTR                3 (objects)
                            476 LOAD_METHOD              8 (create)
                
-               633         498 LOAD_FAST                0 (self)
+               644         498 LOAD_FAST                0 (self)
                            500 LOAD_ATTR               13 (thread)
                            510 LOAD_FAST                0 (self)
                            512 LOAD_ATTR                5 (user)
                            522 LOAD_CONST               1 ('test')
                
-               632         524 KW_NAMES                 7
+               643         524 KW_NAMES                 7
                            526 PRECALL                  3
                            530 CALL                     3
                            540 LOAD_FAST                0 (self)
                            542 STORE_ATTR              15 (post)
                
-               635         552 LOAD_GLOBAL             33 (NULL + reverse)
+               646         552 LOAD_GLOBAL             33 (NULL + reverse)
                            564 LOAD_CONST               8 ('punkweb_bb:post_update')
                            566 LOAD_FAST                0 (self)
                            568 LOAD_ATTR               15 (post)
                            578 LOAD_ATTR               17 (id)
                            588 BUILD_LIST               1
                            590 KW_NAMES                 9
                            592 PRECALL                  2
@@ -6063,40 +6185,40 @@
                   ('args',)
                names      ('Client', 'client', 'User', 'objects', 'create_user', 'user', 'other_user', 'Category', 'create', 'category', 'Subcategory', 'subcategory', 'Thread', 'thread', 'Post', 'post', 'reverse', 'id', 'url')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'setUp'
-               firstlineno 621
+               firstlineno 632
                lnotab 0x020126014c014c014a012c0110ff1c032c011cff1c032c011aff1c03
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 6
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c006a020000000000000000a6010000ab010000000000
                   0000007d017c00a00300000000000000000000000000000000000000007c
                   017409000000000000000000006401a6010000ab0100000000000000009b
                   0064027c006a0200000000000000009b009d03a6020000ab020000000000
                   000000010064005300
-               637           0 RESUME                   0
+               648           0 RESUME                   0
                
-               638           2 LOAD_FAST                0 (self)
+               649           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (client)
                             14 LOAD_METHOD              1 (get)
                             36 LOAD_FAST                0 (self)
                             38 LOAD_ATTR                2 (url)
                             48 PRECALL                  1
                             52 CALL                     1
                             62 STORE_FAST               1 (response)
                
-               640          64 LOAD_FAST                0 (self)
+               651          64 LOAD_FAST                0 (self)
                             66 LOAD_METHOD              3 (assertRedirects)
                             88 LOAD_FAST                1 (response)
                             90 LOAD_GLOBAL              9 (NULL + reverse)
                            102 LOAD_CONST               1 ('punkweb_bb:login')
                            104 PRECALL                  1
                            108 CALL                     1
                            118 FORMAT_VALUE             0
@@ -6116,15 +6238,15 @@
                   '?next='
                names      ('client', 'get', 'url', 'assertRedirects', 'reverse')
                varnames   ('self', 'response')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'test_redirect_unauthenticated_user'
-               firstlineno 637
+               firstlineno 648
                lnotab 0x02013e02
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
@@ -6137,62 +6259,62 @@
                   007c006a000000000000000000a001000000000000000000000000000000
                   00000000007c006a070000000000000000a6010000ab0100000000000000
                   0001007c006a000000000000000000a00300000000000000000000000000
                   000000000000007c006a040000000000000000a6010000ab010000000000
                   0000007d017c00a00500000000000000000000000000000000000000007c
                   016a0600000000000000006402a6020000ab020000000000000000010064
                   005300
-               642           0 RESUME                   0
+               653           0 RESUME                   0
                
-               643           2 LOAD_FAST                0 (self)
+               654           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (client)
                             14 LOAD_METHOD              1 (force_login)
                             36 LOAD_FAST                0 (self)
                             38 LOAD_ATTR                2 (other_user)
                             48 PRECALL                  1
                             52 CALL                     1
                             62 POP_TOP
                
-               644          64 LOAD_FAST                0 (self)
+               655          64 LOAD_FAST                0 (self)
                             66 LOAD_ATTR                0 (client)
                             76 LOAD_METHOD              3 (get)
                             98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                4 (url)
                            110 PRECALL                  1
                            114 CALL                     1
                            124 STORE_FAST               1 (response)
                
-               645         126 LOAD_FAST                0 (self)
+               656         126 LOAD_FAST                0 (self)
                            128 LOAD_METHOD              5 (assertEqual)
                            150 LOAD_FAST                1 (response)
                            152 LOAD_ATTR                6 (status_code)
                            162 LOAD_CONST               1 (404)
                            164 PRECALL                  2
                            168 CALL                     2
                            178 POP_TOP
                
-               647         180 LOAD_FAST                0 (self)
+               658         180 LOAD_FAST                0 (self)
                            182 LOAD_ATTR                0 (client)
                            192 LOAD_METHOD              1 (force_login)
                            214 LOAD_FAST                0 (self)
                            216 LOAD_ATTR                7 (user)
                            226 PRECALL                  1
                            230 CALL                     1
                            240 POP_TOP
                
-               648         242 LOAD_FAST                0 (self)
+               659         242 LOAD_FAST                0 (self)
                            244 LOAD_ATTR                0 (client)
                            254 LOAD_METHOD              3 (get)
                            276 LOAD_FAST                0 (self)
                            278 LOAD_ATTR                4 (url)
                            288 PRECALL                  1
                            292 CALL                     1
                            302 STORE_FAST               1 (response)
                
-               649         304 LOAD_FAST                0 (self)
+               660         304 LOAD_FAST                0 (self)
                            306 LOAD_METHOD              5 (assertEqual)
                            328 LOAD_FAST                1 (response)
                            330 LOAD_ATTR                6 (status_code)
                            340 LOAD_CONST               2 (200)
                            342 PRECALL                  2
                            346 CALL                     2
                            356 POP_TOP
@@ -6204,15 +6326,15 @@
                   200
                names      ('client', 'force_login', 'other_user', 'get', 'url', 'assertEqual', 'status_code', 'user')
                varnames   ('self', 'response')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'test_is_author'
-               firstlineno 642
+               firstlineno 653
                lnotab 0x02013e013e0136023e013e01
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
@@ -6228,82 +6350,82 @@
                   000000000000007c017c006a070000000000000000a00900000000000000
                   00000000000000000000000000a6000000ab000000000000000000a60200
                   00ab02000000000000000001007c006a070000000000000000a00a000000
                   0000000000000000000000000000000000a6000000ab0000000000000000
                   0001007c00a00500000000000000000000000000000000000000007c006a
                   0700000000000000006a0b00000000000000006403a6020000ab02000000
                   0000000000010064005300
-               651           0 RESUME                   0
+               662           0 RESUME                   0
                
-               652           2 LOAD_FAST                0 (self)
+               663           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (client)
                             14 LOAD_METHOD              1 (force_login)
                             36 LOAD_FAST                0 (self)
                             38 LOAD_ATTR                2 (user)
                             48 PRECALL                  1
                             52 CALL                     1
                             62 POP_TOP
                
-               653          64 LOAD_FAST                0 (self)
+               664          64 LOAD_FAST                0 (self)
                             66 LOAD_ATTR                0 (client)
                             76 LOAD_METHOD              3 (get)
                             98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                4 (url)
                            110 PRECALL                  1
                            114 CALL                     1
                            124 STORE_FAST               1 (response)
                
-               655         126 LOAD_FAST                0 (self)
+               666         126 LOAD_FAST                0 (self)
                            128 LOAD_METHOD              5 (assertEqual)
                            150 LOAD_FAST                1 (response)
                            152 LOAD_ATTR                6 (status_code)
                            162 LOAD_CONST               1 (200)
                            164 PRECALL                  2
                            168 CALL                     2
                            178 POP_TOP
                
-               657         180 LOAD_FAST                0 (self)
+               668         180 LOAD_FAST                0 (self)
                            182 LOAD_ATTR                0 (client)
                            192 LOAD_METHOD              7 (post)
                
-               658         214 LOAD_FAST                0 (self)
+               669         214 LOAD_FAST                0 (self)
                            216 LOAD_ATTR                4 (url)
                
-               660         226 LOAD_CONST               2 ('content')
+               671         226 LOAD_CONST               2 ('content')
                            228 LOAD_CONST               3 ('edit')
                
-               659         230 BUILD_MAP                1
+               670         230 BUILD_MAP                1
                
-               662         232 LOAD_CONST               4 (True)
+               673         232 LOAD_CONST               4 (True)
                
-               657         234 KW_NAMES                 5
+               668         234 KW_NAMES                 5
                            236 PRECALL                  3
                            240 CALL                     3
                            250 STORE_FAST               1 (response)
                
-               665         252 LOAD_FAST                0 (self)
+               676         252 LOAD_FAST                0 (self)
                            254 LOAD_METHOD              8 (assertRedirects)
                            276 LOAD_FAST                1 (response)
                            278 LOAD_FAST                0 (self)
                            280 LOAD_ATTR                7 (post)
                            290 LOAD_METHOD              9 (get_absolute_url)
                            312 PRECALL                  0
                            316 CALL                     0
                            326 PRECALL                  2
                            330 CALL                     2
                            340 POP_TOP
                
-               666         342 LOAD_FAST                0 (self)
+               677         342 LOAD_FAST                0 (self)
                            344 LOAD_ATTR                7 (post)
                            354 LOAD_METHOD             10 (refresh_from_db)
                            376 PRECALL                  0
                            380 CALL                     0
                            390 POP_TOP
                
-               667         392 LOAD_FAST                0 (self)
+               678         392 LOAD_FAST                0 (self)
                            394 LOAD_METHOD              5 (assertEqual)
                            416 LOAD_FAST                0 (self)
                            418 LOAD_ATTR                7 (post)
                            428 LOAD_ATTR               11 (_content_rendered)
                            438 LOAD_CONST               3 ('edit')
                            440 PRECALL                  2
                            444 CALL                     2
@@ -6319,53 +6441,53 @@
                   ('follow',)
                names      ('client', 'force_login', 'user', 'get', 'url', 'assertEqual', 'status_code', 'post', 'assertRedirects', 'get_absolute_url', 'refresh_from_db', '_content_rendered')
                varnames   ('self', 'response')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'test_post_update'
-               firstlineno 651
+               firstlineno 662
                lnotab 0x02013e013e02360222010c0204ff020302fb12085a013201
             None
          names      ('__name__', '__module__', '__qualname__', 'setUp', 'test_redirect_unauthenticated_user', 'test_is_author', 'test_post_update')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
          name       'PostUpdateViewTestCase'
-         firstlineno 620
+         firstlineno 631
          lnotab 0x0a01061006050609
       'PostUpdateViewTestCase'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a02640184005a03640284005a04640384005a0564
             0484005a0664055300
-         670           0 RESUME                   0
+         681           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('PostDeleteViewTestCase')
                        8 STORE_NAME               2 (__qualname__)
          
-         671          10 LOAD_CONST               1 (<code object setUp, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 671>)
+         682          10 LOAD_CONST               1 (<code object setUp, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 682>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (setUp)
          
-         687          16 LOAD_CONST               2 (<code object test_redirect_unauthenticated_user, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 687>)
+         698          16 LOAD_CONST               2 (<code object test_redirect_unauthenticated_user, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 698>)
                       18 MAKE_FUNCTION            0
                       20 STORE_NAME               4 (test_redirect_unauthenticated_user)
          
-         692          22 LOAD_CONST               3 (<code object test_is_author, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 692>)
+         703          22 LOAD_CONST               3 (<code object test_is_author, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 703>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               5 (test_is_author)
          
-         701          28 LOAD_CONST               4 (<code object test_post_delete, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 701>)
+         712          28 LOAD_CONST               4 (<code object test_post_delete, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 712>)
                       30 MAKE_FUNCTION            0
                       32 STORE_NAME               6 (test_post_delete)
                       34 LOAD_CONST               5 (None)
                       36 RETURN_VALUE
          consts
             'PostDeleteViewTestCase'
             code
@@ -6391,103 +6513,103 @@
                   00000064016401ac06a6040000ab0400000000000000007c005f0d000000
                   0000000000741c000000000000000000006a030000000000000000a00800
                   000000000000000000000000000000000000007c006a0d00000000000000
                   007c006a0500000000000000006401ac07a6030000ab0300000000000000
                   007c005f0f000000000000000074210000000000000000000064087c006a
                   0f00000000000000006a1100000000000000006701ac09a6020000ab0200
                   000000000000007c005f12000000000000000064005300
-               671           0 RESUME                   0
+               682           0 RESUME                   0
                
-               672           2 LOAD_GLOBAL              1 (NULL + Client)
+               683           2 LOAD_GLOBAL              1 (NULL + Client)
                             14 PRECALL                  0
                             18 CALL                     0
                             28 LOAD_FAST                0 (self)
                             30 STORE_ATTR               1 (client)
                
-               673          40 LOAD_GLOBAL              4 (User)
+               684          40 LOAD_GLOBAL              4 (User)
                             52 LOAD_ATTR                3 (objects)
                             62 LOAD_METHOD              4 (create_user)
                             84 LOAD_CONST               1 ('test')
                             86 LOAD_CONST               1 ('test')
                             88 KW_NAMES                 2
                             90 PRECALL                  2
                             94 CALL                     2
                            104 LOAD_FAST                0 (self)
                            106 STORE_ATTR               5 (user)
                
-               674         116 LOAD_GLOBAL              4 (User)
+               685         116 LOAD_GLOBAL              4 (User)
                            128 LOAD_ATTR                3 (objects)
                            138 LOAD_METHOD              4 (create_user)
                            160 LOAD_CONST               3 ('other')
                            162 LOAD_CONST               3 ('other')
                            164 KW_NAMES                 2
                            166 PRECALL                  2
                            170 CALL                     2
                            180 LOAD_FAST                0 (self)
                            182 STORE_ATTR               6 (other_user)
                
-               675         192 LOAD_GLOBAL             14 (Category)
+               686         192 LOAD_GLOBAL             14 (Category)
                            204 LOAD_ATTR                3 (objects)
                            214 LOAD_METHOD              8 (create)
                            236 LOAD_CONST               1 ('test')
                            238 KW_NAMES                 4
                            240 PRECALL                  1
                            244 CALL                     1
                            254 LOAD_FAST                0 (self)
                            256 STORE_ATTR               9 (category)
                
-               676         266 LOAD_GLOBAL             20 (Subcategory)
+               687         266 LOAD_GLOBAL             20 (Subcategory)
                            278 LOAD_ATTR                3 (objects)
                            288 LOAD_METHOD              8 (create)
                
-               677         310 LOAD_CONST               1 ('test')
+               688         310 LOAD_CONST               1 ('test')
                            312 LOAD_FAST                0 (self)
                            314 LOAD_ATTR                9 (category)
                            324 LOAD_CONST               1 ('test')
                
-               676         326 KW_NAMES                 5
+               687         326 KW_NAMES                 5
                            328 PRECALL                  3
                            332 CALL                     3
                            342 LOAD_FAST                0 (self)
                            344 STORE_ATTR              11 (subcategory)
                
-               679         354 LOAD_GLOBAL             24 (Thread)
+               690         354 LOAD_GLOBAL             24 (Thread)
                            366 LOAD_ATTR                3 (objects)
                            376 LOAD_METHOD              8 (create)
                
-               680         398 LOAD_FAST                0 (self)
+               691         398 LOAD_FAST                0 (self)
                            400 LOAD_ATTR               11 (subcategory)
                            410 LOAD_FAST                0 (self)
                            412 LOAD_ATTR                5 (user)
                            422 LOAD_CONST               1 ('test')
                            424 LOAD_CONST               1 ('test')
                
-               679         426 KW_NAMES                 6
+               690         426 KW_NAMES                 6
                            428 PRECALL                  4
                            432 CALL                     4
                            442 LOAD_FAST                0 (self)
                            444 STORE_ATTR              13 (thread)
                
-               682         454 LOAD_GLOBAL             28 (Post)
+               693         454 LOAD_GLOBAL             28 (Post)
                            466 LOAD_ATTR                3 (objects)
                            476 LOAD_METHOD              8 (create)
                
-               683         498 LOAD_FAST                0 (self)
+               694         498 LOAD_FAST                0 (self)
                            500 LOAD_ATTR               13 (thread)
                            510 LOAD_FAST                0 (self)
                            512 LOAD_ATTR                5 (user)
                            522 LOAD_CONST               1 ('test')
                
-               682         524 KW_NAMES                 7
+               693         524 KW_NAMES                 7
                            526 PRECALL                  3
                            530 CALL                     3
                            540 LOAD_FAST                0 (self)
                            542 STORE_ATTR              15 (post)
                
-               685         552 LOAD_GLOBAL             33 (NULL + reverse)
+               696         552 LOAD_GLOBAL             33 (NULL + reverse)
                            564 LOAD_CONST               8 ('punkweb_bb:post_delete')
                            566 LOAD_FAST                0 (self)
                            568 LOAD_ATTR               15 (post)
                            578 LOAD_ATTR               17 (id)
                            588 BUILD_LIST               1
                            590 KW_NAMES                 9
                            592 PRECALL                  2
@@ -6509,40 +6631,40 @@
                   ('args',)
                names      ('Client', 'client', 'User', 'objects', 'create_user', 'user', 'other_user', 'Category', 'create', 'category', 'Subcategory', 'subcategory', 'Thread', 'thread', 'Post', 'post', 'reverse', 'id', 'url')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'setUp'
-               firstlineno 671
+               firstlineno 682
                lnotab 0x020126014c014c014a012c0110ff1c032c011cff1c032c011aff1c03
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 6
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c006a020000000000000000a6010000ab010000000000
                   0000007d017c00a00300000000000000000000000000000000000000007c
                   017409000000000000000000006401a6010000ab0100000000000000009b
                   0064027c006a0200000000000000009b009d03a6020000ab020000000000
                   000000010064005300
-               687           0 RESUME                   0
+               698           0 RESUME                   0
                
-               688           2 LOAD_FAST                0 (self)
+               699           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (client)
                             14 LOAD_METHOD              1 (get)
                             36 LOAD_FAST                0 (self)
                             38 LOAD_ATTR                2 (url)
                             48 PRECALL                  1
                             52 CALL                     1
                             62 STORE_FAST               1 (response)
                
-               690          64 LOAD_FAST                0 (self)
+               701          64 LOAD_FAST                0 (self)
                             66 LOAD_METHOD              3 (assertRedirects)
                             88 LOAD_FAST                1 (response)
                             90 LOAD_GLOBAL              9 (NULL + reverse)
                            102 LOAD_CONST               1 ('punkweb_bb:login')
                            104 PRECALL                  1
                            108 CALL                     1
                            118 FORMAT_VALUE             0
@@ -6562,15 +6684,15 @@
                   '?next='
                names      ('client', 'get', 'url', 'assertRedirects', 'reverse')
                varnames   ('self', 'response')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'test_redirect_unauthenticated_user'
-               firstlineno 687
+               firstlineno 698
                lnotab 0x02013e02
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
@@ -6583,62 +6705,62 @@
                   007c006a000000000000000000a001000000000000000000000000000000
                   00000000007c006a070000000000000000a6010000ab0100000000000000
                   0001007c006a000000000000000000a00300000000000000000000000000
                   000000000000007c006a040000000000000000a6010000ab010000000000
                   0000007d017c00a00500000000000000000000000000000000000000007c
                   016a0600000000000000006402a6020000ab020000000000000000010064
                   005300
-               692           0 RESUME                   0
+               703           0 RESUME                   0
                
-               693           2 LOAD_FAST                0 (self)
+               704           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (client)
                             14 LOAD_METHOD              1 (force_login)
                             36 LOAD_FAST                0 (self)
                             38 LOAD_ATTR                2 (other_user)
                             48 PRECALL                  1
                             52 CALL                     1
                             62 POP_TOP
                
-               694          64 LOAD_FAST                0 (self)
+               705          64 LOAD_FAST                0 (self)
                             66 LOAD_ATTR                0 (client)
                             76 LOAD_METHOD              3 (get)
                             98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                4 (url)
                            110 PRECALL                  1
                            114 CALL                     1
                            124 STORE_FAST               1 (response)
                
-               695         126 LOAD_FAST                0 (self)
+               706         126 LOAD_FAST                0 (self)
                            128 LOAD_METHOD              5 (assertEqual)
                            150 LOAD_FAST                1 (response)
                            152 LOAD_ATTR                6 (status_code)
                            162 LOAD_CONST               1 (404)
                            164 PRECALL                  2
                            168 CALL                     2
                            178 POP_TOP
                
-               697         180 LOAD_FAST                0 (self)
+               708         180 LOAD_FAST                0 (self)
                            182 LOAD_ATTR                0 (client)
                            192 LOAD_METHOD              1 (force_login)
                            214 LOAD_FAST                0 (self)
                            216 LOAD_ATTR                7 (user)
                            226 PRECALL                  1
                            230 CALL                     1
                            240 POP_TOP
                
-               698         242 LOAD_FAST                0 (self)
+               709         242 LOAD_FAST                0 (self)
                            244 LOAD_ATTR                0 (client)
                            254 LOAD_METHOD              3 (get)
                            276 LOAD_FAST                0 (self)
                            278 LOAD_ATTR                4 (url)
                            288 PRECALL                  1
                            292 CALL                     1
                            302 STORE_FAST               1 (response)
                
-               699         304 LOAD_FAST                0 (self)
+               710         304 LOAD_FAST                0 (self)
                            306 LOAD_METHOD              5 (assertEqual)
                            328 LOAD_FAST                1 (response)
                            330 LOAD_ATTR                6 (status_code)
                            340 LOAD_CONST               2 (200)
                            342 PRECALL                  2
                            346 CALL                     2
                            356 POP_TOP
@@ -6650,15 +6772,15 @@
                   200
                names      ('client', 'force_login', 'other_user', 'get', 'url', 'assertEqual', 'status_code', 'user')
                varnames   ('self', 'response')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'test_is_author'
-               firstlineno 692
+               firstlineno 703
                lnotab 0x02013e013e0136023e013e01
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
@@ -6674,72 +6796,72 @@
                   007c016a0800000000000000006404190000000000000000007c006a0900
                   00000000000000a00a0000000000000000000000000000000000000000a6
                   000000ab000000000000000000a6020000ab02000000000000000001007c
                   00a005000000000000000000000000000000000000000074160000000000
                   00000000006a0c0000000000000000a00d00000000000000000000000000
                   00000000000000a6000000ab0000000000000000006405a6020000ab0200
                   00000000000000010064005300
-               701           0 RESUME                   0
+               712           0 RESUME                   0
                
-               702           2 LOAD_FAST                0 (self)
+               713           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (client)
                             14 LOAD_METHOD              1 (force_login)
                             36 LOAD_FAST                0 (self)
                             38 LOAD_ATTR                2 (user)
                             48 PRECALL                  1
                             52 CALL                     1
                             62 POP_TOP
                
-               703          64 LOAD_FAST                0 (self)
+               714          64 LOAD_FAST                0 (self)
                             66 LOAD_ATTR                0 (client)
                             76 LOAD_METHOD              3 (get)
                             98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                4 (url)
                            110 PRECALL                  1
                            114 CALL                     1
                            124 STORE_FAST               1 (response)
                
-               705         126 LOAD_FAST                0 (self)
+               716         126 LOAD_FAST                0 (self)
                            128 LOAD_METHOD              5 (assertEqual)
                            150 LOAD_FAST                1 (response)
                            152 LOAD_ATTR                6 (status_code)
                            162 LOAD_CONST               1 (200)
                            164 PRECALL                  2
                            168 CALL                     2
                            178 POP_TOP
                
-               707         180 LOAD_FAST                0 (self)
+               718         180 LOAD_FAST                0 (self)
                            182 LOAD_ATTR                0 (client)
                            192 LOAD_METHOD              7 (delete)
                            214 LOAD_FAST                0 (self)
                            216 LOAD_ATTR                4 (url)
                            226 LOAD_CONST               2 (True)
                            228 KW_NAMES                 3
                            230 PRECALL                  2
                            234 CALL                     2
                            244 STORE_FAST               1 (response)
                
-               709         246 LOAD_FAST                0 (self)
+               720         246 LOAD_FAST                0 (self)
                            248 LOAD_METHOD              5 (assertEqual)
                
-               710         270 LOAD_FAST                1 (response)
+               721         270 LOAD_FAST                1 (response)
                            272 LOAD_ATTR                8 (headers)
                            282 LOAD_CONST               4 ('HX-Redirect')
                            284 BINARY_SUBSCR
                            294 LOAD_FAST                0 (self)
                            296 LOAD_ATTR                9 (thread)
                            306 LOAD_METHOD             10 (get_absolute_url)
                            328 PRECALL                  0
                            332 CALL                     0
                
-               709         342 PRECALL                  2
+               720         342 PRECALL                  2
                            346 CALL                     2
                            356 POP_TOP
                
-               712         358 LOAD_FAST                0 (self)
+               723         358 LOAD_FAST                0 (self)
                            360 LOAD_METHOD              5 (assertEqual)
                            382 LOAD_GLOBAL             22 (Post)
                            394 LOAD_ATTR               12 (objects)
                            404 LOAD_METHOD             13 (count)
                            426 PRECALL                  0
                            430 CALL                     0
                            440 LOAD_CONST               5 (0)
@@ -6757,49 +6879,49 @@
                   0
                names      ('client', 'force_login', 'user', 'get', 'url', 'assertEqual', 'status_code', 'delete', 'headers', 'thread', 'get_absolute_url', 'Post', 'objects', 'count')
                varnames   ('self', 'response')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'test_post_delete'
-               firstlineno 701
+               firstlineno 712
                lnotab 0x02013e013e0236024202180148ff1003
             None
          names      ('__name__', '__module__', '__qualname__', 'setUp', 'test_redirect_unauthenticated_user', 'test_is_author', 'test_post_delete')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
          name       'PostDeleteViewTestCase'
-         firstlineno 670
+         firstlineno 681
          lnotab 0x0a01061006050609
       'PostDeleteViewTestCase'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a02640184005a03640284005a04640384005a0564
             045300
-         715           0 RESUME                   0
+         726           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ShoutCreateViewTestCase')
                        8 STORE_NAME               2 (__qualname__)
          
-         716          10 LOAD_CONST               1 (<code object setUp, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 716>)
+         727          10 LOAD_CONST               1 (<code object setUp, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 727>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (setUp)
          
-         721          16 LOAD_CONST               2 (<code object test_unauthenticated, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 721>)
+         732          16 LOAD_CONST               2 (<code object test_unauthenticated, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 732>)
                       18 MAKE_FUNCTION            0
                       20 STORE_NAME               4 (test_unauthenticated)
          
-         734          22 LOAD_CONST               3 (<code object test_shout_create, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 734>)
+         745          22 LOAD_CONST               3 (<code object test_shout_create, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py", line 745>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               5 (test_shout_create)
                       28 LOAD_CONST               4 (None)
                       30 RETURN_VALUE
          consts
             'ShoutCreateViewTestCase'
             code
@@ -6810,34 +6932,34 @@
                code
                   0x9700740100000000000000000000a6000000ab0000000000000000007c
                   005f0100000000000000007404000000000000000000006a030000000000
                   000000a004000000000000000000000000000000000000000064016401ac
                   02a6020000ab0200000000000000007c005f050000000000000000740d00
                   0000000000000000006403a6010000ab0100000000000000007c005f0700
                   0000000000000064005300
-               716           0 RESUME                   0
+               727           0 RESUME                   0
                
-               717           2 LOAD_GLOBAL              1 (NULL + Client)
+               728           2 LOAD_GLOBAL              1 (NULL + Client)
                             14 PRECALL                  0
                             18 CALL                     0
                             28 LOAD_FAST                0 (self)
                             30 STORE_ATTR               1 (client)
                
-               718          40 LOAD_GLOBAL              4 (User)
+               729          40 LOAD_GLOBAL              4 (User)
                             52 LOAD_ATTR                3 (objects)
                             62 LOAD_METHOD              4 (create_user)
                             84 LOAD_CONST               1 ('test')
                             86 LOAD_CONST               1 ('test')
                             88 KW_NAMES                 2
                             90 PRECALL                  2
                             94 CALL                     2
                            104 LOAD_FAST                0 (self)
                            106 STORE_ATTR               5 (user)
                
-               719         116 LOAD_GLOBAL             13 (NULL + reverse)
+               730         116 LOAD_GLOBAL             13 (NULL + reverse)
                            128 LOAD_CONST               3 ('punkweb_bb:shout_create')
                            130 PRECALL                  1
                            134 CALL                     1
                            144 LOAD_FAST                0 (self)
                            146 STORE_ATTR               7 (url)
                            156 LOAD_CONST               0 (None)
                            158 RETURN_VALUE
@@ -6848,15 +6970,15 @@
                   'punkweb_bb:shout_create'
                names      ('Client', 'client', 'User', 'objects', 'create_user', 'user', 'reverse', 'url')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'setUp'
-               firstlineno 716
+               firstlineno 727
                lnotab 0x020126014c01
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
@@ -6866,54 +6988,54 @@
                   0000000000000000007c006a020000000000000000640164026901a60200
                   00ab02000000000000000001007c00a00400000000000000000000000000
                   00000000000000740a000000000000000000006a060000000000000000a0
                   070000000000000000000000000000000000000000a6000000ab00000000
                   00000000006403a6020000ab02000000000000000001007c00a004000000
                   00000000000000000000000000000000007c016a08000000000000000064
                   04a6020000ab020000000000000000010064005300
-               721           0 RESUME                   0
+               732           0 RESUME                   0
                
-               722           2 LOAD_FAST                0 (self)
+               733           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (client)
                             14 LOAD_METHOD              1 (get)
                             36 LOAD_FAST                0 (self)
                             38 LOAD_ATTR                2 (url)
                             48 PRECALL                  1
                             52 CALL                     1
                             62 STORE_FAST               1 (response)
                
-               724          64 LOAD_FAST                0 (self)
+               735          64 LOAD_FAST                0 (self)
                             66 LOAD_ATTR                0 (client)
                             76 LOAD_METHOD              3 (post)
                
-               725          98 LOAD_FAST                0 (self)
+               736          98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                2 (url)
                
-               727         110 LOAD_CONST               1 ('content')
+               738         110 LOAD_CONST               1 ('content')
                            112 LOAD_CONST               2 ('test')
                
-               726         114 BUILD_MAP                1
+               737         114 BUILD_MAP                1
                
-               724         116 PRECALL                  2
+               735         116 PRECALL                  2
                            120 CALL                     2
                            130 POP_TOP
                
-               731         132 LOAD_FAST                0 (self)
+               742         132 LOAD_FAST                0 (self)
                            134 LOAD_METHOD              4 (assertEqual)
                            156 LOAD_GLOBAL             10 (Shout)
                            168 LOAD_ATTR                6 (objects)
                            178 LOAD_METHOD              7 (count)
                            200 PRECALL                  0
                            204 CALL                     0
                            214 LOAD_CONST               3 (0)
                            216 PRECALL                  2
                            220 CALL                     2
                            230 POP_TOP
                
-               732         232 LOAD_FAST                0 (self)
+               743         232 LOAD_FAST                0 (self)
                            234 LOAD_METHOD              4 (assertEqual)
                            256 LOAD_FAST                1 (response)
                            258 LOAD_ATTR                8 (status_code)
                            268 LOAD_CONST               4 (200)
                            270 PRECALL                  2
                            274 CALL                     2
                            284 POP_TOP
@@ -6927,15 +7049,15 @@
                   200
                names      ('client', 'get', 'url', 'post', 'assertEqual', 'Shout', 'objects', 'count', 'status_code')
                varnames   ('self', 'response')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'test_unauthenticated'
-               firstlineno 721
+               firstlineno 732
                lnotab 0x02013e0222010c0204ff02fe10076401
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
@@ -6945,57 +7067,57 @@
                   0000000000000000007c006a0400000000000000006401640269016403ac
                   04a6030000ab0300000000000000007d017c00a005000000000000000000
                   0000000000000000000000740c000000000000000000006a070000000000
                   000000a0080000000000000000000000000000000000000000a6000000ab
                   0000000000000000006405a6020000ab02000000000000000001007c00a0
                   0500000000000000000000000000000000000000007c016a090000000000
                   0000006406a6020000ab020000000000000000010064005300
-               734           0 RESUME                   0
+               745           0 RESUME                   0
                
-               735           2 LOAD_FAST                0 (self)
+               746           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (client)
                             14 LOAD_METHOD              1 (force_login)
                             36 LOAD_FAST                0 (self)
                             38 LOAD_ATTR                2 (user)
                             48 PRECALL                  1
                             52 CALL                     1
                             62 POP_TOP
                
-               737          64 LOAD_FAST                0 (self)
+               748          64 LOAD_FAST                0 (self)
                             66 LOAD_ATTR                0 (client)
                             76 LOAD_METHOD              3 (post)
                
-               738          98 LOAD_FAST                0 (self)
+               749          98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                4 (url)
                
-               740         110 LOAD_CONST               1 ('content')
+               751         110 LOAD_CONST               1 ('content')
                            112 LOAD_CONST               2 ('test')
                
-               739         114 BUILD_MAP                1
+               750         114 BUILD_MAP                1
                
-               742         116 LOAD_CONST               3 (True)
+               753         116 LOAD_CONST               3 (True)
                
-               737         118 KW_NAMES                 4
+               748         118 KW_NAMES                 4
                            120 PRECALL                  3
                            124 CALL                     3
                            134 STORE_FAST               1 (response)
                
-               745         136 LOAD_FAST                0 (self)
+               756         136 LOAD_FAST                0 (self)
                            138 LOAD_METHOD              5 (assertEqual)
                            160 LOAD_GLOBAL             12 (Shout)
                            172 LOAD_ATTR                7 (objects)
                            182 LOAD_METHOD              8 (count)
                            204 PRECALL                  0
                            208 CALL                     0
                            218 LOAD_CONST               5 (1)
                            220 PRECALL                  2
                            224 CALL                     2
                            234 POP_TOP
                
-               746         236 LOAD_FAST                0 (self)
+               757         236 LOAD_FAST                0 (self)
                            238 LOAD_METHOD              5 (assertEqual)
                            260 LOAD_FAST                1 (response)
                            262 LOAD_ATTR                9 (status_code)
                            272 LOAD_CONST               6 (200)
                            274 PRECALL                  2
                            278 CALL                     2
                            288 POP_TOP
@@ -7011,30 +7133,30 @@
                   200
                names      ('client', 'force_login', 'user', 'post', 'url', 'assertEqual', 'Shout', 'objects', 'count', 'status_code')
                varnames   ('self', 'response')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'test_shout_create'
-               firstlineno 734
+               firstlineno 745
                lnotab 0x02013e0222010c0204ff020302fb12086401
             None
          names      ('__name__', '__module__', '__qualname__', 'setUp', 'test_unauthenticated', 'test_shout_create')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
          name       'ShoutCreateViewTestCase'
-         firstlineno 715
+         firstlineno 726
          lnotab 0x0a010605060d
       'ShoutCreateViewTestCase'
    names      ('math', 'django.contrib.auth', 'get_user_model', 'django.core.cache', 'cache', 'django.forms', 'ValidationError', 'django.test', 'Client', 'TestCase', 'django.urls', 'reverse', 'django.utils', 'timezone', 'punkweb_bb.models', 'Category', 'Post', 'Shout', 'Subcategory', 'Thread', 'profile_image_upload_to', 'punkweb_bb.response', 'htmx_redirect', 'User', 'HTMXRedirectTestCase', 'BoardProfileTestCase', 'CategoryTestCase', 'SubcategoryTestCase', 'ThreadTestCase', 'PostTestCase', 'ShoutTestCase', 'IndexViewTestCase', 'LoginViewTestCase', 'LogoutViewTestCase', 'SignupViewTestCase', 'SettingsViewTestCase', 'ThreadCreateViewTestCase', 'ThreadViewTestCase', 'ThreadUpdateViewTestCase', 'ThreadDeleteViewTestCase', 'PostCreateViewTestCase', 'PostUpdateViewTestCase', 'PostDeleteViewTestCase', 'ShoutCreateViewTestCase')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020108020c010c010c0110010c010c0220080c0214031c071c2a1c
-      0a1c3b1c681c271c091c241c151c0e1c191c1e1c321c171c311c2a1c251c
+      0a1c3b1c681c271c091c2f1c151c0e1c191c1e1c321c171c311c2a1c251c
       321c2d
```

### Comparing `punkweb_bb-0.1.3/punkweb_bb/__pycache__/urls.cpython-311.pyc` & `punkweb_bb-0.1.4/punkweb_bb/__pycache__/urls.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/__pycache__/views.cpython-311.pyc` & `punkweb_bb-0.1.4/punkweb_bb/__pycache__/views.cpython-311.pyc`

 * *Files 9% similar despite different names*

#### Python bytecode

```diff
@@ -1,35 +1,36 @@
 magic:    0xa70d0d0a
-moddate:  0x72c63966 (Tue May  7 06:13:06 2024 UTC)
-files sz: 10723
+moddate:  0x0a653c66 (Thu May  9 05:54:18 2024 UTC)
+files sz: 11036
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 3
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a026d035a036d045a046d
       055a050100640064036c066d075a070100640064046c086d095a09010064
       0064056c0a6d0b5a0b6d0c5a0c6d0d5a0d0100640064066c0e6d0f5a0f01
-      00640064076c106d115a116d125a126d135a136d145a146d155a156d165a
-      160100640064086c176d185a186d195a196d1a5a1a6d1b5a1b6d1c5a1c01
-      00640064096c1d6d1e5a1e01006400640a6c1f6d205a20010002006503a6
-      000000ab0000000000000000005a21640b84005a22640c84005a23640d84
-      005a24640e84005a25640f84005a26641084005a27020065076411ac12a6
-      010000ab01000000000000000064138400a6000000ab0000000000000000
-      005a28641484005a29020065076411ac12a6010000ab0100000000000000
-      0064158400a6000000ab0000000000000000005a2a641684005a2b020065
-      076411ac12a6010000ab01000000000000000064178400a6000000ab0000
-      000000000000005a2c020065076411ac12a6010000ab0100000000000000
-      0064188400a6000000ab0000000000000000005a2d020065076411ac12a6
+      00640064076c106d115a110100640064086c126d135a136d145a146d155a
+      156d165a166d175a176d185a180100640064096c196d1a5a1a6d1b5a1b6d
+      1c5a1c6d1d5a1d6d1e5a1e01006400640a6c1f6d205a2001006400640b6c
+      216d225a22010002006503a6000000ab0000000000000000005a23640c84
+      005a24640d84005a25640e84005a26640f84005a27641084005a28641184
+      005a29020065076412ac13a6010000ab01000000000000000064148400a6
+      000000ab0000000000000000005a2a641584005a2b020065076412ac13a6
+      010000ab01000000000000000064168400a6000000ab0000000000000000
+      005a2c641784005a2d020065076412ac13a6010000ab0100000000000000
+      0064188400a6000000ab0000000000000000005a2e020065076412ac13a6
       010000ab01000000000000000064198400a6000000ab0000000000000000
-      005a2e020065076411ac12a6010000ab010000000000000000641a8400a6
-      000000ab0000000000000000005a2f020065076411ac12a6010000ab0100
-      00000000000000641b8400a6000000ab0000000000000000005a30641c84
-      005a31641d84005a32641e84005a33641f84005a3464015300
+      005a2f020065076412ac13a6010000ab010000000000000000641a8400a6
+      000000ab0000000000000000005a30020065076412ac13a6010000ab0100
+      00000000000000641b8400a6000000ab0000000000000000005a31020065
+      076412ac13a6010000ab010000000000000000641c8400a6000000ab0000
+      000000000000005a32641d84005a33641e84005a34641f84005a35642084
+      005a3664015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (datetime)
                  8 STORE_NAME               0 (datetime)
    
@@ -75,235 +76,243 @@
                 80 LOAD_CONST               6 (('timezone',))
                 82 IMPORT_NAME             14 (django.utils)
                 84 IMPORT_FROM             15 (timezone)
                 86 STORE_NAME              15 (timezone)
                 88 POP_TOP
    
      9          90 LOAD_CONST               0 (0)
-                92 LOAD_CONST               7 (('BoardProfileModelForm', 'LoginForm', 'PostModelForm', 'ShoutModelForm', 'SignUpForm', 'ThreadModelForm'))
-                94 IMPORT_NAME             16 (punkweb_bb.forms)
-                96 IMPORT_FROM             17 (BoardProfileModelForm)
-                98 STORE_NAME              17 (BoardProfileModelForm)
-               100 IMPORT_FROM             18 (LoginForm)
-               102 STORE_NAME              18 (LoginForm)
-               104 IMPORT_FROM             19 (PostModelForm)
-               106 STORE_NAME              19 (PostModelForm)
-               108 IMPORT_FROM             20 (ShoutModelForm)
-               110 STORE_NAME              20 (ShoutModelForm)
-               112 IMPORT_FROM             21 (SignUpForm)
-               114 STORE_NAME              21 (SignUpForm)
-               116 IMPORT_FROM             22 (ThreadModelForm)
-               118 STORE_NAME              22 (ThreadModelForm)
-               120 POP_TOP
-   
-    17         122 LOAD_CONST               0 (0)
-               124 LOAD_CONST               8 (('Category', 'Post', 'Shout', 'Subcategory', 'Thread'))
-               126 IMPORT_NAME             23 (punkweb_bb.models)
-               128 IMPORT_FROM             24 (Category)
-               130 STORE_NAME              24 (Category)
-               132 IMPORT_FROM             25 (Post)
-               134 STORE_NAME              25 (Post)
-               136 IMPORT_FROM             26 (Shout)
-               138 STORE_NAME              26 (Shout)
-               140 IMPORT_FROM             27 (Subcategory)
-               142 STORE_NAME              27 (Subcategory)
-               144 IMPORT_FROM             28 (Thread)
-               146 STORE_NAME              28 (Thread)
-               148 POP_TOP
-   
-    18         150 LOAD_CONST               0 (0)
-               152 LOAD_CONST               9 (('paginate_qs',))
-               154 IMPORT_NAME             29 (punkweb_bb.pagination)
-               156 IMPORT_FROM             30 (paginate_qs)
-               158 STORE_NAME              30 (paginate_qs)
+                92 LOAD_CONST               7 (('guest_list',))
+                94 IMPORT_NAME             16 (punkweb_bb.guests)
+                96 IMPORT_FROM             17 (guest_list)
+                98 STORE_NAME              17 (guest_list)
+               100 POP_TOP
+   
+    10         102 LOAD_CONST               0 (0)
+               104 LOAD_CONST               8 (('BoardProfileModelForm', 'LoginForm', 'PostModelForm', 'ShoutModelForm', 'SignUpForm', 'ThreadModelForm'))
+               106 IMPORT_NAME             18 (punkweb_bb.forms)
+               108 IMPORT_FROM             19 (BoardProfileModelForm)
+               110 STORE_NAME              19 (BoardProfileModelForm)
+               112 IMPORT_FROM             20 (LoginForm)
+               114 STORE_NAME              20 (LoginForm)
+               116 IMPORT_FROM             21 (PostModelForm)
+               118 STORE_NAME              21 (PostModelForm)
+               120 IMPORT_FROM             22 (ShoutModelForm)
+               122 STORE_NAME              22 (ShoutModelForm)
+               124 IMPORT_FROM             23 (SignUpForm)
+               126 STORE_NAME              23 (SignUpForm)
+               128 IMPORT_FROM             24 (ThreadModelForm)
+               130 STORE_NAME              24 (ThreadModelForm)
+               132 POP_TOP
+   
+    18         134 LOAD_CONST               0 (0)
+               136 LOAD_CONST               9 (('Category', 'Post', 'Shout', 'Subcategory', 'Thread'))
+               138 IMPORT_NAME             25 (punkweb_bb.models)
+               140 IMPORT_FROM             26 (Category)
+               142 STORE_NAME              26 (Category)
+               144 IMPORT_FROM             27 (Post)
+               146 STORE_NAME              27 (Post)
+               148 IMPORT_FROM             28 (Shout)
+               150 STORE_NAME              28 (Shout)
+               152 IMPORT_FROM             29 (Subcategory)
+               154 STORE_NAME              29 (Subcategory)
+               156 IMPORT_FROM             30 (Thread)
+               158 STORE_NAME              30 (Thread)
                160 POP_TOP
    
     19         162 LOAD_CONST               0 (0)
-               164 LOAD_CONST              10 (('htmx_redirect',))
-               166 IMPORT_NAME             31 (punkweb_bb.response)
-               168 IMPORT_FROM             32 (htmx_redirect)
-               170 STORE_NAME              32 (htmx_redirect)
+               164 LOAD_CONST              10 (('paginate_qs',))
+               166 IMPORT_NAME             31 (punkweb_bb.pagination)
+               168 IMPORT_FROM             32 (paginate_qs)
+               170 STORE_NAME              32 (paginate_qs)
                172 POP_TOP
    
-    21         174 PUSH_NULL
-               176 LOAD_NAME                3 (get_user_model)
-               178 PRECALL                  0
-               182 CALL                     0
-               192 STORE_NAME              33 (User)
-   
-    24         194 LOAD_CONST              11 (<code object index_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 24>)
-               196 MAKE_FUNCTION            0
-               198 STORE_NAME              34 (index_view)
-   
-    50         200 LOAD_CONST              12 (<code object login_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 50>)
-               202 MAKE_FUNCTION            0
-               204 STORE_NAME              35 (login_view)
+    20         174 LOAD_CONST               0 (0)
+               176 LOAD_CONST              11 (('htmx_redirect',))
+               178 IMPORT_NAME             33 (punkweb_bb.response)
+               180 IMPORT_FROM             34 (htmx_redirect)
+               182 STORE_NAME              34 (htmx_redirect)
+               184 POP_TOP
+   
+    22         186 PUSH_NULL
+               188 LOAD_NAME                3 (get_user_model)
+               190 PRECALL                  0
+               194 CALL                     0
+               204 STORE_NAME              35 (User)
    
-    76         206 LOAD_CONST              13 (<code object logout_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 76>)
+    25         206 LOAD_CONST              12 (<code object index_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 25>)
                208 MAKE_FUNCTION            0
-               210 STORE_NAME              36 (logout_view)
+               210 STORE_NAME              36 (index_view)
    
-    81         212 LOAD_CONST              14 (<code object signup_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 81>)
+    57         212 LOAD_CONST              13 (<code object login_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 57>)
                214 MAKE_FUNCTION            0
-               216 STORE_NAME              37 (signup_view)
+               216 STORE_NAME              37 (login_view)
    
-   101         218 LOAD_CONST              15 (<code object profile_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 101>)
+    83         218 LOAD_CONST              14 (<code object logout_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 83>)
                220 MAKE_FUNCTION            0
-               222 STORE_NAME              38 (profile_view)
+               222 STORE_NAME              38 (logout_view)
    
-   110         224 LOAD_CONST              16 (<code object members_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 110>)
+    88         224 LOAD_CONST              15 (<code object signup_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 88>)
                226 MAKE_FUNCTION            0
-               228 STORE_NAME              39 (members_view)
+               228 STORE_NAME              39 (signup_view)
    
-   121         230 PUSH_NULL
-               232 LOAD_NAME                7 (login_required)
-               234 LOAD_CONST              17 ('/login/')
-               236 KW_NAMES                18
-               238 PRECALL                  1
-               242 CALL                     1
+   108         230 LOAD_CONST              16 (<code object profile_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 108>)
+               232 MAKE_FUNCTION            0
+               234 STORE_NAME              40 (profile_view)
    
-   122         252 LOAD_CONST              19 (<code object settings_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 121>)
-               254 MAKE_FUNCTION            0
+   117         236 LOAD_CONST              17 (<code object members_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 117>)
+               238 MAKE_FUNCTION            0
+               240 STORE_NAME              41 (members_view)
    
-   121         256 PRECALL                  0
-               260 CALL                     0
+   128         242 PUSH_NULL
+               244 LOAD_NAME                7 (login_required)
+               246 LOAD_CONST              18 ('/login/')
+               248 KW_NAMES                19
+               250 PRECALL                  1
+               254 CALL                     1
    
-   122         270 STORE_NAME              40 (settings_view)
+   129         264 LOAD_CONST              20 (<code object settings_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 128>)
+               266 MAKE_FUNCTION            0
    
-   144         272 LOAD_CONST              20 (<code object subcategory_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 144>)
-               274 MAKE_FUNCTION            0
-               276 STORE_NAME              41 (subcategory_view)
+   128         268 PRECALL                  0
+               272 CALL                     0
    
-   156         278 PUSH_NULL
-               280 LOAD_NAME                7 (login_required)
-               282 LOAD_CONST              17 ('/login/')
-               284 KW_NAMES                18
-               286 PRECALL                  1
-               290 CALL                     1
+   129         282 STORE_NAME              42 (settings_view)
    
-   157         300 LOAD_CONST              21 (<code object thread_create_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 156>)
-               302 MAKE_FUNCTION            0
+   151         284 LOAD_CONST              21 (<code object subcategory_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 151>)
+               286 MAKE_FUNCTION            0
+               288 STORE_NAME              43 (subcategory_view)
    
-   156         304 PRECALL                  0
-               308 CALL                     0
+   163         290 PUSH_NULL
+               292 LOAD_NAME                7 (login_required)
+               294 LOAD_CONST              18 ('/login/')
+               296 KW_NAMES                19
+               298 PRECALL                  1
+               302 CALL                     1
    
-   157         318 STORE_NAME              42 (thread_create_view)
+   164         312 LOAD_CONST              22 (<code object thread_create_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 163>)
+               314 MAKE_FUNCTION            0
    
-   183         320 LOAD_CONST              22 (<code object thread_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 183>)
-               322 MAKE_FUNCTION            0
-               324 STORE_NAME              43 (thread_view)
+   163         316 PRECALL                  0
+               320 CALL                     0
    
-   205         326 PUSH_NULL
-               328 LOAD_NAME                7 (login_required)
-               330 LOAD_CONST              17 ('/login/')
-               332 KW_NAMES                18
-               334 PRECALL                  1
-               338 CALL                     1
+   164         330 STORE_NAME              44 (thread_create_view)
    
-   206         348 LOAD_CONST              23 (<code object thread_update_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 205>)
-               350 MAKE_FUNCTION            0
+   190         332 LOAD_CONST              23 (<code object thread_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 190>)
+               334 MAKE_FUNCTION            0
+               336 STORE_NAME              45 (thread_view)
    
-   205         352 PRECALL                  0
-               356 CALL                     0
+   212         338 PUSH_NULL
+               340 LOAD_NAME                7 (login_required)
+               342 LOAD_CONST              18 ('/login/')
+               344 KW_NAMES                19
+               346 PRECALL                  1
+               350 CALL                     1
    
-   206         366 STORE_NAME              44 (thread_update_view)
+   213         360 LOAD_CONST              24 (<code object thread_update_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 212>)
+               362 MAKE_FUNCTION            0
    
-   226         368 PUSH_NULL
-               370 LOAD_NAME                7 (login_required)
-               372 LOAD_CONST              17 ('/login/')
-               374 KW_NAMES                18
-               376 PRECALL                  1
-               380 CALL                     1
+   212         364 PRECALL                  0
+               368 CALL                     0
    
-   227         390 LOAD_CONST              24 (<code object thread_delete_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 226>)
-               392 MAKE_FUNCTION            0
+   213         378 STORE_NAME              46 (thread_update_view)
    
-   226         394 PRECALL                  0
-               398 CALL                     0
+   233         380 PUSH_NULL
+               382 LOAD_NAME                7 (login_required)
+               384 LOAD_CONST              18 ('/login/')
+               386 KW_NAMES                19
+               388 PRECALL                  1
+               392 CALL                     1
    
-   227         408 STORE_NAME              45 (thread_delete_view)
+   234         402 LOAD_CONST              25 (<code object thread_delete_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 233>)
+               404 MAKE_FUNCTION            0
    
-   242         410 PUSH_NULL
-               412 LOAD_NAME                7 (login_required)
-               414 LOAD_CONST              17 ('/login/')
-               416 KW_NAMES                18
-               418 PRECALL                  1
-               422 CALL                     1
+   233         406 PRECALL                  0
+               410 CALL                     0
    
-   243         432 LOAD_CONST              25 (<code object post_create_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 242>)
-               434 MAKE_FUNCTION            0
+   234         420 STORE_NAME              47 (thread_delete_view)
    
-   242         436 PRECALL                  0
-               440 CALL                     0
+   249         422 PUSH_NULL
+               424 LOAD_NAME                7 (login_required)
+               426 LOAD_CONST              18 ('/login/')
+               428 KW_NAMES                19
+               430 PRECALL                  1
+               434 CALL                     1
    
-   243         450 STORE_NAME              46 (post_create_view)
+   250         444 LOAD_CONST              26 (<code object post_create_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 249>)
+               446 MAKE_FUNCTION            0
    
-   260         452 PUSH_NULL
-               454 LOAD_NAME                7 (login_required)
-               456 LOAD_CONST              17 ('/login/')
-               458 KW_NAMES                18
-               460 PRECALL                  1
-               464 CALL                     1
+   249         448 PRECALL                  0
+               452 CALL                     0
    
-   261         474 LOAD_CONST              26 (<code object post_update_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 260>)
-               476 MAKE_FUNCTION            0
+   250         462 STORE_NAME              48 (post_create_view)
    
-   260         478 PRECALL                  0
-               482 CALL                     0
+   267         464 PUSH_NULL
+               466 LOAD_NAME                7 (login_required)
+               468 LOAD_CONST              18 ('/login/')
+               470 KW_NAMES                19
+               472 PRECALL                  1
+               476 CALL                     1
    
-   261         492 STORE_NAME              47 (post_update_view)
+   268         486 LOAD_CONST              27 (<code object post_update_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 267>)
+               488 MAKE_FUNCTION            0
    
-   282         494 PUSH_NULL
-               496 LOAD_NAME                7 (login_required)
-               498 LOAD_CONST              17 ('/login/')
-               500 KW_NAMES                18
-               502 PRECALL                  1
-               506 CALL                     1
+   267         490 PRECALL                  0
+               494 CALL                     0
    
-   283         516 LOAD_CONST              27 (<code object post_delete_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 282>)
-               518 MAKE_FUNCTION            0
+   268         504 STORE_NAME              49 (post_update_view)
    
-   282         520 PRECALL                  0
-               524 CALL                     0
+   289         506 PUSH_NULL
+               508 LOAD_NAME                7 (login_required)
+               510 LOAD_CONST              18 ('/login/')
+               512 KW_NAMES                19
+               514 PRECALL                  1
+               518 CALL                     1
    
-   283         534 STORE_NAME              48 (post_delete_view)
+   290         528 LOAD_CONST              28 (<code object post_delete_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 289>)
+               530 MAKE_FUNCTION            0
    
-   298         536 LOAD_CONST              28 (<code object current_shouts, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 298>)
-               538 MAKE_FUNCTION            0
-               540 STORE_NAME              49 (current_shouts)
+   289         532 PRECALL                  0
+               536 CALL                     0
    
-   304         542 LOAD_CONST              29 (<code object shout_list_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 304>)
-               544 MAKE_FUNCTION            0
-               546 STORE_NAME              50 (shout_list_view)
+   290         546 STORE_NAME              50 (post_delete_view)
    
-   313         548 LOAD_CONST              30 (<code object shout_create_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 313>)
+   305         548 LOAD_CONST              29 (<code object current_shouts, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 305>)
                550 MAKE_FUNCTION            0
-               552 STORE_NAME              51 (shout_create_view)
+               552 STORE_NAME              51 (current_shouts)
    
-   336         554 LOAD_CONST              31 (<code object bbcode_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 336>)
+   311         554 LOAD_CONST              30 (<code object shout_list_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 311>)
                556 MAKE_FUNCTION            0
-               558 STORE_NAME              52 (bbcode_view)
-               560 LOAD_CONST               1 (None)
-               562 RETURN_VALUE
+               558 STORE_NAME              52 (shout_list_view)
+   
+   320         560 LOAD_CONST              31 (<code object shout_create_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 320>)
+               562 MAKE_FUNCTION            0
+               564 STORE_NAME              53 (shout_create_view)
+   
+   343         566 LOAD_CONST              32 (<code object bbcode_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 343>)
+               568 MAKE_FUNCTION            0
+               570 STORE_NAME              54 (bbcode_view)
+               572 LOAD_CONST               1 (None)
+               574 RETURN_VALUE
    consts
       0
       None
       ('authenticate', 'get_user_model', 'login', 'logout')
       ('login_required',)
       ('HttpResponseForbidden',)
       ('get_object_or_404', 'redirect', 'render')
       ('timezone',)
+      ('guest_list',)
       ('BoardProfileModelForm', 'LoginForm', 'PostModelForm', 'ShoutModelForm', 'SignUpForm', 'ThreadModelForm')
       ('Category', 'Post', 'Shout', 'Subcategory', 'Thread')
       ('paginate_qs',)
       ('htmx_redirect',)
       code
          argcount  : 1
-         nlocals   : 10
-         stacksize : 9
+         nlocals   : 13
+         stacksize : 11
          flags     : 3
          code
             0x97007400000000000000000000006a010000000000000000a002000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             007d017406000000000000000000006a010000000000000000a002000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00a00400000000000000000000000000000000000000006401a6010000ab
@@ -315,135 +324,170 @@
             0000000000000000006a010000000000000000a008000000000000000000
             00000000000000000000006403a6010000ab010000000000000000a00200
             00000000000000000000000000000000000000a6000000ab000000000000
             0000007d057c05a004000000000000000000000000000000000000000064
             04a6010000ab010000000000000000a00900000000000000000000000000
             00000000000000a6000000ab0000000000000000007d06640584007c0544
             00a6000000ab0000000000000000007d07640684007c074400a6000000ab
-            0000000000000000007d087c017c027c037c047c057c067c077c0864079c
-            087d097415000000000000000000007c0064087c09ac09a6030000ab0300
-            000000000000005300
-          24           0 RESUME                   0
+            0000000000000000007d08640784007c074400a6000000ab000000000000
+            0000007d097415000000000000000000006a0b0000000000000000a60000
+            00ab0000000000000000007d0a7419000000000000000000007c08a60100
+            00ab0100000000000000007419000000000000000000007c09a6010000ab
+            0100000000000000007a0000007c0a7a0000007d0b7c017c027c037c047c
+            057c067c087c097c0a7c0b64089c0a7d0c741b000000000000000000007c
+            0064097c0cac0aa6030000ab0300000000000000005300
+          25           0 RESUME                   0
          
-          25           2 LOAD_GLOBAL              0 (Category)
+          26           2 LOAD_GLOBAL              0 (Category)
                       14 LOAD_ATTR                1 (objects)
                       24 LOAD_METHOD              2 (all)
                       46 PRECALL                  0
                       50 CALL                     0
                       60 STORE_FAST               1 (categories)
          
-          27          62 LOAD_GLOBAL              6 (Thread)
+          28          62 LOAD_GLOBAL              6 (Thread)
                       74 LOAD_ATTR                1 (objects)
                       84 LOAD_METHOD              2 (all)
                      106 PRECALL                  0
                      110 CALL                     0
                      120 LOAD_METHOD              4 (order_by)
                      142 LOAD_CONST               1 ('-created_at')
                      144 PRECALL                  1
                      148 CALL                     1
                      158 LOAD_CONST               0 (None)
                      160 LOAD_CONST               2 (5)
                      162 BUILD_SLICE              2
                      164 BINARY_SUBSCR
                      174 STORE_FAST               2 (recent_threads)
          
-          29         176 LOAD_GLOBAL              6 (Thread)
+          30         176 LOAD_GLOBAL              6 (Thread)
                      188 LOAD_ATTR                1 (objects)
                      198 LOAD_METHOD              5 (count)
                      220 PRECALL                  0
                      224 CALL                     0
                      234 STORE_FAST               3 (thread_count)
          
-          30         236 LOAD_GLOBAL             12 (Post)
+          31         236 LOAD_GLOBAL             12 (Post)
                      248 LOAD_ATTR                1 (objects)
                      258 LOAD_METHOD              5 (count)
                      280 PRECALL                  0
                      284 CALL                     0
                      294 STORE_FAST               4 (post_count)
          
-          32         296 LOAD_GLOBAL             14 (User)
+          33         296 LOAD_GLOBAL             14 (User)
                      308 LOAD_ATTR                1 (objects)
                      318 LOAD_METHOD              8 (select_related)
                      340 LOAD_CONST               3 ('profile')
                      342 PRECALL                  1
                      346 CALL                     1
                      356 LOAD_METHOD              2 (all)
                      378 PRECALL                  0
                      382 CALL                     0
                      392 STORE_FAST               5 (users)
          
-          33         394 LOAD_FAST                5 (users)
+          34         394 LOAD_FAST                5 (users)
                      396 LOAD_METHOD              4 (order_by)
                      418 LOAD_CONST               4 ('-profile__created_at')
                      420 PRECALL                  1
                      424 CALL                     1
                      434 LOAD_METHOD              9 (first)
                      456 PRECALL                  0
                      460 CALL                     0
                      470 STORE_FAST               6 (newest_user)
          
-          34         472 LOAD_CONST               5 (<code object <listcomp>, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 34>)
+          36         472 LOAD_CONST               5 (<code object <listcomp>, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 36>)
                      474 MAKE_FUNCTION            0
                      476 LOAD_FAST                5 (users)
                      478 GET_ITER
                      480 PRECALL                  0
                      484 CALL                     0
                      494 STORE_FAST               7 (users_online)
          
-          35         496 LOAD_CONST               6 (<code object <listcomp>, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 35>)
+          37         496 LOAD_CONST               6 (<code object <listcomp>, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 37>)
                      498 MAKE_FUNCTION            0
                      500 LOAD_FAST                7 (users_online)
                      502 GET_ITER
                      504 PRECALL                  0
                      508 CALL                     0
-                     518 STORE_FAST               8 (staff_online)
-         
-          38         520 LOAD_FAST                1 (categories)
-         
-          39         522 LOAD_FAST                2 (recent_threads)
-         
-          40         524 LOAD_FAST                3 (thread_count)
-         
-          41         526 LOAD_FAST                4 (post_count)
-         
-          42         528 LOAD_FAST                5 (users)
-         
-          43         530 LOAD_FAST                6 (newest_user)
-         
-          44         532 LOAD_FAST                7 (users_online)
-         
-          45         534 LOAD_FAST                8 (staff_online)
+                     518 STORE_FAST               8 (members_online)
          
-          37         536 LOAD_CONST               7 (('categories', 'recent_threads', 'thread_count', 'post_count', 'users', 'newest_user', 'users_online', 'staff_online'))
-                     538 BUILD_CONST_KEY_MAP      8
-                     540 STORE_FAST               9 (context)
-         
-          47         542 LOAD_GLOBAL             21 (NULL + render)
-                     554 LOAD_FAST                0 (request)
-                     556 LOAD_CONST               8 ('punkweb_bb/index.html')
-                     558 LOAD_FAST                9 (context)
-                     560 KW_NAMES                 9
-                     562 PRECALL                  3
-                     566 CALL                     3
-                     576 RETURN_VALUE
+          38         520 LOAD_CONST               7 (<code object <listcomp>, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 38>)
+                     522 MAKE_FUNCTION            0
+                     524 LOAD_FAST                7 (users_online)
+                     526 GET_ITER
+                     528 PRECALL                  0
+                     532 CALL                     0
+                     542 STORE_FAST               9 (staff_online)
+         
+          39         544 LOAD_GLOBAL             21 (NULL + guest_list)
+                     556 LOAD_ATTR               11 (length)
+                     566 PRECALL                  0
+                     570 CALL                     0
+                     580 STORE_FAST              10 (guests_online)
+         
+          40         582 LOAD_GLOBAL             25 (NULL + len)
+                     594 LOAD_FAST                8 (members_online)
+                     596 PRECALL                  1
+                     600 CALL                     1
+                     610 LOAD_GLOBAL             25 (NULL + len)
+                     622 LOAD_FAST                9 (staff_online)
+                     624 PRECALL                  1
+                     628 CALL                     1
+                     638 BINARY_OP                0 (+)
+                     642 LOAD_FAST               10 (guests_online)
+                     644 BINARY_OP                0 (+)
+                     648 STORE_FAST              11 (total_online)
+         
+          43         650 LOAD_FAST                1 (categories)
+         
+          44         652 LOAD_FAST                2 (recent_threads)
+         
+          45         654 LOAD_FAST                3 (thread_count)
+         
+          46         656 LOAD_FAST                4 (post_count)
+         
+          47         658 LOAD_FAST                5 (users)
+         
+          48         660 LOAD_FAST                6 (newest_user)
+         
+          49         662 LOAD_FAST                8 (members_online)
+         
+          50         664 LOAD_FAST                9 (staff_online)
+         
+          51         666 LOAD_FAST               10 (guests_online)
+         
+          52         668 LOAD_FAST               11 (total_online)
+         
+          42         670 LOAD_CONST               8 (('categories', 'recent_threads', 'thread_count', 'post_count', 'users', 'newest_user', 'members_online', 'staff_online', 'guests_online', 'total_online'))
+                     672 BUILD_CONST_KEY_MAP     10
+                     674 STORE_FAST              12 (context)
+         
+          54         676 LOAD_GLOBAL             27 (NULL + render)
+                     688 LOAD_FAST                0 (request)
+                     690 LOAD_CONST               9 ('punkweb_bb/index.html')
+                     692 LOAD_FAST               12 (context)
+                     694 KW_NAMES                10
+                     696 PRECALL                  3
+                     700 CALL                     3
+                     710 RETURN_VALUE
          consts
             None
             '-created_at'
             5
             'profile'
             '-profile__created_at'
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 19
                code
                   0x970067007c005d107d017c016a0000000000000000006a010000000000
                   000000af0e7c0191028c115300
-                34           0 RESUME                   0
+                36           0 RESUME                   0
                              2 BUILD_LIST               0
                              4 LOAD_FAST                0 (.0)
                        >>    6 FOR_ITER                16 (to 40)
                              8 STORE_FAST               1 (user)
                             10 LOAD_FAST                1 (user)
                             12 LOAD_ATTR                0 (profile)
                             22 LOAD_ATTR                1 (is_online)
@@ -455,25 +499,54 @@
                consts
                names      ('profile', 'is_online')
                varnames   ('.0', 'user')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
                name       '<listcomp>'
-               firstlineno 34
+               firstlineno 36
+               lnotab 0x
+            code
+               argcount  : 1
+               nlocals   : 2
+               stacksize : 3
+               flags     : 19
+               code
+                  0x970067007c005d0b7d017c016a000000000000000000b0097c0191028c
+                  0c5300
+                37           0 RESUME                   0
+                             2 BUILD_LIST               0
+                             4 LOAD_FAST                0 (.0)
+                       >>    6 FOR_ITER                11 (to 30)
+                             8 STORE_FAST               1 (user)
+                            10 LOAD_FAST                1 (user)
+                            12 LOAD_ATTR                0 (is_staff)
+                            22 POP_JUMP_BACKWARD_IF_TRUE     9 (to 6)
+                            24 LOAD_FAST                1 (user)
+                            26 LIST_APPEND              2
+                            28 JUMP_BACKWARD           12 (to 6)
+                       >>   30 RETURN_VALUE
+               consts
+               names      ('is_staff',)
+               varnames   ('.0', 'user')
+               freevars   ()
+               cellvars   ()
+               filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
+               name       '<listcomp>'
+               firstlineno 37
                lnotab 0x
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 19
                code
                   0x970067007c005d0b7d017c016a000000000000000000af097c0191028c
                   0c5300
-                35           0 RESUME                   0
+                38           0 RESUME                   0
                              2 BUILD_LIST               0
                              4 LOAD_FAST                0 (.0)
                        >>    6 FOR_ITER                11 (to 30)
                              8 STORE_FAST               1 (user)
                             10 LOAD_FAST                1 (user)
                             12 LOAD_ATTR                0 (is_staff)
                             22 POP_JUMP_BACKWARD_IF_FALSE     9 (to 6)
@@ -484,29 +557,29 @@
                consts
                names      ('is_staff',)
                varnames   ('.0', 'user')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
                name       '<listcomp>'
-               firstlineno 35
+               firstlineno 38
                lnotab 0x
-            ('categories', 'recent_threads', 'thread_count', 'post_count', 'users', 'newest_user', 'users_online', 'staff_online')
+            ('categories', 'recent_threads', 'thread_count', 'post_count', 'users', 'newest_user', 'members_online', 'staff_online', 'guests_online', 'total_online')
             'punkweb_bb/index.html'
             ('context',)
-         names      ('Category', 'objects', 'all', 'Thread', 'order_by', 'count', 'Post', 'User', 'select_related', 'first', 'render')
-         varnames   ('request', 'categories', 'recent_threads', 'thread_count', 'post_count', 'users', 'newest_user', 'users_online', 'staff_online', 'context')
+         names      ('Category', 'objects', 'all', 'Thread', 'order_by', 'count', 'Post', 'User', 'select_related', 'first', 'guest_list', 'length', 'len', 'render')
+         varnames   ('request', 'categories', 'recent_threads', 'thread_count', 'post_count', 'users', 'newest_user', 'users_online', 'members_online', 'staff_online', 'guests_online', 'total_online', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'index_view'
-         firstlineno 24
+         firstlineno 25
          lnotab
-            0x02013c0272023c013c0262014e01180118030201020102010201020102
-            01020102f8060a
+            0x02013c0272023c013c0262014e02180118011801260144030201020102
+            0102010201020102010201020102f6060c
       code
          argcount  : 1
          nlocals   : 6
          stacksize : 5
          flags     : 3
          code
             0x97007c006a0000000000000000006a010000000000000000720f740500
@@ -518,97 +591,97 @@
             00000000007d027c016a0700000000000000006404190000000000000000
             007d037411000000000000000000007c007c027c03ac05a6030000ab0300
             000000000000007d047c04811f7413000000000000000000007c007c04a6
             020000ab02000000000000000001007405000000000000000000006401a6
             010000ab01000000000000000053006e0e740900000000000000000000a6
             000000ab0000000000000000007d0164067c0169017d0574150000000000
             00000000007c0064077c05a6030000ab0300000000000000005300
-          50           0 RESUME                   0
+          57           0 RESUME                   0
          
-          51           2 LOAD_FAST                0 (request)
+          58           2 LOAD_FAST                0 (request)
                        4 LOAD_ATTR                0 (user)
                       14 LOAD_ATTR                1 (is_authenticated)
                       24 POP_JUMP_FORWARD_IF_FALSE    15 (to 56)
          
-          52          26 LOAD_GLOBAL              5 (NULL + redirect)
+          59          26 LOAD_GLOBAL              5 (NULL + redirect)
                       38 LOAD_CONST               1 ('punkweb_bb:index')
                       40 PRECALL                  1
                       44 CALL                     1
                       54 RETURN_VALUE
          
-          54     >>   56 LOAD_FAST                0 (request)
+          61     >>   56 LOAD_FAST                0 (request)
                       58 LOAD_ATTR                3 (method)
                       68 LOAD_CONST               2 ('POST')
                       70 COMPARE_OP               2 (==)
                       76 POP_JUMP_FORWARD_IF_FALSE   119 (to 316)
          
-          55          78 LOAD_GLOBAL              9 (NULL + LoginForm)
+          62          78 LOAD_GLOBAL              9 (NULL + LoginForm)
                       90 LOAD_FAST                0 (request)
                       92 LOAD_FAST                0 (request)
                       94 LOAD_ATTR                5 (POST)
                      104 PRECALL                  2
                      108 CALL                     2
                      118 STORE_FAST               1 (form)
          
-          57         120 LOAD_FAST                1 (form)
+          64         120 LOAD_FAST                1 (form)
                      122 LOAD_METHOD              6 (is_valid)
                      144 PRECALL                  0
                      148 CALL                     0
                      158 POP_JUMP_FORWARD_IF_FALSE    77 (to 314)
          
-          58         160 LOAD_FAST                1 (form)
+          65         160 LOAD_FAST                1 (form)
                      162 LOAD_ATTR                7 (cleaned_data)
                      172 LOAD_CONST               3 ('username')
                      174 BINARY_SUBSCR
                      184 STORE_FAST               2 (username)
          
-          59         186 LOAD_FAST                1 (form)
+          66         186 LOAD_FAST                1 (form)
                      188 LOAD_ATTR                7 (cleaned_data)
                      198 LOAD_CONST               4 ('password')
                      200 BINARY_SUBSCR
                      210 STORE_FAST               3 (password)
          
-          61         212 LOAD_GLOBAL             17 (NULL + authenticate)
+          68         212 LOAD_GLOBAL             17 (NULL + authenticate)
                      224 LOAD_FAST                0 (request)
                      226 LOAD_FAST                2 (username)
                      228 LOAD_FAST                3 (password)
                      230 KW_NAMES                 5
                      232 PRECALL                  3
                      236 CALL                     3
                      246 STORE_FAST               4 (user)
          
-          63         248 LOAD_FAST                4 (user)
+          70         248 LOAD_FAST                4 (user)
                      250 POP_JUMP_FORWARD_IF_NONE    31 (to 314)
          
-          64         252 LOAD_GLOBAL             19 (NULL + login)
+          71         252 LOAD_GLOBAL             19 (NULL + login)
                      264 LOAD_FAST                0 (request)
                      266 LOAD_FAST                4 (user)
                      268 PRECALL                  2
                      272 CALL                     2
                      282 POP_TOP
          
-          66         284 LOAD_GLOBAL              5 (NULL + redirect)
+          73         284 LOAD_GLOBAL              5 (NULL + redirect)
                      296 LOAD_CONST               1 ('punkweb_bb:index')
                      298 PRECALL                  1
                      302 CALL                     1
                      312 RETURN_VALUE
                  >>  314 JUMP_FORWARD            14 (to 344)
          
-          68     >>  316 LOAD_GLOBAL              9 (NULL + LoginForm)
+          75     >>  316 LOAD_GLOBAL              9 (NULL + LoginForm)
                      328 PRECALL                  0
                      332 CALL                     0
                      342 STORE_FAST               1 (form)
          
-          71     >>  344 LOAD_CONST               6 ('form')
+          78     >>  344 LOAD_CONST               6 ('form')
                      346 LOAD_FAST                1 (form)
          
-          70         348 BUILD_MAP                1
+          77         348 BUILD_MAP                1
                      350 STORE_FAST               5 (context)
          
-          73         352 LOAD_GLOBAL             21 (NULL + render)
+          80         352 LOAD_GLOBAL             21 (NULL + render)
                      364 LOAD_FAST                0 (request)
                      366 LOAD_CONST               7 ('punkweb_bb/login.html')
                      368 LOAD_FAST                5 (context)
                      370 PRECALL                  3
                      374 CALL                     3
                      384 RETURN_VALUE
          consts
@@ -622,50 +695,50 @@
             'punkweb_bb/login.html'
          names      ('user', 'is_authenticated', 'redirect', 'method', 'LoginForm', 'POST', 'is_valid', 'cleaned_data', 'authenticate', 'login', 'render')
          varnames   ('request', 'form', 'username', 'password', 'user', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'login_view'
-         firstlineno 50
+         firstlineno 57
          lnotab
             0x020118011e0216012a0228011a011a0224020401200220021c0304ff04
             03
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000007c00a6010000ab0100000000000000
             0001007403000000000000000000006401a6010000ab0100000000000000
             005300
-          76           0 RESUME                   0
+          83           0 RESUME                   0
          
-          77           2 LOAD_GLOBAL              1 (NULL + logout)
+          84           2 LOAD_GLOBAL              1 (NULL + logout)
                       14 LOAD_FAST                0 (request)
                       16 PRECALL                  1
                       20 CALL                     1
                       30 POP_TOP
          
-          78          32 LOAD_GLOBAL              3 (NULL + redirect)
+          85          32 LOAD_GLOBAL              3 (NULL + redirect)
                       44 LOAD_CONST               1 ('punkweb_bb:login')
                       46 PRECALL                  1
                       50 CALL                     1
                       60 RETURN_VALUE
          consts
             None
             'punkweb_bb:login'
          names      ('logout', 'redirect')
          varnames   ('request',)
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'logout_view'
-         firstlineno 76
+         firstlineno 83
          lnotab 0x02011e01
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 5
          flags     : 3
          code
@@ -676,72 +749,72 @@
             01a0060000000000000000000000000000000000000000a6000000ab0000
             0000000000000072237c01a0070000000000000000000000000000000000
             000000a6000000ab00000000000000000001007405000000000000000000
             006403a6010000ab01000000000000000053006e0e740900000000000000
             000000a6000000ab0000000000000000007d0164047c0169017d02741100
             0000000000000000007c0064057c02a6030000ab03000000000000000053
             00
-          81           0 RESUME                   0
+          88           0 RESUME                   0
          
-          82           2 LOAD_FAST                0 (request)
+          89           2 LOAD_FAST                0 (request)
                        4 LOAD_ATTR                0 (user)
                       14 LOAD_ATTR                1 (is_authenticated)
                       24 POP_JUMP_FORWARD_IF_FALSE    15 (to 56)
          
-          83          26 LOAD_GLOBAL              5 (NULL + redirect)
+          90          26 LOAD_GLOBAL              5 (NULL + redirect)
                       38 LOAD_CONST               1 ('punkweb_bb:index')
                       40 PRECALL                  1
                       44 CALL                     1
                       54 RETURN_VALUE
          
-          85     >>   56 LOAD_FAST                0 (request)
+          92     >>   56 LOAD_FAST                0 (request)
                       58 LOAD_ATTR                3 (method)
                       68 LOAD_CONST               2 ('POST')
                       70 COMPARE_OP               2 (==)
                       76 POP_JUMP_FORWARD_IF_FALSE    76 (to 230)
          
-          86          78 LOAD_GLOBAL              9 (NULL + SignUpForm)
+          93          78 LOAD_GLOBAL              9 (NULL + SignUpForm)
                       90 LOAD_FAST                0 (request)
                       92 LOAD_ATTR                5 (POST)
                      102 PRECALL                  1
                      106 CALL                     1
                      116 STORE_FAST               1 (form)
          
-          88         118 LOAD_FAST                1 (form)
+          95         118 LOAD_FAST                1 (form)
                      120 LOAD_METHOD              6 (is_valid)
                      142 PRECALL                  0
                      146 CALL                     0
                      156 POP_JUMP_FORWARD_IF_FALSE    35 (to 228)
          
-          89         158 LOAD_FAST                1 (form)
+          96         158 LOAD_FAST                1 (form)
                      160 LOAD_METHOD              7 (save)
                      182 PRECALL                  0
                      186 CALL                     0
                      196 POP_TOP
          
-          91         198 LOAD_GLOBAL              5 (NULL + redirect)
+          98         198 LOAD_GLOBAL              5 (NULL + redirect)
                      210 LOAD_CONST               3 ('punkweb_bb:login')
                      212 PRECALL                  1
                      216 CALL                     1
                      226 RETURN_VALUE
          
-          88     >>  228 JUMP_FORWARD            14 (to 258)
+          95     >>  228 JUMP_FORWARD            14 (to 258)
          
-          93     >>  230 LOAD_GLOBAL              9 (NULL + SignUpForm)
+         100     >>  230 LOAD_GLOBAL              9 (NULL + SignUpForm)
                      242 PRECALL                  0
                      246 CALL                     0
                      256 STORE_FAST               1 (form)
          
-          96     >>  258 LOAD_CONST               4 ('form')
+         103     >>  258 LOAD_CONST               4 ('form')
                      260 LOAD_FAST                1 (form)
          
-          95         262 BUILD_MAP                1
+         102         262 BUILD_MAP                1
                      264 STORE_FAST               2 (context)
          
-          98         266 LOAD_GLOBAL             17 (NULL + render)
+         105         266 LOAD_GLOBAL             17 (NULL + render)
                      278 LOAD_FAST                0 (request)
                      280 LOAD_CONST               5 ('punkweb_bb/signup.html')
                      282 LOAD_FAST                2 (context)
                      284 PRECALL                  3
                      288 CALL                     3
                      298 RETURN_VALUE
          consts
@@ -753,43 +826,43 @@
             'punkweb_bb/signup.html'
          names      ('user', 'is_authenticated', 'redirect', 'method', 'SignUpForm', 'POST', 'is_valid', 'save', 'render')
          varnames   ('request', 'form', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'signup_view'
-         firstlineno 81
+         firstlineno 88
          lnotab 0x020118011e0216012802280128021efd02051c0304ff0403
       code
          argcount  : 2
          nlocals   : 4
          stacksize : 5
          flags     : 3
          code
             0x97007401000000000000000000007402000000000000000000007c01ac
             01a6020000ab0200000000000000007d0264027c0269017d037405000000
             000000000000007c0064037c03ac04a6030000ab03000000000000000053
             00
-         101           0 RESUME                   0
+         108           0 RESUME                   0
          
-         102           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+         109           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
                       14 LOAD_GLOBAL              2 (User)
                       26 LOAD_FAST                1 (user_id)
                       28 KW_NAMES                 1
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               2 (user)
          
-         105          46 LOAD_CONST               2 ('user')
+         112          46 LOAD_CONST               2 ('user')
                       48 LOAD_FAST                2 (user)
          
-         104          50 BUILD_MAP                1
+         111          50 BUILD_MAP                1
                       52 STORE_FAST               3 (context)
          
-         107          54 LOAD_GLOBAL              5 (NULL + render)
+         114          54 LOAD_GLOBAL              5 (NULL + render)
                       66 LOAD_FAST                0 (request)
                       68 LOAD_CONST               3 ('punkweb_bb/profile.html')
                       70 LOAD_FAST                3 (context)
                       72 KW_NAMES                 4
                       74 PRECALL                  3
                       78 CALL                     3
                       88 RETURN_VALUE
@@ -801,55 +874,55 @@
             ('context',)
          names      ('get_object_or_404', 'User', 'render')
          varnames   ('request', 'user_id', 'user', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'profile_view'
-         firstlineno 101
+         firstlineno 108
          lnotab 0x02012c0304ff0403
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 6
          flags     : 3
          code
             0x97007401000000000000000000007c007402000000000000000000006a
             020000000000000000a00300000000000000000000000000000000000000
             006401a6010000ab010000000000000000a0040000000000000000000000
             0000000000000000006402a6010000ab010000000000000000a6020000ab
             0200000000000000007d0164037c0169017d02740b000000000000000000
             007c0064047c02ac05a6030000ab0300000000000000005300
-         110           0 RESUME                   0
+         117           0 RESUME                   0
          
-         111           2 LOAD_GLOBAL              1 (NULL + paginate_qs)
+         118           2 LOAD_GLOBAL              1 (NULL + paginate_qs)
          
-         112          14 LOAD_FAST                0 (request)
+         119          14 LOAD_FAST                0 (request)
                       16 LOAD_GLOBAL              2 (User)
                       28 LOAD_ATTR                2 (objects)
                       38 LOAD_METHOD              3 (select_related)
                       60 LOAD_CONST               1 ('profile')
                       62 PRECALL                  1
                       66 CALL                     1
                       76 LOAD_METHOD              4 (order_by)
                       98 LOAD_CONST               2 ('username')
                      100 PRECALL                  1
                      104 CALL                     1
          
-         111         114 PRECALL                  2
+         118         114 PRECALL                  2
                      118 CALL                     2
                      128 STORE_FAST               1 (users)
          
-         116         130 LOAD_CONST               3 ('users')
+         123         130 LOAD_CONST               3 ('users')
                      132 LOAD_FAST                1 (users)
          
-         115         134 BUILD_MAP                1
+         122         134 BUILD_MAP                1
                      136 STORE_FAST               2 (context)
          
-         118         138 LOAD_GLOBAL             11 (NULL + render)
+         125         138 LOAD_GLOBAL             11 (NULL + render)
                      150 LOAD_FAST                0 (request)
                      152 LOAD_CONST               4 ('punkweb_bb/members.html')
                      154 LOAD_FAST                2 (context)
                      156 KW_NAMES                 5
                      158 PRECALL                  3
                      162 CALL                     3
                      172 RETURN_VALUE
@@ -862,15 +935,15 @@
             ('context',)
          names      ('paginate_qs', 'User', 'objects', 'select_related', 'order_by', 'render')
          varnames   ('request', 'users', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'members_view'
-         firstlineno 110
+         firstlineno 117
          lnotab 0x02010c0164ff100504ff0403
       '/login/'
       ('login_url',)
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 6
@@ -884,82 +957,82 @@
             000000000000000000000000000000a6000000ab00000000000000000001
             007411000000000000000000006403a6010000ab01000000000000000053
             007413000000000000000000007c00640464057c016901ac06a6030000ab
             03000000000000000053007403000000000000000000007c006a04000000
             00000000006a050000000000000000ac02a6010000ab0100000000000000
             007d0164057c0169017d027413000000000000000000007c0064047c02ac
             06a6030000ab0300000000000000005300
-         121           0 RESUME                   0
+         128           0 RESUME                   0
          
-         123           2 LOAD_FAST                0 (request)
+         130           2 LOAD_FAST                0 (request)
                        4 LOAD_ATTR                0 (method)
                       14 LOAD_CONST               1 ('POST')
                       16 COMPARE_OP               2 (==)
                       22 POP_JUMP_FORWARD_IF_FALSE   113 (to 250)
          
-         124          24 LOAD_GLOBAL              3 (NULL + BoardProfileModelForm)
+         131          24 LOAD_GLOBAL              3 (NULL + BoardProfileModelForm)
          
-         125          36 LOAD_FAST                0 (request)
+         132          36 LOAD_FAST                0 (request)
                       38 LOAD_ATTR                2 (POST)
                       48 LOAD_FAST                0 (request)
                       50 LOAD_ATTR                3 (FILES)
                       60 LOAD_FAST                0 (request)
                       62 LOAD_ATTR                4 (user)
                       72 LOAD_ATTR                5 (profile)
          
-         124          82 KW_NAMES                 2
+         131          82 KW_NAMES                 2
                       84 PRECALL                  3
                       88 CALL                     3
                       98 STORE_FAST               1 (form)
          
-         128         100 LOAD_FAST                1 (form)
+         135         100 LOAD_FAST                1 (form)
                      102 LOAD_METHOD              6 (is_valid)
                      124 PRECALL                  0
                      128 CALL                     0
                      138 POP_JUMP_FORWARD_IF_FALSE    35 (to 210)
          
-         129         140 LOAD_FAST                1 (form)
+         136         140 LOAD_FAST                1 (form)
                      142 LOAD_METHOD              7 (save)
                      164 PRECALL                  0
                      168 CALL                     0
                      178 POP_TOP
          
-         131         180 LOAD_GLOBAL             17 (NULL + redirect)
+         138         180 LOAD_GLOBAL             17 (NULL + redirect)
                      192 LOAD_CONST               3 ('punkweb_bb:settings')
                      194 PRECALL                  1
                      198 CALL                     1
                      208 RETURN_VALUE
          
-         133     >>  210 LOAD_GLOBAL             19 (NULL + render)
+         140     >>  210 LOAD_GLOBAL             19 (NULL + render)
                      222 LOAD_FAST                0 (request)
                      224 LOAD_CONST               4 ('punkweb_bb/settings.html')
                      226 LOAD_CONST               5 ('form')
                      228 LOAD_FAST                1 (form)
                      230 BUILD_MAP                1
                      232 KW_NAMES                 6
                      234 PRECALL                  3
                      238 CALL                     3
                      248 RETURN_VALUE
          
-         135     >>  250 LOAD_GLOBAL              3 (NULL + BoardProfileModelForm)
+         142     >>  250 LOAD_GLOBAL              3 (NULL + BoardProfileModelForm)
                      262 LOAD_FAST                0 (request)
                      264 LOAD_ATTR                4 (user)
                      274 LOAD_ATTR                5 (profile)
                      284 KW_NAMES                 2
                      286 PRECALL                  1
                      290 CALL                     1
                      300 STORE_FAST               1 (form)
          
-         138         302 LOAD_CONST               5 ('form')
+         145         302 LOAD_CONST               5 ('form')
                      304 LOAD_FAST                1 (form)
          
-         137         306 BUILD_MAP                1
+         144         306 BUILD_MAP                1
                      308 STORE_FAST               2 (context)
          
-         141         310 LOAD_GLOBAL             19 (NULL + render)
+         148         310 LOAD_GLOBAL             19 (NULL + render)
                      322 LOAD_FAST                0 (request)
                      324 LOAD_CONST               4 ('punkweb_bb/settings.html')
                      326 LOAD_FAST                2 (context)
                      328 KW_NAMES                 6
                      330 PRECALL                  3
                      334 CALL                     3
                      344 RETURN_VALUE
@@ -973,58 +1046,58 @@
             ('context',)
          names      ('method', 'BoardProfileModelForm', 'POST', 'FILES', 'user', 'profile', 'is_valid', 'save', 'redirect', 'render')
          varnames   ('request', 'form', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'settings_view'
-         firstlineno 121
+         firstlineno 128
          lnotab 0x020216010c012eff1204280128021e022802340304ff0404
       code
          argcount  : 2
          nlocals   : 5
          stacksize : 5
          flags     : 3
          code
             0x97007401000000000000000000007402000000000000000000007c01ac
             01a6020000ab0200000000000000007d027405000000000000000000007c
             007c026a030000000000000000a004000000000000000000000000000000
             0000000000a6000000ab000000000000000000a6020000ab020000000000
             0000007d037c027c0364029c027d04740b000000000000000000007c0064
             037c04ac04a6030000ab0300000000000000005300
-         144           0 RESUME                   0
+         151           0 RESUME                   0
          
-         145           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+         152           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
                       14 LOAD_GLOBAL              2 (Subcategory)
                       26 LOAD_FAST                1 (subcategory_slug)
                       28 KW_NAMES                 1
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               2 (subcategory)
          
-         147          46 LOAD_GLOBAL              5 (NULL + paginate_qs)
+         154          46 LOAD_GLOBAL              5 (NULL + paginate_qs)
                       58 LOAD_FAST                0 (request)
                       60 LOAD_FAST                2 (subcategory)
                       62 LOAD_ATTR                3 (threads)
                       72 LOAD_METHOD              4 (all)
                       94 PRECALL                  0
                       98 CALL                     0
                      108 PRECALL                  2
                      112 CALL                     2
                      122 STORE_FAST               3 (threads)
          
-         150         124 LOAD_FAST                2 (subcategory)
+         157         124 LOAD_FAST                2 (subcategory)
          
-         151         126 LOAD_FAST                3 (threads)
+         158         126 LOAD_FAST                3 (threads)
          
-         149         128 LOAD_CONST               2 (('subcategory', 'threads'))
+         156         128 LOAD_CONST               2 (('subcategory', 'threads'))
                      130 BUILD_CONST_KEY_MAP      2
                      132 STORE_FAST               4 (context)
          
-         153         134 LOAD_GLOBAL             11 (NULL + render)
+         160         134 LOAD_GLOBAL             11 (NULL + render)
                      146 LOAD_FAST                0 (request)
                      148 LOAD_CONST               3 ('punkweb_bb/subcategory.html')
                      150 LOAD_FAST                4 (context)
                      152 KW_NAMES                 4
                      154 PRECALL                  3
                      158 CALL                     3
                      168 RETURN_VALUE
@@ -1036,15 +1109,15 @@
             ('context',)
          names      ('get_object_or_404', 'Subcategory', 'paginate_qs', 'threads', 'all', 'render')
          varnames   ('request', 'subcategory_slug', 'subcategory', 'threads', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'subcategory_view'
-         firstlineno 144
+         firstlineno 151
          lnotab 0x02012c024e03020102fe0604
       code
          argcount  : 2
          nlocals   : 6
          stacksize : 5
          flags     : 3
          code
@@ -1059,102 +1132,102 @@
             006403ac04a6010000ab0100000000000000007d047c027c045f0b000000
             00000000007c006a0300000000000000007c045f0300000000000000007c
             04a00a0000000000000000000000000000000000000000a6000000ab0000
             000000000000000100740b000000000000000000007c04a6010000ab0100
             0000000000000053006e0e740f00000000000000000000a6000000ab0000
             000000000000007d037c027c0364059c027d057419000000000000000000
             007c0064067c05ac07a6030000ab0300000000000000005300
-         156           0 RESUME                   0
+         163           0 RESUME                   0
          
-         158           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+         165           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
                       14 LOAD_GLOBAL              2 (Subcategory)
                       26 LOAD_FAST                1 (subcategory_slug)
                       28 KW_NAMES                 1
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               2 (subcategory)
          
-         160          46 LOAD_FAST                2 (subcategory)
+         167          46 LOAD_FAST                2 (subcategory)
                       48 LOAD_ATTR                2 (staff_post_only)
                       58 POP_JUMP_FORWARD_IF_FALSE    27 (to 114)
                       60 LOAD_FAST                0 (request)
                       62 LOAD_ATTR                3 (user)
                       72 LOAD_ATTR                4 (is_staff)
                       82 POP_JUMP_FORWARD_IF_TRUE    15 (to 114)
          
-         161          84 LOAD_GLOBAL             11 (NULL + redirect)
+         168          84 LOAD_GLOBAL             11 (NULL + redirect)
                       96 LOAD_FAST                2 (subcategory)
                       98 PRECALL                  1
                      102 CALL                     1
                      112 RETURN_VALUE
          
-         163     >>  114 LOAD_FAST                0 (request)
+         170     >>  114 LOAD_FAST                0 (request)
                      116 LOAD_ATTR                6 (method)
                      126 LOAD_CONST               2 ('POST')
                      128 COMPARE_OP               2 (==)
                      134 POP_JUMP_FORWARD_IF_FALSE   117 (to 370)
          
-         164         136 LOAD_GLOBAL             15 (NULL + ThreadModelForm)
+         171         136 LOAD_GLOBAL             15 (NULL + ThreadModelForm)
                      148 LOAD_FAST                0 (request)
                      150 LOAD_ATTR                8 (POST)
                      160 PRECALL                  1
                      164 CALL                     1
                      174 STORE_FAST               3 (form)
          
-         166         176 LOAD_FAST                3 (form)
+         173         176 LOAD_FAST                3 (form)
                      178 LOAD_METHOD              9 (is_valid)
                      200 PRECALL                  0
                      204 CALL                     0
                      214 POP_JUMP_FORWARD_IF_FALSE    76 (to 368)
          
-         167         216 LOAD_FAST                3 (form)
+         174         216 LOAD_FAST                3 (form)
                      218 LOAD_METHOD             10 (save)
                      240 LOAD_CONST               3 (False)
                      242 KW_NAMES                 4
                      244 PRECALL                  1
                      248 CALL                     1
                      258 STORE_FAST               4 (thread)
          
-         168         260 LOAD_FAST                2 (subcategory)
+         175         260 LOAD_FAST                2 (subcategory)
                      262 LOAD_FAST                4 (thread)
                      264 STORE_ATTR              11 (subcategory)
          
-         169         274 LOAD_FAST                0 (request)
+         176         274 LOAD_FAST                0 (request)
                      276 LOAD_ATTR                3 (user)
                      286 LOAD_FAST                4 (thread)
                      288 STORE_ATTR               3 (user)
          
-         170         298 LOAD_FAST                4 (thread)
+         177         298 LOAD_FAST                4 (thread)
                      300 LOAD_METHOD             10 (save)
                      322 PRECALL                  0
                      326 CALL                     0
                      336 POP_TOP
          
-         172         338 LOAD_GLOBAL             11 (NULL + redirect)
+         179         338 LOAD_GLOBAL             11 (NULL + redirect)
                      350 LOAD_FAST                4 (thread)
                      352 PRECALL                  1
                      356 CALL                     1
                      366 RETURN_VALUE
          
-         166     >>  368 JUMP_FORWARD            14 (to 398)
+         173     >>  368 JUMP_FORWARD            14 (to 398)
          
-         174     >>  370 LOAD_GLOBAL             15 (NULL + ThreadModelForm)
+         181     >>  370 LOAD_GLOBAL             15 (NULL + ThreadModelForm)
                      382 PRECALL                  0
                      386 CALL                     0
                      396 STORE_FAST               3 (form)
          
-         177     >>  398 LOAD_FAST                2 (subcategory)
+         184     >>  398 LOAD_FAST                2 (subcategory)
          
-         178         400 LOAD_FAST                3 (form)
+         185         400 LOAD_FAST                3 (form)
          
-         176         402 LOAD_CONST               5 (('subcategory', 'form'))
+         183         402 LOAD_CONST               5 (('subcategory', 'form'))
                      404 BUILD_CONST_KEY_MAP      2
                      406 STORE_FAST               5 (context)
          
-         180         408 LOAD_GLOBAL             25 (NULL + render)
+         187         408 LOAD_GLOBAL             25 (NULL + render)
                      420 LOAD_FAST                0 (request)
                      422 LOAD_CONST               6 ('punkweb_bb/thread_create.html')
                      424 LOAD_FAST                5 (context)
                      426 KW_NAMES                 7
                      428 PRECALL                  3
                      432 CALL                     3
                      442 RETURN_VALUE
@@ -1169,15 +1242,15 @@
             ('context',)
          names      ('get_object_or_404', 'Subcategory', 'staff_post_only', 'user', 'is_staff', 'redirect', 'method', 'ThreadModelForm', 'POST', 'is_valid', 'save', 'subcategory', 'render')
          varnames   ('request', 'subcategory_slug', 'subcategory', 'form', 'thread', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'thread_create_view'
-         firstlineno 156
+         firstlineno 163
          lnotab
             0x02022c0226011e021601280228012c010e01180128021efa02081c0302
             0102fe0604
       code
          argcount  : 2
          nlocals   : 7
          stacksize : 5
@@ -1192,88 +1265,88 @@
             0000000000000064026700a6020000ab0200000000000000007d057c017c
             05760172327c0278016a08000000000000000064037a0d000063025f0800
             000000000000007c02a00900000000000000000000000000000000000000
             00a6000000ab00000000000000000001007c057c0167017a0000007c006a
             06000000000000000064023c0000007c027c037c0464049c037d06741500
             0000000000000000007c0064057c06ac06a6030000ab0300000000000000
             005300
-         183           0 RESUME                   0
+         190           0 RESUME                   0
          
-         184           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+         191           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
                       14 LOAD_GLOBAL              2 (Thread)
                       26 LOAD_FAST                1 (thread_id)
                       28 KW_NAMES                 1
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               2 (thread)
          
-         186          46 LOAD_GLOBAL              5 (NULL + paginate_qs)
+         193          46 LOAD_GLOBAL              5 (NULL + paginate_qs)
                       58 LOAD_FAST                0 (request)
                       60 LOAD_FAST                2 (thread)
                       62 LOAD_ATTR                3 (posts)
                       72 LOAD_METHOD              4 (all)
                       94 PRECALL                  0
                       98 CALL                     0
                      108 PRECALL                  2
                      112 CALL                     2
                      122 STORE_FAST               3 (posts)
          
-         188         124 LOAD_GLOBAL             11 (NULL + PostModelForm)
+         195         124 LOAD_GLOBAL             11 (NULL + PostModelForm)
                      136 PRECALL                  0
                      140 CALL                     0
                      150 STORE_FAST               4 (post_form)
          
-         191         152 LOAD_FAST                0 (request)
+         198         152 LOAD_FAST                0 (request)
                      154 LOAD_ATTR                6 (session)
                      164 LOAD_METHOD              7 (get)
                      186 LOAD_CONST               2 ('viewed_threads')
                      188 BUILD_LIST               0
                      190 PRECALL                  2
                      194 CALL                     2
                      204 STORE_FAST               5 (viewed_threads)
          
-         192         206 LOAD_FAST                1 (thread_id)
+         199         206 LOAD_FAST                1 (thread_id)
                      208 LOAD_FAST                5 (viewed_threads)
                      210 CONTAINS_OP              1
                      212 POP_JUMP_FORWARD_IF_FALSE    50 (to 314)
          
-         193         214 LOAD_FAST                2 (thread)
+         200         214 LOAD_FAST                2 (thread)
                      216 COPY                     1
                      218 LOAD_ATTR                8 (view_count)
                      228 LOAD_CONST               3 (1)
                      230 BINARY_OP               13 (+=)
                      234 SWAP                     2
                      236 STORE_ATTR               8 (view_count)
          
-         194         246 LOAD_FAST                2 (thread)
+         201         246 LOAD_FAST                2 (thread)
                      248 LOAD_METHOD              9 (save)
                      270 PRECALL                  0
                      274 CALL                     0
                      284 POP_TOP
          
-         195         286 LOAD_FAST                5 (viewed_threads)
+         202         286 LOAD_FAST                5 (viewed_threads)
                      288 LOAD_FAST                1 (thread_id)
                      290 BUILD_LIST               1
                      292 BINARY_OP                0 (+)
                      296 LOAD_FAST                0 (request)
                      298 LOAD_ATTR                6 (session)
                      308 LOAD_CONST               2 ('viewed_threads')
                      310 STORE_SUBSCR
          
-         198     >>  314 LOAD_FAST                2 (thread)
+         205     >>  314 LOAD_FAST                2 (thread)
          
-         199         316 LOAD_FAST                3 (posts)
+         206         316 LOAD_FAST                3 (posts)
          
-         200         318 LOAD_FAST                4 (post_form)
+         207         318 LOAD_FAST                4 (post_form)
          
-         197         320 LOAD_CONST               4 (('thread', 'posts', 'post_form'))
+         204         320 LOAD_CONST               4 (('thread', 'posts', 'post_form'))
                      322 BUILD_CONST_KEY_MAP      3
                      324 STORE_FAST               6 (context)
          
-         202         326 LOAD_GLOBAL             21 (NULL + render)
+         209         326 LOAD_GLOBAL             21 (NULL + render)
                      338 LOAD_FAST                0 (request)
                      340 LOAD_CONST               5 ('punkweb_bb/thread.html')
                      342 LOAD_FAST                6 (context)
                      344 KW_NAMES                 6
                      346 PRECALL                  3
                      350 CALL                     3
                      360 RETURN_VALUE
@@ -1287,15 +1360,15 @@
             ('context',)
          names      ('get_object_or_404', 'Thread', 'paginate_qs', 'posts', 'all', 'PostModelForm', 'session', 'get', 'view_count', 'save', 'render')
          varnames   ('request', 'thread_id', 'thread', 'posts', 'post_form', 'viewed_threads', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'thread_view'
-         firstlineno 183
+         firstlineno 190
          lnotab 0x02012c024e021c0336010801200128011c030201020102fd0605
       code
          argcount  : 2
          nlocals   : 5
          stacksize : 5
          flags     : 3
          code
@@ -1306,77 +1379,77 @@
             0000007d037c03a0060000000000000000000000000000000000000000a6
             000000ab00000000000000000072237c03a0070000000000000000000000
             000000000000000000a6000000ab0000000000000000007d027411000000
             000000000000007c02a6010000ab01000000000000000053006e10740900
             0000000000000000007c02ac03a6010000ab0100000000000000007d037c
             027c0364049c027d047413000000000000000000007c0064057c04ac06a6
             030000ab0300000000000000005300
-         205           0 RESUME                   0
+         212           0 RESUME                   0
          
-         207           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+         214           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
                       14 LOAD_GLOBAL              2 (Thread)
                       26 LOAD_FAST                1 (thread_id)
                       28 LOAD_FAST                0 (request)
                       30 LOAD_ATTR                2 (user)
                       40 KW_NAMES                 1
                       42 PRECALL                  3
                       46 CALL                     3
                       56 STORE_FAST               2 (thread)
          
-         209          58 LOAD_FAST                0 (request)
+         216          58 LOAD_FAST                0 (request)
                       60 LOAD_ATTR                3 (method)
                       70 LOAD_CONST               2 ('POST')
                       72 COMPARE_OP               2 (==)
                       78 POP_JUMP_FORWARD_IF_FALSE    78 (to 236)
          
-         210          80 LOAD_GLOBAL              9 (NULL + ThreadModelForm)
+         217          80 LOAD_GLOBAL              9 (NULL + ThreadModelForm)
                       92 LOAD_FAST                0 (request)
                       94 LOAD_ATTR                5 (POST)
                      104 LOAD_FAST                2 (thread)
                      106 KW_NAMES                 3
                      108 PRECALL                  2
                      112 CALL                     2
                      122 STORE_FAST               3 (form)
          
-         212         124 LOAD_FAST                3 (form)
+         219         124 LOAD_FAST                3 (form)
                      126 LOAD_METHOD              6 (is_valid)
                      148 PRECALL                  0
                      152 CALL                     0
                      162 POP_JUMP_FORWARD_IF_FALSE    35 (to 234)
          
-         213         164 LOAD_FAST                3 (form)
+         220         164 LOAD_FAST                3 (form)
                      166 LOAD_METHOD              7 (save)
                      188 PRECALL                  0
                      192 CALL                     0
                      202 STORE_FAST               2 (thread)
          
-         215         204 LOAD_GLOBAL             17 (NULL + redirect)
+         222         204 LOAD_GLOBAL             17 (NULL + redirect)
                      216 LOAD_FAST                2 (thread)
                      218 PRECALL                  1
                      222 CALL                     1
                      232 RETURN_VALUE
          
-         212     >>  234 JUMP_FORWARD            16 (to 268)
+         219     >>  234 JUMP_FORWARD            16 (to 268)
          
-         217     >>  236 LOAD_GLOBAL              9 (NULL + ThreadModelForm)
+         224     >>  236 LOAD_GLOBAL              9 (NULL + ThreadModelForm)
                      248 LOAD_FAST                2 (thread)
                      250 KW_NAMES                 3
                      252 PRECALL                  1
                      256 CALL                     1
                      266 STORE_FAST               3 (form)
          
-         220     >>  268 LOAD_FAST                2 (thread)
+         227     >>  268 LOAD_FAST                2 (thread)
          
-         221         270 LOAD_FAST                3 (form)
+         228         270 LOAD_FAST                3 (form)
          
-         219         272 LOAD_CONST               4 (('thread', 'form'))
+         226         272 LOAD_CONST               4 (('thread', 'form'))
                      274 BUILD_CONST_KEY_MAP      2
                      276 STORE_FAST               4 (context)
          
-         223         278 LOAD_GLOBAL             19 (NULL + render)
+         230         278 LOAD_GLOBAL             19 (NULL + render)
                      290 LOAD_FAST                0 (request)
                      292 LOAD_CONST               5 ('punkweb_bb/thread_update.html')
                      294 LOAD_FAST                4 (context)
                      296 KW_NAMES                 6
                      298 PRECALL                  3
                      302 CALL                     3
                      312 RETURN_VALUE
@@ -1390,15 +1463,15 @@
             ('context',)
          names      ('get_object_or_404', 'Thread', 'user', 'method', 'ThreadModelForm', 'POST', 'is_valid', 'save', 'redirect', 'render')
          varnames   ('request', 'thread_id', 'thread', 'form', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'thread_update_view'
-         firstlineno 205
+         firstlineno 212
          lnotab 0x0202380216012c02280128021efd02052003020102fe0604
       code
          argcount  : 2
          nlocals   : 4
          stacksize : 5
          flags     : 3
          code
@@ -1407,55 +1480,55 @@
             006a03000000000000000064026b0200000000723a7c02a0040000000000
             000000000000000000000000000000a6000000ab00000000000000000001
             00740b000000000000000000007c026a060000000000000000a007000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00a6010000ab010000000000000000530064037c0269017d037411000000
             000000000000007c0064047c03ac05a6030000ab03000000000000000053
             00
-         226           0 RESUME                   0
+         233           0 RESUME                   0
          
-         228           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+         235           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
                       14 LOAD_GLOBAL              2 (Thread)
                       26 LOAD_FAST                1 (thread_id)
                       28 LOAD_FAST                0 (request)
                       30 LOAD_ATTR                2 (user)
                       40 KW_NAMES                 1
                       42 PRECALL                  3
                       46 CALL                     3
                       56 STORE_FAST               2 (thread)
          
-         230          58 LOAD_FAST                0 (request)
+         237          58 LOAD_FAST                0 (request)
                       60 LOAD_ATTR                3 (method)
                       70 LOAD_CONST               2 ('DELETE')
                       72 COMPARE_OP               2 (==)
                       78 POP_JUMP_FORWARD_IF_FALSE    58 (to 196)
          
-         231          80 LOAD_FAST                2 (thread)
+         238          80 LOAD_FAST                2 (thread)
                       82 LOAD_METHOD              4 (delete)
                      104 PRECALL                  0
                      108 CALL                     0
                      118 POP_TOP
          
-         233         120 LOAD_GLOBAL             11 (NULL + htmx_redirect)
+         240         120 LOAD_GLOBAL             11 (NULL + htmx_redirect)
                      132 LOAD_FAST                2 (thread)
                      134 LOAD_ATTR                6 (subcategory)
                      144 LOAD_METHOD              7 (get_absolute_url)
                      166 PRECALL                  0
                      170 CALL                     0
                      180 PRECALL                  1
                      184 CALL                     1
                      194 RETURN_VALUE
          
-         236     >>  196 LOAD_CONST               3 ('thread')
+         243     >>  196 LOAD_CONST               3 ('thread')
                      198 LOAD_FAST                2 (thread)
          
-         235         200 BUILD_MAP                1
+         242         200 BUILD_MAP                1
                      202 STORE_FAST               3 (context)
          
-         239         204 LOAD_GLOBAL             17 (NULL + render)
+         246         204 LOAD_GLOBAL             17 (NULL + render)
                      216 LOAD_FAST                0 (request)
                      218 LOAD_CONST               4 ('punkweb_bb/partials/thread_delete.html')
                      220 LOAD_FAST                3 (context)
                      222 KW_NAMES                 5
                      224 PRECALL                  3
                      228 CALL                     3
                      238 RETURN_VALUE
@@ -1468,15 +1541,15 @@
             ('context',)
          names      ('get_object_or_404', 'Thread', 'user', 'method', 'delete', 'htmx_redirect', 'subcategory', 'get_absolute_url', 'render')
          varnames   ('request', 'thread_id', 'thread', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'thread_delete_view'
-         firstlineno 226
+         firstlineno 233
          lnotab 0x02023802160128024c0304ff0404
       code
          argcount  : 2
          nlocals   : 5
          stacksize : 4
          flags     : 3
          code
@@ -1487,91 +1560,91 @@
             0100000000000000007d037c03a006000000000000000000000000000000
             0000000000a6000000ab000000000000000000724c7c03a0070000000000
             0000000000000000000000000000006403ac04a6010000ab010000000000
             0000007d047c027c045f0800000000000000007c006a0900000000000000
             007c045f0900000000000000007c04a00700000000000000000000000000
             00000000000000a6000000ab000000000000000000010074150000000000
             00000000007c04a6010000ab010000000000000000530064005300
-         242           0 RESUME                   0
+         249           0 RESUME                   0
          
-         244           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+         251           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
                       14 LOAD_GLOBAL              2 (Thread)
                       26 LOAD_FAST                1 (thread_id)
                       28 KW_NAMES                 1
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               2 (thread)
          
-         246          46 LOAD_FAST                2 (thread)
+         253          46 LOAD_FAST                2 (thread)
                       48 LOAD_ATTR                2 (is_closed)
                       58 POP_JUMP_FORWARD_IF_FALSE    15 (to 90)
          
-         247          60 LOAD_GLOBAL              7 (NULL + HttpResponseForbidden)
+         254          60 LOAD_GLOBAL              7 (NULL + HttpResponseForbidden)
                       72 LOAD_CONST               2 ('Cannot add posts to a closed thread.')
                       74 PRECALL                  1
                       78 CALL                     1
                       88 RETURN_VALUE
          
-         249     >>   90 LOAD_GLOBAL              9 (NULL + PostModelForm)
+         256     >>   90 LOAD_GLOBAL              9 (NULL + PostModelForm)
                      102 LOAD_FAST                0 (request)
                      104 LOAD_ATTR                5 (POST)
                      114 PRECALL                  1
                      118 CALL                     1
                      128 STORE_FAST               3 (form)
          
-         251         130 LOAD_FAST                3 (form)
+         258         130 LOAD_FAST                3 (form)
                      132 LOAD_METHOD              6 (is_valid)
                      154 PRECALL                  0
                      158 CALL                     0
                      168 POP_JUMP_FORWARD_IF_FALSE    76 (to 322)
          
-         252         170 LOAD_FAST                3 (form)
+         259         170 LOAD_FAST                3 (form)
                      172 LOAD_METHOD              7 (save)
                      194 LOAD_CONST               3 (False)
                      196 KW_NAMES                 4
                      198 PRECALL                  1
                      202 CALL                     1
                      212 STORE_FAST               4 (post)
          
-         253         214 LOAD_FAST                2 (thread)
+         260         214 LOAD_FAST                2 (thread)
                      216 LOAD_FAST                4 (post)
                      218 STORE_ATTR               8 (thread)
          
-         254         228 LOAD_FAST                0 (request)
+         261         228 LOAD_FAST                0 (request)
                      230 LOAD_ATTR                9 (user)
                      240 LOAD_FAST                4 (post)
                      242 STORE_ATTR               9 (user)
          
-         255         252 LOAD_FAST                4 (post)
+         262         252 LOAD_FAST                4 (post)
                      254 LOAD_METHOD              7 (save)
                      276 PRECALL                  0
                      280 CALL                     0
                      290 POP_TOP
          
-         257         292 LOAD_GLOBAL             21 (NULL + redirect)
+         264         292 LOAD_GLOBAL             21 (NULL + redirect)
                      304 LOAD_FAST                4 (post)
                      306 PRECALL                  1
                      310 CALL                     1
                      320 RETURN_VALUE
          
-         251     >>  322 LOAD_CONST               0 (None)
+         258     >>  322 LOAD_CONST               0 (None)
                      324 RETURN_VALUE
          consts
             None
             ('pk',)
             'Cannot add posts to a closed thread.'
             False
             ('commit',)
          names      ('get_object_or_404', 'Thread', 'is_closed', 'HttpResponseForbidden', 'PostModelForm', 'POST', 'is_valid', 'save', 'thread', 'user', 'redirect')
          varnames   ('request', 'thread_id', 'thread', 'form', 'post')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'post_create_view'
-         firstlineno 242
+         firstlineno 249
          lnotab 0x02022c020e011e02280228012c010e01180128021efa
       code
          argcount  : 2
          nlocals   : 5
          stacksize : 5
          flags     : 3
          code
@@ -1582,75 +1655,75 @@
             0000007d037c03a0060000000000000000000000000000000000000000a6
             000000ab00000000000000000072237c03a0070000000000000000000000
             000000000000000000a6000000ab0000000000000000007d027411000000
             000000000000007c02a6010000ab01000000000000000053007409000000
             000000000000007c02ac03a6010000ab0100000000000000007d037c027c
             0364049c027d047413000000000000000000007c0064057c04ac06a60300
             00ab0300000000000000005300
-         260           0 RESUME                   0
+         267           0 RESUME                   0
          
-         262           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+         269           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
                       14 LOAD_GLOBAL              2 (Post)
                       26 LOAD_FAST                1 (post_id)
                       28 LOAD_FAST                0 (request)
                       30 LOAD_ATTR                2 (user)
                       40 KW_NAMES                 1
                       42 PRECALL                  3
                       46 CALL                     3
                       56 STORE_FAST               2 (post)
          
-         264          58 LOAD_FAST                0 (request)
+         271          58 LOAD_FAST                0 (request)
                       60 LOAD_ATTR                3 (method)
                       70 LOAD_CONST               2 ('POST')
                       72 COMPARE_OP               2 (==)
                       78 POP_JUMP_FORWARD_IF_FALSE    77 (to 234)
          
-         265          80 LOAD_GLOBAL              9 (NULL + PostModelForm)
+         272          80 LOAD_GLOBAL              9 (NULL + PostModelForm)
                       92 LOAD_FAST                0 (request)
                       94 LOAD_ATTR                5 (POST)
                      104 LOAD_FAST                2 (post)
                      106 KW_NAMES                 3
                      108 PRECALL                  2
                      112 CALL                     2
                      122 STORE_FAST               3 (form)
          
-         267         124 LOAD_FAST                3 (form)
+         274         124 LOAD_FAST                3 (form)
                      126 LOAD_METHOD              6 (is_valid)
                      148 PRECALL                  0
                      152 CALL                     0
                      162 POP_JUMP_FORWARD_IF_FALSE    35 (to 234)
          
-         268         164 LOAD_FAST                3 (form)
+         275         164 LOAD_FAST                3 (form)
                      166 LOAD_METHOD              7 (save)
                      188 PRECALL                  0
                      192 CALL                     0
                      202 STORE_FAST               2 (post)
          
-         270         204 LOAD_GLOBAL             17 (NULL + redirect)
+         277         204 LOAD_GLOBAL             17 (NULL + redirect)
                      216 LOAD_FAST                2 (post)
                      218 PRECALL                  1
                      222 CALL                     1
                      232 RETURN_VALUE
          
-         272     >>  234 LOAD_GLOBAL              9 (NULL + PostModelForm)
+         279     >>  234 LOAD_GLOBAL              9 (NULL + PostModelForm)
                      246 LOAD_FAST                2 (post)
                      248 KW_NAMES                 3
                      250 PRECALL                  1
                      254 CALL                     1
                      264 STORE_FAST               3 (form)
          
-         275         266 LOAD_FAST                2 (post)
+         282         266 LOAD_FAST                2 (post)
          
-         276         268 LOAD_FAST                3 (form)
+         283         268 LOAD_FAST                3 (form)
          
-         274         270 LOAD_CONST               4 (('post', 'form'))
+         281         270 LOAD_CONST               4 (('post', 'form'))
                      272 BUILD_CONST_KEY_MAP      2
                      274 STORE_FAST               4 (context)
          
-         279         276 LOAD_GLOBAL             19 (NULL + render)
+         286         276 LOAD_GLOBAL             19 (NULL + render)
                      288 LOAD_FAST                0 (request)
                      290 LOAD_CONST               5 ('punkweb_bb/partials/post_update.html')
                      292 LOAD_FAST                4 (context)
                      294 KW_NAMES                 6
                      296 PRECALL                  3
                      300 CALL                     3
                      310 RETURN_VALUE
@@ -1664,15 +1737,15 @@
             ('context',)
          names      ('get_object_or_404', 'Post', 'user', 'method', 'PostModelForm', 'POST', 'is_valid', 'save', 'redirect', 'render')
          varnames   ('request', 'post_id', 'post', 'form', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'post_update_view'
-         firstlineno 260
+         firstlineno 267
          lnotab 0x0202380216012c02280128021e022003020102fe0605
       code
          argcount  : 2
          nlocals   : 4
          stacksize : 5
          flags     : 3
          code
@@ -1681,55 +1754,55 @@
             006a03000000000000000064026b0200000000723a7c02a0040000000000
             000000000000000000000000000000a6000000ab00000000000000000001
             00740b000000000000000000007c026a060000000000000000a007000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00a6010000ab010000000000000000530064037c0269017d037411000000
             000000000000007c0064047c03ac05a6030000ab03000000000000000053
             00
-         282           0 RESUME                   0
+         289           0 RESUME                   0
          
-         284           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+         291           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
                       14 LOAD_GLOBAL              2 (Post)
                       26 LOAD_FAST                1 (post_id)
                       28 LOAD_FAST                0 (request)
                       30 LOAD_ATTR                2 (user)
                       40 KW_NAMES                 1
                       42 PRECALL                  3
                       46 CALL                     3
                       56 STORE_FAST               2 (post)
          
-         286          58 LOAD_FAST                0 (request)
+         293          58 LOAD_FAST                0 (request)
                       60 LOAD_ATTR                3 (method)
                       70 LOAD_CONST               2 ('DELETE')
                       72 COMPARE_OP               2 (==)
                       78 POP_JUMP_FORWARD_IF_FALSE    58 (to 196)
          
-         287          80 LOAD_FAST                2 (post)
+         294          80 LOAD_FAST                2 (post)
                       82 LOAD_METHOD              4 (delete)
                      104 PRECALL                  0
                      108 CALL                     0
                      118 POP_TOP
          
-         289         120 LOAD_GLOBAL             11 (NULL + htmx_redirect)
+         296         120 LOAD_GLOBAL             11 (NULL + htmx_redirect)
                      132 LOAD_FAST                2 (post)
                      134 LOAD_ATTR                6 (thread)
                      144 LOAD_METHOD              7 (get_absolute_url)
                      166 PRECALL                  0
                      170 CALL                     0
                      180 PRECALL                  1
                      184 CALL                     1
                      194 RETURN_VALUE
          
-         292     >>  196 LOAD_CONST               3 ('post')
+         299     >>  196 LOAD_CONST               3 ('post')
                      198 LOAD_FAST                2 (post)
          
-         291         200 BUILD_MAP                1
+         298         200 BUILD_MAP                1
                      202 STORE_FAST               3 (context)
          
-         295         204 LOAD_GLOBAL             17 (NULL + render)
+         302         204 LOAD_GLOBAL             17 (NULL + render)
                      216 LOAD_FAST                0 (request)
                      218 LOAD_CONST               4 ('punkweb_bb/partials/post_delete.html')
                      220 LOAD_FAST                3 (context)
                      222 KW_NAMES                 5
                      224 PRECALL                  3
                      228 CALL                     3
                      238 RETURN_VALUE
@@ -1742,94 +1815,94 @@
             ('context',)
          names      ('get_object_or_404', 'Post', 'user', 'method', 'delete', 'htmx_redirect', 'thread', 'get_absolute_url', 'render')
          varnames   ('request', 'post_id', 'post', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'post_delete_view'
-         firstlineno 282
+         firstlineno 289
          lnotab 0x02023802160128024c0304ff0404
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 6
          flags     : 3
          code
             0x97007400000000000000000000006a010000000000000000a002000000
             00000000000000000000000000000000007407000000000000000000006a
             040000000000000000a6000000ab000000000000000000740b0000000000
             00000000006a0600000000000000006401ac02a6010000ab010000000000
             0000007a0a0000ac03a6010000ab010000000000000000a0070000000000
             0000000000000000000000000000006404a6010000ab0100000000000000
             005300
-         298           0 RESUME                   0
+         305           0 RESUME                   0
          
-         299           2 LOAD_GLOBAL              0 (Shout)
+         306           2 LOAD_GLOBAL              0 (Shout)
                       14 LOAD_ATTR                1 (objects)
                       24 LOAD_METHOD              2 (filter)
          
-         300          46 LOAD_GLOBAL              7 (NULL + timezone)
+         307          46 LOAD_GLOBAL              7 (NULL + timezone)
                       58 LOAD_ATTR                4 (now)
                       68 PRECALL                  0
                       72 CALL                     0
                       82 LOAD_GLOBAL             11 (NULL + datetime)
                       94 LOAD_ATTR                6 (timedelta)
                      104 LOAD_CONST               1 (12)
                      106 KW_NAMES                 2
                      108 PRECALL                  1
                      112 CALL                     1
                      122 BINARY_OP               10 (-)
          
-         299         126 KW_NAMES                 3
+         306         126 KW_NAMES                 3
                      128 PRECALL                  1
                      132 CALL                     1
          
-         301         142 LOAD_METHOD              7 (order_by)
+         308         142 LOAD_METHOD              7 (order_by)
                      164 LOAD_CONST               4 ('created_at')
                      166 PRECALL                  1
                      170 CALL                     1
          
-         299         180 RETURN_VALUE
+         306         180 RETURN_VALUE
          consts
             None
             12
             ('hours',)
             ('created_at__gt',)
             'created_at'
          names      ('Shout', 'objects', 'filter', 'timezone', 'now', 'datetime', 'timedelta', 'order_by')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'current_shouts'
-         firstlineno 298
+         firstlineno 305
          lnotab 0x02012c0150ff100226fe
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 5
          flags     : 3
          code
             0x9700740100000000000000000000a6000000ab0000000000000000007d
             0164017c0169017d027403000000000000000000007c0064027c02ac03a6
             030000ab0300000000000000005300
-         304           0 RESUME                   0
+         311           0 RESUME                   0
          
-         305           2 LOAD_GLOBAL              1 (NULL + current_shouts)
+         312           2 LOAD_GLOBAL              1 (NULL + current_shouts)
                       14 PRECALL                  0
                       18 CALL                     0
                       28 STORE_FAST               1 (shouts)
          
-         308          30 LOAD_CONST               1 ('shouts')
+         315          30 LOAD_CONST               1 ('shouts')
                       32 LOAD_FAST                1 (shouts)
          
-         307          34 BUILD_MAP                1
+         314          34 BUILD_MAP                1
                       36 STORE_FAST               2 (context)
          
-         310          38 LOAD_GLOBAL              3 (NULL + render)
+         317          38 LOAD_GLOBAL              3 (NULL + render)
                       50 LOAD_FAST                0 (request)
                       52 LOAD_CONST               2 ('punkweb_bb/shoutbox/shout_list.html')
                       54 LOAD_FAST                2 (context)
                       56 KW_NAMES                 3
                       58 PRECALL                  3
                       62 CALL                     3
                       72 RETURN_VALUE
@@ -1840,15 +1913,15 @@
             ('context',)
          names      ('current_shouts', 'render')
          varnames   ('request', 'shouts', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'shout_list_view'
-         firstlineno 304
+         firstlineno 311
          lnotab 0x02011c0304ff0403
       code
          argcount  : 1
          nlocals   : 4
          stacksize : 5
          flags     : 3
          code
@@ -1861,99 +1934,99 @@
             00a6000000ab000000000000000000725a7c02a008000000000000000000
             00000000000000000000006405ac06a6010000ab0100000000000000007d
             037c006a0000000000000000007c035f0000000000000000007c03a00800
             00000000000000000000000000000000000000a6000000ab000000000000
             00000001006401740500000000000000000000a6000000ab000000000000
             00000069017d017407000000000000000000007c0064027c01ac03a60300
             00ab03000000000000000053006400530064005300
-         313           0 RESUME                   0
+         320           0 RESUME                   0
          
-         314           2 LOAD_FAST                0 (request)
+         321           2 LOAD_FAST                0 (request)
                        4 LOAD_ATTR                0 (user)
                       14 LOAD_ATTR                1 (is_authenticated)
                       24 POP_JUMP_FORWARD_IF_TRUE    34 (to 94)
          
-         316          26 LOAD_CONST               1 ('shouts')
+         323          26 LOAD_CONST               1 ('shouts')
                       28 LOAD_GLOBAL              5 (NULL + current_shouts)
                       40 PRECALL                  0
                       44 CALL                     0
          
-         315          54 BUILD_MAP                1
+         322          54 BUILD_MAP                1
                       56 STORE_FAST               1 (context)
          
-         318          58 LOAD_GLOBAL              7 (NULL + render)
+         325          58 LOAD_GLOBAL              7 (NULL + render)
                       70 LOAD_FAST                0 (request)
                       72 LOAD_CONST               2 ('punkweb_bb/shoutbox/shout_list.html')
                       74 LOAD_FAST                1 (context)
                       76 KW_NAMES                 3
                       78 PRECALL                  3
                       82 CALL                     3
                       92 RETURN_VALUE
          
-         320     >>   94 LOAD_FAST                0 (request)
+         327     >>   94 LOAD_FAST                0 (request)
                       96 LOAD_ATTR                4 (method)
                      106 LOAD_CONST               4 ('POST')
                      108 COMPARE_OP               2 (==)
                      114 POP_JUMP_FORWARD_IF_FALSE   128 (to 372)
          
-         321         116 LOAD_GLOBAL             11 (NULL + ShoutModelForm)
+         328         116 LOAD_GLOBAL             11 (NULL + ShoutModelForm)
                      128 LOAD_FAST                0 (request)
                      130 LOAD_ATTR                6 (POST)
                      140 PRECALL                  1
                      144 CALL                     1
                      154 STORE_FAST               2 (form)
          
-         323         156 LOAD_FAST                2 (form)
+         330         156 LOAD_FAST                2 (form)
                      158 LOAD_METHOD              7 (is_valid)
                      180 PRECALL                  0
                      184 CALL                     0
                      194 POP_JUMP_FORWARD_IF_FALSE    90 (to 376)
          
-         324         196 LOAD_FAST                2 (form)
+         331         196 LOAD_FAST                2 (form)
                      198 LOAD_METHOD              8 (save)
                      220 LOAD_CONST               5 (False)
                      222 KW_NAMES                 6
                      224 PRECALL                  1
                      228 CALL                     1
                      238 STORE_FAST               3 (shout)
          
-         325         240 LOAD_FAST                0 (request)
+         332         240 LOAD_FAST                0 (request)
                      242 LOAD_ATTR                0 (user)
                      252 LOAD_FAST                3 (shout)
                      254 STORE_ATTR               0 (user)
          
-         326         264 LOAD_FAST                3 (shout)
+         333         264 LOAD_FAST                3 (shout)
                      266 LOAD_METHOD              8 (save)
                      288 PRECALL                  0
                      292 CALL                     0
                      302 POP_TOP
          
-         329         304 LOAD_CONST               1 ('shouts')
+         336         304 LOAD_CONST               1 ('shouts')
                      306 LOAD_GLOBAL              5 (NULL + current_shouts)
                      318 PRECALL                  0
                      322 CALL                     0
          
-         328         332 BUILD_MAP                1
+         335         332 BUILD_MAP                1
                      334 STORE_FAST               1 (context)
          
-         331         336 LOAD_GLOBAL              7 (NULL + render)
+         338         336 LOAD_GLOBAL              7 (NULL + render)
          
-         332         348 LOAD_FAST                0 (request)
+         339         348 LOAD_FAST                0 (request)
                      350 LOAD_CONST               2 ('punkweb_bb/shoutbox/shout_list.html')
                      352 LOAD_FAST                1 (context)
          
-         331         354 KW_NAMES                 3
+         338         354 KW_NAMES                 3
                      356 PRECALL                  3
                      360 CALL                     3
                      370 RETURN_VALUE
          
-         320     >>  372 LOAD_CONST               0 (None)
+         327     >>  372 LOAD_CONST               0 (None)
                      374 RETURN_VALUE
          
-         323     >>  376 LOAD_CONST               0 (None)
+         330     >>  376 LOAD_CONST               0 (None)
                      378 RETURN_VALUE
          consts
             None
             'shouts'
             'punkweb_bb/shoutbox/shout_list.html'
             ('context',)
             'POST'
@@ -1961,38 +2034,38 @@
             ('commit',)
          names      ('user', 'is_authenticated', 'current_shouts', 'render', 'method', 'ShoutModelForm', 'POST', 'is_valid', 'save')
          varnames   ('request', 'context', 'form', 'shout')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'shout_create_view'
-         firstlineno 313
+         firstlineno 320
          lnotab
             0x020118021cff040324021601280228012c01180128031cff04030c0106
             ff12f50403
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 5
          flags     : 3
          code
             0x970064017d0164027c0169017d027401000000000000000000007c0064
             037c02ac04a6030000ab0300000000000000005300
-         336           0 RESUME                   0
+         343           0 RESUME                   0
          
-         337           2 LOAD_CONST               1 ((('Bold', '[b]Bold Text[/b]'), ('Italic', '[i]Italic Text[/i]'), ('Underline', '[u]Underlined Text[/u]'), ('Strikethrough', '[s]Strikethrough Text[/s]'), ('Quote', '[quote=Example]Quoted Text[/quote]'), ('Center', '[center]Centered Text[/center]'), ('Color', '[color=red]Red Text[/color]'), ('Url', '[url=https://google.com]Link Text[/url]'), ('Image', '[img]https://placehold.co/400[/img]'), ('Horizontal Rule', '[hr]'), ('Code', '\n[code=python]\nclass ThreadModelForm(forms.ModelForm):\n    class Meta:\n        model = Thread\n        fields = (\n            "title",\n            "content",\n        )\n        widgets = {\n            "title": forms.TextInput(attrs={"autofocus": True, "class": "pw-input"}),\n            "content": BBCodeEditorWidget(),\n        }\n[/code]\n'), ('Email', '[email=test@example.com]Example[/email]'), ('Font', '[font=serif]Serif Text[/font]'), ('Ordered List', '[ol][li]Item 1[/li][li]Item 2[/li][/ol]'), ('Unordered List', '[ul][li]Item 1[/li][li]Item 2[/li][/ul]'), ('Shadow', '[shadow=red]Red Shadow Text[/shadow]'), ('Size', '[size=7]Size 7 Text[/size]'), ('Checkbox', '\n[n]Unchecked\n[y]Checked\n            '), ('Superscript', 'Sup [sup]Superscript Text[/sup]'), ('Subscript', 'Sub [sub]Subscript Text[/sub]'), ('Left', '[left]Left Text[/left]'), ('Right', '[right]Right Text[/right]'), ('Escape', '[escape][b]Escaped bbcode[/b][/escape]')))
+         344           2 LOAD_CONST               1 ((('Bold', '[b]Bold Text[/b]'), ('Italic', '[i]Italic Text[/i]'), ('Underline', '[u]Underlined Text[/u]'), ('Strikethrough', '[s]Strikethrough Text[/s]'), ('Quote', '[quote=Example]Quoted Text[/quote]'), ('Center', '[center]Centered Text[/center]'), ('Color', '[color=red]Red Text[/color]'), ('Url', '[url=https://google.com]Link Text[/url]'), ('Image', '[img]https://placehold.co/400[/img]'), ('Horizontal Rule', '[hr]'), ('Code', '\n[code=python]\nclass ThreadModelForm(forms.ModelForm):\n    class Meta:\n        model = Thread\n        fields = (\n            "title",\n            "content",\n        )\n        widgets = {\n            "title": forms.TextInput(attrs={"autofocus": True, "class": "pw-input"}),\n            "content": BBCodeEditorWidget(),\n        }\n[/code]\n'), ('Email', '[email=test@example.com]Example[/email]'), ('Font', '[font=serif]Serif Text[/font]'), ('Ordered List', '[ol][li]Item 1[/li][li]Item 2[/li][/ol]'), ('Unordered List', '[ul][li]Item 1[/li][li]Item 2[/li][/ul]'), ('Shadow', '[shadow=red]Red Shadow Text[/shadow]'), ('Size', '[size=7]Size 7 Text[/size]'), ('Checkbox', '\n[n]Unchecked\n[y]Checked\n            '), ('Superscript', 'Sup [sup]Superscript Text[/sup]'), ('Subscript', 'Sub [sub]Subscript Text[/sub]'), ('Left', '[left]Left Text[/left]'), ('Right', '[right]Right Text[/right]'), ('Escape', '[escape][b]Escaped bbcode[/b][/escape]')))
                        4 STORE_FAST               1 (codes)
          
-         391           6 LOAD_CONST               2 ('codes')
+         398           6 LOAD_CONST               2 ('codes')
                        8 LOAD_FAST                1 (codes)
          
-         390          10 BUILD_MAP                1
+         397          10 BUILD_MAP                1
                       12 STORE_FAST               2 (context)
          
-         394          14 LOAD_GLOBAL              1 (NULL + render)
+         401          14 LOAD_GLOBAL              1 (NULL + render)
                       26 LOAD_FAST                0 (request)
                       28 LOAD_CONST               3 ('punkweb_bb/bbcode.html')
                       30 LOAD_FAST                2 (context)
                       32 KW_NAMES                 4
                       34 PRECALL                  3
                       38 CALL                     3
                       48 RETURN_VALUE
@@ -2004,21 +2077,21 @@
             ('context',)
          names      ('render',)
          varnames   ('request', 'codes', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'bbcode_view'
-         firstlineno 336
+         firstlineno 343
          lnotab 0x0201043604ff0404
-   names      ('datetime', 'django.contrib.auth', 'authenticate', 'get_user_model', 'login', 'logout', 'django.contrib.auth.decorators', 'login_required', 'django.http', 'HttpResponseForbidden', 'django.shortcuts', 'get_object_or_404', 'redirect', 'render', 'django.utils', 'timezone', 'punkweb_bb.forms', 'BoardProfileModelForm', 'LoginForm', 'PostModelForm', 'ShoutModelForm', 'SignUpForm', 'ThreadModelForm', 'punkweb_bb.models', 'Category', 'Post', 'Shout', 'Subcategory', 'Thread', 'punkweb_bb.pagination', 'paginate_qs', 'punkweb_bb.response', 'htmx_redirect', 'User', 'index_view', 'login_view', 'logout_view', 'signup_view', 'profile_view', 'members_view', 'settings_view', 'subcategory_view', 'thread_create_view', 'thread_view', 'thread_update_view', 'thread_delete_view', 'post_create_view', 'post_update_view', 'post_delete_view', 'current_shouts', 'shout_list_view', 'shout_create_view', 'bbcode_view')
+   names      ('datetime', 'django.contrib.auth', 'authenticate', 'get_user_model', 'login', 'logout', 'django.contrib.auth.decorators', 'login_required', 'django.http', 'HttpResponseForbidden', 'django.shortcuts', 'get_object_or_404', 'redirect', 'render', 'django.utils', 'timezone', 'punkweb_bb.guests', 'guest_list', 'punkweb_bb.forms', 'BoardProfileModelForm', 'LoginForm', 'PostModelForm', 'ShoutModelForm', 'SignUpForm', 'ThreadModelForm', 'punkweb_bb.models', 'Category', 'Post', 'Shout', 'Subcategory', 'Thread', 'punkweb_bb.pagination', 'paginate_qs', 'punkweb_bb.response', 'htmx_redirect', 'User', 'index_view', 'login_view', 'logout_view', 'signup_view', 'profile_view', 'members_view', 'settings_view', 'subcategory_view', 'thread_create_view', 'thread_view', 'thread_update_view', 'thread_delete_view', 'post_create_view', 'post_update_view', 'post_delete_view', 'current_shouts', 'shout_list_view', 'shout_create_view', 'bbcode_view')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff0201080218010c010c0114010c0220081c010c010c021403061a06
-      1a060506140609060b160104ff0e010216060c160104ff0e01021a061616
-      0104ff0e010214160104ff0e01020f160104ff0e010211160104ff0e0102
-      15160104ff0e01020f060606090617
+      0x00ff0201080218010c010c0114010c020c0120081c010c010c02140306
+      20061a060506140609060b160104ff0e010216060c160104ff0e01021a06
+      16160104ff0e010214160104ff0e01020f160104ff0e010211160104ff0e
+      010215160104ff0e01020f060606090617
```

### Comparing `punkweb_bb-0.1.3/punkweb_bb/__pycache__/widgets.cpython-311.pyc` & `punkweb_bb-0.1.4/punkweb_bb/__pycache__/widgets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/admin.py` & `punkweb_bb-0.1.4/punkweb_bb/admin.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/admin_forms.py` & `punkweb_bb-0.1.4/punkweb_bb/admin_forms.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/bbcode_tags.py` & `punkweb_bb-0.1.4/punkweb_bb/bbcode_tags.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/forms.py` & `punkweb_bb-0.1.4/punkweb_bb/forms.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/migrations/0001_initial.py` & `punkweb_bb-0.1.4/punkweb_bb/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/migrations/__pycache__/0001_initial.cpython-311.pyc` & `punkweb_bb-0.1.4/punkweb_bb/migrations/__pycache__/0001_initial.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/migrations/__pycache__/0002_thread_view_count.cpython-311.pyc` & `punkweb_bb-0.1.4/punkweb_bb/migrations/__pycache__/0002_thread_view_count.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/models.py` & `punkweb_bb-0.1.4/punkweb_bb/models.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/parsers.py` & `punkweb_bb-0.1.4/punkweb_bb/parsers.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/defaults.css` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/defaults.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/index.css` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/index.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/profile.css` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/profile.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/punkweb-modal.css` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/punkweb-modal.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/punkweb.css` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/punkweb.css`

 * *Files 3% similar despite different names*

```diff
@@ -642,7 +642,30 @@
   padding: 0 0.5rem;
   pointer-events: none;
 }
 
 .pw-breadcrumb-item.active {
   color: var(--breadcrumb-active);
 }
+
+/* Callout */
+
+.pw-callout {
+  background-color: var(--oc-gray-1);
+  border: 1px solid var(--border);
+  border-radius: 0.25rem;
+  color: var(--oc-gray-9);
+  padding: 0.5rem 1rem;
+  width: 100%;
+}
+
+.pw-callout.primary {
+  background-color: var(--primary-0);
+  border-color: 1px solid var(--primary-4);
+  color: var(--primary-9);
+}
+
+.pw-callout.danger {
+  background-color: var(--oc-red-0);
+  border-color: 1px solid var(--oc-red-4);
+  color: var(--oc-red-9);
+}
```

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/subcategory.css` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/subcategory.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/thread.css` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/thread.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/css/variables.css` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/variables.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-content.css` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-content.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-tags.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-tags.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/img/default-profile-image.png` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/img/default-profile-image.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/htmx-1.9.4.min.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/htmx-1.9.4.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/jquery-3.7.0.min.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/jquery-3.7.0.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/open-color.css` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/open-color.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/prism.css` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/prism.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/prism.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/prism.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/README.md` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/bbcode.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/bbcode.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/xhtml.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/xhtml.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/material.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/material.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/monocons.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/monocons.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.bbcode.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.bbcode.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.xhtml.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.xhtml.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/alternative-lists.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/alternative-lists.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autosave.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autosave.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autoyoutube.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autoyoutube.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/dragdrop.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/dragdrop.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/format.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/format.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/plaintext.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/plaintext.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/undo.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/undo.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/v1compat.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/v1compat.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/sceditor.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/sceditor.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/default.css` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/default.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/default.css` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/default.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/defaultdark.css` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/defaultdark.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/famfamfam.png` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/famfamfam.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/modern.css` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/modern.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office-toolbar.css` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office-toolbar.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office.css` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/square.css` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/square.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/alien.png` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/alien.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angel.png` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angel.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angry.png` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angry.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blink.png` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blink.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blush.png` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blush.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cheerful.png` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cheerful.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cool.png` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cool.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cwy.png` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cwy.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/devil.png` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/devil.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/dizzy.png` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/dizzy.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ermm.png` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ermm.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/face.png` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/face.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/getlost.png` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/getlost.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/grin.png` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/grin.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/happy.png` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/happy.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/heart.png` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/heart.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/kissing.png` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/kissing.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/laughing.png` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/laughing.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ninja.png` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ninja.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pinch.png` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pinch.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pouty.png` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pouty.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sad.png` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sad.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/shocked.png` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/shocked.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sick.png` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sick.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sideways.png` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sideways.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/silly.png` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/silly.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sleeping.png` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sleeping.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/smile.png` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/smile.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/tongue.png` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/tongue.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/unsure.png` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/unsure.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/w00t.png` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/w00t.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wassat.png` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wassat.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/whistling.png` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/whistling.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wink.png` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wink.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wub.png` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wub.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/example.html` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/example.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ar.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ar.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ca.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ca.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cn.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cn.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cs.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cs.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/de.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/de.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/el.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/el.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/es.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/es.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/et.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/et.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fa.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fa.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fi.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fi.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fr.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fr.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/gl.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/gl.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/hu.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/hu.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/id.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/id.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/it.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/it.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ja.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ja.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/lt.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/lt.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nb.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nb.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nl.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nl.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pl.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pl.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt-BR.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt-BR.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ru.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ru.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sk.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sk.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sv.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sv.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/template.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/template.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tr.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tr.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tw.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tw.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/uk.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/uk.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/vi.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/vi.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/bbcode.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/bbcode.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/xhtml.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/xhtml.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/material.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/material.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/monocons.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/monocons.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.bbcode.min.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.bbcode.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.min.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.xhtml.min.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.xhtml.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/alternative-lists.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/alternative-lists.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autosave.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autosave.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autoyoutube.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autoyoutube.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/dragdrop.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/dragdrop.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/format.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/format.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/plaintext.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/plaintext.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/undo.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/undo.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/v1compat.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/v1compat.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/sceditor.min.js` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/sceditor.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/default.min.css` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/default.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/default.min.css` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/default.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/defaultdark.min.css` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/defaultdark.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/famfamfam.png` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/famfamfam.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/modern.min.css` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/modern.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office-toolbar.min.css` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office-toolbar.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office.min.css` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/square.min.css` & `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/square.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/base.html` & `punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/base.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/index.html` & `punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/index.html`

 * *Files 16% similar despite different names*

```diff
@@ -167,22 +167,35 @@
                 <a href="{% url 'punkweb_bb:profile' newest_user.id %}">
                   {{newest_user.username}}
                 </a>
               </div>
             </div>
             {% endif %}
             <div class="index__statistics__row">
-              <div class="index__statistics__label">Members online:</div>
-              <div class="index__statistics__value">{{users_online|length}}</div>
-            </div>
-            <div class="index__statistics__row">
-              <div class="index__statistics__label">Staff online:</div>
-              <div class="index__statistics__value">{{staff_online|length}}</div>
+              <div class="index__statistics__label">Users online:</div>
+              <div class="index__statistics__value">{{total_online}} ({{members_online|length}} members, {{staff_online|length}} staff, {{guests_online}} guests)</div>
             </div>
           </div>
         </div>
       </div>
+      {% if punkweb_bb.settings.DISCORD_WIDGET_ENABLED %}
+      {% if punkweb_bb.settings.DISCORD_SERVER_ID %}
+      <iframe
+        src="https://discord.com/widget?id={{ punkweb_bb.settings.DISCORD_SERVER_ID }}&theme={{ punkweb_bb.settings.DISCORD_WIDGET_THEME|default:'dark' }}"
+        width="100%"
+        height="384"
+        allowtransparency="true"
+        frameborder="0"
+        sandbox="allow-popups allow-popups-to-escape-sandbox allow-same-origin allow-scripts">
+      </iframe>
+      {% else %}
+      <div class="pw-callout danger">
+        <h4>Discord Widget Error</h4>
+        <p><code>DISCORD_SERVER_ID</code> not configured in settings module.</p>
+      </div>
+      {% endif %}
+      {% endif %}
     </div>
   </div>
 </div>
 
 {% endblock %}
```

#### html2text {}

```diff
@@ -43,12 +43,16 @@
 {{post_count}}
 Total members:
 {{users|length}}
 {% if newest_user %}
 Newest member:
 _{_{_n_e_w_e_s_t___u_s_e_r_._u_s_e_r_n_a_m_e_}_}
 {% endif %}
-Members online:
-{{users_online|length}}
-Staff online:
-{{staff_online|length}}
+Users online:
+{{total_online}} ({{members_online|length}} members, {{staff_online|length}}
+staff, {{guests_online}} guests)
+{% if punkweb_bb.settings.DISCORD_WIDGET_ENABLED %} {% if
+punkweb_bb.settings.DISCORD_SERVER_ID %} {% else %}
+****** DDiissccoorrdd WWiiddggeett EErrrroorr ******
+DISCORD_SERVER_ID not configured in settings module.
+{% endif %} {% endif %}
 {% endblock %}
```

### Comparing `punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/login.html` & `punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/login.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/members.html` & `punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/members.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/partials/post_update.html` & `punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/partials/post_update.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/profile.html` & `punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/profile.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/settings.html` & `punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/settings.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/shoutbox/shoutbox.html` & `punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/shoutbox/shoutbox.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/signup.html` & `punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/signup.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/subcategory.html` & `punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/subcategory.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/thread.html` & `punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/thread.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/thread_create.html` & `punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/thread_create.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/templates/punkweb_bb/thread_update.html` & `punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/thread_update.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/templatetags/__pycache__/humanize_count.cpython-311.pyc` & `punkweb_bb-0.1.4/punkweb_bb/templatetags/__pycache__/humanize_count.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/templatetags/__pycache__/humanize_int.cpython-311.pyc` & `punkweb_bb-0.1.4/punkweb_bb/templatetags/__pycache__/humanize_int.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/templatetags/__pycache__/shoutbox_bbcode.cpython-311.pyc` & `punkweb_bb-0.1.4/punkweb_bb/templatetags/__pycache__/shoutbox_bbcode.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/tests.py` & `punkweb_bb-0.1.4/punkweb_bb/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -295,32 +295,43 @@
         self.client = Client()
         self.url = reverse("punkweb_bb:index")
         self.user = User.objects.create(username="test", password="test")
         self.staff_user = User.objects.create(
             username="staff", password="staff", is_staff=True
         )
 
-    def test_users_online(self):
+    def test_members_online(self):
         response = self.client.get(self.url)
-        self.assertEqual(len(response.context["users_online"]), 0)
+        self.assertEqual(len(response.context["members_online"]), 0)
 
         self.client.force_login(self.user)
         response = self.client.get(self.url)
 
-        self.assertEqual(len(response.context["users_online"]), 1)
+        self.assertEqual(len(response.context["members_online"]), 1)
 
     def test_staff_online(self):
         response = self.client.get(self.url)
         self.assertEqual(len(response.context["staff_online"]), 0)
 
         self.client.force_login(self.staff_user)
         response = self.client.get(self.url)
 
         self.assertEqual(len(response.context["staff_online"]), 1)
 
+    def test_guests_online(self):
+        response = self.client.get(self.url)
+        self.assertEqual(response.context["guests_online"], 1)
+
+    def test_total_online(self):
+        response = self.client.get(self.url)
+        self.client.force_login(self.user)
+        response = self.client.get(self.url)
+
+        self.assertEqual(response.context["total_online"], 2)
+
     def test_newest_user(self):
         response = self.client.get(self.url)
         self.assertEqual(response.context["newest_user"], self.staff_user)
 
     def test_users_count(self):
         response = self.client.get(self.url)
         self.assertEqual(response.context["users"].count(), 2)
```

### Comparing `punkweb_bb-0.1.3/punkweb_bb/urls.py` & `punkweb_bb-0.1.4/punkweb_bb/urls.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb/views.py` & `punkweb_bb-0.1.4/punkweb_bb/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from django.contrib.auth import authenticate, get_user_model, login, logout
 from django.contrib.auth.decorators import login_required
 from django.http import HttpResponseForbidden
 from django.shortcuts import get_object_or_404, redirect, render
 from django.utils import timezone
 
+from punkweb_bb.guests import guest_list
 from punkweb_bb.forms import (
     BoardProfileModelForm,
     LoginForm,
     PostModelForm,
     ShoutModelForm,
     SignUpForm,
     ThreadModelForm,
@@ -27,26 +28,32 @@
     recent_threads = Thread.objects.all().order_by("-created_at")[:5]
 
     thread_count = Thread.objects.count()
     post_count = Post.objects.count()
 
     users = User.objects.select_related("profile").all()
     newest_user = users.order_by("-profile__created_at").first()
+
     users_online = [user for user in users if user.profile.is_online]
+    members_online = [user for user in users_online if not user.is_staff]
     staff_online = [user for user in users_online if user.is_staff]
+    guests_online = guest_list.length()
+    total_online = len(members_online) + len(staff_online) + guests_online
 
     context = {
         "categories": categories,
         "recent_threads": recent_threads,
         "thread_count": thread_count,
         "post_count": post_count,
         "users": users,
         "newest_user": newest_user,
-        "users_online": users_online,
+        "members_online": members_online,
         "staff_online": staff_online,
+        "guests_online": guests_online,
+        "total_online": total_online,
     }
     return render(request, "punkweb_bb/index.html", context=context)
 
 
 def login_view(request):
     if request.user.is_authenticated:
         return redirect("punkweb_bb:index")
```

### Comparing `punkweb_bb-0.1.3/punkweb_bb/widgets.py` & `punkweb_bb-0.1.4/punkweb_bb/widgets.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.3/punkweb_bb.egg-info/PKG-INFO` & `punkweb_bb-0.1.4/punkweb_bb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: punkweb-bb
-Version: 0.1.3
+Version: 0.1.4
 Summary: Django application that provides a simple and modern forum board software for your Django website.
 Home-page: https://github.com/Punkweb/PunkwebBB
 Author: Punkweb
 Author-email: punkwebnet@gmail.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -108,14 +108,17 @@
 
 ```python
 PUNKWEB_BB = {
   "SITE_NAME": "PUNKWEB",
   "SITE_TITLE": "PunkwebBB",
   "FAVICON": "punkweb_bb/favicon.ico",
   "SHOUTBOX_ENABLED": True,
+  "DISCORD_WIDGET_ENABLED": False,
+  "DISCORD_WIDGET_THEME": "dark",
+  "DISCORD_SERVER_ID": None, # Found under Server Settings > Widget > Server ID
 }
 ```
 
 ## Testing
 
 Report:
```

### Comparing `punkweb_bb-0.1.3/punkweb_bb.egg-info/SOURCES.txt` & `punkweb_bb-0.1.4/punkweb_bb.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 punkweb_bb/__init__.py
 punkweb_bb/admin.py
 punkweb_bb/admin_forms.py
 punkweb_bb/apps.py
 punkweb_bb/bbcode_tags.py
 punkweb_bb/context_processors.py
 punkweb_bb/forms.py
+punkweb_bb/guests.py
 punkweb_bb/middleware.py
 punkweb_bb/mixins.py
 punkweb_bb/models.py
 punkweb_bb/pagination.py
 punkweb_bb/parsers.py
 punkweb_bb/response.py
 punkweb_bb/settings.py
@@ -30,14 +31,15 @@
 punkweb_bb/__pycache__/__init__.cpython-311.pyc
 punkweb_bb/__pycache__/admin.cpython-311.pyc
 punkweb_bb/__pycache__/admin_forms.cpython-311.pyc
 punkweb_bb/__pycache__/apps.cpython-311.pyc
 punkweb_bb/__pycache__/bbcode_tags.cpython-311.pyc
 punkweb_bb/__pycache__/context_processors.cpython-311.pyc
 punkweb_bb/__pycache__/forms.cpython-311.pyc
+punkweb_bb/__pycache__/guests.cpython-311.pyc
 punkweb_bb/__pycache__/middleware.cpython-311.pyc
 punkweb_bb/__pycache__/mixins.cpython-311.pyc
 punkweb_bb/__pycache__/models.cpython-311.pyc
 punkweb_bb/__pycache__/pagination.cpython-311.pyc
 punkweb_bb/__pycache__/parsers.cpython-311.pyc
 punkweb_bb/__pycache__/response.cpython-311.pyc
 punkweb_bb/__pycache__/settings.cpython-311.pyc
```

### Comparing `punkweb_bb-0.1.3/setup.py` & `punkweb_bb-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from setuptools import setup
 
 setup(
     name="punkweb_bb",
-    version="0.1.3",
+    version="0.1.4",
     author="Punkweb",
     author_email="punkwebnet@gmail.com",
     packages=["punkweb_bb"],
     url="https://github.com/Punkweb/PunkwebBB",
     license="BSD-3-Clause",
     description="Django application that provides a simple and modern forum board software for your Django website.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     zip_safe=False,
     include_package_data=True,
     package_data={"": ["README.md"]},
     install_requires=[
         "django>=4.0",
         "django-precise-bbcode",
+        "expiringdict",
         "pillow",
     ],
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Django",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
```

