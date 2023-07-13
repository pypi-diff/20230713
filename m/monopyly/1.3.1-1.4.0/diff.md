# Comparing `tmp/monopyly-1.3.1.tar.gz` & `tmp/monopyly-1.4.0.tar.gz`

## Comparing `monopyly-1.3.1.tar` & `monopyly-1.4.0.tar`

### file list

```diff
@@ -1,198 +1,201 @@
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 monopyly-1.3.1/README.md -> monopyly/README.md
--rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/README.md
--rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/_version.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/auth/actions.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/auth/blueprint.py
--rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/auth/routes.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/auth/tools.py
--rw-r--r--   0        0        0     9837 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/banking/accounts.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/banking/actions.py
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/banking/banks.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/banking/blueprint.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/banking/filters.py
--rw-r--r--   0        0        0    10504 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/banking/forms.py
--rw-r--r--   0        0        0     8092 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/banking/routes.py
--rw-r--r--   0        0        0     8453 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/banking/transactions.py
--rwxr-xr-x   0        0        0     3031 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/cli/run.py
--rw-r--r--   0        0        0    12194 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/common/transactions.py
--rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/common/utils.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/common/forms/__init__.py
--rw-r--r--   0        0        0     7811 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/common/forms/_forms.py
--rw-r--r--   0        0        0     3793 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/common/forms/fields.py
--rw-r--r--   0        0        0     5685 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/common/forms/utils.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/common/forms/validators.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/config/__init__.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/config/default_settings.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/config/settings.py
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/core/actions.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/core/blueprint.py
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/core/context_processors.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/core/filters.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/core/internal_transactions.py
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/core/routes.py
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/credit/accounts.py
--rw-r--r--   0        0        0     5333 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/credit/actions.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/credit/blueprint.py
--rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/credit/cards.py
--rw-r--r--   0        0        0    12008 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/credit/forms.py
--rw-r--r--   0        0        0    18264 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/credit/routes.py
--rw-r--r--   0        0        0     6495 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/credit/statements.py
--rw-r--r--   0        0        0     8767 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/credit/transactions.py
--rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/database/__init__.py
--rw-r--r--   0        0        0    14568 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/database/models.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/database/preloads.sql
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/database/schema.sql
--rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/database/views.sql
--rw-r--r--   0        0        0    87462 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/jquery-3.7.0.min.js
--rw-r--r--   0        0        0    47401 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/css/style.css
--rwxr-xr-x   0        0        0      315 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/favicon/browserconfig.xml
--rwxr-xr-x   0        0        0    20601 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/favicon/favicon-114.png
--rwxr-xr-x   0        0        0    22077 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/favicon/favicon-120.png
--rwxr-xr-x   0        0        0    29107 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/favicon/favicon-144.png
--rwxr-xr-x   0        0        0    30832 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/favicon/favicon-150.png
--rwxr-xr-x   0        0        0    31554 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/favicon/favicon-152.png
--rwxr-xr-x   0        0        0     1400 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/favicon/favicon-16.png
--rwxr-xr-x   0        0        0    34059 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/favicon/favicon-160.png
--rwxr-xr-x   0        0        0    40519 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/favicon/favicon-180.png
--rwxr-xr-x   0        0        0    44600 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/favicon/favicon-192.png
--rwxr-xr-x   0        0        0    91499 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/favicon/favicon-310.png
--rwxr-xr-x   0        0        0     3189 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/favicon/favicon-32.png
--rwxr-xr-x   0        0        0     7536 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/favicon/favicon-57.png
--rwxr-xr-x   0        0        0     8084 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/favicon/favicon-60.png
--rwxr-xr-x   0        0        0     8928 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/favicon/favicon-64.png
--rwxr-xr-x   0        0        0    10091 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/favicon/favicon-70.png
--rwxr-xr-x   0        0        0    10523 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/favicon/favicon-72.png
--rwxr-xr-x   0        0        0    11516 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/favicon/favicon-76.png
--rwxr-xr-x   0        0        0    16052 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/favicon/favicon-96.png
--rwxr-xr-x   0        0        0    22382 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/favicon/favicon.ico
--rw-r--r--   0        0        0   263409 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/favicon/favicon.png
--rw-r--r--   0        0        0    19863 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/statement.png
--rw-r--r--   0        0        0   370982 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/about/bank-account-details.png
--rw-r--r--   0        0        0   389739 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/about/bank-account-summaries.png
--rw-r--r--   0        0        0   387290 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/about/bank-accounts.png
--rw-r--r--   0        0        0   373677 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/about/credit-account-details.png
--rw-r--r--   0        0        0   452288 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/about/credit-transactions.png
--rw-r--r--   0        0        0   551891 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/about/homepage-user.png
--rw-r--r--   0        0        0   277799 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/about/homepage.png
--rw-r--r--   0        0        0   434617 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/about/statement-details.png
--rw-r--r--   0        0        0   325208 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/cards/chase-card.png
--rw-r--r--   0        0        0   326928 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/cards/discover-card.png
--rw-r--r--   0        0        0    16245 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/cards/new-card.png
--rw-r--r--   0        0        0    27829 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/cards/template-card.png
--rw-r--r--   0        0        0    11375 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/icons/arrow-down.png
--rw-r--r--   0        0        0     9574 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/icons/arrow-left.png
--rw-r--r--   0        0        0     8488 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/icons/arrow-up.png
--rw-r--r--   0        0        0     7713 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/icons/checkmark.png
--rw-r--r--   0        0        0    24685 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/icons/delete-orange-thick.png
--rw-r--r--   0        0        0    52116 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/icons/delete-orange.png
--rw-r--r--   0        0        0    22892 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/icons/delete-thick.png
--rw-r--r--   0        0        0    34259 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/icons/delete.png
--rw-r--r--   0        0        0    62744 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/icons/edit.png
--rw-r--r--   0        0        0    22117 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/icons/link.png
--rw-r--r--   0        0        0    19158 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/icons/minus-thick.png
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/icons/minus.png
--rw-r--r--   0        0        0    25963 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/icons/plus-thick.png
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/icons/plus.png
--rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/icons/refresh.png
--rw-r--r--   0        0        0    27520 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/icons/save.png
--rw-r--r--   0        0        0    13596 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/icons/sort-asc.png
--rw-r--r--   0        0        0    13302 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/icons/sort-desc.png
--rw-r--r--   0        0        0    26146 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/icons/statement.png
--rw-r--r--   0        0        0    38482 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/img/icons/x-thick.png
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/add_subtransaction.js
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/add_transfer.js
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/autocomplete_transaction.js
--rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/bind_tag_actions.js
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/define_filter.js
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/display_new_account_type_inputs.js
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/display_new_bank_inputs.js
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/display_new_credit_account_inputs.js
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/expand_bank.js
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/expand_bank_account.js
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/expand_transaction.js
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/flip_card.js
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/infer_card.js
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/infer_statement.js
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/make_payment.js
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/show_linked_transaction.js
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/update_account_statement_parameters.js
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/update_bank_name.js
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/update_card_status.js
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/update_statement_parameters.js
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/update_statements_display.js
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/update_transactions_display.js
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/modules/ajax.js
--rw-r--r--   0        0        0     8035 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/modules/autocomplete_input.js
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/modules/expand_box_row.js
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/modules/expand_transaction.js
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/modules/manage_acquisition_form.js
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/modules/manage_overlays.js
--rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/modules/manage_subforms.js
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/modules/update_database_widget.js
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/static/js/modules/update_display_ajax.js
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credits.html
--rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/index.html
--rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/layout.html
--rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/profile.html
--rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/story.html
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/auth/login.html
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/auth/register.html
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/banking/account_page.html
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/banking/account_summaries.html
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/banking/account_summaries_page.html
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/banking/account_summary.html
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/banking/accounts_page.html
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/banking/account_form/account_form.html
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/banking/account_form/account_form_page_new.html
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/banking/transaction_form/bank_info_form.html
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/banking/transaction_form/transaction_form.html
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/banking/transaction_form/transaction_form_page.html
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/banking/transaction_form/transaction_form_page_new.html
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/banking/transaction_form/transaction_form_page_update.html
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/banking/transaction_form/transfer_form.html
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/banking/transactions_table/condensed_row_content.html
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/banking/transactions_table/expanded_row_content.html
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/banking/transactions_table/transaction_field_titles.html
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/banking/transactions_table/transactions.html
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/common/form_page.html
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/common/transaction_form/subform.html
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/common/transaction_form/subtransaction_subform.html
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/common/transactions_table/linked_bank_transaction.html
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/common/transactions_table/linked_credit_transaction.html
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/common/transactions_table/linked_transaction_overlay.html
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/common/transactions_table/subtransactions.html
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/common/transactions_table/transaction_condensed.html
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/common/transactions_table/transaction_expanded.html
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/common/transactions_table/transactions.html
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/account_page.html
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/card_submission_page.html
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/cards.html
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/cards_page.html
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/statement_page.html
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/statement_summary.html
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/statements.html
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/statements_page.html
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/tags_page.html
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/transaction_submission_page.html
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/transactions_page.html
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/card_form/card_form.html
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/card_form/card_form_page_new.html
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/card_form/transfer_statement_inquiry.html
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/card_graphic/card_back.html
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/card_graphic/card_front.html
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/tag_tree/subtag_tree.html
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/tag_tree/tag_tree.html
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/transaction_form/transaction_form.html
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/transaction_form/transaction_form_page.html
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/transaction_form/transaction_form_page_new.html
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/transaction_form/transaction_form_page_update.html
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/transactions_table/condensed_row_content.html
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/transactions_table/expanded_row_content.html
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/transactions_table/transaction_field_titles.html
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 monopyly-1.3.1/monopyly/templates/credit/transactions_table/transactions.html
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 monopyly-1.3.1/.gitignore
--rw-r--r--   0        0        0    35150 2020-02-02 00:00:00.000000 monopyly-1.3.1/COPYING
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 monopyly-1.3.1/LICENSE
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 monopyly-1.3.1/pyproject.toml
--rw-r--r--   0        0        0    10058 2020-02-02 00:00:00.000000 monopyly-1.3.1/PKG-INFO
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 monopyly-1.4.0/README.md -> monopyly/README.md
+-rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/README.md
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/_version.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/auth/actions.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/auth/blueprint.py
+-rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/auth/routes.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/auth/tools.py
+-rw-r--r--   0        0        0     9837 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/banking/accounts.py
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/banking/actions.py
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/banking/banks.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/banking/blueprint.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/banking/filters.py
+-rw-r--r--   0        0        0    10504 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/banking/forms.py
+-rw-r--r--   0        0        0     8158 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/banking/routes.py
+-rw-r--r--   0        0        0     8453 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/banking/transactions.py
+-rwxr-xr-x   0        0        0     3031 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/cli/run.py
+-rw-r--r--   0        0        0    12194 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/common/transactions.py
+-rw-r--r--   0        0        0     5775 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/common/utils.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/common/forms/__init__.py
+-rw-r--r--   0        0        0     7811 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/common/forms/_forms.py
+-rw-r--r--   0        0        0     3793 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/common/forms/fields.py
+-rw-r--r--   0        0        0     5685 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/common/forms/utils.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/common/forms/validators.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/config/__init__.py
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/config/default_settings.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/config/settings.py
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/core/actions.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/core/blueprint.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/core/context_processors.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/core/filters.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/core/internal_transactions.py
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/core/routes.py
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/credit/accounts.py
+-rw-r--r--   0        0        0     5333 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/credit/actions.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/credit/blueprint.py
+-rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/credit/cards.py
+-rw-r--r--   0        0        0    12008 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/credit/forms.py
+-rw-r--r--   0        0        0    17889 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/credit/routes.py
+-rw-r--r--   0        0        0     6495 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/credit/statements.py
+-rw-r--r--   0        0        0     8767 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/credit/transactions.py
+-rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/database/__init__.py
+-rw-r--r--   0        0        0    14629 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/database/models.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/database/preloads.sql
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/database/schema.sql
+-rw-r--r--   0        0        0     3840 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/database/views.sql
+-rw-r--r--   0        0        0    87462 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/jquery-3.7.0.min.js
+-rw-r--r--   0        0        0    48633 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/css/style.css
+-rwxr-xr-x   0        0        0      315 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/favicon/browserconfig.xml
+-rwxr-xr-x   0        0        0    20601 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/favicon/favicon-114.png
+-rwxr-xr-x   0        0        0    22077 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/favicon/favicon-120.png
+-rwxr-xr-x   0        0        0    29107 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/favicon/favicon-144.png
+-rwxr-xr-x   0        0        0    30832 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/favicon/favicon-150.png
+-rwxr-xr-x   0        0        0    31554 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/favicon/favicon-152.png
+-rwxr-xr-x   0        0        0     1400 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/favicon/favicon-16.png
+-rwxr-xr-x   0        0        0    34059 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/favicon/favicon-160.png
+-rwxr-xr-x   0        0        0    40519 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/favicon/favicon-180.png
+-rwxr-xr-x   0        0        0    44600 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/favicon/favicon-192.png
+-rwxr-xr-x   0        0        0    91499 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/favicon/favicon-310.png
+-rwxr-xr-x   0        0        0     3189 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/favicon/favicon-32.png
+-rwxr-xr-x   0        0        0     7536 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/favicon/favicon-57.png
+-rwxr-xr-x   0        0        0     8084 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/favicon/favicon-60.png
+-rwxr-xr-x   0        0        0     8928 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/favicon/favicon-64.png
+-rwxr-xr-x   0        0        0    10091 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/favicon/favicon-70.png
+-rwxr-xr-x   0        0        0    10523 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/favicon/favicon-72.png
+-rwxr-xr-x   0        0        0    11516 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/favicon/favicon-76.png
+-rwxr-xr-x   0        0        0    16052 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/favicon/favicon-96.png
+-rwxr-xr-x   0        0        0    22382 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/favicon/favicon.ico
+-rw-r--r--   0        0        0   263409 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/favicon/favicon.png
+-rw-r--r--   0        0        0    19863 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/img/statement.png
+-rw-r--r--   0        0        0   370982 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/img/about/bank-account-details.png
+-rw-r--r--   0        0        0   389739 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/img/about/bank-account-summaries.png
+-rw-r--r--   0        0        0   387290 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/img/about/bank-accounts.png
+-rw-r--r--   0        0        0   373677 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/img/about/credit-account-details.png
+-rw-r--r--   0        0        0   452288 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/img/about/credit-transactions.png
+-rw-r--r--   0        0        0   551891 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/img/about/homepage-user.png
+-rw-r--r--   0        0        0   277799 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/img/about/homepage.png
+-rw-r--r--   0        0        0   434617 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/img/about/statement-details.png
+-rw-r--r--   0        0        0   325208 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/img/cards/chase-card.png
+-rw-r--r--   0        0        0   326928 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/img/cards/discover-card.png
+-rw-r--r--   0        0        0    16245 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/img/cards/new-card.png
+-rw-r--r--   0        0        0    27829 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/img/cards/template-card.png
+-rw-r--r--   0        0        0    11375 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/img/icons/arrow-down.png
+-rw-r--r--   0        0        0     9574 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/img/icons/arrow-left.png
+-rw-r--r--   0        0        0     8488 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/img/icons/arrow-up.png
+-rw-r--r--   0        0        0     7713 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/img/icons/checkmark.png
+-rw-r--r--   0        0        0    24685 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/img/icons/delete-orange-thick.png
+-rw-r--r--   0        0        0    52116 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/img/icons/delete-orange.png
+-rw-r--r--   0        0        0    22892 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/img/icons/delete-thick.png
+-rw-r--r--   0        0        0    34259 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/img/icons/delete.png
+-rw-r--r--   0        0        0    62744 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/img/icons/edit.png
+-rw-r--r--   0        0        0    22117 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/img/icons/link.png
+-rw-r--r--   0        0        0    19158 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/img/icons/minus-thick.png
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/img/icons/minus.png
+-rw-r--r--   0        0        0    25963 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/img/icons/plus-thick.png
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/img/icons/plus.png
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/img/icons/refresh.png
+-rw-r--r--   0        0        0    27520 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/img/icons/save.png
+-rw-r--r--   0        0        0    13596 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/img/icons/sort-asc.png
+-rw-r--r--   0        0        0    13302 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/img/icons/sort-desc.png
+-rw-r--r--   0        0        0    26146 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/img/icons/statement.png
+-rw-r--r--   0        0        0    38482 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/img/icons/x-thick.png
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/js/add-subtransaction.js
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/js/add-transfer.js
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/js/autocomplete-transaction.js
+-rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/js/bind-tag-actions.js
+-rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/js/create-balance-chart.js
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/js/define-filter.js
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/js/display-new-account-type-inputs.js
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/js/display-new-bank-inputs.js
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/js/display-new-credit-account-inputs.js
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/js/expand-bank-account.js
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/js/expand-bank.js
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/js/expand-transaction.js
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/js/flip-card.js
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/js/hide-homepage-block.js
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/js/infer-card.js
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/js/infer-statement.js
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/js/make-payment.js
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/js/show-linked-transaction.js
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/js/update-account-statement-parameters.js
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/js/update-bank-name.js
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/js/update-card-status.js
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/js/update-statement-parameters.js
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/js/update-statements-display.js
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/js/update-transactions-display.js
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/js/modules/ajax.js
+-rw-r--r--   0        0        0     8035 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/js/modules/autocomplete-input.js
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/js/modules/expand-box-row.js
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/js/modules/expand-transaction.js
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/js/modules/manage-acquisition-form.js
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/js/modules/manage-overlays.js
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/js/modules/manage-subforms.js
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/js/modules/update-database-widget.js
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/static/js/modules/update-display-ajax.js
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/credits.html
+-rw-r--r--   0        0        0     4309 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/index.html
+-rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/layout.html
+-rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/profile.html
+-rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/story.html
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/auth/login.html
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/auth/register.html
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/banking/account_page.html
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/banking/account_summaries.html
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/banking/account_summaries_page.html
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/banking/account_summary.html
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/banking/accounts_page.html
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/banking/account_form/account_form.html
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/banking/account_form/account_form_page_new.html
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/banking/transaction_form/bank_info_form.html
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/banking/transaction_form/transaction_form.html
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/banking/transaction_form/transaction_form_page.html
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/banking/transaction_form/transaction_form_page_new.html
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/banking/transaction_form/transaction_form_page_update.html
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/banking/transaction_form/transfer_form.html
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/banking/transactions_table/condensed_row_content.html
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/banking/transactions_table/expanded_row_content.html
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/banking/transactions_table/transaction_field_titles.html
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/banking/transactions_table/transactions.html
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/common/form_page.html
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/common/transaction_form/subform.html
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/common/transaction_form/subtransaction_subform.html
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/common/transaction_form/transaction_form_page.html
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/common/transactions_table/linked_bank_transaction.html
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/common/transactions_table/linked_credit_transaction.html
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/common/transactions_table/linked_transaction_overlay.html
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/common/transactions_table/subtransactions.html
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/common/transactions_table/transaction_condensed.html
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/common/transactions_table/transaction_expanded.html
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/common/transactions_table/transactions.html
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/credit/account_page.html
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/credit/card_submission_page.html
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/credit/cards.html
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/credit/cards_page.html
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/credit/statement_page.html
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/credit/statement_summary.html
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/credit/statements.html
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/credit/statements_page.html
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/credit/tags_page.html
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/credit/transaction_submission_page.html
+-rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/credit/transactions_page.html
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/credit/card_form/card_form.html
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/credit/card_form/card_form_page_new.html
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/credit/card_form/transfer_statement_inquiry.html
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/credit/card_graphic/card_back.html
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/credit/card_graphic/card_front.html
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/credit/tag_tree/subtag_tree.html
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/credit/tag_tree/tag_tree.html
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/credit/transaction_form/transaction_form.html
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/credit/transaction_form/transaction_form_page.html
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/credit/transaction_form/transaction_form_page_new.html
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/credit/transaction_form/transaction_form_page_update.html
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/credit/transactions_table/condensed_row_content.html
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/credit/transactions_table/expanded_row_content.html
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/credit/transactions_table/transaction_field_titles.html
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 monopyly-1.4.0/monopyly/templates/credit/transactions_table/transactions.html
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 monopyly-1.4.0/.gitignore
+-rw-r--r--   0        0        0    35150 2020-02-02 00:00:00.000000 monopyly-1.4.0/COPYING
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 monopyly-1.4.0/LICENSE
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 monopyly-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0    10058 2020-02-02 00:00:00.000000 monopyly-1.4.0/PKG-INFO
```

