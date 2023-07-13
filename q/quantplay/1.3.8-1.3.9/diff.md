# Comparing `tmp/quantplay-1.3.8.tar.gz` & `tmp/quantplay-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantplay-1.3.8.tar", last modified: Sun Jul  9 13:53:15 2023, max compression
+gzip compressed data, was "quantplay-1.3.9.tar", last modified: Mon Jul 10 05:04:45 2023, max compression
```

## Comparing `quantplay-1.3.8.tar` & `quantplay-1.3.9.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-09 13:53:15.320752 quantplay-1.3.8/
--rw-r--r--   0 ashok      (502) staff       (20)      662 2023-07-09 13:53:15.320817 quantplay-1.3.8/PKG-INFO
--rw-r--r--   0 ashok      (502) staff       (20)      494 2023-04-19 06:36:45.000000 quantplay-1.3.8/README.md
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-09 13:53:15.302414 quantplay-1.3.8/quantplay/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-09 13:53:15.303457 quantplay-1.3.8/quantplay/backtest/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/backtest/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    17605 2023-05-17 07:17:28.000000 quantplay-1.3.8/quantplay/backtest/backtest_trades.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-09 13:53:15.306512 quantplay-1.3.8/quantplay/broker/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/broker/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    10902 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/broker/angelone.py
--rw-r--r--   0 ashok      (502) staff       (20)     3738 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/broker/broker_client.py
--rw-r--r--   0 ashok      (502) staff       (20)       87 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/broker/client.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-09 13:53:15.306805 quantplay-1.3.8/quantplay/broker/finvasia_utils/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/broker/finvasia_utils/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     2576 2023-05-11 13:49:53.000000 quantplay-1.3.8/quantplay/broker/finvasia_utils/shoonya.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-09 13:53:15.307215 quantplay-1.3.8/quantplay/broker/generics/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/broker/generics/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    28852 2023-07-07 06:10:11.000000 quantplay-1.3.8/quantplay/broker/generics/broker.py
--rw-r--r--   0 ashok      (502) staff       (20)     3897 2023-05-17 07:17:28.000000 quantplay-1.3.8/quantplay/broker/iifl.py
--rw-r--r--   0 ashok      (502) staff       (20)      588 2023-06-01 01:35:25.000000 quantplay-1.3.8/quantplay/broker/iifl_xts.py
--rw-r--r--   0 ashok      (502) staff       (20)     2002 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/broker/kite_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)    28517 2023-07-09 13:42:22.000000 quantplay-1.3.8/quantplay/broker/motilal.py
--rw-r--r--   0 ashok      (502) staff       (20)    19618 2023-05-11 13:57:44.000000 quantplay-1.3.8/quantplay/broker/shoonya.py
--rw-r--r--   0 ashok      (502) staff       (20)      515 2023-04-19 06:37:00.000000 quantplay-1.3.8/quantplay/broker/symphony.py
--rw-r--r--   0 ashok      (502) staff       (20)    19145 2023-06-09 05:00:32.000000 quantplay-1.3.8/quantplay/broker/xts.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-09 13:53:15.309218 quantplay-1.3.8/quantplay/broker/xts_utils/
--rw-r--r--   0 ashok      (502) staff       (20)    33446 2023-04-24 08:10:10.000000 quantplay-1.3.8/quantplay/broker/xts_utils/Connect.py
--rw-r--r--   0 ashok      (502) staff       (20)     3046 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/broker/xts_utils/Exception.py
--rw-r--r--   0 ashok      (502) staff       (20)     6456 2023-06-02 03:04:08.000000 quantplay-1.3.8/quantplay/broker/xts_utils/InteractiveSocketClient.py
--rw-r--r--   0 ashok      (502) staff       (20)     9106 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/broker/xts_utils/MarketDataSocketClient.py
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/broker/xts_utils/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    17159 2023-07-09 13:52:57.000000 quantplay-1.3.8/quantplay/broker/zerodha.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-09 13:53:15.309361 quantplay-1.3.8/quantplay/brokerage/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/brokerage/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-09 13:53:15.309639 quantplay-1.3.8/quantplay/brokerage/angelone/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/brokerage/angelone/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    10989 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/brokerage/angelone/angel_broker.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-09 13:53:15.310088 quantplay-1.3.8/quantplay/brokerage/generics/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/brokerage/generics/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    28260 2023-07-06 16:08:51.000000 quantplay-1.3.8/quantplay/brokerage/generics/broker.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-09 13:53:15.310901 quantplay-1.3.8/quantplay/brokerage/zerodha/
--rw-r--r--   0 ashok      (502) staff       (20)    17690 2023-04-24 06:31:05.000000 quantplay-1.3.8/quantplay/brokerage/zerodha/ZBroker.py
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/brokerage/zerodha/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-09 13:53:15.311152 quantplay-1.3.8/quantplay/config/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/config/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     1461 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/config/qplay_config.py
--rw-r--r--   0 ashok      (502) staff       (20)     1127 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/create_sample_data.py
--rw-r--r--   0 ashok      (502) staff       (20)     1725 2023-04-19 06:37:00.000000 quantplay-1.3.8/quantplay/data_modify_script.py
--rw-r--r--   0 ashok      (502) staff       (20)     3481 2023-06-23 06:49:50.000000 quantplay-1.3.8/quantplay/date_fix.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-09 13:53:15.311449 quantplay-1.3.8/quantplay/exception/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/exception/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     2162 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/exception/exceptions.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-09 13:53:15.311829 quantplay-1.3.8/quantplay/executor/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/executor/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     6064 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/executor/strategy_executor.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-09 13:53:15.312450 quantplay-1.3.8/quantplay/indicators/
--rw-r--r--   0 ashok      (502) staff       (20)     1747 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/indicators/Indicator.py
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/indicators/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      455 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/indicators/atr.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-09 13:53:15.312607 quantplay-1.3.8/quantplay/model/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/model/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-09 13:53:15.313284 quantplay-1.3.8/quantplay/model/exchange/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/model/exchange/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     1472 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/model/exchange/instrument.py
--rw-r--r--   0 ashok      (502) staff       (20)     8794 2023-05-17 08:03:33.000000 quantplay-1.3.8/quantplay/model/exchange/order.py
--rw-r--r--   0 ashok      (502) staff       (20)     3238 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/model/exchange/tick.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-09 13:53:15.313581 quantplay-1.3.8/quantplay/model/strategy/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/model/strategy/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      206 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/model/strategy/strategy_response.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-09 13:53:15.313766 quantplay-1.3.8/quantplay/oms/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/oms/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-09 13:53:15.314225 quantplay-1.3.8/quantplay/order_execution/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/order_execution/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     2048 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/order_execution/execution_algorithm.py
--rw-r--r--   0 ashok      (502) staff       (20)     1281 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/order_execution/mean_price.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-09 13:53:15.314789 quantplay-1.3.8/quantplay/reporting/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/reporting/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    10801 2023-06-23 06:49:43.000000 quantplay-1.3.8/quantplay/reporting/strategy_report.py
--rw-r--r--   0 ashok      (502) staff       (20)     1521 2023-04-19 06:37:00.000000 quantplay-1.3.8/quantplay/reporting/visuals.py
--rw-r--r--   0 ashok      (502) staff       (20)      231 2023-04-24 06:31:05.000000 quantplay-1.3.8/quantplay/service.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-09 13:53:15.315531 quantplay-1.3.8/quantplay/services/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/services/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    18366 2023-05-26 07:55:13.000000 quantplay-1.3.8/quantplay/services/market.py
--rw-r--r--   0 ashok      (502) staff       (20)    11648 2023-06-23 06:49:43.000000 quantplay-1.3.8/quantplay/services/tradelens.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-09 13:53:15.315798 quantplay-1.3.8/quantplay/strategies/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:35:41.000000 quantplay-1.3.8/quantplay/strategies/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-09 13:53:15.315911 quantplay-1.3.8/quantplay/strategies/equities/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:48:09.000000 quantplay-1.3.8/quantplay/strategies/equities/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-09 13:53:15.316023 quantplay-1.3.8/quantplay/strategies/equities/intraday/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:48:26.000000 quantplay-1.3.8/quantplay/strategies/equities/intraday/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-09 13:53:15.316137 quantplay-1.3.8/quantplay/strategies/equities/overnight/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:49:47.000000 quantplay-1.3.8/quantplay/strategies/equities/overnight/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-09 13:53:15.316250 quantplay-1.3.8/quantplay/strategies/futures/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-24 08:54:42.000000 quantplay-1.3.8/quantplay/strategies/futures/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-09 13:53:15.316369 quantplay-1.3.8/quantplay/strategies/futures/overnight/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-24 08:54:48.000000 quantplay-1.3.8/quantplay/strategies/futures/overnight/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-09 13:53:15.316491 quantplay-1.3.8/quantplay/strategies/options/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:35:52.000000 quantplay-1.3.8/quantplay/strategies/options/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-09 13:53:15.317265 quantplay-1.3.8/quantplay/strategies/options/intraday/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:36:03.000000 quantplay-1.3.8/quantplay/strategies/options/intraday/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     1958 2022-09-14 18:05:01.000000 quantplay-1.3.8/quantplay/strategies/options/intraday/ladder.py
--rw-r--r--   0 ashok      (502) staff       (20)     2675 2022-06-25 11:41:44.000000 quantplay-1.3.8/quantplay/strategies/options/intraday/musk.py
--rw-r--r--   0 ashok      (502) staff       (20)      403 2022-09-17 07:36:48.000000 quantplay-1.3.8/quantplay/strategies/options/intraday/short_straddle.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-09 13:53:15.317587 quantplay-1.3.8/quantplay/strategy/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/strategy/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    12759 2023-05-17 07:17:28.000000 quantplay-1.3.8/quantplay/strategy/base.py
--rw-r--r--   0 ashok      (502) staff       (20)      214 2022-06-28 09:52:29.000000 quantplay-1.3.8/quantplay/strategy_run.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-09 13:53:15.319297 quantplay-1.3.8/quantplay/utils/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/utils/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      723 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/utils/config_util.py
--rw-r--r--   0 ashok      (502) staff       (20)    24181 2023-04-24 06:31:05.000000 quantplay-1.3.8/quantplay/utils/constant.py
--rw-r--r--   0 ashok      (502) staff       (20)     5433 2023-04-19 06:37:00.000000 quantplay-1.3.8/quantplay/utils/data_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)      711 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/utils/exchange.py
--rw-r--r--   0 ashok      (502) staff       (20)      517 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/utils/number_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)      458 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/utils/pickle_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)     1181 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/utils/selenium_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)     4094 2023-04-19 06:36:45.000000 quantplay-1.3.8/quantplay/utils/transaction_utils.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-09 13:53:15.303216 quantplay-1.3.8/quantplay.egg-info/
--rw-r--r--   0 ashok      (502) staff       (20)      662 2023-07-09 13:53:15.000000 quantplay-1.3.8/quantplay.egg-info/PKG-INFO
--rw-r--r--   0 ashok      (502) staff       (20)     3391 2023-07-09 13:53:15.000000 quantplay-1.3.8/quantplay.egg-info/SOURCES.txt
--rw-r--r--   0 ashok      (502) staff       (20)        1 2023-07-09 13:53:15.000000 quantplay-1.3.8/quantplay.egg-info/dependency_links.txt
--rw-r--r--   0 ashok      (502) staff       (20)      221 2023-07-09 13:53:15.000000 quantplay-1.3.8/quantplay.egg-info/requires.txt
--rw-r--r--   0 ashok      (502) staff       (20)       15 2023-07-09 13:53:15.000000 quantplay-1.3.8/quantplay.egg-info/top_level.txt
--rw-r--r--   0 ashok      (502) staff       (20)       49 2023-07-09 13:53:15.321049 quantplay-1.3.8/setup.cfg
--rw-r--r--   0 ashok      (502) staff       (20)      875 2023-07-09 13:53:11.000000 quantplay-1.3.8/setup.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-09 13:53:15.319583 quantplay-1.3.8/test/
--rw-------   0 ashok      (502) staff       (20)        0 2022-04-15 16:22:35.000000 quantplay-1.3.8/test/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-09 13:53:15.319860 quantplay-1.3.8/test/broker/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.8/test/broker/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      220 2023-04-19 06:36:45.000000 quantplay-1.3.8/test/broker/finvasia.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-09 13:53:15.320140 quantplay-1.3.8/test/executor/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.8/test/executor/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      304 2023-04-19 06:36:45.000000 quantplay-1.3.8/test/executor/strategy_executor.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-09 13:53:15.320591 quantplay-1.3.8/test/strategy/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.8/test/strategy/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      292 2023-04-19 06:36:45.000000 quantplay-1.3.8/test/strategy/base.py
--rw-r--r--   0 ashok      (502) staff       (20)     2194 2023-04-19 06:36:45.000000 quantplay-1.3.8/test/strategy/sample_strategy.py
--rw-r--r--   0 ashok      (502) staff       (20)     3302 2023-04-19 06:36:45.000000 quantplay-1.3.8/test/test_motilal.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-10 05:04:45.395949 quantplay-1.3.9/
+-rw-r--r--   0 ashok      (502) staff       (20)      662 2023-07-10 05:04:45.396017 quantplay-1.3.9/PKG-INFO
+-rw-r--r--   0 ashok      (502) staff       (20)      494 2023-04-19 06:36:45.000000 quantplay-1.3.9/README.md
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-10 05:04:45.378778 quantplay-1.3.9/quantplay/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-10 05:04:45.379747 quantplay-1.3.9/quantplay/backtest/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/backtest/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    17605 2023-05-17 07:17:28.000000 quantplay-1.3.9/quantplay/backtest/backtest_trades.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-10 05:04:45.383286 quantplay-1.3.9/quantplay/broker/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/broker/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    10902 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/broker/angelone.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3738 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/broker/broker_client.py
+-rw-r--r--   0 ashok      (502) staff       (20)       87 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/broker/client.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-10 05:04:45.383925 quantplay-1.3.9/quantplay/broker/finvasia_utils/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/broker/finvasia_utils/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2576 2023-05-11 13:49:53.000000 quantplay-1.3.9/quantplay/broker/finvasia_utils/shoonya.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-10 05:04:45.384276 quantplay-1.3.9/quantplay/broker/generics/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/broker/generics/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    28869 2023-07-10 04:35:08.000000 quantplay-1.3.9/quantplay/broker/generics/broker.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3897 2023-05-17 07:17:28.000000 quantplay-1.3.9/quantplay/broker/iifl.py
+-rw-r--r--   0 ashok      (502) staff       (20)      588 2023-06-01 01:35:25.000000 quantplay-1.3.9/quantplay/broker/iifl_xts.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2002 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/broker/kite_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)    29057 2023-07-10 05:04:27.000000 quantplay-1.3.9/quantplay/broker/motilal.py
+-rw-r--r--   0 ashok      (502) staff       (20)    19773 2023-07-10 04:53:00.000000 quantplay-1.3.9/quantplay/broker/shoonya.py
+-rw-r--r--   0 ashok      (502) staff       (20)      515 2023-04-19 06:37:00.000000 quantplay-1.3.9/quantplay/broker/symphony.py
+-rw-r--r--   0 ashok      (502) staff       (20)    19145 2023-06-09 05:00:32.000000 quantplay-1.3.9/quantplay/broker/xts.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-10 05:04:45.386256 quantplay-1.3.9/quantplay/broker/xts_utils/
+-rw-r--r--   0 ashok      (502) staff       (20)    33446 2023-04-24 08:10:10.000000 quantplay-1.3.9/quantplay/broker/xts_utils/Connect.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3046 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/broker/xts_utils/Exception.py
+-rw-r--r--   0 ashok      (502) staff       (20)     6456 2023-06-02 03:04:08.000000 quantplay-1.3.9/quantplay/broker/xts_utils/InteractiveSocketClient.py
+-rw-r--r--   0 ashok      (502) staff       (20)     9106 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/broker/xts_utils/MarketDataSocketClient.py
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/broker/xts_utils/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    17159 2023-07-09 13:52:57.000000 quantplay-1.3.9/quantplay/broker/zerodha.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-10 05:04:45.386384 quantplay-1.3.9/quantplay/brokerage/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/brokerage/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-10 05:04:45.386619 quantplay-1.3.9/quantplay/brokerage/angelone/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/brokerage/angelone/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    10989 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/brokerage/angelone/angel_broker.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-10 05:04:45.387069 quantplay-1.3.9/quantplay/brokerage/generics/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/brokerage/generics/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    28260 2023-07-06 16:08:51.000000 quantplay-1.3.9/quantplay/brokerage/generics/broker.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-10 05:04:45.387910 quantplay-1.3.9/quantplay/brokerage/zerodha/
+-rw-r--r--   0 ashok      (502) staff       (20)    17690 2023-04-24 06:31:05.000000 quantplay-1.3.9/quantplay/brokerage/zerodha/ZBroker.py
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/brokerage/zerodha/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-10 05:04:45.388097 quantplay-1.3.9/quantplay/config/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/config/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1461 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/config/qplay_config.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1127 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/create_sample_data.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1725 2023-04-19 06:37:00.000000 quantplay-1.3.9/quantplay/data_modify_script.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3481 2023-06-23 06:49:50.000000 quantplay-1.3.9/quantplay/date_fix.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-10 05:04:45.388321 quantplay-1.3.9/quantplay/exception/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/exception/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2162 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/exception/exceptions.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-10 05:04:45.388644 quantplay-1.3.9/quantplay/executor/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/executor/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     6064 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/executor/strategy_executor.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-10 05:04:45.389186 quantplay-1.3.9/quantplay/indicators/
+-rw-r--r--   0 ashok      (502) staff       (20)     1747 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/indicators/Indicator.py
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/indicators/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      455 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/indicators/atr.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-10 05:04:45.389314 quantplay-1.3.9/quantplay/model/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/model/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-10 05:04:45.389864 quantplay-1.3.9/quantplay/model/exchange/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/model/exchange/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1472 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/model/exchange/instrument.py
+-rw-r--r--   0 ashok      (502) staff       (20)     8794 2023-05-17 08:03:33.000000 quantplay-1.3.9/quantplay/model/exchange/order.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3238 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/model/exchange/tick.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-10 05:04:45.390090 quantplay-1.3.9/quantplay/model/strategy/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/model/strategy/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      206 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/model/strategy/strategy_response.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-10 05:04:45.390220 quantplay-1.3.9/quantplay/oms/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/oms/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-10 05:04:45.390526 quantplay-1.3.9/quantplay/order_execution/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/order_execution/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2048 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/order_execution/execution_algorithm.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1281 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/order_execution/mean_price.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-10 05:04:45.391104 quantplay-1.3.9/quantplay/reporting/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/reporting/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    10801 2023-06-23 06:49:43.000000 quantplay-1.3.9/quantplay/reporting/strategy_report.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1521 2023-04-19 06:37:00.000000 quantplay-1.3.9/quantplay/reporting/visuals.py
+-rw-r--r--   0 ashok      (502) staff       (20)      231 2023-04-24 06:31:05.000000 quantplay-1.3.9/quantplay/service.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-10 05:04:45.391725 quantplay-1.3.9/quantplay/services/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/services/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    18366 2023-05-26 07:55:13.000000 quantplay-1.3.9/quantplay/services/market.py
+-rw-r--r--   0 ashok      (502) staff       (20)    11648 2023-06-23 06:49:43.000000 quantplay-1.3.9/quantplay/services/tradelens.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-10 05:04:45.391957 quantplay-1.3.9/quantplay/strategies/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:35:41.000000 quantplay-1.3.9/quantplay/strategies/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-10 05:04:45.392047 quantplay-1.3.9/quantplay/strategies/equities/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:48:09.000000 quantplay-1.3.9/quantplay/strategies/equities/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-10 05:04:45.392142 quantplay-1.3.9/quantplay/strategies/equities/intraday/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:48:26.000000 quantplay-1.3.9/quantplay/strategies/equities/intraday/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-10 05:04:45.392240 quantplay-1.3.9/quantplay/strategies/equities/overnight/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:49:47.000000 quantplay-1.3.9/quantplay/strategies/equities/overnight/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-10 05:04:45.392340 quantplay-1.3.9/quantplay/strategies/futures/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-24 08:54:42.000000 quantplay-1.3.9/quantplay/strategies/futures/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-10 05:04:45.392433 quantplay-1.3.9/quantplay/strategies/futures/overnight/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-24 08:54:48.000000 quantplay-1.3.9/quantplay/strategies/futures/overnight/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-10 05:04:45.392521 quantplay-1.3.9/quantplay/strategies/options/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:35:52.000000 quantplay-1.3.9/quantplay/strategies/options/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-10 05:04:45.393188 quantplay-1.3.9/quantplay/strategies/options/intraday/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:36:03.000000 quantplay-1.3.9/quantplay/strategies/options/intraday/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1958 2022-09-14 18:05:01.000000 quantplay-1.3.9/quantplay/strategies/options/intraday/ladder.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2675 2022-06-25 11:41:44.000000 quantplay-1.3.9/quantplay/strategies/options/intraday/musk.py
+-rw-r--r--   0 ashok      (502) staff       (20)      403 2022-09-17 07:36:48.000000 quantplay-1.3.9/quantplay/strategies/options/intraday/short_straddle.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-10 05:04:45.393479 quantplay-1.3.9/quantplay/strategy/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/strategy/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    12759 2023-05-17 07:17:28.000000 quantplay-1.3.9/quantplay/strategy/base.py
+-rw-r--r--   0 ashok      (502) staff       (20)      214 2022-06-28 09:52:29.000000 quantplay-1.3.9/quantplay/strategy_run.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-10 05:04:45.394833 quantplay-1.3.9/quantplay/utils/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/utils/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      723 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/utils/config_util.py
+-rw-r--r--   0 ashok      (502) staff       (20)    24181 2023-04-24 06:31:05.000000 quantplay-1.3.9/quantplay/utils/constant.py
+-rw-r--r--   0 ashok      (502) staff       (20)     5433 2023-04-19 06:37:00.000000 quantplay-1.3.9/quantplay/utils/data_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)      711 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/utils/exchange.py
+-rw-r--r--   0 ashok      (502) staff       (20)      517 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/utils/number_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)      458 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/utils/pickle_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1181 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/utils/selenium_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)     4094 2023-04-19 06:36:45.000000 quantplay-1.3.9/quantplay/utils/transaction_utils.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-10 05:04:45.379545 quantplay-1.3.9/quantplay.egg-info/
+-rw-r--r--   0 ashok      (502) staff       (20)      662 2023-07-10 05:04:45.000000 quantplay-1.3.9/quantplay.egg-info/PKG-INFO
+-rw-r--r--   0 ashok      (502) staff       (20)     3391 2023-07-10 05:04:45.000000 quantplay-1.3.9/quantplay.egg-info/SOURCES.txt
+-rw-r--r--   0 ashok      (502) staff       (20)        1 2023-07-10 05:04:45.000000 quantplay-1.3.9/quantplay.egg-info/dependency_links.txt
+-rw-r--r--   0 ashok      (502) staff       (20)      221 2023-07-10 05:04:45.000000 quantplay-1.3.9/quantplay.egg-info/requires.txt
+-rw-r--r--   0 ashok      (502) staff       (20)       15 2023-07-10 05:04:45.000000 quantplay-1.3.9/quantplay.egg-info/top_level.txt
+-rw-r--r--   0 ashok      (502) staff       (20)       49 2023-07-10 05:04:45.396312 quantplay-1.3.9/setup.cfg
+-rw-r--r--   0 ashok      (502) staff       (20)      875 2023-07-10 05:04:41.000000 quantplay-1.3.9/setup.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-10 05:04:45.395045 quantplay-1.3.9/test/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-04-15 16:22:35.000000 quantplay-1.3.9/test/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-10 05:04:45.395261 quantplay-1.3.9/test/broker/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.9/test/broker/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      220 2023-04-19 06:36:45.000000 quantplay-1.3.9/test/broker/finvasia.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-10 05:04:45.395468 quantplay-1.3.9/test/executor/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.9/test/executor/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      304 2023-04-19 06:36:45.000000 quantplay-1.3.9/test/executor/strategy_executor.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-10 05:04:45.395826 quantplay-1.3.9/test/strategy/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.9/test/strategy/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      292 2023-04-19 06:36:45.000000 quantplay-1.3.9/test/strategy/base.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2194 2023-04-19 06:36:45.000000 quantplay-1.3.9/test/strategy/sample_strategy.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3302 2023-04-19 06:36:45.000000 quantplay-1.3.9/test/test_motilal.py
```

### Comparing `quantplay-1.3.8/PKG-INFO` & `quantplay-1.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantplay
-Version: 1.3.8
+Version: 1.3.9
 Summary: This python package will be stored in AWS CodeArtifact
 Home-page: 
 Author: 
 Author-email: 
 License: MIT
 
 # Quantplay Alpha playground
