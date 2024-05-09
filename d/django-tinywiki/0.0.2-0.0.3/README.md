# Comparing `tmp/django_tinywiki-0.0.2.tar.gz` & `tmp/django_tinywiki-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tinywiki-0.0.2.tar", last modified: Thu May  9 10:34:06 2024, max compression
+gzip compressed data, was "django_tinywiki-0.0.3.tar", last modified: Thu May  9 13:04:11 2024, max compression
```

## Comparing `django_tinywiki-0.0.2.tar` & `django_tinywiki-0.0.3.tar`

### file list

```diff
@@ -1,80 +1,96 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 10:34:06.668733 django_tinywiki-0.0.2/
--rw-rw-rw-   0        0        0     1374 2024-02-06 21:19:42.000000 django_tinywiki-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      581 2024-05-09 10:34:06.667733 django_tinywiki-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2577 2024-03-13 02:20:24.000000 django_tinywiki-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 10:34:06.607964 django_tinywiki-0.0.2/django_tinywiki/
--rw-rw-rw-   0        0        0        0 2024-01-13 05:59:06.000000 django_tinywiki-0.0.2/django_tinywiki/__init__.py
--rw-rw-rw-   0        0        0       63 2024-01-13 05:59:06.000000 django_tinywiki-0.0.2/django_tinywiki/admin.py
--rw-rw-rw-   0        0        0      161 2024-01-13 05:59:06.000000 django_tinywiki-0.0.2/django_tinywiki/apps.py
-drwxrwxrwx   0        0        0        0 2024-05-09 10:34:06.624964 django_tinywiki-0.0.2/django_tinywiki/builtin_wiki_pages/
--rw-rw-rw-   0        0        0  2860906 2020-06-17 08:08:41.000000 django_tinywiki-0.0.2/django_tinywiki/builtin_wiki_pages/Lama.jpg
--rw-rw-rw-   0        0        0     2550 2024-02-22 18:05:01.000000 django_tinywiki-0.0.2/django_tinywiki/builtin_wiki_pages/__init__.py
--rw-rw-rw-   0        0        0     4326 2024-03-07 16:06:11.000000 django_tinywiki-0.0.2/django_tinywiki/builtin_wiki_pages/de.index.md
--rw-rw-rw-   0        0        0    11420 2024-03-03 14:59:52.000000 django_tinywiki-0.0.2/django_tinywiki/builtin_wiki_pages/de.markdown.md
--rw-rw-rw-   0        0        0    19458 2024-03-16 13:37:33.000000 django_tinywiki-0.0.2/django_tinywiki/builtin_wiki_pages/de.settings.md
--rw-rw-rw-   0        0        0     3905 2024-03-07 16:04:21.000000 django_tinywiki-0.0.2/django_tinywiki/builtin_wiki_pages/en.index.md
--rw-rw-rw-   0        0        0     1405 2024-02-10 10:35:36.000000 django_tinywiki-0.0.2/django_tinywiki/builtin_wiki_pages/en.license.md
--rw-rw-rw-   0        0        0    10202 2024-03-03 15:24:46.000000 django_tinywiki-0.0.2/django_tinywiki/builtin_wiki_pages/en.markdown.md
--rw-rw-rw-   0        0        0    17950 2024-03-16 13:37:26.000000 django_tinywiki-0.0.2/django_tinywiki/builtin_wiki_pages/en.settings.md
--rw-rw-rw-   0        0        0  5811876 2020-11-13 18:25:14.000000 django_tinywiki-0.0.2/django_tinywiki/builtin_wiki_pages/vineyard-styria.jpg
--rw-rw-rw-   0        0        0      861 2024-02-12 20:31:35.000000 django_tinywiki-0.0.2/django_tinywiki/decorators.py
-drwxrwxrwx   0        0        0        0 2024-05-09 10:34:06.633478 django_tinywiki-0.0.2/django_tinywiki/forms/
--rw-rw-rw-   0        0        0       40 2024-01-27 07:31:59.000000 django_tinywiki-0.0.2/django_tinywiki/forms/__init__.py
--rw-rw-rw-   0        0        0      742 2024-03-03 12:02:38.000000 django_tinywiki-0.0.2/django_tinywiki/forms/auth.py
--rw-rw-rw-   0        0        0     2895 2024-02-14 14:23:31.000000 django_tinywiki-0.0.2/django_tinywiki/forms/wiki.py
-drwxrwxrwx   0        0        0        0 2024-05-09 10:34:06.639477 django_tinywiki-0.0.2/django_tinywiki/functions/
--rw-rw-rw-   0        0        0       38 2024-03-05 21:18:55.000000 django_tinywiki-0.0.2/django_tinywiki/functions/__init__.py
--rw-rw-rw-   0        0        0     2438 2024-03-03 15:43:02.000000 django_tinywiki-0.0.2/django_tinywiki/functions/auth.py
--rw-rw-rw-   0        0        0     3575 2024-02-14 16:45:41.000000 django_tinywiki-0.0.2/django_tinywiki/functions/init.py
--rw-rw-rw-   0        0        0     5313 2024-03-05 21:27:18.000000 django_tinywiki-0.0.2/django_tinywiki/functions/sidebar.py
--rw-rw-rw-   0        0        0      714 2024-02-22 23:32:53.000000 django_tinywiki-0.0.2/django_tinywiki/functions/utils.py
--rw-rw-rw-   0        0        0    10320 2024-03-03 14:37:42.000000 django_tinywiki-0.0.2/django_tinywiki/functions/wiki.py
-drwxrwxrwx   0        0        0        0 2024-05-09 10:34:06.640477 django_tinywiki-0.0.2/django_tinywiki/locale/
--rw-rw-rw-   0        0        0        0 2024-02-06 21:35:35.000000 django_tinywiki-0.0.2/django_tinywiki/locale/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 10:34:06.640477 django_tinywiki-0.0.2/django_tinywiki/locale/de/
-drwxrwxrwx   0        0        0        0 2024-05-09 10:34:06.642476 django_tinywiki-0.0.2/django_tinywiki/locale/de/LC_MESSAGES/
--rw-rw-rw-   0        0        0        0 2024-02-06 21:35:52.000000 django_tinywiki-0.0.2/django_tinywiki/locale/de/LC_MESSAGES/__init__.py
--rw-rw-rw-   0        0        0     5997 2024-03-03 13:47:35.000000 django_tinywiki-0.0.2/django_tinywiki/locale/de/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0        0 2024-02-06 21:35:44.000000 django_tinywiki-0.0.2/django_tinywiki/locale/de/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 10:34:06.649481 django_tinywiki-0.0.2/django_tinywiki/markdown_extensions/
--rw-rw-rw-   0        0        0      249 2024-02-03 20:58:29.000000 django_tinywiki-0.0.2/django_tinywiki/markdown_extensions/__init__.py
--rw-rw-rw-   0        0        0     1286 2024-02-03 21:17:33.000000 django_tinywiki-0.0.2/django_tinywiki/markdown_extensions/copyright.py
--rw-rw-rw-   0        0        0      307 2024-02-08 19:45:28.000000 django_tinywiki-0.0.2/django_tinywiki/markdown_extensions/delpattern.py
--rw-rw-rw-   0        0        0     1250 2024-01-19 21:10:19.000000 django_tinywiki-0.0.2/django_tinywiki/markdown_extensions/djangourl.py
--rw-rw-rw-   0        0        0     8035 2024-03-02 17:48:54.000000 django_tinywiki-0.0.2/django_tinywiki/markdown_extensions/tinywikiimage.py
--rw-rw-rw-   0        0        0     1553 2024-02-13 19:25:47.000000 django_tinywiki-0.0.2/django_tinywiki/markdown_extensions/tinywikilink.py
--rw-rw-rw-   0        0        0     2985 2024-03-02 12:42:52.000000 django_tinywiki-0.0.2/django_tinywiki/markdown_extensions/video.py
-drwxrwxrwx   0        0        0        0 2024-05-09 10:34:06.653481 django_tinywiki-0.0.2/django_tinywiki/migrations/
--rw-rw-rw-   0        0        0     8507 2024-02-15 21:55:36.000000 django_tinywiki-0.0.2/django_tinywiki/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     1641 2024-03-03 14:32:52.000000 django_tinywiki-0.0.2/django_tinywiki/migrations/0002_alter_wikiimage_image_alter_wikiimage_image_preview_and_more.py
--rw-rw-rw-   0        0        0        0 2024-01-13 05:59:06.000000 django_tinywiki-0.0.2/django_tinywiki/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 10:34:06.656480 django_tinywiki-0.0.2/django_tinywiki/models/
--rw-rw-rw-   0        0        0      123 2024-01-21 01:18:25.000000 django_tinywiki-0.0.2/django_tinywiki/models/__init__.py
--rw-rw-rw-   0        0        0      285 2024-01-13 05:59:06.000000 django_tinywiki-0.0.2/django_tinywiki/models/language.py
--rw-rw-rw-   0        0        0     6379 2024-02-11 13:50:40.000000 django_tinywiki-0.0.2/django_tinywiki/models/wiki.py
-drwxrwxrwx   0        0        0        0 2024-05-09 10:34:06.660729 django_tinywiki-0.0.2/django_tinywiki/scripts/
--rw-rw-rw-   0        0        0        0 2024-02-07 14:35:58.000000 django_tinywiki-0.0.2/django_tinywiki/scripts/__init__.py
--rw-rw-rw-   0        0        0     1208 2024-02-10 21:41:33.000000 django_tinywiki-0.0.2/django_tinywiki/scripts/initapp.py
--rw-rw-rw-   0        0        0      130 2024-02-22 23:23:50.000000 django_tinywiki-0.0.2/django_tinywiki/scripts/tinywiki_codehilite_styles.py
--rw-rw-rw-   0        0        0      135 2024-02-28 17:30:26.000000 django_tinywiki-0.0.2/django_tinywiki/scripts/tinywiki_languages.py
--rw-rw-rw-   0        0        0      108 2024-02-22 23:22:49.000000 django_tinywiki-0.0.2/django_tinywiki/scripts/tinywiki_styles.py
--rw-rw-rw-   0        0        0    11866 2024-03-06 21:41:08.000000 django_tinywiki-0.0.2/django_tinywiki/settings.py
--rw-rw-rw-   0        0        0       60 2024-01-13 05:59:06.000000 django_tinywiki-0.0.2/django_tinywiki/tests.py
--rw-rw-rw-   0        0        0     2002 2024-03-03 13:14:09.000000 django_tinywiki-0.0.2/django_tinywiki/urls.py
--rw-rw-rw-   0        0        0       24 2024-02-17 20:32:14.000000 django_tinywiki-0.0.2/django_tinywiki/version.py
-drwxrwxrwx   0        0        0        0 2024-05-09 10:34:06.665735 django_tinywiki-0.0.2/django_tinywiki/views/
--rw-rw-rw-   0        0        0      148 2024-02-01 12:06:22.000000 django_tinywiki-0.0.2/django_tinywiki/views/__init__.py
--rw-rw-rw-   0        0        0     6393 2024-03-03 14:03:01.000000 django_tinywiki-0.0.2/django_tinywiki/views/auth.py
--rw-rw-rw-   0        0        0     1874 2024-02-10 21:50:08.000000 django_tinywiki-0.0.2/django_tinywiki/views/manage.py
--rw-rw-rw-   0        0        0     5481 2024-03-06 21:43:39.000000 django_tinywiki-0.0.2/django_tinywiki/views/view.py
--rw-rw-rw-   0        0        0    16843 2024-03-03 15:40:58.000000 django_tinywiki-0.0.2/django_tinywiki/views/wiki.py
-drwxrwxrwx   0        0        0        0 2024-05-09 10:34:06.666736 django_tinywiki-0.0.2/django_tinywiki.egg-info/
--rw-rw-rw-   0        0        0      581 2024-05-09 10:34:06.000000 django_tinywiki-0.0.2/django_tinywiki.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2445 2024-05-09 10:34:06.000000 django_tinywiki-0.0.2/django_tinywiki.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 10:34:06.000000 django_tinywiki-0.0.2/django_tinywiki.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-09 10:34:06.000000 django_tinywiki-0.0.2/django_tinywiki.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       57 2024-05-09 10:34:06.000000 django_tinywiki-0.0.2/django_tinywiki.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-09 10:34:06.000000 django_tinywiki-0.0.2/django_tinywiki.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      230 2024-02-08 17:56:40.000000 django_tinywiki-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-09 10:34:06.668733 django_tinywiki-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1039 2024-05-09 10:32:27.000000 django_tinywiki-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 13:04:11.797765 django_tinywiki-0.0.3/
+-rw-rw-rw-   0        0        0     1374 2024-02-06 21:19:42.000000 django_tinywiki-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      581 2024-05-09 13:04:11.796260 django_tinywiki-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2577 2024-03-13 02:20:24.000000 django_tinywiki-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 13:04:11.697520 django_tinywiki-0.0.3/django_tinywiki/
+-rw-rw-rw-   0        0        0        0 2024-01-13 05:59:06.000000 django_tinywiki-0.0.3/django_tinywiki/__init__.py
+-rw-rw-rw-   0        0        0       63 2024-01-13 05:59:06.000000 django_tinywiki-0.0.3/django_tinywiki/admin.py
+-rw-rw-rw-   0        0        0      161 2024-01-13 05:59:06.000000 django_tinywiki-0.0.3/django_tinywiki/apps.py
+drwxrwxrwx   0        0        0        0 2024-05-09 13:04:11.709984 django_tinywiki-0.0.3/django_tinywiki/builtin_wiki_pages/
+-rw-rw-rw-   0        0        0     2550 2024-02-22 18:05:01.000000 django_tinywiki-0.0.3/django_tinywiki/builtin_wiki_pages/__init__.py
+-rw-rw-rw-   0        0        0      861 2024-02-12 20:31:35.000000 django_tinywiki-0.0.3/django_tinywiki/decorators.py
+drwxrwxrwx   0        0        0        0 2024-05-09 13:04:11.715749 django_tinywiki-0.0.3/django_tinywiki/forms/
+-rw-rw-rw-   0        0        0       40 2024-01-27 07:31:59.000000 django_tinywiki-0.0.3/django_tinywiki/forms/__init__.py
+-rw-rw-rw-   0        0        0      742 2024-03-03 12:02:38.000000 django_tinywiki-0.0.3/django_tinywiki/forms/auth.py
+-rw-rw-rw-   0        0        0     2895 2024-02-14 14:23:31.000000 django_tinywiki-0.0.3/django_tinywiki/forms/wiki.py
+drwxrwxrwx   0        0        0        0 2024-05-09 13:04:11.726197 django_tinywiki-0.0.3/django_tinywiki/functions/
+-rw-rw-rw-   0        0        0       38 2024-03-05 21:18:55.000000 django_tinywiki-0.0.3/django_tinywiki/functions/__init__.py
+-rw-rw-rw-   0        0        0     2438 2024-03-03 15:43:02.000000 django_tinywiki-0.0.3/django_tinywiki/functions/auth.py
+-rw-rw-rw-   0        0        0     3575 2024-02-14 16:45:41.000000 django_tinywiki-0.0.3/django_tinywiki/functions/init.py
+-rw-rw-rw-   0        0        0     5313 2024-03-05 21:27:18.000000 django_tinywiki-0.0.3/django_tinywiki/functions/sidebar.py
+-rw-rw-rw-   0        0        0      714 2024-02-22 23:32:53.000000 django_tinywiki-0.0.3/django_tinywiki/functions/utils.py
+-rw-rw-rw-   0        0        0    10320 2024-03-03 14:37:42.000000 django_tinywiki-0.0.3/django_tinywiki/functions/wiki.py
+drwxrwxrwx   0        0        0        0 2024-05-09 13:04:11.670957 django_tinywiki-0.0.3/django_tinywiki/locale/
+drwxrwxrwx   0        0        0        0 2024-05-09 13:04:11.670957 django_tinywiki-0.0.3/django_tinywiki/locale/de/
+drwxrwxrwx   0        0        0        0 2024-05-09 13:04:11.730209 django_tinywiki-0.0.3/django_tinywiki/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     5997 2024-03-03 13:47:35.000000 django_tinywiki-0.0.3/django_tinywiki/locale/de/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    10981 2024-03-03 13:47:13.000000 django_tinywiki-0.0.3/django_tinywiki/locale/de/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-05-09 13:04:11.741724 django_tinywiki-0.0.3/django_tinywiki/markdown_extensions/
+-rw-rw-rw-   0        0        0      249 2024-02-03 20:58:29.000000 django_tinywiki-0.0.3/django_tinywiki/markdown_extensions/__init__.py
+-rw-rw-rw-   0        0        0     1286 2024-02-03 21:17:33.000000 django_tinywiki-0.0.3/django_tinywiki/markdown_extensions/copyright.py
+-rw-rw-rw-   0        0        0      307 2024-02-08 19:45:28.000000 django_tinywiki-0.0.3/django_tinywiki/markdown_extensions/delpattern.py
+-rw-rw-rw-   0        0        0     1250 2024-01-19 21:10:19.000000 django_tinywiki-0.0.3/django_tinywiki/markdown_extensions/djangourl.py
+-rw-rw-rw-   0        0        0     8035 2024-03-02 17:48:54.000000 django_tinywiki-0.0.3/django_tinywiki/markdown_extensions/tinywikiimage.py
+-rw-rw-rw-   0        0        0     1553 2024-02-13 19:25:47.000000 django_tinywiki-0.0.3/django_tinywiki/markdown_extensions/tinywikilink.py
+-rw-rw-rw-   0        0        0     2985 2024-03-02 12:42:52.000000 django_tinywiki-0.0.3/django_tinywiki/markdown_extensions/video.py
+drwxrwxrwx   0        0        0        0 2024-05-09 13:04:11.746251 django_tinywiki-0.0.3/django_tinywiki/migrations/
+-rw-rw-rw-   0        0        0     8507 2024-02-15 21:55:36.000000 django_tinywiki-0.0.3/django_tinywiki/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     1641 2024-03-03 14:32:52.000000 django_tinywiki-0.0.3/django_tinywiki/migrations/0002_alter_wikiimage_image_alter_wikiimage_image_preview_and_more.py
+-rw-rw-rw-   0        0        0        0 2024-01-13 05:59:06.000000 django_tinywiki-0.0.3/django_tinywiki/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 13:04:11.752263 django_tinywiki-0.0.3/django_tinywiki/models/
+-rw-rw-rw-   0        0        0      123 2024-01-21 01:18:25.000000 django_tinywiki-0.0.3/django_tinywiki/models/__init__.py
+-rw-rw-rw-   0        0        0      285 2024-01-13 05:59:06.000000 django_tinywiki-0.0.3/django_tinywiki/models/language.py
+-rw-rw-rw-   0        0        0     6379 2024-02-11 13:50:40.000000 django_tinywiki-0.0.3/django_tinywiki/models/wiki.py
+drwxrwxrwx   0        0        0        0 2024-05-09 13:04:11.760284 django_tinywiki-0.0.3/django_tinywiki/scripts/
+-rw-rw-rw-   0        0        0        0 2024-02-07 14:35:58.000000 django_tinywiki-0.0.3/django_tinywiki/scripts/__init__.py
+-rw-rw-rw-   0        0        0     1208 2024-02-10 21:41:33.000000 django_tinywiki-0.0.3/django_tinywiki/scripts/initapp.py
+-rw-rw-rw-   0        0        0      130 2024-02-22 23:23:50.000000 django_tinywiki-0.0.3/django_tinywiki/scripts/tinywiki_codehilite_styles.py
+-rw-rw-rw-   0        0        0      135 2024-02-28 17:30:26.000000 django_tinywiki-0.0.3/django_tinywiki/scripts/tinywiki_languages.py
+-rw-rw-rw-   0        0        0      108 2024-02-22 23:22:49.000000 django_tinywiki-0.0.3/django_tinywiki/scripts/tinywiki_styles.py
+-rw-rw-rw-   0        0        0    11866 2024-03-06 21:41:08.000000 django_tinywiki-0.0.3/django_tinywiki/settings.py
+drwxrwxrwx   0        0        0        0 2024-05-09 13:04:11.674463 django_tinywiki-0.0.3/django_tinywiki/static/
+drwxrwxrwx   0        0        0        0 2024-05-09 13:04:11.675469 django_tinywiki-0.0.3/django_tinywiki/static/django_tinywiki/
+drwxrwxrwx   0        0        0        0 2024-05-09 13:04:11.761291 django_tinywiki-0.0.3/django_tinywiki/static/django_tinywiki/images/
+-rw-rw-rw-   0        0        0  7993048 2020-11-13 18:24:45.000000 django_tinywiki-0.0.3/django_tinywiki/static/django_tinywiki/images/peacock.jpg
+drwxrwxrwx   0        0        0        0 2024-05-09 13:04:11.771380 django_tinywiki-0.0.3/django_tinywiki/static/django_tinywiki/styles/
+-rw-rw-rw-   0        0        0     5724 2024-03-03 13:18:39.000000 django_tinywiki-0.0.3/django_tinywiki/static/django_tinywiki/styles/default.css
+drwxrwxrwx   0        0        0        0 2024-05-09 13:04:11.675997 django_tinywiki-0.0.3/django_tinywiki/templates/
+drwxrwxrwx   0        0        0        0 2024-05-09 13:04:11.678010 django_tinywiki-0.0.3/django_tinywiki/templates/django_tinywiki/
+drwxrwxrwx   0        0        0        0 2024-05-09 13:04:11.778209 django_tinywiki-0.0.3/django_tinywiki/templates/django_tinywiki/auth/
+-rw-rw-rw-   0        0        0      472 2024-02-14 18:55:52.000000 django_tinywiki-0.0.3/django_tinywiki/templates/django_tinywiki/auth/login.html
+-rw-rw-rw-   0        0        0      313 2024-02-03 21:07:28.000000 django_tinywiki-0.0.3/django_tinywiki/templates/django_tinywiki/auth/logout.html
+-rw-rw-rw-   0        0        0        0 2024-01-13 05:59:06.000000 django_tinywiki-0.0.3/django_tinywiki/templates/django_tinywiki/auth/profile.html
+-rw-rw-rw-   0        0        0      350 2024-03-03 13:20:37.000000 django_tinywiki-0.0.3/django_tinywiki/templates/django_tinywiki/auth/signup-success.html
+-rw-rw-rw-   0        0        0      733 2024-03-03 12:03:58.000000 django_tinywiki-0.0.3/django_tinywiki/templates/django_tinywiki/auth/signup.html
+drwxrwxrwx   0        0        0        0 2024-05-09 13:04:11.782215 django_tinywiki-0.0.3/django_tinywiki/templates/django_tinywiki/manage/
+-rw-rw-rw-   0        0        0      432 2024-02-03 21:07:06.000000 django_tinywiki-0.0.3/django_tinywiki/templates/django_tinywiki/manage/initialize.html
+-rw-rw-rw-   0        0        0        0 2024-01-15 04:39:56.000000 django_tinywiki-0.0.3/django_tinywiki/templates/django_tinywiki/manage/manage.html
+-rw-rw-rw-   0        0        0        0 2024-01-13 05:59:06.000000 django_tinywiki-0.0.3/django_tinywiki/templates/django_tinywiki/manage/userlist.html
+-rw-rw-rw-   0        0        0        0 2024-01-13 05:59:06.000000 django_tinywiki-0.0.3/django_tinywiki/templates/django_tinywiki/manage/usermanage.html
+drwxrwxrwx   0        0        0        0 2024-05-09 13:04:11.789241 django_tinywiki-0.0.3/django_tinywiki/templates/django_tinywiki/wiki/
+-rw-rw-rw-   0        0        0     1083 2024-02-14 18:56:11.000000 django_tinywiki-0.0.3/django_tinywiki/templates/django_tinywiki/wiki/create.html
+-rw-rw-rw-   0        0        0      596 2024-02-16 21:07:21.000000 django_tinywiki-0.0.3/django_tinywiki/templates/django_tinywiki/wiki/delete-done.html
+-rw-rw-rw-   0        0        0      689 2024-02-17 09:45:48.000000 django_tinywiki-0.0.3/django_tinywiki/templates/django_tinywiki/wiki/delete.html
+-rw-rw-rw-   0        0        0     1147 2024-02-03 11:31:14.000000 django_tinywiki-0.0.3/django_tinywiki/templates/django_tinywiki/wiki/edit.html
+-rw-rw-rw-   0        0        0      589 2024-02-03 18:49:37.000000 django_tinywiki-0.0.3/django_tinywiki/templates/django_tinywiki/wiki/image-upload.html
+-rw-rw-rw-   0        0        0      761 2024-02-14 15:56:38.000000 django_tinywiki-0.0.3/django_tinywiki/templates/django_tinywiki/wiki/overview.html
+-rw-rw-rw-   0        0        0     1418 2024-02-09 17:41:22.000000 django_tinywiki-0.0.3/django_tinywiki/templates/django_tinywiki/wiki/page.html
+-rw-rw-rw-   0        0        0       60 2024-01-13 05:59:06.000000 django_tinywiki-0.0.3/django_tinywiki/tests.py
+-rw-rw-rw-   0        0        0     2002 2024-03-03 13:14:09.000000 django_tinywiki-0.0.3/django_tinywiki/urls.py
+-rw-rw-rw-   0        0        0       25 2024-05-09 10:36:18.000000 django_tinywiki-0.0.3/django_tinywiki/version.py
+drwxrwxrwx   0        0        0        0 2024-05-09 13:04:11.794752 django_tinywiki-0.0.3/django_tinywiki/views/
+-rw-rw-rw-   0        0        0      148 2024-02-01 12:06:22.000000 django_tinywiki-0.0.3/django_tinywiki/views/__init__.py
+-rw-rw-rw-   0        0        0     6393 2024-03-03 14:03:01.000000 django_tinywiki-0.0.3/django_tinywiki/views/auth.py
+-rw-rw-rw-   0        0        0     1874 2024-02-10 21:50:08.000000 django_tinywiki-0.0.3/django_tinywiki/views/manage.py
+-rw-rw-rw-   0        0        0     5481 2024-03-06 21:43:39.000000 django_tinywiki-0.0.3/django_tinywiki/views/view.py
+-rw-rw-rw-   0        0        0    16843 2024-03-03 15:40:58.000000 django_tinywiki-0.0.3/django_tinywiki/views/wiki.py
+drwxrwxrwx   0        0        0        0 2024-05-09 13:04:11.795753 django_tinywiki-0.0.3/django_tinywiki.egg-info/
+-rw-rw-rw-   0        0        0      581 2024-05-09 13:04:11.000000 django_tinywiki-0.0.3/django_tinywiki.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3023 2024-05-09 13:04:11.000000 django_tinywiki-0.0.3/django_tinywiki.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 13:04:11.000000 django_tinywiki-0.0.3/django_tinywiki.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-09 13:04:11.000000 django_tinywiki-0.0.3/django_tinywiki.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       57 2024-05-09 13:04:11.000000 django_tinywiki-0.0.3/django_tinywiki.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-09 13:04:11.000000 django_tinywiki-0.0.3/django_tinywiki.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      230 2024-02-08 17:56:40.000000 django_tinywiki-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-09 13:04:11.797765 django_tinywiki-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1566 2024-05-09 13:03:36.000000 django_tinywiki-0.0.3/setup.py
```

### Comparing `django_tinywiki-0.0.2/LICENSE` & `django_tinywiki-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_tinywiki-0.0.2/PKG-INFO` & `django_tinywiki-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tinywiki
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple wiki app for the django framework
 Home-page: https://github.com/c9moser/django-tinywiki
 Author: Christian Moser
 Author-email: christian@cmoser.eu
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/c9moser/django-tinywiki
 Project-URL: Issues, https://www.github.com/c9moser/django-tinywiki/issues