### Comparing `monopyly-1.3.1/monopyly/README.md` & `monopyly-1.4.0/monopyly/README.md`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/auth/routes.py` & `monopyly-1.4.0/monopyly/auth/routes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Routes for site authentication.
 """
-from authanor.database import db_transaction
+from fuisce.database import db_transaction
 from flask import (
     current_app,
     flash,
     redirect,
     render_template,
     request,
     session,
```

### Comparing `monopyly-1.3.1/monopyly/auth/tools.py` & `monopyly-1.4.0/monopyly/auth/tools.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/banking/accounts.py` & `monopyly-1.4.0/monopyly/banking/accounts.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/banking/banks.py` & `monopyly-1.4.0/monopyly/banking/banks.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/banking/filters.py` & `monopyly-1.4.0/monopyly/banking/filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,8 +12,7 @@
         if len(linked_bank_transactions) > 1:
             common_bank_id = linked_bank_transactions[0].account.bank_id
             return all(
                 transaction.account.bank_id == common_bank_id
                 for transaction in linked_bank_transactions
             )
     return False
-
```

### Comparing `monopyly-1.3.1/monopyly/banking/forms.py` & `monopyly-1.4.0/monopyly/banking/forms.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/banking/routes.py` & `monopyly-1.4.0/monopyly/banking/routes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 """
 Routes for banking financials.
 """
-from itertools import islice
-
-from authanor.database import db_transaction
+from fuisce.database import db_transaction
 from flask import jsonify, redirect, render_template, request, url_for
 
 from ..auth.tools import login_required
 from ..common.forms.utils import extend_field_list_for_ajax
 from ..common.transactions import get_linked_transaction
 from .accounts import BankAccountHandler, BankAccountTypeHandler, save_account
-from .actions import get_bank_account_type_grouping
+from .actions import get_balance_chart_data, get_bank_account_type_grouping
 from .banks import BankHandler
 from .blueprint import bp
 from .forms import BankAccountForm, BankTransactionForm
 from .transactions import BankTransactionHandler, save_transaction
 
 
 @bp.route("/accounts")
@@ -66,23 +64,25 @@
     )
 
 
 @bp.route("/account/<int:account_id>")
 @login_required
 def load_account_details(account_id):
     account = BankAccountHandler.get_entry(account_id)
-    transactions = BankTransactionHandler.get_transactions(
-        account_ids=(account_id,),
-        sort_order="DESC",
+    transactions = list(
+        BankTransactionHandler.get_transactions(
+            account_ids=(account_id,), sort_order="DESC"
+        )
     )
     # Only display the first 100 transactions
     return render_template(
         "banking/account_page.html",
         account=account,
-        account_transactions=islice(transactions, 100),
+        account_transactions=transactions[:100],
+        chart_data=get_balance_chart_data(transactions),
     )
 
 
 @bp.route("/_expand_transaction", methods=("POST",))
 @login_required
 def expand_transaction():
     # Get the transaction ID from the AJAX request
@@ -94,15 +94,15 @@
     )
 
 
 @bp.route("/_show_linked_transaction", methods=("POST",))
 @login_required
 def show_linked_transaction():
     post_args = request.get_json()
-    transaction_id = post_args["transaction_id"]
+    transaction_id = int(post_args["transaction_id"])
     transaction = BankTransactionHandler.get_entry(transaction_id)
     linked_transaction = get_linked_transaction(transaction)
     return render_template(
         "common/transactions_table/linked_transaction_overlay.html",
         selected_transaction_type="bank",
         transaction=transaction,
         linked_transaction=linked_transaction,
```

### Comparing `monopyly-1.3.1/monopyly/banking/transactions.py` & `monopyly-1.4.0/monopyly/banking/transactions.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/cli/run.py` & `monopyly-1.4.0/monopyly/cli/run.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/common/transactions.py` & `monopyly-1.4.0/monopyly/common/transactions.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/common/forms/_forms.py` & `monopyly-1.4.0/monopyly/common/forms/_forms.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/common/forms/fields.py` & `monopyly-1.4.0/monopyly/common/forms/fields.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/common/forms/utils.py` & `monopyly-1.4.0/monopyly/common/forms/utils.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/common/forms/validators.py` & `monopyly-1.4.0/monopyly/common/forms/validators.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/core/actions.py` & `monopyly-1.4.0/monopyly/core/actions.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/core/context_processors.py` & `monopyly-1.4.0/monopyly/core/context_processors.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/core/filters.py` & `monopyly-1.4.0/monopyly/core/filters.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/core/routes.py` & `monopyly-1.4.0/monopyly/core/routes.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """
 Routes for core functionality.
 """
 from pathlib import Path
 
-from flask import g, render_template, render_template_string
+from flask import g, render_template, render_template_string, session
 
 from ..auth.tools import login_required
 from ..banking.accounts import BankAccountHandler
 from ..banking.banks import BankHandler
 from ..credit.cards import CreditCardHandler
 from ..credit.statements import CreditStatementHandler
 from .actions import format_readme_as_html_template
 from .blueprint import bp
 
 
 @bp.route("/")
 def index():
     if g.user:
+        # Set the homepage to show the welcome statement (unless otherwise set)
+        session.setdefault("show_homepage_block", True)
         # Get the user's banks and credit cards from the database
         banks = BankHandler.get_banks()
         bank_accounts = {}
         for bank in banks:
             accounts = BankAccountHandler.get_accounts((bank.id,)).all()
             # Only return banks which have bank accounts
             if accounts:
@@ -30,20 +32,28 @@
             statements = CreditStatementHandler.get_statements((card.id,))
             last_statement = statements.first()
             if last_statement:
                 card.last_statement_id = last_statement.id
             else:
                 card.last_statement_id = None
     else:
+        session["show_homepage_block"] = True
         bank_accounts, active_cards = None, None
     return render_template(
         "index.html", bank_accounts=bank_accounts, cards=active_cards
     )
 
 
+@bp.route("/_hide_homepage_block")
+@login_required
+def hide_homepage_block():
+    session["show_homepage_block"] = False
+    return ""
+
+
 @bp.route("/about")
 def about():
     readme_path = Path(__file__).parents[1] / "README.md"
     with readme_path.open(encoding="utf-8") as readme_file:
         raw_readme_text = readme_file.read()
     about_page_template = format_readme_as_html_template(raw_readme_text)
     return render_template_string(about_page_template)
```

### Comparing `monopyly-1.3.1/monopyly/credit/accounts.py` & `monopyly-1.4.0/monopyly/credit/accounts.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/credit/actions.py` & `monopyly-1.4.0/monopyly/credit/actions.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/credit/cards.py` & `monopyly-1.4.0/monopyly/credit/cards.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/credit/forms.py` & `monopyly-1.4.0/monopyly/credit/forms.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/credit/routes.py` & `monopyly-1.4.0/monopyly/credit/routes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Routes for credit card financials.
 """
 from itertools import islice
 
