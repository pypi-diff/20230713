# Comparing `tmp/sfctools-1.1.0.2.tar.gz` & `tmp/sfctools-1.1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sfctools-1.1.0.2.tar", max compression
+gzip compressed data, was "sfctools-1.1.0.3.tar", max compression
```

## Comparing `sfctools-1.1.0.2.tar` & `sfctools-1.1.0.3.tar`

### file list

```diff
@@ -1,110 +1,110 @@
--rw-r--r--   0        0        0     1157 2022-11-23 08:34:47.643840 sfctools-1.1.0.2/LICENSE
--rw-r--r--   0        0        0     1620 2023-07-04 09:46:03.075401 sfctools-1.1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1865 2023-06-23 11:07:04.102942 sfctools-1.1.0.2/README.md
--rw-r--r--   0        0        0     1938 2022-11-23 08:34:47.783372 sfctools-1.1.0.2/sfctools/__init__.py
--rw-r--r--   0        0        0     2655 2023-01-26 10:34:36.652567 sfctools-1.1.0.2/sfctools/__main__.py
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.785439 sfctools-1.1.0.2/sfctools/automation/__init__.py
--rw-r--r--   0        0        0    10574 2023-03-21 16:33:08.099326 sfctools-1.1.0.2/sfctools/automation/calibration.py
--rw-r--r--   0        0        0    14589 2023-03-21 16:33:08.100325 sfctools-1.1.0.2/sfctools/automation/cgesolver.py
--rw-r--r--   0        0        0       75 2022-11-23 08:34:47.785439 sfctools-1.1.0.2/sfctools/automation/README.md
--rw-r--r--   0        0        0     5077 2022-11-23 08:34:47.790242 sfctools-1.1.0.2/sfctools/automation/runner.py
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.791250 sfctools-1.1.0.2/sfctools/bottomup/__init__.py
--rw-r--r--   0        0        0     8900 2023-01-26 10:34:36.653567 sfctools-1.1.0.2/sfctools/bottomup/matching.py
--rw-r--r--   0        0        0    17465 2023-03-21 16:33:08.101324 sfctools-1.1.0.2/sfctools/bottomup/productiontree.py
--rw-r--r--   0        0        0     6904 2022-11-23 08:34:47.794005 sfctools-1.1.0.2/sfctools/bottomup/stock_manager.py
--rw-r--r--   0        0        0     2737 2022-11-23 08:34:47.795896 sfctools-1.1.0.2/sfctools/bottomup/treestruct.py
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.796902 sfctools-1.1.0.2/sfctools/core/__init__.py
--rw-r--r--   0        0        0     7572 2022-11-23 08:34:47.797213 sfctools-1.1.0.2/sfctools/core/agent.py
--rw-r--r--   0        0        0     2249 2022-11-23 08:34:47.798441 sfctools-1.1.0.2/sfctools/core/clock.py
--rw-r--r--   0        0        0      495 2023-03-21 16:33:08.101324 sfctools-1.1.0.2/sfctools/core/custom_warnings.py
--rw-r--r--   0        0        0    15252 2023-06-23 11:02:51.691877 sfctools-1.1.0.2/sfctools/core/flow_matrix.py
--rw-r--r--   0        0        0    11632 2023-03-21 16:33:08.102324 sfctools-1.1.0.2/sfctools/core/settings.py
--rw-r--r--   0        0        0      661 2022-11-23 08:34:47.802978 sfctools-1.1.0.2/sfctools/core/singleton.py
--rw-r--r--   0        0        0     7304 2023-01-26 10:34:36.655075 sfctools-1.1.0.2/sfctools/core/world.py
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.805666 sfctools-1.1.0.2/sfctools/datastructs/__init__.py
--rw-r--r--   0        0        0    32494 2023-03-21 16:33:08.103324 sfctools-1.1.0.2/sfctools/datastructs/balance.py
--rw-r--r--   0        0        0    17441 2023-01-26 10:34:36.656502 sfctools-1.1.0.2/sfctools/datastructs/bank_order_book.py
--rw-r--r--   0        0        0     6175 2023-03-21 16:33:08.104324 sfctools-1.1.0.2/sfctools/datastructs/cash_flow_statement.py
--rw-r--r--   0        0        0     4900 2022-11-23 08:34:47.810921 sfctools-1.1.0.2/sfctools/datastructs/collection.py
--rw-r--r--   0        0        0    14094 2023-06-23 11:02:51.692877 sfctools-1.1.0.2/sfctools/datastructs/income_statement.py
--rw-r--r--   0        0        0     6043 2022-11-23 08:34:47.812908 sfctools-1.1.0.2/sfctools/datastructs/inventory.py
--rw-r--r--   0        0        0     4272 2022-11-23 08:34:47.813916 sfctools-1.1.0.2/sfctools/datastructs/market_registry.py
--rw-r--r--   0        0        0     5313 2022-11-23 08:34:47.815910 sfctools-1.1.0.2/sfctools/datastructs/signalslot.py
--rw-r--r--   0        0        0     3096 2023-06-23 11:02:51.692877 sfctools-1.1.0.2/sfctools/datastructs/worker_registry.py
--rw-r--r--   0        0        0      591 2023-06-23 11:02:51.693876 sfctools-1.1.0.2/sfctools/examples/__init__.py
--rw-r--r--   0        0        0     2491 2023-03-21 16:33:08.105387 sfctools-1.1.0.2/sfctools/examples/balance.py
--rw-r--r--   0        0        0     1811 2023-06-23 11:02:51.693876 sfctools-1.1.0.2/sfctools/examples/basic_example/basic_example.py
--rw-r--r--   0        0        0      202 2023-03-21 16:33:08.106499 sfctools-1.1.0.2/sfctools/examples/basic_example/my_settings.yml
--rw-r--r--   0        0        0     1087 2023-03-21 16:33:08.106499 sfctools-1.1.0.2/sfctools/examples/clock.py
--rw-r--r--   0        0        0     1397 2023-06-23 11:02:51.694877 sfctools-1.1.0.2/sfctools/examples/example_wrapper.py
--rw-r--r--   0        0        0        0 2023-03-21 16:33:08.107730 sfctools-1.1.0.2/sfctools/examples/exampleabm/agents/__init__.py
--rw-r--r--   0        0        0     1845 2023-03-21 16:33:08.107730 sfctools-1.1.0.2/sfctools/examples/exampleabm/agents/government.py
--rw-r--r--   0        0        0     2370 2023-03-21 16:33:08.108754 sfctools-1.1.0.2/sfctools/examples/exampleabm/agents/household.py
--rw-r--r--   0        0        0     2198 2023-03-21 16:33:08.108754 sfctools-1.1.0.2/sfctools/examples/exampleabm/agents/production.py
--rw-r--r--   0        0        0     4365 2023-03-21 16:33:08.108754 sfctools-1.1.0.2/sfctools/examples/exampleabm/agents/transactions.py
--rw-r--r--   0        0        0      910 2023-03-21 16:33:08.109754 sfctools-1.1.0.2/sfctools/examples/exampleabm/data/preprocess.py
--rw-r--r--   0        0        0    13152 2023-03-21 16:33:08.109754 sfctools-1.1.0.2/sfctools/examples/exampleabm/data/processed/tipsau20_gdp_processed.txt
--rw-r--r--   0        0        0      818 2023-03-21 16:33:08.110388 sfctools-1.1.0.2/sfctools/examples/exampleabm/data/raw/tipsau20_gdp.csv
--rw-r--r--   0        0        0    31241 2023-03-21 16:33:08.111510 sfctools-1.1.0.2/sfctools/examples/exampleabm/figures/matrix.png
--rw-r--r--   0        0        0    42423 2023-03-21 16:33:08.111510 sfctools-1.1.0.2/sfctools/examples/exampleabm/figures/outputs.png
--rw-r--r--   0        0        0    43865 2023-03-21 16:33:08.112510 sfctools-1.1.0.2/sfctools/examples/exampleabm/figures/sankey.png
--rw-r--r--   0        0        0     1264 2023-03-21 16:33:08.112510 sfctools-1.1.0.2/sfctools/examples/exampleabm/info.md
--rw-r--r--   0        0        0     3730 2023-03-21 16:33:08.113510 sfctools-1.1.0.2/sfctools/examples/exampleabm/model.py
--rw-r--r--   0        0        0     1148 2023-03-21 16:33:08.113510 sfctools-1.1.0.2/sfctools/examples/exampleabm/settings.yml
--rw-r--r--   0        0        0     2805 2023-03-21 16:33:08.113510 sfctools-1.1.0.2/sfctools/examples/flowmatrix.py
--rw-r--r--   0        0        0      813 2023-03-21 16:33:08.114513 sfctools-1.1.0.2/sfctools/examples/hello_agent.py
--rw-r--r--   0        0        0     1249 2023-06-23 11:02:51.694877 sfctools-1.1.0.2/sfctools/examples/inventory.py
--rw-r--r--   0        0        0     1839 2023-06-23 11:02:51.695876 sfctools-1.1.0.2/sfctools/examples/market_example/market.py
--rw-r--r--   0        0        0     2791 2023-06-23 11:02:51.695876 sfctools-1.1.0.2/sfctools/examples/market_example/market2.py
--rw-r--r--   0        0        0     2548 2023-06-23 11:02:51.696877 sfctools-1.1.0.2/sfctools/examples/monte_carlo/monte_carlo.py
--rw-r--r--   0        0        0      188 2023-06-23 11:02:51.697422 sfctools-1.1.0.2/sfctools/examples/monte_carlo/testsettings.yml
--rw-r--r--   0        0        0     3907 2023-06-23 17:31:16.217873 sfctools-1.1.0.2/sfctools/examples/order_book.py
--rw-r--r--   0        0        0      124 2023-03-21 16:33:08.119972 sfctools-1.1.0.2/sfctools/examples/paper_example.py
--rw-r--r--   0        0        0      798 2023-06-23 11:02:51.697878 sfctools-1.1.0.2/sfctools/examples/readme_example.py
--rw-r--r--   0        0        0     1561 2023-06-23 11:02:51.698876 sfctools-1.1.0.2/sfctools/examples/signal_slot.py
--rw-r--r--   0        0        0     1285 2023-06-23 11:02:51.698876 sfctools-1.1.0.2/sfctools/examples/worker_registry.py
--rw-r--r--   0        0        0       27 2022-11-23 08:34:47.817910 sfctools-1.1.0.2/sfctools/gui/.gitignore
--rw-r--r--   0        0        0      854 2022-11-23 08:34:47.818915 sfctools-1.1.0.2/sfctools/gui/.gitlab-ci.yml
--rw-r--r--   0        0        0       64 2022-11-23 08:34:47.822910 sfctools-1.1.0.2/sfctools/gui/__init__.py
--rw-r--r--   0        0        0       41 2022-11-23 08:34:47.824049 sfctools-1.1.0.2/sfctools/gui/attune/.gitignore
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.824049 sfctools-1.1.0.2/sfctools/gui/attune/__init__.py
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.825207 sfctools-1.1.0.2/sfctools/gui/attune/src/__init__.py
--rw-r--r--   0        0        0    34562 2023-06-23 11:02:51.699876 sfctools-1.1.0.2/sfctools/gui/attune/src/agent_editor.py
--rw-r--r--   0        0        0     6944 2023-06-23 11:02:51.699876 sfctools-1.1.0.2/sfctools/gui/attune/src/code_editor.ui
--rw-r--r--   0        0        0    76992 2023-07-04 09:46:03.076666 sfctools-1.1.0.2/sfctools/gui/attune/src/draw_widget.py
--rw-r--r--   0        0        0     1645 2023-01-26 10:34:36.660166 sfctools-1.1.0.2/sfctools/gui/attune/src/income_viewer.ui
--rw-r--r--   0        0        0    13478 2023-06-23 11:02:51.701876 sfctools-1.1.0.2/sfctools/gui/attune/src/mainloop_editor.py
--rw-r--r--   0        0        0     8176 2023-01-26 10:34:36.661270 sfctools-1.1.0.2/sfctools/gui/attune/src/mamba_interpreter2.py
--rw-r--r--   0        0        0     1334 2023-03-21 16:33:08.123171 sfctools-1.1.0.2/sfctools/gui/attune/src/matrix_viewer.ui
--rw-r--r--   0        0        0     1199 2023-07-04 09:26:32.598315 sfctools-1.1.0.2/sfctools/gui/attune/src/my_interpolation.py
--rw-r--r--   0        0        0    19411 2023-03-21 16:33:08.124171 sfctools-1.1.0.2/sfctools/gui/attune/src/output_display.py
--rw-r--r--   0        0        0    11200 2022-11-23 08:34:47.835944 sfctools-1.1.0.2/sfctools/gui/attune/src/output_display.ui
--rw-r--r--   0        0        0     1066 2023-06-23 11:02:51.701876 sfctools-1.1.0.2/sfctools/gui/attune/src/pandasmodel.py
--rw-r--r--   0        0        0   137422 2023-06-23 17:31:16.220161 sfctools-1.1.0.2/sfctools/gui/attune/src/qtattune.py
--rw-r--r--   0        0        0    24104 2022-11-23 08:34:47.840835 sfctools-1.1.0.2/sfctools/gui/attune/src/resources.py
--rw-r--r--   0        0        0      107 2022-11-23 08:34:47.840835 sfctools-1.1.0.2/sfctools/gui/attune/src/resources.qrc
--rw-r--r--   0        0        0     1259 2023-06-23 11:02:51.703877 sfctools-1.1.0.2/sfctools/gui/attune/src/search_dialog.ui
--rw-r--r--   0        0        0     5927 2023-03-21 16:33:08.126466 sfctools-1.1.0.2/sfctools/gui/attune/src/settings_edit.ui
--rw-r--r--   0        0        0     3012 2023-03-21 16:33:08.127467 sfctools-1.1.0.2/sfctools/gui/attune/src/simulation_edit.ui
--rw-r--r--   0        0        0      216 2023-07-04 09:26:12.233558 sfctools-1.1.0.2/sfctools/gui/attune/src/styles/bright/background.txt
--rw-r--r--   0        0        0     4018 2023-07-04 09:26:32.598315 sfctools-1.1.0.2/sfctools/gui/attune/src/styles/bright/main.txt
--rw-r--r--   0        0        0       62 2023-01-26 10:34:36.665242 sfctools-1.1.0.2/sfctools/gui/attune/src/styles/bright/tables.txt
--rw-r--r--   0        0        0      727 2023-01-26 10:34:36.665497 sfctools-1.1.0.2/sfctools/gui/attune/src/styles/dark/background.txt
--rw-r--r--   0        0        0     4228 2023-03-21 16:33:08.128524 sfctools-1.1.0.2/sfctools/gui/attune/src/styles/dark/main.txt
--rw-r--r--   0        0        0       37 2023-01-26 10:34:36.666498 sfctools-1.1.0.2/sfctools/gui/attune/src/styles/dark/tables.txt
--rw-r--r--   0        0        0     6968 2023-07-04 09:26:32.599316 sfctools-1.1.0.2/sfctools/gui/attune/src/theme_manager.py
--rw-r--r--   0        0        0    85503 2023-07-04 09:46:03.077402 sfctools-1.1.0.2/sfctools/gui/attune/src/transaction_designer_mainwindow.ui
--rw-r--r--   0        0        0    11727 2023-07-04 09:26:32.601318 sfctools-1.1.0.2/sfctools/gui/attune/src/yaml_editor.py
--rw-r--r--   0        0        0      357 2023-03-21 16:33:08.130565 sfctools-1.1.0.2/sfctools/gui/attune_main.py
--rw-r--r--   0        0        0      389 2023-03-21 16:33:08.130565 sfctools-1.1.0.2/sfctools/gui/attune_starter.py
--rw-r--r--   0        0        0    27804 2022-11-23 08:34:47.819952 sfctools-1.1.0.2/sfctools/gui/CLA.pdf
--rw-r--r--   0        0        0     1434 2022-11-23 08:34:47.820915 sfctools-1.1.0.2/sfctools/gui/CONTRIBUTING.md
--rw-r--r--   0        0        0     1157 2022-11-23 08:34:47.821917 sfctools-1.1.0.2/sfctools/gui/LICENSE
--rw-r--r--   0        0        0      819 2023-01-26 10:34:36.656502 sfctools-1.1.0.2/sfctools/gui/README.md
--rw-r--r--   0        0        0       47 2022-12-22 09:03:58.496002 sfctools-1.1.0.2/sfctools/gui/runner.py
--rw-r--r--   0        0        0      275 2023-06-23 11:02:51.705877 sfctools-1.1.0.2/sfctools/gui/sfctheme
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.855670 sfctools-1.1.0.2/sfctools/misc/__init__.py
--rw-r--r--   0        0        0    21989 2023-06-23 11:02:51.706741 sfctools-1.1.0.2/sfctools/misc/mpl_plotting.py
--rw-r--r--   0        0        0     7795 2023-03-21 16:33:08.131566 sfctools-1.1.0.2/sfctools/misc/reporting_sheet.py
--rw-r--r--   0        0        0     7074 2022-11-23 08:34:47.858698 sfctools-1.1.0.2/sfctools/misc/timeseries.py
--rw-r--r--   0        0        0     3430 1970-01-01 00:00:00.000000 sfctools-1.1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1157 2023-07-12 14:00:56.426582 sfctools-1.1.0.3/LICENSE
+-rw-r--r--   0        0        0     1620 2023-07-13 10:05:03.820781 sfctools-1.1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1945 2023-07-12 14:00:56.427602 sfctools-1.1.0.3/README.md
+-rw-r--r--   0        0        0     1938 2023-07-12 14:00:56.450604 sfctools-1.1.0.3/sfctools/__init__.py
+-rw-r--r--   0        0        0     2655 2023-07-12 14:00:56.451604 sfctools-1.1.0.3/sfctools/__main__.py
+-rw-r--r--   0        0        0        0 2023-07-12 14:00:56.451604 sfctools-1.1.0.3/sfctools/automation/__init__.py
+-rw-r--r--   0        0        0    10574 2023-07-12 14:00:56.451604 sfctools-1.1.0.3/sfctools/automation/calibration.py
+-rw-r--r--   0        0        0    14589 2023-07-12 14:00:56.451604 sfctools-1.1.0.3/sfctools/automation/cgesolver.py
+-rw-r--r--   0        0        0       75 2023-07-12 14:00:56.451604 sfctools-1.1.0.3/sfctools/automation/README.md
+-rw-r--r--   0        0        0     5077 2023-07-12 14:00:56.452603 sfctools-1.1.0.3/sfctools/automation/runner.py
+-rw-r--r--   0        0        0        0 2023-07-12 14:00:56.452603 sfctools-1.1.0.3/sfctools/bottomup/__init__.py
+-rw-r--r--   0        0        0     8900 2023-07-12 14:00:56.452603 sfctools-1.1.0.3/sfctools/bottomup/matching.py
+-rw-r--r--   0        0        0    17465 2023-07-12 14:00:56.452603 sfctools-1.1.0.3/sfctools/bottomup/productiontree.py
+-rw-r--r--   0        0        0     6904 2023-07-12 14:00:56.453604 sfctools-1.1.0.3/sfctools/bottomup/stock_manager.py
+-rw-r--r--   0        0        0     2737 2023-07-12 14:00:56.453604 sfctools-1.1.0.3/sfctools/bottomup/treestruct.py
+-rw-r--r--   0        0        0        0 2023-07-12 14:00:56.453604 sfctools-1.1.0.3/sfctools/core/__init__.py
+-rw-r--r--   0        0        0     7572 2023-07-12 14:00:56.453604 sfctools-1.1.0.3/sfctools/core/agent.py
+-rw-r--r--   0        0        0     2249 2023-07-12 14:00:56.453604 sfctools-1.1.0.3/sfctools/core/clock.py
+-rw-r--r--   0        0        0      495 2023-07-12 14:00:56.453604 sfctools-1.1.0.3/sfctools/core/custom_warnings.py
+-rw-r--r--   0        0        0    15252 2023-07-12 14:00:56.454604 sfctools-1.1.0.3/sfctools/core/flow_matrix.py
+-rw-r--r--   0        0        0    11632 2023-07-12 14:00:56.454604 sfctools-1.1.0.3/sfctools/core/settings.py
+-rw-r--r--   0        0        0      661 2023-07-12 14:00:56.454604 sfctools-1.1.0.3/sfctools/core/singleton.py
+-rw-r--r--   0        0        0     7304 2023-07-12 14:00:56.454604 sfctools-1.1.0.3/sfctools/core/world.py
+-rw-r--r--   0        0        0        0 2023-07-12 14:00:56.455604 sfctools-1.1.0.3/sfctools/datastructs/__init__.py
+-rw-r--r--   0        0        0    32494 2023-07-12 14:00:56.455604 sfctools-1.1.0.3/sfctools/datastructs/balance.py
+-rw-r--r--   0        0        0    17441 2023-07-12 14:00:56.455604 sfctools-1.1.0.3/sfctools/datastructs/bank_order_book.py
+-rw-r--r--   0        0        0     6175 2023-07-12 14:00:56.455604 sfctools-1.1.0.3/sfctools/datastructs/cash_flow_statement.py
+-rw-r--r--   0        0        0     4900 2023-07-12 14:00:56.456604 sfctools-1.1.0.3/sfctools/datastructs/collection.py
+-rw-r--r--   0        0        0    14094 2023-07-12 14:00:56.456604 sfctools-1.1.0.3/sfctools/datastructs/income_statement.py
+-rw-r--r--   0        0        0     6043 2023-07-12 14:00:56.456604 sfctools-1.1.0.3/sfctools/datastructs/inventory.py
+-rw-r--r--   0        0        0     4272 2023-07-12 14:00:56.456604 sfctools-1.1.0.3/sfctools/datastructs/market_registry.py
+-rw-r--r--   0        0        0     5313 2023-07-12 14:00:56.456604 sfctools-1.1.0.3/sfctools/datastructs/signalslot.py
+-rw-r--r--   0        0        0     3096 2023-07-12 14:00:56.456604 sfctools-1.1.0.3/sfctools/datastructs/worker_registry.py
+-rw-r--r--   0        0        0      591 2023-07-12 14:00:56.457604 sfctools-1.1.0.3/sfctools/examples/__init__.py
+-rw-r--r--   0        0        0     2491 2023-07-12 14:00:56.457604 sfctools-1.1.0.3/sfctools/examples/balance.py
+-rw-r--r--   0        0        0     1811 2023-07-12 14:00:56.457604 sfctools-1.1.0.3/sfctools/examples/basic_example/basic_example.py
+-rw-r--r--   0        0        0      202 2023-07-12 14:00:56.457604 sfctools-1.1.0.3/sfctools/examples/basic_example/my_settings.yml
+-rw-r--r--   0        0        0     1087 2023-07-12 14:00:56.457604 sfctools-1.1.0.3/sfctools/examples/clock.py
+-rw-r--r--   0        0        0     1397 2023-07-12 14:00:56.458604 sfctools-1.1.0.3/sfctools/examples/example_wrapper.py
+-rw-r--r--   0        0        0        0 2023-07-12 14:00:56.458604 sfctools-1.1.0.3/sfctools/examples/exampleabm/agents/__init__.py
+-rw-r--r--   0        0        0     1845 2023-07-12 14:00:56.458604 sfctools-1.1.0.3/sfctools/examples/exampleabm/agents/government.py
+-rw-r--r--   0        0        0     2370 2023-07-12 14:00:56.458604 sfctools-1.1.0.3/sfctools/examples/exampleabm/agents/household.py
+-rw-r--r--   0        0        0     2198 2023-07-12 14:00:56.458604 sfctools-1.1.0.3/sfctools/examples/exampleabm/agents/production.py
+-rw-r--r--   0        0        0     4365 2023-07-12 14:00:56.459603 sfctools-1.1.0.3/sfctools/examples/exampleabm/agents/transactions.py
+-rw-r--r--   0        0        0      910 2023-07-12 14:00:56.459603 sfctools-1.1.0.3/sfctools/examples/exampleabm/data/preprocess.py
+-rw-r--r--   0        0        0    13152 2023-07-12 14:00:56.459603 sfctools-1.1.0.3/sfctools/examples/exampleabm/data/processed/tipsau20_gdp_processed.txt
+-rw-r--r--   0        0        0      818 2023-07-12 14:00:56.459603 sfctools-1.1.0.3/sfctools/examples/exampleabm/data/raw/tipsau20_gdp.csv
+-rw-r--r--   0        0        0    31241 2023-07-12 14:00:56.460605 sfctools-1.1.0.3/sfctools/examples/exampleabm/figures/matrix.png
+-rw-r--r--   0        0        0    42423 2023-07-12 14:00:56.460605 sfctools-1.1.0.3/sfctools/examples/exampleabm/figures/outputs.png
+-rw-r--r--   0        0        0    43865 2023-07-12 14:00:56.461604 sfctools-1.1.0.3/sfctools/examples/exampleabm/figures/sankey.png
+-rw-r--r--   0        0        0     1264 2023-07-12 14:00:56.461604 sfctools-1.1.0.3/sfctools/examples/exampleabm/info.md
+-rw-r--r--   0        0        0     3730 2023-07-12 14:00:56.461604 sfctools-1.1.0.3/sfctools/examples/exampleabm/model.py
+-rw-r--r--   0        0        0     1148 2023-07-12 14:00:56.461604 sfctools-1.1.0.3/sfctools/examples/exampleabm/settings.yml
+-rw-r--r--   0        0        0     2805 2023-07-12 14:00:56.462604 sfctools-1.1.0.3/sfctools/examples/flowmatrix.py
+-rw-r--r--   0        0        0      813 2023-07-12 14:00:56.462604 sfctools-1.1.0.3/sfctools/examples/hello_agent.py
+-rw-r--r--   0        0        0     1249 2023-07-12 14:00:56.462604 sfctools-1.1.0.3/sfctools/examples/inventory.py
+-rw-r--r--   0        0        0     1839 2023-07-12 14:00:56.462604 sfctools-1.1.0.3/sfctools/examples/market_example/market.py
+-rw-r--r--   0        0        0     2791 2023-07-12 14:00:56.462604 sfctools-1.1.0.3/sfctools/examples/market_example/market2.py
+-rw-r--r--   0        0        0     2548 2023-07-12 14:00:56.463604 sfctools-1.1.0.3/sfctools/examples/monte_carlo/monte_carlo.py
+-rw-r--r--   0        0        0      188 2023-07-12 14:00:56.463604 sfctools-1.1.0.3/sfctools/examples/monte_carlo/testsettings.yml
+-rw-r--r--   0        0        0     3907 2023-07-12 14:00:56.463604 sfctools-1.1.0.3/sfctools/examples/order_book.py
+-rw-r--r--   0        0        0      124 2023-07-12 14:00:56.463604 sfctools-1.1.0.3/sfctools/examples/paper_example.py
+-rw-r--r--   0        0        0      798 2023-07-12 14:00:56.463604 sfctools-1.1.0.3/sfctools/examples/readme_example.py
+-rw-r--r--   0        0        0     1561 2023-07-12 14:00:56.463604 sfctools-1.1.0.3/sfctools/examples/signal_slot.py
+-rw-r--r--   0        0        0     1285 2023-07-12 14:00:56.464604 sfctools-1.1.0.3/sfctools/examples/worker_registry.py
+-rw-r--r--   0        0        0       27 2023-07-12 14:00:56.464604 sfctools-1.1.0.3/sfctools/gui/.gitignore
+-rw-r--r--   0        0        0      854 2023-07-12 14:00:56.464604 sfctools-1.1.0.3/sfctools/gui/.gitlab-ci.yml
+-rw-r--r--   0        0        0       64 2023-07-12 14:00:56.465604 sfctools-1.1.0.3/sfctools/gui/__init__.py
+-rw-r--r--   0        0        0       41 2023-07-12 14:00:56.465604 sfctools-1.1.0.3/sfctools/gui/attune/.gitignore
+-rw-r--r--   0        0        0        0 2023-07-12 14:00:56.465604 sfctools-1.1.0.3/sfctools/gui/attune/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 14:00:56.465604 sfctools-1.1.0.3/sfctools/gui/attune/src/__init__.py
+-rw-r--r--   0        0        0    34562 2023-07-12 14:00:56.466604 sfctools-1.1.0.3/sfctools/gui/attune/src/agent_editor.py
+-rw-r--r--   0        0        0     6944 2023-07-12 14:00:56.466604 sfctools-1.1.0.3/sfctools/gui/attune/src/code_editor.ui
+-rw-r--r--   0        0        0    77010 2023-07-12 14:08:04.372782 sfctools-1.1.0.3/sfctools/gui/attune/src/draw_widget.py
+-rw-r--r--   0        0        0     1645 2023-07-12 14:00:56.467604 sfctools-1.1.0.3/sfctools/gui/attune/src/income_viewer.ui
+-rw-r--r--   0        0        0    13478 2023-07-12 14:00:56.467604 sfctools-1.1.0.3/sfctools/gui/attune/src/mainloop_editor.py
+-rw-r--r--   0        0        0     8176 2023-07-12 14:00:56.468605 sfctools-1.1.0.3/sfctools/gui/attune/src/mamba_interpreter2.py
+-rw-r--r--   0        0        0     1334 2023-07-12 14:00:56.468605 sfctools-1.1.0.3/sfctools/gui/attune/src/matrix_viewer.ui
+-rw-r--r--   0        0        0     1199 2023-07-12 14:00:56.468605 sfctools-1.1.0.3/sfctools/gui/attune/src/my_interpolation.py
+-rw-r--r--   0        0        0    19411 2023-07-12 14:00:56.468605 sfctools-1.1.0.3/sfctools/gui/attune/src/output_display.py
+-rw-r--r--   0        0        0    11200 2023-07-12 14:00:56.469605 sfctools-1.1.0.3/sfctools/gui/attune/src/output_display.ui
+-rw-r--r--   0        0        0     1066 2023-07-12 14:00:56.469605 sfctools-1.1.0.3/sfctools/gui/attune/src/pandasmodel.py
+-rw-r--r--   0        0        0   137422 2023-07-12 14:00:56.470605 sfctools-1.1.0.3/sfctools/gui/attune/src/qtattune.py
+-rw-r--r--   0        0        0    24104 2023-07-12 14:00:56.470605 sfctools-1.1.0.3/sfctools/gui/attune/src/resources.py
+-rw-r--r--   0        0        0      107 2023-07-12 14:00:56.470605 sfctools-1.1.0.3/sfctools/gui/attune/src/resources.qrc
+-rw-r--r--   0        0        0     1259 2023-07-12 14:00:56.470605 sfctools-1.1.0.3/sfctools/gui/attune/src/search_dialog.ui
+-rw-r--r--   0        0        0     5927 2023-07-12 14:00:56.470605 sfctools-1.1.0.3/sfctools/gui/attune/src/settings_edit.ui
+-rw-r--r--   0        0        0     3012 2023-07-12 14:00:56.471604 sfctools-1.1.0.3/sfctools/gui/attune/src/simulation_edit.ui
+-rw-r--r--   0        0        0      216 2023-07-12 14:00:56.471604 sfctools-1.1.0.3/sfctools/gui/attune/src/styles/bright/background.txt
+-rw-r--r--   0        0        0     4018 2023-07-12 14:00:56.471604 sfctools-1.1.0.3/sfctools/gui/attune/src/styles/bright/main.txt
+-rw-r--r--   0        0        0       62 2023-07-12 14:00:56.471604 sfctools-1.1.0.3/sfctools/gui/attune/src/styles/bright/tables.txt
+-rw-r--r--   0        0        0      727 2023-07-12 14:00:56.471604 sfctools-1.1.0.3/sfctools/gui/attune/src/styles/dark/background.txt
+-rw-r--r--   0        0        0     4228 2023-07-12 14:00:56.472604 sfctools-1.1.0.3/sfctools/gui/attune/src/styles/dark/main.txt
+-rw-r--r--   0        0        0       37 2023-07-12 14:00:56.472604 sfctools-1.1.0.3/sfctools/gui/attune/src/styles/dark/tables.txt
+-rw-r--r--   0        0        0     6968 2023-07-12 14:00:56.472604 sfctools-1.1.0.3/sfctools/gui/attune/src/theme_manager.py
+-rw-r--r--   0        0        0    85503 2023-07-12 14:00:56.473605 sfctools-1.1.0.3/sfctools/gui/attune/src/transaction_designer_mainwindow.ui
+-rw-r--r--   0        0        0    11727 2023-07-12 14:00:56.473605 sfctools-1.1.0.3/sfctools/gui/attune/src/yaml_editor.py
+-rw-r--r--   0        0        0      357 2023-07-12 14:00:56.473605 sfctools-1.1.0.3/sfctools/gui/attune_main.py
+-rw-r--r--   0        0        0      389 2023-07-12 14:00:56.473605 sfctools-1.1.0.3/sfctools/gui/attune_starter.py
+-rw-r--r--   0        0        0    27804 2023-07-12 14:00:56.464604 sfctools-1.1.0.3/sfctools/gui/CLA.pdf
+-rw-r--r--   0        0        0     1434 2023-07-12 14:00:56.464604 sfctools-1.1.0.3/sfctools/gui/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1157 2023-07-12 14:00:56.465604 sfctools-1.1.0.3/sfctools/gui/LICENSE
+-rw-r--r--   0        0        0      819 2023-07-12 14:00:56.465604 sfctools-1.1.0.3/sfctools/gui/README.md
+-rw-r--r--   0        0        0       47 2023-07-12 14:00:56.473605 sfctools-1.1.0.3/sfctools/gui/runner.py
+-rw-r--r--   0        0        0      275 2023-07-12 14:00:56.473605 sfctools-1.1.0.3/sfctools/gui/sfctheme
+-rw-r--r--   0        0        0        0 2023-07-12 14:00:56.474605 sfctools-1.1.0.3/sfctools/misc/__init__.py
+-rw-r--r--   0        0        0    21989 2023-07-12 14:00:56.474605 sfctools-1.1.0.3/sfctools/misc/mpl_plotting.py
+-rw-r--r--   0        0        0     7795 2023-07-12 14:00:56.474605 sfctools-1.1.0.3/sfctools/misc/reporting_sheet.py
+-rw-r--r--   0        0        0     7074 2023-07-12 14:00:56.474605 sfctools-1.1.0.3/sfctools/misc/timeseries.py
+-rw-r--r--   0        0        0     3511 1970-01-01 00:00:00.000000 sfctools-1.1.0.3/PKG-INFO
```

### Comparing `sfctools-1.1.0.2/LICENSE` & `sfctools-1.1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/pyproject.toml` & `sfctools-1.1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sfctools"
-version = "1.1.0.2"
+version = "1.1.0.3"
 description = "Framework for stock-flow consistent agent-based modeling, being developed at the German Aerospace Center (DLR) for and in the scientific context of energy systems analysis, however, it is widely applicable in other scientific fields."
 
 authors = ["Thomas Baldauf <thomas.baldauf@dlr.de>"]
 license = "MIT"
 maintainers = ["Thomas Baldauf, Benjamin Fuchs <thomas.baldauf@dlr.de, benjamin.fuchs@dlr.de>"]
 homepage = 'https://gitlab.com/dlr-ve/esy/sfctools/framework'
 documentation = 'https://sfctools-framework.readthedocs.io/en/latest/'