```

### Comparing `django_tinywiki-0.0.2/README.md` & `django_tinywiki-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `django_tinywiki-0.0.2/django_tinywiki/builtin_wiki_pages/__init__.py` & `django_tinywiki-0.0.3/django_tinywiki/builtin_wiki_pages/__init__.py`

 * *Files identical despite different names*

### Comparing `django_tinywiki-0.0.2/django_tinywiki/decorators.py` & `django_tinywiki-0.0.3/django_tinywiki/decorators.py`

 * *Files identical despite different names*

### Comparing `django_tinywiki-0.0.2/django_tinywiki/forms/auth.py` & `django_tinywiki-0.0.3/django_tinywiki/forms/auth.py`

 * *Files identical despite different names*

### Comparing `django_tinywiki-0.0.2/django_tinywiki/forms/wiki.py` & `django_tinywiki-0.0.3/django_tinywiki/forms/wiki.py`

 * *Files identical despite different names*

### Comparing `django_tinywiki-0.0.2/django_tinywiki/functions/auth.py` & `django_tinywiki-0.0.3/django_tinywiki/functions/auth.py`

 * *Files identical despite different names*

### Comparing `django_tinywiki-0.0.2/django_tinywiki/functions/init.py` & `django_tinywiki-0.0.3/django_tinywiki/functions/init.py`

 * *Files identical despite different names*