```

### Comparing `quantplay-1.3.8/quantplay/backtest/backtest_trades.py` & `quantplay-1.3.9/quantplay/backtest/backtest_trades.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/quantplay/broker/angelone.py` & `quantplay-1.3.9/quantplay/broker/angelone.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/quantplay/broker/broker_client.py` & `quantplay-1.3.9/quantplay/broker/broker_client.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/quantplay/broker/finvasia_utils/shoonya.py` & `quantplay-1.3.9/quantplay/broker/finvasia_utils/shoonya.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/quantplay/broker/generics/broker.py` & `quantplay-1.3.9/quantplay/broker/generics/broker.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         self.instrument_id_to_security_type_map = dict()
         self.exchange_symbol_to_instrument_id_map = defaultdict(dict)
         self.order_type_sl = "SL"
         self.nfo_exchange = "NFO"
 
         self.orders_column_list = ['order_id', 'user_id', 'tradingsymbol', 'tag', 'average_price', 'transaction_type',
                                    'status', 'ltp', 'exchange', 'product', 'quantity', 'filled_quantity',
-                                   'pending_quantity', 'order_timestamp']
+                                   'pending_quantity', 'order_timestamp', 'trigger_price']
         self.positions_column_list = ['tradingsymbol', 'quantity', 'ltp', 'pnl', 'buy_quantity',
                                       'sell_quantity', 'exchange', 'product', 'option_type']
         self.trigger_pending_status = "TRIGGER PENDING"
         self.lock = Lock()
 
     def initialize_symbol_data(self, save_as=None):
         instruments = self.instrument_data