```

### Comparing `sfctools-1.1.0.2/README.md` & `sfctools-1.1.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # sfctools - A toolbox for stock-flow consistent, agent-based models
 
-Sfctools is a lightweight and easy-to-use Python framework for agent-based macroeconomic, stock-flow consistent (ABM-SFC) modeling. It concentrates on agents in economics and helps you to construct agents, helps you to manage and document your model parameters, assures stock-flow consistency, and facilitates basic economic data structures (such as the balance sheet).
-
+Sfctools is a lightweight and easy-to-use Python framework for agent-based macroeconomic, stock-flow consistent (ABM-SFC) modeling. It concentrates on agents in economics and helps you to construct agents, helps you to manage and document your model parameters, assures stock-flow consistency, and facilitates basic economic data structures (such as the balance sheet). For more documentation, see https://sfctools-framework.readthedocs.io/en/latest/.
 
 ## Installation
 
 We recommend to install sfctools in a fresh Python 3.8 environment. For example, with conda, do
 
     conda create --name sfcenv python=3.8
     conda activate sfcenv
```

### Comparing `sfctools-1.1.0.2/sfctools/__init__.py` & `sfctools-1.1.0.3/sfctools/__init__.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/__main__.py` & `sfctools-1.1.0.3/sfctools/__main__.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/automation/calibration.py` & `sfctools-1.1.0.3/sfctools/automation/calibration.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/automation/cgesolver.py` & `sfctools-1.1.0.3/sfctools/automation/cgesolver.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/automation/runner.py` & `sfctools-1.1.0.3/sfctools/automation/runner.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/bottomup/matching.py` & `sfctools-1.1.0.3/sfctools/bottomup/matching.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/bottomup/productiontree.py` & `sfctools-1.1.0.3/sfctools/bottomup/productiontree.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/bottomup/stock_manager.py` & `sfctools-1.1.0.3/sfctools/bottomup/stock_manager.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/bottomup/treestruct.py` & `sfctools-1.1.0.3/sfctools/bottomup/treestruct.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/core/agent.py` & `sfctools-1.1.0.3/sfctools/core/agent.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/core/clock.py` & `sfctools-1.1.0.3/sfctools/core/clock.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/core/flow_matrix.py` & `sfctools-1.1.0.3/sfctools/core/flow_matrix.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/core/settings.py` & `sfctools-1.1.0.3/sfctools/core/settings.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/core/singleton.py` & `sfctools-1.1.0.3/sfctools/core/singleton.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/core/world.py` & `sfctools-1.1.0.3/sfctools/core/world.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/datastructs/balance.py` & `sfctools-1.1.0.3/sfctools/datastructs/balance.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/datastructs/bank_order_book.py` & `sfctools-1.1.0.3/sfctools/datastructs/bank_order_book.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/datastructs/cash_flow_statement.py` & `sfctools-1.1.0.3/sfctools/datastructs/cash_flow_statement.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/datastructs/collection.py` & `sfctools-1.1.0.3/sfctools/datastructs/collection.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/datastructs/income_statement.py` & `sfctools-1.1.0.3/sfctools/datastructs/income_statement.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/datastructs/inventory.py` & `sfctools-1.1.0.3/sfctools/datastructs/inventory.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/datastructs/market_registry.py` & `sfctools-1.1.0.3/sfctools/datastructs/market_registry.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/datastructs/signalslot.py` & `sfctools-1.1.0.3/sfctools/datastructs/signalslot.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/datastructs/worker_registry.py` & `sfctools-1.1.0.3/sfctools/datastructs/worker_registry.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/examples/__init__.py` & `sfctools-1.1.0.3/sfctools/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/examples/balance.py` & `sfctools-1.1.0.3/sfctools/examples/balance.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/examples/basic_example/basic_example.py` & `sfctools-1.1.0.3/sfctools/examples/basic_example/basic_example.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/examples/clock.py` & `sfctools-1.1.0.3/sfctools/examples/clock.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/examples/example_wrapper.py` & `sfctools-1.1.0.3/sfctools/examples/example_wrapper.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/examples/exampleabm/agents/government.py` & `sfctools-1.1.0.3/sfctools/examples/exampleabm/agents/government.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/examples/exampleabm/agents/household.py` & `sfctools-1.1.0.3/sfctools/examples/exampleabm/agents/household.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/examples/exampleabm/agents/production.py` & `sfctools-1.1.0.3/sfctools/examples/exampleabm/agents/production.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/examples/exampleabm/agents/transactions.py` & `sfctools-1.1.0.3/sfctools/examples/exampleabm/agents/transactions.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/examples/exampleabm/data/preprocess.py` & `sfctools-1.1.0.3/sfctools/examples/exampleabm/data/preprocess.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/examples/exampleabm/data/processed/tipsau20_gdp_processed.txt` & `sfctools-1.1.0.3/sfctools/examples/exampleabm/data/processed/tipsau20_gdp_processed.txt`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/examples/exampleabm/data/raw/tipsau20_gdp.csv` & `sfctools-1.1.0.3/sfctools/examples/exampleabm/data/raw/tipsau20_gdp.csv`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/examples/exampleabm/figures/matrix.png` & `sfctools-1.1.0.3/sfctools/examples/exampleabm/figures/matrix.png`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/examples/exampleabm/figures/outputs.png` & `sfctools-1.1.0.3/sfctools/examples/exampleabm/figures/outputs.png`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/examples/exampleabm/figures/sankey.png` & `sfctools-1.1.0.3/sfctools/examples/exampleabm/figures/sankey.png`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/examples/exampleabm/info.md` & `sfctools-1.1.0.3/sfctools/examples/exampleabm/info.md`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/examples/exampleabm/model.py` & `sfctools-1.1.0.3/sfctools/examples/exampleabm/model.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/examples/exampleabm/settings.yml` & `sfctools-1.1.0.3/sfctools/examples/exampleabm/settings.yml`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/examples/flowmatrix.py` & `sfctools-1.1.0.3/sfctools/examples/flowmatrix.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/examples/hello_agent.py` & `sfctools-1.1.0.3/sfctools/examples/hello_agent.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/examples/inventory.py` & `sfctools-1.1.0.3/sfctools/examples/inventory.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/examples/market_example/market.py` & `sfctools-1.1.0.3/sfctools/examples/market_example/market.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/examples/market_example/market2.py` & `sfctools-1.1.0.3/sfctools/examples/market_example/market2.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/examples/monte_carlo/monte_carlo.py` & `sfctools-1.1.0.3/sfctools/examples/monte_carlo/monte_carlo.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/examples/order_book.py` & `sfctools-1.1.0.3/sfctools/examples/order_book.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/examples/readme_example.py` & `sfctools-1.1.0.3/sfctools/examples/readme_example.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/examples/signal_slot.py` & `sfctools-1.1.0.3/sfctools/examples/signal_slot.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/examples/worker_registry.py` & `sfctools-1.1.0.3/sfctools/examples/worker_registry.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/gui/.gitlab-ci.yml` & `sfctools-1.1.0.3/sfctools/gui/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/gui/attune/src/agent_editor.py` & `sfctools-1.1.0.3/sfctools/gui/attune/src/agent_editor.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/gui/attune/src/code_editor.ui` & `sfctools-1.1.0.3/sfctools/gui/attune/src/code_editor.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/gui/attune/src/draw_widget.py` & `sfctools-1.1.0.3/sfctools/gui/attune/src/draw_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -1366,28 +1366,28 @@
 
         x_vals = [move_x +int(distance/2)+x-2-10 for x in x_vals]
         y_vals = [move_y +int(distance/2)+y-2-10 for y in y_vals]
 
         # transform all points
 
         for i in range(len(x_vals)-2):
-            x = x_vals[i]
-            y = y_vals[i]
+            x = int(x_vals[i])
+            y = int(y_vals[i])
             if self.boxes[i].ishelper:
                     qp.drawRect(x,y,1,1)
             else:
                 #if self.boxes[i] == self.highlighted:
                 #    pen = QtGui.QPen(self.parent().theme_manager.get_color(3),1)
                 #    brush = QtGui.QBrush(self.parent().theme_manager.get_color(3))
                 #    qp.setPen(pen)
 
                 #    qp.fillRect(QtCore.QRectF(x,y,4,4),brush)
                 #else:
                 qp.drawRect(x,y,4,4)
-
+        
         # skip origin ...
         x = x_vals[-1]
         y = y_vals[-1]
         pen = QtGui.QPen(self.main_widget.theme_manager.get_color(4),1)
         qp.setPen(pen)
         ox = x
         oy =  y
```