### Comparing `django_tinywiki-0.0.2/django_tinywiki/functions/sidebar.py` & `django_tinywiki-0.0.3/django_tinywiki/functions/sidebar.py`

 * *Files identical despite different names*

### Comparing `django_tinywiki-0.0.2/django_tinywiki/functions/utils.py` & `django_tinywiki-0.0.3/django_tinywiki/functions/utils.py`

 * *Files identical despite different names*

### Comparing `django_tinywiki-0.0.2/django_tinywiki/functions/wiki.py` & `django_tinywiki-0.0.3/django_tinywiki/functions/wiki.py`

 * *Files identical despite different names*

### Comparing `django_tinywiki-0.0.2/django_tinywiki/locale/de/LC_MESSAGES/django.mo` & `django_tinywiki-0.0.3/django_tinywiki/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_tinywiki-0.0.2/django_tinywiki/markdown_extensions/copyright.py` & `django_tinywiki-0.0.3/django_tinywiki/markdown_extensions/copyright.py`

 * *Files identical despite different names*

### Comparing `django_tinywiki-0.0.2/django_tinywiki/markdown_extensions/djangourl.py` & `django_tinywiki-0.0.3/django_tinywiki/markdown_extensions/djangourl.py`

 * *Files identical despite different names*

### Comparing `django_tinywiki-0.0.2/django_tinywiki/markdown_extensions/tinywikiimage.py` & `django_tinywiki-0.0.3/django_tinywiki/markdown_extensions/tinywikiimage.py`

 * *Files identical despite different names*

