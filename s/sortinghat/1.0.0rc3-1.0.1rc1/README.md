# Comparing `tmp/sortinghat-1.0.0rc3.tar.gz` & `tmp/sortinghat-1.0.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sortinghat-1.0.0rc3.tar", max compression
+gzip compressed data, was "sortinghat-1.0.1rc1.tar", max compression
```

## Comparing `sortinghat-1.0.0rc3.tar` & `sortinghat-1.0.1rc1.tar`

### file list

```diff
@@ -1,205 +1,205 @@
--rw-r--r--   0        0        0      431 2024-04-12 14:43:30.535004 sortinghat-1.0.0rc3/AUTHORS
--rw-r--r--   0        0        0    35147 2024-04-12 14:43:30.535004 sortinghat-1.0.0rc3/LICENSE
--rw-r--r--   0        0        0    27792 2024-04-12 14:43:30.535004 sortinghat-1.0.0rc3/NEWS
--rw-r--r--   0        0        0     9640 2024-04-12 14:43:30.535004 sortinghat-1.0.0rc3/README.md
--rw-r--r--   0        0        0     2149 2024-04-12 14:43:30.539003 sortinghat-1.0.0rc3/pyproject.toml
--rw-r--r--   0        0        0       91 2024-04-12 14:43:30.539003 sortinghat-1.0.0rc3/sortinghat/_version.py
--rw-r--r--   0        0        0        0 2024-04-12 14:43:30.539003 sortinghat-1.0.0rc3/sortinghat/app/__init__.py
--rw-r--r--   0        0        0     1250 2024-04-12 14:43:30.539003 sortinghat-1.0.0rc3/sortinghat/app/schema.py
--rw-r--r--   0        0        0      647 2024-04-12 14:43:30.539003 sortinghat-1.0.0rc3/sortinghat/app/urls.py
--rw-r--r--   0        0        0      196 2024-04-12 14:43:30.539003 sortinghat-1.0.0rc3/sortinghat/app/wsgi.py
--rw-r--r--   0        0        0        0 2024-04-12 14:43:30.539003 sortinghat-1.0.0rc3/sortinghat/cli/__init__.py
--rw-r--r--   0        0        0      977 2024-04-12 14:43:30.539003 sortinghat-1.0.0rc3/sortinghat/cli/client/__init__.py
--rw-r--r--   0        0        0     5411 2024-04-12 14:43:30.539003 sortinghat-1.0.0rc3/sortinghat/cli/client/client.py
--rw-r--r--   0        0        0    43408 2024-04-12 14:43:30.539003 sortinghat-1.0.0rc3/sortinghat/cli/client/schema.py
--rw-r--r--   0        0        0        0 2024-04-12 14:43:30.539003 sortinghat-1.0.0rc3/sortinghat/cli/cmds/__init__.py
--rw-r--r--   0        0        0     3072 2024-04-12 14:43:30.539003 sortinghat-1.0.0rc3/sortinghat/cli/cmds/add.py
--rw-r--r--   0        0        0     6145 2024-04-12 14:43:30.539003 sortinghat-1.0.0rc3/sortinghat/cli/cmds/config.py
--rw-r--r--   0        0        0     3219 2024-04-12 14:43:30.539003 sortinghat-1.0.0rc3/sortinghat/cli/cmds/countries.py
--rw-r--r--   0        0        0     3462 2024-04-12 14:43:30.539003 sortinghat-1.0.0rc3/sortinghat/cli/cmds/enroll.py
--rw-r--r--   0        0        0     2860 2024-04-12 14:43:30.539003 sortinghat-1.0.0rc3/sortinghat/cli/cmds/lock.py
--rw-r--r--   0        0        0     2342 2024-04-12 14:43:30.539003 sortinghat-1.0.0rc3/sortinghat/cli/cmds/merge.py
--rw-r--r--   0        0        0     2352 2024-04-12 14:43:30.539003 sortinghat-1.0.0rc3/sortinghat/cli/cmds/mv.py
--rw-r--r--   0        0        0     7466 2024-04-12 14:43:30.539003 sortinghat-1.0.0rc3/sortinghat/cli/cmds/orgs.py
--rw-r--r--   0        0        0     2934 2024-04-12 14:43:30.539003 sortinghat-1.0.0rc3/sortinghat/cli/cmds/profile.py
--rw-r--r--   0        0        0     1992 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/cli/cmds/rm.py
--rw-r--r--   0        0        0     2909 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/cli/cmds/show.py
--rw-r--r--   0        0        0     2365 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/cli/cmds/split.py
--rw-r--r--   0        0        0     3364 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/cli/cmds/withdraw.py
--rwxr-xr-x   0        0        0     2857 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/cli/sortinghat.py
--rw-r--r--   0        0        0       43 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/cli/templates/add.tmpl
--rw-r--r--   0        0        0       23 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/cli/templates/config.tmpl
--rw-r--r--   0        0        0       83 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/cli/templates/countries.tmpl
--rw-r--r--   0        0        0       54 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/cli/templates/lock.tmpl
--rw-r--r--   0        0        0      169 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/cli/templates/mv.tmpl
--rw-r--r--   0        0        0      208 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/cli/templates/organizations.tmpl
--rw-r--r--   0        0        0      375 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/cli/templates/profile.tmpl
--rw-r--r--   0        0        0      106 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/cli/templates/rm.tmpl
--rw-r--r--   0        0        0     1016 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/cli/templates/show.tmpl
--rw-r--r--   0        0        0       69 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/cli/templates/split.tmpl
--rw-r--r--   0        0        0     4856 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/cli/utils.py
--rw-r--r--   0        0        0        0 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/config/__init__.py
--rw-r--r--   0        0        0    10011 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/config/settings.py
--rw-r--r--   0        0        0       20 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/config/tenants.json
--rw-r--r--   0        0        0     1544 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/admin.py
--rw-r--r--   0        0        0    58676 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/api.py
--rw-r--r--   0        0        0      926 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/apps.py
--rw-r--r--   0        0        0     5169 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/aux.py
--rw-r--r--   0        0        0      997 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/context.py
--rw-r--r--   0        0        0    43214 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/db.py
--rw-r--r--   0        0        0     4700 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/decorators.py
--rw-r--r--   0        0        0     4006 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/errors.py
--rw-r--r--   0        0        0    41236 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/fixtures/countries.json
--rw-r--r--   0        0        0     7820 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/importer/backend.py
--rw-r--r--   0        0        0    13977 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/importer/backends/gitdm.py
--rw-r--r--   0        0        0     7136 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/importer/backends/mailmap.py
--rw-r--r--   0        0        0     3628 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/importer/base.py
--rw-r--r--   0        0        0     2143 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/importer/models.py
--rw-r--r--   0        0        0     2059 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/importer/utils.py
--rw-r--r--   0        0        0    33234 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/jobs.py
--rw-r--r--   0        0        0     7298 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/log.py
--rw-r--r--   0        0        0        0 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/management/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/management/commands/__init__.py
--rw-r--r--   0        0        0     4155 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/management/commands/create_groups.py
--rw-r--r--   0        0        0     4372 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/middleware.py
--rw-r--r--   0        0        0    14033 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/migrations/0001_sortinghat.py
--rw-r--r--   0        0        0     1717 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/migrations/0002_importidentitiestask.py
--rw-r--r--   0        0        0     1502 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/migrations/0003_multi_tenancy.py
--rw-r--r--   0        0        0      582 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/migrations/0004_tenant_using_header.py
--rw-r--r--   0        0        0     1597 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/migrations/0005_scheduledtask.py
--rw-r--r--   0        0        0     1117 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/migrations/0006_unify_scheduled_tasks.py
--rw-r--r--   0        0        0      310 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/migrations/0007_delete_importidentitiestask.py
--rw-r--r--   0        0        0     1245 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/migrations/0008_alias.py
--rw-r--r--   0        0        0        0 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/migrations/__init__.py
--rw-r--r--   0        0        0    12140 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/models.py
--rw-r--r--   0        0        0      839 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/recommendations/__init__.py
--rw-r--r--   0        0        0     5219 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/recommendations/affiliation.py
--rw-r--r--   0        0        0     3151 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/recommendations/engine.py
--rw-r--r--   0        0        0     5313 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/recommendations/exclusion.py
--rw-r--r--   0        0        0     5657 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/recommendations/gender.py
--rw-r--r--   0        0        0     9792 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/recommendations/matching.py
--rw-r--r--   0        0        0    80917 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/schema.py
--rw-r--r--   0        0        0      893 2024-04-12 14:44:35.507217 sortinghat-1.0.0rc3/sortinghat/core/static/css/105.858cd75e.css
--rw-r--r--   0        0        0    16227 2024-04-12 14:44:35.495217 sortinghat-1.0.0rc3/sortinghat/core/static/css/119.87ef3a04.css
--rw-r--r--   0        0        0    16726 2024-04-12 14:44:35.515217 sortinghat-1.0.0rc3/sortinghat/core/static/css/206.7bb5d056.css
--rw-r--r--   0        0        0       71 2024-04-12 14:44:35.507217 sortinghat-1.0.0rc3/sortinghat/core/static/css/253.193dbe55.css
--rw-r--r--   0        0        0     6900 2024-04-12 14:44:35.507217 sortinghat-1.0.0rc3/sortinghat/core/static/css/488.19ce97b1.css
--rw-r--r--   0        0        0     5954 2024-04-12 14:44:35.507217 sortinghat-1.0.0rc3/sortinghat/core/static/css/546.696b6ba4.css
--rw-r--r--   0        0        0    10467 2024-04-12 14:44:35.507217 sortinghat-1.0.0rc3/sortinghat/core/static/css/764.ddc4524e.css
--rw-r--r--   0        0        0     6252 2024-04-12 14:44:35.495217 sortinghat-1.0.0rc3/sortinghat/core/static/css/812.39b5238d.css
--rw-r--r--   0        0        0    25071 2024-04-12 14:44:35.507217 sortinghat-1.0.0rc3/sortinghat/core/static/css/912.a5e49ce0.css
--rw-r--r--   0        0        0     5368 2024-04-12 14:44:35.495217 sortinghat-1.0.0rc3/sortinghat/core/static/css/app.1adeaa19.css
--rw-r--r--   0        0        0   698806 2024-04-12 14:44:35.507217 sortinghat-1.0.0rc3/sortinghat/core/static/css/chunk-vendors.42fea764.css
--rw-r--r--   0        0        0    15086 2024-04-12 14:44:35.511217 sortinghat-1.0.0rc3/sortinghat/core/static/favicon-grimoirelab.ico
--rw-r--r--   0        0        0    99428 2024-04-12 14:44:35.487217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Italic.76b8308b.woff
--rw-r--r--   0        0        0   173516 2024-04-12 14:44:35.487217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Italic.991def81.ttf
--rw-r--r--   0        0        0    30612 2024-04-12 14:44:35.487217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Italic.ca10c790.woff2
--rw-r--r--   0        0        0    93472 2024-04-12 14:44:35.483217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Light.2d3c72a3.woff
--rw-r--r--   0        0        0    65564 2024-04-12 14:44:35.483217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Light.41cb61ed.woff2
--rw-r--r--   0        0        0   170012 2024-04-12 14:44:35.483217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Light.f2e7274e.ttf
--rw-r--r--   0        0        0    72036 2024-04-12 14:44:35.483217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-LightItalic.07369d23.woff2
--rw-r--r--   0        0        0   101120 2024-04-12 14:44:35.483217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-LightItalic.45582c0c.woff
--rw-r--r--   0        0        0   176184 2024-04-12 14:44:35.483217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-LightItalic.b694f0fe.ttf
--rw-r--r--   0        0        0    50224 2024-04-12 14:44:35.487217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Medium.0519ad6f.woff2
--rw-r--r--   0        0        0    94364 2024-04-12 14:44:35.487217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Medium.483a3bd1.woff
--rw-r--r--   0        0        0   171656 2024-04-12 14:44:35.487217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Medium.af9d0139.ttf
--rw-r--r--   0        0        0   176428 2024-04-12 14:44:35.491217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-MediumItalic.3723a2e7.ttf
--rw-r--r--   0        0        0   101008 2024-04-12 14:44:35.491217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-MediumItalic.8b19cc18.woff
--rw-r--r--   0        0        0   139529 2024-04-12 14:44:35.491217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-MediumItalic.b35d3641.woff2
--rw-r--r--   0        0        0    93784 2024-04-12 14:44:35.487217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Regular.36d4503d.woff
--rw-r--r--   0        0        0   171272 2024-04-12 14:44:35.487217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Regular.ae3a8db9.ttf
--rw-r--r--   0        0        0    66012 2024-04-12 14:44:35.483217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Regular.e0553e00.woff2
--rw-r--r--   0        0        0  1026176 2024-04-12 14:44:35.495217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/materialdesignicons-webfont.21f691f0.ttf
--rw-r--r--   0        0        0   325244 2024-04-12 14:44:35.495217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/materialdesignicons-webfont.54b0f60d.woff2
--rw-r--r--   0        0        0  1026396 2024-04-12 14:44:35.491217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/materialdesignicons-webfont.5d875350.eot
--rw-r--r--   0        0        0   465188 2024-04-12 14:44:35.495217 sortinghat-1.0.0rc3/sortinghat/core/static/fonts/materialdesignicons-webfont.d671cbf6.woff
--rw-r--r--   0        0        0    13357 2024-04-12 14:44:35.507217 sortinghat-1.0.0rc3/sortinghat/core/static/js/105.2c5bfa40.js
--rw-r--r--   0        0        0    30516 2024-04-12 14:44:35.515217 sortinghat-1.0.0rc3/sortinghat/core/static/js/105.2c5bfa40.js.map
--rw-r--r--   0        0        0    66424 2024-04-12 14:44:35.495217 sortinghat-1.0.0rc3/sortinghat/core/static/js/119.6bdc5ff2.js
--rw-r--r--   0        0        0   154025 2024-04-12 14:44:35.515217 sortinghat-1.0.0rc3/sortinghat/core/static/js/119.6bdc5ff2.js.map
--rw-r--r--   0        0        0    54509 2024-04-12 14:44:35.515217 sortinghat-1.0.0rc3/sortinghat/core/static/js/206.75232ba8.js
--rw-r--r--   0        0        0   131975 2024-04-12 14:44:35.543217 sortinghat-1.0.0rc3/sortinghat/core/static/js/206.75232ba8.js.map
--rw-r--r--   0        0        0     1900 2024-04-12 14:44:35.507217 sortinghat-1.0.0rc3/sortinghat/core/static/js/253.61ce8eec.js
--rw-r--r--   0        0        0     4676 2024-04-12 14:44:35.515217 sortinghat-1.0.0rc3/sortinghat/core/static/js/253.61ce8eec.js.map
--rw-r--r--   0        0        0     2783 2024-04-12 14:44:35.495217 sortinghat-1.0.0rc3/sortinghat/core/static/js/414.13cae85b.js
--rw-r--r--   0        0        0     6249 2024-04-12 14:44:35.515217 sortinghat-1.0.0rc3/sortinghat/core/static/js/414.13cae85b.js.map
--rw-r--r--   0        0        0    23895 2024-04-12 14:44:35.507217 sortinghat-1.0.0rc3/sortinghat/core/static/js/488.0a0d2dda.js
--rw-r--r--   0        0        0    59037 2024-04-12 14:44:35.515217 sortinghat-1.0.0rc3/sortinghat/core/static/js/488.0a0d2dda.js.map
--rw-r--r--   0        0        0     7069 2024-04-12 14:44:35.507217 sortinghat-1.0.0rc3/sortinghat/core/static/js/544.b1834368.js
--rw-r--r--   0        0        0    13923 2024-04-12 14:44:35.515217 sortinghat-1.0.0rc3/sortinghat/core/static/js/544.b1834368.js.map
--rw-r--r--   0        0        0    12841 2024-04-12 14:44:35.507217 sortinghat-1.0.0rc3/sortinghat/core/static/js/546.718bab60.js
--rw-r--r--   0        0        0    29507 2024-04-12 14:44:35.515217 sortinghat-1.0.0rc3/sortinghat/core/static/js/546.718bab60.js.map
--rw-r--r--   0        0        0    50765 2024-04-12 14:44:35.507217 sortinghat-1.0.0rc3/sortinghat/core/static/js/689.e598fac2.js
--rw-r--r--   0        0        0   167791 2024-04-12 14:44:35.543217 sortinghat-1.0.0rc3/sortinghat/core/static/js/689.e598fac2.js.map
--rw-r--r--   0        0        0    14356 2024-04-12 14:44:35.507217 sortinghat-1.0.0rc3/sortinghat/core/static/js/764.5fe45faf.js
--rw-r--r--   0        0        0    31925 2024-04-12 14:44:35.515217 sortinghat-1.0.0rc3/sortinghat/core/static/js/764.5fe45faf.js.map
--rw-r--r--   0        0        0    23708 2024-04-12 14:44:35.495217 sortinghat-1.0.0rc3/sortinghat/core/static/js/812.711cab61.js
--rw-r--r--   0        0        0    54522 2024-04-12 14:44:35.515217 sortinghat-1.0.0rc3/sortinghat/core/static/js/812.711cab61.js.map
--rw-r--r--   0        0        0     3680 2024-04-12 14:44:35.495217 sortinghat-1.0.0rc3/sortinghat/core/static/js/858.8246391b.js
--rw-r--r--   0        0        0     7696 2024-04-12 14:44:35.515217 sortinghat-1.0.0rc3/sortinghat/core/static/js/858.8246391b.js.map
--rw-r--r--   0        0        0    58642 2024-04-12 14:44:35.515217 sortinghat-1.0.0rc3/sortinghat/core/static/js/912.ddb83f31.js
--rw-r--r--   0        0        0   156277 2024-04-12 14:44:35.543217 sortinghat-1.0.0rc3/sortinghat/core/static/js/912.ddb83f31.js.map
--rw-r--r--   0        0        0    14541 2024-04-12 14:44:35.495217 sortinghat-1.0.0rc3/sortinghat/core/static/js/app.014c6257.js
--rw-r--r--   0        0        0    47793 2024-04-12 14:44:35.515217 sortinghat-1.0.0rc3/sortinghat/core/static/js/app.014c6257.js.map
--rw-r--r--   0        0        0   922197 2024-04-12 14:44:35.507217 sortinghat-1.0.0rc3/sortinghat/core/static/js/chunk-vendors.dba6d507.js
--rw-r--r--   0        0        0  4116361 2024-04-12 14:44:35.535217 sortinghat-1.0.0rc3/sortinghat/core/static/js/chunk-vendors.dba6d507.js.map
--rw-r--r--   0        0        0      867 2024-04-12 14:44:35.543217 sortinghat-1.0.0rc3/sortinghat/core/templates/index.html
--rw-r--r--   0        0        0     2436 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/tenant.py
--rw-r--r--   0        0        0     3881 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/core/views.py
--rw-r--r--   0        0        0        0 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/server/__init__.py
--rw-r--r--   0        0        0    13717 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/server/sortinghat_admin.py
--rw-r--r--   0        0        0     3062 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/server/sortinghatd.py
--rw-r--r--   0        0        0     2365 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/server/sortinghatw.py
--rwxr-xr-x   0        0        0     9218 2024-04-12 14:43:30.543003 sortinghat-1.0.0rc3/sortinghat/server/utils/create_sh_0_7_fixture.py
--rw-r--r--   0        0        0     3485 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/sortinghat/utils/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/cli/__init__.py
--rw-r--r--   0        0        0       57 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/cli/config_file.cfg
--rw-r--r--   0        0        0     7601 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/cli/test_cmd_add.py
--rw-r--r--   0        0        0    17698 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/cli/test_cmd_config.py
--rw-r--r--   0        0        0    10234 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/cli/test_cmd_countries.py
--rw-r--r--   0        0        0     7597 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/cli/test_cmd_enroll.py
--rw-r--r--   0        0        0     5397 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/cli/test_cmd_lock.py
--rw-r--r--   0        0        0     3851 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/cli/test_cmd_merge.py
--rw-r--r--   0        0        0     5041 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/cli/test_cmd_mv.py
--rw-r--r--   0        0        0    13658 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/cli/test_cmd_orgs.py
--rw-r--r--   0        0        0     9117 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/cli/test_cmd_profile.py
--rw-r--r--   0        0        0     4599 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/cli/test_cmd_rm.py
--rw-r--r--   0        0        0    10993 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/cli/test_cmd_show.py
--rw-r--r--   0        0        0     5280 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/cli/test_cmd_split.py
--rw-r--r--   0        0        0     6294 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/cli/test_cmd_withdraw.py
--rw-r--r--   0        0        0        0 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/importer/__init__.py
--rw-r--r--   0        0        0      159 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/importer/data/gitdm/gitdm_email_aliases_valid.txt
--rw-r--r--   0        0        0      244 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/importer/data/gitdm/gitdm_email_to_employer_invalid.txt
--rw-r--r--   0        0        0      249 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/importer/data/gitdm/gitdm_email_to_employer_valid.txt
--rw-r--r--   0        0        0        0 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/importer/mocked_package/__init__.py
--rw-r--r--   0        0        0     1055 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/importer/mocked_package/backend_a.py
--rw-r--r--   0        0        0        0 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/importer/mocked_package/nested_package/__init__.py
--rw-r--r--   0        0        0      950 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/importer/mocked_package/nested_package/nested_backend_b.py
--rw-r--r--   0        0        0     1050 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/importer/mocked_package/nested_package/nested_backend_c.py
--rw-r--r--   0        0        0      865 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/importer/mocked_package/nested_package/nested_not_backend.py
--rw-r--r--   0        0        0     4797 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/importer/test_backend.py
--rw-r--r--   0        0        0    25058 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/importer/test_gitdm.py
--rw-r--r--   0        0        0     2416 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/importer/test_utils.py
--rw-r--r--   0        0        0        0 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/rec/__init__.py
--rw-r--r--   0        0        0    10028 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/rec/test_affiliations.py
--rw-r--r--   0        0        0     2925 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/rec/test_engine.py
--rw-r--r--   0        0        0     3937 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/rec/test_exclusion.py
--rw-r--r--   0        0        0     9040 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/rec/test_gender.py
--rw-r--r--   0        0        0    21600 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/rec/test_matches.py
--rw-r--r--   0        0        0      825 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/runners.py
--rw-r--r--   0        0        0        0 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/tenants/__init__.py
--rw-r--r--   0        0        0     7242 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/tenants/test_jobs.py
--rw-r--r--   0        0        0     2277 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/tenants/test_middleware.py
--rw-r--r--   0        0        0     5872 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/tenants/test_schema.py
--rw-r--r--   0        0        0   287020 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/test_api.py
--rw-r--r--   0        0        0    18365 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/test_aux.py
--rw-r--r--   0        0        0     9779 2024-04-12 14:43:30.547003 sortinghat-1.0.0rc3/tests/test_client.py
--rw-r--r--   0        0        0   135031 2024-04-12 14:43:30.551004 sortinghat-1.0.0rc3/tests/test_db.py
--rw-r--r--   0        0        0     9785 2024-04-12 14:43:30.551004 sortinghat-1.0.0rc3/tests/test_errors.py
--rw-r--r--   0        0        0    72127 2024-04-12 14:43:30.551004 sortinghat-1.0.0rc3/tests/test_jobs.py
--rw-r--r--   0        0        0    14074 2024-04-12 14:43:30.551004 sortinghat-1.0.0rc3/tests/test_log.py
--rw-r--r--   0        0        0    48532 2024-04-12 14:43:30.551004 sortinghat-1.0.0rc3/tests/test_model.py
--rw-r--r--   0        0        0   430482 2024-04-12 14:43:30.551004 sortinghat-1.0.0rc3/tests/test_schema.py
--rw-r--r--   0        0        0     6316 2024-04-12 14:43:30.551004 sortinghat-1.0.0rc3/tests/test_utils.py
--rw-r--r--   0        0        0    11519 1970-01-01 00:00:00.000000 sortinghat-1.0.0rc3/PKG-INFO
+-rw-r--r--   0        0        0      431 2024-05-09 07:57:57.357551 sortinghat-1.0.1rc1/AUTHORS
+-rw-r--r--   0        0        0    35147 2024-05-09 07:57:57.357551 sortinghat-1.0.1rc1/LICENSE
+-rw-r--r--   0        0        0    28400 2024-05-09 07:57:57.357551 sortinghat-1.0.1rc1/NEWS
+-rw-r--r--   0        0        0     9655 2024-05-09 07:57:57.357551 sortinghat-1.0.1rc1/README.md
+-rw-r--r--   0        0        0     2149 2024-05-09 07:57:57.361551 sortinghat-1.0.1rc1/pyproject.toml
+-rw-r--r--   0        0        0       91 2024-05-09 07:57:57.361551 sortinghat-1.0.1rc1/sortinghat/_version.py
+-rw-r--r--   0        0        0        0 2024-05-09 07:57:57.361551 sortinghat-1.0.1rc1/sortinghat/app/__init__.py
+-rw-r--r--   0        0        0     1250 2024-05-09 07:57:57.361551 sortinghat-1.0.1rc1/sortinghat/app/schema.py
+-rw-r--r--   0        0        0      647 2024-05-09 07:57:57.361551 sortinghat-1.0.1rc1/sortinghat/app/urls.py
+-rw-r--r--   0        0        0      196 2024-05-09 07:57:57.361551 sortinghat-1.0.1rc1/sortinghat/app/wsgi.py
+-rw-r--r--   0        0        0        0 2024-05-09 07:57:57.361551 sortinghat-1.0.1rc1/sortinghat/cli/__init__.py
+-rw-r--r--   0        0        0      977 2024-05-09 07:57:57.361551 sortinghat-1.0.1rc1/sortinghat/cli/client/__init__.py
+-rw-r--r--   0        0        0     5411 2024-05-09 07:57:57.361551 sortinghat-1.0.1rc1/sortinghat/cli/client/client.py
+-rw-r--r--   0        0        0    43408 2024-05-09 07:57:57.361551 sortinghat-1.0.1rc1/sortinghat/cli/client/schema.py
+-rw-r--r--   0        0        0        0 2024-05-09 07:57:57.361551 sortinghat-1.0.1rc1/sortinghat/cli/cmds/__init__.py
+-rw-r--r--   0        0        0     3072 2024-05-09 07:57:57.361551 sortinghat-1.0.1rc1/sortinghat/cli/cmds/add.py
+-rw-r--r--   0        0        0     6145 2024-05-09 07:57:57.361551 sortinghat-1.0.1rc1/sortinghat/cli/cmds/config.py
+-rw-r--r--   0        0        0     3219 2024-05-09 07:57:57.361551 sortinghat-1.0.1rc1/sortinghat/cli/cmds/countries.py
+-rw-r--r--   0        0        0     3462 2024-05-09 07:57:57.361551 sortinghat-1.0.1rc1/sortinghat/cli/cmds/enroll.py
+-rw-r--r--   0        0        0     2860 2024-05-09 07:57:57.361551 sortinghat-1.0.1rc1/sortinghat/cli/cmds/lock.py
+-rw-r--r--   0        0        0     2342 2024-05-09 07:57:57.361551 sortinghat-1.0.1rc1/sortinghat/cli/cmds/merge.py
+-rw-r--r--   0        0        0     2352 2024-05-09 07:57:57.361551 sortinghat-1.0.1rc1/sortinghat/cli/cmds/mv.py
+-rw-r--r--   0        0        0     7466 2024-05-09 07:57:57.361551 sortinghat-1.0.1rc1/sortinghat/cli/cmds/orgs.py
+-rw-r--r--   0        0        0     2934 2024-05-09 07:57:57.361551 sortinghat-1.0.1rc1/sortinghat/cli/cmds/profile.py
+-rw-r--r--   0        0        0     1992 2024-05-09 07:57:57.361551 sortinghat-1.0.1rc1/sortinghat/cli/cmds/rm.py
+-rw-r--r--   0        0        0     2909 2024-05-09 07:57:57.361551 sortinghat-1.0.1rc1/sortinghat/cli/cmds/show.py
+-rw-r--r--   0        0        0     2365 2024-05-09 07:57:57.361551 sortinghat-1.0.1rc1/sortinghat/cli/cmds/split.py
+-rw-r--r--   0        0        0     3364 2024-05-09 07:57:57.361551 sortinghat-1.0.1rc1/sortinghat/cli/cmds/withdraw.py
+-rwxr-xr-x   0        0        0     2857 2024-05-09 07:57:57.361551 sortinghat-1.0.1rc1/sortinghat/cli/sortinghat.py
+-rw-r--r--   0        0        0       43 2024-05-09 07:57:57.361551 sortinghat-1.0.1rc1/sortinghat/cli/templates/add.tmpl
+-rw-r--r--   0        0        0       23 2024-05-09 07:57:57.361551 sortinghat-1.0.1rc1/sortinghat/cli/templates/config.tmpl
+-rw-r--r--   0        0        0       83 2024-05-09 07:57:57.361551 sortinghat-1.0.1rc1/sortinghat/cli/templates/countries.tmpl
+-rw-r--r--   0        0        0       54 2024-05-09 07:57:57.361551 sortinghat-1.0.1rc1/sortinghat/cli/templates/lock.tmpl
+-rw-r--r--   0        0        0      169 2024-05-09 07:57:57.361551 sortinghat-1.0.1rc1/sortinghat/cli/templates/mv.tmpl
+-rw-r--r--   0        0        0      208 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/cli/templates/organizations.tmpl
+-rw-r--r--   0        0        0      375 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/cli/templates/profile.tmpl
+-rw-r--r--   0        0        0      106 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/cli/templates/rm.tmpl
+-rw-r--r--   0        0        0     1016 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/cli/templates/show.tmpl
+-rw-r--r--   0        0        0       69 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/cli/templates/split.tmpl
+-rw-r--r--   0        0        0     4856 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/cli/utils.py
+-rw-r--r--   0        0        0        0 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/config/__init__.py
+-rw-r--r--   0        0        0    10011 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/config/settings.py
+-rw-r--r--   0        0        0       20 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/config/tenants.json
+-rw-r--r--   0        0        0     1544 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/core/admin.py
+-rw-r--r--   0        0        0    58676 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/core/api.py
+-rw-r--r--   0        0        0      926 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/core/apps.py
+-rw-r--r--   0        0        0     5169 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/core/aux.py
+-rw-r--r--   0        0        0      997 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/core/context.py
+-rw-r--r--   0        0        0    43214 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/core/db.py
+-rw-r--r--   0        0        0     4700 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/core/decorators.py
+-rw-r--r--   0        0        0     4006 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/core/errors.py
+-rw-r--r--   0        0        0    41236 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/core/fixtures/countries.json
+-rw-r--r--   0        0        0     7820 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/core/importer/backend.py
+-rw-r--r--   0        0        0    13977 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/core/importer/backends/gitdm.py
+-rw-r--r--   0        0        0     7136 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/core/importer/backends/mailmap.py
+-rw-r--r--   0        0        0     3628 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/core/importer/base.py
+-rw-r--r--   0        0        0     2143 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/core/importer/models.py
+-rw-r--r--   0        0        0     2059 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/core/importer/utils.py
+-rw-r--r--   0        0        0    33234 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/core/jobs.py
+-rw-r--r--   0        0        0     7298 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/core/log.py
+-rw-r--r--   0        0        0        0 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/core/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/core/management/commands/__init__.py
+-rw-r--r--   0        0        0     4155 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/core/management/commands/create_groups.py
+-rw-r--r--   0        0        0     4372 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/core/middleware.py
+-rw-r--r--   0        0        0    14033 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/core/migrations/0001_sortinghat.py
+-rw-r--r--   0        0        0     1717 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/core/migrations/0002_importidentitiestask.py
+-rw-r--r--   0        0        0     1502 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/core/migrations/0003_multi_tenancy.py
+-rw-r--r--   0        0        0      582 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/core/migrations/0004_tenant_using_header.py
+-rw-r--r--   0        0        0     1597 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/core/migrations/0005_scheduledtask.py
+-rw-r--r--   0        0        0     1117 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/core/migrations/0006_unify_scheduled_tasks.py
+-rw-r--r--   0        0        0      310 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/core/migrations/0007_delete_importidentitiestask.py
+-rw-r--r--   0        0        0     1245 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/core/migrations/0008_alias.py
+-rw-r--r--   0        0        0        0 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/core/migrations/__init__.py
+-rw-r--r--   0        0        0    12140 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/core/models.py
+-rw-r--r--   0        0        0      839 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/core/recommendations/__init__.py
+-rw-r--r--   0        0        0     5219 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/core/recommendations/affiliation.py
+-rw-r--r--   0        0        0     3151 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/core/recommendations/engine.py
+-rw-r--r--   0        0        0     5313 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/core/recommendations/exclusion.py
+-rw-r--r--   0        0        0     5657 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/core/recommendations/gender.py
+-rw-r--r--   0        0        0     9792 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/core/recommendations/matching.py
+-rw-r--r--   0        0        0    81170 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/core/schema.py
+-rw-r--r--   0        0        0      893 2024-05-09 07:59:01.025792 sortinghat-1.0.1rc1/sortinghat/core/static/css/105.858cd75e.css
+-rw-r--r--   0        0        0    16227 2024-05-09 07:59:01.005792 sortinghat-1.0.1rc1/sortinghat/core/static/css/119.87ef3a04.css
+-rw-r--r--   0        0        0    16726 2024-05-09 07:59:01.025792 sortinghat-1.0.1rc1/sortinghat/core/static/css/206.7bb5d056.css
+-rw-r--r--   0        0        0       71 2024-05-09 07:59:01.025792 sortinghat-1.0.1rc1/sortinghat/core/static/css/253.193dbe55.css
+-rw-r--r--   0        0        0     6900 2024-05-09 07:59:01.025792 sortinghat-1.0.1rc1/sortinghat/core/static/css/488.19ce97b1.css
+-rw-r--r--   0        0        0     5954 2024-05-09 07:59:01.025792 sortinghat-1.0.1rc1/sortinghat/core/static/css/546.696b6ba4.css
+-rw-r--r--   0        0        0    10467 2024-05-09 07:59:01.025792 sortinghat-1.0.1rc1/sortinghat/core/static/css/764.ddc4524e.css
+-rw-r--r--   0        0        0     6252 2024-05-09 07:59:01.005792 sortinghat-1.0.1rc1/sortinghat/core/static/css/812.39b5238d.css
+-rw-r--r--   0        0        0    25071 2024-05-09 07:59:01.025792 sortinghat-1.0.1rc1/sortinghat/core/static/css/912.a5e49ce0.css
+-rw-r--r--   0        0        0     5368 2024-05-09 07:59:01.005792 sortinghat-1.0.1rc1/sortinghat/core/static/css/app.1adeaa19.css
+-rw-r--r--   0        0        0   698806 2024-05-09 07:59:01.025792 sortinghat-1.0.1rc1/sortinghat/core/static/css/chunk-vendors.42fea764.css
+-rw-r--r--   0        0        0    15086 2024-05-09 07:59:01.025792 sortinghat-1.0.1rc1/sortinghat/core/static/favicon-grimoirelab.ico
+-rw-r--r--   0        0        0    99428 2024-05-09 07:59:00.989792 sortinghat-1.0.1rc1/sortinghat/core/static/fonts/Roboto-Italic.76b8308b.woff
+-rw-r--r--   0        0        0   173516 2024-05-09 07:59:00.989792 sortinghat-1.0.1rc1/sortinghat/core/static/fonts/Roboto-Italic.991def81.ttf
+-rw-r--r--   0        0        0    30612 2024-05-09 07:59:00.989792 sortinghat-1.0.1rc1/sortinghat/core/static/fonts/Roboto-Italic.ca10c790.woff2
+-rw-r--r--   0        0        0    93472 2024-05-09 07:59:00.989792 sortinghat-1.0.1rc1/sortinghat/core/static/fonts/Roboto-Light.2d3c72a3.woff
+-rw-r--r--   0        0        0    65564 2024-05-09 07:59:00.989792 sortinghat-1.0.1rc1/sortinghat/core/static/fonts/Roboto-Light.41cb61ed.woff2
+-rw-r--r--   0        0        0   170012 2024-05-09 07:59:00.989792 sortinghat-1.0.1rc1/sortinghat/core/static/fonts/Roboto-Light.f2e7274e.ttf
+-rw-r--r--   0        0        0    72036 2024-05-09 07:59:00.989792 sortinghat-1.0.1rc1/sortinghat/core/static/fonts/Roboto-LightItalic.07369d23.woff2
+-rw-r--r--   0        0        0   101120 2024-05-09 07:59:00.989792 sortinghat-1.0.1rc1/sortinghat/core/static/fonts/Roboto-LightItalic.45582c0c.woff
+-rw-r--r--   0        0        0   176184 2024-05-09 07:59:00.989792 sortinghat-1.0.1rc1/sortinghat/core/static/fonts/Roboto-LightItalic.b694f0fe.ttf
+-rw-r--r--   0        0        0    50224 2024-05-09 07:59:00.989792 sortinghat-1.0.1rc1/sortinghat/core/static/fonts/Roboto-Medium.0519ad6f.woff2
+-rw-r--r--   0        0        0    94364 2024-05-09 07:59:00.989792 sortinghat-1.0.1rc1/sortinghat/core/static/fonts/Roboto-Medium.483a3bd1.woff
+-rw-r--r--   0        0        0   171656 2024-05-09 07:59:00.989792 sortinghat-1.0.1rc1/sortinghat/core/static/fonts/Roboto-Medium.af9d0139.ttf
+-rw-r--r--   0        0        0   176428 2024-05-09 07:59:01.001793 sortinghat-1.0.1rc1/sortinghat/core/static/fonts/Roboto-MediumItalic.3723a2e7.ttf
+-rw-r--r--   0        0        0   101008 2024-05-09 07:59:01.001793 sortinghat-1.0.1rc1/sortinghat/core/static/fonts/Roboto-MediumItalic.8b19cc18.woff
+-rw-r--r--   0        0        0   139529 2024-05-09 07:59:01.001793 sortinghat-1.0.1rc1/sortinghat/core/static/fonts/Roboto-MediumItalic.b35d3641.woff2
+-rw-r--r--   0        0        0    93784 2024-05-09 07:59:00.989792 sortinghat-1.0.1rc1/sortinghat/core/static/fonts/Roboto-Regular.36d4503d.woff
+-rw-r--r--   0        0        0   171272 2024-05-09 07:59:00.989792 sortinghat-1.0.1rc1/sortinghat/core/static/fonts/Roboto-Regular.ae3a8db9.ttf
+-rw-r--r--   0        0        0    66012 2024-05-09 07:59:00.989792 sortinghat-1.0.1rc1/sortinghat/core/static/fonts/Roboto-Regular.e0553e00.woff2
+-rw-r--r--   0        0        0  1026176 2024-05-09 07:59:01.005792 sortinghat-1.0.1rc1/sortinghat/core/static/fonts/materialdesignicons-webfont.21f691f0.ttf
+-rw-r--r--   0        0        0   325244 2024-05-09 07:59:01.001793 sortinghat-1.0.1rc1/sortinghat/core/static/fonts/materialdesignicons-webfont.54b0f60d.woff2
+-rw-r--r--   0        0        0  1026396 2024-05-09 07:59:01.001793 sortinghat-1.0.1rc1/sortinghat/core/static/fonts/materialdesignicons-webfont.5d875350.eot
+-rw-r--r--   0        0        0   465188 2024-05-09 07:59:01.001793 sortinghat-1.0.1rc1/sortinghat/core/static/fonts/materialdesignicons-webfont.d671cbf6.woff
+-rw-r--r--   0        0        0    13357 2024-05-09 07:59:01.025792 sortinghat-1.0.1rc1/sortinghat/core/static/js/105.2c5bfa40.js
+-rw-r--r--   0        0        0    30516 2024-05-09 07:59:01.029793 sortinghat-1.0.1rc1/sortinghat/core/static/js/105.2c5bfa40.js.map
+-rw-r--r--   0        0        0    66424 2024-05-09 07:59:01.005792 sortinghat-1.0.1rc1/sortinghat/core/static/js/119.6bdc5ff2.js
+-rw-r--r--   0        0        0   154025 2024-05-09 07:59:01.025792 sortinghat-1.0.1rc1/sortinghat/core/static/js/119.6bdc5ff2.js.map
+-rw-r--r--   0        0        0    54509 2024-05-09 07:59:01.025792 sortinghat-1.0.1rc1/sortinghat/core/static/js/206.75232ba8.js
+-rw-r--r--   0        0        0   131975 2024-05-09 07:59:01.061793 sortinghat-1.0.1rc1/sortinghat/core/static/js/206.75232ba8.js.map
+-rw-r--r--   0        0        0     1900 2024-05-09 07:59:01.025792 sortinghat-1.0.1rc1/sortinghat/core/static/js/253.61ce8eec.js
+-rw-r--r--   0        0        0     4676 2024-05-09 07:59:01.029793 sortinghat-1.0.1rc1/sortinghat/core/static/js/253.61ce8eec.js.map
+-rw-r--r--   0        0        0     2783 2024-05-09 07:59:01.005792 sortinghat-1.0.1rc1/sortinghat/core/static/js/414.13cae85b.js
+-rw-r--r--   0        0        0     6249 2024-05-09 07:59:01.025792 sortinghat-1.0.1rc1/sortinghat/core/static/js/414.13cae85b.js.map
+-rw-r--r--   0        0        0    23895 2024-05-09 07:59:01.025792 sortinghat-1.0.1rc1/sortinghat/core/static/js/488.0a0d2dda.js
+-rw-r--r--   0        0        0    59037 2024-05-09 07:59:01.025792 sortinghat-1.0.1rc1/sortinghat/core/static/js/488.0a0d2dda.js.map
+-rw-r--r--   0        0        0     7069 2024-05-09 07:59:01.025792 sortinghat-1.0.1rc1/sortinghat/core/static/js/544.b1834368.js
+-rw-r--r--   0        0        0    13923 2024-05-09 07:59:01.025792 sortinghat-1.0.1rc1/sortinghat/core/static/js/544.b1834368.js.map
+-rw-r--r--   0        0        0    12841 2024-05-09 07:59:01.025792 sortinghat-1.0.1rc1/sortinghat/core/static/js/546.718bab60.js
+-rw-r--r--   0        0        0    29507 2024-05-09 07:59:01.029793 sortinghat-1.0.1rc1/sortinghat/core/static/js/546.718bab60.js.map
+-rw-r--r--   0        0        0    50765 2024-05-09 07:59:01.025792 sortinghat-1.0.1rc1/sortinghat/core/static/js/689.e598fac2.js
+-rw-r--r--   0        0        0   167791 2024-05-09 07:59:01.061793 sortinghat-1.0.1rc1/sortinghat/core/static/js/689.e598fac2.js.map
+-rw-r--r--   0        0        0    14356 2024-05-09 07:59:01.025792 sortinghat-1.0.1rc1/sortinghat/core/static/js/764.5fe45faf.js
+-rw-r--r--   0        0        0    31925 2024-05-09 07:59:01.029793 sortinghat-1.0.1rc1/sortinghat/core/static/js/764.5fe45faf.js.map
+-rw-r--r--   0        0        0    23708 2024-05-09 07:59:01.005792 sortinghat-1.0.1rc1/sortinghat/core/static/js/812.711cab61.js
+-rw-r--r--   0        0        0    54522 2024-05-09 07:59:01.025792 sortinghat-1.0.1rc1/sortinghat/core/static/js/812.711cab61.js.map
+-rw-r--r--   0        0        0     3680 2024-05-09 07:59:01.005792 sortinghat-1.0.1rc1/sortinghat/core/static/js/858.8246391b.js
+-rw-r--r--   0        0        0     7696 2024-05-09 07:59:01.025792 sortinghat-1.0.1rc1/sortinghat/core/static/js/858.8246391b.js.map
+-rw-r--r--   0        0        0    58642 2024-05-09 07:59:01.025792 sortinghat-1.0.1rc1/sortinghat/core/static/js/912.ddb83f31.js
+-rw-r--r--   0        0        0   156277 2024-05-09 07:59:01.061793 sortinghat-1.0.1rc1/sortinghat/core/static/js/912.ddb83f31.js.map
+-rw-r--r--   0        0        0    14541 2024-05-09 07:59:01.005792 sortinghat-1.0.1rc1/sortinghat/core/static/js/app.014c6257.js
+-rw-r--r--   0        0        0    47793 2024-05-09 07:59:01.025792 sortinghat-1.0.1rc1/sortinghat/core/static/js/app.014c6257.js.map
+-rw-r--r--   0        0        0   922197 2024-05-09 07:59:01.025792 sortinghat-1.0.1rc1/sortinghat/core/static/js/chunk-vendors.dba6d507.js
+-rw-r--r--   0        0        0  4116361 2024-05-09 07:59:01.057793 sortinghat-1.0.1rc1/sortinghat/core/static/js/chunk-vendors.dba6d507.js.map
+-rw-r--r--   0        0        0      867 2024-05-09 07:59:01.061793 sortinghat-1.0.1rc1/sortinghat/core/templates/index.html
+-rw-r--r--   0        0        0     2436 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/core/tenant.py
+-rw-r--r--   0        0        0     3881 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/core/views.py
+-rw-r--r--   0        0        0        0 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/server/__init__.py
+-rw-r--r--   0        0        0    13717 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/server/sortinghat_admin.py
+-rw-r--r--   0        0        0     3062 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/server/sortinghatd.py
+-rw-r--r--   0        0        0     2365 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/server/sortinghatw.py
+-rwxr-xr-x   0        0        0     9218 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/server/utils/create_sh_0_7_fixture.py
+-rw-r--r--   0        0        0     3485 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/sortinghat/utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/tests/cli/__init__.py
+-rw-r--r--   0        0        0       57 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/tests/cli/config_file.cfg
+-rw-r--r--   0        0        0     7601 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/tests/cli/test_cmd_add.py
+-rw-r--r--   0        0        0    17698 2024-05-09 07:57:57.365551 sortinghat-1.0.1rc1/tests/cli/test_cmd_config.py
+-rw-r--r--   0        0        0    10234 2024-05-09 07:57:57.369551 sortinghat-1.0.1rc1/tests/cli/test_cmd_countries.py
+-rw-r--r--   0        0        0     7597 2024-05-09 07:57:57.369551 sortinghat-1.0.1rc1/tests/cli/test_cmd_enroll.py
+-rw-r--r--   0        0        0     5397 2024-05-09 07:57:57.369551 sortinghat-1.0.1rc1/tests/cli/test_cmd_lock.py
+-rw-r--r--   0        0        0     3851 2024-05-09 07:57:57.369551 sortinghat-1.0.1rc1/tests/cli/test_cmd_merge.py
+-rw-r--r--   0        0        0     5041 2024-05-09 07:57:57.369551 sortinghat-1.0.1rc1/tests/cli/test_cmd_mv.py
+-rw-r--r--   0        0        0    13658 2024-05-09 07:57:57.369551 sortinghat-1.0.1rc1/tests/cli/test_cmd_orgs.py
+-rw-r--r--   0        0        0     9117 2024-05-09 07:57:57.369551 sortinghat-1.0.1rc1/tests/cli/test_cmd_profile.py
+-rw-r--r--   0        0        0     4599 2024-05-09 07:57:57.369551 sortinghat-1.0.1rc1/tests/cli/test_cmd_rm.py
+-rw-r--r--   0        0        0    10993 2024-05-09 07:57:57.369551 sortinghat-1.0.1rc1/tests/cli/test_cmd_show.py
+-rw-r--r--   0        0        0     5280 2024-05-09 07:57:57.369551 sortinghat-1.0.1rc1/tests/cli/test_cmd_split.py
+-rw-r--r--   0        0        0     6294 2024-05-09 07:57:57.369551 sortinghat-1.0.1rc1/tests/cli/test_cmd_withdraw.py
+-rw-r--r--   0        0        0        0 2024-05-09 07:57:57.369551 sortinghat-1.0.1rc1/tests/importer/__init__.py
+-rw-r--r--   0        0        0      159 2024-05-09 07:57:57.369551 sortinghat-1.0.1rc1/tests/importer/data/gitdm/gitdm_email_aliases_valid.txt
+-rw-r--r--   0        0        0      244 2024-05-09 07:57:57.369551 sortinghat-1.0.1rc1/tests/importer/data/gitdm/gitdm_email_to_employer_invalid.txt
+-rw-r--r--   0        0        0      249 2024-05-09 07:57:57.369551 sortinghat-1.0.1rc1/tests/importer/data/gitdm/gitdm_email_to_employer_valid.txt
+-rw-r--r--   0        0        0        0 2024-05-09 07:57:57.369551 sortinghat-1.0.1rc1/tests/importer/mocked_package/__init__.py
+-rw-r--r--   0        0        0     1055 2024-05-09 07:57:57.369551 sortinghat-1.0.1rc1/tests/importer/mocked_package/backend_a.py
+-rw-r--r--   0        0        0        0 2024-05-09 07:57:57.369551 sortinghat-1.0.1rc1/tests/importer/mocked_package/nested_package/__init__.py
+-rw-r--r--   0        0        0      950 2024-05-09 07:57:57.369551 sortinghat-1.0.1rc1/tests/importer/mocked_package/nested_package/nested_backend_b.py
+-rw-r--r--   0        0        0     1050 2024-05-09 07:57:57.369551 sortinghat-1.0.1rc1/tests/importer/mocked_package/nested_package/nested_backend_c.py
+-rw-r--r--   0        0        0      865 2024-05-09 07:57:57.369551 sortinghat-1.0.1rc1/tests/importer/mocked_package/nested_package/nested_not_backend.py
+-rw-r--r--   0        0        0     4797 2024-05-09 07:57:57.369551 sortinghat-1.0.1rc1/tests/importer/test_backend.py
+-rw-r--r--   0        0        0    25058 2024-05-09 07:57:57.369551 sortinghat-1.0.1rc1/tests/importer/test_gitdm.py
+-rw-r--r--   0        0        0     2416 2024-05-09 07:57:57.369551 sortinghat-1.0.1rc1/tests/importer/test_utils.py
+-rw-r--r--   0        0        0        0 2024-05-09 07:57:57.369551 sortinghat-1.0.1rc1/tests/rec/__init__.py
+-rw-r--r--   0        0        0    10028 2024-05-09 07:57:57.369551 sortinghat-1.0.1rc1/tests/rec/test_affiliations.py
+-rw-r--r--   0        0        0     2925 2024-05-09 07:57:57.369551 sortinghat-1.0.1rc1/tests/rec/test_engine.py
+-rw-r--r--   0        0        0     3937 2024-05-09 07:57:57.369551 sortinghat-1.0.1rc1/tests/rec/test_exclusion.py
+-rw-r--r--   0        0        0     9040 2024-05-09 07:57:57.369551 sortinghat-1.0.1rc1/tests/rec/test_gender.py
+-rw-r--r--   0        0        0    21600 2024-05-09 07:57:57.369551 sortinghat-1.0.1rc1/tests/rec/test_matches.py
+-rw-r--r--   0        0        0      825 2024-05-09 07:57:57.369551 sortinghat-1.0.1rc1/tests/runners.py
+-rw-r--r--   0        0        0        0 2024-05-09 07:57:57.369551 sortinghat-1.0.1rc1/tests/tenants/__init__.py
+-rw-r--r--   0        0        0     7242 2024-05-09 07:57:57.369551 sortinghat-1.0.1rc1/tests/tenants/test_jobs.py
+-rw-r--r--   0        0        0     2277 2024-05-09 07:57:57.369551 sortinghat-1.0.1rc1/tests/tenants/test_middleware.py
+-rw-r--r--   0        0        0     5872 2024-05-09 07:57:57.369551 sortinghat-1.0.1rc1/tests/tenants/test_schema.py
+-rw-r--r--   0        0        0   287020 2024-05-09 07:57:57.369551 sortinghat-1.0.1rc1/tests/test_api.py
+-rw-r--r--   0        0        0    18365 2024-05-09 07:57:57.369551 sortinghat-1.0.1rc1/tests/test_aux.py
+-rw-r--r--   0        0        0     9779 2024-05-09 07:57:57.369551 sortinghat-1.0.1rc1/tests/test_client.py
+-rw-r--r--   0        0        0   135031 2024-05-09 07:57:57.373551 sortinghat-1.0.1rc1/tests/test_db.py
+-rw-r--r--   0        0        0     9785 2024-05-09 07:57:57.373551 sortinghat-1.0.1rc1/tests/test_errors.py
+-rw-r--r--   0        0        0    72127 2024-05-09 07:57:57.373551 sortinghat-1.0.1rc1/tests/test_jobs.py
+-rw-r--r--   0        0        0    14074 2024-05-09 07:57:57.373551 sortinghat-1.0.1rc1/tests/test_log.py
+-rw-r--r--   0        0        0    48532 2024-05-09 07:57:57.373551 sortinghat-1.0.1rc1/tests/test_model.py
+-rw-r--r--   0        0        0   430482 2024-05-09 07:57:57.373551 sortinghat-1.0.1rc1/tests/test_schema.py
+-rw-r--r--   0        0        0     6316 2024-05-09 07:57:57.373551 sortinghat-1.0.1rc1/tests/test_utils.py
+-rw-r--r--   0        0        0    11534 1970-01-01 00:00:00.000000 sortinghat-1.0.1rc1/PKG-INFO
```

### Comparing `sortinghat-1.0.0rc3/LICENSE` & `sortinghat-1.0.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/NEWS` & `sortinghat-1.0.1rc1/NEWS`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,31 @@
 # Releases
 
+## sortinghat 1.0.0 - (2024-04-13)
+
+**New features:**
+
+ * First major release\
+   GrimoireLab reached a stable status. This is our first major release.
+
+**Bug fixes:**
+
+ * Change password form fixed\
+   An unused header in the UI made the attempts to change the password
+   fail. It tried to guess the user from an invalid JWT token when
+   multitenancy was enabled.
+
+**Dependencies updateds:**
+
+ * Django version updated\
+   Upgrade the Django version from 3.2 to 4.2. Support for Django 3.2
+   ended at April 1, 2024. This change ensures compability with the
+   latests features and an extended support.
+
+
 ## sortinghat 0.21.2 - (2024-03-27)
 
 **Bug fixes:**
 
  * Refetch general settings after they are changed\
    The "unify" and "affiliate" switches on the general settings page
    sometimes reflected outdated information. The page now reloads the
```