-from authanor.database import db_transaction
+from fuisce.database import db_transaction
 from flask import flash, g, jsonify, redirect, render_template, request, url_for
 from sqlalchemy.exc import MultipleResultsFound
 from werkzeug.exceptions import abort
 from wtforms.validators import ValidationError
 
 from ..auth.tools import login_required
 from ..banking.accounts import BankAccountHandler
@@ -90,18 +90,16 @@
 
 @bp.route("/_update_card_status", methods=("POST",))
 @login_required
 @db_transaction
 def update_card_status():
     # Get the field from the AJAX request
     post_args = request.get_json()
-    input_id = post_args["input_id"]
+    card_id = int(post_args["card_id"])
     active = int(post_args["active"])
-    # Get the card ID as the second component of the input's ID attribute
-    card_id = input_id.split("-")[1]
     # Update the card in the database
     card = CreditCardHandler.update_entry(card_id, active=active)
     return render_template("credit/card_graphic/card_front.html", card=card)
 
 
 @bp.route("/delete_card/<int:card_id>")
 @login_required
@@ -163,17 +161,17 @@
 
 
 @bp.route("/_update_statements_display", methods=("POST",))
 @login_required
 def update_statements_display():
     # Separate the arguments of the POST method
     post_args = request.get_json()
-    filter_ids = post_args["filter_ids"]
+    card_ids = map(int, post_args["card_ids"])
     # Determine the cards from the arguments of POST method
-    cards = [CreditCardHandler.find_card(*tag.split("-")) for tag in filter_ids]
+    cards = [CreditCardHandler.get_entry(card_id) for card_id in card_ids]
     card_statements = get_card_statement_grouping(cards)
     # Filter selected statements from the database
     return render_template("credit/statements.html", card_statements=card_statements)
 
 
 @bp.route("/statement/<int:statement_id>")
 @login_required
@@ -269,15 +267,15 @@
     )
 
 
 @bp.route("/_show_linked_transaction", methods=("POST",))
 @login_required
 def show_linked_transaction():
     post_args = request.get_json()
