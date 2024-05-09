# Comparing `tmp/django-tinywiki-0.0.1.tar.gz` & `tmp/django_tinywiki-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-tinywiki-0.0.1.tar", last modified: Fri Feb  9 19:18:13 2024, max compression
+gzip compressed data, was "django_tinywiki-0.0.2.tar", last modified: Thu May  9 10:34:06 2024, max compression
```

## Comparing `django-tinywiki-0.0.1.tar` & `django_tinywiki-0.0.2.tar`

### file list

```diff
@@ -1,72 +1,80 @@
-drwxrwxrwx   0        0        0        0 2024-02-09 19:18:13.230631 django-tinywiki-0.0.1/
--rw-rw-rw-   0        0        0     1374 2024-02-06 21:19:42.000000 django-tinywiki-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      556 2024-02-09 19:18:13.229632 django-tinywiki-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-02-06 21:09:45.000000 django-tinywiki-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-02-09 19:18:13.184578 django-tinywiki-0.0.1/django_tinywiki/
--rw-rw-rw-   0        0        0        0 2024-01-13 05:59:06.000000 django-tinywiki-0.0.1/django_tinywiki/__init__.py
--rw-rw-rw-   0        0        0       63 2024-01-13 05:59:06.000000 django-tinywiki-0.0.1/django_tinywiki/admin.py
--rw-rw-rw-   0        0        0      161 2024-01-13 05:59:06.000000 django-tinywiki-0.0.1/django_tinywiki/apps.py
-drwxrwxrwx   0        0        0        0 2024-02-09 19:18:13.199092 django-tinywiki-0.0.1/django_tinywiki/builtin_wiki_pages/
--rw-rw-rw-   0        0        0  2860906 2020-06-17 08:08:41.000000 django-tinywiki-0.0.1/django_tinywiki/builtin_wiki_pages/Lama.jpg
--rw-rw-rw-   0        0        0     1274 2024-02-01 16:49:59.000000 django-tinywiki-0.0.1/django_tinywiki/builtin_wiki_pages/__init__.py
--rw-rw-rw-   0        0        0     3876 2024-02-09 18:23:30.000000 django-tinywiki-0.0.1/django_tinywiki/builtin_wiki_pages/de.index.md
--rw-rw-rw-   0        0        0     9317 2024-02-04 09:55:06.000000 django-tinywiki-0.0.1/django_tinywiki/builtin_wiki_pages/de.markdown.md
--rw-rw-rw-   0        0        0     3445 2024-02-09 18:22:53.000000 django-tinywiki-0.0.1/django_tinywiki/builtin_wiki_pages/en.index.md
--rw-rw-rw-   0        0        0     7662 2024-02-02 16:12:12.000000 django-tinywiki-0.0.1/django_tinywiki/builtin_wiki_pages/en.markdown.md
--rw-rw-rw-   0        0        0      490 2024-02-03 11:57:37.000000 django-tinywiki-0.0.1/django_tinywiki/decorators.py
-drwxrwxrwx   0        0        0        0 2024-02-09 19:18:13.202091 django-tinywiki-0.0.1/django_tinywiki/forms/
--rw-rw-rw-   0        0        0       40 2024-01-27 07:31:59.000000 django-tinywiki-0.0.1/django_tinywiki/forms/__init__.py
--rw-rw-rw-   0        0        0      570 2024-01-13 06:22:46.000000 django-tinywiki-0.0.1/django_tinywiki/forms/auth.py
--rw-rw-rw-   0        0        0     2663 2024-02-02 22:59:48.000000 django-tinywiki-0.0.1/django_tinywiki/forms/wiki.py
--rw-rw-rw-   0        0        0    11500 2024-02-09 10:42:29.000000 django-tinywiki-0.0.1/django_tinywiki/functions.py
-drwxrwxrwx   0        0        0        0 2024-02-09 19:18:13.202091 django-tinywiki-0.0.1/django_tinywiki/locale/
--rw-rw-rw-   0        0        0        0 2024-02-06 21:35:35.000000 django-tinywiki-0.0.1/django_tinywiki/locale/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-09 19:18:13.203597 django-tinywiki-0.0.1/django_tinywiki/locale/de/
-drwxrwxrwx   0        0        0        0 2024-02-09 19:18:13.205603 django-tinywiki-0.0.1/django_tinywiki/locale/de/LC_MESSAGES/
--rw-rw-rw-   0        0        0        0 2024-02-06 21:35:52.000000 django-tinywiki-0.0.1/django_tinywiki/locale/de/LC_MESSAGES/__init__.py
--rw-rw-rw-   0        0        0     3751 2024-02-06 04:48:09.000000 django-tinywiki-0.0.1/django_tinywiki/locale/de/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0        0 2024-02-06 21:35:44.000000 django-tinywiki-0.0.1/django_tinywiki/locale/de/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-09 19:18:13.210603 django-tinywiki-0.0.1/django_tinywiki/markdown_extensions/
--rw-rw-rw-   0        0        0      249 2024-02-03 20:58:29.000000 django-tinywiki-0.0.1/django_tinywiki/markdown_extensions/__init__.py
--rw-rw-rw-   0        0        0     1286 2024-02-03 21:17:33.000000 django-tinywiki-0.0.1/django_tinywiki/markdown_extensions/copyright.py
--rw-rw-rw-   0        0        0      307 2024-02-08 19:45:28.000000 django-tinywiki-0.0.1/django_tinywiki/markdown_extensions/delpattern.py
--rw-rw-rw-   0        0        0     1250 2024-01-19 21:10:19.000000 django-tinywiki-0.0.1/django_tinywiki/markdown_extensions/djangourl.py
--rw-rw-rw-   0        0        0     8657 2024-02-03 22:00:12.000000 django-tinywiki-0.0.1/django_tinywiki/markdown_extensions/tinywikiimage.py
--rw-rw-rw-   0        0        0     1535 2024-02-08 19:45:37.000000 django-tinywiki-0.0.1/django_tinywiki/markdown_extensions/tinywikilink.py
-drwxrwxrwx   0        0        0        0 2024-02-09 19:18:13.219117 django-tinywiki-0.0.1/django_tinywiki/migrations/
--rw-rw-rw-   0        0        0     3360 2024-01-13 05:59:06.000000 django-tinywiki-0.0.1/django_tinywiki/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     1437 2024-01-21 01:02:37.000000 django-tinywiki-0.0.1/django_tinywiki/migrations/0002_wikiimage.py
--rw-rw-rw-   0        0        0      441 2024-01-24 20:19:30.000000 django-tinywiki-0.0.1/django_tinywiki/migrations/0003_wikiimage_image_sidebar.py
--rw-rw-rw-   0        0        0      623 2024-01-28 10:07:24.000000 django-tinywiki-0.0.1/django_tinywiki/migrations/0004_wikipage_user.py
--rw-rw-rw-   0        0        0      927 2024-01-28 12:30:17.000000 django-tinywiki-0.0.1/django_tinywiki/migrations/0005_wikipagebackup_user_alter_wikipage_user.py
--rw-rw-rw-   0        0        0      437 2024-01-31 04:38:50.000000 django-tinywiki-0.0.1/django_tinywiki/migrations/0006_wikiimage_builtin_id.py
--rw-rw-rw-   0        0        0     1765 2024-01-31 15:09:48.000000 django-tinywiki-0.0.1/django_tinywiki/migrations/0007_alter_wikiimage_builtin_id_alter_wikiimage_image_and_more.py
--rw-rw-rw-   0        0        0     1667 2024-01-31 21:47:51.000000 django-tinywiki-0.0.1/django_tinywiki/migrations/0008_alter_wikiimage_image_alter_wikiimage_image_preview_and_more.py
--rw-rw-rw-   0        0        0     5463 2024-02-09 10:28:03.000000 django-tinywiki-0.0.1/django_tinywiki/migrations/0009_alter_wikiimage_alt_alter_wikiimage_image_and_more.py
--rw-rw-rw-   0        0        0        0 2024-01-13 05:59:06.000000 django-tinywiki-0.0.1/django_tinywiki/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-09 19:18:13.222117 django-tinywiki-0.0.1/django_tinywiki/models/
--rw-rw-rw-   0        0        0      123 2024-01-21 01:18:25.000000 django-tinywiki-0.0.1/django_tinywiki/models/__init__.py
--rw-rw-rw-   0        0        0      285 2024-01-13 05:59:06.000000 django-tinywiki-0.0.1/django_tinywiki/models/language.py
--rw-rw-rw-   0        0        0     5953 2024-02-09 17:30:39.000000 django-tinywiki-0.0.1/django_tinywiki/models/wiki.py
-drwxrwxrwx   0        0        0        0 2024-02-09 19:18:13.223632 django-tinywiki-0.0.1/django_tinywiki/scripts/
--rw-rw-rw-   0        0        0        0 2024-02-07 14:35:58.000000 django-tinywiki-0.0.1/django_tinywiki/scripts/__init__.py
--rw-rw-rw-   0        0        0     1268 2024-02-09 11:43:46.000000 django-tinywiki-0.0.1/django_tinywiki/scripts/initapp.py
--rw-rw-rw-   0        0        0     7432 2024-02-09 18:20:38.000000 django-tinywiki-0.0.1/django_tinywiki/settings.py
--rw-rw-rw-   0        0        0       60 2024-01-13 05:59:06.000000 django-tinywiki-0.0.1/django_tinywiki/tests.py
--rw-rw-rw-   0        0        0     1709 2024-02-09 18:18:55.000000 django-tinywiki-0.0.1/django_tinywiki/urls.py
-drwxrwxrwx   0        0        0        0 2024-02-09 19:18:13.227631 django-tinywiki-0.0.1/django_tinywiki/views/
--rw-rw-rw-   0        0        0      148 2024-02-01 12:06:22.000000 django-tinywiki-0.0.1/django_tinywiki/views/__init__.py
--rw-rw-rw-   0        0        0     4975 2024-02-09 18:17:11.000000 django-tinywiki-0.0.1/django_tinywiki/views/auth.py
--rw-rw-rw-   0        0        0     1869 2024-02-03 21:06:58.000000 django-tinywiki-0.0.1/django_tinywiki/views/manage.py
--rw-rw-rw-   0        0        0     3471 2024-02-03 09:03:59.000000 django-tinywiki-0.0.1/django_tinywiki/views/view.py
--rw-rw-rw-   0        0        0    13098 2024-02-03 11:42:14.000000 django-tinywiki-0.0.1/django_tinywiki/views/wiki.py
-drwxrwxrwx   0        0        0        0 2024-02-09 19:18:13.228631 django-tinywiki-0.0.1/django_tinywiki.egg-info/
--rw-rw-rw-   0        0        0      556 2024-02-09 19:18:13.000000 django-tinywiki-0.0.1/django_tinywiki.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2306 2024-02-09 19:18:13.000000 django-tinywiki-0.0.1/django_tinywiki.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-09 19:18:13.000000 django-tinywiki-0.0.1/django_tinywiki.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-02-08 18:30:03.000000 django-tinywiki-0.0.1/django_tinywiki.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       48 2024-02-09 19:18:13.000000 django-tinywiki-0.0.1/django_tinywiki.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-02-09 19:18:13.000000 django-tinywiki-0.0.1/django_tinywiki.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      230 2024-02-08 17:56:40.000000 django-tinywiki-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-09 19:18:13.230631 django-tinywiki-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1016 2024-02-08 18:29:55.000000 django-tinywiki-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 10:34:06.668733 django_tinywiki-0.0.2/
+-rw-rw-rw-   0        0        0     1374 2024-02-06 21:19:42.000000 django_tinywiki-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      581 2024-05-09 10:34:06.667733 django_tinywiki-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2577 2024-03-13 02:20:24.000000 django_tinywiki-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 10:34:06.607964 django_tinywiki-0.0.2/django_tinywiki/
+-rw-rw-rw-   0        0        0        0 2024-01-13 05:59:06.000000 django_tinywiki-0.0.2/django_tinywiki/__init__.py
+-rw-rw-rw-   0        0        0       63 2024-01-13 05:59:06.000000 django_tinywiki-0.0.2/django_tinywiki/admin.py
+-rw-rw-rw-   0        0        0      161 2024-01-13 05:59:06.000000 django_tinywiki-0.0.2/django_tinywiki/apps.py
+drwxrwxrwx   0        0        0        0 2024-05-09 10:34:06.624964 django_tinywiki-0.0.2/django_tinywiki/builtin_wiki_pages/
+-rw-rw-rw-   0        0        0  2860906 2020-06-17 08:08:41.000000 django_tinywiki-0.0.2/django_tinywiki/builtin_wiki_pages/Lama.jpg
+-rw-rw-rw-   0        0        0     2550 2024-02-22 18:05:01.000000 django_tinywiki-0.0.2/django_tinywiki/builtin_wiki_pages/__init__.py
+-rw-rw-rw-   0        0        0     4326 2024-03-07 16:06:11.000000 django_tinywiki-0.0.2/django_tinywiki/builtin_wiki_pages/de.index.md
+-rw-rw-rw-   0        0        0    11420 2024-03-03 14:59:52.000000 django_tinywiki-0.0.2/django_tinywiki/builtin_wiki_pages/de.markdown.md
+-rw-rw-rw-   0        0        0    19458 2024-03-16 13:37:33.000000 django_tinywiki-0.0.2/django_tinywiki/builtin_wiki_pages/de.settings.md
+-rw-rw-rw-   0        0        0     3905 2024-03-07 16:04:21.000000 django_tinywiki-0.0.2/django_tinywiki/builtin_wiki_pages/en.index.md
+-rw-rw-rw-   0        0        0     1405 2024-02-10 10:35:36.000000 django_tinywiki-0.0.2/django_tinywiki/builtin_wiki_pages/en.license.md
+-rw-rw-rw-   0        0        0    10202 2024-03-03 15:24:46.000000 django_tinywiki-0.0.2/django_tinywiki/builtin_wiki_pages/en.markdown.md
+-rw-rw-rw-   0        0        0    17950 2024-03-16 13:37:26.000000 django_tinywiki-0.0.2/django_tinywiki/builtin_wiki_pages/en.settings.md
+-rw-rw-rw-   0        0        0  5811876 2020-11-13 18:25:14.000000 django_tinywiki-0.0.2/django_tinywiki/builtin_wiki_pages/vineyard-styria.jpg
+-rw-rw-rw-   0        0        0      861 2024-02-12 20:31:35.000000 django_tinywiki-0.0.2/django_tinywiki/decorators.py
+drwxrwxrwx   0        0        0        0 2024-05-09 10:34:06.633478 django_tinywiki-0.0.2/django_tinywiki/forms/
+-rw-rw-rw-   0        0        0       40 2024-01-27 07:31:59.000000 django_tinywiki-0.0.2/django_tinywiki/forms/__init__.py
+-rw-rw-rw-   0        0        0      742 2024-03-03 12:02:38.000000 django_tinywiki-0.0.2/django_tinywiki/forms/auth.py
+-rw-rw-rw-   0        0        0     2895 2024-02-14 14:23:31.000000 django_tinywiki-0.0.2/django_tinywiki/forms/wiki.py
+drwxrwxrwx   0        0        0        0 2024-05-09 10:34:06.639477 django_tinywiki-0.0.2/django_tinywiki/functions/
+-rw-rw-rw-   0        0        0       38 2024-03-05 21:18:55.000000 django_tinywiki-0.0.2/django_tinywiki/functions/__init__.py
+-rw-rw-rw-   0        0        0     2438 2024-03-03 15:43:02.000000 django_tinywiki-0.0.2/django_tinywiki/functions/auth.py
+-rw-rw-rw-   0        0        0     3575 2024-02-14 16:45:41.000000 django_tinywiki-0.0.2/django_tinywiki/functions/init.py
+-rw-rw-rw-   0        0        0     5313 2024-03-05 21:27:18.000000 django_tinywiki-0.0.2/django_tinywiki/functions/sidebar.py
+-rw-rw-rw-   0        0        0      714 2024-02-22 23:32:53.000000 django_tinywiki-0.0.2/django_tinywiki/functions/utils.py
+-rw-rw-rw-   0        0        0    10320 2024-03-03 14:37:42.000000 django_tinywiki-0.0.2/django_tinywiki/functions/wiki.py
+drwxrwxrwx   0        0        0        0 2024-05-09 10:34:06.640477 django_tinywiki-0.0.2/django_tinywiki/locale/
+-rw-rw-rw-   0        0        0        0 2024-02-06 21:35:35.000000 django_tinywiki-0.0.2/django_tinywiki/locale/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 10:34:06.640477 django_tinywiki-0.0.2/django_tinywiki/locale/de/
+drwxrwxrwx   0        0        0        0 2024-05-09 10:34:06.642476 django_tinywiki-0.0.2/django_tinywiki/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0        0        0        0 2024-02-06 21:35:52.000000 django_tinywiki-0.0.2/django_tinywiki/locale/de/LC_MESSAGES/__init__.py
+-rw-rw-rw-   0        0        0     5997 2024-03-03 13:47:35.000000 django_tinywiki-0.0.2/django_tinywiki/locale/de/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0        0 2024-02-06 21:35:44.000000 django_tinywiki-0.0.2/django_tinywiki/locale/de/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 10:34:06.649481 django_tinywiki-0.0.2/django_tinywiki/markdown_extensions/
+-rw-rw-rw-   0        0        0      249 2024-02-03 20:58:29.000000 django_tinywiki-0.0.2/django_tinywiki/markdown_extensions/__init__.py
+-rw-rw-rw-   0        0        0     1286 2024-02-03 21:17:33.000000 django_tinywiki-0.0.2/django_tinywiki/markdown_extensions/copyright.py
+-rw-rw-rw-   0        0        0      307 2024-02-08 19:45:28.000000 django_tinywiki-0.0.2/django_tinywiki/markdown_extensions/delpattern.py
+-rw-rw-rw-   0        0        0     1250 2024-01-19 21:10:19.000000 django_tinywiki-0.0.2/django_tinywiki/markdown_extensions/djangourl.py
+-rw-rw-rw-   0        0        0     8035 2024-03-02 17:48:54.000000 django_tinywiki-0.0.2/django_tinywiki/markdown_extensions/tinywikiimage.py
+-rw-rw-rw-   0        0        0     1553 2024-02-13 19:25:47.000000 django_tinywiki-0.0.2/django_tinywiki/markdown_extensions/tinywikilink.py
+-rw-rw-rw-   0        0        0     2985 2024-03-02 12:42:52.000000 django_tinywiki-0.0.2/django_tinywiki/markdown_extensions/video.py
+drwxrwxrwx   0        0        0        0 2024-05-09 10:34:06.653481 django_tinywiki-0.0.2/django_tinywiki/migrations/
+-rw-rw-rw-   0        0        0     8507 2024-02-15 21:55:36.000000 django_tinywiki-0.0.2/django_tinywiki/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     1641 2024-03-03 14:32:52.000000 django_tinywiki-0.0.2/django_tinywiki/migrations/0002_alter_wikiimage_image_alter_wikiimage_image_preview_and_more.py
+-rw-rw-rw-   0        0        0        0 2024-01-13 05:59:06.000000 django_tinywiki-0.0.2/django_tinywiki/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 10:34:06.656480 django_tinywiki-0.0.2/django_tinywiki/models/
+-rw-rw-rw-   0        0        0      123 2024-01-21 01:18:25.000000 django_tinywiki-0.0.2/django_tinywiki/models/__init__.py
+-rw-rw-rw-   0        0        0      285 2024-01-13 05:59:06.000000 django_tinywiki-0.0.2/django_tinywiki/models/language.py
+-rw-rw-rw-   0        0        0     6379 2024-02-11 13:50:40.000000 django_tinywiki-0.0.2/django_tinywiki/models/wiki.py
+drwxrwxrwx   0        0        0        0 2024-05-09 10:34:06.660729 django_tinywiki-0.0.2/django_tinywiki/scripts/
+-rw-rw-rw-   0        0        0        0 2024-02-07 14:35:58.000000 django_tinywiki-0.0.2/django_tinywiki/scripts/__init__.py
+-rw-rw-rw-   0        0        0     1208 2024-02-10 21:41:33.000000 django_tinywiki-0.0.2/django_tinywiki/scripts/initapp.py
+-rw-rw-rw-   0        0        0      130 2024-02-22 23:23:50.000000 django_tinywiki-0.0.2/django_tinywiki/scripts/tinywiki_codehilite_styles.py
+-rw-rw-rw-   0        0        0      135 2024-02-28 17:30:26.000000 django_tinywiki-0.0.2/django_tinywiki/scripts/tinywiki_languages.py
+-rw-rw-rw-   0        0        0      108 2024-02-22 23:22:49.000000 django_tinywiki-0.0.2/django_tinywiki/scripts/tinywiki_styles.py
+-rw-rw-rw-   0        0        0    11866 2024-03-06 21:41:08.000000 django_tinywiki-0.0.2/django_tinywiki/settings.py
+-rw-rw-rw-   0        0        0       60 2024-01-13 05:59:06.000000 django_tinywiki-0.0.2/django_tinywiki/tests.py
+-rw-rw-rw-   0        0        0     2002 2024-03-03 13:14:09.000000 django_tinywiki-0.0.2/django_tinywiki/urls.py
+-rw-rw-rw-   0        0        0       24 2024-02-17 20:32:14.000000 django_tinywiki-0.0.2/django_tinywiki/version.py
+drwxrwxrwx   0        0        0        0 2024-05-09 10:34:06.665735 django_tinywiki-0.0.2/django_tinywiki/views/
+-rw-rw-rw-   0        0        0      148 2024-02-01 12:06:22.000000 django_tinywiki-0.0.2/django_tinywiki/views/__init__.py
+-rw-rw-rw-   0        0        0     6393 2024-03-03 14:03:01.000000 django_tinywiki-0.0.2/django_tinywiki/views/auth.py
+-rw-rw-rw-   0        0        0     1874 2024-02-10 21:50:08.000000 django_tinywiki-0.0.2/django_tinywiki/views/manage.py
+-rw-rw-rw-   0        0        0     5481 2024-03-06 21:43:39.000000 django_tinywiki-0.0.2/django_tinywiki/views/view.py
+-rw-rw-rw-   0        0        0    16843 2024-03-03 15:40:58.000000 django_tinywiki-0.0.2/django_tinywiki/views/wiki.py
+drwxrwxrwx   0        0        0        0 2024-05-09 10:34:06.666736 django_tinywiki-0.0.2/django_tinywiki.egg-info/
+-rw-rw-rw-   0        0        0      581 2024-05-09 10:34:06.000000 django_tinywiki-0.0.2/django_tinywiki.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2445 2024-05-09 10:34:06.000000 django_tinywiki-0.0.2/django_tinywiki.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 10:34:06.000000 django_tinywiki-0.0.2/django_tinywiki.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-09 10:34:06.000000 django_tinywiki-0.0.2/django_tinywiki.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       57 2024-05-09 10:34:06.000000 django_tinywiki-0.0.2/django_tinywiki.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-09 10:34:06.000000 django_tinywiki-0.0.2/django_tinywiki.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      230 2024-02-08 17:56:40.000000 django_tinywiki-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-09 10:34:06.668733 django_tinywiki-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1039 2024-05-09 10:32:27.000000 django_tinywiki-0.0.2/setup.py
```

### Comparing `django-tinywiki-0.0.1/LICENSE` & `django_tinywiki-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-tinywiki-0.0.1/PKG-INFO` & `django_tinywiki-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: django-tinywiki
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple wiki app for the django framework
 Home-page: https://github.com/c9moser/django-tinywiki
 Author: Christian Moser
 Author-email: christian@cmoser.eu
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/c9moser/django-tinywiki
 Project-URL: Issues, https://www.github.com/c9moser/django-tinywiki/issues
 Requires-Python: >= 3.9
 License-File: LICENSE
 Requires-Dist: django>=4.2
 Requires-Dist: django-extras
 Requires-Dist: pillow>=10.2
 Requires-Dist: markdown