### Comparing `django_tinywiki-0.0.2/django_tinywiki/markdown_extensions/tinywikilink.py` & `django_tinywiki-0.0.3/django_tinywiki/markdown_extensions/tinywikilink.py`

 * *Files identical despite different names*

### Comparing `django_tinywiki-0.0.2/django_tinywiki/markdown_extensions/video.py` & `django_tinywiki-0.0.3/django_tinywiki/markdown_extensions/video.py`

 * *Files identical despite different names*

### Comparing `django_tinywiki-0.0.2/django_tinywiki/migrations/0001_initial.py` & `django_tinywiki-0.0.3/django_tinywiki/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_tinywiki-0.0.2/django_tinywiki/migrations/0002_alter_wikiimage_image_alter_wikiimage_image_preview_and_more.py` & `django_tinywiki-0.0.3/django_tinywiki/migrations/0002_alter_wikiimage_image_alter_wikiimage_image_preview_and_more.py`

 * *Files identical despite different names*

### Comparing `django_tinywiki-0.0.2/django_tinywiki/models/wiki.py` & `django_tinywiki-0.0.3/django_tinywiki/models/wiki.py`

 * *Files identical despite different names*

### Comparing `django_tinywiki-0.0.2/django_tinywiki/scripts/initapp.py` & `django_tinywiki-0.0.3/django_tinywiki/scripts/initapp.py`

 * *Files identical despite different names*