```

### Comparing `quantplay-1.3.8/quantplay/broker/iifl.py` & `quantplay-1.3.9/quantplay/broker/iifl.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/quantplay/broker/iifl_xts.py` & `quantplay-1.3.9/quantplay/broker/iifl_xts.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/quantplay/broker/kite_utils.py` & `quantplay-1.3.9/quantplay/broker/kite_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/quantplay/broker/motilal.py` & `quantplay-1.3.9/quantplay/broker/motilal.py`

 * *Files 2% similar despite different names*

```diff
@@ -671,21 +671,29 @@
                 "LTP": 'ltp',
                 'buyorsell': 'transaction_type',
                 "averageprice": "average_price",
                 "orderid" : "order_id",
                 "orderstatus" : "status",
                 "entrydatetime" : "order_timestamp",
                 "orderqty" : "quantity",
+                "triggerprice" : "trigger_price",
                 "totalqtytraded" : "filled_quantity",
                 "totalqtyremaining" : "pending_quantity"
             }, inplace=True)
         orders.loc[:, 'product'] = orders.ordercategory
 
         orders = orders[self.orders_column_list]
         orders.loc[:, 'pnl'] = orders.ltp * orders.filled_quantity - orders.average_price * orders.filled_quantity
         orders.loc[:, 'pnl'] = np.where(orders.transaction_type == "SELL", -orders.pnl, orders.pnl)
 