+Requires-Dist: pygments
```

### Comparing `django-tinywiki-0.0.1/django_tinywiki/builtin_wiki_pages/Lama.jpg` & `django_tinywiki-0.0.2/django_tinywiki/builtin_wiki_pages/Lama.jpg`

 * *Files identical despite different names*

### Comparing `django-tinywiki-0.0.1/django_tinywiki/builtin_wiki_pages/de.index.md` & `django_tinywiki-0.0.2/django_tinywiki/builtin_wiki_pages/de.index.md`

 * *Files 9% similar despite different names*

```diff
@@ -27,24 +27,42 @@
 [Writing Extensions for Python-Markdown](https://python-markdown.github.io/extensions/api/#writing-extensions-for-python-markdown).
 
 Für einen Überblick über das verwendete Markdonwn kontaktiere die
 [[Anleitung zum verwendeten Markdown]](de-tinywiki-markdown).
 
 ## Installation
 
-``` {.sh}
-python -m pip install --upgrade django-tinywiki
+``` { .sh use_pygments=true }
+python -m pip install django-tinywiki
+```
+
+Nach dem Installieren aktiviere *django-tinywiki* in der *setup.py*
+des Projekts.
+
+``` { .python }
+INSTALLED_APPS = [
+    ...
+    "django_tinywiki",
+    ...
+]
+```
+
+Danach Initialisiere *django-tinywiki* durch das ausführen des 
+*initapp*-Scripts.
+
+``` { .sh }
+python manage.py runscript initapp
 ```
 
 ### Installation per git
 
-``` {.sh}
-$ git clone https://github.com/c9moser/django-tinywiki.git
-$ cd django-tinywiki
-$ pip install .
+``` { .sh }
+git clone https://github.com/c9moser/django-tinywiki.git
+cd django-tinywiki
+pip install .
 ```
 
 ### TinyWiki testen oder als Standalone
 
 Um *django-tinywiki* zu testen, lade es em besten über git herunter. Das 
 Git-Repository beinhaltet das komplette Django Projekt. 
 
@@ -52,40 +70,40 @@
 *python-venv* direkt im Projektverzeichnis oder dem Elternverzeichnis des
 Projekts. Das erlaubt die asuführung des *manage* Scripts.
 
 Aktiviere das Venv und installiere im Anschluß die benötigten Abhängigkeiten,
 lege einen Superuser account an und initialisiere TinyWiki mit dem 
 Django-Script *initapp*.
 
-``` {.sh}
-$ # django-tinywiki per git herunterladen
-$ git clone https://github.com/c9moser/django-tinywiki.git
+``` { .sh }
+# django-tinywiki per git herunterladen
+git clone https://github.com/c9moser/django-tinywiki.git
 
-$ # ins django-tinywiki Verzeichnis wechseln
-$ cd django-tinywiki
+# ins django-tinywiki Verzeichnis wechseln
+cd django-tinywiki
 
-$ # Venv initialisieren
-$ python -m venv --system-site-packages python-venv
+# Venv initialisieren
+python -m venv --system-site-packages python-venv
 
-# # Venv aktivieren
-$ . python-venv/bin/activate
+# Venv aktivieren
+. python-venv/bin/activate
 
-$ # Abhängigkeiten installieren
-$ pip install -r requirements.txt
+# Abhängigkeiten installieren
+pip install -r requirements.txt
 
-$ # Superuser anlegen
-$ ./manage createsuperuser --email "email@example.com" --username "nutzername"
+# Superuser anlegen
+./manage createsuperuser --email "email@example.com" --username "nutzername"
 
-$ # TinyWiki initialisieren (TODO)
-$ ./manage runscript initapp
+# TinyWiki initialisieren
+./manage runscript initapp
 ```
 
 Danach kann der Wiki ausgeführt werden.
 
-``` {.sh}
+``` { .sh }
 ./manage runserver
 ```
 
 Es emfielt sich unter Windows [MSYS2](https://www.msys2.org/) zu verwenden, 
 da das *manage* script für *sh* geschrieben wurde. Andernfalls wirst du
 selbst ein Script für *PowerShell* oder die *cmd.exe* schreiben wollen,
 um die *manage.py* Datei mit der inkludierten virtuellen Pyton-Umgebung
@@ -97,22 +115,27 @@
 Wenn du nur deinen eigenen *SECRET_KEY* bereitstellen, was empfohlen wird,
 willst, erstelle eine Datei mit dem Namen *secret_key.py* und der *SECRET_KEY*
 Variablen im *tinywiki* Verzeichnis. Du kannst auch *SECRET_KEY_FALLBACKS* in
 diese Datei einfügen.
 
 Inhalt der *secret_key.py*:
 
-``` {.python}
+``` { .python }
 SECRET_KEY = "django-secret-key-with-your-secret"
 SECRET_KEY_FALLBACKS = [
     "last-django-secret-key",
     "older-django-secret-key",
 ]
 ```
 
 #### Überschreiben der Standardkonfiguration
 
 Um einen oder mehrere Werte der Stnadardeinstellungen zu überschreiben,
 erstelle die Datei *project_settings.py* im *tinywiki* Verzeichnis. Diese
 Datei sollte alle Konfiurationsvariablen enthalten, die überschreiben werden
 sollen. Die Werte dieser Datei werden am Ende der *settings.py* eingebunden
 und überschreiben alle vorherigen Werte.
+
+## Einstellungen
+
+Die verfügbaren Einstellungen für *TinyWiki* entnehmen sie der 
+[[Anleitung für TinyWiki Einstellungen]](de-tinywiki-settings)
```

### Comparing `django-tinywiki-0.0.1/django_tinywiki/builtin_wiki_pages/de.markdown.md` & `django_tinywiki-0.0.2/django_tinywiki/builtin_wiki_pages/de.markdown.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,66 @@
+{% load static %}
 # TinyWiki Markdown Syntax
 
 ## Inhaltsverzeichnis
 
 [TOC]
 
 ## Einleitung
 
 **Markdown** ist eine simple Auszeichnungssprache, die es erlaubt ihren Inhalt
 als HTML abzubilden. TinyWiki nutzt Markdown für seine Wikiseiten. Guthub zum
 Beispiel nutzt auch Markdown für seien README-Dateien.
 
-Die kurze Anleitung gibt einen Überblick des Markdown Syntax.
+Die kurze Anleitung gibt einen Überblick des verwendeten Markdown Syntax und
+die verwendeten Markdown Erwetierungen.
+
+## WikiPage als Templates
+*TinyWiki*-Seiten werden zuerst von dem Django's Template Prozessor bearbeitet
+bevor sie als Markdown bearbeitet werden. Das erlaubt z.B.: das Verlinken auf
+statischen Inhalt.
+
+Wie z.B.:
+
+``` { .markdown }
+{% templatetag openblock %} load static {% templatetag closeblock %}
+
+![Pfau im Schloss Eggenberg]({% templatetag openblock %} static 'django_tinywiki/images/peacock.jpg' {% templatetag closeblock %})
+```
+
+![Pfau im Schloss Eggenberg]({% static 'django_tinywiki/images/peacock.jpg' %})
+
+### Django Template Tags
+
+Um Django's Templatetags auszugeben verwende das Template ```templatetag```.
+
+``` { .markdown }
+{% templatetag openblock %} templatetag openblock {% templatetag closeblock %}
+```
+
+Template Argumente sind wie folgt:
+
+Argument      |      Tag
+------------- | --------------------------------
+openblock     | {% templatetag openblock %}
+closeblock    | {% templatetag closeblock %}
+openvariable  | {% templatetag openvariable %}
+closevariable | {% templatetag closevariable %}
+openbrace     | {% templatetag openbrace %}
+closebrace    | {% templatetag closebrace %}
+opencomment   | {% templatetag opencomment %}
+closecomment  | {% templatetag closecomment %}
 
 ## Überschriften
 
 Um eine Überschrift in Markdown zu erstellen, beginne eine Zeile mit mindestens
 einen Rautezeichen ```#``` gefolgt von einem Leerzeichen. Die Anzahl der
 Rautezeichen bestimmen die Ebene der Überschrift.
 
-```
+``` { .markdown }
 # Überschrift Ebene 1
 
 ## Überschrift Ebene 2
 
 ### Überschrift Ebene 3
 
 #### Überschrift Ebene 4
@@ -36,15 +74,15 @@
 
 Um eine Ebene-1 Überschrift zu erzeugen, kann man den Text der Überschrift mit
 einem Gleich-Zeichen ```=``` unterstreichen. Für eiene Ebene-2 Überschrift
 kann man den Text mit einem Minuszeichen unterstreichen. Es kann jede beliebige
 Anzahl an Zeichen zum Unterstreichen verwendet werden, es sollten aber
 mindestens drei Zeichen sein.
 
-```
+``` { .markdown }
 Überschrift Ebene 1
 ===================
 
 Überschrift Ebene 2
 -------------------
 ```
 
@@ -54,15 +92,15 @@
 oder mehereren Zeilen an Text.
 
 Einen Zeilenumbruch erstellt man, in dem man die Zeile mit Text mit zwei oder
 mehr Leerzeichen beendet.
 
 ### Beispiel
 
-```
+``` { .markdown }
 Das ist eine Zeile,
 gefolgt von einer Zeile.
 
 Das ist ein neuer Absatz.
 Diese Zeile endet mit zwei Leerzeichen.  
 Das ist eine neue Zeile.
 ```
@@ -86,15 +124,15 @@
 
 Um einen Text ***fett und kursiv zu machen*** nutze drei Sternzeichen
 ```***text***```, beziehungsweise drei Unterstriche ```___text___```.
 
 Einen ~~durchgestrichenen Text~~ erzeugt man in dem man ihn zwischen zwei
 Tildezeichen einbettet ```~~text~~```.
 
-```
+``` { .markdown }
 *kursiv*,
 **fett**,
 ***kursiv und fett***,
 **_fett und krusiv_ - nur mehr fett**,
 ~~durchgestrichen~~
 ```
 
@@ -108,43 +146,43 @@
 
 ## Copyright usw.
 
 Um ein Copyright Zeichen (C) wird mit ```(C)```, eine registrierte
 Handelsmarke (R) mit ```(R)``` und ein Warenzeichen mit (TM) mit
 ```(TM)``` dargestellt.
 
-```
+``` { .markdown }
 (C) 2024 Django(R) TinyWiki(TM)
 ```
 
 (C) 2024 Django(R) TinyWiki(TM)
 
 **_CopyrightExtension_ ist eine TinyWiki erweiterung und kein Markdown Standard!**
 
 ## Zitate
 
 Um ein Zitat hinzuzufügen, beginne einen Absatz mit einem Größerzeichen
 ```>```.
 
-```
+``` { .markdown }
 > Das ist ein Zitat.
 > Das Zitat wird fortgesetzt.
 ```
 
 **Das obige Beispiel wird wi folgt Ausgegeben:**
 
 > Das ist ein Zitat.
 > Das Zitat wird fortgesetzt.
 
 ### Zitate und Absätze
 
 Um ein, mehrere Absätze umspannended Zitat, zu erzeugen, plaziere bis auf ein
 ```>``` leere Zeilen als Absatztrenner zwischen den Zitattext.
 
-```
+``` { .markdown }
 > Das ist der erste Absatz.
 >
 > Das ist der Zweite Absatz.
 ```
 
 **Die Ausgabe des obigen Beispiels:**
 
@@ -153,15 +191,15 @@
 > Das ist der Zweite Absatz.
 
 ### Verschachtelte Zitate
 
 Verschachtelte Zitate werden erzeugt, in dem man mehrere Größerzeichen
 ```>>``` verwendet.
 
-```
+``` { .markdown }
 > Das ist ein Zitat.
 >
 >> Das ist ein verschachteltes Zitat.
 ```
 
 **Die Ausgabe de Beispiels:**
 
@@ -172,15 +210,15 @@
 ## Listen
 
 Um ungeordnete Listen zu erstellen verwendet man einen Stern ```*```, ein Plus
 ```+``` oder einen Strich ```-```. Jedes dieser Zeichen führt zu dem selben
 Ergebnis. Um eine verschachtelte Liste zu erstellen, rücke das Listenzeichen
 mit einem Tabulator oder mit vier Leerzeichen ein.
 
-```
+``` { .markdown }
 * Posten 1
 * Posten 2
 * Posten 3
     * Posten 3.1
 ```
 
 **Die Ausgabe sieht wie folgt aus:**
@@ -189,15 +227,15 @@
 * Listenposten 2
 * Listenposten 3
     * Listenposten 3.1
 
 Eine geordnete Liste wird erstellt, in dem man eine Zahl mit einem Punkt danach
 verwndet ```1. Listenposten```.
 
-```
+``` { .markdown }
 1. Listenposten 1
 2. Listenposten 2
 3. Listenposten 3
     1. Listenposten 3.1
 ```
 
 **Und die Ausgabe:**
@@ -211,16 +249,16 @@
 
 Mit *Pipes* ```|``` werden Markdowntabellen erstellt. Jede Spalte wird mit
 einem Pipezeichen getrennt. Um Tabellenüberschriften zu erzeugen, 
 unterstreiche die Spalte mit einem Strich ```-```.
 
 Hier ein Beispiel:
 
-```
-Spalte 1 | Spalte 2 | Splate 3
+``` { .markdown }
+Spalte 1 | Spalte 2 | Spalte 3
 -------- | -------- | --------
     A1   |    B1    |    C1
     A2   |    B2    |    C2
     A3   |    B3    |    C3
 ```
 
 **Das Beispiel sieht wie folgt aus:**
@@ -234,30 +272,30 @@
 ## Codeblöcke
 
 Du kannst Codeblöcke erzeugen, in dem du den Quelltext zwischen
 drei Backticks ``` ` ``` einbettest. Um einen mehreren Zeilen
 umspannenden Codeblock zu erzeugen, beginne und beende einen
 Absatz mit drei Backticks.
 
-```
+```` { .markdown }
 Text ```Code kommt hier rein``` Text
 
-  ```
-  Viele
-  Zeilen
-  von
-  Quelltext
-  ```
 ```
+Viele
+Zeilen
+von
+Quelltext
+```
+````
 
 **Die Ausgabe des obigen Beispiels:**
 
 Text ```Code kommt hier rein``` Text
 
-```
+``` { .markdown }
 Viele
 Zeilen
 von
 Quelltext
 ```
 
 Um eine detaillierterte Anleitung über Codeblöcke zu erhalten, besuche die
@@ -265,15 +303,15 @@
 
 ## Links
 
 Um einen Link den Text hinzuzufügen plaziere den Linktitel zwischen eckige 
 Klammern ```[]``` gefolgt von der Linkadresse in runden Klammern ```()```.
 Der Link hat das Format ```[Link Titel](url)```.
 
-```
+``` { .markdown }
 [Goole Suche](https://www.google.com)
 ```
 
 **Das ergibt:**
 
 [Goole Suche](https://www.google.com)
 
@@ -284,15 +322,15 @@
 
 Man kann auch einen Link mit alternativen Titel erzeugen, indem man den Titel
 ziwschen zwei eckige Klammern, gefolgt von dem Slug in runden Klammern, setzt
 ```[[Alternativer Titel]](wiki-slug)```.
 
 **_TinyWiki Links_ sind eine TinyWiki Erweiterung!**
 
-```
+``` { .markdown }
 * [[de-tinywiki-index]]
 * [[link-existiert-nicht]]
 * [[Deutsche Django's TinyWiki Hauptseite]](de-tinywiki-index)
 * [[Diese Seite existiert nicht]](link-existiert-nicht)
 ```
 
 **Dieses Beispiel wird wie folgt ausgegeben:**
@@ -313,15 +351,15 @@
 ```$[text](app:name|variable|...)``` Format, bei welchem die variablen mit
 einem Pipezeichen ```|``` getrennt werden.
 
 **_Django Links_ sind eine TinyWiki erweiterung und kein Teil des Django-Frameworks!**
 
 Hier ein Beispiel:
 
-```
+``` { .markdown }
 * $[Hauptseite](tinywiki:index)
 * $[Hauptseite erneut](tinywiki:page|de-tinywiki-index)
 ```
 
 * $[Hauptseite](tinywiki:index)
 * $[Hauptseite erneut](tinywiki:page|de-tinywiki-index)
 
@@ -331,52 +369,71 @@
 
 Um mit der Wikiseite verlinkte Bilder einzubinden, verwende das Format
 ```![[image-id]]```. Eingebaute Bilder lassen sich mit dem Format
 ```![[!eingebaute-bild-id]]``` einbinden. Negative Zahlen für
 *eingebaute-bild-id* sind für die TinyWiki internen Seiten reserviert.
 Nutze also positive Nummern für deine *eingebaute-bilder-id*s.
 
-```
+``` { .markdown .overflow-auto}
 ![Picture of hemp](https://de.seedfinder.eu/pics/galerie/Serious_Seeds/AK47/17092099828694083_big.jpg)
 
-![[---2--]]
+![[---1000--]]
 
-![[!-2]]
+![[!-1001]]
 ```
 
 **Die Ausgabe des Beispiels sieht wie folgt aus:**
 
 ![Picture of hemp](https://de.seedfinder.eu/pics/galerie/Serious_Seeds/AK47/17092099828694083_big.jpg)
 
-![[---2--]]
+![[---1000--]]
+
+![[!-1001]]
 
-![[!-2]]
 
 Um die verknüpften Bilder deiner TinyWiki-Seite anzuzeigen, nutze den Tag
 ```[WIKI-IMAGES]```. Dieser Tag generiert einen Grid mit den Vorschaubildern
 der, mit deiner Seite verknüpften, Bilder.
 
-```
+``` { .markdown }
 ### Verknüpfte Bilder
 
 [WIKI-IMAGES]
 ```
 
 **Das ergibt:**
 
 ### Verknüpfte Bilder
 
 [WIKI-IMAGES]
 
-## Ein Inhatlsverzeichnis erstellen
+## Vidoes einbinden
+
+``` { .markdown }
+?[Django tutorial](youtube:rHux0gMZ3Eg)
+
+?[Quallen]({% static 'django_tinywiki/videos/Jellyfish.mp4' %})
+
+?[Quallen mit Breite und Höhe]({% static 'django_tinywiki/videos/Jellyfish.mp4' %}|560,315)
+```
+
+?[Django tutorial](youtube:rHux0gMZ3Eg)
+
+?[Quallen]({% static 'django_tinywiki/videos/Jellyfish.mp4' %})
+
+?[Quallen mit Breite und Höhe]({% static 'django_tinywiki/videos/Jellyfish.mp4' %}|560,315)
+
+**Embedding Videos is a TinyWiki extension**
+
+## Ein Inhaltsverzeichnis erstellen
 
 Um ein Inhaltsverzeichnis zu erstellen, verwende den ```[TOC]```-Tag in einem
 eigenen Absatz.
 
-```
+```{ .markdown }
 ...
 
 [TOC]
 
 ...
 ```
```

### Comparing `django-tinywiki-0.0.1/django_tinywiki/builtin_wiki_pages/en.index.md` & `django_tinywiki-0.0.2/django_tinywiki/builtin_wiki_pages/en.index.md`

 * *Files 14% similar despite different names*

```diff
@@ -25,21 +25,39 @@
 [Writing Extensions for Python-Markdown](https://python-markdown.github.io/extensions/api/#writing-extensions-for-python-markdown).
 
 An overview of the used Markdown for Wiki-pages can be found in the
 [[Guide for used Markdown]](en-tinywiki-markdown).
 
 ## Installation
 
+You can install *django-tinywiki* directly from PyPI.
+
+```
+python -m pip install django-tinywiki
 ```
-python -m pip install --upgrade django-tinywiki
+
+After installing *django-tinywiki* enable it in your project's *settings.py*.
+
+``` { .python }
+INSTALLED_APPS = [
+    ...
+    "django_tinywiki",
+    ...
+]
+```
+
+Then initialize it by running the initapp script:
+
+``` { .sh }
+python manage.py runscript initapp
 ```
 
 ### Installation via git
 
-``` {.sh}
+``` { .sh }
 $ git clone https://github.com/c9moser/django-tinywiki.git
 $ cd django-tinywiki
 $ pip install .
 ```
 
 ### Testing TinyWiki or running it standalone
 
@@ -53,15 +71,15 @@
 After that activate the virtual environment and install the requirements
 of the app. They are found in the *requirements.txt*.
 
 Then create a superuser account and initialize TinyWiki by running the
 *initapp* script.
 
 
-``` {.sh}
+``` { .sh }
 $ # download the django-tinywiki repository using git
 $ git clone https://github.com/c9moser/django-tinywiki.git
 
 $ # Move in the django-tinywiki directory
 $ cd django-tinywiki
 
 $ # Python Virtual environment initialisieren
@@ -78,15 +96,15 @@
 
 $ # Initialize TinyWiki
 $ ./manage runscript initapp
 ```
 
 You can run TinyWiki after the initial setup.
 
-``` {.sh}
+``` { .sh }
 ./manage runserver
 ```
 
 For Windows users, it is recomended to use [MSYS2](https://www.msys2.org),
 to be able to use the manage script. If not you might want to write your
 own script for *PowerShell* or *cmd.exe*.
 
@@ -94,20 +112,25 @@
 
 If you just want to provide your own *SECRET_KEY*, which is recommended,
 create a file *secret_key.py* in the *tinywiki* directory. You can also
 provide the *SECRET_KEY_FALLBACKS* value in *secret_key.py*
 
 Content of the *secret_key.py*
 
-``` {.python}
+``` { .python }
 SECRET_KEY = "django-secret-key-with-your-secret"
 SECRET_KEY_FALLBACKS = [
     "last-django-secret-key",
     "older-django-secret-key",
 ]
 ```
 
 #### Overwriting default settings
 
 To overwrite one or more of the default settings, provide the file
 *project_settings.py* in the *tinywiki* directory. You can place all
 of your settings there. They will overwrite the default settings.
+
+## Settings
+
+To view the available settings for *TinyWiki* visit the [[Settings Documentation]](en-tinywiki-settings).
+
```

### Comparing `django-tinywiki-0.0.1/django_tinywiki/forms/auth.py` & `django_tinywiki-0.0.2/django_tinywiki/forms/auth.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,11 +2,13 @@
 from django.utils.translation import gettext_lazy as _
 
 class LoginForm(forms.Form):
     name = forms.CharField(label=_("Name or Email"),max_length=256)
     password = forms.CharField(label=_("Your Password"),widget=forms.PasswordInput)
 
 class SignupForm(forms.Form):
-    name = forms.CharField(label=_("Name"),max_length=64)
+    username = forms.CharField(label=_("Name"),max_length=64)
     email = forms.EmailField(label=_("Email"))
+    first_name = forms.CharField(label=_("First Name"),max_length=64,required=False)
+    last_name = forms.CharField(label=_("Last Name"),max_length=64,required=False)
     password0 = forms.CharField(label=_("Password"),widget=forms.PasswordInput())
     password1 = forms.CharField(label=_("Confirm Password"),widget=forms.PasswordInput())
```

### Comparing `django-tinywiki-0.0.1/django_tinywiki/forms/wiki.py` & `django_tinywiki-0.0.2/django_tinywiki/forms/wiki.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 def _get_user_choices():
     ret = []
     for user in get_user_model().objects.all():
         inserted = False
         username = user.get_username()
         for i in range(len(ret)):
-            if user.username < i[1]:
+            if user.username < ret[i][1]:
                 ret.insert(i,(user.id,username))
                 inserted = True
         if not inserted:
             ret.append((user.id,username))
 
     return ret
 
@@ -58,7 +58,11 @@
     alt_text = forms.CharField(max_length=1024,
                                required=True,
                                label=_("Alternative Text"))
     description = forms.CharField(max_length=1024,
                                   required=False,
                                   label=_("Descriptions"))
     image = forms.ImageField(label=_("Image to upload"))
+
+class DeletePageForm(forms.Form):
+    delete_page = forms.BooleanField(label=_("Delete Page?"),initial=False,required=False)
+    delete_images = forms.BooleanField(label=_("Delete Images too?"),initial=False,required=False)
```

### Comparing `django-tinywiki-0.0.1/django_tinywiki/markdown_extensions/copyright.py` & `django_tinywiki-0.0.2/django_tinywiki/markdown_extensions/copyright.py`

 * *Files identical despite different names*

### Comparing `django-tinywiki-0.0.1/django_tinywiki/markdown_extensions/djangourl.py` & `django_tinywiki-0.0.2/django_tinywiki/markdown_extensions/djangourl.py`

 * *Files identical despite different names*

### Comparing `django-tinywiki-0.0.1/django_tinywiki/markdown_extensions/tinywikiimage.py` & `django_tinywiki-0.0.2/django_tinywiki/markdown_extensions/tinywikiimage.py`

 * *Files 9% similar despite different names*

```diff
@@ -62,33 +62,17 @@
                 link_element.append(etree.Element("br"))
                 desc_element = etree.Element("span",attrib={'class':'wiki-image-description'})
                 desc_element.text = img.description
                 link_element.append(desc_element)
             element.append(link_element)
 
             
-        except Exception as error:
+        except WikiImage.DoesNotExist:
             element = etree.Element("div", attrib={"class":"wiki-image image-not-found"})
             element.text = _("Image with id {img_id} not found!".format(img_id=m.group(1)))
-
-            if img.image_wiki:
-                attrib = {'src':img.image_wiki.url}
-            else:
-                attrib = {'src':img.image.url}
-
-            if img.alt:
-                attrib['alt'] = img.alt
-
-            link_element.append(etree.Element("img",attrib=attrib))
-            if img.description:
-                link_element.append(etree.Element("br"))
-                desc_element = etree.Element("span",attrib={'class':'wiki-image-description'})
-                desc_element.text = img.description
-                link_element.append(desc_element)
-            element.append(link_element)
         
         return element, m.start(0), m.end(0)
 
 class TinywikiBuiltinImageInlineProcessor(InlineProcessor):
     def handleMatch(self, m: Match, data):
         builtin_id = int(m.group(1))
```

### Comparing `django-tinywiki-0.0.1/django_tinywiki/markdown_extensions/tinywikilink.py` & `django_tinywiki-0.0.2/django_tinywiki/markdown_extensions/tinywikilink.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,28 +15,28 @@
     
         try:
             page = models.WikiPage.objects.get(slug=slug)
             title = escape(page.title)
         except models.WikiPage.DoesNotExist:
             title = slug
     
-        url = str(reverse(settings.TINYWIKI_PAGE_VIEW_URL,args=[slug]))
+        url = str(reverse(settings.TINYWIKI_PAGE_VIEW_URL_TEMPLATE,args=[slug]))
                 
         element = etree.Element("a",attrib={'href':url})
         element.text = title
 
         
         return element, m.start(0), m.end(0)
 
 class TinyWikiLinkTitleInlineProcessor(InlineProcessor):
     def handleMatch(self,m,data):
         slug = m.group(2)
         title = m.group(1)
     
-        url = str(reverse(settings.TINYWIKI_PAGE_VIEW_URL,args=[slug]))
+        url = str(reverse(settings.TINYWIKI_PAGE_VIEW_URL_TEMPLATE,args=[slug]))
 
         element = etree.Element("a",attrib={'href':url})
         element.text = title
 
         return element, m.start(0), m.end(0)
 class TinywikiLinkExtension(extensions.Extension):
     def extendMarkdown(self,md):
```

### Comparing `django-tinywiki-0.0.1/django_tinywiki/migrations/0007_alter_wikiimage_builtin_id_alter_wikiimage_image_and_more.py` & `django_tinywiki-0.0.2/django_tinywiki/migrations/0002_alter_wikiimage_image_alter_wikiimage_image_preview_and_more.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,34 @@
-# Generated by Django 4.2.7 on 2024-01-31 15:09
+# Generated by Django 4.2.7 on 2024-03-03 14:32
 
 import django.core.files.storage
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
-        ('django_tinywiki', '0006_wikiimage_builtin_id'),
+        ('django_tinywiki', '0001_initial'),
     ]
 
     operations = [
         migrations.AlterField(
             model_name='wikiimage',
-            name='builtin_id',
-            field=models.IntegerField(null=True, unique=True),
-        ),
-        migrations.AlterField(
-            model_name='wikiimage',
             name='image',
-            field=models.ImageField(storage=django.core.files.storage.FileSystemStorage(base_url='/wiki/', location='C:/msys64/home/c9mos/projekte/django/django-tinywiki/media/wiki'), upload_to='img/original'),
+            field=models.ImageField(storage=django.core.files.storage.FileSystemStorage(base_url='/media/wiki/', location='C:/msys64/home/c9mos/projekte/django/django-tinywiki/media/wiki'), upload_to='images/original'),
         ),
         migrations.AlterField(
             model_name='wikiimage',
             name='image_preview',
-            field=models.ImageField(null=True, storage=django.core.files.storage.FileSystemStorage(base_url='/wiki/', location='C:/msys64/home/c9mos/projekte/django/django-tinywiki/media/wiki'), upload_to=''),
+            field=models.ImageField(null=True, storage=django.core.files.storage.FileSystemStorage(base_url='/media/wiki/', location='C:/msys64/home/c9mos/projekte/django/django-tinywiki/media/wiki'), upload_to='images/preview'),
         ),
         migrations.AlterField(
             model_name='wikiimage',
             name='image_sidebar',
-            field=models.ImageField(null=True, storage=django.core.files.storage.FileSystemStorage(base_url='/wiki/', location='C:/msys64/home/c9mos/projekte/django/django-tinywiki/media/wiki'), upload_to=''),
+            field=models.ImageField(null=True, storage=django.core.files.storage.FileSystemStorage(base_url='/media/wiki/', location='C:/msys64/home/c9mos/projekte/django/django-tinywiki/media/wiki'), upload_to='images/sidebar'),
         ),
         migrations.AlterField(
             model_name='wikiimage',
             name='image_wiki',
-            field=models.ImageField(null=True, storage=django.core.files.storage.FileSystemStorage(base_url='/wiki/', location='C:/msys64/home/c9mos/projekte/django/django-tinywiki/media/wiki'), upload_to=''),
+            field=models.ImageField(null=True, storage=django.core.files.storage.FileSystemStorage(base_url='/media/wiki/', location='C:/msys64/home/c9mos/projekte/django/django-tinywiki/media/wiki'), upload_to='images/wiki'),
         ),
     ]
```

### Comparing `django-tinywiki-0.0.1/django_tinywiki/models/wiki.py` & `django_tinywiki-0.0.2/django_tinywiki/models/wiki.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
         max_length=512)
     language = models.ForeignKey(
         WikiLanguage,
         on_delete=models.RESTRICT,
         null=False,
         related_name="tinywiki_pages")
     content = models.TextField(null=False,blank=True)
+    contentfile_md5 = models.CharField(null=True,max_length=32,default=None)
     user = models.ForeignKey(settings.TINYWIKI_AUTH_USER_MODEL,
                              on_delete=models.SET_NULL,
                              null=True,
                              related_name='tinywiki_pages_user')
     created_on = models.DateTimeField(auto_now_add=True)
     created_by = models.ForeignKey(
         settings.TINYWIKI_AUTH_USER_MODEL,
@@ -48,14 +49,22 @@
             models.Index(name="tinywiki_wp_lang_index",fields=["language"]),
             models.Index(name="tinywiki_wp_user_index",fields=["user",]),
             models.Index(name="tinywiki_wp_cby_index",fields=["created_by"]),
             models.Index(name="tinywiki_wp_con_index",fields=["created_on"]),
             models.Index(name="tinywiki_wp_eby_index",fields=["edited_by"]),
             models.Index(name="tinywiki_wp_eon_index",fields=["edited_on"]),
         ]
+
+        permissions = [
+            (settings.TINYWIKI_PERM_CREATE_PAGE, "User can create pages"),
+            (settings.TINYWIKI_PERM_DELETE_PAGE, "User can delete pages"),
+            (settings.TINYWIKI_PERM_EDIT_PAGE, "User can edit all pages"),
+            (settings.TINYWIKI_PERM_EDIT_USER_PAGE, "User can edit the pages he owns"),
+        ]
+
 # WikiPage class
 
 class WikiPageBackup(models.Model):
     wiki_page = models.ForeignKey(
         WikiPage,
         on_delete=models.CASCADE,
         related_name="backups")
```

### Comparing `django-tinywiki-0.0.1/django_tinywiki/scripts/initapp.py` & `django_tinywiki-0.0.2/django_tinywiki/scripts/initapp.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,25 +17,22 @@
             user.save()
         except:
             pass
     except UserModel.DoesNotExist:
         try:
             user = UserModel.objects.create(**settings.TINYWIKI_USER)
             user.password = get_random_string(length=32)
-            try:
-                user.is_superuser = True
-            except:
-                pass
+            user.is_superuser = True
             user.save()
         except Exception as err:
             print(_("Unable to create TinyWiki user! ({error_message})").format(error_message=str(err)),file=sys.stderr)
             for i in UserModel.objects.filter(is_superuser=True).order_by('id'):
                 if i.is_superuser:
                     user = i
                     break
     if user is None:
         raise LookupError("No user to select to initialize TinyWiki! ABORTING!")
     
-    func.init_app(user)
+    func.init.init_app(user)
```

### Comparing `django-tinywiki-0.0.1/django_tinywiki/views/manage.py` & `django_tinywiki-0.0.2/django_tinywiki/views/manage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .view import ViewBase
 from .. import settings
 from django.shortcuts import render
-from ..functions import init_app
+from ..functions.init import init_app
 from django.urls import reverse_lazy
 from django.conf import settings as django_settings
 from ..decorators import perm_superuser
 from django.contrib.auth.decorators import login_required
 from django.utils.decorators import method_decorator
 
 class ManageView(ViewBase):
```

### Comparing `django-tinywiki-0.0.1/django_tinywiki/views/wiki.py` & `django_tinywiki-0.0.2/django_tinywiki/views/wiki.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from django.urls import reverse
 from django.views import View
 from django.utils.translation import gettext
 from django.contrib.auth import get_user_model
 from django.core.files import File
 from django.core.exceptions import PermissionDenied
 from django.utils.decorators import method_decorator
-from django.contrib.auth.decorators import login_required
+from django.contrib.auth.decorators import login_required,permission_required
+from django.http import HttpResponseNotFound
 
 
 from PIL import Image
 
 import re
 
 _ = gettext
@@ -23,23 +24,21 @@
     WikiLanguage,
     WikiImage
 )
 
 from ..forms.wiki import (
     PageForm,
     ImageUploadForm,
+    DeletePageForm,
 )
 
 import os
 
-from ..functions import (
-    user_can_create_pages,
-    get_language_code,
-    render_markdown)
-
+from ..functions.wiki import render_markdown
+from ..decorators import perm_can_edit_page
 from .view import ViewBase
 # Create your views here.
 
 class WikiPageView(ViewBase):
     page_template = settings.TINYWIKI_PAGE_VIEW_TEMPLATE
     image_upload_url = settings.TINYWIKI_IMAGE_UPLOAD_URL
 
@@ -48,21 +47,23 @@
         if page:
             page_context = {
                 'slug':page.slug,
                 'title': page.title,
                 'language': page.language.code,
                 'edit_page': self.get_user_can_edit_page(request.user,page),
             }
+            
             context.update({
                 "header_subtitle": page.title,
                 "title":page.title,
                 "content": render_markdown(page.content,page_context),
                 "edit-page": render_markdown(False),
                 "page": page,
                 'image_upload_url': reverse(self.image_upload_url,kwargs={'page':page.slug}),
+                'codehilite_css': settings.TINYWIKI_CODEHILITE_CSS,
             })
 
         return context
 
     def get(self,request,page):
 
         page_context = {}
@@ -86,43 +87,48 @@
                                        orphaned_images=orphaned_images,
                                        login_url=self.build_login_url(request))
 
         except WikiPage.DoesNotExist:
             if self.get_user_can_create_pages(request.user):
                 return redirect(reverse(settings.TINYWIKI_PAGE_CREATE_URL,args=[page]))
 
-            context = self.get_context(request)
-
-            content_file = os.path.join(os.path.dirname(__file__),"en.404.md")
-            title = _("404 - Page not found!")
-            check_file = os.path.join(os.path.dirname(__file__),'.'.join((get_language_code,"404","md")))
-            if os.path.isfile(check_file):
-                content_file = check_file
-
-            with open(content_file,"r") as ifile:
-                page_content = ifile.read()
-
-            context.update({
-                'header_subtitle': title,
-                'title': title,
-                'content': render_markdown(page_content,page_context)
-            })
+            return HttpResponseNotFound("<h1>Page not found</h1>")
 
         return render(request,self.page_template,context)
 
 class WikiIndexView(WikiPageView):
     index_page=settings.TINYWIKI_INDEX
 
     def get(self,request):
         return WikiPageView.get(self,request,page=self.index_page)
 
+class WikiPageOverviewView(ViewBase):
+    template=settings.TINYWIKI_PAGE_OVERVIEW_TEMPLATE
+
+    def get(self,request):
+        wikilang=[]
+        for lang in WikiLanguage.objects.all().order_by("code"):
+            if lang.tinywiki_pages.all().count() > 0:
+                lang_name = _(lang.name)
+                lang_inserted = False
+                for i in range(len(wikilang)):
+                    if lang_name < wikilang[i]['language_name']:
+                        wikilang.insert(i,{'language_name':lang_name,'language':lang})
+                        lang_inserted = True
+                        break
+                if not lang_inserted:
+                    wikilang.append({'language_name':lang_name,'language':lang})
+
+        context = self.get_context(request,wiki_languages=wikilang)
+        return render(request,self.template,context)
 class WikiCreateView(ViewBase):
     template = settings.TINYWIKI_PAGE_EDIT_TEMPLATE
     
     @method_decorator(login_required(login_url=settings.TINYWIKI_LOGIN_URL))
+    @method_decorator(permission_required(settings.TINYWIKI_USERPERM_CREATE_PAGE,raise_exception=True))
     def get(self,request,page=None):
         if not self.get_user_can_create_pages(request.user):
             raise PermissionDenied
         
         context=self.get_context(request=request)
         if page:
             try:
@@ -136,14 +142,15 @@
         }
         if page is not None:
             form_defaults['slug'] = page
         context['form'] = PageForm(form_defaults)
         return render(request,self.template,context)
 
     @method_decorator(login_required(login_url=settings.TINYWIKI_LOGIN_URL))
+    @method_decorator(permission_required(settings.TINYWIKI_USERPERM_CREATE_PAGE,raise_exception=True))
     def post(self,request,page=None):
         if not self.get_user_can_create_pages(request.user):
             raise PermissionDenied
         
         context = self.get_context(request=request,page=page)
 
         form = PageForm(request.POST)
@@ -182,19 +189,20 @@
                 
         return render(request,self.template,context)
 
 class WikiEditView(ViewBase):
     template = settings.TINYWIKI_PAGE_EDIT_TEMPLATE
 
     @method_decorator(login_required(login_url=settings.TINYWIKI_LOGIN_URL))
+    @method_decorator(perm_can_edit_page())
     def get(self,request,page):
         try:
             p = WikiPage.objects.get(slug=page)
         except WikiPage.DoesNotExist:
-            return redirect(reverse(settings.TINYWIKI_PAGE_CREATE_URL,kwargs={'page':page}))
+            return redirect(reverse(settings.TINYWIKI_PAGE_CREATE_URL_TEMPLATE,kwargs={'page':page}))
         
         if not self.get_user_can_edit_page(request.user,p):
             raise PermissionDenied
         
         if p.user:
             page_user_id = p.user.id
         else:
@@ -212,14 +220,15 @@
         form = PageForm(form_data)
 
         context = self.get_context(request=request,page=p,form=form,slug=p.slug)
         
         return render(request,self.template,context)
     
     @method_decorator(login_required(login_url=settings.TINYWIKI_LOGIN_URL))
+    @method_decorator(perm_can_edit_page())
     def post(self,request,page):
         try:
             p = WikiPage.objects.get(id=page)
         except WikiPage.DoesNotExist:
             return redirect(reverse(settings.TINYWIKI_PAGE_CREATE_URL,kwargs={'page':page}))
         
         if not self.get_user_can_edit_page(request.user,p):
@@ -271,22 +280,26 @@
 
         return render(request,self.base_template,context)
     
 class WikiImageUploadView(ViewBase):
     template = settings.TINYWIKI_IMAGE_UPLOAD_TEMPLATE
     image_upload_directory = settings.TINYWIKI_IMAGE_UPLOAD_DIRECTORY
 
+    @method_decorator(login_required(login_url=settings.TINYWIKI_LOGIN_URL))
+    @method_decorator(perm_can_edit_page())
     def get(self,request,page):
         p = get_object_or_404(WikiPage,slug=page)
 
         form = ImageUploadForm()
 
         context = self.get_context(request=request,page=p,form=form)
         return render(request,self.template,context)
 
+    @method_decorator(login_required(login_url=settings.TINYWIKI_LOGIN_URL))
+    @method_decorator(perm_can_edit_page())
     def post(self,request,page):
         p = get_object_or_404(WikiPage,slug=page)
 
         form = ImageUploadForm(request.POST,request.FILES)
         if form.is_valid():
 
             img_create_kwargs = {
@@ -359,7 +372,69 @@
                 os.unlink(wiki_name)
 
             return redirect(reverse(self.page_view_url,kwargs={'page':page}))
         
         context = self.get_context(request=request,page=p,form=form)
 
         return render(request,self.template,context)
+
+class WikiDeletePageView(ViewBase):
+    template=settings.TINYWIKI_PAGE_DELETE_TEMPLATE
+    done_template=settings.TINYWIKI_PAGE_DELETE_DONE_TEMPLATE
+
+    @method_decorator(login_required(login_url=settings.TINYWIKI_LOGIN_URL))
+    @method_decorator(permission_required(settings.TINYWIKI_USERPERM_DELETE_PAGE))
+    def get(self,request,page):
+        p = get_object_or_404(WikiPage,slug=page)
+        context = self.get_context(request,page=p,form=DeletePageForm(),slug=page)
+        return render(request,self.template,context)
+    
+    @method_decorator(login_required(login_url=settings.TINYWIKI_LOGIN_URL))
+    @method_decorator(permission_required(settings.TINYWIKI_USERPERM_DELETE_PAGE))
+    def post(self,request,page):
+        p = get_object_or_404(WikiPage,slug=page)
+        form = DeletePageForm(request.POST)
+        if form.is_valid():
+            delete_page = form.cleaned_data['delete_page']
+            delete_images = form.cleaned_data['delete_images']
+
+            if delete_page:
+                class PageData:
+                    title = p.title
+                    slug = p.slug
+                    user = p.user
+                    created_on = p.created_on
+                    created_by = p.created_by
+                    edited_on = p.edited_on
+                    edited_by = p.edited_by
+
+                backup = WikiPageBackup.objects.create(
+                    wiki_page=p,
+                    user=p.user,
+                    language=p.language,
+                    slug=p.slug,
+                    title = p.title,
+                    edited_by=p.edited_by,
+                    edited_on=p.edited_on,
+                    created_by=p.created_by,
+                    created_on=p.created_on,
+                    content=p.content,
+                    edited_reason=p.edited_reason
+                )
+
+                if delete_images:
+                    for page_img in p.images.all():
+                        if os.path.isfile(page_img.image_wiki.path):
+                            os.unlink(page_img.image_wiki.path)
+                        if os.path.isfile(page_img.image_preview.path):
+                            os.unlink(page_img.image_preview.path)
+                        if os.path.isfile(page_img.image_sidebar.path):
+                            os.unlink(page_img.image_sidebar.path)
+                        if os.path.isfile(page_img.image.path):
+                            os.path.unlink(page_img.image.path)
+                        page_img.delete()
+               
+                p.delete()
+                context = self.get_context(request)
+                return render(request,self.done_template,context,page_data=PageData())
+            
+        return redirect(reverse(self.page_view_url,kwargs={'page':page}))
```

### Comparing `django-tinywiki-0.0.1/django_tinywiki.egg-info/PKG-INFO` & `django_tinywiki-0.0.2/django_tinywiki.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: django-tinywiki
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple wiki app for the django framework
 Home-page: https://github.com/c9moser/django-tinywiki
 Author: Christian Moser
 Author-email: christian@cmoser.eu
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/c9moser/django-tinywiki
 Project-URL: Issues, https://www.github.com/c9moser/django-tinywiki/issues
 Requires-Python: >= 3.9
 License-File: LICENSE
 Requires-Dist: django>=4.2
 Requires-Dist: django-extras
 Requires-Dist: pillow>=10.2
 Requires-Dist: markdown
+Requires-Dist: pygments
```

### Comparing `django-tinywiki-0.0.1/setup.py` & `django_tinywiki-0.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from setuptools import setup,find_packages
 
 setup(
     name="django-tinywiki",
     description="A simple wiki app for the django framework",
-    version="0.0.1",
+    version="0.0.2",
     author="Christian Moser",
     author_email="christian@cmoser.eu",
     install_requires=[
         "django >= 4.2",
 	    "django-extras",
 	    "pillow >=10.2",
 	    "markdown",
+        "pygments",
     ],
     packages=find_packages(
         include=["django_tinywiki*"],
         exclude=["tinywiki","media","locale"]
     ),
     include_package_data=True,
     package_data={
@@ -26,8 +27,8 @@
     license_files=["LICENSE",],
     zip_safe=False,
     python_requires=">= 3.9",
     project_urls={
         'Homepage':"https://github.com/c9moser/django-tinywiki",
         'Issues': "https://www.github.com/c9moser/django-tinywiki/issues",
     }
-)
+)
```