### Comparing `django_tinywiki-0.0.2/django_tinywiki/settings.py` & `django_tinywiki-0.0.3/django_tinywiki/settings.py`

 * *Files identical despite different names*

### Comparing `django_tinywiki-0.0.2/django_tinywiki/urls.py` & `django_tinywiki-0.0.3/django_tinywiki/urls.py`

 * *Files identical despite different names*

### Comparing `django_tinywiki-0.0.2/django_tinywiki/views/auth.py` & `django_tinywiki-0.0.3/django_tinywiki/views/auth.py`

 * *Files identical despite different names*

### Comparing `django_tinywiki-0.0.2/django_tinywiki/views/manage.py` & `django_tinywiki-0.0.3/django_tinywiki/views/manage.py`

 * *Files identical despite different names*

### Comparing `django_tinywiki-0.0.2/django_tinywiki/views/view.py` & `django_tinywiki-0.0.3/django_tinywiki/views/view.py`

 * *Files identical despite different names*

### Comparing `django_tinywiki-0.0.2/django_tinywiki/views/wiki.py` & `django_tinywiki-0.0.3/django_tinywiki/views/wiki.py`

 * *Files identical despite different names*

### Comparing `django_tinywiki-0.0.2/django_tinywiki.egg-info/PKG-INFO` & `django_tinywiki-0.0.3/django_tinywiki.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tinywiki
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple wiki app for the django framework
 Home-page: https://github.com/c9moser/django-tinywiki
 Author: Christian Moser
 Author-email: christian@cmoser.eu
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/c9moser/django-tinywiki
 Project-URL: Issues, https://www.github.com/c9moser/django-tinywiki/issues