+        orders.loc[:, 'status'] = np.where(((orders.status == "Confirm") & (orders.trigger_price > 0)),
+                                           "TRIGGER PENDING", orders.status)
+        orders.loc[:, 'status'] = np.where(((orders.status == "Confirm") & (orders.trigger_price == 0)),
+                                           "OPEN", orders.status)
         if tag:
             orders = orders[orders.tag == tag]
 
+        orders.status = orders.status.replace(
+            ["Traded", "Error", "Cancel"], ["COMPLETE", "REJECTED", "CANCELLED"]
+        )
         return orders
```

### Comparing `quantplay-1.3.8/quantplay/broker/shoonya.py` & `quantplay-1.3.9/quantplay/broker/shoonya.py`

 * *Files 2% similar despite different names*

```diff
@@ -395,14 +395,15 @@
                 'uid': 'user_id',
                 'exch' : 'exchange',
                 'remarks' : 'tag',
                 'avgprc' : 'average_price',
                 'prd' : 'product',
                 'trantype' : 'transaction_type',
                 'qty' : 'quantity',
+                "trgprc" : "trigger_price",
                 'fillshares' : 'filled_quantity',
                 'rorgqty' : 'pending_quantity',
                 'norentm' : 'order_timestamp'
 
             }, inplace=True)
 
         orders = orders[self.orders_column_list]