-    transaction_id = post_args["transaction_id"]
+    transaction_id = int(post_args["transaction_id"])
     transaction = CreditTransactionHandler.get_entry(transaction_id)
     linked_transaction = get_linked_transaction(transaction)
     return render_template(
         "common/transactions_table/linked_transaction_overlay.html",
         selected_transaction_type="credit",
         transaction=transaction,
         linked_transaction=linked_transaction,
@@ -285,22 +283,16 @@
 
 
 @bp.route("/_update_transactions_display", methods=("POST",))
 @login_required
 def update_transactions_display():
     # Separate the arguments of the POST method
     post_args = request.get_json()
-    filter_ids = post_args["filter_ids"]
+    card_ids = map(int, post_args["card_ids"])
     sort_order = "ASC" if post_args["sort_order"] == "asc" else "DESC"
-    # Determine the card IDs from the arguments of POST method
-    card_ids = []
-    for card_tag in filter_ids:
-        bank_name, last_four_digits = card_tag.split("-")
-        card = CreditCardHandler.find_card(bank_name, last_four_digits)
-        card_ids.append(card.id)
     # Filter selected transactions from the database
     transactions = CreditTransactionHandler.get_transactions(
         card_ids=card_ids,
         sort_order=sort_order,
     )
     return render_template(
         "credit/transactions_table/transactions.html",
```

### Comparing `monopyly-1.3.1/monopyly/credit/statements.py` & `monopyly-1.4.0/monopyly/credit/statements.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/credit/transactions.py` & `monopyly-1.4.0/monopyly/credit/transactions.py`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/database/__init__.py` & `monopyly-1.4.0/monopyly/database/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
 Expose commonly used database functionality to the rest of the package.
 """
 import sqlite3
 from pathlib import Path
 
 import click
-from authanor.database import SQLAlchemy as _SQLAlchemy
+from fuisce.database import SQLAlchemy as _SQLAlchemy
 from flask import current_app
 from flask.cli import with_appcontext
 
 from ..core.actions import get_timestamp
 
-DB_NAME = "monopyly.sqlite"
+BASE_DB_NAME = "monopyly.sqlite"
 
 
 class SQLAlchemy(_SQLAlchemy):
     """Store an interface to SQLAlchemy database objects."""
 
     def initialize(self, app):
         """
@@ -45,15 +45,15 @@
                 with current_app.open_resource(sql_filepath) as sql_file:
                     raw_conn.executescript(sql_file.read().decode("utf8"))
             raw_conn.close()
         # Top level initialization does not overwrite tables, so it goes at the end
         super().initialize(app)
 
 
-db = SQLAlchemy()
+SQLAlchemy.create_default_interface()
 
 
 @click.command("init-db")
 @with_appcontext
 def init_db_command():
     """Initialize the database from the command line (if it does not exist)."""
     db_path = current_app.config["DATABASE"]
@@ -88,7 +88,13 @@
     """Create a backup of the database."""
     # Backup the database
     with backup_db:
         db.backup(backup_db)
     # Close the connections
     backup_db.close()
     db.close()
+
+
+def register_db_cli_commands(app):
+    """Register database CLI commands with the app."""
+    app.cli.add_command(init_db_command)
+    app.cli.add_command(back_up_db_command)
```

### Comparing `monopyly-1.3.1/monopyly/database/models.py` & `monopyly-1.4.0/monopyly/database/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,14 +176,15 @@
         Integer,
         ForeignKey("bank_account_types_view.id"),
         nullable=False,
     )
     last_four_digits = mapped_column(String, nullable=False)
     active = mapped_column(Integer, nullable=False)
     balance = mapped_column(Float, nullable=False)
+    projected_balance = mapped_column(Float, nullable=False)
     # Relationships
     account = relationship("BankAccount", back_populates="view")
     bank = relationship("Bank", back_populates="bank_accounts")
     account_type = relationship(
         "BankAccountTypeView",
         viewonly=True,
         back_populates="accounts",
```

### Comparing `monopyly-1.3.1/monopyly/database/schema.sql` & `monopyly-1.4.0/monopyly/database/schema.sql`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/database/views.sql` & `monopyly-1.4.0/monopyly/database/views.sql`

 * *Files 6% similar despite different names*

```diff
@@ -12,27 +12,14 @@
 CREATE VIEW bank_account_types_view AS
 SELECT
   t.*,
   IFNULL(t.type_abbreviation, t.type_name) type_common_name
 FROM bank_account_types AS t;
 
 
-/* Prepare a view giving enhanced bank account information */
-CREATE VIEW bank_accounts_view AS
-SELECT
-  a.*,
-  ROUND(COALESCE(SUM(subtotal), 0), 2) balance
-FROM bank_accounts AS a
-  LEFT OUTER JOIN bank_transactions AS t
-    ON t.account_id = a.id
-  LEFT OUTER JOIN bank_subtransactions AS s_t
-    ON s_t.transaction_id = t.id
-GROUP BY a.id;
-
-
 /* Prepare a view giving enhanced bank account transaction information */
 CREATE VIEW bank_transactions_view AS
 WITH view AS (
   SELECT
     t.*,
     ROUND(SUM(subtotal), 2) total,
     GROUP_CONCAT(note, '; ') notes
@@ -46,14 +33,29 @@
   ROUND(
     SUM(total) OVER (PARTITION BY account_id ORDER BY transaction_date, id),
     2
   ) balance
 FROM view;
 
 
+/* Prepare a view giving enhanced bank account information */
+CREATE VIEW bank_accounts_view AS
+SELECT
+  a.*,
+  ROUND(COALESCE(
+      SUM(CASE WHEN t.transaction_date <= DATE('now') THEN t.total END),
+      0
+  ), 2) balance,
+  ROUND(COALESCE(SUM(t.total), 0), 2) projected_balance
+FROM bank_accounts AS a
+  LEFT OUTER JOIN bank_transactions_view AS t
+    ON t.account_id = a.id
+GROUP BY a.id;
+
+
 /* Prepare a view giving consolidated credit card transaction information */
 CREATE VIEW credit_transactions_view AS
 SELECT
   t.*,
   ROUND(SUM(subtotal), 2) total,
   GROUP_CONCAT(note, '; ') notes
 FROM credit_transactions AS t
```

### Comparing `monopyly-1.3.1/monopyly/static/jquery-3.7.0.min.js` & `monopyly-1.4.0/monopyly/static/jquery-3.7.0.min.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/css/style.css` & `monopyly-1.4.0/monopyly/static/css/style.css`

 * *Files 2% similar despite different names*

```diff
@@ -507,15 +507,15 @@
  */
 .sidebar-menu {
   display: flex;
   flex-direction: column;
   align-self: flex-start;
   height: min-content;
   width: 30px;
-  margin-left: 20px;
+  margin-left: 30px;
   padding: 10px;
   border-radius: 10px;
   background-color: #f8f8f8;
 }
 
 .sidebar-menu div:first-of-type {
   margin-top: 5px;
@@ -1039,23 +1039,28 @@
   min-width: 80px;
 }
 
 .transactions-table .notes.column {
   flex: 4;
   min-width: 175px;
   white-space: nowrap;
-  overflow: auto;
+  overflow: hidden;
 }
 @media screen and (max-width: 1000px) {
   /* Mobile layout */
   .transactions-table .notes.column {
     display: none;
   }
 }
 
+.transactions-table .notes.column:hover {
+  overflow: auto;
+}
+
+
 .transactions-table .card.column {
   flex: 1;
   min-width: 110px;
   text-align: right;
 }
 @media screen and (max-width: 1200px) {
   /* Statement disappear */
@@ -1584,42 +1589,53 @@
 /*
  * Define styles for the general "Details" page layout
  * (with balance/total and transactions)
  */
 .details {
   display: flex;
   flex-direction: column;
+  height: 100%;
   width: 100%;
 }
 
 .details .primary-info {
   display: flex;
-  justify-content: space-around;
+  flex-direction: column;
+  flex-wrap: wrap;
+  align-items: center;
+  gap: 10px;
   width: 100%;
 }
 @media screen and (max-width: 1500px) {
   .details .primary-info {
     display: flex;
-    flex-direction: column;
     align-items: center;
   }
 }
 
-.details .summary-container {
-  display: flex;
-  flex-direction: column;
-  align-items: flex-start;
-  margin: 0 20px 50px 0;
+.details .primary-info::after {
+  content: "";
+  flex-shrink: 0;
+  order: 1;
+  height: 100%;
 }
 @media screen and (max-width: 1500px) {
-  .details .summary-container {
-    margin: 0 0 50px 0;
+  .details .primary-info::after {
+    order: 2;
+    height: 0%;
   }
 }
 
+.details .summary-container {
+  display: flex;
+  justify-content: center;
+  min-width: 45%;
+  margin: 0 0 0 0;
+}
+
 .details .summary-box {
   display: flex;
   flex-direction: column;
   width: min-content;
   padding: 40px 50px 60px;
   border-radius: 25px;
   box-shadow: 1px 1px 5px #dddddd;
@@ -1633,36 +1649,54 @@
   margin: 20px 0;
   font-size: 72pt;
   font-weight: bold;
   letter-spacing: 1px;
   text-align: center;
 }
 
+.details .summary-box .projected-balance .amount {
+  color: var(--moneytree);
+}
+
+.details .summary-box .projected-balance .amount.negative {
+  color: crimson;
+}
+
 .details .summary-box .title {
   font-size: 28pt;
 }
 
+.details .summary-box .suptitle,
+.details .summary-box .subtitle {
+  color: #888888;
+  letter-spacing: 1px;
+  text-transform: uppercase;
+}
+
 .details .summary-box .suptitle {
   margin-bottom: 10px;
-  color: #888888;
   font-size: 14pt;
 }
 
+.details .summary-box .subtitle {
+  font-size: 12pt;
+}
+
 .details .transactions-container {
   width: 50%;
+  order: 2;
   min-width: 500px;
 }
 @media screen and (max-width: 1500px) {
   .details .transactions-container {
+    order: 1;
     margin-top: 50px;
   }
 }
 
-.details #
-
 .details .transactions-table {
   width: 100%;
   min-width: inherit;
 }
 
 .details .transactions-table .date.column {
   flex: 1;
@@ -1677,16 +1711,14 @@
   flex: 1;
   margin-left: auto;
 }
 
 .details .transactions-table .notes.column {
   flex: 4;
   min-width: 100px;
-  white-space: nowrap;
-  overflow: auto;
 }
 
 @media screen and (max-width: 1500px) {
   .details .transactions-table .expanded .row-content {
     margin-left: 28px;
   }
 }
@@ -1766,37 +1798,56 @@
   height: 60%;
 }
 
 /*
  * Customization for the 'Home' page
  */
 #homepage-block {
-  padding: 30px 0 30px 0;
+  margin-bottom: 20px;
+  padding: 0 0 30px 0;
   background-color: #dddddd;
   border: 1px solid #d8d8d8;
   border-radius: 6px;
   box-shadow: 2px 2px 5px #cccccc;
 }
 
 #homepage-block h2 {
-  margin: 25px 0;
+  margin: 0 0;
   font-size: 3em;
   letter-spacing: -2px;
   text-align: center;
 }
 
 #homepage-block h3 {
   margin: 25px 0;
   color: #777777;
   font-size: 1.7em;
   font-weight: 100;
   letter-spacing: 0.5px;
   text-align: center;
 }
 
+#homepage-block .buttons {
+  display: flex;
+  justify-content: flex-end;
+  height: 30px;
+  padding: 10px;
+  filter: brightness(0.90);
+}
+
+#homepage-block .button {
+  height: 25px;
+  opacity: 0;
+  transition: opacity 0.5s ease;
+}
+
+#homepage-block:hover .button {
+  opacity: 100%;
+}
+
 #homepage-panels {
   display: flex;
   justify-content: space-between;
   width: 100%;
 }
 
 #homepage-panels .panel {
@@ -2084,14 +2135,49 @@
 #bank-account-summaries .account-block .balance {
   font-size: 24pt;
   font-weight: bold;
 }
 
 
 /*
+ * Customization for the (bank) 'Account Details' page
+ */
+@media screen and (max-width: 1500px) {
+  #bank-account-details .summary-container {
+    margin: 0 0 0 0;
+  }
+}
+
+#balance-chart {
+  width: 42.5%;
+  max-width: 600px;
+  margin-top: 40px;
+}
+@media screen and (max-width: 1500px) {
+  #balance-chart {
+    order: 2;
+    width: 45%;
+    min-width: 450px;
+  }
+}
+
+#balance-chart .ct-chart-line {
+  overflow: visible;
+}
+
+#balance-chart .ct-point, #balance-chart .ct-line {
+  stroke: var(--moneytree-leaves);
+}
+
+#balance-chart .ct-line {
+  stroke-width: 2px;
+}
+
+
+/*
  * Customization for the 'New Bank Transaction'/'Update Bank Transaction' pages
  */
 form#bank-transaction .bank-field {
   flex: 3;
 }
 
 form#bank-transaction .account-type-field {
@@ -2499,23 +2585,14 @@
 #statement-statistics table td {
   padding: 3px 15px;
   text-align: right;
 }
 
 
 /*
- * Customization for the 'Credit Transactions' page
- */
-.transactions-container .transactions {
-  width: 100%;
-  margin: 0 auto;
-}
-
-
-/*
  * Customization for the 'New Credit Transaction'/
  * 'Update Credit Transaction' pages
  */
 form#credit-transaction .bank-field {
   flex: 3;
 }
```

### Comparing `monopyly-1.3.1/monopyly/static/favicon/favicon-114.png` & `monopyly-1.4.0/monopyly/static/favicon/favicon-114.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/favicon/favicon-120.png` & `monopyly-1.4.0/monopyly/static/favicon/favicon-120.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/favicon/favicon-144.png` & `monopyly-1.4.0/monopyly/static/favicon/favicon-144.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/favicon/favicon-150.png` & `monopyly-1.4.0/monopyly/static/favicon/favicon-150.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/favicon/favicon-152.png` & `monopyly-1.4.0/monopyly/static/favicon/favicon-152.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/favicon/favicon-16.png` & `monopyly-1.4.0/monopyly/static/favicon/favicon-16.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/favicon/favicon-160.png` & `monopyly-1.4.0/monopyly/static/favicon/favicon-160.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/favicon/favicon-180.png` & `monopyly-1.4.0/monopyly/static/favicon/favicon-180.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/favicon/favicon-192.png` & `monopyly-1.4.0/monopyly/static/favicon/favicon-192.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/favicon/favicon-310.png` & `monopyly-1.4.0/monopyly/static/favicon/favicon-310.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/favicon/favicon-32.png` & `monopyly-1.4.0/monopyly/static/favicon/favicon-32.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/favicon/favicon-57.png` & `monopyly-1.4.0/monopyly/static/favicon/favicon-57.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/favicon/favicon-60.png` & `monopyly-1.4.0/monopyly/static/favicon/favicon-60.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/favicon/favicon-64.png` & `monopyly-1.4.0/monopyly/static/favicon/favicon-64.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/favicon/favicon-70.png` & `monopyly-1.4.0/monopyly/static/favicon/favicon-70.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/favicon/favicon-72.png` & `monopyly-1.4.0/monopyly/static/favicon/favicon-72.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/favicon/favicon-76.png` & `monopyly-1.4.0/monopyly/static/favicon/favicon-76.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/favicon/favicon-96.png` & `monopyly-1.4.0/monopyly/static/favicon/favicon-96.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/favicon/favicon.ico` & `monopyly-1.4.0/monopyly/static/favicon/favicon.ico`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/favicon/favicon.png` & `monopyly-1.4.0/monopyly/static/favicon/favicon.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/img/statement.png` & `monopyly-1.4.0/monopyly/static/img/statement.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/img/about/bank-account-details.png` & `monopyly-1.4.0/monopyly/static/img/about/bank-account-details.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/img/about/bank-account-summaries.png` & `monopyly-1.4.0/monopyly/static/img/about/bank-account-summaries.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/img/about/bank-accounts.png` & `monopyly-1.4.0/monopyly/static/img/about/bank-accounts.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/img/about/credit-account-details.png` & `monopyly-1.4.0/monopyly/static/img/about/credit-account-details.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/img/about/credit-transactions.png` & `monopyly-1.4.0/monopyly/static/img/about/credit-transactions.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/img/about/homepage-user.png` & `monopyly-1.4.0/monopyly/static/img/about/homepage-user.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/img/about/homepage.png` & `monopyly-1.4.0/monopyly/static/img/about/homepage.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/img/about/statement-details.png` & `monopyly-1.4.0/monopyly/static/img/about/statement-details.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/img/cards/chase-card.png` & `monopyly-1.4.0/monopyly/static/img/cards/chase-card.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/img/cards/discover-card.png` & `monopyly-1.4.0/monopyly/static/img/cards/discover-card.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/img/cards/new-card.png` & `monopyly-1.4.0/monopyly/static/img/cards/new-card.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/img/cards/template-card.png` & `monopyly-1.4.0/monopyly/static/img/cards/template-card.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/img/icons/arrow-down.png` & `monopyly-1.4.0/monopyly/static/img/icons/arrow-down.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/img/icons/arrow-left.png` & `monopyly-1.4.0/monopyly/static/img/icons/arrow-left.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/img/icons/arrow-up.png` & `monopyly-1.4.0/monopyly/static/img/icons/arrow-up.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/img/icons/checkmark.png` & `monopyly-1.4.0/monopyly/static/img/icons/checkmark.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/img/icons/delete-orange-thick.png` & `monopyly-1.4.0/monopyly/static/img/icons/delete-orange-thick.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/img/icons/delete-orange.png` & `monopyly-1.4.0/monopyly/static/img/icons/delete-orange.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/img/icons/delete-thick.png` & `monopyly-1.4.0/monopyly/static/img/icons/delete-thick.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/img/icons/delete.png` & `monopyly-1.4.0/monopyly/static/img/icons/delete.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/img/icons/edit.png` & `monopyly-1.4.0/monopyly/static/img/icons/edit.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/img/icons/link.png` & `monopyly-1.4.0/monopyly/static/img/icons/link.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/img/icons/minus-thick.png` & `monopyly-1.4.0/monopyly/static/img/icons/minus-thick.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/img/icons/minus.png` & `monopyly-1.4.0/monopyly/static/img/icons/minus.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/img/icons/plus-thick.png` & `monopyly-1.4.0/monopyly/static/img/icons/plus-thick.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/img/icons/plus.png` & `monopyly-1.4.0/monopyly/static/img/icons/plus.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/img/icons/refresh.png` & `monopyly-1.4.0/monopyly/static/img/icons/refresh.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/img/icons/save.png` & `monopyly-1.4.0/monopyly/static/img/icons/save.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/img/icons/sort-asc.png` & `monopyly-1.4.0/monopyly/static/img/icons/sort-asc.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/img/icons/sort-desc.png` & `monopyly-1.4.0/monopyly/static/img/icons/sort-desc.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/img/icons/statement.png` & `monopyly-1.4.0/monopyly/static/img/icons/statement.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/img/icons/x-thick.png` & `monopyly-1.4.0/monopyly/static/img/icons/x-thick.png`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/js/add_subtransaction.js` & `monopyly-1.4.0/monopyly/static/js/add-subtransaction.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -8,15 +8,15 @@
  * the number of current subtransactions already being displayed, so
  * that new subtransaction fields may be indexed accordingly. The page
  * is updated with the new field information.
  */
 
 import {
     SubformManager
-} from './modules/manage_subforms.js';
+} from './modules/manage-subforms.js';
 
 
 /**
  * A class for managing subtransaction subforms.
  */
 class SubtransactionSubformManager extends SubformManager {
```

### Comparing `monopyly-1.3.1/monopyly/static/js/add_transfer.js` & `monopyly-1.4.0/monopyly/static/js/add-transfer.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -6,15 +6,15 @@
  * the button is pressed to record a transfer, an AJAX request is
  * executed to retrieve an extra set of subfields for the transaction
  * form. The page is updated with the new field information.
  */
 
 import {
     SubformManager
-} from './modules/manage_subforms.js';
+} from './modules/manage-subforms.js';
 
 
 /**
  * A class for managing bank transfer subforms.
  */
 class BankTransferSubformManager extends SubformManager {
```

### Comparing `monopyly-1.3.1/monopyly/static/js/autocomplete_transaction.js` & `monopyly-1.4.0/monopyly/static/js/autocomplete-transaction.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -6,15 +6,15 @@
  * using an AJAX request. They are ordered (on the server side) by their
  * occurrence frequency and then filtered here by the current input text after
  * the input field is changed.
  */
 
 import {
     AutocompleteBox
-} from './modules/autocomplete_input.js';
+} from './modules/autocomplete-input.js';
 
 
 (function() {
 
     setAutocomplete();
 
     function setAutocomplete() {
```

### Comparing `monopyly-1.3.1/monopyly/static/js/bind_tag_actions.js` & `monopyly-1.4.0/monopyly/static/js/bind-tag-actions.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/js/define_filter.js` & `monopyly-1.4.0/monopyly/static/js/define-filter.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/js/display_new_account_type_inputs.js` & `monopyly-1.4.0/monopyly/static/js/display-new-account-type-inputs.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 /* Display inputs for a new account type when collecting new bank account info.
  */
 
 import {
     AcquisitionFormManager
-} from './modules/manage_acquisition_form.js';
+} from './modules/manage-acquisition-form.js';
 
 
 (function() {
 
     // Display the bank account type name input box for the new account type
     let $inputAccountType = $('form#bank-account #account_type_info-account_type_id');
     let $fieldAccountTypeName = $('form#bank-account #account-type-name-field');
```

### Comparing `monopyly-1.3.1/monopyly/static/js/display_new_credit_account_inputs.js` & `monopyly-1.4.0/monopyly/static/js/display-new-credit-account-inputs.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 /* Display inputs for a new credit account when collecting new credit card info.
  */
 
 import {
     AcquisitionFormManager
-} from './modules/manage_acquisition_form.js';
+} from './modules/manage-acquisition-form.js';
 
 
 (function() {
 
     // Display the bank information inputs for a new account
     let $inputAccount = $('form#card #account_info-account_id');
     let $secondaryAccountInfo = $('form#card #secondary-account-info');
```

### Comparing `monopyly-1.3.1/monopyly/static/js/expand_bank.js` & `monopyly-1.4.0/monopyly/static/js/expand-bank.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -6,15 +6,15 @@
  * bank information (e.g., updating or deleting the bank). A user can
  * can exit the expanded view by clicking anywhere within the expanded
  * view (that is not otherwise a button).
  */
 
 import {
     toggleBoxRow
-} from './modules/expand_box_row.js';
+} from './modules/expand-box-row.js';
 
 
 (function() {
 
     // Identify the bank rows
     const $bankRow = $('.bank-list .bank-block');
     toggleBoxRow($bankRow);
```

### Comparing `monopyly-1.3.1/monopyly/static/js/expand_bank_account.js` & `monopyly-1.4.0/monopyly/static/js/expand-bank-account.js`

 * *Files 23% similar despite different names*

#### js-beautify {}

```diff
@@ -6,15 +6,15 @@
  * for editing bank information (e.g., deleting the account). A user
  * can exit the expanded view by clicking anywhere within the expanded
  * view (that is not otherwise a button).
  */
 
 import {
     toggleBoxRow
-} from './modules/expand_box_row.js';
+} from './modules/expand-box-row.js';
 
 
 (function() {
 
     // Identify the account rows
     const $accountRow = $('#bank-container .account-block');
     toggleBoxRow($accountRow);
```

### Comparing `monopyly-1.3.1/monopyly/static/js/expand_transaction.js` & `monopyly-1.4.0/monopyly/static/js/expand-transaction.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -6,28 +6,29 @@
  * more detail (and a larger font) than the rest of the transaction
  * table. For both credit card and bank transactions, this expanded row
  * shows subtransaction information.
  */
 
 import {
     replaceDisplayContentsAjaxRequest
-} from './modules/update_display_ajax.js';
+} from './modules/update-display-ajax.js';
 import {
     toggleTransactionRow
-} from './modules/expand_transaction.js';
+} from './modules/expand-transaction.js';
 
 
-function display_subtransactions($transaction) {
+function displaySubtransactions($transaction) {
 
     // Execute an AJAX request to get transaction/subtransaction information
     const endpoint = EXPAND_TRANSACTION_ENDPOINT;
     const rawData = $transaction[0].id;
     const $container = $transaction.find('.subtransaction-container');
     replaceDisplayContentsAjaxRequest(endpoint, rawData, $container);
 
 }
 
+
 (function() {
 
-    toggleTransactionRow(display_subtransactions);
+    toggleTransactionRow(displaySubtransactions);
 
 })();
```

### Comparing `monopyly-1.3.1/monopyly/static/js/flip_card.js` & `monopyly-1.4.0/monopyly/static/js/flip-card.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/js/infer_card.js` & `monopyly-1.4.0/monopyly/static/js/infer-card.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/js/infer_statement.js` & `monopyly-1.4.0/monopyly/static/js/infer-statement.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/js/make_payment.js` & `monopyly-1.4.0/monopyly/static/js/make-payment.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -19,41 +19,45 @@
 
 (function() {
 
     const $container = $('#statement-summary-container');
     prepareForm();
 
     function prepareForm() {
+
         // Identify the key elements
         let $buttonPay = $('#make-payment[type="button"]');
-        let $inputPayAmount = $('#pay-amount');
-        let $inputPayDate = $('#pay-date');
-        let $selectPayBankAccount = $('#pay-bank-account');
-        // Change the form to allow information to be entered/submitted
-        bindButtonChange(
-            $buttonPay,
-            $inputPayAmount,
-            $inputPayDate,
-            $selectPayBankAccount
-        );
-        // Clicking outside the form returns the form to its original state
-        $(document).on('click', function(event) {
-            const $formPay = $('form#pay');
-            // Change the button type back to 'button' for clicks outside the form
-            if (!$formPay.is(event.target) && $formPay.has(event.target).length === 0) {
-                $buttonPay.off('click');
-                $buttonPay[0].type = 'button';
-                bindButtonChange(
-                    $buttonPay,
-                    $inputPayAmount,
-                    $inputPayDate,
-                    $selectPayBankAccount
-                );
-            }
-        });
+
+        if ($buttonPay.length) {
+            let $inputPayAmount = $('#pay-amount');
+            let $inputPayDate = $('#pay-date');
+            let $selectPayBankAccount = $('#pay-bank-account');
+            // Change the form to allow information to be entered/submitted
+            bindButtonChange(
+                $buttonPay,
+                $inputPayAmount,
+                $inputPayDate,
+                $selectPayBankAccount
+            );
+            // Clicking outside the form returns the form to its original state
+            $(document).on('click', function(event) {
+                const $formPay = $('form#pay');
+                // Change the button type back to 'button' for clicks outside the form
+                if (!$formPay.is(event.target) && $formPay.has(event.target).length === 0) {
+                    $buttonPay.off('click');
+                    $buttonPay[0].type = 'button';
+                    bindButtonChange(
+                        $buttonPay,
+                        $inputPayAmount,
+                        $inputPayDate,
+                        $selectPayBankAccount
+                    );
+                }
+            });
+        }
     }
 
     function bindButtonChange($buttonPay, $inputPayAmount, $inputPayDate,
         $selectPayBankAccount) {
         $buttonPay.on('click', function(event) {
             // Change the button type to 'submit'
             this.type = 'submit';
```

### Comparing `monopyly-1.3.1/monopyly/static/js/show_linked_transaction.js` & `monopyly-1.4.0/monopyly/static/js/show-linked-transaction.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -8,15 +8,15 @@
  */
 
 import {
     executeAjaxRequest
 } from './modules/ajax.js';
 import {
     OverlayManager
-} from './modules/manage_overlays.js';
+} from './modules/manage-overlays.js';
 
 
 (function() {
 
     const endpoint = LINKED_TRANSACTION_ENDPOINT;
 
     const $linkButton = $('img.link.button');
@@ -26,15 +26,15 @@
     // Define the action to execute after executing the request
     function action(response) {
         overlayManager.addOverlay(response);
     }
 
     // Add AJAX request action to the link button
     $linkButton.on('click', function() {
-        const transactionID = this.dataset.transactionId;
+        const transactionID = this.data("transaction-id");
         const rawData = {
             'transaction_id': transactionID,
         };
         executeAjaxRequest(endpoint, rawData, action);
     });
 
 })();
```

### Comparing `monopyly-1.3.1/monopyly/static/js/update_account_statement_parameters.js` & `monopyly-1.4.0/monopyly/static/js/update-account-statement-parameters.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -8,15 +8,15 @@
  * in an acceptable format, the new day is saved and the displayed day
  * is updated. If not, the existing statement due day or issue day in
  * the database is preserved and displayed.
  */
 
 import {
     updateDBWidget
-} from './modules/update_database_widget.js';
+} from './modules/update-database-widget.js';
 
 
 (function() {
 
     const endpointDueDay = UPDATE_ACCOUNT_STATEMENT_DUE_DAY_ENDPOINT;
     const endpointIssueDay = UPDATE_ACCOUNT_STATEMENT_ISSUE_DAY_ENDPOINT;
     // Identify the key elements
```

### Comparing `monopyly-1.3.1/monopyly/static/js/update_bank_name.js` & `monopyly-1.4.0/monopyly/static/js/update-bank-name.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -8,24 +8,24 @@
  * day is saved and the displayed day is updated. If not, the existing
  * statement due day or issue day in the database is preserved and
  * displayed.
  */
 
 import {
     updateDBWidget
-} from './modules/update_database_widget.js';
+} from './modules/update-database-widget.js';
 
 
 (function() {
 
     const endpoints = UPDATE_BANK_NAME_ENDPOINTS;
     // Identify the key elements
     const $widgets = $('#profile .bank-block.update-db-widget');
     $widgets.each(function() {
         const $widget = $(this);
-        const bankID = $widget.data("bank_id");
+        const bankID = $widget.data("bank-id");
         const endpoint = endpoints[bankID]
         // Prepare the widget
         updateDBWidget(endpoint, $widget);
     });
 
 })();
```

### Comparing `monopyly-1.3.1/monopyly/static/js/update_card_status.js` & `monopyly-1.4.0/monopyly/static/js/update-card-status.js`

 * *Files 23% similar despite different names*

#### js-beautify {}

```diff
@@ -6,36 +6,38 @@
  * selected as either 'Active' or 'Inactive'. Toggling the option
  * completes an AJAX request. The status is updated in the database and
  * the card is given a class of inactive.
  */
 
 import {
     replaceDisplayContentsAjaxRequest
-} from './modules/update_display_ajax.js';
+} from "./modules/update-display-ajax.js";
 
 
 (function() {
 
     const endpoint = UPDATE_CARD_STATUS_ENDPOINT;
     // Identify the key elements
-    const $switches = $('.toggle-switch-gadget');
+    const $switches = $(".toggle-switch-gadget");
 
     // Send an AJAX request when the switch is toggled
-    $switches.on('change', function() {
+    $switches.on("change", function() {
         const $toggleSwitch = $(this);
-        const $card = $toggleSwitch.closest('.credit-card');
-        const $cardFront = $card.find('.card-face.front');
-        const $checkbox = $toggleSwitch.find('input[type="checkbox"]');
-        const cardActive = $checkbox.is(':checked');
+        const $card = $toggleSwitch.closest(".credit-card");
+        const $cardFront = $card.find(".card-face.front");
+        const $checkbox = $toggleSwitch.find("input[type="
+            checkbox "]");
+        const cardActive = $checkbox.is(":checked");
+        const cardID = $checkbox.data("card-id");
         const rawData = {
-            'input_id': $checkbox[0].id,
-            'active': cardActive,
+            "card_id": cardID,
+            "active": cardActive,
         };
         replaceDisplayContentsAjaxRequest(endpoint, rawData, $cardFront);
         if (cardActive) {
-            $card.removeClass('inactive');
+            $card.removeClass("inactive");
         } else {
-            $card.addClass('inactive');
+            $card.addClass("inactive");
         }
     });
 
 })();
```

### Comparing `monopyly-1.3.1/monopyly/static/js/update_statement_parameters.js` & `monopyly-1.4.0/monopyly/static/js/update-statement-parameters.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -8,15 +8,15 @@
  * format, the new date is saved and the displayed due date is updated.
  * If not, the existing statement due date in the database is preserved
  * and displayed.
  */
 
 import {
     updateDBWidget
-} from './modules/update_database_widget.js';
+} from './modules/update-database-widget.js';
 
 
 (function() {
 
     const endpoint = UPDATE_STATEMENT_DUE_DATE_ENDPOINT;
     // Identify the key elements
     const $widget = $('#due-date.update-db-widget');
```

### Comparing `monopyly-1.3.1/monopyly/static/js/update_statements_display.js` & `monopyly-1.4.0/monopyly/static/js/update-statements-display.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -6,15 +6,15 @@
  * the user's selection. Updates are triggered by changing the card
  * filters. A user can click on any of the card filters to show/hide
  * transactions from that card.
  */
 
 import {
     replaceDisplayContentsAjaxRequest
-} from './modules/update_display_ajax.js';
+} from './modules/update-display-ajax.js';
 
 
 (function() {
 
     // Identify the card filters
     const $filterContainer = $('#card-filter');
     // Identify the statements container
@@ -26,20 +26,20 @@
         // Add or remove the selected tag when clicked
         replaceDisplay();
     });
 
     function replaceDisplay() {
         // Determine the selected credit cards to use from the filters
         const $selectedFilters = $filterContainer.find('.card.selected');
-        const filterIDs = [];
+        const cardIDs = [];
         $selectedFilters.each(function() {
-            filterIDs.push(this.id);
+            cardIDs.push(this.dataset.cardId);
         });
         // Update the display with the filters
         const endpoint = FILTER_ENDPOINT;
         const rawData = {
-            'filter_ids': filterIDs
+            'card_ids': cardIDs
         };
         replaceDisplayContentsAjaxRequest(endpoint, rawData, $container);
     }
 
 })();
```

### Comparing `monopyly-1.3.1/monopyly/static/js/update_transactions_display.js` & `monopyly-1.4.0/monopyly/static/js/update-transactions-display.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -11,15 +11,15 @@
  * 	- Sorting the table by transaction date: a user can click on the
  * 	  'Date' column header to sort the transaction date in ascending
  * 	  or descending order.
  */
 
 import {
     replaceDisplayContentsAjaxRequest
-} from './modules/update_display_ajax.js';
+} from './modules/update-display-ajax.js';
 
 
 (function() {
 
     // Identify the card filters
     const $filterContainer = $('#card-filter');
     // Identify the transactions container
@@ -40,29 +40,29 @@
         // Update the table
         updateTable();
     });
 
     function updateTable() {
         // Determine the selected credit cards to use from the filters
         const $selectedFilters = $filterContainer.find('.card.selected');
-        const filterIDs = [];
+        const cardIDs = [];
         $selectedFilters.each(function() {
-            filterIDs.push(this.id);
+            cardIDs.push(this.dataset.cardId);
         });
         // Determine the table ordering (ascending/descending transaction date)
         const $sorter = $('.transactions-table .sort-button.selected');
         let sortOrder
         if ($sorter.hasClass('asc')) {
             sortOrder = 'asc';
         } else {
             sortOrder = 'desc';
         }
         // Update the table with the filters and ordering
         const endpoint = FILTER_ENDPOINT;
         const rawData = {
-            'filter_ids': filterIDs,
-            'sort_order': sortOrder
+            'card_ids': cardIDs,
+            'sort_order': sortOrder,
         };
         replaceDisplayContentsAjaxRequest(endpoint, rawData, $container);
     }
 
 })();
```

### Comparing `monopyly-1.3.1/monopyly/static/js/modules/ajax.js` & `monopyly-1.4.0/monopyly/static/js/modules/ajax.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/js/modules/autocomplete_input.js` & `monopyly-1.4.0/monopyly/static/js/modules/autocomplete-input.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/js/modules/expand_box_row.js` & `monopyly-1.4.0/monopyly/static/js/modules/expand-box-row.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/js/modules/expand_transaction.js` & `monopyly-1.4.0/monopyly/static/js/modules/expand-transaction.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/js/modules/manage_acquisition_form.js` & `monopyly-1.4.0/monopyly/static/js/modules/manage-acquisition-form.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/js/modules/manage_overlays.js` & `monopyly-1.4.0/monopyly/static/js/modules/manage-overlays.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/js/modules/manage_subforms.js` & `monopyly-1.4.0/monopyly/static/js/modules/manage-subforms.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/static/js/modules/update_database_widget.js` & `monopyly-1.4.0/monopyly/static/js/modules/update-database-widget.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -6,15 +6,15 @@
  * is replaced with an input. The value can be edited in the input, and
  * then this new value is saved after the user takes the focus off of
  * the input or the enter button is pressed.
  */
 
 import {
     replaceDisplayContentsAjaxRequest
-} from './update_display_ajax.js';
+} from './update-display-ajax.js';
 
 
 function updateDBWidget(endpoint, $widget) {
 
     // Identify the key elements of the widget
     const $button = $widget.find('.widget-edit-button');
     const $display = $widget.find('.widget-display');
```

### Comparing `monopyly-1.3.1/monopyly/static/js/modules/update_display_ajax.js` & `monopyly-1.4.0/monopyly/static/js/modules/update-display-ajax.js`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/templates/index.html` & `monopyly-1.4.0/monopyly/templates/index.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 {% extends "layout.html" %}
 
 {% block content %}
-  <div id="homepage-block">
-    <h2>Don't go broke!</h2>
-    <h3>A homemade personal finance manager, built in Flask.</h3>
-  </div>
-  <br>
+  {% if session["show_homepage_block"] %}
+    <div id="homepage-block">
+      <div class="buttons">
+        {% if g.user %}
+          <img class="hide button" src="{{ url_for('static', filename='img/icons/x-thick.png') }}">
+        {% endif %}
+      </div>
+      <h2>Don't go broke!</h2>
+      <h3>A homemade personal finance manager, built in Flask.</h3>
+    </div>
+  {% endif %}
 
   {% if g.user %}
     <div id="homepage-panels">
 
       <div id="banking" class="panel">
 
         <h2>Bank Accounts</h2>
@@ -139,7 +145,15 @@
       <div id="investments" class="panel">
         <h2>Coming soon!</h2>
       </div>
 
     </div>
   {% endif %}
 {% endblock %}
+
+{% block javascript %}
+  <script>
+    const HIDE_HOMEPAGE_BLOCK_ENDPOINT = "{{ url_for('core.hide_homepage_block') }}";
+  </script>
+  <script type="module" src="{{ url_for('static', filename='js/hide-homepage-block.js') }}">
+  </script>
+{% endblock %}
```

#### html2text {}

```diff
@@ -1,12 +1,14 @@
-{% extends "layout.html" %} {% block content %}
+{% extends "layout.html" %} {% block content %} {% if session
+["show_homepage_block"] %}
+{% if g.user %} [{{ url_for('static', filename='img/icons/x-thick.png') }}] {%
+endif %}
 ***** Don't go broke! *****
 **** A homemade personal finance manager, built in Flask. ****
-
-{% if g.user %}
+{% endif %} {% if g.user %}
 ***** Bank Accounts *****
 *** Profile ***
 Manage_accounts
 Add_a_new_account
 Manage_transaction_tags
 **** Banks ****
 {% for bank in bank_accounts %}
@@ -33,8 +35,9 @@
 {% if card.last_statement_id %}
 See_most_recent_statement
 {% endif %}
 See_transaction_history
 Create_a_new_transaction
 {% endfor %}
 ***** Coming soon! *****
-{% endif %} {% endblock %}
+{% endif %} {% endblock %} {% block javascript %}
+ {% endblock %}
```

### Comparing `monopyly-1.3.1/monopyly/templates/layout.html` & `monopyly-1.4.0/monopyly/templates/layout.html`

 * *Files 7% similar despite different names*

```diff
@@ -29,14 +29,17 @@
     <meta name="msapplication-TileColor" content="#FFFFFF">
     <meta name="msapplication-TileImage" content="{{ url_for('static', filename='favicon/favicon-144.png') }}">
     <meta name="msapplication-config" content="{{ url_for('static', filename='favicon/browserconfig.xml') }}">
     <!-- ****** faviconit.com favicons ****** -->
     <!-- Use Google JQuery CDN -->
     <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.7.0/jquery.min.js"></script>
     <script>window.jQuery || document.write('<script src="{{ url_for('static', filename='jquery-3.7.0.min.js') }}"><\/script>')</script>
+    <!-- Use Chartist via CDN -->
+    <link rel="stylesheet" href="//cdn.jsdelivr.net/chartist.js/latest/chartist.min.css">
+    <script src="//cdn.jsdelivr.net/chartist.js/latest/chartist.min.js"></script>
   </head>
   <body>
 
     <header id="masthead">
       <div class="container">
 
         <a href="{{ url_for('core.index') }}">
```

#### html2text {}

```diff
@@ -15,14 +15,15 @@
 
 
 
 
 
 
 
+
 ******_Monopyly_******
 
 Home
 About
 {% if g.user %}
 {{_g.user.username_}}
 Log_Out
```

### Comparing `monopyly-1.3.1/monopyly/templates/profile.html` & `monopyly-1.4.0/monopyly/templates/profile.html`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
       <div class="banking profile-section">
 
         <h2>Banks</h2>
 
         <div class="bank-list box-table">
           {% for bank in banks %}
 
-            <div class="bank-block box-row update-db-widget" data-bank_id="{{ bank.id }}">
+            <div class="bank-block box-row update-db-widget" data-bank-id="{{ bank.id }}">
 
               <div class="widget-text">
                 <div class="bank widget-display">{{ bank.bank_name }}</div>
                 <input class="widget-input" type="text" name="bank_name" value="{{ bank.bank_name }}" />
               </div>
 
               <div class="expanded">
@@ -81,12 +81,12 @@
 
     const UPDATE_BANK_NAME_ENDPOINTS = {
       {% for bank in banks %}
         {{ bank.id }}: "{{ url_for('banking.update_bank_name', bank_id=bank.id) }}",
       {% endfor %}
     };
   </script>
-  <script type="module" src="{{ url_for('static', filename='js/expand_bank.js') }}">
+  <script type="module" src="{{ url_for('static', filename='js/expand-bank.js') }}">
   </script>
-  <script type="module" src="{{ url_for('static', filename='js/update_bank_name.js') }}">
+  <script type="module" src="{{ url_for('static', filename='js/update-bank-name.js') }}">
   </script>
 {% endblock %}
```

### Comparing `monopyly-1.3.1/monopyly/templates/story.html` & `monopyly-1.4.0/monopyly/templates/story.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/templates/banking/account_page.html` & `monopyly-1.4.0/monopyly/templates/banking/account_page.html`

 * *Files 18% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 
     <div id="bank-account-info" class="primary-info">
 
       <div id="account-summary-container" class="summary-container">
         {% include 'banking/account_summary.html' %}
       </div>
 
+      <div id="balance-chart" class="ct-chart ct-octave"></div>
+
       <div id="account-transactions-container" class="transactions-container">
         {% with transactions = account_transactions %}
           {% include 'banking/transactions_table/transactions.html' %}
         {% endwith %}
       </div>
 
     </div>
@@ -52,13 +54,29 @@
 
 {% block javascript %}
 
   <script>
     const EXPAND_TRANSACTION_ENDPOINT = "{{ url_for('banking.expand_transaction') }}";
     const LINKED_TRANSACTION_ENDPOINT = "{{ url_for('banking.show_linked_transaction') }}";
   </script>
-  <script type="module" src="{{ url_for('static', filename='js/expand_transaction.js') }}">
+  <script>
+    const BALANCE_CHART_DATA = {
+      series: [
+        {
+          name: 'balances',
+          data: [
+            {% for x, y in chart_data %}
+              {x: {{ x }}, y: {{ y }}},
+            {% endfor %}
+          ],
+        },
+      ],
+    };
+  </script>
+  <script type="module" src="{{ url_for('static', filename='js/expand-transaction.js') }}">
+  </script>
+  <script type="module" src="{{ url_for('static', filename='js/show-linked-transaction.js') }}">
   </script>
-  <script type="module" src="{{ url_for('static', filename='js/show_linked_transaction.js') }}">
+  <script type="module" src="{{ url_for('static', filename='js/create-balance-chart.js') }}">
   </script>
 
 {% endblock %}
```

### Comparing `monopyly-1.3.1/monopyly/templates/banking/account_summaries.html` & `monopyly-1.4.0/monopyly/templates/banking/account_summaries.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/templates/banking/account_summaries_page.html` & `monopyly-1.4.0/monopyly/templates/banking/account_summaries_page.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/templates/banking/accounts_page.html` & `monopyly-1.4.0/monopyly/templates/banking/accounts_page.html`

 * *Files 1% similar despite different names*

```diff
@@ -86,10 +86,10 @@
 
     </div>
 
 {% endblock %}
 
 
 {% block javascript %}
-  <script type="module" src="{{ url_for('static', filename='js/expand_bank_account.js') }}">
+  <script type="module" src="{{ url_for('static', filename='js/expand-bank-account.js') }}">
   </script>
 {% endblock %}
```

### Comparing `monopyly-1.3.1/monopyly/templates/banking/account_form/account_form.html` & `monopyly-1.4.0/monopyly/templates/banking/account_form/account_form.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/templates/banking/account_form/account_form_page_new.html` & `monopyly-1.4.0/monopyly/templates/banking/account_form/account_form_page_new.html`

 * *Files 7% similar despite different names*

```diff
@@ -12,12 +12,12 @@
     {% include 'banking/account_form/account_form.html' %}
   {% endwith %}
 
 {% endblock %}
 
 
 {% block javascript %}
-  <script type="module" src="{{ url_for('static', filename='js/display_new_bank_inputs.js') }}">
+  <script type="module" src="{{ url_for('static', filename='js/display-new-bank-inputs.js') }}">
   </script>
-  <script type="module" src="{{ url_for('static', filename='js/display_new_account_type_inputs.js') }}">
+  <script type="module" src="{{ url_for('static', filename='js/display-new-account-type-inputs.js') }}">
   </script>
 {% endblock %}
```

### Comparing `monopyly-1.3.1/monopyly/templates/banking/transaction_form/bank_info_form.html` & `monopyly-1.4.0/monopyly/templates/banking/transaction_form/bank_info_form.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/templates/banking/transaction_form/transaction_form.html` & `monopyly-1.4.0/monopyly/templates/banking/transaction_form/transaction_form.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/templates/banking/transaction_form/transaction_form_page.html` & `monopyly-1.4.0/monopyly/templates/banking/transaction_form/transaction_form_page.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-{% extends "common/form_page.html" %}
+{% extends "common/transaction_form/transaction_form_page.html" %}
 
 
 {% block javascript %}
 
   <script>
     const AUTOCOMPLETE_ENDPOINT = "{{ url_for('banking.suggest_transaction_autocomplete') }}";
     const ADD_SUBTRANSACTION_FORM_ENDPOINT = "{{ url_for('banking.add_subtransaction_fields') }}";
     const ADD_TRANSFER_FORM_ENDPOINT = "{{ url_for('banking.add_transfer_field') }}";
   </script>
-  <script type="module" src="{{ url_for('static', filename='js/autocomplete_transaction.js') }}">
-  </script>
-  <script type="module" src="{{ url_for('static', filename='js/add_subtransaction.js') }}">
-  </script>
-  <script type="module" src="{{ url_for('static', filename='js/add_transfer.js') }}">
+  <script type="module" src="{{ url_for('static', filename='js/add-transfer.js') }}">
   </script>
+  {{ super() }}
 
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,2 +1,3 @@
-{% extends "common/form_page.html" %} {% block javascript %}
- {% endblock %}
+{% extends "common/transaction_form/transaction_form_page.html" %} {% block
+javascript %}
+ {{ super() }} {% endblock %}
```

### Comparing `monopyly-1.3.1/monopyly/templates/banking/transactions_table/expanded_row_content.html` & `monopyly-1.4.0/monopyly/templates/banking/transactions_table/expanded_row_content.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/templates/banking/transactions_table/transaction_field_titles.html` & `monopyly-1.4.0/monopyly/templates/banking/transactions_table/transaction_field_titles.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/templates/common/transaction_form/subtransaction_subform.html` & `monopyly-1.4.0/monopyly/templates/common/transaction_form/subtransaction_subform.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/templates/common/transactions_table/linked_bank_transaction.html` & `monopyly-1.4.0/monopyly/templates/common/transactions_table/linked_bank_transaction.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/templates/common/transactions_table/linked_credit_transaction.html` & `monopyly-1.4.0/monopyly/templates/common/transactions_table/linked_credit_transaction.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/templates/common/transactions_table/linked_transaction_overlay.html` & `monopyly-1.4.0/monopyly/templates/common/transactions_table/linked_transaction_overlay.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/templates/common/transactions_table/transaction_expanded.html` & `monopyly-1.4.0/monopyly/templates/common/transactions_table/transaction_expanded.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/templates/credit/account_page.html` & `monopyly-1.4.0/monopyly/templates/credit/account_page.html`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 {% block javascript %}
 
   <script>
     const UPDATE_CARD_STATUS_ENDPOINT = "{{ url_for('credit.update_card_status') }}";
     const UPDATE_ACCOUNT_STATEMENT_ISSUE_DAY_ENDPOINT = "{{ url_for('credit.update_account_statement_issue_day', account_id=account.id) }}";
     const UPDATE_ACCOUNT_STATEMENT_DUE_DAY_ENDPOINT = "{{ url_for('credit.update_account_statement_due_day', account_id=account.id) }}";
   </script>
-  <script src="{{ url_for('static', filename='js/flip_card.js') }}">
+  <script src="{{ url_for('static', filename='js/flip-card.js') }}">
   </script>
-  <script type="module" src="{{ url_for('static', filename='js/update_card_status.js') }}">
+  <script type="module" src="{{ url_for('static', filename='js/update-card-status.js') }}">
   </script>
-  <script type="module" src="{{ url_for('static', filename='js/update_account_statement_parameters.js') }}">
+  <script type="module" src="{{ url_for('static', filename='js/update-account-statement-parameters.js') }}">
   </script>
 
 {% endblock %}
```

### Comparing `monopyly-1.3.1/monopyly/templates/credit/cards.html` & `monopyly-1.4.0/monopyly/templates/credit/cards.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/templates/credit/statement_page.html` & `monopyly-1.4.0/monopyly/templates/credit/statement_page.html`

 * *Files 9% similar despite different names*

```diff
@@ -54,18 +54,18 @@
 
   <script>
     const UPDATE_STATEMENT_DUE_DATE_ENDPOINT = "{{ url_for('credit.update_statement_due_date', statement_id=statement.id) }}";
     const MAKE_PAYMENT_ENDPOINT = "{{ url_for('credit.pay_credit_card', card_id=statement.card_id, statement_id=statement.id) }}";
     const EXPAND_TRANSACTION_ENDPOINT = "{{ url_for('credit.expand_transaction') }}";
     const LINKED_TRANSACTION_ENDPOINT = "{{ url_for('credit.show_linked_transaction') }}";
   </script>
-  <script type="module" src="{{ url_for('static', filename='js/update_statement_parameters.js') }}">
+  <script type="module" src="{{ url_for('static', filename='js/update-statement-parameters.js') }}">
   </script>
-  <script type="module" src="{{ url_for('static', filename='js/make_payment.js') }}">
+  <script type="module" src="{{ url_for('static', filename='js/make-payment.js') }}">
   </script>
-  <script type="module" src="{{ url_for('static', filename='js/expand_transaction.js') }}">
+  <script type="module" src="{{ url_for('static', filename='js/expand-transaction.js') }}">
   </script>
-  <script type="module" src="{{ url_for('static', filename='js/show_linked_transaction.js') }}">
+  <script type="module" src="{{ url_for('static', filename='js/show-linked-transaction.js') }}">
   </script>
 
 {% endblock %}
```

### Comparing `monopyly-1.3.1/monopyly/templates/credit/statement_summary.html` & `monopyly-1.4.0/monopyly/templates/credit/statement_summary.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/templates/credit/statements.html` & `monopyly-1.4.0/monopyly/templates/credit/statements.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/templates/credit/statements_page.html` & `monopyly-1.4.0/monopyly/templates/credit/statements_page.html`

 * *Files 9% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 
 {% block content %}
 
   <div id="card-filter">
     {% for card in filter_cards %}
 
-      <a id="{{ card.account.bank.bank_name }}-{{ card.last_four_digits }}" class="card {{ 'active selected' if card.active else 'inactive' }}">
+      <a id="{{ card.account.bank.bank_name }}-{{ card.last_four_digits }}" class="card {{ 'active selected' if card.active else 'inactive' }}" data-card-id="{{ card.id }}">
         {{ card.account.bank.bank_name }} (-{{card.last_four_digits }})
       </a>
 
     {% endfor %}
   </div>
 
   <div id="credit-statements-container">
@@ -54,16 +54,16 @@
   <a name="bottom"></a>
 
 {% endblock %}
 
 
 {% block javascript %}
 
-  <script src="{{ url_for('static', filename='js/define_filter.js') }}">
+  <script src="{{ url_for('static', filename='js/define-filter.js') }}">
   </script>
   <script>
     const FILTER_ENDPOINT = "{{ url_for('credit.update_statements_display') }}";
   </script>
-  <script type="module" src="{{ url_for('static', filename='js/update_statements_display.js') }}">
+  <script type="module" src="{{ url_for('static', filename='js/update-statements-display.js') }}">
   </script>
 
 {% endblock %}
```

### Comparing `monopyly-1.3.1/monopyly/templates/credit/tags_page.html` & `monopyly-1.4.0/monopyly/templates/credit/tags_page.html`

 * *Files 2% similar despite different names*

```diff
@@ -31,11 +31,11 @@
 
 {% block javascript %}
 
   <script>
     const ADD_TAG_ENDPOINT = "{{ url_for('credit.add_tag') }}";
     const REMOVE_TAG_ENDPOINT = "{{ url_for('credit.delete_tag') }}";
   </script>
-  <script type="module" src="{{ url_for('static', filename='js/bind_tag_actions.js') }}">
+  <script type="module" src="{{ url_for('static', filename='js/bind-tag-actions.js') }}">
   </script>
 
 {% endblock %}
```

### Comparing `monopyly-1.3.1/monopyly/templates/credit/transaction_submission_page.html` & `monopyly-1.4.0/monopyly/templates/credit/transaction_submission_page.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/templates/credit/transactions_page.html` & `monopyly-1.4.0/monopyly/templates/credit/transactions_page.html`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 
 {% block content %}
 
   <div id="card-filter">
     {% for card in filter_cards %}
 
-    <a id="{{ card.account.bank.bank_name }}-{{ card.last_four_digits }}" class="card {{ 'active' if card.active else 'inactive' }}{{ ' selected' if card.id in selected_card_ids else '' }}">
+    <a id="{{ card.account.bank.bank_name }}-{{ card.last_four_digits }}" class="card {{ 'active' if card.active else 'inactive' }}{{ ' selected' if card.id in selected_card_ids else '' }}" data-card-id="{{ card.id }}">
         {{ card.account.bank.bank_name }} (-{{card.last_four_digits }})
       </a>
 
     {% endfor %}
   </div>
 
   <div class="transactions-container">
@@ -68,22 +68,22 @@
   <a name="bottom"></a>
 
 {% endblock %}
 
 
 {% block javascript %}
 
-  <script src="{{ url_for('static', filename='js/define_filter.js') }}">
+  <script src="{{ url_for('static', filename='js/define-filter.js') }}">
   </script>
   <script>
     const FILTER_ENDPOINT = "{{ url_for('credit.update_transactions_display') }}";
     const EXPAND_TRANSACTION_ENDPOINT = "{{ url_for('credit.expand_transaction') }}";
     const LINKED_TRANSACTION_ENDPOINT = "{{ url_for('credit.show_linked_transaction') }}";
   </script>
-  <script type="module" src="{{ url_for('static', filename='js/update_transactions_display.js') }}">
+  <script type="module" src="{{ url_for('static', filename='js/update-transactions-display.js') }}">
   </script>
-  <script type="module" src="{{ url_for('static', filename='js/expand_transaction.js') }}">
+  <script type="module" src="{{ url_for('static', filename='js/expand-transaction.js') }}">
   </script>
-  <script type="module" src="{{ url_for('static', filename='js/show_linked_transaction.js') }}">
+  <script type="module" src="{{ url_for('static', filename='js/show-linked-transaction.js') }}">
   </script>
 
 {% endblock %}
```

### Comparing `monopyly-1.3.1/monopyly/templates/credit/card_form/card_form.html` & `monopyly-1.4.0/monopyly/templates/credit/card_form/card_form.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/templates/credit/card_form/card_form_page_new.html` & `monopyly-1.4.0/monopyly/templates/credit/card_form/card_form_page_new.html`

 * *Files 20% similar despite different names*

```diff
@@ -15,10 +15,10 @@
   {% if transfer_statement_form %}
     {% include 'credit/card_form/transfer_statement_inquiry.html' %}
   {% endif %}
 
 {% endblock %}
 
 {% block javascript %}
-  <script type="module" src="{{ url_for('static', filename='js/display_new_credit_account_inputs.js') }}">
+  <script type="module" src="{{ url_for('static', filename='js/display-new-credit-account-inputs.js') }}">
   </script>
 {% endblock %}
```

### Comparing `monopyly-1.3.1/monopyly/templates/credit/card_form/transfer_statement_inquiry.html` & `monopyly-1.4.0/monopyly/templates/credit/card_form/transfer_statement_inquiry.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/templates/credit/card_graphic/card_back.html` & `monopyly-1.4.0/monopyly/templates/credit/card_graphic/card_back.html`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   <div class="digits obscure">▐▐▐▐</div>
   <div class="digits">{{ card.last_four_digits }}</div>
 </div>
 
 <div class="options">
 
   <label class="toggle-switch-gadget" for="card-{{ card.id }}-status">
-    <input id="card-{{ card.id }}-status" type="checkbox" {{ 'checked' if card.active else '' }}/>
+    <input id="card-{{ card.id }}-status" data-card-id="{{ card.id }}" type="checkbox" {{ 'checked' if card.active else '' }}/>
 
     <div class="option">
       <div class="text">
         Active
       </div>
       <div class="slider">
         <div class="switch"></div>
```

### Comparing `monopyly-1.3.1/monopyly/templates/credit/card_graphic/card_front.html` & `monopyly-1.4.0/monopyly/templates/credit/card_graphic/card_front.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/templates/credit/tag_tree/subtag_tree.html` & `monopyly-1.4.0/monopyly/templates/credit/tag_tree/subtag_tree.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/templates/credit/transaction_form/transaction_form.html` & `monopyly-1.4.0/monopyly/templates/credit/transaction_form/transaction_form.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/templates/credit/transaction_form/transaction_form_page.html` & `monopyly-1.4.0/monopyly/templates/credit/transaction_form/transaction_form_page.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-{% extends "common/form_page.html" %}
+{% extends "common/transaction_form/transaction_form_page.html" %}
 
 
 {% block javascript %}
 
   <script>
     const AUTOCOMPLETE_ENDPOINT = "{{ url_for('credit.suggest_transaction_autocomplete') }}";
     const INFER_CARD_ENDPOINT = "{{ url_for('credit.infer_card') }}";
     const INFER_STATEMENT_ENDPOINT = "{{ url_for('credit.infer_statement') }}";
     const ADD_SUBTRANSACTION_FORM_ENDPOINT = "{{ url_for('credit.add_subtransaction_fields') }}";
   </script>
-  <script type="module" src="{{ url_for('static', filename='js/autocomplete_transaction.js') }}">
+  <script type="module" src="{{ url_for('static', filename='js/infer-card.js') }}">
   </script>
-  <script type="module" src="{{ url_for('static', filename='js/infer_card.js') }}">
-  </script>
-  <script type="module" src="{{ url_for('static', filename='js/infer_statement.js') }}">
-  </script>
-  <script type="module" src="{{ url_for('static', filename='js/add_subtransaction.js') }}">
+  <script type="module" src="{{ url_for('static', filename='js/infer-statement.js') }}">
   </script>
+  {{ super() }}
 
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,2 +1,3 @@
-{% extends "common/form_page.html" %} {% block javascript %}
- {% endblock %}
+{% extends "common/transaction_form/transaction_form_page.html" %} {% block
+javascript %}
+ {{ super() }} {% endblock %}
```

### Comparing `monopyly-1.3.1/monopyly/templates/credit/transactions_table/condensed_row_content.html` & `monopyly-1.4.0/monopyly/templates/credit/transactions_table/condensed_row_content.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/templates/credit/transactions_table/expanded_row_content.html` & `monopyly-1.4.0/monopyly/templates/credit/transactions_table/expanded_row_content.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/monopyly/templates/credit/transactions_table/transaction_field_titles.html` & `monopyly-1.4.0/monopyly/templates/credit/transactions_table/transaction_field_titles.html`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/.gitignore` & `monopyly-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/COPYING` & `monopyly-1.4.0/COPYING`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/pyproject.toml` & `monopyly-1.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `monopyly-1.3.1/PKG-INFO` & `monopyly-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monopyly
-Version: 1.3.1
+Version: 1.4.0
 Summary: A homemade personal finance manager.
 Project-URL: Download, https://pypi.org/project/monopyly
 Project-URL: Homepage, https://github.com/mitchnegus/monopyly
 Project-URL: Repository, https://github.com/mitchnegus/monopyly
 Project-URL: Changelog, https://github.com/mitchnegus/monopyly/blob/main/CHANGELOG.md
 Author-email: Mitch Negus <mitchnegus57@gmail.com>
 License: GNU GPLv3
```

