# Comparing `tmp/vega_sim-1.1.1.tar.gz` & `tmp/vega_sim-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vega_sim-1.1.1.tar", max compression
+gzip compressed data, was "vega_sim-1.2.0.tar", max compression
```

## Comparing `vega_sim-1.1.1.tar` & `vega_sim-1.2.0.tar`

### file list

```diff
@@ -1,223 +1,236 @@
--rw-r--r--   0        0        0     1061 2023-05-18 13:16:50.926272 vega_sim-1.1.1/LICENSE
--rw-r--r--   0        0        0     1742 2023-05-18 13:16:50.998279 vega_sim-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      224 2023-05-18 13:16:51.002280 vega_sim-1.1.1/vega_sim/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 13:16:51.002280 vega_sim-1.1.1/vega_sim/api/__init__.py
--rw-r--r--   0        0        0    52771 2023-05-18 13:16:51.002280 vega_sim-1.1.1/vega_sim/api/data.py
--rw-r--r--   0        0        0    22276 2023-05-18 13:16:51.002280 vega_sim-1.1.1/vega_sim/api/data_raw.py
--rw-r--r--   0        0        0      548 2023-05-18 13:16:51.002280 vega_sim-1.1.1/vega_sim/api/faucet.py
--rw-r--r--   0        0        0    20460 2023-05-18 13:16:51.002280 vega_sim-1.1.1/vega_sim/api/governance.py
--rw-r--r--   0        0        0     4806 2023-05-18 13:16:51.002280 vega_sim-1.1.1/vega_sim/api/helpers.py
--rw-r--r--   0        0        0    12851 2023-05-18 13:16:51.002280 vega_sim-1.1.1/vega_sim/api/market.py
--rw-r--r--   0        0        0    22594 2023-05-18 13:16:51.002280 vega_sim-1.1.1/vega_sim/api/trading.py
--rw-r--r--   0        0        0      122 2023-05-18 13:16:51.002280 vega_sim-1.1.1/vega_sim/constants.py
--rw-r--r--   0        0        0     4575 2023-05-18 13:16:51.002280 vega_sim-1.1.1/vega_sim/devops/README.md
--rw-r--r--   0        0        0     1377 2023-05-18 13:16:51.002280 vega_sim-1.1.1/vega_sim/devops/classes.py
--rw-r--r--   0        0        0       41 2023-05-18 13:16:51.002280 vega_sim-1.1.1/vega_sim/devops/example_tokens.json
--rw-r--r--   0        0        0     7517 2023-05-18 13:16:51.002280 vega_sim-1.1.1/vega_sim/devops/registry.py
--rw-r--r--   0        0        0     4592 2023-05-18 13:16:51.002280 vega_sim-1.1.1/vega_sim/devops/run_agent.py
--rw-r--r--   0        0        0     2994 2023-05-18 13:16:51.002280 vega_sim-1.1.1/vega_sim/devops/run_scenario.py
--rw-r--r--   0        0        0    11453 2023-05-18 13:16:51.002280 vega_sim-1.1.1/vega_sim/devops/scenario.py
--rw-r--r--   0        0        0     2137 2023-05-18 13:16:51.002280 vega_sim-1.1.1/vega_sim/devops/wallet.py
--rw-r--r--   0        0        0       48 2023-05-18 13:16:51.002280 vega_sim-1.1.1/vega_sim/environment/__init__.py
--rw-r--r--   0        0        0     2743 2023-05-18 13:16:51.002280 vega_sim-1.1.1/vega_sim/environment/agent.py
--rw-r--r--   0        0        0    26236 2023-05-18 13:16:51.002280 vega_sim-1.1.1/vega_sim/environment/environment.py
--rw-r--r--   0        0        0        0 2023-05-18 13:16:51.002280 vega_sim-1.1.1/vega_sim/grpc/__init__.py
--rw-r--r--   0        0        0     1560 2023-05-18 13:16:51.002280 vega_sim-1.1.1/vega_sim/grpc/client.py
--rw-r--r--   0        0        0    20179 2023-05-18 13:16:51.002280 vega_sim-1.1.1/vega_sim/local_data_cache.py
--rw-r--r--   0        0        0    19674 2023-05-18 13:16:51.002280 vega_sim-1.1.1/vega_sim/network_service.py
--rw-r--r--   0        0        0    27342 2023-05-18 13:16:51.002280 vega_sim-1.1.1/vega_sim/null_service.py
--rw-r--r--   0        0        0        0 2023-05-18 13:16:51.002280 vega_sim-1.1.1/vega_sim/parameter_test/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 13:16:51.002280 vega_sim-1.1.1/vega_sim/parameter_test/parameter/__init__.py
--rw-r--r--   0        0        0     3042 2023-05-18 13:16:51.002280 vega_sim-1.1.1/vega_sim/parameter_test/parameter/configs.py
--rw-r--r--   0        0        0     6665 2023-05-18 13:16:51.002280 vega_sim-1.1.1/vega_sim/parameter_test/parameter/experiment.py
--rw-r--r--   0        0        0    13541 2023-05-18 13:16:51.002280 vega_sim-1.1.1/vega_sim/parameter_test/parameter/loggers.py
--rw-r--r--   0        0        0      636 2023-05-18 13:16:51.002280 vega_sim-1.1.1/vega_sim/parameter_test/run.py
--rw-r--r--   0        0        0       63 2023-05-18 13:16:51.002280 vega_sim-1.1.1/vega_sim/proto/__init__.py
--rw-r--r--   0        0        0     5048 2023-05-18 13:16:51.002280 vega_sim-1.1.1/vega_sim/proto/blockexplorer/api/v1/blockexplorer_pb2.py
--rw-r--r--   0        0        0     6827 2023-05-18 13:16:51.002280 vega_sim-1.1.1/vega_sim/proto/blockexplorer/api/v1/blockexplorer_pb2_grpc.py
--rw-r--r--   0        0        0       37 2023-05-18 13:16:51.002280 vega_sim-1.1.1/vega_sim/proto/data_node/__init__.py
--rw-r--r--   0        0        0       35 2023-05-18 13:16:51.002280 vega_sim-1.1.1/vega_sim/proto/data_node/api/__init__.py
--rw-r--r--   0        0        0      164 2023-05-18 13:16:51.002280 vega_sim-1.1.1/vega_sim/proto/data_node/api/v2/__init__.py
--rw-r--r--   0        0        0   127521 2023-05-18 13:16:51.002280 vega_sim-1.1.1/vega_sim/proto/data_node/api/v2/trading_data_pb2.py
--rw-r--r--   0        0        0   178382 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/data_node/api/v2/trading_data_pb2_grpc.py
--rw-r--r--   0        0        0     1075 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/__init__.py
--rw-r--r--   0        0        0       35 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/api/__init__.py
--rw-r--r--   0        0        0      247 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/api/v1/__init__.py
--rw-r--r--   0        0        0    16905 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/api/v1/core_pb2.py
--rw-r--r--   0        0        0    18869 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/api/v1/core_pb2_grpc.py
--rw-r--r--   0        0        0     8684 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/api/v1/corestate_pb2.py
--rw-r--r--   0        0        0    22463 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/api/v1/corestate_pb2_grpc.py
--rw-r--r--   0        0        0     3113 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/assets_pb2.py
--rw-r--r--   0        0        0      158 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/assets_pb2_grpc.py
--rw-r--r--   0        0        0     7055 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/chain_events_pb2.py
--rw-r--r--   0        0        0      158 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/chain_events_pb2_grpc.py
--rw-r--r--   0        0        0       35 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/checkpoint/__init__.py
--rw-r--r--   0        0        0      152 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/checkpoint/v1/__init__.py
--rw-r--r--   0        0        0    12357 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/checkpoint/v1/checkpoint_pb2.py
--rw-r--r--   0        0        0      158 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/checkpoint/v1/checkpoint_pb2_grpc.py
--rw-r--r--   0        0        0       35 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/commands/__init__.py
--rw-r--r--   0        0        0      700 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/commands/v1/__init__.py
--rw-r--r--   0        0        0     8192 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/commands/v1/commands_pb2.py
--rw-r--r--   0        0        0      158 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/commands/v1/commands_pb2_grpc.py
--rw-r--r--   0        0        0     1623 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/commands/v1/data_pb2.py
--rw-r--r--   0        0        0      158 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/commands/v1/data_pb2_grpc.py
--rw-r--r--   0        0        0     1296 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/commands/v1/signature_pb2.py
--rw-r--r--   0        0        0      158 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/commands/v1/signature_pb2_grpc.py
--rw-r--r--   0        0        0     5943 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/commands/v1/transaction_pb2.py
--rw-r--r--   0        0        0      158 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/commands/v1/transaction_pb2_grpc.py
--rw-r--r--   0        0        0     6388 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/commands/v1/validator_commands_pb2.py
--rw-r--r--   0        0        0      158 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/commands/v1/validator_commands_pb2_grpc.py
--rw-r--r--   0        0        0       35 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/data/__init__.py
--rw-r--r--   0        0        0      217 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/data/v1/__init__.py
--rw-r--r--   0        0        0     2311 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/data/v1/data_pb2.py
--rw-r--r--   0        0        0      158 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/data/v1/data_pb2_grpc.py
--rw-r--r--   0        0        0     2568 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/data/v1/spec_pb2.py
--rw-r--r--   0        0        0      158 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/data/v1/spec_pb2_grpc.py
--rw-r--r--   0        0        0     3490 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/data_source_pb2.py
--rw-r--r--   0        0        0      158 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/data_source_pb2_grpc.py
--rw-r--r--   0        0        0       35 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/events/__init__.py
--rw-r--r--   0        0        0      128 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/events/v1/__init__.py
--rw-r--r--   0        0        0    34047 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/events/v1/events_pb2.py
--rw-r--r--   0        0        0      158 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/events/v1/events_pb2_grpc.py
--rw-r--r--   0        0        0    13475 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/governance_pb2.py
--rw-r--r--   0        0        0      158 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/governance_pb2_grpc.py
--rw-r--r--   0        0        0     9423 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/markets_pb2.py
--rw-r--r--   0        0        0      158 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/markets_pb2_grpc.py
--rw-r--r--   0        0        0     1559 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/oracle_pb2.py
--rw-r--r--   0        0        0      158 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/oracle_pb2_grpc.py
--rw-r--r--   0        0        0       35 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/snapshot/__init__.py
--rw-r--r--   0        0        0      140 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/snapshot/v1/__init__.py
--rw-r--r--   0        0        0    48044 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/snapshot/v1/snapshot_pb2.py
--rw-r--r--   0        0        0      158 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/snapshot/v1/snapshot_pb2_grpc.py
--rw-r--r--   0        0        0    38139 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/vega_pb2.py
--rw-r--r--   0        0        0      158 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/vega_pb2_grpc.py
--rw-r--r--   0        0        0       35 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/wallet/__init__.py
--rw-r--r--   0        0        0      128 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/wallet/v1/__init__.py
--rw-r--r--   0        0        0     4846 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/wallet/v1/wallet_pb2.py
--rw-r--r--   0        0        0      158 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/proto/vega/wallet/v1/wallet_pb2_grpc.py
--rw-r--r--   0        0        0        0 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/quant/__init__.py
--rw-r--r--   0        0        0     2961 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/quant/quant.py
--rw-r--r--   0        0        0       29 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/reinforcement/.gitignore
--rw-r--r--   0        0        0        0 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/reinforcement/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/reinforcement/agents/__init__.py
--rw-r--r--   0        0        0     8048 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/reinforcement/agents/learning_agent.py
--rw-r--r--   0        0        0    13440 2023-05-18 13:16:51.006280 vega_sim-1.1.1/vega_sim/reinforcement/agents/learning_agent_MO.py
--rw-r--r--   0        0        0    18985 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/reinforcement/agents/learning_agent_MO_with_vol.py
--rw-r--r--   0        0        0    13019 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/reinforcement/agents/learning_agent_heuristic.py
--rw-r--r--   0        0        0     4754 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/reinforcement/agents/simple_agent.py
--rw-r--r--   0        0        0      925 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/reinforcement/distributions.py
--rw-r--r--   0        0        0        0 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/reinforcement/full_market_sim/__init__.py
--rw-r--r--   0        0        0      608 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/reinforcement/full_market_sim/environments.py
--rw-r--r--   0        0        0        0 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/reinforcement/full_market_sim/utils/__init__.py
--rw-r--r--   0        0        0     4458 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/reinforcement/full_market_sim/utils/create_csv.py
--rw-r--r--   0        0        0     1932 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/reinforcement/full_market_sim/utils/external_assetprice.py
--rw-r--r--   0        0        0     4782 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/reinforcement/full_market_sim/utils/logdata.py
--rw-r--r--   0        0        0     4809 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/reinforcement/full_market_sim/utils/strategy.py
--rw-r--r--   0        0        0      662 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/reinforcement/helpers.py
--rw-r--r--   0        0        0     3092 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/reinforcement/la_market_state.py
--rw-r--r--   0        0        0     4243 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/reinforcement/networks.py
--rw-r--r--   0        0        0     4015 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/reinforcement/plot.py
--rw-r--r--   0        0        0     9642 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/reinforcement/run_rl_agent.py
--rw-r--r--   0        0        0     2446 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/reinforcement/run_simple_agent.py
--rw-r--r--   0        0        0      505 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/reinforcement/theory_intro/Bibliography.bib
--rw-r--r--   0        0        0    13970 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/reinforcement/theory_intro/RL.tex
--rw-r--r--   0        0        0    36669 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/reinforcement/theory_intro/images/RL.png
--rw-r--r--   0        0        0    29521 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/reinforcement/theory_intro/images/RL_inv.png
--rw-r--r--   0        0        0    39266 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/reinforcement/theory_intro/images/logo.png
--rw-r--r--   0        0        0    52831 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/reinforcement/theory_intro/images/logo_inv.png
--rw-r--r--   0        0        0        0 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/reinforcement/v2/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/reinforcement/v2/agents/__init__.py
--rw-r--r--   0        0        0     3661 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/reinforcement/v2/agents/learning_agent.py
--rw-r--r--   0        0        0    12222 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/reinforcement/v2/agents/learning_agent_MO.py
--rw-r--r--   0        0        0     2554 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/reinforcement/v2/agents/puppets.py
--rw-r--r--   0        0        0     5382 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/reinforcement/v2/learning_environment.py
--rw-r--r--   0        0        0     1204 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/reinforcement/v2/rewards.py
--rw-r--r--   0        0        0     4365 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/reinforcement/v2/run.py
--rw-r--r--   0        0        0        0 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/reinforcement/v2/stable_baselines/__init__.py
--rw-r--r--   0        0        0     3773 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/reinforcement/v2/stable_baselines/environment.py
--rw-r--r--   0        0        0      392 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/reinforcement/v2/stable_baselines/run.py
--rw-r--r--   0        0        0      603 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/reinforcement/v2/stable_baselines/states.py
--rw-r--r--   0        0        0     4377 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/reinforcement/v2/states.py
--rw-r--r--   0        0        0        0 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/replay/__init__.py
--rw-r--r--   0        0        0     1386 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/replay/replay.py
--rw-r--r--   0        0        0        0 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/scenario/__init__.py
--rw-r--r--   0        0        0     2260 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/scenario/adhoc.py
--rw-r--r--   0        0        0        0 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/scenario/common/__init__.py
--rw-r--r--   0        0        0   105264 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/scenario/common/agents.py
--rw-r--r--   0        0        0     7797 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/scenario/common/utils/ideal_mm_models.py
--rw-r--r--   0        0        0     6107 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/scenario/common/utils/price_process.py
--rw-r--r--   0        0        0      779 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/scenario/comprehensive_market/agents.py
--rw-r--r--   0        0        0    12572 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/scenario/comprehensive_market/scenario.py
--rw-r--r--   0        0        0     5306 2023-05-18 13:16:51.010280 vega_sim-1.1.1/vega_sim/scenario/configurable_market/agents.py
--rw-r--r--   0        0        0     8149 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/scenario/configurable_market/scenario.py
--rw-r--r--   0        0        0      286 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/scenario/constants.py
--rw-r--r--   0        0        0        0 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/scenario/curve_market_maker/__init__.py
--rw-r--r--   0        0        0    11025 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/scenario/curve_market_maker/scenario.py
--rw-r--r--   0        0        0    19682 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/scenario/fuzzed_markets/agents.py
--rw-r--r--   0        0        0     2213 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/scenario/fuzzed_markets/run_fuzz_test.py
--rw-r--r--   0        0        0    15845 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/scenario/fuzzed_markets/scenario.py
--rw-r--r--   0        0        0        0 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/scenario/hedged_market_maker/__init__.py
--rw-r--r--   0        0        0      827 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/scenario/hedged_market_maker/agents.py
--rw-r--r--   0        0        0    18488 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/scenario/hedged_market_maker/scenario.py
--rw-r--r--   0        0        0        0 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/scenario/ideal_market_maker/__init__.py
--rw-r--r--   0        0        0    31515 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/scenario/ideal_market_maker/agents.py
--rw-r--r--   0        0        0     3160 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/scenario/ideal_market_maker/environments.py
--rw-r--r--   0        0        0     8680 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/scenario/ideal_market_maker/scenario.py
--rw-r--r--   0        0        0        0 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/scenario/ideal_market_maker/utils/__init__.py
--rw-r--r--   0        0        0     4782 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/scenario/ideal_market_maker/utils/log_data.py
--rw-r--r--   0        0        0     4818 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/scenario/ideal_market_maker/utils/strategy.py
--rw-r--r--   0        0        0        0 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/scenario/ideal_market_maker_v2/__init__.py
--rw-r--r--   0        0        0    11478 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/scenario/ideal_market_maker_v2/agents.py
--rw-r--r--   0        0        0     9525 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/scenario/ideal_market_maker_v2/scenario.py
--rw-r--r--   0        0        0        0 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/scenario/ideal_market_maker_v2/utils/__init__.py
--rw-r--r--   0        0        0     4818 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/scenario/ideal_market_maker_v2/utils/strategy.py
--rw-r--r--   0        0        0     1687 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/scenario/market_crash/price_process.py
--rw-r--r--   0        0        0     9288 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/scenario/market_crash/scenario.py
--rw-r--r--   0        0        0     1948 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/scenario/multi_market/agents.py
--rw-r--r--   0        0        0    20142 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/scenario/multi_market/scenario.py
--rw-r--r--   0        0        0    10779 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/scenario/parameter_experiment/scenario.py
--rw-r--r--   0        0        0        0 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/scenario/realtime_market/__init__.py
--rw-r--r--   0        0        0     4646 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/scenario/realtime_market/scenario.py
--rw-r--r--   0        0        0     7018 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/scenario/registry.py
--rw-r--r--   0        0        0     3510 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/scenario/scenario.py
--rw-r--r--   0        0        0    88827 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/service.py
--rw-r--r--   0        0        0        0 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/tools/__init__.py
--rw-r--r--   0        0        0     2011 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/tools/load_binaries.py
--rw-r--r--   0        0        0     9207 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/tools/scenario_output.py
--rw-r--r--   0        0        0    21009 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/tools/scenario_plots.py
--rw-r--r--   0        0        0     2612 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/vegahome/config/data-node/config.toml
--rw-r--r--   0        0        0      277 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/vegahome/config/faucet/config.toml
--rw-r--r--   0        0        0     3968 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/vegahome/config/node/config.toml
--rw-r--r--   0        0        0      312 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/vegahome/config/node/wallets.encrypted
--rw-r--r--   0        0        0      114 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/vegahome/config/wallet-service/config.toml
--rw-r--r--   0        0        0      321 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/vegahome/config/wallet-service/networks/local.toml
--rw-r--r--   0        0        0      586 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/vegahome/data/faucet/wallets/vega.1639051237294446827
--rw-r--r--   0        0        0      586 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/vegahome/data/faucet/wallets/vega.1641976836892788243
--rw-r--r--   0        0        0      586 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/vegahome/data/faucet/wallets/vega.1641977214518086643
--rw-r--r--   0        0        0      586 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/vegahome/data/faucet/wallets/vega.1641977270881740938
--rw-r--r--   0        0        0      586 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/vegahome/data/faucet/wallets/vega.1641977376563008654
--rw-r--r--   0        0        0      586 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/vegahome/data/faucet/wallets/vega.1641977471442889253
--rw-r--r--   0        0        0      586 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/vegahome/data/faucet/wallets/vega.1641977537535784009
--rw-r--r--   0        0        0      586 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/vegahome/data/faucet/wallets/vega.1641977956797580358
--rw-r--r--   0        0        0      586 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/vegahome/data/faucet/wallets/vega.1641978034856367487
--rw-r--r--   0        0        0      586 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/vegahome/data/faucet/wallets/vega.1643100690865690276
--rw-r--r--   0        0        0      491 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/vegahome/data/node/wallets/ethereum/UTC--2021-12-09T12-00-28.751280926Z--b6ea7744971f455bbd754a97e8e05ea13dc1a033
--rw-r--r--   0        0        0      491 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/vegahome/data/node/wallets/ethereum/UTC--2022-01-12T08-54-28.446104867Z--d1b7ef68bb457b47837c6e81da24455be7a8be0d
--rw-r--r--   0        0        0      491 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/vegahome/data/node/wallets/ethereum/UTC--2022-01-12T08-57-18.522457076Z--dc699ecdab1705ebe83b60345060b6b7620263a3
--rw-r--r--   0        0        0      491 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/vegahome/data/node/wallets/ethereum/UTC--2022-01-12T08-58-36.643184436Z--760895ae7f813d685b048336fac88625441d6aa7
--rw-r--r--   0        0        0      491 2023-05-18 13:16:51.014281 vega_sim-1.1.1/vega_sim/vegahome/data/node/wallets/ethereum/UTC--2022-01-12T08-59-08.359696969Z--9e5beec6e56b28ccbd02864840b0f1e0125e42ce
--rw-r--r--   0        0        0      586 2023-05-18 13:16:51.018281 vega_sim-1.1.1/vega_sim/vegahome/data/node/wallets/vega/vega.1639051228296308758
--rw-r--r--   0        0        0      586 2023-05-18 13:16:51.018281 vega_sim-1.1.1/vega_sim/vegahome/data/node/wallets/vega/vega.1641977668033624243
--rw-r--r--   0        0        0      586 2023-05-18 13:16:51.018281 vega_sim-1.1.1/vega_sim/vegahome/data/node/wallets/vega/vega.1641977838095755067
--rw-r--r--   0        0        0      586 2023-05-18 13:16:51.018281 vega_sim-1.1.1/vega_sim/vegahome/data/node/wallets/vega/vega.1641977916225009082
--rw-r--r--   0        0        0      586 2023-05-18 13:16:51.018281 vega_sim-1.1.1/vega_sim/vegahome/data/node/wallets/vega/vega.1641977947934016124
--rw-r--r--   0        0        0       46 2023-05-18 13:16:51.018281 vega_sim-1.1.1/vega_sim/vegahome/data/priv_validator_state.json
--rw-r--r--   0        0        0     3243 2023-05-18 13:16:51.018281 vega_sim-1.1.1/vega_sim/vegahome/data/wallet-service/rsa-keys/private.pem
--rw-r--r--   0        0        0      800 2023-05-18 13:16:51.018281 vega_sim-1.1.1/vega_sim/vegahome/data/wallet-service/rsa-keys/public.pem
--rw-r--r--   0        0        0     9045 2023-05-18 13:16:51.018281 vega_sim-1.1.1/vega_sim/vegahome/genesis.json
--rw-r--r--   0        0        0        3 2023-05-18 13:16:51.018281 vega_sim-1.1.1/vega_sim/vegahome/passphrase-file
--rw-r--r--   0        0        0        0 2023-05-18 13:16:51.018281 vega_sim-1.1.1/vega_sim/wallet/__init__.py
--rw-r--r--   0        0        0     1552 2023-05-18 13:16:51.018281 vega_sim-1.1.1/vega_sim/wallet/base.py
--rw-r--r--   0        0        0     6855 2023-05-18 13:16:51.018281 vega_sim-1.1.1/vega_sim/wallet/slim_wallet.py
--rw-r--r--   0        0        0     9304 2023-05-18 13:16:51.018281 vega_sim-1.1.1/vega_sim/wallet/vega_wallet.py
--rw-r--r--   0        0        0     1870 1970-01-01 00:00:00.000000 vega_sim-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-07-13 15:30:06.191975 vega_sim-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1736 2023-07-13 15:30:06.255976 vega_sim-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      292 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/api/__init__.py
+-rw-r--r--   0        0        0    53438 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/api/data.py
+-rw-r--r--   0        0        0    23160 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/api/data_raw.py
+-rw-r--r--   0        0        0      548 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/api/faucet.py
+-rw-r--r--   0        0        0    20460 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/api/governance.py
+-rw-r--r--   0        0        0     4995 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/api/helpers.py
+-rw-r--r--   0        0        0    12928 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/api/market.py
+-rw-r--r--   0        0        0    22664 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/api/trading.py
+-rw-r--r--   0        0        0      122 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/constants.py
+-rw-r--r--   0        0        0     4575 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/devops/README.md
+-rw-r--r--   0        0        0     1377 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/devops/classes.py
+-rw-r--r--   0        0        0       41 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/devops/example_tokens.json
+-rw-r--r--   0        0        0     7517 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/devops/registry.py
+-rw-r--r--   0        0        0     4592 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/devops/run_agent.py
+-rw-r--r--   0        0        0     2994 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/devops/run_scenario.py
+-rw-r--r--   0        0        0    11453 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/devops/scenario.py
+-rw-r--r--   0        0        0     2137 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/devops/wallet.py
+-rw-r--r--   0        0        0       48 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/environment/__init__.py
+-rw-r--r--   0        0        0     2947 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/environment/agent.py
+-rw-r--r--   0        0        0    26761 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/environment/environment.py
+-rw-r--r--   0        0        0        0 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/grpc/__init__.py
+-rw-r--r--   0        0        0     1560 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/grpc/client.py
+-rw-r--r--   0        0        0    20381 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/local_data_cache.py
+-rw-r--r--   0        0        0    27039 2023-07-13 15:30:06.255976 vega_sim-1.2.0/vega_sim/network_service.py
+-rw-r--r--   0        0        0    27824 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/null_service.py
+-rw-r--r--   0        0        0        0 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/parameter_test/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/parameter_test/parameter/__init__.py
+-rw-r--r--   0        0        0     3042 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/parameter_test/parameter/configs.py
+-rw-r--r--   0        0        0     6665 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/parameter_test/parameter/experiment.py
+-rw-r--r--   0        0        0    13541 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/parameter_test/parameter/loggers.py
+-rw-r--r--   0        0        0      636 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/parameter_test/run.py
+-rw-r--r--   0        0        0       63 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/__init__.py
+-rw-r--r--   0        0        0     5463 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/blockexplorer/api/v1/blockexplorer_pb2.py
+-rw-r--r--   0        0        0     6827 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/blockexplorer/api/v1/blockexplorer_pb2_grpc.py
+-rw-r--r--   0        0        0       37 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/data_node/__init__.py
+-rw-r--r--   0        0        0       35 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/data_node/api/__init__.py
+-rw-r--r--   0        0        0      164 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/data_node/api/v2/__init__.py
+-rw-r--r--   0        0        0   136996 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/data_node/api/v2/trading_data_pb2.py
+-rw-r--r--   0        0        0   180423 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/data_node/api/v2/trading_data_pb2_grpc.py
+-rw-r--r--   0        0        0     1075 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/__init__.py
+-rw-r--r--   0        0        0       35 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/api/__init__.py
+-rw-r--r--   0        0        0      247 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/api/v1/__init__.py
+-rw-r--r--   0        0        0    17777 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/api/v1/core_pb2.py
+-rw-r--r--   0        0        0    18869 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/api/v1/core_pb2_grpc.py
+-rw-r--r--   0        0        0     9351 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/api/v1/corestate_pb2.py
+-rw-r--r--   0        0        0    22463 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/api/v1/corestate_pb2_grpc.py
+-rw-r--r--   0        0        0     3300 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/assets_pb2.py
+-rw-r--r--   0        0        0      158 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/assets_pb2_grpc.py
+-rw-r--r--   0        0        0     7856 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/chain_events_pb2.py
+-rw-r--r--   0        0        0      158 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/chain_events_pb2_grpc.py
+-rw-r--r--   0        0        0       35 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/checkpoint/__init__.py
+-rw-r--r--   0        0        0      152 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/checkpoint/v1/__init__.py
+-rw-r--r--   0        0        0    15518 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/checkpoint/v1/checkpoint_pb2.py
+-rw-r--r--   0        0        0      158 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/checkpoint/v1/checkpoint_pb2_grpc.py
+-rw-r--r--   0        0        0       35 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/commands/__init__.py
+-rw-r--r--   0        0        0      700 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/commands/v1/__init__.py
+-rw-r--r--   0        0        0    10698 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/commands/v1/commands_pb2.py
+-rw-r--r--   0        0        0      158 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/commands/v1/commands_pb2_grpc.py
+-rw-r--r--   0        0        0     1690 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/commands/v1/data_pb2.py
+-rw-r--r--   0        0        0      158 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/commands/v1/data_pb2_grpc.py
+-rw-r--r--   0        0        0     1339 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/commands/v1/signature_pb2.py
+-rw-r--r--   0        0        0      158 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/commands/v1/signature_pb2_grpc.py
+-rw-r--r--   0        0        0     6323 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/commands/v1/transaction_pb2.py
+-rw-r--r--   0        0        0      158 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/commands/v1/transaction_pb2_grpc.py
+-rw-r--r--   0        0        0     6777 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/commands/v1/validator_commands_pb2.py
+-rw-r--r--   0        0        0      158 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/commands/v1/validator_commands_pb2_grpc.py
+-rw-r--r--   0        0        0       35 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/data/__init__.py
+-rw-r--r--   0        0        0      217 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/data/v1/__init__.py
+-rw-r--r--   0        0        0     2474 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/data/v1/data_pb2.py
+-rw-r--r--   0        0        0      158 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/data/v1/data_pb2_grpc.py
+-rw-r--r--   0        0        0     2707 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/data/v1/spec_pb2.py
+-rw-r--r--   0        0        0      158 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/data/v1/spec_pb2_grpc.py
+-rw-r--r--   0        0        0     5045 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/data_source_pb2.py
+-rw-r--r--   0        0        0      158 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/data_source_pb2_grpc.py
+-rw-r--r--   0        0        0       35 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/events/__init__.py
+-rw-r--r--   0        0        0      128 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/events/v1/__init__.py
+-rw-r--r--   0        0        0    36828 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/events/v1/events_pb2.py
+-rw-r--r--   0        0        0      158 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/events/v1/events_pb2_grpc.py
+-rw-r--r--   0        0        0    20036 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/governance_pb2.py
+-rw-r--r--   0        0        0      158 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/governance_pb2_grpc.py
+-rw-r--r--   0        0        0    10667 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/markets_pb2.py
+-rw-r--r--   0        0        0      158 2023-07-13 15:30:06.259976 vega_sim-1.2.0/vega_sim/proto/vega/markets_pb2_grpc.py
+-rw-r--r--   0        0        0     1626 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/proto/vega/oracle_pb2.py
+-rw-r--r--   0        0        0      158 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/proto/vega/oracle_pb2_grpc.py
+-rw-r--r--   0        0        0       35 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/proto/vega/snapshot/__init__.py
+-rw-r--r--   0        0        0      140 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/proto/vega/snapshot/v1/__init__.py
+-rw-r--r--   0        0        0    56652 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/proto/vega/snapshot/v1/snapshot_pb2.py
+-rw-r--r--   0        0        0      158 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/proto/vega/snapshot/v1/snapshot_pb2_grpc.py
+-rw-r--r--   0        0        0    42924 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/proto/vega/vega_pb2.py
+-rw-r--r--   0        0        0      158 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/proto/vega/vega_pb2_grpc.py
+-rw-r--r--   0        0        0       35 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/proto/vega/wallet/__init__.py
+-rw-r--r--   0        0        0      128 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/proto/vega/wallet/v1/__init__.py
+-rw-r--r--   0        0        0     5154 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/proto/vega/wallet/v1/wallet_pb2.py
+-rw-r--r--   0        0        0      158 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/proto/vega/wallet/v1/wallet_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/quant/__init__.py
+-rw-r--r--   0        0        0     2961 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/quant/quant.py
+-rw-r--r--   0        0        0       29 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/.gitignore
+-rw-r--r--   0        0        0        0 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/agents/__init__.py
+-rw-r--r--   0        0        0     8048 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/agents/learning_agent.py
+-rw-r--r--   0        0        0    13440 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/agents/learning_agent_MO.py
+-rw-r--r--   0        0        0    18985 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/agents/learning_agent_MO_with_vol.py
+-rw-r--r--   0        0        0    13019 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/agents/learning_agent_heuristic.py
+-rw-r--r--   0        0        0     4754 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/agents/simple_agent.py
+-rw-r--r--   0        0        0      925 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/distributions.py
+-rw-r--r--   0        0        0        0 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/full_market_sim/__init__.py
+-rw-r--r--   0        0        0      608 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/full_market_sim/environments.py
+-rw-r--r--   0        0        0        0 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/full_market_sim/utils/__init__.py
+-rw-r--r--   0        0        0     4458 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/full_market_sim/utils/create_csv.py
+-rw-r--r--   0        0        0     1932 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/full_market_sim/utils/external_assetprice.py
+-rw-r--r--   0        0        0     4782 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/full_market_sim/utils/logdata.py
+-rw-r--r--   0        0        0     4809 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/full_market_sim/utils/strategy.py
+-rw-r--r--   0        0        0      662 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/helpers.py
+-rw-r--r--   0        0        0     3092 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/la_market_state.py
+-rw-r--r--   0        0        0     4243 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/networks.py
+-rw-r--r--   0        0        0     4015 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/plot.py
+-rw-r--r--   0        0        0     9642 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/run_rl_agent.py
+-rw-r--r--   0        0        0     2446 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/run_simple_agent.py
+-rw-r--r--   0        0        0      505 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/theory_intro/Bibliography.bib
+-rw-r--r--   0        0        0    13970 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/theory_intro/RL.tex
+-rw-r--r--   0        0        0    36669 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/theory_intro/images/RL.png
+-rw-r--r--   0        0        0    29521 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/theory_intro/images/RL_inv.png
+-rw-r--r--   0        0        0    39266 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/theory_intro/images/logo.png
+-rw-r--r--   0        0        0    52831 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/theory_intro/images/logo_inv.png
+-rw-r--r--   0        0        0        0 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/v2/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/v2/agents/__init__.py
+-rw-r--r--   0        0        0     3661 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/v2/agents/learning_agent.py
+-rw-r--r--   0        0        0    12222 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/v2/agents/learning_agent_MO.py
+-rw-r--r--   0        0        0     4442 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/v2/agents/puppets.py
+-rw-r--r--   0        0        0     5571 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/v2/learning_environment.py
+-rw-r--r--   0        0        0        0 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/v2/pettingzoo/__init__.py
+-rw-r--r--   0        0        0     8091 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/v2/pettingzoo/environment.py
+-rw-r--r--   0        0        0     4012 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/v2/pettingzoo/run.py
+-rw-r--r--   0        0        0     1641 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/v2/rewards.py
+-rw-r--r--   0        0        0     4365 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/v2/run.py
+-rw-r--r--   0        0        0        0 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/v2/stable_baselines/__init__.py
+-rw-r--r--   0        0        0     5547 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/v2/stable_baselines/environment.py
+-rw-r--r--   0        0        0      680 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/v2/stable_baselines/run.py
+-rw-r--r--   0        0        0      867 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/v2/stable_baselines/states.py
+-rw-r--r--   0        0        0     5070 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/reinforcement/v2/states.py
+-rw-r--r--   0        0        0        0 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/replay/__init__.py
+-rw-r--r--   0        0        0     1386 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/replay/replay.py
+-rw-r--r--   0        0        0        0 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/scenario/__init__.py
+-rw-r--r--   0        0        0     2260 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/scenario/adhoc.py
+-rw-r--r--   0        0        0        0 2023-07-13 15:30:06.263976 vega_sim-1.2.0/vega_sim/scenario/common/__init__.py
+-rw-r--r--   0        0        0   116585 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/common/agents.py
+-rw-r--r--   0        0        0     7797 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/common/utils/ideal_mm_models.py
+-rw-r--r--   0        0        0     6107 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/common/utils/price_process.py
+-rw-r--r--   0        0        0      779 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/comprehensive_market/agents.py
+-rw-r--r--   0        0        0    12572 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/comprehensive_market/scenario.py
+-rw-r--r--   0        0        0     5609 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/configurable_market/agents.py
+-rw-r--r--   0        0        0     9050 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/configurable_market/scenario.py
+-rw-r--r--   0        0        0      309 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/constants.py
+-rw-r--r--   0        0        0        0 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/curve_market_maker/__init__.py
+-rw-r--r--   0        0        0    11025 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/curve_market_maker/scenario.py
+-rw-r--r--   0        0        0    19699 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/fuzzed_markets/agents.py
+-rw-r--r--   0        0        0     3656 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/fuzzed_markets/run_capsule_test.py
+-rw-r--r--   0        0        0     2497 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/fuzzed_markets/run_fuzz_test.py
+-rw-r--r--   0        0        0    19014 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/fuzzed_markets/scenario.py
+-rw-r--r--   0        0        0        0 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/hedged_market_maker/__init__.py
+-rw-r--r--   0        0        0      827 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/hedged_market_maker/agents.py
+-rw-r--r--   0        0        0    18488 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/hedged_market_maker/scenario.py
+-rw-r--r--   0        0        0        0 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/ideal_market_maker/__init__.py
+-rw-r--r--   0        0        0    31515 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/ideal_market_maker/agents.py
+-rw-r--r--   0        0        0     3160 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/ideal_market_maker/environments.py
+-rw-r--r--   0        0        0     8680 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/ideal_market_maker/scenario.py
+-rw-r--r--   0        0        0        0 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/ideal_market_maker/utils/__init__.py
+-rw-r--r--   0        0        0     4782 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/ideal_market_maker/utils/log_data.py
+-rw-r--r--   0        0        0     4818 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/ideal_market_maker/utils/strategy.py
+-rw-r--r--   0        0        0        0 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/ideal_market_maker_v2/__init__.py
+-rw-r--r--   0        0        0    11478 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/ideal_market_maker_v2/agents.py
+-rw-r--r--   0        0        0     9525 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/ideal_market_maker_v2/scenario.py
+-rw-r--r--   0        0        0        0 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/ideal_market_maker_v2/utils/__init__.py
+-rw-r--r--   0        0        0     4818 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/ideal_market_maker_v2/utils/strategy.py
+-rw-r--r--   0        0        0     1687 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/market_crash/price_process.py
+-rw-r--r--   0        0        0     9288 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/market_crash/scenario.py
+-rw-r--r--   0        0        0     1948 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/multi_market/agents.py
+-rw-r--r--   0        0        0    20142 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/multi_market/scenario.py
+-rw-r--r--   0        0        0    10779 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/parameter_experiment/scenario.py
+-rw-r--r--   0        0        0        0 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/realtime_market/__init__.py
+-rw-r--r--   0        0        0     4646 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/realtime_market/scenario.py
+-rw-r--r--   0        0        0     7018 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/registry.py
+-rw-r--r--   0        0        0     4105 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/scenario/scenario.py
+-rw-r--r--   0        0        0    95509 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/service.py
+-rw-r--r--   0        0        0        0 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/tools/__init__.py
+-rw-r--r--   0        0        0     2038 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/tools/load_binaries.py
+-rw-r--r--   0        0        0    12360 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/tools/scenario_output.py
+-rw-r--r--   0        0        0    26331 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/tools/scenario_plots.py
+-rw-r--r--   0        0        0     3111 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/vegacapsule/config.hcl
+-rw-r--r--   0        0        0     3728 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/vegacapsule/genesis.tmpl
+-rw-r--r--   0        0        0        4 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/vegacapsule/passphrase-file
+-rw-r--r--   0        0        0     1606 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/vegacapsule/smart_contracts_addresses.json
+-rw-r--r--   0        0        0     1436 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/vegacapsule/templates/data_node_full.tmpl
+-rw-r--r--   0        0        0      965 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/vegacapsule/templates/tendermint_full.tmpl
+-rw-r--r--   0        0        0      965 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/vegacapsule/templates/tendermint_validators.tmpl
+-rw-r--r--   0        0        0     1920 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/vegacapsule/templates/vega_full.tmpl
+-rw-r--r--   0        0        0     1971 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/vegacapsule/templates/vega_validators.tmpl
+-rw-r--r--   0        0        0     2612 2023-07-13 15:30:06.267977 vega_sim-1.2.0/vega_sim/vegahome/config/data-node/config.toml
+-rw-r--r--   0        0        0      277 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/config/faucet/config.toml
+-rw-r--r--   0        0        0     3968 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/config/node/config.toml
+-rw-r--r--   0        0        0      312 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/config/node/wallets.encrypted
+-rw-r--r--   0        0        0      114 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/config/wallet-service/config.toml
+-rw-r--r--   0        0        0      321 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/config/wallet-service/networks/local.toml
+-rw-r--r--   0        0        0      586 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/faucet/wallets/vega.1639051237294446827
+-rw-r--r--   0        0        0      586 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/faucet/wallets/vega.1641976836892788243
+-rw-r--r--   0        0        0      586 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/faucet/wallets/vega.1641977214518086643
+-rw-r--r--   0        0        0      586 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/faucet/wallets/vega.1641977270881740938
+-rw-r--r--   0        0        0      586 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/faucet/wallets/vega.1641977376563008654
+-rw-r--r--   0        0        0      586 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/faucet/wallets/vega.1641977471442889253
+-rw-r--r--   0        0        0      586 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/faucet/wallets/vega.1641977537535784009
+-rw-r--r--   0        0        0      586 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/faucet/wallets/vega.1641977956797580358
+-rw-r--r--   0        0        0      586 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/faucet/wallets/vega.1641978034856367487
+-rw-r--r--   0        0        0      586 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/faucet/wallets/vega.1643100690865690276
+-rw-r--r--   0        0        0      491 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/node/wallets/ethereum/UTC--2021-12-09T12-00-28.751280926Z--b6ea7744971f455bbd754a97e8e05ea13dc1a033
+-rw-r--r--   0        0        0      491 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/node/wallets/ethereum/UTC--2022-01-12T08-54-28.446104867Z--d1b7ef68bb457b47837c6e81da24455be7a8be0d
+-rw-r--r--   0        0        0      491 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/node/wallets/ethereum/UTC--2022-01-12T08-57-18.522457076Z--dc699ecdab1705ebe83b60345060b6b7620263a3
+-rw-r--r--   0        0        0      491 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/node/wallets/ethereum/UTC--2022-01-12T08-58-36.643184436Z--760895ae7f813d685b048336fac88625441d6aa7
+-rw-r--r--   0        0        0      491 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/node/wallets/ethereum/UTC--2022-01-12T08-59-08.359696969Z--9e5beec6e56b28ccbd02864840b0f1e0125e42ce
+-rw-r--r--   0        0        0      586 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/node/wallets/vega/vega.1639051228296308758
+-rw-r--r--   0        0        0      586 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/node/wallets/vega/vega.1641977668033624243
+-rw-r--r--   0        0        0      586 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/node/wallets/vega/vega.1641977838095755067
+-rw-r--r--   0        0        0      586 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/node/wallets/vega/vega.1641977916225009082
+-rw-r--r--   0        0        0      586 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/node/wallets/vega/vega.1641977947934016124
+-rw-r--r--   0        0        0       46 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/priv_validator_state.json
+-rw-r--r--   0        0        0     3243 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/wallet-service/rsa-keys/private.pem
+-rw-r--r--   0        0        0      800 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/data/wallet-service/rsa-keys/public.pem
+-rw-r--r--   0        0        0     9044 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/genesis.json
+-rw-r--r--   0        0        0        3 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/vegahome/passphrase-file
+-rw-r--r--   0        0        0        0 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/wallet/__init__.py
+-rw-r--r--   0        0        0     1552 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/wallet/base.py
+-rw-r--r--   0        0        0     6855 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/wallet/slim_wallet.py
+-rw-r--r--   0        0        0     9442 2023-07-13 15:30:06.271977 vega_sim-1.2.0/vega_sim/wallet/vega_wallet.py
+-rw-r--r--   0        0        0     1649 1970-01-01 00:00:00.000000 vega_sim-1.2.0/PKG-INFO
```

### Comparing `vega_sim-1.1.1/LICENSE` & `vega_sim-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/pyproject.toml` & `vega_sim-1.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,64 @@
 [tool.poetry]
 name = "vega_sim"
 description = "Simulator for running self-contained Vega chain on local PC"
 authors = ["Tom McLean <tom@vegaprotocol.io>"]
 license = "MIT"
-version = "1.1.1"
+version = "1.2.0"
 
 [tool.setuptools]
 zip-safe = false
 
 [tool.poetry.dependencies]
-python = "^3.9,<3.11"
-requests = "^2.28.0"
-toml = "^0.10.2"
-grpcio-tools = "1.48.1"
-PyNaCl = "^1.5.0"
-inflection = "^0.5.1"
-scipy = "^1.8.1"
-pandas = "^1.4.2"
-numpy = "^1.22.4"
-torch = {version = "^1.12.1", optional = true}
-jupyterlab = {version = "^3.4.3", optional = true}
-jupyter = {version = "^1.0.0", optional = true}
-tqdm = {version = "^4.64.0", optional = true}
-matplotlib = {version = "^3.5.2", optional = true}
-snakeviz = {version = "^2.1.1", optional = true}
-pytest-profiling = {version = "^1.7.0", optional = true}
-ipywidgets = {version = "^7.7.1", optional = true}
-grpc-gateway-protoc-gen-openapiv2 = "^0.1.0"
-plotly = "^5.10.0"
-TA-Lib = {version = "^0.4.25", optional = true}
-python-dotenv = "^0.21.0"
-deprecated = "^1.2.13"
-gymnasium = {version = "^0.28.1", optional = true}
-sb3-contrib = {version = "^2.0.0a1", optional = true}
-stable-baselines3 = {version = "^2.0.0a1", optional = true }
-tensorboard = {version = "^2.12.2", optional = true}
+python = "^3.9,<3.12"
+requests = "*"
+toml = "*"
+grpcio-tools = "*"
+PyNaCl = "*"
+inflection = "*"
+scipy = "*"
+pandas = "*"
+numpy = "*"
+torch = {version = "*", optional = true}
+jupyterlab = {version = "*", optional = true}
+jupyter = {version = "*", optional = true}
+tqdm = {version = "*", optional = true}
+matplotlib = {version = "*", optional = true}
+snakeviz = {version = "*", optional = true}
+pytest-profiling = {version = "*", optional = true}
+ipywidgets = {version = "*", optional = true}
+protoc-gen-openapiv2 = "*"
+plotly = "*"
+TA-Lib = {version = "*", optional = true}
+python-dotenv = "*"
+deprecated = "*"
+psutil = "*"
+gymnasium = {version = "*", optional = true}
+sb3-contrib = {version = "*", optional = true}
+stable-baselines3 = {version = "*", optional = true }
+tensorboard = {version = "*", optional = true}
+pettingzoo = {version = "*", optional = true}
+numba = {version = "^0.57.1", optional = true}
+tianshou = {version = "*", optional = true}
+
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.1.0"
-pytest = "^7.1.2"
-requests-mock = "^1.9.3"
-flake8 = "^4.0.1"
-Jinja2 = "^3.1.2"
-nbmake = "^1.3.2"
-matplotlib = "^3.5.2"
-pytest-xdist = "^2.5.0"
+black = "*"
+pytest = "*"
+requests-mock = "*"
+flake8 = "*"
+Jinja2 = "*"
+nbmake = "*"
+matplotlib = "*"
+pytest-xdist = "*"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
+
+
 [tool.poetry.extras]
-learning = ["matplotlib", "tqdm", "torch", "gymnasium", "stable-baselines3", "tensorboard"]
+learning = ["matplotlib", "tqdm", "torch", "gymnasium", "stable-baselines3", "tensorboard", "tianshou", "numba", "pettingzoo"]
 jupyter = ["jupyterlab", "jupyter", "matplotlib", "ipywidgets"]
 profile = ["snakeviz", "pytest-profiling"]
 agents = ["TA-Lib"]
```

### Comparing `vega_sim-1.1.1/vega_sim/api/data.py` & `vega_sim-1.2.0/vega_sim/api/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -759,14 +759,15 @@
             + "please propose and create this market first"
         )
 
 
 def find_asset_id(
     symbol: str,
     data_client: vac.VegaTradingDataClientV2,
+    enabled: bool = True,
     raise_on_missing: bool = False,
 ) -> str:
     """Looks up the Asset ID of a given asset name
 
     Args:
         symbol:
             str, The symbol of the asset to look up
@@ -779,14 +780,16 @@
     Returns:
         str, the ID of the asset
     """
     assets = data_raw.list_assets(data_client=data_client)
     # Find settlement asset
     for asset in assets:
         if asset.details.symbol == symbol:
+            if (enabled) and (asset.status != vega_protos.assets.Asset.STATUS_ENABLED):
+                continue
             return asset.id
     if raise_on_missing:
         raise MissingAssetError(
             f"{symbol} asset not found on specified Vega network, "
             + "please propose and create this asset first"
         )
 
@@ -1166,20 +1169,24 @@
     data_client: vac.VegaTradingDataClientV2,
     market_id: str,
     party_id: Optional[str] = None,
     order_id: Optional[str] = None,
     market_price_decimals_map: Optional[Dict[str, int]] = None,
     market_position_decimals_map: Optional[Dict[str, int]] = None,
     market_asset_decimals_map: Optional[Dict[str, int]] = None,
+    start: Optional[datetime.datetime] = None,
+    end: Optional[datetime.datetime] = None,
 ) -> List[Trade]:
     base_trades = data_raw.get_trades(
         data_client=data_client,
         party_id=party_id,
         market_id=market_id,
         order_id=order_id,
+        start=start,
+        end=end,
     )
     market_price_decimals_map = market_price_decimals_map or {}
     market_position_decimals_map = market_position_decimals_map or {}
     market_asset_decimals_map = market_asset_decimals_map or {}
 
     res_trades = []
     for trade in base_trades:
@@ -1609,7 +1616,23 @@
     )
 
     converted_liquidation_estimate = _liquidation_estimate_from_proto(
         liquidation_estimate=liquidation_estimate,
     )
 
     return converted_margin_estimate, converted_liquidation_estimate
+
+
+def get_stake(
+    data_client: vac.trading_data_grpc_v2, party_id: str, asset_decimals: int
+):
+    return num_from_padded_int(
+        data_raw.get_stake(data_client=data_client, party_id=party_id),
+        decimals=asset_decimals,
+    )
+
+
+def get_asset(
+    data_client: vac.trading_data_grpc_v2,
+    asset_id: str,
+):
+    return data_raw.asset_info(data_client=data_client, asset_id=asset_id)
```

### Comparing `vega_sim-1.1.1/vega_sim/api/data_raw.py` & `vega_sim-1.2.0/vega_sim/api/data_raw.py`

 * *Files 1% similar despite different names*

```diff
@@ -412,20 +412,28 @@
 
 @_retry(3)
 def get_trades(
     data_client: vac.VegaTradingDataClientV2,
     market_id: str,
     party_id: Optional[str] = None,
     order_id: Optional[str] = None,
+    start: Optional[datetime.datetime] = None,
+    end: Optional[datetime.datetime] = None,
 ) -> List[vega_protos.vega.Trade]:
     return unroll_v2_pagination(
         data_node_protos_v2.trading_data.ListTradesRequest(
             market_ids=[market_id],
             party_ids=[party_id] if party_id is not None else None,
             order_ids=[order_id] if order_id is not None else None,
+            date_range=data_node_protos_v2.trading_data.DateRange(
+                start_timestamp=int(start.timestamp() * 1e9)
+                if start is not None
+                else None,
+                end_timestamp=int(end.timestamp() * 1e9) if end is not None else None,
+            ),
         ),
         request_func=lambda x: data_client.ListTrades(x).trades,
         extraction_func=lambda res: [i.node for i in res.edges],
     )
 
 
 @_retry(3)
@@ -656,7 +664,19 @@
         [base_request.orders.append(order) for order in orders]
     if collateral_available is not None:
         setattr(base_request, "collateral_available", collateral_available)
 
     response = data_client.EstimatePosition(base_request)
 
     return response.margin, response.liquidation
+
+
+def get_stake(data_client: vac.trading_data_grpc_v2, party_id: str = None):
+    base_request = data_node_protos_v2.trading_data.GetStakeRequest(party_id=party_id)
+    return data_client.GetStake(base_request).current_stake_available
+
+
+def list_all_network_history_segments(data_client: vac.trading_data_grpc_v2):
+    base_request = (
+        data_node_protos_v2.trading_data.ListAllNetworkHistorySegmentsRequest()
+    )
+    return data_client.ListAllNetworkHistorySegments(base_request).segments
```

### Comparing `vega_sim-1.1.1/vega_sim/api/faucet.py` & `vega_sim-1.2.0/vega_sim/api/faucet.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/api/governance.py` & `vega_sim-1.2.0/vega_sim/api/governance.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/api/helpers.py` & `vega_sim-1.2.0/vega_sim/api/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import string
 import time
 from typing import Any, Optional, TypeVar, Union, Callable
 
 import requests
 from vega_sim.grpc.client import VegaCoreClient, VegaTradingDataClientV2
 from vega_sim.proto.data_node.api.v2.trading_data_pb2 import GetVegaTimeRequest
+from vega_sim.proto.vega.api.v1.core_pb2 import StatisticsRequest
 
 
 T = TypeVar("T")
 
 TIME_FORWARD_URL = "{base_url}/api/v1/forwardtime"
 
 logger = logging.getLogger(__name__)
@@ -143,7 +144,11 @@
         vega_node_url:
             str, url for a Vega nullchain node
     """
     payload = {"forward": time}
 
     req = requests.post(TIME_FORWARD_URL.format(base_url=vega_node_url), json=payload)
     req.raise_for_status()
+
+
+def statistics(core_data_client: VegaCoreClient):
+    return core_data_client.Statistics(StatisticsRequest()).statistics
```

### Comparing `vega_sim-1.1.1/vega_sim/api/market.py` & `vega_sim-1.2.0/vega_sim/api/market.py`

 * *Files 10% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
     $ new_market_configuration_proto = market_config.build()
 
 """
 
 import functools
 import logging
-from typing import Optional
+from typing import Optional, Union
 
 import vega_sim.proto.vega as vega_protos
 import vega_sim.proto.vega.data.v1 as oracles_protos
 import vega_sim.proto.vega.data_source_pb2 as data_source_protos
 
 
 def rsetattr(obj, attr, val):
@@ -73,23 +73,33 @@
 
 class Config:
     OPTS = {}
 
     def __init__(self, opt: Optional[str] = None) -> None:
         self.load(opt=opt)
 
-    def load(self, opt: Optional[str] = None):
+    def load(self, opt: Optional[Union[dict, str]] = None) -> dict:
         if opt is None:
             opt = list(self.OPTS.keys())[0]
             logging.debug(f"No 'opt' arg given. Using default value '{opt}'.")
 
-        if opt not in self.OPTS:
-            raise ValueError(f"Invalid 'opt' arg '{opt}' specified.")
+        if isinstance(opt, str):
+            if opt not in self.OPTS:
+                raise ValueError(f"Invalid 'opt' arg '{opt}' specified.")
+            return self.OPTS[opt]
+
+        if isinstance(opt, dict):
+            defaults = self.OPTS["default"]
+            for key in defaults.keys():
+                if key not in opt.keys():
+                    opt[key] = defaults[key]
+            return opt
 
-        return opt
+        else:
+            raise TypeError(f"Invalid type '{type(opt)}' for arg 'opt'.")
 
 
 class MarketConfig(Config):
     OPTS = {
         "default": {
             "decimal_places": 4,
             "position_decimal_places": 2,
@@ -101,33 +111,31 @@
             "lp_price_range": 0.5,
             "linear_slippage_factor": 1e-3,
             "quadratic_slippage_factor": 0,
         }
     }
 
     def load(self, opt: Optional[str] = None):
-        opt = super().load(opt=opt)
+        config = super().load(opt=opt)
 
-        self.decimal_places = self.OPTS[opt]["decimal_places"]
-        self.position_decimal_places = self.OPTS[opt]["position_decimal_places"]
-        self.lp_price_range = str(self.OPTS[opt]["lp_price_range"])
-        self.linear_slippage_factor = str(self.OPTS[opt]["linear_slippage_factor"])
-        self.quadratic_slippage_factor = str(
-            self.OPTS[opt]["quadratic_slippage_factor"]
-        )
-        self.metadata = self.OPTS[opt]["metadata"]
+        self.decimal_places = config["decimal_places"]
+        self.position_decimal_places = config["position_decimal_places"]
+        self.lp_price_range = str(config["lp_price_range"])
+        self.linear_slippage_factor = str(config["linear_slippage_factor"])
+        self.quadratic_slippage_factor = str(config["quadratic_slippage_factor"])
+        self.metadata = config["metadata"]
 
-        self.instrument = InstrumentConfiguration(opt=self.OPTS[opt]["instrument"])
+        self.instrument = InstrumentConfiguration(opt=config["instrument"])
         self.price_monitoring_parameters = PriceMonitoringParameters(
-            opt=self.OPTS[opt]["price_monitoring_parameters"]
+            opt=config["price_monitoring_parameters"]
         )
         self.liquidity_monitoring_parameters = LiquidityMonitoringParameters(
-            opt=self.OPTS[opt]["liquidity_monitoring_parameters"]
+            opt=config["liquidity_monitoring_parameters"]
         )
-        self.log_normal = LogNormalRiskModel(opt=self.OPTS[opt]["log_normal"])
+        self.log_normal = LogNormalRiskModel(opt=config["log_normal"])
 
     def build(self):
         return vega_protos.governance.NewMarket(
             changes=vega_protos.governance.NewMarketConfiguration(
                 decimal_places=self.decimal_places,
                 position_decimal_places=self.position_decimal_places,
                 lp_price_range=self.lp_price_range,
@@ -143,41 +151,43 @@
 
     def set(self, parameter, value):
         rsetattr(self, attr=parameter, val=value)
 
 
 class PriceMonitoringParameters(Config):
     OPTS = {
-        "default": [
-            {
-                "horizon": 900,  # 15 minutes
-                "probability": "0.90001",
-                "auction_extension": 60,
-            },
-            {
-                "horizon": 3600,  # 1 hour
-                "probability": "0.90001",
-                "auction_extension": 300,
-            },
-            {
-                "horizon": 14_400,  # 4 hour
-                "probability": "0.90001",
-                "auction_extension": 900,
-            },
-            {
-                "horizon": 86_400,  # 1 day
-                "probability": "0.90001",
-                "auction_extension": 3600,
-            },
-        ]
+        "default": {
+            "triggers": [
+                {
+                    "horizon": 900,  # 15 minutes
+                    "probability": "0.90001",
+                    "auction_extension": 60,
+                },
+                {
+                    "horizon": 3600,  # 1 hour
+                    "probability": "0.90001",
+                    "auction_extension": 300,
+                },
+                {
+                    "horizon": 14_400,  # 4 hour
+                    "probability": "0.90001",
+                    "auction_extension": 900,
+                },
+                {
+                    "horizon": 86_400,  # 1 day
+                    "probability": "0.90001",
+                    "auction_extension": 3600,
+                },
+            ]
+        }
     }
 
     def load(self, opt: Optional[str] = None):
-        opt = super().load(opt=opt)
-        self.triggers = self.OPTS[opt]
+        config = super().load(opt=opt)
+        self.triggers = config["triggers"]
 
     def build(self):
         return vega_protos.markets.PriceMonitoringParameters(triggers=self.triggers)
 
 
 class LiquidityMonitoringParameters(Config):
     OPTS = {
@@ -185,21 +195,21 @@
             "triggering_ratio": "0.7",
             "auction_extension": 0,
             "target_stake_parameters": "default",
         }
     }
 
     def load(self, opt: Optional[str] = None):
-        opt = super().load(opt=opt)
+        config = super().load(opt=opt)
 
-        self.triggering_ratio = self.OPTS[opt]["triggering_ratio"]
-        self.auction_extension = self.OPTS[opt]["auction_extension"]
+        self.triggering_ratio = config["triggering_ratio"]
+        self.auction_extension = config["auction_extension"]
 
         self.target_stake_parameters = TargetStakeParameters(
-            opt=self.OPTS[opt]["target_stake_parameters"]
+            opt=config["target_stake_parameters"]
         )
 
     def build(self):
         return vega_protos.markets.LiquidityMonitoringParameters(
             triggering_ratio=self.triggering_ratio,
             auction_extension=self.auction_extension,
             target_stake_parameters=self.target_stake_parameters.build(),
@@ -211,18 +221,18 @@
         "default": {
             "time_window": 60 * 60,
             "scaling_factor": 1,
         }
     }
 
     def load(self, opt: Optional[str] = None):
-        opt = super().load(opt=opt)
+        config = super().load(opt=opt)
 
-        self.time_window = self.OPTS[opt]["time_window"]
-        self.scaling_factor = self.OPTS[opt]["scaling_factor"]
+        self.time_window = config["time_window"]
+        self.scaling_factor = config["scaling_factor"]
 
     def build(self):
         return vega_protos.markets.TargetStakeParameters(
             time_window=self.time_window,
             scaling_factor=self.scaling_factor,
         )
 
@@ -233,20 +243,20 @@
             "risk_aversion_parameter": 0.01,
             "tau": 1.90128526884173e-06,
             "params": "default",
         }
     }
 
     def load(self, opt: Optional[str] = None):
-        opt = super().load(opt=opt)
+        config = super().load(opt=opt)
 
-        self.risk_aversion_parameter = self.OPTS[opt]["risk_aversion_parameter"]
-        self.tau = self.OPTS[opt]["tau"]
+        self.risk_aversion_parameter = config["risk_aversion_parameter"]
+        self.tau = config["tau"]
 
-        self.params = LogNormalModelParams(opt=self.OPTS[opt]["params"])
+        self.params = LogNormalModelParams(opt=config["params"])
 
     def build(self):
         return vega_protos.markets.LogNormalRiskModel(
             risk_aversion_parameter=self.risk_aversion_parameter,
             tau=self.tau,
             params=self.params.build(),
         )
@@ -261,19 +271,19 @@
         }
     }
 
     def __init__(self, opt: Optional[str] = None) -> None:
         super().__init__(opt)
 
     def load(self, opt: Optional[str] = None):
-        opt = super().load(opt=opt)
+        config = super().load(opt=opt)
 
-        self.mu = self.OPTS[opt]["mu"]
-        self.r = self.OPTS[opt]["r"]
-        self.sigma = self.OPTS[opt]["sigma"]
+        self.mu = config["mu"]
+        self.r = config["r"]
+        self.sigma = config["sigma"]
 
     def build(self):
         return vega_protos.markets.LogNormalModelParams(
             mu=self.mu,
             r=self.r,
             sigma=self.sigma,
         )
@@ -285,19 +295,19 @@
             "name": None,
             "code": None,
             "future": "default",
         }
     }
 
     def load(self, opt: Optional[str] = None):
-        opt = super().load(opt=opt)
+        config = super().load(opt=opt)
 
-        self.name = self.OPTS[opt]["name"]
-        self.code = self.OPTS[opt]["code"]
-        self.future = FutureProduct(opt=self.OPTS[opt]["future"])
+        self.name = config["name"]
+        self.code = config["code"]
+        self.future = FutureProduct(opt=config["future"])
 
     def build(self):
         return vega_protos.governance.InstrumentConfiguration(
             name=self.name, code=self.code, future=self.future.build()
         )
 
 
@@ -307,37 +317,29 @@
             "settlement_asset": None,
             "quote_name": None,
             "number_decimal_places": None,
             "terminating_key": None,
         }
     }
 
-    def load(self, opt: Optional[str] = None):
-        opt = super().load(opt=opt)
+    def load(self, opt: Optional[Union[dict, str]] = None):
+        config = super().load(opt=opt)
 
-        self.settlement_asset = self.OPTS[opt]["settlement_asset"]
-        self.quote_name = self.OPTS[opt]["quote_name"]
-        self.number_decimal_places = self.OPTS[opt]["number_decimal_places"]
-        self.terminating_key = self.OPTS[opt]["terminating_key"]
+        self.settlement_asset = config["settlement_asset"]
+        self.quote_name = config["quote_name"]
+        self.number_decimal_places = config["number_decimal_places"]
+        self.terminating_key = config["terminating_key"]
 
     def build(self):
         if None in [
             self.settlement_asset,
             self.quote_name,
             self.number_decimal_places,
             self.terminating_key,
         ]:
-            print(
-                [
-                    self.settlement_asset,
-                    self.quote_name,
-                    self.number_decimal_places,
-                    self.terminating_key,
-                ]
-            )
             raise ValueError(
                 "MarketConfig has not been updated with settlement asset information."
             )
 
         data_source_spec_for_settlement_data = data_source_protos.DataSourceDefinition(
             external=data_source_protos.DataSourceDefinitionExternal(
                 oracle=data_source_protos.DataSourceSpecConfiguration(
```

### Comparing `vega_sim-1.1.1/vega_sim/api/trading.py` & `vega_sim-1.2.0/vega_sim/api/trading.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,15 +236,15 @@
     logger.debug(f"Submitted Order amendment for {order_id}.")
 
 
 def cancel_order(
     wallet_name: str,
     wallet: Wallet,
     market_id: str,
-    order_id: str,
+    order_id: Optional[str],
     key_name: Optional[str] = None,
 ):
     """
     Cancel Order
 
     Args:
         wallet_name:
@@ -644,32 +644,33 @@
         f"Submitted a batch of {len(cancellations)} cancellation,"
         f" {len(amendments)} amendment, and {len(submissions)} submission instructions."
     )
 
 
 def transfer(
     wallet: Wallet,
-    wallet_name: str,
     key_name: str,
     from_account_type: vega_protos.vega.AccountType,
     to: str,
     to_account_type: vega_protos.vega.AccountType,
     asset: str,
     amount: str,
     reference: Optional[str] = None,
     one_off: Optional[vega_protos.commands.v1.commands.OneOffTransfer] = None,
     recurring: Optional[vega_protos.commands.v1.commands.RecurringTransfer] = None,
+    wallet_name: Optional[str] = None,
 ):
     command = vega_protos.commands.v1.commands.Transfer(
         from_account_type=from_account_type,
-        to=to,
         to_account_type=to_account_type,
         asset=asset,
         amount=amount,
     )
+    if to is not None:
+        setattr(command, "to", to)
 
     if reference is not None:
         setattr(command, "reference", reference)
 
     if (one_off is not None) and (recurring is not None):
         raise ValueError("Both 'one_off' and 'recurring' cannot be specified")
```

### Comparing `vega_sim-1.1.1/vega_sim/devops/README.md` & `vega_sim-1.2.0/vega_sim/devops/README.md`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/devops/classes.py` & `vega_sim-1.2.0/vega_sim/devops/classes.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/devops/registry.py` & `vega_sim-1.2.0/vega_sim/devops/registry.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/devops/run_agent.py` & `vega_sim-1.2.0/vega_sim/devops/run_agent.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/devops/run_scenario.py` & `vega_sim-1.2.0/vega_sim/devops/run_scenario.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/devops/scenario.py` & `vega_sim-1.2.0/vega_sim/devops/scenario.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/devops/wallet.py` & `vega_sim-1.2.0/vega_sim/devops/wallet.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/environment/agent.py` & `vega_sim-1.2.0/vega_sim/environment/agent.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 from abc import ABC
 from dataclasses import dataclass
-from typing import Any, Tuple, Dict, Optional, List
+from typing import Any, Tuple, Dict, Optional, List, Union
 
-from vega_sim.service import VegaService
+from vega_sim.null_service import VegaServiceNull
+from vega_sim.network_service import VegaServiceNetwork
 
 
 @dataclass
 class VegaState:
     network_state: Tuple
     market_state: Dict[str, Any]
 
 
 class Agent(ABC):
     NAME_BASE = "base_agent"
 
     def __init__(self, tag: Optional[str] = None):
         self.tag = tag
 
-    def step(self, vega: VegaService):
+    def step(self, vega: Union[VegaServiceNull, VegaServiceNetwork]):
         pass
 
     def initialise(
-        self, vega: VegaService, create_key: bool = False, mint_key: bool = False
+        self,
+        vega: Union[VegaServiceNull, VegaServiceNetwork],
+        create_key: bool = False,
+        mint_key: bool = False,
     ):
         self.vega = vega
 
     def finalise(self):
         pass
 
     def _update_state(self, current_step: int):
@@ -70,15 +74,17 @@
         self.key_name = key_name
 
         self.state_update_freq = state_update_freq
 
     def step(self):
         pass
 
-    def initialise(self, vega: VegaService, create_key: bool = True):
+    def initialise(
+        self, vega: Union[VegaServiceNull, VegaServiceNetwork], create_key: bool = True
+    ):
         super().initialise(vega=vega)
         if create_key:
             self.vega.create_key(
                 wallet_name=self.wallet_name,
                 name=self.key_name,
             )
             self._public_key = vega.wallet.public_key(
```

### Comparing `vega_sim-1.1.1/vega_sim/environment/environment.py` & `vega_sim-1.2.0/vega_sim/environment/environment.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         n_steps: int,
         random_agent_ordering: bool = True,
         transactions_per_block: int = 1,
         block_length_seconds: int = 1,
         step_length_seconds: Optional[int] = None,
         vega_service: Optional[VegaServiceNull] = None,
         pause_every_n_steps: Optional[int] = None,
-        random_state: np.random.RandomState = None,
+        random_state: Optional[np.random.RandomState] = None,
     ):
         """Set up a Vega protocol environment with some specified agents.
         Handles the entire Vega setup and environment lifetime process, allowing the
         user to focus on building the Agents themselves.
 
         Once an environment has been created, calling the 'run' function will
         run a complete simulation of the environment lifecycle then shut down
@@ -163,21 +163,24 @@
                 self._vega,
                 pause_at_completion=pause_at_completion,
                 log_every_n_steps=log_every_n_steps,
             )
 
     def _start_live_feeds(self, vega: VegaService):
         # Get lists of unique market_ids and party_ids to observe
-        market_ids = list(
-            {
-                vega.find_market_id(name=agent.market_name)
+
+        market_ids = [
+            vega.find_market_id(market_name)
+            for market_name in {
+                agent.market_name
                 for agent in self.agents
                 if hasattr(agent, "market_name")
             }
-        )
+        ]
+
         party_ids = list(
             {
                 vega.wallet.public_key(
                     wallet_name=agent.wallet_name, name=agent.key_name
                 )
                 for agent in self.agents
                 if hasattr(agent, "key_name")
@@ -421,14 +424,16 @@
         step_length_seconds: int = 5,
         random_agent_ordering: bool = True,
         vega_service: Optional[VegaServiceNetwork] = None,
         state_func: Optional[Callable[[VegaService], VegaState]] = None,
         raise_datanode_errors: Optional[bool] = True,
         raise_step_errors: Optional[bool] = True,
         random_state: np.random.RandomState = None,
+        create_keys: Optional[bool] = False,
+        mint_keys: Optional[bool] = False,
     ):
         super().__init__(
             agents=agents,
             n_steps=n_steps,
             random_agent_ordering=random_agent_ordering,
             step_length_seconds=step_length_seconds,
             vega_service=vega_service,
@@ -437,14 +442,17 @@
         self.state_func = (
             state_func if state_func is not None else self._default_state_extraction
         )
 
         self.raise_datanode_errors = raise_datanode_errors
         self.raise_step_errors = raise_step_errors
 
+        self.create_keys = create_keys
+        self.mint_keys = mint_keys
+
     def run(
         self,
         run_with_console: bool = False,
         pause_at_completion: bool = False,
         log_every_n_steps: Optional[int] = None,
     ):
         if self._vega is None:
@@ -468,15 +476,17 @@
         log_every_n_steps: Optional[int] = None,
     ) -> None:
         # Initial datanode connection check
         vega.check_datanode(raise_on_error=self.raise_datanode_errors)
 
         # Initialise agents without minting assets
         for agent in self.agents:
-            agent.initialise(vega=vega, create_key=False, mint_key=False)
+            agent.initialise(
+                vega=vega, create_key=self.create_keys, mint_key=self.mint_keys
+            )
 
         self._start_live_feeds(vega=vega)
 
         i = 0
         # A negative self.n_steps will loop indefinitely
         while i != self.n_steps:
             t_start = time.time()
@@ -494,16 +504,22 @@
                     f"Environment step, {round(t_elapsed,2)}s, taking longer than"
                     f" defined scenario step length, {self.step_length_seconds}s,"
                 )
             if log_every_n_steps is not None and i % log_every_n_steps == 0:
                 logger.info(f"Completed {i} steps")
 
         for agent in self.agents:
-            agent.finalise()
-
+            try:
+                agent.finalise()
+            except Exception as e:
+                msg = f"Agent '{agent.key_name}' failed to step. Error: {e}"
+                if self.raise_step_errors:
+                    raise (e)
+                else:
+                    logging.warning(msg)
         if pause_at_completion:
             input(
                 "Environment run completed. Pausing to allow inspection of state."
                 " Press Enter to continue"
             )
 
     def step(self, vega: VegaServiceNetwork) -> None:
@@ -514,15 +530,15 @@
             sorted(self.agents, key=lambda _: self.random_state.random())
             if self.random_agent_ordering
             else self.agents
         ):
             try:
                 agent.step(state)
             except Exception as e:
-                msg = f"Agent '{agent.key_name}' failed to step. Error: {e}"
+                msg = f"Agent '{agent.name()}' failed to step. Error: {e}"
                 if self.raise_step_errors:
                     raise e(msg)
                 else:
                     logging.warning(msg)
 
 
 class RealtimeMarketEnvironment(MarketEnvironmentWithState):
```

### Comparing `vega_sim-1.1.1/vega_sim/grpc/client.py` & `vega_sim-1.2.0/vega_sim/grpc/client.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/local_data_cache.py` & `vega_sim-1.2.0/vega_sim/local_data_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
                 Any,
             ],
         ]
     ],
     sink: Queue[Any],
     market_id: Optional[str] = None,
     party_id: Optional[str] = None,
+    kill_thread_sig: Optional[threading.Event()] = None,
 ) -> None:
     obs = data_raw.observe_event_bus(
         data_client=data_client,
         type=list(chain(*[ev[0] for ev in stream_registry])),
         market_id=market_id,
         party_id=party_id,
     )
@@ -49,14 +50,16 @@
     handlers = {}
     for evts, handler in stream_registry:
         for evt in evts:
             handlers[evt] = handler
     try:
         for o in obs:
             for event in o.events:
+                if (kill_thread_sig is not None) and kill_thread_sig.is_set():
+                    return
                 output = handlers[event.type](event)
                 if isinstance(output, (list, GeneratorType)):
                     for elem in output:
                         sink.put(elem)
                 else:
                     sink.put(output)
     except grpc._channel._MultiThreadedRendezvous as e:
@@ -306,14 +309,15 @@
                     else None
                 ),
                 (
                     (party_ids[0] if len(party_ids) == 1 else None)
                     if party_ids is not None
                     else None
                 ),
+                self._kill_thread_sig,
             ),
             daemon=True,
         )
         self._forwarding_thread.start()
 
     def initialise_assets(self):
         base_assets = data_raw.list_assets(data_client=self._trading_data_client)
```

### Comparing `vega_sim-1.1.1/vega_sim/network_service.py` & `vega_sim-1.2.0/vega_sim/network_service.py`

 * *Files 25% similar despite different names*

```diff
@@ -55,14 +55,16 @@
 from vega_sim.wallet.base import Wallet
 from vega_sim.wallet.vega_wallet import VegaWallet
 from vega_sim.null_service import find_free_port, _popen_process
 
 from vega_sim.constants import DATA_NODE_GRPC_PORT
 from vega_sim.scenario.constants import Network
 
+from vega_sim.api.helpers import num_to_padded_int, num_from_padded_int
+
 logger = logging.getLogger(__name__)
 
 
 class VegaWalletStartupTimeoutError(Exception):
     pass
 
 
@@ -214,15 +216,24 @@
         network: Network,
         run_with_wallet: bool = True,
         run_with_console: bool = True,
         vega_console_path: Optional[str] = None,
         network_config_path: Optional[str] = None,
         wallet_path: Optional[str] = None,
         vega_home_path: Optional[str] = None,
+        wallet_home_path: Optional[str] = None,
         wallet_token_path: Optional[str] = None,
+        wallet_passphrase_path: Optional[str] = None,
+        wallet_url: Optional[bool] = None,
+        faucet_url: Optional[bool] = None,
+        vega_node_grpc_url: Optional[str] = None,
+        load_existing_keys: Optional[bool] = None,
+        governance_symbol: Optional[str] = "VEGA",
+        vegacapsule_bin_path: Optional[str] = "./vega_sim/bin/vegacapsule",
+        network_on_host: Optional[bool] = False,
     ):
         """Method initialises the class.
 
         Args:
             network (Network):
                 Defines which network to connect service to.
             run_with_wallet (bool, optional):
@@ -243,24 +254,32 @@
                 Note: Only needed if creating keys
             wallet_token_path (str, optional):
                 Path to the json file containing wallet tokens. Otherwise
                 uses VEGA_WALLET_TOKENS_FILE environment variable.
         """
 
         # Run init method inherited from VegaService with network arguments.
-        super().__init__(can_control_time=False, warn_on_raw_data_access=False)
+        super().__init__(
+            can_control_time=False,
+            warn_on_raw_data_access=False,
+            governance_symbol=governance_symbol,
+        )
 
         self.network = network
         self.run_with_wallet = run_with_wallet
         self.run_with_console = run_with_console
 
         self._wallet = None
-        self._wallet_url = None
         self._data_node_grpc_url = None
         self._data_node_query_url = None
+        self._data_node_rest_url = None
+
+        self._wallet_url = wallet_url
+        self._faucet_url = faucet_url
+
         self._network_config = None
 
         self.vega_console_path = (
             vega_console_path
             if vega_console_path is not None
             else path.join(vega_bin_path, "console")
         )
@@ -275,36 +294,78 @@
             if wallet_path is not None
             else environ.get("VEGA_WALLET_PATH", "vegawallet")
         )
 
         self._vega_home = (
             vega_home_path if vega_home_path is not None else environ.get("VEGA_HOME")
         )
+        self._wallet_home = (
+            wallet_home_path
+            if wallet_home_path is not None
+            else environ.get("WALLET_HOME")
+        )
+        self._passphrase_file_path = wallet_passphrase_path
 
         self._token_path = (
             wallet_token_path
             if wallet_token_path is not None
             else environ.get("VEGA_WALLET_TOKENS_FILE")
         )
-        if self._token_path is None:
-            raise Exception(
-                "Either path to tokens JSON must be passed to wallet class or"
-                " VEGA_WALLET_TOKENS_FILE environment variable set"
-            )
 
         self._network_config_path = _find_network_config_toml(
             network=self.network, config_path=self._base_network_config_path
         )
         if self._network_config_path is None:
             raise ValueError(
                 f"ERROR! {self.network.name.lower()} network config could not be found"
             )
+        self._grpc_endpoints = itertools.cycle(
+            self.network_config["API"]["GRPC"]["Hosts"]
+        )
+        self._rest_endpoints = itertools.cycle(
+            self.network_config["API"]["REST"]["Hosts"]
+        )
+        self._graphql_endpoints = itertools.cycle(
+            self.network_config["API"]["GraphQL"]["Hosts"]
+        )
+
+        self.load_existing_keys = load_existing_keys
+        self.vegacapsule_bin_path = vegacapsule_bin_path
 
         self.log_dir = tempfile.mkdtemp(prefix="vega-sim-")
 
+        self._vega_node_grpc_url = vega_node_grpc_url
+
+        if network_on_host:
+            logging.info(
+                "Network running on host machine. Updating url to use host.docker.internal"
+            )
+
+            def update_endpoint(endpoint, http: bool = True):
+                return (
+                    ("http://" if http else "")
+                    + "host.docker.internal:"
+                    + endpoint.split(":")[-1]
+                )
+
+            def update_iterator(iterator, http: bool = True):
+                for endpoint in iterator:
+                    yield update_endpoint(endpoint, http)
+
+            self._grpc_endpoints = update_iterator(self._grpc_endpoints, http=False)
+            self._rest_endpoints = update_iterator(self._rest_endpoints)
+            self._graphql_endpoints = update_iterator(self._graphql_endpoints)
+            self._wallet_url = update_endpoint(self._wallet_url)
+            self._faucet_url = update_endpoint(self._faucet_url)
+
+            if self._vega_node_grpc_url is not None:
+                self._vega_node_grpc_url = update_endpoint(
+                    self._vega_node_grpc_url, http=False
+                )
+
     def __enter__(self):
         """Defines behaviour when class entered by a with statement."""
         self.start()
 
         return self
 
     def __exit__(self, type, value, traceback):
@@ -352,19 +413,19 @@
             raise VegaWalletStartupTimeoutError(
                 "Timed out waiting for Vega wallet service"
             )
 
         self.check_datanode(raise_on_error=False)
 
     def stop(self) -> None:
-        super().stop()
         if self.proc is None:
             logger.info("Stop called but nothing to stop")
         else:
             self.proc.terminate()
+        super().stop()
 
     def wait_fn(self, wait_multiple: float = 1) -> None:
         """Overrides redundant parent method."""
         logging.debug(
             "Parent method overridden as VegaNetworkService incapable of controlling"
             " time."
         )
@@ -390,68 +451,84 @@
             " time."
         )
 
     @property
     def network_config(self) -> dict:
         if self._network_config is None:
             self._network_config = toml.load(self._network_config_path)
-            add_network_config(self._network_config_path)
+            if self.run_with_wallet:
+                add_network_config(self._network_config_path)
         return self._network_config
 
     @property
     def data_node_grpc_url(self) -> str:
         if self._data_node_grpc_url is None:
-            url = self.network_config["API"]["GRPC"]["Hosts"][0]
-            self._data_node_grpc_url = f"{url.split(':')[0]}:{DATA_NODE_GRPC_PORT}"
+            self._data_node_grpc_url = next(self._grpc_endpoints)
         return self._data_node_grpc_url
 
     @property
+    def data_node_rest_url(self) -> str:
+        if self._data_node_rest_url is None:
+            self._data_node_rest_url = next(self._rest_endpoints)
+        return self._data_node_rest_url
+
+    @property
     def data_node_query_url(self) -> str:
         if self._data_node_query_url is None:
-            url = self.network_config["API"]["GraphQL"]["Hosts"][0]
-            self._data_node_query_url = url
+            self._data_node_query_url = next(self._graphql_endpoints)
         return self._data_node_query_url
 
     @property
+    def vega_node_grpc_url(self) -> str:
+        return self._vega_node_grpc_url
+
+    @property
     def wallet_url(self) -> str:
         if self._wallet_url is None:
             self._wallet_url = f"http://127.0.0.1:1789"
         return self._wallet_url
 
     @property
+    def faucet_url(self) -> str:
+        return self._faucet_url
+
+    @property
     def wallet(self) -> Wallet:
         if self._wallet is None:
-            self._wallet = VegaWallet.from_json(
-                self._token_path,
-                self.wallet_url,
-                wallet_path=self._wallet_path,
-                vega_home_dir=self._vega_home,
-            )
+            if self.load_existing_keys:
+                if self._token_path is None:
+                    raise Exception(
+                        "Either path to tokens JSON must be passed to wallet class or"
+                        " VEGA_WALLET_TOKENS_FILE environment variable set"
+                    )
+                self._wallet = VegaWallet.from_json(
+                    self._token_path,
+                    self.wallet_url,
+                    wallet_path=self._wallet_path,
+                    vega_home_dir=self._vega_home,
+                )
+            else:
+                self._wallet = VegaWallet(
+                    wallet_url=self.wallet_url,
+                    wallet_path=self._wallet_path,
+                    vega_home_dir=self._wallet_home,
+                    passphrase_file_path=self._passphrase_file_path,
+                )
         return self._wallet
 
     @property
     def core_state_client(self) -> None:
         logging.debug(
             (
                 "Parent property overridden as VegaNetworkService does not need a core"
                 " client."
             ),
         )
         pass
 
-    @property
-    def core_client(self) -> None:
-        logging.debug(
-            (
-                "Parent property overridden as VegaNetworkService does not need a core"
-                " client."
-            ),
-        )
-        pass
-
     def check_datanode(
         self, max_time_diff: int = 30, raise_on_error: Optional[bool] = True
     ):
         """Checks if the current data-node connection is healthy.
 
         If the current data-node connection has timed out or the end-point is
         unresponsive then the service will attempt to establish a connection
@@ -514,19 +591,19 @@
         Args:
             max_attempts (int, optional):
                 Maximum number of connection attempts to attempt before raising an
                 error. Defaults to -1 (infinite attempts).
         """
 
         attempts = 0
-        for url in itertools.cycle(self.network_config["API"]["GRPC"]["Hosts"]):
+        while True:
             attempts += 1
 
             try:
-                self._data_node_grpc_url = f"{url.split(':')[0]}:{DATA_NODE_GRPC_PORT}"
+                self._data_node_grpc_url = next(self._grpc_endpoints)
 
                 logging.debug(f"Switched to endpoint {self._data_node_grpc_url}")
 
                 channel = grpc.insecure_channel(
                     self.data_node_grpc_url,
                     options=(
                         ("grpc.enable_http_proxy", 0),
@@ -539,44 +616,187 @@
                     self.data_node_grpc_url,
                     channel=channel,
                 )
 
                 # Ping the datanode to check it is not behind
                 self.ping_datanode()
                 logging.debug(
-                    f"Connection to endpoint {self._data_node_grpc_url} successful."
+                    f"Connection to endpoint {self.data_node_grpc_url} successful."
                 )
 
                 return
 
             except grpc._channel._InactiveRpcError:
                 logging.warning(
-                    f"Connection to endpoint {self._data_node_grpc_url} inactive."
+                    f"Connection to endpoint {self.data_node_grpc_url} inactive."
                 )
 
             except grpc.FutureTimeoutError:
                 logging.warning(
-                    f"Connection to endpoint {self._data_node_grpc_url} timed out."
+                    f"Connection to endpoint {self.data_node_grpc_url} timed out."
                 )
 
             except DatanodeBehindError:
                 logging.warning(
-                    f"Connection to endpoint {self._data_node_grpc_url} is behind."
+                    f"Connection to endpoint {self.data_node_grpc_url} is behind."
                 )
 
             except DatanodeSlowResponseError:
                 logging.warning(
-                    f"Connection to endpoint {self._data_node_grpc_url} is slow."
+                    f"Connection to endpoint {self.data_node_grpc_url} is slow."
                 )
 
             if attempts == max_attempts:
                 break
 
         raise Exception("Unable to establish connection to a data-node.")
 
+    def mint(
+        self,
+        key_name: Optional[str],
+        asset: str,
+        amount: float,
+        wallet_name: Optional[str] = None,
+    ) -> None:
+        """Mints a given amount of requested asset into the associated wallet
+
+        Args:
+            wallet_name:
+                str, The name of the wallet
+            asset:
+                str, The ID of the asset to mint
+            amount:
+                float, the amount of asset to mint
+            key_name:
+                Optional[str], key name stored in metadata. Defaults to None.
+        """
+        details = self.get_asset(asset).details
+        is_erc20 = True if details.erc20.contract_address != "" else False
+
+        if is_erc20:
+            self.deposit(
+                symbol=details.symbol,
+                amount=amount,
+                key_name=key_name,
+                wallet_name=wallet_name,
+            )
+        else:
+            max_faucet_amount = num_from_padded_int(
+                details.builtin_asset.max_faucet_amount_mint, details.decimals
+            )
+            super().mint(
+                key_name=key_name,
+                asset=asset,
+                amount=amount if amount < max_faucet_amount else max_faucet_amount,
+                wallet_name=wallet_name,
+            )
+
+    def deposit(
+        self,
+        symbol: str,
+        amount: float,
+        key_name: str,
+        wallet_name: Optional[str] = None,
+    ):
+        """Deposit an amount of a specified ERC20 asset to a a vega key.
+
+        Args:
+            symbol (str): Symbol of the asset to be deposited.
+            amount (float): Amount to be deposited.
+            key_name (str): Name of the key used for the deposit.
+            wallet_name (Optional[str], optional): Name of the wallet. Defaults to the
+                default wallet_name set in the wallet.
+
+        Raises:
+            Exception: Raised if the deposit does not arrive within a fixed time limit.
+        """
+
+        asset_id = self.find_asset_id(symbol=symbol)
+        amount = str(
+            num_to_padded_int(
+                amount,
+                self.asset_decimals[asset_id],
+            )
+        )
+
+        pub_key = self.wallet.public_key(name=key_name, wallet_name=wallet_name)
+        account_before = self.party_account(party_id=pub_key, asset_id=asset_id).general
+
+        args = [
+            self.vegacapsule_bin,
+            "ethereum",
+            "asset",
+            "deposit",
+            "--asset-symbol",
+            symbol,
+            "--amount",
+            amount,
+            "--pubkey",
+            pub_key,
+        ]
+        subprocess.run(args)
+
+        for _ in range(500):
+            if self.party_account(party_id=pub_key, asset_id=asset_id) > account_before:
+                return
+            self.wait_fn(1)
+        raise Exception("Deposit never arrived.")
+
+    def stake(
+        self,
+        amount: float,
+        key_name: str,
+        wallet_name: Optional[str] = None,
+    ):
+        """Stake a specified amount of a governance asset.
+
+        Args:
+            amount (float): The amount to stake.
+            key_name (str): The name of the key used for staking.
+            wallet_name (Optional[str], optional): The name of the wallet. Defaults to
+                the default value set in the wallet.
+
+        Raises:
+            Exception: Raised if the stake does not arrive within a given time limit.
+        """
+        amount = str(
+            num_to_padded_int(
+                amount,
+                self.asset_decimals[self.find_asset_id(symbol=self.governance_symbol)],
+            )
+        )
+
+        pub_key = self.wallet.public_key(name=key_name, wallet_name=wallet_name)
+        stake_before = self.get_stake(party_id=pub_key)
+
+        args = [
+            self.vegacapsule_bin_path,
+            "ethereum",
+            "asset",
+            "stake",
+            "--amount",
+            amount,
+            "--asset-symbol",
+            self.governance_symbol,
+            "--pub-key",
+            pub_key,
+            "--home-path",
+            self._vega_home,
+        ]
+        subprocess.run(args)
+
+        for _ in range(500):
+            if self.get_stake(party_id=pub_key) > stake_before:
+                return
+            self.wait_fn(1)
+        raise Exception("Stake never arrived.")
+
+    def wait_fn(self, wait_multiple: float = 1) -> None:
+        time.sleep(wait_multiple)
+
 
 if __name__ == "__main__":
     """Module Example"""
 
     log = logging.basicConfig(level=logging.INFO)
 
     # Create a service connected to the fairground network.
```

### Comparing `vega_sim-1.1.1/vega_sim/null_service.py` & `vega_sim-1.2.0/vega_sim/null_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -308,14 +308,15 @@
             elem[config.key] = config.val_func(port_config[port_key])
 
             with open(file_path, "w") as f:
                 toml.dump(config_toml, f)
 
 
 def manage_vega_processes(
+    child_conn: multiprocessing.Pipe,
     vega_path: str,
     data_node_path: str,
     vega_wallet_path: str,
     vega_console_path: Optional[str] = None,
     run_with_console: bool = False,
     port_config: Optional[Dict[Ports, int]] = None,
     transactions_per_block: int = 1,
@@ -420,15 +421,19 @@
 
     vegaNodeProcess = _popen_process(
         vega_args,
         dir_root=tmp_vega_dir,
         log_name="node",
     )
 
-    processes = [dataNodeProcess, vegaFaucetProcess, vegaNodeProcess]
+    processes = {
+        "data-node": dataNodeProcess,
+        "faucet": vegaFaucetProcess,
+        "vega": vegaNodeProcess,
+    }
 
     if run_wallet:
         for _ in range(3000):
             try:
                 requests.get(
                     f"http://localhost:{port_config.get(Ports.DATA_NODE_REST)}/time"
                 ).raise_for_status()
@@ -497,15 +502,15 @@
         ]
 
         vegaWalletProcess = _popen_process(
             wallet_args,
             dir_root=tmp_vega_dir,
             log_name="vegawallet",
         )
-        processes.append(vegaWalletProcess)
+        processes["wallet"] = vegaWalletProcess
 
     if run_with_console:
         env_copy = os.environ.copy()
         env_copy.update(
             {
                 "NX_VEGA_URL": (
                     f"http://localhost:{port_config[Ports.DATA_NODE_REST]}/graphql"
@@ -529,21 +534,23 @@
                 "-o",
                 "trading",
             ],
             dir_root=tmp_vega_dir,
             log_name="console",
             env=env_copy,
         )
-        processes.append(console_process)
+        processes["console"] = console_process
+
+    # Send process pid values for resource monitoring
+    child_conn.send({name: process.pid for name, process in processes.items()})
 
     signal.sigwait([signal.SIGKILL, signal.SIGTERM])
-    for process in processes:
+    for process in processes.values():
         process.terminate()
-    for process in processes:
-        name = psutil.Process(process.pid).name()
+    for name, process in processes.items():
         attempts = 0
         while process.poll() is None:
             time.sleep(1)
             attempts += 1
             if attempts > 60:
                 logging.warning(
                     f"Gracefully terminating process timed-out. Killing process {name}."
@@ -624,19 +631,15 @@
 
         self.log_dir = tempfile.mkdtemp(prefix="vega-sim-")
 
         self.launch_graphql = launch_graphql
         self.replay_from_path = replay_from_path
         self.check_for_binaries = check_for_binaries
 
-        if port_config is None:
-            self._assign_ports()
-        else:
-            for key, name in self.PORT_TO_FIELD_MAP.items():
-                setattr(self, name, port_config[key])
+        self._assign_ports(port_config)
 
         if start_immediately:
             self.start()
 
     def __enter__(self):
         self.start()
         return self
@@ -665,30 +668,14 @@
                 self._wallet = SlimWallet(
                     self.core_client,
                     full_wallet=None,
                     log_dir=self.log_dir,
                 )
         return self._wallet
 
-    def _assign_ports(self):
-        self.wallet_port = 0
-        self.data_node_rest_port = 0
-        self.data_node_grpc_port = 0
-        self.data_node_postgres_port = 0
-        self.faucet_port = 0
-        self.vega_node_port = 0
-        self.vega_node_grpc_port = 0
-        self.vega_node_rest_port = 0
-        self.console_port = 0
-        for port_opt in self.PORT_TO_FIELD_MAP.values():
-            curr_ports = set(
-                [getattr(self, port) for port in self.PORT_TO_FIELD_MAP.values()]
-            )
-            setattr(self, port_opt, find_free_port(curr_ports))
-
     def _check_started(self) -> None:
         if self.proc is None:
             raise ServiceNotStartedError("NullChain Vega accessed without starting")
 
     def _generate_port_config(self) -> Dict[Ports, int]:
         return {
             Ports.WALLET: self.wallet_port,
@@ -698,23 +685,46 @@
             Ports.FAUCET: self.faucet_port,
             Ports.VEGA_NODE: self.vega_node_port,
             Ports.CORE_GRPC: self.vega_node_grpc_port,
             Ports.CORE_REST: self.vega_node_rest_port,
             Ports.CONSOLE: self.console_port,
         }
 
+    # set ports from port_config or alternatively find a free port
+    # to use
+    def _assign_ports(self, port_config: Optional[Dict[Ports, int]]):
+        self.wallet_port = 0
+        self.data_node_rest_port = 0
+        self.data_node_grpc_port = 0
+        self.data_node_postgres_port = 0
+        self.faucet_port = 0
+        self.vega_node_port = 0
+        self.vega_node_grpc_port = 0
+        self.vega_node_rest_port = 0
+        self.console_port = 0
+
+        for key, name in self.PORT_TO_FIELD_MAP.items():
+            if port_config is not None and key in port_config:
+                setattr(self, name, port_config[key])
+            else:
+                curr_ports = set(
+                    [getattr(self, port) for port in self.PORT_TO_FIELD_MAP.values()]
+                )
+                setattr(self, name, find_free_port(curr_ports))
+
     def start(self, block_on_startup: bool = True) -> None:
         if self.check_for_binaries and not self._using_all_custom_paths:
             download_binaries()
-
+        parent_conn, child_conn = multiprocessing.Pipe()
         ctx = multiprocessing.get_context()
         port_config = self._generate_port_config()
         self.proc = ctx.Process(
             target=manage_vega_processes,
             kwargs={
+                "child_conn": child_conn,
                 "vega_path": self.vega_path,
                 "data_node_path": self.data_node_path,
                 "vega_wallet_path": self.vega_wallet_path,
                 "vega_console_path": self.vega_console_path,
                 "run_with_console": self.run_with_console,
                 "port_config": port_config,
                 "transactions_per_block": self.transactions_per_block,
@@ -777,14 +787,16 @@
                     time.sleep(0.1)
             if not started:
                 self.stop()
                 raise VegaStartupTimeoutError(
                     "Timed out waiting for Vega simulator to start up"
                 )
 
+            self.process_pids = parent_conn.recv()
+
             # Create a block before waiting for datanode sync and starting the feeds
             self.wait_fn(1)
             self.wait_for_total_catchup()
             self.wait_for_thread_catchup()
             self.data_cache
 
         if self.run_with_console:
```

### Comparing `vega_sim-1.1.1/vega_sim/parameter_test/parameter/configs.py` & `vega_sim-1.2.0/vega_sim/parameter_test/parameter/configs.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/parameter_test/parameter/experiment.py` & `vega_sim-1.2.0/vega_sim/parameter_test/parameter/experiment.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/parameter_test/parameter/loggers.py` & `vega_sim-1.2.0/vega_sim/parameter_test/parameter/loggers.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/parameter_test/run.py` & `vega_sim-1.2.0/vega_sim/parameter_test/run.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/proto/blockexplorer/api/v1/blockexplorer_pb2.py` & `vega_sim-1.2.0/vega_sim/proto/blockexplorer/api/v1/blockexplorer_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: blockexplorer/api/v1/blockexplorer.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
@@ -21,40 +21,41 @@
 )
 from vega.commands.v1 import (
     transaction_pb2 as vega_dot_commands_dot_v1_dot_transaction__pb2,
 )
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n(blockexplorer/api/v1/blockexplorer.proto\x12\x14\x62lockexplorer.api.v1\x1a\x1fgoogle/api/field_behavior.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\x1a vega/commands/v1/signature.proto\x1a"vega/commands/v1/transaction.proto"\r\n\x0bInfoRequest"I\n\x0cInfoResponse\x12\x18\n\x07version\x18\x01 \x01(\tR\x07version\x12\x1f\n\x0b\x63ommit_hash\x18\x02 \x01(\tR\ncommitHash"0\n\x15GetTransactionRequest\x12\x17\n\x04hash\x18\x01 \x01(\tB\x03\xe0\x41\x02R\x04hash"]\n\x16GetTransactionResponse\x12\x43\n\x0btransaction\x18\x01 \x01(\x0b\x32!.blockexplorer.api.v1.TransactionR\x0btransaction"\x8e\x02\n\x17ListTransactionsRequest\x12\x14\n\x05limit\x18\x01 \x01(\rR\x05limit\x12\x1b\n\x06\x62\x65\x66ore\x18\x02 \x01(\tH\x00R\x06\x62\x65\x66ore\x88\x01\x01\x12\x19\n\x05\x61\x66ter\x18\x03 \x01(\tH\x01R\x05\x61\x66ter\x88\x01\x01\x12T\n\x07\x66ilters\x18\x04 \x03(\x0b\x32:.blockexplorer.api.v1.ListTransactionsRequest.FiltersEntryR\x07\x66ilters\x1a:\n\x0c\x46iltersEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x42\t\n\x07_beforeB\x08\n\x06_after"a\n\x18ListTransactionsResponse\x12\x45\n\x0ctransactions\x18\x03 \x03(\x0b\x32!.blockexplorer.api.v1.TransactionR\x0ctransactions"\xc2\x02\n\x0bTransaction\x12\x14\n\x05\x62lock\x18\x01 \x01(\x04R\x05\x62lock\x12\x14\n\x05index\x18\x02 \x01(\rR\x05index\x12\x12\n\x04hash\x18\x03 \x01(\tR\x04hash\x12\x1c\n\tsubmitter\x18\x04 \x01(\tR\tsubmitter\x12\x12\n\x04type\x18\x05 \x01(\tR\x04type\x12\x12\n\x04\x63ode\x18\x06 \x01(\rR\x04\x63ode\x12\x16\n\x06\x63ursor\x18\x07 \x01(\tR\x06\x63ursor\x12\x35\n\x07\x63ommand\x18\x08 \x01(\x0b\x32\x1b.vega.commands.v1.InputDataR\x07\x63ommand\x12\x39\n\tsignature\x18\t \x01(\x0b\x32\x1b.vega.commands.v1.SignatureR\tsignature\x12\x19\n\x05\x65rror\x18\n \x01(\tH\x00R\x05\x65rror\x88\x01\x01\x42\x08\n\x06_error2\xc9\x02\n\x14\x42lockExplorerService\x12m\n\x0eGetTransaction\x12+.blockexplorer.api.v1.GetTransactionRequest\x1a,.blockexplorer.api.v1.GetTransactionResponse"\x00\x12s\n\x10ListTransactions\x12-.blockexplorer.api.v1.ListTransactionsRequest\x1a..blockexplorer.api.v1.ListTransactionsResponse"\x00\x12M\n\x04Info\x12!.blockexplorer.api.v1.InfoRequest\x1a".blockexplorer.api.v1.InfoResponseBxZ5code.vegaprotocol.io/vega/protos/blockexplorer/api/v1\x92\x41>\x12#\n\x18Vega block explorer APIs2\x07v0.71.4\x1a\x13lb.testnet.vega.xyz*\x02\x01\x02\x62\x06proto3'
+    b'\n(blockexplorer/api/v1/blockexplorer.proto\x12\x14\x62lockexplorer.api.v1\x1a\x1fgoogle/api/field_behavior.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\x1a vega/commands/v1/signature.proto\x1a"vega/commands/v1/transaction.proto"\r\n\x0bInfoRequest"I\n\x0cInfoResponse\x12\x18\n\x07version\x18\x01 \x01(\tR\x07version\x12\x1f\n\x0b\x63ommit_hash\x18\x02 \x01(\tR\ncommitHash"1\n\x15GetTransactionRequest\x12\x18\n\x04hash\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x04hash"]\n\x16GetTransactionResponse\x12\x43\n\x0btransaction\x18\x01 \x01(\x0b\x32!.blockexplorer.api.v1.TransactionR\x0btransaction"\xf1\x02\n\x17ListTransactionsRequest\x12\x14\n\x05limit\x18\x01 \x01(\rR\x05limit\x12\x1b\n\x06\x62\x65\x66ore\x18\x02 \x01(\tH\x00R\x06\x62\x65\x66ore\x88\x01\x01\x12\x19\n\x05\x61\x66ter\x18\x03 \x01(\tH\x01R\x05\x61\x66ter\x88\x01\x01\x12T\n\x07\x66ilters\x18\x04 \x03(\x0b\x32:.blockexplorer.api.v1.ListTransactionsRequest.FiltersEntryR\x07\x66ilters\x12\x1b\n\tcmd_types\x18\x05 \x03(\tR\x08\x63mdTypes\x12*\n\x11\x65xclude_cmd_types\x18\x06 \x03(\tR\x0f\x65xcludeCmdTypes\x12\x18\n\x07parties\x18\x07 \x03(\tR\x07parties\x1a:\n\x0c\x46iltersEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x42\t\n\x07_beforeB\x08\n\x06_after"a\n\x18ListTransactionsResponse\x12\x45\n\x0ctransactions\x18\x03 \x03(\x0b\x32!.blockexplorer.api.v1.TransactionR\x0ctransactions"\xc2\x02\n\x0bTransaction\x12\x14\n\x05\x62lock\x18\x01 \x01(\x04R\x05\x62lock\x12\x14\n\x05index\x18\x02 \x01(\rR\x05index\x12\x12\n\x04hash\x18\x03 \x01(\tR\x04hash\x12\x1c\n\tsubmitter\x18\x04 \x01(\tR\tsubmitter\x12\x12\n\x04type\x18\x05 \x01(\tR\x04type\x12\x12\n\x04\x63ode\x18\x06 \x01(\rR\x04\x63ode\x12\x16\n\x06\x63ursor\x18\x07 \x01(\tR\x06\x63ursor\x12\x35\n\x07\x63ommand\x18\x08 \x01(\x0b\x32\x1b.vega.commands.v1.InputDataR\x07\x63ommand\x12\x39\n\tsignature\x18\t \x01(\x0b\x32\x1b.vega.commands.v1.SignatureR\tsignature\x12\x19\n\x05\x65rror\x18\n \x01(\tH\x00R\x05\x65rror\x88\x01\x01\x42\x08\n\x06_error2\xc9\x02\n\x14\x42lockExplorerService\x12m\n\x0eGetTransaction\x12+.blockexplorer.api.v1.GetTransactionRequest\x1a,.blockexplorer.api.v1.GetTransactionResponse"\x00\x12s\n\x10ListTransactions\x12-.blockexplorer.api.v1.ListTransactionsRequest\x1a..blockexplorer.api.v1.ListTransactionsResponse"\x00\x12M\n\x04Info\x12!.blockexplorer.api.v1.InfoRequest\x1a".blockexplorer.api.v1.InfoResponseBxZ5code.vegaprotocol.io/vega/protos/blockexplorer/api/v1\x92\x41>\x12#\n\x18Vega block explorer APIs2\x07v0.71.0\x1a\x13lb.testnet.vega.xyz*\x02\x01\x02\x62\x06proto3'
 )
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(
-    DESCRIPTOR, "blockexplorer.api.v1.blockexplorer_pb2", globals()
+    DESCRIPTOR, "blockexplorer.api.v1.blockexplorer_pb2", _globals
 )
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    DESCRIPTOR._serialized_options = b"Z5code.vegaprotocol.io/vega/protos/blockexplorer/api/v1\222A>\022#\n\030Vega block explorer APIs2\007v0.71.4\032\023lb.testnet.vega.xyz*\002\001\002"
+    DESCRIPTOR._serialized_options = b"Z5code.vegaprotocol.io/vega/protos/blockexplorer/api/v1\222A>\022#\n\030Vega block explorer APIs2\007v0.71.0\032\023lb.testnet.vega.xyz*\002\001\002"
     _GETTRANSACTIONREQUEST.fields_by_name["hash"]._options = None
-    _GETTRANSACTIONREQUEST.fields_by_name["hash"]._serialized_options = b"\340A\002"
+    _GETTRANSACTIONREQUEST.fields_by_name["hash"]._serialized_options = b"\342A\001\002"
     _LISTTRANSACTIONSREQUEST_FILTERSENTRY._options = None
     _LISTTRANSACTIONSREQUEST_FILTERSENTRY._serialized_options = b"8\001"
-    _INFOREQUEST._serialized_start = 217
-    _INFOREQUEST._serialized_end = 230
-    _INFORESPONSE._serialized_start = 232
-    _INFORESPONSE._serialized_end = 305
-    _GETTRANSACTIONREQUEST._serialized_start = 307
-    _GETTRANSACTIONREQUEST._serialized_end = 355
-    _GETTRANSACTIONRESPONSE._serialized_start = 357
-    _GETTRANSACTIONRESPONSE._serialized_end = 450
-    _LISTTRANSACTIONSREQUEST._serialized_start = 453
-    _LISTTRANSACTIONSREQUEST._serialized_end = 723
-    _LISTTRANSACTIONSREQUEST_FILTERSENTRY._serialized_start = 644
-    _LISTTRANSACTIONSREQUEST_FILTERSENTRY._serialized_end = 702
-    _LISTTRANSACTIONSRESPONSE._serialized_start = 725
-    _LISTTRANSACTIONSRESPONSE._serialized_end = 822
-    _TRANSACTION._serialized_start = 825
-    _TRANSACTION._serialized_end = 1147
-    _BLOCKEXPLORERSERVICE._serialized_start = 1150
-    _BLOCKEXPLORERSERVICE._serialized_end = 1479
+    _globals["_INFOREQUEST"]._serialized_start = 217
+    _globals["_INFOREQUEST"]._serialized_end = 230
+    _globals["_INFORESPONSE"]._serialized_start = 232
+    _globals["_INFORESPONSE"]._serialized_end = 305
+    _globals["_GETTRANSACTIONREQUEST"]._serialized_start = 307
+    _globals["_GETTRANSACTIONREQUEST"]._serialized_end = 356
+    _globals["_GETTRANSACTIONRESPONSE"]._serialized_start = 358
+    _globals["_GETTRANSACTIONRESPONSE"]._serialized_end = 451
+    _globals["_LISTTRANSACTIONSREQUEST"]._serialized_start = 454
+    _globals["_LISTTRANSACTIONSREQUEST"]._serialized_end = 823
+    _globals["_LISTTRANSACTIONSREQUEST_FILTERSENTRY"]._serialized_start = 744
+    _globals["_LISTTRANSACTIONSREQUEST_FILTERSENTRY"]._serialized_end = 802
+    _globals["_LISTTRANSACTIONSRESPONSE"]._serialized_start = 825
+    _globals["_LISTTRANSACTIONSRESPONSE"]._serialized_end = 922
+    _globals["_TRANSACTION"]._serialized_start = 925
+    _globals["_TRANSACTION"]._serialized_end = 1247
+    _globals["_BLOCKEXPLORERSERVICE"]._serialized_start = 1250
+    _globals["_BLOCKEXPLORERSERVICE"]._serialized_end = 1579
 # @@protoc_insertion_point(module_scope)
```

### Comparing `vega_sim-1.1.1/vega_sim/proto/blockexplorer/api/v1/blockexplorer_pb2_grpc.py` & `vega_sim-1.2.0/vega_sim/proto/blockexplorer/api/v1/blockexplorer_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/proto/data_node/api/v2/trading_data_pb2.py` & `vega_sim-1.2.0/vega_sim/proto/data_node/api/v2/trading_data_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: data-node/api/v2/trading_data.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
@@ -25,142 +25,159 @@
 from ....vega import governance_pb2 as vega_dot_governance__pb2
 from ....vega import markets_pb2 as vega_dot_markets__pb2
 from ....vega import oracle_pb2 as vega_dot_oracle__pb2
 from ....vega import vega_pb2 as vega_dot_vega__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n#data-node/api/v2/trading_data.proto\x12\x0f\x64\x61tanode.api.v2\x1a\x1fgoogle/api/field_behavior.proto\x1a\x19google/api/httpbody.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\x1a\x11vega/assets.proto\x1a)vega/commands/v1/validator_commands.proto\x1a\x1bvega/events/v1/events.proto\x1a\x15vega/governance.proto\x1a\x12vega/markets.proto\x1a\x11vega/oracle.proto\x1a\x0fvega/vega.proto"\xd9\x01\n\nPagination\x12\x19\n\x05\x66irst\x18\x01 \x01(\x05H\x00R\x05\x66irst\x88\x01\x01\x12\x19\n\x05\x61\x66ter\x18\x02 \x01(\tH\x01R\x05\x61\x66ter\x88\x01\x01\x12\x17\n\x04last\x18\x03 \x01(\x05H\x02R\x04last\x88\x01\x01\x12\x1b\n\x06\x62\x65\x66ore\x18\x04 \x01(\tH\x03R\x06\x62\x65\x66ore\x88\x01\x01\x12&\n\x0cnewest_first\x18\x05 \x01(\x08H\x04R\x0bnewestFirst\x88\x01\x01\x42\x08\n\x06_firstB\x08\n\x06_afterB\x07\n\x05_lastB\t\n\x07_beforeB\x0f\n\r_newest_first"\x9c\x01\n\x08PageInfo\x12"\n\rhas_next_page\x18\x01 \x01(\x08R\x0bhasNextPage\x12*\n\x11has_previous_page\x18\x02 \x01(\x08R\x0fhasPreviousPage\x12!\n\x0cstart_cursor\x18\x03 \x01(\tR\x0bstartCursor\x12\x1d\n\nend_cursor\x18\x04 \x01(\tR\tendCursor"\x9a\x01\n\x0e\x41\x63\x63ountBalance\x12\x14\n\x05owner\x18\x02 \x01(\tR\x05owner\x12\x18\n\x07\x62\x61lance\x18\x03 \x01(\tR\x07\x62\x61lance\x12\x14\n\x05\x61sset\x18\x04 \x01(\tR\x05\x61sset\x12\x1b\n\tmarket_id\x18\x05 \x01(\tR\x08marketId\x12%\n\x04type\x18\x06 \x01(\x0e\x32\x11.vega.AccountTypeR\x04type"\x9e\x01\n\x13ListAccountsRequest\x12\x36\n\x06\x66ilter\x18\x01 \x01(\x0b\x32\x1e.datanode.api.v2.AccountFilterR\x06\x66ilter\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"W\n\x14ListAccountsResponse\x12?\n\x08\x61\x63\x63ounts\x18\x01 \x01(\x0b\x32#.datanode.api.v2.AccountsConnectionR\x08\x61\x63\x63ounts"\x80\x01\n\x12\x41\x63\x63ountsConnection\x12\x32\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1c.datanode.api.v2.AccountEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"Z\n\x0b\x41\x63\x63ountEdge\x12\x33\n\x04node\x18\x01 \x01(\x0b\x32\x1f.datanode.api.v2.AccountBalanceR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x8d\x01\n\x16ObserveAccountsRequest\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x14\n\x05\x61sset\x18\x03 \x01(\tR\x05\x61sset\x12%\n\x04type\x18\x04 \x01(\x0e\x32\x11.vega.AccountTypeR\x04type"\xa6\x01\n\x17ObserveAccountsResponse\x12\x42\n\x08snapshot\x18\x01 \x01(\x0b\x32$.datanode.api.v2.AccountSnapshotPageH\x00R\x08snapshot\x12;\n\x07updates\x18\x02 \x01(\x0b\x32\x1f.datanode.api.v2.AccountUpdatesH\x00R\x07updatesB\n\n\x08response"o\n\x13\x41\x63\x63ountSnapshotPage\x12;\n\x08\x61\x63\x63ounts\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.AccountBalanceR\x08\x61\x63\x63ounts\x12\x1b\n\tlast_page\x18\x02 \x01(\x08R\x08lastPage"M\n\x0e\x41\x63\x63ountUpdates\x12;\n\x08\x61\x63\x63ounts\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.AccountBalanceR\x08\x61\x63\x63ounts"\r\n\x0bInfoRequest"I\n\x0cInfoResponse\x12\x18\n\x07version\x18\x01 \x01(\tR\x07version\x12\x1f\n\x0b\x63ommit_hash\x18\x02 \x01(\tR\ncommitHash"\\\n\x0fGetOrderRequest\x12\x1e\n\x08order_id\x18\x01 \x01(\tB\x03\xe0\x41\x02R\x07orderId\x12\x1d\n\x07version\x18\x02 \x01(\x05H\x00R\x07version\x88\x01\x01\x42\n\n\x08_version"5\n\x10GetOrderResponse\x12!\n\x05order\x18\x01 \x01(\x0b\x32\x0b.vega.OrderR\x05order"\xbd\x03\n\x0bOrderFilter\x12.\n\x08statuses\x18\x01 \x03(\x0e\x32\x12.vega.Order.StatusR\x08statuses\x12&\n\x05types\x18\x02 \x03(\x0e\x32\x10.vega.Order.TypeR\x05types\x12=\n\x0etime_in_forces\x18\x03 \x03(\x0e\x32\x17.vega.Order.TimeInForceR\x0ctimeInForces\x12+\n\x11\x65xclude_liquidity\x18\x04 \x01(\x08R\x10\x65xcludeLiquidity\x12\x1b\n\tparty_ids\x18\x05 \x03(\tR\x08partyIds\x12\x1d\n\nmarket_ids\x18\x06 \x03(\tR\tmarketIds\x12!\n\treference\x18\x07 \x01(\tH\x00R\treference\x88\x01\x01\x12>\n\ndate_range\x18\x08 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x01R\tdateRange\x88\x01\x01\x12 \n\tlive_only\x18\t \x01(\x08H\x02R\x08liveOnly\x88\x01\x01\x42\x0c\n\n_referenceB\r\n\x0b_date_rangeB\x0c\n\n_live_only"\xaa\x01\n\x11ListOrdersRequest\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12\x39\n\x06\x66ilter\x18\x05 \x01(\x0b\x32\x1c.datanode.api.v2.OrderFilterH\x01R\x06\x66ilter\x88\x01\x01\x42\r\n\x0b_paginationB\t\n\x07_filter"N\n\x12ListOrdersResponse\x12\x38\n\x06orders\x18\x01 \x01(\x0b\x32 .datanode.api.v2.OrderConnectionR\x06orders"\x8b\x01\n\x18ListOrderVersionsRequest\x12\x1e\n\x08order_id\x18\x01 \x01(\tB\x03\xe0\x41\x02R\x07orderId\x12@\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"U\n\x19ListOrderVersionsResponse\x12\x38\n\x06orders\x18\x01 \x01(\x0b\x32 .datanode.api.v2.OrderConnectionR\x06orders"\x9a\x01\n\x14ObserveOrdersRequest\x12\x1d\n\nmarket_ids\x18\x01 \x03(\tR\tmarketIds\x12\x1b\n\tparty_ids\x18\x02 \x03(\tR\x08partyIds\x12\x30\n\x11\x65xclude_liquidity\x18\x03 \x01(\x08H\x00R\x10\x65xcludeLiquidity\x88\x01\x01\x42\x14\n\x12_exclude_liquidity"\xa0\x01\n\x15ObserveOrdersResponse\x12@\n\x08snapshot\x18\x01 \x01(\x0b\x32".datanode.api.v2.OrderSnapshotPageH\x00R\x08snapshot\x12\x39\n\x07updates\x18\x02 \x01(\x0b\x32\x1d.datanode.api.v2.OrderUpdatesH\x00R\x07updatesB\n\n\x08response"U\n\x11OrderSnapshotPage\x12#\n\x06orders\x18\x01 \x03(\x0b\x32\x0b.vega.OrderR\x06orders\x12\x1b\n\tlast_page\x18\x02 \x01(\x08R\x08lastPage"3\n\x0cOrderUpdates\x12#\n\x06orders\x18\x01 \x03(\x0b\x32\x0b.vega.OrderR\x06orders"\xa3\x01\n\x14ListPositionsRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01:\x02\x18\x01\x42\r\n\x0b_pagination"^\n\x15ListPositionsResponse\x12\x41\n\tpositions\x18\x01 \x01(\x0b\x32#.datanode.api.v2.PositionConnectionR\tpositions:\x02\x18\x01"M\n\x0fPositionsFilter\x12\x1b\n\tparty_ids\x18\x01 \x03(\tR\x08partyIds\x12\x1d\n\nmarket_ids\x18\x02 \x03(\tR\tmarketIds"\xa4\x01\n\x17ListAllPositionsRequest\x12\x38\n\x06\x66ilter\x18\x01 \x01(\x0b\x32 .datanode.api.v2.PositionsFilterR\x06\x66ilter\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"]\n\x18ListAllPositionsResponse\x12\x41\n\tpositions\x18\x01 \x01(\x0b\x32#.datanode.api.v2.PositionConnectionR\tpositions"J\n\x0cPositionEdge\x12"\n\x04node\x18\x01 \x01(\x0b\x32\x0e.vega.PositionR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x81\x01\n\x12PositionConnection\x12\x33\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1d.datanode.api.v2.PositionEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"v\n\x17ObservePositionsRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12 \n\tmarket_id\x18\x02 \x01(\tH\x01R\x08marketId\x88\x01\x01\x42\x0b\n\t_party_idB\x0c\n\n_market_id"\xa9\x01\n\x18ObservePositionsResponse\x12\x43\n\x08snapshot\x18\x01 \x01(\x0b\x32%.datanode.api.v2.PositionSnapshotPageH\x00R\x08snapshot\x12<\n\x07updates\x18\x02 \x01(\x0b\x32 .datanode.api.v2.PositionUpdatesH\x00R\x07updatesB\n\n\x08response"a\n\x14PositionSnapshotPage\x12,\n\tpositions\x18\x01 \x03(\x0b\x32\x0e.vega.PositionR\tpositions\x12\x1b\n\tlast_page\x18\x02 \x01(\x08R\x08lastPage"?\n\x0fPositionUpdates\x12,\n\tpositions\x18\x01 \x03(\x0b\x32\x0e.vega.PositionR\tpositions"\xa3\x02\n\x11LedgerEntryFilter\x12\x37\n\x18\x63lose_on_account_filters\x18\x01 \x01(\x08R\x15\x63loseOnAccountFilters\x12N\n\x13\x66rom_account_filter\x18\x02 \x01(\x0b\x32\x1e.datanode.api.v2.AccountFilterR\x11\x66romAccountFilter\x12J\n\x11to_account_filter\x18\x03 \x01(\x0b\x32\x1e.datanode.api.v2.AccountFilterR\x0ftoAccountFilter\x12\x39\n\x0etransfer_types\x18\x05 \x03(\x0e\x32\x12.vega.TransferTypeR\rtransferTypes"\xd9\x05\n\x15\x41ggregatedLedgerEntry\x12\x1c\n\ttimestamp\x18\x02 \x01(\x03R\ttimestamp\x12\x1a\n\x08quantity\x18\x03 \x01(\tR\x08quantity\x12\x37\n\rtransfer_type\x18\x04 \x01(\x0e\x32\x12.vega.TransferTypeR\x0ctransferType\x12\x1e\n\x08\x61sset_id\x18\x05 \x01(\tH\x00R\x07\x61ssetId\x88\x01\x01\x12=\n\x11\x66rom_account_type\x18\x06 \x01(\x0e\x32\x11.vega.AccountTypeR\x0f\x66romAccountType\x12\x39\n\x0fto_account_type\x18\x07 \x01(\x0e\x32\x11.vega.AccountTypeR\rtoAccountType\x12\x36\n\x15\x66rom_account_party_id\x18\x08 \x01(\tH\x01R\x12\x66romAccountPartyId\x88\x01\x01\x12\x32\n\x13to_account_party_id\x18\t \x01(\tH\x02R\x10toAccountPartyId\x88\x01\x01\x12\x38\n\x16\x66rom_account_market_id\x18\n \x01(\tH\x03R\x13\x66romAccountMarketId\x88\x01\x01\x12\x34\n\x14to_account_market_id\x18\x0b \x01(\tH\x04R\x11toAccountMarketId\x88\x01\x01\x12\x30\n\x14\x66rom_account_balance\x18\x0c \x01(\tR\x12\x66romAccountBalance\x12,\n\x12to_account_balance\x18\r \x01(\tR\x10toAccountBalanceB\x0b\n\t_asset_idB\x18\n\x16_from_account_party_idB\x16\n\x14_to_account_party_idB\x19\n\x17_from_account_market_idB\x17\n\x15_to_account_market_idJ\x04\x08\x01\x10\x02"\xf6\x01\n\x18ListLedgerEntriesRequest\x12:\n\x06\x66ilter\x18\x01 \x01(\x0b\x32".datanode.api.v2.LedgerEntryFilterR\x06\x66ilter\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12>\n\ndate_range\x18\x03 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x01R\tdateRange\x88\x01\x01\x42\r\n\x0b_paginationB\r\n\x0b_date_range"\xab\x01\n\x1a\x45xportLedgerEntriesRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tB\x03\xe0\x41\x02R\x07partyId\x12\x1e\n\x08\x61sset_id\x18\x02 \x01(\tB\x03\xe0\x41\x02R\x07\x61ssetId\x12>\n\ndate_range\x18\x04 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x00R\tdateRange\x88\x01\x01\x42\r\n\x0b_date_range"v\n\x19ListLedgerEntriesResponse\x12Y\n\x0eledger_entries\x18\x01 \x01(\x0b\x32\x32.datanode.api.v2.AggregatedLedgerEntriesConnectionR\rledgerEntries"q\n\x1b\x41ggregatedLedgerEntriesEdge\x12:\n\x04node\x18\x01 \x01(\x0b\x32&.datanode.api.v2.AggregatedLedgerEntryR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x9f\x01\n!AggregatedLedgerEntriesConnection\x12\x42\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32,.datanode.api.v2.AggregatedLedgerEntriesEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xf3\x01\n\x19ListBalanceChangesRequest\x12\x36\n\x06\x66ilter\x18\x01 \x01(\x0b\x32\x1e.datanode.api.v2.AccountFilterR\x06\x66ilter\x12@\n\npagination\x18\x05 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12>\n\ndate_range\x18\x06 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x01R\tdateRange\x88\x01\x01\x42\r\n\x0b_paginationB\r\n\x0b_date_range"f\n\x1aListBalanceChangesResponse\x12H\n\x08\x62\x61lances\x18\x01 \x01(\x0b\x32,.datanode.api.v2.AggregatedBalanceConnectionR\x08\x62\x61lances"\xac\x02\n\x18GetBalanceHistoryRequest\x12\x36\n\x06\x66ilter\x18\x01 \x01(\x0b\x32\x1e.datanode.api.v2.AccountFilterR\x06\x66ilter\x12\x38\n\x08group_by\x18\x02 \x03(\x0e\x32\x1d.datanode.api.v2.AccountFieldR\x07groupBy\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12>\n\ndate_range\x18\x04 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x01R\tdateRange\x88\x01\x01\x42\r\n\x0b_paginationB\r\n\x0b_date_range"e\n\x19GetBalanceHistoryResponse\x12H\n\x08\x62\x61lances\x18\x01 \x01(\x0b\x32,.datanode.api.v2.AggregatedBalanceConnectionR\x08\x62\x61lances"g\n\x15\x41ggregatedBalanceEdge\x12\x36\n\x04node\x18\x01 \x01(\x0b\x32".datanode.api.v2.AggregatedBalanceR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x93\x01\n\x1b\x41ggregatedBalanceConnection\x12<\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32&.datanode.api.v2.AggregatedBalanceEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\x9e\x01\n\rAccountFilter\x12\x19\n\x08\x61sset_id\x18\x01 \x01(\tR\x07\x61ssetId\x12\x1b\n\tparty_ids\x18\x02 \x03(\tR\x08partyIds\x12\x1d\n\nmarket_ids\x18\x03 \x03(\tR\tmarketIds\x12\x36\n\raccount_types\x18\x04 \x03(\x0e\x32\x11.vega.AccountTypeR\x0c\x61\x63\x63ountTypes"\xa1\x02\n\x11\x41ggregatedBalance\x12\x1c\n\ttimestamp\x18\x01 \x01(\x03R\ttimestamp\x12\x18\n\x07\x62\x61lance\x18\x02 \x01(\tR\x07\x62\x61lance\x12\x1e\n\x08party_id\x18\x04 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12\x1e\n\x08\x61sset_id\x18\x05 \x01(\tH\x01R\x07\x61ssetId\x88\x01\x01\x12 \n\tmarket_id\x18\x06 \x01(\tH\x02R\x08marketId\x88\x01\x01\x12\x39\n\x0c\x61\x63\x63ount_type\x18\x07 \x01(\x0e\x32\x11.vega.AccountTypeH\x03R\x0b\x61\x63\x63ountType\x88\x01\x01\x42\x0b\n\t_party_idB\x0b\n\t_asset_idB\x0c\n\n_market_idB\x0f\n\r_account_type";\n\x1aObserveMarketsDepthRequest\x12\x1d\n\nmarket_ids\x18\x01 \x03(\tR\tmarketIds"S\n\x1bObserveMarketsDepthResponse\x12\x34\n\x0cmarket_depth\x18\x01 \x03(\x0b\x32\x11.vega.MarketDepthR\x0bmarketDepth"B\n!ObserveMarketsDepthUpdatesRequest\x12\x1d\n\nmarket_ids\x18\x01 \x03(\tR\tmarketIds"U\n"ObserveMarketsDepthUpdatesResponse\x12/\n\x06update\x18\x01 \x03(\x0b\x32\x17.vega.MarketDepthUpdateR\x06update":\n\x19ObserveMarketsDataRequest\x12\x1d\n\nmarket_ids\x18\x01 \x03(\tR\tmarketIds"O\n\x1aObserveMarketsDataResponse\x12\x31\n\x0bmarket_data\x18\x01 \x03(\x0b\x32\x10.vega.MarketDataR\nmarketData"o\n\x1bGetLatestMarketDepthRequest\x12 \n\tmarket_id\x18\x01 \x01(\tB\x03\xe0\x41\x02R\x08marketId\x12 \n\tmax_depth\x18\x02 \x01(\x04H\x00R\x08maxDepth\x88\x01\x01\x42\x0c\n\n_max_depth"\xda\x01\n\x1cGetLatestMarketDepthResponse\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12"\n\x03\x62uy\x18\x02 \x03(\x0b\x32\x10.vega.PriceLevelR\x03\x62uy\x12$\n\x04sell\x18\x03 \x03(\x0b\x32\x10.vega.PriceLevelR\x04sell\x12*\n\nlast_trade\x18\x04 \x01(\x0b\x32\x0b.vega.TradeR\tlastTrade\x12\'\n\x0fsequence_number\x18\x05 \x01(\x04R\x0esequenceNumber"\x1d\n\x1bListLatestMarketDataRequest"S\n\x1cListLatestMarketDataResponse\x12\x33\n\x0cmarkets_data\x18\x01 \x03(\x0b\x32\x10.vega.MarketDataR\x0bmarketsData">\n\x1aGetLatestMarketDataRequest\x12 \n\tmarket_id\x18\x01 \x01(\tB\x03\xe0\x41\x02R\x08marketId"P\n\x1bGetLatestMarketDataResponse\x12\x31\n\x0bmarket_data\x18\x01 \x01(\x0b\x32\x10.vega.MarketDataR\nmarketData"\x98\x02\n\x1fGetMarketDataHistoryByIDRequest\x12 \n\tmarket_id\x18\x01 \x01(\tB\x03\xe0\x41\x02R\x08marketId\x12,\n\x0fstart_timestamp\x18\x02 \x01(\x03H\x00R\x0estartTimestamp\x88\x01\x01\x12(\n\rend_timestamp\x18\x03 \x01(\x03H\x01R\x0c\x65ndTimestamp\x88\x01\x01\x12@\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x02R\npagination\x88\x01\x01\x42\x12\n\x10_start_timestampB\x10\n\x0e_end_timestampB\r\n\x0b_paginationJ\x04\x08\x05\x10\x06"j\n GetMarketDataHistoryByIDResponse\x12\x46\n\x0bmarket_data\x18\x01 \x01(\x0b\x32%.datanode.api.v2.MarketDataConnectionR\nmarketData"N\n\x0eMarketDataEdge\x12$\n\x04node\x18\x01 \x01(\x0b\x32\x10.vega.MarketDataR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x85\x01\n\x14MarketDataConnection\x12\x35\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.MarketDataEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xd1\x01\n\x14ListTransfersRequest\x12\x1b\n\x06pubkey\x18\x01 \x01(\tH\x00R\x06pubkey\x88\x01\x01\x12@\n\tdirection\x18\x02 \x01(\x0e\x32".datanode.api.v2.TransferDirectionR\tdirection\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x01R\npagination\x88\x01\x01\x42\t\n\x07_pubkeyB\r\n\x0b_pagination"Z\n\x15ListTransfersResponse\x12\x41\n\ttransfers\x18\x01 \x01(\x0b\x32#.datanode.api.v2.TransferConnectionR\ttransfers"T\n\x0cTransferEdge\x12,\n\x04node\x18\x01 \x01(\x0b\x32\x18.vega.events.v1.TransferR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x81\x01\n\x12TransferConnection\x12\x33\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1d.datanode.api.v2.TransferEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\x19\n\x17GetNetworkLimitsRequest"G\n\x18GetNetworkLimitsResponse\x12+\n\x06limits\x18\x01 \x01(\x0b\x32\x13.vega.NetworkLimitsR\x06limits">\n\x1aListCandleIntervalsRequest\x12 \n\tmarket_id\x18\x01 \x01(\tB\x03\xe0\x41\x02R\x08marketId"M\n\x12IntervalToCandleId\x12\x1a\n\x08interval\x18\x01 \x01(\tR\x08interval\x12\x1b\n\tcandle_id\x18\x02 \x01(\tR\x08\x63\x61ndleId"u\n\x1bListCandleIntervalsResponse\x12V\n\x15interval_to_candle_id\x18\x01 \x03(\x0b\x32#.datanode.api.v2.IntervalToCandleIdR\x12intervalToCandleId"\xa7\x01\n\x06\x43\x61ndle\x12\x14\n\x05start\x18\x01 \x01(\x03R\x05start\x12\x1f\n\x0blast_update\x18\x02 \x01(\x03R\nlastUpdate\x12\x12\n\x04high\x18\x03 \x01(\tR\x04high\x12\x10\n\x03low\x18\x04 \x01(\tR\x03low\x12\x12\n\x04open\x18\x05 \x01(\tR\x04open\x12\x14\n\x05\x63lose\x18\x06 \x01(\tR\x05\x63lose\x12\x16\n\x06volume\x18\x07 \x01(\x04R\x06volume"<\n\x18ObserveCandleDataRequest\x12 \n\tcandle_id\x18\x01 \x01(\tB\x03\xe0\x41\x02R\x08\x63\x61ndleId"L\n\x19ObserveCandleDataResponse\x12/\n\x06\x63\x61ndle\x18\x01 \x01(\x0b\x32\x17.datanode.api.v2.CandleR\x06\x63\x61ndle"\xda\x01\n\x15ListCandleDataRequest\x12 \n\tcandle_id\x18\x01 \x01(\tB\x03\xe0\x41\x02R\x08\x63\x61ndleId\x12%\n\x0e\x66rom_timestamp\x18\x02 \x01(\x03R\rfromTimestamp\x12!\n\x0cto_timestamp\x18\x03 \x01(\x03R\x0btoTimestamp\x12@\n\npagination\x18\x05 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_paginationJ\x04\x08\x04\x10\x05"Y\n\x16ListCandleDataResponse\x12?\n\x07\x63\x61ndles\x18\x01 \x01(\x0b\x32%.datanode.api.v2.CandleDataConnectionR\x07\x63\x61ndles"Q\n\nCandleEdge\x12+\n\x04node\x18\x01 \x01(\x0b\x32\x17.datanode.api.v2.CandleR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x81\x01\n\x14\x43\x61ndleDataConnection\x12\x31\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1b.datanode.api.v2.CandleEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xc6\x01\n\x10ListVotesRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12$\n\x0bproposal_id\x18\x02 \x01(\tH\x01R\nproposalId\x88\x01\x01\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x02R\npagination\x88\x01\x01\x42\x0b\n\t_party_idB\x0e\n\x0c_proposal_idB\r\n\x0b_pagination"J\n\x11ListVotesResponse\x12\x35\n\x05votes\x18\x01 \x01(\x0b\x32\x1f.datanode.api.v2.VoteConnectionR\x05votes"B\n\x08VoteEdge\x12\x1e\n\x04node\x18\x01 \x01(\x0b\x32\n.vega.VoteR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"y\n\x0eVoteConnection\x12/\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x19.datanode.api.v2.VoteEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"x\n\x13ObserveVotesRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12$\n\x0bproposal_id\x18\x02 \x01(\tH\x01R\nproposalId\x88\x01\x01\x42\x0b\n\t_party_idB\x0e\n\x0c_proposal_id"6\n\x14ObserveVotesResponse\x12\x1e\n\x04vote\x18\x01 \x01(\x0b\x32\n.vega.VoteR\x04vote"\xbd\x01\n*ListERC20MultiSigSignerAddedBundlesRequest\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x1c\n\tsubmitter\x18\x02 \x01(\tR\tsubmitter\x12\x1b\n\tepoch_seq\x18\x03 \x01(\tR\x08\x65pochSeq\x12;\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationR\npagination"|\n+ListERC20MultiSigSignerAddedBundlesResponse\x12M\n\x07\x62undles\x18\x01 \x01(\x0b\x32\x33.datanode.api.v2.ERC20MultiSigSignerAddedConnectionR\x07\x62undles"t\n\x1c\x45RC20MultiSigSignerAddedEdge\x12<\n\x04node\x18\x01 \x01(\x0b\x32(.vega.events.v1.ERC20MultiSigSignerAddedR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x81\x01\n"ERC20MultiSigSignerAddedBundleEdge\x12\x43\n\x04node\x18\x01 \x01(\x0b\x32/.datanode.api.v2.ERC20MultiSigSignerAddedBundleR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\xa7\x01\n"ERC20MultiSigSignerAddedConnection\x12I\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x33.datanode.api.v2.ERC20MultiSigSignerAddedBundleEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xce\x01\n\x1e\x45RC20MultiSigSignerAddedBundle\x12\x1d\n\nnew_signer\x18\x01 \x01(\tR\tnewSigner\x12\x1c\n\tsubmitter\x18\x02 \x01(\tR\tsubmitter\x12\x14\n\x05nonce\x18\x04 \x01(\tR\x05nonce\x12\x1c\n\ttimestamp\x18\x05 \x01(\x03R\ttimestamp\x12\x1e\n\nsignatures\x18\x06 \x01(\tR\nsignatures\x12\x1b\n\tepoch_seq\x18\x03 \x01(\tR\x08\x65pochSeq"\xbf\x01\n,ListERC20MultiSigSignerRemovedBundlesRequest\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x1c\n\tsubmitter\x18\x02 \x01(\tR\tsubmitter\x12\x1b\n\tepoch_seq\x18\x03 \x01(\tR\x08\x65pochSeq\x12;\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationR\npagination"\x80\x01\n-ListERC20MultiSigSignerRemovedBundlesResponse\x12O\n\x07\x62undles\x18\x01 \x01(\x0b\x32\x35.datanode.api.v2.ERC20MultiSigSignerRemovedConnectionR\x07\x62undles"x\n\x1e\x45RC20MultiSigSignerRemovedEdge\x12>\n\x04node\x18\x01 \x01(\x0b\x32*.vega.events.v1.ERC20MultiSigSignerRemovedR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x85\x01\n$ERC20MultiSigSignerRemovedBundleEdge\x12\x45\n\x04node\x18\x01 \x01(\x0b\x32\x31.datanode.api.v2.ERC20MultiSigSignerRemovedBundleR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\xab\x01\n$ERC20MultiSigSignerRemovedConnection\x12K\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x35.datanode.api.v2.ERC20MultiSigSignerRemovedBundleEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xd0\x01\n ERC20MultiSigSignerRemovedBundle\x12\x1d\n\nold_signer\x18\x01 \x01(\tR\toldSigner\x12\x1c\n\tsubmitter\x18\x02 \x01(\tR\tsubmitter\x12\x14\n\x05nonce\x18\x04 \x01(\tR\x05nonce\x12\x1c\n\ttimestamp\x18\x05 \x01(\x03R\ttimestamp\x12\x1e\n\nsignatures\x18\x06 \x01(\tR\nsignatures\x12\x1b\n\tepoch_seq\x18\x07 \x01(\tR\x08\x65pochSeq"@\n\x1eGetERC20ListAssetBundleRequest\x12\x1e\n\x08\x61sset_id\x18\x01 \x01(\tB\x03\xe0\x41\x02R\x07\x61ssetId"\x9e\x01\n\x1fGetERC20ListAssetBundleResponse\x12!\n\x0c\x61sset_source\x18\x01 \x01(\tR\x0b\x61ssetSource\x12"\n\rvega_asset_id\x18\x02 \x01(\tR\x0bvegaAssetId\x12\x14\n\x05nonce\x18\x03 \x01(\tR\x05nonce\x12\x1e\n\nsignatures\x18\x04 \x01(\tR\nsignatures"K\n#GetERC20SetAssetLimitsBundleRequest\x12$\n\x0bproposal_id\x18\x01 \x01(\tB\x03\xe0\x41\x02R\nproposalId"\xe8\x01\n$GetERC20SetAssetLimitsBundleResponse\x12!\n\x0c\x61sset_source\x18\x01 \x01(\tR\x0b\x61ssetSource\x12"\n\rvega_asset_id\x18\x02 \x01(\tR\x0bvegaAssetId\x12\x14\n\x05nonce\x18\x03 \x01(\tR\x05nonce\x12%\n\x0elifetime_limit\x18\x04 \x01(\tR\rlifetimeLimit\x12\x1c\n\tthreshold\x18\x05 \x01(\tR\tthreshold\x12\x1e\n\nsignatures\x18\x06 \x01(\tR\nsignatures"M\n!GetERC20WithdrawalApprovalRequest\x12(\n\rwithdrawal_id\x18\x01 \x01(\tB\x03\xe0\x41\x02R\x0cwithdrawalId"\xde\x01\n"GetERC20WithdrawalApprovalResponse\x12!\n\x0c\x61sset_source\x18\x01 \x01(\tR\x0b\x61ssetSource\x12\x16\n\x06\x61mount\x18\x02 \x01(\tR\x06\x61mount\x12\x14\n\x05nonce\x18\x04 \x01(\tR\x05nonce\x12\x1e\n\nsignatures\x18\x05 \x01(\tR\nsignatures\x12%\n\x0etarget_address\x18\x06 \x01(\tR\rtargetAddress\x12\x1a\n\x08\x63reation\x18\x07 \x01(\x03R\x08\x63reationJ\x04\x08\x03\x10\x04"7\n\x13GetLastTradeRequest\x12 \n\tmarket_id\x18\x01 \x01(\tB\x03\xe0\x41\x02R\x08marketId"9\n\x14GetLastTradeResponse\x12!\n\x05trade\x18\x01 \x01(\x0b\x32\x0b.vega.TradeR\x05trade"\x8c\x02\n\x11ListTradesRequest\x12\x1d\n\nmarket_ids\x18\x01 \x03(\tR\tmarketIds\x12\x1b\n\torder_ids\x18\x02 \x03(\tR\x08orderIds\x12\x1b\n\tparty_ids\x18\x03 \x03(\tR\x08partyIds\x12@\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12>\n\ndate_range\x18\x05 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x01R\tdateRange\x88\x01\x01\x42\r\n\x0b_paginationB\r\n\x0b_date_range"N\n\x12ListTradesResponse\x12\x38\n\x06trades\x18\x01 \x01(\x0b\x32 .datanode.api.v2.TradeConnectionR\x06trades"{\n\x0fTradeConnection\x12\x30\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1a.datanode.api.v2.TradeEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"D\n\tTradeEdge\x12\x1f\n\x04node\x18\x01 \x01(\x0b\x32\x0b.vega.TradeR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"R\n\x14ObserveTradesRequest\x12\x1d\n\nmarket_ids\x18\x01 \x03(\tR\tmarketIds\x12\x1b\n\tparty_ids\x18\x02 \x03(\tR\x08partyIds"<\n\x15ObserveTradesResponse\x12#\n\x06trades\x18\x01 \x03(\x0b\x32\x0b.vega.TradeR\x06trades"A\n\x14GetOracleSpecRequest\x12)\n\x0eoracle_spec_id\x18\x01 \x01(\tB\x03\xe0\x41\x02R\x0coracleSpecId"J\n\x15GetOracleSpecResponse\x12\x31\n\x0boracle_spec\x18\x01 \x01(\x0b\x32\x10.vega.OracleSpecR\noracleSpec"i\n\x16ListOracleSpecsRequest\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"d\n\x17ListOracleSpecsResponse\x12I\n\x0coracle_specs\x18\x01 \x01(\x0b\x32&.datanode.api.v2.OracleSpecsConnectionR\x0boracleSpecs"\xa6\x01\n\x15ListOracleDataRequest\x12)\n\x0eoracle_spec_id\x18\x01 \x01(\tH\x00R\x0coracleSpecId\x88\x01\x01\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x01R\npagination\x88\x01\x01\x42\x11\n\x0f_oracle_spec_idB\r\n\x0b_pagination"`\n\x16ListOracleDataResponse\x12\x46\n\x0boracle_data\x18\x01 \x01(\x0b\x32%.datanode.api.v2.OracleDataConnectionR\noracleData"N\n\x0eOracleSpecEdge\x12$\n\x04node\x18\x01 \x01(\x0b\x32\x10.vega.OracleSpecR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x86\x01\n\x15OracleSpecsConnection\x12\x35\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.OracleSpecEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"N\n\x0eOracleDataEdge\x12$\n\x04node\x18\x01 \x01(\x0b\x32\x10.vega.OracleDataR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x85\x01\n\x14OracleDataConnection\x12\x35\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.OracleDataEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"4\n\x10GetMarketRequest\x12 \n\tmarket_id\x18\x01 \x01(\tB\x03\xe0\x41\x02R\x08marketId"9\n\x11GetMarketResponse\x12$\n\x06market\x18\x01 \x01(\x0b\x32\x0c.vega.MarketR\x06market"\xa7\x01\n\x12ListMarketsRequest\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12,\n\x0finclude_settled\x18\x03 \x01(\x08H\x01R\x0eincludeSettled\x88\x01\x01\x42\r\n\x0b_paginationB\x12\n\x10_include_settled"R\n\x13ListMarketsResponse\x12;\n\x07markets\x18\x01 \x01(\x0b\x32!.datanode.api.v2.MarketConnectionR\x07markets"F\n\nMarketEdge\x12 \n\x04node\x18\x01 \x01(\x0b\x32\x0c.vega.MarketR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"}\n\x10MarketConnection\x12\x31\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1b.datanode.api.v2.MarketEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"1\n\x0fGetPartyRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tB\x03\xe0\x41\x02R\x07partyId"5\n\x10GetPartyResponse\x12!\n\x05party\x18\x01 \x01(\x0b\x32\x0b.vega.PartyR\x05party"l\n\x12ListPartiesRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12;\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationR\npagination"Q\n\x13ListPartiesResponse\x12:\n\x07parties\x18\x01 \x01(\x0b\x32 .datanode.api.v2.PartyConnectionR\x07parties"D\n\tPartyEdge\x12\x1f\n\x04node\x18\x01 \x01(\x0b\x32\x0b.vega.PartyR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"{\n\x0fPartyConnection\x12\x30\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1a.datanode.api.v2.PartyEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"D\n\tOrderEdge\x12\x1f\n\x04node\x18\x01 \x01(\x0b\x32\x0b.vega.OrderR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x8e\x01\n\x17ListMarginLevelsRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12;\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationR\npagination"b\n\x18ListMarginLevelsResponse\x12\x46\n\rmargin_levels\x18\x01 \x01(\x0b\x32!.datanode.api.v2.MarginConnectionR\x0cmarginLevels"g\n\x1aObserveMarginLevelsRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12 \n\tmarket_id\x18\x02 \x01(\tH\x00R\x08marketId\x88\x01\x01\x42\x0c\n\n_market_id"V\n\x1bObserveMarginLevelsResponse\x12\x37\n\rmargin_levels\x18\x01 \x01(\x0b\x32\x12.vega.MarginLevelsR\x0cmarginLevels"{\n\x0fOrderConnection\x12\x30\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1a.datanode.api.v2.OrderEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"L\n\nMarginEdge\x12&\n\x04node\x18\x01 \x01(\x0b\x32\x12.vega.MarginLevelsR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"}\n\x10MarginConnection\x12\x31\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1b.datanode.api.v2.MarginEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\x8d\x02\n\x12ListRewardsRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12\x1e\n\x08\x61sset_id\x18\x02 \x01(\tH\x00R\x07\x61ssetId\x88\x01\x01\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x01R\npagination\x88\x01\x01\x12"\n\nfrom_epoch\x18\x04 \x01(\x04H\x02R\tfromEpoch\x88\x01\x01\x12\x1e\n\x08to_epoch\x18\x05 \x01(\x04H\x03R\x07toEpoch\x88\x01\x01\x42\x0b\n\t_asset_idB\r\n\x0b_paginationB\r\n\x0b_from_epochB\x0b\n\t_to_epoch"S\n\x13ListRewardsResponse\x12<\n\x07rewards\x18\x01 \x01(\x0b\x32".datanode.api.v2.RewardsConnectionR\x07rewards"F\n\nRewardEdge\x12 \n\x04node\x18\x01 \x01(\x0b\x32\x0c.vega.RewardR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"~\n\x11RewardsConnection\x12\x31\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1b.datanode.api.v2.RewardEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xc7\x01\n\x1aListRewardSummariesRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12\x1e\n\x08\x61sset_id\x18\x02 \x01(\tH\x01R\x07\x61ssetId\x88\x01\x01\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x02R\npagination\x88\x01\x01\x42\x0b\n\t_party_idB\x0b\n\t_asset_idB\r\n\x0b_pagination"P\n\x1bListRewardSummariesResponse\x12\x31\n\tsummaries\x18\x01 \x03(\x0b\x32\x13.vega.RewardSummaryR\tsummaries"\xb1\x01\n\x13RewardSummaryFilter\x12\x1b\n\tasset_ids\x18\x01 \x03(\tR\x08\x61ssetIds\x12\x1d\n\nmarket_ids\x18\x02 \x03(\tR\tmarketIds\x12"\n\nfrom_epoch\x18\x03 \x01(\x04H\x00R\tfromEpoch\x88\x01\x01\x12\x1e\n\x08to_epoch\x18\x04 \x01(\x04H\x01R\x07toEpoch\x88\x01\x01\x42\r\n\x0b_from_epochB\x0b\n\t_to_epoch"\xb0\x01\n\x1fListEpochRewardSummariesRequest\x12<\n\x06\x66ilter\x18\x01 \x01(\x0b\x32$.datanode.api.v2.RewardSummaryFilterR\x06\x66ilter\x12@\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"o\n ListEpochRewardSummariesResponse\x12K\n\tsummaries\x18\x01 \x01(\x0b\x32-.datanode.api.v2.EpochRewardSummaryConnectionR\tsummaries"\x95\x01\n\x1c\x45pochRewardSummaryConnection\x12=\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\'.datanode.api.v2.EpochRewardSummaryEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"^\n\x16\x45pochRewardSummaryEdge\x12,\n\x04node\x18\x01 \x01(\x0b\x32\x18.vega.EpochRewardSummaryR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"q\n\x15ObserveRewardsRequest\x12\x1e\n\x08\x61sset_id\x18\x01 \x01(\tH\x00R\x07\x61ssetId\x88\x01\x01\x12\x1e\n\x08party_id\x18\x02 \x01(\tH\x01R\x07partyId\x88\x01\x01\x42\x0b\n\t_asset_idB\x0b\n\t_party_id">\n\x16ObserveRewardsResponse\x12$\n\x06reward\x18\x01 \x01(\x0b\x32\x0c.vega.RewardR\x06reward"(\n\x11GetDepositRequest\x12\x13\n\x02id\x18\x01 \x01(\tB\x03\xe0\x41\x02R\x02id"=\n\x12GetDepositResponse\x12\'\n\x07\x64\x65posit\x18\x01 \x01(\x0b\x32\r.vega.DepositR\x07\x64\x65posit"\xd0\x01\n\x13ListDepositsRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12>\n\ndate_range\x18\x03 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x01R\tdateRange\x88\x01\x01\x42\r\n\x0b_paginationB\r\n\x0b_date_range"W\n\x14ListDepositsResponse\x12?\n\x08\x64\x65posits\x18\x01 \x01(\x0b\x32#.datanode.api.v2.DepositsConnectionR\x08\x64\x65posits"H\n\x0b\x44\x65positEdge\x12!\n\x04node\x18\x01 \x01(\x0b\x32\r.vega.DepositR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x80\x01\n\x12\x44\x65positsConnection\x12\x32\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1c.datanode.api.v2.DepositEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"+\n\x14GetWithdrawalRequest\x12\x13\n\x02id\x18\x01 \x01(\tB\x03\xe0\x41\x02R\x02id"I\n\x15GetWithdrawalResponse\x12\x30\n\nwithdrawal\x18\x01 \x01(\x0b\x32\x10.vega.WithdrawalR\nwithdrawal"\xd3\x01\n\x16ListWithdrawalsRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12>\n\ndate_range\x18\x03 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x01R\tdateRange\x88\x01\x01\x42\r\n\x0b_paginationB\r\n\x0b_date_range"c\n\x17ListWithdrawalsResponse\x12H\n\x0bwithdrawals\x18\x01 \x01(\x0b\x32&.datanode.api.v2.WithdrawalsConnectionR\x0bwithdrawals"N\n\x0eWithdrawalEdge\x12$\n\x04node\x18\x01 \x01(\x0b\x32\x10.vega.WithdrawalR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x86\x01\n\x15WithdrawalsConnection\x12\x35\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.WithdrawalEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"1\n\x0fGetAssetRequest\x12\x1e\n\x08\x61sset_id\x18\x01 \x01(\tB\x03\xe0\x41\x02R\x07\x61ssetId"5\n\x10GetAssetResponse\x12!\n\x05\x61sset\x18\x01 \x01(\x0b\x32\x0b.vega.AssetR\x05\x61sset"\x91\x01\n\x11ListAssetsRequest\x12\x1e\n\x08\x61sset_id\x18\x01 \x01(\tH\x00R\x07\x61ssetId\x88\x01\x01\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x01R\npagination\x88\x01\x01\x42\x0b\n\t_asset_idB\r\n\x0b_pagination"O\n\x12ListAssetsResponse\x12\x39\n\x06\x61ssets\x18\x01 \x01(\x0b\x32!.datanode.api.v2.AssetsConnectionR\x06\x61ssets"D\n\tAssetEdge\x12\x1f\n\x04node\x18\x01 \x01(\x0b\x32\x0b.vega.AssetR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"|\n\x10\x41ssetsConnection\x12\x30\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1a.datanode.api.v2.AssetEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xa1\x02\n\x1eListLiquidityProvisionsRequest\x12 \n\tmarket_id\x18\x01 \x01(\tH\x00R\x08marketId\x88\x01\x01\x12\x1e\n\x08party_id\x18\x02 \x01(\tH\x01R\x07partyId\x88\x01\x01\x12!\n\treference\x18\x03 \x01(\tH\x02R\treference\x88\x01\x01\x12\x17\n\x04live\x18\x04 \x01(\x08H\x03R\x04live\x88\x01\x01\x12@\n\npagination\x18\x05 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x04R\npagination\x88\x01\x01\x42\x0c\n\n_market_idB\x0b\n\t_party_idB\x0c\n\n_referenceB\x07\n\x05_liveB\r\n\x0b_pagination"\x84\x01\n\x1fListLiquidityProvisionsResponse\x12\x61\n\x14liquidity_provisions\x18\x01 \x01(\x0b\x32..datanode.api.v2.LiquidityProvisionsConnectionR\x13liquidityProvisions"_\n\x17LiquidityProvisionsEdge\x12,\n\x04node\x18\x01 \x01(\x0b\x32\x18.vega.LiquidityProvisionR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x97\x01\n\x1dLiquidityProvisionsConnection\x12>\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32(.datanode.api.v2.LiquidityProvisionsEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\x80\x01\n!ObserveLiquidityProvisionsRequest\x12 \n\tmarket_id\x18\x01 \x01(\tH\x00R\x08marketId\x88\x01\x01\x12\x1e\n\x08party_id\x18\x02 \x01(\tH\x01R\x07partyId\x88\x01\x01\x42\x0c\n\n_market_idB\x0b\n\t_party_id"q\n"ObserveLiquidityProvisionsResponse\x12K\n\x14liquidity_provisions\x18\x01 \x03(\x0b\x32\x18.vega.LiquidityProvisionR\x13liquidityProvisions"\x81\x01\n\x18GetGovernanceDataRequest\x12$\n\x0bproposal_id\x18\x01 \x01(\tH\x00R\nproposalId\x88\x01\x01\x12!\n\treference\x18\x02 \x01(\tH\x01R\treference\x88\x01\x01\x42\x0e\n\x0c_proposal_idB\x0c\n\n_reference"E\n\x19GetGovernanceDataResponse\x12(\n\x04\x64\x61ta\x18\x01 \x01(\x0b\x32\x14.vega.GovernanceDataR\x04\x64\x61ta"\xfa\x04\n\x19ListGovernanceDataRequest\x12@\n\x0eproposal_state\x18\x01 \x01(\x0e\x32\x14.vega.Proposal.StateH\x00R\rproposalState\x88\x01\x01\x12Y\n\rproposal_type\x18\x02 \x01(\x0e\x32/.datanode.api.v2.ListGovernanceDataRequest.TypeH\x01R\x0cproposalType\x88\x01\x01\x12/\n\x11proposer_party_id\x18\x03 \x01(\tH\x02R\x0fproposerPartyId\x88\x01\x01\x12\x32\n\x12proposal_reference\x18\x04 \x01(\tH\x03R\x11proposalReference\x88\x01\x01\x12@\n\npagination\x18\x05 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x04R\npagination\x88\x01\x01"\xb7\x01\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x0c\n\x08TYPE_ALL\x10\x01\x12\x13\n\x0fTYPE_NEW_MARKET\x10\x02\x12\x16\n\x12TYPE_UPDATE_MARKET\x10\x03\x12\x1b\n\x17TYPE_NETWORK_PARAMETERS\x10\x04\x12\x12\n\x0eTYPE_NEW_ASSET\x10\x05\x12\x16\n\x12TYPE_NEW_FREE_FORM\x10\x06\x12\x15\n\x11TYPE_UPDATE_ASSET\x10\x07\x42\x11\n\x0f_proposal_stateB\x10\n\x0e_proposal_typeB\x14\n\x12_proposer_party_idB\x15\n\x13_proposal_referenceB\r\n\x0b_pagination"g\n\x1aListGovernanceDataResponse\x12I\n\nconnection\x18\x01 \x01(\x0b\x32).datanode.api.v2.GovernanceDataConnectionR\nconnection"V\n\x12GovernanceDataEdge\x12(\n\x04node\x18\x01 \x01(\x0b\x32\x14.vega.GovernanceDataR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x8d\x01\n\x18GovernanceDataConnection\x12\x39\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32#.datanode.api.v2.GovernanceDataEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"G\n\x18ObserveGovernanceRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x42\x0b\n\t_party_id"E\n\x19ObserveGovernanceResponse\x12(\n\x04\x64\x61ta\x18\x01 \x01(\x0b\x32\x14.vega.GovernanceDataR\x04\x64\x61ta"\xed\x01\n\x16ListDelegationsRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12\x1c\n\x07node_id\x18\x02 \x01(\tH\x01R\x06nodeId\x88\x01\x01\x12\x1e\n\x08\x65poch_id\x18\x03 \x01(\tH\x02R\x07\x65pochId\x88\x01\x01\x12@\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x03R\npagination\x88\x01\x01\x42\x0b\n\t_party_idB\n\n\x08_node_idB\x0b\n\t_epoch_idB\r\n\x0b_pagination"c\n\x17ListDelegationsResponse\x12H\n\x0b\x64\x65legations\x18\x01 \x01(\x0b\x32&.datanode.api.v2.DelegationsConnectionR\x0b\x64\x65legations"N\n\x0e\x44\x65legationEdge\x12$\n\x04node\x18\x01 \x01(\x0b\x32\x10.vega.DelegationR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x86\x01\n\x15\x44\x65legationsConnection\x12\x35\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.DelegationEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"r\n\x19ObserveDelegationsRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12\x1c\n\x07node_id\x18\x02 \x01(\tH\x01R\x06nodeId\x88\x01\x01\x42\x0b\n\t_party_idB\n\n\x08_node_id"N\n\x1aObserveDelegationsResponse\x12\x30\n\ndelegation\x18\x01 \x01(\x0b\x32\x10.vega.DelegationR\ndelegation"\x91\x02\n\tNodeBasic\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x17\n\x07pub_key\x18\x02 \x01(\tR\x06pubKey\x12\x1c\n\ntm_pub_key\x18\x03 \x01(\tR\x08tmPubKey\x12)\n\x10\x65thereum_address\x18\x04 \x01(\tR\x0f\x65thereumAddress\x12\x19\n\x08info_url\x18\x05 \x01(\tR\x07infoUrl\x12\x1a\n\x08location\x18\x06 \x01(\tR\x08location\x12(\n\x06status\x18\r \x01(\x0e\x32\x10.vega.NodeStatusR\x06status\x12\x12\n\x04name\x18\x11 \x01(\tR\x04name\x12\x1d\n\navatar_url\x18\x12 \x01(\tR\tavatarUrl"\x17\n\x15GetNetworkDataRequest"E\n\x16GetNetworkDataResponse\x12+\n\tnode_data\x18\x01 \x01(\x0b\x32\x0e.vega.NodeDataR\x08nodeData"%\n\x0eGetNodeRequest\x12\x13\n\x02id\x18\x01 \x01(\tB\x03\xe0\x41\x02R\x02id"1\n\x0fGetNodeResponse\x12\x1e\n\x04node\x18\x01 \x01(\x0b\x32\n.vega.NodeR\x04node"\x93\x01\n\x10ListNodesRequest\x12 \n\tepoch_seq\x18\x01 \x01(\x04H\x00R\x08\x65pochSeq\x88\x01\x01\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x01R\npagination\x88\x01\x01\x42\x0c\n\n_epoch_seqB\r\n\x0b_pagination"K\n\x11ListNodesResponse\x12\x36\n\x05nodes\x18\x01 \x01(\x0b\x32 .datanode.api.v2.NodesConnectionR\x05nodes"B\n\x08NodeEdge\x12\x1e\n\x04node\x18\x01 \x01(\x0b\x32\n.vega.NodeR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"z\n\x0fNodesConnection\x12/\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x19.datanode.api.v2.NodeEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\x81\x01\n\x19ListNodeSignaturesRequest\x12\x13\n\x02id\x18\x01 \x01(\tB\x03\xe0\x41\x02R\x02id\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"g\n\x1aListNodeSignaturesResponse\x12I\n\nsignatures\x18\x01 \x01(\x0b\x32).datanode.api.v2.NodeSignaturesConnectionR\nsignatures"`\n\x11NodeSignatureEdge\x12\x33\n\x04node\x18\x01 \x01(\x0b\x32\x1f.vega.commands.v1.NodeSignatureR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x8c\x01\n\x18NodeSignaturesConnection\x12\x38\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32".datanode.api.v2.NodeSignatureEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"-\n\x0fGetEpochRequest\x12\x13\n\x02id\x18\x01 \x01(\x04H\x00R\x02id\x88\x01\x01\x42\x05\n\x03_id"5\n\x10GetEpochResponse\x12!\n\x05\x65poch\x18\x01 \x01(\x0b\x32\x0b.vega.EpochR\x05\x65poch"j\n\x12\x45stimateFeeRequest\x12 \n\tmarket_id\x18\x01 \x01(\tB\x03\xe0\x41\x02R\x08marketId\x12\x19\n\x05price\x18\x02 \x01(\tB\x03\xe0\x41\x02R\x05price\x12\x17\n\x04size\x18\x03 \x01(\x04\x42\x03\xe0\x41\x02R\x04size"2\n\x13\x45stimateFeeResponse\x12\x1b\n\x03\x66\x65\x65\x18\x02 \x01(\x0b\x32\t.vega.FeeR\x03\x66\x65\x65"\xe1\x01\n\x15\x45stimateMarginRequest\x12 \n\tmarket_id\x18\x01 \x01(\tB\x03\xe0\x41\x02R\x08marketId\x12\x1e\n\x08party_id\x18\x02 \x01(\tB\x03\xe0\x41\x02R\x07partyId\x12#\n\x04side\x18\x03 \x01(\x0e\x32\n.vega.SideB\x03\xe0\x41\x02R\x04side\x12)\n\x04type\x18\x04 \x01(\x0e\x32\x10.vega.Order.TypeB\x03\xe0\x41\x02R\x04type\x12\x17\n\x04size\x18\x05 \x01(\x04\x42\x03\xe0\x41\x02R\x04size\x12\x19\n\x05price\x18\x06 \x01(\tB\x03\xe0\x41\x02R\x05price:\x02\x18\x01"U\n\x16\x45stimateMarginResponse\x12\x37\n\rmargin_levels\x18\x02 \x01(\x0b\x32\x12.vega.MarginLevelsR\x0cmarginLevels:\x02\x18\x01"o\n\x1cListNetworkParametersRequest\x12@\n\npagination\x18\x01 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"{\n\x1dListNetworkParametersResponse\x12Z\n\x12network_parameters\x18\x01 \x01(\x0b\x32+.datanode.api.v2.NetworkParameterConnectionR\x11networkParameters"3\n\x1aGetNetworkParameterRequest\x12\x15\n\x03key\x18\x01 \x01(\tB\x03\xe0\x41\x02R\x03key"b\n\x1bGetNetworkParameterResponse\x12\x43\n\x11network_parameter\x18\x01 \x01(\x0b\x32\x16.vega.NetworkParameterR\x10networkParameter"Z\n\x14NetworkParameterEdge\x12*\n\x04node\x18\x01 \x01(\x0b\x32\x16.vega.NetworkParameterR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x91\x01\n\x1aNetworkParameterConnection\x12;\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32%.datanode.api.v2.NetworkParameterEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"Z\n\nCheckpoint\x12\x12\n\x04hash\x18\x01 \x01(\tR\x04hash\x12\x1d\n\nblock_hash\x18\x02 \x01(\tR\tblockHash\x12\x19\n\x08\x61t_block\x18\x03 \x01(\x04R\x07\x61tBlock"i\n\x16ListCheckpointsRequest\x12@\n\npagination\x18\x01 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"c\n\x17ListCheckpointsResponse\x12H\n\x0b\x63heckpoints\x18\x01 \x01(\x0b\x32&.datanode.api.v2.CheckpointsConnectionR\x0b\x63heckpoints"Y\n\x0e\x43heckpointEdge\x12/\n\x04node\x18\x01 \x01(\x0b\x32\x1b.datanode.api.v2.CheckpointR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x86\x01\n\x15\x43heckpointsConnection\x12\x35\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.CheckpointEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\x82\x01\n\x0fGetStakeRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tB\x03\xe0\x41\x02R\x07partyId\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"\x94\x01\n\x10GetStakeResponse\x12\x36\n\x17\x63urrent_stake_available\x18\x01 \x01(\tR\x15\x63urrentStakeAvailable\x12H\n\x0estake_linkings\x18\x02 \x01(\x0b\x32!.datanode.api.v2.StakesConnectionR\rstakeLinkings"\\\n\x10StakeLinkingEdge\x12\x30\n\x04node\x18\x01 \x01(\x0b\x32\x1c.vega.events.v1.StakeLinkingR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x83\x01\n\x10StakesConnection\x12\x37\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32!.datanode.api.v2.StakeLinkingEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"9\n\x15GetRiskFactorsRequest\x12 \n\tmarket_id\x18\x01 \x01(\tB\x03\xe0\x41\x02R\x08marketId"K\n\x16GetRiskFactorsResponse\x12\x31\n\x0brisk_factor\x18\x01 \x01(\x0b\x32\x10.vega.RiskFactorR\nriskFactor"\xa1\x01\n\x16ObserveEventBusRequest\x12\x30\n\x04type\x18\x01 \x03(\x0e\x32\x1c.vega.events.v1.BusEventTypeR\x04type\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x03 \x01(\tR\x07partyId\x12\x1d\n\nbatch_size\x18\x04 \x01(\x03R\tbatchSize"K\n\x17ObserveEventBusResponse\x12\x30\n\x06\x65vents\x18\x01 \x03(\x0b\x32\x18.vega.events.v1.BusEventR\x06\x65vents"\x1f\n\x1dObserveLedgerMovementsRequest"_\n\x1eObserveLedgerMovementsResponse\x12=\n\x0fledger_movement\x18\x01 \x01(\x0b\x32\x14.vega.LedgerMovementR\x0eledgerMovement"\x94\x01\n\x17ListKeyRotationsRequest\x12\x1c\n\x07node_id\x18\x01 \x01(\tH\x00R\x06nodeId\x88\x01\x01\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x01R\npagination\x88\x01\x01\x42\n\n\x08_node_idB\r\n\x0b_pagination"`\n\x18ListKeyRotationsResponse\x12\x44\n\trotations\x18\x01 \x01(\x0b\x32&.datanode.api.v2.KeyRotationConnectionR\trotations"Z\n\x0fKeyRotationEdge\x12/\n\x04node\x18\x01 \x01(\x0b\x32\x1b.vega.events.v1.KeyRotationR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x87\x01\n\x15KeyRotationConnection\x12\x36\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32 .datanode.api.v2.KeyRotationEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\x9c\x01\n\x1fListEthereumKeyRotationsRequest\x12\x1c\n\x07node_id\x18\x01 \x01(\tH\x00R\x06nodeId\x88\x01\x01\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x01R\npagination\x88\x01\x01\x42\n\n\x08_node_idB\r\n\x0b_pagination"x\n ListEthereumKeyRotationsResponse\x12T\n\rkey_rotations\x18\x01 \x01(\x0b\x32/.datanode.api.v2.EthereumKeyRotationsConnectionR\x0ckeyRotations"\x98\x01\n\x1e\x45thereumKeyRotationsConnection\x12>\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32(.datanode.api.v2.EthereumKeyRotationEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"j\n\x17\x45thereumKeyRotationEdge\x12\x37\n\x04node\x18\x01 \x01(\x0b\x32#.vega.events.v1.EthereumKeyRotationR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x14\n\x12GetVegaTimeRequest"3\n\x13GetVegaTimeResponse\x12\x1c\n\ttimestamp\x18\x01 \x01(\x03R\ttimestamp"\x89\x01\n\tDateRange\x12,\n\x0fstart_timestamp\x18\x01 \x01(\x03H\x00R\x0estartTimestamp\x88\x01\x01\x12(\n\rend_timestamp\x18\x02 \x01(\x03H\x01R\x0c\x65ndTimestamp\x88\x01\x01\x42\x12\n\x10_start_timestampB\x10\n\x0e_end_timestamp"!\n\x1fGetProtocolUpgradeStatusRequest"8\n GetProtocolUpgradeStatusResponse\x12\x14\n\x05ready\x18\x01 \x01(\x08R\x05ready"\x83\x02\n#ListProtocolUpgradeProposalsRequest\x12J\n\x06status\x18\x01 \x01(\x0e\x32-.vega.events.v1.ProtocolUpgradeProposalStatusH\x00R\x06status\x88\x01\x01\x12$\n\x0b\x61pproved_by\x18\x02 \x01(\tH\x01R\napprovedBy\x88\x01\x01\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x02R\npagination\x88\x01\x01\x42\t\n\x07_statusB\x0e\n\x0c_approved_byB\r\n\x0b_pagination"\x98\x01\n$ListProtocolUpgradeProposalsResponse\x12p\n\x1aprotocol_upgrade_proposals\x18\x01 \x01(\x0b\x32\x32.datanode.api.v2.ProtocolUpgradeProposalConnectionR\x18protocolUpgradeProposals"\x9f\x01\n!ProtocolUpgradeProposalConnection\x12\x42\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32,.datanode.api.v2.ProtocolUpgradeProposalEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"o\n\x1bProtocolUpgradeProposalEdge\x12\x38\n\x04node\x18\x01 \x01(\x0b\x32$.vega.events.v1.ProtocolUpgradeEventR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"k\n\x18ListCoreSnapshotsRequest\x12@\n\npagination\x18\x01 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"k\n\x19ListCoreSnapshotsResponse\x12N\n\x0e\x63ore_snapshots\x18\x01 \x01(\x0b\x32\'.datanode.api.v2.CoreSnapshotConnectionR\rcoreSnapshots"\x89\x01\n\x16\x43oreSnapshotConnection\x12\x37\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32!.datanode.api.v2.CoreSnapshotEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"`\n\x10\x43oreSnapshotEdge\x12\x34\n\x04node\x18\x01 \x01(\x0b\x32 .vega.events.v1.CoreSnapshotDataR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x81\x02\n\x0eHistorySegment\x12\x1f\n\x0b\x66rom_height\x18\x01 \x01(\x03R\nfromHeight\x12\x1b\n\tto_height\x18\x02 \x01(\x03R\x08toHeight\x12,\n\x12history_segment_id\x18\x03 \x01(\tR\x10historySegmentId\x12=\n\x1bprevious_history_segment_id\x18\x04 \x01(\tR\x18previousHistorySegmentId\x12)\n\x10\x64\x61tabase_version\x18\x05 \x01(\x03R\x0f\x64\x61tabaseVersion\x12\x19\n\x08\x63hain_id\x18\x06 \x01(\tR\x07\x63hainId"+\n)GetMostRecentNetworkHistorySegmentRequest"\x8d\x01\n*GetMostRecentNetworkHistorySegmentResponse\x12\x39\n\x07segment\x18\x01 \x01(\x0b\x32\x1f.datanode.api.v2.HistorySegmentR\x07segment\x12$\n\x0eswarm_key_seed\x18\x02 \x01(\tR\x0cswarmKeySeed"&\n$ListAllNetworkHistorySegmentsRequest"d\n%ListAllNetworkHistorySegmentsResponse\x12;\n\x08segments\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.HistorySegmentR\x08segments"-\n+GetActiveNetworkHistoryPeerAddressesRequest"Q\n,GetActiveNetworkHistoryPeerAddressesResponse\x12!\n\x0cip_addresses\x18\x01 \x03(\tR\x0bipAddresses" \n\x1eGetNetworkHistoryStatusRequest"\xb0\x01\n\x1fGetNetworkHistoryStatusResponse\x12!\n\x0cipfs_address\x18\x01 \x01(\tR\x0bipfsAddress\x12\x1b\n\tswarm_key\x18\x02 \x01(\tR\x08swarmKey\x12$\n\x0eswarm_key_seed\x18\x03 \x01(\tR\x0cswarmKeySeed\x12\'\n\x0f\x63onnected_peers\x18\x05 \x03(\tR\x0e\x63onnectedPeers"(\n&GetNetworkHistoryBootstrapPeersRequest"R\n\'GetNetworkHistoryBootstrapPeersResponse\x12\'\n\x0f\x62ootstrap_peers\x18\x01 \x03(\tR\x0e\x62ootstrapPeers"\x85\x01\n\x1b\x45xportNetworkHistoryRequest\x12\x1d\n\nfrom_block\x18\x01 \x01(\x03R\tfromBlock\x12\x19\n\x08to_block\x18\x02 \x01(\x03R\x07toBlock\x12,\n\x05table\x18\x03 \x01(\x0e\x32\x16.datanode.api.v2.TableR\x05table"E\n\x13ListEntitiesRequest\x12.\n\x10transaction_hash\x18\x01 \x01(\tB\x03\xe0\x41\x02R\x0ftransactionHash"\xad\r\n\x14ListEntitiesResponse\x12)\n\x08\x61\x63\x63ounts\x18\x01 \x03(\x0b\x32\r.vega.AccountR\x08\x61\x63\x63ounts\x12#\n\x06orders\x18\x02 \x03(\x0b\x32\x0b.vega.OrderR\x06orders\x12,\n\tpositions\x18\x03 \x03(\x0b\x32\x0e.vega.PositionR\tpositions\x12\x38\n\x0eledger_entries\x18\x04 \x03(\x0b\x32\x11.vega.LedgerEntryR\rledgerEntries\x12H\n\x0f\x62\x61lance_changes\x18\x05 \x03(\x0b\x32\x1f.datanode.api.v2.AccountBalanceR\x0e\x62\x61lanceChanges\x12\x36\n\ttransfers\x18\x06 \x03(\x0b\x32\x18.vega.events.v1.TransferR\ttransfers\x12 \n\x05votes\x18\x07 \x03(\x0b\x32\n.vega.VoteR\x05votes\x12~\n$erc20_multi_sig_signer_added_bundles\x18\x08 \x03(\x0b\x32/.datanode.api.v2.ERC20MultiSigSignerAddedBundleR\x1f\x65rc20MultiSigSignerAddedBundles\x12\x84\x01\n&erc20_multi_sig_signer_removed_bundles\x18\t \x03(\x0b\x32\x31.datanode.api.v2.ERC20MultiSigSignerRemovedBundleR!erc20MultiSigSignerRemovedBundles\x12#\n\x06trades\x18\n \x03(\x0b\x32\x0b.vega.TradeR\x06trades\x12\x33\n\x0coracle_specs\x18\x0b \x03(\x0b\x32\x10.vega.OracleSpecR\x0boracleSpecs\x12\x31\n\x0boracle_data\x18\x0c \x03(\x0b\x32\x10.vega.OracleDataR\noracleData\x12&\n\x07markets\x18\r \x03(\x0b\x32\x0c.vega.MarketR\x07markets\x12%\n\x07parties\x18\x0e \x03(\x0b\x32\x0b.vega.PartyR\x07parties\x12\x37\n\rmargin_levels\x18\x0f \x03(\x0b\x32\x12.vega.MarginLevelsR\x0cmarginLevels\x12&\n\x07rewards\x18\x10 \x03(\x0b\x32\x0c.vega.RewardR\x07rewards\x12)\n\x08\x64\x65posits\x18\x11 \x03(\x0b\x32\r.vega.DepositR\x08\x64\x65posits\x12\x32\n\x0bwithdrawals\x18\x12 \x03(\x0b\x32\x10.vega.WithdrawalR\x0bwithdrawals\x12#\n\x06\x61ssets\x18\x13 \x03(\x0b\x32\x0b.vega.AssetR\x06\x61ssets\x12K\n\x14liquidity_provisions\x18\x14 \x03(\x0b\x32\x18.vega.LiquidityProvisionR\x13liquidityProvisions\x12,\n\tproposals\x18\x15 \x03(\x0b\x32\x0e.vega.ProposalR\tproposals\x12\x32\n\x0b\x64\x65legations\x18\x16 \x03(\x0b\x32\x10.vega.DelegationR\x0b\x64\x65legations\x12\x30\n\x05nodes\x18\x17 \x03(\x0b\x32\x1a.datanode.api.v2.NodeBasicR\x05nodes\x12H\n\x0fnode_signatures\x18\x18 \x03(\x0b\x32\x1f.vega.commands.v1.NodeSignatureR\x0enodeSignatures\x12\x45\n\x12network_parameters\x18\x19 \x03(\x0b\x32\x16.vega.NetworkParameterR\x11networkParameters\x12@\n\rkey_rotations\x18\x1a \x03(\x0b\x32\x1b.vega.events.v1.KeyRotationR\x0ckeyRotations\x12Y\n\x16\x65thereum_key_rotations\x18\x1b \x03(\x0b\x32#.vega.events.v1.EthereumKeyRotationR\x14\x65thereumKeyRotations\x12\x62\n\x1aprotocol_upgrade_proposals\x18\x1c \x03(\x0b\x32$.vega.events.v1.ProtocolUpgradeEventR\x18protocolUpgradeProposals"\r\n\x0bPingRequest"\x0e\n\x0cPingResponse"\x87\x01\n\tOrderInfo\x12\x1e\n\x04side\x18\x01 \x01(\x0e\x32\n.vega.SideR\x04side\x12\x14\n\x05price\x18\x02 \x01(\tR\x05price\x12\x1c\n\tremaining\x18\x03 \x01(\x04R\tremaining\x12&\n\x0fis_market_order\x18\x04 \x01(\x08R\risMarketOrder"\xe6\x01\n\x17\x45stimatePositionRequest\x12 \n\tmarket_id\x18\x01 \x01(\tB\x03\xe0\x41\x02R\x08marketId\x12$\n\x0bopen_volume\x18\x02 \x01(\x03\x42\x03\xe0\x41\x02R\nopenVolume\x12\x32\n\x06orders\x18\x03 \x03(\x0b\x32\x1a.datanode.api.v2.OrderInfoR\x06orders\x12\x36\n\x14\x63ollateral_available\x18\x04 \x01(\tH\x00R\x13\x63ollateralAvailable\x88\x01\x01\x42\x17\n\x15_collateral_available"\x9b\x01\n\x18\x45stimatePositionResponse\x12\x37\n\x06margin\x18\x01 \x01(\x0b\x32\x1f.datanode.api.v2.MarginEstimateR\x06margin\x12\x46\n\x0bliquidation\x18\x02 \x01(\x0b\x32$.datanode.api.v2.LiquidationEstimateR\x0bliquidation"t\n\x0eMarginEstimate\x12\x31\n\nworst_case\x18\x01 \x01(\x0b\x32\x12.vega.MarginLevelsR\tworstCase\x12/\n\tbest_case\x18\x02 \x01(\x0b\x32\x12.vega.MarginLevelsR\x08\x62\x65stCase"\x97\x01\n\x13LiquidationEstimate\x12@\n\nworst_case\x18\x01 \x01(\x0b\x32!.datanode.api.v2.LiquidationPriceR\tworstCase\x12>\n\tbest_case\x18\x02 \x01(\x0b\x32!.datanode.api.v2.LiquidationPriceR\x08\x62\x65stCase"\xa2\x01\n\x10LiquidationPrice\x12(\n\x10open_volume_only\x18\x01 \x01(\tR\x0eopenVolumeOnly\x12\x30\n\x14including_buy_orders\x18\x02 \x01(\tR\x12includingBuyOrders\x12\x32\n\x15including_sell_orders\x18\x03 \x01(\tR\x13includingSellOrders*\xaa\x01\n\x10LedgerEntryField\x12"\n\x1eLEDGER_ENTRY_FIELD_UNSPECIFIED\x10\x00\x12&\n"LEDGER_ENTRY_FIELD_ACCOUNT_FROM_ID\x10\x01\x12$\n LEDGER_ENTRY_FIELD_ACCOUNT_TO_ID\x10\x02\x12$\n LEDGER_ENTRY_FIELD_TRANSFER_TYPE\x10\x03*\xb0\x01\n\x0c\x41\x63\x63ountField\x12\x1d\n\x19\x41\x43\x43OUNT_FIELD_UNSPECIFIED\x10\x00\x12\x14\n\x10\x41\x43\x43OUNT_FIELD_ID\x10\x01\x12\x1a\n\x16\x41\x43\x43OUNT_FIELD_PARTY_ID\x10\x02\x12\x1a\n\x16\x41\x43\x43OUNT_FIELD_ASSET_ID\x10\x03\x12\x1b\n\x17\x41\x43\x43OUNT_FIELD_MARKET_ID\x10\x04\x12\x16\n\x12\x41\x43\x43OUNT_FIELD_TYPE\x10\x05*\xad\x01\n\x11TransferDirection\x12"\n\x1eTRANSFER_DIRECTION_UNSPECIFIED\x10\x00\x12$\n TRANSFER_DIRECTION_TRANSFER_FROM\x10\x01\x12"\n\x1eTRANSFER_DIRECTION_TRANSFER_TO\x10\x02\x12*\n&TRANSFER_DIRECTION_TRANSFER_TO_OR_FROM\x10\x03*\xde\x02\n\x05Table\x12\x15\n\x11TABLE_UNSPECIFIED\x10\x00\x12\x12\n\x0eTABLE_BALANCES\x10\x01\x12\x15\n\x11TABLE_CHECKPOINTS\x10\x02\x12\x15\n\x11TABLE_DELEGATIONS\x10\x03\x12\x10\n\x0cTABLE_LEDGER\x10\x04\x12\x10\n\x0cTABLE_ORDERS\x10\x05\x12\x10\n\x0cTABLE_TRADES\x10\x06\x12\x15\n\x11TABLE_MARKET_DATA\x10\x07\x12\x17\n\x13TABLE_MARGIN_LEVELS\x10\x08\x12\x13\n\x0fTABLE_POSITIONS\x10\t\x12\x1e\n\x1aTABLE_LIQUIDITY_PROVISIONS\x10\n\x12\x11\n\rTABLE_MARKETS\x10\x0b\x12\x12\n\x0eTABLE_DEPOSITS\x10\x0c\x12\x15\n\x11TABLE_WITHDRAWALS\x10\r\x12\x10\n\x0cTABLE_BLOCKS\x10\x0e\x12\x11\n\rTABLE_REWARDS\x10\x0f\x32\x94U\n\x12TradingDataService\x12j\n\x0cListAccounts\x12$.datanode.api.v2.ListAccountsRequest\x1a%.datanode.api.v2.ListAccountsResponse"\r\x92\x41\n\n\x08\x41\x63\x63ounts\x12u\n\x0fObserveAccounts\x12\'.datanode.api.v2.ObserveAccountsRequest\x1a(.datanode.api.v2.ObserveAccountsResponse"\r\x92\x41\n\n\x08\x41\x63\x63ounts0\x01\x12Z\n\x04Info\x12\x1c.datanode.api.v2.InfoRequest\x1a\x1d.datanode.api.v2.InfoResponse"\x15\x92\x41\x12\n\x10Node information\x12\\\n\x08GetOrder\x12 .datanode.api.v2.GetOrderRequest\x1a!.datanode.api.v2.GetOrderResponse"\x0b\x92\x41\x08\n\x06Orders\x12\x62\n\nListOrders\x12".datanode.api.v2.ListOrdersRequest\x1a#.datanode.api.v2.ListOrdersResponse"\x0b\x92\x41\x08\n\x06Orders\x12w\n\x11ListOrderVersions\x12).datanode.api.v2.ListOrderVersionsRequest\x1a*.datanode.api.v2.ListOrderVersionsResponse"\x0b\x92\x41\x08\n\x06Orders\x12m\n\rObserveOrders\x12%.datanode.api.v2.ObserveOrdersRequest\x1a&.datanode.api.v2.ObserveOrdersResponse"\x0b\x92\x41\x08\n\x06Orders0\x01\x12q\n\rListPositions\x12%.datanode.api.v2.ListPositionsRequest\x1a&.datanode.api.v2.ListPositionsResponse"\x11\x88\x02\x01\x92\x41\x0b\n\tPositions\x12w\n\x10ListAllPositions\x12(.datanode.api.v2.ListAllPositionsRequest\x1a).datanode.api.v2.ListAllPositionsResponse"\x0e\x92\x41\x0b\n\tPositions\x12y\n\x10ObservePositions\x12(.datanode.api.v2.ObservePositionsRequest\x1a).datanode.api.v2.ObservePositionsResponse"\x0e\x92\x41\x0b\n\tPositions0\x01\x12\x7f\n\x11ListLedgerEntries\x12).datanode.api.v2.ListLedgerEntriesRequest\x1a*.datanode.api.v2.ListLedgerEntriesResponse"\x13\x92\x41\x10\n\x0eLedger entries\x12o\n\x13\x45xportLedgerEntries\x12+.datanode.api.v2.ExportLedgerEntriesRequest\x1a\x14.google.api.HttpBody"\x13\x92\x41\x10\n\x0eLedger entries0\x01\x12|\n\x12ListBalanceChanges\x12*.datanode.api.v2.ListBalanceChangesRequest\x1a+.datanode.api.v2.ListBalanceChangesResponse"\r\x92\x41\n\n\x08\x41\x63\x63ounts\x12~\n\x13GetLatestMarketData\x12+.datanode.api.v2.GetLatestMarketDataRequest\x1a,.datanode.api.v2.GetLatestMarketDataResponse"\x0c\x92\x41\t\n\x07Markets\x12\x81\x01\n\x14ListLatestMarketData\x12,.datanode.api.v2.ListLatestMarketDataRequest\x1a-.datanode.api.v2.ListLatestMarketDataResponse"\x0c\x92\x41\t\n\x07Markets\x12\x81\x01\n\x14GetLatestMarketDepth\x12,.datanode.api.v2.GetLatestMarketDepthRequest\x1a-.datanode.api.v2.GetLatestMarketDepthResponse"\x0c\x92\x41\t\n\x07Markets\x12\x80\x01\n\x13ObserveMarketsDepth\x12+.datanode.api.v2.ObserveMarketsDepthRequest\x1a,.datanode.api.v2.ObserveMarketsDepthResponse"\x0c\x92\x41\t\n\x07Markets0\x01\x12\x95\x01\n\x1aObserveMarketsDepthUpdates\x12\x32.datanode.api.v2.ObserveMarketsDepthUpdatesRequest\x1a\x33.datanode.api.v2.ObserveMarketsDepthUpdatesResponse"\x0c\x92\x41\t\n\x07Markets0\x01\x12}\n\x12ObserveMarketsData\x12*.datanode.api.v2.ObserveMarketsDataRequest\x1a+.datanode.api.v2.ObserveMarketsDataResponse"\x0c\x92\x41\t\n\x07Markets0\x01\x12\x8d\x01\n\x18GetMarketDataHistoryByID\x12\x30.datanode.api.v2.GetMarketDataHistoryByIDRequest\x1a\x31.datanode.api.v2.GetMarketDataHistoryByIDResponse"\x0c\x92\x41\t\n\x07Markets\x12n\n\rListTransfers\x12%.datanode.api.v2.ListTransfersRequest\x1a&.datanode.api.v2.ListTransfersResponse"\x0e\x92\x41\x0b\n\tTransfers\x12u\n\x10GetNetworkLimits\x12(.datanode.api.v2.GetNetworkLimitsRequest\x1a).datanode.api.v2.GetNetworkLimitsResponse"\x0c\x92\x41\t\n\x07Network\x12o\n\x0eListCandleData\x12&.datanode.api.v2.ListCandleDataRequest\x1a\'.datanode.api.v2.ListCandleDataResponse"\x0c\x92\x41\t\n\x07\x43\x61ndles\x12z\n\x11ObserveCandleData\x12).datanode.api.v2.ObserveCandleDataRequest\x1a*.datanode.api.v2.ObserveCandleDataResponse"\x0c\x92\x41\t\n\x07\x43\x61ndles0\x01\x12~\n\x13ListCandleIntervals\x12+.datanode.api.v2.ListCandleIntervalsRequest\x1a,.datanode.api.v2.ListCandleIntervalsResponse"\x0c\x92\x41\t\n\x07\x43\x61ndles\x12\x63\n\tListVotes\x12!.datanode.api.v2.ListVotesRequest\x1a".datanode.api.v2.ListVotesResponse"\x0f\x92\x41\x0c\n\nGovernance\x12n\n\x0cObserveVotes\x12$.datanode.api.v2.ObserveVotesRequest\x1a%.datanode.api.v2.ObserveVotesResponse"\x0f\x92\x41\x0c\n\nGovernance0\x01\x12\xb3\x01\n#ListERC20MultiSigSignerAddedBundles\x12;.datanode.api.v2.ListERC20MultiSigSignerAddedBundlesRequest\x1a<.datanode.api.v2.ListERC20MultiSigSignerAddedBundlesResponse"\x11\x92\x41\x0e\n\x0c\x45RC20 bridge\x12\xb9\x01\n%ListERC20MultiSigSignerRemovedBundles\x12=.datanode.api.v2.ListERC20MultiSigSignerRemovedBundlesRequest\x1a>.datanode.api.v2.ListERC20MultiSigSignerRemovedBundlesResponse"\x11\x92\x41\x0e\n\x0c\x45RC20 bridge\x12\x8f\x01\n\x17GetERC20ListAssetBundle\x12/.datanode.api.v2.GetERC20ListAssetBundleRequest\x1a\x30.datanode.api.v2.GetERC20ListAssetBundleResponse"\x11\x92\x41\x0e\n\x0c\x45RC20 bridge\x12\x9e\x01\n\x1cGetERC20SetAssetLimitsBundle\x12\x34.datanode.api.v2.GetERC20SetAssetLimitsBundleRequest\x1a\x35.datanode.api.v2.GetERC20SetAssetLimitsBundleResponse"\x11\x92\x41\x0e\n\x0c\x45RC20 bridge\x12\x98\x01\n\x1aGetERC20WithdrawalApproval\x12\x32.datanode.api.v2.GetERC20WithdrawalApprovalRequest\x1a\x33.datanode.api.v2.GetERC20WithdrawalApprovalResponse"\x11\x92\x41\x0e\n\x0c\x45RC20 bridge\x12h\n\x0cGetLastTrade\x12$.datanode.api.v2.GetLastTradeRequest\x1a%.datanode.api.v2.GetLastTradeResponse"\x0b\x92\x41\x08\n\x06Trades\x12\x62\n\nListTrades\x12".datanode.api.v2.ListTradesRequest\x1a#.datanode.api.v2.ListTradesResponse"\x0b\x92\x41\x08\n\x06Trades\x12m\n\rObserveTrades\x12%.datanode.api.v2.ObserveTradesRequest\x1a&.datanode.api.v2.ObserveTradesResponse"\x0b\x92\x41\x08\n\x06Trades0\x01\x12q\n\rGetOracleSpec\x12%.datanode.api.v2.GetOracleSpecRequest\x1a&.datanode.api.v2.GetOracleSpecResponse"\x11\x92\x41\x0e\n\x0c\x44\x61ta sources\x12w\n\x0fListOracleSpecs\x12\'.datanode.api.v2.ListOracleSpecsRequest\x1a(.datanode.api.v2.ListOracleSpecsResponse"\x11\x92\x41\x0e\n\x0c\x44\x61ta sources\x12t\n\x0eListOracleData\x12&.datanode.api.v2.ListOracleDataRequest\x1a\'.datanode.api.v2.ListOracleDataResponse"\x11\x92\x41\x0e\n\x0c\x44\x61ta sources\x12`\n\tGetMarket\x12!.datanode.api.v2.GetMarketRequest\x1a".datanode.api.v2.GetMarketResponse"\x0c\x92\x41\t\n\x07Markets\x12\x66\n\x0bListMarkets\x12#.datanode.api.v2.ListMarketsRequest\x1a$.datanode.api.v2.ListMarketsResponse"\x0c\x92\x41\t\n\x07Markets\x12]\n\x08GetParty\x12 .datanode.api.v2.GetPartyRequest\x1a!.datanode.api.v2.GetPartyResponse"\x0c\x92\x41\t\n\x07Parties\x12\x66\n\x0bListParties\x12#.datanode.api.v2.ListPartiesRequest\x1a$.datanode.api.v2.ListPartiesResponse"\x0c\x92\x41\t\n\x07Parties\x12{\n\x10ListMarginLevels\x12(.datanode.api.v2.ListMarginLevelsRequest\x1a).datanode.api.v2.ListMarginLevelsResponse"\x12\x92\x41\x0f\n\rMargin levels\x12\x86\x01\n\x13ObserveMarginLevels\x12+.datanode.api.v2.ObserveMarginLevelsRequest\x1a,.datanode.api.v2.ObserveMarginLevelsResponse"\x12\x92\x41\x0f\n\rMargin levels0\x01\x12\x66\n\x0bListRewards\x12#.datanode.api.v2.ListRewardsRequest\x1a$.datanode.api.v2.ListRewardsResponse"\x0c\x92\x41\t\n\x07Rewards\x12~\n\x13ListRewardSummaries\x12+.datanode.api.v2.ListRewardSummariesRequest\x1a,.datanode.api.v2.ListRewardSummariesResponse"\x0c\x92\x41\t\n\x07Rewards\x12\x8d\x01\n\x18ListEpochRewardSummaries\x12\x30.datanode.api.v2.ListEpochRewardSummariesRequest\x1a\x31.datanode.api.v2.ListEpochRewardSummariesResponse"\x0c\x92\x41\t\n\x07Rewards\x12\x62\n\nGetDeposit\x12".datanode.api.v2.GetDepositRequest\x1a#.datanode.api.v2.GetDepositResponse"\x0b\x92\x41\x08\n\x06\x41ssets\x12h\n\x0cListDeposits\x12$.datanode.api.v2.ListDepositsRequest\x1a%.datanode.api.v2.ListDepositsResponse"\x0b\x92\x41\x08\n\x06\x41ssets\x12k\n\rGetWithdrawal\x12%.datanode.api.v2.GetWithdrawalRequest\x1a&.datanode.api.v2.GetWithdrawalResponse"\x0b\x92\x41\x08\n\x06\x41ssets\x12q\n\x0fListWithdrawals\x12\'.datanode.api.v2.ListWithdrawalsRequest\x1a(.datanode.api.v2.ListWithdrawalsResponse"\x0b\x92\x41\x08\n\x06\x41ssets\x12\\\n\x08GetAsset\x12 .datanode.api.v2.GetAssetRequest\x1a!.datanode.api.v2.GetAssetResponse"\x0b\x92\x41\x08\n\x06\x41ssets\x12\x62\n\nListAssets\x12".datanode.api.v2.ListAssetsRequest\x1a#.datanode.api.v2.ListAssetsResponse"\x0b\x92\x41\x08\n\x06\x41ssets\x12\x97\x01\n\x17ListLiquidityProvisions\x12/.datanode.api.v2.ListLiquidityProvisionsRequest\x1a\x30.datanode.api.v2.ListLiquidityProvisionsResponse"\x19\x92\x41\x16\n\x14Liquidity provisions\x12\xa2\x01\n\x1aObserveLiquidityProvisions\x12\x32.datanode.api.v2.ObserveLiquidityProvisionsRequest\x1a\x33.datanode.api.v2.ObserveLiquidityProvisionsResponse"\x19\x92\x41\x16\n\x14Liquidity provisions0\x01\x12{\n\x11GetGovernanceData\x12).datanode.api.v2.GetGovernanceDataRequest\x1a*.datanode.api.v2.GetGovernanceDataResponse"\x0f\x92\x41\x0c\n\nGovernance\x12~\n\x12ListGovernanceData\x12*.datanode.api.v2.ListGovernanceDataRequest\x1a+.datanode.api.v2.ListGovernanceDataResponse"\x0f\x92\x41\x0c\n\nGovernance\x12}\n\x11ObserveGovernance\x12).datanode.api.v2.ObserveGovernanceRequest\x1a*.datanode.api.v2.ObserveGovernanceResponse"\x0f\x92\x41\x0c\n\nGovernance0\x01\x12r\n\x0fListDelegations\x12\'.datanode.api.v2.ListDelegationsRequest\x1a(.datanode.api.v2.ListDelegationsResponse"\x0c\x92\x41\t\n\x07Network\x12o\n\x0eGetNetworkData\x12&.datanode.api.v2.GetNetworkDataRequest\x1a\'.datanode.api.v2.GetNetworkDataResponse"\x0c\x92\x41\t\n\x07Network\x12Z\n\x07GetNode\x12\x1f.datanode.api.v2.GetNodeRequest\x1a .datanode.api.v2.GetNodeResponse"\x0c\x92\x41\t\n\x07Network\x12`\n\tListNodes\x12!.datanode.api.v2.ListNodesRequest\x1a".datanode.api.v2.ListNodesResponse"\x0c\x92\x41\t\n\x07Network\x12\x80\x01\n\x12ListNodeSignatures\x12*.datanode.api.v2.ListNodeSignaturesRequest\x1a+.datanode.api.v2.ListNodeSignaturesResponse"\x11\x92\x41\x0e\n\x0c\x45RC20 bridge\x12]\n\x08GetEpoch\x12 .datanode.api.v2.GetEpochRequest\x1a!.datanode.api.v2.GetEpochResponse"\x0c\x92\x41\t\n\x07Network\x12\x65\n\x0b\x45stimateFee\x12#.datanode.api.v2.EstimateFeeRequest\x1a$.datanode.api.v2.EstimateFeeResponse"\x0b\x92\x41\x08\n\x06Orders\x12n\n\x0e\x45stimateMargin\x12&.datanode.api.v2.EstimateMarginRequest\x1a\'.datanode.api.v2.EstimateMarginResponse"\x0b\x92\x41\x08\n\x06Orders\x12w\n\x10\x45stimatePosition\x12(.datanode.api.v2.EstimatePositionRequest\x1a).datanode.api.v2.EstimatePositionResponse"\x0e\x92\x41\x0b\n\tPositions\x12\x84\x01\n\x15ListNetworkParameters\x12-.datanode.api.v2.ListNetworkParametersRequest\x1a..datanode.api.v2.ListNetworkParametersResponse"\x0c\x92\x41\t\n\x07Network\x12~\n\x13GetNetworkParameter\x12+.datanode.api.v2.GetNetworkParameterRequest\x1a,.datanode.api.v2.GetNetworkParameterResponse"\x0c\x92\x41\t\n\x07Network\x12r\n\x0fListCheckpoints\x12\'.datanode.api.v2.ListCheckpointsRequest\x1a(.datanode.api.v2.ListCheckpointsResponse"\x0c\x92\x41\t\n\x07Network\x12]\n\x08GetStake\x12 .datanode.api.v2.GetStakeRequest\x1a!.datanode.api.v2.GetStakeResponse"\x0c\x92\x41\t\n\x07Network\x12o\n\x0eGetRiskFactors\x12&.datanode.api.v2.GetRiskFactorsRequest\x1a\'.datanode.api.v2.GetRiskFactorsResponse"\x0c\x92\x41\t\n\x07Markets\x12u\n\x0fObserveEventBus\x12\'.datanode.api.v2.ObserveEventBusRequest\x1a(.datanode.api.v2.ObserveEventBusResponse"\x0b\x92\x41\x08\n\x06\x45vents(\x01\x30\x01\x12\x92\x01\n\x16ObserveLedgerMovements\x12..datanode.api.v2.ObserveLedgerMovementsRequest\x1a/.datanode.api.v2.ObserveLedgerMovementsResponse"\x15\x92\x41\x12\n\x10Ledger movements0\x01\x12u\n\x10ListKeyRotations\x12(.datanode.api.v2.ListKeyRotationsRequest\x1a).datanode.api.v2.ListKeyRotationsResponse"\x0c\x92\x41\t\n\x07Network\x12\x8d\x01\n\x18ListEthereumKeyRotations\x12\x30.datanode.api.v2.ListEthereumKeyRotationsRequest\x1a\x31.datanode.api.v2.ListEthereumKeyRotationsResponse"\x0c\x92\x41\t\n\x07Network\x12\x66\n\x0bGetVegaTime\x12#.datanode.api.v2.GetVegaTimeRequest\x1a$.datanode.api.v2.GetVegaTimeResponse"\x0c\x92\x41\t\n\x07Network\x12\x8d\x01\n\x18GetProtocolUpgradeStatus\x12\x30.datanode.api.v2.GetProtocolUpgradeStatusRequest\x1a\x31.datanode.api.v2.GetProtocolUpgradeStatusResponse"\x0c\x92\x41\t\n\x07Network\x12\x99\x01\n\x1cListProtocolUpgradeProposals\x12\x34.datanode.api.v2.ListProtocolUpgradeProposalsRequest\x1a\x35.datanode.api.v2.ListProtocolUpgradeProposalsResponse"\x0c\x92\x41\t\n\x07Network\x12x\n\x11ListCoreSnapshots\x12).datanode.api.v2.ListCoreSnapshotsRequest\x1a*.datanode.api.v2.ListCoreSnapshotsResponse"\x0c\x92\x41\t\n\x07Network\x12\xb3\x01\n"GetMostRecentNetworkHistorySegment\x12:.datanode.api.v2.GetMostRecentNetworkHistorySegmentRequest\x1a;.datanode.api.v2.GetMostRecentNetworkHistorySegmentResponse"\x14\x92\x41\x11\n\x0fNetwork history\x12\xa4\x01\n\x1dListAllNetworkHistorySegments\x12\x35.datanode.api.v2.ListAllNetworkHistorySegmentsRequest\x1a\x36.datanode.api.v2.ListAllNetworkHistorySegmentsResponse"\x14\x92\x41\x11\n\x0fNetwork history\x12\xb9\x01\n$GetActiveNetworkHistoryPeerAddresses\x12<.datanode.api.v2.GetActiveNetworkHistoryPeerAddressesRequest\x1a=.datanode.api.v2.GetActiveNetworkHistoryPeerAddressesResponse"\x14\x92\x41\x11\n\x0fNetwork history\x12\x92\x01\n\x17GetNetworkHistoryStatus\x12/.datanode.api.v2.GetNetworkHistoryStatusRequest\x1a\x30.datanode.api.v2.GetNetworkHistoryStatusResponse"\x14\x92\x41\x11\n\x0fNetwork history\x12\xaa\x01\n\x1fGetNetworkHistoryBootstrapPeers\x12\x37.datanode.api.v2.GetNetworkHistoryBootstrapPeersRequest\x1a\x38.datanode.api.v2.GetNetworkHistoryBootstrapPeersResponse"\x14\x92\x41\x11\n\x0fNetwork history\x12j\n\x0cListEntities\x12$.datanode.api.v2.ListEntitiesRequest\x1a%.datanode.api.v2.ListEntitiesResponse"\r\x92\x41\n\n\x08\x45xplorer\x12r\n\x14\x45xportNetworkHistory\x12,.datanode.api.v2.ExportNetworkHistoryRequest\x1a\x14.google.api.HttpBody"\x14\x92\x41\x11\n\x0fNetwork history0\x01\x12N\n\x04Ping\x12\x1c.datanode.api.v2.PingRequest\x1a\x1d.datanode.api.v2.PingResponse"\t\x92\x41\x06\n\x04MiscB\xc6\x01Z1code.vegaprotocol.io/vega/protos/data-node/api/v2\x92\x41\x8f\x01\x12\x1e\n\x13Vega data node APIs2\x07v0.71.4\x1a\x1chttps://api.testnet.vega.xyz*\x02\x01\x02\x32\x10\x61pplication/jsonR9\n\x03\x35\x30\x30\x12\x32\n\x18\x41n internal server error\x12\x16\n\x14\x1a\x12.google.rpc.Statusb\x06proto3'
+    b'\n#data-node/api/v2/trading_data.proto\x12\x0f\x64\x61tanode.api.v2\x1a\x1fgoogle/api/field_behavior.proto\x1a\x19google/api/httpbody.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\x1a\x11vega/assets.proto\x1a)vega/commands/v1/validator_commands.proto\x1a\x1bvega/events/v1/events.proto\x1a\x15vega/governance.proto\x1a\x12vega/markets.proto\x1a\x11vega/oracle.proto\x1a\x0fvega/vega.proto"\xd9\x01\n\nPagination\x12\x19\n\x05\x66irst\x18\x01 \x01(\x05H\x00R\x05\x66irst\x88\x01\x01\x12\x19\n\x05\x61\x66ter\x18\x02 \x01(\tH\x01R\x05\x61\x66ter\x88\x01\x01\x12\x17\n\x04last\x18\x03 \x01(\x05H\x02R\x04last\x88\x01\x01\x12\x1b\n\x06\x62\x65\x66ore\x18\x04 \x01(\tH\x03R\x06\x62\x65\x66ore\x88\x01\x01\x12&\n\x0cnewest_first\x18\x05 \x01(\x08H\x04R\x0bnewestFirst\x88\x01\x01\x42\x08\n\x06_firstB\x08\n\x06_afterB\x07\n\x05_lastB\t\n\x07_beforeB\x0f\n\r_newest_first"\x9c\x01\n\x08PageInfo\x12"\n\rhas_next_page\x18\x01 \x01(\x08R\x0bhasNextPage\x12*\n\x11has_previous_page\x18\x02 \x01(\x08R\x0fhasPreviousPage\x12!\n\x0cstart_cursor\x18\x03 \x01(\tR\x0bstartCursor\x12\x1d\n\nend_cursor\x18\x04 \x01(\tR\tendCursor"\x9a\x01\n\x0e\x41\x63\x63ountBalance\x12\x14\n\x05owner\x18\x02 \x01(\tR\x05owner\x12\x18\n\x07\x62\x61lance\x18\x03 \x01(\tR\x07\x62\x61lance\x12\x14\n\x05\x61sset\x18\x04 \x01(\tR\x05\x61sset\x12\x1b\n\tmarket_id\x18\x05 \x01(\tR\x08marketId\x12%\n\x04type\x18\x06 \x01(\x0e\x32\x11.vega.AccountTypeR\x04type"\x9e\x01\n\x13ListAccountsRequest\x12\x36\n\x06\x66ilter\x18\x01 \x01(\x0b\x32\x1e.datanode.api.v2.AccountFilterR\x06\x66ilter\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"W\n\x14ListAccountsResponse\x12?\n\x08\x61\x63\x63ounts\x18\x01 \x01(\x0b\x32#.datanode.api.v2.AccountsConnectionR\x08\x61\x63\x63ounts"\x80\x01\n\x12\x41\x63\x63ountsConnection\x12\x32\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1c.datanode.api.v2.AccountEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"Z\n\x0b\x41\x63\x63ountEdge\x12\x33\n\x04node\x18\x01 \x01(\x0b\x32\x1f.datanode.api.v2.AccountBalanceR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x8d\x01\n\x16ObserveAccountsRequest\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x14\n\x05\x61sset\x18\x03 \x01(\tR\x05\x61sset\x12%\n\x04type\x18\x04 \x01(\x0e\x32\x11.vega.AccountTypeR\x04type"\xa6\x01\n\x17ObserveAccountsResponse\x12\x42\n\x08snapshot\x18\x01 \x01(\x0b\x32$.datanode.api.v2.AccountSnapshotPageH\x00R\x08snapshot\x12;\n\x07updates\x18\x02 \x01(\x0b\x32\x1f.datanode.api.v2.AccountUpdatesH\x00R\x07updatesB\n\n\x08response"o\n\x13\x41\x63\x63ountSnapshotPage\x12;\n\x08\x61\x63\x63ounts\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.AccountBalanceR\x08\x61\x63\x63ounts\x12\x1b\n\tlast_page\x18\x02 \x01(\x08R\x08lastPage"M\n\x0e\x41\x63\x63ountUpdates\x12;\n\x08\x61\x63\x63ounts\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.AccountBalanceR\x08\x61\x63\x63ounts"\r\n\x0bInfoRequest"I\n\x0cInfoResponse\x12\x18\n\x07version\x18\x01 \x01(\tR\x07version\x12\x1f\n\x0b\x63ommit_hash\x18\x02 \x01(\tR\ncommitHash"]\n\x0fGetOrderRequest\x12\x1f\n\x08order_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x07orderId\x12\x1d\n\x07version\x18\x02 \x01(\x05H\x00R\x07version\x88\x01\x01\x42\n\n\x08_version"5\n\x10GetOrderResponse\x12!\n\x05order\x18\x01 \x01(\x0b\x32\x0b.vega.OrderR\x05order"\xbd\x03\n\x0bOrderFilter\x12.\n\x08statuses\x18\x01 \x03(\x0e\x32\x12.vega.Order.StatusR\x08statuses\x12&\n\x05types\x18\x02 \x03(\x0e\x32\x10.vega.Order.TypeR\x05types\x12=\n\x0etime_in_forces\x18\x03 \x03(\x0e\x32\x17.vega.Order.TimeInForceR\x0ctimeInForces\x12+\n\x11\x65xclude_liquidity\x18\x04 \x01(\x08R\x10\x65xcludeLiquidity\x12\x1b\n\tparty_ids\x18\x05 \x03(\tR\x08partyIds\x12\x1d\n\nmarket_ids\x18\x06 \x03(\tR\tmarketIds\x12!\n\treference\x18\x07 \x01(\tH\x00R\treference\x88\x01\x01\x12>\n\ndate_range\x18\x08 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x01R\tdateRange\x88\x01\x01\x12 \n\tlive_only\x18\t \x01(\x08H\x02R\x08liveOnly\x88\x01\x01\x42\x0c\n\n_referenceB\r\n\x0b_date_rangeB\x0c\n\n_live_only"\xaa\x01\n\x11ListOrdersRequest\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12\x39\n\x06\x66ilter\x18\x05 \x01(\x0b\x32\x1c.datanode.api.v2.OrderFilterH\x01R\x06\x66ilter\x88\x01\x01\x42\r\n\x0b_paginationB\t\n\x07_filter"N\n\x12ListOrdersResponse\x12\x38\n\x06orders\x18\x01 \x01(\x0b\x32 .datanode.api.v2.OrderConnectionR\x06orders"\x8c\x01\n\x18ListOrderVersionsRequest\x12\x1f\n\x08order_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x07orderId\x12@\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"U\n\x19ListOrderVersionsResponse\x12\x38\n\x06orders\x18\x01 \x01(\x0b\x32 .datanode.api.v2.OrderConnectionR\x06orders"\x9a\x01\n\x14ObserveOrdersRequest\x12\x1d\n\nmarket_ids\x18\x01 \x03(\tR\tmarketIds\x12\x1b\n\tparty_ids\x18\x02 \x03(\tR\x08partyIds\x12\x30\n\x11\x65xclude_liquidity\x18\x03 \x01(\x08H\x00R\x10\x65xcludeLiquidity\x88\x01\x01\x42\x14\n\x12_exclude_liquidity"\xa0\x01\n\x15ObserveOrdersResponse\x12@\n\x08snapshot\x18\x01 \x01(\x0b\x32".datanode.api.v2.OrderSnapshotPageH\x00R\x08snapshot\x12\x39\n\x07updates\x18\x02 \x01(\x0b\x32\x1d.datanode.api.v2.OrderUpdatesH\x00R\x07updatesB\n\n\x08response"U\n\x11OrderSnapshotPage\x12#\n\x06orders\x18\x01 \x03(\x0b\x32\x0b.vega.OrderR\x06orders\x12\x1b\n\tlast_page\x18\x02 \x01(\x08R\x08lastPage"3\n\x0cOrderUpdates\x12#\n\x06orders\x18\x01 \x03(\x0b\x32\x0b.vega.OrderR\x06orders"\xa3\x01\n\x14ListPositionsRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01:\x02\x18\x01\x42\r\n\x0b_pagination"^\n\x15ListPositionsResponse\x12\x41\n\tpositions\x18\x01 \x01(\x0b\x32#.datanode.api.v2.PositionConnectionR\tpositions:\x02\x18\x01"M\n\x0fPositionsFilter\x12\x1b\n\tparty_ids\x18\x01 \x03(\tR\x08partyIds\x12\x1d\n\nmarket_ids\x18\x02 \x03(\tR\tmarketIds"\xa4\x01\n\x17ListAllPositionsRequest\x12\x38\n\x06\x66ilter\x18\x01 \x01(\x0b\x32 .datanode.api.v2.PositionsFilterR\x06\x66ilter\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"]\n\x18ListAllPositionsResponse\x12\x41\n\tpositions\x18\x01 \x01(\x0b\x32#.datanode.api.v2.PositionConnectionR\tpositions"J\n\x0cPositionEdge\x12"\n\x04node\x18\x01 \x01(\x0b\x32\x0e.vega.PositionR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x81\x01\n\x12PositionConnection\x12\x33\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1d.datanode.api.v2.PositionEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"v\n\x17ObservePositionsRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12 \n\tmarket_id\x18\x02 \x01(\tH\x01R\x08marketId\x88\x01\x01\x42\x0b\n\t_party_idB\x0c\n\n_market_id"\xa9\x01\n\x18ObservePositionsResponse\x12\x43\n\x08snapshot\x18\x01 \x01(\x0b\x32%.datanode.api.v2.PositionSnapshotPageH\x00R\x08snapshot\x12<\n\x07updates\x18\x02 \x01(\x0b\x32 .datanode.api.v2.PositionUpdatesH\x00R\x07updatesB\n\n\x08response"a\n\x14PositionSnapshotPage\x12,\n\tpositions\x18\x01 \x03(\x0b\x32\x0e.vega.PositionR\tpositions\x12\x1b\n\tlast_page\x18\x02 \x01(\x08R\x08lastPage"?\n\x0fPositionUpdates\x12,\n\tpositions\x18\x01 \x03(\x0b\x32\x0e.vega.PositionR\tpositions"\xa3\x02\n\x11LedgerEntryFilter\x12\x37\n\x18\x63lose_on_account_filters\x18\x01 \x01(\x08R\x15\x63loseOnAccountFilters\x12N\n\x13\x66rom_account_filter\x18\x02 \x01(\x0b\x32\x1e.datanode.api.v2.AccountFilterR\x11\x66romAccountFilter\x12J\n\x11to_account_filter\x18\x03 \x01(\x0b\x32\x1e.datanode.api.v2.AccountFilterR\x0ftoAccountFilter\x12\x39\n\x0etransfer_types\x18\x05 \x03(\x0e\x32\x12.vega.TransferTypeR\rtransferTypes"\xd9\x05\n\x15\x41ggregatedLedgerEntry\x12\x1c\n\ttimestamp\x18\x02 \x01(\x03R\ttimestamp\x12\x1a\n\x08quantity\x18\x03 \x01(\tR\x08quantity\x12\x37\n\rtransfer_type\x18\x04 \x01(\x0e\x32\x12.vega.TransferTypeR\x0ctransferType\x12\x1e\n\x08\x61sset_id\x18\x05 \x01(\tH\x00R\x07\x61ssetId\x88\x01\x01\x12=\n\x11\x66rom_account_type\x18\x06 \x01(\x0e\x32\x11.vega.AccountTypeR\x0f\x66romAccountType\x12\x39\n\x0fto_account_type\x18\x07 \x01(\x0e\x32\x11.vega.AccountTypeR\rtoAccountType\x12\x36\n\x15\x66rom_account_party_id\x18\x08 \x01(\tH\x01R\x12\x66romAccountPartyId\x88\x01\x01\x12\x32\n\x13to_account_party_id\x18\t \x01(\tH\x02R\x10toAccountPartyId\x88\x01\x01\x12\x38\n\x16\x66rom_account_market_id\x18\n \x01(\tH\x03R\x13\x66romAccountMarketId\x88\x01\x01\x12\x34\n\x14to_account_market_id\x18\x0b \x01(\tH\x04R\x11toAccountMarketId\x88\x01\x01\x12\x30\n\x14\x66rom_account_balance\x18\x0c \x01(\tR\x12\x66romAccountBalance\x12,\n\x12to_account_balance\x18\r \x01(\tR\x10toAccountBalanceB\x0b\n\t_asset_idB\x18\n\x16_from_account_party_idB\x16\n\x14_to_account_party_idB\x19\n\x17_from_account_market_idB\x17\n\x15_to_account_market_idJ\x04\x08\x01\x10\x02"\xf6\x01\n\x18ListLedgerEntriesRequest\x12:\n\x06\x66ilter\x18\x01 \x01(\x0b\x32".datanode.api.v2.LedgerEntryFilterR\x06\x66ilter\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12>\n\ndate_range\x18\x03 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x01R\tdateRange\x88\x01\x01\x42\r\n\x0b_paginationB\r\n\x0b_date_range"\xad\x01\n\x1a\x45xportLedgerEntriesRequest\x12\x1f\n\x08party_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x07partyId\x12\x1f\n\x08\x61sset_id\x18\x02 \x01(\tB\x04\xe2\x41\x01\x02R\x07\x61ssetId\x12>\n\ndate_range\x18\x04 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x00R\tdateRange\x88\x01\x01\x42\r\n\x0b_date_range"v\n\x19ListLedgerEntriesResponse\x12Y\n\x0eledger_entries\x18\x01 \x01(\x0b\x32\x32.datanode.api.v2.AggregatedLedgerEntriesConnectionR\rledgerEntries"q\n\x1b\x41ggregatedLedgerEntriesEdge\x12:\n\x04node\x18\x01 \x01(\x0b\x32&.datanode.api.v2.AggregatedLedgerEntryR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x9f\x01\n!AggregatedLedgerEntriesConnection\x12\x42\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32,.datanode.api.v2.AggregatedLedgerEntriesEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xf3\x01\n\x19ListBalanceChangesRequest\x12\x36\n\x06\x66ilter\x18\x01 \x01(\x0b\x32\x1e.datanode.api.v2.AccountFilterR\x06\x66ilter\x12@\n\npagination\x18\x05 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12>\n\ndate_range\x18\x06 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x01R\tdateRange\x88\x01\x01\x42\r\n\x0b_paginationB\r\n\x0b_date_range"f\n\x1aListBalanceChangesResponse\x12H\n\x08\x62\x61lances\x18\x01 \x01(\x0b\x32,.datanode.api.v2.AggregatedBalanceConnectionR\x08\x62\x61lances"\xac\x02\n\x18GetBalanceHistoryRequest\x12\x36\n\x06\x66ilter\x18\x01 \x01(\x0b\x32\x1e.datanode.api.v2.AccountFilterR\x06\x66ilter\x12\x38\n\x08group_by\x18\x02 \x03(\x0e\x32\x1d.datanode.api.v2.AccountFieldR\x07groupBy\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12>\n\ndate_range\x18\x04 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x01R\tdateRange\x88\x01\x01\x42\r\n\x0b_paginationB\r\n\x0b_date_range"e\n\x19GetBalanceHistoryResponse\x12H\n\x08\x62\x61lances\x18\x01 \x01(\x0b\x32,.datanode.api.v2.AggregatedBalanceConnectionR\x08\x62\x61lances"g\n\x15\x41ggregatedBalanceEdge\x12\x36\n\x04node\x18\x01 \x01(\x0b\x32".datanode.api.v2.AggregatedBalanceR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x93\x01\n\x1b\x41ggregatedBalanceConnection\x12<\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32&.datanode.api.v2.AggregatedBalanceEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\x9e\x01\n\rAccountFilter\x12\x19\n\x08\x61sset_id\x18\x01 \x01(\tR\x07\x61ssetId\x12\x1b\n\tparty_ids\x18\x02 \x03(\tR\x08partyIds\x12\x1d\n\nmarket_ids\x18\x03 \x03(\tR\tmarketIds\x12\x36\n\raccount_types\x18\x04 \x03(\x0e\x32\x11.vega.AccountTypeR\x0c\x61\x63\x63ountTypes"\xa1\x02\n\x11\x41ggregatedBalance\x12\x1c\n\ttimestamp\x18\x01 \x01(\x03R\ttimestamp\x12\x18\n\x07\x62\x61lance\x18\x02 \x01(\tR\x07\x62\x61lance\x12\x1e\n\x08party_id\x18\x04 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12\x1e\n\x08\x61sset_id\x18\x05 \x01(\tH\x01R\x07\x61ssetId\x88\x01\x01\x12 \n\tmarket_id\x18\x06 \x01(\tH\x02R\x08marketId\x88\x01\x01\x12\x39\n\x0c\x61\x63\x63ount_type\x18\x07 \x01(\x0e\x32\x11.vega.AccountTypeH\x03R\x0b\x61\x63\x63ountType\x88\x01\x01\x42\x0b\n\t_party_idB\x0b\n\t_asset_idB\x0c\n\n_market_idB\x0f\n\r_account_type";\n\x1aObserveMarketsDepthRequest\x12\x1d\n\nmarket_ids\x18\x01 \x03(\tR\tmarketIds"S\n\x1bObserveMarketsDepthResponse\x12\x34\n\x0cmarket_depth\x18\x01 \x03(\x0b\x32\x11.vega.MarketDepthR\x0bmarketDepth"B\n!ObserveMarketsDepthUpdatesRequest\x12\x1d\n\nmarket_ids\x18\x01 \x03(\tR\tmarketIds"U\n"ObserveMarketsDepthUpdatesResponse\x12/\n\x06update\x18\x01 \x03(\x0b\x32\x17.vega.MarketDepthUpdateR\x06update":\n\x19ObserveMarketsDataRequest\x12\x1d\n\nmarket_ids\x18\x01 \x03(\tR\tmarketIds"O\n\x1aObserveMarketsDataResponse\x12\x31\n\x0bmarket_data\x18\x01 \x03(\x0b\x32\x10.vega.MarketDataR\nmarketData"p\n\x1bGetLatestMarketDepthRequest\x12!\n\tmarket_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x08marketId\x12 \n\tmax_depth\x18\x02 \x01(\x04H\x00R\x08maxDepth\x88\x01\x01\x42\x0c\n\n_max_depth"\xda\x01\n\x1cGetLatestMarketDepthResponse\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12"\n\x03\x62uy\x18\x02 \x03(\x0b\x32\x10.vega.PriceLevelR\x03\x62uy\x12$\n\x04sell\x18\x03 \x03(\x0b\x32\x10.vega.PriceLevelR\x04sell\x12*\n\nlast_trade\x18\x04 \x01(\x0b\x32\x0b.vega.TradeR\tlastTrade\x12\'\n\x0fsequence_number\x18\x05 \x01(\x04R\x0esequenceNumber"\x1d\n\x1bListLatestMarketDataRequest"S\n\x1cListLatestMarketDataResponse\x12\x33\n\x0cmarkets_data\x18\x01 \x03(\x0b\x32\x10.vega.MarketDataR\x0bmarketsData"?\n\x1aGetLatestMarketDataRequest\x12!\n\tmarket_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x08marketId"P\n\x1bGetLatestMarketDataResponse\x12\x31\n\x0bmarket_data\x18\x01 \x01(\x0b\x32\x10.vega.MarketDataR\nmarketData"\x99\x02\n\x1fGetMarketDataHistoryByIDRequest\x12!\n\tmarket_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x08marketId\x12,\n\x0fstart_timestamp\x18\x02 \x01(\x03H\x00R\x0estartTimestamp\x88\x01\x01\x12(\n\rend_timestamp\x18\x03 \x01(\x03H\x01R\x0c\x65ndTimestamp\x88\x01\x01\x12@\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x02R\npagination\x88\x01\x01\x42\x12\n\x10_start_timestampB\x10\n\x0e_end_timestampB\r\n\x0b_paginationJ\x04\x08\x05\x10\x06"j\n GetMarketDataHistoryByIDResponse\x12\x46\n\x0bmarket_data\x18\x01 \x01(\x0b\x32%.datanode.api.v2.MarketDataConnectionR\nmarketData"N\n\x0eMarketDataEdge\x12$\n\x04node\x18\x01 \x01(\x0b\x32\x10.vega.MarketDataR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x85\x01\n\x14MarketDataConnection\x12\x35\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.MarketDataEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xd1\x01\n\x14ListTransfersRequest\x12\x1b\n\x06pubkey\x18\x01 \x01(\tH\x00R\x06pubkey\x88\x01\x01\x12@\n\tdirection\x18\x02 \x01(\x0e\x32".datanode.api.v2.TransferDirectionR\tdirection\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x01R\npagination\x88\x01\x01\x42\t\n\x07_pubkeyB\r\n\x0b_pagination"Z\n\x15ListTransfersResponse\x12\x41\n\ttransfers\x18\x01 \x01(\x0b\x32#.datanode.api.v2.TransferConnectionR\ttransfers"T\n\x0cTransferEdge\x12,\n\x04node\x18\x01 \x01(\x0b\x32\x18.vega.events.v1.TransferR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x81\x01\n\x12TransferConnection\x12\x33\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1d.datanode.api.v2.TransferEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\x19\n\x17GetNetworkLimitsRequest"G\n\x18GetNetworkLimitsResponse\x12+\n\x06limits\x18\x01 \x01(\x0b\x32\x13.vega.NetworkLimitsR\x06limits"?\n\x1aListCandleIntervalsRequest\x12!\n\tmarket_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x08marketId"M\n\x12IntervalToCandleId\x12\x1a\n\x08interval\x18\x01 \x01(\tR\x08interval\x12\x1b\n\tcandle_id\x18\x02 \x01(\tR\x08\x63\x61ndleId"u\n\x1bListCandleIntervalsResponse\x12V\n\x15interval_to_candle_id\x18\x01 \x03(\x0b\x32#.datanode.api.v2.IntervalToCandleIdR\x12intervalToCandleId"\xa7\x01\n\x06\x43\x61ndle\x12\x14\n\x05start\x18\x01 \x01(\x03R\x05start\x12\x1f\n\x0blast_update\x18\x02 \x01(\x03R\nlastUpdate\x12\x12\n\x04high\x18\x03 \x01(\tR\x04high\x12\x10\n\x03low\x18\x04 \x01(\tR\x03low\x12\x12\n\x04open\x18\x05 \x01(\tR\x04open\x12\x14\n\x05\x63lose\x18\x06 \x01(\tR\x05\x63lose\x12\x16\n\x06volume\x18\x07 \x01(\x04R\x06volume"=\n\x18ObserveCandleDataRequest\x12!\n\tcandle_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x08\x63\x61ndleId"L\n\x19ObserveCandleDataResponse\x12/\n\x06\x63\x61ndle\x18\x01 \x01(\x0b\x32\x17.datanode.api.v2.CandleR\x06\x63\x61ndle"\xdb\x01\n\x15ListCandleDataRequest\x12!\n\tcandle_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x08\x63\x61ndleId\x12%\n\x0e\x66rom_timestamp\x18\x02 \x01(\x03R\rfromTimestamp\x12!\n\x0cto_timestamp\x18\x03 \x01(\x03R\x0btoTimestamp\x12@\n\npagination\x18\x05 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_paginationJ\x04\x08\x04\x10\x05"Y\n\x16ListCandleDataResponse\x12?\n\x07\x63\x61ndles\x18\x01 \x01(\x0b\x32%.datanode.api.v2.CandleDataConnectionR\x07\x63\x61ndles"Q\n\nCandleEdge\x12+\n\x04node\x18\x01 \x01(\x0b\x32\x17.datanode.api.v2.CandleR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x81\x01\n\x14\x43\x61ndleDataConnection\x12\x31\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1b.datanode.api.v2.CandleEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xc6\x01\n\x10ListVotesRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12$\n\x0bproposal_id\x18\x02 \x01(\tH\x01R\nproposalId\x88\x01\x01\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x02R\npagination\x88\x01\x01\x42\x0b\n\t_party_idB\x0e\n\x0c_proposal_idB\r\n\x0b_pagination"J\n\x11ListVotesResponse\x12\x35\n\x05votes\x18\x01 \x01(\x0b\x32\x1f.datanode.api.v2.VoteConnectionR\x05votes"B\n\x08VoteEdge\x12\x1e\n\x04node\x18\x01 \x01(\x0b\x32\n.vega.VoteR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"y\n\x0eVoteConnection\x12/\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x19.datanode.api.v2.VoteEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"x\n\x13ObserveVotesRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12$\n\x0bproposal_id\x18\x02 \x01(\tH\x01R\nproposalId\x88\x01\x01\x42\x0b\n\t_party_idB\x0e\n\x0c_proposal_id"6\n\x14ObserveVotesResponse\x12\x1e\n\x04vote\x18\x01 \x01(\x0b\x32\n.vega.VoteR\x04vote"\xbd\x01\n*ListERC20MultiSigSignerAddedBundlesRequest\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x1c\n\tsubmitter\x18\x02 \x01(\tR\tsubmitter\x12\x1b\n\tepoch_seq\x18\x03 \x01(\tR\x08\x65pochSeq\x12;\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationR\npagination"|\n+ListERC20MultiSigSignerAddedBundlesResponse\x12M\n\x07\x62undles\x18\x01 \x01(\x0b\x32\x33.datanode.api.v2.ERC20MultiSigSignerAddedConnectionR\x07\x62undles"t\n\x1c\x45RC20MultiSigSignerAddedEdge\x12<\n\x04node\x18\x01 \x01(\x0b\x32(.vega.events.v1.ERC20MultiSigSignerAddedR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x81\x01\n"ERC20MultiSigSignerAddedBundleEdge\x12\x43\n\x04node\x18\x01 \x01(\x0b\x32/.datanode.api.v2.ERC20MultiSigSignerAddedBundleR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\xa7\x01\n"ERC20MultiSigSignerAddedConnection\x12I\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x33.datanode.api.v2.ERC20MultiSigSignerAddedBundleEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xce\x01\n\x1e\x45RC20MultiSigSignerAddedBundle\x12\x1d\n\nnew_signer\x18\x01 \x01(\tR\tnewSigner\x12\x1c\n\tsubmitter\x18\x02 \x01(\tR\tsubmitter\x12\x14\n\x05nonce\x18\x04 \x01(\tR\x05nonce\x12\x1c\n\ttimestamp\x18\x05 \x01(\x03R\ttimestamp\x12\x1e\n\nsignatures\x18\x06 \x01(\tR\nsignatures\x12\x1b\n\tepoch_seq\x18\x03 \x01(\tR\x08\x65pochSeq"\xbf\x01\n,ListERC20MultiSigSignerRemovedBundlesRequest\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x1c\n\tsubmitter\x18\x02 \x01(\tR\tsubmitter\x12\x1b\n\tepoch_seq\x18\x03 \x01(\tR\x08\x65pochSeq\x12;\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationR\npagination"\x80\x01\n-ListERC20MultiSigSignerRemovedBundlesResponse\x12O\n\x07\x62undles\x18\x01 \x01(\x0b\x32\x35.datanode.api.v2.ERC20MultiSigSignerRemovedConnectionR\x07\x62undles"x\n\x1e\x45RC20MultiSigSignerRemovedEdge\x12>\n\x04node\x18\x01 \x01(\x0b\x32*.vega.events.v1.ERC20MultiSigSignerRemovedR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x85\x01\n$ERC20MultiSigSignerRemovedBundleEdge\x12\x45\n\x04node\x18\x01 \x01(\x0b\x32\x31.datanode.api.v2.ERC20MultiSigSignerRemovedBundleR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\xab\x01\n$ERC20MultiSigSignerRemovedConnection\x12K\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x35.datanode.api.v2.ERC20MultiSigSignerRemovedBundleEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xd0\x01\n ERC20MultiSigSignerRemovedBundle\x12\x1d\n\nold_signer\x18\x01 \x01(\tR\toldSigner\x12\x1c\n\tsubmitter\x18\x02 \x01(\tR\tsubmitter\x12\x14\n\x05nonce\x18\x04 \x01(\tR\x05nonce\x12\x1c\n\ttimestamp\x18\x05 \x01(\x03R\ttimestamp\x12\x1e\n\nsignatures\x18\x06 \x01(\tR\nsignatures\x12\x1b\n\tepoch_seq\x18\x07 \x01(\tR\x08\x65pochSeq"A\n\x1eGetERC20ListAssetBundleRequest\x12\x1f\n\x08\x61sset_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x07\x61ssetId"\x9e\x01\n\x1fGetERC20ListAssetBundleResponse\x12!\n\x0c\x61sset_source\x18\x01 \x01(\tR\x0b\x61ssetSource\x12"\n\rvega_asset_id\x18\x02 \x01(\tR\x0bvegaAssetId\x12\x14\n\x05nonce\x18\x03 \x01(\tR\x05nonce\x12\x1e\n\nsignatures\x18\x04 \x01(\tR\nsignatures"L\n#GetERC20SetAssetLimitsBundleRequest\x12%\n\x0bproposal_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\nproposalId"\xe8\x01\n$GetERC20SetAssetLimitsBundleResponse\x12!\n\x0c\x61sset_source\x18\x01 \x01(\tR\x0b\x61ssetSource\x12"\n\rvega_asset_id\x18\x02 \x01(\tR\x0bvegaAssetId\x12\x14\n\x05nonce\x18\x03 \x01(\tR\x05nonce\x12%\n\x0elifetime_limit\x18\x04 \x01(\tR\rlifetimeLimit\x12\x1c\n\tthreshold\x18\x05 \x01(\tR\tthreshold\x12\x1e\n\nsignatures\x18\x06 \x01(\tR\nsignatures"N\n!GetERC20WithdrawalApprovalRequest\x12)\n\rwithdrawal_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x0cwithdrawalId"\xde\x01\n"GetERC20WithdrawalApprovalResponse\x12!\n\x0c\x61sset_source\x18\x01 \x01(\tR\x0b\x61ssetSource\x12\x16\n\x06\x61mount\x18\x02 \x01(\tR\x06\x61mount\x12\x14\n\x05nonce\x18\x04 \x01(\tR\x05nonce\x12\x1e\n\nsignatures\x18\x05 \x01(\tR\nsignatures\x12%\n\x0etarget_address\x18\x06 \x01(\tR\rtargetAddress\x12\x1a\n\x08\x63reation\x18\x07 \x01(\x03R\x08\x63reationJ\x04\x08\x03\x10\x04"8\n\x13GetLastTradeRequest\x12!\n\tmarket_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x08marketId"9\n\x14GetLastTradeResponse\x12!\n\x05trade\x18\x01 \x01(\x0b\x32\x0b.vega.TradeR\x05trade"\x8c\x02\n\x11ListTradesRequest\x12\x1d\n\nmarket_ids\x18\x01 \x03(\tR\tmarketIds\x12\x1b\n\torder_ids\x18\x02 \x03(\tR\x08orderIds\x12\x1b\n\tparty_ids\x18\x03 \x03(\tR\x08partyIds\x12@\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12>\n\ndate_range\x18\x05 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x01R\tdateRange\x88\x01\x01\x42\r\n\x0b_paginationB\r\n\x0b_date_range"N\n\x12ListTradesResponse\x12\x38\n\x06trades\x18\x01 \x01(\x0b\x32 .datanode.api.v2.TradeConnectionR\x06trades"{\n\x0fTradeConnection\x12\x30\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1a.datanode.api.v2.TradeEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"D\n\tTradeEdge\x12\x1f\n\x04node\x18\x01 \x01(\x0b\x32\x0b.vega.TradeR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"R\n\x14ObserveTradesRequest\x12\x1d\n\nmarket_ids\x18\x01 \x03(\tR\tmarketIds\x12\x1b\n\tparty_ids\x18\x02 \x03(\tR\x08partyIds"<\n\x15ObserveTradesResponse\x12#\n\x06trades\x18\x01 \x03(\x0b\x32\x0b.vega.TradeR\x06trades"B\n\x14GetOracleSpecRequest\x12*\n\x0eoracle_spec_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x0coracleSpecId"J\n\x15GetOracleSpecResponse\x12\x31\n\x0boracle_spec\x18\x01 \x01(\x0b\x32\x10.vega.OracleSpecR\noracleSpec"i\n\x16ListOracleSpecsRequest\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"d\n\x17ListOracleSpecsResponse\x12I\n\x0coracle_specs\x18\x01 \x01(\x0b\x32&.datanode.api.v2.OracleSpecsConnectionR\x0boracleSpecs"\xa6\x01\n\x15ListOracleDataRequest\x12)\n\x0eoracle_spec_id\x18\x01 \x01(\tH\x00R\x0coracleSpecId\x88\x01\x01\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x01R\npagination\x88\x01\x01\x42\x11\n\x0f_oracle_spec_idB\r\n\x0b_pagination"`\n\x16ListOracleDataResponse\x12\x46\n\x0boracle_data\x18\x01 \x01(\x0b\x32%.datanode.api.v2.OracleDataConnectionR\noracleData"N\n\x0eOracleSpecEdge\x12$\n\x04node\x18\x01 \x01(\x0b\x32\x10.vega.OracleSpecR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x86\x01\n\x15OracleSpecsConnection\x12\x35\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.OracleSpecEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"N\n\x0eOracleDataEdge\x12$\n\x04node\x18\x01 \x01(\x0b\x32\x10.vega.OracleDataR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x85\x01\n\x14OracleDataConnection\x12\x35\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.OracleDataEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"5\n\x10GetMarketRequest\x12!\n\tmarket_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x08marketId"9\n\x11GetMarketResponse\x12$\n\x06market\x18\x01 \x01(\x0b\x32\x0c.vega.MarketR\x06market"\xa7\x01\n\x12ListMarketsRequest\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12,\n\x0finclude_settled\x18\x03 \x01(\x08H\x01R\x0eincludeSettled\x88\x01\x01\x42\r\n\x0b_paginationB\x12\n\x10_include_settled"R\n\x13ListMarketsResponse\x12;\n\x07markets\x18\x01 \x01(\x0b\x32!.datanode.api.v2.MarketConnectionR\x07markets"F\n\nMarketEdge\x12 \n\x04node\x18\x01 \x01(\x0b\x32\x0c.vega.MarketR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"}\n\x10MarketConnection\x12\x31\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1b.datanode.api.v2.MarketEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xaf\x01\n\x1bListSuccessorMarketsRequest\x12!\n\tmarket_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x08marketId\x12\x30\n\x14include_full_history\x18\x02 \x01(\x08R\x12includeFullHistory\x12;\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationR\npagination"k\n\x0fSuccessorMarket\x12$\n\x06market\x18\x01 \x01(\x0b\x32\x0c.vega.MarketR\x06market\x12\x32\n\tproposals\x18\x02 \x03(\x0b\x32\x14.vega.GovernanceDataR\tproposals"c\n\x13SuccessorMarketEdge\x12\x34\n\x04node\x18\x01 \x01(\x0b\x32 .datanode.api.v2.SuccessorMarketR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x8f\x01\n\x19SuccessorMarketConnection\x12:\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32$.datanode.api.v2.SuccessorMarketEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"d\n\x1cListSuccessorMarketsResponse\x12\x44\n\x07markets\x18\x01 \x01(\x0b\x32*.datanode.api.v2.SuccessorMarketConnectionR\x07markets"2\n\x0fGetPartyRequest\x12\x1f\n\x08party_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x07partyId"5\n\x10GetPartyResponse\x12!\n\x05party\x18\x01 \x01(\x0b\x32\x0b.vega.PartyR\x05party"l\n\x12ListPartiesRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12;\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationR\npagination"Q\n\x13ListPartiesResponse\x12:\n\x07parties\x18\x01 \x01(\x0b\x32 .datanode.api.v2.PartyConnectionR\x07parties"D\n\tPartyEdge\x12\x1f\n\x04node\x18\x01 \x01(\x0b\x32\x0b.vega.PartyR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"{\n\x0fPartyConnection\x12\x30\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1a.datanode.api.v2.PartyEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"D\n\tOrderEdge\x12\x1f\n\x04node\x18\x01 \x01(\x0b\x32\x0b.vega.OrderR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x8e\x01\n\x17ListMarginLevelsRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12;\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationR\npagination"b\n\x18ListMarginLevelsResponse\x12\x46\n\rmargin_levels\x18\x01 \x01(\x0b\x32!.datanode.api.v2.MarginConnectionR\x0cmarginLevels"g\n\x1aObserveMarginLevelsRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12 \n\tmarket_id\x18\x02 \x01(\tH\x00R\x08marketId\x88\x01\x01\x42\x0c\n\n_market_id"V\n\x1bObserveMarginLevelsResponse\x12\x37\n\rmargin_levels\x18\x01 \x01(\x0b\x32\x12.vega.MarginLevelsR\x0cmarginLevels"{\n\x0fOrderConnection\x12\x30\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1a.datanode.api.v2.OrderEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"L\n\nMarginEdge\x12&\n\x04node\x18\x01 \x01(\x0b\x32\x12.vega.MarginLevelsR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"}\n\x10MarginConnection\x12\x31\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1b.datanode.api.v2.MarginEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\x8d\x02\n\x12ListRewardsRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12\x1e\n\x08\x61sset_id\x18\x02 \x01(\tH\x00R\x07\x61ssetId\x88\x01\x01\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x01R\npagination\x88\x01\x01\x12"\n\nfrom_epoch\x18\x04 \x01(\x04H\x02R\tfromEpoch\x88\x01\x01\x12\x1e\n\x08to_epoch\x18\x05 \x01(\x04H\x03R\x07toEpoch\x88\x01\x01\x42\x0b\n\t_asset_idB\r\n\x0b_paginationB\r\n\x0b_from_epochB\x0b\n\t_to_epoch"S\n\x13ListRewardsResponse\x12<\n\x07rewards\x18\x01 \x01(\x0b\x32".datanode.api.v2.RewardsConnectionR\x07rewards"F\n\nRewardEdge\x12 \n\x04node\x18\x01 \x01(\x0b\x32\x0c.vega.RewardR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"~\n\x11RewardsConnection\x12\x31\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1b.datanode.api.v2.RewardEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xc7\x01\n\x1aListRewardSummariesRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12\x1e\n\x08\x61sset_id\x18\x02 \x01(\tH\x01R\x07\x61ssetId\x88\x01\x01\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x02R\npagination\x88\x01\x01\x42\x0b\n\t_party_idB\x0b\n\t_asset_idB\r\n\x0b_pagination"P\n\x1bListRewardSummariesResponse\x12\x31\n\tsummaries\x18\x01 \x03(\x0b\x32\x13.vega.RewardSummaryR\tsummaries"\xb1\x01\n\x13RewardSummaryFilter\x12\x1b\n\tasset_ids\x18\x01 \x03(\tR\x08\x61ssetIds\x12\x1d\n\nmarket_ids\x18\x02 \x03(\tR\tmarketIds\x12"\n\nfrom_epoch\x18\x03 \x01(\x04H\x00R\tfromEpoch\x88\x01\x01\x12\x1e\n\x08to_epoch\x18\x04 \x01(\x04H\x01R\x07toEpoch\x88\x01\x01\x42\r\n\x0b_from_epochB\x0b\n\t_to_epoch"\xb0\x01\n\x1fListEpochRewardSummariesRequest\x12<\n\x06\x66ilter\x18\x01 \x01(\x0b\x32$.datanode.api.v2.RewardSummaryFilterR\x06\x66ilter\x12@\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"o\n ListEpochRewardSummariesResponse\x12K\n\tsummaries\x18\x01 \x01(\x0b\x32-.datanode.api.v2.EpochRewardSummaryConnectionR\tsummaries"\x95\x01\n\x1c\x45pochRewardSummaryConnection\x12=\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\'.datanode.api.v2.EpochRewardSummaryEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"^\n\x16\x45pochRewardSummaryEdge\x12,\n\x04node\x18\x01 \x01(\x0b\x32\x18.vega.EpochRewardSummaryR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"q\n\x15ObserveRewardsRequest\x12\x1e\n\x08\x61sset_id\x18\x01 \x01(\tH\x00R\x07\x61ssetId\x88\x01\x01\x12\x1e\n\x08party_id\x18\x02 \x01(\tH\x01R\x07partyId\x88\x01\x01\x42\x0b\n\t_asset_idB\x0b\n\t_party_id">\n\x16ObserveRewardsResponse\x12$\n\x06reward\x18\x01 \x01(\x0b\x32\x0c.vega.RewardR\x06reward")\n\x11GetDepositRequest\x12\x14\n\x02id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x02id"=\n\x12GetDepositResponse\x12\'\n\x07\x64\x65posit\x18\x01 \x01(\x0b\x32\r.vega.DepositR\x07\x64\x65posit"\xd0\x01\n\x13ListDepositsRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12>\n\ndate_range\x18\x03 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x01R\tdateRange\x88\x01\x01\x42\r\n\x0b_paginationB\r\n\x0b_date_range"W\n\x14ListDepositsResponse\x12?\n\x08\x64\x65posits\x18\x01 \x01(\x0b\x32#.datanode.api.v2.DepositsConnectionR\x08\x64\x65posits"H\n\x0b\x44\x65positEdge\x12!\n\x04node\x18\x01 \x01(\x0b\x32\r.vega.DepositR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x80\x01\n\x12\x44\x65positsConnection\x12\x32\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1c.datanode.api.v2.DepositEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo",\n\x14GetWithdrawalRequest\x12\x14\n\x02id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x02id"I\n\x15GetWithdrawalResponse\x12\x30\n\nwithdrawal\x18\x01 \x01(\x0b\x32\x10.vega.WithdrawalR\nwithdrawal"\xd3\x01\n\x16ListWithdrawalsRequest\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x12>\n\ndate_range\x18\x03 \x01(\x0b\x32\x1a.datanode.api.v2.DateRangeH\x01R\tdateRange\x88\x01\x01\x42\r\n\x0b_paginationB\r\n\x0b_date_range"c\n\x17ListWithdrawalsResponse\x12H\n\x0bwithdrawals\x18\x01 \x01(\x0b\x32&.datanode.api.v2.WithdrawalsConnectionR\x0bwithdrawals"N\n\x0eWithdrawalEdge\x12$\n\x04node\x18\x01 \x01(\x0b\x32\x10.vega.WithdrawalR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x86\x01\n\x15WithdrawalsConnection\x12\x35\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.WithdrawalEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"2\n\x0fGetAssetRequest\x12\x1f\n\x08\x61sset_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x07\x61ssetId"5\n\x10GetAssetResponse\x12!\n\x05\x61sset\x18\x01 \x01(\x0b\x32\x0b.vega.AssetR\x05\x61sset"\x91\x01\n\x11ListAssetsRequest\x12\x1e\n\x08\x61sset_id\x18\x01 \x01(\tH\x00R\x07\x61ssetId\x88\x01\x01\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x01R\npagination\x88\x01\x01\x42\x0b\n\t_asset_idB\r\n\x0b_pagination"O\n\x12ListAssetsResponse\x12\x39\n\x06\x61ssets\x18\x01 \x01(\x0b\x32!.datanode.api.v2.AssetsConnectionR\x06\x61ssets"D\n\tAssetEdge\x12\x1f\n\x04node\x18\x01 \x01(\x0b\x32\x0b.vega.AssetR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"|\n\x10\x41ssetsConnection\x12\x30\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1a.datanode.api.v2.AssetEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\xa1\x02\n\x1eListLiquidityProvisionsRequest\x12 \n\tmarket_id\x18\x01 \x01(\tH\x00R\x08marketId\x88\x01\x01\x12\x1e\n\x08party_id\x18\x02 \x01(\tH\x01R\x07partyId\x88\x01\x01\x12!\n\treference\x18\x03 \x01(\tH\x02R\treference\x88\x01\x01\x12\x17\n\x04live\x18\x04 \x01(\x08H\x03R\x04live\x88\x01\x01\x12@\n\npagination\x18\x05 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x04R\npagination\x88\x01\x01\x42\x0c\n\n_market_idB\x0b\n\t_party_idB\x0c\n\n_referenceB\x07\n\x05_liveB\r\n\x0b_pagination"\x84\x01\n\x1fListLiquidityProvisionsResponse\x12\x61\n\x14liquidity_provisions\x18\x01 \x01(\x0b\x32..datanode.api.v2.LiquidityProvisionsConnectionR\x13liquidityProvisions"_\n\x17LiquidityProvisionsEdge\x12,\n\x04node\x18\x01 \x01(\x0b\x32\x18.vega.LiquidityProvisionR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x97\x01\n\x1dLiquidityProvisionsConnection\x12>\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32(.datanode.api.v2.LiquidityProvisionsEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\x80\x01\n!ObserveLiquidityProvisionsRequest\x12 \n\tmarket_id\x18\x01 \x01(\tH\x00R\x08marketId\x88\x01\x01\x12\x1e\n\x08party_id\x18\x02 \x01(\tH\x01R\x07partyId\x88\x01\x01\x42\x0c\n\n_market_idB\x0b\n\t_party_id"q\n"ObserveLiquidityProvisionsResponse\x12K\n\x14liquidity_provisions\x18\x01 \x03(\x0b\x32\x18.vega.LiquidityProvisionR\x13liquidityProvisions"\x81\x01\n\x18GetGovernanceDataRequest\x12$\n\x0bproposal_id\x18\x01 \x01(\tH\x00R\nproposalId\x88\x01\x01\x12!\n\treference\x18\x02 \x01(\tH\x01R\treference\x88\x01\x01\x42\x0e\n\x0c_proposal_idB\x0c\n\n_reference"E\n\x19GetGovernanceDataResponse\x12(\n\x04\x64\x61ta\x18\x01 \x01(\x0b\x32\x14.vega.GovernanceDataR\x04\x64\x61ta"\xfa\x04\n\x19ListGovernanceDataRequest\x12@\n\x0eproposal_state\x18\x01 \x01(\x0e\x32\x14.vega.Proposal.StateH\x00R\rproposalState\x88\x01\x01\x12Y\n\rproposal_type\x18\x02 \x01(\x0e\x32/.datanode.api.v2.ListGovernanceDataRequest.TypeH\x01R\x0cproposalType\x88\x01\x01\x12/\n\x11proposer_party_id\x18\x03 \x01(\tH\x02R\x0fproposerPartyId\x88\x01\x01\x12\x32\n\x12proposal_reference\x18\x04 \x01(\tH\x03R\x11proposalReference\x88\x01\x01\x12@\n\npagination\x18\x05 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x04R\npagination\x88\x01\x01"\xb7\x01\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x0c\n\x08TYPE_ALL\x10\x01\x12\x13\n\x0fTYPE_NEW_MARKET\x10\x02\x12\x16\n\x12TYPE_UPDATE_MARKET\x10\x03\x12\x1b\n\x17TYPE_NETWORK_PARAMETERS\x10\x04\x12\x12\n\x0eTYPE_NEW_ASSET\x10\x05\x12\x16\n\x12TYPE_NEW_FREE_FORM\x10\x06\x12\x15\n\x11TYPE_UPDATE_ASSET\x10\x07\x42\x11\n\x0f_proposal_stateB\x10\n\x0e_proposal_typeB\x14\n\x12_proposer_party_idB\x15\n\x13_proposal_referenceB\r\n\x0b_pagination"g\n\x1aListGovernanceDataResponse\x12I\n\nconnection\x18\x01 \x01(\x0b\x32).datanode.api.v2.GovernanceDataConnectionR\nconnection"V\n\x12GovernanceDataEdge\x12(\n\x04node\x18\x01 \x01(\x0b\x32\x14.vega.GovernanceDataR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x8d\x01\n\x18GovernanceDataConnection\x12\x39\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32#.datanode.api.v2.GovernanceDataEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"G\n\x18ObserveGovernanceRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x42\x0b\n\t_party_id"E\n\x19ObserveGovernanceResponse\x12(\n\x04\x64\x61ta\x18\x01 \x01(\x0b\x32\x14.vega.GovernanceDataR\x04\x64\x61ta"\xed\x01\n\x16ListDelegationsRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12\x1c\n\x07node_id\x18\x02 \x01(\tH\x01R\x06nodeId\x88\x01\x01\x12\x1e\n\x08\x65poch_id\x18\x03 \x01(\tH\x02R\x07\x65pochId\x88\x01\x01\x12@\n\npagination\x18\x04 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x03R\npagination\x88\x01\x01\x42\x0b\n\t_party_idB\n\n\x08_node_idB\x0b\n\t_epoch_idB\r\n\x0b_pagination"c\n\x17ListDelegationsResponse\x12H\n\x0b\x64\x65legations\x18\x01 \x01(\x0b\x32&.datanode.api.v2.DelegationsConnectionR\x0b\x64\x65legations"N\n\x0e\x44\x65legationEdge\x12$\n\x04node\x18\x01 \x01(\x0b\x32\x10.vega.DelegationR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x86\x01\n\x15\x44\x65legationsConnection\x12\x35\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.DelegationEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"r\n\x19ObserveDelegationsRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tH\x00R\x07partyId\x88\x01\x01\x12\x1c\n\x07node_id\x18\x02 \x01(\tH\x01R\x06nodeId\x88\x01\x01\x42\x0b\n\t_party_idB\n\n\x08_node_id"N\n\x1aObserveDelegationsResponse\x12\x30\n\ndelegation\x18\x01 \x01(\x0b\x32\x10.vega.DelegationR\ndelegation"\x91\x02\n\tNodeBasic\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x17\n\x07pub_key\x18\x02 \x01(\tR\x06pubKey\x12\x1c\n\ntm_pub_key\x18\x03 \x01(\tR\x08tmPubKey\x12)\n\x10\x65thereum_address\x18\x04 \x01(\tR\x0f\x65thereumAddress\x12\x19\n\x08info_url\x18\x05 \x01(\tR\x07infoUrl\x12\x1a\n\x08location\x18\x06 \x01(\tR\x08location\x12(\n\x06status\x18\r \x01(\x0e\x32\x10.vega.NodeStatusR\x06status\x12\x12\n\x04name\x18\x11 \x01(\tR\x04name\x12\x1d\n\navatar_url\x18\x12 \x01(\tR\tavatarUrl"\x17\n\x15GetNetworkDataRequest"E\n\x16GetNetworkDataResponse\x12+\n\tnode_data\x18\x01 \x01(\x0b\x32\x0e.vega.NodeDataR\x08nodeData"&\n\x0eGetNodeRequest\x12\x14\n\x02id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x02id"1\n\x0fGetNodeResponse\x12\x1e\n\x04node\x18\x01 \x01(\x0b\x32\n.vega.NodeR\x04node"\x93\x01\n\x10ListNodesRequest\x12 \n\tepoch_seq\x18\x01 \x01(\x04H\x00R\x08\x65pochSeq\x88\x01\x01\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x01R\npagination\x88\x01\x01\x42\x0c\n\n_epoch_seqB\r\n\x0b_pagination"K\n\x11ListNodesResponse\x12\x36\n\x05nodes\x18\x01 \x01(\x0b\x32 .datanode.api.v2.NodesConnectionR\x05nodes"B\n\x08NodeEdge\x12\x1e\n\x04node\x18\x01 \x01(\x0b\x32\n.vega.NodeR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"z\n\x0fNodesConnection\x12/\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x19.datanode.api.v2.NodeEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\x82\x01\n\x19ListNodeSignaturesRequest\x12\x14\n\x02id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x02id\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"g\n\x1aListNodeSignaturesResponse\x12I\n\nsignatures\x18\x01 \x01(\x0b\x32).datanode.api.v2.NodeSignaturesConnectionR\nsignatures"`\n\x11NodeSignatureEdge\x12\x33\n\x04node\x18\x01 \x01(\x0b\x32\x1f.vega.commands.v1.NodeSignatureR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x8c\x01\n\x18NodeSignaturesConnection\x12\x38\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32".datanode.api.v2.NodeSignatureEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"R\n\x0fGetEpochRequest\x12\x13\n\x02id\x18\x01 \x01(\x04H\x00R\x02id\x88\x01\x01\x12\x19\n\x05\x62lock\x18\x02 \x01(\x04H\x01R\x05\x62lock\x88\x01\x01\x42\x05\n\x03_idB\x08\n\x06_block"5\n\x10GetEpochResponse\x12!\n\x05\x65poch\x18\x01 \x01(\x0b\x32\x0b.vega.EpochR\x05\x65poch"m\n\x12\x45stimateFeeRequest\x12!\n\tmarket_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x08marketId\x12\x1a\n\x05price\x18\x02 \x01(\tB\x04\xe2\x41\x01\x02R\x05price\x12\x18\n\x04size\x18\x03 \x01(\x04\x42\x04\xe2\x41\x01\x02R\x04size"2\n\x13\x45stimateFeeResponse\x12\x1b\n\x03\x66\x65\x65\x18\x02 \x01(\x0b\x32\t.vega.FeeR\x03\x66\x65\x65"\xe7\x01\n\x15\x45stimateMarginRequest\x12!\n\tmarket_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x08marketId\x12\x1f\n\x08party_id\x18\x02 \x01(\tB\x04\xe2\x41\x01\x02R\x07partyId\x12$\n\x04side\x18\x03 \x01(\x0e\x32\n.vega.SideB\x04\xe2\x41\x01\x02R\x04side\x12*\n\x04type\x18\x04 \x01(\x0e\x32\x10.vega.Order.TypeB\x04\xe2\x41\x01\x02R\x04type\x12\x18\n\x04size\x18\x05 \x01(\x04\x42\x04\xe2\x41\x01\x02R\x04size\x12\x1a\n\x05price\x18\x06 \x01(\tB\x04\xe2\x41\x01\x02R\x05price:\x02\x18\x01"U\n\x16\x45stimateMarginResponse\x12\x37\n\rmargin_levels\x18\x02 \x01(\x0b\x32\x12.vega.MarginLevelsR\x0cmarginLevels:\x02\x18\x01"o\n\x1cListNetworkParametersRequest\x12@\n\npagination\x18\x01 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"{\n\x1dListNetworkParametersResponse\x12Z\n\x12network_parameters\x18\x01 \x01(\x0b\x32+.datanode.api.v2.NetworkParameterConnectionR\x11networkParameters"4\n\x1aGetNetworkParameterRequest\x12\x16\n\x03key\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x03key"b\n\x1bGetNetworkParameterResponse\x12\x43\n\x11network_parameter\x18\x01 \x01(\x0b\x32\x16.vega.NetworkParameterR\x10networkParameter"Z\n\x14NetworkParameterEdge\x12*\n\x04node\x18\x01 \x01(\x0b\x32\x16.vega.NetworkParameterR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x91\x01\n\x1aNetworkParameterConnection\x12;\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32%.datanode.api.v2.NetworkParameterEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"Z\n\nCheckpoint\x12\x12\n\x04hash\x18\x01 \x01(\tR\x04hash\x12\x1d\n\nblock_hash\x18\x02 \x01(\tR\tblockHash\x12\x19\n\x08\x61t_block\x18\x03 \x01(\x04R\x07\x61tBlock"i\n\x16ListCheckpointsRequest\x12@\n\npagination\x18\x01 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"c\n\x17ListCheckpointsResponse\x12H\n\x0b\x63heckpoints\x18\x01 \x01(\x0b\x32&.datanode.api.v2.CheckpointsConnectionR\x0b\x63heckpoints"Y\n\x0e\x43heckpointEdge\x12/\n\x04node\x18\x01 \x01(\x0b\x32\x1b.datanode.api.v2.CheckpointR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x86\x01\n\x15\x43heckpointsConnection\x12\x35\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.CheckpointEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\x83\x01\n\x0fGetStakeRequest\x12\x1f\n\x08party_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x07partyId\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"\x94\x01\n\x10GetStakeResponse\x12\x36\n\x17\x63urrent_stake_available\x18\x01 \x01(\tR\x15\x63urrentStakeAvailable\x12H\n\x0estake_linkings\x18\x02 \x01(\x0b\x32!.datanode.api.v2.StakesConnectionR\rstakeLinkings"\\\n\x10StakeLinkingEdge\x12\x30\n\x04node\x18\x01 \x01(\x0b\x32\x1c.vega.events.v1.StakeLinkingR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x83\x01\n\x10StakesConnection\x12\x37\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32!.datanode.api.v2.StakeLinkingEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo":\n\x15GetRiskFactorsRequest\x12!\n\tmarket_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x08marketId"K\n\x16GetRiskFactorsResponse\x12\x31\n\x0brisk_factor\x18\x01 \x01(\x0b\x32\x10.vega.RiskFactorR\nriskFactor"\xa1\x01\n\x16ObserveEventBusRequest\x12\x30\n\x04type\x18\x01 \x03(\x0e\x32\x1c.vega.events.v1.BusEventTypeR\x04type\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x03 \x01(\tR\x07partyId\x12\x1d\n\nbatch_size\x18\x04 \x01(\x03R\tbatchSize"K\n\x17ObserveEventBusResponse\x12\x30\n\x06\x65vents\x18\x01 \x03(\x0b\x32\x18.vega.events.v1.BusEventR\x06\x65vents"\x1f\n\x1dObserveLedgerMovementsRequest"_\n\x1eObserveLedgerMovementsResponse\x12=\n\x0fledger_movement\x18\x01 \x01(\x0b\x32\x14.vega.LedgerMovementR\x0eledgerMovement"\x94\x01\n\x17ListKeyRotationsRequest\x12\x1c\n\x07node_id\x18\x01 \x01(\tH\x00R\x06nodeId\x88\x01\x01\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x01R\npagination\x88\x01\x01\x42\n\n\x08_node_idB\r\n\x0b_pagination"`\n\x18ListKeyRotationsResponse\x12\x44\n\trotations\x18\x01 \x01(\x0b\x32&.datanode.api.v2.KeyRotationConnectionR\trotations"Z\n\x0fKeyRotationEdge\x12/\n\x04node\x18\x01 \x01(\x0b\x32\x1b.vega.events.v1.KeyRotationR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x87\x01\n\x15KeyRotationConnection\x12\x36\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32 .datanode.api.v2.KeyRotationEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"\x9c\x01\n\x1fListEthereumKeyRotationsRequest\x12\x1c\n\x07node_id\x18\x01 \x01(\tH\x00R\x06nodeId\x88\x01\x01\x12@\n\npagination\x18\x02 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x01R\npagination\x88\x01\x01\x42\n\n\x08_node_idB\r\n\x0b_pagination"x\n ListEthereumKeyRotationsResponse\x12T\n\rkey_rotations\x18\x01 \x01(\x0b\x32/.datanode.api.v2.EthereumKeyRotationsConnectionR\x0ckeyRotations"\x98\x01\n\x1e\x45thereumKeyRotationsConnection\x12>\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32(.datanode.api.v2.EthereumKeyRotationEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"j\n\x17\x45thereumKeyRotationEdge\x12\x37\n\x04node\x18\x01 \x01(\x0b\x32#.vega.events.v1.EthereumKeyRotationR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x14\n\x12GetVegaTimeRequest"3\n\x13GetVegaTimeResponse\x12\x1c\n\ttimestamp\x18\x01 \x01(\x03R\ttimestamp"\x89\x01\n\tDateRange\x12,\n\x0fstart_timestamp\x18\x01 \x01(\x03H\x00R\x0estartTimestamp\x88\x01\x01\x12(\n\rend_timestamp\x18\x02 \x01(\x03H\x01R\x0c\x65ndTimestamp\x88\x01\x01\x42\x12\n\x10_start_timestampB\x10\n\x0e_end_timestamp"!\n\x1fGetProtocolUpgradeStatusRequest"8\n GetProtocolUpgradeStatusResponse\x12\x14\n\x05ready\x18\x01 \x01(\x08R\x05ready"\x83\x02\n#ListProtocolUpgradeProposalsRequest\x12J\n\x06status\x18\x01 \x01(\x0e\x32-.vega.events.v1.ProtocolUpgradeProposalStatusH\x00R\x06status\x88\x01\x01\x12$\n\x0b\x61pproved_by\x18\x02 \x01(\tH\x01R\napprovedBy\x88\x01\x01\x12@\n\npagination\x18\x03 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x02R\npagination\x88\x01\x01\x42\t\n\x07_statusB\x0e\n\x0c_approved_byB\r\n\x0b_pagination"\x98\x01\n$ListProtocolUpgradeProposalsResponse\x12p\n\x1aprotocol_upgrade_proposals\x18\x01 \x01(\x0b\x32\x32.datanode.api.v2.ProtocolUpgradeProposalConnectionR\x18protocolUpgradeProposals"\x9f\x01\n!ProtocolUpgradeProposalConnection\x12\x42\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32,.datanode.api.v2.ProtocolUpgradeProposalEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"o\n\x1bProtocolUpgradeProposalEdge\x12\x38\n\x04node\x18\x01 \x01(\x0b\x32$.vega.events.v1.ProtocolUpgradeEventR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"k\n\x18ListCoreSnapshotsRequest\x12@\n\npagination\x18\x01 \x01(\x0b\x32\x1b.datanode.api.v2.PaginationH\x00R\npagination\x88\x01\x01\x42\r\n\x0b_pagination"k\n\x19ListCoreSnapshotsResponse\x12N\n\x0e\x63ore_snapshots\x18\x01 \x01(\x0b\x32\'.datanode.api.v2.CoreSnapshotConnectionR\rcoreSnapshots"\x89\x01\n\x16\x43oreSnapshotConnection\x12\x37\n\x05\x65\x64ges\x18\x01 \x03(\x0b\x32!.datanode.api.v2.CoreSnapshotEdgeR\x05\x65\x64ges\x12\x36\n\tpage_info\x18\x02 \x01(\x0b\x32\x19.datanode.api.v2.PageInfoR\x08pageInfo"`\n\x10\x43oreSnapshotEdge\x12\x34\n\x04node\x18\x01 \x01(\x0b\x32 .vega.events.v1.CoreSnapshotDataR\x04node\x12\x16\n\x06\x63ursor\x18\x02 \x01(\tR\x06\x63ursor"\x81\x02\n\x0eHistorySegment\x12\x1f\n\x0b\x66rom_height\x18\x01 \x01(\x03R\nfromHeight\x12\x1b\n\tto_height\x18\x02 \x01(\x03R\x08toHeight\x12,\n\x12history_segment_id\x18\x03 \x01(\tR\x10historySegmentId\x12=\n\x1bprevious_history_segment_id\x18\x04 \x01(\tR\x18previousHistorySegmentId\x12)\n\x10\x64\x61tabase_version\x18\x05 \x01(\x03R\x0f\x64\x61tabaseVersion\x12\x19\n\x08\x63hain_id\x18\x06 \x01(\tR\x07\x63hainId"+\n)GetMostRecentNetworkHistorySegmentRequest"\x8d\x01\n*GetMostRecentNetworkHistorySegmentResponse\x12\x39\n\x07segment\x18\x01 \x01(\x0b\x32\x1f.datanode.api.v2.HistorySegmentR\x07segment\x12$\n\x0eswarm_key_seed\x18\x02 \x01(\tR\x0cswarmKeySeed"&\n$ListAllNetworkHistorySegmentsRequest"d\n%ListAllNetworkHistorySegmentsResponse\x12;\n\x08segments\x18\x01 \x03(\x0b\x32\x1f.datanode.api.v2.HistorySegmentR\x08segments"-\n+GetActiveNetworkHistoryPeerAddressesRequest"Q\n,GetActiveNetworkHistoryPeerAddressesResponse\x12!\n\x0cip_addresses\x18\x01 \x03(\tR\x0bipAddresses" \n\x1eGetNetworkHistoryStatusRequest"\xb0\x01\n\x1fGetNetworkHistoryStatusResponse\x12!\n\x0cipfs_address\x18\x01 \x01(\tR\x0bipfsAddress\x12\x1b\n\tswarm_key\x18\x02 \x01(\tR\x08swarmKey\x12$\n\x0eswarm_key_seed\x18\x03 \x01(\tR\x0cswarmKeySeed\x12\'\n\x0f\x63onnected_peers\x18\x05 \x03(\tR\x0e\x63onnectedPeers"(\n&GetNetworkHistoryBootstrapPeersRequest"R\n\'GetNetworkHistoryBootstrapPeersResponse\x12\'\n\x0f\x62ootstrap_peers\x18\x01 \x03(\tR\x0e\x62ootstrapPeers"\x85\x01\n\x1b\x45xportNetworkHistoryRequest\x12\x1d\n\nfrom_block\x18\x01 \x01(\x03R\tfromBlock\x12\x19\n\x08to_block\x18\x02 \x01(\x03R\x07toBlock\x12,\n\x05table\x18\x03 \x01(\x0e\x32\x16.datanode.api.v2.TableR\x05table"F\n\x13ListEntitiesRequest\x12/\n\x10transaction_hash\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x0ftransactionHash"\xad\r\n\x14ListEntitiesResponse\x12)\n\x08\x61\x63\x63ounts\x18\x01 \x03(\x0b\x32\r.vega.AccountR\x08\x61\x63\x63ounts\x12#\n\x06orders\x18\x02 \x03(\x0b\x32\x0b.vega.OrderR\x06orders\x12,\n\tpositions\x18\x03 \x03(\x0b\x32\x0e.vega.PositionR\tpositions\x12\x38\n\x0eledger_entries\x18\x04 \x03(\x0b\x32\x11.vega.LedgerEntryR\rledgerEntries\x12H\n\x0f\x62\x61lance_changes\x18\x05 \x03(\x0b\x32\x1f.datanode.api.v2.AccountBalanceR\x0e\x62\x61lanceChanges\x12\x36\n\ttransfers\x18\x06 \x03(\x0b\x32\x18.vega.events.v1.TransferR\ttransfers\x12 \n\x05votes\x18\x07 \x03(\x0b\x32\n.vega.VoteR\x05votes\x12~\n$erc20_multi_sig_signer_added_bundles\x18\x08 \x03(\x0b\x32/.datanode.api.v2.ERC20MultiSigSignerAddedBundleR\x1f\x65rc20MultiSigSignerAddedBundles\x12\x84\x01\n&erc20_multi_sig_signer_removed_bundles\x18\t \x03(\x0b\x32\x31.datanode.api.v2.ERC20MultiSigSignerRemovedBundleR!erc20MultiSigSignerRemovedBundles\x12#\n\x06trades\x18\n \x03(\x0b\x32\x0b.vega.TradeR\x06trades\x12\x33\n\x0coracle_specs\x18\x0b \x03(\x0b\x32\x10.vega.OracleSpecR\x0boracleSpecs\x12\x31\n\x0boracle_data\x18\x0c \x03(\x0b\x32\x10.vega.OracleDataR\noracleData\x12&\n\x07markets\x18\r \x03(\x0b\x32\x0c.vega.MarketR\x07markets\x12%\n\x07parties\x18\x0e \x03(\x0b\x32\x0b.vega.PartyR\x07parties\x12\x37\n\rmargin_levels\x18\x0f \x03(\x0b\x32\x12.vega.MarginLevelsR\x0cmarginLevels\x12&\n\x07rewards\x18\x10 \x03(\x0b\x32\x0c.vega.RewardR\x07rewards\x12)\n\x08\x64\x65posits\x18\x11 \x03(\x0b\x32\r.vega.DepositR\x08\x64\x65posits\x12\x32\n\x0bwithdrawals\x18\x12 \x03(\x0b\x32\x10.vega.WithdrawalR\x0bwithdrawals\x12#\n\x06\x61ssets\x18\x13 \x03(\x0b\x32\x0b.vega.AssetR\x06\x61ssets\x12K\n\x14liquidity_provisions\x18\x14 \x03(\x0b\x32\x18.vega.LiquidityProvisionR\x13liquidityProvisions\x12,\n\tproposals\x18\x15 \x03(\x0b\x32\x0e.vega.ProposalR\tproposals\x12\x32\n\x0b\x64\x65legations\x18\x16 \x03(\x0b\x32\x10.vega.DelegationR\x0b\x64\x65legations\x12\x30\n\x05nodes\x18\x17 \x03(\x0b\x32\x1a.datanode.api.v2.NodeBasicR\x05nodes\x12H\n\x0fnode_signatures\x18\x18 \x03(\x0b\x32\x1f.vega.commands.v1.NodeSignatureR\x0enodeSignatures\x12\x45\n\x12network_parameters\x18\x19 \x03(\x0b\x32\x16.vega.NetworkParameterR\x11networkParameters\x12@\n\rkey_rotations\x18\x1a \x03(\x0b\x32\x1b.vega.events.v1.KeyRotationR\x0ckeyRotations\x12Y\n\x16\x65thereum_key_rotations\x18\x1b \x03(\x0b\x32#.vega.events.v1.EthereumKeyRotationR\x14\x65thereumKeyRotations\x12\x62\n\x1aprotocol_upgrade_proposals\x18\x1c \x03(\x0b\x32$.vega.events.v1.ProtocolUpgradeEventR\x18protocolUpgradeProposals"\r\n\x0bPingRequest"\x0e\n\x0cPingResponse"\x87\x01\n\tOrderInfo\x12\x1e\n\x04side\x18\x01 \x01(\x0e\x32\n.vega.SideR\x04side\x12\x14\n\x05price\x18\x02 \x01(\tR\x05price\x12\x1c\n\tremaining\x18\x03 \x01(\x04R\tremaining\x12&\n\x0fis_market_order\x18\x04 \x01(\x08R\risMarketOrder"\xe8\x01\n\x17\x45stimatePositionRequest\x12!\n\tmarket_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x08marketId\x12%\n\x0bopen_volume\x18\x02 \x01(\x03\x42\x04\xe2\x41\x01\x02R\nopenVolume\x12\x32\n\x06orders\x18\x03 \x03(\x0b\x32\x1a.datanode.api.v2.OrderInfoR\x06orders\x12\x36\n\x14\x63ollateral_available\x18\x04 \x01(\tH\x00R\x13\x63ollateralAvailable\x88\x01\x01\x42\x17\n\x15_collateral_available"\x9b\x01\n\x18\x45stimatePositionResponse\x12\x37\n\x06margin\x18\x01 \x01(\x0b\x32\x1f.datanode.api.v2.MarginEstimateR\x06margin\x12\x46\n\x0bliquidation\x18\x02 \x01(\x0b\x32$.datanode.api.v2.LiquidationEstimateR\x0bliquidation"t\n\x0eMarginEstimate\x12\x31\n\nworst_case\x18\x01 \x01(\x0b\x32\x12.vega.MarginLevelsR\tworstCase\x12/\n\tbest_case\x18\x02 \x01(\x0b\x32\x12.vega.MarginLevelsR\x08\x62\x65stCase"\x97\x01\n\x13LiquidationEstimate\x12@\n\nworst_case\x18\x01 \x01(\x0b\x32!.datanode.api.v2.LiquidationPriceR\tworstCase\x12>\n\tbest_case\x18\x02 \x01(\x0b\x32!.datanode.api.v2.LiquidationPriceR\x08\x62\x65stCase"\xa2\x01\n\x10LiquidationPrice\x12(\n\x10open_volume_only\x18\x01 \x01(\tR\x0eopenVolumeOnly\x12\x30\n\x14including_buy_orders\x18\x02 \x01(\tR\x12includingBuyOrders\x12\x32\n\x15including_sell_orders\x18\x03 \x01(\tR\x13includingSellOrders*\xaa\x01\n\x10LedgerEntryField\x12"\n\x1eLEDGER_ENTRY_FIELD_UNSPECIFIED\x10\x00\x12&\n"LEDGER_ENTRY_FIELD_ACCOUNT_FROM_ID\x10\x01\x12$\n LEDGER_ENTRY_FIELD_ACCOUNT_TO_ID\x10\x02\x12$\n LEDGER_ENTRY_FIELD_TRANSFER_TYPE\x10\x03*\xb0\x01\n\x0c\x41\x63\x63ountField\x12\x1d\n\x19\x41\x43\x43OUNT_FIELD_UNSPECIFIED\x10\x00\x12\x14\n\x10\x41\x43\x43OUNT_FIELD_ID\x10\x01\x12\x1a\n\x16\x41\x43\x43OUNT_FIELD_PARTY_ID\x10\x02\x12\x1a\n\x16\x41\x43\x43OUNT_FIELD_ASSET_ID\x10\x03\x12\x1b\n\x17\x41\x43\x43OUNT_FIELD_MARKET_ID\x10\x04\x12\x16\n\x12\x41\x43\x43OUNT_FIELD_TYPE\x10\x05*\xad\x01\n\x11TransferDirection\x12"\n\x1eTRANSFER_DIRECTION_UNSPECIFIED\x10\x00\x12$\n TRANSFER_DIRECTION_TRANSFER_FROM\x10\x01\x12"\n\x1eTRANSFER_DIRECTION_TRANSFER_TO\x10\x02\x12*\n&TRANSFER_DIRECTION_TRANSFER_TO_OR_FROM\x10\x03*\xde\x02\n\x05Table\x12\x15\n\x11TABLE_UNSPECIFIED\x10\x00\x12\x12\n\x0eTABLE_BALANCES\x10\x01\x12\x15\n\x11TABLE_CHECKPOINTS\x10\x02\x12\x15\n\x11TABLE_DELEGATIONS\x10\x03\x12\x10\n\x0cTABLE_LEDGER\x10\x04\x12\x10\n\x0cTABLE_ORDERS\x10\x05\x12\x10\n\x0cTABLE_TRADES\x10\x06\x12\x15\n\x11TABLE_MARKET_DATA\x10\x07\x12\x17\n\x13TABLE_MARGIN_LEVELS\x10\x08\x12\x13\n\x0fTABLE_POSITIONS\x10\t\x12\x1e\n\x1aTABLE_LIQUIDITY_PROVISIONS\x10\n\x12\x11\n\rTABLE_MARKETS\x10\x0b\x12\x12\n\x0eTABLE_DEPOSITS\x10\x0c\x12\x15\n\x11TABLE_WITHDRAWALS\x10\r\x12\x10\n\x0cTABLE_BLOCKS\x10\x0e\x12\x11\n\rTABLE_REWARDS\x10\x0f\x32\x98V\n\x12TradingDataService\x12j\n\x0cListAccounts\x12$.datanode.api.v2.ListAccountsRequest\x1a%.datanode.api.v2.ListAccountsResponse"\r\x92\x41\n\n\x08\x41\x63\x63ounts\x12u\n\x0fObserveAccounts\x12\'.datanode.api.v2.ObserveAccountsRequest\x1a(.datanode.api.v2.ObserveAccountsResponse"\r\x92\x41\n\n\x08\x41\x63\x63ounts0\x01\x12Z\n\x04Info\x12\x1c.datanode.api.v2.InfoRequest\x1a\x1d.datanode.api.v2.InfoResponse"\x15\x92\x41\x12\n\x10Node information\x12\\\n\x08GetOrder\x12 .datanode.api.v2.GetOrderRequest\x1a!.datanode.api.v2.GetOrderResponse"\x0b\x92\x41\x08\n\x06Orders\x12\x62\n\nListOrders\x12".datanode.api.v2.ListOrdersRequest\x1a#.datanode.api.v2.ListOrdersResponse"\x0b\x92\x41\x08\n\x06Orders\x12w\n\x11ListOrderVersions\x12).datanode.api.v2.ListOrderVersionsRequest\x1a*.datanode.api.v2.ListOrderVersionsResponse"\x0b\x92\x41\x08\n\x06Orders\x12m\n\rObserveOrders\x12%.datanode.api.v2.ObserveOrdersRequest\x1a&.datanode.api.v2.ObserveOrdersResponse"\x0b\x92\x41\x08\n\x06Orders0\x01\x12q\n\rListPositions\x12%.datanode.api.v2.ListPositionsRequest\x1a&.datanode.api.v2.ListPositionsResponse"\x11\x88\x02\x01\x92\x41\x0b\n\tPositions\x12w\n\x10ListAllPositions\x12(.datanode.api.v2.ListAllPositionsRequest\x1a).datanode.api.v2.ListAllPositionsResponse"\x0e\x92\x41\x0b\n\tPositions\x12y\n\x10ObservePositions\x12(.datanode.api.v2.ObservePositionsRequest\x1a).datanode.api.v2.ObservePositionsResponse"\x0e\x92\x41\x0b\n\tPositions0\x01\x12\x7f\n\x11ListLedgerEntries\x12).datanode.api.v2.ListLedgerEntriesRequest\x1a*.datanode.api.v2.ListLedgerEntriesResponse"\x13\x92\x41\x10\n\x0eLedger entries\x12o\n\x13\x45xportLedgerEntries\x12+.datanode.api.v2.ExportLedgerEntriesRequest\x1a\x14.google.api.HttpBody"\x13\x92\x41\x10\n\x0eLedger entries0\x01\x12|\n\x12ListBalanceChanges\x12*.datanode.api.v2.ListBalanceChangesRequest\x1a+.datanode.api.v2.ListBalanceChangesResponse"\r\x92\x41\n\n\x08\x41\x63\x63ounts\x12~\n\x13GetLatestMarketData\x12+.datanode.api.v2.GetLatestMarketDataRequest\x1a,.datanode.api.v2.GetLatestMarketDataResponse"\x0c\x92\x41\t\n\x07Markets\x12\x81\x01\n\x14ListLatestMarketData\x12,.datanode.api.v2.ListLatestMarketDataRequest\x1a-.datanode.api.v2.ListLatestMarketDataResponse"\x0c\x92\x41\t\n\x07Markets\x12\x81\x01\n\x14GetLatestMarketDepth\x12,.datanode.api.v2.GetLatestMarketDepthRequest\x1a-.datanode.api.v2.GetLatestMarketDepthResponse"\x0c\x92\x41\t\n\x07Markets\x12\x80\x01\n\x13ObserveMarketsDepth\x12+.datanode.api.v2.ObserveMarketsDepthRequest\x1a,.datanode.api.v2.ObserveMarketsDepthResponse"\x0c\x92\x41\t\n\x07Markets0\x01\x12\x95\x01\n\x1aObserveMarketsDepthUpdates\x12\x32.datanode.api.v2.ObserveMarketsDepthUpdatesRequest\x1a\x33.datanode.api.v2.ObserveMarketsDepthUpdatesResponse"\x0c\x92\x41\t\n\x07Markets0\x01\x12}\n\x12ObserveMarketsData\x12*.datanode.api.v2.ObserveMarketsDataRequest\x1a+.datanode.api.v2.ObserveMarketsDataResponse"\x0c\x92\x41\t\n\x07Markets0\x01\x12\x8d\x01\n\x18GetMarketDataHistoryByID\x12\x30.datanode.api.v2.GetMarketDataHistoryByIDRequest\x1a\x31.datanode.api.v2.GetMarketDataHistoryByIDResponse"\x0c\x92\x41\t\n\x07Markets\x12n\n\rListTransfers\x12%.datanode.api.v2.ListTransfersRequest\x1a&.datanode.api.v2.ListTransfersResponse"\x0e\x92\x41\x0b\n\tTransfers\x12u\n\x10GetNetworkLimits\x12(.datanode.api.v2.GetNetworkLimitsRequest\x1a).datanode.api.v2.GetNetworkLimitsResponse"\x0c\x92\x41\t\n\x07Network\x12o\n\x0eListCandleData\x12&.datanode.api.v2.ListCandleDataRequest\x1a\'.datanode.api.v2.ListCandleDataResponse"\x0c\x92\x41\t\n\x07\x43\x61ndles\x12z\n\x11ObserveCandleData\x12).datanode.api.v2.ObserveCandleDataRequest\x1a*.datanode.api.v2.ObserveCandleDataResponse"\x0c\x92\x41\t\n\x07\x43\x61ndles0\x01\x12~\n\x13ListCandleIntervals\x12+.datanode.api.v2.ListCandleIntervalsRequest\x1a,.datanode.api.v2.ListCandleIntervalsResponse"\x0c\x92\x41\t\n\x07\x43\x61ndles\x12\x63\n\tListVotes\x12!.datanode.api.v2.ListVotesRequest\x1a".datanode.api.v2.ListVotesResponse"\x0f\x92\x41\x0c\n\nGovernance\x12n\n\x0cObserveVotes\x12$.datanode.api.v2.ObserveVotesRequest\x1a%.datanode.api.v2.ObserveVotesResponse"\x0f\x92\x41\x0c\n\nGovernance0\x01\x12\xb3\x01\n#ListERC20MultiSigSignerAddedBundles\x12;.datanode.api.v2.ListERC20MultiSigSignerAddedBundlesRequest\x1a<.datanode.api.v2.ListERC20MultiSigSignerAddedBundlesResponse"\x11\x92\x41\x0e\n\x0c\x45RC20 bridge\x12\xb9\x01\n%ListERC20MultiSigSignerRemovedBundles\x12=.datanode.api.v2.ListERC20MultiSigSignerRemovedBundlesRequest\x1a>.datanode.api.v2.ListERC20MultiSigSignerRemovedBundlesResponse"\x11\x92\x41\x0e\n\x0c\x45RC20 bridge\x12\x8f\x01\n\x17GetERC20ListAssetBundle\x12/.datanode.api.v2.GetERC20ListAssetBundleRequest\x1a\x30.datanode.api.v2.GetERC20ListAssetBundleResponse"\x11\x92\x41\x0e\n\x0c\x45RC20 bridge\x12\x9e\x01\n\x1cGetERC20SetAssetLimitsBundle\x12\x34.datanode.api.v2.GetERC20SetAssetLimitsBundleRequest\x1a\x35.datanode.api.v2.GetERC20SetAssetLimitsBundleResponse"\x11\x92\x41\x0e\n\x0c\x45RC20 bridge\x12\x98\x01\n\x1aGetERC20WithdrawalApproval\x12\x32.datanode.api.v2.GetERC20WithdrawalApprovalRequest\x1a\x33.datanode.api.v2.GetERC20WithdrawalApprovalResponse"\x11\x92\x41\x0e\n\x0c\x45RC20 bridge\x12h\n\x0cGetLastTrade\x12$.datanode.api.v2.GetLastTradeRequest\x1a%.datanode.api.v2.GetLastTradeResponse"\x0b\x92\x41\x08\n\x06Trades\x12\x62\n\nListTrades\x12".datanode.api.v2.ListTradesRequest\x1a#.datanode.api.v2.ListTradesResponse"\x0b\x92\x41\x08\n\x06Trades\x12m\n\rObserveTrades\x12%.datanode.api.v2.ObserveTradesRequest\x1a&.datanode.api.v2.ObserveTradesResponse"\x0b\x92\x41\x08\n\x06Trades0\x01\x12q\n\rGetOracleSpec\x12%.datanode.api.v2.GetOracleSpecRequest\x1a&.datanode.api.v2.GetOracleSpecResponse"\x11\x92\x41\x0e\n\x0c\x44\x61ta sources\x12w\n\x0fListOracleSpecs\x12\'.datanode.api.v2.ListOracleSpecsRequest\x1a(.datanode.api.v2.ListOracleSpecsResponse"\x11\x92\x41\x0e\n\x0c\x44\x61ta sources\x12t\n\x0eListOracleData\x12&.datanode.api.v2.ListOracleDataRequest\x1a\'.datanode.api.v2.ListOracleDataResponse"\x11\x92\x41\x0e\n\x0c\x44\x61ta sources\x12`\n\tGetMarket\x12!.datanode.api.v2.GetMarketRequest\x1a".datanode.api.v2.GetMarketResponse"\x0c\x92\x41\t\n\x07Markets\x12\x66\n\x0bListMarkets\x12#.datanode.api.v2.ListMarketsRequest\x1a$.datanode.api.v2.ListMarketsResponse"\x0c\x92\x41\t\n\x07Markets\x12\x81\x01\n\x14ListSuccessorMarkets\x12,.datanode.api.v2.ListSuccessorMarketsRequest\x1a-.datanode.api.v2.ListSuccessorMarketsResponse"\x0c\x92\x41\t\n\x07Markets\x12]\n\x08GetParty\x12 .datanode.api.v2.GetPartyRequest\x1a!.datanode.api.v2.GetPartyResponse"\x0c\x92\x41\t\n\x07Parties\x12\x66\n\x0bListParties\x12#.datanode.api.v2.ListPartiesRequest\x1a$.datanode.api.v2.ListPartiesResponse"\x0c\x92\x41\t\n\x07Parties\x12{\n\x10ListMarginLevels\x12(.datanode.api.v2.ListMarginLevelsRequest\x1a).datanode.api.v2.ListMarginLevelsResponse"\x12\x92\x41\x0f\n\rMargin levels\x12\x86\x01\n\x13ObserveMarginLevels\x12+.datanode.api.v2.ObserveMarginLevelsRequest\x1a,.datanode.api.v2.ObserveMarginLevelsResponse"\x12\x92\x41\x0f\n\rMargin levels0\x01\x12\x66\n\x0bListRewards\x12#.datanode.api.v2.ListRewardsRequest\x1a$.datanode.api.v2.ListRewardsResponse"\x0c\x92\x41\t\n\x07Rewards\x12~\n\x13ListRewardSummaries\x12+.datanode.api.v2.ListRewardSummariesRequest\x1a,.datanode.api.v2.ListRewardSummariesResponse"\x0c\x92\x41\t\n\x07Rewards\x12\x8d\x01\n\x18ListEpochRewardSummaries\x12\x30.datanode.api.v2.ListEpochRewardSummariesRequest\x1a\x31.datanode.api.v2.ListEpochRewardSummariesResponse"\x0c\x92\x41\t\n\x07Rewards\x12\x62\n\nGetDeposit\x12".datanode.api.v2.GetDepositRequest\x1a#.datanode.api.v2.GetDepositResponse"\x0b\x92\x41\x08\n\x06\x41ssets\x12h\n\x0cListDeposits\x12$.datanode.api.v2.ListDepositsRequest\x1a%.datanode.api.v2.ListDepositsResponse"\x0b\x92\x41\x08\n\x06\x41ssets\x12k\n\rGetWithdrawal\x12%.datanode.api.v2.GetWithdrawalRequest\x1a&.datanode.api.v2.GetWithdrawalResponse"\x0b\x92\x41\x08\n\x06\x41ssets\x12q\n\x0fListWithdrawals\x12\'.datanode.api.v2.ListWithdrawalsRequest\x1a(.datanode.api.v2.ListWithdrawalsResponse"\x0b\x92\x41\x08\n\x06\x41ssets\x12\\\n\x08GetAsset\x12 .datanode.api.v2.GetAssetRequest\x1a!.datanode.api.v2.GetAssetResponse"\x0b\x92\x41\x08\n\x06\x41ssets\x12\x62\n\nListAssets\x12".datanode.api.v2.ListAssetsRequest\x1a#.datanode.api.v2.ListAssetsResponse"\x0b\x92\x41\x08\n\x06\x41ssets\x12\x97\x01\n\x17ListLiquidityProvisions\x12/.datanode.api.v2.ListLiquidityProvisionsRequest\x1a\x30.datanode.api.v2.ListLiquidityProvisionsResponse"\x19\x92\x41\x16\n\x14Liquidity provisions\x12\xa2\x01\n\x1aObserveLiquidityProvisions\x12\x32.datanode.api.v2.ObserveLiquidityProvisionsRequest\x1a\x33.datanode.api.v2.ObserveLiquidityProvisionsResponse"\x19\x92\x41\x16\n\x14Liquidity provisions0\x01\x12{\n\x11GetGovernanceData\x12).datanode.api.v2.GetGovernanceDataRequest\x1a*.datanode.api.v2.GetGovernanceDataResponse"\x0f\x92\x41\x0c\n\nGovernance\x12~\n\x12ListGovernanceData\x12*.datanode.api.v2.ListGovernanceDataRequest\x1a+.datanode.api.v2.ListGovernanceDataResponse"\x0f\x92\x41\x0c\n\nGovernance\x12}\n\x11ObserveGovernance\x12).datanode.api.v2.ObserveGovernanceRequest\x1a*.datanode.api.v2.ObserveGovernanceResponse"\x0f\x92\x41\x0c\n\nGovernance0\x01\x12r\n\x0fListDelegations\x12\'.datanode.api.v2.ListDelegationsRequest\x1a(.datanode.api.v2.ListDelegationsResponse"\x0c\x92\x41\t\n\x07Network\x12o\n\x0eGetNetworkData\x12&.datanode.api.v2.GetNetworkDataRequest\x1a\'.datanode.api.v2.GetNetworkDataResponse"\x0c\x92\x41\t\n\x07Network\x12Z\n\x07GetNode\x12\x1f.datanode.api.v2.GetNodeRequest\x1a .datanode.api.v2.GetNodeResponse"\x0c\x92\x41\t\n\x07Network\x12`\n\tListNodes\x12!.datanode.api.v2.ListNodesRequest\x1a".datanode.api.v2.ListNodesResponse"\x0c\x92\x41\t\n\x07Network\x12\x80\x01\n\x12ListNodeSignatures\x12*.datanode.api.v2.ListNodeSignaturesRequest\x1a+.datanode.api.v2.ListNodeSignaturesResponse"\x11\x92\x41\x0e\n\x0c\x45RC20 bridge\x12]\n\x08GetEpoch\x12 .datanode.api.v2.GetEpochRequest\x1a!.datanode.api.v2.GetEpochResponse"\x0c\x92\x41\t\n\x07Network\x12\x65\n\x0b\x45stimateFee\x12#.datanode.api.v2.EstimateFeeRequest\x1a$.datanode.api.v2.EstimateFeeResponse"\x0b\x92\x41\x08\n\x06Orders\x12n\n\x0e\x45stimateMargin\x12&.datanode.api.v2.EstimateMarginRequest\x1a\'.datanode.api.v2.EstimateMarginResponse"\x0b\x92\x41\x08\n\x06Orders\x12w\n\x10\x45stimatePosition\x12(.datanode.api.v2.EstimatePositionRequest\x1a).datanode.api.v2.EstimatePositionResponse"\x0e\x92\x41\x0b\n\tPositions\x12\x84\x01\n\x15ListNetworkParameters\x12-.datanode.api.v2.ListNetworkParametersRequest\x1a..datanode.api.v2.ListNetworkParametersResponse"\x0c\x92\x41\t\n\x07Network\x12~\n\x13GetNetworkParameter\x12+.datanode.api.v2.GetNetworkParameterRequest\x1a,.datanode.api.v2.GetNetworkParameterResponse"\x0c\x92\x41\t\n\x07Network\x12r\n\x0fListCheckpoints\x12\'.datanode.api.v2.ListCheckpointsRequest\x1a(.datanode.api.v2.ListCheckpointsResponse"\x0c\x92\x41\t\n\x07Network\x12]\n\x08GetStake\x12 .datanode.api.v2.GetStakeRequest\x1a!.datanode.api.v2.GetStakeResponse"\x0c\x92\x41\t\n\x07Network\x12o\n\x0eGetRiskFactors\x12&.datanode.api.v2.GetRiskFactorsRequest\x1a\'.datanode.api.v2.GetRiskFactorsResponse"\x0c\x92\x41\t\n\x07Markets\x12u\n\x0fObserveEventBus\x12\'.datanode.api.v2.ObserveEventBusRequest\x1a(.datanode.api.v2.ObserveEventBusResponse"\x0b\x92\x41\x08\n\x06\x45vents(\x01\x30\x01\x12\x92\x01\n\x16ObserveLedgerMovements\x12..datanode.api.v2.ObserveLedgerMovementsRequest\x1a/.datanode.api.v2.ObserveLedgerMovementsResponse"\x15\x92\x41\x12\n\x10Ledger movements0\x01\x12u\n\x10ListKeyRotations\x12(.datanode.api.v2.ListKeyRotationsRequest\x1a).datanode.api.v2.ListKeyRotationsResponse"\x0c\x92\x41\t\n\x07Network\x12\x8d\x01\n\x18ListEthereumKeyRotations\x12\x30.datanode.api.v2.ListEthereumKeyRotationsRequest\x1a\x31.datanode.api.v2.ListEthereumKeyRotationsResponse"\x0c\x92\x41\t\n\x07Network\x12\x66\n\x0bGetVegaTime\x12#.datanode.api.v2.GetVegaTimeRequest\x1a$.datanode.api.v2.GetVegaTimeResponse"\x0c\x92\x41\t\n\x07Network\x12\x8d\x01\n\x18GetProtocolUpgradeStatus\x12\x30.datanode.api.v2.GetProtocolUpgradeStatusRequest\x1a\x31.datanode.api.v2.GetProtocolUpgradeStatusResponse"\x0c\x92\x41\t\n\x07Network\x12\x99\x01\n\x1cListProtocolUpgradeProposals\x12\x34.datanode.api.v2.ListProtocolUpgradeProposalsRequest\x1a\x35.datanode.api.v2.ListProtocolUpgradeProposalsResponse"\x0c\x92\x41\t\n\x07Network\x12x\n\x11ListCoreSnapshots\x12).datanode.api.v2.ListCoreSnapshotsRequest\x1a*.datanode.api.v2.ListCoreSnapshotsResponse"\x0c\x92\x41\t\n\x07Network\x12\xb3\x01\n"GetMostRecentNetworkHistorySegment\x12:.datanode.api.v2.GetMostRecentNetworkHistorySegmentRequest\x1a;.datanode.api.v2.GetMostRecentNetworkHistorySegmentResponse"\x14\x92\x41\x11\n\x0fNetwork history\x12\xa4\x01\n\x1dListAllNetworkHistorySegments\x12\x35.datanode.api.v2.ListAllNetworkHistorySegmentsRequest\x1a\x36.datanode.api.v2.ListAllNetworkHistorySegmentsResponse"\x14\x92\x41\x11\n\x0fNetwork history\x12\xb9\x01\n$GetActiveNetworkHistoryPeerAddresses\x12<.datanode.api.v2.GetActiveNetworkHistoryPeerAddressesRequest\x1a=.datanode.api.v2.GetActiveNetworkHistoryPeerAddressesResponse"\x14\x92\x41\x11\n\x0fNetwork history\x12\x92\x01\n\x17GetNetworkHistoryStatus\x12/.datanode.api.v2.GetNetworkHistoryStatusRequest\x1a\x30.datanode.api.v2.GetNetworkHistoryStatusResponse"\x14\x92\x41\x11\n\x0fNetwork history\x12\xaa\x01\n\x1fGetNetworkHistoryBootstrapPeers\x12\x37.datanode.api.v2.GetNetworkHistoryBootstrapPeersRequest\x1a\x38.datanode.api.v2.GetNetworkHistoryBootstrapPeersResponse"\x14\x92\x41\x11\n\x0fNetwork history\x12j\n\x0cListEntities\x12$.datanode.api.v2.ListEntitiesRequest\x1a%.datanode.api.v2.ListEntitiesResponse"\r\x92\x41\n\n\x08\x45xplorer\x12r\n\x14\x45xportNetworkHistory\x12,.datanode.api.v2.ExportNetworkHistoryRequest\x1a\x14.google.api.HttpBody"\x14\x92\x41\x11\n\x0fNetwork history0\x01\x12N\n\x04Ping\x12\x1c.datanode.api.v2.PingRequest\x1a\x1d.datanode.api.v2.PingResponse"\t\x92\x41\x06\n\x04MiscB\xc6\x01Z1code.vegaprotocol.io/vega/protos/data-node/api/v2\x92\x41\x8f\x01\x12\x1e\n\x13Vega data node APIs2\x07v0.71.0\x1a\x1chttps://api.testnet.vega.xyz*\x02\x01\x02\x32\x10\x61pplication/jsonR9\n\x03\x35\x30\x30\x12\x32\n\x18\x41n internal server error\x12\x16\n\x14\x1a\x12.google.rpc.Statusb\x06proto3'
 )
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(
-    DESCRIPTOR, "data_node.api.v2.trading_data_pb2", globals()
+    DESCRIPTOR, "data_node.api.v2.trading_data_pb2", _globals
 )
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    DESCRIPTOR._serialized_options = b"Z1code.vegaprotocol.io/vega/protos/data-node/api/v2\222A\217\001\022\036\n\023Vega data node APIs2\007v0.71.4\032\034https://api.testnet.vega.xyz*\002\001\0022\020application/jsonR9\n\003500\0222\n\030An internal server error\022\026\n\024\032\022.google.rpc.Status"
+    DESCRIPTOR._serialized_options = b"Z1code.vegaprotocol.io/vega/protos/data-node/api/v2\222A\217\001\022\036\n\023Vega data node APIs2\007v0.71.0\032\034https://api.testnet.vega.xyz*\002\001\0022\020application/jsonR9\n\003500\0222\n\030An internal server error\022\026\n\024\032\022.google.rpc.Status"
     _GETORDERREQUEST.fields_by_name["order_id"]._options = None
-    _GETORDERREQUEST.fields_by_name["order_id"]._serialized_options = b"\340A\002"
+    _GETORDERREQUEST.fields_by_name["order_id"]._serialized_options = b"\342A\001\002"
     _LISTORDERVERSIONSREQUEST.fields_by_name["order_id"]._options = None
     _LISTORDERVERSIONSREQUEST.fields_by_name[
         "order_id"
-    ]._serialized_options = b"\340A\002"
+    ]._serialized_options = b"\342A\001\002"
     _LISTPOSITIONSREQUEST._options = None
     _LISTPOSITIONSREQUEST._serialized_options = b"\030\001"
     _LISTPOSITIONSRESPONSE._options = None
     _LISTPOSITIONSRESPONSE._serialized_options = b"\030\001"
     _EXPORTLEDGERENTRIESREQUEST.fields_by_name["party_id"]._options = None
     _EXPORTLEDGERENTRIESREQUEST.fields_by_name[
         "party_id"
-    ]._serialized_options = b"\340A\002"
+    ]._serialized_options = b"\342A\001\002"
     _EXPORTLEDGERENTRIESREQUEST.fields_by_name["asset_id"]._options = None
     _EXPORTLEDGERENTRIESREQUEST.fields_by_name[
         "asset_id"
-    ]._serialized_options = b"\340A\002"
+    ]._serialized_options = b"\342A\001\002"
     _GETLATESTMARKETDEPTHREQUEST.fields_by_name["market_id"]._options = None
     _GETLATESTMARKETDEPTHREQUEST.fields_by_name[
         "market_id"
-    ]._serialized_options = b"\340A\002"
+    ]._serialized_options = b"\342A\001\002"
     _GETLATESTMARKETDATAREQUEST.fields_by_name["market_id"]._options = None
     _GETLATESTMARKETDATAREQUEST.fields_by_name[
         "market_id"
-    ]._serialized_options = b"\340A\002"
+    ]._serialized_options = b"\342A\001\002"
     _GETMARKETDATAHISTORYBYIDREQUEST.fields_by_name["market_id"]._options = None
     _GETMARKETDATAHISTORYBYIDREQUEST.fields_by_name[
         "market_id"
-    ]._serialized_options = b"\340A\002"
+    ]._serialized_options = b"\342A\001\002"
     _LISTCANDLEINTERVALSREQUEST.fields_by_name["market_id"]._options = None
     _LISTCANDLEINTERVALSREQUEST.fields_by_name[
         "market_id"
-    ]._serialized_options = b"\340A\002"
+    ]._serialized_options = b"\342A\001\002"
     _OBSERVECANDLEDATAREQUEST.fields_by_name["candle_id"]._options = None
     _OBSERVECANDLEDATAREQUEST.fields_by_name[
         "candle_id"
-    ]._serialized_options = b"\340A\002"
+    ]._serialized_options = b"\342A\001\002"
     _LISTCANDLEDATAREQUEST.fields_by_name["candle_id"]._options = None
     _LISTCANDLEDATAREQUEST.fields_by_name[
         "candle_id"
-    ]._serialized_options = b"\340A\002"
+    ]._serialized_options = b"\342A\001\002"
     _GETERC20LISTASSETBUNDLEREQUEST.fields_by_name["asset_id"]._options = None
     _GETERC20LISTASSETBUNDLEREQUEST.fields_by_name[
         "asset_id"
-    ]._serialized_options = b"\340A\002"
+    ]._serialized_options = b"\342A\001\002"
     _GETERC20SETASSETLIMITSBUNDLEREQUEST.fields_by_name["proposal_id"]._options = None
     _GETERC20SETASSETLIMITSBUNDLEREQUEST.fields_by_name[
         "proposal_id"
-    ]._serialized_options = b"\340A\002"
+    ]._serialized_options = b"\342A\001\002"
     _GETERC20WITHDRAWALAPPROVALREQUEST.fields_by_name["withdrawal_id"]._options = None
     _GETERC20WITHDRAWALAPPROVALREQUEST.fields_by_name[
         "withdrawal_id"
-    ]._serialized_options = b"\340A\002"
+    ]._serialized_options = b"\342A\001\002"
     _GETLASTTRADEREQUEST.fields_by_name["market_id"]._options = None
-    _GETLASTTRADEREQUEST.fields_by_name["market_id"]._serialized_options = b"\340A\002"
+    _GETLASTTRADEREQUEST.fields_by_name[
+        "market_id"
+    ]._serialized_options = b"\342A\001\002"
     _GETORACLESPECREQUEST.fields_by_name["oracle_spec_id"]._options = None
     _GETORACLESPECREQUEST.fields_by_name[
         "oracle_spec_id"
-    ]._serialized_options = b"\340A\002"
+    ]._serialized_options = b"\342A\001\002"
     _GETMARKETREQUEST.fields_by_name["market_id"]._options = None
-    _GETMARKETREQUEST.fields_by_name["market_id"]._serialized_options = b"\340A\002"
+    _GETMARKETREQUEST.fields_by_name["market_id"]._serialized_options = b"\342A\001\002"
+    _LISTSUCCESSORMARKETSREQUEST.fields_by_name["market_id"]._options = None
+    _LISTSUCCESSORMARKETSREQUEST.fields_by_name[
+        "market_id"
+    ]._serialized_options = b"\342A\001\002"
     _GETPARTYREQUEST.fields_by_name["party_id"]._options = None
-    _GETPARTYREQUEST.fields_by_name["party_id"]._serialized_options = b"\340A\002"
+    _GETPARTYREQUEST.fields_by_name["party_id"]._serialized_options = b"\342A\001\002"
     _GETDEPOSITREQUEST.fields_by_name["id"]._options = None
-    _GETDEPOSITREQUEST.fields_by_name["id"]._serialized_options = b"\340A\002"
+    _GETDEPOSITREQUEST.fields_by_name["id"]._serialized_options = b"\342A\001\002"
     _GETWITHDRAWALREQUEST.fields_by_name["id"]._options = None
-    _GETWITHDRAWALREQUEST.fields_by_name["id"]._serialized_options = b"\340A\002"
+    _GETWITHDRAWALREQUEST.fields_by_name["id"]._serialized_options = b"\342A\001\002"
     _GETASSETREQUEST.fields_by_name["asset_id"]._options = None
-    _GETASSETREQUEST.fields_by_name["asset_id"]._serialized_options = b"\340A\002"
+    _GETASSETREQUEST.fields_by_name["asset_id"]._serialized_options = b"\342A\001\002"
     _GETNODEREQUEST.fields_by_name["id"]._options = None
-    _GETNODEREQUEST.fields_by_name["id"]._serialized_options = b"\340A\002"
+    _GETNODEREQUEST.fields_by_name["id"]._serialized_options = b"\342A\001\002"
     _LISTNODESIGNATURESREQUEST.fields_by_name["id"]._options = None
-    _LISTNODESIGNATURESREQUEST.fields_by_name["id"]._serialized_options = b"\340A\002"
+    _LISTNODESIGNATURESREQUEST.fields_by_name[
+        "id"
+    ]._serialized_options = b"\342A\001\002"
     _ESTIMATEFEEREQUEST.fields_by_name["market_id"]._options = None
-    _ESTIMATEFEEREQUEST.fields_by_name["market_id"]._serialized_options = b"\340A\002"
+    _ESTIMATEFEEREQUEST.fields_by_name[
+        "market_id"
+    ]._serialized_options = b"\342A\001\002"
     _ESTIMATEFEEREQUEST.fields_by_name["price"]._options = None
-    _ESTIMATEFEEREQUEST.fields_by_name["price"]._serialized_options = b"\340A\002"
+    _ESTIMATEFEEREQUEST.fields_by_name["price"]._serialized_options = b"\342A\001\002"
     _ESTIMATEFEEREQUEST.fields_by_name["size"]._options = None
-    _ESTIMATEFEEREQUEST.fields_by_name["size"]._serialized_options = b"\340A\002"
+    _ESTIMATEFEEREQUEST.fields_by_name["size"]._serialized_options = b"\342A\001\002"
     _ESTIMATEMARGINREQUEST.fields_by_name["market_id"]._options = None
     _ESTIMATEMARGINREQUEST.fields_by_name[
         "market_id"
-    ]._serialized_options = b"\340A\002"
+    ]._serialized_options = b"\342A\001\002"
     _ESTIMATEMARGINREQUEST.fields_by_name["party_id"]._options = None
-    _ESTIMATEMARGINREQUEST.fields_by_name["party_id"]._serialized_options = b"\340A\002"
+    _ESTIMATEMARGINREQUEST.fields_by_name[
+        "party_id"
+    ]._serialized_options = b"\342A\001\002"
     _ESTIMATEMARGINREQUEST.fields_by_name["side"]._options = None
-    _ESTIMATEMARGINREQUEST.fields_by_name["side"]._serialized_options = b"\340A\002"
+    _ESTIMATEMARGINREQUEST.fields_by_name["side"]._serialized_options = b"\342A\001\002"
     _ESTIMATEMARGINREQUEST.fields_by_name["type"]._options = None
-    _ESTIMATEMARGINREQUEST.fields_by_name["type"]._serialized_options = b"\340A\002"
+    _ESTIMATEMARGINREQUEST.fields_by_name["type"]._serialized_options = b"\342A\001\002"
     _ESTIMATEMARGINREQUEST.fields_by_name["size"]._options = None
-    _ESTIMATEMARGINREQUEST.fields_by_name["size"]._serialized_options = b"\340A\002"
+    _ESTIMATEMARGINREQUEST.fields_by_name["size"]._serialized_options = b"\342A\001\002"
     _ESTIMATEMARGINREQUEST.fields_by_name["price"]._options = None
-    _ESTIMATEMARGINREQUEST.fields_by_name["price"]._serialized_options = b"\340A\002"
+    _ESTIMATEMARGINREQUEST.fields_by_name[
+        "price"
+    ]._serialized_options = b"\342A\001\002"
     _ESTIMATEMARGINREQUEST._options = None
     _ESTIMATEMARGINREQUEST._serialized_options = b"\030\001"
     _ESTIMATEMARGINRESPONSE._options = None
     _ESTIMATEMARGINRESPONSE._serialized_options = b"\030\001"
     _GETNETWORKPARAMETERREQUEST.fields_by_name["key"]._options = None
-    _GETNETWORKPARAMETERREQUEST.fields_by_name["key"]._serialized_options = b"\340A\002"
+    _GETNETWORKPARAMETERREQUEST.fields_by_name[
+        "key"
+    ]._serialized_options = b"\342A\001\002"
     _GETSTAKEREQUEST.fields_by_name["party_id"]._options = None
-    _GETSTAKEREQUEST.fields_by_name["party_id"]._serialized_options = b"\340A\002"
+    _GETSTAKEREQUEST.fields_by_name["party_id"]._serialized_options = b"\342A\001\002"
     _GETRISKFACTORSREQUEST.fields_by_name["market_id"]._options = None
     _GETRISKFACTORSREQUEST.fields_by_name[
         "market_id"
-    ]._serialized_options = b"\340A\002"
+    ]._serialized_options = b"\342A\001\002"
     _LISTENTITIESREQUEST.fields_by_name["transaction_hash"]._options = None
     _LISTENTITIESREQUEST.fields_by_name[
         "transaction_hash"
-    ]._serialized_options = b"\340A\002"
+    ]._serialized_options = b"\342A\001\002"
     _ESTIMATEPOSITIONREQUEST.fields_by_name["market_id"]._options = None
     _ESTIMATEPOSITIONREQUEST.fields_by_name[
         "market_id"
-    ]._serialized_options = b"\340A\002"
+    ]._serialized_options = b"\342A\001\002"
     _ESTIMATEPOSITIONREQUEST.fields_by_name["open_volume"]._options = None
     _ESTIMATEPOSITIONREQUEST.fields_by_name[
         "open_volume"
-    ]._serialized_options = b"\340A\002"
+    ]._serialized_options = b"\342A\001\002"
     _TRADINGDATASERVICE.methods_by_name["ListAccounts"]._options = None
     _TRADINGDATASERVICE.methods_by_name[
         "ListAccounts"
     ]._serialized_options = b"\222A\n\n\010Accounts"
     _TRADINGDATASERVICE.methods_by_name["ObserveAccounts"]._options = None
     _TRADINGDATASERVICE.methods_by_name[
         "ObserveAccounts"
@@ -317,14 +334,18 @@
     _TRADINGDATASERVICE.methods_by_name[
         "GetMarket"
     ]._serialized_options = b"\222A\t\n\007Markets"
     _TRADINGDATASERVICE.methods_by_name["ListMarkets"]._options = None
     _TRADINGDATASERVICE.methods_by_name[
         "ListMarkets"
     ]._serialized_options = b"\222A\t\n\007Markets"
+    _TRADINGDATASERVICE.methods_by_name["ListSuccessorMarkets"]._options = None
+    _TRADINGDATASERVICE.methods_by_name[
+        "ListSuccessorMarkets"
+    ]._serialized_options = b"\222A\t\n\007Markets"
     _TRADINGDATASERVICE.methods_by_name["GetParty"]._options = None
     _TRADINGDATASERVICE.methods_by_name[
         "GetParty"
     ]._serialized_options = b"\222A\t\n\007Parties"
     _TRADINGDATASERVICE.methods_by_name["ListParties"]._options = None
     _TRADINGDATASERVICE.methods_by_name[
         "ListParties"
@@ -515,576 +536,586 @@
     _TRADINGDATASERVICE.methods_by_name[
         "ExportNetworkHistory"
     ]._serialized_options = b"\222A\021\n\017Network history"
     _TRADINGDATASERVICE.methods_by_name["Ping"]._options = None
     _TRADINGDATASERVICE.methods_by_name[
         "Ping"
     ]._serialized_options = b"\222A\006\n\004Misc"
-    _LEDGERENTRYFIELD._serialized_start = 35684
-    _LEDGERENTRYFIELD._serialized_end = 35854
-    _ACCOUNTFIELD._serialized_start = 35857
-    _ACCOUNTFIELD._serialized_end = 36033
-    _TRANSFERDIRECTION._serialized_start = 36036
-    _TRANSFERDIRECTION._serialized_end = 36209
-    _TABLE._serialized_start = 36212
-    _TABLE._serialized_end = 36562
-    _PAGINATION._serialized_start = 335
-    _PAGINATION._serialized_end = 552
-    _PAGEINFO._serialized_start = 555
-    _PAGEINFO._serialized_end = 711
-    _ACCOUNTBALANCE._serialized_start = 714
-    _ACCOUNTBALANCE._serialized_end = 868
-    _LISTACCOUNTSREQUEST._serialized_start = 871
-    _LISTACCOUNTSREQUEST._serialized_end = 1029
-    _LISTACCOUNTSRESPONSE._serialized_start = 1031
-    _LISTACCOUNTSRESPONSE._serialized_end = 1118
-    _ACCOUNTSCONNECTION._serialized_start = 1121
-    _ACCOUNTSCONNECTION._serialized_end = 1249
-    _ACCOUNTEDGE._serialized_start = 1251
-    _ACCOUNTEDGE._serialized_end = 1341
-    _OBSERVEACCOUNTSREQUEST._serialized_start = 1344
-    _OBSERVEACCOUNTSREQUEST._serialized_end = 1485
-    _OBSERVEACCOUNTSRESPONSE._serialized_start = 1488
-    _OBSERVEACCOUNTSRESPONSE._serialized_end = 1654
-    _ACCOUNTSNAPSHOTPAGE._serialized_start = 1656
-    _ACCOUNTSNAPSHOTPAGE._serialized_end = 1767
-    _ACCOUNTUPDATES._serialized_start = 1769
-    _ACCOUNTUPDATES._serialized_end = 1846
-    _INFOREQUEST._serialized_start = 1848
-    _INFOREQUEST._serialized_end = 1861
-    _INFORESPONSE._serialized_start = 1863
-    _INFORESPONSE._serialized_end = 1936
-    _GETORDERREQUEST._serialized_start = 1938
-    _GETORDERREQUEST._serialized_end = 2030
-    _GETORDERRESPONSE._serialized_start = 2032
-    _GETORDERRESPONSE._serialized_end = 2085
-    _ORDERFILTER._serialized_start = 2088
-    _ORDERFILTER._serialized_end = 2533
-    _LISTORDERSREQUEST._serialized_start = 2536
-    _LISTORDERSREQUEST._serialized_end = 2706
-    _LISTORDERSRESPONSE._serialized_start = 2708
-    _LISTORDERSRESPONSE._serialized_end = 2786
-    _LISTORDERVERSIONSREQUEST._serialized_start = 2789
-    _LISTORDERVERSIONSREQUEST._serialized_end = 2928
-    _LISTORDERVERSIONSRESPONSE._serialized_start = 2930
-    _LISTORDERVERSIONSRESPONSE._serialized_end = 3015
-    _OBSERVEORDERSREQUEST._serialized_start = 3018
-    _OBSERVEORDERSREQUEST._serialized_end = 3172
-    _OBSERVEORDERSRESPONSE._serialized_start = 3175
-    _OBSERVEORDERSRESPONSE._serialized_end = 3335
-    _ORDERSNAPSHOTPAGE._serialized_start = 3337
-    _ORDERSNAPSHOTPAGE._serialized_end = 3422
-    _ORDERUPDATES._serialized_start = 3424
-    _ORDERUPDATES._serialized_end = 3475
-    _LISTPOSITIONSREQUEST._serialized_start = 3478
-    _LISTPOSITIONSREQUEST._serialized_end = 3641
-    _LISTPOSITIONSRESPONSE._serialized_start = 3643
-    _LISTPOSITIONSRESPONSE._serialized_end = 3737
-    _POSITIONSFILTER._serialized_start = 3739
-    _POSITIONSFILTER._serialized_end = 3816
-    _LISTALLPOSITIONSREQUEST._serialized_start = 3819
-    _LISTALLPOSITIONSREQUEST._serialized_end = 3983
-    _LISTALLPOSITIONSRESPONSE._serialized_start = 3985
-    _LISTALLPOSITIONSRESPONSE._serialized_end = 4078
-    _POSITIONEDGE._serialized_start = 4080
-    _POSITIONEDGE._serialized_end = 4154
-    _POSITIONCONNECTION._serialized_start = 4157
-    _POSITIONCONNECTION._serialized_end = 4286
-    _OBSERVEPOSITIONSREQUEST._serialized_start = 4288
-    _OBSERVEPOSITIONSREQUEST._serialized_end = 4406
-    _OBSERVEPOSITIONSRESPONSE._serialized_start = 4409
-    _OBSERVEPOSITIONSRESPONSE._serialized_end = 4578
-    _POSITIONSNAPSHOTPAGE._serialized_start = 4580
-    _POSITIONSNAPSHOTPAGE._serialized_end = 4677
-    _POSITIONUPDATES._serialized_start = 4679
-    _POSITIONUPDATES._serialized_end = 4742
-    _LEDGERENTRYFILTER._serialized_start = 4745
-    _LEDGERENTRYFILTER._serialized_end = 5036
-    _AGGREGATEDLEDGERENTRY._serialized_start = 5039
-    _AGGREGATEDLEDGERENTRY._serialized_end = 5768
-    _LISTLEDGERENTRIESREQUEST._serialized_start = 5771
-    _LISTLEDGERENTRIESREQUEST._serialized_end = 6017
-    _EXPORTLEDGERENTRIESREQUEST._serialized_start = 6020
-    _EXPORTLEDGERENTRIESREQUEST._serialized_end = 6191
-    _LISTLEDGERENTRIESRESPONSE._serialized_start = 6193
-    _LISTLEDGERENTRIESRESPONSE._serialized_end = 6311
-    _AGGREGATEDLEDGERENTRIESEDGE._serialized_start = 6313
-    _AGGREGATEDLEDGERENTRIESEDGE._serialized_end = 6426
-    _AGGREGATEDLEDGERENTRIESCONNECTION._serialized_start = 6429
-    _AGGREGATEDLEDGERENTRIESCONNECTION._serialized_end = 6588
-    _LISTBALANCECHANGESREQUEST._serialized_start = 6591
-    _LISTBALANCECHANGESREQUEST._serialized_end = 6834
-    _LISTBALANCECHANGESRESPONSE._serialized_start = 6836
-    _LISTBALANCECHANGESRESPONSE._serialized_end = 6938
-    _GETBALANCEHISTORYREQUEST._serialized_start = 6941
-    _GETBALANCEHISTORYREQUEST._serialized_end = 7241
-    _GETBALANCEHISTORYRESPONSE._serialized_start = 7243
-    _GETBALANCEHISTORYRESPONSE._serialized_end = 7344
-    _AGGREGATEDBALANCEEDGE._serialized_start = 7346
-    _AGGREGATEDBALANCEEDGE._serialized_end = 7449
-    _AGGREGATEDBALANCECONNECTION._serialized_start = 7452
-    _AGGREGATEDBALANCECONNECTION._serialized_end = 7599
-    _ACCOUNTFILTER._serialized_start = 7602
-    _ACCOUNTFILTER._serialized_end = 7760
-    _AGGREGATEDBALANCE._serialized_start = 7763
-    _AGGREGATEDBALANCE._serialized_end = 8052
-    _OBSERVEMARKETSDEPTHREQUEST._serialized_start = 8054
-    _OBSERVEMARKETSDEPTHREQUEST._serialized_end = 8113
-    _OBSERVEMARKETSDEPTHRESPONSE._serialized_start = 8115
-    _OBSERVEMARKETSDEPTHRESPONSE._serialized_end = 8198
-    _OBSERVEMARKETSDEPTHUPDATESREQUEST._serialized_start = 8200
-    _OBSERVEMARKETSDEPTHUPDATESREQUEST._serialized_end = 8266
-    _OBSERVEMARKETSDEPTHUPDATESRESPONSE._serialized_start = 8268
-    _OBSERVEMARKETSDEPTHUPDATESRESPONSE._serialized_end = 8353
-    _OBSERVEMARKETSDATAREQUEST._serialized_start = 8355
-    _OBSERVEMARKETSDATAREQUEST._serialized_end = 8413
-    _OBSERVEMARKETSDATARESPONSE._serialized_start = 8415
-    _OBSERVEMARKETSDATARESPONSE._serialized_end = 8494
-    _GETLATESTMARKETDEPTHREQUEST._serialized_start = 8496
-    _GETLATESTMARKETDEPTHREQUEST._serialized_end = 8607
-    _GETLATESTMARKETDEPTHRESPONSE._serialized_start = 8610
-    _GETLATESTMARKETDEPTHRESPONSE._serialized_end = 8828
-    _LISTLATESTMARKETDATAREQUEST._serialized_start = 8830
-    _LISTLATESTMARKETDATAREQUEST._serialized_end = 8859
-    _LISTLATESTMARKETDATARESPONSE._serialized_start = 8861
-    _LISTLATESTMARKETDATARESPONSE._serialized_end = 8944
-    _GETLATESTMARKETDATAREQUEST._serialized_start = 8946
-    _GETLATESTMARKETDATAREQUEST._serialized_end = 9008
-    _GETLATESTMARKETDATARESPONSE._serialized_start = 9010
-    _GETLATESTMARKETDATARESPONSE._serialized_end = 9090
-    _GETMARKETDATAHISTORYBYIDREQUEST._serialized_start = 9093
-    _GETMARKETDATAHISTORYBYIDREQUEST._serialized_end = 9373
-    _GETMARKETDATAHISTORYBYIDRESPONSE._serialized_start = 9375
-    _GETMARKETDATAHISTORYBYIDRESPONSE._serialized_end = 9481
-    _MARKETDATAEDGE._serialized_start = 9483
-    _MARKETDATAEDGE._serialized_end = 9561
-    _MARKETDATACONNECTION._serialized_start = 9564
-    _MARKETDATACONNECTION._serialized_end = 9697
-    _LISTTRANSFERSREQUEST._serialized_start = 9700
-    _LISTTRANSFERSREQUEST._serialized_end = 9909
-    _LISTTRANSFERSRESPONSE._serialized_start = 9911
-    _LISTTRANSFERSRESPONSE._serialized_end = 10001
-    _TRANSFEREDGE._serialized_start = 10003
-    _TRANSFEREDGE._serialized_end = 10087
-    _TRANSFERCONNECTION._serialized_start = 10090
-    _TRANSFERCONNECTION._serialized_end = 10219
-    _GETNETWORKLIMITSREQUEST._serialized_start = 10221
-    _GETNETWORKLIMITSREQUEST._serialized_end = 10246
-    _GETNETWORKLIMITSRESPONSE._serialized_start = 10248
-    _GETNETWORKLIMITSRESPONSE._serialized_end = 10319
-    _LISTCANDLEINTERVALSREQUEST._serialized_start = 10321
-    _LISTCANDLEINTERVALSREQUEST._serialized_end = 10383
-    _INTERVALTOCANDLEID._serialized_start = 10385
-    _INTERVALTOCANDLEID._serialized_end = 10462
-    _LISTCANDLEINTERVALSRESPONSE._serialized_start = 10464
-    _LISTCANDLEINTERVALSRESPONSE._serialized_end = 10581
-    _CANDLE._serialized_start = 10584
-    _CANDLE._serialized_end = 10751
-    _OBSERVECANDLEDATAREQUEST._serialized_start = 10753
-    _OBSERVECANDLEDATAREQUEST._serialized_end = 10813
-    _OBSERVECANDLEDATARESPONSE._serialized_start = 10815
-    _OBSERVECANDLEDATARESPONSE._serialized_end = 10891
-    _LISTCANDLEDATAREQUEST._serialized_start = 10894
-    _LISTCANDLEDATAREQUEST._serialized_end = 11112
-    _LISTCANDLEDATARESPONSE._serialized_start = 11114
-    _LISTCANDLEDATARESPONSE._serialized_end = 11203
-    _CANDLEEDGE._serialized_start = 11205
-    _CANDLEEDGE._serialized_end = 11286
-    _CANDLEDATACONNECTION._serialized_start = 11289
-    _CANDLEDATACONNECTION._serialized_end = 11418
-    _LISTVOTESREQUEST._serialized_start = 11421
-    _LISTVOTESREQUEST._serialized_end = 11619
-    _LISTVOTESRESPONSE._serialized_start = 11621
-    _LISTVOTESRESPONSE._serialized_end = 11695
-    _VOTEEDGE._serialized_start = 11697
-    _VOTEEDGE._serialized_end = 11763
-    _VOTECONNECTION._serialized_start = 11765
-    _VOTECONNECTION._serialized_end = 11886
-    _OBSERVEVOTESREQUEST._serialized_start = 11888
-    _OBSERVEVOTESREQUEST._serialized_end = 12008
-    _OBSERVEVOTESRESPONSE._serialized_start = 12010
-    _OBSERVEVOTESRESPONSE._serialized_end = 12064
-    _LISTERC20MULTISIGSIGNERADDEDBUNDLESREQUEST._serialized_start = 12067
-    _LISTERC20MULTISIGSIGNERADDEDBUNDLESREQUEST._serialized_end = 12256
-    _LISTERC20MULTISIGSIGNERADDEDBUNDLESRESPONSE._serialized_start = 12258
-    _LISTERC20MULTISIGSIGNERADDEDBUNDLESRESPONSE._serialized_end = 12382
-    _ERC20MULTISIGSIGNERADDEDEDGE._serialized_start = 12384
-    _ERC20MULTISIGSIGNERADDEDEDGE._serialized_end = 12500
-    _ERC20MULTISIGSIGNERADDEDBUNDLEEDGE._serialized_start = 12503
-    _ERC20MULTISIGSIGNERADDEDBUNDLEEDGE._serialized_end = 12632
-    _ERC20MULTISIGSIGNERADDEDCONNECTION._serialized_start = 12635
-    _ERC20MULTISIGSIGNERADDEDCONNECTION._serialized_end = 12802
-    _ERC20MULTISIGSIGNERADDEDBUNDLE._serialized_start = 12805
-    _ERC20MULTISIGSIGNERADDEDBUNDLE._serialized_end = 13011
-    _LISTERC20MULTISIGSIGNERREMOVEDBUNDLESREQUEST._serialized_start = 13014
-    _LISTERC20MULTISIGSIGNERREMOVEDBUNDLESREQUEST._serialized_end = 13205
-    _LISTERC20MULTISIGSIGNERREMOVEDBUNDLESRESPONSE._serialized_start = 13208
-    _LISTERC20MULTISIGSIGNERREMOVEDBUNDLESRESPONSE._serialized_end = 13336
-    _ERC20MULTISIGSIGNERREMOVEDEDGE._serialized_start = 13338
-    _ERC20MULTISIGSIGNERREMOVEDEDGE._serialized_end = 13458
-    _ERC20MULTISIGSIGNERREMOVEDBUNDLEEDGE._serialized_start = 13461
-    _ERC20MULTISIGSIGNERREMOVEDBUNDLEEDGE._serialized_end = 13594
-    _ERC20MULTISIGSIGNERREMOVEDCONNECTION._serialized_start = 13597
-    _ERC20MULTISIGSIGNERREMOVEDCONNECTION._serialized_end = 13768
-    _ERC20MULTISIGSIGNERREMOVEDBUNDLE._serialized_start = 13771
-    _ERC20MULTISIGSIGNERREMOVEDBUNDLE._serialized_end = 13979
-    _GETERC20LISTASSETBUNDLEREQUEST._serialized_start = 13981
-    _GETERC20LISTASSETBUNDLEREQUEST._serialized_end = 14045
-    _GETERC20LISTASSETBUNDLERESPONSE._serialized_start = 14048
-    _GETERC20LISTASSETBUNDLERESPONSE._serialized_end = 14206
-    _GETERC20SETASSETLIMITSBUNDLEREQUEST._serialized_start = 14208
-    _GETERC20SETASSETLIMITSBUNDLEREQUEST._serialized_end = 14283
-    _GETERC20SETASSETLIMITSBUNDLERESPONSE._serialized_start = 14286
-    _GETERC20SETASSETLIMITSBUNDLERESPONSE._serialized_end = 14518
-    _GETERC20WITHDRAWALAPPROVALREQUEST._serialized_start = 14520
-    _GETERC20WITHDRAWALAPPROVALREQUEST._serialized_end = 14597
-    _GETERC20WITHDRAWALAPPROVALRESPONSE._serialized_start = 14600
-    _GETERC20WITHDRAWALAPPROVALRESPONSE._serialized_end = 14822
-    _GETLASTTRADEREQUEST._serialized_start = 14824
-    _GETLASTTRADEREQUEST._serialized_end = 14879
-    _GETLASTTRADERESPONSE._serialized_start = 14881
-    _GETLASTTRADERESPONSE._serialized_end = 14938
-    _LISTTRADESREQUEST._serialized_start = 14941
-    _LISTTRADESREQUEST._serialized_end = 15209
-    _LISTTRADESRESPONSE._serialized_start = 15211
-    _LISTTRADESRESPONSE._serialized_end = 15289
-    _TRADECONNECTION._serialized_start = 15291
-    _TRADECONNECTION._serialized_end = 15414
-    _TRADEEDGE._serialized_start = 15416
-    _TRADEEDGE._serialized_end = 15484
-    _OBSERVETRADESREQUEST._serialized_start = 15486
-    _OBSERVETRADESREQUEST._serialized_end = 15568
-    _OBSERVETRADESRESPONSE._serialized_start = 15570
-    _OBSERVETRADESRESPONSE._serialized_end = 15630
-    _GETORACLESPECREQUEST._serialized_start = 15632
-    _GETORACLESPECREQUEST._serialized_end = 15697
-    _GETORACLESPECRESPONSE._serialized_start = 15699
-    _GETORACLESPECRESPONSE._serialized_end = 15773
-    _LISTORACLESPECSREQUEST._serialized_start = 15775
-    _LISTORACLESPECSREQUEST._serialized_end = 15880
-    _LISTORACLESPECSRESPONSE._serialized_start = 15882
-    _LISTORACLESPECSRESPONSE._serialized_end = 15982
-    _LISTORACLEDATAREQUEST._serialized_start = 15985
-    _LISTORACLEDATAREQUEST._serialized_end = 16151
-    _LISTORACLEDATARESPONSE._serialized_start = 16153
-    _LISTORACLEDATARESPONSE._serialized_end = 16249
-    _ORACLESPECEDGE._serialized_start = 16251
-    _ORACLESPECEDGE._serialized_end = 16329
-    _ORACLESPECSCONNECTION._serialized_start = 16332
-    _ORACLESPECSCONNECTION._serialized_end = 16466
-    _ORACLEDATAEDGE._serialized_start = 16468
-    _ORACLEDATAEDGE._serialized_end = 16546
-    _ORACLEDATACONNECTION._serialized_start = 16549
-    _ORACLEDATACONNECTION._serialized_end = 16682
-    _GETMARKETREQUEST._serialized_start = 16684
-    _GETMARKETREQUEST._serialized_end = 16736
-    _GETMARKETRESPONSE._serialized_start = 16738
-    _GETMARKETRESPONSE._serialized_end = 16795
-    _LISTMARKETSREQUEST._serialized_start = 16798
-    _LISTMARKETSREQUEST._serialized_end = 16965
-    _LISTMARKETSRESPONSE._serialized_start = 16967
-    _LISTMARKETSRESPONSE._serialized_end = 17049
-    _MARKETEDGE._serialized_start = 17051
-    _MARKETEDGE._serialized_end = 17121
-    _MARKETCONNECTION._serialized_start = 17123
-    _MARKETCONNECTION._serialized_end = 17248
-    _GETPARTYREQUEST._serialized_start = 17250
-    _GETPARTYREQUEST._serialized_end = 17299
-    _GETPARTYRESPONSE._serialized_start = 17301
-    _GETPARTYRESPONSE._serialized_end = 17354
-    _LISTPARTIESREQUEST._serialized_start = 17356
-    _LISTPARTIESREQUEST._serialized_end = 17464
-    _LISTPARTIESRESPONSE._serialized_start = 17466
-    _LISTPARTIESRESPONSE._serialized_end = 17547
-    _PARTYEDGE._serialized_start = 17549
-    _PARTYEDGE._serialized_end = 17617
-    _PARTYCONNECTION._serialized_start = 17619
-    _PARTYCONNECTION._serialized_end = 17742
-    _ORDEREDGE._serialized_start = 17744
-    _ORDEREDGE._serialized_end = 17812
-    _LISTMARGINLEVELSREQUEST._serialized_start = 17815
-    _LISTMARGINLEVELSREQUEST._serialized_end = 17957
-    _LISTMARGINLEVELSRESPONSE._serialized_start = 17959
-    _LISTMARGINLEVELSRESPONSE._serialized_end = 18057
-    _OBSERVEMARGINLEVELSREQUEST._serialized_start = 18059
-    _OBSERVEMARGINLEVELSREQUEST._serialized_end = 18162
-    _OBSERVEMARGINLEVELSRESPONSE._serialized_start = 18164
-    _OBSERVEMARGINLEVELSRESPONSE._serialized_end = 18250
-    _ORDERCONNECTION._serialized_start = 18252
-    _ORDERCONNECTION._serialized_end = 18375
-    _MARGINEDGE._serialized_start = 18377
-    _MARGINEDGE._serialized_end = 18453
-    _MARGINCONNECTION._serialized_start = 18455
-    _MARGINCONNECTION._serialized_end = 18580
-    _LISTREWARDSREQUEST._serialized_start = 18583
-    _LISTREWARDSREQUEST._serialized_end = 18852
-    _LISTREWARDSRESPONSE._serialized_start = 18854
-    _LISTREWARDSRESPONSE._serialized_end = 18937
-    _REWARDEDGE._serialized_start = 18939
-    _REWARDEDGE._serialized_end = 19009
-    _REWARDSCONNECTION._serialized_start = 19011
-    _REWARDSCONNECTION._serialized_end = 19137
-    _LISTREWARDSUMMARIESREQUEST._serialized_start = 19140
-    _LISTREWARDSUMMARIESREQUEST._serialized_end = 19339
-    _LISTREWARDSUMMARIESRESPONSE._serialized_start = 19341
-    _LISTREWARDSUMMARIESRESPONSE._serialized_end = 19421
-    _REWARDSUMMARYFILTER._serialized_start = 19424
-    _REWARDSUMMARYFILTER._serialized_end = 19601
-    _LISTEPOCHREWARDSUMMARIESREQUEST._serialized_start = 19604
-    _LISTEPOCHREWARDSUMMARIESREQUEST._serialized_end = 19780
-    _LISTEPOCHREWARDSUMMARIESRESPONSE._serialized_start = 19782
-    _LISTEPOCHREWARDSUMMARIESRESPONSE._serialized_end = 19893
-    _EPOCHREWARDSUMMARYCONNECTION._serialized_start = 19896
-    _EPOCHREWARDSUMMARYCONNECTION._serialized_end = 20045
-    _EPOCHREWARDSUMMARYEDGE._serialized_start = 20047
-    _EPOCHREWARDSUMMARYEDGE._serialized_end = 20141
-    _OBSERVEREWARDSREQUEST._serialized_start = 20143
-    _OBSERVEREWARDSREQUEST._serialized_end = 20256
-    _OBSERVEREWARDSRESPONSE._serialized_start = 20258
-    _OBSERVEREWARDSRESPONSE._serialized_end = 20320
-    _GETDEPOSITREQUEST._serialized_start = 20322
-    _GETDEPOSITREQUEST._serialized_end = 20362
-    _GETDEPOSITRESPONSE._serialized_start = 20364
-    _GETDEPOSITRESPONSE._serialized_end = 20425
-    _LISTDEPOSITSREQUEST._serialized_start = 20428
-    _LISTDEPOSITSREQUEST._serialized_end = 20636
-    _LISTDEPOSITSRESPONSE._serialized_start = 20638
-    _LISTDEPOSITSRESPONSE._serialized_end = 20725
-    _DEPOSITEDGE._serialized_start = 20727
-    _DEPOSITEDGE._serialized_end = 20799
-    _DEPOSITSCONNECTION._serialized_start = 20802
-    _DEPOSITSCONNECTION._serialized_end = 20930
-    _GETWITHDRAWALREQUEST._serialized_start = 20932
-    _GETWITHDRAWALREQUEST._serialized_end = 20975
-    _GETWITHDRAWALRESPONSE._serialized_start = 20977
-    _GETWITHDRAWALRESPONSE._serialized_end = 21050
-    _LISTWITHDRAWALSREQUEST._serialized_start = 21053
-    _LISTWITHDRAWALSREQUEST._serialized_end = 21264
-    _LISTWITHDRAWALSRESPONSE._serialized_start = 21266
-    _LISTWITHDRAWALSRESPONSE._serialized_end = 21365
-    _WITHDRAWALEDGE._serialized_start = 21367
-    _WITHDRAWALEDGE._serialized_end = 21445
-    _WITHDRAWALSCONNECTION._serialized_start = 21448
-    _WITHDRAWALSCONNECTION._serialized_end = 21582
-    _GETASSETREQUEST._serialized_start = 21584
-    _GETASSETREQUEST._serialized_end = 21633
-    _GETASSETRESPONSE._serialized_start = 21635
-    _GETASSETRESPONSE._serialized_end = 21688
-    _LISTASSETSREQUEST._serialized_start = 21691
-    _LISTASSETSREQUEST._serialized_end = 21836
-    _LISTASSETSRESPONSE._serialized_start = 21838
-    _LISTASSETSRESPONSE._serialized_end = 21917
-    _ASSETEDGE._serialized_start = 21919
-    _ASSETEDGE._serialized_end = 21987
-    _ASSETSCONNECTION._serialized_start = 21989
-    _ASSETSCONNECTION._serialized_end = 22113
-    _LISTLIQUIDITYPROVISIONSREQUEST._serialized_start = 22116
-    _LISTLIQUIDITYPROVISIONSREQUEST._serialized_end = 22405
-    _LISTLIQUIDITYPROVISIONSRESPONSE._serialized_start = 22408
-    _LISTLIQUIDITYPROVISIONSRESPONSE._serialized_end = 22540
-    _LIQUIDITYPROVISIONSEDGE._serialized_start = 22542
-    _LIQUIDITYPROVISIONSEDGE._serialized_end = 22637
-    _LIQUIDITYPROVISIONSCONNECTION._serialized_start = 22640
-    _LIQUIDITYPROVISIONSCONNECTION._serialized_end = 22791
-    _OBSERVELIQUIDITYPROVISIONSREQUEST._serialized_start = 22794
-    _OBSERVELIQUIDITYPROVISIONSREQUEST._serialized_end = 22922
-    _OBSERVELIQUIDITYPROVISIONSRESPONSE._serialized_start = 22924
-    _OBSERVELIQUIDITYPROVISIONSRESPONSE._serialized_end = 23037
-    _GETGOVERNANCEDATAREQUEST._serialized_start = 23040
-    _GETGOVERNANCEDATAREQUEST._serialized_end = 23169
-    _GETGOVERNANCEDATARESPONSE._serialized_start = 23171
-    _GETGOVERNANCEDATARESPONSE._serialized_end = 23240
-    _LISTGOVERNANCEDATAREQUEST._serialized_start = 23243
-    _LISTGOVERNANCEDATAREQUEST._serialized_end = 23877
-    _LISTGOVERNANCEDATAREQUEST_TYPE._serialized_start = 23597
-    _LISTGOVERNANCEDATAREQUEST_TYPE._serialized_end = 23780
-    _LISTGOVERNANCEDATARESPONSE._serialized_start = 23879
-    _LISTGOVERNANCEDATARESPONSE._serialized_end = 23982
-    _GOVERNANCEDATAEDGE._serialized_start = 23984
-    _GOVERNANCEDATAEDGE._serialized_end = 24070
-    _GOVERNANCEDATACONNECTION._serialized_start = 24073
-    _GOVERNANCEDATACONNECTION._serialized_end = 24214
-    _OBSERVEGOVERNANCEREQUEST._serialized_start = 24216
-    _OBSERVEGOVERNANCEREQUEST._serialized_end = 24287
-    _OBSERVEGOVERNANCERESPONSE._serialized_start = 24289
-    _OBSERVEGOVERNANCERESPONSE._serialized_end = 24358
-    _LISTDELEGATIONSREQUEST._serialized_start = 24361
-    _LISTDELEGATIONSREQUEST._serialized_end = 24598
-    _LISTDELEGATIONSRESPONSE._serialized_start = 24600
-    _LISTDELEGATIONSRESPONSE._serialized_end = 24699
-    _DELEGATIONEDGE._serialized_start = 24701
-    _DELEGATIONEDGE._serialized_end = 24779
-    _DELEGATIONSCONNECTION._serialized_start = 24782
-    _DELEGATIONSCONNECTION._serialized_end = 24916
-    _OBSERVEDELEGATIONSREQUEST._serialized_start = 24918
-    _OBSERVEDELEGATIONSREQUEST._serialized_end = 25032
-    _OBSERVEDELEGATIONSRESPONSE._serialized_start = 25034
-    _OBSERVEDELEGATIONSRESPONSE._serialized_end = 25112
-    _NODEBASIC._serialized_start = 25115
-    _NODEBASIC._serialized_end = 25388
-    _GETNETWORKDATAREQUEST._serialized_start = 25390
-    _GETNETWORKDATAREQUEST._serialized_end = 25413
-    _GETNETWORKDATARESPONSE._serialized_start = 25415
-    _GETNETWORKDATARESPONSE._serialized_end = 25484
-    _GETNODEREQUEST._serialized_start = 25486
-    _GETNODEREQUEST._serialized_end = 25523
-    _GETNODERESPONSE._serialized_start = 25525
-    _GETNODERESPONSE._serialized_end = 25574
-    _LISTNODESREQUEST._serialized_start = 25577
-    _LISTNODESREQUEST._serialized_end = 25724
-    _LISTNODESRESPONSE._serialized_start = 25726
-    _LISTNODESRESPONSE._serialized_end = 25801
-    _NODEEDGE._serialized_start = 25803
-    _NODEEDGE._serialized_end = 25869
-    _NODESCONNECTION._serialized_start = 25871
-    _NODESCONNECTION._serialized_end = 25993
-    _LISTNODESIGNATURESREQUEST._serialized_start = 25996
-    _LISTNODESIGNATURESREQUEST._serialized_end = 26125
-    _LISTNODESIGNATURESRESPONSE._serialized_start = 26127
-    _LISTNODESIGNATURESRESPONSE._serialized_end = 26230
-    _NODESIGNATUREEDGE._serialized_start = 26232
-    _NODESIGNATUREEDGE._serialized_end = 26328
-    _NODESIGNATURESCONNECTION._serialized_start = 26331
-    _NODESIGNATURESCONNECTION._serialized_end = 26471
-    _GETEPOCHREQUEST._serialized_start = 26473
-    _GETEPOCHREQUEST._serialized_end = 26518
-    _GETEPOCHRESPONSE._serialized_start = 26520
-    _GETEPOCHRESPONSE._serialized_end = 26573
-    _ESTIMATEFEEREQUEST._serialized_start = 26575
-    _ESTIMATEFEEREQUEST._serialized_end = 26681
-    _ESTIMATEFEERESPONSE._serialized_start = 26683
-    _ESTIMATEFEERESPONSE._serialized_end = 26733
-    _ESTIMATEMARGINREQUEST._serialized_start = 26736
-    _ESTIMATEMARGINREQUEST._serialized_end = 26961
-    _ESTIMATEMARGINRESPONSE._serialized_start = 26963
-    _ESTIMATEMARGINRESPONSE._serialized_end = 27048
-    _LISTNETWORKPARAMETERSREQUEST._serialized_start = 27050
-    _LISTNETWORKPARAMETERSREQUEST._serialized_end = 27161
-    _LISTNETWORKPARAMETERSRESPONSE._serialized_start = 27163
-    _LISTNETWORKPARAMETERSRESPONSE._serialized_end = 27286
-    _GETNETWORKPARAMETERREQUEST._serialized_start = 27288
-    _GETNETWORKPARAMETERREQUEST._serialized_end = 27339
-    _GETNETWORKPARAMETERRESPONSE._serialized_start = 27341
-    _GETNETWORKPARAMETERRESPONSE._serialized_end = 27439
-    _NETWORKPARAMETEREDGE._serialized_start = 27441
-    _NETWORKPARAMETEREDGE._serialized_end = 27531
-    _NETWORKPARAMETERCONNECTION._serialized_start = 27534
-    _NETWORKPARAMETERCONNECTION._serialized_end = 27679
-    _CHECKPOINT._serialized_start = 27681
-    _CHECKPOINT._serialized_end = 27771
-    _LISTCHECKPOINTSREQUEST._serialized_start = 27773
-    _LISTCHECKPOINTSREQUEST._serialized_end = 27878
-    _LISTCHECKPOINTSRESPONSE._serialized_start = 27880
-    _LISTCHECKPOINTSRESPONSE._serialized_end = 27979
-    _CHECKPOINTEDGE._serialized_start = 27981
-    _CHECKPOINTEDGE._serialized_end = 28070
-    _CHECKPOINTSCONNECTION._serialized_start = 28073
-    _CHECKPOINTSCONNECTION._serialized_end = 28207
-    _GETSTAKEREQUEST._serialized_start = 28210
-    _GETSTAKEREQUEST._serialized_end = 28340
-    _GETSTAKERESPONSE._serialized_start = 28343
-    _GETSTAKERESPONSE._serialized_end = 28491
-    _STAKELINKINGEDGE._serialized_start = 28493
-    _STAKELINKINGEDGE._serialized_end = 28585
-    _STAKESCONNECTION._serialized_start = 28588
-    _STAKESCONNECTION._serialized_end = 28719
-    _GETRISKFACTORSREQUEST._serialized_start = 28721
-    _GETRISKFACTORSREQUEST._serialized_end = 28778
-    _GETRISKFACTORSRESPONSE._serialized_start = 28780
-    _GETRISKFACTORSRESPONSE._serialized_end = 28855
-    _OBSERVEEVENTBUSREQUEST._serialized_start = 28858
-    _OBSERVEEVENTBUSREQUEST._serialized_end = 29019
-    _OBSERVEEVENTBUSRESPONSE._serialized_start = 29021
-    _OBSERVEEVENTBUSRESPONSE._serialized_end = 29096
-    _OBSERVELEDGERMOVEMENTSREQUEST._serialized_start = 29098
-    _OBSERVELEDGERMOVEMENTSREQUEST._serialized_end = 29129
-    _OBSERVELEDGERMOVEMENTSRESPONSE._serialized_start = 29131
-    _OBSERVELEDGERMOVEMENTSRESPONSE._serialized_end = 29226
-    _LISTKEYROTATIONSREQUEST._serialized_start = 29229
-    _LISTKEYROTATIONSREQUEST._serialized_end = 29377
-    _LISTKEYROTATIONSRESPONSE._serialized_start = 29379
-    _LISTKEYROTATIONSRESPONSE._serialized_end = 29475
-    _KEYROTATIONEDGE._serialized_start = 29477
-    _KEYROTATIONEDGE._serialized_end = 29567
-    _KEYROTATIONCONNECTION._serialized_start = 29570
-    _KEYROTATIONCONNECTION._serialized_end = 29705
-    _LISTETHEREUMKEYROTATIONSREQUEST._serialized_start = 29708
-    _LISTETHEREUMKEYROTATIONSREQUEST._serialized_end = 29864
-    _LISTETHEREUMKEYROTATIONSRESPONSE._serialized_start = 29866
-    _LISTETHEREUMKEYROTATIONSRESPONSE._serialized_end = 29986
-    _ETHEREUMKEYROTATIONSCONNECTION._serialized_start = 29989
-    _ETHEREUMKEYROTATIONSCONNECTION._serialized_end = 30141
-    _ETHEREUMKEYROTATIONEDGE._serialized_start = 30143
-    _ETHEREUMKEYROTATIONEDGE._serialized_end = 30249
-    _GETVEGATIMEREQUEST._serialized_start = 30251
-    _GETVEGATIMEREQUEST._serialized_end = 30271
-    _GETVEGATIMERESPONSE._serialized_start = 30273
-    _GETVEGATIMERESPONSE._serialized_end = 30324
-    _DATERANGE._serialized_start = 30327
-    _DATERANGE._serialized_end = 30464
-    _GETPROTOCOLUPGRADESTATUSREQUEST._serialized_start = 30466
-    _GETPROTOCOLUPGRADESTATUSREQUEST._serialized_end = 30499
-    _GETPROTOCOLUPGRADESTATUSRESPONSE._serialized_start = 30501
-    _GETPROTOCOLUPGRADESTATUSRESPONSE._serialized_end = 30557
-    _LISTPROTOCOLUPGRADEPROPOSALSREQUEST._serialized_start = 30560
-    _LISTPROTOCOLUPGRADEPROPOSALSREQUEST._serialized_end = 30819
-    _LISTPROTOCOLUPGRADEPROPOSALSRESPONSE._serialized_start = 30822
-    _LISTPROTOCOLUPGRADEPROPOSALSRESPONSE._serialized_end = 30974
-    _PROTOCOLUPGRADEPROPOSALCONNECTION._serialized_start = 30977
-    _PROTOCOLUPGRADEPROPOSALCONNECTION._serialized_end = 31136
-    _PROTOCOLUPGRADEPROPOSALEDGE._serialized_start = 31138
-    _PROTOCOLUPGRADEPROPOSALEDGE._serialized_end = 31249
-    _LISTCORESNAPSHOTSREQUEST._serialized_start = 31251
-    _LISTCORESNAPSHOTSREQUEST._serialized_end = 31358
-    _LISTCORESNAPSHOTSRESPONSE._serialized_start = 31360
-    _LISTCORESNAPSHOTSRESPONSE._serialized_end = 31467
-    _CORESNAPSHOTCONNECTION._serialized_start = 31470
-    _CORESNAPSHOTCONNECTION._serialized_end = 31607
-    _CORESNAPSHOTEDGE._serialized_start = 31609
-    _CORESNAPSHOTEDGE._serialized_end = 31705
-    _HISTORYSEGMENT._serialized_start = 31708
-    _HISTORYSEGMENT._serialized_end = 31965
-    _GETMOSTRECENTNETWORKHISTORYSEGMENTREQUEST._serialized_start = 31967
-    _GETMOSTRECENTNETWORKHISTORYSEGMENTREQUEST._serialized_end = 32010
-    _GETMOSTRECENTNETWORKHISTORYSEGMENTRESPONSE._serialized_start = 32013
-    _GETMOSTRECENTNETWORKHISTORYSEGMENTRESPONSE._serialized_end = 32154
-    _LISTALLNETWORKHISTORYSEGMENTSREQUEST._serialized_start = 32156
-    _LISTALLNETWORKHISTORYSEGMENTSREQUEST._serialized_end = 32194
-    _LISTALLNETWORKHISTORYSEGMENTSRESPONSE._serialized_start = 32196
-    _LISTALLNETWORKHISTORYSEGMENTSRESPONSE._serialized_end = 32296
-    _GETACTIVENETWORKHISTORYPEERADDRESSESREQUEST._serialized_start = 32298
-    _GETACTIVENETWORKHISTORYPEERADDRESSESREQUEST._serialized_end = 32343
-    _GETACTIVENETWORKHISTORYPEERADDRESSESRESPONSE._serialized_start = 32345
-    _GETACTIVENETWORKHISTORYPEERADDRESSESRESPONSE._serialized_end = 32426
-    _GETNETWORKHISTORYSTATUSREQUEST._serialized_start = 32428
-    _GETNETWORKHISTORYSTATUSREQUEST._serialized_end = 32460
-    _GETNETWORKHISTORYSTATUSRESPONSE._serialized_start = 32463
-    _GETNETWORKHISTORYSTATUSRESPONSE._serialized_end = 32639
-    _GETNETWORKHISTORYBOOTSTRAPPEERSREQUEST._serialized_start = 32641
-    _GETNETWORKHISTORYBOOTSTRAPPEERSREQUEST._serialized_end = 32681
-    _GETNETWORKHISTORYBOOTSTRAPPEERSRESPONSE._serialized_start = 32683
-    _GETNETWORKHISTORYBOOTSTRAPPEERSRESPONSE._serialized_end = 32765
-    _EXPORTNETWORKHISTORYREQUEST._serialized_start = 32768
-    _EXPORTNETWORKHISTORYREQUEST._serialized_end = 32901
-    _LISTENTITIESREQUEST._serialized_start = 32903
-    _LISTENTITIESREQUEST._serialized_end = 32972
-    _LISTENTITIESRESPONSE._serialized_start = 32975
-    _LISTENTITIESRESPONSE._serialized_end = 34684
-    _PINGREQUEST._serialized_start = 34686
-    _PINGREQUEST._serialized_end = 34699
-    _PINGRESPONSE._serialized_start = 34701
-    _PINGRESPONSE._serialized_end = 34715
-    _ORDERINFO._serialized_start = 34718
-    _ORDERINFO._serialized_end = 34853
-    _ESTIMATEPOSITIONREQUEST._serialized_start = 34856
-    _ESTIMATEPOSITIONREQUEST._serialized_end = 35086
-    _ESTIMATEPOSITIONRESPONSE._serialized_start = 35089
-    _ESTIMATEPOSITIONRESPONSE._serialized_end = 35244
-    _MARGINESTIMATE._serialized_start = 35246
-    _MARGINESTIMATE._serialized_end = 35362
-    _LIQUIDATIONESTIMATE._serialized_start = 35365
-    _LIQUIDATIONESTIMATE._serialized_end = 35516
-    _LIQUIDATIONPRICE._serialized_start = 35519
-    _LIQUIDATIONPRICE._serialized_end = 35681
-    _TRADINGDATASERVICE._serialized_start = 36565
-    _TRADINGDATASERVICE._serialized_end = 47465
+    _globals["_LEDGERENTRYFIELD"]._serialized_start = 36394
+    _globals["_LEDGERENTRYFIELD"]._serialized_end = 36564
+    _globals["_ACCOUNTFIELD"]._serialized_start = 36567
+    _globals["_ACCOUNTFIELD"]._serialized_end = 36743
+    _globals["_TRANSFERDIRECTION"]._serialized_start = 36746
+    _globals["_TRANSFERDIRECTION"]._serialized_end = 36919
+    _globals["_TABLE"]._serialized_start = 36922
+    _globals["_TABLE"]._serialized_end = 37272
+    _globals["_PAGINATION"]._serialized_start = 335
+    _globals["_PAGINATION"]._serialized_end = 552
+    _globals["_PAGEINFO"]._serialized_start = 555
+    _globals["_PAGEINFO"]._serialized_end = 711
+    _globals["_ACCOUNTBALANCE"]._serialized_start = 714
+    _globals["_ACCOUNTBALANCE"]._serialized_end = 868
+    _globals["_LISTACCOUNTSREQUEST"]._serialized_start = 871
+    _globals["_LISTACCOUNTSREQUEST"]._serialized_end = 1029
+    _globals["_LISTACCOUNTSRESPONSE"]._serialized_start = 1031
+    _globals["_LISTACCOUNTSRESPONSE"]._serialized_end = 1118
+    _globals["_ACCOUNTSCONNECTION"]._serialized_start = 1121
+    _globals["_ACCOUNTSCONNECTION"]._serialized_end = 1249
+    _globals["_ACCOUNTEDGE"]._serialized_start = 1251
+    _globals["_ACCOUNTEDGE"]._serialized_end = 1341
+    _globals["_OBSERVEACCOUNTSREQUEST"]._serialized_start = 1344
+    _globals["_OBSERVEACCOUNTSREQUEST"]._serialized_end = 1485
+    _globals["_OBSERVEACCOUNTSRESPONSE"]._serialized_start = 1488
+    _globals["_OBSERVEACCOUNTSRESPONSE"]._serialized_end = 1654
+    _globals["_ACCOUNTSNAPSHOTPAGE"]._serialized_start = 1656
+    _globals["_ACCOUNTSNAPSHOTPAGE"]._serialized_end = 1767
+    _globals["_ACCOUNTUPDATES"]._serialized_start = 1769
+    _globals["_ACCOUNTUPDATES"]._serialized_end = 1846
+    _globals["_INFOREQUEST"]._serialized_start = 1848
+    _globals["_INFOREQUEST"]._serialized_end = 1861
+    _globals["_INFORESPONSE"]._serialized_start = 1863
+    _globals["_INFORESPONSE"]._serialized_end = 1936
+    _globals["_GETORDERREQUEST"]._serialized_start = 1938
+    _globals["_GETORDERREQUEST"]._serialized_end = 2031
+    _globals["_GETORDERRESPONSE"]._serialized_start = 2033
+    _globals["_GETORDERRESPONSE"]._serialized_end = 2086
+    _globals["_ORDERFILTER"]._serialized_start = 2089
+    _globals["_ORDERFILTER"]._serialized_end = 2534
+    _globals["_LISTORDERSREQUEST"]._serialized_start = 2537
+    _globals["_LISTORDERSREQUEST"]._serialized_end = 2707
+    _globals["_LISTORDERSRESPONSE"]._serialized_start = 2709
+    _globals["_LISTORDERSRESPONSE"]._serialized_end = 2787
+    _globals["_LISTORDERVERSIONSREQUEST"]._serialized_start = 2790
+    _globals["_LISTORDERVERSIONSREQUEST"]._serialized_end = 2930
+    _globals["_LISTORDERVERSIONSRESPONSE"]._serialized_start = 2932
+    _globals["_LISTORDERVERSIONSRESPONSE"]._serialized_end = 3017
+    _globals["_OBSERVEORDERSREQUEST"]._serialized_start = 3020
+    _globals["_OBSERVEORDERSREQUEST"]._serialized_end = 3174
+    _globals["_OBSERVEORDERSRESPONSE"]._serialized_start = 3177
+    _globals["_OBSERVEORDERSRESPONSE"]._serialized_end = 3337
+    _globals["_ORDERSNAPSHOTPAGE"]._serialized_start = 3339
+    _globals["_ORDERSNAPSHOTPAGE"]._serialized_end = 3424
+    _globals["_ORDERUPDATES"]._serialized_start = 3426
+    _globals["_ORDERUPDATES"]._serialized_end = 3477
+    _globals["_LISTPOSITIONSREQUEST"]._serialized_start = 3480
+    _globals["_LISTPOSITIONSREQUEST"]._serialized_end = 3643
+    _globals["_LISTPOSITIONSRESPONSE"]._serialized_start = 3645
+    _globals["_LISTPOSITIONSRESPONSE"]._serialized_end = 3739
+    _globals["_POSITIONSFILTER"]._serialized_start = 3741
+    _globals["_POSITIONSFILTER"]._serialized_end = 3818
+    _globals["_LISTALLPOSITIONSREQUEST"]._serialized_start = 3821
+    _globals["_LISTALLPOSITIONSREQUEST"]._serialized_end = 3985
+    _globals["_LISTALLPOSITIONSRESPONSE"]._serialized_start = 3987
+    _globals["_LISTALLPOSITIONSRESPONSE"]._serialized_end = 4080
+    _globals["_POSITIONEDGE"]._serialized_start = 4082
+    _globals["_POSITIONEDGE"]._serialized_end = 4156
+    _globals["_POSITIONCONNECTION"]._serialized_start = 4159
+    _globals["_POSITIONCONNECTION"]._serialized_end = 4288
+    _globals["_OBSERVEPOSITIONSREQUEST"]._serialized_start = 4290
+    _globals["_OBSERVEPOSITIONSREQUEST"]._serialized_end = 4408
+    _globals["_OBSERVEPOSITIONSRESPONSE"]._serialized_start = 4411
+    _globals["_OBSERVEPOSITIONSRESPONSE"]._serialized_end = 4580
+    _globals["_POSITIONSNAPSHOTPAGE"]._serialized_start = 4582
+    _globals["_POSITIONSNAPSHOTPAGE"]._serialized_end = 4679
+    _globals["_POSITIONUPDATES"]._serialized_start = 4681
+    _globals["_POSITIONUPDATES"]._serialized_end = 4744
+    _globals["_LEDGERENTRYFILTER"]._serialized_start = 4747
+    _globals["_LEDGERENTRYFILTER"]._serialized_end = 5038
+    _globals["_AGGREGATEDLEDGERENTRY"]._serialized_start = 5041
+    _globals["_AGGREGATEDLEDGERENTRY"]._serialized_end = 5770
+    _globals["_LISTLEDGERENTRIESREQUEST"]._serialized_start = 5773
+    _globals["_LISTLEDGERENTRIESREQUEST"]._serialized_end = 6019
+    _globals["_EXPORTLEDGERENTRIESREQUEST"]._serialized_start = 6022
+    _globals["_EXPORTLEDGERENTRIESREQUEST"]._serialized_end = 6195
+    _globals["_LISTLEDGERENTRIESRESPONSE"]._serialized_start = 6197
+    _globals["_LISTLEDGERENTRIESRESPONSE"]._serialized_end = 6315
+    _globals["_AGGREGATEDLEDGERENTRIESEDGE"]._serialized_start = 6317
+    _globals["_AGGREGATEDLEDGERENTRIESEDGE"]._serialized_end = 6430
+    _globals["_AGGREGATEDLEDGERENTRIESCONNECTION"]._serialized_start = 6433
+    _globals["_AGGREGATEDLEDGERENTRIESCONNECTION"]._serialized_end = 6592
+    _globals["_LISTBALANCECHANGESREQUEST"]._serialized_start = 6595
+    _globals["_LISTBALANCECHANGESREQUEST"]._serialized_end = 6838
+    _globals["_LISTBALANCECHANGESRESPONSE"]._serialized_start = 6840
+    _globals["_LISTBALANCECHANGESRESPONSE"]._serialized_end = 6942
+    _globals["_GETBALANCEHISTORYREQUEST"]._serialized_start = 6945
+    _globals["_GETBALANCEHISTORYREQUEST"]._serialized_end = 7245
+    _globals["_GETBALANCEHISTORYRESPONSE"]._serialized_start = 7247
+    _globals["_GETBALANCEHISTORYRESPONSE"]._serialized_end = 7348
+    _globals["_AGGREGATEDBALANCEEDGE"]._serialized_start = 7350
+    _globals["_AGGREGATEDBALANCEEDGE"]._serialized_end = 7453
+    _globals["_AGGREGATEDBALANCECONNECTION"]._serialized_start = 7456
+    _globals["_AGGREGATEDBALANCECONNECTION"]._serialized_end = 7603
+    _globals["_ACCOUNTFILTER"]._serialized_start = 7606
+    _globals["_ACCOUNTFILTER"]._serialized_end = 7764
+    _globals["_AGGREGATEDBALANCE"]._serialized_start = 7767
+    _globals["_AGGREGATEDBALANCE"]._serialized_end = 8056
+    _globals["_OBSERVEMARKETSDEPTHREQUEST"]._serialized_start = 8058
+    _globals["_OBSERVEMARKETSDEPTHREQUEST"]._serialized_end = 8117
+    _globals["_OBSERVEMARKETSDEPTHRESPONSE"]._serialized_start = 8119
+    _globals["_OBSERVEMARKETSDEPTHRESPONSE"]._serialized_end = 8202
+    _globals["_OBSERVEMARKETSDEPTHUPDATESREQUEST"]._serialized_start = 8204
+    _globals["_OBSERVEMARKETSDEPTHUPDATESREQUEST"]._serialized_end = 8270
+    _globals["_OBSERVEMARKETSDEPTHUPDATESRESPONSE"]._serialized_start = 8272
+    _globals["_OBSERVEMARKETSDEPTHUPDATESRESPONSE"]._serialized_end = 8357
+    _globals["_OBSERVEMARKETSDATAREQUEST"]._serialized_start = 8359
+    _globals["_OBSERVEMARKETSDATAREQUEST"]._serialized_end = 8417
+    _globals["_OBSERVEMARKETSDATARESPONSE"]._serialized_start = 8419
+    _globals["_OBSERVEMARKETSDATARESPONSE"]._serialized_end = 8498
+    _globals["_GETLATESTMARKETDEPTHREQUEST"]._serialized_start = 8500
+    _globals["_GETLATESTMARKETDEPTHREQUEST"]._serialized_end = 8612
+    _globals["_GETLATESTMARKETDEPTHRESPONSE"]._serialized_start = 8615
+    _globals["_GETLATESTMARKETDEPTHRESPONSE"]._serialized_end = 8833
+    _globals["_LISTLATESTMARKETDATAREQUEST"]._serialized_start = 8835
+    _globals["_LISTLATESTMARKETDATAREQUEST"]._serialized_end = 8864
+    _globals["_LISTLATESTMARKETDATARESPONSE"]._serialized_start = 8866
+    _globals["_LISTLATESTMARKETDATARESPONSE"]._serialized_end = 8949
+    _globals["_GETLATESTMARKETDATAREQUEST"]._serialized_start = 8951
+    _globals["_GETLATESTMARKETDATAREQUEST"]._serialized_end = 9014
+    _globals["_GETLATESTMARKETDATARESPONSE"]._serialized_start = 9016
+    _globals["_GETLATESTMARKETDATARESPONSE"]._serialized_end = 9096
+    _globals["_GETMARKETDATAHISTORYBYIDREQUEST"]._serialized_start = 9099
+    _globals["_GETMARKETDATAHISTORYBYIDREQUEST"]._serialized_end = 9380
+    _globals["_GETMARKETDATAHISTORYBYIDRESPONSE"]._serialized_start = 9382
+    _globals["_GETMARKETDATAHISTORYBYIDRESPONSE"]._serialized_end = 9488
+    _globals["_MARKETDATAEDGE"]._serialized_start = 9490
+    _globals["_MARKETDATAEDGE"]._serialized_end = 9568
+    _globals["_MARKETDATACONNECTION"]._serialized_start = 9571
+    _globals["_MARKETDATACONNECTION"]._serialized_end = 9704
+    _globals["_LISTTRANSFERSREQUEST"]._serialized_start = 9707
+    _globals["_LISTTRANSFERSREQUEST"]._serialized_end = 9916
+    _globals["_LISTTRANSFERSRESPONSE"]._serialized_start = 9918
+    _globals["_LISTTRANSFERSRESPONSE"]._serialized_end = 10008
+    _globals["_TRANSFEREDGE"]._serialized_start = 10010
+    _globals["_TRANSFEREDGE"]._serialized_end = 10094
+    _globals["_TRANSFERCONNECTION"]._serialized_start = 10097
+    _globals["_TRANSFERCONNECTION"]._serialized_end = 10226
+    _globals["_GETNETWORKLIMITSREQUEST"]._serialized_start = 10228
+    _globals["_GETNETWORKLIMITSREQUEST"]._serialized_end = 10253
+    _globals["_GETNETWORKLIMITSRESPONSE"]._serialized_start = 10255
+    _globals["_GETNETWORKLIMITSRESPONSE"]._serialized_end = 10326
+    _globals["_LISTCANDLEINTERVALSREQUEST"]._serialized_start = 10328
+    _globals["_LISTCANDLEINTERVALSREQUEST"]._serialized_end = 10391
+    _globals["_INTERVALTOCANDLEID"]._serialized_start = 10393
+    _globals["_INTERVALTOCANDLEID"]._serialized_end = 10470
+    _globals["_LISTCANDLEINTERVALSRESPONSE"]._serialized_start = 10472
+    _globals["_LISTCANDLEINTERVALSRESPONSE"]._serialized_end = 10589
+    _globals["_CANDLE"]._serialized_start = 10592
+    _globals["_CANDLE"]._serialized_end = 10759
+    _globals["_OBSERVECANDLEDATAREQUEST"]._serialized_start = 10761
+    _globals["_OBSERVECANDLEDATAREQUEST"]._serialized_end = 10822
+    _globals["_OBSERVECANDLEDATARESPONSE"]._serialized_start = 10824
+    _globals["_OBSERVECANDLEDATARESPONSE"]._serialized_end = 10900
+    _globals["_LISTCANDLEDATAREQUEST"]._serialized_start = 10903
+    _globals["_LISTCANDLEDATAREQUEST"]._serialized_end = 11122
+    _globals["_LISTCANDLEDATARESPONSE"]._serialized_start = 11124
+    _globals["_LISTCANDLEDATARESPONSE"]._serialized_end = 11213
+    _globals["_CANDLEEDGE"]._serialized_start = 11215
+    _globals["_CANDLEEDGE"]._serialized_end = 11296
+    _globals["_CANDLEDATACONNECTION"]._serialized_start = 11299
+    _globals["_CANDLEDATACONNECTION"]._serialized_end = 11428
+    _globals["_LISTVOTESREQUEST"]._serialized_start = 11431
+    _globals["_LISTVOTESREQUEST"]._serialized_end = 11629
+    _globals["_LISTVOTESRESPONSE"]._serialized_start = 11631
+    _globals["_LISTVOTESRESPONSE"]._serialized_end = 11705
+    _globals["_VOTEEDGE"]._serialized_start = 11707
+    _globals["_VOTEEDGE"]._serialized_end = 11773
+    _globals["_VOTECONNECTION"]._serialized_start = 11775
+    _globals["_VOTECONNECTION"]._serialized_end = 11896
+    _globals["_OBSERVEVOTESREQUEST"]._serialized_start = 11898
+    _globals["_OBSERVEVOTESREQUEST"]._serialized_end = 12018
+    _globals["_OBSERVEVOTESRESPONSE"]._serialized_start = 12020
+    _globals["_OBSERVEVOTESRESPONSE"]._serialized_end = 12074
+    _globals["_LISTERC20MULTISIGSIGNERADDEDBUNDLESREQUEST"]._serialized_start = 12077
+    _globals["_LISTERC20MULTISIGSIGNERADDEDBUNDLESREQUEST"]._serialized_end = 12266
+    _globals["_LISTERC20MULTISIGSIGNERADDEDBUNDLESRESPONSE"]._serialized_start = 12268
+    _globals["_LISTERC20MULTISIGSIGNERADDEDBUNDLESRESPONSE"]._serialized_end = 12392
+    _globals["_ERC20MULTISIGSIGNERADDEDEDGE"]._serialized_start = 12394
+    _globals["_ERC20MULTISIGSIGNERADDEDEDGE"]._serialized_end = 12510
+    _globals["_ERC20MULTISIGSIGNERADDEDBUNDLEEDGE"]._serialized_start = 12513
+    _globals["_ERC20MULTISIGSIGNERADDEDBUNDLEEDGE"]._serialized_end = 12642
+    _globals["_ERC20MULTISIGSIGNERADDEDCONNECTION"]._serialized_start = 12645
+    _globals["_ERC20MULTISIGSIGNERADDEDCONNECTION"]._serialized_end = 12812
+    _globals["_ERC20MULTISIGSIGNERADDEDBUNDLE"]._serialized_start = 12815
+    _globals["_ERC20MULTISIGSIGNERADDEDBUNDLE"]._serialized_end = 13021
+    _globals["_LISTERC20MULTISIGSIGNERREMOVEDBUNDLESREQUEST"]._serialized_start = 13024
+    _globals["_LISTERC20MULTISIGSIGNERREMOVEDBUNDLESREQUEST"]._serialized_end = 13215
+    _globals["_LISTERC20MULTISIGSIGNERREMOVEDBUNDLESRESPONSE"]._serialized_start = 13218
+    _globals["_LISTERC20MULTISIGSIGNERREMOVEDBUNDLESRESPONSE"]._serialized_end = 13346
+    _globals["_ERC20MULTISIGSIGNERREMOVEDEDGE"]._serialized_start = 13348
+    _globals["_ERC20MULTISIGSIGNERREMOVEDEDGE"]._serialized_end = 13468
+    _globals["_ERC20MULTISIGSIGNERREMOVEDBUNDLEEDGE"]._serialized_start = 13471
+    _globals["_ERC20MULTISIGSIGNERREMOVEDBUNDLEEDGE"]._serialized_end = 13604
+    _globals["_ERC20MULTISIGSIGNERREMOVEDCONNECTION"]._serialized_start = 13607
+    _globals["_ERC20MULTISIGSIGNERREMOVEDCONNECTION"]._serialized_end = 13778
+    _globals["_ERC20MULTISIGSIGNERREMOVEDBUNDLE"]._serialized_start = 13781
+    _globals["_ERC20MULTISIGSIGNERREMOVEDBUNDLE"]._serialized_end = 13989
+    _globals["_GETERC20LISTASSETBUNDLEREQUEST"]._serialized_start = 13991
+    _globals["_GETERC20LISTASSETBUNDLEREQUEST"]._serialized_end = 14056
+    _globals["_GETERC20LISTASSETBUNDLERESPONSE"]._serialized_start = 14059
+    _globals["_GETERC20LISTASSETBUNDLERESPONSE"]._serialized_end = 14217
+    _globals["_GETERC20SETASSETLIMITSBUNDLEREQUEST"]._serialized_start = 14219
+    _globals["_GETERC20SETASSETLIMITSBUNDLEREQUEST"]._serialized_end = 14295
+    _globals["_GETERC20SETASSETLIMITSBUNDLERESPONSE"]._serialized_start = 14298
+    _globals["_GETERC20SETASSETLIMITSBUNDLERESPONSE"]._serialized_end = 14530
+    _globals["_GETERC20WITHDRAWALAPPROVALREQUEST"]._serialized_start = 14532
+    _globals["_GETERC20WITHDRAWALAPPROVALREQUEST"]._serialized_end = 14610
+    _globals["_GETERC20WITHDRAWALAPPROVALRESPONSE"]._serialized_start = 14613
+    _globals["_GETERC20WITHDRAWALAPPROVALRESPONSE"]._serialized_end = 14835
+    _globals["_GETLASTTRADEREQUEST"]._serialized_start = 14837
+    _globals["_GETLASTTRADEREQUEST"]._serialized_end = 14893
+    _globals["_GETLASTTRADERESPONSE"]._serialized_start = 14895
+    _globals["_GETLASTTRADERESPONSE"]._serialized_end = 14952
+    _globals["_LISTTRADESREQUEST"]._serialized_start = 14955
+    _globals["_LISTTRADESREQUEST"]._serialized_end = 15223
+    _globals["_LISTTRADESRESPONSE"]._serialized_start = 15225
+    _globals["_LISTTRADESRESPONSE"]._serialized_end = 15303
+    _globals["_TRADECONNECTION"]._serialized_start = 15305
+    _globals["_TRADECONNECTION"]._serialized_end = 15428
+    _globals["_TRADEEDGE"]._serialized_start = 15430
+    _globals["_TRADEEDGE"]._serialized_end = 15498
+    _globals["_OBSERVETRADESREQUEST"]._serialized_start = 15500
+    _globals["_OBSERVETRADESREQUEST"]._serialized_end = 15582
+    _globals["_OBSERVETRADESRESPONSE"]._serialized_start = 15584
+    _globals["_OBSERVETRADESRESPONSE"]._serialized_end = 15644
+    _globals["_GETORACLESPECREQUEST"]._serialized_start = 15646
+    _globals["_GETORACLESPECREQUEST"]._serialized_end = 15712
+    _globals["_GETORACLESPECRESPONSE"]._serialized_start = 15714
+    _globals["_GETORACLESPECRESPONSE"]._serialized_end = 15788
+    _globals["_LISTORACLESPECSREQUEST"]._serialized_start = 15790
+    _globals["_LISTORACLESPECSREQUEST"]._serialized_end = 15895
+    _globals["_LISTORACLESPECSRESPONSE"]._serialized_start = 15897
+    _globals["_LISTORACLESPECSRESPONSE"]._serialized_end = 15997
+    _globals["_LISTORACLEDATAREQUEST"]._serialized_start = 16000
+    _globals["_LISTORACLEDATAREQUEST"]._serialized_end = 16166
+    _globals["_LISTORACLEDATARESPONSE"]._serialized_start = 16168
+    _globals["_LISTORACLEDATARESPONSE"]._serialized_end = 16264
+    _globals["_ORACLESPECEDGE"]._serialized_start = 16266
+    _globals["_ORACLESPECEDGE"]._serialized_end = 16344
+    _globals["_ORACLESPECSCONNECTION"]._serialized_start = 16347
+    _globals["_ORACLESPECSCONNECTION"]._serialized_end = 16481
+    _globals["_ORACLEDATAEDGE"]._serialized_start = 16483
+    _globals["_ORACLEDATAEDGE"]._serialized_end = 16561
+    _globals["_ORACLEDATACONNECTION"]._serialized_start = 16564
+    _globals["_ORACLEDATACONNECTION"]._serialized_end = 16697
+    _globals["_GETMARKETREQUEST"]._serialized_start = 16699
+    _globals["_GETMARKETREQUEST"]._serialized_end = 16752
+    _globals["_GETMARKETRESPONSE"]._serialized_start = 16754
+    _globals["_GETMARKETRESPONSE"]._serialized_end = 16811
+    _globals["_LISTMARKETSREQUEST"]._serialized_start = 16814
+    _globals["_LISTMARKETSREQUEST"]._serialized_end = 16981
+    _globals["_LISTMARKETSRESPONSE"]._serialized_start = 16983
+    _globals["_LISTMARKETSRESPONSE"]._serialized_end = 17065
+    _globals["_MARKETEDGE"]._serialized_start = 17067
+    _globals["_MARKETEDGE"]._serialized_end = 17137
+    _globals["_MARKETCONNECTION"]._serialized_start = 17139
+    _globals["_MARKETCONNECTION"]._serialized_end = 17264
+    _globals["_LISTSUCCESSORMARKETSREQUEST"]._serialized_start = 17267
+    _globals["_LISTSUCCESSORMARKETSREQUEST"]._serialized_end = 17442
+    _globals["_SUCCESSORMARKET"]._serialized_start = 17444
+    _globals["_SUCCESSORMARKET"]._serialized_end = 17551
+    _globals["_SUCCESSORMARKETEDGE"]._serialized_start = 17553
+    _globals["_SUCCESSORMARKETEDGE"]._serialized_end = 17652
+    _globals["_SUCCESSORMARKETCONNECTION"]._serialized_start = 17655
+    _globals["_SUCCESSORMARKETCONNECTION"]._serialized_end = 17798
+    _globals["_LISTSUCCESSORMARKETSRESPONSE"]._serialized_start = 17800
+    _globals["_LISTSUCCESSORMARKETSRESPONSE"]._serialized_end = 17900
+    _globals["_GETPARTYREQUEST"]._serialized_start = 17902
+    _globals["_GETPARTYREQUEST"]._serialized_end = 17952
+    _globals["_GETPARTYRESPONSE"]._serialized_start = 17954
+    _globals["_GETPARTYRESPONSE"]._serialized_end = 18007
+    _globals["_LISTPARTIESREQUEST"]._serialized_start = 18009
+    _globals["_LISTPARTIESREQUEST"]._serialized_end = 18117
+    _globals["_LISTPARTIESRESPONSE"]._serialized_start = 18119
+    _globals["_LISTPARTIESRESPONSE"]._serialized_end = 18200
+    _globals["_PARTYEDGE"]._serialized_start = 18202
+    _globals["_PARTYEDGE"]._serialized_end = 18270
+    _globals["_PARTYCONNECTION"]._serialized_start = 18272
+    _globals["_PARTYCONNECTION"]._serialized_end = 18395
+    _globals["_ORDEREDGE"]._serialized_start = 18397
+    _globals["_ORDEREDGE"]._serialized_end = 18465
+    _globals["_LISTMARGINLEVELSREQUEST"]._serialized_start = 18468
+    _globals["_LISTMARGINLEVELSREQUEST"]._serialized_end = 18610
+    _globals["_LISTMARGINLEVELSRESPONSE"]._serialized_start = 18612
+    _globals["_LISTMARGINLEVELSRESPONSE"]._serialized_end = 18710
+    _globals["_OBSERVEMARGINLEVELSREQUEST"]._serialized_start = 18712
+    _globals["_OBSERVEMARGINLEVELSREQUEST"]._serialized_end = 18815
+    _globals["_OBSERVEMARGINLEVELSRESPONSE"]._serialized_start = 18817
+    _globals["_OBSERVEMARGINLEVELSRESPONSE"]._serialized_end = 18903
+    _globals["_ORDERCONNECTION"]._serialized_start = 18905
+    _globals["_ORDERCONNECTION"]._serialized_end = 19028
+    _globals["_MARGINEDGE"]._serialized_start = 19030
+    _globals["_MARGINEDGE"]._serialized_end = 19106
+    _globals["_MARGINCONNECTION"]._serialized_start = 19108
+    _globals["_MARGINCONNECTION"]._serialized_end = 19233
+    _globals["_LISTREWARDSREQUEST"]._serialized_start = 19236
+    _globals["_LISTREWARDSREQUEST"]._serialized_end = 19505
+    _globals["_LISTREWARDSRESPONSE"]._serialized_start = 19507
+    _globals["_LISTREWARDSRESPONSE"]._serialized_end = 19590
+    _globals["_REWARDEDGE"]._serialized_start = 19592
+    _globals["_REWARDEDGE"]._serialized_end = 19662
+    _globals["_REWARDSCONNECTION"]._serialized_start = 19664
+    _globals["_REWARDSCONNECTION"]._serialized_end = 19790
+    _globals["_LISTREWARDSUMMARIESREQUEST"]._serialized_start = 19793
+    _globals["_LISTREWARDSUMMARIESREQUEST"]._serialized_end = 19992
+    _globals["_LISTREWARDSUMMARIESRESPONSE"]._serialized_start = 19994
+    _globals["_LISTREWARDSUMMARIESRESPONSE"]._serialized_end = 20074
+    _globals["_REWARDSUMMARYFILTER"]._serialized_start = 20077
+    _globals["_REWARDSUMMARYFILTER"]._serialized_end = 20254
+    _globals["_LISTEPOCHREWARDSUMMARIESREQUEST"]._serialized_start = 20257
+    _globals["_LISTEPOCHREWARDSUMMARIESREQUEST"]._serialized_end = 20433
+    _globals["_LISTEPOCHREWARDSUMMARIESRESPONSE"]._serialized_start = 20435
+    _globals["_LISTEPOCHREWARDSUMMARIESRESPONSE"]._serialized_end = 20546
+    _globals["_EPOCHREWARDSUMMARYCONNECTION"]._serialized_start = 20549
+    _globals["_EPOCHREWARDSUMMARYCONNECTION"]._serialized_end = 20698
+    _globals["_EPOCHREWARDSUMMARYEDGE"]._serialized_start = 20700
+    _globals["_EPOCHREWARDSUMMARYEDGE"]._serialized_end = 20794
+    _globals["_OBSERVEREWARDSREQUEST"]._serialized_start = 20796
+    _globals["_OBSERVEREWARDSREQUEST"]._serialized_end = 20909
+    _globals["_OBSERVEREWARDSRESPONSE"]._serialized_start = 20911
+    _globals["_OBSERVEREWARDSRESPONSE"]._serialized_end = 20973
+    _globals["_GETDEPOSITREQUEST"]._serialized_start = 20975
+    _globals["_GETDEPOSITREQUEST"]._serialized_end = 21016
+    _globals["_GETDEPOSITRESPONSE"]._serialized_start = 21018
+    _globals["_GETDEPOSITRESPONSE"]._serialized_end = 21079
+    _globals["_LISTDEPOSITSREQUEST"]._serialized_start = 21082
+    _globals["_LISTDEPOSITSREQUEST"]._serialized_end = 21290
+    _globals["_LISTDEPOSITSRESPONSE"]._serialized_start = 21292
+    _globals["_LISTDEPOSITSRESPONSE"]._serialized_end = 21379
+    _globals["_DEPOSITEDGE"]._serialized_start = 21381
+    _globals["_DEPOSITEDGE"]._serialized_end = 21453
+    _globals["_DEPOSITSCONNECTION"]._serialized_start = 21456
+    _globals["_DEPOSITSCONNECTION"]._serialized_end = 21584
+    _globals["_GETWITHDRAWALREQUEST"]._serialized_start = 21586
+    _globals["_GETWITHDRAWALREQUEST"]._serialized_end = 21630
+    _globals["_GETWITHDRAWALRESPONSE"]._serialized_start = 21632
+    _globals["_GETWITHDRAWALRESPONSE"]._serialized_end = 21705
+    _globals["_LISTWITHDRAWALSREQUEST"]._serialized_start = 21708
+    _globals["_LISTWITHDRAWALSREQUEST"]._serialized_end = 21919
+    _globals["_LISTWITHDRAWALSRESPONSE"]._serialized_start = 21921
+    _globals["_LISTWITHDRAWALSRESPONSE"]._serialized_end = 22020
+    _globals["_WITHDRAWALEDGE"]._serialized_start = 22022
+    _globals["_WITHDRAWALEDGE"]._serialized_end = 22100
+    _globals["_WITHDRAWALSCONNECTION"]._serialized_start = 22103
+    _globals["_WITHDRAWALSCONNECTION"]._serialized_end = 22237
+    _globals["_GETASSETREQUEST"]._serialized_start = 22239
+    _globals["_GETASSETREQUEST"]._serialized_end = 22289
+    _globals["_GETASSETRESPONSE"]._serialized_start = 22291
+    _globals["_GETASSETRESPONSE"]._serialized_end = 22344
+    _globals["_LISTASSETSREQUEST"]._serialized_start = 22347
+    _globals["_LISTASSETSREQUEST"]._serialized_end = 22492
+    _globals["_LISTASSETSRESPONSE"]._serialized_start = 22494
+    _globals["_LISTASSETSRESPONSE"]._serialized_end = 22573
+    _globals["_ASSETEDGE"]._serialized_start = 22575
+    _globals["_ASSETEDGE"]._serialized_end = 22643
+    _globals["_ASSETSCONNECTION"]._serialized_start = 22645
+    _globals["_ASSETSCONNECTION"]._serialized_end = 22769
+    _globals["_LISTLIQUIDITYPROVISIONSREQUEST"]._serialized_start = 22772
+    _globals["_LISTLIQUIDITYPROVISIONSREQUEST"]._serialized_end = 23061
+    _globals["_LISTLIQUIDITYPROVISIONSRESPONSE"]._serialized_start = 23064
+    _globals["_LISTLIQUIDITYPROVISIONSRESPONSE"]._serialized_end = 23196
+    _globals["_LIQUIDITYPROVISIONSEDGE"]._serialized_start = 23198
+    _globals["_LIQUIDITYPROVISIONSEDGE"]._serialized_end = 23293
+    _globals["_LIQUIDITYPROVISIONSCONNECTION"]._serialized_start = 23296
+    _globals["_LIQUIDITYPROVISIONSCONNECTION"]._serialized_end = 23447
+    _globals["_OBSERVELIQUIDITYPROVISIONSREQUEST"]._serialized_start = 23450
+    _globals["_OBSERVELIQUIDITYPROVISIONSREQUEST"]._serialized_end = 23578
+    _globals["_OBSERVELIQUIDITYPROVISIONSRESPONSE"]._serialized_start = 23580
+    _globals["_OBSERVELIQUIDITYPROVISIONSRESPONSE"]._serialized_end = 23693
+    _globals["_GETGOVERNANCEDATAREQUEST"]._serialized_start = 23696
+    _globals["_GETGOVERNANCEDATAREQUEST"]._serialized_end = 23825
+    _globals["_GETGOVERNANCEDATARESPONSE"]._serialized_start = 23827
+    _globals["_GETGOVERNANCEDATARESPONSE"]._serialized_end = 23896
+    _globals["_LISTGOVERNANCEDATAREQUEST"]._serialized_start = 23899
+    _globals["_LISTGOVERNANCEDATAREQUEST"]._serialized_end = 24533
+    _globals["_LISTGOVERNANCEDATAREQUEST_TYPE"]._serialized_start = 24253
+    _globals["_LISTGOVERNANCEDATAREQUEST_TYPE"]._serialized_end = 24436
+    _globals["_LISTGOVERNANCEDATARESPONSE"]._serialized_start = 24535
+    _globals["_LISTGOVERNANCEDATARESPONSE"]._serialized_end = 24638
+    _globals["_GOVERNANCEDATAEDGE"]._serialized_start = 24640
+    _globals["_GOVERNANCEDATAEDGE"]._serialized_end = 24726
+    _globals["_GOVERNANCEDATACONNECTION"]._serialized_start = 24729
+    _globals["_GOVERNANCEDATACONNECTION"]._serialized_end = 24870
+    _globals["_OBSERVEGOVERNANCEREQUEST"]._serialized_start = 24872
+    _globals["_OBSERVEGOVERNANCEREQUEST"]._serialized_end = 24943
+    _globals["_OBSERVEGOVERNANCERESPONSE"]._serialized_start = 24945
+    _globals["_OBSERVEGOVERNANCERESPONSE"]._serialized_end = 25014
+    _globals["_LISTDELEGATIONSREQUEST"]._serialized_start = 25017
+    _globals["_LISTDELEGATIONSREQUEST"]._serialized_end = 25254
+    _globals["_LISTDELEGATIONSRESPONSE"]._serialized_start = 25256
+    _globals["_LISTDELEGATIONSRESPONSE"]._serialized_end = 25355
+    _globals["_DELEGATIONEDGE"]._serialized_start = 25357
+    _globals["_DELEGATIONEDGE"]._serialized_end = 25435
+    _globals["_DELEGATIONSCONNECTION"]._serialized_start = 25438
+    _globals["_DELEGATIONSCONNECTION"]._serialized_end = 25572
+    _globals["_OBSERVEDELEGATIONSREQUEST"]._serialized_start = 25574
+    _globals["_OBSERVEDELEGATIONSREQUEST"]._serialized_end = 25688
+    _globals["_OBSERVEDELEGATIONSRESPONSE"]._serialized_start = 25690
+    _globals["_OBSERVEDELEGATIONSRESPONSE"]._serialized_end = 25768
+    _globals["_NODEBASIC"]._serialized_start = 25771
+    _globals["_NODEBASIC"]._serialized_end = 26044
+    _globals["_GETNETWORKDATAREQUEST"]._serialized_start = 26046
+    _globals["_GETNETWORKDATAREQUEST"]._serialized_end = 26069
+    _globals["_GETNETWORKDATARESPONSE"]._serialized_start = 26071
+    _globals["_GETNETWORKDATARESPONSE"]._serialized_end = 26140
+    _globals["_GETNODEREQUEST"]._serialized_start = 26142
+    _globals["_GETNODEREQUEST"]._serialized_end = 26180
+    _globals["_GETNODERESPONSE"]._serialized_start = 26182
+    _globals["_GETNODERESPONSE"]._serialized_end = 26231
+    _globals["_LISTNODESREQUEST"]._serialized_start = 26234
+    _globals["_LISTNODESREQUEST"]._serialized_end = 26381
+    _globals["_LISTNODESRESPONSE"]._serialized_start = 26383
+    _globals["_LISTNODESRESPONSE"]._serialized_end = 26458
+    _globals["_NODEEDGE"]._serialized_start = 26460
+    _globals["_NODEEDGE"]._serialized_end = 26526
+    _globals["_NODESCONNECTION"]._serialized_start = 26528
+    _globals["_NODESCONNECTION"]._serialized_end = 26650
+    _globals["_LISTNODESIGNATURESREQUEST"]._serialized_start = 26653
+    _globals["_LISTNODESIGNATURESREQUEST"]._serialized_end = 26783
+    _globals["_LISTNODESIGNATURESRESPONSE"]._serialized_start = 26785
+    _globals["_LISTNODESIGNATURESRESPONSE"]._serialized_end = 26888
+    _globals["_NODESIGNATUREEDGE"]._serialized_start = 26890
+    _globals["_NODESIGNATUREEDGE"]._serialized_end = 26986
+    _globals["_NODESIGNATURESCONNECTION"]._serialized_start = 26989
+    _globals["_NODESIGNATURESCONNECTION"]._serialized_end = 27129
+    _globals["_GETEPOCHREQUEST"]._serialized_start = 27131
+    _globals["_GETEPOCHREQUEST"]._serialized_end = 27213
+    _globals["_GETEPOCHRESPONSE"]._serialized_start = 27215
+    _globals["_GETEPOCHRESPONSE"]._serialized_end = 27268
+    _globals["_ESTIMATEFEEREQUEST"]._serialized_start = 27270
+    _globals["_ESTIMATEFEEREQUEST"]._serialized_end = 27379
+    _globals["_ESTIMATEFEERESPONSE"]._serialized_start = 27381
+    _globals["_ESTIMATEFEERESPONSE"]._serialized_end = 27431
+    _globals["_ESTIMATEMARGINREQUEST"]._serialized_start = 27434
+    _globals["_ESTIMATEMARGINREQUEST"]._serialized_end = 27665
+    _globals["_ESTIMATEMARGINRESPONSE"]._serialized_start = 27667
+    _globals["_ESTIMATEMARGINRESPONSE"]._serialized_end = 27752
+    _globals["_LISTNETWORKPARAMETERSREQUEST"]._serialized_start = 27754
+    _globals["_LISTNETWORKPARAMETERSREQUEST"]._serialized_end = 27865
+    _globals["_LISTNETWORKPARAMETERSRESPONSE"]._serialized_start = 27867
+    _globals["_LISTNETWORKPARAMETERSRESPONSE"]._serialized_end = 27990
+    _globals["_GETNETWORKPARAMETERREQUEST"]._serialized_start = 27992
+    _globals["_GETNETWORKPARAMETERREQUEST"]._serialized_end = 28044
+    _globals["_GETNETWORKPARAMETERRESPONSE"]._serialized_start = 28046
+    _globals["_GETNETWORKPARAMETERRESPONSE"]._serialized_end = 28144
+    _globals["_NETWORKPARAMETEREDGE"]._serialized_start = 28146
+    _globals["_NETWORKPARAMETEREDGE"]._serialized_end = 28236
+    _globals["_NETWORKPARAMETERCONNECTION"]._serialized_start = 28239
+    _globals["_NETWORKPARAMETERCONNECTION"]._serialized_end = 28384
+    _globals["_CHECKPOINT"]._serialized_start = 28386
+    _globals["_CHECKPOINT"]._serialized_end = 28476
+    _globals["_LISTCHECKPOINTSREQUEST"]._serialized_start = 28478
+    _globals["_LISTCHECKPOINTSREQUEST"]._serialized_end = 28583
+    _globals["_LISTCHECKPOINTSRESPONSE"]._serialized_start = 28585
+    _globals["_LISTCHECKPOINTSRESPONSE"]._serialized_end = 28684
+    _globals["_CHECKPOINTEDGE"]._serialized_start = 28686
+    _globals["_CHECKPOINTEDGE"]._serialized_end = 28775
+    _globals["_CHECKPOINTSCONNECTION"]._serialized_start = 28778
+    _globals["_CHECKPOINTSCONNECTION"]._serialized_end = 28912
+    _globals["_GETSTAKEREQUEST"]._serialized_start = 28915
+    _globals["_GETSTAKEREQUEST"]._serialized_end = 29046
+    _globals["_GETSTAKERESPONSE"]._serialized_start = 29049
+    _globals["_GETSTAKERESPONSE"]._serialized_end = 29197
+    _globals["_STAKELINKINGEDGE"]._serialized_start = 29199
+    _globals["_STAKELINKINGEDGE"]._serialized_end = 29291
+    _globals["_STAKESCONNECTION"]._serialized_start = 29294
+    _globals["_STAKESCONNECTION"]._serialized_end = 29425
+    _globals["_GETRISKFACTORSREQUEST"]._serialized_start = 29427
+    _globals["_GETRISKFACTORSREQUEST"]._serialized_end = 29485
+    _globals["_GETRISKFACTORSRESPONSE"]._serialized_start = 29487
+    _globals["_GETRISKFACTORSRESPONSE"]._serialized_end = 29562
+    _globals["_OBSERVEEVENTBUSREQUEST"]._serialized_start = 29565
+    _globals["_OBSERVEEVENTBUSREQUEST"]._serialized_end = 29726
+    _globals["_OBSERVEEVENTBUSRESPONSE"]._serialized_start = 29728
+    _globals["_OBSERVEEVENTBUSRESPONSE"]._serialized_end = 29803
+    _globals["_OBSERVELEDGERMOVEMENTSREQUEST"]._serialized_start = 29805
+    _globals["_OBSERVELEDGERMOVEMENTSREQUEST"]._serialized_end = 29836
+    _globals["_OBSERVELEDGERMOVEMENTSRESPONSE"]._serialized_start = 29838
+    _globals["_OBSERVELEDGERMOVEMENTSRESPONSE"]._serialized_end = 29933
+    _globals["_LISTKEYROTATIONSREQUEST"]._serialized_start = 29936
+    _globals["_LISTKEYROTATIONSREQUEST"]._serialized_end = 30084
+    _globals["_LISTKEYROTATIONSRESPONSE"]._serialized_start = 30086
+    _globals["_LISTKEYROTATIONSRESPONSE"]._serialized_end = 30182
+    _globals["_KEYROTATIONEDGE"]._serialized_start = 30184
+    _globals["_KEYROTATIONEDGE"]._serialized_end = 30274
+    _globals["_KEYROTATIONCONNECTION"]._serialized_start = 30277
+    _globals["_KEYROTATIONCONNECTION"]._serialized_end = 30412
+    _globals["_LISTETHEREUMKEYROTATIONSREQUEST"]._serialized_start = 30415
+    _globals["_LISTETHEREUMKEYROTATIONSREQUEST"]._serialized_end = 30571
+    _globals["_LISTETHEREUMKEYROTATIONSRESPONSE"]._serialized_start = 30573
+    _globals["_LISTETHEREUMKEYROTATIONSRESPONSE"]._serialized_end = 30693
+    _globals["_ETHEREUMKEYROTATIONSCONNECTION"]._serialized_start = 30696
+    _globals["_ETHEREUMKEYROTATIONSCONNECTION"]._serialized_end = 30848
+    _globals["_ETHEREUMKEYROTATIONEDGE"]._serialized_start = 30850
+    _globals["_ETHEREUMKEYROTATIONEDGE"]._serialized_end = 30956
+    _globals["_GETVEGATIMEREQUEST"]._serialized_start = 30958
+    _globals["_GETVEGATIMEREQUEST"]._serialized_end = 30978
+    _globals["_GETVEGATIMERESPONSE"]._serialized_start = 30980
+    _globals["_GETVEGATIMERESPONSE"]._serialized_end = 31031
+    _globals["_DATERANGE"]._serialized_start = 31034
+    _globals["_DATERANGE"]._serialized_end = 31171
+    _globals["_GETPROTOCOLUPGRADESTATUSREQUEST"]._serialized_start = 31173
+    _globals["_GETPROTOCOLUPGRADESTATUSREQUEST"]._serialized_end = 31206
+    _globals["_GETPROTOCOLUPGRADESTATUSRESPONSE"]._serialized_start = 31208
+    _globals["_GETPROTOCOLUPGRADESTATUSRESPONSE"]._serialized_end = 31264
+    _globals["_LISTPROTOCOLUPGRADEPROPOSALSREQUEST"]._serialized_start = 31267
+    _globals["_LISTPROTOCOLUPGRADEPROPOSALSREQUEST"]._serialized_end = 31526
+    _globals["_LISTPROTOCOLUPGRADEPROPOSALSRESPONSE"]._serialized_start = 31529
+    _globals["_LISTPROTOCOLUPGRADEPROPOSALSRESPONSE"]._serialized_end = 31681
+    _globals["_PROTOCOLUPGRADEPROPOSALCONNECTION"]._serialized_start = 31684
+    _globals["_PROTOCOLUPGRADEPROPOSALCONNECTION"]._serialized_end = 31843
+    _globals["_PROTOCOLUPGRADEPROPOSALEDGE"]._serialized_start = 31845
+    _globals["_PROTOCOLUPGRADEPROPOSALEDGE"]._serialized_end = 31956
+    _globals["_LISTCORESNAPSHOTSREQUEST"]._serialized_start = 31958
+    _globals["_LISTCORESNAPSHOTSREQUEST"]._serialized_end = 32065
+    _globals["_LISTCORESNAPSHOTSRESPONSE"]._serialized_start = 32067
+    _globals["_LISTCORESNAPSHOTSRESPONSE"]._serialized_end = 32174
+    _globals["_CORESNAPSHOTCONNECTION"]._serialized_start = 32177
+    _globals["_CORESNAPSHOTCONNECTION"]._serialized_end = 32314
+    _globals["_CORESNAPSHOTEDGE"]._serialized_start = 32316
+    _globals["_CORESNAPSHOTEDGE"]._serialized_end = 32412
+    _globals["_HISTORYSEGMENT"]._serialized_start = 32415
+    _globals["_HISTORYSEGMENT"]._serialized_end = 32672
+    _globals["_GETMOSTRECENTNETWORKHISTORYSEGMENTREQUEST"]._serialized_start = 32674
+    _globals["_GETMOSTRECENTNETWORKHISTORYSEGMENTREQUEST"]._serialized_end = 32717
+    _globals["_GETMOSTRECENTNETWORKHISTORYSEGMENTRESPONSE"]._serialized_start = 32720
+    _globals["_GETMOSTRECENTNETWORKHISTORYSEGMENTRESPONSE"]._serialized_end = 32861
+    _globals["_LISTALLNETWORKHISTORYSEGMENTSREQUEST"]._serialized_start = 32863
+    _globals["_LISTALLNETWORKHISTORYSEGMENTSREQUEST"]._serialized_end = 32901
+    _globals["_LISTALLNETWORKHISTORYSEGMENTSRESPONSE"]._serialized_start = 32903
+    _globals["_LISTALLNETWORKHISTORYSEGMENTSRESPONSE"]._serialized_end = 33003
+    _globals["_GETACTIVENETWORKHISTORYPEERADDRESSESREQUEST"]._serialized_start = 33005
+    _globals["_GETACTIVENETWORKHISTORYPEERADDRESSESREQUEST"]._serialized_end = 33050
+    _globals["_GETACTIVENETWORKHISTORYPEERADDRESSESRESPONSE"]._serialized_start = 33052
+    _globals["_GETACTIVENETWORKHISTORYPEERADDRESSESRESPONSE"]._serialized_end = 33133
+    _globals["_GETNETWORKHISTORYSTATUSREQUEST"]._serialized_start = 33135
+    _globals["_GETNETWORKHISTORYSTATUSREQUEST"]._serialized_end = 33167
+    _globals["_GETNETWORKHISTORYSTATUSRESPONSE"]._serialized_start = 33170
+    _globals["_GETNETWORKHISTORYSTATUSRESPONSE"]._serialized_end = 33346
+    _globals["_GETNETWORKHISTORYBOOTSTRAPPEERSREQUEST"]._serialized_start = 33348
+    _globals["_GETNETWORKHISTORYBOOTSTRAPPEERSREQUEST"]._serialized_end = 33388
+    _globals["_GETNETWORKHISTORYBOOTSTRAPPEERSRESPONSE"]._serialized_start = 33390
+    _globals["_GETNETWORKHISTORYBOOTSTRAPPEERSRESPONSE"]._serialized_end = 33472
+    _globals["_EXPORTNETWORKHISTORYREQUEST"]._serialized_start = 33475
+    _globals["_EXPORTNETWORKHISTORYREQUEST"]._serialized_end = 33608
+    _globals["_LISTENTITIESREQUEST"]._serialized_start = 33610
+    _globals["_LISTENTITIESREQUEST"]._serialized_end = 33680
+    _globals["_LISTENTITIESRESPONSE"]._serialized_start = 33683
+    _globals["_LISTENTITIESRESPONSE"]._serialized_end = 35392
+    _globals["_PINGREQUEST"]._serialized_start = 35394
+    _globals["_PINGREQUEST"]._serialized_end = 35407
+    _globals["_PINGRESPONSE"]._serialized_start = 35409
+    _globals["_PINGRESPONSE"]._serialized_end = 35423
+    _globals["_ORDERINFO"]._serialized_start = 35426
+    _globals["_ORDERINFO"]._serialized_end = 35561
+    _globals["_ESTIMATEPOSITIONREQUEST"]._serialized_start = 35564
+    _globals["_ESTIMATEPOSITIONREQUEST"]._serialized_end = 35796
+    _globals["_ESTIMATEPOSITIONRESPONSE"]._serialized_start = 35799
+    _globals["_ESTIMATEPOSITIONRESPONSE"]._serialized_end = 35954
+    _globals["_MARGINESTIMATE"]._serialized_start = 35956
+    _globals["_MARGINESTIMATE"]._serialized_end = 36072
+    _globals["_LIQUIDATIONESTIMATE"]._serialized_start = 36075
+    _globals["_LIQUIDATIONESTIMATE"]._serialized_end = 36226
+    _globals["_LIQUIDATIONPRICE"]._serialized_start = 36229
+    _globals["_LIQUIDATIONPRICE"]._serialized_end = 36391
+    _globals["_TRADINGDATASERVICE"]._serialized_start = 37275
+    _globals["_TRADINGDATASERVICE"]._serialized_end = 48307
 # @@protoc_insertion_point(module_scope)
```

### Comparing `vega_sim-1.1.1/vega_sim/proto/data_node/api/v2/trading_data_pb2_grpc.py` & `vega_sim-1.2.0/vega_sim/proto/data_node/api/v2/trading_data_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,14 +213,19 @@
             response_deserializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.GetMarketResponse.FromString,
         )
         self.ListMarkets = channel.unary_unary(
             "/datanode.api.v2.TradingDataService/ListMarkets",
             request_serializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.ListMarketsRequest.SerializeToString,
             response_deserializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.ListMarketsResponse.FromString,
         )
+        self.ListSuccessorMarkets = channel.unary_unary(
+            "/datanode.api.v2.TradingDataService/ListSuccessorMarkets",
+            request_serializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.ListSuccessorMarketsRequest.SerializeToString,
+            response_deserializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.ListSuccessorMarketsResponse.FromString,
+        )
         self.GetParty = channel.unary_unary(
             "/datanode.api.v2.TradingDataService/GetParty",
             request_serializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.GetPartyRequest.SerializeToString,
             response_deserializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.GetPartyResponse.FromString,
         )
         self.ListParties = channel.unary_unary(
             "/datanode.api.v2.TradingDataService/ListParties",
@@ -490,15 +495,15 @@
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def GetOrder(self, request, context):
         """Get order
 
-        Get the current version of an order, or optionally provide a version ID to retrieve a given version if order was amended.
+        Get an order by its ID. An order's ID will be the SHA3-256 hash of the signature that the order was submitted with
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def ListOrders(self, request, context):
         """List orders
@@ -536,24 +541,25 @@
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def ListAllPositions(self, request, context):
         """List positions
 
-        Get a list of positions by party's public key using cursor based pagination
+        Get a list of all of a party's positions
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def ObservePositions(self, request, context):
         """Observe positions
 
-        Subscribe to a stream of positions
+        Subscribe to a stream of position updates. The first messages sent through the stream will contain
+        information about current positions, followed by updates to those positions.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def ListLedgerEntries(self, request, context):
         """List ledger entries
@@ -590,24 +596,14 @@
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def ListBalanceChanges(self, request, context):
         """List balance changes
 
         Get a list of the changes in account balances over a period of time.
-
-        An account is defined as a set of asset_id, type, party_id, and market_id.
-        - Every account has an associated asset and type.
-        - Certain account types such as the global reward pool for example, do not have an associated party.
-        These are denoted by the special party ID 'network'
-        - Certain account types do not have an associated market such as the general party accounts, for example.
-        These are denoted by the special market ID '' (the empty string)
-
-        `ListBalanceChangesRequest` will return a list of `AggregatedBalance` records,
-        with a row for each block at which a given account's balance changes.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def GetLatestMarketData(self, request, context):
         """Get latest market data
@@ -662,42 +658,45 @@
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def GetMarketDataHistoryByID(self, request, context):
         """Get market data history
 
-        Get market data history for a market ID between given dates
+        Get market data history for a market ID from between a given date range
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def ListTransfers(self, request, context):
         """List transfers
 
-        Get a list of transfers to/from/either a public key
+        Get a list of transfers between public keys. A valid value for public key can be one of:
+        - a party ID
+        - "network"
+        - "0000000000000000000000000000000000000000000000000000000000000000", the public key for the global rewards account
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def GetNetworkLimits(self, request, context):
         """Get network limits
 
-        Get the current network limits, for example: is bootstrapping finished, are proposals enabled etc.
+        Get the network limits relating to asset and market creation
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def ListCandleData(self, request, context):
         """List candle data
 
-        Get a list of candle data for a given candle ID. You can get a candle ID from the list candle intervals query
+        Get a list of candle data for a given candle ID. Candle IDs can be obtained by calling list-candle-intervals
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def ObserveCandleData(self, request, context):
         """Observe candle data
@@ -716,24 +715,24 @@
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def ListVotes(self, request, context):
         """List votes
 
-        Get a list of votes for a party ID
+        Get a list of votes. A party ID or a proposal ID must be provided.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def ObserveVotes(self, request, context):
         """Observe votes
 
-        Subscribe to a stream of votes
+        Subscribe to a stream of votes cast on a given proposal, or by all votes made by a given party
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def ListERC20MultiSigSignerAddedBundles(self, request, context):
         """List ERC20 multi-sig signer added bundles
@@ -771,24 +770,24 @@
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def GetERC20WithdrawalApproval(self, request, context):
         """Get ERC20 withdrawal approval
 
-        Get the signature bundle to finalize a withdrawal on ethereum
+        Get the signature bundle to finalise a withdrawal on Ethereum
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def GetLastTrade(self, request, context):
-        """Get latest trade
+        """Get last trade
 
-        Get latest trade
+        Get the last trade made for a given market.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def ListTrades(self, request, context):
         """List trades
@@ -807,51 +806,63 @@
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def GetOracleSpec(self, request, context):
         """Get oracle spec
 
-        Get an oracle spec by ID. Use the oracle spec list to query for oracle spec IDs
+        Get an oracle spec by ID. Oracle spec IDs can be found by querying markets that use them as a data source
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def ListOracleSpecs(self, request, context):
         """List oracle specs
 
-        Get a list of specs for an oracle
+        Get a list of all oracles specs that are defined against all markets
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def ListOracleData(self, request, context):
         """List oracle data
 
-        Get a list of all oracle data
+        Get a list of all oracle data that have been broadcast to any market
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def GetMarket(self, request, context):
         """Get market
 
-        Get information about a specific market using its ID. Use the market lists query to get a market's ID
+        Get information about a specific market using its ID. A market's ID will be the same as the ID of the proposal that
+        generated it
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def ListMarkets(self, request, context):
         """List markets
 
-        Get a list of markets using a cursor based pagination
+        Get a list of markets
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details("Method not implemented!")
+        raise NotImplementedError("Method not implemented!")
+
+    def ListSuccessorMarkets(self, request, context):
+        """List successor markets
+
+        Given a market ID, return the full lineage of markets since inception, or all successor markets since and including
+        the given market ID. The markets will be returned in succession order, i.e. the market at position i will be the parent
+        of the market at position i+1.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def GetParty(self, request, context):
         """Get party
@@ -861,15 +872,15 @@
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def ListParties(self, request, context):
         """List parties
 
-        Get a list of parties. If a party ID is provided, only that party will be returned.
+        Get a list of parties
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def ListMarginLevels(self, request, context):
         """List margin levels
@@ -879,15 +890,15 @@
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def ObserveMarginLevels(self, request, context):
         """Observe margin levels
 
-        Subscribe to a stream of margin levels
+        Subscribe to a stream of margin levels updates
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def ListRewards(self, request, context):
         """List rewards
@@ -940,15 +951,15 @@
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def GetWithdrawal(self, request, context):
         """Get withdrawal
 
-        Get a withdrawal by its ID. Use the withdrawals list query to get withdrawal IDs
+        Get a withdrawal by its ID. A withdrawal's ID will be the SHA3-256 hash of the signature that the withdrawal was submitted with
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def ListWithdrawals(self, request, context):
         """List withdrawals
@@ -967,24 +978,24 @@
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def ListAssets(self, request, context):
         """List assets
 
-        Get a list of assets using cursor based pagination
+        Get a list of assets available on the Vega network
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def ListLiquidityProvisions(self, request, context):
         """List liquidity provisions
 
-        Get a list of liquidity provisions for a given market using a cursor based pagination
+        Get a list of liquidity provisions for a given market
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def ObserveLiquidityProvisions(self, request, context):
         """Observe liquidity provisions
@@ -994,15 +1005,15 @@
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def GetGovernanceData(self, request, context):
         """Get governance data
 
-        Get a single proposal's details
+        Get a single proposal's details either by proposal ID or by reference
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def ListGovernanceData(self, request, context):
         """List governance data
@@ -1012,15 +1023,15 @@
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def ObserveGovernance(self, request, context):
         """Observe governance
 
-        Subscribe to a stream of governance proposals
+        Subscribe to a stream of updates to governance proposals
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def ListDelegations(self, request, context):
         """List delegations
@@ -1104,24 +1115,24 @@
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def ListNetworkParameters(self, request, context):
         """List network parameters
 
-        Get a list of the network parameters
+        Get a list of the network parameter keys and their values
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def GetNetworkParameter(self, request, context):
         """Get network parameter
 
-        Get a single network parameter
+        Get a network parameter's value by its key
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def ListCheckpoints(self, request, context):
         """List checkpoints
@@ -1129,15 +1140,15 @@
         Get a list of information about checkpoints generated by the network
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def GetStake(self, request, context):
-        """Get Stake
+        """Get stake
 
         Get staking information for a given party
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
@@ -1185,15 +1196,15 @@
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def GetVegaTime(self, request, context):
         """Get Vega time
 
-        Get the current time of the network, displayed as a Unix timestamp in nano seconds
+        Get the current time of the network in Unix nanoseconds
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def GetProtocolUpgradeStatus(self, request, context):
         """Get protocol upgrade status
@@ -1255,26 +1266,24 @@
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def GetNetworkHistoryStatus(self, request, context):
         """Network history status
 
-        Get information about the current state of network history
-        Response contains the network history status
+        Get information about the current state of network history's IPFS swarm
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def GetNetworkHistoryBootstrapPeers(self, request, context):
         """Network history bootstrap peers
 
-        Get the bootstrap peers for data nodes.
-        Response contains the bootstrap peers
+        Get a list of IPFS peers that can be used to initialise a new data node with network history
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def ListEntities(self, request, context):
         """List entities
@@ -1292,15 +1301,15 @@
 
         The requested block heights must fall on network history segment boundaries, which can
         be discovered by calling the API to list all network history segments. By default
         segments contain 1000 blocks. In that case ranges such as (1, 1000), (1001, 2000), (1, 3000)
         would all fall on segment boundaries and be valid.
 
         The generated CSV file is compressed into a ZIP file and returned, with the file name
-        in the following format: [chain id]-[table name]-[start block]-[end block].zip
+        in the following format: `[chain id]-[table name]-[start block]-[end block].zip`
 
         In gRPC, results are returned in a chunked stream of base64 encoded data.
 
         Through the REST gateway, the base64 data chunks are decoded and streamed as a
         `content-type: application/zip` HTTP response.
 
         The CSV exported data uses a comma as a DELIMITER between fields, and " for QUOTE-ing fields.
@@ -1325,25 +1334,25 @@
         the (from_block, to_block) request spans over a range of blocks in which the underlying
         schema of the database changes. For example, a column may have been added, removed, or renamed.
 
         If this happens, the CSV file will be split at the point of the schema change and the zip
         file will contain multiple CSV files, with a potentially different set of headers. The
         'version' number of the database schema is part of the in the CSV filename:
 
-        [chain id]-[table name]-[schema version]-[start block]-[end block].zip
+        `[chain id]-[table name]-[schema version]-[start block]-[end block].zip`
 
         For example, a zip file might be called mainnet-sometable-000001-003000.zip
 
-        And contain two CSV files: mainnet-sometable-1-000001-002000.csv:
+        And contain two CSV files: `mainnet-sometable-1-000001-002000.csv`:
 
         timestamp, value
         1, foo
         2, bar
 
-        And mainnet-sometable-2-002001-003000.csv:
+        And `mainnet-sometable-2-002001-003000.csv`:
 
         timestamp, value, extra_value
         3, baz, apple
 
         It is worth noting that the schema will not change within a single network history segment.
         buf:lint:ignore RPC_RESPONSE_STANDARD_NAME
         buf:lint:ignore RPC_REQUEST_RESPONSE_UNIQUE
@@ -1560,14 +1569,19 @@
             response_serializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.GetMarketResponse.SerializeToString,
         ),
         "ListMarkets": grpc.unary_unary_rpc_method_handler(
             servicer.ListMarkets,
             request_deserializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.ListMarketsRequest.FromString,
             response_serializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.ListMarketsResponse.SerializeToString,
         ),
+        "ListSuccessorMarkets": grpc.unary_unary_rpc_method_handler(
+            servicer.ListSuccessorMarkets,
+            request_deserializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.ListSuccessorMarketsRequest.FromString,
+            response_serializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.ListSuccessorMarketsResponse.SerializeToString,
+        ),
         "GetParty": grpc.unary_unary_rpc_method_handler(
             servicer.GetParty,
             request_deserializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.GetPartyRequest.FromString,
             response_serializer=data__node_dot_api_dot_v2_dot_trading__data__pb2.GetPartyResponse.SerializeToString,
         ),
         "ListParties": grpc.unary_unary_rpc_method_handler(
             servicer.ListParties,
@@ -2968,14 +2982,43 @@
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
+            metadata,
+        )
+
+    @staticmethod
+    def ListSuccessorMarkets(
+        request,
+        target,
+        options=(),
+        channel_credentials=None,
+        call_credentials=None,
+        insecure=False,
+        compression=None,
+        wait_for_ready=None,
+        timeout=None,
+        metadata=None,
+    ):
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            "/datanode.api.v2.TradingDataService/ListSuccessorMarkets",
+            data__node_dot_api_dot_v2_dot_trading__data__pb2.ListSuccessorMarketsRequest.SerializeToString,
+            data__node_dot_api_dot_v2_dot_trading__data__pb2.ListSuccessorMarketsResponse.FromString,
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
             metadata,
         )
 
     @staticmethod
     def GetParty(
         request,
         target,
```

### Comparing `vega_sim-1.1.1/vega_sim/proto/vega/__init__.py` & `vega_sim-1.2.0/vega_sim/proto/vega/__init__.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/proto/vega/api/v1/core_pb2.py` & `vega_sim-1.2.0/vega_sim/proto/vega/api/v1/core_pb2.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: vega/api/v1/core.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
@@ -20,106 +20,115 @@
     transaction_pb2 as vega_dot_commands_dot_v1_dot_transaction__pb2,
 )
 from ...events.v1 import events_pb2 as vega_dot_events_dot_v1_dot_events__pb2
 from ... import vega_pb2 as vega_dot_vega__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x16vega/api/v1/core.proto\x12\x0bvega.api.v1\x1a\x1fgoogle/api/field_behavior.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\x1a"vega/commands/v1/transaction.proto\x1a\x1bvega/events/v1/events.proto\x1a\x0fvega/vega.proto"x\n\x1aPropagateChainEventRequest\x12\x19\n\x05\x65vent\x18\x01 \x01(\x0c\x42\x03\xe0\x41\x02R\x05\x65vent\x12\x1c\n\x07pub_key\x18\x02 \x01(\tB\x03\xe0\x41\x02R\x06pubKey\x12!\n\tsignature\x18\x03 \x01(\x0c\x42\x03\xe0\x41\x02R\tsignature"7\n\x1bPropagateChainEventResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success"\xe1\x01\n\x18SubmitTransactionRequest\x12\x32\n\x02tx\x18\x01 \x01(\x0b\x32\x1d.vega.commands.v1.TransactionB\x03\xe0\x41\x02R\x02tx\x12\x43\n\x04type\x18\x02 \x01(\x0e\x32*.vega.api.v1.SubmitTransactionRequest.TypeB\x03\xe0\x41\x02R\x04type"L\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x0e\n\nTYPE_ASYNC\x10\x01\x12\r\n\tTYPE_SYNC\x10\x02\x12\x0f\n\x0bTYPE_COMMIT\x10\x03"\xa0\x01\n\x19SubmitTransactionResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12\x17\n\x07tx_hash\x18\x02 \x01(\tR\x06txHash\x12\x12\n\x04\x63ode\x18\x03 \x01(\rR\x04\x63ode\x12\x12\n\x04\x64\x61ta\x18\x04 \x01(\tR\x04\x64\x61ta\x12\x10\n\x03log\x18\x05 \x01(\tR\x03log\x12\x16\n\x06height\x18\x06 \x01(\x03R\x06height"M\n\x17\x43heckTransactionRequest\x12\x32\n\x02tx\x18\x01 \x01(\x0b\x32\x1d.vega.commands.v1.TransactionB\x03\xe0\x41\x02R\x02tx"\xbc\x01\n\x18\x43heckTransactionResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12\x12\n\x04\x63ode\x18\x02 \x01(\rR\x04\x63ode\x12\x1d\n\ngas_wanted\x18\x03 \x01(\x03R\tgasWanted\x12\x19\n\x08gas_used\x18\x04 \x01(\x03R\x07gasUsed\x12\x12\n\x04\x64\x61ta\x18\x05 \x01(\tR\x04\x64\x61ta\x12\x10\n\x03log\x18\x06 \x01(\tR\x03log\x12\x12\n\x04info\x18\x07 \x01(\tR\x04info"\xc8\x01\n\x1bSubmitRawTransactionRequest\x12\x13\n\x02tx\x18\x01 \x01(\x0c\x42\x03\xe0\x41\x02R\x02tx\x12\x46\n\x04type\x18\x02 \x01(\x0e\x32-.vega.api.v1.SubmitRawTransactionRequest.TypeB\x03\xe0\x41\x02R\x04type"L\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x0e\n\nTYPE_ASYNC\x10\x01\x12\r\n\tTYPE_SYNC\x10\x02\x12\x0f\n\x0bTYPE_COMMIT\x10\x03"\xa3\x01\n\x1cSubmitRawTransactionResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12\x17\n\x07tx_hash\x18\x02 \x01(\tR\x06txHash\x12\x12\n\x04\x63ode\x18\x03 \x01(\rR\x04\x63ode\x12\x12\n\x04\x64\x61ta\x18\x04 \x01(\tR\x04\x64\x61ta\x12\x10\n\x03log\x18\x05 \x01(\tR\x03log\x12\x16\n\x06height\x18\x06 \x01(\x03R\x06height"1\n\x1a\x43heckRawTransactionRequest\x12\x13\n\x02tx\x18\x01 \x01(\x0c\x42\x03\xe0\x41\x02R\x02tx"\xbf\x01\n\x1b\x43heckRawTransactionResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12\x12\n\x04\x63ode\x18\x02 \x01(\rR\x04\x63ode\x12\x1d\n\ngas_wanted\x18\x03 \x01(\x03R\tgasWanted\x12\x19\n\x08gas_used\x18\x04 \x01(\x03R\x07gasUsed\x12\x12\n\x04\x64\x61ta\x18\x05 \x01(\tR\x04\x64\x61ta\x12\x10\n\x03log\x18\x06 \x01(\tR\x03log\x12\x12\n\x04info\x18\x07 \x01(\tR\x04info"\x14\n\x12GetVegaTimeRequest"3\n\x13GetVegaTimeResponse\x12\x1c\n\ttimestamp\x18\x01 \x01(\x03R\ttimestamp"\xa1\x01\n\x16ObserveEventBusRequest\x12\x30\n\x04type\x18\x01 \x03(\x0e\x32\x1c.vega.events.v1.BusEventTypeR\x04type\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x03 \x01(\tR\x07partyId\x12\x1d\n\nbatch_size\x18\x04 \x01(\x03R\tbatchSize"K\n\x17ObserveEventBusResponse\x12\x30\n\x06\x65vents\x18\x01 \x03(\x0b\x32\x18.vega.events.v1.BusEventR\x06\x65vents"\x13\n\x11StatisticsRequest"M\n\x12StatisticsResponse\x12\x37\n\nstatistics\x18\x01 \x01(\x0b\x32\x17.vega.api.v1.StatisticsR\nstatistics"\xc8\x0c\n\nStatistics\x12!\n\x0c\x62lock_height\x18\x01 \x01(\x04R\x0b\x62lockHeight\x12%\n\x0e\x62\x61\x63klog_length\x18\x02 \x01(\x04R\rbacklogLength\x12\x1f\n\x0btotal_peers\x18\x03 \x01(\x04R\ntotalPeers\x12!\n\x0cgenesis_time\x18\x04 \x01(\tR\x0bgenesisTime\x12!\n\x0c\x63urrent_time\x18\x05 \x01(\tR\x0b\x63urrentTime\x12\x1b\n\tvega_time\x18\x06 \x01(\tR\x08vegaTime\x12)\n\x06status\x18\x07 \x01(\x0e\x32\x11.vega.ChainStatusR\x06status\x12 \n\x0ctx_per_block\x18\x08 \x01(\x04R\ntxPerBlock\x12(\n\x10\x61verage_tx_bytes\x18\t \x01(\x04R\x0e\x61verageTxBytes\x12\x37\n\x18\x61verage_orders_per_block\x18\n \x01(\x04R\x15\x61verageOrdersPerBlock\x12*\n\x11trades_per_second\x18\x0b \x01(\x04R\x0ftradesPerSecond\x12*\n\x11orders_per_second\x18\x0c \x01(\x04R\x0fordersPerSecond\x12#\n\rtotal_markets\x18\r \x01(\x04R\x0ctotalMarkets\x12*\n\x11total_amend_order\x18\x10 \x01(\x04R\x0ftotalAmendOrder\x12,\n\x12total_cancel_order\x18\x11 \x01(\x04R\x10totalCancelOrder\x12,\n\x12total_create_order\x18\x12 \x01(\x04R\x10totalCreateOrder\x12!\n\x0ctotal_orders\x18\x13 \x01(\x04R\x0btotalOrders\x12!\n\x0ctotal_trades\x18\x14 \x01(\x04R\x0btotalTrades\x12/\n\x13order_subscriptions\x18\x15 \x01(\rR\x12orderSubscriptions\x12/\n\x13trade_subscriptions\x18\x16 \x01(\rR\x12tradeSubscriptions\x12\x31\n\x14\x63\x61ndle_subscriptions\x18\x17 \x01(\rR\x13\x63\x61ndleSubscriptions\x12<\n\x1amarket_depth_subscriptions\x18\x18 \x01(\rR\x18marketDepthSubscriptions\x12\x37\n\x17positions_subscriptions\x18\x19 \x01(\rR\x16positionsSubscriptions\x12\x33\n\x15\x61\x63\x63ount_subscriptions\x18\x1a \x01(\rR\x14\x61\x63\x63ountSubscriptions\x12:\n\x19market_data_subscriptions\x18\x1b \x01(\rR\x17marketDataSubscriptions\x12(\n\x10\x61pp_version_hash\x18\x1c \x01(\tR\x0e\x61ppVersionHash\x12\x1f\n\x0b\x61pp_version\x18\x1d \x01(\tR\nappVersion\x12#\n\rchain_version\x18\x1e \x01(\tR\x0c\x63hainVersion\x12%\n\x0e\x62lock_duration\x18\x1f \x01(\x04R\rblockDuration\x12\x16\n\x06uptime\x18  \x01(\tR\x06uptime\x12\x19\n\x08\x63hain_id\x18! \x01(\tR\x07\x63hainId\x12K\n"market_depth_updates_subscriptions\x18" \x01(\rR\x1fmarketDepthUpdatesSubscriptions\x12\x1d\n\nblock_hash\x18# \x01(\tR\tblockHash\x12\x1b\n\tepoch_seq\x18$ \x01(\x04R\x08\x65pochSeq\x12(\n\x10\x65poch_start_time\x18% \x01(\tR\x0e\x65pochStartTime\x12*\n\x11\x65poch_expiry_time\x18& \x01(\tR\x0f\x65pochExpiryTime\x12\x1f\n\x0b\x65vent_count\x18\' \x01(\x04R\neventCount\x12*\n\x11\x65vents_per_second\x18( \x01(\x04R\x0f\x65ventsPerSecond"\x18\n\x16LastBlockHeightRequest"\x91\x03\n\x17LastBlockHeightResponse\x12\x16\n\x06height\x18\x01 \x01(\x04R\x06height\x12\x12\n\x04hash\x18\x02 \x01(\tR\x04hash\x12\x33\n\x16spam_pow_hash_function\x18\x03 \x01(\tR\x13spamPowHashFunction\x12.\n\x13spam_pow_difficulty\x18\x04 \x01(\rR\x11spamPowDifficulty\x12\x41\n\x1espam_pow_number_of_past_blocks\x18\x05 \x01(\rR\x19spamPowNumberOfPastBlocks\x12\x42\n\x1fspam_pow_number_of_tx_per_block\x18\x06 \x01(\rR\x19spamPowNumberOfTxPerBlock\x12\x43\n\x1espam_pow_increasing_difficulty\x18\x07 \x01(\x08R\x1bspamPowIncreasingDifficulty\x12\x19\n\x08\x63hain_id\x18\x08 \x01(\tR\x07\x63hainId":\n\x18GetSpamStatisticsRequest\x12\x1e\n\x08party_id\x18\x01 \x01(\tB\x03\xe0\x41\x02R\x07partyId"\xc4\x01\n\rSpamStatistic\x12&\n\x0f\x63ount_for_epoch\x18\x01 \x01(\x04R\rcountForEpoch\x12"\n\rmax_for_epoch\x18\x02 \x01(\x04R\x0bmaxForEpoch\x12&\n\x0c\x62\x61nned_until\x18\x04 \x01(\tH\x00R\x0b\x62\x61nnedUntil\x88\x01\x01\x12.\n\x13min_tokens_required\x18\x05 \x01(\tR\x11minTokensRequiredB\x0f\n\r_banned_until"\xb1\x01\n\x12VoteSpamStatistics\x12>\n\nstatistics\x18\x01 \x03(\x0b\x32\x1e.vega.api.v1.VoteSpamStatisticR\nstatistics\x12"\n\rmax_for_epoch\x18\x02 \x01(\x04R\x0bmaxForEpoch\x12&\n\x0c\x62\x61nned_until\x18\x03 \x01(\tH\x00R\x0b\x62\x61nnedUntil\x88\x01\x01\x42\x0f\n\r_banned_until"\x87\x01\n\x11VoteSpamStatistic\x12\x1a\n\x08proposal\x18\x01 \x01(\tR\x08proposal\x12&\n\x0f\x63ount_for_epoch\x18\x02 \x01(\x04R\rcountForEpoch\x12.\n\x13min_tokens_required\x18\x03 \x01(\tR\x11minTokensRequired"\xe8\x02\n\rPoWBlockState\x12!\n\x0c\x62lock_height\x18\x01 \x01(\x04R\x0b\x62lockHeight\x12\x1d\n\nblock_hash\x18\x02 \x01(\tR\tblockHash\x12+\n\x11transactions_seen\x18\x03 \x01(\x04R\x10transactionsSeen\x12\x34\n\x13\x65xpected_difficulty\x18\x04 \x01(\x04H\x00R\x12\x65xpectedDifficulty\x88\x01\x01\x12#\n\rhash_function\x18\x05 \x01(\tR\x0chashFunction\x12\x1e\n\ndifficulty\x18\x06 \x01(\x04R\ndifficulty\x12 \n\x0ctx_per_block\x18\x07 \x01(\x04R\ntxPerBlock\x12\x33\n\x15increasing_difficulty\x18\x08 \x01(\x08R\x14increasingDifficultyB\x16\n\x14_expected_difficulty"\xb9\x01\n\x0cPoWStatistic\x12=\n\x0c\x62lock_states\x18\x01 \x03(\x0b\x32\x1a.vega.api.v1.PoWBlockStateR\x0b\x62lockStates\x12&\n\x0c\x62\x61nned_until\x18\x02 \x01(\tH\x00R\x0b\x62\x61nnedUntil\x88\x01\x01\x12\x31\n\x15number_of_past_blocks\x18\x03 \x01(\x04R\x12numberOfPastBlocksB\x0f\n\r_banned_until"\xd5\x03\n\x0eSpamStatistics\x12\x38\n\tproposals\x18\x01 \x01(\x0b\x32\x1a.vega.api.v1.SpamStatisticR\tproposals\x12<\n\x0b\x64\x65legations\x18\x02 \x01(\x0b\x32\x1a.vega.api.v1.SpamStatisticR\x0b\x64\x65legations\x12\x38\n\ttransfers\x18\x03 \x01(\x0b\x32\x1a.vega.api.v1.SpamStatisticR\ttransfers\x12I\n\x12node_announcements\x18\x04 \x01(\x0b\x32\x1a.vega.api.v1.SpamStatisticR\x11nodeAnnouncements\x12\x35\n\x05votes\x18\x05 \x01(\x0b\x32\x1f.vega.api.v1.VoteSpamStatisticsR\x05votes\x12+\n\x03pow\x18\x06 \x01(\x0b\x32\x19.vega.api.v1.PoWStatisticR\x03pow\x12\x45\n\x10issue_signatures\x18\x07 \x01(\x0b\x32\x1a.vega.api.v1.SpamStatisticR\x0fissueSignatures\x12\x1b\n\tepoch_seq\x18\x08 \x01(\x04R\x08\x65pochSeq"s\n\x19GetSpamStatisticsResponse\x12\x19\n\x08\x63hain_id\x18\x01 \x01(\tR\x07\x63hainId\x12;\n\nstatistics\x18\x02 \x01(\x0b\x32\x1b.vega.api.v1.SpamStatisticsR\nstatistics2\xd8\x07\n\x0b\x43oreService\x12\x62\n\x11SubmitTransaction\x12%.vega.api.v1.SubmitTransactionRequest\x1a&.vega.api.v1.SubmitTransactionResponse\x12h\n\x13PropagateChainEvent\x12\'.vega.api.v1.PropagateChainEventRequest\x1a(.vega.api.v1.PropagateChainEventResponse\x12M\n\nStatistics\x12\x1e.vega.api.v1.StatisticsRequest\x1a\x1f.vega.api.v1.StatisticsResponse\x12\\\n\x0fLastBlockHeight\x12#.vega.api.v1.LastBlockHeightRequest\x1a$.vega.api.v1.LastBlockHeightResponse\x12P\n\x0bGetVegaTime\x12\x1f.vega.api.v1.GetVegaTimeRequest\x1a .vega.api.v1.GetVegaTimeResponse\x12`\n\x0fObserveEventBus\x12#.vega.api.v1.ObserveEventBusRequest\x1a$.vega.api.v1.ObserveEventBusResponse(\x01\x30\x01\x12k\n\x14SubmitRawTransaction\x12(.vega.api.v1.SubmitRawTransactionRequest\x1a).vega.api.v1.SubmitRawTransactionResponse\x12_\n\x10\x43heckTransaction\x12$.vega.api.v1.CheckTransactionRequest\x1a%.vega.api.v1.CheckTransactionResponse\x12h\n\x13\x43heckRawTransaction\x12\'.vega.api.v1.CheckRawTransactionRequest\x1a(.vega.api.v1.CheckRawTransactionResponse\x12\x62\n\x11GetSpamStatistics\x12%.vega.api.v1.GetSpamStatisticsRequest\x1a&.vega.api.v1.GetSpamStatisticsResponseBeZ,code.vegaprotocol.io/vega/protos/vega/api/v1\x92\x41\x34\x12\x19\n\x0eVega core APIs2\x07v0.71.4\x1a\x13lb.testnet.vega.xyz*\x02\x01\x02\x62\x06proto3'
+    b'\n\x16vega/api/v1/core.proto\x12\x0bvega.api.v1\x1a\x1fgoogle/api/field_behavior.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\x1a"vega/commands/v1/transaction.proto\x1a\x1bvega/events/v1/events.proto\x1a\x0fvega/vega.proto"{\n\x1aPropagateChainEventRequest\x12\x1a\n\x05\x65vent\x18\x01 \x01(\x0c\x42\x04\xe2\x41\x01\x02R\x05\x65vent\x12\x1d\n\x07pub_key\x18\x02 \x01(\tB\x04\xe2\x41\x01\x02R\x06pubKey\x12"\n\tsignature\x18\x03 \x01(\x0c\x42\x04\xe2\x41\x01\x02R\tsignature"7\n\x1bPropagateChainEventResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success"\xe3\x01\n\x18SubmitTransactionRequest\x12\x33\n\x02tx\x18\x01 \x01(\x0b\x32\x1d.vega.commands.v1.TransactionB\x04\xe2\x41\x01\x02R\x02tx\x12\x44\n\x04type\x18\x02 \x01(\x0e\x32*.vega.api.v1.SubmitTransactionRequest.TypeB\x04\xe2\x41\x01\x02R\x04type"L\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x0e\n\nTYPE_ASYNC\x10\x01\x12\r\n\tTYPE_SYNC\x10\x02\x12\x0f\n\x0bTYPE_COMMIT\x10\x03"\xa0\x01\n\x19SubmitTransactionResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12\x17\n\x07tx_hash\x18\x02 \x01(\tR\x06txHash\x12\x12\n\x04\x63ode\x18\x03 \x01(\rR\x04\x63ode\x12\x12\n\x04\x64\x61ta\x18\x04 \x01(\tR\x04\x64\x61ta\x12\x10\n\x03log\x18\x05 \x01(\tR\x03log\x12\x16\n\x06height\x18\x06 \x01(\x03R\x06height"N\n\x17\x43heckTransactionRequest\x12\x33\n\x02tx\x18\x01 \x01(\x0b\x32\x1d.vega.commands.v1.TransactionB\x04\xe2\x41\x01\x02R\x02tx"\xbc\x01\n\x18\x43heckTransactionResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12\x12\n\x04\x63ode\x18\x02 \x01(\rR\x04\x63ode\x12\x1d\n\ngas_wanted\x18\x03 \x01(\x03R\tgasWanted\x12\x19\n\x08gas_used\x18\x04 \x01(\x03R\x07gasUsed\x12\x12\n\x04\x64\x61ta\x18\x05 \x01(\tR\x04\x64\x61ta\x12\x10\n\x03log\x18\x06 \x01(\tR\x03log\x12\x12\n\x04info\x18\x07 \x01(\tR\x04info"\xca\x01\n\x1bSubmitRawTransactionRequest\x12\x14\n\x02tx\x18\x01 \x01(\x0c\x42\x04\xe2\x41\x01\x02R\x02tx\x12G\n\x04type\x18\x02 \x01(\x0e\x32-.vega.api.v1.SubmitRawTransactionRequest.TypeB\x04\xe2\x41\x01\x02R\x04type"L\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x0e\n\nTYPE_ASYNC\x10\x01\x12\r\n\tTYPE_SYNC\x10\x02\x12\x0f\n\x0bTYPE_COMMIT\x10\x03"\xa3\x01\n\x1cSubmitRawTransactionResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12\x17\n\x07tx_hash\x18\x02 \x01(\tR\x06txHash\x12\x12\n\x04\x63ode\x18\x03 \x01(\rR\x04\x63ode\x12\x12\n\x04\x64\x61ta\x18\x04 \x01(\tR\x04\x64\x61ta\x12\x10\n\x03log\x18\x05 \x01(\tR\x03log\x12\x16\n\x06height\x18\x06 \x01(\x03R\x06height"2\n\x1a\x43heckRawTransactionRequest\x12\x14\n\x02tx\x18\x01 \x01(\x0c\x42\x04\xe2\x41\x01\x02R\x02tx"\xbf\x01\n\x1b\x43heckRawTransactionResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12\x12\n\x04\x63ode\x18\x02 \x01(\rR\x04\x63ode\x12\x1d\n\ngas_wanted\x18\x03 \x01(\x03R\tgasWanted\x12\x19\n\x08gas_used\x18\x04 \x01(\x03R\x07gasUsed\x12\x12\n\x04\x64\x61ta\x18\x05 \x01(\tR\x04\x64\x61ta\x12\x10\n\x03log\x18\x06 \x01(\tR\x03log\x12\x12\n\x04info\x18\x07 \x01(\tR\x04info"\x14\n\x12GetVegaTimeRequest"3\n\x13GetVegaTimeResponse\x12\x1c\n\ttimestamp\x18\x01 \x01(\x03R\ttimestamp"\xa1\x01\n\x16ObserveEventBusRequest\x12\x30\n\x04type\x18\x01 \x03(\x0e\x32\x1c.vega.events.v1.BusEventTypeR\x04type\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x03 \x01(\tR\x07partyId\x12\x1d\n\nbatch_size\x18\x04 \x01(\x03R\tbatchSize"K\n\x17ObserveEventBusResponse\x12\x30\n\x06\x65vents\x18\x01 \x03(\x0b\x32\x18.vega.events.v1.BusEventR\x06\x65vents"\x13\n\x11StatisticsRequest"M\n\x12StatisticsResponse\x12\x37\n\nstatistics\x18\x01 \x01(\x0b\x32\x17.vega.api.v1.StatisticsR\nstatistics"\xc8\x0c\n\nStatistics\x12!\n\x0c\x62lock_height\x18\x01 \x01(\x04R\x0b\x62lockHeight\x12%\n\x0e\x62\x61\x63klog_length\x18\x02 \x01(\x04R\rbacklogLength\x12\x1f\n\x0btotal_peers\x18\x03 \x01(\x04R\ntotalPeers\x12!\n\x0cgenesis_time\x18\x04 \x01(\tR\x0bgenesisTime\x12!\n\x0c\x63urrent_time\x18\x05 \x01(\tR\x0b\x63urrentTime\x12\x1b\n\tvega_time\x18\x06 \x01(\tR\x08vegaTime\x12)\n\x06status\x18\x07 \x01(\x0e\x32\x11.vega.ChainStatusR\x06status\x12 \n\x0ctx_per_block\x18\x08 \x01(\x04R\ntxPerBlock\x12(\n\x10\x61verage_tx_bytes\x18\t \x01(\x04R\x0e\x61verageTxBytes\x12\x37\n\x18\x61verage_orders_per_block\x18\n \x01(\x04R\x15\x61verageOrdersPerBlock\x12*\n\x11trades_per_second\x18\x0b \x01(\x04R\x0ftradesPerSecond\x12*\n\x11orders_per_second\x18\x0c \x01(\x04R\x0fordersPerSecond\x12#\n\rtotal_markets\x18\r \x01(\x04R\x0ctotalMarkets\x12*\n\x11total_amend_order\x18\x10 \x01(\x04R\x0ftotalAmendOrder\x12,\n\x12total_cancel_order\x18\x11 \x01(\x04R\x10totalCancelOrder\x12,\n\x12total_create_order\x18\x12 \x01(\x04R\x10totalCreateOrder\x12!\n\x0ctotal_orders\x18\x13 \x01(\x04R\x0btotalOrders\x12!\n\x0ctotal_trades\x18\x14 \x01(\x04R\x0btotalTrades\x12/\n\x13order_subscriptions\x18\x15 \x01(\rR\x12orderSubscriptions\x12/\n\x13trade_subscriptions\x18\x16 \x01(\rR\x12tradeSubscriptions\x12\x31\n\x14\x63\x61ndle_subscriptions\x18\x17 \x01(\rR\x13\x63\x61ndleSubscriptions\x12<\n\x1amarket_depth_subscriptions\x18\x18 \x01(\rR\x18marketDepthSubscriptions\x12\x37\n\x17positions_subscriptions\x18\x19 \x01(\rR\x16positionsSubscriptions\x12\x33\n\x15\x61\x63\x63ount_subscriptions\x18\x1a \x01(\rR\x14\x61\x63\x63ountSubscriptions\x12:\n\x19market_data_subscriptions\x18\x1b \x01(\rR\x17marketDataSubscriptions\x12(\n\x10\x61pp_version_hash\x18\x1c \x01(\tR\x0e\x61ppVersionHash\x12\x1f\n\x0b\x61pp_version\x18\x1d \x01(\tR\nappVersion\x12#\n\rchain_version\x18\x1e \x01(\tR\x0c\x63hainVersion\x12%\n\x0e\x62lock_duration\x18\x1f \x01(\x04R\rblockDuration\x12\x16\n\x06uptime\x18  \x01(\tR\x06uptime\x12\x19\n\x08\x63hain_id\x18! \x01(\tR\x07\x63hainId\x12K\n"market_depth_updates_subscriptions\x18" \x01(\rR\x1fmarketDepthUpdatesSubscriptions\x12\x1d\n\nblock_hash\x18# \x01(\tR\tblockHash\x12\x1b\n\tepoch_seq\x18$ \x01(\x04R\x08\x65pochSeq\x12(\n\x10\x65poch_start_time\x18% \x01(\tR\x0e\x65pochStartTime\x12*\n\x11\x65poch_expiry_time\x18& \x01(\tR\x0f\x65pochExpiryTime\x12\x1f\n\x0b\x65vent_count\x18\' \x01(\x04R\neventCount\x12*\n\x11\x65vents_per_second\x18( \x01(\x04R\x0f\x65ventsPerSecond"\x18\n\x16LastBlockHeightRequest"\x91\x03\n\x17LastBlockHeightResponse\x12\x16\n\x06height\x18\x01 \x01(\x04R\x06height\x12\x12\n\x04hash\x18\x02 \x01(\tR\x04hash\x12\x33\n\x16spam_pow_hash_function\x18\x03 \x01(\tR\x13spamPowHashFunction\x12.\n\x13spam_pow_difficulty\x18\x04 \x01(\rR\x11spamPowDifficulty\x12\x41\n\x1espam_pow_number_of_past_blocks\x18\x05 \x01(\rR\x19spamPowNumberOfPastBlocks\x12\x42\n\x1fspam_pow_number_of_tx_per_block\x18\x06 \x01(\rR\x19spamPowNumberOfTxPerBlock\x12\x43\n\x1espam_pow_increasing_difficulty\x18\x07 \x01(\x08R\x1bspamPowIncreasingDifficulty\x12\x19\n\x08\x63hain_id\x18\x08 \x01(\tR\x07\x63hainId";\n\x18GetSpamStatisticsRequest\x12\x1f\n\x08party_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02R\x07partyId"\xc4\x01\n\rSpamStatistic\x12&\n\x0f\x63ount_for_epoch\x18\x01 \x01(\x04R\rcountForEpoch\x12"\n\rmax_for_epoch\x18\x02 \x01(\x04R\x0bmaxForEpoch\x12&\n\x0c\x62\x61nned_until\x18\x04 \x01(\tH\x00R\x0b\x62\x61nnedUntil\x88\x01\x01\x12.\n\x13min_tokens_required\x18\x05 \x01(\tR\x11minTokensRequiredB\x0f\n\r_banned_until"\xb1\x01\n\x12VoteSpamStatistics\x12>\n\nstatistics\x18\x01 \x03(\x0b\x32\x1e.vega.api.v1.VoteSpamStatisticR\nstatistics\x12"\n\rmax_for_epoch\x18\x02 \x01(\x04R\x0bmaxForEpoch\x12&\n\x0c\x62\x61nned_until\x18\x03 \x01(\tH\x00R\x0b\x62\x61nnedUntil\x88\x01\x01\x42\x0f\n\r_banned_until"\x87\x01\n\x11VoteSpamStatistic\x12\x1a\n\x08proposal\x18\x01 \x01(\tR\x08proposal\x12&\n\x0f\x63ount_for_epoch\x18\x02 \x01(\x04R\rcountForEpoch\x12.\n\x13min_tokens_required\x18\x03 \x01(\tR\x11minTokensRequired"\xe8\x02\n\rPoWBlockState\x12!\n\x0c\x62lock_height\x18\x01 \x01(\x04R\x0b\x62lockHeight\x12\x1d\n\nblock_hash\x18\x02 \x01(\tR\tblockHash\x12+\n\x11transactions_seen\x18\x03 \x01(\x04R\x10transactionsSeen\x12\x34\n\x13\x65xpected_difficulty\x18\x04 \x01(\x04H\x00R\x12\x65xpectedDifficulty\x88\x01\x01\x12#\n\rhash_function\x18\x05 \x01(\tR\x0chashFunction\x12\x1e\n\ndifficulty\x18\x06 \x01(\x04R\ndifficulty\x12 \n\x0ctx_per_block\x18\x07 \x01(\x04R\ntxPerBlock\x12\x33\n\x15increasing_difficulty\x18\x08 \x01(\x08R\x14increasingDifficultyB\x16\n\x14_expected_difficulty"\xb9\x01\n\x0cPoWStatistic\x12=\n\x0c\x62lock_states\x18\x01 \x03(\x0b\x32\x1a.vega.api.v1.PoWBlockStateR\x0b\x62lockStates\x12&\n\x0c\x62\x61nned_until\x18\x02 \x01(\tH\x00R\x0b\x62\x61nnedUntil\x88\x01\x01\x12\x31\n\x15number_of_past_blocks\x18\x03 \x01(\x04R\x12numberOfPastBlocksB\x0f\n\r_banned_until"\xd5\x03\n\x0eSpamStatistics\x12\x38\n\tproposals\x18\x01 \x01(\x0b\x32\x1a.vega.api.v1.SpamStatisticR\tproposals\x12<\n\x0b\x64\x65legations\x18\x02 \x01(\x0b\x32\x1a.vega.api.v1.SpamStatisticR\x0b\x64\x65legations\x12\x38\n\ttransfers\x18\x03 \x01(\x0b\x32\x1a.vega.api.v1.SpamStatisticR\ttransfers\x12I\n\x12node_announcements\x18\x04 \x01(\x0b\x32\x1a.vega.api.v1.SpamStatisticR\x11nodeAnnouncements\x12\x35\n\x05votes\x18\x05 \x01(\x0b\x32\x1f.vega.api.v1.VoteSpamStatisticsR\x05votes\x12+\n\x03pow\x18\x06 \x01(\x0b\x32\x19.vega.api.v1.PoWStatisticR\x03pow\x12\x45\n\x10issue_signatures\x18\x07 \x01(\x0b\x32\x1a.vega.api.v1.SpamStatisticR\x0fissueSignatures\x12\x1b\n\tepoch_seq\x18\x08 \x01(\x04R\x08\x65pochSeq"s\n\x19GetSpamStatisticsResponse\x12\x19\n\x08\x63hain_id\x18\x01 \x01(\tR\x07\x63hainId\x12;\n\nstatistics\x18\x02 \x01(\x0b\x32\x1b.vega.api.v1.SpamStatisticsR\nstatistics2\xd8\x07\n\x0b\x43oreService\x12\x62\n\x11SubmitTransaction\x12%.vega.api.v1.SubmitTransactionRequest\x1a&.vega.api.v1.SubmitTransactionResponse\x12h\n\x13PropagateChainEvent\x12\'.vega.api.v1.PropagateChainEventRequest\x1a(.vega.api.v1.PropagateChainEventResponse\x12M\n\nStatistics\x12\x1e.vega.api.v1.StatisticsRequest\x1a\x1f.vega.api.v1.StatisticsResponse\x12\\\n\x0fLastBlockHeight\x12#.vega.api.v1.LastBlockHeightRequest\x1a$.vega.api.v1.LastBlockHeightResponse\x12P\n\x0bGetVegaTime\x12\x1f.vega.api.v1.GetVegaTimeRequest\x1a .vega.api.v1.GetVegaTimeResponse\x12`\n\x0fObserveEventBus\x12#.vega.api.v1.ObserveEventBusRequest\x1a$.vega.api.v1.ObserveEventBusResponse(\x01\x30\x01\x12k\n\x14SubmitRawTransaction\x12(.vega.api.v1.SubmitRawTransactionRequest\x1a).vega.api.v1.SubmitRawTransactionResponse\x12_\n\x10\x43heckTransaction\x12$.vega.api.v1.CheckTransactionRequest\x1a%.vega.api.v1.CheckTransactionResponse\x12h\n\x13\x43heckRawTransaction\x12\'.vega.api.v1.CheckRawTransactionRequest\x1a(.vega.api.v1.CheckRawTransactionResponse\x12\x62\n\x11GetSpamStatistics\x12%.vega.api.v1.GetSpamStatisticsRequest\x1a&.vega.api.v1.GetSpamStatisticsResponseBeZ,code.vegaprotocol.io/vega/protos/vega/api/v1\x92\x41\x34\x12\x19\n\x0eVega core APIs2\x07v0.71.0\x1a\x13lb.testnet.vega.xyz*\x02\x01\x02\x62\x06proto3'
 )
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "vega.api.v1.core_pb2", globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "vega.api.v1.core_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    DESCRIPTOR._serialized_options = b"Z,code.vegaprotocol.io/vega/protos/vega/api/v1\222A4\022\031\n\016Vega core APIs2\007v0.71.4\032\023lb.testnet.vega.xyz*\002\001\002"
+    DESCRIPTOR._serialized_options = b"Z,code.vegaprotocol.io/vega/protos/vega/api/v1\222A4\022\031\n\016Vega core APIs2\007v0.71.0\032\023lb.testnet.vega.xyz*\002\001\002"
     _PROPAGATECHAINEVENTREQUEST.fields_by_name["event"]._options = None
     _PROPAGATECHAINEVENTREQUEST.fields_by_name[
         "event"
-    ]._serialized_options = b"\340A\002"
+    ]._serialized_options = b"\342A\001\002"
     _PROPAGATECHAINEVENTREQUEST.fields_by_name["pub_key"]._options = None
     _PROPAGATECHAINEVENTREQUEST.fields_by_name[
         "pub_key"
-    ]._serialized_options = b"\340A\002"
+    ]._serialized_options = b"\342A\001\002"
     _PROPAGATECHAINEVENTREQUEST.fields_by_name["signature"]._options = None
     _PROPAGATECHAINEVENTREQUEST.fields_by_name[
         "signature"
-    ]._serialized_options = b"\340A\002"
+    ]._serialized_options = b"\342A\001\002"
     _SUBMITTRANSACTIONREQUEST.fields_by_name["tx"]._options = None
-    _SUBMITTRANSACTIONREQUEST.fields_by_name["tx"]._serialized_options = b"\340A\002"
+    _SUBMITTRANSACTIONREQUEST.fields_by_name[
+        "tx"
+    ]._serialized_options = b"\342A\001\002"
     _SUBMITTRANSACTIONREQUEST.fields_by_name["type"]._options = None
-    _SUBMITTRANSACTIONREQUEST.fields_by_name["type"]._serialized_options = b"\340A\002"
+    _SUBMITTRANSACTIONREQUEST.fields_by_name[
+        "type"
+    ]._serialized_options = b"\342A\001\002"
     _CHECKTRANSACTIONREQUEST.fields_by_name["tx"]._options = None
-    _CHECKTRANSACTIONREQUEST.fields_by_name["tx"]._serialized_options = b"\340A\002"
+    _CHECKTRANSACTIONREQUEST.fields_by_name["tx"]._serialized_options = b"\342A\001\002"
     _SUBMITRAWTRANSACTIONREQUEST.fields_by_name["tx"]._options = None
-    _SUBMITRAWTRANSACTIONREQUEST.fields_by_name["tx"]._serialized_options = b"\340A\002"
+    _SUBMITRAWTRANSACTIONREQUEST.fields_by_name[
+        "tx"
+    ]._serialized_options = b"\342A\001\002"
     _SUBMITRAWTRANSACTIONREQUEST.fields_by_name["type"]._options = None
     _SUBMITRAWTRANSACTIONREQUEST.fields_by_name[
         "type"
-    ]._serialized_options = b"\340A\002"
+    ]._serialized_options = b"\342A\001\002"
     _CHECKRAWTRANSACTIONREQUEST.fields_by_name["tx"]._options = None
-    _CHECKRAWTRANSACTIONREQUEST.fields_by_name["tx"]._serialized_options = b"\340A\002"
+    _CHECKRAWTRANSACTIONREQUEST.fields_by_name[
+        "tx"
+    ]._serialized_options = b"\342A\001\002"
     _GETSPAMSTATISTICSREQUEST.fields_by_name["party_id"]._options = None
     _GETSPAMSTATISTICSREQUEST.fields_by_name[
         "party_id"
-    ]._serialized_options = b"\340A\002"
-    _PROPAGATECHAINEVENTREQUEST._serialized_start = 202
-    _PROPAGATECHAINEVENTREQUEST._serialized_end = 322
-    _PROPAGATECHAINEVENTRESPONSE._serialized_start = 324
-    _PROPAGATECHAINEVENTRESPONSE._serialized_end = 379
-    _SUBMITTRANSACTIONREQUEST._serialized_start = 382
-    _SUBMITTRANSACTIONREQUEST._serialized_end = 607
-    _SUBMITTRANSACTIONREQUEST_TYPE._serialized_start = 531
-    _SUBMITTRANSACTIONREQUEST_TYPE._serialized_end = 607
-    _SUBMITTRANSACTIONRESPONSE._serialized_start = 610
-    _SUBMITTRANSACTIONRESPONSE._serialized_end = 770
-    _CHECKTRANSACTIONREQUEST._serialized_start = 772
-    _CHECKTRANSACTIONREQUEST._serialized_end = 849
-    _CHECKTRANSACTIONRESPONSE._serialized_start = 852
-    _CHECKTRANSACTIONRESPONSE._serialized_end = 1040
-    _SUBMITRAWTRANSACTIONREQUEST._serialized_start = 1043
-    _SUBMITRAWTRANSACTIONREQUEST._serialized_end = 1243
-    _SUBMITRAWTRANSACTIONREQUEST_TYPE._serialized_start = 531
-    _SUBMITRAWTRANSACTIONREQUEST_TYPE._serialized_end = 607
-    _SUBMITRAWTRANSACTIONRESPONSE._serialized_start = 1246
-    _SUBMITRAWTRANSACTIONRESPONSE._serialized_end = 1409
-    _CHECKRAWTRANSACTIONREQUEST._serialized_start = 1411
-    _CHECKRAWTRANSACTIONREQUEST._serialized_end = 1460
-    _CHECKRAWTRANSACTIONRESPONSE._serialized_start = 1463
-    _CHECKRAWTRANSACTIONRESPONSE._serialized_end = 1654
-    _GETVEGATIMEREQUEST._serialized_start = 1656
-    _GETVEGATIMEREQUEST._serialized_end = 1676
-    _GETVEGATIMERESPONSE._serialized_start = 1678
-    _GETVEGATIMERESPONSE._serialized_end = 1729
-    _OBSERVEEVENTBUSREQUEST._serialized_start = 1732
-    _OBSERVEEVENTBUSREQUEST._serialized_end = 1893
-    _OBSERVEEVENTBUSRESPONSE._serialized_start = 1895
-    _OBSERVEEVENTBUSRESPONSE._serialized_end = 1970
-    _STATISTICSREQUEST._serialized_start = 1972
-    _STATISTICSREQUEST._serialized_end = 1991
-    _STATISTICSRESPONSE._serialized_start = 1993
-    _STATISTICSRESPONSE._serialized_end = 2070
-    _STATISTICS._serialized_start = 2073
-    _STATISTICS._serialized_end = 3681
-    _LASTBLOCKHEIGHTREQUEST._serialized_start = 3683
-    _LASTBLOCKHEIGHTREQUEST._serialized_end = 3707
-    _LASTBLOCKHEIGHTRESPONSE._serialized_start = 3710
-    _LASTBLOCKHEIGHTRESPONSE._serialized_end = 4111
-    _GETSPAMSTATISTICSREQUEST._serialized_start = 4113
-    _GETSPAMSTATISTICSREQUEST._serialized_end = 4171
-    _SPAMSTATISTIC._serialized_start = 4174
-    _SPAMSTATISTIC._serialized_end = 4370
-    _VOTESPAMSTATISTICS._serialized_start = 4373
-    _VOTESPAMSTATISTICS._serialized_end = 4550
-    _VOTESPAMSTATISTIC._serialized_start = 4553
-    _VOTESPAMSTATISTIC._serialized_end = 4688
-    _POWBLOCKSTATE._serialized_start = 4691
-    _POWBLOCKSTATE._serialized_end = 5051
-    _POWSTATISTIC._serialized_start = 5054
-    _POWSTATISTIC._serialized_end = 5239
-    _SPAMSTATISTICS._serialized_start = 5242
-    _SPAMSTATISTICS._serialized_end = 5711
-    _GETSPAMSTATISTICSRESPONSE._serialized_start = 5713
-    _GETSPAMSTATISTICSRESPONSE._serialized_end = 5828
-    _CORESERVICE._serialized_start = 5831
-    _CORESERVICE._serialized_end = 6815
+    ]._serialized_options = b"\342A\001\002"
+    _globals["_PROPAGATECHAINEVENTREQUEST"]._serialized_start = 202
+    _globals["_PROPAGATECHAINEVENTREQUEST"]._serialized_end = 325
+    _globals["_PROPAGATECHAINEVENTRESPONSE"]._serialized_start = 327
+    _globals["_PROPAGATECHAINEVENTRESPONSE"]._serialized_end = 382
+    _globals["_SUBMITTRANSACTIONREQUEST"]._serialized_start = 385
+    _globals["_SUBMITTRANSACTIONREQUEST"]._serialized_end = 612
+    _globals["_SUBMITTRANSACTIONREQUEST_TYPE"]._serialized_start = 536
+    _globals["_SUBMITTRANSACTIONREQUEST_TYPE"]._serialized_end = 612
+    _globals["_SUBMITTRANSACTIONRESPONSE"]._serialized_start = 615
+    _globals["_SUBMITTRANSACTIONRESPONSE"]._serialized_end = 775
+    _globals["_CHECKTRANSACTIONREQUEST"]._serialized_start = 777
+    _globals["_CHECKTRANSACTIONREQUEST"]._serialized_end = 855
+    _globals["_CHECKTRANSACTIONRESPONSE"]._serialized_start = 858
+    _globals["_CHECKTRANSACTIONRESPONSE"]._serialized_end = 1046
+    _globals["_SUBMITRAWTRANSACTIONREQUEST"]._serialized_start = 1049
+    _globals["_SUBMITRAWTRANSACTIONREQUEST"]._serialized_end = 1251
+    _globals["_SUBMITRAWTRANSACTIONREQUEST_TYPE"]._serialized_start = 536
+    _globals["_SUBMITRAWTRANSACTIONREQUEST_TYPE"]._serialized_end = 612
+    _globals["_SUBMITRAWTRANSACTIONRESPONSE"]._serialized_start = 1254
+    _globals["_SUBMITRAWTRANSACTIONRESPONSE"]._serialized_end = 1417
+    _globals["_CHECKRAWTRANSACTIONREQUEST"]._serialized_start = 1419
+    _globals["_CHECKRAWTRANSACTIONREQUEST"]._serialized_end = 1469
+    _globals["_CHECKRAWTRANSACTIONRESPONSE"]._serialized_start = 1472
+    _globals["_CHECKRAWTRANSACTIONRESPONSE"]._serialized_end = 1663
+    _globals["_GETVEGATIMEREQUEST"]._serialized_start = 1665
+    _globals["_GETVEGATIMEREQUEST"]._serialized_end = 1685
+    _globals["_GETVEGATIMERESPONSE"]._serialized_start = 1687
+    _globals["_GETVEGATIMERESPONSE"]._serialized_end = 1738
+    _globals["_OBSERVEEVENTBUSREQUEST"]._serialized_start = 1741
+    _globals["_OBSERVEEVENTBUSREQUEST"]._serialized_end = 1902
+    _globals["_OBSERVEEVENTBUSRESPONSE"]._serialized_start = 1904
+    _globals["_OBSERVEEVENTBUSRESPONSE"]._serialized_end = 1979
+    _globals["_STATISTICSREQUEST"]._serialized_start = 1981
+    _globals["_STATISTICSREQUEST"]._serialized_end = 2000
+    _globals["_STATISTICSRESPONSE"]._serialized_start = 2002
+    _globals["_STATISTICSRESPONSE"]._serialized_end = 2079
+    _globals["_STATISTICS"]._serialized_start = 2082
+    _globals["_STATISTICS"]._serialized_end = 3690
+    _globals["_LASTBLOCKHEIGHTREQUEST"]._serialized_start = 3692
+    _globals["_LASTBLOCKHEIGHTREQUEST"]._serialized_end = 3716
+    _globals["_LASTBLOCKHEIGHTRESPONSE"]._serialized_start = 3719
+    _globals["_LASTBLOCKHEIGHTRESPONSE"]._serialized_end = 4120
+    _globals["_GETSPAMSTATISTICSREQUEST"]._serialized_start = 4122
+    _globals["_GETSPAMSTATISTICSREQUEST"]._serialized_end = 4181
+    _globals["_SPAMSTATISTIC"]._serialized_start = 4184
+    _globals["_SPAMSTATISTIC"]._serialized_end = 4380
+    _globals["_VOTESPAMSTATISTICS"]._serialized_start = 4383
+    _globals["_VOTESPAMSTATISTICS"]._serialized_end = 4560
+    _globals["_VOTESPAMSTATISTIC"]._serialized_start = 4563
+    _globals["_VOTESPAMSTATISTIC"]._serialized_end = 4698
+    _globals["_POWBLOCKSTATE"]._serialized_start = 4701
+    _globals["_POWBLOCKSTATE"]._serialized_end = 5061
+    _globals["_POWSTATISTIC"]._serialized_start = 5064
+    _globals["_POWSTATISTIC"]._serialized_end = 5249
+    _globals["_SPAMSTATISTICS"]._serialized_start = 5252
+    _globals["_SPAMSTATISTICS"]._serialized_end = 5721
+    _globals["_GETSPAMSTATISTICSRESPONSE"]._serialized_start = 5723
+    _globals["_GETSPAMSTATISTICSRESPONSE"]._serialized_end = 5838
+    _globals["_CORESERVICE"]._serialized_start = 5841
+    _globals["_CORESERVICE"]._serialized_end = 6825
 # @@protoc_insertion_point(module_scope)
```

### Comparing `vega_sim-1.1.1/vega_sim/proto/vega/api/v1/core_pb2_grpc.py` & `vega_sim-1.2.0/vega_sim/proto/vega/api/v1/core_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/proto/vega/api/v1/corestate_pb2.py` & `vega_sim-1.2.0/vega_sim/proto/vega/api/v1/corestate_pb2.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: vega/api/v1/corestate.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from protoc_gen_openapiv2.options import (
@@ -19,72 +19,73 @@
 from ...events.v1 import events_pb2 as vega_dot_events_dot_v1_dot_events__pb2
 from ... import governance_pb2 as vega_dot_governance__pb2
 from ... import markets_pb2 as vega_dot_markets__pb2
 from ... import vega_pb2 as vega_dot_vega__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x1bvega/api/v1/corestate.proto\x12\x0bvega.api.v1\x1a.protoc-gen-openapiv2/options/annotations.proto\x1a\x11vega/assets.proto\x1a\x1bvega/events/v1/events.proto\x1a\x15vega/governance.proto\x1a\x12vega/markets.proto\x1a\x0fvega/vega.proto"{\n\x07\x41\x63\x63ount\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x16\n\x06market\x18\x02 \x01(\tR\x06market\x12\x18\n\x07\x62\x61lance\x18\x03 \x01(\tR\x07\x62\x61lance\x12\x14\n\x05\x61sset\x18\x05 \x01(\tR\x05\x61sset\x12\x12\n\x04type\x18\x06 \x01(\tR\x04type"C\n\x13ListAccountsRequest\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x16\n\x06market\x18\x02 \x01(\tR\x06market"H\n\x14ListAccountsResponse\x12\x30\n\x08\x61\x63\x63ounts\x18\x01 \x03(\x0b\x32\x14.vega.api.v1.AccountR\x08\x61\x63\x63ounts")\n\x11ListAssetsRequest\x12\x14\n\x05\x61sset\x18\x01 \x01(\tR\x05\x61sset"9\n\x12ListAssetsResponse\x12#\n\x06\x61ssets\x18\x01 \x03(\x0b\x32\x0b.vega.AssetR\x06\x61ssets"R\n\x1cListNetworkParametersRequest\x12\x32\n\x15network_parameter_key\x18\x01 \x01(\tR\x13networkParameterKey"f\n\x1dListNetworkParametersResponse\x12\x45\n\x12network_parameters\x18\x01 \x03(\x0b\x32\x16.vega.NetworkParameterR\x11networkParameters"\x1a\n\x18ListNetworkLimitsRequest"W\n\x19ListNetworkLimitsResponse\x12:\n\x0enetwork_limits\x18\x01 \x01(\x0b\x32\x13.vega.NetworkLimitsR\rnetworkLimits"\x14\n\x12ListPartiesRequest"<\n\x13ListPartiesResponse\x12%\n\x07parties\x18\x01 \x03(\x0b\x32\x0b.vega.PartyR\x07parties"\x17\n\x15ListValidatorsRequest"Y\n\x16ListValidatorsResponse\x12?\n\nvalidators\x18\x01 \x03(\x0b\x32\x1f.vega.events.v1.ValidatorUpdateR\nvalidators",\n\x12ListMarketsRequest\x12\x16\n\x06market\x18\x01 \x01(\tR\x06market"=\n\x13ListMarketsResponse\x12&\n\x07markets\x18\x01 \x03(\x0b\x32\x0c.vega.MarketR\x07markets"N\n\x14ListProposalsRequest\x12\x1a\n\x08proposal\x18\x01 \x01(\tR\x08proposal\x12\x1a\n\x08proposer\x18\x02 \x01(\tR\x08proposer"E\n\x15ListProposalsResponse\x12,\n\tproposals\x18\x01 \x03(\x0b\x32\x0e.vega.ProposalR\tproposals"0\n\x16ListMarketsDataRequest\x12\x16\n\x06market\x18\x01 \x01(\tR\x06market"N\n\x17ListMarketsDataResponse\x12\x33\n\x0cmarkets_data\x18\x01 \x03(\x0b\x32\x10.vega.MarketDataR\x0bmarketsData"D\n\x10ListVotesRequest\x12\x1a\n\x08proposal\x18\x01 \x01(\tR\x08proposal\x12\x14\n\x05party\x18\x02 \x01(\tR\x05party"5\n\x11ListVotesResponse\x12 \n\x05votes\x18\x01 \x03(\x0b\x32\n.vega.VoteR\x05votes"\x9f\x01\n\nPartyStake\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x36\n\x17\x63urrent_stake_available\x18\x02 \x01(\tR\x15\x63urrentStakeAvailable\x12\x43\n\x0estake_linkings\x18\x03 \x03(\x0b\x32\x1c.vega.events.v1.StakeLinkingR\rstakeLinkings"/\n\x17ListPartiesStakeRequest\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party"X\n\x18ListPartiesStakeResponse\x12<\n\rparties_stake\x18\x01 \x03(\x0b\x32\x17.vega.api.v1.PartyStakeR\x0cpartiesStake"_\n\x16ListDelegationsRequest\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x12\n\x04node\x18\x02 \x01(\tR\x04node\x12\x1b\n\tepoch_seq\x18\x03 \x01(\tR\x08\x65pochSeq"M\n\x17ListDelegationsResponse\x12\x32\n\x0b\x64\x65legations\x18\x01 \x03(\x0b\x32\x10.vega.DelegationR\x0b\x64\x65legations2\xca\x08\n\x10\x43oreStateService\x12S\n\x0cListAccounts\x12 .vega.api.v1.ListAccountsRequest\x1a!.vega.api.v1.ListAccountsResponse\x12M\n\nListAssets\x12\x1e.vega.api.v1.ListAssetsRequest\x1a\x1f.vega.api.v1.ListAssetsResponse\x12n\n\x15ListNetworkParameters\x12).vega.api.v1.ListNetworkParametersRequest\x1a*.vega.api.v1.ListNetworkParametersResponse\x12\x62\n\x11ListNetworkLimits\x12%.vega.api.v1.ListNetworkLimitsRequest\x1a&.vega.api.v1.ListNetworkLimitsResponse\x12P\n\x0bListParties\x12\x1f.vega.api.v1.ListPartiesRequest\x1a .vega.api.v1.ListPartiesResponse\x12Y\n\x0eListValidators\x12".vega.api.v1.ListValidatorsRequest\x1a#.vega.api.v1.ListValidatorsResponse\x12P\n\x0bListMarkets\x12\x1f.vega.api.v1.ListMarketsRequest\x1a .vega.api.v1.ListMarketsResponse\x12V\n\rListProposals\x12!.vega.api.v1.ListProposalsRequest\x1a".vega.api.v1.ListProposalsResponse\x12\\\n\x0fListMarketsData\x12#.vega.api.v1.ListMarketsDataRequest\x1a$.vega.api.v1.ListMarketsDataResponse\x12J\n\tListVotes\x12\x1d.vega.api.v1.ListVotesRequest\x1a\x1e.vega.api.v1.ListVotesResponse\x12_\n\x10ListPartiesStake\x12$.vega.api.v1.ListPartiesStakeRequest\x1a%.vega.api.v1.ListPartiesStakeResponse\x12\\\n\x0fListDelegations\x12#.vega.api.v1.ListDelegationsRequest\x1a$.vega.api.v1.ListDelegationsResponseBkZ,code.vegaprotocol.io/vega/protos/vega/api/v1\x92\x41:\x12\x1f\n\x14Vega core state APIs2\x07v0.71.4\x1a\x13lb.testnet.vega.xyz*\x02\x01\x02\x62\x06proto3'
+    b'\n\x1bvega/api/v1/corestate.proto\x12\x0bvega.api.v1\x1a.protoc-gen-openapiv2/options/annotations.proto\x1a\x11vega/assets.proto\x1a\x1bvega/events/v1/events.proto\x1a\x15vega/governance.proto\x1a\x12vega/markets.proto\x1a\x0fvega/vega.proto"{\n\x07\x41\x63\x63ount\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x16\n\x06market\x18\x02 \x01(\tR\x06market\x12\x18\n\x07\x62\x61lance\x18\x03 \x01(\tR\x07\x62\x61lance\x12\x14\n\x05\x61sset\x18\x05 \x01(\tR\x05\x61sset\x12\x12\n\x04type\x18\x06 \x01(\tR\x04type"C\n\x13ListAccountsRequest\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x16\n\x06market\x18\x02 \x01(\tR\x06market"H\n\x14ListAccountsResponse\x12\x30\n\x08\x61\x63\x63ounts\x18\x01 \x03(\x0b\x32\x14.vega.api.v1.AccountR\x08\x61\x63\x63ounts")\n\x11ListAssetsRequest\x12\x14\n\x05\x61sset\x18\x01 \x01(\tR\x05\x61sset"9\n\x12ListAssetsResponse\x12#\n\x06\x61ssets\x18\x01 \x03(\x0b\x32\x0b.vega.AssetR\x06\x61ssets"R\n\x1cListNetworkParametersRequest\x12\x32\n\x15network_parameter_key\x18\x01 \x01(\tR\x13networkParameterKey"f\n\x1dListNetworkParametersResponse\x12\x45\n\x12network_parameters\x18\x01 \x03(\x0b\x32\x16.vega.NetworkParameterR\x11networkParameters"\x1a\n\x18ListNetworkLimitsRequest"W\n\x19ListNetworkLimitsResponse\x12:\n\x0enetwork_limits\x18\x01 \x01(\x0b\x32\x13.vega.NetworkLimitsR\rnetworkLimits"\x14\n\x12ListPartiesRequest"<\n\x13ListPartiesResponse\x12%\n\x07parties\x18\x01 \x03(\x0b\x32\x0b.vega.PartyR\x07parties"\x17\n\x15ListValidatorsRequest"Y\n\x16ListValidatorsResponse\x12?\n\nvalidators\x18\x01 \x03(\x0b\x32\x1f.vega.events.v1.ValidatorUpdateR\nvalidators",\n\x12ListMarketsRequest\x12\x16\n\x06market\x18\x01 \x01(\tR\x06market"=\n\x13ListMarketsResponse\x12&\n\x07markets\x18\x01 \x03(\x0b\x32\x0c.vega.MarketR\x07markets"N\n\x14ListProposalsRequest\x12\x1a\n\x08proposal\x18\x01 \x01(\tR\x08proposal\x12\x1a\n\x08proposer\x18\x02 \x01(\tR\x08proposer"E\n\x15ListProposalsResponse\x12,\n\tproposals\x18\x01 \x03(\x0b\x32\x0e.vega.ProposalR\tproposals"0\n\x16ListMarketsDataRequest\x12\x16\n\x06market\x18\x01 \x01(\tR\x06market"N\n\x17ListMarketsDataResponse\x12\x33\n\x0cmarkets_data\x18\x01 \x03(\x0b\x32\x10.vega.MarketDataR\x0bmarketsData"D\n\x10ListVotesRequest\x12\x1a\n\x08proposal\x18\x01 \x01(\tR\x08proposal\x12\x14\n\x05party\x18\x02 \x01(\tR\x05party"5\n\x11ListVotesResponse\x12 \n\x05votes\x18\x01 \x03(\x0b\x32\n.vega.VoteR\x05votes"\x9f\x01\n\nPartyStake\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x36\n\x17\x63urrent_stake_available\x18\x02 \x01(\tR\x15\x63urrentStakeAvailable\x12\x43\n\x0estake_linkings\x18\x03 \x03(\x0b\x32\x1c.vega.events.v1.StakeLinkingR\rstakeLinkings"/\n\x17ListPartiesStakeRequest\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party"X\n\x18ListPartiesStakeResponse\x12<\n\rparties_stake\x18\x01 \x03(\x0b\x32\x17.vega.api.v1.PartyStakeR\x0cpartiesStake"_\n\x16ListDelegationsRequest\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x12\n\x04node\x18\x02 \x01(\tR\x04node\x12\x1b\n\tepoch_seq\x18\x03 \x01(\tR\x08\x65pochSeq"M\n\x17ListDelegationsResponse\x12\x32\n\x0b\x64\x65legations\x18\x01 \x03(\x0b\x32\x10.vega.DelegationR\x0b\x64\x65legations2\xca\x08\n\x10\x43oreStateService\x12S\n\x0cListAccounts\x12 .vega.api.v1.ListAccountsRequest\x1a!.vega.api.v1.ListAccountsResponse\x12M\n\nListAssets\x12\x1e.vega.api.v1.ListAssetsRequest\x1a\x1f.vega.api.v1.ListAssetsResponse\x12n\n\x15ListNetworkParameters\x12).vega.api.v1.ListNetworkParametersRequest\x1a*.vega.api.v1.ListNetworkParametersResponse\x12\x62\n\x11ListNetworkLimits\x12%.vega.api.v1.ListNetworkLimitsRequest\x1a&.vega.api.v1.ListNetworkLimitsResponse\x12P\n\x0bListParties\x12\x1f.vega.api.v1.ListPartiesRequest\x1a .vega.api.v1.ListPartiesResponse\x12Y\n\x0eListValidators\x12".vega.api.v1.ListValidatorsRequest\x1a#.vega.api.v1.ListValidatorsResponse\x12P\n\x0bListMarkets\x12\x1f.vega.api.v1.ListMarketsRequest\x1a .vega.api.v1.ListMarketsResponse\x12V\n\rListProposals\x12!.vega.api.v1.ListProposalsRequest\x1a".vega.api.v1.ListProposalsResponse\x12\\\n\x0fListMarketsData\x12#.vega.api.v1.ListMarketsDataRequest\x1a$.vega.api.v1.ListMarketsDataResponse\x12J\n\tListVotes\x12\x1d.vega.api.v1.ListVotesRequest\x1a\x1e.vega.api.v1.ListVotesResponse\x12_\n\x10ListPartiesStake\x12$.vega.api.v1.ListPartiesStakeRequest\x1a%.vega.api.v1.ListPartiesStakeResponse\x12\\\n\x0fListDelegations\x12#.vega.api.v1.ListDelegationsRequest\x1a$.vega.api.v1.ListDelegationsResponseBkZ,code.vegaprotocol.io/vega/protos/vega/api/v1\x92\x41:\x12\x1f\n\x14Vega core state APIs2\x07v0.71.0\x1a\x13lb.testnet.vega.xyz*\x02\x01\x02\x62\x06proto3'
 )
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(
-    DESCRIPTOR, "vega.api.v1.corestate_pb2", globals()
+    DESCRIPTOR, "vega.api.v1.corestate_pb2", _globals
 )
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    DESCRIPTOR._serialized_options = b"Z,code.vegaprotocol.io/vega/protos/vega/api/v1\222A:\022\037\n\024Vega core state APIs2\007v0.71.4\032\023lb.testnet.vega.xyz*\002\001\002"
-    _ACCOUNT._serialized_start = 200
-    _ACCOUNT._serialized_end = 323
-    _LISTACCOUNTSREQUEST._serialized_start = 325
-    _LISTACCOUNTSREQUEST._serialized_end = 392
-    _LISTACCOUNTSRESPONSE._serialized_start = 394
-    _LISTACCOUNTSRESPONSE._serialized_end = 466
-    _LISTASSETSREQUEST._serialized_start = 468
-    _LISTASSETSREQUEST._serialized_end = 509
-    _LISTASSETSRESPONSE._serialized_start = 511
-    _LISTASSETSRESPONSE._serialized_end = 568
-    _LISTNETWORKPARAMETERSREQUEST._serialized_start = 570
-    _LISTNETWORKPARAMETERSREQUEST._serialized_end = 652
-    _LISTNETWORKPARAMETERSRESPONSE._serialized_start = 654
-    _LISTNETWORKPARAMETERSRESPONSE._serialized_end = 756
-    _LISTNETWORKLIMITSREQUEST._serialized_start = 758
-    _LISTNETWORKLIMITSREQUEST._serialized_end = 784
-    _LISTNETWORKLIMITSRESPONSE._serialized_start = 786
-    _LISTNETWORKLIMITSRESPONSE._serialized_end = 873
-    _LISTPARTIESREQUEST._serialized_start = 875
-    _LISTPARTIESREQUEST._serialized_end = 895
-    _LISTPARTIESRESPONSE._serialized_start = 897
-    _LISTPARTIESRESPONSE._serialized_end = 957
-    _LISTVALIDATORSREQUEST._serialized_start = 959
-    _LISTVALIDATORSREQUEST._serialized_end = 982
-    _LISTVALIDATORSRESPONSE._serialized_start = 984
-    _LISTVALIDATORSRESPONSE._serialized_end = 1073
-    _LISTMARKETSREQUEST._serialized_start = 1075
-    _LISTMARKETSREQUEST._serialized_end = 1119
-    _LISTMARKETSRESPONSE._serialized_start = 1121
-    _LISTMARKETSRESPONSE._serialized_end = 1182
-    _LISTPROPOSALSREQUEST._serialized_start = 1184
-    _LISTPROPOSALSREQUEST._serialized_end = 1262
-    _LISTPROPOSALSRESPONSE._serialized_start = 1264
-    _LISTPROPOSALSRESPONSE._serialized_end = 1333
-    _LISTMARKETSDATAREQUEST._serialized_start = 1335
-    _LISTMARKETSDATAREQUEST._serialized_end = 1383
-    _LISTMARKETSDATARESPONSE._serialized_start = 1385
-    _LISTMARKETSDATARESPONSE._serialized_end = 1463
-    _LISTVOTESREQUEST._serialized_start = 1465
-    _LISTVOTESREQUEST._serialized_end = 1533
-    _LISTVOTESRESPONSE._serialized_start = 1535
-    _LISTVOTESRESPONSE._serialized_end = 1588
-    _PARTYSTAKE._serialized_start = 1591
-    _PARTYSTAKE._serialized_end = 1750
-    _LISTPARTIESSTAKEREQUEST._serialized_start = 1752
-    _LISTPARTIESSTAKEREQUEST._serialized_end = 1799
-    _LISTPARTIESSTAKERESPONSE._serialized_start = 1801
-    _LISTPARTIESSTAKERESPONSE._serialized_end = 1889
-    _LISTDELEGATIONSREQUEST._serialized_start = 1891
-    _LISTDELEGATIONSREQUEST._serialized_end = 1986
-    _LISTDELEGATIONSRESPONSE._serialized_start = 1988
-    _LISTDELEGATIONSRESPONSE._serialized_end = 2065
-    _CORESTATESERVICE._serialized_start = 2068
-    _CORESTATESERVICE._serialized_end = 3166
+    DESCRIPTOR._serialized_options = b"Z,code.vegaprotocol.io/vega/protos/vega/api/v1\222A:\022\037\n\024Vega core state APIs2\007v0.71.0\032\023lb.testnet.vega.xyz*\002\001\002"
+    _globals["_ACCOUNT"]._serialized_start = 200
+    _globals["_ACCOUNT"]._serialized_end = 323
+    _globals["_LISTACCOUNTSREQUEST"]._serialized_start = 325
+    _globals["_LISTACCOUNTSREQUEST"]._serialized_end = 392
+    _globals["_LISTACCOUNTSRESPONSE"]._serialized_start = 394
+    _globals["_LISTACCOUNTSRESPONSE"]._serialized_end = 466
+    _globals["_LISTASSETSREQUEST"]._serialized_start = 468
+    _globals["_LISTASSETSREQUEST"]._serialized_end = 509
+    _globals["_LISTASSETSRESPONSE"]._serialized_start = 511
+    _globals["_LISTASSETSRESPONSE"]._serialized_end = 568
+    _globals["_LISTNETWORKPARAMETERSREQUEST"]._serialized_start = 570
+    _globals["_LISTNETWORKPARAMETERSREQUEST"]._serialized_end = 652
+    _globals["_LISTNETWORKPARAMETERSRESPONSE"]._serialized_start = 654
+    _globals["_LISTNETWORKPARAMETERSRESPONSE"]._serialized_end = 756
+    _globals["_LISTNETWORKLIMITSREQUEST"]._serialized_start = 758
+    _globals["_LISTNETWORKLIMITSREQUEST"]._serialized_end = 784
+    _globals["_LISTNETWORKLIMITSRESPONSE"]._serialized_start = 786
+    _globals["_LISTNETWORKLIMITSRESPONSE"]._serialized_end = 873
+    _globals["_LISTPARTIESREQUEST"]._serialized_start = 875
+    _globals["_LISTPARTIESREQUEST"]._serialized_end = 895
+    _globals["_LISTPARTIESRESPONSE"]._serialized_start = 897
+    _globals["_LISTPARTIESRESPONSE"]._serialized_end = 957
+    _globals["_LISTVALIDATORSREQUEST"]._serialized_start = 959
+    _globals["_LISTVALIDATORSREQUEST"]._serialized_end = 982
+    _globals["_LISTVALIDATORSRESPONSE"]._serialized_start = 984
+    _globals["_LISTVALIDATORSRESPONSE"]._serialized_end = 1073
+    _globals["_LISTMARKETSREQUEST"]._serialized_start = 1075
+    _globals["_LISTMARKETSREQUEST"]._serialized_end = 1119
+    _globals["_LISTMARKETSRESPONSE"]._serialized_start = 1121
+    _globals["_LISTMARKETSRESPONSE"]._serialized_end = 1182
+    _globals["_LISTPROPOSALSREQUEST"]._serialized_start = 1184
+    _globals["_LISTPROPOSALSREQUEST"]._serialized_end = 1262
+    _globals["_LISTPROPOSALSRESPONSE"]._serialized_start = 1264
+    _globals["_LISTPROPOSALSRESPONSE"]._serialized_end = 1333
+    _globals["_LISTMARKETSDATAREQUEST"]._serialized_start = 1335
+    _globals["_LISTMARKETSDATAREQUEST"]._serialized_end = 1383
+    _globals["_LISTMARKETSDATARESPONSE"]._serialized_start = 1385
+    _globals["_LISTMARKETSDATARESPONSE"]._serialized_end = 1463
+    _globals["_LISTVOTESREQUEST"]._serialized_start = 1465
+    _globals["_LISTVOTESREQUEST"]._serialized_end = 1533
+    _globals["_LISTVOTESRESPONSE"]._serialized_start = 1535
+    _globals["_LISTVOTESRESPONSE"]._serialized_end = 1588
+    _globals["_PARTYSTAKE"]._serialized_start = 1591
+    _globals["_PARTYSTAKE"]._serialized_end = 1750
+    _globals["_LISTPARTIESSTAKEREQUEST"]._serialized_start = 1752
+    _globals["_LISTPARTIESSTAKEREQUEST"]._serialized_end = 1799
+    _globals["_LISTPARTIESSTAKERESPONSE"]._serialized_start = 1801
+    _globals["_LISTPARTIESSTAKERESPONSE"]._serialized_end = 1889
+    _globals["_LISTDELEGATIONSREQUEST"]._serialized_start = 1891
+    _globals["_LISTDELEGATIONSREQUEST"]._serialized_end = 1986
+    _globals["_LISTDELEGATIONSRESPONSE"]._serialized_start = 1988
+    _globals["_LISTDELEGATIONSRESPONSE"]._serialized_end = 2065
+    _globals["_CORESTATESERVICE"]._serialized_start = 2068
+    _globals["_CORESTATESERVICE"]._serialized_end = 3166
 # @@protoc_insertion_point(module_scope)
```

### Comparing `vega_sim-1.1.1/vega_sim/proto/vega/api/v1/corestate_pb2_grpc.py` & `vega_sim-1.2.0/vega_sim/proto/vega/api/v1/corestate_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/proto/vega/assets_pb2.py` & `vega_sim-1.2.0/vega_sim/proto/vega/assets_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: vega/assets.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
     b'\n\x11vega/assets.proto\x12\x04vega"\xed\x01\n\x05\x41sset\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12,\n\x07\x64\x65tails\x18\x02 \x01(\x0b\x32\x12.vega.AssetDetailsR\x07\x64\x65tails\x12*\n\x06status\x18\x03 \x01(\x0e\x32\x12.vega.Asset.StatusR\x06status"z\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x13\n\x0fSTATUS_PROPOSED\x10\x01\x12\x13\n\x0fSTATUS_REJECTED\x10\x02\x12\x1a\n\x16STATUS_PENDING_LISTING\x10\x03\x12\x12\n\x0eSTATUS_ENABLED\x10\x04"\xe0\x01\n\x0c\x41ssetDetails\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x16\n\x06symbol\x18\x02 \x01(\tR\x06symbol\x12\x1a\n\x08\x64\x65\x63imals\x18\x04 \x01(\x04R\x08\x64\x65\x63imals\x12\x18\n\x07quantum\x18\x05 \x01(\tR\x07quantum\x12\x39\n\rbuiltin_asset\x18\x65 \x01(\x0b\x32\x12.vega.BuiltinAssetH\x00R\x0c\x62uiltinAsset\x12#\n\x05\x65rc20\x18\x66 \x01(\x0b\x32\x0b.vega.ERC20H\x00R\x05\x65rc20B\x08\n\x06sourceJ\x04\x08\x03\x10\x04"C\n\x0c\x42uiltinAsset\x12\x33\n\x16max_faucet_amount_mint\x18\x01 \x01(\tR\x13maxFaucetAmountMint"\x88\x01\n\x05\x45RC20\x12)\n\x10\x63ontract_address\x18\x01 \x01(\tR\x0f\x63ontractAddress\x12%\n\x0elifetime_limit\x18\x02 \x01(\tR\rlifetimeLimit\x12-\n\x12withdraw_threshold\x18\x03 \x01(\tR\x11withdrawThreshold"{\n\x12\x41ssetDetailsUpdate\x12\x18\n\x07quantum\x18\x05 \x01(\tR\x07quantum\x12)\n\x05\x65rc20\x18\x65 \x01(\x0b\x32\x11.vega.ERC20UpdateH\x00R\x05\x65rc20B\x08\n\x06sourceJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05"c\n\x0b\x45RC20Update\x12%\n\x0elifetime_limit\x18\x01 \x01(\tR\rlifetimeLimit\x12-\n\x12withdraw_threshold\x18\x02 \x01(\tR\x11withdrawThresholdB\'Z%code.vegaprotocol.io/vega/protos/vegab\x06proto3'
 )
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "vega.assets_pb2", globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "vega.assets_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b"Z%code.vegaprotocol.io/vega/protos/vega"
-    _ASSET._serialized_start = 28
-    _ASSET._serialized_end = 265
-    _ASSET_STATUS._serialized_start = 143
-    _ASSET_STATUS._serialized_end = 265
-    _ASSETDETAILS._serialized_start = 268
-    _ASSETDETAILS._serialized_end = 492
-    _BUILTINASSET._serialized_start = 494
-    _BUILTINASSET._serialized_end = 561
-    _ERC20._serialized_start = 564
-    _ERC20._serialized_end = 700
-    _ASSETDETAILSUPDATE._serialized_start = 702
-    _ASSETDETAILSUPDATE._serialized_end = 825
-    _ERC20UPDATE._serialized_start = 827
-    _ERC20UPDATE._serialized_end = 926
+    _globals["_ASSET"]._serialized_start = 28
+    _globals["_ASSET"]._serialized_end = 265
+    _globals["_ASSET_STATUS"]._serialized_start = 143
+    _globals["_ASSET_STATUS"]._serialized_end = 265
+    _globals["_ASSETDETAILS"]._serialized_start = 268
+    _globals["_ASSETDETAILS"]._serialized_end = 492
+    _globals["_BUILTINASSET"]._serialized_start = 494
+    _globals["_BUILTINASSET"]._serialized_end = 561
+    _globals["_ERC20"]._serialized_start = 564
+    _globals["_ERC20"]._serialized_end = 700
+    _globals["_ASSETDETAILSUPDATE"]._serialized_start = 702
+    _globals["_ASSETDETAILSUPDATE"]._serialized_end = 825
+    _globals["_ERC20UPDATE"]._serialized_start = 827
+    _globals["_ERC20UPDATE"]._serialized_end = 926
 # @@protoc_insertion_point(module_scope)
```

### Comparing `vega_sim-1.1.1/vega_sim/proto/vega/chain_events_pb2.py` & `vega_sim-1.2.0/vega_sim/proto/vega/chain_events_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,61 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: vega/chain_events.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x17vega/chain_events.proto\x12\x04vega"l\n\x13\x42uiltinAssetDeposit\x12"\n\rvega_asset_id\x18\x01 \x01(\tR\x0bvegaAssetId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount"o\n\x16\x42uiltinAssetWithdrawal\x12"\n\rvega_asset_id\x18\x01 \x01(\tR\x0bvegaAssetId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount"\x96\x01\n\x11\x42uiltinAssetEvent\x12\x36\n\x07\x64\x65posit\x18\xe9\x07 \x01(\x0b\x32\x19.vega.BuiltinAssetDepositH\x00R\x07\x64\x65posit\x12?\n\nwithdrawal\x18\xea\x07 \x01(\x0b\x32\x1c.vega.BuiltinAssetWithdrawalH\x00R\nwithdrawalB\x08\n\x06\x61\x63tion"W\n\x0e\x45RC20AssetList\x12"\n\rvega_asset_id\x18\x01 \x01(\tR\x0bvegaAssetId\x12!\n\x0c\x61sset_source\x18\x02 \x01(\tR\x0b\x61ssetSource"6\n\x10\x45RC20AssetDelist\x12"\n\rvega_asset_id\x18\x01 \x01(\tR\x0bvegaAssetId"\xcd\x01\n\x17\x45RC20AssetLimitsUpdated\x12"\n\rvega_asset_id\x18\x01 \x01(\tR\x0bvegaAssetId\x12\x36\n\x17source_ethereum_address\x18\x02 \x01(\tR\x15sourceEthereumAddress\x12\'\n\x0flifetime_limits\x18\x03 \x01(\tR\x0elifetimeLimits\x12-\n\x12withdraw_threshold\x18\x04 \x01(\tR\x11withdrawThreshold"\xaa\x01\n\x0c\x45RC20Deposit\x12"\n\rvega_asset_id\x18\x01 \x01(\tR\x0bvegaAssetId\x12\x36\n\x17source_ethereum_address\x18\x02 \x01(\tR\x15sourceEthereumAddress\x12&\n\x0ftarget_party_id\x18\x03 \x01(\tR\rtargetPartyId\x12\x16\n\x06\x61mount\x18\x04 \x01(\tR\x06\x61mount"\x96\x01\n\x0f\x45RC20Withdrawal\x12"\n\rvega_asset_id\x18\x01 \x01(\tR\x0bvegaAssetId\x12\x36\n\x17target_ethereum_address\x18\x02 \x01(\tR\x15targetEthereumAddress\x12\'\n\x0freference_nonce\x18\x03 \x01(\tR\x0ereferenceNonce"\xcb\x03\n\nERC20Event\x12\x14\n\x05index\x18\x01 \x01(\x04R\x05index\x12\x14\n\x05\x62lock\x18\x02 \x01(\x04R\x05\x62lock\x12\x36\n\nasset_list\x18\xe9\x07 \x01(\x0b\x32\x14.vega.ERC20AssetListH\x00R\tassetList\x12<\n\x0c\x61sset_delist\x18\xea\x07 \x01(\x0b\x32\x16.vega.ERC20AssetDelistH\x00R\x0b\x61ssetDelist\x12/\n\x07\x64\x65posit\x18\xeb\x07 \x01(\x0b\x32\x12.vega.ERC20DepositH\x00R\x07\x64\x65posit\x12\x38\n\nwithdrawal\x18\xec\x07 \x01(\x0b\x32\x15.vega.ERC20WithdrawalH\x00R\nwithdrawal\x12R\n\x14\x61sset_limits_updated\x18\xed\x07 \x01(\x0b\x32\x1d.vega.ERC20AssetLimitsUpdatedH\x00R\x12\x61ssetLimitsUpdated\x12(\n\x0e\x62ridge_stopped\x18\xee\x07 \x01(\x08H\x00R\rbridgeStopped\x12(\n\x0e\x62ridge_resumed\x18\xef\x07 \x01(\x08H\x00R\rbridgeResumedB\x08\n\x06\x61\x63tion"f\n\x10\x45RC20SignerAdded\x12\x1d\n\nnew_signer\x18\x01 \x01(\tR\tnewSigner\x12\x14\n\x05nonce\x18\x02 \x01(\tR\x05nonce\x12\x1d\n\nblock_time\x18\x03 \x01(\x03R\tblockTime"h\n\x12\x45RC20SignerRemoved\x12\x1d\n\nold_signer\x18\x01 \x01(\tR\toldSigner\x12\x14\n\x05nonce\x18\x02 \x01(\tR\x05nonce\x12\x1d\n\nblock_time\x18\x03 \x01(\x03R\tblockTime"m\n\x11\x45RC20ThresholdSet\x12#\n\rnew_threshold\x18\x01 \x01(\rR\x0cnewThreshold\x12\x14\n\x05nonce\x18\x02 \x01(\tR\x05nonce\x12\x1d\n\nblock_time\x18\x03 \x01(\x03R\tblockTime"\x8d\x02\n\x12\x45RC20MultiSigEvent\x12\x14\n\x05index\x18\x01 \x01(\x04R\x05index\x12\x14\n\x05\x62lock\x18\x02 \x01(\x04R\x05\x62lock\x12<\n\x0csigner_added\x18\xe9\x07 \x01(\x0b\x32\x16.vega.ERC20SignerAddedH\x00R\x0bsignerAdded\x12\x42\n\x0esigner_removed\x18\xea\x07 \x01(\x0b\x32\x18.vega.ERC20SignerRemovedH\x00R\rsignerRemoved\x12?\n\rthreshold_set\x18\xeb\x07 \x01(\x0b\x32\x17.vega.ERC20ThresholdSetH\x00R\x0cthresholdSetB\x08\n\x06\x61\x63tion"\x80\x02\n\x0cStakingEvent\x12\x14\n\x05index\x18\x01 \x01(\x04R\x05index\x12\x14\n\x05\x62lock\x18\x02 \x01(\x04R\x05\x62lock\x12@\n\x0fstake_deposited\x18\xe9\x07 \x01(\x0b\x32\x14.vega.StakeDepositedH\x00R\x0estakeDeposited\x12:\n\rstake_removed\x18\xea\x07 \x01(\x0b\x32\x12.vega.StakeRemovedH\x00R\x0cstakeRemoved\x12<\n\x0ctotal_supply\x18\xeb\x07 \x01(\x0b\x32\x16.vega.StakeTotalSupplyH\x00R\x0btotalSupplyB\x08\n\x06\x61\x63tion"\x9a\x01\n\x0eStakeDeposited\x12)\n\x10\x65thereum_address\x18\x01 \x01(\tR\x0f\x65thereumAddress\x12&\n\x0fvega_public_key\x18\x02 \x01(\tR\rvegaPublicKey\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount\x12\x1d\n\nblock_time\x18\x04 \x01(\x03R\tblockTime"\x98\x01\n\x0cStakeRemoved\x12)\n\x10\x65thereum_address\x18\x01 \x01(\tR\x0f\x65thereumAddress\x12&\n\x0fvega_public_key\x18\x02 \x01(\tR\rvegaPublicKey\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount\x12\x1d\n\nblock_time\x18\x04 \x01(\x03R\tblockTime"Z\n\x10StakeTotalSupply\x12#\n\rtoken_address\x18\x01 \x01(\tR\x0ctokenAddress\x12!\n\x0ctotal_supply\x18\x02 \x01(\tR\x0btotalSupplyB\'Z%code.vegaprotocol.io/vega/protos/vegab\x06proto3'
+    b'\n\x17vega/chain_events.proto\x12\x04vega"\x89\x01\n\x14\x45thContractCallEvent\x12\x17\n\x07spec_id\x18\x01 \x01(\tR\x06specId\x12!\n\x0c\x62lock_height\x18\x02 \x01(\x04R\x0b\x62lockHeight\x12\x1d\n\nblock_time\x18\x03 \x01(\x04R\tblockTime\x12\x16\n\x06result\x18\x04 \x01(\x0cR\x06result"l\n\x13\x42uiltinAssetDeposit\x12"\n\rvega_asset_id\x18\x01 \x01(\tR\x0bvegaAssetId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount"o\n\x16\x42uiltinAssetWithdrawal\x12"\n\rvega_asset_id\x18\x01 \x01(\tR\x0bvegaAssetId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount"\x96\x01\n\x11\x42uiltinAssetEvent\x12\x36\n\x07\x64\x65posit\x18\xe9\x07 \x01(\x0b\x32\x19.vega.BuiltinAssetDepositH\x00R\x07\x64\x65posit\x12?\n\nwithdrawal\x18\xea\x07 \x01(\x0b\x32\x1c.vega.BuiltinAssetWithdrawalH\x00R\nwithdrawalB\x08\n\x06\x61\x63tion"W\n\x0e\x45RC20AssetList\x12"\n\rvega_asset_id\x18\x01 \x01(\tR\x0bvegaAssetId\x12!\n\x0c\x61sset_source\x18\x02 \x01(\tR\x0b\x61ssetSource"6\n\x10\x45RC20AssetDelist\x12"\n\rvega_asset_id\x18\x01 \x01(\tR\x0bvegaAssetId"\xcd\x01\n\x17\x45RC20AssetLimitsUpdated\x12"\n\rvega_asset_id\x18\x01 \x01(\tR\x0bvegaAssetId\x12\x36\n\x17source_ethereum_address\x18\x02 \x01(\tR\x15sourceEthereumAddress\x12\'\n\x0flifetime_limits\x18\x03 \x01(\tR\x0elifetimeLimits\x12-\n\x12withdraw_threshold\x18\x04 \x01(\tR\x11withdrawThreshold"\xaa\x01\n\x0c\x45RC20Deposit\x12"\n\rvega_asset_id\x18\x01 \x01(\tR\x0bvegaAssetId\x12\x36\n\x17source_ethereum_address\x18\x02 \x01(\tR\x15sourceEthereumAddress\x12&\n\x0ftarget_party_id\x18\x03 \x01(\tR\rtargetPartyId\x12\x16\n\x06\x61mount\x18\x04 \x01(\tR\x06\x61mount"\x96\x01\n\x0f\x45RC20Withdrawal\x12"\n\rvega_asset_id\x18\x01 \x01(\tR\x0bvegaAssetId\x12\x36\n\x17target_ethereum_address\x18\x02 \x01(\tR\x15targetEthereumAddress\x12\'\n\x0freference_nonce\x18\x03 \x01(\tR\x0ereferenceNonce"\xcb\x03\n\nERC20Event\x12\x14\n\x05index\x18\x01 \x01(\x04R\x05index\x12\x14\n\x05\x62lock\x18\x02 \x01(\x04R\x05\x62lock\x12\x36\n\nasset_list\x18\xe9\x07 \x01(\x0b\x32\x14.vega.ERC20AssetListH\x00R\tassetList\x12<\n\x0c\x61sset_delist\x18\xea\x07 \x01(\x0b\x32\x16.vega.ERC20AssetDelistH\x00R\x0b\x61ssetDelist\x12/\n\x07\x64\x65posit\x18\xeb\x07 \x01(\x0b\x32\x12.vega.ERC20DepositH\x00R\x07\x64\x65posit\x12\x38\n\nwithdrawal\x18\xec\x07 \x01(\x0b\x32\x15.vega.ERC20WithdrawalH\x00R\nwithdrawal\x12R\n\x14\x61sset_limits_updated\x18\xed\x07 \x01(\x0b\x32\x1d.vega.ERC20AssetLimitsUpdatedH\x00R\x12\x61ssetLimitsUpdated\x12(\n\x0e\x62ridge_stopped\x18\xee\x07 \x01(\x08H\x00R\rbridgeStopped\x12(\n\x0e\x62ridge_resumed\x18\xef\x07 \x01(\x08H\x00R\rbridgeResumedB\x08\n\x06\x61\x63tion"f\n\x10\x45RC20SignerAdded\x12\x1d\n\nnew_signer\x18\x01 \x01(\tR\tnewSigner\x12\x14\n\x05nonce\x18\x02 \x01(\tR\x05nonce\x12\x1d\n\nblock_time\x18\x03 \x01(\x03R\tblockTime"h\n\x12\x45RC20SignerRemoved\x12\x1d\n\nold_signer\x18\x01 \x01(\tR\toldSigner\x12\x14\n\x05nonce\x18\x02 \x01(\tR\x05nonce\x12\x1d\n\nblock_time\x18\x03 \x01(\x03R\tblockTime"m\n\x11\x45RC20ThresholdSet\x12#\n\rnew_threshold\x18\x01 \x01(\rR\x0cnewThreshold\x12\x14\n\x05nonce\x18\x02 \x01(\tR\x05nonce\x12\x1d\n\nblock_time\x18\x03 \x01(\x03R\tblockTime"\x8d\x02\n\x12\x45RC20MultiSigEvent\x12\x14\n\x05index\x18\x01 \x01(\x04R\x05index\x12\x14\n\x05\x62lock\x18\x02 \x01(\x04R\x05\x62lock\x12<\n\x0csigner_added\x18\xe9\x07 \x01(\x0b\x32\x16.vega.ERC20SignerAddedH\x00R\x0bsignerAdded\x12\x42\n\x0esigner_removed\x18\xea\x07 \x01(\x0b\x32\x18.vega.ERC20SignerRemovedH\x00R\rsignerRemoved\x12?\n\rthreshold_set\x18\xeb\x07 \x01(\x0b\x32\x17.vega.ERC20ThresholdSetH\x00R\x0cthresholdSetB\x08\n\x06\x61\x63tion"\x80\x02\n\x0cStakingEvent\x12\x14\n\x05index\x18\x01 \x01(\x04R\x05index\x12\x14\n\x05\x62lock\x18\x02 \x01(\x04R\x05\x62lock\x12@\n\x0fstake_deposited\x18\xe9\x07 \x01(\x0b\x32\x14.vega.StakeDepositedH\x00R\x0estakeDeposited\x12:\n\rstake_removed\x18\xea\x07 \x01(\x0b\x32\x12.vega.StakeRemovedH\x00R\x0cstakeRemoved\x12<\n\x0ctotal_supply\x18\xeb\x07 \x01(\x0b\x32\x16.vega.StakeTotalSupplyH\x00R\x0btotalSupplyB\x08\n\x06\x61\x63tion"\x9a\x01\n\x0eStakeDeposited\x12)\n\x10\x65thereum_address\x18\x01 \x01(\tR\x0f\x65thereumAddress\x12&\n\x0fvega_public_key\x18\x02 \x01(\tR\rvegaPublicKey\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount\x12\x1d\n\nblock_time\x18\x04 \x01(\x03R\tblockTime"\x98\x01\n\x0cStakeRemoved\x12)\n\x10\x65thereum_address\x18\x01 \x01(\tR\x0f\x65thereumAddress\x12&\n\x0fvega_public_key\x18\x02 \x01(\tR\rvegaPublicKey\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount\x12\x1d\n\nblock_time\x18\x04 \x01(\x03R\tblockTime"Z\n\x10StakeTotalSupply\x12#\n\rtoken_address\x18\x01 \x01(\tR\x0ctokenAddress\x12!\n\x0ctotal_supply\x18\x02 \x01(\tR\x0btotalSupplyB\'Z%code.vegaprotocol.io/vega/protos/vegab\x06proto3'
 )
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "vega.chain_events_pb2", globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "vega.chain_events_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b"Z%code.vegaprotocol.io/vega/protos/vega"
-    _BUILTINASSETDEPOSIT._serialized_start = 33
-    _BUILTINASSETDEPOSIT._serialized_end = 141
-    _BUILTINASSETWITHDRAWAL._serialized_start = 143
-    _BUILTINASSETWITHDRAWAL._serialized_end = 254
-    _BUILTINASSETEVENT._serialized_start = 257
-    _BUILTINASSETEVENT._serialized_end = 407
-    _ERC20ASSETLIST._serialized_start = 409
-    _ERC20ASSETLIST._serialized_end = 496
-    _ERC20ASSETDELIST._serialized_start = 498
-    _ERC20ASSETDELIST._serialized_end = 552
-    _ERC20ASSETLIMITSUPDATED._serialized_start = 555
-    _ERC20ASSETLIMITSUPDATED._serialized_end = 760
-    _ERC20DEPOSIT._serialized_start = 763
-    _ERC20DEPOSIT._serialized_end = 933
-    _ERC20WITHDRAWAL._serialized_start = 936
-    _ERC20WITHDRAWAL._serialized_end = 1086
-    _ERC20EVENT._serialized_start = 1089
-    _ERC20EVENT._serialized_end = 1548
-    _ERC20SIGNERADDED._serialized_start = 1550
-    _ERC20SIGNERADDED._serialized_end = 1652
-    _ERC20SIGNERREMOVED._serialized_start = 1654
-    _ERC20SIGNERREMOVED._serialized_end = 1758
-    _ERC20THRESHOLDSET._serialized_start = 1760
-    _ERC20THRESHOLDSET._serialized_end = 1869
-    _ERC20MULTISIGEVENT._serialized_start = 1872
-    _ERC20MULTISIGEVENT._serialized_end = 2141
-    _STAKINGEVENT._serialized_start = 2144
-    _STAKINGEVENT._serialized_end = 2400
-    _STAKEDEPOSITED._serialized_start = 2403
-    _STAKEDEPOSITED._serialized_end = 2557
-    _STAKEREMOVED._serialized_start = 2560
-    _STAKEREMOVED._serialized_end = 2712
-    _STAKETOTALSUPPLY._serialized_start = 2714
-    _STAKETOTALSUPPLY._serialized_end = 2804
+    _globals["_ETHCONTRACTCALLEVENT"]._serialized_start = 34
+    _globals["_ETHCONTRACTCALLEVENT"]._serialized_end = 171
+    _globals["_BUILTINASSETDEPOSIT"]._serialized_start = 173
+    _globals["_BUILTINASSETDEPOSIT"]._serialized_end = 281
+    _globals["_BUILTINASSETWITHDRAWAL"]._serialized_start = 283
+    _globals["_BUILTINASSETWITHDRAWAL"]._serialized_end = 394
+    _globals["_BUILTINASSETEVENT"]._serialized_start = 397
+    _globals["_BUILTINASSETEVENT"]._serialized_end = 547
+    _globals["_ERC20ASSETLIST"]._serialized_start = 549
+    _globals["_ERC20ASSETLIST"]._serialized_end = 636
+    _globals["_ERC20ASSETDELIST"]._serialized_start = 638
+    _globals["_ERC20ASSETDELIST"]._serialized_end = 692
+    _globals["_ERC20ASSETLIMITSUPDATED"]._serialized_start = 695
+    _globals["_ERC20ASSETLIMITSUPDATED"]._serialized_end = 900
+    _globals["_ERC20DEPOSIT"]._serialized_start = 903
+    _globals["_ERC20DEPOSIT"]._serialized_end = 1073
+    _globals["_ERC20WITHDRAWAL"]._serialized_start = 1076
+    _globals["_ERC20WITHDRAWAL"]._serialized_end = 1226
+    _globals["_ERC20EVENT"]._serialized_start = 1229
+    _globals["_ERC20EVENT"]._serialized_end = 1688
+    _globals["_ERC20SIGNERADDED"]._serialized_start = 1690
+    _globals["_ERC20SIGNERADDED"]._serialized_end = 1792
+    _globals["_ERC20SIGNERREMOVED"]._serialized_start = 1794
+    _globals["_ERC20SIGNERREMOVED"]._serialized_end = 1898
+    _globals["_ERC20THRESHOLDSET"]._serialized_start = 1900
+    _globals["_ERC20THRESHOLDSET"]._serialized_end = 2009
+    _globals["_ERC20MULTISIGEVENT"]._serialized_start = 2012
+    _globals["_ERC20MULTISIGEVENT"]._serialized_end = 2281
+    _globals["_STAKINGEVENT"]._serialized_start = 2284
+    _globals["_STAKINGEVENT"]._serialized_end = 2540
+    _globals["_STAKEDEPOSITED"]._serialized_start = 2543
+    _globals["_STAKEDEPOSITED"]._serialized_end = 2697
+    _globals["_STAKEREMOVED"]._serialized_start = 2700
+    _globals["_STAKEREMOVED"]._serialized_end = 2852
+    _globals["_STAKETOTALSUPPLY"]._serialized_start = 2854
+    _globals["_STAKETOTALSUPPLY"]._serialized_end = 2944
 # @@protoc_insertion_point(module_scope)
```

### Comparing `vega_sim-1.1.1/vega_sim/proto/vega/checkpoint/v1/checkpoint_pb2.py` & `vega_sim-1.2.0/vega_sim/proto/vega/checkpoint/v1/checkpoint_pb2.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,95 +1,107 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: vega/checkpoint/v1/checkpoint.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from ... import assets_pb2 as vega_dot_assets__pb2
 from ... import chain_events_pb2 as vega_dot_chain__events__pb2
 from ...events.v1 import events_pb2 as vega_dot_events_dot_v1_dot_events__pb2
 from ... import governance_pb2 as vega_dot_governance__pb2
+from ... import markets_pb2 as vega_dot_markets__pb2
 from ... import vega_pb2 as vega_dot_vega__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n#vega/checkpoint/v1/checkpoint.proto\x12\x12vega.checkpoint.v1\x1a\x11vega/assets.proto\x1a\x17vega/chain_events.proto\x1a\x1bvega/events/v1/events.proto\x1a\x15vega/governance.proto\x1a\x0fvega/vega.proto";\n\x0f\x43heckpointState\x12\x12\n\x04hash\x18\x01 \x01(\x0cR\x04hash\x12\x14\n\x05state\x18\x02 \x01(\x0cR\x05state"\x9f\x03\n\nCheckpoint\x12\x1e\n\ngovernance\x18\x01 \x01(\x0cR\ngovernance\x12\x16\n\x06\x61ssets\x18\x02 \x01(\x0cR\x06\x61ssets\x12\x1e\n\ncollateral\x18\x03 \x01(\x0cR\ncollateral\x12-\n\x12network_parameters\x18\x04 \x01(\x0cR\x11networkParameters\x12\x1e\n\ndelegation\x18\x05 \x01(\x0cR\ndelegation\x12\x14\n\x05\x65poch\x18\x06 \x01(\x0cR\x05\x65poch\x12\x14\n\x05\x62lock\x18\x07 \x01(\x0cR\x05\x62lock\x12\x18\n\x07rewards\x18\x08 \x01(\x0cR\x07rewards\x12\x18\n\x07\x62\x61nking\x18\t \x01(\x0cR\x07\x62\x61nking\x12\x1e\n\nvalidators\x18\n \x01(\x0cR\nvalidators\x12\x18\n\x07staking\x18\x0b \x01(\x0cR\x07staking\x12)\n\x10multisig_control\x18\x0c \x01(\x0cR\x0fmultisigControl\x12%\n\x0emarket_tracker\x18\r \x01(\x0cR\rmarketTracker"U\n\nAssetEntry\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x37\n\rasset_details\x18\x02 \x01(\x0b\x32\x12.vega.AssetDetailsR\x0c\x61ssetDetails"\x96\x01\n\x06\x41ssets\x12\x36\n\x06\x61ssets\x18\x01 \x03(\x0b\x32\x1e.vega.checkpoint.v1.AssetEntryR\x06\x61ssets\x12T\n\x16pending_listing_assets\x18\x02 \x03(\x0b\x32\x1e.vega.checkpoint.v1.AssetEntryR\x14pendingListingAssets"T\n\x0c\x41ssetBalance\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x14\n\x05\x61sset\x18\x02 \x01(\tR\x05\x61sset\x12\x18\n\x07\x62\x61lance\x18\x03 \x01(\tR\x07\x62\x61lance"J\n\nCollateral\x12<\n\x08\x62\x61lances\x18\x01 \x03(\x0b\x32 .vega.checkpoint.v1.AssetBalanceR\x08\x62\x61lances";\n\tNetParams\x12.\n\x06params\x18\x01 \x03(\x0b\x32\x16.vega.NetworkParameterR\x06params"9\n\tProposals\x12,\n\tproposals\x18\x01 \x03(\x0b\x32\x0e.vega.ProposalR\tproposals"\x8e\x01\n\rDelegateEntry\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x12\n\x04node\x18\x02 \x01(\tR\x04node\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount\x12\x1e\n\nundelegate\x18\x04 \x01(\x08R\nundelegate\x12\x1b\n\tepoch_seq\x18\x05 \x01(\x04R\x08\x65pochSeq"\xab\x01\n\x08\x44\x65legate\x12\x39\n\x06\x61\x63tive\x18\x01 \x03(\x0b\x32!.vega.checkpoint.v1.DelegateEntryR\x06\x61\x63tive\x12;\n\x07pending\x18\x02 \x03(\x0b\x32!.vega.checkpoint.v1.DelegateEntryR\x07pending\x12\'\n\x0f\x61uto_delegation\x18\x03 \x03(\tR\x0e\x61utoDelegation"\x1f\n\x05\x42lock\x12\x16\n\x06height\x18\x01 \x01(\x03R\x06height"E\n\x07Rewards\x12:\n\x07rewards\x18\x01 \x03(\x0b\x32 .vega.checkpoint.v1.RewardPayoutR\x07rewards"\x7f\n\x0cRewardPayout\x12\x1f\n\x0bpayout_time\x18\x01 \x01(\x03R\npayoutTime\x12N\n\x0erewards_payout\x18\x02 \x03(\x0b\x32\'.vega.checkpoint.v1.PendingRewardPayoutR\rrewardsPayout"\xf0\x01\n\x13PendingRewardPayout\x12!\n\x0c\x66rom_account\x18\x01 \x01(\tR\x0b\x66romAccount\x12\x14\n\x05\x61sset\x18\x02 \x01(\tR\x05\x61sset\x12\x42\n\x0cparty_amount\x18\x03 \x03(\x0b\x32\x1f.vega.checkpoint.v1.PartyAmountR\x0bpartyAmount\x12!\n\x0ctotal_reward\x18\x04 \x01(\tR\x0btotalReward\x12\x1b\n\tepoch_seq\x18\x05 \x01(\tR\x08\x65pochSeq\x12\x1c\n\ttimestamp\x18\x06 \x01(\x03R\ttimestamp";\n\x0bPartyAmount\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x16\n\x06\x61mount\x18\x02 \x01(\tR\x06\x61mount"\xb9\x01\n\x12PendingKeyRotation\x12?\n\x1crelative_target_block_height\x18\x01 \x01(\x04R\x19relativeTargetBlockHeight\x12\x17\n\x07node_id\x18\x02 \x01(\tR\x06nodeId\x12\x1e\n\x0bnew_pub_key\x18\x03 \x01(\tR\tnewPubKey\x12)\n\x11new_pub_key_index\x18\x04 \x01(\rR\x0enewPubKeyIndex"\x97\x01\n\x1aPendingEthereumKeyRotation\x12?\n\x1crelative_target_block_height\x18\x01 \x01(\x04R\x19relativeTargetBlockHeight\x12\x17\n\x07node_id\x18\x02 \x01(\tR\x06nodeId\x12\x1f\n\x0bnew_address\x18\x03 \x01(\tR\nnewAddress"\xd6\x01\n\x11ScheduledTransfer\x12*\n\x08transfer\x18\x01 \x01(\x0b\x32\x0e.vega.TransferR\x08transfer\x12\x34\n\x0c\x61\x63\x63ount_type\x18\x02 \x01(\x0e\x32\x11.vega.AccountTypeR\x0b\x61\x63\x63ountType\x12\x1c\n\treference\x18\x03 \x01(\tR\treference\x12\x41\n\x0foneoff_transfer\x18\x04 \x01(\x0b\x32\x18.vega.events.v1.TransferR\x0eoneoffTransfer"}\n\x17ScheduledTransferAtTime\x12\x1d\n\ndeliver_on\x18\x01 \x01(\x03R\tdeliverOn\x12\x43\n\ttransfers\x18\x02 \x03(\x0b\x32%.vega.checkpoint.v1.ScheduledTransferR\ttransfers"_\n\x12RecurringTransfers\x12I\n\x13recurring_transfers\x18\x01 \x03(\x0b\x32\x18.vega.events.v1.TransferR\x12recurringTransfers"\x91\x03\n\x07\x42\x61nking\x12W\n\x11transfers_at_time\x18\x01 \x03(\x0b\x32+.vega.checkpoint.v1.ScheduledTransferAtTimeR\x0ftransfersAtTime\x12W\n\x13recurring_transfers\x18\x02 \x01(\x0b\x32&.vega.checkpoint.v1.RecurringTransfersR\x12recurringTransfers\x12\x42\n\x0c\x62ridge_state\x18\x03 \x01(\x0b\x32\x1f.vega.checkpoint.v1.BridgeStateR\x0b\x62ridgeState\x12\x44\n\rasset_actions\x18\x04 \x03(\x0b\x32\x1f.vega.checkpoint.v1.AssetActionR\x0c\x61ssetActions\x12-\n\x13last_seen_eth_block\x18\x05 \x01(\x04R\x10lastSeenEthBlock\x12\x1b\n\tseen_refs\x18\x06 \x03(\tR\x08seenRefs"e\n\x0b\x42ridgeState\x12\x16\n\x06\x61\x63tive\x18\x01 \x01(\x08R\x06\x61\x63tive\x12!\n\x0c\x62lock_height\x18\x02 \x01(\x04R\x0b\x62lockHeight\x12\x1b\n\tlog_index\x18\x03 \x01(\x04R\x08logIndex"\xaa\x02\n\nValidators\x12K\n\x0fvalidator_state\x18\x01 \x03(\x0b\x32".vega.checkpoint.v1.ValidatorStateR\x0evalidatorState\x12Z\n\x15pending_key_rotations\x18\x02 \x03(\x0b\x32&.vega.checkpoint.v1.PendingKeyRotationR\x13pendingKeyRotations\x12s\n\x1epending_ethereum_key_rotations\x18\x03 \x03(\x0b\x32..vega.checkpoint.v1.PendingEthereumKeyRotationR\x1bpendingEthereumKeyRotations"\xee\x02\n\x0eValidatorState\x12J\n\x10validator_update\x18\x01 \x01(\x0b\x32\x1f.vega.events.v1.ValidatorUpdateR\x0fvalidatorUpdate\x12\x16\n\x06status\x18\x02 \x01(\x05R\x06status\x12\x30\n\x14\x65th_events_forwarded\x18\x03 \x01(\x04R\x12\x65thEventsForwarded\x12\'\n\x0fvalidator_power\x18\x04 \x01(\x03R\x0evalidatorPower\x12\x37\n\rranking_score\x18\x05 \x01(\x0b\x32\x12.vega.RankingScoreR\x0crankingScore\x12\x32\n\x15heartbeat_block_index\x18\x06 \x01(\x05R\x13heartbeatBlockIndex\x12\x30\n\x14heartbeat_block_sigs\x18\x07 \x03(\x08R\x12heartbeatBlockSigs"k\n\x07Staking\x12\x38\n\x08\x61\x63\x63\x65pted\x18\x01 \x03(\x0b\x32\x1c.vega.events.v1.StakeLinkingR\x08\x61\x63\x63\x65pted\x12&\n\x0flast_block_seen\x18\x02 \x01(\x04R\rlastBlockSeen"\xd2\x01\n\x0fMultisigControl\x12\x42\n\x07signers\x18\x01 \x03(\x0b\x32(.vega.events.v1.ERC20MultiSigSignerEventR\x07signers\x12S\n\rthreshold_set\x18\x02 \x01(\x0b\x32..vega.events.v1.ERC20MultiSigThresholdSetEventR\x0cthresholdSet\x12&\n\x0flast_block_seen\x18\x03 \x01(\x04R\rlastBlockSeen"c\n\rMarketTracker\x12R\n\x0fmarket_activity\x18\x01 \x03(\x0b\x32).vega.checkpoint.v1.MarketActivityTrackerR\x0emarketActivity"\x99\x03\n\x15MarketActivityTracker\x12\x16\n\x06market\x18\x01 \x01(\tR\x06market\x12\x14\n\x05\x61sset\x18\x02 \x01(\tR\x05\x61sset\x12M\n\x13maker_fees_received\x18\x03 \x03(\x0b\x32\x1d.vega.checkpoint.v1.PartyFeesR\x11makerFeesReceived\x12\x45\n\x0fmaker_fees_paid\x18\x04 \x03(\x0b\x32\x1d.vega.checkpoint.v1.PartyFeesR\rmakerFeesPaid\x12\x36\n\x07lp_fees\x18\x05 \x03(\x0b\x32\x1d.vega.checkpoint.v1.PartyFeesR\x06lpFees\x12\x1a\n\x08proposer\x18\x06 \x01(\tR\x08proposer\x12\x1d\n\nbonus_paid\x18\x07 \x03(\tR\tbonusPaid\x12!\n\x0cvalue_traded\x18\x08 \x01(\tR\x0bvalueTraded\x12&\n\x0fready_to_delete\x18\t \x01(\x08R\rreadyToDelete"3\n\tPartyFees\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x10\n\x03\x66\x65\x65\x18\x02 \x01(\tR\x03\x66\x65\x65"\x8d\x04\n\x0b\x41ssetAction\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x14\n\x05state\x18\x02 \x01(\rR\x05state\x12\x14\n\x05\x61sset\x18\x03 \x01(\tR\x05\x61sset\x12!\n\x0c\x62lock_number\x18\x04 \x01(\x04R\x0b\x62lockNumber\x12\x19\n\x08tx_index\x18\x05 \x01(\x04R\x07txIndex\x12\x12\n\x04hash\x18\x06 \x01(\tR\x04hash\x12\x42\n\x0f\x62uiltin_deposit\x18\x07 \x01(\x0b\x32\x19.vega.BuiltinAssetDepositR\x0e\x62uiltinDeposit\x12\x37\n\rerc20_deposit\x18\x08 \x01(\x0b\x32\x12.vega.ERC20DepositR\x0c\x65rc20Deposit\x12\x33\n\nasset_list\x18\t \x01(\x0b\x32\x14.vega.ERC20AssetListR\tassetList\x12Z\n\x1a\x65rc20_asset_limits_updated\x18\n \x01(\x0b\x32\x1d.vega.ERC20AssetLimitsUpdatedR\x17\x65rc20AssetLimitsUpdated\x12\x30\n\x14\x65rc20_bridge_stopped\x18\x0b \x01(\x08R\x12\x65rc20BridgeStopped\x12\x30\n\x14\x65rc20_bridge_resumed\x18\x0c \x01(\x08R\x12\x65rc20BridgeResumedB5Z3code.vegaprotocol.io/vega/protos/vega/checkpoint/v1b\x06proto3'
+    b'\n#vega/checkpoint/v1/checkpoint.proto\x12\x12vega.checkpoint.v1\x1a\x11vega/assets.proto\x1a\x17vega/chain_events.proto\x1a\x1bvega/events/v1/events.proto\x1a\x15vega/governance.proto\x1a\x12vega/markets.proto\x1a\x0fvega/vega.proto";\n\x0f\x43heckpointState\x12\x12\n\x04hash\x18\x01 \x01(\x0cR\x04hash\x12\x14\n\x05state\x18\x02 \x01(\x0cR\x05state"\xbd\x03\n\nCheckpoint\x12\x1e\n\ngovernance\x18\x01 \x01(\x0cR\ngovernance\x12\x16\n\x06\x61ssets\x18\x02 \x01(\x0cR\x06\x61ssets\x12\x1e\n\ncollateral\x18\x03 \x01(\x0cR\ncollateral\x12-\n\x12network_parameters\x18\x04 \x01(\x0cR\x11networkParameters\x12\x1e\n\ndelegation\x18\x05 \x01(\x0cR\ndelegation\x12\x14\n\x05\x65poch\x18\x06 \x01(\x0cR\x05\x65poch\x12\x14\n\x05\x62lock\x18\x07 \x01(\x0cR\x05\x62lock\x12\x18\n\x07rewards\x18\x08 \x01(\x0cR\x07rewards\x12\x18\n\x07\x62\x61nking\x18\t \x01(\x0cR\x07\x62\x61nking\x12\x1e\n\nvalidators\x18\n \x01(\x0cR\nvalidators\x12\x18\n\x07staking\x18\x0b \x01(\x0cR\x07staking\x12)\n\x10multisig_control\x18\x0c \x01(\x0cR\x0fmultisigControl\x12%\n\x0emarket_tracker\x18\r \x01(\x0cR\rmarketTracker\x12\x1c\n\texecution\x18\x0e \x01(\x0cR\texecution"U\n\nAssetEntry\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x37\n\rasset_details\x18\x02 \x01(\x0b\x32\x12.vega.AssetDetailsR\x0c\x61ssetDetails"\x96\x01\n\x06\x41ssets\x12\x36\n\x06\x61ssets\x18\x01 \x03(\x0b\x32\x1e.vega.checkpoint.v1.AssetEntryR\x06\x61ssets\x12T\n\x16pending_listing_assets\x18\x02 \x03(\x0b\x32\x1e.vega.checkpoint.v1.AssetEntryR\x14pendingListingAssets"T\n\x0c\x41ssetBalance\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x14\n\x05\x61sset\x18\x02 \x01(\tR\x05\x61sset\x12\x18\n\x07\x62\x61lance\x18\x03 \x01(\tR\x07\x62\x61lance"J\n\nCollateral\x12<\n\x08\x62\x61lances\x18\x01 \x03(\x0b\x32 .vega.checkpoint.v1.AssetBalanceR\x08\x62\x61lances";\n\tNetParams\x12.\n\x06params\x18\x01 \x03(\x0b\x32\x16.vega.NetworkParameterR\x06params"9\n\tProposals\x12,\n\tproposals\x18\x01 \x03(\x0b\x32\x0e.vega.ProposalR\tproposals"\x8e\x01\n\rDelegateEntry\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x12\n\x04node\x18\x02 \x01(\tR\x04node\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount\x12\x1e\n\nundelegate\x18\x04 \x01(\x08R\nundelegate\x12\x1b\n\tepoch_seq\x18\x05 \x01(\x04R\x08\x65pochSeq"\xab\x01\n\x08\x44\x65legate\x12\x39\n\x06\x61\x63tive\x18\x01 \x03(\x0b\x32!.vega.checkpoint.v1.DelegateEntryR\x06\x61\x63tive\x12;\n\x07pending\x18\x02 \x03(\x0b\x32!.vega.checkpoint.v1.DelegateEntryR\x07pending\x12\'\n\x0f\x61uto_delegation\x18\x03 \x03(\tR\x0e\x61utoDelegation"\x1f\n\x05\x42lock\x12\x16\n\x06height\x18\x01 \x01(\x03R\x06height"E\n\x07Rewards\x12:\n\x07rewards\x18\x01 \x03(\x0b\x32 .vega.checkpoint.v1.RewardPayoutR\x07rewards"\x7f\n\x0cRewardPayout\x12\x1f\n\x0bpayout_time\x18\x01 \x01(\x03R\npayoutTime\x12N\n\x0erewards_payout\x18\x02 \x03(\x0b\x32\'.vega.checkpoint.v1.PendingRewardPayoutR\rrewardsPayout"\xf0\x01\n\x13PendingRewardPayout\x12!\n\x0c\x66rom_account\x18\x01 \x01(\tR\x0b\x66romAccount\x12\x14\n\x05\x61sset\x18\x02 \x01(\tR\x05\x61sset\x12\x42\n\x0cparty_amount\x18\x03 \x03(\x0b\x32\x1f.vega.checkpoint.v1.PartyAmountR\x0bpartyAmount\x12!\n\x0ctotal_reward\x18\x04 \x01(\tR\x0btotalReward\x12\x1b\n\tepoch_seq\x18\x05 \x01(\tR\x08\x65pochSeq\x12\x1c\n\ttimestamp\x18\x06 \x01(\x03R\ttimestamp";\n\x0bPartyAmount\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x16\n\x06\x61mount\x18\x02 \x01(\tR\x06\x61mount"\xb9\x01\n\x12PendingKeyRotation\x12?\n\x1crelative_target_block_height\x18\x01 \x01(\x04R\x19relativeTargetBlockHeight\x12\x17\n\x07node_id\x18\x02 \x01(\tR\x06nodeId\x12\x1e\n\x0bnew_pub_key\x18\x03 \x01(\tR\tnewPubKey\x12)\n\x11new_pub_key_index\x18\x04 \x01(\rR\x0enewPubKeyIndex"\x97\x01\n\x1aPendingEthereumKeyRotation\x12?\n\x1crelative_target_block_height\x18\x01 \x01(\x04R\x19relativeTargetBlockHeight\x12\x17\n\x07node_id\x18\x02 \x01(\tR\x06nodeId\x12\x1f\n\x0bnew_address\x18\x03 \x01(\tR\nnewAddress"\xd6\x01\n\x11ScheduledTransfer\x12*\n\x08transfer\x18\x01 \x01(\x0b\x32\x0e.vega.TransferR\x08transfer\x12\x34\n\x0c\x61\x63\x63ount_type\x18\x02 \x01(\x0e\x32\x11.vega.AccountTypeR\x0b\x61\x63\x63ountType\x12\x1c\n\treference\x18\x03 \x01(\tR\treference\x12\x41\n\x0foneoff_transfer\x18\x04 \x01(\x0b\x32\x18.vega.events.v1.TransferR\x0eoneoffTransfer"}\n\x17ScheduledTransferAtTime\x12\x1d\n\ndeliver_on\x18\x01 \x01(\x03R\tdeliverOn\x12\x43\n\ttransfers\x18\x02 \x03(\x0b\x32%.vega.checkpoint.v1.ScheduledTransferR\ttransfers"_\n\x12RecurringTransfers\x12I\n\x13recurring_transfers\x18\x01 \x03(\x0b\x32\x18.vega.events.v1.TransferR\x12recurringTransfers"\xd1\x01\n\x12GovernanceTransfer\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1c\n\treference\x18\x02 \x01(\tR\treference\x12\x37\n\x06status\x18\x03 \x01(\x0e\x32\x1f.vega.events.v1.Transfer.StatusR\x06status\x12\x1c\n\ttimestamp\x18\x04 \x01(\x03R\ttimestamp\x12\x36\n\x06\x63onfig\x18\x05 \x01(\x0b\x32\x1e.vega.NewTransferConfigurationR\x06\x63onfig"\x88\x01\n!ScheduledGovernanceTransferAtTime\x12\x1d\n\ndeliver_on\x18\x01 \x01(\x03R\tdeliverOn\x12\x44\n\ttransfers\x18\x02 \x03(\x0b\x32&.vega.checkpoint.v1.GovernanceTransferR\ttransfers"\xf7\x04\n\x07\x42\x61nking\x12W\n\x11transfers_at_time\x18\x01 \x03(\x0b\x32+.vega.checkpoint.v1.ScheduledTransferAtTimeR\x0ftransfersAtTime\x12W\n\x13recurring_transfers\x18\x02 \x01(\x0b\x32&.vega.checkpoint.v1.RecurringTransfersR\x12recurringTransfers\x12\x42\n\x0c\x62ridge_state\x18\x03 \x01(\x0b\x32\x1f.vega.checkpoint.v1.BridgeStateR\x0b\x62ridgeState\x12\x44\n\rasset_actions\x18\x04 \x03(\x0b\x32\x1f.vega.checkpoint.v1.AssetActionR\x0c\x61ssetActions\x12-\n\x13last_seen_eth_block\x18\x05 \x01(\x04R\x10lastSeenEthBlock\x12\x1b\n\tseen_refs\x18\x06 \x03(\tR\x08seenRefs\x12v\n\x1cgovernance_transfers_at_time\x18\x07 \x03(\x0b\x32\x35.vega.checkpoint.v1.ScheduledGovernanceTransferAtTimeR\x19governanceTransfersAtTime\x12l\n\x1erecurring_governance_transfers\x18\x08 \x03(\x0b\x32&.vega.checkpoint.v1.GovernanceTransferR\x1crecurringGovernanceTransfers"e\n\x0b\x42ridgeState\x12\x16\n\x06\x61\x63tive\x18\x01 \x01(\x08R\x06\x61\x63tive\x12!\n\x0c\x62lock_height\x18\x02 \x01(\x04R\x0b\x62lockHeight\x12\x1b\n\tlog_index\x18\x03 \x01(\x04R\x08logIndex"\xaa\x02\n\nValidators\x12K\n\x0fvalidator_state\x18\x01 \x03(\x0b\x32".vega.checkpoint.v1.ValidatorStateR\x0evalidatorState\x12Z\n\x15pending_key_rotations\x18\x02 \x03(\x0b\x32&.vega.checkpoint.v1.PendingKeyRotationR\x13pendingKeyRotations\x12s\n\x1epending_ethereum_key_rotations\x18\x03 \x03(\x0b\x32..vega.checkpoint.v1.PendingEthereumKeyRotationR\x1bpendingEthereumKeyRotations"\xee\x02\n\x0eValidatorState\x12J\n\x10validator_update\x18\x01 \x01(\x0b\x32\x1f.vega.events.v1.ValidatorUpdateR\x0fvalidatorUpdate\x12\x16\n\x06status\x18\x02 \x01(\x05R\x06status\x12\x30\n\x14\x65th_events_forwarded\x18\x03 \x01(\x04R\x12\x65thEventsForwarded\x12\'\n\x0fvalidator_power\x18\x04 \x01(\x03R\x0evalidatorPower\x12\x37\n\rranking_score\x18\x05 \x01(\x0b\x32\x12.vega.RankingScoreR\x0crankingScore\x12\x32\n\x15heartbeat_block_index\x18\x06 \x01(\x05R\x13heartbeatBlockIndex\x12\x30\n\x14heartbeat_block_sigs\x18\x07 \x03(\x08R\x12heartbeatBlockSigs"k\n\x07Staking\x12\x38\n\x08\x61\x63\x63\x65pted\x18\x01 \x03(\x0b\x32\x1c.vega.events.v1.StakeLinkingR\x08\x61\x63\x63\x65pted\x12&\n\x0flast_block_seen\x18\x02 \x01(\x04R\rlastBlockSeen"\xd2\x01\n\x0fMultisigControl\x12\x42\n\x07signers\x18\x01 \x03(\x0b\x32(.vega.events.v1.ERC20MultiSigSignerEventR\x07signers\x12S\n\rthreshold_set\x18\x02 \x01(\x0b\x32..vega.events.v1.ERC20MultiSigThresholdSetEventR\x0cthresholdSet\x12&\n\x0flast_block_seen\x18\x03 \x01(\x04R\rlastBlockSeen"c\n\rMarketTracker\x12R\n\x0fmarket_activity\x18\x01 \x03(\x0b\x32).vega.checkpoint.v1.MarketActivityTrackerR\x0emarketActivity"\x99\x03\n\x15MarketActivityTracker\x12\x16\n\x06market\x18\x01 \x01(\tR\x06market\x12\x14\n\x05\x61sset\x18\x02 \x01(\tR\x05\x61sset\x12M\n\x13maker_fees_received\x18\x03 \x03(\x0b\x32\x1d.vega.checkpoint.v1.PartyFeesR\x11makerFeesReceived\x12\x45\n\x0fmaker_fees_paid\x18\x04 \x03(\x0b\x32\x1d.vega.checkpoint.v1.PartyFeesR\rmakerFeesPaid\x12\x36\n\x07lp_fees\x18\x05 \x03(\x0b\x32\x1d.vega.checkpoint.v1.PartyFeesR\x06lpFees\x12\x1a\n\x08proposer\x18\x06 \x01(\tR\x08proposer\x12\x1d\n\nbonus_paid\x18\x07 \x03(\tR\tbonusPaid\x12!\n\x0cvalue_traded\x18\x08 \x01(\tR\x0bvalueTraded\x12&\n\x0fready_to_delete\x18\t \x01(\x08R\rreadyToDelete"3\n\tPartyFees\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x10\n\x03\x66\x65\x65\x18\x02 \x01(\tR\x03\x66\x65\x65"\x8d\x04\n\x0b\x41ssetAction\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x14\n\x05state\x18\x02 \x01(\rR\x05state\x12\x14\n\x05\x61sset\x18\x03 \x01(\tR\x05\x61sset\x12!\n\x0c\x62lock_number\x18\x04 \x01(\x04R\x0b\x62lockNumber\x12\x19\n\x08tx_index\x18\x05 \x01(\x04R\x07txIndex\x12\x12\n\x04hash\x18\x06 \x01(\tR\x04hash\x12\x42\n\x0f\x62uiltin_deposit\x18\x07 \x01(\x0b\x32\x19.vega.BuiltinAssetDepositR\x0e\x62uiltinDeposit\x12\x37\n\rerc20_deposit\x18\x08 \x01(\x0b\x32\x12.vega.ERC20DepositR\x0c\x65rc20Deposit\x12\x33\n\nasset_list\x18\t \x01(\x0b\x32\x14.vega.ERC20AssetListR\tassetList\x12Z\n\x1a\x65rc20_asset_limits_updated\x18\n \x01(\x0b\x32\x1d.vega.ERC20AssetLimitsUpdatedR\x17\x65rc20AssetLimitsUpdated\x12\x30\n\x14\x65rc20_bridge_stopped\x18\x0b \x01(\x08R\x12\x65rc20BridgeStopped\x12\x30\n\x14\x65rc20_bridge_resumed\x18\x0c \x01(\x08R\x12\x65rc20BridgeResumed"\x99\x01\n\x08\x45LSShare\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12\x14\n\x05share\x18\x02 \x01(\tR\x05share\x12%\n\x0esupplied_stake\x18\x03 \x01(\tR\rsuppliedStake\x12#\n\rvirtual_stake\x18\x04 \x01(\tR\x0cvirtualStake\x12\x10\n\x03\x61vg\x18\x05 \x01(\tR\x03\x61vg"\xa9\x02\n\x0bMarketState\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x34\n\x06shares\x18\x02 \x03(\x0b\x32\x1c.vega.checkpoint.v1.ELSShareR\x06shares\x12+\n\x11insurance_balance\x18\x03 \x01(\tR\x10insuranceBalance\x12(\n\x10last_trade_value\x18\x04 \x01(\tR\x0elastTradeValue\x12*\n\x11last_trade_volume\x18\x05 \x01(\tR\x0flastTradeVolume\x12+\n\x11succession_window\x18\x06 \x01(\x03R\x10successionWindow\x12$\n\x06market\x18\x07 \x01(\x0b\x32\x0c.vega.MarketR\x06market"E\n\x0e\x45xecutionState\x12\x33\n\x04\x64\x61ta\x18\x01 \x03(\x0b\x32\x1f.vega.checkpoint.v1.MarketStateR\x04\x64\x61taB5Z3code.vegaprotocol.io/vega/protos/vega/checkpoint/v1b\x06proto3'
 )
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(
-    DESCRIPTOR, "vega.checkpoint.v1.checkpoint_pb2", globals()
+    DESCRIPTOR, "vega.checkpoint.v1.checkpoint_pb2", _globals
 )
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = (
         b"Z3code.vegaprotocol.io/vega/protos/vega/checkpoint/v1"
     )
-    _CHECKPOINTSTATE._serialized_start = 172
-    _CHECKPOINTSTATE._serialized_end = 231
-    _CHECKPOINT._serialized_start = 234
-    _CHECKPOINT._serialized_end = 649
-    _ASSETENTRY._serialized_start = 651
-    _ASSETENTRY._serialized_end = 736
-    _ASSETS._serialized_start = 739
-    _ASSETS._serialized_end = 889
-    _ASSETBALANCE._serialized_start = 891
-    _ASSETBALANCE._serialized_end = 975
-    _COLLATERAL._serialized_start = 977
-    _COLLATERAL._serialized_end = 1051
-    _NETPARAMS._serialized_start = 1053
-    _NETPARAMS._serialized_end = 1112
-    _PROPOSALS._serialized_start = 1114
-    _PROPOSALS._serialized_end = 1171
-    _DELEGATEENTRY._serialized_start = 1174
-    _DELEGATEENTRY._serialized_end = 1316
-    _DELEGATE._serialized_start = 1319
-    _DELEGATE._serialized_end = 1490
-    _BLOCK._serialized_start = 1492
-    _BLOCK._serialized_end = 1523
-    _REWARDS._serialized_start = 1525
-    _REWARDS._serialized_end = 1594
-    _REWARDPAYOUT._serialized_start = 1596
-    _REWARDPAYOUT._serialized_end = 1723
-    _PENDINGREWARDPAYOUT._serialized_start = 1726
-    _PENDINGREWARDPAYOUT._serialized_end = 1966
-    _PARTYAMOUNT._serialized_start = 1968
-    _PARTYAMOUNT._serialized_end = 2027
-    _PENDINGKEYROTATION._serialized_start = 2030
-    _PENDINGKEYROTATION._serialized_end = 2215
-    _PENDINGETHEREUMKEYROTATION._serialized_start = 2218
-    _PENDINGETHEREUMKEYROTATION._serialized_end = 2369
-    _SCHEDULEDTRANSFER._serialized_start = 2372
-    _SCHEDULEDTRANSFER._serialized_end = 2586
-    _SCHEDULEDTRANSFERATTIME._serialized_start = 2588
-    _SCHEDULEDTRANSFERATTIME._serialized_end = 2713
-    _RECURRINGTRANSFERS._serialized_start = 2715
-    _RECURRINGTRANSFERS._serialized_end = 2810
-    _BANKING._serialized_start = 2813
-    _BANKING._serialized_end = 3214
-    _BRIDGESTATE._serialized_start = 3216
-    _BRIDGESTATE._serialized_end = 3317
-    _VALIDATORS._serialized_start = 3320
-    _VALIDATORS._serialized_end = 3618
-    _VALIDATORSTATE._serialized_start = 3621
-    _VALIDATORSTATE._serialized_end = 3987
-    _STAKING._serialized_start = 3989
-    _STAKING._serialized_end = 4096
-    _MULTISIGCONTROL._serialized_start = 4099
-    _MULTISIGCONTROL._serialized_end = 4309
-    _MARKETTRACKER._serialized_start = 4311
-    _MARKETTRACKER._serialized_end = 4410
-    _MARKETACTIVITYTRACKER._serialized_start = 4413
-    _MARKETACTIVITYTRACKER._serialized_end = 4822
-    _PARTYFEES._serialized_start = 4824
-    _PARTYFEES._serialized_end = 4875
-    _ASSETACTION._serialized_start = 4878
-    _ASSETACTION._serialized_end = 5403
+    _globals["_CHECKPOINTSTATE"]._serialized_start = 192
+    _globals["_CHECKPOINTSTATE"]._serialized_end = 251
+    _globals["_CHECKPOINT"]._serialized_start = 254
+    _globals["_CHECKPOINT"]._serialized_end = 699
+    _globals["_ASSETENTRY"]._serialized_start = 701
+    _globals["_ASSETENTRY"]._serialized_end = 786
+    _globals["_ASSETS"]._serialized_start = 789
+    _globals["_ASSETS"]._serialized_end = 939
+    _globals["_ASSETBALANCE"]._serialized_start = 941
+    _globals["_ASSETBALANCE"]._serialized_end = 1025
+    _globals["_COLLATERAL"]._serialized_start = 1027
+    _globals["_COLLATERAL"]._serialized_end = 1101
+    _globals["_NETPARAMS"]._serialized_start = 1103
+    _globals["_NETPARAMS"]._serialized_end = 1162
+    _globals["_PROPOSALS"]._serialized_start = 1164
+    _globals["_PROPOSALS"]._serialized_end = 1221
+    _globals["_DELEGATEENTRY"]._serialized_start = 1224
+    _globals["_DELEGATEENTRY"]._serialized_end = 1366
+    _globals["_DELEGATE"]._serialized_start = 1369
+    _globals["_DELEGATE"]._serialized_end = 1540
+    _globals["_BLOCK"]._serialized_start = 1542
+    _globals["_BLOCK"]._serialized_end = 1573
+    _globals["_REWARDS"]._serialized_start = 1575
+    _globals["_REWARDS"]._serialized_end = 1644
+    _globals["_REWARDPAYOUT"]._serialized_start = 1646
+    _globals["_REWARDPAYOUT"]._serialized_end = 1773
+    _globals["_PENDINGREWARDPAYOUT"]._serialized_start = 1776
+    _globals["_PENDINGREWARDPAYOUT"]._serialized_end = 2016
+    _globals["_PARTYAMOUNT"]._serialized_start = 2018
+    _globals["_PARTYAMOUNT"]._serialized_end = 2077
+    _globals["_PENDINGKEYROTATION"]._serialized_start = 2080
+    _globals["_PENDINGKEYROTATION"]._serialized_end = 2265
+    _globals["_PENDINGETHEREUMKEYROTATION"]._serialized_start = 2268
+    _globals["_PENDINGETHEREUMKEYROTATION"]._serialized_end = 2419
+    _globals["_SCHEDULEDTRANSFER"]._serialized_start = 2422
+    _globals["_SCHEDULEDTRANSFER"]._serialized_end = 2636
+    _globals["_SCHEDULEDTRANSFERATTIME"]._serialized_start = 2638
+    _globals["_SCHEDULEDTRANSFERATTIME"]._serialized_end = 2763
+    _globals["_RECURRINGTRANSFERS"]._serialized_start = 2765
+    _globals["_RECURRINGTRANSFERS"]._serialized_end = 2860
+    _globals["_GOVERNANCETRANSFER"]._serialized_start = 2863
+    _globals["_GOVERNANCETRANSFER"]._serialized_end = 3072
+    _globals["_SCHEDULEDGOVERNANCETRANSFERATTIME"]._serialized_start = 3075
+    _globals["_SCHEDULEDGOVERNANCETRANSFERATTIME"]._serialized_end = 3211
+    _globals["_BANKING"]._serialized_start = 3214
+    _globals["_BANKING"]._serialized_end = 3845
+    _globals["_BRIDGESTATE"]._serialized_start = 3847
+    _globals["_BRIDGESTATE"]._serialized_end = 3948
+    _globals["_VALIDATORS"]._serialized_start = 3951
+    _globals["_VALIDATORS"]._serialized_end = 4249
+    _globals["_VALIDATORSTATE"]._serialized_start = 4252
+    _globals["_VALIDATORSTATE"]._serialized_end = 4618
+    _globals["_STAKING"]._serialized_start = 4620
+    _globals["_STAKING"]._serialized_end = 4727
+    _globals["_MULTISIGCONTROL"]._serialized_start = 4730
+    _globals["_MULTISIGCONTROL"]._serialized_end = 4940
+    _globals["_MARKETTRACKER"]._serialized_start = 4942
+    _globals["_MARKETTRACKER"]._serialized_end = 5041
+    _globals["_MARKETACTIVITYTRACKER"]._serialized_start = 5044
+    _globals["_MARKETACTIVITYTRACKER"]._serialized_end = 5453
+    _globals["_PARTYFEES"]._serialized_start = 5455
+    _globals["_PARTYFEES"]._serialized_end = 5506
+    _globals["_ASSETACTION"]._serialized_start = 5509
+    _globals["_ASSETACTION"]._serialized_end = 6034
+    _globals["_ELSSHARE"]._serialized_start = 6037
+    _globals["_ELSSHARE"]._serialized_end = 6190
+    _globals["_MARKETSTATE"]._serialized_start = 6193
+    _globals["_MARKETSTATE"]._serialized_end = 6490
+    _globals["_EXECUTIONSTATE"]._serialized_start = 6492
+    _globals["_EXECUTIONSTATE"]._serialized_end = 6561
 # @@protoc_insertion_point(module_scope)
```

### Comparing `vega_sim-1.1.1/vega_sim/proto/vega/commands/v1/__init__.py` & `vega_sim-1.2.0/vega_sim/proto/vega/commands/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/proto/vega/commands/v1/commands_pb2.py` & `vega_sim-1.2.0/vega_sim/proto/vega/commands/v1/commands_pb2.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,71 +1,80 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: vega/commands/v1/commands.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from ...commands.v1 import (
     validator_commands_pb2 as vega_dot_commands_dot_v1_dot_validator__commands__pb2,
 )
 from ... import governance_pb2 as vega_dot_governance__pb2
 from ... import vega_pb2 as vega_dot_vega__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x1fvega/commands/v1/commands.proto\x12\x10vega.commands.v1\x1a)vega/commands/v1/validator_commands.proto\x1a\x15vega/governance.proto\x1a\x0fvega/vega.proto"\xeb\x01\n\x17\x42\x61tchMarketInstructions\x12I\n\rcancellations\x18\x01 \x03(\x0b\x32#.vega.commands.v1.OrderCancellationR\rcancellations\x12@\n\namendments\x18\x02 \x03(\x0b\x32 .vega.commands.v1.OrderAmendmentR\namendments\x12\x43\n\x0bsubmissions\x18\x03 \x03(\x0b\x32!.vega.commands.v1.OrderSubmissionR\x0bsubmissions"\x8c\x03\n\x0fOrderSubmission\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x14\n\x05price\x18\x02 \x01(\tR\x05price\x12\x12\n\x04size\x18\x03 \x01(\x04R\x04size\x12\x1e\n\x04side\x18\x04 \x01(\x0e\x32\n.vega.SideR\x04side\x12;\n\rtime_in_force\x18\x05 \x01(\x0e\x32\x17.vega.Order.TimeInForceR\x0btimeInForce\x12\x1d\n\nexpires_at\x18\x06 \x01(\x03R\texpiresAt\x12$\n\x04type\x18\x07 \x01(\x0e\x32\x10.vega.Order.TypeR\x04type\x12\x1c\n\treference\x18\x08 \x01(\tR\treference\x12\x34\n\x0cpegged_order\x18\t \x01(\x0b\x32\x11.vega.PeggedOrderR\x0bpeggedOrder\x12\x1b\n\tpost_only\x18\n \x01(\x08R\x08postOnly\x12\x1f\n\x0breduce_only\x18\x0b \x01(\x08R\nreduceOnly"K\n\x11OrderCancellation\x12\x19\n\x08order_id\x18\x01 \x01(\tR\x07orderId\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId"\xe3\x02\n\x0eOrderAmendment\x12\x19\n\x08order_id\x18\x01 \x01(\tR\x07orderId\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12\x19\n\x05price\x18\x03 \x01(\tH\x00R\x05price\x88\x01\x01\x12\x1d\n\nsize_delta\x18\x04 \x01(\x03R\tsizeDelta\x12"\n\nexpires_at\x18\x05 \x01(\x03H\x01R\texpiresAt\x88\x01\x01\x12;\n\rtime_in_force\x18\x06 \x01(\x0e\x32\x17.vega.Order.TimeInForceR\x0btimeInForce\x12#\n\rpegged_offset\x18\x07 \x01(\tR\x0cpeggedOffset\x12@\n\x10pegged_reference\x18\x08 \x01(\x0e\x32\x15.vega.PeggedReferenceR\x0fpeggedReferenceB\x08\n\x06_priceB\r\n\x0b_expires_at"\xee\x01\n\x1cLiquidityProvisionSubmission\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12+\n\x11\x63ommitment_amount\x18\x02 \x01(\tR\x10\x63ommitmentAmount\x12\x10\n\x03\x66\x65\x65\x18\x03 \x01(\tR\x03\x66\x65\x65\x12*\n\x05sells\x18\x04 \x03(\x0b\x32\x14.vega.LiquidityOrderR\x05sells\x12(\n\x04\x62uys\x18\x05 \x03(\x0b\x32\x14.vega.LiquidityOrderR\x04\x62uys\x12\x1c\n\treference\x18\x06 \x01(\tR\treference"=\n\x1eLiquidityProvisionCancellation\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId"\xed\x01\n\x1bLiquidityProvisionAmendment\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12+\n\x11\x63ommitment_amount\x18\x02 \x01(\tR\x10\x63ommitmentAmount\x12\x10\n\x03\x66\x65\x65\x18\x03 \x01(\tR\x03\x66\x65\x65\x12*\n\x05sells\x18\x04 \x03(\x0b\x32\x14.vega.LiquidityOrderR\x05sells\x12(\n\x04\x62uys\x18\x05 \x03(\x0b\x32\x14.vega.LiquidityOrderR\x04\x62uys\x12\x1c\n\treference\x18\x06 \x01(\tR\treference"g\n\x12WithdrawSubmission\x12\x16\n\x06\x61mount\x18\x01 \x01(\tR\x06\x61mount\x12\x14\n\x05\x61sset\x18\x02 \x01(\tR\x05\x61sset\x12#\n\x03\x65xt\x18\x03 \x01(\x0b\x32\x11.vega.WithdrawExtR\x03\x65xt"\x94\x01\n\x12ProposalSubmission\x12\x1c\n\treference\x18\x01 \x01(\tR\treference\x12)\n\x05terms\x18\x02 \x01(\x0b\x32\x13.vega.ProposalTermsR\x05terms\x12\x35\n\trationale\x18\x03 \x01(\x0b\x32\x17.vega.ProposalRationaleR\trationale"Y\n\x0eVoteSubmission\x12\x1f\n\x0bproposal_id\x18\x01 \x01(\tR\nproposalId\x12&\n\x05value\x18\x02 \x01(\x0e\x32\x10.vega.Vote.ValueR\x05value"E\n\x12\x44\x65legateSubmission\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x16\n\x06\x61mount\x18\x02 \x01(\tR\x06\x61mount"\xe2\x01\n\x14UndelegateSubmission\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x16\n\x06\x61mount\x18\x02 \x01(\tR\x06\x61mount\x12\x45\n\x06method\x18\x03 \x01(\x0e\x32-.vega.commands.v1.UndelegateSubmission.MethodR\x06method"R\n\x06Method\x12\x16\n\x12METHOD_UNSPECIFIED\x10\x00\x12\x0e\n\nMETHOD_NOW\x10\x01\x12\x1a\n\x16METHOD_AT_END_OF_EPOCH\x10\x02"\x04\x08\x03\x10\x03"\xea\x02\n\x08Transfer\x12=\n\x11\x66rom_account_type\x18\x01 \x01(\x0e\x32\x11.vega.AccountTypeR\x0f\x66romAccountType\x12\x0e\n\x02to\x18\x02 \x01(\tR\x02to\x12\x39\n\x0fto_account_type\x18\x03 \x01(\x0e\x32\x11.vega.AccountTypeR\rtoAccountType\x12\x14\n\x05\x61sset\x18\x04 \x01(\tR\x05\x61sset\x12\x16\n\x06\x61mount\x18\x05 \x01(\tR\x06\x61mount\x12\x1c\n\treference\x18\x06 \x01(\tR\treference\x12;\n\x07one_off\x18\x65 \x01(\x0b\x32 .vega.commands.v1.OneOffTransferH\x00R\x06oneOff\x12\x43\n\trecurring\x18\x66 \x01(\x0b\x32#.vega.commands.v1.RecurringTransferH\x00R\trecurringB\x06\n\x04kind"/\n\x0eOneOffTransfer\x12\x1d\n\ndeliver_on\x18\x01 \x01(\x03R\tdeliverOn"\xc1\x01\n\x11RecurringTransfer\x12\x1f\n\x0bstart_epoch\x18\x01 \x01(\x04R\nstartEpoch\x12 \n\tend_epoch\x18\x02 \x01(\x04H\x00R\x08\x65ndEpoch\x88\x01\x01\x12\x16\n\x06\x66\x61\x63tor\x18\x03 \x01(\tR\x06\x66\x61\x63tor\x12\x43\n\x11\x64ispatch_strategy\x18\x04 \x01(\x0b\x32\x16.vega.DispatchStrategyR\x10\x64ispatchStrategyB\x0c\n\n_end_epoch"1\n\x0e\x43\x61ncelTransfer\x12\x1f\n\x0btransfer_id\x18\x01 \x01(\tR\ntransferId"\x94\x01\n\x0fIssueSignatures\x12\x1c\n\tsubmitter\x18\x01 \x01(\tR\tsubmitter\x12\x37\n\x04kind\x18\x02 \x01(\x0e\x32#.vega.commands.v1.NodeSignatureKindR\x04kind\x12*\n\x11validator_node_id\x18\x03 \x01(\tR\x0fvalidatorNodeIdB3Z1code.vegaprotocol.io/vega/protos/vega/commands/v1b\x06proto3'
+    b'\n\x1fvega/commands/v1/commands.proto\x12\x10vega.commands.v1\x1a)vega/commands/v1/validator_commands.proto\x1a\x15vega/governance.proto\x1a\x0fvega/vega.proto"\xad\x03\n\x17\x42\x61tchMarketInstructions\x12I\n\rcancellations\x18\x01 \x03(\x0b\x32#.vega.commands.v1.OrderCancellationR\rcancellations\x12@\n\namendments\x18\x02 \x03(\x0b\x32 .vega.commands.v1.OrderAmendmentR\namendments\x12\x43\n\x0bsubmissions\x18\x03 \x03(\x0b\x32!.vega.commands.v1.OrderSubmissionR\x0bsubmissions\x12\x62\n\x18stop_orders_cancellation\x18\x04 \x03(\x0b\x32(.vega.commands.v1.StopOrdersCancellationR\x16stopOrdersCancellation\x12\\\n\x16stop_orders_submission\x18\x05 \x03(\x0b\x32&.vega.commands.v1.StopOrdersSubmissionR\x14stopOrdersSubmission"\xc6\x01\n\x14StopOrdersSubmission\x12\x46\n\x0brises_above\x18\x01 \x01(\x0b\x32 .vega.commands.v1.StopOrderSetupH\x00R\nrisesAbove\x88\x01\x01\x12\x46\n\x0b\x66\x61lls_below\x18\x02 \x01(\x0b\x32 .vega.commands.v1.StopOrderSetupH\x01R\nfallsBelow\x88\x01\x01\x42\x0e\n\x0c_rises_aboveB\x0e\n\x0c_falls_below"\xd0\x02\n\x0eStopOrderSetup\x12L\n\x10order_submission\x18\x01 \x01(\x0b\x32!.vega.commands.v1.OrderSubmissionR\x0forderSubmission\x12"\n\nexpires_at\x18\x02 \x01(\x03H\x01R\texpiresAt\x88\x01\x01\x12L\n\x0f\x65xpiry_strategy\x18\x03 \x01(\x0e\x32\x1e.vega.StopOrder.ExpiryStrategyH\x02R\x0e\x65xpiryStrategy\x88\x01\x01\x12\x16\n\x05price\x18\x64 \x01(\tH\x00R\x05price\x12\x38\n\x17trailing_percent_offset\x18\x65 \x01(\tH\x00R\x15trailingPercentOffsetB\t\n\x07triggerB\r\n\x0b_expires_atB\x12\n\x10_expiry_strategy"\x83\x01\n\x16StopOrdersCancellation\x12 \n\tmarket_id\x18\x01 \x01(\tH\x00R\x08marketId\x88\x01\x01\x12\'\n\rstop_order_id\x18\x02 \x01(\tH\x01R\x0bstopOrderId\x88\x01\x01\x42\x0c\n\n_market_idB\x10\n\x0e_stop_order_id"\xe4\x03\n\x0fOrderSubmission\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x14\n\x05price\x18\x02 \x01(\tR\x05price\x12\x12\n\x04size\x18\x03 \x01(\x04R\x04size\x12\x1e\n\x04side\x18\x04 \x01(\x0e\x32\n.vega.SideR\x04side\x12;\n\rtime_in_force\x18\x05 \x01(\x0e\x32\x17.vega.Order.TimeInForceR\x0btimeInForce\x12\x1d\n\nexpires_at\x18\x06 \x01(\x03R\texpiresAt\x12$\n\x04type\x18\x07 \x01(\x0e\x32\x10.vega.Order.TypeR\x04type\x12\x1c\n\treference\x18\x08 \x01(\tR\treference\x12\x34\n\x0cpegged_order\x18\t \x01(\x0b\x32\x11.vega.PeggedOrderR\x0bpeggedOrder\x12\x1b\n\tpost_only\x18\n \x01(\x08R\x08postOnly\x12\x1f\n\x0breduce_only\x18\x0b \x01(\x08R\nreduceOnly\x12\x45\n\x0ciceberg_opts\x18\x0c \x01(\x0b\x32\x1d.vega.commands.v1.IcebergOptsH\x00R\x0bicebergOpts\x88\x01\x01\x42\x0f\n\r_iceberg_opts"\\\n\x0bIcebergOpts\x12\x1b\n\tpeak_size\x18\x01 \x01(\x04R\x08peakSize\x12\x30\n\x14minimum_visible_size\x18\x02 \x01(\x04R\x12minimumVisibleSize"K\n\x11OrderCancellation\x12\x19\n\x08order_id\x18\x01 \x01(\tR\x07orderId\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId"\xe3\x02\n\x0eOrderAmendment\x12\x19\n\x08order_id\x18\x01 \x01(\tR\x07orderId\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12\x19\n\x05price\x18\x03 \x01(\tH\x00R\x05price\x88\x01\x01\x12\x1d\n\nsize_delta\x18\x04 \x01(\x03R\tsizeDelta\x12"\n\nexpires_at\x18\x05 \x01(\x03H\x01R\texpiresAt\x88\x01\x01\x12;\n\rtime_in_force\x18\x06 \x01(\x0e\x32\x17.vega.Order.TimeInForceR\x0btimeInForce\x12#\n\rpegged_offset\x18\x07 \x01(\tR\x0cpeggedOffset\x12@\n\x10pegged_reference\x18\x08 \x01(\x0e\x32\x15.vega.PeggedReferenceR\x0fpeggedReferenceB\x08\n\x06_priceB\r\n\x0b_expires_at"\xee\x01\n\x1cLiquidityProvisionSubmission\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12+\n\x11\x63ommitment_amount\x18\x02 \x01(\tR\x10\x63ommitmentAmount\x12\x10\n\x03\x66\x65\x65\x18\x03 \x01(\tR\x03\x66\x65\x65\x12*\n\x05sells\x18\x04 \x03(\x0b\x32\x14.vega.LiquidityOrderR\x05sells\x12(\n\x04\x62uys\x18\x05 \x03(\x0b\x32\x14.vega.LiquidityOrderR\x04\x62uys\x12\x1c\n\treference\x18\x06 \x01(\tR\treference"=\n\x1eLiquidityProvisionCancellation\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId"\xed\x01\n\x1bLiquidityProvisionAmendment\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12+\n\x11\x63ommitment_amount\x18\x02 \x01(\tR\x10\x63ommitmentAmount\x12\x10\n\x03\x66\x65\x65\x18\x03 \x01(\tR\x03\x66\x65\x65\x12*\n\x05sells\x18\x04 \x03(\x0b\x32\x14.vega.LiquidityOrderR\x05sells\x12(\n\x04\x62uys\x18\x05 \x03(\x0b\x32\x14.vega.LiquidityOrderR\x04\x62uys\x12\x1c\n\treference\x18\x06 \x01(\tR\treference"g\n\x12WithdrawSubmission\x12\x16\n\x06\x61mount\x18\x01 \x01(\tR\x06\x61mount\x12\x14\n\x05\x61sset\x18\x02 \x01(\tR\x05\x61sset\x12#\n\x03\x65xt\x18\x03 \x01(\x0b\x32\x11.vega.WithdrawExtR\x03\x65xt"\x94\x01\n\x12ProposalSubmission\x12\x1c\n\treference\x18\x01 \x01(\tR\treference\x12)\n\x05terms\x18\x02 \x01(\x0b\x32\x13.vega.ProposalTermsR\x05terms\x12\x35\n\trationale\x18\x03 \x01(\x0b\x32\x17.vega.ProposalRationaleR\trationale"Y\n\x0eVoteSubmission\x12\x1f\n\x0bproposal_id\x18\x01 \x01(\tR\nproposalId\x12&\n\x05value\x18\x02 \x01(\x0e\x32\x10.vega.Vote.ValueR\x05value"E\n\x12\x44\x65legateSubmission\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x16\n\x06\x61mount\x18\x02 \x01(\tR\x06\x61mount"\xe2\x01\n\x14UndelegateSubmission\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x16\n\x06\x61mount\x18\x02 \x01(\tR\x06\x61mount\x12\x45\n\x06method\x18\x03 \x01(\x0e\x32-.vega.commands.v1.UndelegateSubmission.MethodR\x06method"R\n\x06Method\x12\x16\n\x12METHOD_UNSPECIFIED\x10\x00\x12\x0e\n\nMETHOD_NOW\x10\x01\x12\x1a\n\x16METHOD_AT_END_OF_EPOCH\x10\x02"\x04\x08\x03\x10\x03"\xea\x02\n\x08Transfer\x12=\n\x11\x66rom_account_type\x18\x01 \x01(\x0e\x32\x11.vega.AccountTypeR\x0f\x66romAccountType\x12\x0e\n\x02to\x18\x02 \x01(\tR\x02to\x12\x39\n\x0fto_account_type\x18\x03 \x01(\x0e\x32\x11.vega.AccountTypeR\rtoAccountType\x12\x14\n\x05\x61sset\x18\x04 \x01(\tR\x05\x61sset\x12\x16\n\x06\x61mount\x18\x05 \x01(\tR\x06\x61mount\x12\x1c\n\treference\x18\x06 \x01(\tR\treference\x12;\n\x07one_off\x18\x65 \x01(\x0b\x32 .vega.commands.v1.OneOffTransferH\x00R\x06oneOff\x12\x43\n\trecurring\x18\x66 \x01(\x0b\x32#.vega.commands.v1.RecurringTransferH\x00R\trecurringB\x06\n\x04kind"/\n\x0eOneOffTransfer\x12\x1d\n\ndeliver_on\x18\x01 \x01(\x03R\tdeliverOn"\xc1\x01\n\x11RecurringTransfer\x12\x1f\n\x0bstart_epoch\x18\x01 \x01(\x04R\nstartEpoch\x12 \n\tend_epoch\x18\x02 \x01(\x04H\x00R\x08\x65ndEpoch\x88\x01\x01\x12\x16\n\x06\x66\x61\x63tor\x18\x03 \x01(\tR\x06\x66\x61\x63tor\x12\x43\n\x11\x64ispatch_strategy\x18\x04 \x01(\x0b\x32\x16.vega.DispatchStrategyR\x10\x64ispatchStrategyB\x0c\n\n_end_epoch"1\n\x0e\x43\x61ncelTransfer\x12\x1f\n\x0btransfer_id\x18\x01 \x01(\tR\ntransferId"\x94\x01\n\x0fIssueSignatures\x12\x1c\n\tsubmitter\x18\x01 \x01(\tR\tsubmitter\x12\x37\n\x04kind\x18\x02 \x01(\x0e\x32#.vega.commands.v1.NodeSignatureKindR\x04kind\x12*\n\x11validator_node_id\x18\x03 \x01(\tR\x0fvalidatorNodeIdB3Z1code.vegaprotocol.io/vega/protos/vega/commands/v1b\x06proto3'
 )
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(
-    DESCRIPTOR, "vega.commands.v1.commands_pb2", globals()
+    DESCRIPTOR, "vega.commands.v1.commands_pb2", _globals
 )
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = (
         b"Z1code.vegaprotocol.io/vega/protos/vega/commands/v1"
     )
-    _BATCHMARKETINSTRUCTIONS._serialized_start = 137
-    _BATCHMARKETINSTRUCTIONS._serialized_end = 372
-    _ORDERSUBMISSION._serialized_start = 375
-    _ORDERSUBMISSION._serialized_end = 771
-    _ORDERCANCELLATION._serialized_start = 773
-    _ORDERCANCELLATION._serialized_end = 848
-    _ORDERAMENDMENT._serialized_start = 851
-    _ORDERAMENDMENT._serialized_end = 1206
-    _LIQUIDITYPROVISIONSUBMISSION._serialized_start = 1209
-    _LIQUIDITYPROVISIONSUBMISSION._serialized_end = 1447
-    _LIQUIDITYPROVISIONCANCELLATION._serialized_start = 1449
-    _LIQUIDITYPROVISIONCANCELLATION._serialized_end = 1510
-    _LIQUIDITYPROVISIONAMENDMENT._serialized_start = 1513
-    _LIQUIDITYPROVISIONAMENDMENT._serialized_end = 1750
-    _WITHDRAWSUBMISSION._serialized_start = 1752
-    _WITHDRAWSUBMISSION._serialized_end = 1855
-    _PROPOSALSUBMISSION._serialized_start = 1858
-    _PROPOSALSUBMISSION._serialized_end = 2006
-    _VOTESUBMISSION._serialized_start = 2008
-    _VOTESUBMISSION._serialized_end = 2097
-    _DELEGATESUBMISSION._serialized_start = 2099
-    _DELEGATESUBMISSION._serialized_end = 2168
-    _UNDELEGATESUBMISSION._serialized_start = 2171
-    _UNDELEGATESUBMISSION._serialized_end = 2397
-    _UNDELEGATESUBMISSION_METHOD._serialized_start = 2315
-    _UNDELEGATESUBMISSION_METHOD._serialized_end = 2397
-    _TRANSFER._serialized_start = 2400
-    _TRANSFER._serialized_end = 2762
-    _ONEOFFTRANSFER._serialized_start = 2764
-    _ONEOFFTRANSFER._serialized_end = 2811
-    _RECURRINGTRANSFER._serialized_start = 2814
-    _RECURRINGTRANSFER._serialized_end = 3007
-    _CANCELTRANSFER._serialized_start = 3009
-    _CANCELTRANSFER._serialized_end = 3058
-    _ISSUESIGNATURES._serialized_start = 3061
-    _ISSUESIGNATURES._serialized_end = 3209
+    _globals["_BATCHMARKETINSTRUCTIONS"]._serialized_start = 137
+    _globals["_BATCHMARKETINSTRUCTIONS"]._serialized_end = 566
+    _globals["_STOPORDERSSUBMISSION"]._serialized_start = 569
+    _globals["_STOPORDERSSUBMISSION"]._serialized_end = 767
+    _globals["_STOPORDERSETUP"]._serialized_start = 770
+    _globals["_STOPORDERSETUP"]._serialized_end = 1106
+    _globals["_STOPORDERSCANCELLATION"]._serialized_start = 1109
+    _globals["_STOPORDERSCANCELLATION"]._serialized_end = 1240
+    _globals["_ORDERSUBMISSION"]._serialized_start = 1243
+    _globals["_ORDERSUBMISSION"]._serialized_end = 1727
+    _globals["_ICEBERGOPTS"]._serialized_start = 1729
+    _globals["_ICEBERGOPTS"]._serialized_end = 1821
+    _globals["_ORDERCANCELLATION"]._serialized_start = 1823
+    _globals["_ORDERCANCELLATION"]._serialized_end = 1898
+    _globals["_ORDERAMENDMENT"]._serialized_start = 1901
+    _globals["_ORDERAMENDMENT"]._serialized_end = 2256
+    _globals["_LIQUIDITYPROVISIONSUBMISSION"]._serialized_start = 2259
+    _globals["_LIQUIDITYPROVISIONSUBMISSION"]._serialized_end = 2497
+    _globals["_LIQUIDITYPROVISIONCANCELLATION"]._serialized_start = 2499
+    _globals["_LIQUIDITYPROVISIONCANCELLATION"]._serialized_end = 2560
+    _globals["_LIQUIDITYPROVISIONAMENDMENT"]._serialized_start = 2563
+    _globals["_LIQUIDITYPROVISIONAMENDMENT"]._serialized_end = 2800
+    _globals["_WITHDRAWSUBMISSION"]._serialized_start = 2802
+    _globals["_WITHDRAWSUBMISSION"]._serialized_end = 2905
+    _globals["_PROPOSALSUBMISSION"]._serialized_start = 2908
+    _globals["_PROPOSALSUBMISSION"]._serialized_end = 3056
+    _globals["_VOTESUBMISSION"]._serialized_start = 3058
+    _globals["_VOTESUBMISSION"]._serialized_end = 3147
+    _globals["_DELEGATESUBMISSION"]._serialized_start = 3149
+    _globals["_DELEGATESUBMISSION"]._serialized_end = 3218
+    _globals["_UNDELEGATESUBMISSION"]._serialized_start = 3221
+    _globals["_UNDELEGATESUBMISSION"]._serialized_end = 3447
+    _globals["_UNDELEGATESUBMISSION_METHOD"]._serialized_start = 3365
+    _globals["_UNDELEGATESUBMISSION_METHOD"]._serialized_end = 3447
+    _globals["_TRANSFER"]._serialized_start = 3450
+    _globals["_TRANSFER"]._serialized_end = 3812
+    _globals["_ONEOFFTRANSFER"]._serialized_start = 3814
+    _globals["_ONEOFFTRANSFER"]._serialized_end = 3861
+    _globals["_RECURRINGTRANSFER"]._serialized_start = 3864
+    _globals["_RECURRINGTRANSFER"]._serialized_end = 4057
+    _globals["_CANCELTRANSFER"]._serialized_start = 4059
+    _globals["_CANCELTRANSFER"]._serialized_end = 4108
+    _globals["_ISSUESIGNATURES"]._serialized_start = 4111
+    _globals["_ISSUESIGNATURES"]._serialized_end = 4259
 # @@protoc_insertion_point(module_scope)
```

### Comparing `vega_sim-1.1.1/vega_sim/proto/vega/commands/v1/data_pb2.py` & `vega_sim-1.2.0/vega_sim/proto/vega/commands/v1/signature_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: vega/commands/v1/data.proto
+# source: vega/commands/v1/signature.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x1bvega/commands/v1/data.proto\x12\x10vega.commands.v1"\xe3\x01\n\x14OracleDataSubmission\x12K\n\x06source\x18\x01 \x01(\x0e\x32\x33.vega.commands.v1.OracleDataSubmission.OracleSourceR\x06source\x12\x18\n\x07payload\x18\x02 \x01(\x0cR\x07payload"d\n\x0cOracleSource\x12\x1d\n\x19ORACLE_SOURCE_UNSPECIFIED\x10\x00\x12\x1d\n\x19ORACLE_SOURCE_OPEN_ORACLE\x10\x01\x12\x16\n\x12ORACLE_SOURCE_JSON\x10\x02\x42\x33Z1code.vegaprotocol.io/vega/protos/vega/commands/v1b\x06proto3'
+    b'\n vega/commands/v1/signature.proto\x12\x10vega.commands.v1"O\n\tSignature\x12\x14\n\x05value\x18\x01 \x01(\tR\x05value\x12\x12\n\x04\x61lgo\x18\x02 \x01(\tR\x04\x61lgo\x12\x18\n\x07version\x18\x03 \x01(\rR\x07versionB3Z1code.vegaprotocol.io/vega/protos/vega/commands/v1b\x06proto3'
 )
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(
-    DESCRIPTOR, "vega.commands.v1.data_pb2", globals()
+    DESCRIPTOR, "vega.commands.v1.signature_pb2", _globals
 )
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = (
         b"Z1code.vegaprotocol.io/vega/protos/vega/commands/v1"
     )
-    _ORACLEDATASUBMISSION._serialized_start = 50
-    _ORACLEDATASUBMISSION._serialized_end = 277
-    _ORACLEDATASUBMISSION_ORACLESOURCE._serialized_start = 177
-    _ORACLEDATASUBMISSION_ORACLESOURCE._serialized_end = 277
+    _globals["_SIGNATURE"]._serialized_start = 54
+    _globals["_SIGNATURE"]._serialized_end = 133
 # @@protoc_insertion_point(module_scope)
```

### Comparing `vega_sim-1.1.1/vega_sim/proto/vega/commands/v1/signature_pb2.py` & `vega_sim-1.2.0/vega_sim/proto/vega/oracle_pb2.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: vega/commands/v1/signature.proto
+# source: vega/oracle.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from .data.v1 import data_pb2 as vega_dot_data_dot_v1_dot_data__pb2
+from . import data_source_pb2 as vega_dot_data__source__pb2
+
+
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n vega/commands/v1/signature.proto\x12\x10vega.commands.v1"O\n\tSignature\x12\x14\n\x05value\x18\x01 \x01(\tR\x05value\x12\x12\n\x04\x61lgo\x18\x02 \x01(\tR\x04\x61lgo\x12\x18\n\x07version\x18\x03 \x01(\rR\x07versionB3Z1code.vegaprotocol.io/vega/protos/vega/commands/v1b\x06proto3'
+    b'\n\x11vega/oracle.proto\x12\x04vega\x1a\x17vega/data/v1/data.proto\x1a\x16vega/data_source.proto"e\n\nOracleSpec\x12W\n\x19\x65xternal_data_source_spec\x18\x01 \x01(\x0b\x32\x1c.vega.ExternalDataSourceSpecR\x16\x65xternalDataSourceSpec"M\n\nOracleData\x12?\n\rexternal_data\x18\x01 \x01(\x0b\x32\x1a.vega.data.v1.ExternalDataR\x0c\x65xternalDataB\'Z%code.vegaprotocol.io/vega/protos/vegab\x06proto3'
 )
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(
-    DESCRIPTOR, "vega.commands.v1.signature_pb2", globals()
-)
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "vega.oracle_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    DESCRIPTOR._serialized_options = (
-        b"Z1code.vegaprotocol.io/vega/protos/vega/commands/v1"
-    )
-    _SIGNATURE._serialized_start = 54
-    _SIGNATURE._serialized_end = 133
+    DESCRIPTOR._serialized_options = b"Z%code.vegaprotocol.io/vega/protos/vega"
+    _globals["_ORACLESPEC"]._serialized_start = 76
+    _globals["_ORACLESPEC"]._serialized_end = 177
+    _globals["_ORACLEDATA"]._serialized_start = 179
+    _globals["_ORACLEDATA"]._serialized_end = 256
 # @@protoc_insertion_point(module_scope)
```

### Comparing `vega_sim-1.1.1/vega_sim/proto/vega/commands/v1/transaction_pb2.py` & `vega_sim-1.2.0/vega_sim/proto/vega/commands/v1/transaction_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: vega/commands/v1/transaction.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from ...commands.v1 import commands_pb2 as vega_dot_commands_dot_v1_dot_commands__pb2
@@ -17,28 +17,29 @@
 from ...commands.v1 import signature_pb2 as vega_dot_commands_dot_v1_dot_signature__pb2
 from ...commands.v1 import (
     validator_commands_pb2 as vega_dot_commands_dot_v1_dot_validator__commands__pb2,
 )
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n"vega/commands/v1/transaction.proto\x12\x10vega.commands.v1\x1a\x1fvega/commands/v1/commands.proto\x1a\x1bvega/commands/v1/data.proto\x1a vega/commands/v1/signature.proto\x1a)vega/commands/v1/validator_commands.proto"\xaa\x12\n\tInputData\x12\x14\n\x05nonce\x18\x01 \x01(\x04R\x05nonce\x12!\n\x0c\x62lock_height\x18\x02 \x01(\x04R\x0b\x62lockHeight\x12O\n\x10order_submission\x18\xe9\x07 \x01(\x0b\x32!.vega.commands.v1.OrderSubmissionH\x00R\x0forderSubmission\x12U\n\x12order_cancellation\x18\xea\x07 \x01(\x0b\x32#.vega.commands.v1.OrderCancellationH\x00R\x11orderCancellation\x12L\n\x0forder_amendment\x18\xeb\x07 \x01(\x0b\x32 .vega.commands.v1.OrderAmendmentH\x00R\x0eorderAmendment\x12X\n\x13withdraw_submission\x18\xec\x07 \x01(\x0b\x32$.vega.commands.v1.WithdrawSubmissionH\x00R\x12withdrawSubmission\x12X\n\x13proposal_submission\x18\xed\x07 \x01(\x0b\x32$.vega.commands.v1.ProposalSubmissionH\x00R\x12proposalSubmission\x12L\n\x0fvote_submission\x18\xee\x07 \x01(\x0b\x32 .vega.commands.v1.VoteSubmissionH\x00R\x0evoteSubmission\x12w\n\x1eliquidity_provision_submission\x18\xef\x07 \x01(\x0b\x32..vega.commands.v1.LiquidityProvisionSubmissionH\x00R\x1cliquidityProvisionSubmission\x12X\n\x13\x64\x65legate_submission\x18\xf0\x07 \x01(\x0b\x32$.vega.commands.v1.DelegateSubmissionH\x00R\x12\x64\x65legateSubmission\x12^\n\x15undelegate_submission\x18\xf1\x07 \x01(\x0b\x32&.vega.commands.v1.UndelegateSubmissionH\x00R\x14undelegateSubmission\x12}\n liquidity_provision_cancellation\x18\xf2\x07 \x01(\x0b\x32\x30.vega.commands.v1.LiquidityProvisionCancellationH\x00R\x1eliquidityProvisionCancellation\x12t\n\x1dliquidity_provision_amendment\x18\xf3\x07 \x01(\x0b\x32-.vega.commands.v1.LiquidityProvisionAmendmentH\x00R\x1bliquidityProvisionAmendment\x12\x39\n\x08transfer\x18\xf4\x07 \x01(\x0b\x32\x1a.vega.commands.v1.TransferH\x00R\x08transfer\x12L\n\x0f\x63\x61ncel_transfer\x18\xf5\x07 \x01(\x0b\x32 .vega.commands.v1.CancelTransferH\x00R\x0e\x63\x61ncelTransfer\x12\x46\n\rannounce_node\x18\xf6\x07 \x01(\x0b\x32\x1e.vega.commands.v1.AnnounceNodeH\x00R\x0c\x61nnounceNode\x12h\n\x19\x62\x61tch_market_instructions\x18\xf7\x07 \x01(\x0b\x32).vega.commands.v1.BatchMarketInstructionsH\x00R\x17\x62\x61tchMarketInstructions\x12:\n\tnode_vote\x18\xd2\x0f \x01(\x0b\x32\x1a.vega.commands.v1.NodeVoteH\x00R\x08nodeVote\x12I\n\x0enode_signature\x18\xd3\x0f \x01(\x0b\x32\x1f.vega.commands.v1.NodeSignatureH\x00R\rnodeSignature\x12@\n\x0b\x63hain_event\x18\xd4\x0f \x01(\x0b\x32\x1c.vega.commands.v1.ChainEventH\x00R\nchainEvent\x12\\\n\x15key_rotate_submission\x18\xd5\x0f \x01(\x0b\x32%.vega.commands.v1.KeyRotateSubmissionH\x00R\x13keyRotateSubmission\x12\x62\n\x17state_variable_proposal\x18\xd6\x0f \x01(\x0b\x32\'.vega.commands.v1.StateVariableProposalH\x00R\x15stateVariableProposal\x12X\n\x13validator_heartbeat\x18\xd7\x0f \x01(\x0b\x32$.vega.commands.v1.ValidatorHeartbeatH\x00R\x12validatorHeartbeat\x12u\n\x1e\x65thereum_key_rotate_submission\x18\xd8\x0f \x01(\x0b\x32-.vega.commands.v1.EthereumKeyRotateSubmissionH\x00R\x1b\x65thereumKeyRotateSubmission\x12h\n\x19protocol_upgrade_proposal\x18\xd9\x0f \x01(\x0b\x32).vega.commands.v1.ProtocolUpgradeProposalH\x00R\x17protocolUpgradeProposal\x12O\n\x10issue_signatures\x18\xda\x0f \x01(\x0b\x32!.vega.commands.v1.IssueSignaturesH\x00R\x0fissueSignatures\x12_\n\x16oracle_data_submission\x18\xb9\x17 \x01(\x0b\x32&.vega.commands.v1.OracleDataSubmissionH\x00R\x14oracleDataSubmissionB\t\n\x07\x63ommandJ\x06\x08\xa1\x1f\x10\xa2\x1f"\x92\x02\n\x0bTransaction\x12\x1d\n\ninput_data\x18\x01 \x01(\x0cR\tinputData\x12\x39\n\tsignature\x18\x02 \x01(\x0b\x32\x1b.vega.commands.v1.SignatureR\tsignature\x12\x1b\n\x07\x61\x64\x64ress\x18\xe9\x07 \x01(\tH\x00R\x07\x61\x64\x64ress\x12\x1a\n\x07pub_key\x18\xea\x07 \x01(\tH\x00R\x06pubKey\x12\x36\n\x07version\x18\xd0\x0f \x01(\x0e\x32\x1b.vega.commands.v1.TxVersionR\x07version\x12\x30\n\x03pow\x18\xb8\x17 \x01(\x0b\x32\x1d.vega.commands.v1.ProofOfWorkR\x03powB\x06\n\x04\x66rom"5\n\x0bProofOfWork\x12\x10\n\x03tid\x18\x01 \x01(\tR\x03tid\x12\x14\n\x05nonce\x18\x02 \x01(\x04R\x05nonce*S\n\tTxVersion\x12\x1a\n\x16TX_VERSION_UNSPECIFIED\x10\x00\x12\x11\n\rTX_VERSION_V2\x10\x02\x12\x11\n\rTX_VERSION_V3\x10\x03"\x04\x08\x01\x10\x01\x42\x33Z1code.vegaprotocol.io/vega/protos/vega/commands/v1b\x06proto3'
+    b'\n"vega/commands/v1/transaction.proto\x12\x10vega.commands.v1\x1a\x1fvega/commands/v1/commands.proto\x1a\x1bvega/commands/v1/data.proto\x1a vega/commands/v1/signature.proto\x1a)vega/commands/v1/validator_commands.proto"\xf2\x13\n\tInputData\x12\x14\n\x05nonce\x18\x01 \x01(\x04R\x05nonce\x12!\n\x0c\x62lock_height\x18\x02 \x01(\x04R\x0b\x62lockHeight\x12O\n\x10order_submission\x18\xe9\x07 \x01(\x0b\x32!.vega.commands.v1.OrderSubmissionH\x00R\x0forderSubmission\x12U\n\x12order_cancellation\x18\xea\x07 \x01(\x0b\x32#.vega.commands.v1.OrderCancellationH\x00R\x11orderCancellation\x12L\n\x0forder_amendment\x18\xeb\x07 \x01(\x0b\x32 .vega.commands.v1.OrderAmendmentH\x00R\x0eorderAmendment\x12X\n\x13withdraw_submission\x18\xec\x07 \x01(\x0b\x32$.vega.commands.v1.WithdrawSubmissionH\x00R\x12withdrawSubmission\x12X\n\x13proposal_submission\x18\xed\x07 \x01(\x0b\x32$.vega.commands.v1.ProposalSubmissionH\x00R\x12proposalSubmission\x12L\n\x0fvote_submission\x18\xee\x07 \x01(\x0b\x32 .vega.commands.v1.VoteSubmissionH\x00R\x0evoteSubmission\x12w\n\x1eliquidity_provision_submission\x18\xef\x07 \x01(\x0b\x32..vega.commands.v1.LiquidityProvisionSubmissionH\x00R\x1cliquidityProvisionSubmission\x12X\n\x13\x64\x65legate_submission\x18\xf0\x07 \x01(\x0b\x32$.vega.commands.v1.DelegateSubmissionH\x00R\x12\x64\x65legateSubmission\x12^\n\x15undelegate_submission\x18\xf1\x07 \x01(\x0b\x32&.vega.commands.v1.UndelegateSubmissionH\x00R\x14undelegateSubmission\x12}\n liquidity_provision_cancellation\x18\xf2\x07 \x01(\x0b\x32\x30.vega.commands.v1.LiquidityProvisionCancellationH\x00R\x1eliquidityProvisionCancellation\x12t\n\x1dliquidity_provision_amendment\x18\xf3\x07 \x01(\x0b\x32-.vega.commands.v1.LiquidityProvisionAmendmentH\x00R\x1bliquidityProvisionAmendment\x12\x39\n\x08transfer\x18\xf4\x07 \x01(\x0b\x32\x1a.vega.commands.v1.TransferH\x00R\x08transfer\x12L\n\x0f\x63\x61ncel_transfer\x18\xf5\x07 \x01(\x0b\x32 .vega.commands.v1.CancelTransferH\x00R\x0e\x63\x61ncelTransfer\x12\x46\n\rannounce_node\x18\xf6\x07 \x01(\x0b\x32\x1e.vega.commands.v1.AnnounceNodeH\x00R\x0c\x61nnounceNode\x12h\n\x19\x62\x61tch_market_instructions\x18\xf7\x07 \x01(\x0b\x32).vega.commands.v1.BatchMarketInstructionsH\x00R\x17\x62\x61tchMarketInstructions\x12_\n\x16stop_orders_submission\x18\xf8\x07 \x01(\x0b\x32&.vega.commands.v1.StopOrdersSubmissionH\x00R\x14stopOrdersSubmission\x12\x65\n\x18stop_orders_cancellation\x18\xf9\x07 \x01(\x0b\x32(.vega.commands.v1.StopOrdersCancellationH\x00R\x16stopOrdersCancellation\x12:\n\tnode_vote\x18\xd2\x0f \x01(\x0b\x32\x1a.vega.commands.v1.NodeVoteH\x00R\x08nodeVote\x12I\n\x0enode_signature\x18\xd3\x0f \x01(\x0b\x32\x1f.vega.commands.v1.NodeSignatureH\x00R\rnodeSignature\x12@\n\x0b\x63hain_event\x18\xd4\x0f \x01(\x0b\x32\x1c.vega.commands.v1.ChainEventH\x00R\nchainEvent\x12\\\n\x15key_rotate_submission\x18\xd5\x0f \x01(\x0b\x32%.vega.commands.v1.KeyRotateSubmissionH\x00R\x13keyRotateSubmission\x12\x62\n\x17state_variable_proposal\x18\xd6\x0f \x01(\x0b\x32\'.vega.commands.v1.StateVariableProposalH\x00R\x15stateVariableProposal\x12X\n\x13validator_heartbeat\x18\xd7\x0f \x01(\x0b\x32$.vega.commands.v1.ValidatorHeartbeatH\x00R\x12validatorHeartbeat\x12u\n\x1e\x65thereum_key_rotate_submission\x18\xd8\x0f \x01(\x0b\x32-.vega.commands.v1.EthereumKeyRotateSubmissionH\x00R\x1b\x65thereumKeyRotateSubmission\x12h\n\x19protocol_upgrade_proposal\x18\xd9\x0f \x01(\x0b\x32).vega.commands.v1.ProtocolUpgradeProposalH\x00R\x17protocolUpgradeProposal\x12O\n\x10issue_signatures\x18\xda\x0f \x01(\x0b\x32!.vega.commands.v1.IssueSignaturesH\x00R\x0fissueSignatures\x12_\n\x16oracle_data_submission\x18\xb9\x17 \x01(\x0b\x32&.vega.commands.v1.OracleDataSubmissionH\x00R\x14oracleDataSubmissionB\t\n\x07\x63ommandJ\x06\x08\xa1\x1f\x10\xa2\x1f"\x92\x02\n\x0bTransaction\x12\x1d\n\ninput_data\x18\x01 \x01(\x0cR\tinputData\x12\x39\n\tsignature\x18\x02 \x01(\x0b\x32\x1b.vega.commands.v1.SignatureR\tsignature\x12\x1b\n\x07\x61\x64\x64ress\x18\xe9\x07 \x01(\tH\x00R\x07\x61\x64\x64ress\x12\x1a\n\x07pub_key\x18\xea\x07 \x01(\tH\x00R\x06pubKey\x12\x36\n\x07version\x18\xd0\x0f \x01(\x0e\x32\x1b.vega.commands.v1.TxVersionR\x07version\x12\x30\n\x03pow\x18\xb8\x17 \x01(\x0b\x32\x1d.vega.commands.v1.ProofOfWorkR\x03powB\x06\n\x04\x66rom"5\n\x0bProofOfWork\x12\x10\n\x03tid\x18\x01 \x01(\tR\x03tid\x12\x14\n\x05nonce\x18\x02 \x01(\x04R\x05nonce*S\n\tTxVersion\x12\x1a\n\x16TX_VERSION_UNSPECIFIED\x10\x00\x12\x11\n\rTX_VERSION_V2\x10\x02\x12\x11\n\rTX_VERSION_V3\x10\x03"\x04\x08\x01\x10\x01\x42\x33Z1code.vegaprotocol.io/vega/protos/vega/commands/v1b\x06proto3'
 )
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(
-    DESCRIPTOR, "vega.commands.v1.transaction_pb2", globals()
+    DESCRIPTOR, "vega.commands.v1.transaction_pb2", _globals
 )
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = (
         b"Z1code.vegaprotocol.io/vega/protos/vega/commands/v1"
     )
-    _TXVERSION._serialized_start = 2876
-    _TXVERSION._serialized_end = 2959
-    _INPUTDATA._serialized_start = 196
-    _INPUTDATA._serialized_end = 2542
-    _TRANSACTION._serialized_start = 2545
-    _TRANSACTION._serialized_end = 2819
-    _PROOFOFWORK._serialized_start = 2821
-    _PROOFOFWORK._serialized_end = 2874
+    _globals["_TXVERSION"]._serialized_start = 3076
+    _globals["_TXVERSION"]._serialized_end = 3159
+    _globals["_INPUTDATA"]._serialized_start = 196
+    _globals["_INPUTDATA"]._serialized_end = 2742
+    _globals["_TRANSACTION"]._serialized_start = 2745
+    _globals["_TRANSACTION"]._serialized_end = 3019
+    _globals["_PROOFOFWORK"]._serialized_start = 3021
+    _globals["_PROOFOFWORK"]._serialized_end = 3074
 # @@protoc_insertion_point(module_scope)
```

### Comparing `vega_sim-1.1.1/vega_sim/proto/vega/commands/v1/validator_commands_pb2.py` & `vega_sim-1.2.0/vega_sim/proto/vega/commands/v1/validator_commands_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,56 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: vega/commands/v1/validator_commands.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from ... import chain_events_pb2 as vega_dot_chain__events__pb2
 from ...commands.v1 import signature_pb2 as vega_dot_commands_dot_v1_dot_signature__pb2
 from ... import vega_pb2 as vega_dot_vega__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n)vega/commands/v1/validator_commands.proto\x12\x10vega.commands.v1\x1a\x17vega/chain_events.proto\x1a vega/commands/v1/signature.proto\x1a\x0fvega/vega.proto"\xd7\x01\n\x12ValidatorHeartbeat\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12J\n\x12\x65thereum_signature\x18\x02 \x01(\x0b\x32\x1b.vega.commands.v1.SignatureR\x11\x65thereumSignature\x12\x42\n\x0evega_signature\x18\x03 \x01(\x0b\x32\x1b.vega.commands.v1.SignatureR\rvegaSignature\x12\x18\n\x07message\x18\x04 \x01(\tR\x07message"\x80\x04\n\x0c\x41nnounceNode\x12 \n\x0cvega_pub_key\x18\x01 \x01(\tR\nvegaPubKey\x12)\n\x10\x65thereum_address\x18\x02 \x01(\tR\x0f\x65thereumAddress\x12"\n\rchain_pub_key\x18\x03 \x01(\tR\x0b\x63hainPubKey\x12\x19\n\x08info_url\x18\x04 \x01(\tR\x07infoUrl\x12\x18\n\x07\x63ountry\x18\x05 \x01(\tR\x07\x63ountry\x12\x0e\n\x02id\x18\x06 \x01(\tR\x02id\x12\x12\n\x04name\x18\x07 \x01(\tR\x04name\x12\x1d\n\navatar_url\x18\x08 \x01(\tR\tavatarUrl\x12+\n\x12vega_pub_key_index\x18\t \x01(\rR\x0fvegaPubKeyIndex\x12\x1d\n\nfrom_epoch\x18\n \x01(\x04R\tfromEpoch\x12J\n\x12\x65thereum_signature\x18\x0b \x01(\x0b\x32\x1b.vega.commands.v1.SignatureR\x11\x65thereumSignature\x12\x42\n\x0evega_signature\x18\x0c \x01(\x0b\x32\x1b.vega.commands.v1.SignatureR\rvegaSignature\x12+\n\x11submitter_address\x18\r \x01(\tR\x10submitterAddress"\xc0\x03\n\x08NodeVote\x12\x1c\n\treference\x18\x02 \x01(\tR\treference\x12\x33\n\x04type\x18\x03 \x01(\x0e\x32\x1f.vega.commands.v1.NodeVote.TypeR\x04type"\xda\x02\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x18\n\x14TYPE_STAKE_DEPOSITED\x10\x01\x12\x16\n\x12TYPE_STAKE_REMOVED\x10\x02\x12\x18\n\x14TYPE_FUNDS_DEPOSITED\x10\x03\x12\x15\n\x11TYPE_SIGNER_ADDED\x10\x04\x12\x17\n\x13TYPE_SIGNER_REMOVED\x10\x05\x12\x17\n\x13TYPE_BRIDGE_STOPPED\x10\x06\x12\x17\n\x13TYPE_BRIDGE_RESUMED\x10\x07\x12\x15\n\x11TYPE_ASSET_LISTED\x10\x08\x12\x17\n\x13TYPE_LIMITS_UPDATED\x10\t\x12\x1b\n\x17TYPE_STAKE_TOTAL_SUPPLY\x10\n\x12\x1d\n\x19TYPE_SIGNER_THRESHOLD_SET\x10\x0b\x12"\n\x1eTYPE_GOVERNANCE_VALIDATE_ASSET\x10\x0cJ\x04\x08\x01\x10\x02"j\n\rNodeSignature\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x10\n\x03sig\x18\x02 \x01(\x0cR\x03sig\x12\x37\n\x04kind\x18\x03 \x01(\x0e\x32#.vega.commands.v1.NodeSignatureKindR\x04kind"\xb1\x02\n\nChainEvent\x12\x13\n\x05tx_id\x18\x01 \x01(\tR\x04txId\x12\x14\n\x05nonce\x18\x02 \x01(\x04R\x05nonce\x12\x34\n\x07\x62uiltin\x18\xe9\x07 \x01(\x0b\x32\x17.vega.BuiltinAssetEventH\x00R\x07\x62uiltin\x12)\n\x05\x65rc20\x18\xea\x07 \x01(\x0b\x32\x10.vega.ERC20EventH\x00R\x05\x65rc20\x12:\n\rstaking_event\x18\xed\x07 \x01(\x0b\x32\x12.vega.StakingEventH\x00R\x0cstakingEvent\x12\x42\n\x0e\x65rc20_multisig\x18\xee\x07 \x01(\x0b\x32\x18.vega.ERC20MultiSigEventH\x00R\rerc20MultisigB\x07\n\x05\x65ventJ\x06\x08\xeb\x07\x10\xec\x07J\x06\x08\xec\x07\x10\xed\x07"\xb4\x01\n\x13KeyRotateSubmission\x12)\n\x11new_pub_key_index\x18\x01 \x01(\rR\x0enewPubKeyIndex\x12!\n\x0ctarget_block\x18\x02 \x01(\x04R\x0btargetBlock\x12\x1e\n\x0bnew_pub_key\x18\x03 \x01(\tR\tnewPubKey\x12/\n\x14\x63urrent_pub_key_hash\x18\x04 \x01(\tR\x11\x63urrentPubKeyHash"\x83\x02\n\x1b\x45thereumKeyRotateSubmission\x12!\n\x0ctarget_block\x18\x01 \x01(\x04R\x0btargetBlock\x12\x1f\n\x0bnew_address\x18\x02 \x01(\tR\nnewAddress\x12\'\n\x0f\x63urrent_address\x18\x03 \x01(\tR\x0e\x63urrentAddress\x12+\n\x11submitter_address\x18\x04 \x01(\tR\x10submitterAddress\x12J\n\x12\x65thereum_signature\x18\x05 \x01(\x0b\x32\x1b.vega.commands.v1.SignatureR\x11\x65thereumSignature"M\n\x15StateVariableProposal\x12\x34\n\x08proposal\x18\x01 \x01(\x0b\x32\x18.vega.StateValueProposalR\x08proposal"u\n\x17ProtocolUpgradeProposal\x12\x30\n\x14upgrade_block_height\x18\x01 \x01(\x04R\x12upgradeBlockHeight\x12(\n\x10vega_release_tag\x18\x02 \x01(\tR\x0evegaReleaseTag*\x97\x02\n\x11NodeSignatureKind\x12#\n\x1fNODE_SIGNATURE_KIND_UNSPECIFIED\x10\x00\x12!\n\x1dNODE_SIGNATURE_KIND_ASSET_NEW\x10\x01\x12(\n$NODE_SIGNATURE_KIND_ASSET_WITHDRAWAL\x10\x02\x12\x33\n/NODE_SIGNATURE_KIND_ERC20_MULTISIG_SIGNER_ADDED\x10\x03\x12\x35\n1NODE_SIGNATURE_KIND_ERC20_MULTISIG_SIGNER_REMOVED\x10\x04\x12$\n NODE_SIGNATURE_KIND_ASSET_UPDATE\x10\x05\x42\x33Z1code.vegaprotocol.io/vega/protos/vega/commands/v1b\x06proto3'
+    b'\n)vega/commands/v1/validator_commands.proto\x12\x10vega.commands.v1\x1a\x17vega/chain_events.proto\x1a vega/commands/v1/signature.proto\x1a\x0fvega/vega.proto"\xd7\x01\n\x12ValidatorHeartbeat\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12J\n\x12\x65thereum_signature\x18\x02 \x01(\x0b\x32\x1b.vega.commands.v1.SignatureR\x11\x65thereumSignature\x12\x42\n\x0evega_signature\x18\x03 \x01(\x0b\x32\x1b.vega.commands.v1.SignatureR\rvegaSignature\x12\x18\n\x07message\x18\x04 \x01(\tR\x07message"\x80\x04\n\x0c\x41nnounceNode\x12 \n\x0cvega_pub_key\x18\x01 \x01(\tR\nvegaPubKey\x12)\n\x10\x65thereum_address\x18\x02 \x01(\tR\x0f\x65thereumAddress\x12"\n\rchain_pub_key\x18\x03 \x01(\tR\x0b\x63hainPubKey\x12\x19\n\x08info_url\x18\x04 \x01(\tR\x07infoUrl\x12\x18\n\x07\x63ountry\x18\x05 \x01(\tR\x07\x63ountry\x12\x0e\n\x02id\x18\x06 \x01(\tR\x02id\x12\x12\n\x04name\x18\x07 \x01(\tR\x04name\x12\x1d\n\navatar_url\x18\x08 \x01(\tR\tavatarUrl\x12+\n\x12vega_pub_key_index\x18\t \x01(\rR\x0fvegaPubKeyIndex\x12\x1d\n\nfrom_epoch\x18\n \x01(\x04R\tfromEpoch\x12J\n\x12\x65thereum_signature\x18\x0b \x01(\x0b\x32\x1b.vega.commands.v1.SignatureR\x11\x65thereumSignature\x12\x42\n\x0evega_signature\x18\x0c \x01(\x0b\x32\x1b.vega.commands.v1.SignatureR\rvegaSignature\x12+\n\x11submitter_address\x18\r \x01(\tR\x10submitterAddress"\xc0\x03\n\x08NodeVote\x12\x1c\n\treference\x18\x02 \x01(\tR\treference\x12\x33\n\x04type\x18\x03 \x01(\x0e\x32\x1f.vega.commands.v1.NodeVote.TypeR\x04type"\xda\x02\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x18\n\x14TYPE_STAKE_DEPOSITED\x10\x01\x12\x16\n\x12TYPE_STAKE_REMOVED\x10\x02\x12\x18\n\x14TYPE_FUNDS_DEPOSITED\x10\x03\x12\x15\n\x11TYPE_SIGNER_ADDED\x10\x04\x12\x17\n\x13TYPE_SIGNER_REMOVED\x10\x05\x12\x17\n\x13TYPE_BRIDGE_STOPPED\x10\x06\x12\x17\n\x13TYPE_BRIDGE_RESUMED\x10\x07\x12\x15\n\x11TYPE_ASSET_LISTED\x10\x08\x12\x17\n\x13TYPE_LIMITS_UPDATED\x10\t\x12\x1b\n\x17TYPE_STAKE_TOTAL_SUPPLY\x10\n\x12\x1d\n\x19TYPE_SIGNER_THRESHOLD_SET\x10\x0b\x12"\n\x1eTYPE_GOVERNANCE_VALIDATE_ASSET\x10\x0cJ\x04\x08\x01\x10\x02"j\n\rNodeSignature\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x10\n\x03sig\x18\x02 \x01(\x0cR\x03sig\x12\x37\n\x04kind\x18\x03 \x01(\x0e\x32#.vega.commands.v1.NodeSignatureKindR\x04kind"\xf5\x02\n\nChainEvent\x12\x13\n\x05tx_id\x18\x01 \x01(\tR\x04txId\x12\x14\n\x05nonce\x18\x02 \x01(\x04R\x05nonce\x12\x34\n\x07\x62uiltin\x18\xe9\x07 \x01(\x0b\x32\x17.vega.BuiltinAssetEventH\x00R\x07\x62uiltin\x12)\n\x05\x65rc20\x18\xea\x07 \x01(\x0b\x32\x10.vega.ERC20EventH\x00R\x05\x65rc20\x12:\n\rstaking_event\x18\xed\x07 \x01(\x0b\x32\x12.vega.StakingEventH\x00R\x0cstakingEvent\x12\x42\n\x0e\x65rc20_multisig\x18\xee\x07 \x01(\x0b\x32\x18.vega.ERC20MultiSigEventH\x00R\rerc20Multisig\x12\x42\n\rcontract_call\x18\xef\x07 \x01(\x0b\x32\x1a.vega.EthContractCallEventH\x00R\x0c\x63ontractCallB\x07\n\x05\x65ventJ\x06\x08\xeb\x07\x10\xec\x07J\x06\x08\xec\x07\x10\xed\x07"\xb4\x01\n\x13KeyRotateSubmission\x12)\n\x11new_pub_key_index\x18\x01 \x01(\rR\x0enewPubKeyIndex\x12!\n\x0ctarget_block\x18\x02 \x01(\x04R\x0btargetBlock\x12\x1e\n\x0bnew_pub_key\x18\x03 \x01(\tR\tnewPubKey\x12/\n\x14\x63urrent_pub_key_hash\x18\x04 \x01(\tR\x11\x63urrentPubKeyHash"\x83\x02\n\x1b\x45thereumKeyRotateSubmission\x12!\n\x0ctarget_block\x18\x01 \x01(\x04R\x0btargetBlock\x12\x1f\n\x0bnew_address\x18\x02 \x01(\tR\nnewAddress\x12\'\n\x0f\x63urrent_address\x18\x03 \x01(\tR\x0e\x63urrentAddress\x12+\n\x11submitter_address\x18\x04 \x01(\tR\x10submitterAddress\x12J\n\x12\x65thereum_signature\x18\x05 \x01(\x0b\x32\x1b.vega.commands.v1.SignatureR\x11\x65thereumSignature"M\n\x15StateVariableProposal\x12\x34\n\x08proposal\x18\x01 \x01(\x0b\x32\x18.vega.StateValueProposalR\x08proposal"u\n\x17ProtocolUpgradeProposal\x12\x30\n\x14upgrade_block_height\x18\x01 \x01(\x04R\x12upgradeBlockHeight\x12(\n\x10vega_release_tag\x18\x02 \x01(\tR\x0evegaReleaseTag*\x97\x02\n\x11NodeSignatureKind\x12#\n\x1fNODE_SIGNATURE_KIND_UNSPECIFIED\x10\x00\x12!\n\x1dNODE_SIGNATURE_KIND_ASSET_NEW\x10\x01\x12(\n$NODE_SIGNATURE_KIND_ASSET_WITHDRAWAL\x10\x02\x12\x33\n/NODE_SIGNATURE_KIND_ERC20_MULTISIG_SIGNER_ADDED\x10\x03\x12\x35\n1NODE_SIGNATURE_KIND_ERC20_MULTISIG_SIGNER_REMOVED\x10\x04\x12$\n NODE_SIGNATURE_KIND_ASSET_UPDATE\x10\x05\x42\x33Z1code.vegaprotocol.io/vega/protos/vega/commands/v1b\x06proto3'
 )
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(
-    DESCRIPTOR, "vega.commands.v1.validator_commands_pb2", globals()
+    DESCRIPTOR, "vega.commands.v1.validator_commands_pb2", _globals
 )
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = (
         b"Z1code.vegaprotocol.io/vega/protos/vega/commands/v1"
     )
-    _NODESIGNATUREKIND._serialized_start = 2383
-    _NODESIGNATUREKIND._serialized_end = 2662
-    _VALIDATORHEARTBEAT._serialized_start = 140
-    _VALIDATORHEARTBEAT._serialized_end = 355
-    _ANNOUNCENODE._serialized_start = 358
-    _ANNOUNCENODE._serialized_end = 870
-    _NODEVOTE._serialized_start = 873
-    _NODEVOTE._serialized_end = 1321
-    _NODEVOTE_TYPE._serialized_start = 969
-    _NODEVOTE_TYPE._serialized_end = 1315
-    _NODESIGNATURE._serialized_start = 1323
-    _NODESIGNATURE._serialized_end = 1429
-    _CHAINEVENT._serialized_start = 1432
-    _CHAINEVENT._serialized_end = 1737
-    _KEYROTATESUBMISSION._serialized_start = 1740
-    _KEYROTATESUBMISSION._serialized_end = 1920
-    _ETHEREUMKEYROTATESUBMISSION._serialized_start = 1923
-    _ETHEREUMKEYROTATESUBMISSION._serialized_end = 2182
-    _STATEVARIABLEPROPOSAL._serialized_start = 2184
-    _STATEVARIABLEPROPOSAL._serialized_end = 2261
-    _PROTOCOLUPGRADEPROPOSAL._serialized_start = 2263
-    _PROTOCOLUPGRADEPROPOSAL._serialized_end = 2380
+    _globals["_NODESIGNATUREKIND"]._serialized_start = 2451
+    _globals["_NODESIGNATUREKIND"]._serialized_end = 2730
+    _globals["_VALIDATORHEARTBEAT"]._serialized_start = 140
+    _globals["_VALIDATORHEARTBEAT"]._serialized_end = 355
+    _globals["_ANNOUNCENODE"]._serialized_start = 358
+    _globals["_ANNOUNCENODE"]._serialized_end = 870
+    _globals["_NODEVOTE"]._serialized_start = 873
+    _globals["_NODEVOTE"]._serialized_end = 1321
+    _globals["_NODEVOTE_TYPE"]._serialized_start = 969
+    _globals["_NODEVOTE_TYPE"]._serialized_end = 1315
+    _globals["_NODESIGNATURE"]._serialized_start = 1323
+    _globals["_NODESIGNATURE"]._serialized_end = 1429
+    _globals["_CHAINEVENT"]._serialized_start = 1432
+    _globals["_CHAINEVENT"]._serialized_end = 1805
+    _globals["_KEYROTATESUBMISSION"]._serialized_start = 1808
+    _globals["_KEYROTATESUBMISSION"]._serialized_end = 1988
+    _globals["_ETHEREUMKEYROTATESUBMISSION"]._serialized_start = 1991
+    _globals["_ETHEREUMKEYROTATESUBMISSION"]._serialized_end = 2250
+    _globals["_STATEVARIABLEPROPOSAL"]._serialized_start = 2252
+    _globals["_STATEVARIABLEPROPOSAL"]._serialized_end = 2329
+    _globals["_PROTOCOLUPGRADEPROPOSAL"]._serialized_start = 2331
+    _globals["_PROTOCOLUPGRADEPROPOSAL"]._serialized_end = 2448
 # @@protoc_insertion_point(module_scope)
```

### Comparing `vega_sim-1.1.1/vega_sim/proto/vega/data/v1/spec_pb2.py` & `vega_sim-1.2.0/vega_sim/proto/vega/data/v1/spec_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: vega/data/v1/spec.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
     b'\n\x17vega/data/v1/spec.proto\x12\x0cvega.data.v1"n\n\x06\x46ilter\x12+\n\x03key\x18\x01 \x01(\x0b\x32\x19.vega.data.v1.PropertyKeyR\x03key\x12\x37\n\nconditions\x18\x02 \x03(\x0b\x32\x17.vega.data.v1.ConditionR\nconditions"\xb2\x02\n\x0bPropertyKey\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x32\n\x04type\x18\x02 \x01(\x0e\x32\x1e.vega.data.v1.PropertyKey.TypeR\x04type\x12\x37\n\x15number_decimal_places\x18\x03 \x01(\x04H\x00R\x13numberDecimalPlaces\x88\x01\x01"\x87\x01\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x0e\n\nTYPE_EMPTY\x10\x01\x12\x10\n\x0cTYPE_INTEGER\x10\x02\x12\x0f\n\x0bTYPE_STRING\x10\x03\x12\x10\n\x0cTYPE_BOOLEAN\x10\x04\x12\x10\n\x0cTYPE_DECIMAL\x10\x05\x12\x12\n\x0eTYPE_TIMESTAMP\x10\x06\x42\x18\n\x16_number_decimal_places"\x93\x02\n\tCondition\x12<\n\x08operator\x18\x01 \x01(\x0e\x32 .vega.data.v1.Condition.OperatorR\x08operator\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value"\xb1\x01\n\x08Operator\x12\x18\n\x14OPERATOR_UNSPECIFIED\x10\x00\x12\x13\n\x0fOPERATOR_EQUALS\x10\x01\x12\x19\n\x15OPERATOR_GREATER_THAN\x10\x02\x12"\n\x1eOPERATOR_GREATER_THAN_OR_EQUAL\x10\x03\x12\x16\n\x12OPERATOR_LESS_THAN\x10\x04\x12\x1f\n\x1bOPERATOR_LESS_THAN_OR_EQUAL\x10\x05\x42/Z-code.vegaprotocol.io/vega/protos/vega/data/v1b\x06proto3'
 )
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "vega.data.v1.spec_pb2", globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "vega.data.v1.spec_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b"Z-code.vegaprotocol.io/vega/protos/vega/data/v1"
-    _FILTER._serialized_start = 41
-    _FILTER._serialized_end = 151
-    _PROPERTYKEY._serialized_start = 154
-    _PROPERTYKEY._serialized_end = 460
-    _PROPERTYKEY_TYPE._serialized_start = 299
-    _PROPERTYKEY_TYPE._serialized_end = 434
-    _CONDITION._serialized_start = 463
-    _CONDITION._serialized_end = 738
-    _CONDITION_OPERATOR._serialized_start = 561
-    _CONDITION_OPERATOR._serialized_end = 738
+    _globals["_FILTER"]._serialized_start = 41
+    _globals["_FILTER"]._serialized_end = 151
+    _globals["_PROPERTYKEY"]._serialized_start = 154
+    _globals["_PROPERTYKEY"]._serialized_end = 460
+    _globals["_PROPERTYKEY_TYPE"]._serialized_start = 299
+    _globals["_PROPERTYKEY_TYPE"]._serialized_end = 434
+    _globals["_CONDITION"]._serialized_start = 463
+    _globals["_CONDITION"]._serialized_end = 738
+    _globals["_CONDITION_OPERATOR"]._serialized_start = 561
+    _globals["_CONDITION_OPERATOR"]._serialized_end = 738
 # @@protoc_insertion_point(module_scope)
```

### Comparing `vega_sim-1.1.1/vega_sim/proto/vega/events/v1/events_pb2.py` & `vega_sim-1.2.0/vega_sim/proto/vega/events/v1/events_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: vega/events/v1/events.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from ... import assets_pb2 as vega_dot_assets__pb2
@@ -21,124 +21,131 @@
 from ... import governance_pb2 as vega_dot_governance__pb2
 from ... import markets_pb2 as vega_dot_markets__pb2
 from ... import oracle_pb2 as vega_dot_oracle__pb2
 from ... import vega_pb2 as vega_dot_vega__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x1bvega/events/v1/events.proto\x12\x0evega.events.v1\x1a\x11vega/assets.proto\x1a\x1fvega/commands/v1/commands.proto\x1a\x1bvega/commands/v1/data.proto\x1a)vega/commands/v1/validator_commands.proto\x1a\x15vega/governance.proto\x1a\x12vega/markets.proto\x1a\x11vega/oracle.proto\x1a\x0fvega/vega.proto"\xee\x01\n\x18\x45RC20MultiSigSignerAdded\x12!\n\x0csignature_id\x18\x01 \x01(\tR\x0bsignatureId\x12!\n\x0cvalidator_id\x18\x02 \x01(\tR\x0bvalidatorId\x12\x1c\n\ttimestamp\x18\x03 \x01(\x03R\ttimestamp\x12\x1d\n\nnew_signer\x18\x04 \x01(\tR\tnewSigner\x12\x1c\n\tsubmitter\x18\x05 \x01(\tR\tsubmitter\x12\x14\n\x05nonce\x18\x06 \x01(\tR\x05nonce\x12\x1b\n\tepoch_seq\x18\x07 \x01(\tR\x08\x65pochSeq"f\n#ERC20MultiSigSignerRemovedSubmitter\x12!\n\x0csignature_id\x18\x01 \x01(\tR\x0bsignatureId\x12\x1c\n\tsubmitter\x18\x02 \x01(\tR\tsubmitter"\x97\x02\n\x1a\x45RC20MultiSigSignerRemoved\x12\x66\n\x14signature_submitters\x18\x01 \x03(\x0b\x32\x33.vega.events.v1.ERC20MultiSigSignerRemovedSubmitterR\x13signatureSubmitters\x12!\n\x0cvalidator_id\x18\x02 \x01(\tR\x0bvalidatorId\x12\x1c\n\ttimestamp\x18\x03 \x01(\x03R\ttimestamp\x12\x1d\n\nold_signer\x18\x04 \x01(\tR\toldSigner\x12\x14\n\x05nonce\x18\x05 \x01(\tR\x05nonce\x12\x1b\n\tepoch_seq\x18\x06 \x01(\tR\x08\x65pochSeq"\x90\x05\n\x08Transfer\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04\x66rom\x18\x02 \x01(\tR\x04\x66rom\x12=\n\x11\x66rom_account_type\x18\x03 \x01(\x0e\x32\x11.vega.AccountTypeR\x0f\x66romAccountType\x12\x0e\n\x02to\x18\x04 \x01(\tR\x02to\x12\x39\n\x0fto_account_type\x18\x05 \x01(\x0e\x32\x11.vega.AccountTypeR\rtoAccountType\x12\x14\n\x05\x61sset\x18\x06 \x01(\tR\x05\x61sset\x12\x16\n\x06\x61mount\x18\x07 \x01(\tR\x06\x61mount\x12\x1c\n\treference\x18\x08 \x01(\tR\treference\x12\x37\n\x06status\x18\t \x01(\x0e\x32\x1f.vega.events.v1.Transfer.StatusR\x06status\x12\x1c\n\ttimestamp\x18\n \x01(\x03R\ttimestamp\x12\x1b\n\x06reason\x18\x0b \x01(\tH\x01R\x06reason\x88\x01\x01\x12\x39\n\x07one_off\x18\x65 \x01(\x0b\x32\x1e.vega.events.v1.OneOffTransferH\x00R\x06oneOff\x12\x41\n\trecurring\x18\x66 \x01(\x0b\x32!.vega.events.v1.RecurringTransferH\x00R\trecurring"\x84\x01\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x12\n\x0eSTATUS_PENDING\x10\x01\x12\x0f\n\x0bSTATUS_DONE\x10\x02\x12\x13\n\x0fSTATUS_REJECTED\x10\x03\x12\x12\n\x0eSTATUS_STOPPED\x10\x04\x12\x14\n\x10STATUS_CANCELLED\x10\x05\x42\x06\n\x04kindB\t\n\x07_reason"/\n\x0eOneOffTransfer\x12\x1d\n\ndeliver_on\x18\x01 \x01(\x03R\tdeliverOn"\xc1\x01\n\x11RecurringTransfer\x12\x1f\n\x0bstart_epoch\x18\x01 \x01(\x04R\nstartEpoch\x12 \n\tend_epoch\x18\x02 \x01(\x04H\x00R\x08\x65ndEpoch\x88\x01\x01\x12\x16\n\x06\x66\x61\x63tor\x18\x03 \x01(\tR\x06\x66\x61\x63tor\x12\x43\n\x11\x64ispatch_strategy\x18\x04 \x01(\x0b\x32\x16.vega.DispatchStrategyR\x10\x64ispatchStrategyB\x0c\n\n_end_epoch"\xb4\x04\n\x0cStakeLinking\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x35\n\x04type\x18\x02 \x01(\x0e\x32!.vega.events.v1.StakeLinking.TypeR\x04type\x12\x0e\n\x02ts\x18\x03 \x01(\x03R\x02ts\x12\x14\n\x05party\x18\x04 \x01(\tR\x05party\x12\x16\n\x06\x61mount\x18\x05 \x01(\tR\x06\x61mount\x12;\n\x06status\x18\x06 \x01(\x0e\x32#.vega.events.v1.StakeLinking.StatusR\x06status\x12!\n\x0c\x66inalized_at\x18\x07 \x01(\x03R\x0b\x66inalizedAt\x12\x17\n\x07tx_hash\x18\x08 \x01(\tR\x06txHash\x12!\n\x0c\x62lock_height\x18\t \x01(\x04R\x0b\x62lockHeight\x12\x1d\n\nblock_time\x18\n \x01(\x03R\tblockTime\x12\x1b\n\tlog_index\x18\x0b \x01(\x04R\x08logIndex\x12)\n\x10\x65thereum_address\x18\x0c \x01(\tR\x0f\x65thereumAddress"<\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\r\n\tTYPE_LINK\x10\x01\x12\x0f\n\x0bTYPE_UNLINK\x10\x02"^\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x12\n\x0eSTATUS_PENDING\x10\x01\x12\x13\n\x0fSTATUS_ACCEPTED\x10\x02\x12\x13\n\x0fSTATUS_REJECTED\x10\x03"\xd3\x02\n\x18\x45RC20MultiSigSignerEvent\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x41\n\x04type\x18\x02 \x01(\x0e\x32-.vega.events.v1.ERC20MultiSigSignerEvent.TypeR\x04type\x12\x16\n\x06signer\x18\x03 \x01(\tR\x06signer\x12\x14\n\x05nonce\x18\x04 \x01(\tR\x05nonce\x12\x1d\n\nblock_time\x18\x05 \x01(\x03R\tblockTime\x12\x17\n\x07tx_hash\x18\x06 \x01(\tR\x06txHash\x12\x1b\n\tlog_index\x18\x07 \x01(\x04R\x08logIndex\x12!\n\x0c\x62lock_number\x18\x08 \x01(\x04R\x0b\x62lockNumber">\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x0e\n\nTYPE_ADDED\x10\x01\x12\x10\n\x0cTYPE_REMOVED\x10\x02"\xe3\x01\n\x1e\x45RC20MultiSigThresholdSetEvent\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12#\n\rnew_threshold\x18\x02 \x01(\rR\x0cnewThreshold\x12\x14\n\x05nonce\x18\x03 \x01(\tR\x05nonce\x12\x1d\n\nblock_time\x18\x04 \x01(\x03R\tblockTime\x12\x17\n\x07tx_hash\x18\x05 \x01(\tR\x06txHash\x12\x1b\n\tlog_index\x18\x06 \x01(\x04R\x08logIndex\x12!\n\x0c\x62lock_number\x18\x07 \x01(\x04R\x0b\x62lockNumber"g\n\x0f\x43heckpointEvent\x12\x12\n\x04hash\x18\x01 \x01(\tR\x04hash\x12\x1d\n\nblock_hash\x18\x02 \x01(\tR\tblockHash\x12!\n\x0c\x62lock_height\x18\x03 \x01(\x04R\x0b\x62lockHeight"-\n\x10StreamStartEvent\x12\x19\n\x08\x63hain_id\x18\x01 \x01(\tR\x07\x63hainId"\x82\x02\n\x11RewardPayoutEvent\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x1b\n\tepoch_seq\x18\x02 \x01(\tR\x08\x65pochSeq\x12\x14\n\x05\x61sset\x18\x03 \x01(\tR\x05\x61sset\x12\x16\n\x06\x61mount\x18\x04 \x01(\tR\x06\x61mount\x12\x35\n\x17percent_of_total_reward\x18\x05 \x01(\tR\x14percentOfTotalReward\x12\x1c\n\ttimestamp\x18\x06 \x01(\x03R\ttimestamp\x12\x1f\n\x0breward_type\x18\x07 \x01(\tR\nrewardType\x12\x16\n\x06market\x18\x08 \x01(\tR\x06market"\xd6\x02\n\x13ValidatorScoreEvent\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x1b\n\tepoch_seq\x18\x02 \x01(\tR\x08\x65pochSeq\x12\'\n\x0fvalidator_score\x18\x03 \x01(\tR\x0evalidatorScore\x12)\n\x10normalised_score\x18\x04 \x01(\tR\x0fnormalisedScore\x12\x33\n\x15validator_performance\x18\x05 \x01(\tR\x14validatorPerformance\x12.\n\x13raw_validator_score\x18\x06 \x01(\tR\x11rawValidatorScore\x12)\n\x10validator_status\x18\x07 \x01(\tR\x0fvalidatorStatus\x12%\n\x0emultisig_score\x18\x08 \x01(\tR\rmultisigScore"|\n\x16\x44\x65legationBalanceEvent\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x17\n\x07node_id\x18\x02 \x01(\tR\x06nodeId\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount\x12\x1b\n\tepoch_seq\x18\x04 \x01(\tR\x08\x65pochSeq"D\n\x0bMarketEvent\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x18\n\x07payload\x18\x02 \x01(\tR\x07payload"\xed\x10\n\x11TransactionResult\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12\x16\n\x06status\x18\x02 \x01(\x08R\x06status\x12\x12\n\x04hash\x18\x03 \x01(\tR\x04hash\x12N\n\x10order_submission\x18\x65 \x01(\x0b\x32!.vega.commands.v1.OrderSubmissionH\x00R\x0forderSubmission\x12K\n\x0forder_amendment\x18\x66 \x01(\x0b\x32 .vega.commands.v1.OrderAmendmentH\x00R\x0eorderAmendment\x12T\n\x12order_cancellation\x18g \x01(\x0b\x32#.vega.commands.v1.OrderCancellationH\x00R\x11orderCancellation\x12\x42\n\x08proposal\x18h \x01(\x0b\x32$.vega.commands.v1.ProposalSubmissionH\x00R\x08proposal\x12K\n\x0fvote_submission\x18i \x01(\x0b\x32 .vega.commands.v1.VoteSubmissionH\x00R\x0evoteSubmission\x12v\n\x1eliquidity_provision_submission\x18j \x01(\x0b\x32..vega.commands.v1.LiquidityProvisionSubmissionH\x00R\x1cliquidityProvisionSubmission\x12W\n\x13withdraw_submission\x18k \x01(\x0b\x32$.vega.commands.v1.WithdrawSubmissionH\x00R\x12withdrawSubmission\x12W\n\x13\x64\x65legate_submission\x18l \x01(\x0b\x32$.vega.commands.v1.DelegateSubmissionH\x00R\x12\x64\x65legateSubmission\x12]\n\x15undelegate_submission\x18m \x01(\x0b\x32&.vega.commands.v1.UndelegateSubmissionH\x00R\x14undelegateSubmission\x12|\n liquidity_provision_cancellation\x18o \x01(\x0b\x32\x30.vega.commands.v1.LiquidityProvisionCancellationH\x00R\x1eliquidityProvisionCancellation\x12s\n\x1dliquidity_provision_amendment\x18p \x01(\x0b\x32-.vega.commands.v1.LiquidityProvisionAmendmentH\x00R\x1bliquidityProvisionAmendment\x12\x38\n\x08transfer\x18q \x01(\x0b\x32\x1a.vega.commands.v1.TransferH\x00R\x08transfer\x12K\n\x0f\x63\x61ncel_transfer\x18r \x01(\x0b\x32 .vega.commands.v1.CancelTransferH\x00R\x0e\x63\x61ncelTransfer\x12\x45\n\rannounce_node\x18s \x01(\x0b\x32\x1e.vega.commands.v1.AnnounceNodeH\x00R\x0c\x61nnounceNode\x12^\n\x16oracle_data_submission\x18t \x01(\x0b\x32&.vega.commands.v1.OracleDataSubmissionH\x00R\x14oracleDataSubmission\x12g\n\x19protocol_upgrade_proposal\x18u \x01(\x0b\x32).vega.commands.v1.ProtocolUpgradeProposalH\x00R\x17protocolUpgradeProposal\x12N\n\x10issue_signatures\x18v \x01(\x0b\x32!.vega.commands.v1.IssueSignaturesH\x00R\x0fissueSignatures\x12g\n\x19\x62\x61tch_market_instructions\x18w \x01(\x0b\x32).vega.commands.v1.BatchMarketInstructionsH\x00R\x17\x62\x61tchMarketInstructions\x12[\n\x15key_rotate_submission\x18x \x01(\x0b\x32%.vega.commands.v1.KeyRotateSubmissionH\x00R\x13keyRotateSubmission\x12t\n\x1e\x65thereum_key_rotate_submission\x18y \x01(\x0b\x32-.vega.commands.v1.EthereumKeyRotateSubmissionH\x00R\x1b\x65thereumKeyRotateSubmission\x12M\n\x07success\x18\xe9\x07 \x01(\x0b\x32\x30.vega.events.v1.TransactionResult.SuccessDetailsH\x01R\x07success\x12M\n\x07\x66\x61ilure\x18\xea\x07 \x01(\x0b\x32\x30.vega.events.v1.TransactionResult.FailureDetailsH\x01R\x07\x66\x61ilure\x1a\x10\n\x0eSuccessDetails\x1a&\n\x0e\x46\x61ilureDetails\x12\x14\n\x05\x65rror\x18\x01 \x01(\tR\x05\x65rrorB\r\n\x0btransactionB\x07\n\x05\x65xtra"\xa7\r\n\x0cTxErrorEvent\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12\x17\n\x07\x65rr_msg\x18\x02 \x01(\tR\x06\x65rrMsg\x12N\n\x10order_submission\x18\x65 \x01(\x0b\x32!.vega.commands.v1.OrderSubmissionH\x00R\x0forderSubmission\x12K\n\x0forder_amendment\x18\x66 \x01(\x0b\x32 .vega.commands.v1.OrderAmendmentH\x00R\x0eorderAmendment\x12T\n\x12order_cancellation\x18g \x01(\x0b\x32#.vega.commands.v1.OrderCancellationH\x00R\x11orderCancellation\x12\x42\n\x08proposal\x18h \x01(\x0b\x32$.vega.commands.v1.ProposalSubmissionH\x00R\x08proposal\x12K\n\x0fvote_submission\x18i \x01(\x0b\x32 .vega.commands.v1.VoteSubmissionH\x00R\x0evoteSubmission\x12v\n\x1eliquidity_provision_submission\x18j \x01(\x0b\x32..vega.commands.v1.LiquidityProvisionSubmissionH\x00R\x1cliquidityProvisionSubmission\x12W\n\x13withdraw_submission\x18k \x01(\x0b\x32$.vega.commands.v1.WithdrawSubmissionH\x00R\x12withdrawSubmission\x12W\n\x13\x64\x65legate_submission\x18l \x01(\x0b\x32$.vega.commands.v1.DelegateSubmissionH\x00R\x12\x64\x65legateSubmission\x12]\n\x15undelegate_submission\x18m \x01(\x0b\x32&.vega.commands.v1.UndelegateSubmissionH\x00R\x14undelegateSubmission\x12|\n liquidity_provision_cancellation\x18o \x01(\x0b\x32\x30.vega.commands.v1.LiquidityProvisionCancellationH\x00R\x1eliquidityProvisionCancellation\x12s\n\x1dliquidity_provision_amendment\x18p \x01(\x0b\x32-.vega.commands.v1.LiquidityProvisionAmendmentH\x00R\x1bliquidityProvisionAmendment\x12\x38\n\x08transfer\x18q \x01(\x0b\x32\x1a.vega.commands.v1.TransferH\x00R\x08transfer\x12K\n\x0f\x63\x61ncel_transfer\x18r \x01(\x0b\x32 .vega.commands.v1.CancelTransferH\x00R\x0e\x63\x61ncelTransfer\x12\x45\n\rannounce_node\x18s \x01(\x0b\x32\x1e.vega.commands.v1.AnnounceNodeH\x00R\x0c\x61nnounceNode\x12^\n\x16oracle_data_submission\x18t \x01(\x0b\x32&.vega.commands.v1.OracleDataSubmissionH\x00R\x14oracleDataSubmission\x12g\n\x19protocol_upgrade_proposal\x18u \x01(\x0b\x32).vega.commands.v1.ProtocolUpgradeProposalH\x00R\x17protocolUpgradeProposal\x12N\n\x10issue_signatures\x18v \x01(\x0b\x32!.vega.commands.v1.IssueSignaturesH\x00R\x0fissueSignatures\x12g\n\x19\x62\x61tch_market_instructions\x18w \x01(\x0b\x32).vega.commands.v1.BatchMarketInstructionsH\x00R\x17\x62\x61tchMarketInstructionsB\r\n\x0btransactionJ\x04\x08n\x10o"*\n\nTimeUpdate\x12\x1c\n\ttimestamp\x18\x01 \x01(\x03R\ttimestamp"\xa4\x01\n\nEpochEvent\x12\x10\n\x03seq\x18\x01 \x01(\x04R\x03seq\x12)\n\x06\x61\x63tion\x18\x02 \x01(\x0e\x32\x11.vega.EpochActionR\x06\x61\x63tion\x12\x1d\n\nstart_time\x18\x03 \x01(\x03R\tstartTime\x12\x1f\n\x0b\x65xpire_time\x18\x04 \x01(\x03R\nexpireTime\x12\x19\n\x08\x65nd_time\x18\x05 \x01(\x03R\x07\x65ndTime"R\n\x0fLedgerMovements\x12?\n\x10ledger_movements\x18\x01 \x03(\x0b\x32\x14.vega.LedgerMovementR\x0fledgerMovements"\x88\x01\n\x12PositionResolution\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x1e\n\ndistressed\x18\x02 \x01(\x03R\ndistressed\x12\x16\n\x06\x63losed\x18\x03 \x01(\x03R\x06\x63losed\x12\x1d\n\nmark_price\x18\x04 \x01(\tR\tmarkPrice"c\n\x11LossSocialization\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount"^\n\x0fTradeSettlement\x12\x12\n\x04size\x18\x01 \x01(\x03R\x04size\x12\x14\n\x05price\x18\x02 \x01(\tR\x05price\x12!\n\x0cmarket_price\x18\x03 \x01(\tR\x0bmarketPrice"\xd5\x01\n\x0eSettlePosition\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x14\n\x05price\x18\x03 \x01(\tR\x05price\x12L\n\x11trade_settlements\x18\x04 \x03(\x0b\x32\x1f.vega.events.v1.TradeSettlementR\x10tradeSettlements\x12\'\n\x0fposition_factor\x18\x05 \x01(\tR\x0epositionFactor"j\n\x0cSettleMarket\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x14\n\x05price\x18\x02 \x01(\tR\x05price\x12\'\n\x0fposition_factor\x18\x03 \x01(\tR\x0epositionFactor"\xf6\x01\n\x12PositionStateEvent\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12\x12\n\x04size\x18\x03 \x01(\x03R\x04size\x12%\n\x0epotential_buys\x18\x04 \x01(\x03R\rpotentialBuys\x12\'\n\x0fpotential_sells\x18\x05 \x01(\x03R\x0epotentialSells\x12 \n\x0cvw_buy_price\x18\x06 \x01(\tR\nvwBuyPrice\x12"\n\rvw_sell_price\x18\x07 \x01(\tR\x0bvwSellPrice"x\n\x10SettleDistressed\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x16\n\x06margin\x18\x03 \x01(\tR\x06margin\x12\x14\n\x05price\x18\x04 \x01(\tR\x05price"I\n\x10\x44istressedOrders\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x18\n\x07parties\x18\x02 \x03(\tR\x07parties"\x84\x01\n\x13\x44istressedPositions\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12-\n\x12\x64istressed_parties\x18\x02 \x03(\tR\x11\x64istressedParties\x12!\n\x0csafe_parties\x18\x03 \x03(\tR\x0bsafeParties"0\n\nMarketTick\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04time\x18\x02 \x01(\x03R\x04time"\x85\x02\n\x0c\x41uctionEvent\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\'\n\x0fopening_auction\x18\x02 \x01(\x08R\x0eopeningAuction\x12\x14\n\x05leave\x18\x03 \x01(\x08R\x05leave\x12\x14\n\x05start\x18\x04 \x01(\x03R\x05start\x12\x10\n\x03\x65nd\x18\x05 \x01(\x03R\x03\x65nd\x12.\n\x07trigger\x18\x06 \x01(\x0e\x32\x14.vega.AuctionTriggerR\x07trigger\x12\x41\n\x11\x65xtension_trigger\x18\x07 \x01(\x0e\x32\x14.vega.AuctionTriggerR\x10\x65xtensionTrigger"\xa9\x03\n\x0fValidatorUpdate\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12 \n\x0cvega_pub_key\x18\x02 \x01(\tR\nvegaPubKey\x12)\n\x10\x65thereum_address\x18\x03 \x01(\tR\x0f\x65thereumAddress\x12\x1c\n\ntm_pub_key\x18\x04 \x01(\tR\x08tmPubKey\x12\x19\n\x08info_url\x18\x05 \x01(\tR\x07infoUrl\x12\x18\n\x07\x63ountry\x18\x06 \x01(\tR\x07\x63ountry\x12\x12\n\x04name\x18\x07 \x01(\tR\x04name\x12\x1d\n\navatar_url\x18\x08 \x01(\tR\tavatarUrl\x12+\n\x12vega_pub_key_index\x18\t \x01(\rR\x0fvegaPubKeyIndex\x12\x14\n\x05\x61\x64\x64\x65\x64\x18\n \x01(\x08R\x05\x61\x64\x64\x65\x64\x12\x1d\n\nfrom_epoch\x18\x0b \x01(\x04R\tfromEpoch\x12+\n\x11submitter_address\x18\x0c \x01(\tR\x10submitterAddress\x12\x1b\n\tepoch_seq\x18\r \x01(\x04R\x08\x65pochSeq"\xb2\x02\n\x15ValidatorRankingEvent\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x1f\n\x0bstake_score\x18\x02 \x01(\tR\nstakeScore\x12+\n\x11performance_score\x18\x03 \x01(\tR\x10performanceScore\x12#\n\rranking_score\x18\x04 \x01(\tR\x0crankingScore\x12\'\n\x0fprevious_status\x18\x05 \x01(\tR\x0epreviousStatus\x12\x1f\n\x0bnext_status\x18\x06 \x01(\tR\nnextStatus\x12\x1b\n\tepoch_seq\x18\x07 \x01(\tR\x08\x65pochSeq\x12&\n\x0ftm_voting_power\x18\x08 \x01(\rR\rtmVotingPower"\x89\x01\n\x0bKeyRotation\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x1e\n\x0bold_pub_key\x18\x02 \x01(\tR\toldPubKey\x12\x1e\n\x0bnew_pub_key\x18\x03 \x01(\tR\tnewPubKey\x12!\n\x0c\x62lock_height\x18\x04 \x01(\x04R\x0b\x62lockHeight"\x93\x01\n\x13\x45thereumKeyRotation\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x1f\n\x0bold_address\x18\x02 \x01(\tR\noldAddress\x12\x1f\n\x0bnew_address\x18\x03 \x01(\tR\nnewAddress\x12!\n\x0c\x62lock_height\x18\x04 \x01(\x04R\x0b\x62lockHeight"\xd7\x01\n\x14ProtocolUpgradeEvent\x12\x30\n\x14upgrade_block_height\x18\x01 \x01(\x04R\x12upgradeBlockHeight\x12(\n\x10vega_release_tag\x18\x02 \x01(\tR\x0evegaReleaseTag\x12\x1c\n\tapprovers\x18\x03 \x03(\tR\tapprovers\x12\x45\n\x06status\x18\x04 \x01(\x0e\x32-.vega.events.v1.ProtocolUpgradeProposalStatusR\x06status"K\n\x08StateVar\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x19\n\x08\x65vent_id\x18\x02 \x01(\tR\x07\x65ventId\x12\x14\n\x05state\x18\x03 \x01(\tR\x05state"V\n\nBeginBlock\x12\x16\n\x06height\x18\x01 \x01(\x04R\x06height\x12\x1c\n\ttimestamp\x18\x02 \x01(\x03R\ttimestamp\x12\x12\n\x04hash\x18\x03 \x01(\tR\x04hash""\n\x08\x45ndBlock\x12\x16\n\x06height\x18\x01 \x01(\x04R\x06height"D\n\x16ProtocolUpgradeStarted\x12*\n\x11last_block_height\x18\x01 \x01(\x04R\x0flastBlockHeight"J\n\x1cProtocolUpgradeDataNodeReady\x12*\n\x11last_block_height\x18\x01 \x01(\x04R\x0flastBlockHeight"\xad\x01\n\x10\x43oreSnapshotData\x12!\n\x0c\x62lock_height\x18\x01 \x01(\x04R\x0b\x62lockHeight\x12\x1d\n\nblock_hash\x18\x02 \x01(\tR\tblockHash\x12!\n\x0c\x63ore_version\x18\x03 \x01(\tR\x0b\x63oreVersion\x12\x34\n\x16protocol_upgrade_block\x18\x04 \x01(\x08R\x14protocolUpgradeBlock"\xb8!\n\x08\x42usEvent\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x14\n\x05\x62lock\x18\x02 \x01(\tR\x05\x62lock\x12\x30\n\x04type\x18\x03 \x01(\x0e\x32\x1c.vega.events.v1.BusEventTypeR\x04type\x12=\n\x0btime_update\x18\x65 \x01(\x0b\x32\x1a.vega.events.v1.TimeUpdateH\x00R\ntimeUpdate\x12L\n\x10ledger_movements\x18\x66 \x01(\x0b\x32\x1f.vega.events.v1.LedgerMovementsH\x00R\x0fledgerMovements\x12U\n\x13position_resolution\x18g \x01(\x0b\x32".vega.events.v1.PositionResolutionH\x00R\x12positionResolution\x12#\n\x05order\x18h \x01(\x0b\x32\x0b.vega.OrderH\x00R\x05order\x12)\n\x07\x61\x63\x63ount\x18i \x01(\x0b\x32\r.vega.AccountH\x00R\x07\x61\x63\x63ount\x12#\n\x05party\x18j \x01(\x0b\x32\x0b.vega.PartyH\x00R\x05party\x12#\n\x05trade\x18k \x01(\x0b\x32\x0b.vega.TradeH\x00R\x05trade\x12\x39\n\rmargin_levels\x18l \x01(\x0b\x32\x12.vega.MarginLevelsH\x00R\x0cmarginLevels\x12,\n\x08proposal\x18m \x01(\x0b\x32\x0e.vega.ProposalH\x00R\x08proposal\x12 \n\x04vote\x18n \x01(\x0b\x32\n.vega.VoteH\x00R\x04vote\x12\x33\n\x0bmarket_data\x18o \x01(\x0b\x32\x10.vega.MarketDataH\x00R\nmarketData\x12H\n\x0enode_signature\x18p \x01(\x0b\x32\x1f.vega.commands.v1.NodeSignatureH\x00R\rnodeSignature\x12R\n\x12loss_socialization\x18q \x01(\x0b\x32!.vega.events.v1.LossSocializationH\x00R\x11lossSocialization\x12I\n\x0fsettle_position\x18r \x01(\x0b\x32\x1e.vega.events.v1.SettlePositionH\x00R\x0esettlePosition\x12O\n\x11settle_distressed\x18s \x01(\x0b\x32 .vega.events.v1.SettleDistressedH\x00R\x10settleDistressed\x12\x35\n\x0emarket_created\x18t \x01(\x0b\x32\x0c.vega.MarketH\x00R\rmarketCreated\x12#\n\x05\x61sset\x18u \x01(\x0b\x32\x0b.vega.AssetH\x00R\x05\x61sset\x12=\n\x0bmarket_tick\x18v \x01(\x0b\x32\x1a.vega.events.v1.MarketTickH\x00R\nmarketTick\x12\x32\n\nwithdrawal\x18w \x01(\x0b\x32\x10.vega.WithdrawalH\x00R\nwithdrawal\x12)\n\x07\x64\x65posit\x18x \x01(\x0b\x32\r.vega.DepositH\x00R\x07\x64\x65posit\x12\x38\n\x07\x61uction\x18y \x01(\x0b\x32\x1c.vega.events.v1.AuctionEventH\x00R\x07\x61uction\x12\x33\n\x0brisk_factor\x18z \x01(\x0b\x32\x10.vega.RiskFactorH\x00R\nriskFactor\x12\x45\n\x11network_parameter\x18{ \x01(\x0b\x32\x16.vega.NetworkParameterH\x00R\x10networkParameter\x12K\n\x13liquidity_provision\x18| \x01(\x0b\x32\x18.vega.LiquidityProvisionH\x00R\x12liquidityProvision\x12\x35\n\x0emarket_updated\x18} \x01(\x0b\x32\x0c.vega.MarketH\x00R\rmarketUpdated\x12\x33\n\x0boracle_spec\x18~ \x01(\x0b\x32\x10.vega.OracleSpecH\x00R\noracleSpec\x12\x33\n\x0boracle_data\x18\x7f \x01(\x0b\x32\x10.vega.OracleDataH\x00R\noracleData\x12X\n\x12\x64\x65legation_balance\x18\x81\x01 \x01(\x0b\x32&.vega.events.v1.DelegationBalanceEventH\x00R\x11\x64\x65legationBalance\x12O\n\x0fvalidator_score\x18\x82\x01 \x01(\x0b\x32#.vega.events.v1.ValidatorScoreEventH\x00R\x0evalidatorScore\x12>\n\x0b\x65poch_event\x18\x83\x01 \x01(\x0b\x32\x1a.vega.events.v1.EpochEventH\x00R\nepochEvent\x12M\n\x10validator_update\x18\x84\x01 \x01(\x0b\x32\x1f.vega.events.v1.ValidatorUpdateH\x00R\x0fvalidatorUpdate\x12\x44\n\rstake_linking\x18\x85\x01 \x01(\x0b\x32\x1c.vega.events.v1.StakeLinkingH\x00R\x0cstakeLinking\x12I\n\rreward_payout\x18\x86\x01 \x01(\x0b\x32!.vega.events.v1.RewardPayoutEventH\x00R\x0crewardPayout\x12\x42\n\ncheckpoint\x18\x87\x01 \x01(\x0b\x32\x1f.vega.events.v1.CheckpointEventH\x00R\ncheckpoint\x12\x41\n\x0ckey_rotation\x18\x88\x01 \x01(\x0b\x32\x1b.vega.events.v1.KeyRotationH\x00R\x0bkeyRotation\x12\x38\n\tstate_var\x18\x89\x01 \x01(\x0b\x32\x18.vega.events.v1.StateVarH\x00R\x08stateVar\x12=\n\x0enetwork_limits\x18\x8a\x01 \x01(\x0b\x32\x13.vega.NetworkLimitsH\x00R\rnetworkLimits\x12\x37\n\x08transfer\x18\x8b\x01 \x01(\x0b\x32\x18.vega.events.v1.TransferH\x00R\x08transfer\x12M\n\rranking_event\x18\x8c\x01 \x01(\x0b\x32%.vega.events.v1.ValidatorRankingEventH\x00R\x0crankingEvent\x12j\n\x1b\x65rc20_multisig_signer_event\x18\x8d\x01 \x01(\x0b\x32(.vega.events.v1.ERC20MultiSigSignerEventH\x00R\x18\x65rc20MultisigSignerEvent\x12}\n"erc20_multisig_set_threshold_event\x18\x8e\x01 \x01(\x0b\x32..vega.events.v1.ERC20MultiSigThresholdSetEventH\x00R\x1e\x65rc20MultisigSetThresholdEvent\x12j\n\x1b\x65rc20_multisig_signer_added\x18\x8f\x01 \x01(\x0b\x32(.vega.events.v1.ERC20MultiSigSignerAddedH\x00R\x18\x65rc20MultisigSignerAdded\x12p\n\x1d\x65rc20_multisig_signer_removed\x18\x90\x01 \x01(\x0b\x32*.vega.events.v1.ERC20MultiSigSignerRemovedH\x00R\x1a\x65rc20MultisigSignerRemoved\x12W\n\x14position_state_event\x18\x91\x01 \x01(\x0b\x32".vega.events.v1.PositionStateEventH\x00R\x12positionStateEvent\x12Z\n\x15\x65thereum_key_rotation\x18\x92\x01 \x01(\x0b\x32#.vega.events.v1.EthereumKeyRotationH\x00R\x13\x65thereumKeyRotation\x12]\n\x16protocol_upgrade_event\x18\x93\x01 \x01(\x0b\x32$.vega.events.v1.ProtocolUpgradeEventH\x00R\x14protocolUpgradeEvent\x12>\n\x0b\x62\x65gin_block\x18\x94\x01 \x01(\x0b\x32\x1a.vega.events.v1.BeginBlockH\x00R\nbeginBlock\x12\x38\n\tend_block\x18\x95\x01 \x01(\x0b\x32\x18.vega.events.v1.EndBlockH\x00R\x08\x65ndBlock\x12\x63\n\x18protocol_upgrade_started\x18\x96\x01 \x01(\x0b\x32&.vega.events.v1.ProtocolUpgradeStartedH\x00R\x16protocolUpgradeStarted\x12\x44\n\rsettle_market\x18\x97\x01 \x01(\x0b\x32\x1c.vega.events.v1.SettleMarketH\x00R\x0csettleMarket\x12S\n\x12transaction_result\x18\x98\x01 \x01(\x0b\x32!.vega.events.v1.TransactionResultH\x00R\x11transactionResult\x12S\n\x13\x63ore_snapshot_event\x18\x99\x01 \x01(\x0b\x32 .vega.events.v1.CoreSnapshotDataH\x00R\x11\x63oreSnapshotEvent\x12w\n protocol_upgrade_data_node_ready\x18\x9a\x01 \x01(\x0b\x32,.vega.events.v1.ProtocolUpgradeDataNodeReadyH\x00R\x1cprotocolUpgradeDataNodeReady\x12P\n\x11\x64istressed_orders\x18\x9b\x01 \x01(\x0b\x32 .vega.events.v1.DistressedOrdersH\x00R\x10\x64istressedOrders\x12G\n\x0e\x65xpired_orders\x18\x9c\x01 \x01(\x0b\x32\x1d.vega.events.v1.ExpiredOrdersH\x00R\rexpiredOrders\x12Y\n\x14\x64istressed_positions\x18\x9d\x01 \x01(\x0b\x32#.vega.events.v1.DistressedPositionsH\x00R\x13\x64istressedPositions\x12\x36\n\x06market\x18\xe9\x07 \x01(\x0b\x32\x1b.vega.events.v1.MarketEventH\x00R\x06market\x12\x41\n\x0ctx_err_event\x18\xd1\x0f \x01(\x0b\x32\x1c.vega.events.v1.TxErrorEventH\x00R\ntxErrEvent\x12\x18\n\x07version\x18\x04 \x01(\rR\x07version\x12\x19\n\x08\x63hain_id\x18\x05 \x01(\tR\x07\x63hainId\x12\x17\n\x07tx_hash\x18\x06 \x01(\tR\x06txHashB\x07\n\x05\x65vent"I\n\rExpiredOrders\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x1b\n\torder_ids\x18\x02 \x03(\tR\x08orderIds*\xdd\x01\n\x1dProtocolUpgradeProposalStatus\x12\x30\n,PROTOCOL_UPGRADE_PROPOSAL_STATUS_UNSPECIFIED\x10\x00\x12,\n(PROTOCOL_UPGRADE_PROPOSAL_STATUS_PENDING\x10\x01\x12-\n)PROTOCOL_UPGRADE_PROPOSAL_STATUS_APPROVED\x10\x02\x12-\n)PROTOCOL_UPGRADE_PROPOSAL_STATUS_REJECTED\x10\x03*\xee\x10\n\x0c\x42usEventType\x12\x1e\n\x1a\x42US_EVENT_TYPE_UNSPECIFIED\x10\x00\x12\x16\n\x12\x42US_EVENT_TYPE_ALL\x10\x01\x12\x1e\n\x1a\x42US_EVENT_TYPE_TIME_UPDATE\x10\x02\x12#\n\x1f\x42US_EVENT_TYPE_LEDGER_MOVEMENTS\x10\x03\x12&\n"BUS_EVENT_TYPE_POSITION_RESOLUTION\x10\x04\x12\x18\n\x14\x42US_EVENT_TYPE_ORDER\x10\x05\x12\x1a\n\x16\x42US_EVENT_TYPE_ACCOUNT\x10\x06\x12\x18\n\x14\x42US_EVENT_TYPE_PARTY\x10\x07\x12\x18\n\x14\x42US_EVENT_TYPE_TRADE\x10\x08\x12 \n\x1c\x42US_EVENT_TYPE_MARGIN_LEVELS\x10\t\x12\x1b\n\x17\x42US_EVENT_TYPE_PROPOSAL\x10\n\x12\x17\n\x13\x42US_EVENT_TYPE_VOTE\x10\x0b\x12\x1e\n\x1a\x42US_EVENT_TYPE_MARKET_DATA\x10\x0c\x12!\n\x1d\x42US_EVENT_TYPE_NODE_SIGNATURE\x10\r\x12%\n!BUS_EVENT_TYPE_LOSS_SOCIALIZATION\x10\x0e\x12"\n\x1e\x42US_EVENT_TYPE_SETTLE_POSITION\x10\x0f\x12$\n BUS_EVENT_TYPE_SETTLE_DISTRESSED\x10\x10\x12!\n\x1d\x42US_EVENT_TYPE_MARKET_CREATED\x10\x11\x12\x18\n\x14\x42US_EVENT_TYPE_ASSET\x10\x12\x12\x1e\n\x1a\x42US_EVENT_TYPE_MARKET_TICK\x10\x13\x12\x1d\n\x19\x42US_EVENT_TYPE_WITHDRAWAL\x10\x14\x12\x1a\n\x16\x42US_EVENT_TYPE_DEPOSIT\x10\x15\x12\x1a\n\x16\x42US_EVENT_TYPE_AUCTION\x10\x16\x12\x1e\n\x1a\x42US_EVENT_TYPE_RISK_FACTOR\x10\x17\x12$\n BUS_EVENT_TYPE_NETWORK_PARAMETER\x10\x18\x12&\n"BUS_EVENT_TYPE_LIQUIDITY_PROVISION\x10\x19\x12!\n\x1d\x42US_EVENT_TYPE_MARKET_UPDATED\x10\x1a\x12\x1e\n\x1a\x42US_EVENT_TYPE_ORACLE_SPEC\x10\x1b\x12\x1e\n\x1a\x42US_EVENT_TYPE_ORACLE_DATA\x10\x1c\x12%\n!BUS_EVENT_TYPE_DELEGATION_BALANCE\x10\x1d\x12"\n\x1e\x42US_EVENT_TYPE_VALIDATOR_SCORE\x10\x1e\x12\x1f\n\x1b\x42US_EVENT_TYPE_EPOCH_UPDATE\x10\x1f\x12#\n\x1f\x42US_EVENT_TYPE_VALIDATOR_UPDATE\x10 \x12 \n\x1c\x42US_EVENT_TYPE_STAKE_LINKING\x10!\x12&\n"BUS_EVENT_TYPE_REWARD_PAYOUT_EVENT\x10"\x12\x1d\n\x19\x42US_EVENT_TYPE_CHECKPOINT\x10#\x12\x1f\n\x1b\x42US_EVENT_TYPE_STREAM_START\x10$\x12\x1f\n\x1b\x42US_EVENT_TYPE_KEY_ROTATION\x10%\x12\x1c\n\x18\x42US_EVENT_TYPE_STATE_VAR\x10&\x12!\n\x1d\x42US_EVENT_TYPE_NETWORK_LIMITS\x10\'\x12\x1b\n\x17\x42US_EVENT_TYPE_TRANSFER\x10(\x12$\n BUS_EVENT_TYPE_VALIDATOR_RANKING\x10)\x12/\n+BUS_EVENT_TYPE_ERC20_MULTI_SIG_SIGNER_EVENT\x10*\x12\x30\n,BUS_EVENT_TYPE_ERC20_MULTI_SIG_SET_THRESHOLD\x10+\x12/\n+BUS_EVENT_TYPE_ERC20_MULTI_SIG_SIGNER_ADDED\x10,\x12\x31\n-BUS_EVENT_TYPE_ERC20_MULTI_SIG_SIGNER_REMOVED\x10-\x12!\n\x1d\x42US_EVENT_TYPE_POSITION_STATE\x10.\x12(\n$BUS_EVENT_TYPE_ETHEREUM_KEY_ROTATION\x10/\x12,\n(BUS_EVENT_TYPE_PROTOCOL_UPGRADE_PROPOSAL\x10\x30\x12\x1e\n\x1a\x42US_EVENT_TYPE_BEGIN_BLOCK\x10\x31\x12\x1c\n\x18\x42US_EVENT_TYPE_END_BLOCK\x10\x32\x12+\n\'BUS_EVENT_TYPE_PROTOCOL_UPGRADE_STARTED\x10\x33\x12 \n\x1c\x42US_EVENT_TYPE_SETTLE_MARKET\x10\x34\x12%\n!BUS_EVENT_TYPE_TRANSACTION_RESULT\x10\x35\x12!\n\x1d\x42US_EVENT_TYPE_SNAPSHOT_TAKEN\x10\x36\x12\x33\n/BUS_EVENT_TYPE_PROTOCOL_UPGRADE_DATA_NODE_READY\x10\x37\x12+\n\'BUS_EVENT_TYPE_DISTRESSED_ORDERS_CLOSED\x10\x38\x12!\n\x1d\x42US_EVENT_TYPE_EXPIRED_ORDERS\x10\x39\x12\'\n#BUS_EVENT_TYPE_DISTRESSED_POSITIONS\x10:\x12\x19\n\x15\x42US_EVENT_TYPE_MARKET\x10\x65\x12\x1c\n\x17\x42US_EVENT_TYPE_TX_ERROR\x10\xc9\x01\x42\x31Z/code.vegaprotocol.io/vega/protos/vega/events/v1b\x06proto3'
+    b'\n\x1bvega/events/v1/events.proto\x12\x0evega.events.v1\x1a\x11vega/assets.proto\x1a\x1fvega/commands/v1/commands.proto\x1a\x1bvega/commands/v1/data.proto\x1a)vega/commands/v1/validator_commands.proto\x1a\x15vega/governance.proto\x1a\x12vega/markets.proto\x1a\x11vega/oracle.proto\x1a\x0fvega/vega.proto"\x83\x01\n\x0eStopOrderEvent\x12\x41\n\nsubmission\x18\x01 \x01(\x0b\x32!.vega.commands.v1.OrderSubmissionR\nsubmission\x12.\n\nstop_order\x18\x02 \x01(\x0b\x32\x0f.vega.StopOrderR\tstopOrder"\xee\x01\n\x18\x45RC20MultiSigSignerAdded\x12!\n\x0csignature_id\x18\x01 \x01(\tR\x0bsignatureId\x12!\n\x0cvalidator_id\x18\x02 \x01(\tR\x0bvalidatorId\x12\x1c\n\ttimestamp\x18\x03 \x01(\x03R\ttimestamp\x12\x1d\n\nnew_signer\x18\x04 \x01(\tR\tnewSigner\x12\x1c\n\tsubmitter\x18\x05 \x01(\tR\tsubmitter\x12\x14\n\x05nonce\x18\x06 \x01(\tR\x05nonce\x12\x1b\n\tepoch_seq\x18\x07 \x01(\tR\x08\x65pochSeq"f\n#ERC20MultiSigSignerRemovedSubmitter\x12!\n\x0csignature_id\x18\x01 \x01(\tR\x0bsignatureId\x12\x1c\n\tsubmitter\x18\x02 \x01(\tR\tsubmitter"\x97\x02\n\x1a\x45RC20MultiSigSignerRemoved\x12\x66\n\x14signature_submitters\x18\x01 \x03(\x0b\x32\x33.vega.events.v1.ERC20MultiSigSignerRemovedSubmitterR\x13signatureSubmitters\x12!\n\x0cvalidator_id\x18\x02 \x01(\tR\x0bvalidatorId\x12\x1c\n\ttimestamp\x18\x03 \x01(\x03R\ttimestamp\x12\x1d\n\nold_signer\x18\x04 \x01(\tR\toldSigner\x12\x14\n\x05nonce\x18\x05 \x01(\tR\x05nonce\x12\x1b\n\tepoch_seq\x18\x06 \x01(\tR\x08\x65pochSeq"\xcc\x06\n\x08Transfer\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04\x66rom\x18\x02 \x01(\tR\x04\x66rom\x12=\n\x11\x66rom_account_type\x18\x03 \x01(\x0e\x32\x11.vega.AccountTypeR\x0f\x66romAccountType\x12\x0e\n\x02to\x18\x04 \x01(\tR\x02to\x12\x39\n\x0fto_account_type\x18\x05 \x01(\x0e\x32\x11.vega.AccountTypeR\rtoAccountType\x12\x14\n\x05\x61sset\x18\x06 \x01(\tR\x05\x61sset\x12\x16\n\x06\x61mount\x18\x07 \x01(\tR\x06\x61mount\x12\x1c\n\treference\x18\x08 \x01(\tR\treference\x12\x37\n\x06status\x18\t \x01(\x0e\x32\x1f.vega.events.v1.Transfer.StatusR\x06status\x12\x1c\n\ttimestamp\x18\n \x01(\x03R\ttimestamp\x12\x1b\n\x06reason\x18\x0b \x01(\tH\x01R\x06reason\x88\x01\x01\x12\x39\n\x07one_off\x18\x65 \x01(\x0b\x32\x1e.vega.events.v1.OneOffTransferH\x00R\x06oneOff\x12\x41\n\trecurring\x18\x66 \x01(\x0b\x32!.vega.events.v1.RecurringTransferH\x00R\trecurring\x12X\n\x12one_off_governance\x18g \x01(\x0b\x32(.vega.events.v1.OneOffGovernanceTransferH\x00R\x10oneOffGovernance\x12`\n\x14recurring_governance\x18h \x01(\x0b\x32+.vega.events.v1.RecurringGovernanceTransferH\x00R\x13recurringGovernance"\x84\x01\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x12\n\x0eSTATUS_PENDING\x10\x01\x12\x0f\n\x0bSTATUS_DONE\x10\x02\x12\x13\n\x0fSTATUS_REJECTED\x10\x03\x12\x12\n\x0eSTATUS_STOPPED\x10\x04\x12\x14\n\x10STATUS_CANCELLED\x10\x05\x42\x06\n\x04kindB\t\n\x07_reason"9\n\x18OneOffGovernanceTransfer\x12\x1d\n\ndeliver_on\x18\x01 \x01(\x03R\tdeliverOn"/\n\x0eOneOffTransfer\x12\x1d\n\ndeliver_on\x18\x01 \x01(\x03R\tdeliverOn"\xc1\x01\n\x11RecurringTransfer\x12\x1f\n\x0bstart_epoch\x18\x01 \x01(\x04R\nstartEpoch\x12 \n\tend_epoch\x18\x02 \x01(\x04H\x00R\x08\x65ndEpoch\x88\x01\x01\x12\x16\n\x06\x66\x61\x63tor\x18\x03 \x01(\tR\x06\x66\x61\x63tor\x12\x43\n\x11\x64ispatch_strategy\x18\x04 \x01(\x0b\x32\x16.vega.DispatchStrategyR\x10\x64ispatchStrategyB\x0c\n\n_end_epoch"n\n\x1bRecurringGovernanceTransfer\x12\x1f\n\x0bstart_epoch\x18\x01 \x01(\x04R\nstartEpoch\x12 \n\tend_epoch\x18\x02 \x01(\x04H\x00R\x08\x65ndEpoch\x88\x01\x01\x42\x0c\n\n_end_epoch"\xb4\x04\n\x0cStakeLinking\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x35\n\x04type\x18\x02 \x01(\x0e\x32!.vega.events.v1.StakeLinking.TypeR\x04type\x12\x0e\n\x02ts\x18\x03 \x01(\x03R\x02ts\x12\x14\n\x05party\x18\x04 \x01(\tR\x05party\x12\x16\n\x06\x61mount\x18\x05 \x01(\tR\x06\x61mount\x12;\n\x06status\x18\x06 \x01(\x0e\x32#.vega.events.v1.StakeLinking.StatusR\x06status\x12!\n\x0c\x66inalized_at\x18\x07 \x01(\x03R\x0b\x66inalizedAt\x12\x17\n\x07tx_hash\x18\x08 \x01(\tR\x06txHash\x12!\n\x0c\x62lock_height\x18\t \x01(\x04R\x0b\x62lockHeight\x12\x1d\n\nblock_time\x18\n \x01(\x03R\tblockTime\x12\x1b\n\tlog_index\x18\x0b \x01(\x04R\x08logIndex\x12)\n\x10\x65thereum_address\x18\x0c \x01(\tR\x0f\x65thereumAddress"<\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\r\n\tTYPE_LINK\x10\x01\x12\x0f\n\x0bTYPE_UNLINK\x10\x02"^\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x12\n\x0eSTATUS_PENDING\x10\x01\x12\x13\n\x0fSTATUS_ACCEPTED\x10\x02\x12\x13\n\x0fSTATUS_REJECTED\x10\x03"\xd3\x02\n\x18\x45RC20MultiSigSignerEvent\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x41\n\x04type\x18\x02 \x01(\x0e\x32-.vega.events.v1.ERC20MultiSigSignerEvent.TypeR\x04type\x12\x16\n\x06signer\x18\x03 \x01(\tR\x06signer\x12\x14\n\x05nonce\x18\x04 \x01(\tR\x05nonce\x12\x1d\n\nblock_time\x18\x05 \x01(\x03R\tblockTime\x12\x17\n\x07tx_hash\x18\x06 \x01(\tR\x06txHash\x12\x1b\n\tlog_index\x18\x07 \x01(\x04R\x08logIndex\x12!\n\x0c\x62lock_number\x18\x08 \x01(\x04R\x0b\x62lockNumber">\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x0e\n\nTYPE_ADDED\x10\x01\x12\x10\n\x0cTYPE_REMOVED\x10\x02"\xe3\x01\n\x1e\x45RC20MultiSigThresholdSetEvent\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12#\n\rnew_threshold\x18\x02 \x01(\rR\x0cnewThreshold\x12\x14\n\x05nonce\x18\x03 \x01(\tR\x05nonce\x12\x1d\n\nblock_time\x18\x04 \x01(\x03R\tblockTime\x12\x17\n\x07tx_hash\x18\x05 \x01(\tR\x06txHash\x12\x1b\n\tlog_index\x18\x06 \x01(\x04R\x08logIndex\x12!\n\x0c\x62lock_number\x18\x07 \x01(\x04R\x0b\x62lockNumber"g\n\x0f\x43heckpointEvent\x12\x12\n\x04hash\x18\x01 \x01(\tR\x04hash\x12\x1d\n\nblock_hash\x18\x02 \x01(\tR\tblockHash\x12!\n\x0c\x62lock_height\x18\x03 \x01(\x04R\x0b\x62lockHeight"-\n\x10StreamStartEvent\x12\x19\n\x08\x63hain_id\x18\x01 \x01(\tR\x07\x63hainId"\x82\x02\n\x11RewardPayoutEvent\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x1b\n\tepoch_seq\x18\x02 \x01(\tR\x08\x65pochSeq\x12\x14\n\x05\x61sset\x18\x03 \x01(\tR\x05\x61sset\x12\x16\n\x06\x61mount\x18\x04 \x01(\tR\x06\x61mount\x12\x35\n\x17percent_of_total_reward\x18\x05 \x01(\tR\x14percentOfTotalReward\x12\x1c\n\ttimestamp\x18\x06 \x01(\x03R\ttimestamp\x12\x1f\n\x0breward_type\x18\x07 \x01(\tR\nrewardType\x12\x16\n\x06market\x18\x08 \x01(\tR\x06market"\xd6\x02\n\x13ValidatorScoreEvent\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x1b\n\tepoch_seq\x18\x02 \x01(\tR\x08\x65pochSeq\x12\'\n\x0fvalidator_score\x18\x03 \x01(\tR\x0evalidatorScore\x12)\n\x10normalised_score\x18\x04 \x01(\tR\x0fnormalisedScore\x12\x33\n\x15validator_performance\x18\x05 \x01(\tR\x14validatorPerformance\x12.\n\x13raw_validator_score\x18\x06 \x01(\tR\x11rawValidatorScore\x12)\n\x10validator_status\x18\x07 \x01(\tR\x0fvalidatorStatus\x12%\n\x0emultisig_score\x18\x08 \x01(\tR\rmultisigScore"|\n\x16\x44\x65legationBalanceEvent\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x17\n\x07node_id\x18\x02 \x01(\tR\x06nodeId\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount\x12\x1b\n\tepoch_seq\x18\x04 \x01(\tR\x08\x65pochSeq"D\n\x0bMarketEvent\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x18\n\x07payload\x18\x02 \x01(\tR\x07payload"\xaf\x12\n\x11TransactionResult\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12\x16\n\x06status\x18\x02 \x01(\x08R\x06status\x12\x12\n\x04hash\x18\x03 \x01(\tR\x04hash\x12N\n\x10order_submission\x18\x65 \x01(\x0b\x32!.vega.commands.v1.OrderSubmissionH\x00R\x0forderSubmission\x12K\n\x0forder_amendment\x18\x66 \x01(\x0b\x32 .vega.commands.v1.OrderAmendmentH\x00R\x0eorderAmendment\x12T\n\x12order_cancellation\x18g \x01(\x0b\x32#.vega.commands.v1.OrderCancellationH\x00R\x11orderCancellation\x12\x42\n\x08proposal\x18h \x01(\x0b\x32$.vega.commands.v1.ProposalSubmissionH\x00R\x08proposal\x12K\n\x0fvote_submission\x18i \x01(\x0b\x32 .vega.commands.v1.VoteSubmissionH\x00R\x0evoteSubmission\x12v\n\x1eliquidity_provision_submission\x18j \x01(\x0b\x32..vega.commands.v1.LiquidityProvisionSubmissionH\x00R\x1cliquidityProvisionSubmission\x12W\n\x13withdraw_submission\x18k \x01(\x0b\x32$.vega.commands.v1.WithdrawSubmissionH\x00R\x12withdrawSubmission\x12W\n\x13\x64\x65legate_submission\x18l \x01(\x0b\x32$.vega.commands.v1.DelegateSubmissionH\x00R\x12\x64\x65legateSubmission\x12]\n\x15undelegate_submission\x18m \x01(\x0b\x32&.vega.commands.v1.UndelegateSubmissionH\x00R\x14undelegateSubmission\x12|\n liquidity_provision_cancellation\x18o \x01(\x0b\x32\x30.vega.commands.v1.LiquidityProvisionCancellationH\x00R\x1eliquidityProvisionCancellation\x12s\n\x1dliquidity_provision_amendment\x18p \x01(\x0b\x32-.vega.commands.v1.LiquidityProvisionAmendmentH\x00R\x1bliquidityProvisionAmendment\x12\x38\n\x08transfer\x18q \x01(\x0b\x32\x1a.vega.commands.v1.TransferH\x00R\x08transfer\x12K\n\x0f\x63\x61ncel_transfer\x18r \x01(\x0b\x32 .vega.commands.v1.CancelTransferH\x00R\x0e\x63\x61ncelTransfer\x12\x45\n\rannounce_node\x18s \x01(\x0b\x32\x1e.vega.commands.v1.AnnounceNodeH\x00R\x0c\x61nnounceNode\x12^\n\x16oracle_data_submission\x18t \x01(\x0b\x32&.vega.commands.v1.OracleDataSubmissionH\x00R\x14oracleDataSubmission\x12g\n\x19protocol_upgrade_proposal\x18u \x01(\x0b\x32).vega.commands.v1.ProtocolUpgradeProposalH\x00R\x17protocolUpgradeProposal\x12N\n\x10issue_signatures\x18v \x01(\x0b\x32!.vega.commands.v1.IssueSignaturesH\x00R\x0fissueSignatures\x12g\n\x19\x62\x61tch_market_instructions\x18w \x01(\x0b\x32).vega.commands.v1.BatchMarketInstructionsH\x00R\x17\x62\x61tchMarketInstructions\x12[\n\x15key_rotate_submission\x18x \x01(\x0b\x32%.vega.commands.v1.KeyRotateSubmissionH\x00R\x13keyRotateSubmission\x12t\n\x1e\x65thereum_key_rotate_submission\x18y \x01(\x0b\x32-.vega.commands.v1.EthereumKeyRotateSubmissionH\x00R\x1b\x65thereumKeyRotateSubmission\x12\\\n\x15stop_order_submission\x18z \x01(\x0b\x32&.vega.commands.v1.StopOrdersSubmissionH\x00R\x13stopOrderSubmission\x12\x62\n\x17stop_order_cancellation\x18{ \x01(\x0b\x32(.vega.commands.v1.StopOrdersCancellationH\x00R\x15stopOrderCancellation\x12M\n\x07success\x18\xe9\x07 \x01(\x0b\x32\x30.vega.events.v1.TransactionResult.SuccessDetailsH\x01R\x07success\x12M\n\x07\x66\x61ilure\x18\xea\x07 \x01(\x0b\x32\x30.vega.events.v1.TransactionResult.FailureDetailsH\x01R\x07\x66\x61ilure\x1a\x10\n\x0eSuccessDetails\x1a&\n\x0e\x46\x61ilureDetails\x12\x14\n\x05\x65rror\x18\x01 \x01(\tR\x05\x65rrorB\r\n\x0btransactionB\x07\n\x05\x65xtra"\xa7\r\n\x0cTxErrorEvent\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12\x17\n\x07\x65rr_msg\x18\x02 \x01(\tR\x06\x65rrMsg\x12N\n\x10order_submission\x18\x65 \x01(\x0b\x32!.vega.commands.v1.OrderSubmissionH\x00R\x0forderSubmission\x12K\n\x0forder_amendment\x18\x66 \x01(\x0b\x32 .vega.commands.v1.OrderAmendmentH\x00R\x0eorderAmendment\x12T\n\x12order_cancellation\x18g \x01(\x0b\x32#.vega.commands.v1.OrderCancellationH\x00R\x11orderCancellation\x12\x42\n\x08proposal\x18h \x01(\x0b\x32$.vega.commands.v1.ProposalSubmissionH\x00R\x08proposal\x12K\n\x0fvote_submission\x18i \x01(\x0b\x32 .vega.commands.v1.VoteSubmissionH\x00R\x0evoteSubmission\x12v\n\x1eliquidity_provision_submission\x18j \x01(\x0b\x32..vega.commands.v1.LiquidityProvisionSubmissionH\x00R\x1cliquidityProvisionSubmission\x12W\n\x13withdraw_submission\x18k \x01(\x0b\x32$.vega.commands.v1.WithdrawSubmissionH\x00R\x12withdrawSubmission\x12W\n\x13\x64\x65legate_submission\x18l \x01(\x0b\x32$.vega.commands.v1.DelegateSubmissionH\x00R\x12\x64\x65legateSubmission\x12]\n\x15undelegate_submission\x18m \x01(\x0b\x32&.vega.commands.v1.UndelegateSubmissionH\x00R\x14undelegateSubmission\x12|\n liquidity_provision_cancellation\x18o \x01(\x0b\x32\x30.vega.commands.v1.LiquidityProvisionCancellationH\x00R\x1eliquidityProvisionCancellation\x12s\n\x1dliquidity_provision_amendment\x18p \x01(\x0b\x32-.vega.commands.v1.LiquidityProvisionAmendmentH\x00R\x1bliquidityProvisionAmendment\x12\x38\n\x08transfer\x18q \x01(\x0b\x32\x1a.vega.commands.v1.TransferH\x00R\x08transfer\x12K\n\x0f\x63\x61ncel_transfer\x18r \x01(\x0b\x32 .vega.commands.v1.CancelTransferH\x00R\x0e\x63\x61ncelTransfer\x12\x45\n\rannounce_node\x18s \x01(\x0b\x32\x1e.vega.commands.v1.AnnounceNodeH\x00R\x0c\x61nnounceNode\x12^\n\x16oracle_data_submission\x18t \x01(\x0b\x32&.vega.commands.v1.OracleDataSubmissionH\x00R\x14oracleDataSubmission\x12g\n\x19protocol_upgrade_proposal\x18u \x01(\x0b\x32).vega.commands.v1.ProtocolUpgradeProposalH\x00R\x17protocolUpgradeProposal\x12N\n\x10issue_signatures\x18v \x01(\x0b\x32!.vega.commands.v1.IssueSignaturesH\x00R\x0fissueSignatures\x12g\n\x19\x62\x61tch_market_instructions\x18w \x01(\x0b\x32).vega.commands.v1.BatchMarketInstructionsH\x00R\x17\x62\x61tchMarketInstructionsB\r\n\x0btransactionJ\x04\x08n\x10o"*\n\nTimeUpdate\x12\x1c\n\ttimestamp\x18\x01 \x01(\x03R\ttimestamp"\xa4\x01\n\nEpochEvent\x12\x10\n\x03seq\x18\x01 \x01(\x04R\x03seq\x12)\n\x06\x61\x63tion\x18\x02 \x01(\x0e\x32\x11.vega.EpochActionR\x06\x61\x63tion\x12\x1d\n\nstart_time\x18\x03 \x01(\x03R\tstartTime\x12\x1f\n\x0b\x65xpire_time\x18\x04 \x01(\x03R\nexpireTime\x12\x19\n\x08\x65nd_time\x18\x05 \x01(\x03R\x07\x65ndTime"R\n\x0fLedgerMovements\x12?\n\x10ledger_movements\x18\x01 \x03(\x0b\x32\x14.vega.LedgerMovementR\x0fledgerMovements"\x88\x01\n\x12PositionResolution\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x1e\n\ndistressed\x18\x02 \x01(\x03R\ndistressed\x12\x16\n\x06\x63losed\x18\x03 \x01(\x03R\x06\x63losed\x12\x1d\n\nmark_price\x18\x04 \x01(\tR\tmarkPrice"c\n\x11LossSocialization\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount"^\n\x0fTradeSettlement\x12\x12\n\x04size\x18\x01 \x01(\x03R\x04size\x12\x14\n\x05price\x18\x02 \x01(\tR\x05price\x12!\n\x0cmarket_price\x18\x03 \x01(\tR\x0bmarketPrice"\xd5\x01\n\x0eSettlePosition\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x14\n\x05price\x18\x03 \x01(\tR\x05price\x12L\n\x11trade_settlements\x18\x04 \x03(\x0b\x32\x1f.vega.events.v1.TradeSettlementR\x10tradeSettlements\x12\'\n\x0fposition_factor\x18\x05 \x01(\tR\x0epositionFactor"j\n\x0cSettleMarket\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x14\n\x05price\x18\x02 \x01(\tR\x05price\x12\'\n\x0fposition_factor\x18\x03 \x01(\tR\x0epositionFactor"\xf6\x01\n\x12PositionStateEvent\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12\x12\n\x04size\x18\x03 \x01(\x03R\x04size\x12%\n\x0epotential_buys\x18\x04 \x01(\x03R\rpotentialBuys\x12\'\n\x0fpotential_sells\x18\x05 \x01(\x03R\x0epotentialSells\x12 \n\x0cvw_buy_price\x18\x06 \x01(\tR\nvwBuyPrice\x12"\n\rvw_sell_price\x18\x07 \x01(\tR\x0bvwSellPrice"x\n\x10SettleDistressed\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x16\n\x06margin\x18\x03 \x01(\tR\x06margin\x12\x14\n\x05price\x18\x04 \x01(\tR\x05price"I\n\x10\x44istressedOrders\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x18\n\x07parties\x18\x02 \x03(\tR\x07parties"\x84\x01\n\x13\x44istressedPositions\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12-\n\x12\x64istressed_parties\x18\x02 \x03(\tR\x11\x64istressedParties\x12!\n\x0csafe_parties\x18\x03 \x03(\tR\x0bsafeParties"0\n\nMarketTick\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04time\x18\x02 \x01(\x03R\x04time"\x85\x02\n\x0c\x41uctionEvent\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\'\n\x0fopening_auction\x18\x02 \x01(\x08R\x0eopeningAuction\x12\x14\n\x05leave\x18\x03 \x01(\x08R\x05leave\x12\x14\n\x05start\x18\x04 \x01(\x03R\x05start\x12\x10\n\x03\x65nd\x18\x05 \x01(\x03R\x03\x65nd\x12.\n\x07trigger\x18\x06 \x01(\x0e\x32\x14.vega.AuctionTriggerR\x07trigger\x12\x41\n\x11\x65xtension_trigger\x18\x07 \x01(\x0e\x32\x14.vega.AuctionTriggerR\x10\x65xtensionTrigger"\xa9\x03\n\x0fValidatorUpdate\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12 \n\x0cvega_pub_key\x18\x02 \x01(\tR\nvegaPubKey\x12)\n\x10\x65thereum_address\x18\x03 \x01(\tR\x0f\x65thereumAddress\x12\x1c\n\ntm_pub_key\x18\x04 \x01(\tR\x08tmPubKey\x12\x19\n\x08info_url\x18\x05 \x01(\tR\x07infoUrl\x12\x18\n\x07\x63ountry\x18\x06 \x01(\tR\x07\x63ountry\x12\x12\n\x04name\x18\x07 \x01(\tR\x04name\x12\x1d\n\navatar_url\x18\x08 \x01(\tR\tavatarUrl\x12+\n\x12vega_pub_key_index\x18\t \x01(\rR\x0fvegaPubKeyIndex\x12\x14\n\x05\x61\x64\x64\x65\x64\x18\n \x01(\x08R\x05\x61\x64\x64\x65\x64\x12\x1d\n\nfrom_epoch\x18\x0b \x01(\x04R\tfromEpoch\x12+\n\x11submitter_address\x18\x0c \x01(\tR\x10submitterAddress\x12\x1b\n\tepoch_seq\x18\r \x01(\x04R\x08\x65pochSeq"\xb2\x02\n\x15ValidatorRankingEvent\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x1f\n\x0bstake_score\x18\x02 \x01(\tR\nstakeScore\x12+\n\x11performance_score\x18\x03 \x01(\tR\x10performanceScore\x12#\n\rranking_score\x18\x04 \x01(\tR\x0crankingScore\x12\'\n\x0fprevious_status\x18\x05 \x01(\tR\x0epreviousStatus\x12\x1f\n\x0bnext_status\x18\x06 \x01(\tR\nnextStatus\x12\x1b\n\tepoch_seq\x18\x07 \x01(\tR\x08\x65pochSeq\x12&\n\x0ftm_voting_power\x18\x08 \x01(\rR\rtmVotingPower"\x89\x01\n\x0bKeyRotation\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x1e\n\x0bold_pub_key\x18\x02 \x01(\tR\toldPubKey\x12\x1e\n\x0bnew_pub_key\x18\x03 \x01(\tR\tnewPubKey\x12!\n\x0c\x62lock_height\x18\x04 \x01(\x04R\x0b\x62lockHeight"\x93\x01\n\x13\x45thereumKeyRotation\x12\x17\n\x07node_id\x18\x01 \x01(\tR\x06nodeId\x12\x1f\n\x0bold_address\x18\x02 \x01(\tR\noldAddress\x12\x1f\n\x0bnew_address\x18\x03 \x01(\tR\nnewAddress\x12!\n\x0c\x62lock_height\x18\x04 \x01(\x04R\x0b\x62lockHeight"\xd7\x01\n\x14ProtocolUpgradeEvent\x12\x30\n\x14upgrade_block_height\x18\x01 \x01(\x04R\x12upgradeBlockHeight\x12(\n\x10vega_release_tag\x18\x02 \x01(\tR\x0evegaReleaseTag\x12\x1c\n\tapprovers\x18\x03 \x03(\tR\tapprovers\x12\x45\n\x06status\x18\x04 \x01(\x0e\x32-.vega.events.v1.ProtocolUpgradeProposalStatusR\x06status"K\n\x08StateVar\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x19\n\x08\x65vent_id\x18\x02 \x01(\tR\x07\x65ventId\x12\x14\n\x05state\x18\x03 \x01(\tR\x05state"V\n\nBeginBlock\x12\x16\n\x06height\x18\x01 \x01(\x04R\x06height\x12\x1c\n\ttimestamp\x18\x02 \x01(\x03R\ttimestamp\x12\x12\n\x04hash\x18\x03 \x01(\tR\x04hash""\n\x08\x45ndBlock\x12\x16\n\x06height\x18\x01 \x01(\x04R\x06height"D\n\x16ProtocolUpgradeStarted\x12*\n\x11last_block_height\x18\x01 \x01(\x04R\x0flastBlockHeight"J\n\x1cProtocolUpgradeDataNodeReady\x12*\n\x11last_block_height\x18\x01 \x01(\x04R\x0flastBlockHeight"\xad\x01\n\x10\x43oreSnapshotData\x12!\n\x0c\x62lock_height\x18\x01 \x01(\x04R\x0b\x62lockHeight\x12\x1d\n\nblock_hash\x18\x02 \x01(\tR\tblockHash\x12!\n\x0c\x63ore_version\x18\x03 \x01(\tR\x0b\x63oreVersion\x12\x34\n\x16protocol_upgrade_block\x18\x04 \x01(\x08R\x14protocolUpgradeBlock"\xeb!\n\x08\x42usEvent\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x14\n\x05\x62lock\x18\x02 \x01(\tR\x05\x62lock\x12\x30\n\x04type\x18\x03 \x01(\x0e\x32\x1c.vega.events.v1.BusEventTypeR\x04type\x12=\n\x0btime_update\x18\x65 \x01(\x0b\x32\x1a.vega.events.v1.TimeUpdateH\x00R\ntimeUpdate\x12L\n\x10ledger_movements\x18\x66 \x01(\x0b\x32\x1f.vega.events.v1.LedgerMovementsH\x00R\x0fledgerMovements\x12U\n\x13position_resolution\x18g \x01(\x0b\x32".vega.events.v1.PositionResolutionH\x00R\x12positionResolution\x12#\n\x05order\x18h \x01(\x0b\x32\x0b.vega.OrderH\x00R\x05order\x12)\n\x07\x61\x63\x63ount\x18i \x01(\x0b\x32\r.vega.AccountH\x00R\x07\x61\x63\x63ount\x12#\n\x05party\x18j \x01(\x0b\x32\x0b.vega.PartyH\x00R\x05party\x12#\n\x05trade\x18k \x01(\x0b\x32\x0b.vega.TradeH\x00R\x05trade\x12\x39\n\rmargin_levels\x18l \x01(\x0b\x32\x12.vega.MarginLevelsH\x00R\x0cmarginLevels\x12,\n\x08proposal\x18m \x01(\x0b\x32\x0e.vega.ProposalH\x00R\x08proposal\x12 \n\x04vote\x18n \x01(\x0b\x32\n.vega.VoteH\x00R\x04vote\x12\x33\n\x0bmarket_data\x18o \x01(\x0b\x32\x10.vega.MarketDataH\x00R\nmarketData\x12H\n\x0enode_signature\x18p \x01(\x0b\x32\x1f.vega.commands.v1.NodeSignatureH\x00R\rnodeSignature\x12R\n\x12loss_socialization\x18q \x01(\x0b\x32!.vega.events.v1.LossSocializationH\x00R\x11lossSocialization\x12I\n\x0fsettle_position\x18r \x01(\x0b\x32\x1e.vega.events.v1.SettlePositionH\x00R\x0esettlePosition\x12O\n\x11settle_distressed\x18s \x01(\x0b\x32 .vega.events.v1.SettleDistressedH\x00R\x10settleDistressed\x12\x35\n\x0emarket_created\x18t \x01(\x0b\x32\x0c.vega.MarketH\x00R\rmarketCreated\x12#\n\x05\x61sset\x18u \x01(\x0b\x32\x0b.vega.AssetH\x00R\x05\x61sset\x12=\n\x0bmarket_tick\x18v \x01(\x0b\x32\x1a.vega.events.v1.MarketTickH\x00R\nmarketTick\x12\x32\n\nwithdrawal\x18w \x01(\x0b\x32\x10.vega.WithdrawalH\x00R\nwithdrawal\x12)\n\x07\x64\x65posit\x18x \x01(\x0b\x32\r.vega.DepositH\x00R\x07\x64\x65posit\x12\x38\n\x07\x61uction\x18y \x01(\x0b\x32\x1c.vega.events.v1.AuctionEventH\x00R\x07\x61uction\x12\x33\n\x0brisk_factor\x18z \x01(\x0b\x32\x10.vega.RiskFactorH\x00R\nriskFactor\x12\x45\n\x11network_parameter\x18{ \x01(\x0b\x32\x16.vega.NetworkParameterH\x00R\x10networkParameter\x12K\n\x13liquidity_provision\x18| \x01(\x0b\x32\x18.vega.LiquidityProvisionH\x00R\x12liquidityProvision\x12\x35\n\x0emarket_updated\x18} \x01(\x0b\x32\x0c.vega.MarketH\x00R\rmarketUpdated\x12\x33\n\x0boracle_spec\x18~ \x01(\x0b\x32\x10.vega.OracleSpecH\x00R\noracleSpec\x12\x33\n\x0boracle_data\x18\x7f \x01(\x0b\x32\x10.vega.OracleDataH\x00R\noracleData\x12X\n\x12\x64\x65legation_balance\x18\x81\x01 \x01(\x0b\x32&.vega.events.v1.DelegationBalanceEventH\x00R\x11\x64\x65legationBalance\x12O\n\x0fvalidator_score\x18\x82\x01 \x01(\x0b\x32#.vega.events.v1.ValidatorScoreEventH\x00R\x0evalidatorScore\x12>\n\x0b\x65poch_event\x18\x83\x01 \x01(\x0b\x32\x1a.vega.events.v1.EpochEventH\x00R\nepochEvent\x12M\n\x10validator_update\x18\x84\x01 \x01(\x0b\x32\x1f.vega.events.v1.ValidatorUpdateH\x00R\x0fvalidatorUpdate\x12\x44\n\rstake_linking\x18\x85\x01 \x01(\x0b\x32\x1c.vega.events.v1.StakeLinkingH\x00R\x0cstakeLinking\x12I\n\rreward_payout\x18\x86\x01 \x01(\x0b\x32!.vega.events.v1.RewardPayoutEventH\x00R\x0crewardPayout\x12\x42\n\ncheckpoint\x18\x87\x01 \x01(\x0b\x32\x1f.vega.events.v1.CheckpointEventH\x00R\ncheckpoint\x12\x41\n\x0ckey_rotation\x18\x88\x01 \x01(\x0b\x32\x1b.vega.events.v1.KeyRotationH\x00R\x0bkeyRotation\x12\x38\n\tstate_var\x18\x89\x01 \x01(\x0b\x32\x18.vega.events.v1.StateVarH\x00R\x08stateVar\x12=\n\x0enetwork_limits\x18\x8a\x01 \x01(\x0b\x32\x13.vega.NetworkLimitsH\x00R\rnetworkLimits\x12\x37\n\x08transfer\x18\x8b\x01 \x01(\x0b\x32\x18.vega.events.v1.TransferH\x00R\x08transfer\x12M\n\rranking_event\x18\x8c\x01 \x01(\x0b\x32%.vega.events.v1.ValidatorRankingEventH\x00R\x0crankingEvent\x12j\n\x1b\x65rc20_multisig_signer_event\x18\x8d\x01 \x01(\x0b\x32(.vega.events.v1.ERC20MultiSigSignerEventH\x00R\x18\x65rc20MultisigSignerEvent\x12}\n"erc20_multisig_set_threshold_event\x18\x8e\x01 \x01(\x0b\x32..vega.events.v1.ERC20MultiSigThresholdSetEventH\x00R\x1e\x65rc20MultisigSetThresholdEvent\x12j\n\x1b\x65rc20_multisig_signer_added\x18\x8f\x01 \x01(\x0b\x32(.vega.events.v1.ERC20MultiSigSignerAddedH\x00R\x18\x65rc20MultisigSignerAdded\x12p\n\x1d\x65rc20_multisig_signer_removed\x18\x90\x01 \x01(\x0b\x32*.vega.events.v1.ERC20MultiSigSignerRemovedH\x00R\x1a\x65rc20MultisigSignerRemoved\x12W\n\x14position_state_event\x18\x91\x01 \x01(\x0b\x32".vega.events.v1.PositionStateEventH\x00R\x12positionStateEvent\x12Z\n\x15\x65thereum_key_rotation\x18\x92\x01 \x01(\x0b\x32#.vega.events.v1.EthereumKeyRotationH\x00R\x13\x65thereumKeyRotation\x12]\n\x16protocol_upgrade_event\x18\x93\x01 \x01(\x0b\x32$.vega.events.v1.ProtocolUpgradeEventH\x00R\x14protocolUpgradeEvent\x12>\n\x0b\x62\x65gin_block\x18\x94\x01 \x01(\x0b\x32\x1a.vega.events.v1.BeginBlockH\x00R\nbeginBlock\x12\x38\n\tend_block\x18\x95\x01 \x01(\x0b\x32\x18.vega.events.v1.EndBlockH\x00R\x08\x65ndBlock\x12\x63\n\x18protocol_upgrade_started\x18\x96\x01 \x01(\x0b\x32&.vega.events.v1.ProtocolUpgradeStartedH\x00R\x16protocolUpgradeStarted\x12\x44\n\rsettle_market\x18\x97\x01 \x01(\x0b\x32\x1c.vega.events.v1.SettleMarketH\x00R\x0csettleMarket\x12S\n\x12transaction_result\x18\x98\x01 \x01(\x0b\x32!.vega.events.v1.TransactionResultH\x00R\x11transactionResult\x12S\n\x13\x63ore_snapshot_event\x18\x99\x01 \x01(\x0b\x32 .vega.events.v1.CoreSnapshotDataH\x00R\x11\x63oreSnapshotEvent\x12w\n protocol_upgrade_data_node_ready\x18\x9a\x01 \x01(\x0b\x32,.vega.events.v1.ProtocolUpgradeDataNodeReadyH\x00R\x1cprotocolUpgradeDataNodeReady\x12P\n\x11\x64istressed_orders\x18\x9b\x01 \x01(\x0b\x32 .vega.events.v1.DistressedOrdersH\x00R\x10\x64istressedOrders\x12G\n\x0e\x65xpired_orders\x18\x9c\x01 \x01(\x0b\x32\x1d.vega.events.v1.ExpiredOrdersH\x00R\rexpiredOrders\x12Y\n\x14\x64istressed_positions\x18\x9d\x01 \x01(\x0b\x32#.vega.events.v1.DistressedPositionsH\x00R\x13\x64istressedPositions\x12\x31\n\nstop_order\x18\x9e\x01 \x01(\x0b\x32\x0f.vega.StopOrderH\x00R\tstopOrder\x12\x36\n\x06market\x18\xe9\x07 \x01(\x0b\x32\x1b.vega.events.v1.MarketEventH\x00R\x06market\x12\x41\n\x0ctx_err_event\x18\xd1\x0f \x01(\x0b\x32\x1c.vega.events.v1.TxErrorEventH\x00R\ntxErrEvent\x12\x18\n\x07version\x18\x04 \x01(\rR\x07version\x12\x19\n\x08\x63hain_id\x18\x05 \x01(\tR\x07\x63hainId\x12\x17\n\x07tx_hash\x18\x06 \x01(\tR\x06txHashB\x07\n\x05\x65vent"I\n\rExpiredOrders\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x1b\n\torder_ids\x18\x02 \x03(\tR\x08orderIds*\xdd\x01\n\x1dProtocolUpgradeProposalStatus\x12\x30\n,PROTOCOL_UPGRADE_PROPOSAL_STATUS_UNSPECIFIED\x10\x00\x12,\n(PROTOCOL_UPGRADE_PROPOSAL_STATUS_PENDING\x10\x01\x12-\n)PROTOCOL_UPGRADE_PROPOSAL_STATUS_APPROVED\x10\x02\x12-\n)PROTOCOL_UPGRADE_PROPOSAL_STATUS_REJECTED\x10\x03*\xba\x11\n\x0c\x42usEventType\x12\x1e\n\x1a\x42US_EVENT_TYPE_UNSPECIFIED\x10\x00\x12\x16\n\x12\x42US_EVENT_TYPE_ALL\x10\x01\x12\x1e\n\x1a\x42US_EVENT_TYPE_TIME_UPDATE\x10\x02\x12#\n\x1f\x42US_EVENT_TYPE_LEDGER_MOVEMENTS\x10\x03\x12&\n"BUS_EVENT_TYPE_POSITION_RESOLUTION\x10\x04\x12\x18\n\x14\x42US_EVENT_TYPE_ORDER\x10\x05\x12\x1a\n\x16\x42US_EVENT_TYPE_ACCOUNT\x10\x06\x12\x18\n\x14\x42US_EVENT_TYPE_PARTY\x10\x07\x12\x18\n\x14\x42US_EVENT_TYPE_TRADE\x10\x08\x12 \n\x1c\x42US_EVENT_TYPE_MARGIN_LEVELS\x10\t\x12\x1b\n\x17\x42US_EVENT_TYPE_PROPOSAL\x10\n\x12\x17\n\x13\x42US_EVENT_TYPE_VOTE\x10\x0b\x12\x1e\n\x1a\x42US_EVENT_TYPE_MARKET_DATA\x10\x0c\x12!\n\x1d\x42US_EVENT_TYPE_NODE_SIGNATURE\x10\r\x12%\n!BUS_EVENT_TYPE_LOSS_SOCIALIZATION\x10\x0e\x12"\n\x1e\x42US_EVENT_TYPE_SETTLE_POSITION\x10\x0f\x12$\n BUS_EVENT_TYPE_SETTLE_DISTRESSED\x10\x10\x12!\n\x1d\x42US_EVENT_TYPE_MARKET_CREATED\x10\x11\x12\x18\n\x14\x42US_EVENT_TYPE_ASSET\x10\x12\x12\x1e\n\x1a\x42US_EVENT_TYPE_MARKET_TICK\x10\x13\x12\x1d\n\x19\x42US_EVENT_TYPE_WITHDRAWAL\x10\x14\x12\x1a\n\x16\x42US_EVENT_TYPE_DEPOSIT\x10\x15\x12\x1a\n\x16\x42US_EVENT_TYPE_AUCTION\x10\x16\x12\x1e\n\x1a\x42US_EVENT_TYPE_RISK_FACTOR\x10\x17\x12$\n BUS_EVENT_TYPE_NETWORK_PARAMETER\x10\x18\x12&\n"BUS_EVENT_TYPE_LIQUIDITY_PROVISION\x10\x19\x12!\n\x1d\x42US_EVENT_TYPE_MARKET_UPDATED\x10\x1a\x12\x1e\n\x1a\x42US_EVENT_TYPE_ORACLE_SPEC\x10\x1b\x12\x1e\n\x1a\x42US_EVENT_TYPE_ORACLE_DATA\x10\x1c\x12%\n!BUS_EVENT_TYPE_DELEGATION_BALANCE\x10\x1d\x12"\n\x1e\x42US_EVENT_TYPE_VALIDATOR_SCORE\x10\x1e\x12\x1f\n\x1b\x42US_EVENT_TYPE_EPOCH_UPDATE\x10\x1f\x12#\n\x1f\x42US_EVENT_TYPE_VALIDATOR_UPDATE\x10 \x12 \n\x1c\x42US_EVENT_TYPE_STAKE_LINKING\x10!\x12&\n"BUS_EVENT_TYPE_REWARD_PAYOUT_EVENT\x10"\x12\x1d\n\x19\x42US_EVENT_TYPE_CHECKPOINT\x10#\x12\x1f\n\x1b\x42US_EVENT_TYPE_STREAM_START\x10$\x12\x1f\n\x1b\x42US_EVENT_TYPE_KEY_ROTATION\x10%\x12\x1c\n\x18\x42US_EVENT_TYPE_STATE_VAR\x10&\x12!\n\x1d\x42US_EVENT_TYPE_NETWORK_LIMITS\x10\'\x12\x1b\n\x17\x42US_EVENT_TYPE_TRANSFER\x10(\x12$\n BUS_EVENT_TYPE_VALIDATOR_RANKING\x10)\x12/\n+BUS_EVENT_TYPE_ERC20_MULTI_SIG_SIGNER_EVENT\x10*\x12\x30\n,BUS_EVENT_TYPE_ERC20_MULTI_SIG_SET_THRESHOLD\x10+\x12/\n+BUS_EVENT_TYPE_ERC20_MULTI_SIG_SIGNER_ADDED\x10,\x12\x31\n-BUS_EVENT_TYPE_ERC20_MULTI_SIG_SIGNER_REMOVED\x10-\x12!\n\x1d\x42US_EVENT_TYPE_POSITION_STATE\x10.\x12(\n$BUS_EVENT_TYPE_ETHEREUM_KEY_ROTATION\x10/\x12,\n(BUS_EVENT_TYPE_PROTOCOL_UPGRADE_PROPOSAL\x10\x30\x12\x1e\n\x1a\x42US_EVENT_TYPE_BEGIN_BLOCK\x10\x31\x12\x1c\n\x18\x42US_EVENT_TYPE_END_BLOCK\x10\x32\x12+\n\'BUS_EVENT_TYPE_PROTOCOL_UPGRADE_STARTED\x10\x33\x12 \n\x1c\x42US_EVENT_TYPE_SETTLE_MARKET\x10\x34\x12%\n!BUS_EVENT_TYPE_TRANSACTION_RESULT\x10\x35\x12!\n\x1d\x42US_EVENT_TYPE_SNAPSHOT_TAKEN\x10\x36\x12\x33\n/BUS_EVENT_TYPE_PROTOCOL_UPGRADE_DATA_NODE_READY\x10\x37\x12+\n\'BUS_EVENT_TYPE_DISTRESSED_ORDERS_CLOSED\x10\x38\x12!\n\x1d\x42US_EVENT_TYPE_EXPIRED_ORDERS\x10\x39\x12\'\n#BUS_EVENT_TYPE_DISTRESSED_POSITIONS\x10:\x12+\n\'BUS_EVENT_TYPE_SPOT_LIQUIDITY_PROVISION\x10;\x12\x1d\n\x19\x42US_EVENT_TYPE_STOP_ORDER\x10<\x12\x19\n\x15\x42US_EVENT_TYPE_MARKET\x10\x65\x12\x1c\n\x17\x42US_EVENT_TYPE_TX_ERROR\x10\xc9\x01\x42\x31Z/code.vegaprotocol.io/vega/protos/vega/events/v1b\x06proto3'
 )
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(
-    DESCRIPTOR, "vega.events.v1.events_pb2", globals()
+    DESCRIPTOR, "vega.events.v1.events_pb2", _globals
 )
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = (
         b"Z/code.vegaprotocol.io/vega/protos/vega/events/v1"
     )
-    _PROTOCOLUPGRADEPROPOSALSTATUS._serialized_start = 15717
-    _PROTOCOLUPGRADEPROPOSALSTATUS._serialized_end = 15938
-    _BUSEVENTTYPE._serialized_start = 15941
-    _BUSEVENTTYPE._serialized_end = 18099
-    _ERC20MULTISIGSIGNERADDED._serialized_start = 251
-    _ERC20MULTISIGSIGNERADDED._serialized_end = 489
-    _ERC20MULTISIGSIGNERREMOVEDSUBMITTER._serialized_start = 491
-    _ERC20MULTISIGSIGNERREMOVEDSUBMITTER._serialized_end = 593
-    _ERC20MULTISIGSIGNERREMOVED._serialized_start = 596
-    _ERC20MULTISIGSIGNERREMOVED._serialized_end = 875
-    _TRANSFER._serialized_start = 878
-    _TRANSFER._serialized_end = 1534
-    _TRANSFER_STATUS._serialized_start = 1383
-    _TRANSFER_STATUS._serialized_end = 1515
-    _ONEOFFTRANSFER._serialized_start = 1536
-    _ONEOFFTRANSFER._serialized_end = 1583
-    _RECURRINGTRANSFER._serialized_start = 1586
-    _RECURRINGTRANSFER._serialized_end = 1779
-    _STAKELINKING._serialized_start = 1782
-    _STAKELINKING._serialized_end = 2346
-    _STAKELINKING_TYPE._serialized_start = 2190
-    _STAKELINKING_TYPE._serialized_end = 2250
-    _STAKELINKING_STATUS._serialized_start = 2252
-    _STAKELINKING_STATUS._serialized_end = 2346
-    _ERC20MULTISIGSIGNEREVENT._serialized_start = 2349
-    _ERC20MULTISIGSIGNEREVENT._serialized_end = 2688
-    _ERC20MULTISIGSIGNEREVENT_TYPE._serialized_start = 2626
-    _ERC20MULTISIGSIGNEREVENT_TYPE._serialized_end = 2688
-    _ERC20MULTISIGTHRESHOLDSETEVENT._serialized_start = 2691
-    _ERC20MULTISIGTHRESHOLDSETEVENT._serialized_end = 2918
-    _CHECKPOINTEVENT._serialized_start = 2920
-    _CHECKPOINTEVENT._serialized_end = 3023
-    _STREAMSTARTEVENT._serialized_start = 3025
-    _STREAMSTARTEVENT._serialized_end = 3070
-    _REWARDPAYOUTEVENT._serialized_start = 3073
-    _REWARDPAYOUTEVENT._serialized_end = 3331
-    _VALIDATORSCOREEVENT._serialized_start = 3334
-    _VALIDATORSCOREEVENT._serialized_end = 3676
-    _DELEGATIONBALANCEEVENT._serialized_start = 3678
-    _DELEGATIONBALANCEEVENT._serialized_end = 3802
-    _MARKETEVENT._serialized_start = 3804
-    _MARKETEVENT._serialized_end = 3872
-    _TRANSACTIONRESULT._serialized_start = 3875
-    _TRANSACTIONRESULT._serialized_end = 6032
-    _TRANSACTIONRESULT_SUCCESSDETAILS._serialized_start = 5952
-    _TRANSACTIONRESULT_SUCCESSDETAILS._serialized_end = 5968
-    _TRANSACTIONRESULT_FAILUREDETAILS._serialized_start = 5970
-    _TRANSACTIONRESULT_FAILUREDETAILS._serialized_end = 6008
-    _TXERROREVENT._serialized_start = 6035
-    _TXERROREVENT._serialized_end = 7738
-    _TIMEUPDATE._serialized_start = 7740
-    _TIMEUPDATE._serialized_end = 7782
-    _EPOCHEVENT._serialized_start = 7785
-    _EPOCHEVENT._serialized_end = 7949
-    _LEDGERMOVEMENTS._serialized_start = 7951
-    _LEDGERMOVEMENTS._serialized_end = 8033
-    _POSITIONRESOLUTION._serialized_start = 8036
-    _POSITIONRESOLUTION._serialized_end = 8172
-    _LOSSSOCIALIZATION._serialized_start = 8174
-    _LOSSSOCIALIZATION._serialized_end = 8273
-    _TRADESETTLEMENT._serialized_start = 8275
-    _TRADESETTLEMENT._serialized_end = 8369
-    _SETTLEPOSITION._serialized_start = 8372
-    _SETTLEPOSITION._serialized_end = 8585
-    _SETTLEMARKET._serialized_start = 8587
-    _SETTLEMARKET._serialized_end = 8693
-    _POSITIONSTATEEVENT._serialized_start = 8696
-    _POSITIONSTATEEVENT._serialized_end = 8942
-    _SETTLEDISTRESSED._serialized_start = 8944
-    _SETTLEDISTRESSED._serialized_end = 9064
-    _DISTRESSEDORDERS._serialized_start = 9066
-    _DISTRESSEDORDERS._serialized_end = 9139
-    _DISTRESSEDPOSITIONS._serialized_start = 9142
-    _DISTRESSEDPOSITIONS._serialized_end = 9274
-    _MARKETTICK._serialized_start = 9276
-    _MARKETTICK._serialized_end = 9324
-    _AUCTIONEVENT._serialized_start = 9327
-    _AUCTIONEVENT._serialized_end = 9588
-    _VALIDATORUPDATE._serialized_start = 9591
-    _VALIDATORUPDATE._serialized_end = 10016
-    _VALIDATORRANKINGEVENT._serialized_start = 10019
-    _VALIDATORRANKINGEVENT._serialized_end = 10325
-    _KEYROTATION._serialized_start = 10328
-    _KEYROTATION._serialized_end = 10465
-    _ETHEREUMKEYROTATION._serialized_start = 10468
-    _ETHEREUMKEYROTATION._serialized_end = 10615
-    _PROTOCOLUPGRADEEVENT._serialized_start = 10618
-    _PROTOCOLUPGRADEEVENT._serialized_end = 10833
-    _STATEVAR._serialized_start = 10835
-    _STATEVAR._serialized_end = 10910
-    _BEGINBLOCK._serialized_start = 10912
-    _BEGINBLOCK._serialized_end = 10998
-    _ENDBLOCK._serialized_start = 11000
-    _ENDBLOCK._serialized_end = 11034
-    _PROTOCOLUPGRADESTARTED._serialized_start = 11036
-    _PROTOCOLUPGRADESTARTED._serialized_end = 11104
-    _PROTOCOLUPGRADEDATANODEREADY._serialized_start = 11106
-    _PROTOCOLUPGRADEDATANODEREADY._serialized_end = 11180
-    _CORESNAPSHOTDATA._serialized_start = 11183
-    _CORESNAPSHOTDATA._serialized_end = 11356
-    _BUSEVENT._serialized_start = 11359
-    _BUSEVENT._serialized_end = 15639
-    _EXPIREDORDERS._serialized_start = 15641
-    _EXPIREDORDERS._serialized_end = 15714
+    _globals["_PROTOCOLUPGRADEPROPOSALSTATUS"]._serialized_start = 16455
+    _globals["_PROTOCOLUPGRADEPROPOSALSTATUS"]._serialized_end = 16676
+    _globals["_BUSEVENTTYPE"]._serialized_start = 16679
+    _globals["_BUSEVENTTYPE"]._serialized_end = 18913
+    _globals["_STOPORDEREVENT"]._serialized_start = 251
+    _globals["_STOPORDEREVENT"]._serialized_end = 382
+    _globals["_ERC20MULTISIGSIGNERADDED"]._serialized_start = 385
+    _globals["_ERC20MULTISIGSIGNERADDED"]._serialized_end = 623
+    _globals["_ERC20MULTISIGSIGNERREMOVEDSUBMITTER"]._serialized_start = 625
+    _globals["_ERC20MULTISIGSIGNERREMOVEDSUBMITTER"]._serialized_end = 727
+    _globals["_ERC20MULTISIGSIGNERREMOVED"]._serialized_start = 730
+    _globals["_ERC20MULTISIGSIGNERREMOVED"]._serialized_end = 1009
+    _globals["_TRANSFER"]._serialized_start = 1012
+    _globals["_TRANSFER"]._serialized_end = 1856
+    _globals["_TRANSFER_STATUS"]._serialized_start = 1705
+    _globals["_TRANSFER_STATUS"]._serialized_end = 1837
+    _globals["_ONEOFFGOVERNANCETRANSFER"]._serialized_start = 1858
+    _globals["_ONEOFFGOVERNANCETRANSFER"]._serialized_end = 1915
+    _globals["_ONEOFFTRANSFER"]._serialized_start = 1917
+    _globals["_ONEOFFTRANSFER"]._serialized_end = 1964
+    _globals["_RECURRINGTRANSFER"]._serialized_start = 1967
+    _globals["_RECURRINGTRANSFER"]._serialized_end = 2160
+    _globals["_RECURRINGGOVERNANCETRANSFER"]._serialized_start = 2162
+    _globals["_RECURRINGGOVERNANCETRANSFER"]._serialized_end = 2272
+    _globals["_STAKELINKING"]._serialized_start = 2275
+    _globals["_STAKELINKING"]._serialized_end = 2839
+    _globals["_STAKELINKING_TYPE"]._serialized_start = 2683
+    _globals["_STAKELINKING_TYPE"]._serialized_end = 2743
+    _globals["_STAKELINKING_STATUS"]._serialized_start = 2745
+    _globals["_STAKELINKING_STATUS"]._serialized_end = 2839
+    _globals["_ERC20MULTISIGSIGNEREVENT"]._serialized_start = 2842
+    _globals["_ERC20MULTISIGSIGNEREVENT"]._serialized_end = 3181
+    _globals["_ERC20MULTISIGSIGNEREVENT_TYPE"]._serialized_start = 3119
+    _globals["_ERC20MULTISIGSIGNEREVENT_TYPE"]._serialized_end = 3181
+    _globals["_ERC20MULTISIGTHRESHOLDSETEVENT"]._serialized_start = 3184
+    _globals["_ERC20MULTISIGTHRESHOLDSETEVENT"]._serialized_end = 3411
+    _globals["_CHECKPOINTEVENT"]._serialized_start = 3413
+    _globals["_CHECKPOINTEVENT"]._serialized_end = 3516
+    _globals["_STREAMSTARTEVENT"]._serialized_start = 3518
+    _globals["_STREAMSTARTEVENT"]._serialized_end = 3563
+    _globals["_REWARDPAYOUTEVENT"]._serialized_start = 3566
+    _globals["_REWARDPAYOUTEVENT"]._serialized_end = 3824
+    _globals["_VALIDATORSCOREEVENT"]._serialized_start = 3827
+    _globals["_VALIDATORSCOREEVENT"]._serialized_end = 4169
+    _globals["_DELEGATIONBALANCEEVENT"]._serialized_start = 4171
+    _globals["_DELEGATIONBALANCEEVENT"]._serialized_end = 4295
+    _globals["_MARKETEVENT"]._serialized_start = 4297
+    _globals["_MARKETEVENT"]._serialized_end = 4365
+    _globals["_TRANSACTIONRESULT"]._serialized_start = 4368
+    _globals["_TRANSACTIONRESULT"]._serialized_end = 6719
+    _globals["_TRANSACTIONRESULT_SUCCESSDETAILS"]._serialized_start = 6639
+    _globals["_TRANSACTIONRESULT_SUCCESSDETAILS"]._serialized_end = 6655
+    _globals["_TRANSACTIONRESULT_FAILUREDETAILS"]._serialized_start = 6657
+    _globals["_TRANSACTIONRESULT_FAILUREDETAILS"]._serialized_end = 6695
+    _globals["_TXERROREVENT"]._serialized_start = 6722
+    _globals["_TXERROREVENT"]._serialized_end = 8425
+    _globals["_TIMEUPDATE"]._serialized_start = 8427
+    _globals["_TIMEUPDATE"]._serialized_end = 8469
+    _globals["_EPOCHEVENT"]._serialized_start = 8472
+    _globals["_EPOCHEVENT"]._serialized_end = 8636
+    _globals["_LEDGERMOVEMENTS"]._serialized_start = 8638
+    _globals["_LEDGERMOVEMENTS"]._serialized_end = 8720
+    _globals["_POSITIONRESOLUTION"]._serialized_start = 8723
+    _globals["_POSITIONRESOLUTION"]._serialized_end = 8859
+    _globals["_LOSSSOCIALIZATION"]._serialized_start = 8861
+    _globals["_LOSSSOCIALIZATION"]._serialized_end = 8960
+    _globals["_TRADESETTLEMENT"]._serialized_start = 8962
+    _globals["_TRADESETTLEMENT"]._serialized_end = 9056
+    _globals["_SETTLEPOSITION"]._serialized_start = 9059
+    _globals["_SETTLEPOSITION"]._serialized_end = 9272
+    _globals["_SETTLEMARKET"]._serialized_start = 9274
+    _globals["_SETTLEMARKET"]._serialized_end = 9380
+    _globals["_POSITIONSTATEEVENT"]._serialized_start = 9383
+    _globals["_POSITIONSTATEEVENT"]._serialized_end = 9629
+    _globals["_SETTLEDISTRESSED"]._serialized_start = 9631
+    _globals["_SETTLEDISTRESSED"]._serialized_end = 9751
+    _globals["_DISTRESSEDORDERS"]._serialized_start = 9753
+    _globals["_DISTRESSEDORDERS"]._serialized_end = 9826
+    _globals["_DISTRESSEDPOSITIONS"]._serialized_start = 9829
+    _globals["_DISTRESSEDPOSITIONS"]._serialized_end = 9961
+    _globals["_MARKETTICK"]._serialized_start = 9963
+    _globals["_MARKETTICK"]._serialized_end = 10011
+    _globals["_AUCTIONEVENT"]._serialized_start = 10014
+    _globals["_AUCTIONEVENT"]._serialized_end = 10275
+    _globals["_VALIDATORUPDATE"]._serialized_start = 10278
+    _globals["_VALIDATORUPDATE"]._serialized_end = 10703
+    _globals["_VALIDATORRANKINGEVENT"]._serialized_start = 10706
+    _globals["_VALIDATORRANKINGEVENT"]._serialized_end = 11012
+    _globals["_KEYROTATION"]._serialized_start = 11015
+    _globals["_KEYROTATION"]._serialized_end = 11152
+    _globals["_ETHEREUMKEYROTATION"]._serialized_start = 11155
+    _globals["_ETHEREUMKEYROTATION"]._serialized_end = 11302
+    _globals["_PROTOCOLUPGRADEEVENT"]._serialized_start = 11305
+    _globals["_PROTOCOLUPGRADEEVENT"]._serialized_end = 11520
+    _globals["_STATEVAR"]._serialized_start = 11522
+    _globals["_STATEVAR"]._serialized_end = 11597
+    _globals["_BEGINBLOCK"]._serialized_start = 11599
+    _globals["_BEGINBLOCK"]._serialized_end = 11685
+    _globals["_ENDBLOCK"]._serialized_start = 11687
+    _globals["_ENDBLOCK"]._serialized_end = 11721
+    _globals["_PROTOCOLUPGRADESTARTED"]._serialized_start = 11723
+    _globals["_PROTOCOLUPGRADESTARTED"]._serialized_end = 11791
+    _globals["_PROTOCOLUPGRADEDATANODEREADY"]._serialized_start = 11793
+    _globals["_PROTOCOLUPGRADEDATANODEREADY"]._serialized_end = 11867
+    _globals["_CORESNAPSHOTDATA"]._serialized_start = 11870
+    _globals["_CORESNAPSHOTDATA"]._serialized_end = 12043
+    _globals["_BUSEVENT"]._serialized_start = 12046
+    _globals["_BUSEVENT"]._serialized_end = 16377
+    _globals["_EXPIREDORDERS"]._serialized_start = 16379
+    _globals["_EXPIREDORDERS"]._serialized_end = 16452
 # @@protoc_insertion_point(module_scope)
```

### Comparing `vega_sim-1.1.1/vega_sim/proto/vega/governance_pb2.py` & `vega_sim-1.2.0/vega_sim/proto/vega/governance_pb2.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,78 +1,105 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: vega/governance.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from . import assets_pb2 as vega_dot_assets__pb2
 from . import data_source_pb2 as vega_dot_data__source__pb2
 from . import markets_pb2 as vega_dot_markets__pb2
 from . import vega_pb2 as vega_dot_vega__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x15vega/governance.proto\x12\x04vega\x1a\x11vega/assets.proto\x1a\x16vega/data_source.proto\x1a\x12vega/markets.proto\x1a\x0fvega/vega.proto"\x95\x03\n\rFutureProduct\x12)\n\x10settlement_asset\x18\x01 \x01(\tR\x0fsettlementAsset\x12\x1d\n\nquote_name\x18\x02 \x01(\tR\tquoteName\x12i\n$data_source_spec_for_settlement_data\x18\x03 \x01(\x0b\x32\x1a.vega.DataSourceDefinitionR\x1f\x64\x61taSourceSpecForSettlementData\x12q\n(data_source_spec_for_trading_termination\x18\x04 \x01(\x0b\x32\x1a.vega.DataSourceDefinitionR#dataSourceSpecForTradingTermination\x12\\\n\x18\x64\x61ta_source_spec_binding\x18\x05 \x01(\x0b\x32#.vega.DataSourceSpecToFutureBindingR\x15\x64\x61taSourceSpecBinding"{\n\x17InstrumentConfiguration\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x12\n\x04\x63ode\x18\x02 \x01(\tR\x04\x63ode\x12-\n\x06\x66uture\x18\x64 \x01(\x0b\x32\x13.vega.FutureProductH\x00R\x06\x66utureB\t\n\x07product"\xb9\x05\n\x16NewMarketConfiguration\x12=\n\ninstrument\x18\x01 \x01(\x0b\x32\x1d.vega.InstrumentConfigurationR\ninstrument\x12%\n\x0e\x64\x65\x63imal_places\x18\x02 \x01(\x04R\rdecimalPlaces\x12\x1a\n\x08metadata\x18\x03 \x03(\tR\x08metadata\x12_\n\x1bprice_monitoring_parameters\x18\x04 \x01(\x0b\x32\x1f.vega.PriceMonitoringParametersR\x19priceMonitoringParameters\x12k\n\x1fliquidity_monitoring_parameters\x18\x05 \x01(\x0b\x32#.vega.LiquidityMonitoringParametersR\x1dliquidityMonitoringParameters\x12\x31\n\x06simple\x18\x64 \x01(\x0b\x32\x17.vega.SimpleModelParamsH\x00R\x06simple\x12\x39\n\nlog_normal\x18\x65 \x01(\x0b\x32\x18.vega.LogNormalRiskModelH\x00R\tlogNormal\x12\x36\n\x17position_decimal_places\x18\x06 \x01(\x03R\x15positionDecimalPlaces\x12$\n\x0elp_price_range\x18\x08 \x01(\tR\x0clpPriceRange\x12\x34\n\x16linear_slippage_factor\x18\t \x01(\tR\x14linearSlippageFactor\x12:\n\x19quadratic_slippage_factor\x18\n \x01(\tR\x17quadraticSlippageFactorB\x11\n\x0frisk_parameters"C\n\tNewMarket\x12\x36\n\x07\x63hanges\x18\x01 \x01(\x0b\x32\x1c.vega.NewMarketConfigurationR\x07\x63hanges"f\n\x0cUpdateMarket\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x39\n\x07\x63hanges\x18\x02 \x01(\x0b\x32\x1f.vega.UpdateMarketConfigurationR\x07\x63hanges"\xe3\x04\n\x19UpdateMarketConfiguration\x12\x43\n\ninstrument\x18\x01 \x01(\x0b\x32#.vega.UpdateInstrumentConfigurationR\ninstrument\x12\x1a\n\x08metadata\x18\x02 \x03(\tR\x08metadata\x12_\n\x1bprice_monitoring_parameters\x18\x03 \x01(\x0b\x32\x1f.vega.PriceMonitoringParametersR\x19priceMonitoringParameters\x12k\n\x1fliquidity_monitoring_parameters\x18\x04 \x01(\x0b\x32#.vega.LiquidityMonitoringParametersR\x1dliquidityMonitoringParameters\x12\x31\n\x06simple\x18\x64 \x01(\x0b\x32\x17.vega.SimpleModelParamsH\x00R\x06simple\x12\x39\n\nlog_normal\x18\x65 \x01(\x0b\x32\x18.vega.LogNormalRiskModelH\x00R\tlogNormal\x12$\n\x0elp_price_range\x18\x05 \x01(\tR\x0clpPriceRange\x12\x34\n\x16linear_slippage_factor\x18\x06 \x01(\tR\x14linearSlippageFactor\x12:\n\x19quadratic_slippage_factor\x18\x07 \x01(\tR\x17quadraticSlippageFactorB\x11\n\x0frisk_parameters"s\n\x1dUpdateInstrumentConfiguration\x12\x12\n\x04\x63ode\x18\x01 \x01(\tR\x04\x63ode\x12\x33\n\x06\x66uture\x18\x64 \x01(\x0b\x32\x19.vega.UpdateFutureProductH\x00R\x06\x66utureB\t\n\x07product"\xf0\x02\n\x13UpdateFutureProduct\x12\x1d\n\nquote_name\x18\x01 \x01(\tR\tquoteName\x12i\n$data_source_spec_for_settlement_data\x18\x02 \x01(\x0b\x32\x1a.vega.DataSourceDefinitionR\x1f\x64\x61taSourceSpecForSettlementData\x12q\n(data_source_spec_for_trading_termination\x18\x03 \x01(\x0b\x32\x1a.vega.DataSourceDefinitionR#dataSourceSpecForTradingTermination\x12\\\n\x18\x64\x61ta_source_spec_binding\x18\x04 \x01(\x0b\x32#.vega.DataSourceSpecToFutureBindingR\x15\x64\x61taSourceSpecBinding"J\n\x16UpdateNetworkParameter\x12\x30\n\x07\x63hanges\x18\x01 \x01(\x0b\x32\x16.vega.NetworkParameterR\x07\x63hanges"8\n\x08NewAsset\x12,\n\x07\x63hanges\x18\x01 \x01(\x0b\x32\x12.vega.AssetDetailsR\x07\x63hanges"\\\n\x0bUpdateAsset\x12\x19\n\x08\x61sset_id\x18\x01 \x01(\tR\x07\x61ssetId\x12\x32\n\x07\x63hanges\x18\x02 \x01(\x0b\x32\x18.vega.AssetDetailsUpdateR\x07\x63hanges"\r\n\x0bNewFreeform"\x90\x04\n\rProposalTerms\x12+\n\x11\x63losing_timestamp\x18\x01 \x01(\x03R\x10\x63losingTimestamp\x12/\n\x13\x65nactment_timestamp\x18\x02 \x01(\x03R\x12\x65nactmentTimestamp\x12\x31\n\x14validation_timestamp\x18\x03 \x01(\x03R\x13validationTimestamp\x12\x39\n\rupdate_market\x18\x65 \x01(\x0b\x32\x12.vega.UpdateMarketH\x00R\x0cupdateMarket\x12\x30\n\nnew_market\x18\x66 \x01(\x0b\x32\x0f.vega.NewMarketH\x00R\tnewMarket\x12X\n\x18update_network_parameter\x18g \x01(\x0b\x32\x1c.vega.UpdateNetworkParameterH\x00R\x16updateNetworkParameter\x12-\n\tnew_asset\x18h \x01(\x0b\x32\x0e.vega.NewAssetH\x00R\x08newAsset\x12\x36\n\x0cnew_freeform\x18i \x01(\x0b\x32\x11.vega.NewFreeformH\x00R\x0bnewFreeform\x12\x36\n\x0cupdate_asset\x18j \x01(\x0b\x32\x11.vega.UpdateAssetH\x00R\x0bupdateAssetB\x08\n\x06\x63hange"W\n\x11ProposalRationale\x12 \n\x0b\x64\x65scription\x18\x01 \x01(\tR\x0b\x64\x65scription\x12\x14\n\x05title\x18\x04 \x01(\tR\x05titleJ\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04"\x86\x03\n\x0eGovernanceData\x12*\n\x08proposal\x18\x01 \x01(\x0b\x32\x0e.vega.ProposalR\x08proposal\x12\x1c\n\x03yes\x18\x02 \x03(\x0b\x32\n.vega.VoteR\x03yes\x12\x1a\n\x02no\x18\x03 \x03(\x0b\x32\n.vega.VoteR\x02no\x12?\n\tyes_party\x18\x04 \x03(\x0b\x32".vega.GovernanceData.YesPartyEntryR\x08yesParty\x12<\n\x08no_party\x18\x05 \x03(\x0b\x32!.vega.GovernanceData.NoPartyEntryR\x07noParty\x1aG\n\rYesPartyEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12 \n\x05value\x18\x02 \x01(\x0b\x32\n.vega.VoteR\x05value:\x02\x38\x01\x1a\x46\n\x0cNoPartyEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12 \n\x05value\x18\x02 \x01(\x0b\x32\n.vega.VoteR\x05value:\x02\x38\x01"\x9a\x07\n\x08Proposal\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1c\n\treference\x18\x02 \x01(\tR\treference\x12\x19\n\x08party_id\x18\x03 \x01(\tR\x07partyId\x12*\n\x05state\x18\x04 \x01(\x0e\x32\x14.vega.Proposal.StateR\x05state\x12\x1c\n\ttimestamp\x18\x05 \x01(\x03R\ttimestamp\x12)\n\x05terms\x18\x06 \x01(\x0b\x32\x13.vega.ProposalTermsR\x05terms\x12\x30\n\x06reason\x18\x07 \x01(\x0e\x32\x13.vega.ProposalErrorH\x00R\x06reason\x88\x01\x01\x12(\n\rerror_details\x18\x08 \x01(\tH\x01R\x0c\x65rrorDetails\x88\x01\x01\x12\x35\n\trationale\x18\t \x01(\x0b\x32\x17.vega.ProposalRationaleR\trationale\x12\x35\n\x16required_participation\x18\n \x01(\tR\x15requiredParticipation\x12+\n\x11required_majority\x18\x0b \x01(\tR\x10requiredMajority\x12^\n)required_liquidity_provider_participation\x18\x0c \x01(\tH\x02R&requiredLiquidityProviderParticipation\x88\x01\x01\x12T\n$required_liquidity_provider_majority\x18\r \x01(\tH\x03R!requiredLiquidityProviderMajority\x88\x01\x01"\xae\x01\n\x05State\x12\x15\n\x11STATE_UNSPECIFIED\x10\x00\x12\x10\n\x0cSTATE_FAILED\x10\x01\x12\x0e\n\nSTATE_OPEN\x10\x02\x12\x10\n\x0cSTATE_PASSED\x10\x03\x12\x12\n\x0eSTATE_REJECTED\x10\x04\x12\x12\n\x0eSTATE_DECLINED\x10\x05\x12\x11\n\rSTATE_ENACTED\x10\x06\x12\x1f\n\x1bSTATE_WAITING_FOR_NODE_VOTE\x10\x07\x42\t\n\x07_reasonB\x10\n\x0e_error_detailsB,\n*_required_liquidity_provider_participationB\'\n%_required_liquidity_provider_majority"\x91\x03\n\x04Vote\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12&\n\x05value\x18\x02 \x01(\x0e\x32\x10.vega.Vote.ValueR\x05value\x12\x1f\n\x0bproposal_id\x18\x03 \x01(\tR\nproposalId\x12\x1c\n\ttimestamp\x18\x04 \x01(\x03R\ttimestamp\x12\x43\n\x1etotal_governance_token_balance\x18\x05 \x01(\tR\x1btotalGovernanceTokenBalance\x12\x41\n\x1dtotal_governance_token_weight\x18\x06 \x01(\tR\x1atotalGovernanceTokenWeight\x12\x42\n\x1etotal_equity_like_share_weight\x18\x07 \x01(\tR\x1atotalEquityLikeShareWeight";\n\x05Value\x12\x15\n\x11VALUE_UNSPECIFIED\x10\x00\x12\x0c\n\x08VALUE_NO\x10\x01\x12\r\n\tVALUE_YES\x10\x02*\xa0\x0e\n\rProposalError\x12\x1e\n\x1aPROPOSAL_ERROR_UNSPECIFIED\x10\x00\x12&\n"PROPOSAL_ERROR_CLOSE_TIME_TOO_SOON\x10\x01\x12&\n"PROPOSAL_ERROR_CLOSE_TIME_TOO_LATE\x10\x02\x12&\n"PROPOSAL_ERROR_ENACT_TIME_TOO_SOON\x10\x03\x12&\n"PROPOSAL_ERROR_ENACT_TIME_TOO_LATE\x10\x04\x12&\n"PROPOSAL_ERROR_INSUFFICIENT_TOKENS\x10\x05\x12.\n*PROPOSAL_ERROR_INVALID_INSTRUMENT_SECURITY\x10\x06\x12\x1d\n\x19PROPOSAL_ERROR_NO_PRODUCT\x10\x07\x12&\n"PROPOSAL_ERROR_UNSUPPORTED_PRODUCT\x10\x08\x12"\n\x1ePROPOSAL_ERROR_NO_TRADING_MODE\x10\x0b\x12+\n\'PROPOSAL_ERROR_UNSUPPORTED_TRADING_MODE\x10\x0c\x12)\n%PROPOSAL_ERROR_NODE_VALIDATION_FAILED\x10\r\x12.\n*PROPOSAL_ERROR_MISSING_BUILTIN_ASSET_FIELD\x10\x0e\x12\x31\n-PROPOSAL_ERROR_MISSING_ERC20_CONTRACT_ADDRESS\x10\x0f\x12 \n\x1cPROPOSAL_ERROR_INVALID_ASSET\x10\x10\x12*\n&PROPOSAL_ERROR_INCOMPATIBLE_TIMESTAMPS\x10\x11\x12%\n!PROPOSAL_ERROR_NO_RISK_PARAMETERS\x10\x12\x12\x30\n,PROPOSAL_ERROR_NETWORK_PARAMETER_INVALID_KEY\x10\x13\x12\x32\n.PROPOSAL_ERROR_NETWORK_PARAMETER_INVALID_VALUE\x10\x14\x12\x36\n2PROPOSAL_ERROR_NETWORK_PARAMETER_VALIDATION_FAILED\x10\x15\x12\x35\n1PROPOSAL_ERROR_OPENING_AUCTION_DURATION_TOO_SMALL\x10\x16\x12\x35\n1PROPOSAL_ERROR_OPENING_AUCTION_DURATION_TOO_LARGE\x10\x17\x12/\n+PROPOSAL_ERROR_COULD_NOT_INSTANTIATE_MARKET\x10\x19\x12)\n%PROPOSAL_ERROR_INVALID_FUTURE_PRODUCT\x10\x1a\x12)\n%PROPOSAL_ERROR_INVALID_RISK_PARAMETER\x10\x1e\x12\x31\n-PROPOSAL_ERROR_MAJORITY_THRESHOLD_NOT_REACHED\x10\x1f\x12\x36\n2PROPOSAL_ERROR_PARTICIPATION_THRESHOLD_NOT_REACHED\x10 \x12(\n$PROPOSAL_ERROR_INVALID_ASSET_DETAILS\x10!\x12\x1f\n\x1bPROPOSAL_ERROR_UNKNOWN_TYPE\x10"\x12.\n*PROPOSAL_ERROR_UNKNOWN_RISK_PARAMETER_TYPE\x10#\x12#\n\x1fPROPOSAL_ERROR_INVALID_FREEFORM\x10$\x12\x31\n-PROPOSAL_ERROR_INSUFFICIENT_EQUITY_LIKE_SHARE\x10%\x12!\n\x1dPROPOSAL_ERROR_INVALID_MARKET\x10&\x12\x31\n-PROPOSAL_ERROR_TOO_MANY_MARKET_DECIMAL_PLACES\x10\'\x12\x35\n1PROPOSAL_ERROR_TOO_MANY_PRICE_MONITORING_TRIGGERS\x10(\x12/\n+PROPOSAL_ERROR_ERC20_ADDRESS_ALREADY_IN_USE\x10)\x12-\n)PROPOSAL_ERROR_LP_PRICE_RANGE_NONPOSITIVE\x10*\x12+\n\'PROPOSAL_ERROR_LP_PRICE_RANGE_TOO_LARGE\x10+\x12\x36\n2PROPOSAL_ERROR_LINEAR_SLIPPAGE_FACTOR_OUT_OF_RANGE\x10,\x12\x39\n5PROPOSAL_ERROR_QUADRATIC_SLIPPAGE_FACTOR_OUT_OF_RANGE\x10-B\'Z%code.vegaprotocol.io/vega/protos/vegab\x06proto3'
+    b'\n\x15vega/governance.proto\x12\x04vega\x1a\x11vega/assets.proto\x1a\x16vega/data_source.proto\x1a\x12vega/markets.proto\x1a\x0fvega/vega.proto"a\n\x0bSpotProduct\x12\x1d\n\nbase_asset\x18\x01 \x01(\tR\tbaseAsset\x12\x1f\n\x0bquote_asset\x18\x02 \x01(\tR\nquoteAsset\x12\x12\n\x04name\x18\x03 \x01(\tR\x04name"\x95\x03\n\rFutureProduct\x12)\n\x10settlement_asset\x18\x01 \x01(\tR\x0fsettlementAsset\x12\x1d\n\nquote_name\x18\x02 \x01(\tR\tquoteName\x12i\n$data_source_spec_for_settlement_data\x18\x03 \x01(\x0b\x32\x1a.vega.DataSourceDefinitionR\x1f\x64\x61taSourceSpecForSettlementData\x12q\n(data_source_spec_for_trading_termination\x18\x04 \x01(\x0b\x32\x1a.vega.DataSourceDefinitionR#dataSourceSpecForTradingTermination\x12\\\n\x18\x64\x61ta_source_spec_binding\x18\x05 \x01(\x0b\x32#.vega.DataSourceSpecToFutureBindingR\x15\x64\x61taSourceSpecBinding"\xa4\x01\n\x17InstrumentConfiguration\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x12\n\x04\x63ode\x18\x02 \x01(\tR\x04\x63ode\x12-\n\x06\x66uture\x18\x64 \x01(\x0b\x32\x13.vega.FutureProductH\x00R\x06\x66uture\x12\'\n\x04spot\x18\x65 \x01(\x0b\x32\x11.vega.SpotProductH\x00R\x04spotB\t\n\x07product"\x8d\x04\n\x1aNewSpotMarketConfiguration\x12=\n\ninstrument\x18\x01 \x01(\x0b\x32\x1d.vega.InstrumentConfigurationR\ninstrument\x12%\n\x0e\x64\x65\x63imal_places\x18\x02 \x01(\x04R\rdecimalPlaces\x12\x1a\n\x08metadata\x18\x03 \x03(\tR\x08metadata\x12_\n\x1bprice_monitoring_parameters\x18\x04 \x01(\x0b\x32\x1f.vega.PriceMonitoringParametersR\x19priceMonitoringParameters\x12S\n\x17target_stake_parameters\x18\x05 \x01(\x0b\x32\x1b.vega.TargetStakeParametersR\x15targetStakeParameters\x12\x31\n\x06simple\x18\x64 \x01(\x0b\x32\x17.vega.SimpleModelParamsH\x00R\x06simple\x12\x39\n\nlog_normal\x18\x65 \x01(\x0b\x32\x18.vega.LogNormalRiskModelH\x00R\tlogNormal\x12\x36\n\x17position_decimal_places\x18\x06 \x01(\x03R\x15positionDecimalPlacesB\x11\n\x0frisk_parameters"\x88\x06\n\x16NewMarketConfiguration\x12=\n\ninstrument\x18\x01 \x01(\x0b\x32\x1d.vega.InstrumentConfigurationR\ninstrument\x12%\n\x0e\x64\x65\x63imal_places\x18\x02 \x01(\x04R\rdecimalPlaces\x12\x1a\n\x08metadata\x18\x03 \x03(\tR\x08metadata\x12_\n\x1bprice_monitoring_parameters\x18\x04 \x01(\x0b\x32\x1f.vega.PriceMonitoringParametersR\x19priceMonitoringParameters\x12k\n\x1fliquidity_monitoring_parameters\x18\x05 \x01(\x0b\x32#.vega.LiquidityMonitoringParametersR\x1dliquidityMonitoringParameters\x12\x31\n\x06simple\x18\x64 \x01(\x0b\x32\x17.vega.SimpleModelParamsH\x00R\x06simple\x12\x39\n\nlog_normal\x18\x65 \x01(\x0b\x32\x18.vega.LogNormalRiskModelH\x00R\tlogNormal\x12\x36\n\x17position_decimal_places\x18\x06 \x01(\x03R\x15positionDecimalPlaces\x12$\n\x0elp_price_range\x18\x08 \x01(\tR\x0clpPriceRange\x12\x34\n\x16linear_slippage_factor\x18\t \x01(\tR\x14linearSlippageFactor\x12:\n\x19quadratic_slippage_factor\x18\n \x01(\tR\x17quadraticSlippageFactor\x12?\n\tsuccessor\x18\x0b \x01(\x0b\x32\x1c.vega.SuccessorConfigurationH\x01R\tsuccessor\x88\x01\x01\x42\x11\n\x0frisk_parametersB\x0c\n\n_successor"K\n\rNewSpotMarket\x12:\n\x07\x63hanges\x18\x01 \x01(\x0b\x32 .vega.NewSpotMarketConfigurationR\x07\x63hanges"z\n\x16SuccessorConfiguration\x12(\n\x10parent_market_id\x18\x01 \x01(\tR\x0eparentMarketId\x12\x36\n\x17insurance_pool_fraction\x18\x02 \x01(\tR\x15insurancePoolFraction"C\n\tNewMarket\x12\x36\n\x07\x63hanges\x18\x01 \x01(\x0b\x32\x1c.vega.NewMarketConfigurationR\x07\x63hanges"f\n\x0cUpdateMarket\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x39\n\x07\x63hanges\x18\x02 \x01(\x0b\x32\x1f.vega.UpdateMarketConfigurationR\x07\x63hanges"n\n\x10UpdateSpotMarket\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12=\n\x07\x63hanges\x18\x02 \x01(\x0b\x32#.vega.UpdateSpotMarketConfigurationR\x07\x63hanges"\xe3\x04\n\x19UpdateMarketConfiguration\x12\x43\n\ninstrument\x18\x01 \x01(\x0b\x32#.vega.UpdateInstrumentConfigurationR\ninstrument\x12\x1a\n\x08metadata\x18\x02 \x03(\tR\x08metadata\x12_\n\x1bprice_monitoring_parameters\x18\x03 \x01(\x0b\x32\x1f.vega.PriceMonitoringParametersR\x19priceMonitoringParameters\x12k\n\x1fliquidity_monitoring_parameters\x18\x04 \x01(\x0b\x32#.vega.LiquidityMonitoringParametersR\x1dliquidityMonitoringParameters\x12\x31\n\x06simple\x18\x64 \x01(\x0b\x32\x17.vega.SimpleModelParamsH\x00R\x06simple\x12\x39\n\nlog_normal\x18\x65 \x01(\x0b\x32\x18.vega.LogNormalRiskModelH\x00R\tlogNormal\x12$\n\x0elp_price_range\x18\x05 \x01(\tR\x0clpPriceRange\x12\x34\n\x16linear_slippage_factor\x18\x06 \x01(\tR\x14linearSlippageFactor\x12:\n\x19quadratic_slippage_factor\x18\x07 \x01(\tR\x17quadraticSlippageFactorB\x11\n\x0frisk_parameters"\xf2\x02\n\x1dUpdateSpotMarketConfiguration\x12\x1a\n\x08metadata\x18\x01 \x03(\tR\x08metadata\x12_\n\x1bprice_monitoring_parameters\x18\x02 \x01(\x0b\x32\x1f.vega.PriceMonitoringParametersR\x19priceMonitoringParameters\x12S\n\x17target_stake_parameters\x18\x03 \x01(\x0b\x32\x1b.vega.TargetStakeParametersR\x15targetStakeParameters\x12\x31\n\x06simple\x18\x64 \x01(\x0b\x32\x17.vega.SimpleModelParamsH\x00R\x06simple\x12\x39\n\nlog_normal\x18\x65 \x01(\x0b\x32\x18.vega.LogNormalRiskModelH\x00R\tlogNormalB\x11\n\x0frisk_parameters"s\n\x1dUpdateInstrumentConfiguration\x12\x12\n\x04\x63ode\x18\x01 \x01(\tR\x04\x63ode\x12\x33\n\x06\x66uture\x18\x64 \x01(\x0b\x32\x19.vega.UpdateFutureProductH\x00R\x06\x66utureB\t\n\x07product"\xf0\x02\n\x13UpdateFutureProduct\x12\x1d\n\nquote_name\x18\x01 \x01(\tR\tquoteName\x12i\n$data_source_spec_for_settlement_data\x18\x02 \x01(\x0b\x32\x1a.vega.DataSourceDefinitionR\x1f\x64\x61taSourceSpecForSettlementData\x12q\n(data_source_spec_for_trading_termination\x18\x03 \x01(\x0b\x32\x1a.vega.DataSourceDefinitionR#dataSourceSpecForTradingTermination\x12\\\n\x18\x64\x61ta_source_spec_binding\x18\x04 \x01(\x0b\x32#.vega.DataSourceSpecToFutureBindingR\x15\x64\x61taSourceSpecBinding"J\n\x16UpdateNetworkParameter\x12\x30\n\x07\x63hanges\x18\x01 \x01(\x0b\x32\x16.vega.NetworkParameterR\x07\x63hanges"8\n\x08NewAsset\x12,\n\x07\x63hanges\x18\x01 \x01(\x0b\x32\x12.vega.AssetDetailsR\x07\x63hanges"\\\n\x0bUpdateAsset\x12\x19\n\x08\x61sset_id\x18\x01 \x01(\tR\x07\x61ssetId\x12\x32\n\x07\x63hanges\x18\x02 \x01(\x0b\x32\x18.vega.AssetDetailsUpdateR\x07\x63hanges"\r\n\x0bNewFreeform"\x90\x06\n\rProposalTerms\x12+\n\x11\x63losing_timestamp\x18\x01 \x01(\x03R\x10\x63losingTimestamp\x12/\n\x13\x65nactment_timestamp\x18\x02 \x01(\x03R\x12\x65nactmentTimestamp\x12\x31\n\x14validation_timestamp\x18\x03 \x01(\x03R\x13validationTimestamp\x12\x39\n\rupdate_market\x18\x65 \x01(\x0b\x32\x12.vega.UpdateMarketH\x00R\x0cupdateMarket\x12\x30\n\nnew_market\x18\x66 \x01(\x0b\x32\x0f.vega.NewMarketH\x00R\tnewMarket\x12X\n\x18update_network_parameter\x18g \x01(\x0b\x32\x1c.vega.UpdateNetworkParameterH\x00R\x16updateNetworkParameter\x12-\n\tnew_asset\x18h \x01(\x0b\x32\x0e.vega.NewAssetH\x00R\x08newAsset\x12\x36\n\x0cnew_freeform\x18i \x01(\x0b\x32\x11.vega.NewFreeformH\x00R\x0bnewFreeform\x12\x36\n\x0cupdate_asset\x18j \x01(\x0b\x32\x11.vega.UpdateAssetH\x00R\x0bupdateAsset\x12=\n\x0fnew_spot_market\x18k \x01(\x0b\x32\x13.vega.NewSpotMarketH\x00R\rnewSpotMarket\x12\x46\n\x12update_spot_market\x18l \x01(\x0b\x32\x16.vega.UpdateSpotMarketH\x00R\x10updateSpotMarket\x12\x36\n\x0cnew_transfer\x18m \x01(\x0b\x32\x11.vega.NewTransferH\x00R\x0bnewTransfer\x12?\n\x0f\x63\x61ncel_transfer\x18n \x01(\x0b\x32\x14.vega.CancelTransferH\x00R\x0e\x63\x61ncelTransferB\x08\n\x06\x63hange"W\n\x11ProposalRationale\x12 \n\x0b\x64\x65scription\x18\x01 \x01(\tR\x0b\x64\x65scription\x12\x14\n\x05title\x18\x04 \x01(\tR\x05titleJ\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04"\x86\x03\n\x0eGovernanceData\x12*\n\x08proposal\x18\x01 \x01(\x0b\x32\x0e.vega.ProposalR\x08proposal\x12\x1c\n\x03yes\x18\x02 \x03(\x0b\x32\n.vega.VoteR\x03yes\x12\x1a\n\x02no\x18\x03 \x03(\x0b\x32\n.vega.VoteR\x02no\x12?\n\tyes_party\x18\x04 \x03(\x0b\x32".vega.GovernanceData.YesPartyEntryR\x08yesParty\x12<\n\x08no_party\x18\x05 \x03(\x0b\x32!.vega.GovernanceData.NoPartyEntryR\x07noParty\x1aG\n\rYesPartyEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12 \n\x05value\x18\x02 \x01(\x0b\x32\n.vega.VoteR\x05value:\x02\x38\x01\x1a\x46\n\x0cNoPartyEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12 \n\x05value\x18\x02 \x01(\x0b\x32\n.vega.VoteR\x05value:\x02\x38\x01"\x9a\x07\n\x08Proposal\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1c\n\treference\x18\x02 \x01(\tR\treference\x12\x19\n\x08party_id\x18\x03 \x01(\tR\x07partyId\x12*\n\x05state\x18\x04 \x01(\x0e\x32\x14.vega.Proposal.StateR\x05state\x12\x1c\n\ttimestamp\x18\x05 \x01(\x03R\ttimestamp\x12)\n\x05terms\x18\x06 \x01(\x0b\x32\x13.vega.ProposalTermsR\x05terms\x12\x30\n\x06reason\x18\x07 \x01(\x0e\x32\x13.vega.ProposalErrorH\x00R\x06reason\x88\x01\x01\x12(\n\rerror_details\x18\x08 \x01(\tH\x01R\x0c\x65rrorDetails\x88\x01\x01\x12\x35\n\trationale\x18\t \x01(\x0b\x32\x17.vega.ProposalRationaleR\trationale\x12\x35\n\x16required_participation\x18\n \x01(\tR\x15requiredParticipation\x12+\n\x11required_majority\x18\x0b \x01(\tR\x10requiredMajority\x12^\n)required_liquidity_provider_participation\x18\x0c \x01(\tH\x02R&requiredLiquidityProviderParticipation\x88\x01\x01\x12T\n$required_liquidity_provider_majority\x18\r \x01(\tH\x03R!requiredLiquidityProviderMajority\x88\x01\x01"\xae\x01\n\x05State\x12\x15\n\x11STATE_UNSPECIFIED\x10\x00\x12\x10\n\x0cSTATE_FAILED\x10\x01\x12\x0e\n\nSTATE_OPEN\x10\x02\x12\x10\n\x0cSTATE_PASSED\x10\x03\x12\x12\n\x0eSTATE_REJECTED\x10\x04\x12\x12\n\x0eSTATE_DECLINED\x10\x05\x12\x11\n\rSTATE_ENACTED\x10\x06\x12\x1f\n\x1bSTATE_WAITING_FOR_NODE_VOTE\x10\x07\x42\t\n\x07_reasonB\x10\n\x0e_error_detailsB,\n*_required_liquidity_provider_participationB\'\n%_required_liquidity_provider_majority"\x91\x03\n\x04Vote\x12\x19\n\x08party_id\x18\x01 \x01(\tR\x07partyId\x12&\n\x05value\x18\x02 \x01(\x0e\x32\x10.vega.Vote.ValueR\x05value\x12\x1f\n\x0bproposal_id\x18\x03 \x01(\tR\nproposalId\x12\x1c\n\ttimestamp\x18\x04 \x01(\x03R\ttimestamp\x12\x43\n\x1etotal_governance_token_balance\x18\x05 \x01(\tR\x1btotalGovernanceTokenBalance\x12\x41\n\x1dtotal_governance_token_weight\x18\x06 \x01(\tR\x1atotalGovernanceTokenWeight\x12\x42\n\x1etotal_equity_like_share_weight\x18\x07 \x01(\tR\x1atotalEquityLikeShareWeight";\n\x05Value\x12\x15\n\x11VALUE_UNSPECIFIED\x10\x00\x12\x0c\n\x08VALUE_NO\x10\x01\x12\r\n\tVALUE_YES\x10\x02"M\n\x0e\x43\x61ncelTransfer\x12;\n\x07\x63hanges\x18\x01 \x01(\x0b\x32!.vega.CancelTransferConfigurationR\x07\x63hanges">\n\x1b\x43\x61ncelTransferConfiguration\x12\x1f\n\x0btransfer_id\x18\x01 \x01(\tR\ntransferId"G\n\x0bNewTransfer\x12\x38\n\x07\x63hanges\x18\x01 \x01(\x0b\x32\x1e.vega.NewTransferConfigurationR\x07\x63hanges"\xd9\x03\n\x18NewTransferConfiguration\x12\x32\n\x0bsource_type\x18\x01 \x01(\x0e\x32\x11.vega.AccountTypeR\nsourceType\x12\x16\n\x06source\x18\x02 \x01(\tR\x06source\x12\x41\n\rtransfer_type\x18\x03 \x01(\x0e\x32\x1c.vega.GovernanceTransferTypeR\x0ctransferType\x12\x16\n\x06\x61mount\x18\x04 \x01(\tR\x06\x61mount\x12\x14\n\x05\x61sset\x18\x05 \x01(\tR\x05\x61sset\x12.\n\x13\x66raction_of_balance\x18\x06 \x01(\tR\x11\x66ractionOfBalance\x12<\n\x10\x64\x65stination_type\x18\x07 \x01(\x0e\x32\x11.vega.AccountTypeR\x0f\x64\x65stinationType\x12 \n\x0b\x64\x65stination\x18\x08 \x01(\tR\x0b\x64\x65stination\x12/\n\x07one_off\x18\x65 \x01(\x0b\x32\x14.vega.OneOffTransferH\x00R\x06oneOff\x12\x37\n\trecurring\x18\x66 \x01(\x0b\x32\x17.vega.RecurringTransferH\x00R\trecurringB\x06\n\x04kind"/\n\x0eOneOffTransfer\x12\x1d\n\ndeliver_on\x18\x01 \x01(\x03R\tdeliverOn"d\n\x11RecurringTransfer\x12\x1f\n\x0bstart_epoch\x18\x01 \x01(\x04R\nstartEpoch\x12 \n\tend_epoch\x18\x02 \x01(\x04H\x00R\x08\x65ndEpoch\x88\x01\x01\x42\x0c\n\n_end_epoch*\xc9\x10\n\rProposalError\x12\x1e\n\x1aPROPOSAL_ERROR_UNSPECIFIED\x10\x00\x12&\n"PROPOSAL_ERROR_CLOSE_TIME_TOO_SOON\x10\x01\x12&\n"PROPOSAL_ERROR_CLOSE_TIME_TOO_LATE\x10\x02\x12&\n"PROPOSAL_ERROR_ENACT_TIME_TOO_SOON\x10\x03\x12&\n"PROPOSAL_ERROR_ENACT_TIME_TOO_LATE\x10\x04\x12&\n"PROPOSAL_ERROR_INSUFFICIENT_TOKENS\x10\x05\x12.\n*PROPOSAL_ERROR_INVALID_INSTRUMENT_SECURITY\x10\x06\x12\x1d\n\x19PROPOSAL_ERROR_NO_PRODUCT\x10\x07\x12&\n"PROPOSAL_ERROR_UNSUPPORTED_PRODUCT\x10\x08\x12"\n\x1ePROPOSAL_ERROR_NO_TRADING_MODE\x10\x0b\x12+\n\'PROPOSAL_ERROR_UNSUPPORTED_TRADING_MODE\x10\x0c\x12)\n%PROPOSAL_ERROR_NODE_VALIDATION_FAILED\x10\r\x12.\n*PROPOSAL_ERROR_MISSING_BUILTIN_ASSET_FIELD\x10\x0e\x12\x31\n-PROPOSAL_ERROR_MISSING_ERC20_CONTRACT_ADDRESS\x10\x0f\x12 \n\x1cPROPOSAL_ERROR_INVALID_ASSET\x10\x10\x12*\n&PROPOSAL_ERROR_INCOMPATIBLE_TIMESTAMPS\x10\x11\x12%\n!PROPOSAL_ERROR_NO_RISK_PARAMETERS\x10\x12\x12\x30\n,PROPOSAL_ERROR_NETWORK_PARAMETER_INVALID_KEY\x10\x13\x12\x32\n.PROPOSAL_ERROR_NETWORK_PARAMETER_INVALID_VALUE\x10\x14\x12\x36\n2PROPOSAL_ERROR_NETWORK_PARAMETER_VALIDATION_FAILED\x10\x15\x12\x35\n1PROPOSAL_ERROR_OPENING_AUCTION_DURATION_TOO_SMALL\x10\x16\x12\x35\n1PROPOSAL_ERROR_OPENING_AUCTION_DURATION_TOO_LARGE\x10\x17\x12/\n+PROPOSAL_ERROR_COULD_NOT_INSTANTIATE_MARKET\x10\x19\x12)\n%PROPOSAL_ERROR_INVALID_FUTURE_PRODUCT\x10\x1a\x12)\n%PROPOSAL_ERROR_INVALID_RISK_PARAMETER\x10\x1e\x12\x31\n-PROPOSAL_ERROR_MAJORITY_THRESHOLD_NOT_REACHED\x10\x1f\x12\x36\n2PROPOSAL_ERROR_PARTICIPATION_THRESHOLD_NOT_REACHED\x10 \x12(\n$PROPOSAL_ERROR_INVALID_ASSET_DETAILS\x10!\x12\x1f\n\x1bPROPOSAL_ERROR_UNKNOWN_TYPE\x10"\x12.\n*PROPOSAL_ERROR_UNKNOWN_RISK_PARAMETER_TYPE\x10#\x12#\n\x1fPROPOSAL_ERROR_INVALID_FREEFORM\x10$\x12\x31\n-PROPOSAL_ERROR_INSUFFICIENT_EQUITY_LIKE_SHARE\x10%\x12!\n\x1dPROPOSAL_ERROR_INVALID_MARKET\x10&\x12\x31\n-PROPOSAL_ERROR_TOO_MANY_MARKET_DECIMAL_PLACES\x10\'\x12\x35\n1PROPOSAL_ERROR_TOO_MANY_PRICE_MONITORING_TRIGGERS\x10(\x12/\n+PROPOSAL_ERROR_ERC20_ADDRESS_ALREADY_IN_USE\x10)\x12-\n)PROPOSAL_ERROR_LP_PRICE_RANGE_NONPOSITIVE\x10*\x12+\n\'PROPOSAL_ERROR_LP_PRICE_RANGE_TOO_LARGE\x10+\x12\x36\n2PROPOSAL_ERROR_LINEAR_SLIPPAGE_FACTOR_OUT_OF_RANGE\x10,\x12\x39\n5PROPOSAL_ERROR_QUADRATIC_SLIPPAGE_FACTOR_OUT_OF_RANGE\x10-\x12\x1f\n\x1bPROPOSAL_ERROR_INVALID_SPOT\x10.\x12(\n$PROPOSAL_ERROR_SPOT_PRODUCT_DISABLED\x10/\x12+\n\'PROPOSAL_ERROR_INVALID_SUCCESSOR_MARKET\x10\x30\x12\x36\n2PROPOSAL_ERROR_GOVERNANCE_TRANSFER_PROPOSAL_FAILED\x10\x31\x12\x37\n3PROPOSAL_ERROR_GOVERNANCE_TRANSFER_PROPOSAL_INVALID\x10\x32\x12>\n:PROPOSAL_ERROR_GOVERNANCE_CANCEL_TRANSFER_PROPOSAL_INVALID\x10\x33*\x99\x01\n\x16GovernanceTransferType\x12(\n$GOVERNANCE_TRANSFER_TYPE_UNSPECIFIED\x10\x00\x12+\n\'GOVERNANCE_TRANSFER_TYPE_ALL_OR_NOTHING\x10\x01\x12(\n$GOVERNANCE_TRANSFER_TYPE_BEST_EFFORT\x10\x02\x42\'Z%code.vegaprotocol.io/vega/protos/vegab\x06proto3'
 )
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "vega.governance_pb2", globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "vega.governance_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b"Z%code.vegaprotocol.io/vega/protos/vega"
     _GOVERNANCEDATA_YESPARTYENTRY._options = None
     _GOVERNANCEDATA_YESPARTYENTRY._serialized_options = b"8\001"
     _GOVERNANCEDATA_NOPARTYENTRY._options = None
     _GOVERNANCEDATA_NOPARTYENTRY._serialized_options = b"8\001"
-    _PROPOSALERROR._serialized_start = 5205
-    _PROPOSALERROR._serialized_end = 7029
-    _FUTUREPRODUCT._serialized_start = 112
-    _FUTUREPRODUCT._serialized_end = 517
-    _INSTRUMENTCONFIGURATION._serialized_start = 519
-    _INSTRUMENTCONFIGURATION._serialized_end = 642
-    _NEWMARKETCONFIGURATION._serialized_start = 645
-    _NEWMARKETCONFIGURATION._serialized_end = 1342
-    _NEWMARKET._serialized_start = 1344
-    _NEWMARKET._serialized_end = 1411
-    _UPDATEMARKET._serialized_start = 1413
-    _UPDATEMARKET._serialized_end = 1515
-    _UPDATEMARKETCONFIGURATION._serialized_start = 1518
-    _UPDATEMARKETCONFIGURATION._serialized_end = 2129
-    _UPDATEINSTRUMENTCONFIGURATION._serialized_start = 2131
-    _UPDATEINSTRUMENTCONFIGURATION._serialized_end = 2246
-    _UPDATEFUTUREPRODUCT._serialized_start = 2249
-    _UPDATEFUTUREPRODUCT._serialized_end = 2617
-    _UPDATENETWORKPARAMETER._serialized_start = 2619
-    _UPDATENETWORKPARAMETER._serialized_end = 2693
-    _NEWASSET._serialized_start = 2695
-    _NEWASSET._serialized_end = 2751
-    _UPDATEASSET._serialized_start = 2753
-    _UPDATEASSET._serialized_end = 2845
-    _NEWFREEFORM._serialized_start = 2847
-    _NEWFREEFORM._serialized_end = 2860
-    _PROPOSALTERMS._serialized_start = 2863
-    _PROPOSALTERMS._serialized_end = 3391
-    _PROPOSALRATIONALE._serialized_start = 3393
-    _PROPOSALRATIONALE._serialized_end = 3480
-    _GOVERNANCEDATA._serialized_start = 3483
-    _GOVERNANCEDATA._serialized_end = 3873
-    _GOVERNANCEDATA_YESPARTYENTRY._serialized_start = 3730
-    _GOVERNANCEDATA_YESPARTYENTRY._serialized_end = 3801
-    _GOVERNANCEDATA_NOPARTYENTRY._serialized_start = 3803
-    _GOVERNANCEDATA_NOPARTYENTRY._serialized_end = 3873
-    _PROPOSAL._serialized_start = 3876
-    _PROPOSAL._serialized_end = 4798
-    _PROPOSAL_STATE._serialized_start = 4508
-    _PROPOSAL_STATE._serialized_end = 4682
-    _VOTE._serialized_start = 4801
-    _VOTE._serialized_end = 5202
-    _VOTE_VALUE._serialized_start = 5143
-    _VOTE_VALUE._serialized_end = 5202
+    _globals["_PROPOSALERROR"]._serialized_start = 7738
+    _globals["_PROPOSALERROR"]._serialized_end = 9859
+    _globals["_GOVERNANCETRANSFERTYPE"]._serialized_start = 9862
+    _globals["_GOVERNANCETRANSFERTYPE"]._serialized_end = 10015
+    _globals["_SPOTPRODUCT"]._serialized_start = 111
+    _globals["_SPOTPRODUCT"]._serialized_end = 208
+    _globals["_FUTUREPRODUCT"]._serialized_start = 211
+    _globals["_FUTUREPRODUCT"]._serialized_end = 616
+    _globals["_INSTRUMENTCONFIGURATION"]._serialized_start = 619
+    _globals["_INSTRUMENTCONFIGURATION"]._serialized_end = 783
+    _globals["_NEWSPOTMARKETCONFIGURATION"]._serialized_start = 786
+    _globals["_NEWSPOTMARKETCONFIGURATION"]._serialized_end = 1311
+    _globals["_NEWMARKETCONFIGURATION"]._serialized_start = 1314
+    _globals["_NEWMARKETCONFIGURATION"]._serialized_end = 2090
+    _globals["_NEWSPOTMARKET"]._serialized_start = 2092
+    _globals["_NEWSPOTMARKET"]._serialized_end = 2167
+    _globals["_SUCCESSORCONFIGURATION"]._serialized_start = 2169
+    _globals["_SUCCESSORCONFIGURATION"]._serialized_end = 2291
+    _globals["_NEWMARKET"]._serialized_start = 2293
+    _globals["_NEWMARKET"]._serialized_end = 2360
+    _globals["_UPDATEMARKET"]._serialized_start = 2362
+    _globals["_UPDATEMARKET"]._serialized_end = 2464
+    _globals["_UPDATESPOTMARKET"]._serialized_start = 2466
+    _globals["_UPDATESPOTMARKET"]._serialized_end = 2576
+    _globals["_UPDATEMARKETCONFIGURATION"]._serialized_start = 2579
+    _globals["_UPDATEMARKETCONFIGURATION"]._serialized_end = 3190
+    _globals["_UPDATESPOTMARKETCONFIGURATION"]._serialized_start = 3193
+    _globals["_UPDATESPOTMARKETCONFIGURATION"]._serialized_end = 3563
+    _globals["_UPDATEINSTRUMENTCONFIGURATION"]._serialized_start = 3565
+    _globals["_UPDATEINSTRUMENTCONFIGURATION"]._serialized_end = 3680
+    _globals["_UPDATEFUTUREPRODUCT"]._serialized_start = 3683
+    _globals["_UPDATEFUTUREPRODUCT"]._serialized_end = 4051
+    _globals["_UPDATENETWORKPARAMETER"]._serialized_start = 4053
+    _globals["_UPDATENETWORKPARAMETER"]._serialized_end = 4127
+    _globals["_NEWASSET"]._serialized_start = 4129
+    _globals["_NEWASSET"]._serialized_end = 4185
+    _globals["_UPDATEASSET"]._serialized_start = 4187
+    _globals["_UPDATEASSET"]._serialized_end = 4279
+    _globals["_NEWFREEFORM"]._serialized_start = 4281
+    _globals["_NEWFREEFORM"]._serialized_end = 4294
+    _globals["_PROPOSALTERMS"]._serialized_start = 4297
+    _globals["_PROPOSALTERMS"]._serialized_end = 5081
+    _globals["_PROPOSALRATIONALE"]._serialized_start = 5083
+    _globals["_PROPOSALRATIONALE"]._serialized_end = 5170
+    _globals["_GOVERNANCEDATA"]._serialized_start = 5173
+    _globals["_GOVERNANCEDATA"]._serialized_end = 5563
+    _globals["_GOVERNANCEDATA_YESPARTYENTRY"]._serialized_start = 5420
+    _globals["_GOVERNANCEDATA_YESPARTYENTRY"]._serialized_end = 5491
+    _globals["_GOVERNANCEDATA_NOPARTYENTRY"]._serialized_start = 5493
+    _globals["_GOVERNANCEDATA_NOPARTYENTRY"]._serialized_end = 5563
+    _globals["_PROPOSAL"]._serialized_start = 5566
+    _globals["_PROPOSAL"]._serialized_end = 6488
+    _globals["_PROPOSAL_STATE"]._serialized_start = 6198
+    _globals["_PROPOSAL_STATE"]._serialized_end = 6372
+    _globals["_VOTE"]._serialized_start = 6491
+    _globals["_VOTE"]._serialized_end = 6892
+    _globals["_VOTE_VALUE"]._serialized_start = 6833
+    _globals["_VOTE_VALUE"]._serialized_end = 6892
+    _globals["_CANCELTRANSFER"]._serialized_start = 6894
+    _globals["_CANCELTRANSFER"]._serialized_end = 6971
+    _globals["_CANCELTRANSFERCONFIGURATION"]._serialized_start = 6973
+    _globals["_CANCELTRANSFERCONFIGURATION"]._serialized_end = 7035
+    _globals["_NEWTRANSFER"]._serialized_start = 7037
+    _globals["_NEWTRANSFER"]._serialized_end = 7108
+    _globals["_NEWTRANSFERCONFIGURATION"]._serialized_start = 7111
+    _globals["_NEWTRANSFERCONFIGURATION"]._serialized_end = 7584
+    _globals["_ONEOFFTRANSFER"]._serialized_start = 7586
+    _globals["_ONEOFFTRANSFER"]._serialized_end = 7633
+    _globals["_RECURRINGTRANSFER"]._serialized_start = 7635
+    _globals["_RECURRINGTRANSFER"]._serialized_end = 7735
 # @@protoc_insertion_point(module_scope)
```

### Comparing `vega_sim-1.1.1/vega_sim/proto/vega/markets_pb2.py` & `vega_sim-1.2.0/vega_sim/proto/vega/markets_pb2.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,73 +1,76 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: vega/markets.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from . import data_source_pb2 as vega_dot_data__source__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x12vega/markets.proto\x12\x04vega\x1a\x16vega/data_source.proto"E\n\x0f\x41uctionDuration\x12\x1a\n\x08\x64uration\x18\x01 \x01(\x03R\x08\x64uration\x12\x16\n\x06volume\x18\x02 \x01(\x04R\x06volume"\x82\x03\n\x06\x46uture\x12)\n\x10settlement_asset\x18\x01 \x01(\tR\x0fsettlementAsset\x12\x1d\n\nquote_name\x18\x02 \x01(\tR\tquoteName\x12\x63\n$data_source_spec_for_settlement_data\x18\x03 \x01(\x0b\x32\x14.vega.DataSourceSpecR\x1f\x64\x61taSourceSpecForSettlementData\x12k\n(data_source_spec_for_trading_termination\x18\x04 \x01(\x0b\x32\x14.vega.DataSourceSpecR#dataSourceSpecForTradingTermination\x12\\\n\x18\x64\x61ta_source_spec_binding\x18\x05 \x01(\x0b\x32#.vega.DataSourceSpecToFutureBindingR\x15\x64\x61taSourceSpecBinding"\x9b\x01\n\x1d\x44\x61taSourceSpecToFutureBinding\x12\x38\n\x18settlement_data_property\x18\x01 \x01(\tR\x16settlementDataProperty\x12@\n\x1ctrading_termination_property\x18\x02 \x01(\tR\x1atradingTerminationProperty"(\n\x12InstrumentMetadata\x12\x12\n\x04tags\x18\x01 \x03(\tR\x04tags"\xad\x01\n\nInstrument\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04\x63ode\x18\x02 \x01(\tR\x04\x63ode\x12\x12\n\x04name\x18\x03 \x01(\tR\x04name\x12\x34\n\x08metadata\x18\x04 \x01(\x0b\x32\x18.vega.InstrumentMetadataR\x08metadata\x12&\n\x06\x66uture\x18\x64 \x01(\x0b\x32\x0c.vega.FutureH\x00R\x06\x66utureB\t\n\x07product"\x92\x01\n\x12LogNormalRiskModel\x12\x36\n\x17risk_aversion_parameter\x18\x01 \x01(\x01R\x15riskAversionParameter\x12\x10\n\x03tau\x18\x02 \x01(\x01R\x03tau\x12\x32\n\x06params\x18\x03 \x01(\x0b\x32\x1a.vega.LogNormalModelParamsR\x06params"J\n\x14LogNormalModelParams\x12\x0e\n\x02mu\x18\x01 \x01(\x01R\x02mu\x12\x0c\n\x01r\x18\x02 \x01(\x01R\x01r\x12\x14\n\x05sigma\x18\x03 \x01(\x01R\x05sigma"B\n\x0fSimpleRiskModel\x12/\n\x06params\x18\x01 \x01(\x0b\x32\x17.vega.SimpleModelParamsR\x06params"\xd1\x01\n\x11SimpleModelParams\x12\x1f\n\x0b\x66\x61\x63tor_long\x18\x01 \x01(\x01R\nfactorLong\x12!\n\x0c\x66\x61\x63tor_short\x18\x02 \x01(\x01R\x0b\x66\x61\x63torShort\x12\x1e\n\x0bmax_move_up\x18\x03 \x01(\x01R\tmaxMoveUp\x12"\n\rmin_move_down\x18\x04 \x01(\x01R\x0bminMoveDown\x12\x34\n\x16probability_of_trading\x18\x05 \x01(\x01R\x14probabilityOfTrading"\x89\x01\n\x0eScalingFactors\x12!\n\x0csearch_level\x18\x01 \x01(\x01R\x0bsearchLevel\x12%\n\x0einitial_margin\x18\x02 \x01(\x01R\rinitialMargin\x12-\n\x12\x63ollateral_release\x18\x03 \x01(\x01R\x11\x63ollateralRelease"Q\n\x10MarginCalculator\x12=\n\x0fscaling_factors\x18\x01 \x01(\x0b\x32\x14.vega.ScalingFactorsR\x0escalingFactors"\xad\x02\n\x12TradableInstrument\x12\x30\n\ninstrument\x18\x01 \x01(\x0b\x32\x10.vega.InstrumentR\ninstrument\x12\x43\n\x11margin_calculator\x18\x02 \x01(\x0b\x32\x16.vega.MarginCalculatorR\x10marginCalculator\x12M\n\x15log_normal_risk_model\x18\x64 \x01(\x0b\x32\x18.vega.LogNormalRiskModelH\x00R\x12logNormalRiskModel\x12\x43\n\x11simple_risk_model\x18\x65 \x01(\x0b\x32\x15.vega.SimpleRiskModelH\x00R\x0fsimpleRiskModelB\x0c\n\nrisk_model"}\n\nFeeFactors\x12\x1b\n\tmaker_fee\x18\x01 \x01(\tR\x08makerFee\x12-\n\x12infrastructure_fee\x18\x02 \x01(\tR\x11infrastructureFee\x12#\n\rliquidity_fee\x18\x03 \x01(\tR\x0cliquidityFee"2\n\x04\x46\x65\x65s\x12*\n\x07\x66\x61\x63tors\x18\x01 \x01(\x0b\x32\x10.vega.FeeFactorsR\x07\x66\x61\x63tors"\x81\x01\n\x16PriceMonitoringTrigger\x12\x18\n\x07horizon\x18\x01 \x01(\x03R\x07horizon\x12 \n\x0bprobability\x18\x02 \x01(\tR\x0bprobability\x12+\n\x11\x61uction_extension\x18\x03 \x01(\x03R\x10\x61uctionExtension"U\n\x19PriceMonitoringParameters\x12\x38\n\x08triggers\x18\x01 \x03(\x0b\x32\x1c.vega.PriceMonitoringTriggerR\x08triggers"Z\n\x17PriceMonitoringSettings\x12?\n\nparameters\x18\x01 \x01(\x0b\x32\x1f.vega.PriceMonitoringParametersR\nparameters"\xcc\x01\n\x1dLiquidityMonitoringParameters\x12S\n\x17target_stake_parameters\x18\x01 \x01(\x0b\x32\x1b.vega.TargetStakeParametersR\x15targetStakeParameters\x12)\n\x10triggering_ratio\x18\x02 \x01(\tR\x0ftriggeringRatio\x12+\n\x11\x61uction_extension\x18\x03 \x01(\x03R\x10\x61uctionExtension"_\n\x15TargetStakeParameters\x12\x1f\n\x0btime_window\x18\x01 \x01(\x03R\ntimeWindow\x12%\n\x0escaling_factor\x18\x02 \x01(\x01R\rscalingFactor"\xd8\t\n\x06Market\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12I\n\x13tradable_instrument\x18\x02 \x01(\x0b\x32\x18.vega.TradableInstrumentR\x12tradableInstrument\x12%\n\x0e\x64\x65\x63imal_places\x18\x03 \x01(\x04R\rdecimalPlaces\x12\x1e\n\x04\x66\x65\x65s\x18\x04 \x01(\x0b\x32\n.vega.FeesR\x04\x66\x65\x65s\x12>\n\x0fopening_auction\x18\x05 \x01(\x0b\x32\x15.vega.AuctionDurationR\x0eopeningAuction\x12Y\n\x19price_monitoring_settings\x18\x06 \x01(\x0b\x32\x1d.vega.PriceMonitoringSettingsR\x17priceMonitoringSettings\x12k\n\x1fliquidity_monitoring_parameters\x18\x07 \x01(\x0b\x32#.vega.LiquidityMonitoringParametersR\x1dliquidityMonitoringParameters\x12;\n\x0ctrading_mode\x18\x08 \x01(\x0e\x32\x18.vega.Market.TradingModeR\x0btradingMode\x12(\n\x05state\x18\t \x01(\x0e\x32\x12.vega.Market.StateR\x05state\x12\x43\n\x11market_timestamps\x18\n \x01(\x0b\x32\x16.vega.MarketTimestampsR\x10marketTimestamps\x12\x36\n\x17position_decimal_places\x18\x0b \x01(\x03R\x15positionDecimalPlaces\x12$\n\x0elp_price_range\x18\x0c \x01(\tR\x0clpPriceRange\x12\x34\n\x16linear_slippage_factor\x18\r \x01(\tR\x14linearSlippageFactor\x12:\n\x19quadratic_slippage_factor\x18\x0e \x01(\tR\x17quadraticSlippageFactor"\xd8\x01\n\x05State\x12\x15\n\x11STATE_UNSPECIFIED\x10\x00\x12\x12\n\x0eSTATE_PROPOSED\x10\x01\x12\x12\n\x0eSTATE_REJECTED\x10\x02\x12\x11\n\rSTATE_PENDING\x10\x03\x12\x13\n\x0fSTATE_CANCELLED\x10\x04\x12\x10\n\x0cSTATE_ACTIVE\x10\x05\x12\x13\n\x0fSTATE_SUSPENDED\x10\x06\x12\x10\n\x0cSTATE_CLOSED\x10\x07\x12\x1c\n\x18STATE_TRADING_TERMINATED\x10\x08\x12\x11\n\rSTATE_SETTLED\x10\t"\xcc\x01\n\x0bTradingMode\x12\x1c\n\x18TRADING_MODE_UNSPECIFIED\x10\x00\x12\x1b\n\x17TRADING_MODE_CONTINUOUS\x10\x01\x12\x1e\n\x1aTRADING_MODE_BATCH_AUCTION\x10\x02\x12 \n\x1cTRADING_MODE_OPENING_AUCTION\x10\x03\x12#\n\x1fTRADING_MODE_MONITORING_AUCTION\x10\x04\x12\x1b\n\x17TRADING_MODE_NO_TRADING\x10\x05"r\n\x10MarketTimestamps\x12\x1a\n\x08proposed\x18\x01 \x01(\x03R\x08proposed\x12\x18\n\x07pending\x18\x02 \x01(\x03R\x07pending\x12\x12\n\x04open\x18\x03 \x01(\x03R\x04open\x12\x14\n\x05\x63lose\x18\x04 \x01(\x03R\x05\x63loseB\'Z%code.vegaprotocol.io/vega/protos/vegab\x06proto3'
+    b'\n\x12vega/markets.proto\x12\x04vega\x1a\x16vega/data_source.proto"E\n\x0f\x41uctionDuration\x12\x1a\n\x08\x64uration\x18\x01 \x01(\x03R\x08\x64uration\x12\x16\n\x06volume\x18\x02 \x01(\x04R\x06volume"Z\n\x04Spot\x12\x1d\n\nbase_asset\x18\x01 \x01(\tR\tbaseAsset\x12\x1f\n\x0bquote_asset\x18\x02 \x01(\tR\nquoteAsset\x12\x12\n\x04name\x18\x03 \x01(\tR\x04name"\x82\x03\n\x06\x46uture\x12)\n\x10settlement_asset\x18\x01 \x01(\tR\x0fsettlementAsset\x12\x1d\n\nquote_name\x18\x02 \x01(\tR\tquoteName\x12\x63\n$data_source_spec_for_settlement_data\x18\x03 \x01(\x0b\x32\x14.vega.DataSourceSpecR\x1f\x64\x61taSourceSpecForSettlementData\x12k\n(data_source_spec_for_trading_termination\x18\x04 \x01(\x0b\x32\x14.vega.DataSourceSpecR#dataSourceSpecForTradingTermination\x12\\\n\x18\x64\x61ta_source_spec_binding\x18\x05 \x01(\x0b\x32#.vega.DataSourceSpecToFutureBindingR\x15\x64\x61taSourceSpecBinding"\x9b\x01\n\x1d\x44\x61taSourceSpecToFutureBinding\x12\x38\n\x18settlement_data_property\x18\x01 \x01(\tR\x16settlementDataProperty\x12@\n\x1ctrading_termination_property\x18\x02 \x01(\tR\x1atradingTerminationProperty"(\n\x12InstrumentMetadata\x12\x12\n\x04tags\x18\x01 \x03(\tR\x04tags"\xcf\x01\n\nInstrument\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04\x63ode\x18\x02 \x01(\tR\x04\x63ode\x12\x12\n\x04name\x18\x03 \x01(\tR\x04name\x12\x34\n\x08metadata\x18\x04 \x01(\x0b\x32\x18.vega.InstrumentMetadataR\x08metadata\x12&\n\x06\x66uture\x18\x64 \x01(\x0b\x32\x0c.vega.FutureH\x00R\x06\x66uture\x12 \n\x04spot\x18\x65 \x01(\x0b\x32\n.vega.SpotH\x00R\x04spotB\t\n\x07product"\x92\x01\n\x12LogNormalRiskModel\x12\x36\n\x17risk_aversion_parameter\x18\x01 \x01(\x01R\x15riskAversionParameter\x12\x10\n\x03tau\x18\x02 \x01(\x01R\x03tau\x12\x32\n\x06params\x18\x03 \x01(\x0b\x32\x1a.vega.LogNormalModelParamsR\x06params"J\n\x14LogNormalModelParams\x12\x0e\n\x02mu\x18\x01 \x01(\x01R\x02mu\x12\x0c\n\x01r\x18\x02 \x01(\x01R\x01r\x12\x14\n\x05sigma\x18\x03 \x01(\x01R\x05sigma"B\n\x0fSimpleRiskModel\x12/\n\x06params\x18\x01 \x01(\x0b\x32\x17.vega.SimpleModelParamsR\x06params"\xd1\x01\n\x11SimpleModelParams\x12\x1f\n\x0b\x66\x61\x63tor_long\x18\x01 \x01(\x01R\nfactorLong\x12!\n\x0c\x66\x61\x63tor_short\x18\x02 \x01(\x01R\x0b\x66\x61\x63torShort\x12\x1e\n\x0bmax_move_up\x18\x03 \x01(\x01R\tmaxMoveUp\x12"\n\rmin_move_down\x18\x04 \x01(\x01R\x0bminMoveDown\x12\x34\n\x16probability_of_trading\x18\x05 \x01(\x01R\x14probabilityOfTrading"\x89\x01\n\x0eScalingFactors\x12!\n\x0csearch_level\x18\x01 \x01(\x01R\x0bsearchLevel\x12%\n\x0einitial_margin\x18\x02 \x01(\x01R\rinitialMargin\x12-\n\x12\x63ollateral_release\x18\x03 \x01(\x01R\x11\x63ollateralRelease"Q\n\x10MarginCalculator\x12=\n\x0fscaling_factors\x18\x01 \x01(\x0b\x32\x14.vega.ScalingFactorsR\x0escalingFactors"\xad\x02\n\x12TradableInstrument\x12\x30\n\ninstrument\x18\x01 \x01(\x0b\x32\x10.vega.InstrumentR\ninstrument\x12\x43\n\x11margin_calculator\x18\x02 \x01(\x0b\x32\x16.vega.MarginCalculatorR\x10marginCalculator\x12M\n\x15log_normal_risk_model\x18\x64 \x01(\x0b\x32\x18.vega.LogNormalRiskModelH\x00R\x12logNormalRiskModel\x12\x43\n\x11simple_risk_model\x18\x65 \x01(\x0b\x32\x15.vega.SimpleRiskModelH\x00R\x0fsimpleRiskModelB\x0c\n\nrisk_model"}\n\nFeeFactors\x12\x1b\n\tmaker_fee\x18\x01 \x01(\tR\x08makerFee\x12-\n\x12infrastructure_fee\x18\x02 \x01(\tR\x11infrastructureFee\x12#\n\rliquidity_fee\x18\x03 \x01(\tR\x0cliquidityFee"2\n\x04\x46\x65\x65s\x12*\n\x07\x66\x61\x63tors\x18\x01 \x01(\x0b\x32\x10.vega.FeeFactorsR\x07\x66\x61\x63tors"\x81\x01\n\x16PriceMonitoringTrigger\x12\x18\n\x07horizon\x18\x01 \x01(\x03R\x07horizon\x12 \n\x0bprobability\x18\x02 \x01(\tR\x0bprobability\x12+\n\x11\x61uction_extension\x18\x03 \x01(\x03R\x10\x61uctionExtension"U\n\x19PriceMonitoringParameters\x12\x38\n\x08triggers\x18\x01 \x03(\x0b\x32\x1c.vega.PriceMonitoringTriggerR\x08triggers"Z\n\x17PriceMonitoringSettings\x12?\n\nparameters\x18\x01 \x01(\x0b\x32\x1f.vega.PriceMonitoringParametersR\nparameters"\xcc\x01\n\x1dLiquidityMonitoringParameters\x12S\n\x17target_stake_parameters\x18\x01 \x01(\x0b\x32\x1b.vega.TargetStakeParametersR\x15targetStakeParameters\x12)\n\x10triggering_ratio\x18\x02 \x01(\tR\x0ftriggeringRatio\x12+\n\x11\x61uction_extension\x18\x03 \x01(\x03R\x10\x61uctionExtension"_\n\x15TargetStakeParameters\x12\x1f\n\x0btime_window\x18\x01 \x01(\x03R\ntimeWindow\x12%\n\x0escaling_factor\x18\x02 \x01(\x01R\rscalingFactor"\xc2\x0b\n\x06Market\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12I\n\x13tradable_instrument\x18\x02 \x01(\x0b\x32\x18.vega.TradableInstrumentR\x12tradableInstrument\x12%\n\x0e\x64\x65\x63imal_places\x18\x03 \x01(\x04R\rdecimalPlaces\x12\x1e\n\x04\x66\x65\x65s\x18\x04 \x01(\x0b\x32\n.vega.FeesR\x04\x66\x65\x65s\x12>\n\x0fopening_auction\x18\x05 \x01(\x0b\x32\x15.vega.AuctionDurationR\x0eopeningAuction\x12Y\n\x19price_monitoring_settings\x18\x06 \x01(\x0b\x32\x1d.vega.PriceMonitoringSettingsR\x17priceMonitoringSettings\x12k\n\x1fliquidity_monitoring_parameters\x18\x07 \x01(\x0b\x32#.vega.LiquidityMonitoringParametersR\x1dliquidityMonitoringParameters\x12;\n\x0ctrading_mode\x18\x08 \x01(\x0e\x32\x18.vega.Market.TradingModeR\x0btradingMode\x12(\n\x05state\x18\t \x01(\x0e\x32\x12.vega.Market.StateR\x05state\x12\x43\n\x11market_timestamps\x18\n \x01(\x0b\x32\x16.vega.MarketTimestampsR\x10marketTimestamps\x12\x36\n\x17position_decimal_places\x18\x0b \x01(\x03R\x15positionDecimalPlaces\x12$\n\x0elp_price_range\x18\x0c \x01(\tR\x0clpPriceRange\x12\x34\n\x16linear_slippage_factor\x18\r \x01(\tR\x14linearSlippageFactor\x12:\n\x19quadratic_slippage_factor\x18\x0e \x01(\tR\x17quadraticSlippageFactor\x12-\n\x10parent_market_id\x18\x0f \x01(\tH\x00R\x0eparentMarketId\x88\x01\x01\x12;\n\x17insurance_pool_fraction\x18\x10 \x01(\tH\x01R\x15insurancePoolFraction\x88\x01\x01\x12\x33\n\x13successor_market_id\x18\x11 \x01(\tH\x02R\x11successorMarketId\x88\x01\x01"\xd8\x01\n\x05State\x12\x15\n\x11STATE_UNSPECIFIED\x10\x00\x12\x12\n\x0eSTATE_PROPOSED\x10\x01\x12\x12\n\x0eSTATE_REJECTED\x10\x02\x12\x11\n\rSTATE_PENDING\x10\x03\x12\x13\n\x0fSTATE_CANCELLED\x10\x04\x12\x10\n\x0cSTATE_ACTIVE\x10\x05\x12\x13\n\x0fSTATE_SUSPENDED\x10\x06\x12\x10\n\x0cSTATE_CLOSED\x10\x07\x12\x1c\n\x18STATE_TRADING_TERMINATED\x10\x08\x12\x11\n\rSTATE_SETTLED\x10\t"\xcc\x01\n\x0bTradingMode\x12\x1c\n\x18TRADING_MODE_UNSPECIFIED\x10\x00\x12\x1b\n\x17TRADING_MODE_CONTINUOUS\x10\x01\x12\x1e\n\x1aTRADING_MODE_BATCH_AUCTION\x10\x02\x12 \n\x1cTRADING_MODE_OPENING_AUCTION\x10\x03\x12#\n\x1fTRADING_MODE_MONITORING_AUCTION\x10\x04\x12\x1b\n\x17TRADING_MODE_NO_TRADING\x10\x05\x42\x13\n\x11_parent_market_idB\x1a\n\x18_insurance_pool_fractionB\x16\n\x14_successor_market_id"r\n\x10MarketTimestamps\x12\x1a\n\x08proposed\x18\x01 \x01(\x03R\x08proposed\x12\x18\n\x07pending\x18\x02 \x01(\x03R\x07pending\x12\x12\n\x04open\x18\x03 \x01(\x03R\x04open\x12\x14\n\x05\x63lose\x18\x04 \x01(\x03R\x05\x63loseB\'Z%code.vegaprotocol.io/vega/protos/vegab\x06proto3'
 )
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "vega.markets_pb2", globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "vega.markets_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b"Z%code.vegaprotocol.io/vega/protos/vega"
-    _AUCTIONDURATION._serialized_start = 52
-    _AUCTIONDURATION._serialized_end = 121
-    _FUTURE._serialized_start = 124
-    _FUTURE._serialized_end = 510
-    _DATASOURCESPECTOFUTUREBINDING._serialized_start = 513
-    _DATASOURCESPECTOFUTUREBINDING._serialized_end = 668
-    _INSTRUMENTMETADATA._serialized_start = 670
-    _INSTRUMENTMETADATA._serialized_end = 710
-    _INSTRUMENT._serialized_start = 713
-    _INSTRUMENT._serialized_end = 886
-    _LOGNORMALRISKMODEL._serialized_start = 889
-    _LOGNORMALRISKMODEL._serialized_end = 1035
-    _LOGNORMALMODELPARAMS._serialized_start = 1037
-    _LOGNORMALMODELPARAMS._serialized_end = 1111
-    _SIMPLERISKMODEL._serialized_start = 1113
-    _SIMPLERISKMODEL._serialized_end = 1179
-    _SIMPLEMODELPARAMS._serialized_start = 1182
-    _SIMPLEMODELPARAMS._serialized_end = 1391
-    _SCALINGFACTORS._serialized_start = 1394
-    _SCALINGFACTORS._serialized_end = 1531
-    _MARGINCALCULATOR._serialized_start = 1533
-    _MARGINCALCULATOR._serialized_end = 1614
-    _TRADABLEINSTRUMENT._serialized_start = 1617
-    _TRADABLEINSTRUMENT._serialized_end = 1918
-    _FEEFACTORS._serialized_start = 1920
-    _FEEFACTORS._serialized_end = 2045
-    _FEES._serialized_start = 2047
-    _FEES._serialized_end = 2097
-    _PRICEMONITORINGTRIGGER._serialized_start = 2100
-    _PRICEMONITORINGTRIGGER._serialized_end = 2229
-    _PRICEMONITORINGPARAMETERS._serialized_start = 2231
-    _PRICEMONITORINGPARAMETERS._serialized_end = 2316
-    _PRICEMONITORINGSETTINGS._serialized_start = 2318
-    _PRICEMONITORINGSETTINGS._serialized_end = 2408
-    _LIQUIDITYMONITORINGPARAMETERS._serialized_start = 2411
-    _LIQUIDITYMONITORINGPARAMETERS._serialized_end = 2615
-    _TARGETSTAKEPARAMETERS._serialized_start = 2617
-    _TARGETSTAKEPARAMETERS._serialized_end = 2712
-    _MARKET._serialized_start = 2715
-    _MARKET._serialized_end = 3955
-    _MARKET_STATE._serialized_start = 3532
-    _MARKET_STATE._serialized_end = 3748
-    _MARKET_TRADINGMODE._serialized_start = 3751
-    _MARKET_TRADINGMODE._serialized_end = 3955
-    _MARKETTIMESTAMPS._serialized_start = 3957
-    _MARKETTIMESTAMPS._serialized_end = 4071
+    _globals["_AUCTIONDURATION"]._serialized_start = 52
+    _globals["_AUCTIONDURATION"]._serialized_end = 121
+    _globals["_SPOT"]._serialized_start = 123
+    _globals["_SPOT"]._serialized_end = 213
+    _globals["_FUTURE"]._serialized_start = 216
+    _globals["_FUTURE"]._serialized_end = 602
+    _globals["_DATASOURCESPECTOFUTUREBINDING"]._serialized_start = 605
+    _globals["_DATASOURCESPECTOFUTUREBINDING"]._serialized_end = 760
+    _globals["_INSTRUMENTMETADATA"]._serialized_start = 762
+    _globals["_INSTRUMENTMETADATA"]._serialized_end = 802
+    _globals["_INSTRUMENT"]._serialized_start = 805
+    _globals["_INSTRUMENT"]._serialized_end = 1012
+    _globals["_LOGNORMALRISKMODEL"]._serialized_start = 1015
+    _globals["_LOGNORMALRISKMODEL"]._serialized_end = 1161
+    _globals["_LOGNORMALMODELPARAMS"]._serialized_start = 1163
+    _globals["_LOGNORMALMODELPARAMS"]._serialized_end = 1237
+    _globals["_SIMPLERISKMODEL"]._serialized_start = 1239
+    _globals["_SIMPLERISKMODEL"]._serialized_end = 1305
+    _globals["_SIMPLEMODELPARAMS"]._serialized_start = 1308
+    _globals["_SIMPLEMODELPARAMS"]._serialized_end = 1517
+    _globals["_SCALINGFACTORS"]._serialized_start = 1520
+    _globals["_SCALINGFACTORS"]._serialized_end = 1657
+    _globals["_MARGINCALCULATOR"]._serialized_start = 1659
+    _globals["_MARGINCALCULATOR"]._serialized_end = 1740
+    _globals["_TRADABLEINSTRUMENT"]._serialized_start = 1743
+    _globals["_TRADABLEINSTRUMENT"]._serialized_end = 2044
+    _globals["_FEEFACTORS"]._serialized_start = 2046
+    _globals["_FEEFACTORS"]._serialized_end = 2171
+    _globals["_FEES"]._serialized_start = 2173
+    _globals["_FEES"]._serialized_end = 2223
+    _globals["_PRICEMONITORINGTRIGGER"]._serialized_start = 2226
+    _globals["_PRICEMONITORINGTRIGGER"]._serialized_end = 2355
+    _globals["_PRICEMONITORINGPARAMETERS"]._serialized_start = 2357
+    _globals["_PRICEMONITORINGPARAMETERS"]._serialized_end = 2442
+    _globals["_PRICEMONITORINGSETTINGS"]._serialized_start = 2444
+    _globals["_PRICEMONITORINGSETTINGS"]._serialized_end = 2534
+    _globals["_LIQUIDITYMONITORINGPARAMETERS"]._serialized_start = 2537
+    _globals["_LIQUIDITYMONITORINGPARAMETERS"]._serialized_end = 2741
+    _globals["_TARGETSTAKEPARAMETERS"]._serialized_start = 2743
+    _globals["_TARGETSTAKEPARAMETERS"]._serialized_end = 2838
+    _globals["_MARKET"]._serialized_start = 2841
+    _globals["_MARKET"]._serialized_end = 4315
+    _globals["_MARKET_STATE"]._serialized_start = 3819
+    _globals["_MARKET_STATE"]._serialized_end = 4035
+    _globals["_MARKET_TRADINGMODE"]._serialized_start = 4038
+    _globals["_MARKET_TRADINGMODE"]._serialized_end = 4242
+    _globals["_MARKETTIMESTAMPS"]._serialized_start = 4317
+    _globals["_MARKETTIMESTAMPS"]._serialized_end = 4431
 # @@protoc_insertion_point(module_scope)
```

### Comparing `vega_sim-1.1.1/vega_sim/proto/vega/oracle_pb2.py` & `vega_sim-1.2.0/vega_sim/proto/vega/commands/v1/data_pb2.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: vega/oracle.proto
+# source: vega/commands/v1/data.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from .data.v1 import data_pb2 as vega_dot_data_dot_v1_dot_data__pb2
-from . import data_source_pb2 as vega_dot_data__source__pb2
-
-
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x11vega/oracle.proto\x12\x04vega\x1a\x17vega/data/v1/data.proto\x1a\x16vega/data_source.proto"e\n\nOracleSpec\x12W\n\x19\x65xternal_data_source_spec\x18\x01 \x01(\x0b\x32\x1c.vega.ExternalDataSourceSpecR\x16\x65xternalDataSourceSpec"M\n\nOracleData\x12?\n\rexternal_data\x18\x01 \x01(\x0b\x32\x1a.vega.data.v1.ExternalDataR\x0c\x65xternalDataB\'Z%code.vegaprotocol.io/vega/protos/vegab\x06proto3'
+    b'\n\x1bvega/commands/v1/data.proto\x12\x10vega.commands.v1"\xe3\x01\n\x14OracleDataSubmission\x12K\n\x06source\x18\x01 \x01(\x0e\x32\x33.vega.commands.v1.OracleDataSubmission.OracleSourceR\x06source\x12\x18\n\x07payload\x18\x02 \x01(\x0cR\x07payload"d\n\x0cOracleSource\x12\x1d\n\x19ORACLE_SOURCE_UNSPECIFIED\x10\x00\x12\x1d\n\x19ORACLE_SOURCE_OPEN_ORACLE\x10\x01\x12\x16\n\x12ORACLE_SOURCE_JSON\x10\x02\x42\x33Z1code.vegaprotocol.io/vega/protos/vega/commands/v1b\x06proto3'
 )
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "vega.oracle_pb2", globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(
+    DESCRIPTOR, "vega.commands.v1.data_pb2", _globals
+)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    DESCRIPTOR._serialized_options = b"Z%code.vegaprotocol.io/vega/protos/vega"
-    _ORACLESPEC._serialized_start = 76
-    _ORACLESPEC._serialized_end = 177
-    _ORACLEDATA._serialized_start = 179
-    _ORACLEDATA._serialized_end = 256
+    DESCRIPTOR._serialized_options = (
+        b"Z1code.vegaprotocol.io/vega/protos/vega/commands/v1"
+    )
+    _globals["_ORACLEDATASUBMISSION"]._serialized_start = 50
+    _globals["_ORACLEDATASUBMISSION"]._serialized_end = 277
+    _globals["_ORACLEDATASUBMISSION_ORACLESOURCE"]._serialized_start = 177
+    _globals["_ORACLEDATASUBMISSION_ORACLESOURCE"]._serialized_end = 277
 # @@protoc_insertion_point(module_scope)
```

### Comparing `vega_sim-1.1.1/vega_sim/proto/vega/vega_pb2.py` & `vega_sim-1.2.0/vega_sim/proto/vega/vega_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,187 +1,198 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: vega/vega.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from . import markets_pb2 as vega_dot_markets__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x0fvega/vega.proto\x12\x04vega\x1a\x12vega/markets.proto"\x17\n\x05Party\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id"N\n\nRiskFactor\x12\x16\n\x06market\x18\x01 \x01(\tR\x06market\x12\x14\n\x05short\x18\x02 \x01(\tR\x05short\x12\x12\n\x04long\x18\x03 \x01(\tR\x04long"Z\n\x0bPeggedOrder\x12\x33\n\treference\x18\x01 \x01(\x0e\x32\x15.vega.PeggedReferenceR\treference\x12\x16\n\x06offset\x18\x02 \x01(\tR\x06offset"\xb0\t\n\x05Order\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x03 \x01(\tR\x07partyId\x12\x1e\n\x04side\x18\x04 \x01(\x0e\x32\n.vega.SideR\x04side\x12\x14\n\x05price\x18\x05 \x01(\tR\x05price\x12\x12\n\x04size\x18\x06 \x01(\x04R\x04size\x12\x1c\n\tremaining\x18\x07 \x01(\x04R\tremaining\x12;\n\rtime_in_force\x18\x08 \x01(\x0e\x32\x17.vega.Order.TimeInForceR\x0btimeInForce\x12$\n\x04type\x18\t \x01(\x0e\x32\x10.vega.Order.TypeR\x04type\x12\x1d\n\ncreated_at\x18\n \x01(\x03R\tcreatedAt\x12*\n\x06status\x18\x0b \x01(\x0e\x32\x12.vega.Order.StatusR\x06status\x12\x1d\n\nexpires_at\x18\x0c \x01(\x03R\texpiresAt\x12\x1c\n\treference\x18\r \x01(\tR\treference\x12-\n\x06reason\x18\x0e \x01(\x0e\x32\x10.vega.OrderErrorH\x00R\x06reason\x88\x01\x01\x12\x1d\n\nupdated_at\x18\x0f \x01(\x03R\tupdatedAt\x12\x18\n\x07version\x18\x10 \x01(\x04R\x07version\x12\x19\n\x08\x62\x61tch_id\x18\x11 \x01(\x04R\x07\x62\x61tchId\x12\x34\n\x0cpegged_order\x18\x12 \x01(\x0b\x32\x11.vega.PeggedOrderR\x0bpeggedOrder\x12\x34\n\x16liquidity_provision_id\x18\x13 \x01(\tR\x14liquidityProvisionId\x12\x1b\n\tpost_only\x18\x14 \x01(\x08R\x08postOnly\x12\x1f\n\x0breduce_only\x18\x15 \x01(\x08R\nreduceOnly"\xb6\x01\n\x0bTimeInForce\x12\x1d\n\x19TIME_IN_FORCE_UNSPECIFIED\x10\x00\x12\x15\n\x11TIME_IN_FORCE_GTC\x10\x01\x12\x15\n\x11TIME_IN_FORCE_GTT\x10\x02\x12\x15\n\x11TIME_IN_FORCE_IOC\x10\x03\x12\x15\n\x11TIME_IN_FORCE_FOK\x10\x04\x12\x15\n\x11TIME_IN_FORCE_GFA\x10\x05\x12\x15\n\x11TIME_IN_FORCE_GFN\x10\x06"O\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x0e\n\nTYPE_LIMIT\x10\x01\x12\x0f\n\x0bTYPE_MARKET\x10\x02\x12\x10\n\x0cTYPE_NETWORK\x10\x03"\xc9\x01\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x11\n\rSTATUS_ACTIVE\x10\x01\x12\x12\n\x0eSTATUS_EXPIRED\x10\x02\x12\x14\n\x10STATUS_CANCELLED\x10\x03\x12\x12\n\x0eSTATUS_STOPPED\x10\x04\x12\x11\n\rSTATUS_FILLED\x10\x05\x12\x13\n\x0fSTATUS_REJECTED\x10\x06\x12\x1b\n\x17STATUS_PARTIALLY_FILLED\x10\x07\x12\x11\n\rSTATUS_PARKED\x10\x08\x42\t\n\x07_reason"B\n\x1dOrderCancellationConfirmation\x12!\n\x05order\x18\x01 \x01(\x0b\x32\x0b.vega.OrderR\x05order"\xa0\x01\n\x11OrderConfirmation\x12!\n\x05order\x18\x01 \x01(\x0b\x32\x0b.vega.OrderR\x05order\x12#\n\x06trades\x18\x02 \x03(\x0b\x32\x0b.vega.TradeR\x06trades\x12\x43\n\x17passive_orders_affected\x18\x03 \x03(\x0b\x32\x0b.vega.OrderR\x15passiveOrdersAffected"\xd3\x01\n\x16\x41uctionIndicativeState\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12)\n\x10indicative_price\x18\x02 \x01(\tR\x0findicativePrice\x12+\n\x11indicative_volume\x18\x03 \x01(\x04R\x10indicativeVolume\x12#\n\rauction_start\x18\x04 \x01(\x03R\x0c\x61uctionStart\x12\x1f\n\x0b\x61uction_end\x18\x05 \x01(\x03R\nauctionEnd"\xdb\x04\n\x05Trade\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12\x14\n\x05price\x18\x03 \x01(\tR\x05price\x12\x12\n\x04size\x18\x04 \x01(\x04R\x04size\x12\x14\n\x05\x62uyer\x18\x05 \x01(\tR\x05\x62uyer\x12\x16\n\x06seller\x18\x06 \x01(\tR\x06seller\x12(\n\taggressor\x18\x07 \x01(\x0e\x32\n.vega.SideR\taggressor\x12\x1b\n\tbuy_order\x18\x08 \x01(\tR\x08\x62uyOrder\x12\x1d\n\nsell_order\x18\t \x01(\tR\tsellOrder\x12\x1c\n\ttimestamp\x18\n \x01(\x03R\ttimestamp\x12$\n\x04type\x18\x0b \x01(\x0e\x32\x10.vega.Trade.TypeR\x04type\x12&\n\tbuyer_fee\x18\x0c \x01(\x0b\x32\t.vega.FeeR\x08\x62uyerFee\x12(\n\nseller_fee\x18\r \x01(\x0b\x32\t.vega.FeeR\tsellerFee\x12.\n\x13\x62uyer_auction_batch\x18\x0e \x01(\x04R\x11\x62uyerAuctionBatch\x12\x30\n\x14seller_auction_batch\x18\x0f \x01(\x04R\x12sellerAuctionBatch"o\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x10\n\x0cTYPE_DEFAULT\x10\x01\x12\x1f\n\x1bTYPE_NETWORK_CLOSE_OUT_GOOD\x10\x02\x12\x1e\n\x1aTYPE_NETWORK_CLOSE_OUT_BAD\x10\x03"v\n\x03\x46\x65\x65\x12\x1b\n\tmaker_fee\x18\x01 \x01(\tR\x08makerFee\x12-\n\x12infrastructure_fee\x18\x02 \x01(\tR\x11infrastructureFee\x12#\n\rliquidity_fee\x18\x03 \x01(\tR\x0cliquidityFee"/\n\x08TradeSet\x12#\n\x06trades\x18\x01 \x03(\x0b\x32\x0b.vega.TradeR\x06trades"\xd6\x01\n\x06\x43\x61ndle\x12\x1c\n\ttimestamp\x18\x01 \x01(\x03R\ttimestamp\x12\x1a\n\x08\x64\x61tetime\x18\x02 \x01(\tR\x08\x64\x61tetime\x12\x12\n\x04high\x18\x03 \x01(\tR\x04high\x12\x10\n\x03low\x18\x04 \x01(\tR\x03low\x12\x12\n\x04open\x18\x05 \x01(\tR\x04open\x12\x14\n\x05\x63lose\x18\x06 \x01(\tR\x05\x63lose\x12\x16\n\x06volume\x18\x07 \x01(\x04R\x06volume\x12*\n\x08interval\x18\x08 \x01(\x0e\x32\x0e.vega.IntervalR\x08interval"d\n\nPriceLevel\x12\x14\n\x05price\x18\x01 \x01(\tR\x05price\x12(\n\x10number_of_orders\x18\x02 \x01(\x04R\x0enumberOfOrders\x12\x16\n\x06volume\x18\x03 \x01(\x04R\x06volume"\x9d\x01\n\x0bMarketDepth\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12"\n\x03\x62uy\x18\x02 \x03(\x0b\x32\x10.vega.PriceLevelR\x03\x62uy\x12$\n\x04sell\x18\x03 \x03(\x0b\x32\x10.vega.PriceLevelR\x04sell\x12\'\n\x0fsequence_number\x18\x04 \x01(\x04R\x0esequenceNumber"\xdd\x01\n\x11MarketDepthUpdate\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12"\n\x03\x62uy\x18\x02 \x03(\x0b\x32\x10.vega.PriceLevelR\x03\x62uy\x12$\n\x04sell\x18\x03 \x03(\x0b\x32\x10.vega.PriceLevelR\x04sell\x12\'\n\x0fsequence_number\x18\x04 \x01(\x04R\x0esequenceNumber\x12\x38\n\x18previous_sequence_number\x18\x05 \x01(\x04R\x16previousSequenceNumber"\xf7\x02\n\x08Position\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x1f\n\x0bopen_volume\x18\x03 \x01(\x03R\nopenVolume\x12!\n\x0crealised_pnl\x18\x04 \x01(\tR\x0brealisedPnl\x12%\n\x0eunrealised_pnl\x18\x05 \x01(\tR\runrealisedPnl\x12.\n\x13\x61verage_entry_price\x18\x06 \x01(\tR\x11\x61verageEntryPrice\x12\x1d\n\nupdated_at\x18\x07 \x01(\x03R\tupdatedAt\x12:\n\x19loss_socialisation_amount\x18\x08 \x01(\tR\x17lossSocialisationAmount\x12=\n\x0fposition_status\x18\t \x01(\x0e\x32\x14.vega.PositionStatusR\x0epositionStatus"=\n\rPositionTrade\x12\x16\n\x06volume\x18\x01 \x01(\x03R\x06volume\x12\x14\n\x05price\x18\x02 \x01(\tR\x05price"\xe4\x02\n\x07\x44\x65posit\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12,\n\x06status\x18\x02 \x01(\x0e\x32\x14.vega.Deposit.StatusR\x06status\x12\x19\n\x08party_id\x18\x03 \x01(\tR\x07partyId\x12\x14\n\x05\x61sset\x18\x04 \x01(\tR\x05\x61sset\x12\x16\n\x06\x61mount\x18\x05 \x01(\tR\x06\x61mount\x12\x17\n\x07tx_hash\x18\x06 \x01(\tR\x06txHash\x12-\n\x12\x63redited_timestamp\x18\x07 \x01(\x03R\x11\x63reditedTimestamp\x12+\n\x11\x63reated_timestamp\x18\x08 \x01(\x03R\x10\x63reatedTimestamp"]\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x0f\n\x0bSTATUS_OPEN\x10\x01\x12\x14\n\x10STATUS_CANCELLED\x10\x02\x12\x14\n\x10STATUS_FINALIZED\x10\x03"\xa8\x03\n\nWithdrawal\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount\x12\x14\n\x05\x61sset\x18\x04 \x01(\tR\x05\x61sset\x12/\n\x06status\x18\x05 \x01(\x0e\x32\x17.vega.Withdrawal.StatusR\x06status\x12\x10\n\x03ref\x18\x06 \x01(\tR\x03ref\x12\x17\n\x07tx_hash\x18\x08 \x01(\tR\x06txHash\x12+\n\x11\x63reated_timestamp\x18\t \x01(\x03R\x10\x63reatedTimestamp\x12/\n\x13withdrawn_timestamp\x18\n \x01(\x03R\x12withdrawnTimestamp\x12#\n\x03\x65xt\x18\x0b \x01(\x0b\x32\x11.vega.WithdrawExtR\x03\x65xt"\\\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x0f\n\x0bSTATUS_OPEN\x10\x01\x12\x13\n\x0fSTATUS_REJECTED\x10\x02\x12\x14\n\x10STATUS_FINALIZED\x10\x03J\x04\x08\x07\x10\x08"D\n\x0bWithdrawExt\x12.\n\x05\x65rc20\x18\x01 \x01(\x0b\x32\x16.vega.Erc20WithdrawExtH\x00R\x05\x65rc20B\x05\n\x03\x65xt"=\n\x10\x45rc20WithdrawExt\x12)\n\x10receiver_address\x18\x01 \x01(\tR\x0freceiverAddress"\xa3\x01\n\x07\x41\x63\x63ount\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x14\n\x05owner\x18\x02 \x01(\tR\x05owner\x12\x18\n\x07\x62\x61lance\x18\x03 \x01(\tR\x07\x62\x61lance\x12\x14\n\x05\x61sset\x18\x04 \x01(\tR\x05\x61sset\x12\x1b\n\tmarket_id\x18\x05 \x01(\tR\x08marketId\x12%\n\x04type\x18\x06 \x01(\x0e\x32\x11.vega.AccountTypeR\x04type"?\n\x0f\x46inancialAmount\x12\x16\n\x06\x61mount\x18\x01 \x01(\tR\x06\x61mount\x12\x14\n\x05\x61sset\x18\x02 \x01(\tR\x05\x61sset"\xb3\x01\n\x08Transfer\x12\x14\n\x05owner\x18\x01 \x01(\tR\x05owner\x12-\n\x06\x61mount\x18\x02 \x01(\x0b\x32\x15.vega.FinancialAmountR\x06\x61mount\x12&\n\x04type\x18\x03 \x01(\x0e\x32\x12.vega.TransferTypeR\x04type\x12\x1d\n\nmin_amount\x18\x04 \x01(\tR\tminAmount\x12\x1b\n\tmarket_id\x18\x05 \x01(\tR\x08marketId"\x84\x01\n\x10\x44ispatchStrategy\x12(\n\x10\x61sset_for_metric\x18\x01 \x01(\tR\x0e\x61ssetForMetric\x12,\n\x06metric\x18\x02 \x01(\x0e\x32\x14.vega.DispatchMetricR\x06metric\x12\x18\n\x07markets\x18\x03 \x03(\tR\x07markets"\xe6\x01\n\x0fTransferRequest\x12\x30\n\x0c\x66rom_account\x18\x01 \x03(\x0b\x32\r.vega.AccountR\x0b\x66romAccount\x12,\n\nto_account\x18\x02 \x03(\x0b\x32\r.vega.AccountR\ttoAccount\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount\x12\x1d\n\nmin_amount\x18\x04 \x01(\tR\tminAmount\x12\x14\n\x05\x61sset\x18\x05 \x01(\tR\x05\x61sset\x12&\n\x04type\x18\x07 \x01(\x0e\x32\x12.vega.TransferTypeR\x04type"\xa7\x01\n\x0e\x41\x63\x63ountDetails\x12\x19\n\x08\x61sset_id\x18\x01 \x01(\tR\x07\x61ssetId\x12%\n\x04type\x18\x02 \x01(\x0e\x32\x11.vega.AccountTypeR\x04type\x12\x19\n\x05owner\x18\x03 \x01(\tH\x00R\x05owner\x88\x01\x01\x12 \n\tmarket_id\x18\x04 \x01(\tH\x01R\x08marketId\x88\x01\x01\x42\x08\n\x06_ownerB\x0c\n\n_market_id"\xb9\x02\n\x0bLedgerEntry\x12\x37\n\x0c\x66rom_account\x18\x01 \x01(\x0b\x32\x14.vega.AccountDetailsR\x0b\x66romAccount\x12\x33\n\nto_account\x18\x02 \x01(\x0b\x32\x14.vega.AccountDetailsR\ttoAccount\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount\x12&\n\x04type\x18\x04 \x01(\x0e\x32\x12.vega.TransferTypeR\x04type\x12\x1c\n\ttimestamp\x18\x05 \x01(\x03R\ttimestamp\x12\x30\n\x14\x66rom_account_balance\x18\x06 \x01(\tR\x12\x66romAccountBalance\x12,\n\x12to_account_balance\x18\x07 \x01(\tR\x10toAccountBalance"_\n\x13PostTransferBalance\x12.\n\x07\x61\x63\x63ount\x18\x01 \x01(\x0b\x32\x14.vega.AccountDetailsR\x07\x61\x63\x63ount\x12\x18\n\x07\x62\x61lance\x18\x02 \x01(\tR\x07\x62\x61lance"t\n\x0eLedgerMovement\x12+\n\x07\x65ntries\x18\x01 \x03(\x0b\x32\x11.vega.LedgerEntryR\x07\x65ntries\x12\x35\n\x08\x62\x61lances\x18\x02 \x03(\x0b\x32\x19.vega.PostTransferBalanceR\x08\x62\x61lances"\xad\x02\n\x0cMarginLevels\x12-\n\x12maintenance_margin\x18\x01 \x01(\tR\x11maintenanceMargin\x12!\n\x0csearch_level\x18\x02 \x01(\tR\x0bsearchLevel\x12%\n\x0einitial_margin\x18\x03 \x01(\tR\rinitialMargin\x12\x38\n\x18\x63ollateral_release_level\x18\x04 \x01(\tR\x16\x63ollateralReleaseLevel\x12\x19\n\x08party_id\x18\x05 \x01(\tR\x07partyId\x12\x1b\n\tmarket_id\x18\x06 \x01(\tR\x08marketId\x12\x14\n\x05\x61sset\x18\x07 \x01(\tR\x05\x61sset\x12\x1c\n\ttimestamp\x18\x08 \x01(\x03R\ttimestamp"\xe5\n\n\nMarketData\x12\x1d\n\nmark_price\x18\x01 \x01(\tR\tmarkPrice\x12$\n\x0e\x62\x65st_bid_price\x18\x02 \x01(\tR\x0c\x62\x65stBidPrice\x12&\n\x0f\x62\x65st_bid_volume\x18\x03 \x01(\x04R\rbestBidVolume\x12(\n\x10\x62\x65st_offer_price\x18\x04 \x01(\tR\x0e\x62\x65stOfferPrice\x12*\n\x11\x62\x65st_offer_volume\x18\x05 \x01(\x04R\x0f\x62\x65stOfferVolume\x12\x31\n\x15\x62\x65st_static_bid_price\x18\x06 \x01(\tR\x12\x62\x65stStaticBidPrice\x12\x33\n\x16\x62\x65st_static_bid_volume\x18\x07 \x01(\x04R\x13\x62\x65stStaticBidVolume\x12\x35\n\x17\x62\x65st_static_offer_price\x18\x08 \x01(\tR\x14\x62\x65stStaticOfferPrice\x12\x37\n\x18\x62\x65st_static_offer_volume\x18\t \x01(\x04R\x15\x62\x65stStaticOfferVolume\x12\x1b\n\tmid_price\x18\n \x01(\tR\x08midPrice\x12(\n\x10static_mid_price\x18\x0b \x01(\tR\x0estaticMidPrice\x12\x16\n\x06market\x18\x0c \x01(\tR\x06market\x12\x1c\n\ttimestamp\x18\r \x01(\x03R\ttimestamp\x12#\n\ropen_interest\x18\x0e \x01(\x04R\x0copenInterest\x12\x1f\n\x0b\x61uction_end\x18\x0f \x01(\x03R\nauctionEnd\x12#\n\rauction_start\x18\x10 \x01(\x03R\x0c\x61uctionStart\x12)\n\x10indicative_price\x18\x11 \x01(\tR\x0findicativePrice\x12+\n\x11indicative_volume\x18\x12 \x01(\x04R\x10indicativeVolume\x12H\n\x13market_trading_mode\x18\x13 \x01(\x0e\x32\x18.vega.Market.TradingModeR\x11marketTradingMode\x12.\n\x07trigger\x18\x14 \x01(\x0e\x32\x14.vega.AuctionTriggerR\x07trigger\x12\x41\n\x11\x65xtension_trigger\x18\x15 \x01(\x0e\x32\x14.vega.AuctionTriggerR\x10\x65xtensionTrigger\x12!\n\x0ctarget_stake\x18\x16 \x01(\tR\x0btargetStake\x12%\n\x0esupplied_stake\x18\x17 \x01(\tR\rsuppliedStake\x12S\n\x17price_monitoring_bounds\x18\x18 \x03(\x0b\x32\x1b.vega.PriceMonitoringBoundsR\x15priceMonitoringBounds\x12,\n\x12market_value_proxy\x18\x19 \x01(\tR\x10marketValueProxy\x12`\n\x1cliquidity_provider_fee_share\x18\x1a \x03(\x0b\x32\x1f.vega.LiquidityProviderFeeShareR\x19liquidityProviderFeeShare\x12\x35\n\x0cmarket_state\x18\x1b \x01(\x0e\x32\x12.vega.Market.StateR\x0bmarketState\x12-\n\x13next_mark_to_market\x18\x1c \x01(\x03R\x10nextMarkToMarket\x12*\n\x11last_traded_price\x18\x1d \x01(\tR\x0flastTradedPrice"\xba\x01\n\x19LiquidityProviderFeeShare\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12*\n\x11\x65quity_like_share\x18\x02 \x01(\tR\x0f\x65quityLikeShare\x12\x36\n\x17\x61verage_entry_valuation\x18\x03 \x01(\tR\x15\x61verageEntryValuation\x12#\n\raverage_score\x18\x04 \x01(\tR\x0c\x61verageScore"\xc8\x01\n\x15PriceMonitoringBounds\x12&\n\x0fmin_valid_price\x18\x01 \x01(\tR\rminValidPrice\x12&\n\x0fmax_valid_price\x18\x02 \x01(\tR\rmaxValidPrice\x12\x36\n\x07trigger\x18\x03 \x01(\x0b\x32\x1c.vega.PriceMonitoringTriggerR\x07trigger\x12\'\n\x0freference_price\x18\x04 \x01(\tR\x0ereferencePrice"Q\n\x0b\x45rrorDetail\x12\x12\n\x04\x63ode\x18\x01 \x01(\x05R\x04\x63ode\x12\x18\n\x07message\x18\x02 \x01(\tR\x07message\x12\x14\n\x05inner\x18\x03 \x01(\tR\x05inner":\n\x10NetworkParameter\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value"\x82\x03\n\rNetworkLimits\x12,\n\x12\x63\x61n_propose_market\x18\x01 \x01(\x08R\x10\x63\x61nProposeMarket\x12*\n\x11\x63\x61n_propose_asset\x18\x02 \x01(\x08R\x0f\x63\x61nProposeAsset\x12\x34\n\x16propose_market_enabled\x18\x04 \x01(\x08R\x14proposeMarketEnabled\x12\x32\n\x15propose_asset_enabled\x18\x05 \x01(\x08R\x13proposeAssetEnabled\x12%\n\x0egenesis_loaded\x18\x07 \x01(\x08R\rgenesisLoaded\x12=\n\x1bpropose_market_enabled_from\x18\x08 \x01(\x03R\x18proposeMarketEnabledFrom\x12;\n\x1apropose_asset_enabled_from\x18\t \x01(\x03R\x17proposeAssetEnabledFromJ\x04\x08\x03\x10\x04J\x04\x08\x06\x10\x07"}\n\x0eLiquidityOrder\x12\x33\n\treference\x18\x01 \x01(\x0e\x32\x15.vega.PeggedReferenceR\treference\x12\x1e\n\nproportion\x18\x02 \x01(\rR\nproportion\x12\x16\n\x06offset\x18\x03 \x01(\tR\x06offset"s\n\x17LiquidityOrderReference\x12\x19\n\x08order_id\x18\x01 \x01(\tR\x07orderId\x12=\n\x0fliquidity_order\x18\x02 \x01(\x0b\x32\x14.vega.LiquidityOrderR\x0eliquidityOrder"\xd2\x04\n\x12LiquidityProvision\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x1d\n\ncreated_at\x18\x03 \x01(\x03R\tcreatedAt\x12\x1d\n\nupdated_at\x18\x04 \x01(\x03R\tupdatedAt\x12\x1b\n\tmarket_id\x18\x05 \x01(\tR\x08marketId\x12+\n\x11\x63ommitment_amount\x18\x06 \x01(\tR\x10\x63ommitmentAmount\x12\x10\n\x03\x66\x65\x65\x18\x07 \x01(\tR\x03\x66\x65\x65\x12\x33\n\x05sells\x18\x08 \x03(\x0b\x32\x1d.vega.LiquidityOrderReferenceR\x05sells\x12\x31\n\x04\x62uys\x18\t \x03(\x0b\x32\x1d.vega.LiquidityOrderReferenceR\x04\x62uys\x12\x18\n\x07version\x18\n \x01(\x04R\x07version\x12\x37\n\x06status\x18\x0b \x01(\x0e\x32\x1f.vega.LiquidityProvision.StatusR\x06status\x12\x1c\n\treference\x18\x0c \x01(\tR\treference"\x9d\x01\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x11\n\rSTATUS_ACTIVE\x10\x01\x12\x12\n\x0eSTATUS_STOPPED\x10\x02\x12\x14\n\x10STATUS_CANCELLED\x10\x03\x12\x13\n\x0fSTATUS_REJECTED\x10\x04\x12\x15\n\x11STATUS_UNDEPLOYED\x10\x05\x12\x12\n\x0eSTATUS_PENDING\x10\x06"\xd0\x03\n\x0e\x45thereumConfig\x12\x1d\n\nnetwork_id\x18\x01 \x01(\tR\tnetworkId\x12\x19\n\x08\x63hain_id\x18\x02 \x01(\tR\x07\x63hainId\x12Z\n\x1a\x63ollateral_bridge_contract\x18\x03 \x01(\x0b\x32\x1c.vega.EthereumContractConfigR\x18\x63ollateralBridgeContract\x12$\n\rconfirmations\x18\x04 \x01(\rR\rconfirmations\x12T\n\x17staking_bridge_contract\x18\x05 \x01(\x0b\x32\x1c.vega.EthereumContractConfigR\x15stakingBridgeContract\x12R\n\x16token_vesting_contract\x18\x06 \x01(\x0b\x32\x1c.vega.EthereumContractConfigR\x14tokenVestingContract\x12X\n\x19multisig_control_contract\x18\x07 \x01(\x0b\x32\x1c.vega.EthereumContractConfigR\x17multisigControlContract"j\n\x16\x45thereumContractConfig\x12\x18\n\x07\x61\x64\x64ress\x18\x01 \x01(\tR\x07\x61\x64\x64ress\x12\x36\n\x17\x64\x65ployment_block_height\x18\x06 \x01(\x04R\x15\x64\x65ploymentBlockHeight"\xac\x01\n\x0f\x45pochTimestamps\x12\x1d\n\nstart_time\x18\x01 \x01(\x03R\tstartTime\x12\x1f\n\x0b\x65xpiry_time\x18\x02 \x01(\x03R\nexpiryTime\x12\x19\n\x08\x65nd_time\x18\x03 \x01(\x03R\x07\x65ndTime\x12\x1f\n\x0b\x66irst_block\x18\x04 \x01(\x04R\nfirstBlock\x12\x1d\n\nlast_block\x18\x05 \x01(\x04R\tlastBlock"\xb0\x01\n\x05\x45poch\x12\x10\n\x03seq\x18\x01 \x01(\x04R\x03seq\x12\x35\n\ntimestamps\x18\x02 \x01(\x0b\x32\x15.vega.EpochTimestampsR\ntimestamps\x12*\n\nvalidators\x18\x03 \x03(\x0b\x32\n.vega.NodeR\nvalidators\x12\x32\n\x0b\x64\x65legations\x18\x04 \x03(\x0b\x32\x10.vega.DelegationR\x0b\x64\x65legations"\x8e\x01\n\x12\x45pochParticipation\x12!\n\x05\x65poch\x18\x01 \x01(\x0b\x32\x0b.vega.EpochR\x05\x65poch\x12\x18\n\x07offline\x18\x02 \x01(\x04R\x07offline\x12\x16\n\x06online\x18\x03 \x01(\x04R\x06online\x12#\n\rtotal_rewards\x18\x04 \x01(\x01R\x0ctotalRewards"S\n\tEpochData\x12\x14\n\x05total\x18\x01 \x01(\x05R\x05total\x12\x18\n\x07offline\x18\x02 \x01(\x05R\x07offline\x12\x16\n\x06online\x18\x03 \x01(\x05R\x06online"\x9b\x02\n\x0cRankingScore\x12\x1f\n\x0bstake_score\x18\x01 \x01(\tR\nstakeScore\x12+\n\x11performance_score\x18\x02 \x01(\tR\x10performanceScore\x12\x42\n\x0fprevious_status\x18\x03 \x01(\x0e\x32\x19.vega.ValidatorNodeStatusR\x0epreviousStatus\x12\x31\n\x06status\x18\x04 \x01(\x0e\x32\x19.vega.ValidatorNodeStatusR\x06status\x12!\n\x0cvoting_power\x18\x05 \x01(\rR\x0bvotingPower\x12#\n\rranking_score\x18\x06 \x01(\tR\x0crankingScore"\xab\x02\n\x0bRewardScore\x12.\n\x13raw_validator_score\x18\x01 \x01(\tR\x11rawValidatorScore\x12+\n\x11performance_score\x18\x02 \x01(\tR\x10performanceScore\x12%\n\x0emultisig_score\x18\x03 \x01(\tR\rmultisigScore\x12\'\n\x0fvalidator_score\x18\x04 \x01(\tR\x0evalidatorScore\x12)\n\x10normalised_score\x18\x05 \x01(\tR\x0fnormalisedScore\x12\x44\n\x10validator_status\x18\x06 \x01(\x0e\x32\x19.vega.ValidatorNodeStatusR\x0fvalidatorStatus"\xb3\x05\n\x04Node\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x17\n\x07pub_key\x18\x02 \x01(\tR\x06pubKey\x12\x1c\n\ntm_pub_key\x18\x03 \x01(\tR\x08tmPubKey\x12)\n\x10\x65thereum_address\x18\x04 \x01(\tR\x0f\x65thereumAddress\x12\x19\n\x08info_url\x18\x05 \x01(\tR\x07infoUrl\x12\x1a\n\x08location\x18\x06 \x01(\tR\x08location\x12,\n\x12staked_by_operator\x18\x07 \x01(\tR\x10stakedByOperator\x12.\n\x13staked_by_delegates\x18\x08 \x01(\tR\x11stakedByDelegates\x12!\n\x0cstaked_total\x18\t \x01(\tR\x0bstakedTotal\x12,\n\x12max_intended_stake\x18\n \x01(\tR\x10maxIntendedStake\x12#\n\rpending_stake\x18\x0b \x01(\tR\x0cpendingStake\x12.\n\nepoch_data\x18\x0c \x01(\x0b\x32\x0f.vega.EpochDataR\tepochData\x12(\n\x06status\x18\r \x01(\x0e\x32\x10.vega.NodeStatusR\x06status\x12\x32\n\x0b\x64\x65legations\x18\x0e \x03(\x0b\x32\x10.vega.DelegationR\x0b\x64\x65legations\x12\x34\n\x0creward_score\x18\x0f \x01(\x0b\x32\x11.vega.RewardScoreR\x0brewardScore\x12\x37\n\rranking_score\x18\x10 \x01(\x0b\x32\x12.vega.RankingScoreR\x0crankingScore\x12\x12\n\x04name\x18\x11 \x01(\tR\x04name\x12\x1d\n\navatar_url\x18\x12 \x01(\tR\tavatarUrl"\x9c\x01\n\x07NodeSet\x12\x14\n\x05total\x18\x01 \x01(\rR\x05total\x12\x1a\n\x08inactive\x18\x02 \x01(\rR\x08inactive\x12\x1a\n\x08promoted\x18\x03 \x03(\tR\x08promoted\x12\x18\n\x07\x64\x65moted\x18\x04 \x03(\tR\x07\x64\x65moted\x12\x1d\n\x07maximum\x18\x05 \x01(\rH\x00R\x07maximum\x88\x01\x01\x42\n\n\x08_maximum"\xad\x02\n\x08NodeData\x12!\n\x0cstaked_total\x18\x01 \x01(\tR\x0bstakedTotal\x12\x1f\n\x0btotal_nodes\x18\x02 \x01(\rR\ntotalNodes\x12%\n\x0einactive_nodes\x18\x03 \x01(\rR\rinactiveNodes\x12\x38\n\x10tendermint_nodes\x18\x04 \x01(\x0b\x32\r.vega.NodeSetR\x0ftendermintNodes\x12\x30\n\x0c\x65rsatz_nodes\x18\x05 \x01(\x0b\x32\r.vega.NodeSetR\x0b\x65rsatzNodes\x12\x32\n\rpending_nodes\x18\x06 \x01(\x0b\x32\r.vega.NodeSetR\x0cpendingNodes\x12\x16\n\x06uptime\x18\x07 \x01(\x02R\x06uptime"p\n\nDelegation\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x17\n\x07node_id\x18\x02 \x01(\tR\x06nodeId\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount\x12\x1b\n\tepoch_seq\x18\x04 \x01(\tR\x08\x65pochSeq"\xfb\x01\n\x06Reward\x12\x19\n\x08\x61sset_id\x18\x01 \x01(\tR\x07\x61ssetId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x14\n\x05\x65poch\x18\x03 \x01(\x04R\x05\x65poch\x12\x16\n\x06\x61mount\x18\x04 \x01(\tR\x06\x61mount\x12.\n\x13percentage_of_total\x18\x05 \x01(\tR\x11percentageOfTotal\x12\x1f\n\x0breceived_at\x18\x06 \x01(\x03R\nreceivedAt\x12\x1b\n\tmarket_id\x18\x07 \x01(\tR\x08marketId\x12\x1f\n\x0breward_type\x18\x08 \x01(\tR\nrewardType"]\n\rRewardSummary\x12\x19\n\x08\x61sset_id\x18\x01 \x01(\tR\x07\x61ssetId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount"\x9b\x01\n\x12\x45pochRewardSummary\x12\x14\n\x05\x65poch\x18\x01 \x01(\x04R\x05\x65poch\x12\x19\n\x08\x61sset_id\x18\x02 \x01(\tR\x07\x61ssetId\x12\x1b\n\tmarket_id\x18\x03 \x01(\tR\x08marketId\x12\x1f\n\x0breward_type\x18\x04 \x01(\tR\nrewardType\x12\x16\n\x06\x61mount\x18\x05 \x01(\tR\x06\x61mount"y\n\x12StateValueProposal\x12 \n\x0cstate_var_id\x18\x01 \x01(\tR\nstateVarId\x12\x19\n\x08\x65vent_id\x18\x02 \x01(\tR\x07\x65ventId\x12&\n\x03kvb\x18\x03 \x03(\x0b\x32\x14.vega.KeyValueBundleR\x03kvb"k\n\x0eKeyValueBundle\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x1c\n\ttolerance\x18\x02 \x01(\tR\ttolerance\x12)\n\x05value\x18\x03 \x01(\x0b\x32\x13.vega.StateVarValueR\x05value"\xb4\x01\n\rStateVarValue\x12\x32\n\nscalar_val\x18\x01 \x01(\x0b\x32\x11.vega.ScalarValueH\x00R\tscalarVal\x12\x32\n\nvector_val\x18\x02 \x01(\x0b\x32\x11.vega.VectorValueH\x00R\tvectorVal\x12\x32\n\nmatrix_val\x18\x03 \x01(\x0b\x32\x11.vega.MatrixValueH\x00R\tmatrixValB\x07\n\x05value"#\n\x0bScalarValue\x12\x14\n\x05value\x18\x01 \x01(\tR\x05value"#\n\x0bVectorValue\x12\x14\n\x05value\x18\x01 \x03(\tR\x05value"6\n\x0bMatrixValue\x12\'\n\x05value\x18\x01 \x03(\x0b\x32\x11.vega.VectorValueR\x05value*9\n\x04Side\x12\x14\n\x10SIDE_UNSPECIFIED\x10\x00\x12\x0c\n\x08SIDE_BUY\x10\x01\x12\r\n\tSIDE_SELL\x10\x02*\xb5\x01\n\x08Interval\x12\x18\n\x14INTERVAL_UNSPECIFIED\x10\x00\x12\x1b\n\x0eINTERVAL_BLOCK\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x10\n\x0cINTERVAL_I1M\x10<\x12\x11\n\x0cINTERVAL_I5M\x10\xac\x02\x12\x12\n\rINTERVAL_I15M\x10\x84\x07\x12\x11\n\x0cINTERVAL_I1H\x10\x90\x1c\x12\x12\n\x0cINTERVAL_I6H\x10\xe0\xa8\x01\x12\x12\n\x0cINTERVAL_I1D\x10\x80\xa3\x05*\x94\x01\n\x0ePositionStatus\x12\x1f\n\x1bPOSITION_STATUS_UNSPECIFIED\x10\x00\x12!\n\x1dPOSITION_STATUS_ORDERS_CLOSED\x10\x01\x12\x1e\n\x1aPOSITION_STATUS_CLOSED_OUT\x10\x02\x12\x1e\n\x1aPOSITION_STATUS_DISTRESSED\x10\x04*\x81\x02\n\x0e\x41uctionTrigger\x12\x1f\n\x1b\x41UCTION_TRIGGER_UNSPECIFIED\x10\x00\x12\x19\n\x15\x41UCTION_TRIGGER_BATCH\x10\x01\x12\x1b\n\x17\x41UCTION_TRIGGER_OPENING\x10\x02\x12\x19\n\x15\x41UCTION_TRIGGER_PRICE\x10\x03\x12\x1d\n\x19\x41UCTION_TRIGGER_LIQUIDITY\x10\x04\x12,\n(AUCTION_TRIGGER_LIQUIDITY_TARGET_NOT_MET\x10\x05\x12.\n*AUCTION_TRIGGER_UNABLE_TO_DEPLOY_LP_ORDERS\x10\x06*\x8b\x01\n\x0fPeggedReference\x12 \n\x1cPEGGED_REFERENCE_UNSPECIFIED\x10\x00\x12\x18\n\x14PEGGED_REFERENCE_MID\x10\x01\x12\x1d\n\x19PEGGED_REFERENCE_BEST_BID\x10\x02\x12\x1d\n\x19PEGGED_REFERENCE_BEST_ASK\x10\x03*\xc9\x10\n\nOrderError\x12\x1b\n\x17ORDER_ERROR_UNSPECIFIED\x10\x00\x12!\n\x1dORDER_ERROR_INVALID_MARKET_ID\x10\x01\x12 \n\x1cORDER_ERROR_INVALID_ORDER_ID\x10\x02\x12\x1f\n\x1bORDER_ERROR_OUT_OF_SEQUENCE\x10\x03\x12&\n"ORDER_ERROR_INVALID_REMAINING_SIZE\x10\x04\x12\x1c\n\x18ORDER_ERROR_TIME_FAILURE\x10\x05\x12\x1f\n\x1bORDER_ERROR_REMOVAL_FAILURE\x10\x06\x12+\n\'ORDER_ERROR_INVALID_EXPIRATION_DATETIME\x10\x07\x12\'\n#ORDER_ERROR_INVALID_ORDER_REFERENCE\x10\x08\x12 \n\x1cORDER_ERROR_EDIT_NOT_ALLOWED\x10\t\x12\x1d\n\x19ORDER_ERROR_AMEND_FAILURE\x10\n\x12\x19\n\x15ORDER_ERROR_NOT_FOUND\x10\x0b\x12 \n\x1cORDER_ERROR_INVALID_PARTY_ID\x10\x0c\x12\x1d\n\x19ORDER_ERROR_MARKET_CLOSED\x10\r\x12#\n\x1fORDER_ERROR_MARGIN_CHECK_FAILED\x10\x0e\x12\'\n#ORDER_ERROR_MISSING_GENERAL_ACCOUNT\x10\x0f\x12\x1e\n\x1aORDER_ERROR_INTERNAL_ERROR\x10\x10\x12\x1c\n\x18ORDER_ERROR_INVALID_SIZE\x10\x11\x12#\n\x1fORDER_ERROR_INVALID_PERSISTENCE\x10\x12\x12\x1c\n\x18ORDER_ERROR_INVALID_TYPE\x10\x13\x12\x1c\n\x18ORDER_ERROR_SELF_TRADING\x10\x14\x12.\n*ORDER_ERROR_INSUFFICIENT_FUNDS_TO_PAY_FEES\x10\x15\x12%\n!ORDER_ERROR_INCORRECT_MARKET_TYPE\x10\x16\x12%\n!ORDER_ERROR_INVALID_TIME_IN_FORCE\x10\x17\x12\x37\n3ORDER_ERROR_CANNOT_SEND_GFN_ORDER_DURING_AN_AUCTION\x10\x18\x12?\n;ORDER_ERROR_CANNOT_SEND_GFA_ORDER_DURING_CONTINUOUS_TRADING\x10\x19\x12\x34\n0ORDER_ERROR_CANNOT_AMEND_TO_GTT_WITHOUT_EXPIRYAT\x10\x1a\x12)\n%ORDER_ERROR_EXPIRYAT_BEFORE_CREATEDAT\x10\x1b\x12,\n(ORDER_ERROR_CANNOT_HAVE_GTC_AND_EXPIRYAT\x10\x1c\x12*\n&ORDER_ERROR_CANNOT_AMEND_TO_FOK_OR_IOC\x10\x1d\x12*\n&ORDER_ERROR_CANNOT_AMEND_TO_GFA_OR_GFN\x10\x1e\x12,\n(ORDER_ERROR_CANNOT_AMEND_FROM_GFA_OR_GFN\x10\x1f\x12\x34\n0ORDER_ERROR_CANNOT_SEND_IOC_ORDER_DURING_AUCTION\x10 \x12\x34\n0ORDER_ERROR_CANNOT_SEND_FOK_ORDER_DURING_AUCTION\x10!\x12#\n\x1fORDER_ERROR_MUST_BE_LIMIT_ORDER\x10"\x12"\n\x1eORDER_ERROR_MUST_BE_GTT_OR_GTC\x10#\x12\'\n#ORDER_ERROR_WITHOUT_REFERENCE_PRICE\x10$\x12\x33\n/ORDER_ERROR_BUY_CANNOT_REFERENCE_BEST_ASK_PRICE\x10%\x12\x37\n3ORDER_ERROR_OFFSET_MUST_BE_GREATER_OR_EQUAL_TO_ZERO\x10(\x12\x34\n0ORDER_ERROR_SELL_CANNOT_REFERENCE_BEST_BID_PRICE\x10)\x12\x30\n,ORDER_ERROR_OFFSET_MUST_BE_GREATER_THAN_ZERO\x10*\x12*\n&ORDER_ERROR_INSUFFICIENT_ASSET_BALANCE\x10+\x12\x45\nAORDER_ERROR_CANNOT_AMEND_PEGGED_ORDER_DETAILS_ON_NON_PEGGED_ORDER\x10,\x12.\n*ORDER_ERROR_UNABLE_TO_REPRICE_PEGGED_ORDER\x10-\x12\x35\n1ORDER_ERROR_UNABLE_TO_AMEND_PRICE_ON_PEGGED_ORDER\x10.\x12\x38\n4ORDER_ERROR_NON_PERSISTENT_ORDER_OUT_OF_PRICE_BOUNDS\x10/\x12&\n"ORDER_ERROR_TOO_MANY_PEGGED_ORDERS\x10\x30\x12+\n\'ORDER_ERROR_POST_ONLY_ORDER_WOULD_TRADE\x10\x31\x12;\n7ORDER_ERROR_REDUCE_ONLY_ORDER_WOULD_NOT_REDUCE_POSITION\x10\x32"\x04\x08&\x10&"\x04\x08\'\x10\'*\x82\x01\n\x0b\x43hainStatus\x12\x1c\n\x18\x43HAIN_STATUS_UNSPECIFIED\x10\x00\x12\x1d\n\x19\x43HAIN_STATUS_DISCONNECTED\x10\x01\x12\x1a\n\x16\x43HAIN_STATUS_REPLAYING\x10\x02\x12\x1a\n\x16\x43HAIN_STATUS_CONNECTED\x10\x03*\xc4\x04\n\x0b\x41\x63\x63ountType\x12\x1c\n\x18\x41\x43\x43OUNT_TYPE_UNSPECIFIED\x10\x00\x12\x1a\n\x16\x41\x43\x43OUNT_TYPE_INSURANCE\x10\x01\x12\x1b\n\x17\x41\x43\x43OUNT_TYPE_SETTLEMENT\x10\x02\x12\x17\n\x13\x41\x43\x43OUNT_TYPE_MARGIN\x10\x03\x12\x18\n\x14\x41\x43\x43OUNT_TYPE_GENERAL\x10\x04\x12$\n ACCOUNT_TYPE_FEES_INFRASTRUCTURE\x10\x05\x12\x1f\n\x1b\x41\x43\x43OUNT_TYPE_FEES_LIQUIDITY\x10\x06\x12\x1b\n\x17\x41\x43\x43OUNT_TYPE_FEES_MAKER\x10\x07\x12\x15\n\x11\x41\x43\x43OUNT_TYPE_BOND\x10\t\x12\x19\n\x15\x41\x43\x43OUNT_TYPE_EXTERNAL\x10\n\x12!\n\x1d\x41\x43\x43OUNT_TYPE_GLOBAL_INSURANCE\x10\x0b\x12\x1e\n\x1a\x41\x43\x43OUNT_TYPE_GLOBAL_REWARD\x10\x0c\x12"\n\x1e\x41\x43\x43OUNT_TYPE_PENDING_TRANSFERS\x10\r\x12\'\n#ACCOUNT_TYPE_REWARD_MAKER_PAID_FEES\x10\x0e\x12+\n\'ACCOUNT_TYPE_REWARD_MAKER_RECEIVED_FEES\x10\x0f\x12(\n$ACCOUNT_TYPE_REWARD_LP_RECEIVED_FEES\x10\x10\x12(\n$ACCOUNT_TYPE_REWARD_MARKET_PROPOSERS\x10\x11"\x04\x08\x08\x10\x08*\xc9\x06\n\x0cTransferType\x12\x1d\n\x19TRANSFER_TYPE_UNSPECIFIED\x10\x00\x12\x16\n\x12TRANSFER_TYPE_LOSS\x10\x01\x12\x15\n\x11TRANSFER_TYPE_WIN\x10\x02\x12\x1a\n\x16TRANSFER_TYPE_MTM_LOSS\x10\x04\x12\x19\n\x15TRANSFER_TYPE_MTM_WIN\x10\x05\x12\x1c\n\x18TRANSFER_TYPE_MARGIN_LOW\x10\x06\x12\x1d\n\x19TRANSFER_TYPE_MARGIN_HIGH\x10\x07\x12$\n TRANSFER_TYPE_MARGIN_CONFISCATED\x10\x08\x12\x1f\n\x1bTRANSFER_TYPE_MAKER_FEE_PAY\x10\t\x12#\n\x1fTRANSFER_TYPE_MAKER_FEE_RECEIVE\x10\n\x12(\n$TRANSFER_TYPE_INFRASTRUCTURE_FEE_PAY\x10\x0b\x12/\n+TRANSFER_TYPE_INFRASTRUCTURE_FEE_DISTRIBUTE\x10\x0c\x12#\n\x1fTRANSFER_TYPE_LIQUIDITY_FEE_PAY\x10\r\x12*\n&TRANSFER_TYPE_LIQUIDITY_FEE_DISTRIBUTE\x10\x0e\x12\x1a\n\x16TRANSFER_TYPE_BOND_LOW\x10\x0f\x12\x1b\n\x17TRANSFER_TYPE_BOND_HIGH\x10\x10\x12\x1a\n\x16TRANSFER_TYPE_WITHDRAW\x10\x12\x12\x19\n\x15TRANSFER_TYPE_DEPOSIT\x10\x13\x12\x1f\n\x1bTRANSFER_TYPE_BOND_SLASHING\x10\x14\x12\x1f\n\x1bTRANSFER_TYPE_REWARD_PAYOUT\x10\x15\x12%\n!TRANSFER_TYPE_TRANSFER_FUNDS_SEND\x10\x16\x12+\n\'TRANSFER_TYPE_TRANSFER_FUNDS_DISTRIBUTE\x10\x17\x12\x1f\n\x1bTRANSFER_TYPE_CLEAR_ACCOUNT\x10\x18\x12,\n(TRANSFER_TYPE_CHECKPOINT_BALANCE_RESTORE\x10\x19"\x04\x08\x03\x10\x03"\x04\x08\x11\x10\x11*\xc7\x01\n\x0e\x44ispatchMetric\x12\x1f\n\x1b\x44ISPATCH_METRIC_UNSPECIFIED\x10\x00\x12#\n\x1f\x44ISPATCH_METRIC_MAKER_FEES_PAID\x10\x01\x12\'\n#DISPATCH_METRIC_MAKER_FEES_RECEIVED\x10\x02\x12$\n DISPATCH_METRIC_LP_FEES_RECEIVED\x10\x03\x12 \n\x1c\x44ISPATCH_METRIC_MARKET_VALUE\x10\x04*c\n\nNodeStatus\x12\x1b\n\x17NODE_STATUS_UNSPECIFIED\x10\x00\x12\x19\n\x15NODE_STATUS_VALIDATOR\x10\x01\x12\x1d\n\x19NODE_STATUS_NON_VALIDATOR\x10\x02*Y\n\x0b\x45pochAction\x12\x1c\n\x18\x45POCH_ACTION_UNSPECIFIED\x10\x00\x12\x16\n\x12\x45POCH_ACTION_START\x10\x01\x12\x14\n\x10\x45POCH_ACTION_END\x10\x02*\xa7\x01\n\x13ValidatorNodeStatus\x12%\n!VALIDATOR_NODE_STATUS_UNSPECIFIED\x10\x00\x12$\n VALIDATOR_NODE_STATUS_TENDERMINT\x10\x01\x12 \n\x1cVALIDATOR_NODE_STATUS_ERSATZ\x10\x02\x12!\n\x1dVALIDATOR_NODE_STATUS_PENDING\x10\x03\x42\'Z%code.vegaprotocol.io/vega/protos/vegab\x06proto3'
+    b'\n\x0fvega/vega.proto\x12\x04vega\x1a\x12vega/markets.proto"\xb8\x07\n\tStopOrder\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12#\n\x0boco_link_id\x18\x02 \x01(\tH\x01R\tocoLinkId\x88\x01\x01\x12"\n\nexpires_at\x18\x03 \x01(\x03H\x02R\texpiresAt\x88\x01\x01\x12L\n\x0f\x65xpiry_strategy\x18\x04 \x01(\x0e\x32\x1e.vega.StopOrder.ExpiryStrategyH\x03R\x0e\x65xpiryStrategy\x88\x01\x01\x12M\n\x11trigger_direction\x18\x05 \x01(\x0e\x32 .vega.StopOrder.TriggerDirectionR\x10triggerDirection\x12.\n\x06status\x18\x06 \x01(\x0e\x32\x16.vega.StopOrder.StatusR\x06status\x12\x1d\n\ncreated_at\x18\x07 \x01(\x03R\tcreatedAt\x12"\n\nupdated_at\x18\x08 \x01(\x03H\x04R\tupdatedAt\x88\x01\x01\x12\x19\n\x08order_id\x18\t \x01(\tR\x07orderId\x12\x14\n\x05party\x18\n \x01(\tR\x05party\x12\x16\n\x05price\x18\x64 \x01(\tH\x00R\x05price\x12\x38\n\x17trailing_percent_offset\x18\x65 \x01(\tH\x00R\x15trailingPercentOffset"j\n\x0e\x45xpiryStrategy\x12\x1f\n\x1b\x45XPIRY_STRATEGY_UNSPECIFIED\x10\x00\x12\x1b\n\x17\x45XPIRY_STRATEGY_CANCELS\x10\x01\x12\x1a\n\x16\x45XPIRY_STRATEGY_SUBMIT\x10\x02"{\n\x10TriggerDirection\x12!\n\x1dTRIGGER_DIRECTION_UNSPECIFIED\x10\x00\x12!\n\x1dTRIGGER_DIRECTION_RISES_ABOVE\x10\x01\x12!\n\x1dTRIGGER_DIRECTION_FALLS_BELOW\x10\x02"\x88\x01\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x12\n\x0eSTATUS_PENDING\x10\x01\x12\x14\n\x10STATUS_CANCELLED\x10\x02\x12\x12\n\x0eSTATUS_STOPPED\x10\x03\x12\x14\n\x10STATUS_TRIGGERED\x10\x04\x12\x12\n\x0eSTATUS_EXPIRED\x10\x05\x42\t\n\x07triggerB\x0e\n\x0c_oco_link_idB\r\n\x0b_expires_atB\x12\n\x10_expiry_strategyB\r\n\x0b_updated_at"\x17\n\x05Party\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id"N\n\nRiskFactor\x12\x16\n\x06market\x18\x01 \x01(\tR\x06market\x12\x14\n\x05short\x18\x02 \x01(\tR\x05short\x12\x12\n\x04long\x18\x03 \x01(\tR\x04long"Z\n\x0bPeggedOrder\x12\x33\n\treference\x18\x01 \x01(\x0e\x32\x15.vega.PeggedReferenceR\treference\x12\x16\n\x06offset\x18\x02 \x01(\tR\x06offset"\x8c\x01\n\x0cIcebergOrder\x12\x1b\n\tpeak_size\x18\x01 \x01(\x04R\x08peakSize\x12\x30\n\x14minimum_visible_size\x18\x02 \x01(\x04R\x12minimumVisibleSize\x12-\n\x12reserved_remaining\x18\x03 \x01(\x04R\x11reservedRemaining"\x80\n\n\x05Order\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x03 \x01(\tR\x07partyId\x12\x1e\n\x04side\x18\x04 \x01(\x0e\x32\n.vega.SideR\x04side\x12\x14\n\x05price\x18\x05 \x01(\tR\x05price\x12\x12\n\x04size\x18\x06 \x01(\x04R\x04size\x12\x1c\n\tremaining\x18\x07 \x01(\x04R\tremaining\x12;\n\rtime_in_force\x18\x08 \x01(\x0e\x32\x17.vega.Order.TimeInForceR\x0btimeInForce\x12$\n\x04type\x18\t \x01(\x0e\x32\x10.vega.Order.TypeR\x04type\x12\x1d\n\ncreated_at\x18\n \x01(\x03R\tcreatedAt\x12*\n\x06status\x18\x0b \x01(\x0e\x32\x12.vega.Order.StatusR\x06status\x12\x1d\n\nexpires_at\x18\x0c \x01(\x03R\texpiresAt\x12\x1c\n\treference\x18\r \x01(\tR\treference\x12-\n\x06reason\x18\x0e \x01(\x0e\x32\x10.vega.OrderErrorH\x00R\x06reason\x88\x01\x01\x12\x1d\n\nupdated_at\x18\x0f \x01(\x03R\tupdatedAt\x12\x18\n\x07version\x18\x10 \x01(\x04R\x07version\x12\x19\n\x08\x62\x61tch_id\x18\x11 \x01(\x04R\x07\x62\x61tchId\x12\x34\n\x0cpegged_order\x18\x12 \x01(\x0b\x32\x11.vega.PeggedOrderR\x0bpeggedOrder\x12\x34\n\x16liquidity_provision_id\x18\x13 \x01(\tR\x14liquidityProvisionId\x12\x1b\n\tpost_only\x18\x14 \x01(\x08R\x08postOnly\x12\x1f\n\x0breduce_only\x18\x15 \x01(\x08R\nreduceOnly\x12<\n\riceberg_order\x18\x16 \x01(\x0b\x32\x12.vega.IcebergOrderH\x01R\x0cicebergOrder\x88\x01\x01"\xb6\x01\n\x0bTimeInForce\x12\x1d\n\x19TIME_IN_FORCE_UNSPECIFIED\x10\x00\x12\x15\n\x11TIME_IN_FORCE_GTC\x10\x01\x12\x15\n\x11TIME_IN_FORCE_GTT\x10\x02\x12\x15\n\x11TIME_IN_FORCE_IOC\x10\x03\x12\x15\n\x11TIME_IN_FORCE_FOK\x10\x04\x12\x15\n\x11TIME_IN_FORCE_GFA\x10\x05\x12\x15\n\x11TIME_IN_FORCE_GFN\x10\x06"O\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x0e\n\nTYPE_LIMIT\x10\x01\x12\x0f\n\x0bTYPE_MARKET\x10\x02\x12\x10\n\x0cTYPE_NETWORK\x10\x03"\xc9\x01\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x11\n\rSTATUS_ACTIVE\x10\x01\x12\x12\n\x0eSTATUS_EXPIRED\x10\x02\x12\x14\n\x10STATUS_CANCELLED\x10\x03\x12\x12\n\x0eSTATUS_STOPPED\x10\x04\x12\x11\n\rSTATUS_FILLED\x10\x05\x12\x13\n\x0fSTATUS_REJECTED\x10\x06\x12\x1b\n\x17STATUS_PARTIALLY_FILLED\x10\x07\x12\x11\n\rSTATUS_PARKED\x10\x08\x42\t\n\x07_reasonB\x10\n\x0e_iceberg_order"B\n\x1dOrderCancellationConfirmation\x12!\n\x05order\x18\x01 \x01(\x0b\x32\x0b.vega.OrderR\x05order"\xa0\x01\n\x11OrderConfirmation\x12!\n\x05order\x18\x01 \x01(\x0b\x32\x0b.vega.OrderR\x05order\x12#\n\x06trades\x18\x02 \x03(\x0b\x32\x0b.vega.TradeR\x06trades\x12\x43\n\x17passive_orders_affected\x18\x03 \x03(\x0b\x32\x0b.vega.OrderR\x15passiveOrdersAffected"\xd3\x01\n\x16\x41uctionIndicativeState\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12)\n\x10indicative_price\x18\x02 \x01(\tR\x0findicativePrice\x12+\n\x11indicative_volume\x18\x03 \x01(\x04R\x10indicativeVolume\x12#\n\rauction_start\x18\x04 \x01(\x03R\x0c\x61uctionStart\x12\x1f\n\x0b\x61uction_end\x18\x05 \x01(\x03R\nauctionEnd"\xdb\x04\n\x05Trade\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1b\n\tmarket_id\x18\x02 \x01(\tR\x08marketId\x12\x14\n\x05price\x18\x03 \x01(\tR\x05price\x12\x12\n\x04size\x18\x04 \x01(\x04R\x04size\x12\x14\n\x05\x62uyer\x18\x05 \x01(\tR\x05\x62uyer\x12\x16\n\x06seller\x18\x06 \x01(\tR\x06seller\x12(\n\taggressor\x18\x07 \x01(\x0e\x32\n.vega.SideR\taggressor\x12\x1b\n\tbuy_order\x18\x08 \x01(\tR\x08\x62uyOrder\x12\x1d\n\nsell_order\x18\t \x01(\tR\tsellOrder\x12\x1c\n\ttimestamp\x18\n \x01(\x03R\ttimestamp\x12$\n\x04type\x18\x0b \x01(\x0e\x32\x10.vega.Trade.TypeR\x04type\x12&\n\tbuyer_fee\x18\x0c \x01(\x0b\x32\t.vega.FeeR\x08\x62uyerFee\x12(\n\nseller_fee\x18\r \x01(\x0b\x32\t.vega.FeeR\tsellerFee\x12.\n\x13\x62uyer_auction_batch\x18\x0e \x01(\x04R\x11\x62uyerAuctionBatch\x12\x30\n\x14seller_auction_batch\x18\x0f \x01(\x04R\x12sellerAuctionBatch"o\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x10\n\x0cTYPE_DEFAULT\x10\x01\x12\x1f\n\x1bTYPE_NETWORK_CLOSE_OUT_GOOD\x10\x02\x12\x1e\n\x1aTYPE_NETWORK_CLOSE_OUT_BAD\x10\x03"v\n\x03\x46\x65\x65\x12\x1b\n\tmaker_fee\x18\x01 \x01(\tR\x08makerFee\x12-\n\x12infrastructure_fee\x18\x02 \x01(\tR\x11infrastructureFee\x12#\n\rliquidity_fee\x18\x03 \x01(\tR\x0cliquidityFee"/\n\x08TradeSet\x12#\n\x06trades\x18\x01 \x03(\x0b\x32\x0b.vega.TradeR\x06trades"\xd6\x01\n\x06\x43\x61ndle\x12\x1c\n\ttimestamp\x18\x01 \x01(\x03R\ttimestamp\x12\x1a\n\x08\x64\x61tetime\x18\x02 \x01(\tR\x08\x64\x61tetime\x12\x12\n\x04high\x18\x03 \x01(\tR\x04high\x12\x10\n\x03low\x18\x04 \x01(\tR\x03low\x12\x12\n\x04open\x18\x05 \x01(\tR\x04open\x12\x14\n\x05\x63lose\x18\x06 \x01(\tR\x05\x63lose\x12\x16\n\x06volume\x18\x07 \x01(\x04R\x06volume\x12*\n\x08interval\x18\x08 \x01(\x0e\x32\x0e.vega.IntervalR\x08interval"d\n\nPriceLevel\x12\x14\n\x05price\x18\x01 \x01(\tR\x05price\x12(\n\x10number_of_orders\x18\x02 \x01(\x04R\x0enumberOfOrders\x12\x16\n\x06volume\x18\x03 \x01(\x04R\x06volume"\x9d\x01\n\x0bMarketDepth\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12"\n\x03\x62uy\x18\x02 \x03(\x0b\x32\x10.vega.PriceLevelR\x03\x62uy\x12$\n\x04sell\x18\x03 \x03(\x0b\x32\x10.vega.PriceLevelR\x04sell\x12\'\n\x0fsequence_number\x18\x04 \x01(\x04R\x0esequenceNumber"\xdd\x01\n\x11MarketDepthUpdate\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12"\n\x03\x62uy\x18\x02 \x03(\x0b\x32\x10.vega.PriceLevelR\x03\x62uy\x12$\n\x04sell\x18\x03 \x03(\x0b\x32\x10.vega.PriceLevelR\x04sell\x12\'\n\x0fsequence_number\x18\x04 \x01(\x04R\x0esequenceNumber\x12\x38\n\x18previous_sequence_number\x18\x05 \x01(\x04R\x16previousSequenceNumber"\xf7\x02\n\x08Position\x12\x1b\n\tmarket_id\x18\x01 \x01(\tR\x08marketId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x1f\n\x0bopen_volume\x18\x03 \x01(\x03R\nopenVolume\x12!\n\x0crealised_pnl\x18\x04 \x01(\tR\x0brealisedPnl\x12%\n\x0eunrealised_pnl\x18\x05 \x01(\tR\runrealisedPnl\x12.\n\x13\x61verage_entry_price\x18\x06 \x01(\tR\x11\x61verageEntryPrice\x12\x1d\n\nupdated_at\x18\x07 \x01(\x03R\tupdatedAt\x12:\n\x19loss_socialisation_amount\x18\x08 \x01(\tR\x17lossSocialisationAmount\x12=\n\x0fposition_status\x18\t \x01(\x0e\x32\x14.vega.PositionStatusR\x0epositionStatus"=\n\rPositionTrade\x12\x16\n\x06volume\x18\x01 \x01(\x03R\x06volume\x12\x14\n\x05price\x18\x02 \x01(\tR\x05price"\xe4\x02\n\x07\x44\x65posit\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12,\n\x06status\x18\x02 \x01(\x0e\x32\x14.vega.Deposit.StatusR\x06status\x12\x19\n\x08party_id\x18\x03 \x01(\tR\x07partyId\x12\x14\n\x05\x61sset\x18\x04 \x01(\tR\x05\x61sset\x12\x16\n\x06\x61mount\x18\x05 \x01(\tR\x06\x61mount\x12\x17\n\x07tx_hash\x18\x06 \x01(\tR\x06txHash\x12-\n\x12\x63redited_timestamp\x18\x07 \x01(\x03R\x11\x63reditedTimestamp\x12+\n\x11\x63reated_timestamp\x18\x08 \x01(\x03R\x10\x63reatedTimestamp"]\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x0f\n\x0bSTATUS_OPEN\x10\x01\x12\x14\n\x10STATUS_CANCELLED\x10\x02\x12\x14\n\x10STATUS_FINALIZED\x10\x03"\xa8\x03\n\nWithdrawal\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount\x12\x14\n\x05\x61sset\x18\x04 \x01(\tR\x05\x61sset\x12/\n\x06status\x18\x05 \x01(\x0e\x32\x17.vega.Withdrawal.StatusR\x06status\x12\x10\n\x03ref\x18\x06 \x01(\tR\x03ref\x12\x17\n\x07tx_hash\x18\x08 \x01(\tR\x06txHash\x12+\n\x11\x63reated_timestamp\x18\t \x01(\x03R\x10\x63reatedTimestamp\x12/\n\x13withdrawn_timestamp\x18\n \x01(\x03R\x12withdrawnTimestamp\x12#\n\x03\x65xt\x18\x0b \x01(\x0b\x32\x11.vega.WithdrawExtR\x03\x65xt"\\\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x0f\n\x0bSTATUS_OPEN\x10\x01\x12\x13\n\x0fSTATUS_REJECTED\x10\x02\x12\x14\n\x10STATUS_FINALIZED\x10\x03J\x04\x08\x07\x10\x08"D\n\x0bWithdrawExt\x12.\n\x05\x65rc20\x18\x01 \x01(\x0b\x32\x16.vega.Erc20WithdrawExtH\x00R\x05\x65rc20B\x05\n\x03\x65xt"=\n\x10\x45rc20WithdrawExt\x12)\n\x10receiver_address\x18\x01 \x01(\tR\x0freceiverAddress"\xa3\x01\n\x07\x41\x63\x63ount\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x14\n\x05owner\x18\x02 \x01(\tR\x05owner\x12\x18\n\x07\x62\x61lance\x18\x03 \x01(\tR\x07\x62\x61lance\x12\x14\n\x05\x61sset\x18\x04 \x01(\tR\x05\x61sset\x12\x1b\n\tmarket_id\x18\x05 \x01(\tR\x08marketId\x12%\n\x04type\x18\x06 \x01(\x0e\x32\x11.vega.AccountTypeR\x04type"?\n\x0f\x46inancialAmount\x12\x16\n\x06\x61mount\x18\x01 \x01(\tR\x06\x61mount\x12\x14\n\x05\x61sset\x18\x02 \x01(\tR\x05\x61sset"\xb3\x01\n\x08Transfer\x12\x14\n\x05owner\x18\x01 \x01(\tR\x05owner\x12-\n\x06\x61mount\x18\x02 \x01(\x0b\x32\x15.vega.FinancialAmountR\x06\x61mount\x12&\n\x04type\x18\x03 \x01(\x0e\x32\x12.vega.TransferTypeR\x04type\x12\x1d\n\nmin_amount\x18\x04 \x01(\tR\tminAmount\x12\x1b\n\tmarket_id\x18\x05 \x01(\tR\x08marketId"\x84\x01\n\x10\x44ispatchStrategy\x12(\n\x10\x61sset_for_metric\x18\x01 \x01(\tR\x0e\x61ssetForMetric\x12,\n\x06metric\x18\x02 \x01(\x0e\x32\x14.vega.DispatchMetricR\x06metric\x12\x18\n\x07markets\x18\x03 \x03(\tR\x07markets"\xe6\x01\n\x0fTransferRequest\x12\x30\n\x0c\x66rom_account\x18\x01 \x03(\x0b\x32\r.vega.AccountR\x0b\x66romAccount\x12,\n\nto_account\x18\x02 \x03(\x0b\x32\r.vega.AccountR\ttoAccount\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount\x12\x1d\n\nmin_amount\x18\x04 \x01(\tR\tminAmount\x12\x14\n\x05\x61sset\x18\x05 \x01(\tR\x05\x61sset\x12&\n\x04type\x18\x07 \x01(\x0e\x32\x12.vega.TransferTypeR\x04type"\xa7\x01\n\x0e\x41\x63\x63ountDetails\x12\x19\n\x08\x61sset_id\x18\x01 \x01(\tR\x07\x61ssetId\x12%\n\x04type\x18\x02 \x01(\x0e\x32\x11.vega.AccountTypeR\x04type\x12\x19\n\x05owner\x18\x03 \x01(\tH\x00R\x05owner\x88\x01\x01\x12 \n\tmarket_id\x18\x04 \x01(\tH\x01R\x08marketId\x88\x01\x01\x42\x08\n\x06_ownerB\x0c\n\n_market_id"\xb9\x02\n\x0bLedgerEntry\x12\x37\n\x0c\x66rom_account\x18\x01 \x01(\x0b\x32\x14.vega.AccountDetailsR\x0b\x66romAccount\x12\x33\n\nto_account\x18\x02 \x01(\x0b\x32\x14.vega.AccountDetailsR\ttoAccount\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount\x12&\n\x04type\x18\x04 \x01(\x0e\x32\x12.vega.TransferTypeR\x04type\x12\x1c\n\ttimestamp\x18\x05 \x01(\x03R\ttimestamp\x12\x30\n\x14\x66rom_account_balance\x18\x06 \x01(\tR\x12\x66romAccountBalance\x12,\n\x12to_account_balance\x18\x07 \x01(\tR\x10toAccountBalance"_\n\x13PostTransferBalance\x12.\n\x07\x61\x63\x63ount\x18\x01 \x01(\x0b\x32\x14.vega.AccountDetailsR\x07\x61\x63\x63ount\x12\x18\n\x07\x62\x61lance\x18\x02 \x01(\tR\x07\x62\x61lance"t\n\x0eLedgerMovement\x12+\n\x07\x65ntries\x18\x01 \x03(\x0b\x32\x11.vega.LedgerEntryR\x07\x65ntries\x12\x35\n\x08\x62\x61lances\x18\x02 \x03(\x0b\x32\x19.vega.PostTransferBalanceR\x08\x62\x61lances"\xad\x02\n\x0cMarginLevels\x12-\n\x12maintenance_margin\x18\x01 \x01(\tR\x11maintenanceMargin\x12!\n\x0csearch_level\x18\x02 \x01(\tR\x0bsearchLevel\x12%\n\x0einitial_margin\x18\x03 \x01(\tR\rinitialMargin\x12\x38\n\x18\x63ollateral_release_level\x18\x04 \x01(\tR\x16\x63ollateralReleaseLevel\x12\x19\n\x08party_id\x18\x05 \x01(\tR\x07partyId\x12\x1b\n\tmarket_id\x18\x06 \x01(\tR\x08marketId\x12\x14\n\x05\x61sset\x18\x07 \x01(\tR\x05\x61sset\x12\x1c\n\ttimestamp\x18\x08 \x01(\x03R\ttimestamp"\x8a\x0b\n\nMarketData\x12\x1d\n\nmark_price\x18\x01 \x01(\tR\tmarkPrice\x12$\n\x0e\x62\x65st_bid_price\x18\x02 \x01(\tR\x0c\x62\x65stBidPrice\x12&\n\x0f\x62\x65st_bid_volume\x18\x03 \x01(\x04R\rbestBidVolume\x12(\n\x10\x62\x65st_offer_price\x18\x04 \x01(\tR\x0e\x62\x65stOfferPrice\x12*\n\x11\x62\x65st_offer_volume\x18\x05 \x01(\x04R\x0f\x62\x65stOfferVolume\x12\x31\n\x15\x62\x65st_static_bid_price\x18\x06 \x01(\tR\x12\x62\x65stStaticBidPrice\x12\x33\n\x16\x62\x65st_static_bid_volume\x18\x07 \x01(\x04R\x13\x62\x65stStaticBidVolume\x12\x35\n\x17\x62\x65st_static_offer_price\x18\x08 \x01(\tR\x14\x62\x65stStaticOfferPrice\x12\x37\n\x18\x62\x65st_static_offer_volume\x18\t \x01(\x04R\x15\x62\x65stStaticOfferVolume\x12\x1b\n\tmid_price\x18\n \x01(\tR\x08midPrice\x12(\n\x10static_mid_price\x18\x0b \x01(\tR\x0estaticMidPrice\x12\x16\n\x06market\x18\x0c \x01(\tR\x06market\x12\x1c\n\ttimestamp\x18\r \x01(\x03R\ttimestamp\x12#\n\ropen_interest\x18\x0e \x01(\x04R\x0copenInterest\x12\x1f\n\x0b\x61uction_end\x18\x0f \x01(\x03R\nauctionEnd\x12#\n\rauction_start\x18\x10 \x01(\x03R\x0c\x61uctionStart\x12)\n\x10indicative_price\x18\x11 \x01(\tR\x0findicativePrice\x12+\n\x11indicative_volume\x18\x12 \x01(\x04R\x10indicativeVolume\x12H\n\x13market_trading_mode\x18\x13 \x01(\x0e\x32\x18.vega.Market.TradingModeR\x11marketTradingMode\x12.\n\x07trigger\x18\x14 \x01(\x0e\x32\x14.vega.AuctionTriggerR\x07trigger\x12\x41\n\x11\x65xtension_trigger\x18\x15 \x01(\x0e\x32\x14.vega.AuctionTriggerR\x10\x65xtensionTrigger\x12!\n\x0ctarget_stake\x18\x16 \x01(\tR\x0btargetStake\x12%\n\x0esupplied_stake\x18\x17 \x01(\tR\rsuppliedStake\x12S\n\x17price_monitoring_bounds\x18\x18 \x03(\x0b\x32\x1b.vega.PriceMonitoringBoundsR\x15priceMonitoringBounds\x12,\n\x12market_value_proxy\x18\x19 \x01(\tR\x10marketValueProxy\x12`\n\x1cliquidity_provider_fee_share\x18\x1a \x03(\x0b\x32\x1f.vega.LiquidityProviderFeeShareR\x19liquidityProviderFeeShare\x12\x35\n\x0cmarket_state\x18\x1b \x01(\x0e\x32\x12.vega.Market.StateR\x0bmarketState\x12-\n\x13next_mark_to_market\x18\x1c \x01(\x03R\x10nextMarkToMarket\x12*\n\x11last_traded_price\x18\x1d \x01(\tR\x0flastTradedPrice\x12#\n\rmarket_growth\x18\x1e \x01(\tR\x0cmarketGrowth"\xdf\x01\n\x19LiquidityProviderFeeShare\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12*\n\x11\x65quity_like_share\x18\x02 \x01(\tR\x0f\x65quityLikeShare\x12\x36\n\x17\x61verage_entry_valuation\x18\x03 \x01(\tR\x15\x61verageEntryValuation\x12#\n\raverage_score\x18\x04 \x01(\tR\x0c\x61verageScore\x12#\n\rvirtual_stake\x18\x05 \x01(\tR\x0cvirtualStake"\xc8\x01\n\x15PriceMonitoringBounds\x12&\n\x0fmin_valid_price\x18\x01 \x01(\tR\rminValidPrice\x12&\n\x0fmax_valid_price\x18\x02 \x01(\tR\rmaxValidPrice\x12\x36\n\x07trigger\x18\x03 \x01(\x0b\x32\x1c.vega.PriceMonitoringTriggerR\x07trigger\x12\'\n\x0freference_price\x18\x04 \x01(\tR\x0ereferencePrice"Q\n\x0b\x45rrorDetail\x12\x12\n\x04\x63ode\x18\x01 \x01(\x05R\x04\x63ode\x12\x18\n\x07message\x18\x02 \x01(\tR\x07message\x12\x14\n\x05inner\x18\x03 \x01(\tR\x05inner":\n\x10NetworkParameter\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value"\x82\x03\n\rNetworkLimits\x12,\n\x12\x63\x61n_propose_market\x18\x01 \x01(\x08R\x10\x63\x61nProposeMarket\x12*\n\x11\x63\x61n_propose_asset\x18\x02 \x01(\x08R\x0f\x63\x61nProposeAsset\x12\x34\n\x16propose_market_enabled\x18\x04 \x01(\x08R\x14proposeMarketEnabled\x12\x32\n\x15propose_asset_enabled\x18\x05 \x01(\x08R\x13proposeAssetEnabled\x12%\n\x0egenesis_loaded\x18\x07 \x01(\x08R\rgenesisLoaded\x12=\n\x1bpropose_market_enabled_from\x18\x08 \x01(\x03R\x18proposeMarketEnabledFrom\x12;\n\x1apropose_asset_enabled_from\x18\t \x01(\x03R\x17proposeAssetEnabledFromJ\x04\x08\x03\x10\x04J\x04\x08\x06\x10\x07"}\n\x0eLiquidityOrder\x12\x33\n\treference\x18\x01 \x01(\x0e\x32\x15.vega.PeggedReferenceR\treference\x12\x1e\n\nproportion\x18\x02 \x01(\rR\nproportion\x12\x16\n\x06offset\x18\x03 \x01(\tR\x06offset"s\n\x17LiquidityOrderReference\x12\x19\n\x08order_id\x18\x01 \x01(\tR\x07orderId\x12=\n\x0fliquidity_order\x18\x02 \x01(\x0b\x32\x14.vega.LiquidityOrderR\x0eliquidityOrder"\xd2\x04\n\x12LiquidityProvision\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x1d\n\ncreated_at\x18\x03 \x01(\x03R\tcreatedAt\x12\x1d\n\nupdated_at\x18\x04 \x01(\x03R\tupdatedAt\x12\x1b\n\tmarket_id\x18\x05 \x01(\tR\x08marketId\x12+\n\x11\x63ommitment_amount\x18\x06 \x01(\tR\x10\x63ommitmentAmount\x12\x10\n\x03\x66\x65\x65\x18\x07 \x01(\tR\x03\x66\x65\x65\x12\x33\n\x05sells\x18\x08 \x03(\x0b\x32\x1d.vega.LiquidityOrderReferenceR\x05sells\x12\x31\n\x04\x62uys\x18\t \x03(\x0b\x32\x1d.vega.LiquidityOrderReferenceR\x04\x62uys\x12\x18\n\x07version\x18\n \x01(\x04R\x07version\x12\x37\n\x06status\x18\x0b \x01(\x0e\x32\x1f.vega.LiquidityProvision.StatusR\x06status\x12\x1c\n\treference\x18\x0c \x01(\tR\treference"\x9d\x01\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x11\n\rSTATUS_ACTIVE\x10\x01\x12\x12\n\x0eSTATUS_STOPPED\x10\x02\x12\x14\n\x10STATUS_CANCELLED\x10\x03\x12\x13\n\x0fSTATUS_REJECTED\x10\x04\x12\x15\n\x11STATUS_UNDEPLOYED\x10\x05\x12\x12\n\x0eSTATUS_PENDING\x10\x06"\xd0\x03\n\x0e\x45thereumConfig\x12\x1d\n\nnetwork_id\x18\x01 \x01(\tR\tnetworkId\x12\x19\n\x08\x63hain_id\x18\x02 \x01(\tR\x07\x63hainId\x12Z\n\x1a\x63ollateral_bridge_contract\x18\x03 \x01(\x0b\x32\x1c.vega.EthereumContractConfigR\x18\x63ollateralBridgeContract\x12$\n\rconfirmations\x18\x04 \x01(\rR\rconfirmations\x12T\n\x17staking_bridge_contract\x18\x05 \x01(\x0b\x32\x1c.vega.EthereumContractConfigR\x15stakingBridgeContract\x12R\n\x16token_vesting_contract\x18\x06 \x01(\x0b\x32\x1c.vega.EthereumContractConfigR\x14tokenVestingContract\x12X\n\x19multisig_control_contract\x18\x07 \x01(\x0b\x32\x1c.vega.EthereumContractConfigR\x17multisigControlContract"j\n\x16\x45thereumContractConfig\x12\x18\n\x07\x61\x64\x64ress\x18\x01 \x01(\tR\x07\x61\x64\x64ress\x12\x36\n\x17\x64\x65ployment_block_height\x18\x06 \x01(\x04R\x15\x64\x65ploymentBlockHeight"\xac\x01\n\x0f\x45pochTimestamps\x12\x1d\n\nstart_time\x18\x01 \x01(\x03R\tstartTime\x12\x1f\n\x0b\x65xpiry_time\x18\x02 \x01(\x03R\nexpiryTime\x12\x19\n\x08\x65nd_time\x18\x03 \x01(\x03R\x07\x65ndTime\x12\x1f\n\x0b\x66irst_block\x18\x04 \x01(\x04R\nfirstBlock\x12\x1d\n\nlast_block\x18\x05 \x01(\x04R\tlastBlock"\xb0\x01\n\x05\x45poch\x12\x10\n\x03seq\x18\x01 \x01(\x04R\x03seq\x12\x35\n\ntimestamps\x18\x02 \x01(\x0b\x32\x15.vega.EpochTimestampsR\ntimestamps\x12*\n\nvalidators\x18\x03 \x03(\x0b\x32\n.vega.NodeR\nvalidators\x12\x32\n\x0b\x64\x65legations\x18\x04 \x03(\x0b\x32\x10.vega.DelegationR\x0b\x64\x65legations"\x8e\x01\n\x12\x45pochParticipation\x12!\n\x05\x65poch\x18\x01 \x01(\x0b\x32\x0b.vega.EpochR\x05\x65poch\x12\x18\n\x07offline\x18\x02 \x01(\x04R\x07offline\x12\x16\n\x06online\x18\x03 \x01(\x04R\x06online\x12#\n\rtotal_rewards\x18\x04 \x01(\x01R\x0ctotalRewards"S\n\tEpochData\x12\x14\n\x05total\x18\x01 \x01(\x05R\x05total\x12\x18\n\x07offline\x18\x02 \x01(\x05R\x07offline\x12\x16\n\x06online\x18\x03 \x01(\x05R\x06online"\x9b\x02\n\x0cRankingScore\x12\x1f\n\x0bstake_score\x18\x01 \x01(\tR\nstakeScore\x12+\n\x11performance_score\x18\x02 \x01(\tR\x10performanceScore\x12\x42\n\x0fprevious_status\x18\x03 \x01(\x0e\x32\x19.vega.ValidatorNodeStatusR\x0epreviousStatus\x12\x31\n\x06status\x18\x04 \x01(\x0e\x32\x19.vega.ValidatorNodeStatusR\x06status\x12!\n\x0cvoting_power\x18\x05 \x01(\rR\x0bvotingPower\x12#\n\rranking_score\x18\x06 \x01(\tR\x0crankingScore"\xab\x02\n\x0bRewardScore\x12.\n\x13raw_validator_score\x18\x01 \x01(\tR\x11rawValidatorScore\x12+\n\x11performance_score\x18\x02 \x01(\tR\x10performanceScore\x12%\n\x0emultisig_score\x18\x03 \x01(\tR\rmultisigScore\x12\'\n\x0fvalidator_score\x18\x04 \x01(\tR\x0evalidatorScore\x12)\n\x10normalised_score\x18\x05 \x01(\tR\x0fnormalisedScore\x12\x44\n\x10validator_status\x18\x06 \x01(\x0e\x32\x19.vega.ValidatorNodeStatusR\x0fvalidatorStatus"\xb3\x05\n\x04Node\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x17\n\x07pub_key\x18\x02 \x01(\tR\x06pubKey\x12\x1c\n\ntm_pub_key\x18\x03 \x01(\tR\x08tmPubKey\x12)\n\x10\x65thereum_address\x18\x04 \x01(\tR\x0f\x65thereumAddress\x12\x19\n\x08info_url\x18\x05 \x01(\tR\x07infoUrl\x12\x1a\n\x08location\x18\x06 \x01(\tR\x08location\x12,\n\x12staked_by_operator\x18\x07 \x01(\tR\x10stakedByOperator\x12.\n\x13staked_by_delegates\x18\x08 \x01(\tR\x11stakedByDelegates\x12!\n\x0cstaked_total\x18\t \x01(\tR\x0bstakedTotal\x12,\n\x12max_intended_stake\x18\n \x01(\tR\x10maxIntendedStake\x12#\n\rpending_stake\x18\x0b \x01(\tR\x0cpendingStake\x12.\n\nepoch_data\x18\x0c \x01(\x0b\x32\x0f.vega.EpochDataR\tepochData\x12(\n\x06status\x18\r \x01(\x0e\x32\x10.vega.NodeStatusR\x06status\x12\x32\n\x0b\x64\x65legations\x18\x0e \x03(\x0b\x32\x10.vega.DelegationR\x0b\x64\x65legations\x12\x34\n\x0creward_score\x18\x0f \x01(\x0b\x32\x11.vega.RewardScoreR\x0brewardScore\x12\x37\n\rranking_score\x18\x10 \x01(\x0b\x32\x12.vega.RankingScoreR\x0crankingScore\x12\x12\n\x04name\x18\x11 \x01(\tR\x04name\x12\x1d\n\navatar_url\x18\x12 \x01(\tR\tavatarUrl"\x9c\x01\n\x07NodeSet\x12\x14\n\x05total\x18\x01 \x01(\rR\x05total\x12\x1a\n\x08inactive\x18\x02 \x01(\rR\x08inactive\x12\x1a\n\x08promoted\x18\x03 \x03(\tR\x08promoted\x12\x18\n\x07\x64\x65moted\x18\x04 \x03(\tR\x07\x64\x65moted\x12\x1d\n\x07maximum\x18\x05 \x01(\rH\x00R\x07maximum\x88\x01\x01\x42\n\n\x08_maximum"\xad\x02\n\x08NodeData\x12!\n\x0cstaked_total\x18\x01 \x01(\tR\x0bstakedTotal\x12\x1f\n\x0btotal_nodes\x18\x02 \x01(\rR\ntotalNodes\x12%\n\x0einactive_nodes\x18\x03 \x01(\rR\rinactiveNodes\x12\x38\n\x10tendermint_nodes\x18\x04 \x01(\x0b\x32\r.vega.NodeSetR\x0ftendermintNodes\x12\x30\n\x0c\x65rsatz_nodes\x18\x05 \x01(\x0b\x32\r.vega.NodeSetR\x0b\x65rsatzNodes\x12\x32\n\rpending_nodes\x18\x06 \x01(\x0b\x32\r.vega.NodeSetR\x0cpendingNodes\x12\x16\n\x06uptime\x18\x07 \x01(\x02R\x06uptime"p\n\nDelegation\x12\x14\n\x05party\x18\x01 \x01(\tR\x05party\x12\x17\n\x07node_id\x18\x02 \x01(\tR\x06nodeId\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount\x12\x1b\n\tepoch_seq\x18\x04 \x01(\tR\x08\x65pochSeq"\xfb\x01\n\x06Reward\x12\x19\n\x08\x61sset_id\x18\x01 \x01(\tR\x07\x61ssetId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x14\n\x05\x65poch\x18\x03 \x01(\x04R\x05\x65poch\x12\x16\n\x06\x61mount\x18\x04 \x01(\tR\x06\x61mount\x12.\n\x13percentage_of_total\x18\x05 \x01(\tR\x11percentageOfTotal\x12\x1f\n\x0breceived_at\x18\x06 \x01(\x03R\nreceivedAt\x12\x1b\n\tmarket_id\x18\x07 \x01(\tR\x08marketId\x12\x1f\n\x0breward_type\x18\x08 \x01(\tR\nrewardType"]\n\rRewardSummary\x12\x19\n\x08\x61sset_id\x18\x01 \x01(\tR\x07\x61ssetId\x12\x19\n\x08party_id\x18\x02 \x01(\tR\x07partyId\x12\x16\n\x06\x61mount\x18\x03 \x01(\tR\x06\x61mount"\x9b\x01\n\x12\x45pochRewardSummary\x12\x14\n\x05\x65poch\x18\x01 \x01(\x04R\x05\x65poch\x12\x19\n\x08\x61sset_id\x18\x02 \x01(\tR\x07\x61ssetId\x12\x1b\n\tmarket_id\x18\x03 \x01(\tR\x08marketId\x12\x1f\n\x0breward_type\x18\x04 \x01(\tR\nrewardType\x12\x16\n\x06\x61mount\x18\x05 \x01(\tR\x06\x61mount"y\n\x12StateValueProposal\x12 \n\x0cstate_var_id\x18\x01 \x01(\tR\nstateVarId\x12\x19\n\x08\x65vent_id\x18\x02 \x01(\tR\x07\x65ventId\x12&\n\x03kvb\x18\x03 \x03(\x0b\x32\x14.vega.KeyValueBundleR\x03kvb"k\n\x0eKeyValueBundle\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x1c\n\ttolerance\x18\x02 \x01(\tR\ttolerance\x12)\n\x05value\x18\x03 \x01(\x0b\x32\x13.vega.StateVarValueR\x05value"\xb4\x01\n\rStateVarValue\x12\x32\n\nscalar_val\x18\x01 \x01(\x0b\x32\x11.vega.ScalarValueH\x00R\tscalarVal\x12\x32\n\nvector_val\x18\x02 \x01(\x0b\x32\x11.vega.VectorValueH\x00R\tvectorVal\x12\x32\n\nmatrix_val\x18\x03 \x01(\x0b\x32\x11.vega.MatrixValueH\x00R\tmatrixValB\x07\n\x05value"#\n\x0bScalarValue\x12\x14\n\x05value\x18\x01 \x01(\tR\x05value"#\n\x0bVectorValue\x12\x14\n\x05value\x18\x01 \x03(\tR\x05value"6\n\x0bMatrixValue\x12\'\n\x05value\x18\x01 \x03(\x0b\x32\x11.vega.VectorValueR\x05value*9\n\x04Side\x12\x14\n\x10SIDE_UNSPECIFIED\x10\x00\x12\x0c\n\x08SIDE_BUY\x10\x01\x12\r\n\tSIDE_SELL\x10\x02*\xb5\x01\n\x08Interval\x12\x18\n\x14INTERVAL_UNSPECIFIED\x10\x00\x12\x1b\n\x0eINTERVAL_BLOCK\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x10\n\x0cINTERVAL_I1M\x10<\x12\x11\n\x0cINTERVAL_I5M\x10\xac\x02\x12\x12\n\rINTERVAL_I15M\x10\x84\x07\x12\x11\n\x0cINTERVAL_I1H\x10\x90\x1c\x12\x12\n\x0cINTERVAL_I6H\x10\xe0\xa8\x01\x12\x12\n\x0cINTERVAL_I1D\x10\x80\xa3\x05*\x94\x01\n\x0ePositionStatus\x12\x1f\n\x1bPOSITION_STATUS_UNSPECIFIED\x10\x00\x12!\n\x1dPOSITION_STATUS_ORDERS_CLOSED\x10\x01\x12\x1e\n\x1aPOSITION_STATUS_CLOSED_OUT\x10\x02\x12\x1e\n\x1aPOSITION_STATUS_DISTRESSED\x10\x04*\x81\x02\n\x0e\x41uctionTrigger\x12\x1f\n\x1b\x41UCTION_TRIGGER_UNSPECIFIED\x10\x00\x12\x19\n\x15\x41UCTION_TRIGGER_BATCH\x10\x01\x12\x1b\n\x17\x41UCTION_TRIGGER_OPENING\x10\x02\x12\x19\n\x15\x41UCTION_TRIGGER_PRICE\x10\x03\x12\x1d\n\x19\x41UCTION_TRIGGER_LIQUIDITY\x10\x04\x12,\n(AUCTION_TRIGGER_LIQUIDITY_TARGET_NOT_MET\x10\x05\x12.\n*AUCTION_TRIGGER_UNABLE_TO_DEPLOY_LP_ORDERS\x10\x06*\x8b\x01\n\x0fPeggedReference\x12 \n\x1cPEGGED_REFERENCE_UNSPECIFIED\x10\x00\x12\x18\n\x14PEGGED_REFERENCE_MID\x10\x01\x12\x1d\n\x19PEGGED_REFERENCE_BEST_BID\x10\x02\x12\x1d\n\x19PEGGED_REFERENCE_BEST_ASK\x10\x03*\xc9\x10\n\nOrderError\x12\x1b\n\x17ORDER_ERROR_UNSPECIFIED\x10\x00\x12!\n\x1dORDER_ERROR_INVALID_MARKET_ID\x10\x01\x12 \n\x1cORDER_ERROR_INVALID_ORDER_ID\x10\x02\x12\x1f\n\x1bORDER_ERROR_OUT_OF_SEQUENCE\x10\x03\x12&\n"ORDER_ERROR_INVALID_REMAINING_SIZE\x10\x04\x12\x1c\n\x18ORDER_ERROR_TIME_FAILURE\x10\x05\x12\x1f\n\x1bORDER_ERROR_REMOVAL_FAILURE\x10\x06\x12+\n\'ORDER_ERROR_INVALID_EXPIRATION_DATETIME\x10\x07\x12\'\n#ORDER_ERROR_INVALID_ORDER_REFERENCE\x10\x08\x12 \n\x1cORDER_ERROR_EDIT_NOT_ALLOWED\x10\t\x12\x1d\n\x19ORDER_ERROR_AMEND_FAILURE\x10\n\x12\x19\n\x15ORDER_ERROR_NOT_FOUND\x10\x0b\x12 \n\x1cORDER_ERROR_INVALID_PARTY_ID\x10\x0c\x12\x1d\n\x19ORDER_ERROR_MARKET_CLOSED\x10\r\x12#\n\x1fORDER_ERROR_MARGIN_CHECK_FAILED\x10\x0e\x12\'\n#ORDER_ERROR_MISSING_GENERAL_ACCOUNT\x10\x0f\x12\x1e\n\x1aORDER_ERROR_INTERNAL_ERROR\x10\x10\x12\x1c\n\x18ORDER_ERROR_INVALID_SIZE\x10\x11\x12#\n\x1fORDER_ERROR_INVALID_PERSISTENCE\x10\x12\x12\x1c\n\x18ORDER_ERROR_INVALID_TYPE\x10\x13\x12\x1c\n\x18ORDER_ERROR_SELF_TRADING\x10\x14\x12.\n*ORDER_ERROR_INSUFFICIENT_FUNDS_TO_PAY_FEES\x10\x15\x12%\n!ORDER_ERROR_INCORRECT_MARKET_TYPE\x10\x16\x12%\n!ORDER_ERROR_INVALID_TIME_IN_FORCE\x10\x17\x12\x37\n3ORDER_ERROR_CANNOT_SEND_GFN_ORDER_DURING_AN_AUCTION\x10\x18\x12?\n;ORDER_ERROR_CANNOT_SEND_GFA_ORDER_DURING_CONTINUOUS_TRADING\x10\x19\x12\x34\n0ORDER_ERROR_CANNOT_AMEND_TO_GTT_WITHOUT_EXPIRYAT\x10\x1a\x12)\n%ORDER_ERROR_EXPIRYAT_BEFORE_CREATEDAT\x10\x1b\x12,\n(ORDER_ERROR_CANNOT_HAVE_GTC_AND_EXPIRYAT\x10\x1c\x12*\n&ORDER_ERROR_CANNOT_AMEND_TO_FOK_OR_IOC\x10\x1d\x12*\n&ORDER_ERROR_CANNOT_AMEND_TO_GFA_OR_GFN\x10\x1e\x12,\n(ORDER_ERROR_CANNOT_AMEND_FROM_GFA_OR_GFN\x10\x1f\x12\x34\n0ORDER_ERROR_CANNOT_SEND_IOC_ORDER_DURING_AUCTION\x10 \x12\x34\n0ORDER_ERROR_CANNOT_SEND_FOK_ORDER_DURING_AUCTION\x10!\x12#\n\x1fORDER_ERROR_MUST_BE_LIMIT_ORDER\x10"\x12"\n\x1eORDER_ERROR_MUST_BE_GTT_OR_GTC\x10#\x12\'\n#ORDER_ERROR_WITHOUT_REFERENCE_PRICE\x10$\x12\x33\n/ORDER_ERROR_BUY_CANNOT_REFERENCE_BEST_ASK_PRICE\x10%\x12\x37\n3ORDER_ERROR_OFFSET_MUST_BE_GREATER_OR_EQUAL_TO_ZERO\x10(\x12\x34\n0ORDER_ERROR_SELL_CANNOT_REFERENCE_BEST_BID_PRICE\x10)\x12\x30\n,ORDER_ERROR_OFFSET_MUST_BE_GREATER_THAN_ZERO\x10*\x12*\n&ORDER_ERROR_INSUFFICIENT_ASSET_BALANCE\x10+\x12\x45\nAORDER_ERROR_CANNOT_AMEND_PEGGED_ORDER_DETAILS_ON_NON_PEGGED_ORDER\x10,\x12.\n*ORDER_ERROR_UNABLE_TO_REPRICE_PEGGED_ORDER\x10-\x12\x35\n1ORDER_ERROR_UNABLE_TO_AMEND_PRICE_ON_PEGGED_ORDER\x10.\x12\x38\n4ORDER_ERROR_NON_PERSISTENT_ORDER_OUT_OF_PRICE_BOUNDS\x10/\x12&\n"ORDER_ERROR_TOO_MANY_PEGGED_ORDERS\x10\x30\x12+\n\'ORDER_ERROR_POST_ONLY_ORDER_WOULD_TRADE\x10\x31\x12;\n7ORDER_ERROR_REDUCE_ONLY_ORDER_WOULD_NOT_REDUCE_POSITION\x10\x32"\x04\x08&\x10&"\x04\x08\'\x10\'*\x82\x01\n\x0b\x43hainStatus\x12\x1c\n\x18\x43HAIN_STATUS_UNSPECIFIED\x10\x00\x12\x1d\n\x19\x43HAIN_STATUS_DISCONNECTED\x10\x01\x12\x1a\n\x16\x43HAIN_STATUS_REPLAYING\x10\x02\x12\x1a\n\x16\x43HAIN_STATUS_CONNECTED\x10\x03*\xde\x04\n\x0b\x41\x63\x63ountType\x12\x1c\n\x18\x41\x43\x43OUNT_TYPE_UNSPECIFIED\x10\x00\x12\x1a\n\x16\x41\x43\x43OUNT_TYPE_INSURANCE\x10\x01\x12\x1b\n\x17\x41\x43\x43OUNT_TYPE_SETTLEMENT\x10\x02\x12\x17\n\x13\x41\x43\x43OUNT_TYPE_MARGIN\x10\x03\x12\x18\n\x14\x41\x43\x43OUNT_TYPE_GENERAL\x10\x04\x12$\n ACCOUNT_TYPE_FEES_INFRASTRUCTURE\x10\x05\x12\x1f\n\x1b\x41\x43\x43OUNT_TYPE_FEES_LIQUIDITY\x10\x06\x12\x1b\n\x17\x41\x43\x43OUNT_TYPE_FEES_MAKER\x10\x07\x12\x15\n\x11\x41\x43\x43OUNT_TYPE_BOND\x10\t\x12\x19\n\x15\x41\x43\x43OUNT_TYPE_EXTERNAL\x10\n\x12!\n\x1d\x41\x43\x43OUNT_TYPE_GLOBAL_INSURANCE\x10\x0b\x12\x1e\n\x1a\x41\x43\x43OUNT_TYPE_GLOBAL_REWARD\x10\x0c\x12"\n\x1e\x41\x43\x43OUNT_TYPE_PENDING_TRANSFERS\x10\r\x12\'\n#ACCOUNT_TYPE_REWARD_MAKER_PAID_FEES\x10\x0e\x12+\n\'ACCOUNT_TYPE_REWARD_MAKER_RECEIVED_FEES\x10\x0f\x12(\n$ACCOUNT_TYPE_REWARD_LP_RECEIVED_FEES\x10\x10\x12(\n$ACCOUNT_TYPE_REWARD_MARKET_PROPOSERS\x10\x11\x12\x18\n\x14\x41\x43\x43OUNT_TYPE_HOLDING\x10\x12"\x04\x08\x08\x10\x08*\xd4\x07\n\x0cTransferType\x12\x1d\n\x19TRANSFER_TYPE_UNSPECIFIED\x10\x00\x12\x16\n\x12TRANSFER_TYPE_LOSS\x10\x01\x12\x15\n\x11TRANSFER_TYPE_WIN\x10\x02\x12\x1a\n\x16TRANSFER_TYPE_MTM_LOSS\x10\x04\x12\x19\n\x15TRANSFER_TYPE_MTM_WIN\x10\x05\x12\x1c\n\x18TRANSFER_TYPE_MARGIN_LOW\x10\x06\x12\x1d\n\x19TRANSFER_TYPE_MARGIN_HIGH\x10\x07\x12$\n TRANSFER_TYPE_MARGIN_CONFISCATED\x10\x08\x12\x1f\n\x1bTRANSFER_TYPE_MAKER_FEE_PAY\x10\t\x12#\n\x1fTRANSFER_TYPE_MAKER_FEE_RECEIVE\x10\n\x12(\n$TRANSFER_TYPE_INFRASTRUCTURE_FEE_PAY\x10\x0b\x12/\n+TRANSFER_TYPE_INFRASTRUCTURE_FEE_DISTRIBUTE\x10\x0c\x12#\n\x1fTRANSFER_TYPE_LIQUIDITY_FEE_PAY\x10\r\x12*\n&TRANSFER_TYPE_LIQUIDITY_FEE_DISTRIBUTE\x10\x0e\x12\x1a\n\x16TRANSFER_TYPE_BOND_LOW\x10\x0f\x12\x1b\n\x17TRANSFER_TYPE_BOND_HIGH\x10\x10\x12\x1a\n\x16TRANSFER_TYPE_WITHDRAW\x10\x12\x12\x19\n\x15TRANSFER_TYPE_DEPOSIT\x10\x13\x12\x1f\n\x1bTRANSFER_TYPE_BOND_SLASHING\x10\x14\x12\x1f\n\x1bTRANSFER_TYPE_REWARD_PAYOUT\x10\x15\x12%\n!TRANSFER_TYPE_TRANSFER_FUNDS_SEND\x10\x16\x12+\n\'TRANSFER_TYPE_TRANSFER_FUNDS_DISTRIBUTE\x10\x17\x12\x1f\n\x1bTRANSFER_TYPE_CLEAR_ACCOUNT\x10\x18\x12,\n(TRANSFER_TYPE_CHECKPOINT_BALANCE_RESTORE\x10\x19\x12\x16\n\x12TRANSFER_TYPE_SPOT\x10\x1a\x12\x1e\n\x1aTRANSFER_TYPE_HOLDING_LOCK\x10\x1b\x12!\n\x1dTRANSFER_TYPE_HOLDING_RELEASE\x10\x1c\x12.\n*TRANSFER_TYPE_SUCCESSOR_INSURANCE_FRACTION\x10\x1d"\x04\x08\x03\x10\x03"\x04\x08\x11\x10\x11*\xc7\x01\n\x0e\x44ispatchMetric\x12\x1f\n\x1b\x44ISPATCH_METRIC_UNSPECIFIED\x10\x00\x12#\n\x1f\x44ISPATCH_METRIC_MAKER_FEES_PAID\x10\x01\x12\'\n#DISPATCH_METRIC_MAKER_FEES_RECEIVED\x10\x02\x12$\n DISPATCH_METRIC_LP_FEES_RECEIVED\x10\x03\x12 \n\x1c\x44ISPATCH_METRIC_MARKET_VALUE\x10\x04*c\n\nNodeStatus\x12\x1b\n\x17NODE_STATUS_UNSPECIFIED\x10\x00\x12\x19\n\x15NODE_STATUS_VALIDATOR\x10\x01\x12\x1d\n\x19NODE_STATUS_NON_VALIDATOR\x10\x02*Y\n\x0b\x45pochAction\x12\x1c\n\x18\x45POCH_ACTION_UNSPECIFIED\x10\x00\x12\x16\n\x12\x45POCH_ACTION_START\x10\x01\x12\x14\n\x10\x45POCH_ACTION_END\x10\x02*\xa7\x01\n\x13ValidatorNodeStatus\x12%\n!VALIDATOR_NODE_STATUS_UNSPECIFIED\x10\x00\x12$\n VALIDATOR_NODE_STATUS_TENDERMINT\x10\x01\x12 \n\x1cVALIDATOR_NODE_STATUS_ERSATZ\x10\x02\x12!\n\x1dVALIDATOR_NODE_STATUS_PENDING\x10\x03\x42\'Z%code.vegaprotocol.io/vega/protos/vegab\x06proto3'
 )
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "vega.vega_pb2", globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "vega.vega_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b"Z%code.vegaprotocol.io/vega/protos/vega"
-    _SIDE._serialized_start = 13733
-    _SIDE._serialized_end = 13790
-    _INTERVAL._serialized_start = 13793
-    _INTERVAL._serialized_end = 13974
-    _POSITIONSTATUS._serialized_start = 13977
-    _POSITIONSTATUS._serialized_end = 14125
-    _AUCTIONTRIGGER._serialized_start = 14128
-    _AUCTIONTRIGGER._serialized_end = 14385
-    _PEGGEDREFERENCE._serialized_start = 14388
-    _PEGGEDREFERENCE._serialized_end = 14527
-    _ORDERERROR._serialized_start = 14530
-    _ORDERERROR._serialized_end = 16651
-    _CHAINSTATUS._serialized_start = 16654
-    _CHAINSTATUS._serialized_end = 16784
-    _ACCOUNTTYPE._serialized_start = 16787
-    _ACCOUNTTYPE._serialized_end = 17367
-    _TRANSFERTYPE._serialized_start = 17370
-    _TRANSFERTYPE._serialized_end = 18211
-    _DISPATCHMETRIC._serialized_start = 18214
-    _DISPATCHMETRIC._serialized_end = 18413
-    _NODESTATUS._serialized_start = 18415
-    _NODESTATUS._serialized_end = 18514
-    _EPOCHACTION._serialized_start = 18516
-    _EPOCHACTION._serialized_end = 18605
-    _VALIDATORNODESTATUS._serialized_start = 18608
-    _VALIDATORNODESTATUS._serialized_end = 18775
-    _PARTY._serialized_start = 45
-    _PARTY._serialized_end = 68
-    _RISKFACTOR._serialized_start = 70
-    _RISKFACTOR._serialized_end = 148
-    _PEGGEDORDER._serialized_start = 150
-    _PEGGEDORDER._serialized_end = 240
-    _ORDER._serialized_start = 243
-    _ORDER._serialized_end = 1443
-    _ORDER_TIMEINFORCE._serialized_start = 965
-    _ORDER_TIMEINFORCE._serialized_end = 1147
-    _ORDER_TYPE._serialized_start = 1149
-    _ORDER_TYPE._serialized_end = 1228
-    _ORDER_STATUS._serialized_start = 1231
-    _ORDER_STATUS._serialized_end = 1432
-    _ORDERCANCELLATIONCONFIRMATION._serialized_start = 1445
-    _ORDERCANCELLATIONCONFIRMATION._serialized_end = 1511
-    _ORDERCONFIRMATION._serialized_start = 1514
-    _ORDERCONFIRMATION._serialized_end = 1674
-    _AUCTIONINDICATIVESTATE._serialized_start = 1677
-    _AUCTIONINDICATIVESTATE._serialized_end = 1888
-    _TRADE._serialized_start = 1891
-    _TRADE._serialized_end = 2494
-    _TRADE_TYPE._serialized_start = 2383
-    _TRADE_TYPE._serialized_end = 2494
-    _FEE._serialized_start = 2496
-    _FEE._serialized_end = 2614
-    _TRADESET._serialized_start = 2616
-    _TRADESET._serialized_end = 2663
-    _CANDLE._serialized_start = 2666
-    _CANDLE._serialized_end = 2880
-    _PRICELEVEL._serialized_start = 2882
-    _PRICELEVEL._serialized_end = 2982
-    _MARKETDEPTH._serialized_start = 2985
-    _MARKETDEPTH._serialized_end = 3142
-    _MARKETDEPTHUPDATE._serialized_start = 3145
-    _MARKETDEPTHUPDATE._serialized_end = 3366
-    _POSITION._serialized_start = 3369
-    _POSITION._serialized_end = 3744
-    _POSITIONTRADE._serialized_start = 3746
-    _POSITIONTRADE._serialized_end = 3807
-    _DEPOSIT._serialized_start = 3810
-    _DEPOSIT._serialized_end = 4166
-    _DEPOSIT_STATUS._serialized_start = 4073
-    _DEPOSIT_STATUS._serialized_end = 4166
-    _WITHDRAWAL._serialized_start = 4169
-    _WITHDRAWAL._serialized_end = 4593
-    _WITHDRAWAL_STATUS._serialized_start = 4495
-    _WITHDRAWAL_STATUS._serialized_end = 4587
-    _WITHDRAWEXT._serialized_start = 4595
-    _WITHDRAWEXT._serialized_end = 4663
-    _ERC20WITHDRAWEXT._serialized_start = 4665
-    _ERC20WITHDRAWEXT._serialized_end = 4726
-    _ACCOUNT._serialized_start = 4729
-    _ACCOUNT._serialized_end = 4892
-    _FINANCIALAMOUNT._serialized_start = 4894
-    _FINANCIALAMOUNT._serialized_end = 4957
-    _TRANSFER._serialized_start = 4960
-    _TRANSFER._serialized_end = 5139
-    _DISPATCHSTRATEGY._serialized_start = 5142
-    _DISPATCHSTRATEGY._serialized_end = 5274
-    _TRANSFERREQUEST._serialized_start = 5277
-    _TRANSFERREQUEST._serialized_end = 5507
-    _ACCOUNTDETAILS._serialized_start = 5510
-    _ACCOUNTDETAILS._serialized_end = 5677
-    _LEDGERENTRY._serialized_start = 5680
-    _LEDGERENTRY._serialized_end = 5993
-    _POSTTRANSFERBALANCE._serialized_start = 5995
-    _POSTTRANSFERBALANCE._serialized_end = 6090
-    _LEDGERMOVEMENT._serialized_start = 6092
-    _LEDGERMOVEMENT._serialized_end = 6208
-    _MARGINLEVELS._serialized_start = 6211
-    _MARGINLEVELS._serialized_end = 6512
-    _MARKETDATA._serialized_start = 6515
-    _MARKETDATA._serialized_end = 7896
-    _LIQUIDITYPROVIDERFEESHARE._serialized_start = 7899
-    _LIQUIDITYPROVIDERFEESHARE._serialized_end = 8085
-    _PRICEMONITORINGBOUNDS._serialized_start = 8088
-    _PRICEMONITORINGBOUNDS._serialized_end = 8288
-    _ERRORDETAIL._serialized_start = 8290
-    _ERRORDETAIL._serialized_end = 8371
-    _NETWORKPARAMETER._serialized_start = 8373
-    _NETWORKPARAMETER._serialized_end = 8431
-    _NETWORKLIMITS._serialized_start = 8434
-    _NETWORKLIMITS._serialized_end = 8820
-    _LIQUIDITYORDER._serialized_start = 8822
-    _LIQUIDITYORDER._serialized_end = 8947
-    _LIQUIDITYORDERREFERENCE._serialized_start = 8949
-    _LIQUIDITYORDERREFERENCE._serialized_end = 9064
-    _LIQUIDITYPROVISION._serialized_start = 9067
-    _LIQUIDITYPROVISION._serialized_end = 9661
-    _LIQUIDITYPROVISION_STATUS._serialized_start = 9504
-    _LIQUIDITYPROVISION_STATUS._serialized_end = 9661
-    _ETHEREUMCONFIG._serialized_start = 9664
-    _ETHEREUMCONFIG._serialized_end = 10128
-    _ETHEREUMCONTRACTCONFIG._serialized_start = 10130
-    _ETHEREUMCONTRACTCONFIG._serialized_end = 10236
-    _EPOCHTIMESTAMPS._serialized_start = 10239
-    _EPOCHTIMESTAMPS._serialized_end = 10411
-    _EPOCH._serialized_start = 10414
-    _EPOCH._serialized_end = 10590
-    _EPOCHPARTICIPATION._serialized_start = 10593
-    _EPOCHPARTICIPATION._serialized_end = 10735
-    _EPOCHDATA._serialized_start = 10737
-    _EPOCHDATA._serialized_end = 10820
-    _RANKINGSCORE._serialized_start = 10823
-    _RANKINGSCORE._serialized_end = 11106
-    _REWARDSCORE._serialized_start = 11109
-    _REWARDSCORE._serialized_end = 11408
-    _NODE._serialized_start = 11411
-    _NODE._serialized_end = 12102
-    _NODESET._serialized_start = 12105
-    _NODESET._serialized_end = 12261
-    _NODEDATA._serialized_start = 12264
-    _NODEDATA._serialized_end = 12565
-    _DELEGATION._serialized_start = 12567
-    _DELEGATION._serialized_end = 12679
-    _REWARD._serialized_start = 12682
-    _REWARD._serialized_end = 12933
-    _REWARDSUMMARY._serialized_start = 12935
-    _REWARDSUMMARY._serialized_end = 13028
-    _EPOCHREWARDSUMMARY._serialized_start = 13031
-    _EPOCHREWARDSUMMARY._serialized_end = 13186
-    _STATEVALUEPROPOSAL._serialized_start = 13188
-    _STATEVALUEPROPOSAL._serialized_end = 13309
-    _KEYVALUEBUNDLE._serialized_start = 13311
-    _KEYVALUEBUNDLE._serialized_end = 13418
-    _STATEVARVALUE._serialized_start = 13421
-    _STATEVARVALUE._serialized_end = 13601
-    _SCALARVALUE._serialized_start = 13603
-    _SCALARVALUE._serialized_end = 13638
-    _VECTORVALUE._serialized_start = 13640
-    _VECTORVALUE._serialized_end = 13675
-    _MATRIXVALUE._serialized_start = 13677
-    _MATRIXVALUE._serialized_end = 13731
+    _globals["_SIDE"]._serialized_start = 14985
+    _globals["_SIDE"]._serialized_end = 15042
+    _globals["_INTERVAL"]._serialized_start = 15045
+    _globals["_INTERVAL"]._serialized_end = 15226
+    _globals["_POSITIONSTATUS"]._serialized_start = 15229
+    _globals["_POSITIONSTATUS"]._serialized_end = 15377
+    _globals["_AUCTIONTRIGGER"]._serialized_start = 15380
+    _globals["_AUCTIONTRIGGER"]._serialized_end = 15637
+    _globals["_PEGGEDREFERENCE"]._serialized_start = 15640
+    _globals["_PEGGEDREFERENCE"]._serialized_end = 15779
+    _globals["_ORDERERROR"]._serialized_start = 15782
+    _globals["_ORDERERROR"]._serialized_end = 17903
+    _globals["_CHAINSTATUS"]._serialized_start = 17906
+    _globals["_CHAINSTATUS"]._serialized_end = 18036
+    _globals["_ACCOUNTTYPE"]._serialized_start = 18039
+    _globals["_ACCOUNTTYPE"]._serialized_end = 18645
+    _globals["_TRANSFERTYPE"]._serialized_start = 18648
+    _globals["_TRANSFERTYPE"]._serialized_end = 19628
+    _globals["_DISPATCHMETRIC"]._serialized_start = 19631
+    _globals["_DISPATCHMETRIC"]._serialized_end = 19830
+    _globals["_NODESTATUS"]._serialized_start = 19832
+    _globals["_NODESTATUS"]._serialized_end = 19931
+    _globals["_EPOCHACTION"]._serialized_start = 19933
+    _globals["_EPOCHACTION"]._serialized_end = 20022
+    _globals["_VALIDATORNODESTATUS"]._serialized_start = 20025
+    _globals["_VALIDATORNODESTATUS"]._serialized_end = 20192
+    _globals["_STOPORDER"]._serialized_start = 46
+    _globals["_STOPORDER"]._serialized_end = 998
+    _globals["_STOPORDER_EXPIRYSTRATEGY"]._serialized_start = 551
+    _globals["_STOPORDER_EXPIRYSTRATEGY"]._serialized_end = 657
+    _globals["_STOPORDER_TRIGGERDIRECTION"]._serialized_start = 659
+    _globals["_STOPORDER_TRIGGERDIRECTION"]._serialized_end = 782
+    _globals["_STOPORDER_STATUS"]._serialized_start = 785
+    _globals["_STOPORDER_STATUS"]._serialized_end = 921
+    _globals["_PARTY"]._serialized_start = 1000
+    _globals["_PARTY"]._serialized_end = 1023
+    _globals["_RISKFACTOR"]._serialized_start = 1025
+    _globals["_RISKFACTOR"]._serialized_end = 1103
+    _globals["_PEGGEDORDER"]._serialized_start = 1105
+    _globals["_PEGGEDORDER"]._serialized_end = 1195
+    _globals["_ICEBERGORDER"]._serialized_start = 1198
+    _globals["_ICEBERGORDER"]._serialized_end = 1338
+    _globals["_ORDER"]._serialized_start = 1341
+    _globals["_ORDER"]._serialized_end = 2621
+    _globals["_ORDER_TIMEINFORCE"]._serialized_start = 2125
+    _globals["_ORDER_TIMEINFORCE"]._serialized_end = 2307
+    _globals["_ORDER_TYPE"]._serialized_start = 2309
+    _globals["_ORDER_TYPE"]._serialized_end = 2388
+    _globals["_ORDER_STATUS"]._serialized_start = 2391
+    _globals["_ORDER_STATUS"]._serialized_end = 2592
+    _globals["_ORDERCANCELLATIONCONFIRMATION"]._serialized_start = 2623
+    _globals["_ORDERCANCELLATIONCONFIRMATION"]._serialized_end = 2689
+    _globals["_ORDERCONFIRMATION"]._serialized_start = 2692
+    _globals["_ORDERCONFIRMATION"]._serialized_end = 2852
+    _globals["_AUCTIONINDICATIVESTATE"]._serialized_start = 2855
+    _globals["_AUCTIONINDICATIVESTATE"]._serialized_end = 3066
+    _globals["_TRADE"]._serialized_start = 3069
+    _globals["_TRADE"]._serialized_end = 3672
+    _globals["_TRADE_TYPE"]._serialized_start = 3561
+    _globals["_TRADE_TYPE"]._serialized_end = 3672
+    _globals["_FEE"]._serialized_start = 3674
+    _globals["_FEE"]._serialized_end = 3792
+    _globals["_TRADESET"]._serialized_start = 3794
+    _globals["_TRADESET"]._serialized_end = 3841
+    _globals["_CANDLE"]._serialized_start = 3844
+    _globals["_CANDLE"]._serialized_end = 4058
+    _globals["_PRICELEVEL"]._serialized_start = 4060
+    _globals["_PRICELEVEL"]._serialized_end = 4160
+    _globals["_MARKETDEPTH"]._serialized_start = 4163
+    _globals["_MARKETDEPTH"]._serialized_end = 4320
+    _globals["_MARKETDEPTHUPDATE"]._serialized_start = 4323
+    _globals["_MARKETDEPTHUPDATE"]._serialized_end = 4544
+    _globals["_POSITION"]._serialized_start = 4547
+    _globals["_POSITION"]._serialized_end = 4922
+    _globals["_POSITIONTRADE"]._serialized_start = 4924
+    _globals["_POSITIONTRADE"]._serialized_end = 4985
+    _globals["_DEPOSIT"]._serialized_start = 4988
+    _globals["_DEPOSIT"]._serialized_end = 5344
+    _globals["_DEPOSIT_STATUS"]._serialized_start = 5251
+    _globals["_DEPOSIT_STATUS"]._serialized_end = 5344
+    _globals["_WITHDRAWAL"]._serialized_start = 5347
+    _globals["_WITHDRAWAL"]._serialized_end = 5771
+    _globals["_WITHDRAWAL_STATUS"]._serialized_start = 5673
+    _globals["_WITHDRAWAL_STATUS"]._serialized_end = 5765
+    _globals["_WITHDRAWEXT"]._serialized_start = 5773
+    _globals["_WITHDRAWEXT"]._serialized_end = 5841
+    _globals["_ERC20WITHDRAWEXT"]._serialized_start = 5843
+    _globals["_ERC20WITHDRAWEXT"]._serialized_end = 5904
+    _globals["_ACCOUNT"]._serialized_start = 5907
+    _globals["_ACCOUNT"]._serialized_end = 6070
+    _globals["_FINANCIALAMOUNT"]._serialized_start = 6072
+    _globals["_FINANCIALAMOUNT"]._serialized_end = 6135
+    _globals["_TRANSFER"]._serialized_start = 6138
+    _globals["_TRANSFER"]._serialized_end = 6317
+    _globals["_DISPATCHSTRATEGY"]._serialized_start = 6320
+    _globals["_DISPATCHSTRATEGY"]._serialized_end = 6452
+    _globals["_TRANSFERREQUEST"]._serialized_start = 6455
+    _globals["_TRANSFERREQUEST"]._serialized_end = 6685
+    _globals["_ACCOUNTDETAILS"]._serialized_start = 6688
+    _globals["_ACCOUNTDETAILS"]._serialized_end = 6855
+    _globals["_LEDGERENTRY"]._serialized_start = 6858
+    _globals["_LEDGERENTRY"]._serialized_end = 7171
+    _globals["_POSTTRANSFERBALANCE"]._serialized_start = 7173
+    _globals["_POSTTRANSFERBALANCE"]._serialized_end = 7268
+    _globals["_LEDGERMOVEMENT"]._serialized_start = 7270
+    _globals["_LEDGERMOVEMENT"]._serialized_end = 7386
+    _globals["_MARGINLEVELS"]._serialized_start = 7389
+    _globals["_MARGINLEVELS"]._serialized_end = 7690
+    _globals["_MARKETDATA"]._serialized_start = 7693
+    _globals["_MARKETDATA"]._serialized_end = 9111
+    _globals["_LIQUIDITYPROVIDERFEESHARE"]._serialized_start = 9114
+    _globals["_LIQUIDITYPROVIDERFEESHARE"]._serialized_end = 9337
+    _globals["_PRICEMONITORINGBOUNDS"]._serialized_start = 9340
+    _globals["_PRICEMONITORINGBOUNDS"]._serialized_end = 9540
+    _globals["_ERRORDETAIL"]._serialized_start = 9542
+    _globals["_ERRORDETAIL"]._serialized_end = 9623
+    _globals["_NETWORKPARAMETER"]._serialized_start = 9625
+    _globals["_NETWORKPARAMETER"]._serialized_end = 9683
+    _globals["_NETWORKLIMITS"]._serialized_start = 9686
+    _globals["_NETWORKLIMITS"]._serialized_end = 10072
+    _globals["_LIQUIDITYORDER"]._serialized_start = 10074
+    _globals["_LIQUIDITYORDER"]._serialized_end = 10199
+    _globals["_LIQUIDITYORDERREFERENCE"]._serialized_start = 10201
+    _globals["_LIQUIDITYORDERREFERENCE"]._serialized_end = 10316
+    _globals["_LIQUIDITYPROVISION"]._serialized_start = 10319
+    _globals["_LIQUIDITYPROVISION"]._serialized_end = 10913
+    _globals["_LIQUIDITYPROVISION_STATUS"]._serialized_start = 10756
+    _globals["_LIQUIDITYPROVISION_STATUS"]._serialized_end = 10913
+    _globals["_ETHEREUMCONFIG"]._serialized_start = 10916
+    _globals["_ETHEREUMCONFIG"]._serialized_end = 11380
+    _globals["_ETHEREUMCONTRACTCONFIG"]._serialized_start = 11382
+    _globals["_ETHEREUMCONTRACTCONFIG"]._serialized_end = 11488
+    _globals["_EPOCHTIMESTAMPS"]._serialized_start = 11491
+    _globals["_EPOCHTIMESTAMPS"]._serialized_end = 11663
+    _globals["_EPOCH"]._serialized_start = 11666
+    _globals["_EPOCH"]._serialized_end = 11842
+    _globals["_EPOCHPARTICIPATION"]._serialized_start = 11845
+    _globals["_EPOCHPARTICIPATION"]._serialized_end = 11987
+    _globals["_EPOCHDATA"]._serialized_start = 11989
+    _globals["_EPOCHDATA"]._serialized_end = 12072
+    _globals["_RANKINGSCORE"]._serialized_start = 12075
+    _globals["_RANKINGSCORE"]._serialized_end = 12358
+    _globals["_REWARDSCORE"]._serialized_start = 12361
+    _globals["_REWARDSCORE"]._serialized_end = 12660
+    _globals["_NODE"]._serialized_start = 12663
+    _globals["_NODE"]._serialized_end = 13354
+    _globals["_NODESET"]._serialized_start = 13357
+    _globals["_NODESET"]._serialized_end = 13513
+    _globals["_NODEDATA"]._serialized_start = 13516
+    _globals["_NODEDATA"]._serialized_end = 13817
+    _globals["_DELEGATION"]._serialized_start = 13819
+    _globals["_DELEGATION"]._serialized_end = 13931
+    _globals["_REWARD"]._serialized_start = 13934
+    _globals["_REWARD"]._serialized_end = 14185
+    _globals["_REWARDSUMMARY"]._serialized_start = 14187
+    _globals["_REWARDSUMMARY"]._serialized_end = 14280
+    _globals["_EPOCHREWARDSUMMARY"]._serialized_start = 14283
+    _globals["_EPOCHREWARDSUMMARY"]._serialized_end = 14438
+    _globals["_STATEVALUEPROPOSAL"]._serialized_start = 14440
+    _globals["_STATEVALUEPROPOSAL"]._serialized_end = 14561
+    _globals["_KEYVALUEBUNDLE"]._serialized_start = 14563
+    _globals["_KEYVALUEBUNDLE"]._serialized_end = 14670
+    _globals["_STATEVARVALUE"]._serialized_start = 14673
+    _globals["_STATEVARVALUE"]._serialized_end = 14853
+    _globals["_SCALARVALUE"]._serialized_start = 14855
+    _globals["_SCALARVALUE"]._serialized_end = 14890
+    _globals["_VECTORVALUE"]._serialized_start = 14892
+    _globals["_VECTORVALUE"]._serialized_end = 14927
+    _globals["_MATRIXVALUE"]._serialized_start = 14929
+    _globals["_MATRIXVALUE"]._serialized_end = 14983
 # @@protoc_insertion_point(module_scope)
```

### Comparing `vega_sim-1.1.1/vega_sim/proto/vega/wallet/v1/wallet_pb2.py` & `vega_sim-1.2.0/vega_sim/proto/vega/wallet/v1/wallet_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: vega/wallet/v1/wallet.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from ...commands.v1 import commands_pb2 as vega_dot_commands_dot_v1_dot_commands__pb2
 from ...commands.v1 import data_pb2 as vega_dot_commands_dot_v1_dot_data__pb2
 from ...commands.v1 import (
     validator_commands_pb2 as vega_dot_commands_dot_v1_dot_validator__commands__pb2,
 )
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b"\n\x1bvega/wallet/v1/wallet.proto\x12\x0evega.wallet.v1\x1a\x1fvega/commands/v1/commands.proto\x1a\x1bvega/commands/v1/data.proto\x1a)vega/commands/v1/validator_commands.proto\"\xb7\x12\n\x18SubmitTransactionRequest\x12\x17\n\x07pub_key\x18\x01 \x01(\tR\x06pubKey\x12\x1c\n\tpropagate\x18\x02 \x01(\x08R\tpropagate\x12O\n\x10order_submission\x18\xe9\x07 \x01(\x0b\x32!.vega.commands.v1.OrderSubmissionH\x00R\x0forderSubmission\x12U\n\x12order_cancellation\x18\xea\x07 \x01(\x0b\x32#.vega.commands.v1.OrderCancellationH\x00R\x11orderCancellation\x12L\n\x0forder_amendment\x18\xeb\x07 \x01(\x0b\x32 .vega.commands.v1.OrderAmendmentH\x00R\x0eorderAmendment\x12X\n\x13withdraw_submission\x18\xec\x07 \x01(\x0b\x32$.vega.commands.v1.WithdrawSubmissionH\x00R\x12withdrawSubmission\x12X\n\x13proposal_submission\x18\xed\x07 \x01(\x0b\x32$.vega.commands.v1.ProposalSubmissionH\x00R\x12proposalSubmission\x12L\n\x0fvote_submission\x18\xee\x07 \x01(\x0b\x32 .vega.commands.v1.VoteSubmissionH\x00R\x0evoteSubmission\x12w\n\x1eliquidity_provision_submission\x18\xef\x07 \x01(\x0b\x32..vega.commands.v1.LiquidityProvisionSubmissionH\x00R\x1cliquidityProvisionSubmission\x12X\n\x13\x64\x65legate_submission\x18\xf0\x07 \x01(\x0b\x32$.vega.commands.v1.DelegateSubmissionH\x00R\x12\x64\x65legateSubmission\x12^\n\x15undelegate_submission\x18\xf1\x07 \x01(\x0b\x32&.vega.commands.v1.UndelegateSubmissionH\x00R\x14undelegateSubmission\x12}\n liquidity_provision_cancellation\x18\xf2\x07 \x01(\x0b\x32\x30.vega.commands.v1.LiquidityProvisionCancellationH\x00R\x1eliquidityProvisionCancellation\x12t\n\x1dliquidity_provision_amendment\x18\xf3\x07 \x01(\x0b\x32-.vega.commands.v1.LiquidityProvisionAmendmentH\x00R\x1bliquidityProvisionAmendment\x12\x39\n\x08transfer\x18\xf4\x07 \x01(\x0b\x32\x1a.vega.commands.v1.TransferH\x00R\x08transfer\x12L\n\x0f\x63\x61ncel_transfer\x18\xf5\x07 \x01(\x0b\x32 .vega.commands.v1.CancelTransferH\x00R\x0e\x63\x61ncelTransfer\x12\x46\n\rannounce_node\x18\xf6\x07 \x01(\x0b\x32\x1e.vega.commands.v1.AnnounceNodeH\x00R\x0c\x61nnounceNode\x12h\n\x19\x62\x61tch_market_instructions\x18\xf7\x07 \x01(\x0b\x32).vega.commands.v1.BatchMarketInstructionsH\x00R\x17\x62\x61tchMarketInstructions\x12:\n\tnode_vote\x18\xd2\x0f \x01(\x0b\x32\x1a.vega.commands.v1.NodeVoteH\x00R\x08nodeVote\x12I\n\x0enode_signature\x18\xd3\x0f \x01(\x0b\x32\x1f.vega.commands.v1.NodeSignatureH\x00R\rnodeSignature\x12@\n\x0b\x63hain_event\x18\xd4\x0f \x01(\x0b\x32\x1c.vega.commands.v1.ChainEventH\x00R\nchainEvent\x12\\\n\x15key_rotate_submission\x18\xd5\x0f \x01(\x0b\x32%.vega.commands.v1.KeyRotateSubmissionH\x00R\x13keyRotateSubmission\x12\x62\n\x17state_variable_proposal\x18\xd6\x0f \x01(\x0b\x32'.vega.commands.v1.StateVariableProposalH\x00R\x15stateVariableProposal\x12X\n\x13validator_heartbeat\x18\xd7\x0f \x01(\x0b\x32$.vega.commands.v1.ValidatorHeartbeatH\x00R\x12validatorHeartbeat\x12u\n\x1e\x65thereum_key_rotate_submission\x18\xd8\x0f \x01(\x0b\x32-.vega.commands.v1.EthereumKeyRotateSubmissionH\x00R\x1b\x65thereumKeyRotateSubmission\x12h\n\x19protocol_upgrade_proposal\x18\xd9\x0f \x01(\x0b\x32).vega.commands.v1.ProtocolUpgradeProposalH\x00R\x17protocolUpgradeProposal\x12O\n\x10issue_signatures\x18\xda\x0f \x01(\x0b\x32!.vega.commands.v1.IssueSignaturesH\x00R\x0fissueSignatures\x12_\n\x16oracle_data_submission\x18\xb9\x17 \x01(\x0b\x32&.vega.commands.v1.OracleDataSubmissionH\x00R\x14oracleDataSubmissionB\t\n\x07\x63ommandJ\x06\x08\xd1\x0f\x10\xd2\x0f\x42\x31Z/code.vegaprotocol.io/vega/protos/vega/wallet/v1b\x06proto3"
+    b"\n\x1bvega/wallet/v1/wallet.proto\x12\x0evega.wallet.v1\x1a\x1fvega/commands/v1/commands.proto\x1a\x1bvega/commands/v1/data.proto\x1a)vega/commands/v1/validator_commands.proto\"\xff\x13\n\x18SubmitTransactionRequest\x12\x17\n\x07pub_key\x18\x01 \x01(\tR\x06pubKey\x12\x1c\n\tpropagate\x18\x02 \x01(\x08R\tpropagate\x12O\n\x10order_submission\x18\xe9\x07 \x01(\x0b\x32!.vega.commands.v1.OrderSubmissionH\x00R\x0forderSubmission\x12U\n\x12order_cancellation\x18\xea\x07 \x01(\x0b\x32#.vega.commands.v1.OrderCancellationH\x00R\x11orderCancellation\x12L\n\x0forder_amendment\x18\xeb\x07 \x01(\x0b\x32 .vega.commands.v1.OrderAmendmentH\x00R\x0eorderAmendment\x12X\n\x13withdraw_submission\x18\xec\x07 \x01(\x0b\x32$.vega.commands.v1.WithdrawSubmissionH\x00R\x12withdrawSubmission\x12X\n\x13proposal_submission\x18\xed\x07 \x01(\x0b\x32$.vega.commands.v1.ProposalSubmissionH\x00R\x12proposalSubmission\x12L\n\x0fvote_submission\x18\xee\x07 \x01(\x0b\x32 .vega.commands.v1.VoteSubmissionH\x00R\x0evoteSubmission\x12w\n\x1eliquidity_provision_submission\x18\xef\x07 \x01(\x0b\x32..vega.commands.v1.LiquidityProvisionSubmissionH\x00R\x1cliquidityProvisionSubmission\x12X\n\x13\x64\x65legate_submission\x18\xf0\x07 \x01(\x0b\x32$.vega.commands.v1.DelegateSubmissionH\x00R\x12\x64\x65legateSubmission\x12^\n\x15undelegate_submission\x18\xf1\x07 \x01(\x0b\x32&.vega.commands.v1.UndelegateSubmissionH\x00R\x14undelegateSubmission\x12}\n liquidity_provision_cancellation\x18\xf2\x07 \x01(\x0b\x32\x30.vega.commands.v1.LiquidityProvisionCancellationH\x00R\x1eliquidityProvisionCancellation\x12t\n\x1dliquidity_provision_amendment\x18\xf3\x07 \x01(\x0b\x32-.vega.commands.v1.LiquidityProvisionAmendmentH\x00R\x1bliquidityProvisionAmendment\x12\x39\n\x08transfer\x18\xf4\x07 \x01(\x0b\x32\x1a.vega.commands.v1.TransferH\x00R\x08transfer\x12L\n\x0f\x63\x61ncel_transfer\x18\xf5\x07 \x01(\x0b\x32 .vega.commands.v1.CancelTransferH\x00R\x0e\x63\x61ncelTransfer\x12\x46\n\rannounce_node\x18\xf6\x07 \x01(\x0b\x32\x1e.vega.commands.v1.AnnounceNodeH\x00R\x0c\x61nnounceNode\x12h\n\x19\x62\x61tch_market_instructions\x18\xf7\x07 \x01(\x0b\x32).vega.commands.v1.BatchMarketInstructionsH\x00R\x17\x62\x61tchMarketInstructions\x12_\n\x16stop_orders_submission\x18\xf8\x07 \x01(\x0b\x32&.vega.commands.v1.StopOrdersSubmissionH\x00R\x14stopOrdersSubmission\x12\x65\n\x18stop_orders_cancellation\x18\xf9\x07 \x01(\x0b\x32(.vega.commands.v1.StopOrdersCancellationH\x00R\x16stopOrdersCancellation\x12:\n\tnode_vote\x18\xd2\x0f \x01(\x0b\x32\x1a.vega.commands.v1.NodeVoteH\x00R\x08nodeVote\x12I\n\x0enode_signature\x18\xd3\x0f \x01(\x0b\x32\x1f.vega.commands.v1.NodeSignatureH\x00R\rnodeSignature\x12@\n\x0b\x63hain_event\x18\xd4\x0f \x01(\x0b\x32\x1c.vega.commands.v1.ChainEventH\x00R\nchainEvent\x12\\\n\x15key_rotate_submission\x18\xd5\x0f \x01(\x0b\x32%.vega.commands.v1.KeyRotateSubmissionH\x00R\x13keyRotateSubmission\x12\x62\n\x17state_variable_proposal\x18\xd6\x0f \x01(\x0b\x32'.vega.commands.v1.StateVariableProposalH\x00R\x15stateVariableProposal\x12X\n\x13validator_heartbeat\x18\xd7\x0f \x01(\x0b\x32$.vega.commands.v1.ValidatorHeartbeatH\x00R\x12validatorHeartbeat\x12u\n\x1e\x65thereum_key_rotate_submission\x18\xd8\x0f \x01(\x0b\x32-.vega.commands.v1.EthereumKeyRotateSubmissionH\x00R\x1b\x65thereumKeyRotateSubmission\x12h\n\x19protocol_upgrade_proposal\x18\xd9\x0f \x01(\x0b\x32).vega.commands.v1.ProtocolUpgradeProposalH\x00R\x17protocolUpgradeProposal\x12O\n\x10issue_signatures\x18\xda\x0f \x01(\x0b\x32!.vega.commands.v1.IssueSignaturesH\x00R\x0fissueSignatures\x12_\n\x16oracle_data_submission\x18\xb9\x17 \x01(\x0b\x32&.vega.commands.v1.OracleDataSubmissionH\x00R\x14oracleDataSubmissionB\t\n\x07\x63ommandJ\x06\x08\xd1\x0f\x10\xd2\x0f\x42\x31Z/code.vegaprotocol.io/vega/protos/vega/wallet/v1b\x06proto3"
 )
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(
-    DESCRIPTOR, "vega.wallet.v1.wallet_pb2", globals()
+    DESCRIPTOR, "vega.wallet.v1.wallet_pb2", _globals
 )
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = (
         b"Z/code.vegaprotocol.io/vega/protos/vega/wallet/v1"
     )
-    _SUBMITTRANSACTIONREQUEST._serialized_start = 153
-    _SUBMITTRANSACTIONREQUEST._serialized_end = 2512
+    _globals["_SUBMITTRANSACTIONREQUEST"]._serialized_start = 153
+    _globals["_SUBMITTRANSACTIONREQUEST"]._serialized_end = 2712
 # @@protoc_insertion_point(module_scope)
```

### Comparing `vega_sim-1.1.1/vega_sim/quant/quant.py` & `vega_sim-1.2.0/vega_sim/quant/quant.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/reinforcement/agents/learning_agent.py` & `vega_sim-1.2.0/vega_sim/reinforcement/agents/learning_agent.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/reinforcement/agents/learning_agent_MO.py` & `vega_sim-1.2.0/vega_sim/reinforcement/agents/learning_agent_MO.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/reinforcement/agents/learning_agent_MO_with_vol.py` & `vega_sim-1.2.0/vega_sim/reinforcement/agents/learning_agent_MO_with_vol.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/reinforcement/agents/learning_agent_heuristic.py` & `vega_sim-1.2.0/vega_sim/reinforcement/agents/learning_agent_heuristic.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/reinforcement/agents/simple_agent.py` & `vega_sim-1.2.0/vega_sim/reinforcement/agents/simple_agent.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/reinforcement/distributions.py` & `vega_sim-1.2.0/vega_sim/reinforcement/distributions.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/reinforcement/full_market_sim/environments.py` & `vega_sim-1.2.0/vega_sim/reinforcement/full_market_sim/environments.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/reinforcement/full_market_sim/utils/create_csv.py` & `vega_sim-1.2.0/vega_sim/reinforcement/full_market_sim/utils/create_csv.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/reinforcement/full_market_sim/utils/external_assetprice.py` & `vega_sim-1.2.0/vega_sim/reinforcement/full_market_sim/utils/external_assetprice.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/reinforcement/full_market_sim/utils/logdata.py` & `vega_sim-1.2.0/vega_sim/reinforcement/full_market_sim/utils/logdata.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/reinforcement/full_market_sim/utils/strategy.py` & `vega_sim-1.2.0/vega_sim/reinforcement/full_market_sim/utils/strategy.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/reinforcement/helpers.py` & `vega_sim-1.2.0/vega_sim/reinforcement/helpers.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/reinforcement/la_market_state.py` & `vega_sim-1.2.0/vega_sim/reinforcement/la_market_state.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/reinforcement/networks.py` & `vega_sim-1.2.0/vega_sim/reinforcement/networks.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/reinforcement/plot.py` & `vega_sim-1.2.0/vega_sim/reinforcement/plot.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/reinforcement/run_rl_agent.py` & `vega_sim-1.2.0/vega_sim/reinforcement/run_rl_agent.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/reinforcement/run_simple_agent.py` & `vega_sim-1.2.0/vega_sim/reinforcement/run_simple_agent.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/reinforcement/theory_intro/RL.tex` & `vega_sim-1.2.0/vega_sim/reinforcement/theory_intro/RL.tex`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/reinforcement/theory_intro/images/RL.png` & `vega_sim-1.2.0/vega_sim/reinforcement/theory_intro/images/RL.png`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/reinforcement/theory_intro/images/RL_inv.png` & `vega_sim-1.2.0/vega_sim/reinforcement/theory_intro/images/RL_inv.png`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/reinforcement/theory_intro/images/logo.png` & `vega_sim-1.2.0/vega_sim/reinforcement/theory_intro/images/logo.png`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/reinforcement/theory_intro/images/logo_inv.png` & `vega_sim-1.2.0/vega_sim/reinforcement/theory_intro/images/logo_inv.png`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/reinforcement/v2/agents/learning_agent.py` & `vega_sim-1.2.0/vega_sim/reinforcement/v2/agents/learning_agent.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/reinforcement/v2/agents/learning_agent_MO.py` & `vega_sim-1.2.0/vega_sim/reinforcement/v2/agents/learning_agent_MO.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/reinforcement/v2/agents/puppets.py` & `vega_sim-1.2.0/vega_sim/reinforcement/v2/agents/puppets.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,56 @@
 import traceback
 from dataclasses import dataclass
 from enum import Enum, auto
 from typing import Optional
 from logging import getLogger
 
+import vega_sim.proto.vega as vega_protos
 from vega_sim.scenario.common.agents import StateAgentWithWallet, VegaService, VegaState
+from vega_sim.service import PeggedOrder
 
 logger = getLogger(__name__)
 
 
 class Side(Enum):
     SELL = 0
     NONE = 1
     BUY = 2
 
 
+class ForcedSide(Enum):
+    SELL = 0
+    BUY = 1
+
+
 @dataclass
 class Action:
     pass
 
 
 @dataclass
 class MarketOrderAction(Action):
     side: Side
     volume: float
 
 
 @dataclass
+class AtTouchOrderAction(Action):
+    side: ForcedSide
+    volume: float
+
+
+@dataclass
 class NoAction(Action):
     pass
 
 
 class AgentType(Enum):
     MARKET_ORDER = auto()
+    AT_TOUCH = auto()
 
 
 class Puppet(StateAgentWithWallet):
     def __init__(
         self,
         key_name: str,
         market_name: str,
@@ -86,9 +100,51 @@
                     volume=self.action.volume,
                     wait=False,
                 )
             except:
                 logger.exception(traceback.format_exc())
 
 
-AGENT_TYPE_TO_AGENT = {AgentType.MARKET_ORDER: MarketOrderPuppet}
-AGENT_TYPE_TO_ACTION = {AgentType.MARKET_ORDER: MarketOrderAction}
+class AtTouchPuppet(Puppet):
+    def initialise(self, vega: VegaService, create_wallet: bool = True):
+        super().initialise(vega, create_wallet)
+        self.market_id = self.vega.find_market_id(name=self.market_name)
+
+    def step(self, vega_state: VegaState):
+        if self.action is not None and self.action is not NoAction:
+            try:
+                self.vega.cancel_order(
+                    trading_key=self.key_name, market_id=self.market_id
+                )
+                self.vega.submit_order(
+                    trading_key=self.key_name,
+                    market_id=self.market_id,
+                    side=(
+                        "SIDE_BUY"
+                        if self.action.side == ForcedSide.BUY
+                        else "SIDE_SELL"
+                    ),
+                    volume=self.action.volume,
+                    time_in_force=vega_protos.vega.Order.TimeInForce.TIME_IN_FORCE_GTC,
+                    order_type=vega_protos.vega.Order.Type.TYPE_LIMIT,
+                    pegged_order=PeggedOrder(
+                        reference=(
+                            vega_protos.vega.PeggedReference.PEGGED_REFERENCE_BEST_BID
+                            if self.action.side == ForcedSide.BUY
+                            else vega_protos.vega.PeggedReference.PEGGED_REFERENCE_BEST_ASK
+                        ),
+                        offset=0,
+                    ),
+                    wait=False,
+                )
+            except:
+                logger.exception(traceback.format_exc())
+
+
+AGENT_TYPE_TO_AGENT = {
+    AgentType.MARKET_ORDER: MarketOrderPuppet,
+    AgentType.AT_TOUCH: AtTouchPuppet,
+}
+AGENT_TYPE_TO_ACTION = {
+    AgentType.MARKET_ORDER: MarketOrderAction,
+    AgentType.AT_TOUCH: AtTouchOrderAction,
+}
```

### Comparing `vega_sim-1.1.1/vega_sim/reinforcement/v2/learning_environment.py` & `vega_sim-1.2.0/vega_sim/reinforcement/v2/learning_environment.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict
+from typing import Dict, Type, Optional
 from dataclasses import dataclass
 from vega_sim.reinforcement.v2.agents.puppets import (
     AGENT_TYPE_TO_AGENT,
     AgentType,
     MarketOrderAction,
     Action,
     Side,
@@ -21,16 +21,16 @@
     reward: float
 
 
 class Environment:
     def __init__(
         self,
         agents: Dict[str, AgentType],
-        agent_to_reward: Dict[str, BaseRewarder],
-        agent_to_state: Dict[str, State],
+        agent_to_reward: Dict[str, Reward],
+        agent_to_state: Dict[str, Type[State]],
         scenario: Scenario,
         reset_vega_every_n_runs: int = 100,
         funds_per_run: float = 10_000,
     ):
         self._agents = agents
         self._agent_to_reward_enum = agent_to_reward
         self._agent_to_state = agent_to_state
@@ -59,28 +59,32 @@
         return self._agent_to_state[agent_name].from_vega(
             self._vega,
             for_key_name=agent_name,
             market_id=self._market_id,
             asset_id=self._asset_id,
         )
 
-    def step(self, actions: Dict[str, Action]) -> Dict[str, StepResult]:
+    def step(self, actions: Dict[str, Optional[Action]]) -> Dict[str, StepResult]:
         for agent_name, action in actions.items():
-            self._puppets[agent_name].set_next_action(action=action)
+            if action is not None:
+                self._puppets[agent_name].set_next_action(action=action)
 
         self._scenario.env.step(self._vega)
         self._vega.wait_fn(1)
         step_res = {}
         for agent_name, reward_gen in self._agent_to_reward.items():
             step_res[agent_name] = StepResult(
                 observation=self._extract_observation(agent_name),
-                reward=reward_gen.get_reward(self._vega),
+                reward=self.calculate_reward(reward_gen),
             )
         return step_res
 
+    def calculate_reward(self, rewarder: Type[BaseRewarder]) -> float:
+        return rewarder.get_reward(vega=self._vega)
+
     def _reset_vega(self) -> None:
         self._vega.stop()
         self._vega = VegaServiceNull(
             warn_on_raw_data_access=False,
             run_with_console=False,
             retain_log_files=True,
             store_transactions=True,
```

### Comparing `vega_sim-1.1.1/vega_sim/reinforcement/v2/run.py` & `vega_sim-1.2.0/vega_sim/reinforcement/v2/run.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/reinforcement/v2/states.py` & `vega_sim-1.2.0/vega_sim/reinforcement/v2/states.py`

 * *Files 9% similar despite different names*

```diff
@@ -140,7 +140,38 @@
             ask_prices=ask_prices,
             bid_volumes=[level.volume for level in book_state.buys]
             + [0] * max(0, 5 - len(book_state.buys)),
             ask_volumes=[level.volume for level in book_state.sells]
             + [0] * max(0, 5 - len(book_state.sells)),
             trading_fee=fee,
         )
+
+
+@dataclass(frozen=True)
+class PositionOnly(State):
+    position: float
+
+    def to_array(self) -> np.array:
+        return np.nan_to_num(
+            np.array(
+                [
+                    self.position,
+                ]
+            )
+        )
+
+    @classmethod
+    def from_vega(
+        cls,
+        vega: VegaService,
+        for_key_name: str,
+        market_id: str,
+        asset_id: str,
+        for_wallet_name: Optional[str] = None,
+    ) -> "PositionOnly":
+        position = vega.positions_by_market(
+            for_key_name, market_id, wallet_name=for_wallet_name
+        )
+
+        return cls(
+            position=position.open_volume if position else 0,
+        )
```

### Comparing `vega_sim-1.1.1/vega_sim/replay/replay.py` & `vega_sim-1.2.0/vega_sim/replay/replay.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/scenario/adhoc.py` & `vega_sim-1.2.0/vega_sim/scenario/adhoc.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/scenario/common/agents.py` & `vega_sim-1.2.0/vega_sim/scenario/common/agents.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 from __future__ import annotations
 
+import uuid
+import psutil
+import platform
+
 import datetime
 import logging
 from dataclasses import dataclass
 from math import exp
 from queue import Queue
 
 import numpy as np
@@ -26,14 +30,17 @@
 from vega_sim.environment import VegaState
 from vega_sim.environment.agent import Agent, StateAgent, StateAgentWithWallet
 from vega_sim.network_service import VegaServiceNetwork
 from vega_sim.null_service import VegaService, VegaServiceNull
 from vega_sim.proto.vega import markets as markets_protos
 from vega_sim.proto.vega import vega as vega_protos
 from vega_sim.scenario.common.utils.ideal_mm_models import GLFT_approx, a_s_mm_model
+from vega_sim.service import PeggedOrder
+
+from vega_sim.api.helpers import get_enum
 
 WalletConfig = namedtuple("WalletConfig", ["name", "passphrase"])
 
 
 @dataclass
 class MarketHistoryData:
     at_time: datetime.datetime
@@ -71,14 +78,25 @@
     base_volume_size: float
     order_distribution_buy_kappa: float
     order_distribution_sell_kappa: float
     from_timepoint: int  # Inclusive
     thru_timepoint: int  # Inclusive
 
 
+@dataclass
+class ResourceData:
+    at_time: str
+    vega_cpu_per: float
+    vega_mem_rss: float
+    vega_mem_vms: float
+    datanode_cpu_per: float
+    datanode_mem_rss: float
+    datanode_mem_vms: float
+
+
 class TradeSignal(Enum):
     NOACTION = 0
     BUY = 1
     SELL = 2
 
 
 class MarketOrderTrader(StateAgentWithWallet):
@@ -2710,19 +2728,27 @@
         additional_state_fn: Optional[
             Callable[[VegaService, Dict[str, Agent]], Any]
         ] = None,
         only_extract_additional: bool = False,
     ):
         self.tag = None
         self.states = []
+        self.resources = []
         self.additional_states = []
         self.agents = agents
         self.additional_state_fn = additional_state_fn
         self.seen_trades = set()
         self.only_extract_additional = only_extract_additional
+        self.process_map: Dict[str, psutil.Process] = {}
+        self.platform = platform.system()
+
+    def initialise(self, vega: VegaService, **kwargs):
+        self.vega = vega
+        if not isinstance(vega, VegaServiceNetwork):
+            self._create_process_map()
 
     def step(self, vega_state: VegaState):
         if not self.only_extract_additional:
             market_infos = {}
             market_datas = {}
             market_depths = {}
             market_trades = {}
@@ -2752,19 +2778,76 @@
                     market_info=market_infos,
                     market_data=market_datas,
                     accounts=accounts,
                     market_depth=market_depths,
                     trades=market_trades,
                 )
             )
+
+            if not isinstance(self.vega, VegaServiceNetwork):
+                if self.platform == "Linux":
+                    mem_vega = (
+                        self.process_map["vega"].memory_full_info()
+                        if "vega" in self.process_map
+                        else None
+                    )
+                    mem_datanode = (
+                        self.process_map["data-node"].memory_full_info()
+                        if "data-node" in self.process_map
+                        else None
+                    )
+                elif self.platform == "Darwin":
+                    mem_vega = (
+                        self.process_map["vega"].memory_info()
+                        if "vega" in self.process_map
+                        else None
+                    )
+                    mem_datanode = (
+                        self.process_map["data-node"].memory_info()
+                        if "data-node" in self.process_map
+                        else None
+                    )
+                else:
+                    mem_vega = None
+                    mem_datanode = None
+                    logging.warning(
+                        "Unable to record memory usage, unsupported operating system"
+                    )
+
+                self.resources.append(
+                    ResourceData(
+                        at_time=start_time,
+                        vega_cpu_per=self.process_map["vega"].cpu_percent()
+                        if "vega" in self.process_map
+                        else 0,
+                        vega_mem_rss=mem_vega.rss if mem_vega is not None else 0,
+                        vega_mem_vms=mem_vega.vms if mem_vega is not None else 0,
+                        datanode_cpu_per=self.process_map["data-node"].cpu_percent()
+                        if "data-node" in self.process_map
+                        else 0,
+                        datanode_mem_rss=mem_datanode.rss
+                        if mem_datanode is not None
+                        else 0,
+                        datanode_mem_vms=mem_datanode.vms
+                        if mem_datanode is not None
+                        else 0,
+                    )
+                )
         if self.additional_state_fn is not None:
             self.additional_states.append(
                 self.additional_state_fn(self.vega, self.agents)
             )
 
+    def _create_process_map(self):
+        for name, p in self.vega.process_pids.items():
+            self.process_map[name] = psutil.Process(self.vega.process_pids[name])
+
+    def finalise(self):
+        self.assets = self.vega.list_assets()
+
 
 class KeyFunder(Agent):
     NAME_BASE = "key_funder"
 
     def __init__(
         self,
         keys_to_fund: List[str],
@@ -3000,7 +3083,257 @@
                 order_type="TYPE_LIMIT",
                 time_in_force="TIME_IN_FORCE_GTT",
                 side=self.side,
                 volume=self.uncrossing_size,
                 price=curr_price,
                 wait=False,
             )
+
+
+class RewardFunder(StateAgentWithWallet):
+    NAME_BASE = "reward_funder"
+
+    def __init__(
+        self,
+        key_name: str,
+        reward_asset_name: str,
+        transfer_amount: str,
+        initial_mint: float = 1e9,
+        account_type: Optional[str] = None,
+        asset_for_metric_name: Optional[str] = None,
+        metric: Optional[str] = None,
+        market_names: Optional[str] = None,
+        wallet_name: Optional[str] = None,
+        stake_key: bool = False,
+        tag: Optional[str] = None,
+    ):
+        super().__init__(wallet_name=wallet_name, key_name=key_name, tag=tag)
+        self.reward_asset_name = reward_asset_name
+        self.transfer_amount = transfer_amount
+        self.initial_mint = initial_mint
+        self.asset_for_metric_name = asset_for_metric_name
+        self.account_type = account_type
+        self.metric = metric
+        self.market_names = market_names
+        self.stake_key = stake_key
+
+    def initialise(
+        self,
+        vega: Union[VegaServiceNull, VegaServiceNetwork],
+        create_key: bool = True,
+        mint_key: bool = True,
+    ):
+        # Initialise wallet
+        super().initialise(vega=vega, create_key=create_key)
+
+        # Faucet vega tokens
+        self.vega.wait_for_total_catchup()
+        if mint_key:
+            self.vega.mint(
+                wallet_name=self.wallet_name,
+                asset="VOTE",
+                amount=1e4,
+                key_name=self.key_name,
+            )
+        if self.stake_key:
+            self.vega.stake(
+                amount=1,
+                key_name=self.key_name,
+                wallet_name=self.wallet_name,
+            )
+        self.vega.wait_fn(1)
+        self.vega.wait_for_total_catchup()
+
+        if vega.find_asset_id(symbol=self.reward_asset_name) is None:
+            # Create asset
+            self.vega.create_asset(
+                wallet_name=self.wallet_name,
+                name=self.reward_asset_name,
+                symbol=self.reward_asset_name,
+                decimals=18,
+                max_faucet_amount=5e10,
+                key_name=self.key_name,
+            )
+        self.vega.wait_fn(1)
+        self.vega.wait_for_total_catchup()
+        reward_asset_id = self.vega.find_asset_id(symbol=self.reward_asset_name)
+
+        if mint_key:
+            # Top up asset
+            self.vega.mint(
+                wallet_name=self.wallet_name,
+                asset=reward_asset_id,
+                amount=self.initial_mint,
+                key_name=self.key_name,
+            )
+        self.vega.wait_fn(1)
+        self.vega.wait_for_total_catchup()
+
+        market_ids = (
+            [self.vega.find_market_id(name) for name in self.market_names]
+            if self.market_names is not None
+            else None
+        )
+        asset_for_metric_id = (
+            self.vega.find_asset_id(self.asset_for_metric_name)
+            if self.asset_for_metric_name is not None
+            else None
+        )
+
+        self.vega.recurring_transfer(
+            from_wallet_name=self.wallet_name,
+            from_key_name=self.key_name,
+            from_account_type=vega_protos.ACCOUNT_TYPE_GENERAL,
+            to_account_type=self.account_type,
+            amount=self.transfer_amount,
+            asset=reward_asset_id,
+            asset_for_metric=asset_for_metric_id,
+            metric=self.metric,
+            markets=market_ids,
+        )
+
+
+class AtTheTouchMarketMaker(StateAgentWithWallet):
+    """Eventually can use the at-the-touch optimal strategy from
+        Algorithmic and High-Frequency Trading by Cartea, Jaimungal and Penalva.
+
+    Posts only pegged limit orders
+    """
+
+    NAME_BASE = "at_the_touch_market_maker"
+
+    def __init__(
+        self,
+        key_name: str,
+        initial_asset_mint: float = 1000000,
+        market_name: Optional[str] = None,
+        asset_name: Optional[str] = None,
+        order_size: float = 1,
+        tag: str = "",
+        wallet_name: str = None,
+        peg_offset=0,
+        max_position=1,
+        buy_peg_reference: Optional[str] = "PEGGED_REFERENCE_BEST_BID",
+        sell_peg_reference: Optional[str] = "PEGGED_REFERENCE_BEST_ASK",
+    ):
+        super().__init__(wallet_name=wallet_name, key_name=key_name, tag=tag)
+        self.initial_asset_mint = initial_asset_mint
+
+        self.current_step = 0
+
+        self.market_name = market_name
+        self.asset_name = asset_name
+
+        self.current_position = 0
+        self.order_size = order_size
+        self.peg_offset = peg_offset
+        self.max_position = max_position
+
+        self.buy_peg_reference = buy_peg_reference
+        self.sell_peg_reference = sell_peg_reference
+
+        self.buy_order_reference = None
+        self.sell_order_reference = None
+
+    def initialise(
+        self,
+        vega: Union[VegaServiceNull, VegaServiceNetwork],
+        create_key: bool = True,
+        mint_key: bool = True,
+    ):
+        # Initialise wallet for LP/ Settle Party
+        super().initialise(vega=vega, create_key=create_key)
+
+        # Get asset id
+        self.asset_id = self.vega.find_asset_id(symbol=self.asset_name)
+        if mint_key:
+            # Top up asset
+            self.vega.mint(
+                wallet_name=self.wallet_name,
+                asset=self.asset_id,
+                amount=self.initial_asset_mint,
+                key_name=self.key_name,
+            )
+            self.vega.wait_for_total_catchup()
+
+        # Get market id
+        self.market_id = self.vega.find_market_id(name=self.market_name)
+
+        self._update_state(current_step=self.current_step)
+
+    def step(self, vega_state: VegaState):
+        self.current_step += 1
+
+        # Each step, get position
+        position = self.vega.positions_by_market(
+            wallet_name=self.wallet_name,
+            market_id=self.market_id,
+            key_name=self.key_name,
+        )
+        self.current_position = float(
+            position.open_volume if position is not None else 0
+        )
+
+        # Get a list of live orders for the party
+        orders = list(
+            (
+                vega_state.market_state[self.market_id]
+                .orders.get(
+                    self.vega.wallet.public_key(
+                        wallet_name=self.wallet_name, name=self.key_name
+                    ),
+                    {},
+                )
+                .values()
+            )
+            if self.market_id in vega_state.market_state
+            else []
+        )
+
+        # Check buy_order_reference and sell_order_reference are still live:
+        buys = []
+        sells = []
+        for order in orders:
+            buys.append(order) if order.side == vega_protos.SIDE_BUY else sells.append(
+                order
+            )
+
+        place_buy = self.current_position < self.max_position
+        place_sell = self.current_position > -self.max_position
+
+        if len(buys) == 0 and place_buy:
+            self.buy_order_reference = self._place_order(side="SIDE_BUY")
+        elif len(sells) != 0 and not place_buy:
+            self._cancel_order(orders_to_cancel=buys)
+
+        if len(sells) == 0 and place_sell:
+            self.sell_order_reference = self._place_order(side="SIDE_SELL")
+        elif len(sells) != 0 and not place_sell:
+            self._cancel_order(orders_to_cancel=sells)
+
+    def _place_order(self, side: str):
+        return self.vega.submit_order(
+            trading_wallet=self.wallet_name,
+            trading_key=self.key_name,
+            market_id=self.market_id,
+            order_type="TYPE_LIMIT",
+            time_in_force="TIME_IN_FORCE_GTC",
+            side=side,
+            volume=self.order_size,
+            price=None,
+            expires_at=None,
+            pegged_order=PeggedOrder(
+                reference=self.buy_peg_reference
+                if side == "SIDE_BUY"
+                else self.sell_peg_reference,
+                offset=self.peg_offset,
+            ),
+        )
+
+    def _cancel_order(self, orders_to_cancel):
+        for order in orders_to_cancel:
+            self.vega.cancel_order(
+                wallet_name=self.wallet_name,
+                trading_key=self.key_name,
+                market_id=self.market_id,
+                order_id=order.id,
+            )
```

### Comparing `vega_sim-1.1.1/vega_sim/scenario/common/utils/ideal_mm_models.py` & `vega_sim-1.2.0/vega_sim/scenario/common/utils/ideal_mm_models.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/scenario/common/utils/price_process.py` & `vega_sim-1.2.0/vega_sim/scenario/common/utils/price_process.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/scenario/comprehensive_market/agents.py` & `vega_sim-1.2.0/vega_sim/scenario/comprehensive_market/agents.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/scenario/comprehensive_market/scenario.py` & `vega_sim-1.2.0/vega_sim/scenario/comprehensive_market/scenario.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/scenario/configurable_market/agents.py` & `vega_sim-1.2.0/vega_sim/scenario/configurable_market/agents.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,15 @@
         asset_dp: int,
         proposal_wallet_name: Optional[str] = None,
         termination_wallet_name: Optional[str] = None,
         market_config: Optional[MarketConfig] = None,
         tag: Optional[str] = None,
         settlement_price: Optional[float] = None,
         initial_mint: Optional[float] = 1e9,
+        stake_key: bool = False,
     ):
         super().__init__(
             wallet_name=proposal_wallet_name,
             key_name=proposal_key_name,
             tag=tag,
         )
 
@@ -58,14 +59,16 @@
 
         self.market_config = (
             market_config if market_config is not None else MarketConfig()
         )
 
         self.settlement_price = settlement_price
 
+        self.stake_key = stake_key
+
     def initialise(
         self,
         vega: Union[VegaServiceNull, VegaServiceNetwork],
         create_key: bool = True,
         mint_key: bool = True,
     ):
         super().initialise(vega=vega, create_key=create_key)
@@ -79,23 +82,30 @@
         if mint_key:
             self.vega.mint(
                 wallet_name=self.wallet_name,
                 asset="VOTE",
                 amount=1e4,
                 key_name=self.key_name,
             )
+        if self.stake_key:
+            self.vega.stake(
+                amount=1,
+                key_name=self.key_name,
+                wallet_name=self.wallet_name,
+            )
 
         self.vega.wait_for_total_catchup()
 
         if self.vega.find_asset_id(symbol=self.asset_name) is None:
             self.vega.create_asset(
                 wallet_name=self.wallet_name,
                 name=self.asset_name,
                 symbol=self.asset_name,
                 decimals=self.asset_dp,
+                quantum=int(10 ** (self.asset_dp)),
                 max_faucet_amount=10_000_000_000,
                 key_name=self.key_name,
             )
 
         self.vega.wait_for_total_catchup()
         self.asset_id = self.vega.find_asset_id(symbol=self.asset_name)
```

### Comparing `vega_sim-1.1.1/vega_sim/scenario/configurable_market/scenario.py` & `vega_sim-1.2.0/vega_sim/scenario/configurable_market/scenario.py`

 * *Files 23% similar despite different names*

```diff
@@ -29,43 +29,46 @@
 
 from vega_sim.scenario.common.agents import (
     OpenAuctionPass,
     ExponentialShapedMarketMaker,
     PriceSensitiveMarketOrderTrader,
     InformedTrader,
     StateAgent,
+    AtTheTouchMarketMaker,
 )
 
 
 class ConfigurableMarket(Scenario):
     def __init__(
         self,
-        market_name: str = None,
-        market_code: str = None,
-        asset_name: str = None,
-        asset_dp: str = None,
+        market_name: Optional[str] = None,
+        market_code: Optional[str] = None,
+        asset_name: Optional[str] = None,
+        asset_dp: Optional[str] = None,
         num_steps: int = 120,
         granularity: Optional[Granularity] = Granularity.MINUTE,
         block_size: int = 1,
         block_length_seconds: int = 1,
         state_extraction_fn: Optional[
             Callable[[VegaServiceNull, Dict[str, Agent]], Any]
         ] = None,
         settle_at_end: bool = True,
         price_process_fn: Optional[Callable] = None,
+        pause_every_n_steps: Optional[int] = None,
     ):
         super().__init__(state_extraction_fn=state_extraction_fn)
 
         # Simulation settings
         self.num_steps = num_steps
         self.granularity = granularity
         self.block_size = block_size
         self.block_length_seconds = block_length_seconds
         self.settle_at_end = settle_at_end
         self.price_process_fn = price_process_fn
+        self.pause_every_n_steps = pause_every_n_steps
 
         # Asset parameters
         self.asset_name = asset_name
         self.asset_decimal = asset_dp
 
         # Market parameters
         self.market_name = market_name
@@ -77,31 +80,33 @@
     ) -> list:
         start = "2021-07-01 00:00:00"
 
         start = datetime.strptime(start, "%Y-%m-%d %H:%M:%S")
 
         start = start + timedelta(days=int(random_state.choice(range(90))))
 
-        end = start + timedelta(seconds=(self.num_steps + 1) * self.granularity.value)
+        end = start + timedelta(seconds=(self.num_steps * 1.1) * self.granularity.value)
 
         price_process = get_historic_price_series(
             product_id="ETH-USD",
             granularity=self.granularity,
             start=str(start),
             end=str(end),
+            interpolation=f"{self.granularity.value}s",
         )
 
         return list(price_process)
 
     def configure_agents(
         self,
         vega: VegaServiceNull,
         tag: str,
         market_config: Optional[MarketConfig] = None,
         random_state: Optional[np.random.RandomState] = None,
+        **kwargs,
     ) -> Dict[str, StateAgent]:
         market_config = market_config if market_config is not None else MarketConfig()
 
         random_state = (
             random_state if random_state is not None else np.random.RandomState()
         )
 
@@ -144,14 +149,28 @@
             inventory_upper_boundary=200,
             inventory_lower_boundary=-200,
             market_kappa=1,
             market_order_arrival_rate=10,
             state_update_freq=10,
         )
 
+        at_the_touch_mm = AtTheTouchMarketMaker(
+            key_name="AT_THE_TOUCH_MM",
+            wallet_name="MM",
+            initial_asset_mint=1e9,
+            market_name=self.market_name,
+            asset_name=self.asset_name,
+            market_decimal_places=market_config.decimal_places,
+            position_decimal_places=market_config.position_decimal_places,
+            asset_decimal_places=self.asset_decimal,
+            peg_offset=0,
+            max_position=10 * 10 ** (-market_config.position_decimal_places),
+            tag="a",
+        )
+
         sensitive_mo_trader_a = PriceSensitiveMarketOrderTrader(
             wallet_name=SENSITIVE_PARTY_A.wallet_name,
             key_name=SENSITIVE_PARTY_A.key_name,
             market_name=market_name,
             asset_name=asset_name,
             initial_asset_mint=1e10,
             buy_intensity=1,
@@ -229,22 +248,24 @@
             shaped_mm,
             sensitive_mo_trader_a,
             sensitive_mo_trader_b,
             sensitive_mo_trader_c,
             auctionpass1,
             auctionpass2,
             info_trader,
+            at_the_touch_mm,
         ]
         return {agent.name(): agent for agent in agents}
 
     def configure_environment(
         self, vega: VegaServiceNull, **kwargs
     ) -> MarketEnvironmentWithState:
         return MarketEnvironmentWithState(
             agents=list(self.agents.values()),
             n_steps=self.num_steps,
             step_length_seconds=self.granularity.value,
             random_agent_ordering=True,
             transactions_per_block=self.block_size,
             vega_service=vega,
             block_length_seconds=self.block_length_seconds,
+            pause_every_n_steps=self.pause_every_n_steps,
         )
```

### Comparing `vega_sim-1.1.1/vega_sim/scenario/curve_market_maker/scenario.py` & `vega_sim-1.2.0/vega_sim/scenario/curve_market_maker/scenario.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/scenario/fuzzed_markets/agents.py` & `vega_sim-1.2.0/vega_sim/scenario/fuzzed_markets/agents.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,16 +269,16 @@
 
                 if not os.path.exists("fuzz_plots"):
                     os.mkdir("fuzz_plots")
 
                 fig.write_html("fuzz_plots/coverage.html")
 
 
-class DegenerateTrader(StateAgentWithWallet):
-    NAME_BASE = "degenerate_trader"
+class RiskyMarketOrderTrader(StateAgentWithWallet):
+    NAME_BASE = "risky_market_order_trader"
 
     def __init__(
         self,
         key_name: str,
         market_name: str,
         asset_name: str,
         tag: Optional[str] = None,
@@ -369,16 +369,16 @@
                 market_id=self.market_id,
                 side=self.side,
                 volume=size,
                 wait=False,
             )
 
 
-class DegenerateLiquidityProvider(StateAgentWithWallet):
-    NAME_BASE = "degenerate_liquidity_provider"
+class RiskySimpleLiquidityProvider(StateAgentWithWallet):
+    NAME_BASE = "risky_simple_liquidity_provider"
 
     def __init__(
         self,
         key_name: str,
         market_name: str,
         asset_name: str,
         tag: Optional[str] = None,
```

### Comparing `vega_sim-1.1.1/vega_sim/scenario/fuzzed_markets/run_fuzz_test.py` & `vega_sim-1.2.0/vega_sim/scenario/fuzzed_markets/run_fuzz_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,34 +9,41 @@
 from vega_sim.scenario.fuzzed_markets.scenario import FuzzingScenario
 
 from vega_sim.tools.scenario_plots import (
     fuzz_plots,
     plot_run_outputs,
     account_plots,
     plot_price_monitoring,
+    reward_plots,
 )
 
 from matplotlib import pyplot as plt
 
 
-def _run(steps: int = 2880, output: bool = False, output_dir: str = "fuzz_plots"):
+def _run(
+    steps: int = 2880,
+    console: bool = False,
+    output: bool = False,
+    output_dir: str = "fuzz_plots",
+):
     scenario = FuzzingScenario(
         num_steps=steps,
         step_length_seconds=30,
         block_length_seconds=1,
         transactions_per_block=4096,
         output=output,
     )
 
     with VegaServiceNull(
         warn_on_raw_data_access=False,
         seconds_per_block=scenario.block_length_seconds,
         transactions_per_block=scenario.transactions_per_block,
         retain_log_files=True,
         use_full_vega_wallet=False,
+        run_with_console=console,
     ) as vega:
         scenario.run_iteration(
             vega=vega,
             network=Network.NULLCHAIN,
             output_data=output,
             log_every_n_steps=100,
         )
@@ -56,16 +63,20 @@
             plt.close(fig)
 
         trading_figs = plot_run_outputs()
         for key, fig in trading_figs.items():
             fig.savefig(f"{output_dir}/trading-{key}.jpg")
             plt.close(fig)
 
+        reward_fig = reward_plots()
+        reward_fig.savefig(f"{output_dir}/rewards.jpg")
+        plt.close(fig)
+
         account_fig = account_plots()
-        account_fig.savefig(f"{output_dir}/accounts-{key}.jpg")
+        account_fig.savefig(f"{output_dir}/accounts.jpg")
         plt.close(account_fig)
 
 
 if __name__ == "__main__":
     logging.basicConfig(
         level=logging.INFO,
         format="%(asctime)s - %(name)s - %(levelname)s - %(message)s",
@@ -74,10 +85,11 @@
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "-s",
         "--steps",
         default=2 * 60 * 12,
         type=int,
     )
+    parser.add_argument("--console", action="store_true")
     args = parser.parse_args()
 
-    _run(steps=args.steps, output=True)
+    _run(steps=args.steps, console=args.console, output=True)
```

### Comparing `vega_sim-1.1.1/vega_sim/scenario/fuzzed_markets/scenario.py` & `vega_sim-1.2.0/vega_sim/scenario/fuzzed_markets/scenario.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,32 +3,40 @@
 import argparse
 import logging
 import numpy as np
 from typing import Optional, List
 from vega_sim.scenario.common.utils.price_process import random_walk
 
 from vega_sim.scenario.scenario import Scenario
-from vega_sim.environment.environment import MarketEnvironmentWithState
+from vega_sim.environment.environment import (
+    MarketEnvironmentWithState,
+    NetworkEnvironment,
+)
+from vega_sim.scenario.constants import Network
 from vega_sim.null_service import VegaServiceNull
 
 from vega_sim.scenario.configurable_market.agents import ConfigurableMarketManager
 from vega_sim.scenario.common.agents import (
     StateAgent,
     UncrossAuctionAgent,
     ExponentialShapedMarketMaker,
     MarketOrderTrader,
     LimitOrderTrader,
+    RewardFunder,
+    AtTheTouchMarketMaker,
 )
 from vega_sim.scenario.fuzzed_markets.agents import (
     FuzzingAgent,
-    DegenerateTrader,
-    DegenerateLiquidityProvider,
+    RiskyMarketOrderTrader,
+    RiskySimpleLiquidityProvider,
     FuzzyLiquidityProvider,
 )
 
+import vega_sim.proto.vega as vega_protos
+
 import datetime
 from typing import Optional, Dict
 from dataclasses import dataclass
 from vega_sim.scenario.common.agents import ExponentialShapedMarketMaker
 import pandas as pd
 
 
@@ -46,19 +54,19 @@
     external_prices = {}
     trader_close_outs = {}
     liquidity_provider_close_outs = {}
 
     for _, agent in agents.items():
         if isinstance(agent, ExponentialShapedMarketMaker):
             external_prices[agent.market_id] = agent.curr_price
-        if isinstance(agent, DegenerateTrader):
+        if isinstance(agent, RiskyMarketOrderTrader):
             trader_close_outs[agent.market_id] = (
                 trader_close_outs.get(agent.market_id, 0) + agent.close_outs
             )
-        if isinstance(agent, DegenerateLiquidityProvider):
+        if isinstance(agent, RiskySimpleLiquidityProvider):
             liquidity_provider_close_outs[agent.market_id] = (
                 liquidity_provider_close_outs.get(agent.market_id, 0) + agent.close_outs
             )
 
     return MarketHistoryAdditionalData(
         at_time=at_time,
         external_prices=external_prices,
@@ -164,26 +172,28 @@
     def configure_agents(
         self,
         vega: VegaServiceNull,
         tag: str,
         random_state: Optional[np.random.RandomState],
         **kwargs,
     ) -> List[StateAgent]:
-        random_state = (
+        self.random_state = (
             random_state if random_state is not None else np.random.RandomState()
         )
 
         market_managers = []
         market_makers = []
+        at_touch_market_makers = []
         auction_traders = []
         random_traders = []
         fuzz_traders = []
-        degenerate_traders = []
+        risky_traders = []
         fuzz_liquidity_providers = []
-        degenerate_liquidity_providers = []
+        risky_liquidity_providers = []
+        reward_funders = []
 
         self.initial_asset_mint = 1e9
 
         for i_market in range(self.n_markets):
             # Define the market and the asset:
             market_name = f"ASSET_{str(i_market).zfill(3)}"
             asset_name = f"ASSET_{str(i_market).zfill(3)}"
@@ -197,56 +207,70 @@
             )
             if self.fuzz_market_config is not None:
                 for param in self.fuzz_market_config:
                     market_config.set(param=self.fuzz_market_config[param])
 
             # Create fuzzed price process
             price_process = _create_price_process(
-                random_state=random_state,
+                random_state=self.random_state,
                 num_steps=self.num_steps,
                 decimal_places=int(market_config.decimal_places),
             )
 
             # Create fuzzed market managers
             market_managers.append(
                 ConfigurableMarketManager(
-                    proposal_wallet_name="MARKET_MANAGER",
                     proposal_key_name="PROPOSAL_KEY",
                     termination_wallet_name="MARKET_MANAGER",
                     termination_key_name="TERMINATION_KEY",
                     market_config=market_config,
                     market_name=market_name,
                     market_code=market_name,
                     asset_dp=asset_dp,
                     asset_name=asset_name,
                     settlement_price=price_process[-1],
+                    stake_key=True if kwargs["network"] == Network.CAPSULE else False,
                     tag=f"MARKET_{str(i_market).zfill(3)}",
                 )
             )
 
             market_makers.append(
                 ExponentialShapedMarketMaker(
                     wallet_name="MARKET_MAKERS",
                     key_name=f"MARKET_{str(i_market).zfill(3)}",
                     price_process_generator=iter(price_process),
                     initial_asset_mint=self.initial_asset_mint,
                     market_name=market_name,
                     asset_name=asset_name,
                     commitment_amount=1e6,
                     market_decimal_places=market_config.decimal_places,
-                    asset_decimal_places=asset_name,
+                    asset_decimal_places=asset_dp,
                     num_steps=self.num_steps,
                     kappa=2.4,
                     tick_spacing=0.05,
                     market_kappa=50,
                     state_update_freq=10,
                     tag=f"MARKET_{str(i_market).zfill(3)}",
                 )
             )
 
+            at_touch_market_makers.append(
+                AtTheTouchMarketMaker(
+                    wallet_name=f"AT_THE_TOUCH_MM",
+                    key_name=f"MARKET_{str(i_market).zfill(3)}",
+                    initial_asset_mint=1e5,
+                    market_name=market_name,
+                    asset_name=asset_name,
+                    order_size=1,
+                    peg_offset=0,
+                    max_position=5,
+                    tag=f"MARKET_{str(i_market).zfill(3)}",
+                )
+            )
+
             for i_agent, side in enumerate(["SIDE_BUY", "SIDE_SELL"]):
                 auction_traders.append(
                     UncrossAuctionAgent(
                         wallet_name=f"AUCTION_TRADERS",
                         key_name=f"MARKET_{str(i_market).zfill(3)}_{side}",
                         side=side,
                         initial_asset_mint=self.initial_asset_mint,
@@ -306,53 +330,53 @@
                         output_plot_on_finalise=self.output,
                         tag=f"MARKET_{str(i_market).zfill(3)}_AGENT_{str(i_agent).zfill(3)}",
                     )
                 )
 
             for side in ["SIDE_BUY", "SIDE_SELL"]:
                 for i_agent in range(10):
-                    degenerate_traders.append(
-                        DegenerateTrader(
-                            wallet_name="DEGENERATE_TRADERS",
+                    risky_traders.append(
+                        RiskyMarketOrderTrader(
+                            wallet_name="risky_traders",
                             key_name=f"MARKET_{str(i_market).zfill(3)}_SIDE_{side}_AGENT_{str(i_agent).zfill(3)}",
                             market_name=market_name,
                             asset_name=asset_name,
                             side=side,
                             initial_asset_mint=1_000,
-                            size_factor=0.7,
+                            size_factor=0.5,
                             step_bias=0.1,
                             tag=f"MARKET_{str(i_market).zfill(3)}_SIDE_{side}_AGENT_{str(i_agent).zfill(3)}",
                         )
                     )
 
             for i_agent in range(5):
-                degenerate_liquidity_providers.append(
-                    DegenerateLiquidityProvider(
-                        wallet_name="DEGENERATE_LIQUIDITY_PROVIDERS",
-                        key_name=f"HIGH_DEGEN_MARKET_{str(i_market).zfill(3)}_AGENT_{str(i_agent).zfill(3)}",
+                risky_liquidity_providers.append(
+                    RiskySimpleLiquidityProvider(
+                        wallet_name="risky_liquidity_providers",
+                        key_name=f"HIGH_RISK_LPS_MARKET_{str(i_market).zfill(3)}_AGENT_{str(i_agent).zfill(3)}",
                         market_name=market_name,
                         asset_name=asset_name,
-                        initial_asset_mint=1_000,
-                        commitment_factor=0.7,
+                        initial_asset_mint=20_000,
+                        commitment_factor=0.5,
                         step_bias=0.1,
-                        tag=f"HIGH_DEGEN_MARKET_{str(i_market).zfill(3)}_AGENT_{str(i_agent).zfill(3)}",
+                        tag=f"HIGH_RISK_LPS_MARKET_{str(i_market).zfill(3)}_AGENT_{str(i_agent).zfill(3)}",
                     )
                 )
 
             for i_agent in range(45):
-                degenerate_liquidity_providers.append(
-                    DegenerateLiquidityProvider(
-                        wallet_name="DEGENERATE_LIQUIDITY_PROVIDERS",
-                        key_name=f"LOW_DEGEN_MARKET_{str(i_market).zfill(3)}_AGENT_{str(i_agent).zfill(3)}",
+                risky_liquidity_providers.append(
+                    RiskySimpleLiquidityProvider(
+                        wallet_name="risky_liquidity_providers",
+                        key_name=f"LOW_RISK_LPS_MARKET_{str(i_market).zfill(3)}_AGENT_{str(i_agent).zfill(3)}",
                         market_name=market_name,
                         asset_name=asset_name,
-                        initial_asset_mint=1_000,
-                        commitment_factor=0.5,
+                        initial_asset_mint=20_000,
+                        commitment_factor=0.3,
                         step_bias=0.1,
-                        tag=f"LOW_DEGEN_MARKET_{str(i_market).zfill(3)}_AGENT_{str(i_agent).zfill(3)}",
+                        tag=f"LOW_RISK_LPS_MARKET_{str(i_market).zfill(3)}_AGENT_{str(i_agent).zfill(3)}",
                     )
                 )
 
             for i_agent in range(5):
                 fuzz_liquidity_providers.append(
                     FuzzyLiquidityProvider(
                         wallet_name="FUZZY_LIQUIDITY_PROVIDERS",
@@ -360,40 +384,91 @@
                         market_name=market_name,
                         asset_name=asset_name,
                         initial_asset_mint=5_000,
                         tag=f"MARKET_{str(i_market).zfill(3)}_AGENT_{str(i_agent).zfill(3)}",
                     )
                 )
 
+            for i_agent, (account_type, metric) in enumerate(
+                [
+                    (
+                        vega_protos.vega.ACCOUNT_TYPE_REWARD_MAKER_PAID_FEES,
+                        vega_protos.vega.DISPATCH_METRIC_MAKER_FEES_PAID,
+                    ),
+                    (
+                        vega_protos.vega.ACCOUNT_TYPE_REWARD_MAKER_RECEIVED_FEES,
+                        vega_protos.vega.DISPATCH_METRIC_MAKER_FEES_RECEIVED,
+                    ),
+                    (
+                        vega_protos.vega.ACCOUNT_TYPE_REWARD_LP_RECEIVED_FEES,
+                        vega_protos.vega.DISPATCH_METRIC_LP_FEES_RECEIVED,
+                    ),
+                    (
+                        vega_protos.vega.ACCOUNT_TYPE_REWARD_MARKET_PROPOSERS,
+                        vega_protos.vega.DISPATCH_METRIC_MARKET_VALUE,
+                    ),
+                ]
+            ):
+                reward_funders.append(
+                    RewardFunder(
+                        wallet_name="REWARD_FUNDERS",
+                        key_name=f"MARKET_{str(i_market).zfill(3)}_AGENT_{str(i_agent).zfill(3)}",
+                        reward_asset_name=vega_protos.vega.DispatchMetric.Name(metric),
+                        initial_mint=1e9,
+                        account_type=account_type,
+                        transfer_amount=100,
+                        asset_for_metric_name=asset_name,
+                        metric=metric,
+                        market_names=[market_name],
+                        stake_key=True,
+                        tag=f"MARKET_{str(i_market).zfill(3)}_AGENT_{str(i_agent).zfill(3)}",
+                    )
+                )
+
         agents = (
             market_managers
             + market_makers
+            + at_touch_market_makers
             + auction_traders
             + random_traders
             + fuzz_traders
-            + degenerate_traders
-            + degenerate_liquidity_providers
+            + risky_traders
+            + risky_liquidity_providers
             + fuzz_liquidity_providers
+            + reward_funders
         )
         return {agent.name(): agent for agent in agents}
 
     def configure_environment(
         self,
         vega: VegaServiceNull,
         **kwargs,
     ) -> MarketEnvironmentWithState:
-        return MarketEnvironmentWithState(
-            agents=list(self.agents.values()),
-            n_steps=self.num_steps,
-            random_agent_ordering=False,
-            transactions_per_block=self.transactions_per_block,
-            vega_service=vega,
-            step_length_seconds=self.step_length_seconds,
-            block_length_seconds=vega.seconds_per_block,
-        )
+        if kwargs.get("network", Network.NULLCHAIN) == Network.NULLCHAIN:
+            return MarketEnvironmentWithState(
+                agents=list(self.agents.values()),
+                n_steps=self.num_steps,
+                random_agent_ordering=False,
+                transactions_per_block=self.transactions_per_block,
+                vega_service=vega,
+                step_length_seconds=self.step_length_seconds,
+                block_length_seconds=vega.seconds_per_block,
+            )
+        else:
+            return NetworkEnvironment(
+                agents=list(self.agents.values()),
+                n_steps=self.num_steps,
+                vega_service=vega,
+                step_length_seconds=self.step_length_seconds,
+                raise_datanode_errors=kwargs.get("raise_datanode_errors", False),
+                raise_step_errors=kwargs.get("raise_step_errors", False),
+                random_state=self.random_state,
+                create_keys=True,
+                mint_keys=True,
+            )
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--debug", action="store_true")
     args = parser.parse_args()
```

### Comparing `vega_sim-1.1.1/vega_sim/scenario/hedged_market_maker/agents.py` & `vega_sim-1.2.0/vega_sim/scenario/hedged_market_maker/agents.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/scenario/hedged_market_maker/scenario.py` & `vega_sim-1.2.0/vega_sim/scenario/hedged_market_maker/scenario.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/scenario/ideal_market_maker/agents.py` & `vega_sim-1.2.0/vega_sim/scenario/ideal_market_maker/agents.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/scenario/ideal_market_maker/environments.py` & `vega_sim-1.2.0/vega_sim/scenario/ideal_market_maker/environments.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/scenario/ideal_market_maker/scenario.py` & `vega_sim-1.2.0/vega_sim/scenario/ideal_market_maker/scenario.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/scenario/ideal_market_maker/utils/log_data.py` & `vega_sim-1.2.0/vega_sim/scenario/ideal_market_maker/utils/log_data.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/scenario/ideal_market_maker/utils/strategy.py` & `vega_sim-1.2.0/vega_sim/scenario/ideal_market_maker/utils/strategy.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/scenario/ideal_market_maker_v2/agents.py` & `vega_sim-1.2.0/vega_sim/scenario/ideal_market_maker_v2/agents.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/scenario/ideal_market_maker_v2/scenario.py` & `vega_sim-1.2.0/vega_sim/scenario/ideal_market_maker_v2/scenario.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/scenario/ideal_market_maker_v2/utils/strategy.py` & `vega_sim-1.2.0/vega_sim/scenario/ideal_market_maker_v2/utils/strategy.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/scenario/market_crash/price_process.py` & `vega_sim-1.2.0/vega_sim/scenario/market_crash/price_process.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/scenario/market_crash/scenario.py` & `vega_sim-1.2.0/vega_sim/scenario/market_crash/scenario.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/scenario/multi_market/agents.py` & `vega_sim-1.2.0/vega_sim/scenario/multi_market/agents.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/scenario/multi_market/scenario.py` & `vega_sim-1.2.0/vega_sim/scenario/multi_market/scenario.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/scenario/parameter_experiment/scenario.py` & `vega_sim-1.2.0/vega_sim/scenario/parameter_experiment/scenario.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/scenario/realtime_market/scenario.py` & `vega_sim-1.2.0/vega_sim/scenario/realtime_market/scenario.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/scenario/registry.py` & `vega_sim-1.2.0/vega_sim/scenario/registry.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/scenario/scenario.py` & `vega_sim-1.2.0/vega_sim/scenario/scenario.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,31 @@
 import abc
 import numpy as np
 from typing import Optional, List, Callable, Any, Dict
 
 from vega_sim.null_service import VegaService
 from vega_sim.environment.environment import MarketEnvironment
 from vega_sim.scenario.constants import Network
-from vega_sim.scenario.common.agents import Snitch, StateAgent, MarketHistoryData, Agent
+from vega_sim.scenario.common.agents import (
+    Snitch,
+    StateAgent,
+    MarketHistoryData,
+    Agent,
+    ResourceData,
+)
 from vega_sim.tools.scenario_output import (
+    agents_standard_output,
+    resources_standard_output,
     market_data_standard_output,
     agents_standard_output,
+    assets_standard_output,
 )
 
+import vega_sim.proto.vega as vega_protos
+
 
 class Scenario(abc.ABC):
     def __init__(
         self,
         state_extraction_fn: Optional[
             Callable[[VegaService, Dict[str, Agent]], Any]
         ] = None,
@@ -85,26 +96,36 @@
         outputs = self.env.run(
             pause_at_completion=pause_at_completion,
             run_with_console=run_with_console,
             log_every_n_steps=log_every_n_steps,
         )
         if output_data:
             agents_standard_output(self.agents)
+            resources_standard_output(self.get_resource_data())
+            assets_standard_output(self.get_assets())
             market_data_standard_output(self.get_run_data())
             if self.additional_data_output_fns is not None:
                 market_data_standard_output(
                     self.get_additional_run_data(),
                     custom_output_fns=self.additional_data_output_fns,
                 )
 
         return outputs
 
     def get_snitch(self) -> Optional[Snitch]:
         return self.agents.get("snitch")
 
+    def get_resource_data(self) -> List[ResourceData]:
+        snitch = self.get_snitch()
+        return snitch.resources if snitch is not None else []
+
+    def get_assets(self) -> List[vega_protos.assets.Asset]:
+        snitch = self.get_snitch()
+        return snitch.assets if snitch is not None else []
+
     def get_run_data(self) -> List[MarketHistoryData]:
         snitch = self.get_snitch()
         return snitch.states if snitch is not None else []
 
     def get_additional_run_data(self) -> List[MarketHistoryData]:
         snitch = self.get_snitch()
         return snitch.additional_states if snitch is not None else []
```

### Comparing `vega_sim-1.1.1/vega_sim/service.py` & `vega_sim-1.2.0/vega_sim/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 import vega_sim.grpc.client as vac
 import vega_sim.proto.data_node.api.v2 as data_node_protos_v2
 import vega_sim.proto.vega as vega_protos
 import vega_sim.proto.vega.data_source_pb2 as data_source_protos
 from vega_sim.api.helpers import (
     get_enum,
     forward,
+    statistics,
     num_to_padded_int,
     wait_for_core_catchup,
     wait_for_datanode_sync,
 )
 from vega_sim.local_data_cache import LocalDataCache
 from vega_sim.proto.vega.commands.v1.commands_pb2 import (
     OrderAmendment,
@@ -100,14 +101,15 @@
 class VegaService(ABC):
     def __init__(
         self,
         can_control_time: bool = False,
         warn_on_raw_data_access: bool = True,
         seconds_per_block: int = 1,
         listen_for_high_volume_stream_updates: bool = False,
+        governance_symbol: Optional[str] = "VOTE",
     ):
         """A generic service for accessing a set of Vega processes.
 
         Contains generic methods aimed at working whether the derived class
         is referencing a locally hosted Nullchain version of Vega
         or a fully-fledged remote market.
 
@@ -134,14 +136,18 @@
                     starting/ending.
             listen_for_high_volume_stream_updates:
                 bool, default False, Whether to listen for high volume stream updates.
                     These are generally less necessary, but contain large numbers of
                     updates per block, such as all ledger transactions. For a network
                     running at ~1s/block these are likely to be fine, but can be a
                     hindrance working at full nullchain speed.
+            governance_symbol:
+                str, default "VOTE", allows the symbol of the governance asset to be
+                    defined. This defaults to "VOTE" for nullchain networks but should
+                    be changed (most likely to "VEGA") for other networks.
 
         """
         self._core_client = None
         self._core_state_client = None
         self._trading_data_client_v2 = None
         self._local_data_cache = None
         self.can_control_time = can_control_time
@@ -152,14 +158,16 @@
         self._asset_decimals = None
         self._market_to_asset = None
         self._listen_for_high_volume_stream_updates = (
             listen_for_high_volume_stream_updates
         )
         self.seconds_per_block = seconds_per_block
 
+        self.governance_symbol = governance_symbol
+
     @property
     def market_price_decimals(self) -> int:
         if self._market_price_decimals is None:
             self._market_price_decimals = DecimalsCache(
                 lambda market_id: self.data_cache.market_from_feed(
                     market_id=market_id
                 ).decimal_places
@@ -450,31 +458,32 @@
 
         proposal_id = gov.propose_asset(
             wallet=self.wallet,
             wallet_name=wallet_name,
             name=name,
             symbol=symbol,
             decimals=decimals,
-            max_faucet_amount=max_faucet_amount * 10**decimals,
+            max_faucet_amount=num_to_padded_int(max_faucet_amount, decimals),
             quantum=quantum,
             data_client=self.trading_data_client_v2,
-            closing_time=blockchain_time_seconds + self.seconds_per_block * 90,
-            enactment_time=blockchain_time_seconds + self.seconds_per_block * 100,
             validation_time=blockchain_time_seconds + self.seconds_per_block * 30,
+            closing_time=blockchain_time_seconds + self.seconds_per_block * 40,
+            enactment_time=blockchain_time_seconds + self.seconds_per_block * 50,
             time_forward_fn=lambda: self.wait_fn(2),
             key_name=key_name,
         )
         self.wait_fn(1)
         gov.approve_proposal(
             proposal_id=proposal_id,
             wallet_name=wallet_name,
             wallet=self.wallet,
             key_name=key_name,
         )
-        self.wait_fn(110)
+        self.wait_fn(60)
+        self.wait_for_thread_catchup()
 
     def create_market_from_config(
         self,
         proposal_key_name: str,
         market_config: market.MarketConfig,
         proposal_wallet_name: Optional[str] = None,
     ):
@@ -482,26 +491,26 @@
 
         proposal_id = gov.propose_market_from_config(
             wallet=self.wallet,
             data_client=self.trading_data_client_v2,
             proposal_wallet_name=proposal_wallet_name,
             proposal_key_name=proposal_key_name,
             market_config=market_config,
-            closing_time=blockchain_time_seconds + self.seconds_per_block * 90,
-            enactment_time=blockchain_time_seconds + self.seconds_per_block * 90,
+            closing_time=blockchain_time_seconds + self.seconds_per_block * 40,
+            enactment_time=blockchain_time_seconds + self.seconds_per_block * 50,
             time_forward_fn=lambda: self.wait_fn(2),
         )
-
         gov.approve_proposal(
             proposal_id=proposal_id,
             wallet=self.wallet,
             wallet_name=proposal_wallet_name,
             key_name=proposal_key_name,
         )
-        self.wait_fn(110)
+        self.wait_fn(60)
+        self.wait_for_thread_catchup()
 
     def create_simple_market(
         self,
         market_name: str,
         proposal_key: str,
         settlement_asset_id: str,
         termination_key: str,
@@ -564,28 +573,29 @@
             settlement_asset_id=settlement_asset_id,
             data_client=self.trading_data_client_v2,
             termination_pub_key=self.wallet.public_key(
                 wallet_name=termination_wallet_name, name=termination_key
             ),
             position_decimals=position_decimals,
             market_decimals=market_decimals,
-            closing_time=blockchain_time_seconds + self.seconds_per_block * 90,
-            enactment_time=blockchain_time_seconds + self.seconds_per_block * 100,
+            closing_time=blockchain_time_seconds + self.seconds_per_block * 40,
+            enactment_time=blockchain_time_seconds + self.seconds_per_block * 50,
             risk_model=risk_model,
             time_forward_fn=lambda: self.wait_fn(2),
             price_monitoring_parameters=price_monitoring_parameters,
             **additional_kwargs,
         )
         gov.approve_proposal(
             proposal_id=proposal_id,
             wallet=self.wallet,
             wallet_name=wallet_name,
             key_name=proposal_key,
         )
-        self.wait_fn(110)
+        self.wait_fn(60)
+        self.wait_for_thread_catchup()
 
     def submit_market_order(
         self,
         trading_key: str,
         market_id: str,
         side: Union[vega_protos.vega.Side, str],
         volume: float,
@@ -842,15 +852,15 @@
             time_in_force=time_in_force,
         )
 
     def cancel_order(
         self,
         trading_key: str,
         market_id: str,
-        order_id: str,
+        order_id: Optional[str] = None,
         wallet_name: Optional[str] = None,
     ):
         """
         Cancel Order
 
         Args:
             trading_wallet:
@@ -893,26 +903,27 @@
 
         proposal_id = gov.propose_network_parameter_change(
             parameter=parameter,
             value=new_value,
             wallet=self.wallet,
             wallet_name=wallet_name,
             data_client=self.trading_data_client_v2,
-            closing_time=blockchain_time_seconds + self.seconds_per_block * 90,
-            enactment_time=blockchain_time_seconds + self.seconds_per_block * 100,
+            closing_time=blockchain_time_seconds + self.seconds_per_block * 40,
+            enactment_time=blockchain_time_seconds + self.seconds_per_block * 50,
             time_forward_fn=lambda: self.wait_fn(2),
             key_name=proposal_key,
         )
         gov.approve_proposal(
             proposal_id=proposal_id,
             wallet=self.wallet,
             wallet_name=wallet_name,
             key_name=proposal_key,
         )
-        self.wait_fn(110)
+        self.wait_fn(60)
+        self.wait_for_thread_catchup()
 
     def update_market(
         self,
         proposal_key: str,
         market_id: str,
         updated_instrument: Optional[UpdateInstrumentConfiguration] = None,
         updated_metadata: Optional[str] = None,
@@ -1020,25 +1031,26 @@
         proposal_id = gov.propose_market_update(
             market_update=update_configuration,
             market_id=market_id,
             wallet=self.wallet,
             key_name=proposal_key,
             wallet_name=wallet_name,
             data_client=self.trading_data_client_v2,
-            closing_time=blockchain_time_seconds + self.seconds_per_block * 90,
-            enactment_time=blockchain_time_seconds + self.seconds_per_block * 100,
+            closing_time=blockchain_time_seconds + self.seconds_per_block * 40,
+            enactment_time=blockchain_time_seconds + self.seconds_per_block * 50,
             time_forward_fn=lambda: self.wait_fn(2),
         )
         gov.approve_proposal(
             proposal_id=proposal_id,
             wallet=self.wallet,
             key_name=proposal_key,
             wallet_name=wallet_name,
         )
-        self.wait_fn(110)
+        self.wait_fn(60)
+        self.wait_for_thread_catchup()
 
     def settle_market(
         self,
         settlement_key: str,
         settlement_price: float,
         market_id: str,
         wallet_name: Optional[str] = None,
@@ -1228,15 +1240,15 @@
             account_type=account_type,
             data_client=self.trading_data_client_v2,
         )
 
     def best_prices(
         self,
         market_id: str,
-    ) -> Tuple[int, int]:
+    ) -> Tuple[float, float]:
         """
         Output the best static bid price and best static ask price in current market.
         """
         market_data = self.get_latest_market_data(
             market_id=market_id,
         )
 
@@ -1465,30 +1477,35 @@
         """
         return data.find_market_id(
             name=name,
             raise_on_missing=raise_on_missing,
             data_client=self.trading_data_client_v2,
         )
 
-    def find_asset_id(self, symbol: str, raise_on_missing: bool = False) -> str:
+    def find_asset_id(
+        self, symbol: str, enabled: bool = True, raise_on_missing: bool = False
+    ) -> str:
         """Looks up the Asset ID of a given asset name
 
         Args:
             symbol:
                 str, The symbol of the asset to look up
+            enabled:
+                bool, whether the asset must be enabled for the id to be returned
             raise_on_missing:
                 bool, whether to raise an Error or silently return if the asset
                  does not exist
 
         Returns:
             str, the ID of the asset
         """
         return data.find_asset_id(
             symbol=symbol,
             raise_on_missing=raise_on_missing,
+            enabled=enabled,
             data_client=self.trading_data_client_v2,
         )
 
     @raw_data
     def order_status(
         self, order_id: str, version: int = 0
     ) -> Optional[vega_protos.vega.Order]:
@@ -2158,14 +2175,126 @@
             to_account_type=to_account_type,
             asset=asset,
             amount=str(num_to_padded_int(amount, adp)),
             reference=reference,
             one_off=one_off,
         )
 
+    def recurring_transfer(
+        self,
+        from_key_name: str,
+        from_account_type: vega_protos.vega.AccountType,
+        to_account_type: vega_protos.vega.AccountType,
+        asset: str,
+        amount: float,
+        to_key_name: Optional[str] = None,
+        reference: Optional[str] = None,
+        from_wallet_name: Optional[str] = None,
+        to_wallet_name: Optional[str] = None,
+        start_epoch: Optional[int] = None,
+        end_epoch: Optional[int] = None,
+        factor: float = 1,
+        asset_for_metric: Optional[str] = None,
+        metric: Optional[vega_protos.vega.DispatchMetric] = None,
+        markets: Optional[List[str]] = None,
+    ):
+        """Create a recurring transfer of funds.
+
+        Function can be used to setup a recurring transfer of funds between two keys or
+        between a key and a network reward pool. If funding a reward pool, a dispatch
+        strategy can be specified to fund a specific pool.
+
+        Args:
+            from_key_name (str):
+                The key name of the source account.
+            from_account_type (vega_protos.vega.AccountType):
+                The account type of the source account.
+            to_account_type (vega_protos.vega.AccountType):
+                The account type of the destination account.
+            asset (str):
+                The id of the asset to transfer.
+            amount (float):
+                The amount of the asset to transfer.
+            to_key_name (Optional[str], optional):
+                The key name of the destination account. Defaults to None.
+            reference (Optional[str], optional):
+                A reference string for the transfer. Defaults to None.
+            from_wallet_name (Optional[str], optional):
+                The name of the source wallet. Defaults to None.
+            to_wallet_name (Optional[str], optional):
+                The name of the destination wallet. Defaults to None.
+            start_epoch (Optional[int], optional):
+                The epoch to start the transfer. Defaults to None (next epoch).
+            end_epoch (Optional[int], optional):
+                The epoch to end the transfer. Defaults to None (never ends).
+            factor (float, optional):
+                The factor to adjust the transfer amount by each epoch. Defaults to 1.
+            asset_for_metric (Optional[str], optional):
+                The asset to use for the dispatch metric. Defaults to None.
+            metric (Optional[vega_protos.vega.DispatchMetric], optional):
+                The dispatch metric. Defaults to None.
+            markets (Optional[List[str]], optional):
+                The list of markets to apply the dispatch strategy. Defaults to None.
+
+        Raises:
+            Exception:
+                If a value is provided for one but not all non-optional
+                DispatchStrategy fields.
+
+        Returns:
+            None
+        """
+
+        # Create the RecurringTransfer message
+        recurring_transfer = vega_protos.commands.v1.commands.RecurringTransfer(
+            start_epoch=(
+                start_epoch
+                if start_epoch is not None
+                else int(self.statistics().epoch_seq)
+            )
+        )
+        # Set the optional RecurringTransfer fields
+        if start_epoch is not None:
+            setattr(recurring_transfer, "start_epoch", start_epoch)
+        if end_epoch is not None:
+            setattr(recurring_transfer, "end_epoch", end_epoch)
+        if factor is not None:
+            setattr(recurring_transfer, "factor", str(factor))
+        if any([val is not None for val in [asset_for_metric, metric, markets]]):
+            if any([val is None for val in [asset_for_metric, metric]]):
+                raise Exception(
+                    "Value for one but not all non-optional DispatchStrategy fields"
+                    " given."
+                )
+            dispatch_strategy = vega_protos.vega.DispatchStrategy(
+                asset_for_metric=asset_for_metric,
+                metric=metric,
+            )
+            # Set the optional DispatchStrategy fields
+            if markets is not None:
+                dispatch_strategy.markets.extend(markets)
+            recurring_transfer.dispatch_strategy.CopyFrom(dispatch_strategy)
+
+        trading.transfer(
+            wallet=self.wallet,
+            wallet_name=from_wallet_name,
+            key_name=from_key_name,
+            from_account_type=from_account_type,
+            to=(
+                self.wallet.public_key(wallet_name=to_wallet_name, name=to_key_name)
+                if to_key_name is not None
+                else "0000000000000000000000000000000000000000000000000000000000000000"
+            ),
+            to_account_type=to_account_type,
+            asset=asset,
+            amount=str(num_to_padded_int(amount, self.asset_decimals[asset])),
+            reference=reference,
+            recurring=recurring_transfer,
+        )
+
     def list_transfers(
         self,
         wallet_name: Optional[str] = None,
         key_name: Optional[str] = None,
         direction: Optional[data_node_protos_v2.trading_data.TransferDirection] = None,
     ) -> List[data.Transfer]:
         """Returns a list of processed transfers.
@@ -2386,17 +2515,49 @@
         return data.estimate_position(
             data_client=self.trading_data_client_v2,
             market_id=market_id,
             open_volume=num_to_padded_int(
                 open_volume, decimals=self.market_pos_decimals[market_id]
             ),
             orders=orders,
-            collateral_available=str(
-                num_to_padded_int(
-                    collateral_available,
-                    self.asset_decimals[self.market_to_asset[market_id]],
+            collateral_available=(
+                str(
+                    num_to_padded_int(
+                        collateral_available,
+                        self.asset_decimals[self.market_to_asset[market_id]],
+                    )
                 )
-            )
-            if collateral_available is not None
-            else None,
+                if collateral_available is not None
+                else None
+            ),
             asset_decimals=self.asset_decimals,
         )
+
+    def get_stake(
+        self,
+        party_id: Optional[str] = None,
+    ):
+        asset_id = self.find_asset_id(symbol=self.governance_symbol)
+        return data.get_stake(
+            data_client=self.trading_data_client_v2,
+            party_id=party_id,
+            asset_decimals=self.asset_decimals[asset_id],
+        )
+
+    def get_asset(self, asset_id: str):
+        return data.get_asset(
+            data_client=self.trading_data_client_v2, asset_id=asset_id
+        )
+
+    def list_all_network_history_segments(self):
+        return data_raw.list_all_network_history_segments(
+            data_client=self.trading_data_client_v2
+        )
+
+    def statistics(self):
+        return statistics(core_data_client=self.core_client)
+
+    def list_assets(self):
+        return self.data_cache._asset_from_feed.values()
+
+    def stake(self, **kwargs):
+        pass
```

### Comparing `vega_sim-1.1.1/vega_sim/tools/load_binaries.py` & `vega_sim-1.2.0/vega_sim/tools/load_binaries.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 def download_binaries(force: bool = False):
     platf = platform.system().lower()
 
     # We have no Windows specific builds, so people have to use WSL to run
     platf = "linux" if platf == "windows" else platf
 
-    chipset = platform.processor()
+    chipset = "arm" if "arm" in platform.machine() else "amd"
 
     if force and os.path.exists(vega_sim.vega_bin_path):
         shutil.rmtree(vega_sim.vega_bin_path)
 
     with tempfile.TemporaryDirectory() as dir:
         if not os.path.exists(vega_sim.vega_bin_path):
             os.mkdir(vega_sim.vega_bin_path)
```

### Comparing `vega_sim-1.1.1/vega_sim/tools/scenario_output.py` & `vega_sim-1.2.0/vega_sim/tools/scenario_output.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,44 @@
 from vega_sim.environment.agent import Agent, StateAgentWithWallet
-from vega_sim.scenario.common.agents import MarketHistoryData
+from vega_sim.scenario.common.agents import MarketHistoryData, ResourceData
 from typing import List, Callable, Optional, Dict
 import pandas as pd
 import itertools
 import os
 import os.path
 
+import vega_sim.proto.vega as vega_protos
+
 DEFAULT_PATH = "./run_logs"
 DEFAULT_RUN_NAME = "latest"
 
 AGENTS_FILE_NAME = "agents.csv"
 DATA_FILE_NAME = "market_data.csv"
 ORDER_BOOK_FILE_NAME = "depth_data.csv"
 TRADES_FILE_NAME = "trades.csv"
 ACCOUNTS_FILE_NAME = "accounts.csv"
 FUZZING_FILE_NAME = "additional_data.csv"
+RESOURCES_FILE_NAME = "resources.csv"
+
+
+def resource_data_to_row(data: ResourceData):
+    return [
+        {
+            "time": data.at_time,
+            "vega_cpu_per": data.vega_cpu_per,
+            "vega_mem_rss": data.vega_mem_rss,
+            "vega_mem_vms": data.vega_mem_vms,
+            "datanode_cpu_per": data.datanode_cpu_per,
+            "datanode_mem_rss": data.datanode_mem_rss,
+            "datanode_mem_vms": data.datanode_mem_vms,
+        }
+    ]
+
+
+ASSETS_FILE_NAME = "assets.csv"
 
 
 def history_data_to_row(data: MarketHistoryData) -> List[pd.Series]:
     results = []
     for market_id in data.market_info.keys():
         market_data = data.market_data[market_id]
 
@@ -160,14 +180,40 @@
             market_history_data=market_history_data,
             file_name=file_name,
             output_path=full_path,
             data_to_row_fn=data_fn,
         )
 
 
+def resources_standard_output(
+    resource_data: List[ResourceData],
+    run_name: str = DEFAULT_RUN_NAME,
+    output_path: str = DEFAULT_PATH,
+    custom_output_fns: Optional[
+        Dict[str, List[Callable[[MarketHistoryData], pd.Series]]]
+    ] = None,
+):
+    run_name = run_name if run_name is not None else DEFAULT_RUN_NAME
+    full_path = os.path.join(output_path, run_name)
+    data_fns = (
+        custom_output_fns
+        if custom_output_fns is not None
+        else {
+            RESOURCES_FILE_NAME: resource_data_to_row,
+        }
+    )
+    for file_name, data_fn in data_fns.items():
+        _market_data_standard_output(
+            market_history_data=resource_data,
+            file_name=file_name,
+            output_path=full_path,
+            data_to_row_fn=data_fn,
+        )
+
+
 def agents_standard_output(
     agents: Dict[str, Agent],
     run_name: str = DEFAULT_RUN_NAME,
     output_path: str = DEFAULT_PATH,
 ):
     results = {
         key: [] for key in ["agent_name", "agent_type", "agent_tag", "agent_key"]
@@ -179,24 +225,72 @@
         if isinstance(agent, StateAgentWithWallet):
             results["agent_key"].append(agent._public_key)
         else:
             results["agent_key"].append(None)
 
     full_path = os.path.join(output_path, run_name)
     os.makedirs(full_path, exist_ok=True)
-    pd.DataFrame.from_dict(results).to_csv(os.path.join(full_path, AGENTS_FILE_NAME))
+    pd.DataFrame.from_dict(results).set_index(
+        "agent_name",
+        drop=True,
+    ).to_csv(os.path.join(full_path, AGENTS_FILE_NAME))
+
+
+def assets_standard_output(
+    assets: List[vega_protos.assets.Asset],
+    run_name: str = DEFAULT_RUN_NAME,
+    output_path: str = DEFAULT_PATH,
+):
+    results = {
+        key: []
+        for key in [
+            "id",
+            "name",
+            "symbol",
+            "decimals",
+            "quantum",
+            "max_faucet_amount_mint",
+            "status",
+        ]
+    }
+    for asset in assets:
+        results["id"].append(asset.id)
+        results["name"].append(asset.details.name)
+        results["symbol"].append(asset.details.symbol)
+        results["decimals"].append(asset.details.decimals)
+        results["quantum"].append(asset.details.quantum)
+        results["max_faucet_amount_mint"].append(
+            asset.details.builtin_asset.max_faucet_amount_mint
+        )
+        results["status"].append(asset.status)
+
+    full_path = os.path.join(output_path, run_name)
+    os.makedirs(full_path, exist_ok=True)
+    pd.DataFrame.from_dict(results).set_index("id", drop=True).to_csv(
+        os.path.join(full_path, ASSETS_FILE_NAME)
+    )
 
 
 def load_agents_df(
     run_name: Optional[str] = None,
     output_path: str = DEFAULT_PATH,
 ) -> pd.DataFrame:
     run_name = run_name if run_name is not None else DEFAULT_RUN_NAME
-    return pd.read_csv(os.path.join(output_path, run_name, AGENTS_FILE_NAME)).set_index(
-        "agent_name"
+    return pd.read_csv(
+        os.path.join(output_path, run_name, AGENTS_FILE_NAME), index_col="agent_name"
+    )
+
+
+def load_assets_df(
+    run_name: Optional[str] = None,
+    output_path: str = DEFAULT_PATH,
+) -> pd.DataFrame:
+    run_name = run_name if run_name is not None else DEFAULT_RUN_NAME
+    return pd.read_csv(
+        os.path.join(output_path, run_name, ASSETS_FILE_NAME), index_col="id"
     )
 
 
 def load_market_data_df(
     run_name: Optional[str] = None,
     output_path: str = DEFAULT_PATH,
 ) -> pd.DataFrame:
@@ -252,7 +346,19 @@
 ) -> pd.DataFrame:
     run_name = run_name if run_name is not None else DEFAULT_RUN_NAME
     df = pd.read_csv(os.path.join(output_path, run_name, FUZZING_FILE_NAME))
     if not df.empty:
         df["time"] = pd.to_datetime(df.time)
         df = df.set_index("time")
     return df
+
+
+def load_resource_df(
+    run_name: Optional[str] = None,
+    output_path: str = DEFAULT_PATH,
+) -> pd.DataFrame:
+    run_name = run_name if run_name is not None else DEFAULT_RUN_NAME
+    df = pd.read_csv(os.path.join(output_path, run_name, RESOURCES_FILE_NAME))
+    if not df.empty:
+        df["time"] = pd.to_datetime(df.time)
+        df = df.set_index("time")
+    return df
```

### Comparing `vega_sim-1.1.1/vega_sim/tools/scenario_plots.py` & `vega_sim-1.2.0/vega_sim/tools/scenario_plots.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import os
 import ast
 
+import argparse
+
 import pandas as pd
 import matplotlib.pyplot as plt
 import vega_sim.proto.vega as vega_protos
 
 from typing import Optional
 from collections import defaultdict
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure
 from matplotlib.markers import MarkerStyle
 from matplotlib.gridspec import GridSpec, SubplotSpec, GridSpecFromSubplotSpec
 
 from vega_sim.scenario.fuzzed_markets.agents import (
     FuzzingAgent,
     FuzzyLiquidityProvider,
-    DegenerateTrader,
-    DegenerateLiquidityProvider,
+    RiskyMarketOrderTrader,
+    RiskySimpleLiquidityProvider,
 )
 
 from vega_sim.proto.vega import markets
 
 import numpy as np
 
 
@@ -43,14 +45,16 @@
 from vega_sim.tools.scenario_output import (
     load_accounts_df,
     load_market_data_df,
     load_order_book_df,
     load_trades_df,
     load_fuzzing_df,
     load_agents_df,
+    load_resource_df,
+    load_assets_df,
 )
 
 
 def _set_xticks(ax, index, freq: int = 60):
     xaxis_ticks = index[0:-1:freq]
     labels = [dt.strftime("%H:%M:%S") for dt in xaxis_ticks.to_pydatetime()]
     ax.set_xticks(
@@ -376,21 +380,21 @@
         transform=ax0.transAxes,
     )
 
     ax0.set_ylabel("PRICE")
     ax0.legend(labels=["external price", "mark price"])
 
 
-def plot_degen_close_outs(
+def plot_risky_close_outs(
     fig: Figure,
     accounts_df: pd.DataFrame,
     fuzzing_df: pd.DataFrame,
     ss: Optional[SubplotSpec] = None,
 ):
-    """Plots the number of close outs of degen traders and degen liquidity providers.
+    """Plots the number of close outs of risky traders and risky liquidity providers.
 
     Args:
         fig (matplotlib.figure.Figure):
             The figure object to plot onto.
         accounts_df (pandas.DataFrame):
             A dataframe containing the accounts data.
         fuzzing_df (pandas.DataFrame):
@@ -435,15 +439,15 @@
         label="insurance pool",
     )
     ln1 = ax0.plot(
         trader_close_outs_ds.index,
         trader_close_outs_ds.values,
         "r.-",
         markersize=1,
-        label="degen trader close outs",
+        label="risky trader close outs",
     )
 
     lns = ln0 + ln1
     ax0.legend(handles=lns, labels=[ln.get_label() for ln in lns], loc="upper left")
 
     ax0.set_ylabel("NB CLOSE OUTS")
     ax0r.set_ylabel("INSURANCE POOL", position="right")
@@ -461,15 +465,15 @@
         label="insurance pool",
     )
     ln4 = ax1.plot(
         liquidity_provider_close_outs_ds.index,
         liquidity_provider_close_outs_ds.values,
         "r.-",
         markersize=1,
-        label="degen LP close outs",
+        label="risky LP close outs",
     )
 
     lns = ln3 + ln4
     ax1.legend(handles=lns, labels=[ln.get_label() for ln in lns], loc="upper left")
 
     ax1.set_ylabel("NB CLOSE OUTS")
     ax1r.set_ylabel("INSURANCE POOL", position="right")
@@ -505,15 +509,15 @@
         plot_trading_mode(fig, ss=gs[0, 0], data_df=market_data_df)
         plot_price_comparison(
             fig,
             ss=gs[1, 0],
             data_df=market_data_df,
             fuzzing_df=market_fuzzing_df,
         )
-        plot_degen_close_outs(
+        plot_risky_close_outs(
             fig,
             ss=gs[2, 0],
             accounts_df=market_accounts_df,
             fuzzing_df=market_fuzzing_df,
         )
 
         figs[market_id] = fig
@@ -535,16 +539,16 @@
     fig.tight_layout()
 
     plt.rcParams.update({"font.size": 8})
 
     agent_types = [
         FuzzingAgent,
         FuzzyLiquidityProvider,
-        DegenerateTrader,
-        DegenerateLiquidityProvider,
+        RiskyMarketOrderTrader,
+        RiskySimpleLiquidityProvider,
     ]
 
     gs = GridSpec(nrows=len(agent_types), ncols=1, hspace=0.5)
 
     axs: list[plt.Axes] = []
 
     for i, agent_type in enumerate(agent_types):
@@ -690,22 +694,195 @@
         ax.set_ylabel("price")
 
         figs[market_id] = fig
 
     return figs
 
 
+def resource_monitoring_plot(run_name: Optional[str] = None):
+    resource_df = load_resource_df(
+        run_name=run_name,
+    )
+
+    fig = plt.figure(figsize=[11.69, 8.27])
+    fig.suptitle(
+        f"Resource Monitoring",
+        fontsize=18,
+        fontweight="bold",
+        color=(0.2, 0.2, 0.2),
+    )
+    fig.tight_layout()
+    plt.rcParams.update({"font.size": 8})
+    plt.rcParams.update({"axes.formatter.useoffset": False})
+
+    gs = GridSpec(nrows=3, ncols=2, hspace=0.5, wspace=0.3)
+
+    ax0 = fig.add_subplot(
+        gs[0, :],
+    )
+    ax0.set_title("CPU Utilization")
+    ax0.plot(resource_df.index, resource_df.vega_cpu_per, "r", label="vega")
+    ax0.plot(resource_df.index, resource_df.datanode_cpu_per, "b", label="data-node")
+    ax0.legend()
+    ax0.set_xlabel("'vega' datetime")
+    ax0.set_ylabel("CPU [%]")
+
+    ax1 = fig.add_subplot(gs[1, 0], sharex=ax0)
+    ax1.set_title("Memory - RSS (vega)")
+    ax1.plot(resource_df.index, resource_df.vega_mem_rss / 1e9, "r", label="vega")
+    ax1.legend()
+    ax1.set_xlabel("'vega' datetime")
+    ax1.set_ylabel("RSS [GB]")
+
+    ax2 = fig.add_subplot(gs[1, 1], sharex=ax0)
+    ax2.set_title("Memory - RSS (data-node)")
+    ax2.plot(
+        resource_df.index, resource_df.datanode_mem_rss / 1e9, "b", label="data-node"
+    )
+    ax2.legend()
+    ax2.set_xlabel("'vega' datetime")
+    ax2.set_ylabel("RSS [GB]")
+
+    ax3 = fig.add_subplot(gs[2, 0], sharex=ax0)
+    ax3.set_title("Memory - VMS (vega)")
+    ax3.plot(resource_df.index, resource_df.vega_mem_vms / 1e9, "r", label="vega")
+    ax3.legend()
+    ax3.set_xlabel("'vega' datetime")
+    ax3.set_ylabel("VMS [GB]")
+
+    ax4 = fig.add_subplot(gs[2, 1], sharex=ax0)
+    ax4.set_title("Memory - VMS (data-node)")
+    ax4.plot(
+        resource_df.index, resource_df.datanode_mem_vms / 1e9, "b", label="data-node"
+    )
+    ax4.legend()
+    ax4.set_xlabel("'vega' datetime")
+    ax4.set_ylabel("VMS [GB]")
+
+    return fig
+
+
+def reward_plots(run_name: Optional[str] = None):
+    accounts_df = load_accounts_df(run_name=run_name)
+    assets_df = load_assets_df(run_name=run_name)
+    agents_df = load_agents_df(run_name=run_name).set_index("agent_key")
+
+    joined_df = accounts_df.join(agents_df, on="party_id").join(assets_df, on="asset")
+
+    datetime = joined_df.index.unique()
+
+    fig = plt.figure(figsize=[11.69, 8.27])
+    fig.suptitle(
+        f"Agent Rewards Plots",
+        fontsize=18,
+        fontweight="bold",
+        color=(0.2, 0.2, 0.2),
+    )
+    fig.tight_layout()
+
+    plt.rcParams.update({"font.size": 8})
+
+    gs = GridSpec(nrows=2, ncols=2, hspace=0.4)
+
+    axs: list[plt.Axes] = []
+
+    plots = [
+        (
+            0,
+            0,
+            vega_protos.vega.DispatchMetric.Name(
+                vega_protos.vega.DISPATCH_METRIC_MAKER_FEES_PAID
+            ),
+        ),
+        (
+            0,
+            1,
+            vega_protos.vega.DispatchMetric.Name(
+                vega_protos.vega.DISPATCH_METRIC_MAKER_FEES_RECEIVED
+            ),
+        ),
+        (
+            1,
+            0,
+            vega_protos.vega.DispatchMetric.Name(
+                vega_protos.vega.DISPATCH_METRIC_LP_FEES_RECEIVED
+            ),
+        ),
+        (
+            1,
+            1,
+            vega_protos.vega.DispatchMetric.Name(
+                vega_protos.vega.DISPATCH_METRIC_MARKET_VALUE
+            ),
+        ),
+    ]
+
+    for plot in plots:
+        axs.append(fig.add_subplot(gs[plot[0], plot[1]]))
+        axs[-1].set_title(f"Asset: {plot[2]}")
+        accounts_for_asset = joined_df[joined_df.symbol == str(plot[2])]
+        grouped = accounts_for_asset.groupby(["agent_type", "time"])["balance"].sum()
+        for index in grouped.index.get_level_values(0).unique():
+            if index == "RewardFunder":
+                continue
+            series = grouped.loc[index]
+            series = series.reindex(datetime, fill_value=0)
+            axs[-1].plot(series.index, series.values, label=index)
+        plt.xticks(rotation=45)
+        axs[-1].legend()
+
+    return fig
+
+
 if __name__ == "__main__":
+    parser = argparse.ArgumentParser()
+    parser.add_argument("--fuzzing", action="store_true")
+    parser.add_argument("--trading", action="store_true")
+    parser.add_argument("--monitoring", action="store_true")
+    parser.add_argument("--accounts", action="store_true")
+    parser.add_argument("--rewards", action="store_true")
+    parser.add_argument("--resources", action="store_true")
+    parser.add_argument("--all", action="store_true")
+
+    parser.add_argument("--show", action="store_true")
+    parser.add_argument("--save", action="store_true")
+    args = parser.parse_args()
+
     dir = "test_plots"
     if not os.path.exists(dir):
         os.mkdir(dir)
-    figs = fuzz_plots()
-    for i, fig in enumerate(figs.values()):
-        fig.savefig(f"{dir}/fuzz-{i}.jpg")
-    figs = plot_run_outputs()
-    for i, fig in enumerate(figs.values()):
-        fig.savefig(f"{dir}/trading-{i}.jpg")
-    figs = plot_price_monitoring()
-    for i, fig in enumerate(figs.values()):
-        fig.savefig(f"{dir}/monitoring-{i}.jpg")
-    fig = account_plots()
-    fig.savefig(f"{dir}/accounts.jpg")
+
+    if args.fuzzing or args.all:
+        figs = fuzz_plots()
+        for i, fig in enumerate(figs.values()):
+            if args.save:
+                fig.savefig(f"{dir}/fuzz-{i}.jpg")
+
+    if args.trading or args.all:
+        figs = plot_run_outputs()
+        for i, fig in enumerate(figs.values()):
+            if args.save:
+                fig.savefig(f"{dir}/trading-{i}.jpg")
+
+    if args.monitoring or args.all:
+        figs = plot_price_monitoring()
+        for i, fig in enumerate(figs.values()):
+            if args.save:
+                fig.savefig(f"{dir}/monitoring-{i}.jpg")
+
+    if args.accounts or args.all:
+        fig = account_plots()
+        if args.save:
+            fig.savefig(f"{dir}/accounts.jpg")
+
+    if args.rewards or args.all:
+        fig = reward_plots()
+        if args.save:
+            fig.savefig(f"{dir}/rewards.jpg")
+
+    if args.resources or args.all:
+        fig = resource_monitoring_plot()
+        if args.save:
+            fig.savefig(f"{dir}/resource_monitoring.jpg")
+
+    if args.show:
+        plt.show()
```

### Comparing `vega_sim-1.1.1/vega_sim/vegahome/config/data-node/config.toml` & `vega_sim-1.2.0/vega_sim/vegahome/config/data-node/config.toml`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/vegahome/config/node/config.toml` & `vega_sim-1.2.0/vega_sim/vegahome/config/node/config.toml`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/vegahome/data/faucet/wallets/vega.1639051237294446827` & `vega_sim-1.2.0/vega_sim/vegahome/data/faucet/wallets/vega.1639051237294446827`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/vegahome/data/faucet/wallets/vega.1641976836892788243` & `vega_sim-1.2.0/vega_sim/vegahome/data/faucet/wallets/vega.1641976836892788243`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/vegahome/data/faucet/wallets/vega.1641977214518086643` & `vega_sim-1.2.0/vega_sim/vegahome/data/faucet/wallets/vega.1641977214518086643`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/vegahome/data/faucet/wallets/vega.1641977270881740938` & `vega_sim-1.2.0/vega_sim/vegahome/data/faucet/wallets/vega.1641977270881740938`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/vegahome/data/faucet/wallets/vega.1641977376563008654` & `vega_sim-1.2.0/vega_sim/vegahome/data/faucet/wallets/vega.1641977376563008654`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/vegahome/data/faucet/wallets/vega.1641977471442889253` & `vega_sim-1.2.0/vega_sim/vegahome/data/faucet/wallets/vega.1641977471442889253`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/vegahome/data/faucet/wallets/vega.1641977537535784009` & `vega_sim-1.2.0/vega_sim/vegahome/data/faucet/wallets/vega.1641977537535784009`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/vegahome/data/faucet/wallets/vega.1641977956797580358` & `vega_sim-1.2.0/vega_sim/vegahome/data/faucet/wallets/vega.1641977956797580358`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/vegahome/data/faucet/wallets/vega.1641978034856367487` & `vega_sim-1.2.0/vega_sim/vegahome/data/faucet/wallets/vega.1641978034856367487`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/vegahome/data/faucet/wallets/vega.1643100690865690276` & `vega_sim-1.2.0/vega_sim/vegahome/data/faucet/wallets/vega.1643100690865690276`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/vegahome/data/node/wallets/vega/vega.1639051228296308758` & `vega_sim-1.2.0/vega_sim/vegahome/data/node/wallets/vega/vega.1639051228296308758`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/vegahome/data/node/wallets/vega/vega.1641977668033624243` & `vega_sim-1.2.0/vega_sim/vegahome/data/node/wallets/vega/vega.1641977668033624243`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/vegahome/data/node/wallets/vega/vega.1641977838095755067` & `vega_sim-1.2.0/vega_sim/vegahome/data/node/wallets/vega/vega.1641977838095755067`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/vegahome/data/node/wallets/vega/vega.1641977916225009082` & `vega_sim-1.2.0/vega_sim/vegahome/data/node/wallets/vega/vega.1641977916225009082`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/vegahome/data/node/wallets/vega/vega.1641977947934016124` & `vega_sim-1.2.0/vega_sim/vegahome/data/node/wallets/vega/vega.1641977947934016124`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/vegahome/data/wallet-service/rsa-keys/private.pem` & `vega_sim-1.2.0/vega_sim/vegahome/data/wallet-service/rsa-keys/private.pem`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/vegahome/data/wallet-service/rsa-keys/public.pem` & `vega_sim-1.2.0/vega_sim/vegahome/data/wallet-service/rsa-keys/public.pem`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/vegahome/genesis.json` & `vega_sim-1.2.0/vega_sim/vegahome/genesis.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999738930659984%*

 * *Differences: {"'app_state'": "{'network_parameters': {'validators.epoch.length': '5m'}}"}*

```diff
@@ -134,15 +134,15 @@
             "spam.protection.minimumWithdrawalQuantumMultiple": "10",
             "spam.protection.proposal.min.tokens": "2000000000000000000000",
             "spam.protection.voting.min.tokens": "1000000000000000000",
             "transfer.fee.factor": "0.001",
             "transfer.minTransferQuantumMultiple": "100",
             "validator.performance.scaling.factor": "0",
             "validators.delegation.minAmount": "1",
-            "validators.epoch.length": "24h",
+            "validators.epoch.length": "5m",
             "validators.vote.required": "0.67"
         },
         "validators": {
             "6NemqXSfN4zfZvAQeIANflEFqQ98izX9C0KLI2dITSY=": {
                 "avatar_url": "",
                 "country": "",
                 "ethereum_address": "0x9e5BEEC6E56B28cCbd02864840B0f1e0125e42Ce",
```

### Comparing `vega_sim-1.1.1/vega_sim/wallet/base.py` & `vega_sim-1.2.0/vega_sim/wallet/base.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/wallet/slim_wallet.py` & `vega_sim-1.2.0/vega_sim/wallet/slim_wallet.py`

 * *Files identical despite different names*

### Comparing `vega_sim-1.1.1/vega_sim/wallet/vega_wallet.py` & `vega_sim-1.2.0/vega_sim/wallet/vega_wallet.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,14 +119,18 @@
         """
         if self._passphrase_file is None:
             raise Exception("Must set wallet passphrase file path to generate keys")
 
         wallet = (
             wallet_name if wallet_name is not None else self.vega_default_wallet_name
         )
+
+        if wallet not in self.pub_keys:
+            self.create_wallet(name=wallet)
+
         cmd = subprocess.run(
             [
                 self._wallet_path,
                 "key",
                 "generate",
                 "--wallet",
                 wallet,
@@ -186,14 +190,16 @@
                 self._passphrase_file,
                 "--wallet-passphrase-file",
                 self._passphrase_file,
                 "--wallet-name",
                 name,
                 "--description",
                 name,
+                "--output",
+                "json",
             ],
             capture_output=True,
             universal_newlines=True,
             encoding="UTF-8",
         ).stdout
 
         self.login_tokens[name] = json.loads(cmd)["token"]
```

