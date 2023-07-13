# Comparing `tmp/aa_moonmining-1.9.2.tar.gz` & `tmp/aa_moonmining-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "aa_moonmining-1.9.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aa_moonmining-1.9.2.tar` & `aa_moonmining-1.9.3.tar`

### file list

```diff
@@ -1,125 +1,124 @@
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/__init__.py
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/admin.py
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/app_settings.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/apps.py
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/auth_hooks.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/constants.py
--rw-r--r--   0        0        0     3487 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/core.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/forms.py
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/helpers.py
--rw-r--r--   0        0        0    14543 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/managers.py
--rw-r--r--   0        0        0    57269 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/models.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/providers.py
--rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/tasks.py
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/urls.py
--rw-r--r--   0        0        0    38642 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/views.py
--rw-r--r--   0        0        0    19771 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/locale/django.pot
--rw-r--r--   0        0        0    19818 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    19818 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    19818 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    19771 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    19771 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    19811 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    19771 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    19962 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    20049 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    19811 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/management/commands/__init__.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/management/commands/moonmining_calculate_all.py
--rw-r--r--   0        0        0     7966 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/management/commands/moonmining_import_moons.py
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/management/commands/moonmining_load_eve.py
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/management/commands/moonstuff_export_moons.py
--rw-r--r--   0        0        0    17813 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/migrations/0001_initial.py
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/migrations/0002_add_mining_ledger.py
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/migrations/0003_mining_ledger_reports.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/migrations/0004_add_permission_moon_ledgers.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/migrations/0005_make_pricing_more_flexible.py
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/migrations/0006_add_labels.py
--rw-r--r--   0        0        0     6352 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/migrations/0007_add_localization.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/migrations/__init__.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/static/moonmining/css/extractions.css
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/static/moonmining/css/global.css
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/static/moonmining/css/moonmining.css
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/static/moonmining/css/moons.css
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/static/moonmining/css/reports.css
--rw-r--r--   0        0        0    43262 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/static/moonmining/img/Spinner-1s-64px-dark.gif
--rw-r--r--   0        0        0    43381 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/static/moonmining/img/Spinner-1s-64px-light.gif
--rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/static/moonmining/vendor/datatables/plugins/dataTables.rowGroup.min.js
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/static/moonmining/vendor/datatables/plugins/datetime.js
--rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/static/moonmining/vendor/datatables/plugins/filterDropDown.min.js
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/static/moonmining/vendor/datatables/plugins/rowGroup.bootstrap.min.css
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/static/moonmining/vendor/datatables/plugins/rowGroup.dataTables.min.css
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/templates/moonmining/_generic_modal_page.html
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/templates/moonmining/base.html
--rw-r--r--   0        0        0     6454 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/templates/moonmining/extractions.html
--rw-r--r--   0        0        0     8877 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/templates/moonmining/moons.html
--rw-r--r--   0        0        0    10101 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/templates/moonmining/reports.html
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/templates/moonmining/tests.html
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/templates/moonmining/modals/base.html
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/templates/moonmining/modals/content_base.html
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/templates/moonmining/modals/extraction_details.html
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/templates/moonmining/modals/extraction_ledger.html
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/templates/moonmining/modals/loader_body.html
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/templates/moonmining/modals/moon_details.html
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/templates/moonmining/modals/upload_survey.html
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/templates/moonmining/partials/extraction_details.html
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/templates/moonmining/partials/extraction_details_head.html
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/templates/moonmining/partials/extraction_details_head_base.html
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/templates/moonmining/partials/extraction_details_products.html
--rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/templates/moonmining/partials/extraction_ledger.html
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/templates/moonmining/partials/extraction_ledger_characters.html
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/templates/moonmining/partials/extraction_ledger_head.html
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/templates/moonmining/partials/extraction_ledger_ledger.html
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/templates/moonmining/partials/extractions_tab.html
--rw-r--r--   0        0        0     3432 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/templates/moonmining/partials/global_js.html
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/templates/moonmining/partials/location.html
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/templates/moonmining/partials/menu.html
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/templates/moonmining/partials/moon_details.html
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/templates/moonmining/partials/moon_details_moon.html
--rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/templates/moonmining/partials/moon_details_products.html
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/templates/moonmining/partials/moons_tab.html
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/templates/moonmining/partials/reports_ore_prices_tab.html
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/templates/moonmining/partials/reports_owned_value_tab.html
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/templates/moonmining/partials/reports_user_mining_tab.html
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/templates/moonmining/partials/reports_user_uploaded_tab.html
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/templates/moonmining/partials/upload_survey.html
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/templates/moonmining/partials/value_estimate_legend.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/templatetags/__init__.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/templatetags/moonmining.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/tests/__init__.py
--rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/tests/helpers.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/tests/test_admin.py
--rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/tests/test_commands.py
--rw-r--r--   0        0        0     4258 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/tests/test_core.py
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/tests/test_helpers.py
--rw-r--r--   0        0        0     8354 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/tests/test_integration.py
--rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/tests/test_managers.py
--rw-r--r--   0        0        0    47598 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/tests/test_models.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/tests/test_templatetags.py
--rw-r--r--   0        0        0    26354 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/tests/test_views.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/tests/testdata/__init__.py
--rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/tests/testdata/allianceauth.json
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/tests/testdata/create_eveuniverse.py
--rw-r--r--   0        0        0    29013 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/tests/testdata/esi.json
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/tests/testdata/esi_client_stub.py
--rw-r--r--   0        0        0  1283587 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/tests/testdata/eveuniverse.json
--rw-r--r--   0        0        0    17156 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/tests/testdata/factories.py
--rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/tests/testdata/generate_many_moons.py
--rw-r--r--   0        0        0    99565 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/tests/testdata/generate_moons.json
--rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/tests/testdata/generate_moons.py
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/tests/testdata/load_allianceauth.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/tests/testdata/load_eveuniverse.py
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/tests/testdata/moon_ids.csv
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/tests/testdata/moon_survey_input_2.txt
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/tests/testdata/moon_survey_input_3.txt
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/tests/testdata/moons_for_import.csv
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/tests/testdata/notification_details.py
--rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/tests/testdata/notifications_full.json
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/tests/testdata/survey_data.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/tools/drop_tables.sql
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/moonmining/tools/esi_notes.md
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/LICENSE
--rw-r--r--   0        0        0    13099 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/README.md
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/pyproject.toml
--rw-r--r--   0        0        0    14516 2020-02-02 00:00:00.000000 aa_moonmining-1.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-13 20:55:19.593872 aa_moonmining-1.9.3/LICENSE
+-rw-r--r--   0        0        0    13099 2023-07-13 20:55:19.593872 aa_moonmining-1.9.3/README.md
+-rw-r--r--   0        0        0      184 2023-07-13 20:55:19.593872 aa_moonmining-1.9.3/moonmining/__init__.py
+-rw-r--r--   0        0        0    11357 2023-07-13 20:55:19.593872 aa_moonmining-1.9.3/moonmining/admin.py
+-rw-r--r--   0        0        0     1438 2023-07-13 20:55:19.593872 aa_moonmining-1.9.3/moonmining/app_settings.py
+-rw-r--r--   0        0        0      204 2023-07-13 20:55:19.593872 aa_moonmining-1.9.3/moonmining/apps.py
+-rw-r--r--   0        0        0      775 2023-07-13 20:55:19.593872 aa_moonmining-1.9.3/moonmining/auth_hooks.py
+-rw-r--r--   0        0        0      882 2023-07-13 20:55:19.593872 aa_moonmining-1.9.3/moonmining/constants.py
+-rw-r--r--   0        0        0     3487 2023-07-13 20:55:19.593872 aa_moonmining-1.9.3/moonmining/core.py
+-rw-r--r--   0        0        0      109 2023-07-13 20:55:19.593872 aa_moonmining-1.9.3/moonmining/forms.py
+-rw-r--r--   0        0        0     1623 2023-07-13 20:55:19.593872 aa_moonmining-1.9.3/moonmining/helpers.py
+-rw-r--r--   0        0        0    19818 2023-07-13 20:55:19.597872 aa_moonmining-1.9.3/moonmining/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    19771 2023-07-13 20:55:19.597872 aa_moonmining-1.9.3/moonmining/locale/django.pot
+-rw-r--r--   0        0        0    19818 2023-07-13 20:55:19.597872 aa_moonmining-1.9.3/moonmining/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    19818 2023-07-13 20:55:19.597872 aa_moonmining-1.9.3/moonmining/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    19771 2023-07-13 20:55:19.597872 aa_moonmining-1.9.3/moonmining/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    19771 2023-07-13 20:55:19.597872 aa_moonmining-1.9.3/moonmining/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    19811 2023-07-13 20:55:19.597872 aa_moonmining-1.9.3/moonmining/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    19771 2023-07-13 20:55:19.597872 aa_moonmining-1.9.3/moonmining/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    19962 2023-07-13 20:55:19.597872 aa_moonmining-1.9.3/moonmining/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    20049 2023-07-13 20:55:19.597872 aa_moonmining-1.9.3/moonmining/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    19811 2023-07-13 20:55:19.597872 aa_moonmining-1.9.3/moonmining/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      102 2023-07-13 20:55:19.597872 aa_moonmining-1.9.3/moonmining/management/commands/__init__.py
+-rw-r--r--   0        0        0     1043 2023-07-13 20:55:19.597872 aa_moonmining-1.9.3/moonmining/management/commands/moonmining_calculate_all.py
+-rw-r--r--   0        0        0     7966 2023-07-13 20:55:19.597872 aa_moonmining-1.9.3/moonmining/management/commands/moonmining_import_moons.py
+-rw-r--r--   0        0        0     1516 2023-07-13 20:55:19.597872 aa_moonmining-1.9.3/moonmining/management/commands/moonmining_load_eve.py
+-rw-r--r--   0        0        0     1867 2023-07-13 20:55:19.597872 aa_moonmining-1.9.3/moonmining/management/commands/moonstuff_export_moons.py
+-rw-r--r--   0        0        0    14543 2023-07-13 20:55:19.597872 aa_moonmining-1.9.3/moonmining/managers.py
+-rw-r--r--   0        0        0    17813 2023-07-13 20:55:19.597872 aa_moonmining-1.9.3/moonmining/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2663 2023-07-13 20:55:19.597872 aa_moonmining-1.9.3/moonmining/migrations/0002_add_mining_ledger.py
+-rw-r--r--   0        0        0     2366 2023-07-13 20:55:19.597872 aa_moonmining-1.9.3/moonmining/migrations/0003_mining_ledger_reports.py
+-rw-r--r--   0        0        0     1041 2023-07-13 20:55:19.597872 aa_moonmining-1.9.3/moonmining/migrations/0004_add_permission_moon_ledgers.py
+-rw-r--r--   0        0        0     1508 2023-07-13 20:55:19.597872 aa_moonmining-1.9.3/moonmining/migrations/0005_make_pricing_more_flexible.py
+-rw-r--r--   0        0        0     1705 2023-07-13 20:55:19.597872 aa_moonmining-1.9.3/moonmining/migrations/0006_add_labels.py
+-rw-r--r--   0        0        0     6352 2023-07-13 20:55:19.597872 aa_moonmining-1.9.3/moonmining/migrations/0007_add_localization.py
+-rw-r--r--   0        0        0        0 2023-07-13 21:10:19.634745 aa_moonmining-1.9.3/moonmining/migrations/__init__.py
+-rw-r--r--   0        0        0    57269 2023-07-13 20:55:19.597872 aa_moonmining-1.9.3/moonmining/models.py
+-rw-r--r--   0        0        0      141 2023-07-13 20:55:19.597872 aa_moonmining-1.9.3/moonmining/providers.py
+-rw-r--r--   0        0        0      639 2023-07-13 20:55:19.597872 aa_moonmining-1.9.3/moonmining/static/moonmining/css/extractions.css
+-rw-r--r--   0        0        0     1306 2023-07-13 20:55:19.597872 aa_moonmining-1.9.3/moonmining/static/moonmining/css/global.css
+-rw-r--r--   0        0        0      722 2023-07-13 20:55:19.597872 aa_moonmining-1.9.3/moonmining/static/moonmining/css/moonmining.css
+-rw-r--r--   0        0        0      404 2023-07-13 20:55:19.597872 aa_moonmining-1.9.3/moonmining/static/moonmining/css/moons.css
+-rw-r--r--   0        0        0     1112 2023-07-13 20:55:19.597872 aa_moonmining-1.9.3/moonmining/static/moonmining/css/reports.css
+-rw-r--r--   0        0        0    43262 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/static/moonmining/img/Spinner-1s-64px-dark.gif
+-rw-r--r--   0        0        0    43381 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/static/moonmining/img/Spinner-1s-64px-light.gif
+-rw-r--r--   0        0        0     5573 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/static/moonmining/vendor/datatables/plugins/dataTables.rowGroup.min.js
+-rw-r--r--   0        0        0     3250 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/static/moonmining/vendor/datatables/plugins/datetime.js
+-rw-r--r--   0        0        0     2529 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/static/moonmining/vendor/datatables/plugins/filterDropDown.min.js
+-rw-r--r--   0        0        0      384 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/static/moonmining/vendor/datatables/plugins/rowGroup.bootstrap.min.css
+-rw-r--r--   0        0        0      384 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/static/moonmining/vendor/datatables/plugins/rowGroup.dataTables.min.css
+-rw-r--r--   0        0        0     6423 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/tasks.py
+-rw-r--r--   0        0        0      350 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/templates/moonmining/_generic_modal_page.html
+-rw-r--r--   0        0        0      869 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/templates/moonmining/base.html
+-rw-r--r--   0        0        0     6454 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/templates/moonmining/extractions.html
+-rw-r--r--   0        0        0      358 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/templates/moonmining/modals/base.html
+-rw-r--r--   0        0        0     1159 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/templates/moonmining/modals/content_base.html
+-rw-r--r--   0        0        0      290 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/templates/moonmining/modals/extraction_details.html
+-rw-r--r--   0        0        0      315 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/templates/moonmining/modals/extraction_ledger.html
+-rw-r--r--   0        0        0      247 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/templates/moonmining/modals/loader_body.html
+-rw-r--r--   0        0        0      260 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/templates/moonmining/modals/moon_details.html
+-rw-r--r--   0        0        0      185 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/templates/moonmining/modals/upload_survey.html
+-rw-r--r--   0        0        0     8877 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/templates/moonmining/moons.html
+-rw-r--r--   0        0        0      175 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/templates/moonmining/partials/extraction_details.html
+-rw-r--r--   0        0        0     2213 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/templates/moonmining/partials/extraction_details_head.html
+-rw-r--r--   0        0        0      649 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/templates/moonmining/partials/extraction_details_head_base.html
+-rw-r--r--   0        0        0     1974 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/templates/moonmining/partials/extraction_details_products.html
+-rw-r--r--   0        0        0     2327 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/templates/moonmining/partials/extraction_ledger.html
+-rw-r--r--   0        0        0     2302 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/templates/moonmining/partials/extraction_ledger_characters.html
+-rw-r--r--   0        0        0     1103 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/templates/moonmining/partials/extraction_ledger_head.html
+-rw-r--r--   0        0        0     2779 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/templates/moonmining/partials/extraction_ledger_ledger.html
+-rw-r--r--   0        0        0     1195 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/templates/moonmining/partials/extractions_tab.html
+-rw-r--r--   0        0        0     3432 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/templates/moonmining/partials/global_js.html
+-rw-r--r--   0        0        0      624 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/templates/moonmining/partials/location.html
+-rw-r--r--   0        0        0     2540 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/templates/moonmining/partials/menu.html
+-rw-r--r--   0        0        0      162 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/templates/moonmining/partials/moon_details.html
+-rw-r--r--   0        0        0     1452 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/templates/moonmining/partials/moon_details_moon.html
+-rw-r--r--   0        0        0     2538 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/templates/moonmining/partials/moon_details_products.html
+-rw-r--r--   0        0        0     1197 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/templates/moonmining/partials/moons_tab.html
+-rw-r--r--   0        0        0     1243 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/templates/moonmining/partials/reports_ore_prices_tab.html
+-rw-r--r--   0        0        0     1417 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/templates/moonmining/partials/reports_owned_value_tab.html
+-rw-r--r--   0        0        0     2253 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/templates/moonmining/partials/reports_user_mining_tab.html
+-rw-r--r--   0        0        0      897 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/templates/moonmining/partials/reports_user_uploaded_tab.html
+-rw-r--r--   0        0        0      537 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/templates/moonmining/partials/upload_survey.html
+-rw-r--r--   0        0        0      351 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/templates/moonmining/partials/value_estimate_legend.html
+-rw-r--r--   0        0        0    10101 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/templates/moonmining/reports.html
+-rw-r--r--   0        0        0     1041 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/templates/moonmining/tests.html
+-rw-r--r--   0        0        0        0 2023-07-13 21:10:19.642745 aa_moonmining-1.9.3/moonmining/templatetags/__init__.py
+-rw-r--r--   0        0        0     1085 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/templatetags/moonmining.py
+-rw-r--r--   0        0        0        0 2023-07-13 21:10:19.642745 aa_moonmining-1.9.3/moonmining/tests/__init__.py
+-rw-r--r--   0        0        0     3462 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/tests/helpers.py
+-rw-r--r--   0        0        0      581 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/tests/test_admin.py
+-rw-r--r--   0        0        0     3440 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/tests/test_commands.py
+-rw-r--r--   0        0        0     4258 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/tests/test_core.py
+-rw-r--r--   0        0        0     1438 2023-07-13 20:55:19.601873 aa_moonmining-1.9.3/moonmining/tests/test_helpers.py
+-rw-r--r--   0        0        0     8354 2023-07-13 20:55:19.605872 aa_moonmining-1.9.3/moonmining/tests/test_integration.py
+-rw-r--r--   0        0        0     7242 2023-07-13 20:55:19.605872 aa_moonmining-1.9.3/moonmining/tests/test_managers.py
+-rw-r--r--   0        0        0    47598 2023-07-13 20:55:19.605872 aa_moonmining-1.9.3/moonmining/tests/test_models.py
+-rw-r--r--   0        0        0     1611 2023-07-13 20:55:19.605872 aa_moonmining-1.9.3/moonmining/tests/test_templatetags.py
+-rw-r--r--   0        0        0    26354 2023-07-13 20:55:19.605872 aa_moonmining-1.9.3/moonmining/tests/test_views.py
+-rw-r--r--   0        0        0      173 2023-07-13 20:55:19.605872 aa_moonmining-1.9.3/moonmining/tests/testdata/__init__.py
+-rw-r--r--   0        0        0     3687 2023-07-13 20:55:19.605872 aa_moonmining-1.9.3/moonmining/tests/testdata/allianceauth.json
+-rw-r--r--   0        0        0     1340 2023-07-13 20:55:19.605872 aa_moonmining-1.9.3/moonmining/tests/testdata/create_eveuniverse.py
+-rw-r--r--   0        0        0    29013 2023-07-13 20:55:19.605872 aa_moonmining-1.9.3/moonmining/tests/testdata/esi.json
+-rw-r--r--   0        0        0     1373 2023-07-13 20:55:19.605872 aa_moonmining-1.9.3/moonmining/tests/testdata/esi_client_stub.py
+-rw-r--r--   0        0        0  1283587 2023-07-13 20:55:19.609873 aa_moonmining-1.9.3/moonmining/tests/testdata/eveuniverse.json
+-rw-r--r--   0        0        0    17156 2023-07-13 20:55:19.609873 aa_moonmining-1.9.3/moonmining/tests/testdata/factories.py
+-rw-r--r--   0        0        0     2562 2023-07-13 20:55:19.609873 aa_moonmining-1.9.3/moonmining/tests/testdata/generate_many_moons.py
+-rw-r--r--   0        0        0    99565 2023-07-13 20:55:19.609873 aa_moonmining-1.9.3/moonmining/tests/testdata/generate_moons.json
+-rw-r--r--   0        0        0     6596 2023-07-13 20:55:19.609873 aa_moonmining-1.9.3/moonmining/tests/testdata/generate_moons.py
+-rw-r--r--   0        0        0     2452 2023-07-13 20:55:19.609873 aa_moonmining-1.9.3/moonmining/tests/testdata/load_allianceauth.py
+-rw-r--r--   0        0        0     1078 2023-07-13 20:55:19.609873 aa_moonmining-1.9.3/moonmining/tests/testdata/load_eveuniverse.py
+-rw-r--r--   0        0        0    50000 2023-07-13 20:55:19.609873 aa_moonmining-1.9.3/moonmining/tests/testdata/moon_ids.csv
+-rw-r--r--   0        0        0      525 2023-07-13 20:55:19.609873 aa_moonmining-1.9.3/moonmining/tests/testdata/moon_survey_input_2.txt
+-rw-r--r--   0        0        0      335 2023-07-13 20:55:19.609873 aa_moonmining-1.9.3/moonmining/tests/testdata/moon_survey_input_3.txt
+-rw-r--r--   0        0        0      195 2023-07-13 20:55:19.609873 aa_moonmining-1.9.3/moonmining/tests/testdata/moons_for_import.csv
+-rw-r--r--   0        0        0      779 2023-07-13 20:55:19.609873 aa_moonmining-1.9.3/moonmining/tests/testdata/notification_details.py
+-rw-r--r--   0        0        0     4033 2023-07-13 20:55:19.609873 aa_moonmining-1.9.3/moonmining/tests/testdata/notifications_full.json
+-rw-r--r--   0        0        0      436 2023-07-13 20:55:19.609873 aa_moonmining-1.9.3/moonmining/tests/testdata/survey_data.py
+-rw-r--r--   0        0        0      460 2023-07-13 20:55:19.609873 aa_moonmining-1.9.3/moonmining/tools/drop_tables.sql
+-rw-r--r--   0        0        0      391 2023-07-13 20:55:19.609873 aa_moonmining-1.9.3/moonmining/tools/esi_notes.md
+-rw-r--r--   0        0        0     1837 2023-07-13 20:55:19.609873 aa_moonmining-1.9.3/moonmining/urls.py
+-rw-r--r--   0        0        0    38642 2023-07-13 20:55:19.609873 aa_moonmining-1.9.3/moonmining/views.py
+-rw-r--r--   0        0        0     1926 2023-07-13 20:55:19.609873 aa_moonmining-1.9.3/pyproject.toml
+-rw-r--r--   0        0        0    14473 1970-01-01 00:00:00.000000 aa_moonmining-1.9.3/PKG-INFO
```

