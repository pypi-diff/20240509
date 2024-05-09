# Comparing `tmp/aa_srp-2.0.0b1.tar.gz` & `tmp/aa_srp-2.0.0b2.tar.gz`

## Comparing `aa_srp-2.0.0b1.tar` & `aa_srp-2.0.0b2.tar`

### file list

```diff
@@ -1,129 +1,129 @@
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/__init__.py
--rw-r--r--   0        0        0     8177 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/admin.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/app_settings.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/apps.py
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/auth_hooks.py
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/constants.py
--rw-r--r--   0        0        0     7390 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/form.py
--rw-r--r--   0        0        0     4865 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/managers.py
--rw-r--r--   0        0        0    14672 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/models.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/providers.py
--rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/urls.py
--rw-r--r--   0        0        0     5485 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/discord/channel_message.py
--rw-r--r--   0        0        0     6468 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/discord/direct_message.py
--rw-r--r--   0        0        0     3626 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/helper/character.py
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/helper/eve_images.py
--rw-r--r--   0        0        0    12271 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/helper/icons.py
--rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/helper/notification.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/helper/user.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/locale/.gitkeep
--rw-r--r--   0        0        0    24140 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/locale/django.pot
--rw-r--r--   0        0        0    16921 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    30673 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    27140 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    24471 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    24317 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    24150 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/locale/ko_KR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    25705 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    22094 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    36181 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    26600 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    15610 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    29766 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/management/commands/aasrp_load_eve.py
--rw-r--r--   0        0        0    10264 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/management/commands/aasrp_migrate_srp_data.py
--rw-r--r--   0        0        0     7609 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/migrations/0001_initial.py
--rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/migrations/0002_relations_update.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/migrations/0003_aasrprequest_reject_info.py
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/migrations/0004_aasrpusersettings.py
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/migrations/0005_insurance.py
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/migrations/0006_related_names.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/migrations/0007_aasrprequestcomment_comment_time_and_more.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/migrations/0008_aasrprequestcomment_new_status_and_more.py
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/migrations/0009_add_fleet_type_to_srp_link.py
--rw-r--r--   0        0        0    14458 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/migrations/0010_model_changes.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/migrations/0011_default_settings.py
--rw-r--r--   0        0        0    11040 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/migrations/0012_alter_fleettype_options_alter_insurance_options_and_more.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/migrations/0013_setting_loss_value_source.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/migrations/__init__.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/static/aasrp/css/aa-srp-form.css
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/static/aasrp/css/aa-srp-form.min.css
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/static/aasrp/css/aa-srp-form.min.css.map
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/static/aasrp/css/aa-srp.css
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/static/aasrp/css/aa-srp.min.css
--rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/static/aasrp/css/aa-srp.min.css.map
--rw-r--r--   0        0        0    11066 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/static/aasrp/javascript/aa-srp-dashboard.js
--rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/static/aasrp/javascript/aa-srp-dashboard.min.js
--rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/static/aasrp/javascript/aa-srp-dashboard.min.js.map
--rw-r--r--   0        0        0    16216 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/static/aasrp/javascript/aa-srp-view-requests.js
--rw-r--r--   0        0        0     6083 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/static/aasrp/javascript/aa-srp-view-requests.min.js
--rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/static/aasrp/javascript/aa-srp-view-requests.min.js.map
--rw-r--r--   0        0        0    21204 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/css/bootstrap-editable.css
--rw-r--r--   0        0        0    17789 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/css/bootstrap-editable.min.css
--rw-r--r--   0        0        0    25994 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/css/bootstrap-editable.min.css.map
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/img/clear.png
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/img/loading.gif
--rw-r--r--   0        0        0   219767 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/js/bootstrap-editable.js
--rw-r--r--   0        0        0    75550 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/js/bootstrap-editable.min.js
--rw-r--r--   0        0        0    98885 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/js/bootstrap-editable.min.js.map
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/templates/aasrp/base.html
--rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/templates/aasrp/dashboard.html
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/templates/aasrp/link-add.html
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/templates/aasrp/link-edit.html
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/templates/aasrp/request-srp.html
--rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/templates/aasrp/view-requests.html
--rw-r--r--   0        0        0     4642 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/templates/aasrp/ajax-render/srp-request-additional-information.html
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/templates/aasrp/bundles/aa-srp-css.html
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/templates/aasrp/bundles/aa-srp-dashboard-js.html
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/templates/aasrp/bundles/aa-srp-form-css.html
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/templates/aasrp/bundles/aa-srp-view-requests-js.html
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/templates/aasrp/bundles/x-editable-css.html
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/templates/aasrp/bundles/x-editable-js.html
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/templates/aasrp/modals/dashboard/delete-srp-link.html
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/templates/aasrp/modals/dashboard/disable-srp-link.html
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/templates/aasrp/modals/dashboard/enable-srp-link.html
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/templates/aasrp/modals/view-requests/accept-rejected-request.html
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/templates/aasrp/modals/view-requests/accept-request.html
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/templates/aasrp/modals/view-requests/delete-request.html
--rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/templates/aasrp/modals/view-requests/mark-complete.html
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/templates/aasrp/modals/view-requests/reject-request.html
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/templates/aasrp/modals/view-requests/request-details.html
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/templates/aasrp/partials/dashboard/navigation.html
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/templates/aasrp/partials/dashboard/srp-links.html
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/templates/aasrp/partials/dashboard/tabs-content.html
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/templates/aasrp/partials/dashboard/tabs-navigation.html
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/templates/aasrp/partials/dashboard/user-settings.html
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/templates/aasrp/partials/dashboard/user-srp-requests.html
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/templates/aasrp/partials/footer/app-translation-footer.html
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/templates/aasrp/partials/form/required-field-hint.html
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/templates/aasrp/partials/link-add/form.html
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/templates/aasrp/partials/link-edit/form.html
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/templates/aasrp/partials/request-srp/fleet-details.html
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/templates/aasrp/partials/request-srp/form.html
--rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/templates/aasrp/partials/view-requests/overview.html
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/templates/aasrp/partials/view-requests/requests.html
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/templatetags/__init__.py
--rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/templatetags/aasrp.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/tests/__init__.py
--rw-r--r--   0        0        0     9678 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/tests/test_access.py
--rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/tests/test_auth_hooks.py
--rw-r--r--   0        0        0    11016 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/tests/test_helper_character.py
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/tests/test_installed_modules.py
--rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/tests/test_model_setting.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/tests/test_models.py
--rw-r--r--   0        0        0    15384 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/tests/test_templatetags.py
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/tests/utils.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/views/__init__.py
--rw-r--r--   0        0        0    24294 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/views/ajax.py
--rw-r--r--   0        0        0    19103 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/aasrp/views/general.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/LICENSE
--rw-r--r--   0        0        0    11381 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/README.md
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/pyproject.toml
--rw-r--r--   0        0        0    53909 2020-02-02 00:00:00.000000 aa_srp-2.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/__init__.py
+-rw-r--r--   0        0        0     8177 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/admin.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/app_settings.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/apps.py
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/auth_hooks.py
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/constants.py
+-rw-r--r--   0        0        0     7390 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/form.py
+-rw-r--r--   0        0        0     4865 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/managers.py
+-rw-r--r--   0        0        0    14672 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/models.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/providers.py
+-rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/urls.py
+-rw-r--r--   0        0        0     5485 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/discord/channel_message.py
+-rw-r--r--   0        0        0     6468 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/discord/direct_message.py
+-rw-r--r--   0        0        0     3626 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/helper/character.py
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/helper/eve_images.py
+-rw-r--r--   0        0        0    12271 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/helper/icons.py
+-rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/helper/notification.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/helper/user.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/locale/.gitkeep
+-rw-r--r--   0        0        0    24140 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/locale/django.pot
+-rw-r--r--   0        0        0    16921 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    30673 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    27140 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    24471 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    24317 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    24150 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    25705 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    22094 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    36181 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    26600 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    15610 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    29766 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/management/commands/aasrp_load_eve.py
+-rw-r--r--   0        0        0    10264 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/management/commands/aasrp_migrate_srp_data.py
+-rw-r--r--   0        0        0     7609 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/migrations/0002_relations_update.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/migrations/0003_aasrprequest_reject_info.py
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/migrations/0004_aasrpusersettings.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/migrations/0005_insurance.py
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/migrations/0006_related_names.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/migrations/0007_aasrprequestcomment_comment_time_and_more.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/migrations/0008_aasrprequestcomment_new_status_and_more.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/migrations/0009_add_fleet_type_to_srp_link.py
+-rw-r--r--   0        0        0    14458 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/migrations/0010_model_changes.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/migrations/0011_default_settings.py
+-rw-r--r--   0        0        0    11040 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/migrations/0012_alter_fleettype_options_alter_insurance_options_and_more.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/migrations/0013_setting_loss_value_source.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/migrations/__init__.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/static/aasrp/css/aa-srp-form.css
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/static/aasrp/css/aa-srp-form.min.css
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/static/aasrp/css/aa-srp-form.min.css.map
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/static/aasrp/css/aa-srp.css
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/static/aasrp/css/aa-srp.min.css
+-rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/static/aasrp/css/aa-srp.min.css.map
+-rw-r--r--   0        0        0    11066 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/static/aasrp/javascript/aa-srp-dashboard.js
+-rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/static/aasrp/javascript/aa-srp-dashboard.min.js
+-rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/static/aasrp/javascript/aa-srp-dashboard.min.js.map
+-rw-r--r--   0        0        0    16216 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/static/aasrp/javascript/aa-srp-view-requests.js
+-rw-r--r--   0        0        0     6083 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/static/aasrp/javascript/aa-srp-view-requests.min.js
+-rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/static/aasrp/javascript/aa-srp-view-requests.min.js.map
+-rw-r--r--   0        0        0    21204 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/css/bootstrap-editable.css
+-rw-r--r--   0        0        0    17789 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/css/bootstrap-editable.min.css
+-rw-r--r--   0        0        0    25994 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/css/bootstrap-editable.min.css.map
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/img/clear.png
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/img/loading.gif
+-rw-r--r--   0        0        0   219767 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/js/bootstrap-editable.js
+-rw-r--r--   0        0        0    75550 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/js/bootstrap-editable.min.js
+-rw-r--r--   0        0        0    98885 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/js/bootstrap-editable.min.js.map
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/templates/aasrp/base.html
+-rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/templates/aasrp/dashboard.html
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/templates/aasrp/link-add.html
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/templates/aasrp/link-edit.html
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/templates/aasrp/request-srp.html
+-rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/templates/aasrp/view-requests.html
+-rw-r--r--   0        0        0     4642 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/templates/aasrp/ajax-render/srp-request-additional-information.html
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/templates/aasrp/bundles/aa-srp-css.html
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/templates/aasrp/bundles/aa-srp-dashboard-js.html
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/templates/aasrp/bundles/aa-srp-form-css.html
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/templates/aasrp/bundles/aa-srp-view-requests-js.html
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/templates/aasrp/bundles/x-editable-css.html
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/templates/aasrp/bundles/x-editable-js.html
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/templates/aasrp/modals/dashboard/delete-srp-link.html
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/templates/aasrp/modals/dashboard/disable-srp-link.html
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/templates/aasrp/modals/dashboard/enable-srp-link.html
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/templates/aasrp/modals/view-requests/accept-rejected-request.html
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/templates/aasrp/modals/view-requests/accept-request.html
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/templates/aasrp/modals/view-requests/delete-request.html
+-rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/templates/aasrp/modals/view-requests/mark-complete.html
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/templates/aasrp/modals/view-requests/reject-request.html
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/templates/aasrp/modals/view-requests/request-details.html
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/templates/aasrp/partials/dashboard/navigation.html
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/templates/aasrp/partials/dashboard/srp-links.html
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/templates/aasrp/partials/dashboard/tabs-content.html
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/templates/aasrp/partials/dashboard/tabs-navigation.html
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/templates/aasrp/partials/dashboard/user-settings.html
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/templates/aasrp/partials/dashboard/user-srp-requests.html
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/templates/aasrp/partials/footer/app-translation-footer.html
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/templates/aasrp/partials/form/required-field-hint.html
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/templates/aasrp/partials/link-add/form.html
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/templates/aasrp/partials/link-edit/form.html
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/templates/aasrp/partials/request-srp/fleet-details.html
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/templates/aasrp/partials/request-srp/form.html
+-rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/templates/aasrp/partials/view-requests/overview.html
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/templates/aasrp/partials/view-requests/requests.html
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/templatetags/__init__.py
+-rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/templatetags/aasrp.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/tests/__init__.py
+-rw-r--r--   0        0        0     9678 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/tests/test_access.py
+-rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/tests/test_auth_hooks.py
+-rw-r--r--   0        0        0    11016 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/tests/test_helper_character.py
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/tests/test_installed_modules.py
+-rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/tests/test_model_setting.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/tests/test_models.py
+-rw-r--r--   0        0        0    15384 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/tests/test_templatetags.py
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/tests/utils.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/views/__init__.py
+-rw-r--r--   0        0        0    24294 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/views/ajax.py
+-rw-r--r--   0        0        0    19103 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/aasrp/views/general.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/LICENSE
+-rw-r--r--   0        0        0    11381 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/README.md
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/pyproject.toml
+-rw-r--r--   0        0        0    53909 2020-02-02 00:00:00.000000 aa_srp-2.0.0b2/PKG-INFO
```