@@ -414,14 +415,18 @@
 
         orders = self.filter_orders(orders, status=status, tag=tag)
 
         orders.transaction_type = orders.transaction_type.replace(
             ["S", "B"], ["SELL", "BUY"]
         )
 
+        orders.status = orders.status.replace(
+            ["TRIGGER_PENDING"], ["TRIGGER PENDING"]
+        )
+
         return orders
 
     def account_summary(self):
         margins = self.api.get_limits()
 
         pnl = 0
         positions = self.positions()
```

### Comparing `quantplay-1.3.8/quantplay/broker/symphony.py` & `quantplay-1.3.9/quantplay/broker/symphony.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/quantplay/broker/xts.py` & `quantplay-1.3.9/quantplay/broker/xts.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/quantplay/broker/xts_utils/Connect.py` & `quantplay-1.3.9/quantplay/broker/xts_utils/Connect.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/quantplay/broker/xts_utils/Exception.py` & `quantplay-1.3.9/quantplay/broker/xts_utils/Exception.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/quantplay/broker/xts_utils/InteractiveSocketClient.py` & `quantplay-1.3.9/quantplay/broker/xts_utils/InteractiveSocketClient.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/quantplay/broker/xts_utils/MarketDataSocketClient.py` & `quantplay-1.3.9/quantplay/broker/xts_utils/MarketDataSocketClient.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/quantplay/broker/zerodha.py` & `quantplay-1.3.9/quantplay/broker/zerodha.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/quantplay/brokerage/angelone/angel_broker.py` & `quantplay-1.3.9/quantplay/brokerage/angelone/angel_broker.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/quantplay/brokerage/generics/broker.py` & `quantplay-1.3.9/quantplay/brokerage/generics/broker.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/quantplay/brokerage/zerodha/ZBroker.py` & `quantplay-1.3.9/quantplay/brokerage/zerodha/ZBroker.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/quantplay/config/qplay_config.py` & `quantplay-1.3.9/quantplay/config/qplay_config.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/quantplay/create_sample_data.py` & `quantplay-1.3.9/quantplay/create_sample_data.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/quantplay/data_modify_script.py` & `quantplay-1.3.9/quantplay/data_modify_script.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/quantplay/date_fix.py` & `quantplay-1.3.9/quantplay/date_fix.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/quantplay/exception/exceptions.py` & `quantplay-1.3.9/quantplay/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/quantplay/executor/strategy_executor.py` & `quantplay-1.3.9/quantplay/executor/strategy_executor.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/quantplay/indicators/Indicator.py` & `quantplay-1.3.9/quantplay/indicators/Indicator.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/quantplay/model/exchange/instrument.py` & `quantplay-1.3.9/quantplay/model/exchange/instrument.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/quantplay/model/exchange/order.py` & `quantplay-1.3.9/quantplay/model/exchange/order.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/quantplay/model/exchange/tick.py` & `quantplay-1.3.9/quantplay/model/exchange/tick.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/quantplay/order_execution/execution_algorithm.py` & `quantplay-1.3.9/quantplay/order_execution/execution_algorithm.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/quantplay/order_execution/mean_price.py` & `quantplay-1.3.9/quantplay/order_execution/mean_price.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/quantplay/reporting/strategy_report.py` & `quantplay-1.3.9/quantplay/reporting/strategy_report.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/quantplay/reporting/visuals.py` & `quantplay-1.3.9/quantplay/reporting/visuals.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/quantplay/services/market.py` & `quantplay-1.3.9/quantplay/services/market.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/quantplay/services/tradelens.py` & `quantplay-1.3.9/quantplay/services/tradelens.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/quantplay/strategies/options/intraday/ladder.py` & `quantplay-1.3.9/quantplay/strategies/options/intraday/ladder.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/quantplay/strategies/options/intraday/musk.py` & `quantplay-1.3.9/quantplay/strategies/options/intraday/musk.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/quantplay/strategy/base.py` & `quantplay-1.3.9/quantplay/strategy/base.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/quantplay/utils/config_util.py` & `quantplay-1.3.9/quantplay/utils/config_util.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/quantplay/utils/constant.py` & `quantplay-1.3.9/quantplay/utils/constant.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/quantplay/utils/data_utils.py` & `quantplay-1.3.9/quantplay/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/quantplay/utils/exchange.py` & `quantplay-1.3.9/quantplay/utils/exchange.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/quantplay/utils/number_utils.py` & `quantplay-1.3.9/quantplay/utils/number_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/quantplay/utils/selenium_utils.py` & `quantplay-1.3.9/quantplay/utils/selenium_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/quantplay/utils/transaction_utils.py` & `quantplay-1.3.9/quantplay/utils/transaction_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/quantplay.egg-info/PKG-INFO` & `quantplay-1.3.9/quantplay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantplay
-Version: 1.3.8
+Version: 1.3.9
 Summary: This python package will be stored in AWS CodeArtifact
 Home-page: 
 Author: 
 Author-email: 
 License: MIT
 
 # Quantplay Alpha playground
```

### Comparing `quantplay-1.3.8/quantplay.egg-info/SOURCES.txt` & `quantplay-1.3.9/quantplay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/setup.py` & `quantplay-1.3.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     for line in Path("requirements.txt").read_text().splitlines()
     if is_requirement(line)
 ]
 
 setup(
     name="quantplay",
     long_description=Path("README.md").read_text(),
-    version="1.3.8",
+    version="1.3.9",
     setup_requires=["pytest-runner"],
     install_requires=requirements,
     tests_require=[],
     packages=find_packages(),
     url="",
     license="MIT",
     author="",
```

### Comparing `quantplay-1.3.8/test/strategy/sample_strategy.py` & `quantplay-1.3.9/test/strategy/sample_strategy.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.8/test/test_motilal.py` & `quantplay-1.3.9/test/test_motilal.py`

 * *Files identical despite different names*