### Comparing `sfctools-1.1.0.2/sfctools/gui/attune/src/income_viewer.ui` & `sfctools-1.1.0.3/sfctools/gui/attune/src/income_viewer.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/gui/attune/src/mainloop_editor.py` & `sfctools-1.1.0.3/sfctools/gui/attune/src/mainloop_editor.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/gui/attune/src/mamba_interpreter2.py` & `sfctools-1.1.0.3/sfctools/gui/attune/src/mamba_interpreter2.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/gui/attune/src/matrix_viewer.ui` & `sfctools-1.1.0.3/sfctools/gui/attune/src/matrix_viewer.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/gui/attune/src/my_interpolation.py` & `sfctools-1.1.0.3/sfctools/gui/attune/src/my_interpolation.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/gui/attune/src/output_display.py` & `sfctools-1.1.0.3/sfctools/gui/attune/src/output_display.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/gui/attune/src/output_display.ui` & `sfctools-1.1.0.3/sfctools/gui/attune/src/output_display.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/gui/attune/src/pandasmodel.py` & `sfctools-1.1.0.3/sfctools/gui/attune/src/pandasmodel.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/gui/attune/src/qtattune.py` & `sfctools-1.1.0.3/sfctools/gui/attune/src/qtattune.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/gui/attune/src/resources.py` & `sfctools-1.1.0.3/sfctools/gui/attune/src/resources.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/gui/attune/src/search_dialog.ui` & `sfctools-1.1.0.3/sfctools/gui/attune/src/search_dialog.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/gui/attune/src/settings_edit.ui` & `sfctools-1.1.0.3/sfctools/gui/attune/src/settings_edit.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/gui/attune/src/simulation_edit.ui` & `sfctools-1.1.0.3/sfctools/gui/attune/src/simulation_edit.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/gui/attune/src/styles/bright/main.txt` & `sfctools-1.1.0.3/sfctools/gui/attune/src/styles/bright/main.txt`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/gui/attune/src/styles/dark/background.txt` & `sfctools-1.1.0.3/sfctools/gui/attune/src/styles/dark/background.txt`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/gui/attune/src/styles/dark/main.txt` & `sfctools-1.1.0.3/sfctools/gui/attune/src/styles/dark/main.txt`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/gui/attune/src/theme_manager.py` & `sfctools-1.1.0.3/sfctools/gui/attune/src/theme_manager.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/gui/attune/src/transaction_designer_mainwindow.ui` & `sfctools-1.1.0.3/sfctools/gui/attune/src/transaction_designer_mainwindow.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/gui/attune/src/yaml_editor.py` & `sfctools-1.1.0.3/sfctools/gui/attune/src/yaml_editor.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/gui/CLA.pdf` & `sfctools-1.1.0.3/sfctools/gui/CLA.pdf`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/gui/CONTRIBUTING.md` & `sfctools-1.1.0.3/sfctools/gui/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/gui/LICENSE` & `sfctools-1.1.0.3/sfctools/gui/LICENSE`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/gui/README.md` & `sfctools-1.1.0.3/sfctools/gui/README.md`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/misc/mpl_plotting.py` & `sfctools-1.1.0.3/sfctools/misc/mpl_plotting.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/misc/reporting_sheet.py` & `sfctools-1.1.0.3/sfctools/misc/reporting_sheet.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/sfctools/misc/timeseries.py` & `sfctools-1.1.0.3/sfctools/misc/timeseries.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.1.0.2/PKG-INFO` & `sfctools-1.1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sfctools
-Version: 1.1.0.2
+Version: 1.1.0.3
 Summary: Framework for stock-flow consistent agent-based modeling, being developed at the German Aerospace Center (DLR) for and in the scientific context of energy systems analysis, however, it is widely applicable in other scientific fields.
 Home-page: https://gitlab.com/dlr-ve/esy/sfctools/framework
 License: MIT
 Keywords: stock-flow-consistent,agent-based,agent,macroeconomics,computational economics
 Author: Thomas Baldauf
 Author-email: thomas.baldauf@dlr.de
 Maintainer: Thomas Baldauf, Benjamin Fuchs
@@ -35,16 +35,15 @@
 Requires-Dist: setuptools (>=50.0.0)
 Requires-Dist: sympy (>=1.10.0)
 Project-URL: Documentation, https://sfctools-framework.readthedocs.io/en/latest/
 Description-Content-Type: text/markdown
 
 # sfctools - A toolbox for stock-flow consistent, agent-based models
 
-Sfctools is a lightweight and easy-to-use Python framework for agent-based macroeconomic, stock-flow consistent (ABM-SFC) modeling. It concentrates on agents in economics and helps you to construct agents, helps you to manage and document your model parameters, assures stock-flow consistency, and facilitates basic economic data structures (such as the balance sheet).
-
+Sfctools is a lightweight and easy-to-use Python framework for agent-based macroeconomic, stock-flow consistent (ABM-SFC) modeling. It concentrates on agents in economics and helps you to construct agents, helps you to manage and document your model parameters, assures stock-flow consistency, and facilitates basic economic data structures (such as the balance sheet). For more documentation, see https://sfctools-framework.readthedocs.io/en/latest/.
 
 ## Installation
 
 We recommend to install sfctools in a fresh Python 3.8 environment. For example, with conda, do
 
     conda create --name sfcenv python=3.8
     conda activate sfcenv
```

