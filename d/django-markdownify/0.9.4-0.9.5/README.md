# Comparing `tmp/django_markdownify-0.9.4.tar.gz` & `tmp/django_markdownify-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_markdownify-0.9.4.tar", last modified: Wed May  8 07:28:48 2024, max compression
+gzip compressed data, was "django_markdownify-0.9.5.tar", last modified: Thu May  9 11:44:47 2024, max compression
```

## Comparing `django_markdownify-0.9.4.tar` & `django_markdownify-0.9.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2024-05-08 07:28:48.648609 django_markdownify-0.9.4/
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)     1080 2020-10-02 20:03:12.000000 django_markdownify-0.9.4/LICENSE
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)       60 2020-10-02 20:03:12.000000 django_markdownify-0.9.4/MANIFEST.in
--rw-r--r--   0 erwin     (1000) erwin     (1000)     3034 2024-05-08 07:28:48.648609 django_markdownify-0.9.4/PKG-INFO
--rw-rw-r--   0 erwin     (1000) erwin     (1000)     2383 2024-05-08 07:24:44.000000 django_markdownify-0.9.4/README.md
-drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2024-05-08 07:28:48.648609 django_markdownify-0.9.4/django_markdownify.egg-info/
--rw-r--r--   0 erwin     (1000) erwin     (1000)     3034 2024-05-08 07:28:48.000000 django_markdownify-0.9.4/django_markdownify.egg-info/PKG-INFO
--rw-rw-r--   0 erwin     (1000) erwin     (1000)      717 2024-05-08 07:28:48.000000 django_markdownify-0.9.4/django_markdownify.egg-info/SOURCES.txt
--rw-rw-r--   0 erwin     (1000) erwin     (1000)        1 2024-05-08 07:28:48.000000 django_markdownify-0.9.4/django_markdownify.egg-info/dependency_links.txt
--rw-rw-r--   0 erwin     (1000) erwin     (1000)       35 2024-05-08 07:28:48.000000 django_markdownify-0.9.4/django_markdownify.egg-info/requires.txt
--rw-rw-r--   0 erwin     (1000) erwin     (1000)       12 2024-05-08 07:28:48.000000 django_markdownify-0.9.4/django_markdownify.egg-info/top_level.txt
-drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2024-05-08 07:28:48.648609 django_markdownify-0.9.4/markdownify/
--rw-rw-r--   0 erwin     (1000) erwin     (1000)        0 2023-03-20 14:40:26.000000 django_markdownify-0.9.4/markdownify/__init__.py
--rw-rw-r--   0 erwin     (1000) erwin     (1000)      153 2023-03-20 14:40:26.000000 django_markdownify-0.9.4/markdownify/apps.py
--rw-rw-r--   0 erwin     (1000) erwin     (1000)      860 2023-03-20 14:40:26.000000 django_markdownify-0.9.4/markdownify/checks.py
-drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2024-05-08 07:28:48.648609 django_markdownify-0.9.4/markdownify/templatetags/
--rw-rw-r--   0 erwin     (1000) erwin     (1000)        0 2023-03-20 14:40:26.000000 django_markdownify-0.9.4/markdownify/templatetags/__init__.py
--rw-rw-r--   0 erwin     (1000) erwin     (1000)     3477 2024-05-08 07:24:29.000000 django_markdownify-0.9.4/markdownify/templatetags/markdownify.py
-drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2024-05-08 07:28:48.648609 django_markdownify-0.9.4/markdownify/tests/
--rw-rw-r--   0 erwin     (1000) erwin     (1000)        0 2023-03-20 14:40:26.000000 django_markdownify-0.9.4/markdownify/tests/__init__.py
--rw-rw-r--   0 erwin     (1000) erwin     (1000)       31 2023-03-20 14:40:26.000000 django_markdownify-0.9.4/markdownify/tests/input_text_alternative.md
--rw-rw-r--   0 erwin     (1000) erwin     (1000)      174 2023-03-20 14:40:26.000000 django_markdownify-0.9.4/markdownify/tests/input_text_bleach.md
--rw-rw-r--   0 erwin     (1000) erwin     (1000)      732 2023-03-20 14:40:26.000000 django_markdownify-0.9.4/markdownify/tests/input_text_default.md
--rw-rw-r--   0 erwin     (1000) erwin     (1000)       93 2023-03-20 14:40:26.000000 django_markdownify-0.9.4/markdownify/tests/input_text_extensions.md
--rw-rw-r--   0 erwin     (1000) erwin     (1000)       90 2023-03-20 14:40:26.000000 django_markdownify-0.9.4/markdownify/tests/input_text_linkify.md
--rw-rw-r--   0 erwin     (1000) erwin     (1000)       72 2023-03-20 14:40:26.000000 django_markdownify-0.9.4/markdownify/tests/input_text_strip.md
--rw-rw-r--   0 erwin     (1000) erwin     (1000)    13273 2024-05-08 07:24:29.000000 django_markdownify-0.9.4/markdownify/tests/test_markdownify.py
--rw-rw-r--   0 erwin     (1000) erwin     (1000)       84 2022-04-15 06:22:01.000000 django_markdownify-0.9.4/pyproject.toml
--rw-rw-r--   0 erwin     (1000) erwin     (1000)       38 2024-05-08 07:28:48.648609 django_markdownify-0.9.4/setup.cfg
--rw-rw-r--   0 erwin     (1000) erwin     (1000)     1138 2024-05-08 07:24:29.000000 django_markdownify-0.9.4/setup.py
+drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2024-05-09 11:44:47.032765 django_markdownify-0.9.5/
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)     1080 2020-10-02 20:03:12.000000 django_markdownify-0.9.5/LICENSE
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)       60 2020-10-02 20:03:12.000000 django_markdownify-0.9.5/MANIFEST.in
+-rw-r--r--   0 erwin     (1000) erwin     (1000)     3034 2024-05-09 11:44:47.032765 django_markdownify-0.9.5/PKG-INFO
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)     2383 2024-05-08 07:24:44.000000 django_markdownify-0.9.5/README.md
+drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2024-05-09 11:44:47.032765 django_markdownify-0.9.5/django_markdownify.egg-info/
+-rw-r--r--   0 erwin     (1000) erwin     (1000)     3034 2024-05-09 11:44:47.000000 django_markdownify-0.9.5/django_markdownify.egg-info/PKG-INFO
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)      717 2024-05-09 11:44:47.000000 django_markdownify-0.9.5/django_markdownify.egg-info/SOURCES.txt
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)        1 2024-05-09 11:44:47.000000 django_markdownify-0.9.5/django_markdownify.egg-info/dependency_links.txt
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)       35 2024-05-09 11:44:47.000000 django_markdownify-0.9.5/django_markdownify.egg-info/requires.txt
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)       12 2024-05-09 11:44:47.000000 django_markdownify-0.9.5/django_markdownify.egg-info/top_level.txt
+drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2024-05-09 11:44:47.032765 django_markdownify-0.9.5/markdownify/
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)        0 2023-03-20 14:40:26.000000 django_markdownify-0.9.5/markdownify/__init__.py
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)      153 2023-03-20 14:40:26.000000 django_markdownify-0.9.5/markdownify/apps.py
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)      860 2023-03-20 14:40:26.000000 django_markdownify-0.9.5/markdownify/checks.py
+drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2024-05-09 11:44:47.032765 django_markdownify-0.9.5/markdownify/templatetags/
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)        0 2023-03-20 14:40:26.000000 django_markdownify-0.9.5/markdownify/templatetags/__init__.py
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)     3498 2024-05-09 11:41:26.000000 django_markdownify-0.9.5/markdownify/templatetags/markdownify.py
+drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2024-05-09 11:44:47.032765 django_markdownify-0.9.5/markdownify/tests/
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)        0 2023-03-20 14:40:26.000000 django_markdownify-0.9.5/markdownify/tests/__init__.py
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)       31 2023-03-20 14:40:26.000000 django_markdownify-0.9.5/markdownify/tests/input_text_alternative.md
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)      174 2023-03-20 14:40:26.000000 django_markdownify-0.9.5/markdownify/tests/input_text_bleach.md
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)      732 2023-03-20 14:40:26.000000 django_markdownify-0.9.5/markdownify/tests/input_text_default.md
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)       93 2023-03-20 14:40:26.000000 django_markdownify-0.9.5/markdownify/tests/input_text_extensions.md
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)       90 2023-03-20 14:40:26.000000 django_markdownify-0.9.5/markdownify/tests/input_text_linkify.md
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)       72 2023-03-20 14:40:26.000000 django_markdownify-0.9.5/markdownify/tests/input_text_strip.md
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)    13273 2024-05-08 07:24:29.000000 django_markdownify-0.9.5/markdownify/tests/test_markdownify.py
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)       84 2022-04-15 06:22:01.000000 django_markdownify-0.9.5/pyproject.toml
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)       38 2024-05-09 11:44:47.032765 django_markdownify-0.9.5/setup.cfg
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)     1138 2024-05-09 11:43:39.000000 django_markdownify-0.9.5/setup.py
```

### Comparing `django_markdownify-0.9.4/LICENSE` & `django_markdownify-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django_markdownify-0.9.4/PKG-INFO` & `django_markdownify-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django-markdownify
-Version: 0.9.4
+Version: 0.9.5
 Summary: Markdown template filter for Django.
 Home-page: https://github.com/erwinmatijsen/django-markdownify