### Comparing `sortinghat-1.0.0rc3/README.md` & `sortinghat-1.0.1rc1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 In the context of GrimoireLab, Sorting Hat is usually run after data is retrieved with [Perceval](https://github.com/chaoss/grimoirelab-perceval), to store the identities obtained into its database, and later merge them into individuals (and maybe affiliate them).
 
 
 ## Requirements
 
 * Python >= 3.8
 * Poetry >= 1.1.0
-* MySQL >= 5.7 or MariaDB 10.0
+* MySQL >= 8.1 or MariaDB >= 10.4
 * Django = 4.2
 * Graphene-Django >= 2.0
 * uWSGI >= 2.0
 
 You will also need some other libraries for running the tool, you can find the
 whole list of dependencies in [pyproject.toml](pyproject.toml) file.
 
@@ -65,16 +65,16 @@
 $ apt install libmariadbclient-dev-compat
 ```
 
 #### Installation and configuration
 
 **Note**: these examples use `sortinghat.config.settings` configuration file.
 In order to use that configuration you need to define the environment variable
-`SORTINGHAT_SECRET_KEY` with a secret. More info here:
-https://docs.djangoproject.com/en/4.2/ref/settings/#std:setting-SECRET_KEY
+`SORTINGHAT_SECRET_KEY` with a secret. More info
+[here](https://docs.djangoproject.com/en/4.2/ref/settings/#std:setting-SECRET_KEY).
 
 
 Install the required dependencies (this will also create a virtual environment).
 ```
 $ poetry install
 ```
 
@@ -249,37 +249,38 @@
 - Set `MULTI_TENANT` settings to `True`.
 - Define a list of tenants using the configuration file `sortinghat/config/tenants.json`.
   You can use a different json file using the environment variable 
   `SORTINGHAT_MULTI_TENANT_LIST_PATH`. The file should have the next schema:
 
   ```json
   {
-    'tenants': [
-      {'name': 'tenant A', 'dedicated_queue': true},
-      {'name': 'tenant B', 'dedicated_queue': false}
+    "tenants": [
+      {"name": "tenant A", "dedicated_queue": true},
+      {"name": "tenant B", "dedicated_queue": false}
     ]
   }
   ```
-  
+
   Where `name` is the name of each tenant and `dedicated_queue`
   is a boolean value to set whether jobs will be run on a specific
   queue with the same tenant name.
 - Assign users to tenants with the following command:
   `sortinghat-admin set-user-tenant username header tenant`
 - The selected tenant should be included in the request using the
-`sortinghat-tenant` header.
+  `sortinghat-tenant` header.
 
 There are some limitations:
+
 - `default` database is only used to store users information and relations between
-users and databases, it won't store anything else related with SortingHat models.
+  users and databases, it won't store anything else related with SortingHat models.
 - Usernames are shared across all instances, which means that it is not possible
-to have the same username with two different passwords in different instances.
+  to have the same username with two different passwords in different instances.
 - Tenants with `dedicated_queue` set as active will add their jobs to the queue
-of the same name. Queues will be created by SortingHat but, you will have
-to run a worker that processes that query.
+  of the same name. Queues will be created by SortingHat but, you will have
+  to run a worker that processes that query.
 
 
 ## Running tests
 
 SortingHat comes with a comprehensive list of unit tests for both 
 frontend and backend.
```

### Comparing `sortinghat-1.0.0rc3/pyproject.toml` & `sortinghat-1.0.1rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sortinghat"
-version = "1.0.0-rc.3"
+version = "1.0.1-rc.1"
 description = "A tool to manage identities."
 authors = [
     "GrimoireLab Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
```

### Comparing `sortinghat-1.0.0rc3/sortinghat/app/schema.py` & `sortinghat-1.0.1rc1/sortinghat/app/schema.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/app/urls.py` & `sortinghat-1.0.1rc1/sortinghat/app/urls.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/cli/client/__init__.py` & `sortinghat-1.0.1rc1/sortinghat/cli/client/__init__.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/cli/client/client.py` & `sortinghat-1.0.1rc1/sortinghat/cli/client/client.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/cli/client/schema.py` & `sortinghat-1.0.1rc1/sortinghat/cli/client/schema.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/cli/cmds/add.py` & `sortinghat-1.0.1rc1/sortinghat/cli/cmds/add.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/cli/cmds/config.py` & `sortinghat-1.0.1rc1/sortinghat/cli/cmds/config.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/cli/cmds/countries.py` & `sortinghat-1.0.1rc1/sortinghat/cli/cmds/countries.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/cli/cmds/enroll.py` & `sortinghat-1.0.1rc1/sortinghat/cli/cmds/enroll.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/cli/cmds/lock.py` & `sortinghat-1.0.1rc1/sortinghat/cli/cmds/lock.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/cli/cmds/merge.py` & `sortinghat-1.0.1rc1/sortinghat/cli/cmds/merge.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/cli/cmds/mv.py` & `sortinghat-1.0.1rc1/sortinghat/cli/cmds/mv.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/cli/cmds/orgs.py` & `sortinghat-1.0.1rc1/sortinghat/cli/cmds/orgs.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/cli/cmds/profile.py` & `sortinghat-1.0.1rc1/sortinghat/cli/cmds/profile.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/cli/cmds/rm.py` & `sortinghat-1.0.1rc1/sortinghat/cli/cmds/rm.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/cli/cmds/show.py` & `sortinghat-1.0.1rc1/sortinghat/cli/cmds/show.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/cli/cmds/split.py` & `sortinghat-1.0.1rc1/sortinghat/cli/cmds/split.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/cli/cmds/withdraw.py` & `sortinghat-1.0.1rc1/sortinghat/cli/cmds/withdraw.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/cli/sortinghat.py` & `sortinghat-1.0.1rc1/sortinghat/cli/sortinghat.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/cli/templates/show.tmpl` & `sortinghat-1.0.1rc1/sortinghat/cli/templates/show.tmpl`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/cli/utils.py` & `sortinghat-1.0.1rc1/sortinghat/cli/utils.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/config/settings.py` & `sortinghat-1.0.1rc1/sortinghat/config/settings.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/admin.py` & `sortinghat-1.0.1rc1/sortinghat/core/admin.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/api.py` & `sortinghat-1.0.1rc1/sortinghat/core/api.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/apps.py` & `sortinghat-1.0.1rc1/sortinghat/core/apps.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/aux.py` & `sortinghat-1.0.1rc1/sortinghat/core/aux.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/context.py` & `sortinghat-1.0.1rc1/sortinghat/core/context.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/db.py` & `sortinghat-1.0.1rc1/sortinghat/core/db.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/decorators.py` & `sortinghat-1.0.1rc1/sortinghat/core/decorators.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/errors.py` & `sortinghat-1.0.1rc1/sortinghat/core/errors.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/fixtures/countries.json` & `sortinghat-1.0.1rc1/sortinghat/core/fixtures/countries.json`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/importer/backend.py` & `sortinghat-1.0.1rc1/sortinghat/core/importer/backend.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/importer/backends/gitdm.py` & `sortinghat-1.0.1rc1/sortinghat/core/importer/backends/gitdm.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/importer/backends/mailmap.py` & `sortinghat-1.0.1rc1/sortinghat/core/importer/backends/mailmap.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/importer/base.py` & `sortinghat-1.0.1rc1/sortinghat/core/importer/base.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/importer/models.py` & `sortinghat-1.0.1rc1/sortinghat/core/importer/models.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/importer/utils.py` & `sortinghat-1.0.1rc1/sortinghat/core/importer/utils.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/jobs.py` & `sortinghat-1.0.1rc1/sortinghat/core/jobs.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/log.py` & `sortinghat-1.0.1rc1/sortinghat/core/log.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/management/commands/create_groups.py` & `sortinghat-1.0.1rc1/sortinghat/core/management/commands/create_groups.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/middleware.py` & `sortinghat-1.0.1rc1/sortinghat/core/middleware.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/migrations/0001_sortinghat.py` & `sortinghat-1.0.1rc1/sortinghat/core/migrations/0001_sortinghat.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/migrations/0002_importidentitiestask.py` & `sortinghat-1.0.1rc1/sortinghat/core/migrations/0002_importidentitiestask.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/migrations/0003_multi_tenancy.py` & `sortinghat-1.0.1rc1/sortinghat/core/migrations/0003_multi_tenancy.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/migrations/0004_tenant_using_header.py` & `sortinghat-1.0.1rc1/sortinghat/core/migrations/0004_tenant_using_header.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/migrations/0005_scheduledtask.py` & `sortinghat-1.0.1rc1/sortinghat/core/migrations/0005_scheduledtask.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/migrations/0006_unify_scheduled_tasks.py` & `sortinghat-1.0.1rc1/sortinghat/core/migrations/0006_unify_scheduled_tasks.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/migrations/0008_alias.py` & `sortinghat-1.0.1rc1/sortinghat/core/migrations/0008_alias.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/models.py` & `sortinghat-1.0.1rc1/sortinghat/core/models.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/recommendations/__init__.py` & `sortinghat-1.0.1rc1/sortinghat/core/recommendations/__init__.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/recommendations/affiliation.py` & `sortinghat-1.0.1rc1/sortinghat/core/recommendations/affiliation.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/recommendations/engine.py` & `sortinghat-1.0.1rc1/sortinghat/core/recommendations/engine.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/recommendations/exclusion.py` & `sortinghat-1.0.1rc1/sortinghat/core/recommendations/exclusion.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/recommendations/gender.py` & `sortinghat-1.0.1rc1/sortinghat/core/recommendations/gender.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/recommendations/matching.py` & `sortinghat-1.0.1rc1/sortinghat/core/recommendations/matching.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/schema.py` & `sortinghat-1.0.1rc1/sortinghat/core/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1612,15 +1612,21 @@
         description='Get all recommended affiliations.'
     )
     recommended_merge = graphene.Field(
         RecommendedMergePaginatedType,
         page_size=graphene.Int(),
         page=graphene.Int(),
         filters=RecommendationFilterType(required=False),
-        description='Get all recommended matched identities.'
+        description=(
+            'Get all identities merge recommendations.'
+            ''
+            'Call without filters to get all the pending recommendations.'
+            'Use the `isApplied` filter with `true` to get applied recommendations'
+            'or with `false` to get dismissed ones.'
+        )
     )
     recommended_gender = graphene.Field(
         RecommendedGenderPaginatedType,
         page_size=graphene.Int(),
         page=graphene.Int(),
         filters=RecommendationFilterType(required=False),
         description='Get all gender recommendations for the identities.'
```

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/css/105.858cd75e.css` & `sortinghat-1.0.1rc1/sortinghat/core/static/css/105.858cd75e.css`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/css/119.87ef3a04.css` & `sortinghat-1.0.1rc1/sortinghat/core/static/css/119.87ef3a04.css`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/css/206.7bb5d056.css` & `sortinghat-1.0.1rc1/sortinghat/core/static/css/206.7bb5d056.css`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/css/488.19ce97b1.css` & `sortinghat-1.0.1rc1/sortinghat/core/static/css/488.19ce97b1.css`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/css/546.696b6ba4.css` & `sortinghat-1.0.1rc1/sortinghat/core/static/css/546.696b6ba4.css`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/css/764.ddc4524e.css` & `sortinghat-1.0.1rc1/sortinghat/core/static/css/764.ddc4524e.css`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/css/812.39b5238d.css` & `sortinghat-1.0.1rc1/sortinghat/core/static/css/812.39b5238d.css`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/css/912.a5e49ce0.css` & `sortinghat-1.0.1rc1/sortinghat/core/static/css/912.a5e49ce0.css`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/css/app.1adeaa19.css` & `sortinghat-1.0.1rc1/sortinghat/core/static/css/app.1adeaa19.css`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/css/chunk-vendors.42fea764.css` & `sortinghat-1.0.1rc1/sortinghat/core/static/css/chunk-vendors.42fea764.css`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/favicon-grimoirelab.ico` & `sortinghat-1.0.1rc1/sortinghat/core/static/favicon-grimoirelab.ico`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Italic.76b8308b.woff` & `sortinghat-1.0.1rc1/sortinghat/core/static/fonts/Roboto-Italic.76b8308b.woff`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Italic.991def81.ttf` & `sortinghat-1.0.1rc1/sortinghat/core/static/fonts/Roboto-Italic.991def81.ttf`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Italic.ca10c790.woff2` & `sortinghat-1.0.1rc1/sortinghat/core/static/fonts/Roboto-Italic.ca10c790.woff2`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Light.2d3c72a3.woff` & `sortinghat-1.0.1rc1/sortinghat/core/static/fonts/Roboto-Light.2d3c72a3.woff`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Light.41cb61ed.woff2` & `sortinghat-1.0.1rc1/sortinghat/core/static/fonts/Roboto-Light.41cb61ed.woff2`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Light.f2e7274e.ttf` & `sortinghat-1.0.1rc1/sortinghat/core/static/fonts/Roboto-Light.f2e7274e.ttf`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-LightItalic.07369d23.woff2` & `sortinghat-1.0.1rc1/sortinghat/core/static/fonts/Roboto-LightItalic.07369d23.woff2`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-LightItalic.45582c0c.woff` & `sortinghat-1.0.1rc1/sortinghat/core/static/fonts/Roboto-LightItalic.45582c0c.woff`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-LightItalic.b694f0fe.ttf` & `sortinghat-1.0.1rc1/sortinghat/core/static/fonts/Roboto-LightItalic.b694f0fe.ttf`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Medium.0519ad6f.woff2` & `sortinghat-1.0.1rc1/sortinghat/core/static/fonts/Roboto-Medium.0519ad6f.woff2`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Medium.483a3bd1.woff` & `sortinghat-1.0.1rc1/sortinghat/core/static/fonts/Roboto-Medium.483a3bd1.woff`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Medium.af9d0139.ttf` & `sortinghat-1.0.1rc1/sortinghat/core/static/fonts/Roboto-Medium.af9d0139.ttf`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-MediumItalic.3723a2e7.ttf` & `sortinghat-1.0.1rc1/sortinghat/core/static/fonts/Roboto-MediumItalic.3723a2e7.ttf`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-MediumItalic.8b19cc18.woff` & `sortinghat-1.0.1rc1/sortinghat/core/static/fonts/Roboto-MediumItalic.8b19cc18.woff`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-MediumItalic.b35d3641.woff2` & `sortinghat-1.0.1rc1/sortinghat/core/static/fonts/Roboto-MediumItalic.b35d3641.woff2`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Regular.36d4503d.woff` & `sortinghat-1.0.1rc1/sortinghat/core/static/fonts/Roboto-Regular.36d4503d.woff`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Regular.ae3a8db9.ttf` & `sortinghat-1.0.1rc1/sortinghat/core/static/fonts/Roboto-Regular.ae3a8db9.ttf`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/Roboto-Regular.e0553e00.woff2` & `sortinghat-1.0.1rc1/sortinghat/core/static/fonts/Roboto-Regular.e0553e00.woff2`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/materialdesignicons-webfont.21f691f0.ttf` & `sortinghat-1.0.1rc1/sortinghat/core/static/fonts/materialdesignicons-webfont.21f691f0.ttf`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/materialdesignicons-webfont.54b0f60d.woff2` & `sortinghat-1.0.1rc1/sortinghat/core/static/fonts/materialdesignicons-webfont.54b0f60d.woff2`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/materialdesignicons-webfont.5d875350.eot` & `sortinghat-1.0.1rc1/sortinghat/core/static/fonts/materialdesignicons-webfont.5d875350.eot`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/fonts/materialdesignicons-webfont.d671cbf6.woff` & `sortinghat-1.0.1rc1/sortinghat/core/static/fonts/materialdesignicons-webfont.d671cbf6.woff`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/js/105.2c5bfa40.js` & `sortinghat-1.0.1rc1/sortinghat/core/static/js/105.2c5bfa40.js`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/js/105.2c5bfa40.js.map` & `sortinghat-1.0.1rc1/sortinghat/core/static/js/105.2c5bfa40.js.map`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/js/119.6bdc5ff2.js` & `sortinghat-1.0.1rc1/sortinghat/core/static/js/119.6bdc5ff2.js`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/js/119.6bdc5ff2.js.map` & `sortinghat-1.0.1rc1/sortinghat/core/static/js/119.6bdc5ff2.js.map`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/js/206.75232ba8.js` & `sortinghat-1.0.1rc1/sortinghat/core/static/js/206.75232ba8.js`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/js/206.75232ba8.js.map` & `sortinghat-1.0.1rc1/sortinghat/core/static/js/206.75232ba8.js.map`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/js/253.61ce8eec.js` & `sortinghat-1.0.1rc1/sortinghat/core/static/js/253.61ce8eec.js`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/js/253.61ce8eec.js.map` & `sortinghat-1.0.1rc1/sortinghat/core/static/js/253.61ce8eec.js.map`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/js/414.13cae85b.js` & `sortinghat-1.0.1rc1/sortinghat/core/static/js/414.13cae85b.js`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/js/414.13cae85b.js.map` & `sortinghat-1.0.1rc1/sortinghat/core/static/js/414.13cae85b.js.map`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/js/488.0a0d2dda.js` & `sortinghat-1.0.1rc1/sortinghat/core/static/js/488.0a0d2dda.js`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/js/488.0a0d2dda.js.map` & `sortinghat-1.0.1rc1/sortinghat/core/static/js/488.0a0d2dda.js.map`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/js/544.b1834368.js` & `sortinghat-1.0.1rc1/sortinghat/core/static/js/544.b1834368.js`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/js/544.b1834368.js.map` & `sortinghat-1.0.1rc1/sortinghat/core/static/js/544.b1834368.js.map`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/js/546.718bab60.js` & `sortinghat-1.0.1rc1/sortinghat/core/static/js/546.718bab60.js`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/js/546.718bab60.js.map` & `sortinghat-1.0.1rc1/sortinghat/core/static/js/546.718bab60.js.map`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/js/689.e598fac2.js` & `sortinghat-1.0.1rc1/sortinghat/core/static/js/689.e598fac2.js`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/js/689.e598fac2.js.map` & `sortinghat-1.0.1rc1/sortinghat/core/static/js/689.e598fac2.js.map`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/js/764.5fe45faf.js` & `sortinghat-1.0.1rc1/sortinghat/core/static/js/764.5fe45faf.js`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/js/764.5fe45faf.js.map` & `sortinghat-1.0.1rc1/sortinghat/core/static/js/764.5fe45faf.js.map`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/js/812.711cab61.js` & `sortinghat-1.0.1rc1/sortinghat/core/static/js/812.711cab61.js`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/js/812.711cab61.js.map` & `sortinghat-1.0.1rc1/sortinghat/core/static/js/812.711cab61.js.map`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/js/858.8246391b.js` & `sortinghat-1.0.1rc1/sortinghat/core/static/js/858.8246391b.js`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/js/858.8246391b.js.map` & `sortinghat-1.0.1rc1/sortinghat/core/static/js/858.8246391b.js.map`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/js/912.ddb83f31.js` & `sortinghat-1.0.1rc1/sortinghat/core/static/js/912.ddb83f31.js`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/js/912.ddb83f31.js.map` & `sortinghat-1.0.1rc1/sortinghat/core/static/js/912.ddb83f31.js.map`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/js/app.014c6257.js` & `sortinghat-1.0.1rc1/sortinghat/core/static/js/app.014c6257.js`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/js/app.014c6257.js.map` & `sortinghat-1.0.1rc1/sortinghat/core/static/js/app.014c6257.js.map`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/js/chunk-vendors.dba6d507.js` & `sortinghat-1.0.1rc1/sortinghat/core/static/js/chunk-vendors.dba6d507.js`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/static/js/chunk-vendors.dba6d507.js.map` & `sortinghat-1.0.1rc1/sortinghat/core/static/js/chunk-vendors.dba6d507.js.map`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/templates/index.html` & `sortinghat-1.0.1rc1/sortinghat/core/templates/index.html`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/tenant.py` & `sortinghat-1.0.1rc1/sortinghat/core/tenant.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/core/views.py` & `sortinghat-1.0.1rc1/sortinghat/core/views.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/server/sortinghat_admin.py` & `sortinghat-1.0.1rc1/sortinghat/server/sortinghat_admin.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/server/sortinghatd.py` & `sortinghat-1.0.1rc1/sortinghat/server/sortinghatd.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/server/sortinghatw.py` & `sortinghat-1.0.1rc1/sortinghat/server/sortinghatw.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/server/utils/create_sh_0_7_fixture.py` & `sortinghat-1.0.1rc1/sortinghat/server/utils/create_sh_0_7_fixture.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/sortinghat/utils/__init__.py` & `sortinghat-1.0.1rc1/sortinghat/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/tests/cli/test_cmd_add.py` & `sortinghat-1.0.1rc1/tests/cli/test_cmd_add.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/tests/cli/test_cmd_config.py` & `sortinghat-1.0.1rc1/tests/cli/test_cmd_config.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/tests/cli/test_cmd_countries.py` & `sortinghat-1.0.1rc1/tests/cli/test_cmd_countries.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/tests/cli/test_cmd_enroll.py` & `sortinghat-1.0.1rc1/tests/cli/test_cmd_enroll.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/tests/cli/test_cmd_lock.py` & `sortinghat-1.0.1rc1/tests/cli/test_cmd_lock.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/tests/cli/test_cmd_merge.py` & `sortinghat-1.0.1rc1/tests/cli/test_cmd_merge.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/tests/cli/test_cmd_mv.py` & `sortinghat-1.0.1rc1/tests/cli/test_cmd_mv.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/tests/cli/test_cmd_orgs.py` & `sortinghat-1.0.1rc1/tests/cli/test_cmd_orgs.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/tests/cli/test_cmd_profile.py` & `sortinghat-1.0.1rc1/tests/cli/test_cmd_profile.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/tests/cli/test_cmd_rm.py` & `sortinghat-1.0.1rc1/tests/cli/test_cmd_rm.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/tests/cli/test_cmd_show.py` & `sortinghat-1.0.1rc1/tests/cli/test_cmd_show.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/tests/cli/test_cmd_split.py` & `sortinghat-1.0.1rc1/tests/cli/test_cmd_split.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/tests/cli/test_cmd_withdraw.py` & `sortinghat-1.0.1rc1/tests/cli/test_cmd_withdraw.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/tests/importer/mocked_package/backend_a.py` & `sortinghat-1.0.1rc1/tests/importer/mocked_package/backend_a.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/tests/importer/mocked_package/nested_package/nested_backend_b.py` & `sortinghat-1.0.1rc1/tests/importer/mocked_package/nested_package/nested_backend_b.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/tests/importer/mocked_package/nested_package/nested_backend_c.py` & `sortinghat-1.0.1rc1/tests/importer/mocked_package/nested_package/nested_backend_c.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/tests/importer/mocked_package/nested_package/nested_not_backend.py` & `sortinghat-1.0.1rc1/tests/importer/mocked_package/nested_package/nested_not_backend.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/tests/importer/test_backend.py` & `sortinghat-1.0.1rc1/tests/importer/test_backend.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/tests/importer/test_gitdm.py` & `sortinghat-1.0.1rc1/tests/importer/test_gitdm.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/tests/importer/test_utils.py` & `sortinghat-1.0.1rc1/tests/importer/test_utils.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/tests/rec/test_affiliations.py` & `sortinghat-1.0.1rc1/tests/rec/test_affiliations.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/tests/rec/test_engine.py` & `sortinghat-1.0.1rc1/tests/rec/test_engine.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/tests/rec/test_exclusion.py` & `sortinghat-1.0.1rc1/tests/rec/test_exclusion.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/tests/rec/test_gender.py` & `sortinghat-1.0.1rc1/tests/rec/test_gender.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/tests/rec/test_matches.py` & `sortinghat-1.0.1rc1/tests/rec/test_matches.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/tests/runners.py` & `sortinghat-1.0.1rc1/tests/runners.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/tests/tenants/test_jobs.py` & `sortinghat-1.0.1rc1/tests/tenants/test_jobs.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/tests/tenants/test_middleware.py` & `sortinghat-1.0.1rc1/tests/tenants/test_middleware.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/tests/tenants/test_schema.py` & `sortinghat-1.0.1rc1/tests/tenants/test_schema.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/tests/test_api.py` & `sortinghat-1.0.1rc1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/tests/test_aux.py` & `sortinghat-1.0.1rc1/tests/test_aux.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/tests/test_client.py` & `sortinghat-1.0.1rc1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/tests/test_db.py` & `sortinghat-1.0.1rc1/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/tests/test_errors.py` & `sortinghat-1.0.1rc1/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/tests/test_jobs.py` & `sortinghat-1.0.1rc1/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/tests/test_log.py` & `sortinghat-1.0.1rc1/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/tests/test_model.py` & `sortinghat-1.0.1rc1/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/tests/test_schema.py` & `sortinghat-1.0.1rc1/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/tests/test_utils.py` & `sortinghat-1.0.1rc1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `sortinghat-1.0.0rc3/PKG-INFO` & `sortinghat-1.0.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sortinghat
-Version: 1.0.0rc3
+Version: 1.0.1rc1
 Summary: A tool to manage identities.
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab
 Author: GrimoireLab Developers
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -58,15 +58,15 @@
 In the context of GrimoireLab, Sorting Hat is usually run after data is retrieved with [Perceval](https://github.com/chaoss/grimoirelab-perceval), to store the identities obtained into its database, and later merge them into individuals (and maybe affiliate them).
 
 
 ## Requirements
 
 * Python >= 3.8
 * Poetry >= 1.1.0
-* MySQL >= 5.7 or MariaDB 10.0
+* MySQL >= 8.1 or MariaDB >= 10.4
 * Django = 4.2
 * Graphene-Django >= 2.0
 * uWSGI >= 2.0
 
 You will also need some other libraries for running the tool, you can find the
 whole list of dependencies in [pyproject.toml](pyproject.toml) file.
 
@@ -110,16 +110,16 @@
 $ apt install libmariadbclient-dev-compat
 ```
 
 #### Installation and configuration
 
 **Note**: these examples use `sortinghat.config.settings` configuration file.
 In order to use that configuration you need to define the environment variable
-`SORTINGHAT_SECRET_KEY` with a secret. More info here:
-https://docs.djangoproject.com/en/4.2/ref/settings/#std:setting-SECRET_KEY
+`SORTINGHAT_SECRET_KEY` with a secret. More info
+[here](https://docs.djangoproject.com/en/4.2/ref/settings/#std:setting-SECRET_KEY).
 
 
 Install the required dependencies (this will also create a virtual environment).
 ```
 $ poetry install
 ```
 
@@ -294,37 +294,38 @@
 - Set `MULTI_TENANT` settings to `True`.
 - Define a list of tenants using the configuration file `sortinghat/config/tenants.json`.
   You can use a different json file using the environment variable 
   `SORTINGHAT_MULTI_TENANT_LIST_PATH`. The file should have the next schema:
 
   ```json
   {
-    'tenants': [
-      {'name': 'tenant A', 'dedicated_queue': true},
-      {'name': 'tenant B', 'dedicated_queue': false}
+    "tenants": [
+      {"name": "tenant A", "dedicated_queue": true},
+      {"name": "tenant B", "dedicated_queue": false}
     ]
   }
   ```
-  
+
   Where `name` is the name of each tenant and `dedicated_queue`
   is a boolean value to set whether jobs will be run on a specific
   queue with the same tenant name.
 - Assign users to tenants with the following command:
   `sortinghat-admin set-user-tenant username header tenant`
 - The selected tenant should be included in the request using the
-`sortinghat-tenant` header.
+  `sortinghat-tenant` header.
 
 There are some limitations:
+
 - `default` database is only used to store users information and relations between
-users and databases, it won't store anything else related with SortingHat models.
+  users and databases, it won't store anything else related with SortingHat models.
 - Usernames are shared across all instances, which means that it is not possible
-to have the same username with two different passwords in different instances.
+  to have the same username with two different passwords in different instances.
 - Tenants with `dedicated_queue` set as active will add their jobs to the queue
-of the same name. Queues will be created by SortingHat but, you will have
-to run a worker that processes that query.
+  of the same name. Queues will be created by SortingHat but, you will have
+  to run a worker that processes that query.
 
 
 ## Running tests
 
 SortingHat comes with a comprehensive list of unit tests for both 
 frontend and backend.
```

