# Comparing `tmp/django_mail_panel-4.0.3.tar.gz` & `tmp/django_mail_panel-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_mail_panel-4.0.3.tar", max compression
+gzip compressed data, was "django_mail_panel-4.0.4.tar", max compression
```

## Comparing `django_mail_panel-4.0.3.tar` & `django_mail_panel-4.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rwxr-xr-x   0        0        0      604 2016-01-09 19:57:58.000000 django_mail_panel-4.0.3/LICENSE
--rwxr-xr-x   0        0        0     4214 2022-08-10 21:05:49.976469 django_mail_panel-4.0.3/README.md
--rw-r--r--   0        0        0      445 2023-03-23 12:54:10.366764 django_mail_panel-4.0.3/mail_panel/__init__.py
--rw-r--r--   0        0        0     1804 2023-03-23 12:44:24.661308 django_mail_panel-4.0.3/mail_panel/backend.py
--rw-r--r--   0        0        0      145 2021-05-29 22:55:49.016400 django_mail_panel-4.0.3/mail_panel/conf.py
--rw-r--r--   0        0        0     2542 2022-01-02 21:13:34.104751 django_mail_panel-4.0.3/mail_panel/panels.py
--rw-r--r--   0        0        0     5747 2021-05-29 22:55:49.016742 django_mail_panel-4.0.3/mail_panel/static/debug_toolbar/mail/mail_toolbar.css
--rw-r--r--   0        0        0     5723 2021-05-29 22:55:49.016867 django_mail_panel-4.0.3/mail_panel/static/debug_toolbar/mail/toolbar.mail.js
--rw-r--r--   0        0        0      684 2021-05-29 22:55:49.016978 django_mail_panel-4.0.3/mail_panel/static/debug_toolbar/mail/trash.png
--rw-r--r--   0        0        0     1431 2021-05-29 22:55:49.017147 django_mail_panel-4.0.3/mail_panel/templates/mail_panel/message_overview.html
--rw-r--r--   0        0        0     1711 2021-05-29 22:55:49.017263 django_mail_panel-4.0.3/mail_panel/templates/mail_panel/panel.html
--rw-r--r--   0        0        0      243 2021-05-29 22:55:49.017378 django_mail_panel-4.0.3/mail_panel/templates/mail_panel/plain_text_message.html
--rw-r--r--   0        0        0      244 2021-05-29 22:55:49.017485 django_mail_panel-4.0.3/mail_panel/templates/mail_panel/raw_message.html
--rw-r--r--   0        0        0      757 2022-01-02 21:14:04.706324 django_mail_panel-4.0.3/mail_panel/urls.py
--rw-r--r--   0        0        0     1130 2021-10-01 00:56:10.680958 django_mail_panel-4.0.3/mail_panel/utils.py
--rw-r--r--   0        0        0     3491 2021-05-29 22:55:49.017806 django_mail_panel-4.0.3/mail_panel/views.py
--rw-r--r--   0        0        0     1485 2023-03-23 12:54:10.365815 django_mail_panel-4.0.3/pyproject.toml
--rw-r--r--   0        0        0     5137 1970-01-01 00:00:00.000000 django_mail_panel-4.0.3/setup.py
--rw-r--r--   0        0        0     5837 1970-01-01 00:00:00.000000 django_mail_panel-4.0.3/PKG-INFO
+-rwxr-xr-x   0        0        0      604 2016-01-09 19:57:58.000000 django_mail_panel-4.0.4/LICENSE
+-rwxr-xr-x   0        0        0     4214 2022-08-10 21:05:49.976469 django_mail_panel-4.0.4/README.md
+-rw-r--r--   0        0        0      445 2024-05-09 15:14:23.051872 django_mail_panel-4.0.4/mail_panel/__init__.py
+-rw-r--r--   0        0        0     1859 2024-05-09 15:13:13.381958 django_mail_panel-4.0.4/mail_panel/backend.py
+-rw-r--r--   0        0        0      145 2021-05-29 22:55:49.016400 django_mail_panel-4.0.4/mail_panel/conf.py
+-rw-r--r--   0        0        0     2542 2022-01-02 21:13:34.104751 django_mail_panel-4.0.4/mail_panel/panels.py
+-rw-r--r--   0        0        0     5747 2021-05-29 22:55:49.016742 django_mail_panel-4.0.4/mail_panel/static/debug_toolbar/mail/mail_toolbar.css
+-rw-r--r--   0        0        0     5723 2021-05-29 22:55:49.016867 django_mail_panel-4.0.4/mail_panel/static/debug_toolbar/mail/toolbar.mail.js
+-rw-r--r--   0        0        0      684 2021-05-29 22:55:49.016978 django_mail_panel-4.0.4/mail_panel/static/debug_toolbar/mail/trash.png
+-rw-r--r--   0        0        0     1431 2021-05-29 22:55:49.017147 django_mail_panel-4.0.4/mail_panel/templates/mail_panel/message_overview.html
+-rw-r--r--   0        0        0     1711 2021-05-29 22:55:49.017263 django_mail_panel-4.0.4/mail_panel/templates/mail_panel/panel.html
+-rw-r--r--   0        0        0      243 2021-05-29 22:55:49.017378 django_mail_panel-4.0.4/mail_panel/templates/mail_panel/plain_text_message.html
+-rw-r--r--   0        0        0      244 2021-05-29 22:55:49.017485 django_mail_panel-4.0.4/mail_panel/templates/mail_panel/raw_message.html
+-rw-r--r--   0        0        0      757 2022-01-02 21:14:04.706324 django_mail_panel-4.0.4/mail_panel/urls.py
+-rw-r--r--   0        0        0     1130 2021-10-01 00:56:10.680958 django_mail_panel-4.0.4/mail_panel/utils.py
+-rw-r--r--   0        0        0     3491 2021-05-29 22:55:49.017806 django_mail_panel-4.0.4/mail_panel/views.py
+-rw-r--r--   0        0        0     1485 2024-05-09 15:14:23.051003 django_mail_panel-4.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5137 1970-01-01 00:00:00.000000 django_mail_panel-4.0.4/setup.py
+-rw-r--r--   0        0        0     5837 1970-01-01 00:00:00.000000 django_mail_panel-4.0.4/PKG-INFO
```

### Comparing `django_mail_panel-4.0.3/LICENSE` & `django_mail_panel-4.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_mail_panel-4.0.3/README.md` & `django_mail_panel-4.0.4/README.md`

 * *Files identical despite different names*

### Comparing `django_mail_panel-4.0.3/mail_panel/backend.py` & `django_mail_panel-4.0.4/mail_panel/backend.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,23 +13,25 @@
             self.id = uuid4().get_hex()
         except AttributeError:
             self.id = uuid4().hex  # python 3
         self.date_sent = now()
         self.read = False
         message.message()  # triggers header validation
 
