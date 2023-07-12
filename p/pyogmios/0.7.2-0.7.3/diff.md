# Comparing `tmp/pyogmios-0.7.2.tar.gz` & `tmp/pyogmios-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyogmios-0.7.2.tar", max compression
+gzip compressed data, was "pyogmios-0.7.3.tar", max compression
```

## Comparing `pyogmios-0.7.2.tar` & `pyogmios-0.7.3.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0    11357 2023-06-20 00:54:20.205293 pyogmios-0.7.2/LICENSE
--rw-r--r--   0        0        0     8987 2023-06-18 20:32:48.588485 pyogmios-0.7.2/README.md
--rw-r--r--   0        0        0       22 2023-06-27 03:12:53.465216 pyogmios-0.7.2/pyogmios_client/__init__.py
--rw-r--r--   0        0        0     6360 2023-06-27 02:56:56.199704 pyogmios-0.7.2/pyogmios_client/connection.py
--rw-r--r--   0        0        0     1767 2023-06-14 02:13:31.891113 pyogmios-0.7.2/pyogmios_client/enums/__init__.py
--rw-r--r--   0        0        0     3120 2023-06-27 02:56:56.187607 pyogmios-0.7.2/pyogmios_client/exceptions.py
--rw-r--r--   0        0        0    49367 2023-06-18 20:29:46.297072 pyogmios-0.7.2/pyogmios_client/models/__init__.py
--rw-r--r--   0        0        0      829 2023-06-02 00:12:52.975582 pyogmios-0.7.2/pyogmios_client/models/base_model.py
--rw-r--r--   0        0        0      391 2023-06-18 20:29:46.297119 pyogmios-0.7.2/pyogmios_client/models/base_request_response_model.py
--rw-r--r--   0        0        0      142 2023-05-29 12:12:30.855476 pyogmios-0.7.2/pyogmios_client/models/generated/Digest_Blake2b___Block_Byron_/__init__.py
--rw-r--r--   0        0        0      768 2023-06-02 05:09:09.052857 pyogmios-0.7.2/pyogmios_client/models/generated/Digest_Blake2b___Block_Byron_/body/__init__.py
--rw-r--r--   0        0        0      481 2023-06-02 05:09:09.053018 pyogmios-0.7.2/pyogmios_client/models/generated/Digest_Blake2b___Block_Byron_/body/txPayload__.py
--rw-r--r--   0        0        0      657 2023-06-02 05:09:09.055011 pyogmios-0.7.2/pyogmios_client/models/generated/Digest_Blake2b___Block___.py
--rw-r--r--   0        0        0    96308 2023-06-04 20:21:45.553261 pyogmios-0.7.2/pyogmios_client/models/generated/__init__.py
--rw-r--r--   0        0        0     2247 2023-06-18 20:29:46.297175 pyogmios-0.7.2/pyogmios_client/models/request_model.py
--rw-r--r--   0        0        0     6746 2023-06-19 19:01:43.896476 pyogmios-0.7.2/pyogmios_client/models/response_model.py
--rw-r--r--   0        0        0     7881 2023-06-19 19:01:43.883277 pyogmios-0.7.2/pyogmios_client/models/result_models.py
--rw-r--r--   0        0        0     1642 2023-06-18 20:29:46.297316 pyogmios-0.7.2/pyogmios_client/models/server_health_model.py
--rw-r--r--   0        0        0        0 2023-05-26 12:54:40.062980 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 12:32:23.680249 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/chain_sync/__init__.py
--rw-r--r--   0        0        0     4979 2023-06-18 20:30:58.307688 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/chain_sync/chain_sync_client.py
--rw-r--r--   0        0        0     2039 2023-06-18 20:30:58.307736 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/chain_sync/find_intersect.py
--rw-r--r--   0        0        0      558 2023-06-18 20:30:58.307782 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/chain_sync/request_next.py
--rw-r--r--   0        0        0        0 2023-05-26 12:32:35.095043 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/__init__.py
--rw-r--r--   0        0        0        0 2023-06-02 11:49:09.937446 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/__init__.py
--rw-r--r--   0        0        0     1124 2023-06-19 13:26:03.805077 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/block_height.py
--rw-r--r--   0        0        0     1058 2023-06-19 13:26:03.799723 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/chain_tip.py
--rw-r--r--   0        0        0     1515 2023-06-19 13:26:03.787064 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/current_epoch.py
--rw-r--r--   0        0        0     2442 2023-06-19 19:01:43.872490 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/current_protocol_parameters.py
--rw-r--r--   0        0        0     2467 2023-06-19 19:01:43.889843 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/delegations_and_rewards.py
--rw-r--r--   0        0        0     1417 2023-06-19 19:01:43.873064 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/era_start.py
--rw-r--r--   0        0        0     1513 2023-06-19 12:51:57.285087 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/era_summaries.py
--rw-r--r--   0        0        0     2330 2023-06-19 19:01:43.881035 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/genesis_config.py
--rw-r--r--   0        0        0     2027 2023-06-19 13:26:03.775214 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/ledger_tip.py
--rw-r--r--   0        0        0     2374 2023-06-19 13:05:31.395379 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/non_myopic_member_rewards.py
--rw-r--r--   0        0        0     1918 2023-06-19 13:26:03.802451 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/pool_ids.py
--rw-r--r--   0        0        0     2201 2023-06-19 13:26:03.782424 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/pool_parameters.py
--rw-r--r--   0        0        0     1905 2023-06-19 13:26:03.776935 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/pools_ranking.py
--rw-r--r--   0        0        0     1720 2023-06-19 13:26:03.779645 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/proposed_protocol_parameters.py
--rw-r--r--   0        0        0     1914 2023-06-19 19:01:44.042282 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/rewards_provenance.py
--rw-r--r--   0        0        0     1958 2023-06-19 13:29:43.173810 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/rewards_provenance_new.py
--rw-r--r--   0        0        0     1902 2023-06-19 19:01:44.042429 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/stake_distribution.py
--rw-r--r--   0        0        0     1093 2023-06-19 13:29:43.176699 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/system_start.py
--rw-r--r--   0        0        0     2106 2023-06-19 13:39:50.892528 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/utxo.py
--rw-r--r--   0        0        0     2297 2023-06-18 20:31:30.892685 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/query.py
--rw-r--r--   0        0        0    14518 2023-06-19 19:01:52.850535 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/state_query_client.py
--rw-r--r--   0        0        0        0 2023-05-26 12:32:49.879933 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_monitor/__init__.py
--rw-r--r--   0        0        0     1534 2023-06-18 12:37:04.955397 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_monitor/await_acquire.py
--rw-r--r--   0        0        0     1384 2023-06-18 20:20:34.012346 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_monitor/has_tx.py
--rw-r--r--   0        0        0     1703 2023-06-18 20:20:34.021771 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_monitor/next_tx.py
--rw-r--r--   0        0        0     1359 2023-06-18 20:20:34.030230 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_monitor/release.py
--rw-r--r--   0        0        0     1507 2023-06-18 12:56:13.502657 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_monitor/size_and_capacity.py
--rw-r--r--   0        0        0     3221 2023-06-18 20:20:34.074501 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_monitor/tx_monitor_client.py
--rw-r--r--   0        0        0        0 2023-05-26 12:33:01.699483 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_submission/__init__.py
--rw-r--r--   0        0        0     5139 2023-06-27 03:11:32.548129 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_submission/evaluate_tx.py
--rw-r--r--   0        0        0     4669 2023-06-27 03:08:43.040389 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_submission/evaluation_errors.py
--rw-r--r--   0        0        0    22331 2023-06-27 03:12:17.329092 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_submission/submission_errors.py
--rw-r--r--   0        0        0    16290 2023-06-18 20:20:34.294212 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_submission/submit_tx.py
--rw-r--r--   0        0        0     3338 2023-06-18 20:20:34.059117 pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_submission/tx_submission_client.py
--rw-r--r--   0        0        0      833 2023-06-27 02:55:56.143439 pyogmios-0.7.2/pyogmios_client/request.py
--rw-r--r--   0        0        0     1407 2023-06-27 02:56:56.179854 pyogmios-0.7.2/pyogmios_client/server_health.py
--rw-r--r--   0        0        0        0 2023-05-27 19:33:04.693841 pyogmios-0.7.2/pyogmios_client/utils/__init__.py
--rw-r--r--   0        0        0     2807 2023-06-27 02:55:56.143555 pyogmios-0.7.2/pyogmios_client/utils/event_emitter.py
--rw-r--r--   0        0        0     3100 2023-06-27 02:55:56.143602 pyogmios-0.7.2/pyogmios_client/utils/queue.py
--rw-r--r--   0        0        0      421 2023-06-27 02:55:56.143664 pyogmios-0.7.2/pyogmios_client/utils/socket_utils.py
--rw-r--r--   0        0        0     1870 2023-06-27 03:17:39.383985 pyogmios-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     9974 1970-01-01 00:00:00.000000 pyogmios-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-20 00:54:20.205293 pyogmios-0.7.3/LICENSE
+-rw-r--r--   0        0        0     8987 2023-06-18 20:32:48.588485 pyogmios-0.7.3/README.md
+-rw-r--r--   0        0        0       22 2023-07-12 23:15:06.806819 pyogmios-0.7.3/pyogmios_client/__init__.py
+-rw-r--r--   0        0        0     6360 2023-06-27 02:56:56.199704 pyogmios-0.7.3/pyogmios_client/connection.py
+-rw-r--r--   0        0        0     1767 2023-06-14 02:13:31.891113 pyogmios-0.7.3/pyogmios_client/enums/__init__.py
+-rw-r--r--   0        0        0     3120 2023-06-27 02:56:56.187607 pyogmios-0.7.3/pyogmios_client/exceptions.py
+-rw-r--r--   0        0        0    49450 2023-07-12 23:13:49.669906 pyogmios-0.7.3/pyogmios_client/models/__init__.py
+-rw-r--r--   0        0        0      829 2023-06-02 00:12:52.975582 pyogmios-0.7.3/pyogmios_client/models/base_model.py
+-rw-r--r--   0        0        0      391 2023-06-18 20:29:46.297119 pyogmios-0.7.3/pyogmios_client/models/base_request_response_model.py
+-rw-r--r--   0        0        0      142 2023-05-29 12:12:30.855476 pyogmios-0.7.3/pyogmios_client/models/generated/Digest_Blake2b___Block_Byron_/__init__.py
+-rw-r--r--   0        0        0      768 2023-06-02 05:09:09.052857 pyogmios-0.7.3/pyogmios_client/models/generated/Digest_Blake2b___Block_Byron_/body/__init__.py
+-rw-r--r--   0        0        0      481 2023-06-02 05:09:09.053018 pyogmios-0.7.3/pyogmios_client/models/generated/Digest_Blake2b___Block_Byron_/body/txPayload__.py
+-rw-r--r--   0        0        0      657 2023-06-02 05:09:09.055011 pyogmios-0.7.3/pyogmios_client/models/generated/Digest_Blake2b___Block___.py
+-rw-r--r--   0        0        0    96308 2023-06-04 20:21:45.553261 pyogmios-0.7.3/pyogmios_client/models/generated/__init__.py
+-rw-r--r--   0        0        0     2247 2023-06-18 20:29:46.297175 pyogmios-0.7.3/pyogmios_client/models/request_model.py
+-rw-r--r--   0        0        0     6746 2023-06-19 19:01:43.896476 pyogmios-0.7.3/pyogmios_client/models/response_model.py
+-rw-r--r--   0        0        0     7881 2023-06-19 19:01:43.883277 pyogmios-0.7.3/pyogmios_client/models/result_models.py
+-rw-r--r--   0        0        0     1642 2023-06-18 20:29:46.297316 pyogmios-0.7.3/pyogmios_client/models/server_health_model.py
+-rw-r--r--   0        0        0        0 2023-05-26 12:54:40.062980 pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 12:32:23.680249 pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/chain_sync/__init__.py
+-rw-r--r--   0        0        0     4929 2023-07-12 23:14:00.706207 pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/chain_sync/chain_sync_client.py
+-rw-r--r--   0        0        0     2039 2023-06-18 20:30:58.307736 pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/chain_sync/find_intersect.py
+-rw-r--r--   0        0        0      558 2023-06-18 20:30:58.307782 pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/chain_sync/request_next.py
+-rw-r--r--   0        0        0        0 2023-05-26 12:32:35.095043 pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-02 11:49:09.937446 pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/queries/__init__.py
+-rw-r--r--   0        0        0     1124 2023-06-19 13:26:03.805077 pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/queries/block_height.py
+-rw-r--r--   0        0        0     1058 2023-06-19 13:26:03.799723 pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/queries/chain_tip.py
+-rw-r--r--   0        0        0     1515 2023-06-19 13:26:03.787064 pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/queries/current_epoch.py
+-rw-r--r--   0        0        0     2442 2023-06-19 19:01:43.872490 pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/queries/current_protocol_parameters.py
+-rw-r--r--   0        0        0     2467 2023-06-19 19:01:43.889843 pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/queries/delegations_and_rewards.py
+-rw-r--r--   0        0        0     1417 2023-06-19 19:01:43.873064 pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/queries/era_start.py
+-rw-r--r--   0        0        0     1513 2023-06-19 12:51:57.285087 pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/queries/era_summaries.py
+-rw-r--r--   0        0        0     2330 2023-06-19 19:01:43.881035 pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/queries/genesis_config.py
+-rw-r--r--   0        0        0     2027 2023-06-19 13:26:03.775214 pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/queries/ledger_tip.py
+-rw-r--r--   0        0        0     2374 2023-06-19 13:05:31.395379 pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/queries/non_myopic_member_rewards.py
+-rw-r--r--   0        0        0     1918 2023-06-19 13:26:03.802451 pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/queries/pool_ids.py
+-rw-r--r--   0        0        0     2201 2023-06-19 13:26:03.782424 pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/queries/pool_parameters.py
+-rw-r--r--   0        0        0     1905 2023-06-19 13:26:03.776935 pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/queries/pools_ranking.py
+-rw-r--r--   0        0        0     1720 2023-06-19 13:26:03.779645 pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/queries/proposed_protocol_parameters.py
+-rw-r--r--   0        0        0     1914 2023-06-19 19:01:44.042282 pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/queries/rewards_provenance.py
+-rw-r--r--   0        0        0     1958 2023-06-19 13:29:43.173810 pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/queries/rewards_provenance_new.py
+-rw-r--r--   0        0        0     1902 2023-06-19 19:01:44.042429 pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/queries/stake_distribution.py
+-rw-r--r--   0        0        0     1093 2023-06-19 13:29:43.176699 pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/queries/system_start.py
+-rw-r--r--   0        0        0     2106 2023-06-19 13:39:50.892528 pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/queries/utxo.py
+-rw-r--r--   0        0        0     2297 2023-06-18 20:31:30.892685 pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/query.py
+-rw-r--r--   0        0        0    14518 2023-06-19 19:01:52.850535 pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/state_query_client.py
+-rw-r--r--   0        0        0        0 2023-05-26 12:32:49.879933 pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/tx_monitor/__init__.py
+-rw-r--r--   0        0        0     1534 2023-06-18 12:37:04.955397 pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/tx_monitor/await_acquire.py
+-rw-r--r--   0        0        0     1384 2023-06-18 20:20:34.012346 pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/tx_monitor/has_tx.py
+-rw-r--r--   0        0        0     1703 2023-06-18 20:20:34.021771 pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/tx_monitor/next_tx.py
+-rw-r--r--   0        0        0     1359 2023-06-18 20:20:34.030230 pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/tx_monitor/release.py
+-rw-r--r--   0        0        0     1507 2023-06-18 12:56:13.502657 pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/tx_monitor/size_and_capacity.py
+-rw-r--r--   0        0        0     3221 2023-06-18 20:20:34.074501 pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/tx_monitor/tx_monitor_client.py
+-rw-r--r--   0        0        0        0 2023-05-26 12:33:01.699483 pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/tx_submission/__init__.py
+-rw-r--r--   0        0        0     5139 2023-06-27 03:11:32.548129 pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/tx_submission/evaluate_tx.py
+-rw-r--r--   0        0        0     4669 2023-06-27 03:08:43.040389 pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/tx_submission/evaluation_errors.py
+-rw-r--r--   0        0        0    22331 2023-06-27 03:12:17.329092 pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/tx_submission/submission_errors.py
+-rw-r--r--   0        0        0    16290 2023-06-18 20:20:34.294212 pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/tx_submission/submit_tx.py
+-rw-r--r--   0        0        0     3338 2023-06-18 20:20:34.059117 pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/tx_submission/tx_submission_client.py
+-rw-r--r--   0        0        0      833 2023-06-27 02:55:56.143439 pyogmios-0.7.3/pyogmios_client/request.py
+-rw-r--r--   0        0        0     1407 2023-06-27 02:56:56.179854 pyogmios-0.7.3/pyogmios_client/server_health.py
+-rw-r--r--   0        0        0        0 2023-05-27 19:33:04.693841 pyogmios-0.7.3/pyogmios_client/utils/__init__.py
+-rw-r--r--   0        0        0     2807 2023-06-27 02:55:56.143555 pyogmios-0.7.3/pyogmios_client/utils/event_emitter.py
+-rw-r--r--   0        0        0     3100 2023-06-27 02:55:56.143602 pyogmios-0.7.3/pyogmios_client/utils/queue.py
+-rw-r--r--   0        0        0      421 2023-06-27 02:55:56.143664 pyogmios-0.7.3/pyogmios_client/utils/socket_utils.py
+-rw-r--r--   0        0        0     1870 2023-07-12 23:15:06.822813 pyogmios-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     9974 1970-01-01 00:00:00.000000 pyogmios-0.7.3/PKG-INFO
```

### Comparing `pyogmios-0.7.2/LICENSE` & `pyogmios-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/README.md` & `pyogmios-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/connection.py` & `pyogmios-0.7.3/pyogmios_client/connection.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/enums/__init__.py` & `pyogmios-0.7.3/pyogmios_client/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/exceptions.py` & `pyogmios-0.7.3/pyogmios_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/models/__init__.py` & `pyogmios-0.7.3/pyogmios_client/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,15 +244,15 @@
         ...,
         description="A Blake2b 32-byte digest of a script-integrity hash (i.e redeemers, datums and cost model, CBOR-encoded).",
         examples=["c248757d390181c517a5beadc9c3fe64bf821d3e889a963fc717003ec248757d"],
     )
 
 
 class DigestBlake2bVerificationKey(BaseModel):