-Download-URL: https://github.com/erwinmatijsen/django-markdownify/archive/0.9.4.tar.gz
+Download-URL: https://github.com/erwinmatijsen/django-markdownify/archive/0.9.5.tar.gz
 Author: Erwin Matijsen, R Moelker
 Author-email: erwin@erwinmatijsen.nl
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: django-markdownify Version: 0.9.4 Summary: Markdown
+Metadata-Version: 2.1 Name: django-markdownify Version: 0.9.5 Summary: Markdown
 template filter for Django. Home-page: https://github.com/erwinmatijsen/django-
 markdownify Download-URL: https://github.com/erwinmatijsen/django-markdownify/
-archive/0.9.4.tar.gz Author: Erwin Matijsen, R Moelker Author-email:
+archive/0.9.5.tar.gz Author: Erwin Matijsen, R Moelker Author-email:
 erwin@erwinmatijsen.nl License: MIT Classifier: Environment :: Web Environment
 Classifier: Framework :: Django Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: Django Requires-Dist: markdown
 Requires-Dist: bleach[css]>=5.0.0 # Django Markdownify - A Django Markdown
 filter ![PyPi Downloads](https://img.shields.io/pypi/dm/django-markdownify) !
 [License](https://img.shields.io/pypi/l/django-markdownify?color=brightgreen)
```

### Comparing `django_markdownify-0.9.4/README.md` & `django_markdownify-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `django_markdownify-0.9.4/django_markdownify.egg-info/PKG-INFO` & `django_markdownify-0.9.5/django_markdownify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django-markdownify
-Version: 0.9.4
+Version: 0.9.5
 Summary: Markdown template filter for Django.
 Home-page: https://github.com/erwinmatijsen/django-markdownify
-Download-URL: https://github.com/erwinmatijsen/django-markdownify/archive/0.9.4.tar.gz
+Download-URL: https://github.com/erwinmatijsen/django-markdownify/archive/0.9.5.tar.gz
 Author: Erwin Matijsen, R Moelker
 Author-email: erwin@erwinmatijsen.nl
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: django-markdownify Version: 0.9.4 Summary: Markdown
+Metadata-Version: 2.1 Name: django-markdownify Version: 0.9.5 Summary: Markdown
 template filter for Django. Home-page: https://github.com/erwinmatijsen/django-
 markdownify Download-URL: https://github.com/erwinmatijsen/django-markdownify/
-archive/0.9.4.tar.gz Author: Erwin Matijsen, R Moelker Author-email:
+archive/0.9.5.tar.gz Author: Erwin Matijsen, R Moelker Author-email:
 erwin@erwinmatijsen.nl License: MIT Classifier: Environment :: Web Environment
 Classifier: Framework :: Django Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: Django Requires-Dist: markdown
 Requires-Dist: bleach[css]>=5.0.0 # Django Markdownify - A Django Markdown
 filter ![PyPi Downloads](https://img.shields.io/pypi/dm/django-markdownify) !
 [License](https://img.shields.io/pypi/l/django-markdownify?color=brightgreen)
```

### Comparing `django_markdownify-0.9.4/django_markdownify.egg-info/SOURCES.txt` & `django_markdownify-0.9.5/django_markdownify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_markdownify-0.9.4/markdownify/checks.py` & `django_markdownify-0.9.5/markdownify/checks.py`

 * *Files identical despite different names*

### Comparing `django_markdownify-0.9.4/markdownify/templatetags/markdownify.py` & `django_markdownify-0.9.5/markdownify/templatetags/markdownify.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from django import template
 from django.conf import settings
 from django.utils.safestring import mark_safe
 
 import markdown
 import bleach
+from bleach import css_sanitizer as cs
 
 
 register = template.Library()
 
 
 @register.filter
 def markdownify(text, custom_settings="default"):
@@ -18,15 +19,15 @@
         markdownify_settings = settings.MARKDOWNIFY[custom_settings]
     except (AttributeError, KeyError):
         markdownify_settings = {}
 
     # Bleach settings
     whitelist_tags = markdownify_settings.get('WHITELIST_TAGS', bleach.sanitizer.ALLOWED_TAGS)
     whitelist_attrs = markdownify_settings.get('WHITELIST_ATTRS', bleach.sanitizer.ALLOWED_ATTRIBUTES)
-    whitelist_styles = markdownify_settings.get('WHITELIST_STYLES', bleach.css_sanitizer.ALLOWED_CSS_PROPERTIES)
+    whitelist_styles = markdownify_settings.get('WHITELIST_STYLES', cs.ALLOWED_CSS_PROPERTIES)
     whitelist_protocols = markdownify_settings.get('WHITELIST_PROTOCOLS', bleach.sanitizer.ALLOWED_PROTOCOLS)
 
     # Markdown settings
     strip = markdownify_settings.get('STRIP', True)
     extensions = markdownify_settings.get('MARKDOWN_EXTENSIONS', [])
     extension_configs = markdownify_settings.get('MARKDOWN_EXTENSION_CONFIGS', {})
```

### Comparing `django_markdownify-0.9.4/markdownify/tests/input_text_default.md` & `django_markdownify-0.9.5/markdownify/tests/input_text_default.md`

 * *Files identical despite different names*

### Comparing `django_markdownify-0.9.4/markdownify/tests/test_markdownify.py` & `django_markdownify-0.9.5/markdownify/tests/test_markdownify.py`

 * *Files identical despite different names*

### Comparing `django_markdownify-0.9.4/setup.py` & `django_markdownify-0.9.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 README = open(os.path.join(os.path.dirname(__file__), 'README.md')).read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-markdownify',
-    version='0.9.4',
+    version='0.9.5',
     packages=['markdownify'],
     package_dir={'markdownify': 'markdownify'},
     package_data={'markdownify': ['tests/*.md']},
     include_package_data=True,
     license='MIT',
     description='Markdown template filter for Django.',
     long_description=README,
     long_description_content_type="text/markdown",
     url='https://github.com/erwinmatijsen/django-markdownify',
-    download_url='https://github.com/erwinmatijsen/django-markdownify/archive/0.9.4.tar.gz',
+    download_url='https://github.com/erwinmatijsen/django-markdownify/archive/0.9.5.tar.gz',
     author='Erwin Matijsen, R Moelker',
     author_email='erwin@erwinmatijsen.nl',
     classifiers=[
         'Environment :: Web Environment',
         'Framework :: Django',
         'Intended Audience :: Developers',
         'Operating System :: OS Independent',
```