### Comparing `aa_srp-2.0.0b1/aasrp/admin.py` & `aa_srp-2.0.0b2/aasrp/admin.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/app_settings.py` & `aa_srp-2.0.0b2/aasrp/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/auth_hooks.py` & `aa_srp-2.0.0b2/aasrp/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/constants.py` & `aa_srp-2.0.0b2/aasrp/constants.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/form.py` & `aa_srp-2.0.0b2/aasrp/form.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/managers.py` & `aa_srp-2.0.0b2/aasrp/managers.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/models.py` & `aa_srp-2.0.0b2/aasrp/models.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/urls.py` & `aa_srp-2.0.0b2/aasrp/urls.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/discord/channel_message.py` & `aa_srp-2.0.0b2/aasrp/discord/channel_message.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/discord/direct_message.py` & `aa_srp-2.0.0b2/aasrp/discord/direct_message.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/helper/character.py` & `aa_srp-2.0.0b2/aasrp/helper/character.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/helper/eve_images.py` & `aa_srp-2.0.0b2/aasrp/helper/eve_images.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/helper/icons.py` & `aa_srp-2.0.0b2/aasrp/helper/icons.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/helper/notification.py` & `aa_srp-2.0.0b2/aasrp/helper/notification.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/locale/django.pot` & `aa_srp-2.0.0b2/aasrp/locale/django.pot`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/locale/de/LC_MESSAGES/django.mo` & `aa_srp-2.0.0b2/aasrp/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/locale/de/LC_MESSAGES/django.po` & `aa_srp-2.0.0b2/aasrp/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/locale/es/LC_MESSAGES/django.mo` & `aa_srp-2.0.0b2/aasrp/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/locale/es/LC_MESSAGES/django.po` & `aa_srp-2.0.0b2/aasrp/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/locale/fr_FR/LC_MESSAGES/django.mo` & `aa_srp-2.0.0b2/aasrp/locale/fr_FR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/locale/fr_FR/LC_MESSAGES/django.po` & `aa_srp-2.0.0b2/aasrp/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/locale/it_IT/LC_MESSAGES/django.mo` & `aa_srp-2.0.0b2/aasrp/locale/it_IT/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/locale/it_IT/LC_MESSAGES/django.po` & `aa_srp-2.0.0b2/aasrp/locale/it_IT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/locale/ja/LC_MESSAGES/django.po` & `aa_srp-2.0.0b2/aasrp/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/locale/ko_KR/LC_MESSAGES/django.mo` & `aa_srp-2.0.0b2/aasrp/locale/ko_KR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/locale/ko_KR/LC_MESSAGES/django.po` & `aa_srp-2.0.0b2/aasrp/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/locale/ru/LC_MESSAGES/django.mo` & `aa_srp-2.0.0b2/aasrp/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/locale/ru/LC_MESSAGES/django.po` & `aa_srp-2.0.0b2/aasrp/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/locale/uk/LC_MESSAGES/django.mo` & `aa_srp-2.0.0b2/aasrp/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/locale/uk/LC_MESSAGES/django.po` & `aa_srp-2.0.0b2/aasrp/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/locale/zh_Hans/LC_MESSAGES/django.mo` & `aa_srp-2.0.0b2/aasrp/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_srp-2.0.0b2/aasrp/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/management/commands/aasrp_load_eve.py` & `aa_srp-2.0.0b2/aasrp/management/commands/aasrp_load_eve.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/management/commands/aasrp_migrate_srp_data.py` & `aa_srp-2.0.0b2/aasrp/management/commands/aasrp_migrate_srp_data.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/migrations/0001_initial.py` & `aa_srp-2.0.0b2/aasrp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/migrations/0002_relations_update.py` & `aa_srp-2.0.0b2/aasrp/migrations/0002_relations_update.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/migrations/0004_aasrpusersettings.py` & `aa_srp-2.0.0b2/aasrp/migrations/0004_aasrpusersettings.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/migrations/0005_insurance.py` & `aa_srp-2.0.0b2/aasrp/migrations/0005_insurance.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/migrations/0006_related_names.py` & `aa_srp-2.0.0b2/aasrp/migrations/0006_related_names.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/migrations/0007_aasrprequestcomment_comment_time_and_more.py` & `aa_srp-2.0.0b2/aasrp/migrations/0007_aasrprequestcomment_comment_time_and_more.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/migrations/0008_aasrprequestcomment_new_status_and_more.py` & `aa_srp-2.0.0b2/aasrp/migrations/0008_aasrprequestcomment_new_status_and_more.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/migrations/0009_add_fleet_type_to_srp_link.py` & `aa_srp-2.0.0b2/aasrp/migrations/0009_add_fleet_type_to_srp_link.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/migrations/0010_model_changes.py` & `aa_srp-2.0.0b2/aasrp/migrations/0010_model_changes.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/migrations/0011_default_settings.py` & `aa_srp-2.0.0b2/aasrp/migrations/0011_default_settings.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/migrations/0012_alter_fleettype_options_alter_insurance_options_and_more.py` & `aa_srp-2.0.0b2/aasrp/migrations/0012_alter_fleettype_options_alter_insurance_options_and_more.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/migrations/0013_setting_loss_value_source.py` & `aa_srp-2.0.0b2/aasrp/migrations/0013_setting_loss_value_source.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/static/aasrp/css/aa-srp.css` & `aa_srp-2.0.0b2/aasrp/static/aasrp/css/aa-srp.css`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/static/aasrp/css/aa-srp.min.css` & `aa_srp-2.0.0b2/aasrp/static/aasrp/css/aa-srp.min.css`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/static/aasrp/css/aa-srp.min.css.map` & `aa_srp-2.0.0b2/aasrp/static/aasrp/css/aa-srp.min.css.map`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/static/aasrp/javascript/aa-srp-dashboard.js` & `aa_srp-2.0.0b2/aasrp/static/aasrp/javascript/aa-srp-dashboard.js`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/static/aasrp/javascript/aa-srp-dashboard.min.js` & `aa_srp-2.0.0b2/aasrp/static/aasrp/javascript/aa-srp-dashboard.min.js`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/static/aasrp/javascript/aa-srp-dashboard.min.js.map` & `aa_srp-2.0.0b2/aasrp/static/aasrp/javascript/aa-srp-dashboard.min.js.map`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/static/aasrp/javascript/aa-srp-view-requests.js` & `aa_srp-2.0.0b2/aasrp/static/aasrp/javascript/aa-srp-view-requests.js`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/static/aasrp/javascript/aa-srp-view-requests.min.js` & `aa_srp-2.0.0b2/aasrp/static/aasrp/javascript/aa-srp-view-requests.min.js`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/static/aasrp/javascript/aa-srp-view-requests.min.js.map` & `aa_srp-2.0.0b2/aasrp/static/aasrp/javascript/aa-srp-view-requests.min.js.map`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/css/bootstrap-editable.css` & `aa_srp-2.0.0b2/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/css/bootstrap-editable.css`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/css/bootstrap-editable.min.css` & `aa_srp-2.0.0b2/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/css/bootstrap-editable.min.css`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/css/bootstrap-editable.min.css.map` & `aa_srp-2.0.0b2/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/css/bootstrap-editable.min.css.map`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/img/loading.gif` & `aa_srp-2.0.0b2/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/img/loading.gif`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/js/bootstrap-editable.js` & `aa_srp-2.0.0b2/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/js/bootstrap-editable.js`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/js/bootstrap-editable.min.js` & `aa_srp-2.0.0b2/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/js/bootstrap-editable.min.js`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/js/bootstrap-editable.min.js.map` & `aa_srp-2.0.0b2/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/js/bootstrap-editable.min.js.map`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/templates/aasrp/base.html` & `aa_srp-2.0.0b2/aasrp/templates/aasrp/base.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/templates/aasrp/dashboard.html` & `aa_srp-2.0.0b2/aasrp/templates/aasrp/dashboard.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/templates/aasrp/link-add.html` & `aa_srp-2.0.0b2/aasrp/templates/aasrp/link-add.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/templates/aasrp/view-requests.html` & `aa_srp-2.0.0b2/aasrp/templates/aasrp/view-requests.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/templates/aasrp/ajax-render/srp-request-additional-information.html` & `aa_srp-2.0.0b2/aasrp/templates/aasrp/ajax-render/srp-request-additional-information.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/templates/aasrp/modals/dashboard/delete-srp-link.html` & `aa_srp-2.0.0b2/aasrp/templates/aasrp/modals/dashboard/delete-srp-link.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/templates/aasrp/modals/dashboard/disable-srp-link.html` & `aa_srp-2.0.0b2/aasrp/templates/aasrp/modals/dashboard/disable-srp-link.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/templates/aasrp/modals/dashboard/enable-srp-link.html` & `aa_srp-2.0.0b2/aasrp/templates/aasrp/modals/dashboard/enable-srp-link.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/templates/aasrp/modals/view-requests/accept-rejected-request.html` & `aa_srp-2.0.0b2/aasrp/templates/aasrp/modals/view-requests/accept-rejected-request.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/templates/aasrp/modals/view-requests/accept-request.html` & `aa_srp-2.0.0b2/aasrp/templates/aasrp/modals/view-requests/accept-request.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/templates/aasrp/modals/view-requests/delete-request.html` & `aa_srp-2.0.0b2/aasrp/templates/aasrp/modals/view-requests/delete-request.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/templates/aasrp/modals/view-requests/mark-complete.html` & `aa_srp-2.0.0b2/aasrp/templates/aasrp/modals/view-requests/mark-complete.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/templates/aasrp/modals/view-requests/reject-request.html` & `aa_srp-2.0.0b2/aasrp/templates/aasrp/modals/view-requests/reject-request.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/templates/aasrp/modals/view-requests/request-details.html` & `aa_srp-2.0.0b2/aasrp/templates/aasrp/modals/view-requests/request-details.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/templates/aasrp/partials/dashboard/navigation.html` & `aa_srp-2.0.0b2/aasrp/templates/aasrp/partials/dashboard/navigation.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/templates/aasrp/partials/dashboard/srp-links.html` & `aa_srp-2.0.0b2/aasrp/templates/aasrp/partials/dashboard/srp-links.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/templates/aasrp/partials/dashboard/tabs-navigation.html` & `aa_srp-2.0.0b2/aasrp/templates/aasrp/partials/dashboard/tabs-navigation.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/templates/aasrp/partials/dashboard/user-settings.html` & `aa_srp-2.0.0b2/aasrp/templates/aasrp/partials/dashboard/user-settings.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/templates/aasrp/partials/dashboard/user-srp-requests.html` & `aa_srp-2.0.0b2/aasrp/templates/aasrp/partials/dashboard/user-srp-requests.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/templates/aasrp/partials/link-add/form.html` & `aa_srp-2.0.0b2/aasrp/templates/aasrp/partials/link-add/form.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/templates/aasrp/partials/link-edit/form.html` & `aa_srp-2.0.0b2/aasrp/templates/aasrp/partials/link-edit/form.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/templates/aasrp/partials/request-srp/fleet-details.html` & `aa_srp-2.0.0b2/aasrp/templates/aasrp/partials/request-srp/fleet-details.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/templates/aasrp/partials/request-srp/form.html` & `aa_srp-2.0.0b2/aasrp/templates/aasrp/partials/request-srp/form.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/templates/aasrp/partials/view-requests/overview.html` & `aa_srp-2.0.0b2/aasrp/templates/aasrp/partials/view-requests/overview.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/templates/aasrp/partials/view-requests/requests.html` & `aa_srp-2.0.0b2/aasrp/templates/aasrp/partials/view-requests/requests.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/templatetags/aasrp.py` & `aa_srp-2.0.0b2/aasrp/templatetags/aasrp.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/tests/test_access.py` & `aa_srp-2.0.0b2/aasrp/tests/test_access.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/tests/test_auth_hooks.py` & `aa_srp-2.0.0b2/aasrp/tests/test_auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/tests/test_helper_character.py` & `aa_srp-2.0.0b2/aasrp/tests/test_helper_character.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/tests/test_installed_modules.py` & `aa_srp-2.0.0b2/aasrp/tests/test_installed_modules.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/tests/test_model_setting.py` & `aa_srp-2.0.0b2/aasrp/tests/test_model_setting.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/tests/test_templatetags.py` & `aa_srp-2.0.0b2/aasrp/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/tests/utils.py` & `aa_srp-2.0.0b2/aasrp/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/views/ajax.py` & `aa_srp-2.0.0b2/aasrp/views/ajax.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/aasrp/views/general.py` & `aa_srp-2.0.0b2/aasrp/views/general.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/LICENSE` & `aa_srp-2.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/README.md` & `aa_srp-2.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.0b1/pyproject.toml` & `aa_srp-2.0.0b2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 authors = [
     { name = "Peter Pfeufer", email = "develop@ppfeufer.de" },
 ]
 requires-python = ">=3.8"
 classifiers = [
     "Environment :: Web Environment",
     "Framework :: Django",
-    "Framework :: Django :: 4.0",
+    "Framework :: Django :: 4.2",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
```

### Comparing `aa_srp-2.0.0b1/PKG-INFO` & `aa_srp-2.0.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-srp
-Version: 2.0.0b1
+Version: 2.0.0b2
 Summary: Improved SRP Module for Alliance Auth
 Project-URL: Changelog, https://github.com/ppfeufer/aa-srp/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://github.com/ppfeufer/aa-srp/blob/master/README.md
 Project-URL: Donations, https://ko-fi.com/ppfeufer
 Project-URL: Homepage, https://github.com/ppfeufer/aa-srp
 Project-URL: Source, https://github.com/ppfeufer/aa-srp.git
 Project-URL: Tracker, https://github.com/ppfeufer/aa-srp/issues
@@ -683,15 +683,15 @@
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
 License-File: LICENSE
 Keywords: allianceauth,eveonline,ship_replacement
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