-    __root__: constr(min_length=56, max_length=56) = Field(
+    __root__: constr(min_length=56) = Field(
         ...,
         description="A Blake2b 28-byte digest of an Ed25519 verification key.",
         examples=["90181c517a5beadc9c3fe64bf821d3e889a963fc717003ec248757d3"],
     )
 
 
 class DigestBlake2bVrfVerificationKey(BaseModel):
@@ -1910,9 +1910,12 @@
 RollForward.update_forward_refs()
 StandardBlock.update_forward_refs()
 StandardBlockBody.update_forward_refs()
 SoftwareVersion.update_forward_refs()
 StandardBlockBodyUpdatePayload.update_forward_refs()
 SubmitTxErrorCollateralIsScript.update_forward_refs()
 TxBabbage.update_forward_refs()
+TxByron.update_forward_refs()
+TxByronBody.update_forward_refs()
 TxOut.update_forward_refs()
+TxWitnessVk.update_forward_refs()
 Witness.update_forward_refs()
```

### Comparing `pyogmios-0.7.2/pyogmios_client/models/base_model.py` & `pyogmios-0.7.3/pyogmios_client/models/base_model.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/models/generated/Digest_Blake2b___Block_Byron_/body/__init__.py` & `pyogmios-0.7.3/pyogmios_client/models/generated/Digest_Blake2b___Block_Byron_/body/__init__.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/models/generated/Digest_Blake2b___Block___.py` & `pyogmios-0.7.3/pyogmios_client/models/generated/Digest_Blake2b___Block___.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/models/generated/__init__.py` & `pyogmios-0.7.3/pyogmios_client/models/generated/__init__.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/models/request_model.py` & `pyogmios-0.7.3/pyogmios_client/models/request_model.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/models/response_model.py` & `pyogmios-0.7.3/pyogmios_client/models/response_model.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/models/result_models.py` & `pyogmios-0.7.3/pyogmios_client/models/result_models.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/models/server_health_model.py` & `pyogmios-0.7.3/pyogmios_client/models/server_health_model.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/chain_sync/chain_sync_client.py` & `pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/chain_sync/chain_sync_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,14 @@
             if response.methodname is MethodName.REQUEST_NEXT:
                 try:
                     response_handler(RequestNextResponse.parse_raw(message))
                 except Exception as err:
                     print(err)
             elif response.methodname is MethodName.FIND_INTERSECT:
                 request_next(websocket_app)
-            websocket_app.on_message = on_message
 
         websocket_app.on_message = on_message
 
         async def shutdown() -> None:
             """
             Shutdown the chain sync client.
             """
```

### Comparing `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/chain_sync/find_intersect.py` & `pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/chain_sync/find_intersect.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/chain_sync/request_next.py` & `pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/chain_sync/request_next.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/block_height.py` & `pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/queries/block_height.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/chain_tip.py` & `pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/queries/chain_tip.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/current_epoch.py` & `pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/queries/current_epoch.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/current_protocol_parameters.py` & `pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/queries/current_protocol_parameters.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/delegations_and_rewards.py` & `pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/queries/delegations_and_rewards.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/era_start.py` & `pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/queries/era_start.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/era_summaries.py` & `pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/queries/era_summaries.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/genesis_config.py` & `pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/queries/genesis_config.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/ledger_tip.py` & `pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/queries/ledger_tip.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/non_myopic_member_rewards.py` & `pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/queries/non_myopic_member_rewards.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/pool_ids.py` & `pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/queries/pool_ids.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/pool_parameters.py` & `pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/queries/pool_parameters.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/pools_ranking.py` & `pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/queries/pools_ranking.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/proposed_protocol_parameters.py` & `pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/queries/proposed_protocol_parameters.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/rewards_provenance.py` & `pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/queries/rewards_provenance.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/rewards_provenance_new.py` & `pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/queries/rewards_provenance_new.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/stake_distribution.py` & `pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/queries/stake_distribution.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/system_start.py` & `pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/queries/system_start.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/queries/utxo.py` & `pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/queries/utxo.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/query.py` & `pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/query.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/state_query/state_query_client.py` & `pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/state_query/state_query_client.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_monitor/await_acquire.py` & `pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/tx_monitor/await_acquire.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_monitor/has_tx.py` & `pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/tx_monitor/has_tx.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_monitor/next_tx.py` & `pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/tx_monitor/next_tx.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_monitor/release.py` & `pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/tx_monitor/release.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_monitor/size_and_capacity.py` & `pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/tx_monitor/size_and_capacity.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_monitor/tx_monitor_client.py` & `pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/tx_monitor/tx_monitor_client.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_submission/evaluate_tx.py` & `pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/tx_submission/evaluate_tx.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_submission/evaluation_errors.py` & `pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/tx_submission/evaluation_errors.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_submission/submission_errors.py` & `pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/tx_submission/submission_errors.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_submission/submit_tx.py` & `pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/tx_submission/submit_tx.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/ouroboros_mini_protocols/tx_submission/tx_submission_client.py` & `pyogmios-0.7.3/pyogmios_client/ouroboros_mini_protocols/tx_submission/tx_submission_client.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/request.py` & `pyogmios-0.7.3/pyogmios_client/request.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/server_health.py` & `pyogmios-0.7.3/pyogmios_client/server_health.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/utils/event_emitter.py` & `pyogmios-0.7.3/pyogmios_client/utils/event_emitter.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyogmios_client/utils/queue.py` & `pyogmios-0.7.3/pyogmios_client/utils/queue.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.7.2/pyproject.toml` & `pyogmios-0.7.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyogmios"
-version = "0.7.2"
+version = "0.7.3"
 description = "Python client for Ogmios"
 authors = ["Hareem Adderley <hadderley@kingpinapps.com>"]
 readme = "README.md"
 packages = [{include = "pyogmios_client"}]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
@@ -49,15 +49,15 @@
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "-p no:cacheprovider"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.7.2"
+version = "0.7.3"
 version_files = [
     "pyogmios_client/__init__.py:__version__",
     "pyproject.toml:version"
 ]
 update_changelog_on_bump = true
 style = [
     ["qmark", "fg:#ff9d00 bold"],
```

### Comparing `pyogmios-0.7.2/PKG-INFO` & `pyogmios-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyogmios
-Version: 0.7.2
+Version: 0.7.3
 Summary: Python client for Ogmios
 Author: Hareem Adderley
 Author-email: hadderley@kingpinapps.com
 Requires-Python: >=3.8.10,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