### Comparing `aa_moonmining-1.9.2/moonmining/admin.py` & `aa_moonmining-1.9.3/moonmining/admin.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/app_settings.py` & `aa_moonmining-1.9.3/moonmining/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/auth_hooks.py` & `aa_moonmining-1.9.3/moonmining/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/constants.py` & `aa_moonmining-1.9.3/moonmining/constants.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/core.py` & `aa_moonmining-1.9.3/moonmining/core.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/helpers.py` & `aa_moonmining-1.9.3/moonmining/helpers.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/managers.py` & `aa_moonmining-1.9.3/moonmining/managers.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/models.py` & `aa_moonmining-1.9.3/moonmining/models.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/tasks.py` & `aa_moonmining-1.9.3/moonmining/tasks.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/urls.py` & `aa_moonmining-1.9.3/moonmining/urls.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/views.py` & `aa_moonmining-1.9.3/moonmining/views.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/locale/django.pot` & `aa_moonmining-1.9.3/moonmining/locale/django.pot`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/locale/de/LC_MESSAGES/django.po` & `aa_moonmining-1.9.3/moonmining/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/locale/en/LC_MESSAGES/django.po` & `aa_moonmining-1.9.3/moonmining/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/locale/es/LC_MESSAGES/django.po` & `aa_moonmining-1.9.3/moonmining/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/locale/fr_FR/LC_MESSAGES/django.po` & `aa_moonmining-1.9.3/moonmining/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/locale/it_IT/LC_MESSAGES/django.po` & `aa_moonmining-1.9.3/moonmining/locale/it_IT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/locale/ja/LC_MESSAGES/django.po` & `aa_moonmining-1.9.3/moonmining/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/locale/ko_KR/LC_MESSAGES/django.po` & `aa_moonmining-1.9.3/moonmining/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/locale/ru/LC_MESSAGES/django.po` & `aa_moonmining-1.9.3/moonmining/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/locale/uk/LC_MESSAGES/django.po` & `aa_moonmining-1.9.3/moonmining/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_moonmining-1.9.3/moonmining/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/management/commands/moonmining_calculate_all.py` & `aa_moonmining-1.9.3/moonmining/management/commands/moonmining_calculate_all.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/management/commands/moonmining_import_moons.py` & `aa_moonmining-1.9.3/moonmining/management/commands/moonmining_import_moons.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/management/commands/moonmining_load_eve.py` & `aa_moonmining-1.9.3/moonmining/management/commands/moonmining_load_eve.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/management/commands/moonstuff_export_moons.py` & `aa_moonmining-1.9.3/moonmining/management/commands/moonstuff_export_moons.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/migrations/0001_initial.py` & `aa_moonmining-1.9.3/moonmining/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/migrations/0002_add_mining_ledger.py` & `aa_moonmining-1.9.3/moonmining/migrations/0002_add_mining_ledger.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/migrations/0003_mining_ledger_reports.py` & `aa_moonmining-1.9.3/moonmining/migrations/0003_mining_ledger_reports.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/migrations/0004_add_permission_moon_ledgers.py` & `aa_moonmining-1.9.3/moonmining/migrations/0004_add_permission_moon_ledgers.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/migrations/0005_make_pricing_more_flexible.py` & `aa_moonmining-1.9.3/moonmining/migrations/0005_make_pricing_more_flexible.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/migrations/0006_add_labels.py` & `aa_moonmining-1.9.3/moonmining/migrations/0006_add_labels.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/migrations/0007_add_localization.py` & `aa_moonmining-1.9.3/moonmining/migrations/0007_add_localization.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/static/moonmining/css/extractions.css` & `aa_moonmining-1.9.3/moonmining/static/moonmining/css/extractions.css`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/static/moonmining/css/global.css` & `aa_moonmining-1.9.3/moonmining/static/moonmining/css/global.css`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/static/moonmining/css/moonmining.css` & `aa_moonmining-1.9.3/moonmining/static/moonmining/css/moonmining.css`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/static/moonmining/css/reports.css` & `aa_moonmining-1.9.3/moonmining/static/moonmining/css/reports.css`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/static/moonmining/img/Spinner-1s-64px-dark.gif` & `aa_moonmining-1.9.3/moonmining/static/moonmining/img/Spinner-1s-64px-dark.gif`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/static/moonmining/img/Spinner-1s-64px-light.gif` & `aa_moonmining-1.9.3/moonmining/static/moonmining/img/Spinner-1s-64px-light.gif`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/static/moonmining/vendor/datatables/plugins/dataTables.rowGroup.min.js` & `aa_moonmining-1.9.3/moonmining/static/moonmining/vendor/datatables/plugins/dataTables.rowGroup.min.js`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/static/moonmining/vendor/datatables/plugins/datetime.js` & `aa_moonmining-1.9.3/moonmining/static/moonmining/vendor/datatables/plugins/datetime.js`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/static/moonmining/vendor/datatables/plugins/filterDropDown.min.js` & `aa_moonmining-1.9.3/moonmining/static/moonmining/vendor/datatables/plugins/filterDropDown.min.js`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/templates/moonmining/base.html` & `aa_moonmining-1.9.3/moonmining/templates/moonmining/base.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/templates/moonmining/extractions.html` & `aa_moonmining-1.9.3/moonmining/templates/moonmining/extractions.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/templates/moonmining/moons.html` & `aa_moonmining-1.9.3/moonmining/templates/moonmining/moons.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/templates/moonmining/reports.html` & `aa_moonmining-1.9.3/moonmining/templates/moonmining/reports.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/templates/moonmining/tests.html` & `aa_moonmining-1.9.3/moonmining/templates/moonmining/tests.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/templates/moonmining/modals/content_base.html` & `aa_moonmining-1.9.3/moonmining/templates/moonmining/modals/content_base.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/templates/moonmining/partials/extraction_details_head.html` & `aa_moonmining-1.9.3/moonmining/templates/moonmining/partials/extraction_details_head.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/templates/moonmining/partials/extraction_details_head_base.html` & `aa_moonmining-1.9.3/moonmining/templates/moonmining/partials/extraction_details_head_base.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/templates/moonmining/partials/extraction_details_products.html` & `aa_moonmining-1.9.3/moonmining/templates/moonmining/partials/extraction_details_products.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/templates/moonmining/partials/extraction_ledger.html` & `aa_moonmining-1.9.3/moonmining/templates/moonmining/partials/extraction_ledger.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/templates/moonmining/partials/extraction_ledger_characters.html` & `aa_moonmining-1.9.3/moonmining/templates/moonmining/partials/extraction_ledger_characters.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/templates/moonmining/partials/extraction_ledger_head.html` & `aa_moonmining-1.9.3/moonmining/templates/moonmining/partials/extraction_ledger_head.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/templates/moonmining/partials/extraction_ledger_ledger.html` & `aa_moonmining-1.9.3/moonmining/templates/moonmining/partials/extraction_ledger_ledger.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/templates/moonmining/partials/extractions_tab.html` & `aa_moonmining-1.9.3/moonmining/templates/moonmining/partials/extractions_tab.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/templates/moonmining/partials/global_js.html` & `aa_moonmining-1.9.3/moonmining/templates/moonmining/partials/global_js.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/templates/moonmining/partials/location.html` & `aa_moonmining-1.9.3/moonmining/templates/moonmining/partials/location.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/templates/moonmining/partials/menu.html` & `aa_moonmining-1.9.3/moonmining/templates/moonmining/partials/menu.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/templates/moonmining/partials/moon_details_moon.html` & `aa_moonmining-1.9.3/moonmining/templates/moonmining/partials/moon_details_moon.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/templates/moonmining/partials/moon_details_products.html` & `aa_moonmining-1.9.3/moonmining/templates/moonmining/partials/moon_details_products.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/templates/moonmining/partials/moons_tab.html` & `aa_moonmining-1.9.3/moonmining/templates/moonmining/partials/moons_tab.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/templates/moonmining/partials/reports_ore_prices_tab.html` & `aa_moonmining-1.9.3/moonmining/templates/moonmining/partials/reports_ore_prices_tab.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/templates/moonmining/partials/reports_owned_value_tab.html` & `aa_moonmining-1.9.3/moonmining/templates/moonmining/partials/reports_owned_value_tab.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/templates/moonmining/partials/reports_user_mining_tab.html` & `aa_moonmining-1.9.3/moonmining/templates/moonmining/partials/reports_user_mining_tab.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/templates/moonmining/partials/reports_user_uploaded_tab.html` & `aa_moonmining-1.9.3/moonmining/templates/moonmining/partials/reports_user_uploaded_tab.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/templates/moonmining/partials/upload_survey.html` & `aa_moonmining-1.9.3/moonmining/templates/moonmining/partials/upload_survey.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/templatetags/moonmining.py` & `aa_moonmining-1.9.3/moonmining/templatetags/moonmining.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/tests/helpers.py` & `aa_moonmining-1.9.3/moonmining/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/tests/test_admin.py` & `aa_moonmining-1.9.3/moonmining/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/tests/test_commands.py` & `aa_moonmining-1.9.3/moonmining/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/tests/test_core.py` & `aa_moonmining-1.9.3/moonmining/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/tests/test_helpers.py` & `aa_moonmining-1.9.3/moonmining/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/tests/test_integration.py` & `aa_moonmining-1.9.3/moonmining/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/tests/test_managers.py` & `aa_moonmining-1.9.3/moonmining/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/tests/test_models.py` & `aa_moonmining-1.9.3/moonmining/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/tests/test_templatetags.py` & `aa_moonmining-1.9.3/moonmining/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/tests/test_views.py` & `aa_moonmining-1.9.3/moonmining/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/tests/testdata/allianceauth.json` & `aa_moonmining-1.9.3/moonmining/tests/testdata/allianceauth.json`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/tests/testdata/create_eveuniverse.py` & `aa_moonmining-1.9.3/moonmining/tests/testdata/create_eveuniverse.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/tests/testdata/esi.json` & `aa_moonmining-1.9.3/moonmining/tests/testdata/esi.json`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/tests/testdata/esi_client_stub.py` & `aa_moonmining-1.9.3/moonmining/tests/testdata/esi_client_stub.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/tests/testdata/eveuniverse.json` & `aa_moonmining-1.9.3/moonmining/tests/testdata/eveuniverse.json`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/tests/testdata/factories.py` & `aa_moonmining-1.9.3/moonmining/tests/testdata/factories.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/tests/testdata/generate_many_moons.py` & `aa_moonmining-1.9.3/moonmining/tests/testdata/generate_many_moons.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/tests/testdata/generate_moons.json` & `aa_moonmining-1.9.3/moonmining/tests/testdata/generate_moons.json`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/tests/testdata/generate_moons.py` & `aa_moonmining-1.9.3/moonmining/tests/testdata/generate_moons.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/tests/testdata/load_allianceauth.py` & `aa_moonmining-1.9.3/moonmining/tests/testdata/load_allianceauth.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/tests/testdata/load_eveuniverse.py` & `aa_moonmining-1.9.3/moonmining/tests/testdata/load_eveuniverse.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/tests/testdata/moon_ids.csv` & `aa_moonmining-1.9.3/moonmining/tests/testdata/moon_ids.csv`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/tests/testdata/moon_survey_input_2.txt` & `aa_moonmining-1.9.3/moonmining/tests/testdata/moon_survey_input_2.txt`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/tests/testdata/notification_details.py` & `aa_moonmining-1.9.3/moonmining/tests/testdata/notification_details.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/moonmining/tests/testdata/notifications_full.json` & `aa_moonmining-1.9.3/moonmining/tests/testdata/notifications_full.json`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/LICENSE` & `aa_moonmining-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/README.md` & `aa_moonmining-1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.2/pyproject.toml` & `aa_moonmining-1.9.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 [build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
+requires = ["flit_core >=3.2,<4"]
+build-backend = "flit_core.buildapi"
 
 [project]
 name = "aa-moonmining"