```

### Comparing `django_tinywiki-0.0.2/django_tinywiki.egg-info/SOURCES.txt` & `django_tinywiki-0.0.3/django_tinywiki.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -12,37 +12,26 @@
 django_tinywiki/version.py
 django_tinywiki.egg-info/PKG-INFO
 django_tinywiki.egg-info/SOURCES.txt
 django_tinywiki.egg-info/dependency_links.txt
 django_tinywiki.egg-info/not-zip-safe
 django_tinywiki.egg-info/requires.txt
 django_tinywiki.egg-info/top_level.txt
-django_tinywiki/builtin_wiki_pages/Lama.jpg
 django_tinywiki/builtin_wiki_pages/__init__.py
-django_tinywiki/builtin_wiki_pages/de.index.md
-django_tinywiki/builtin_wiki_pages/de.markdown.md
-django_tinywiki/builtin_wiki_pages/de.settings.md
-django_tinywiki/builtin_wiki_pages/en.index.md
-django_tinywiki/builtin_wiki_pages/en.license.md
-django_tinywiki/builtin_wiki_pages/en.markdown.md
-django_tinywiki/builtin_wiki_pages/en.settings.md
-django_tinywiki/builtin_wiki_pages/vineyard-styria.jpg
 django_tinywiki/forms/__init__.py
 django_tinywiki/forms/auth.py
 django_tinywiki/forms/wiki.py
 django_tinywiki/functions/__init__.py
 django_tinywiki/functions/auth.py
 django_tinywiki/functions/init.py
 django_tinywiki/functions/sidebar.py
 django_tinywiki/functions/utils.py
 django_tinywiki/functions/wiki.py