+        alternatives = getattr(message, "alternatives", None)
+
         super(MailToolbarBackendEmail, self).__init__(
             subject=message.subject,
             to=message.to,
             cc=message.cc,
             bcc=message.bcc,
             reply_to=message.reply_to,
             from_email=message.from_email,
             body=message.body,
-            alternatives=message.alternatives,
+            alternatives=alternatives,
             headers=message.extra_headers,
             attachments=message.attachments,
         )
 
 
 class MailToolbarBackend(EmailBackend):
     """A email backend for use during testing.
```

### Comparing `django_mail_panel-4.0.3/mail_panel/panels.py` & `django_mail_panel-4.0.4/mail_panel/panels.py`

 * *Files identical despite different names*

### Comparing `django_mail_panel-4.0.3/mail_panel/static/debug_toolbar/mail/mail_toolbar.css` & `django_mail_panel-4.0.4/mail_panel/static/debug_toolbar/mail/mail_toolbar.css`

 * *Files identical despite different names*

### Comparing `django_mail_panel-4.0.3/mail_panel/static/debug_toolbar/mail/toolbar.mail.js` & `django_mail_panel-4.0.4/mail_panel/static/debug_toolbar/mail/toolbar.mail.js`

 * *Files identical despite different names*

### Comparing `django_mail_panel-4.0.3/mail_panel/static/debug_toolbar/mail/trash.png` & `django_mail_panel-4.0.4/mail_panel/static/debug_toolbar/mail/trash.png`

 * *Files identical despite different names*

### Comparing `django_mail_panel-4.0.3/mail_panel/templates/mail_panel/message_overview.html` & `django_mail_panel-4.0.4/mail_panel/templates/mail_panel/message_overview.html`

 * *Files identical despite different names*

### Comparing `django_mail_panel-4.0.3/mail_panel/templates/mail_panel/panel.html` & `django_mail_panel-4.0.4/mail_panel/templates/mail_panel/panel.html`

 * *Files identical despite different names*

### Comparing `django_mail_panel-4.0.3/mail_panel/urls.py` & `django_mail_panel-4.0.4/mail_panel/urls.py`

 * *Files identical despite different names*

### Comparing `django_mail_panel-4.0.3/mail_panel/utils.py` & `django_mail_panel-4.0.4/mail_panel/utils.py`

 * *Files identical despite different names*

### Comparing `django_mail_panel-4.0.3/mail_panel/views.py` & `django_mail_panel-4.0.4/mail_panel/views.py`

 * *Files identical despite different names*

### Comparing `django_mail_panel-4.0.3/pyproject.toml` & `django_mail_panel-4.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-mail-panel"
-version = "4.0.3"
+version = "4.0.4"
 description = "A panel for django-debug-toolbar that allows for viewing of recently sent email."
 authors = ["Stephen Mitchell"]
 license = "Apache Software License"
 readme = "README.md"
 homepage = "https://github.com/scuml/django-mail-panel"
 repository = "https://github.com/scuml/django-mail-panel"
 keywords = ["django", "django-debug-toolbar", "mail"]
```

### Comparing `django_mail_panel-4.0.3/setup.py` & `django_mail_panel-4.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
  'mail_panel': ['static/debug_toolbar/mail/*', 'templates/mail_panel/*']}
 
 install_requires = \
 ['django-debug-toolbar>=1.0']
 
 setup_kwargs = {
     'name': 'django-mail-panel',
-    'version': '4.0.3',
+    'version': '4.0.4',
     'description': 'A panel for django-debug-toolbar that allows for viewing of recently sent email.',
     'long_description': '\n## Django Debug Toolbar - Mail Panel\n\n[![Build Status](https://secure.travis-ci.org/scuml/django-mail-panel.png?branch=master)](http://travis-ci.org/scuml/django-mail-panel)\n\n![](https://cloud.githubusercontent.com/assets/1790447/9289964/6aa7c4ba-434e-11e5-8594-3bb3efd0cd81.png)\n\n\nTesting and debugging e-mail while developing a Django app has never been pleasant.  Sending e-mail to a file-based backend requires a user to click through obtusely-named files and does not provide a way to preview rendered HTML.  Sending e-mail to a valid mailbox incurs a delay as the message is processed though a mail server, and clutters a developer\'s inbox.\n\nThe mail panel attempts to address these problems by providing a way to preview emails within the browser using [django-debug-toolbar](https://github.com/jazzband/django-debug-toolbar).\n\nThis mail panel is released under the Apache license. If you like it, please consider contributing!\n\nSpecial thanks to @ShawnMilo for the code review.\n\n\nInstallation\n============\n\nTo install the mail panel, first install this package with `pip install django-mail-panel`.  Then add the `mail_panel` app after `debug_toolbar`to the `INSTALLED_APPS` setting:\n\n```python\nINSTALLED_APPS = (\n    ...\n    \'debug_toolbar\',\n    \'mail_panel\',\n)\n```\n\nand add the panel `DEBUG_TOOLBAR_PANELS`:\n\n```python\nDEBUG_TOOLBAR_PANELS = (\n    ...\n    \'mail_panel.panels.MailToolbarPanel\',\n)\n```\n\n\nCollect static and you\'ll be good to go.\n\n```bash\n./manage.py collectstatic\n```\n\n\nConfiguration\n=============\n\nAfter installation, you now need to redirect mail to the mail toolbar.  Change your email backend to the following:\n\n```python\nEMAIL_BACKEND = \'mail_panel.backend.MailToolbarBackend\'\n```\n\n**Important:** This plugin uses Django\'s cache backend to store messages.  If you are using `DummyCache`, the mail panel will use a local memory cache, and will reset messages when the server is restarted.\n\n\n**[Optional]** \nBy default, mail toolbar stores messages for one day before removing them from cache.  You can change this with the following setting:\n\n```python\nMAIL_TOOLBAR_TTL = 86400  # 1 Day\n```\n\n**[Optional]**\nIf you use the `DEBUG_TOOLBAR_PANELS` to custom order your panels:\n\n```python\n    DEBUG_TOOLBAR_PANELS = [\n        "debug_toolbar.panels.history.HistoryPanel",\n        "debug_toolbar.panels.versions.VersionsPanel",\n        "debug_toolbar.panels.timer.TimerPanel",\n        "debug_toolbar.panels.settings.SettingsPanel",\n        "debug_toolbar.panels.headers.HeadersPanel",\n        "debug_toolbar.panels.request.RequestPanel",\n        "debug_toolbar.panels.sql.SQLPanel",\n        "debug_toolbar.panels.staticfiles.StaticFilesPanel",\n        "debug_toolbar.panels.templates.TemplatesPanel",\n        "debug_toolbar.panels.cache.CachePanel",\n        "debug_toolbar.panels.signals.SignalsPanel",\n        "debug_toolbar.panels.logging.LoggingPanel",\n        "debug_toolbar.panels.redirects.RedirectsPanel",\n        "debug_toolbar.panels.profiling.ProfilingPanel",\n        "mail_panel.panels.MailToolbarPanel",  # reposition to desired location\n    ]\n```\n\n\n\nTesting\n=======\n\nTo preview emails sent from your test suite, add the email backend override to your tests with the following:\n\n```python\nfrom django.test.utils import override_settings\n\n@override_settings(EMAIL_BACKEND=\'mail_panel.backend.MailToolbarBackend\')\ndef test_send_email(self):\n    # your code here\n```\n\n\nThe backend works similarly to the standard email backend and code should not need to be reworked when using the MailToolbarBackend.\n\n\n```python\nfrom django.core import mail\n\noriginal_outbox = len(mail.outbox)\n# Send mail ...\nassert(len(mail.outbox) == original_outbox + 1)\n```\n\nShameless Plugs\n=======\nLike Django Mail Panel?  Be sure to check out and support these other tools for Mac that will improve your workflow:\n\n**[Kubermagic](https://echodot.com/kubermagic/)** - Automate, and script away tedious kubectl commands with Kubermagic; a UI for developers, QA teams, and those starting to learn the ins-and-outs of Kubernetes.     \n\n\n**[Red](https://echodot.com/red/)** - A visual and interactive Redis client, featuring live updating keys, an interactive console, pub/sub, lua script support and much more.\n',
     'author': 'Stephen Mitchell',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/scuml/django-mail-panel',
```

### Comparing `django_mail_panel-4.0.3/PKG-INFO` & `django_mail_panel-4.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mail-panel
-Version: 4.0.3
+Version: 4.0.4
 Summary: A panel for django-debug-toolbar that allows for viewing of recently sent email.
 Home-page: https://github.com/scuml/django-mail-panel
 License: Apache Software License
 Keywords: django,django-debug-toolbar,mail
 Author: Stephen Mitchell
 Requires-Python: >=3.5,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