-dynamic = ["version"]
-description = "Alliance Auth app for tracking moon extractions and scouting new moons."
+dynamic = ["version", "description"]
 readme = "README.md"
-license = "MIT"
+license = {file = "LICENSE"}
 requires-python = ">=3.8"
 authors = [
     { name = "Erik Kalkoken", email = "kaloken87@gmail.com" },
 ]
 classifiers = [
     "Environment :: Web Environment",
     "Framework :: Django",
@@ -24,36 +23,30 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
 ]
 dependencies = [
     "allianceauth-app-utils>=1.18",
-    "allianceauth>=3",
+    "allianceauth>=3.2",
     "django-bootstrap-form",
     "django-datatables-view>=1.20",
     "django-eveuniverse>=1.0",
     "django-navhelper",
     "PyYAML",
 ]
 
 [project.urls]
 Homepage = "https://gitlab.com/ErikKalkoken/aa-moonmining"
 Source = "https://gitlab.com/ErikKalkoken/aa-moonmining"
 Changelog = "https://gitlab.com/ErikKalkoken/aa-moonmining/-/blob/master/CHANGELOG.md"
 Tracker = "https://gitlab.com/ErikKalkoken/aa-moonmining/-/issues"
 
-
-[tool.hatch.version]
-path = "moonmining/__init__.py"
-
-[tool.hatch.build]
-include = [
-    "/moonmining",
-]
+[tool.flit.module]
+name = "moonmining"
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 sections = [
     "FUTURE",
     "STDLIB",
```

### Comparing `aa_moonmining-1.9.2/PKG-INFO` & `aa_moonmining-1.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 Metadata-Version: 2.1
 Name: aa-moonmining
-Version: 1.9.2
+Version: 1.9.3
 Summary: Alliance Auth app for tracking moon extractions and scouting new moons.
-Project-URL: Homepage, https://gitlab.com/ErikKalkoken/aa-moonmining
-Project-URL: Source, https://gitlab.com/ErikKalkoken/aa-moonmining
-Project-URL: Changelog, https://gitlab.com/ErikKalkoken/aa-moonmining/-/blob/master/CHANGELOG.md
-Project-URL: Tracker, https://gitlab.com/ErikKalkoken/aa-moonmining/-/issues
 Author-email: Erik Kalkoken <kaloken87@gmail.com>
-License-Expression: MIT
-License-File: LICENSE
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: >=3.8
 Requires-Dist: allianceauth-app-utils>=1.18
-Requires-Dist: allianceauth>=3
+Requires-Dist: allianceauth>=3.2
 Requires-Dist: django-bootstrap-form
 Requires-Dist: django-datatables-view>=1.20
 Requires-Dist: django-eveuniverse>=1.0
 Requires-Dist: django-navhelper
-Requires-Dist: pyyaml
-Description-Content-Type: text/markdown
+Requires-Dist: PyYAML
+Project-URL: Changelog, https://gitlab.com/ErikKalkoken/aa-moonmining/-/blob/master/CHANGELOG.md
+Project-URL: Homepage, https://gitlab.com/ErikKalkoken/aa-moonmining
+Project-URL: Source, https://gitlab.com/ErikKalkoken/aa-moonmining
+Project-URL: Tracker, https://gitlab.com/ErikKalkoken/aa-moonmining/-/issues
 
 # Moon Mining
 
 An Alliance Auth app for tracking moon extractions and scouting new moons.
 
 [![release](https://img.shields.io/pypi/v/aa-moonmining?label=release)](https://pypi.org/project/aa-moonmining/)
 [![python](https://img.shields.io/pypi/pyversions/aa-moonmining)](https://pypi.org/project/aa-moonmining/)
@@ -285,7 +283,8 @@
 
 - Q: How are the prices and values of ores calculated?
 - A: All ore prices are **average prices** (not Jita prices), which are the current average price of an item accross all of New Eden and the same that the in-game client is showing, e.g. for price estimates when scheduling an extraction.
 
 ## History
 
 This project started as a fork from [aa-moonstuff](https://gitlab.com/colcrunch/aa-moonstuff) in 2019, but as diverged heavily since then through two major iterations. The first iteration was called Moon Planner and used internally. It had a very different data model build upon [allianceauth-evesde](https://gitlab.com/ErikKalkoken/allianceauth-evesde). The current version is the second iteration and is build upon [django-eveuniverse](https://gitlab.com/ErikKalkoken/django-eveuniverse). Nevertheless, we like to take the opportunity to thank @colcrunch for providing a great starting point with moonstuff.
+
```