-django_tinywiki/locale/__init__.py
-django_tinywiki/locale/de/__init__.py
-django_tinywiki/locale/de/LC_MESSAGES/__init__.py
 django_tinywiki/locale/de/LC_MESSAGES/django.mo
+django_tinywiki/locale/de/LC_MESSAGES/django.po
 django_tinywiki/markdown_extensions/__init__.py
 django_tinywiki/markdown_extensions/copyright.py
 django_tinywiki/markdown_extensions/delpattern.py
 django_tinywiki/markdown_extensions/djangourl.py
 django_tinywiki/markdown_extensions/tinywikiimage.py
 django_tinywiki/markdown_extensions/tinywikilink.py
 django_tinywiki/markdown_extensions/video.py
@@ -53,12 +42,30 @@
 django_tinywiki/models/language.py
 django_tinywiki/models/wiki.py
 django_tinywiki/scripts/__init__.py
 django_tinywiki/scripts/initapp.py
 django_tinywiki/scripts/tinywiki_codehilite_styles.py
 django_tinywiki/scripts/tinywiki_languages.py
 django_tinywiki/scripts/tinywiki_styles.py
+django_tinywiki/static/django_tinywiki/images/peacock.jpg
+django_tinywiki/static/django_tinywiki/styles/default.css
+django_tinywiki/templates/django_tinywiki/auth/login.html
+django_tinywiki/templates/django_tinywiki/auth/logout.html
+django_tinywiki/templates/django_tinywiki/auth/profile.html
+django_tinywiki/templates/django_tinywiki/auth/signup-success.html
+django_tinywiki/templates/django_tinywiki/auth/signup.html
+django_tinywiki/templates/django_tinywiki/manage/initialize.html
+django_tinywiki/templates/django_tinywiki/manage/manage.html
+django_tinywiki/templates/django_tinywiki/manage/userlist.html
+django_tinywiki/templates/django_tinywiki/manage/usermanage.html
+django_tinywiki/templates/django_tinywiki/wiki/create.html
+django_tinywiki/templates/django_tinywiki/wiki/delete-done.html
+django_tinywiki/templates/django_tinywiki/wiki/delete.html
+django_tinywiki/templates/django_tinywiki/wiki/edit.html
+django_tinywiki/templates/django_tinywiki/wiki/image-upload.html
+django_tinywiki/templates/django_tinywiki/wiki/overview.html
+django_tinywiki/templates/django_tinywiki/wiki/page.html
 django_tinywiki/views/__init__.py
 django_tinywiki/views/auth.py
 django_tinywiki/views/manage.py
 django_tinywiki/views/view.py
 django_tinywiki/views/wiki.py
```

