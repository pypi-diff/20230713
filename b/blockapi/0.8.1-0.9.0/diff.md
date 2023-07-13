# Comparing `tmp/blockapi-0.8.1.tar.gz` & `tmp/blockapi-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockapi-0.8.1.tar", last modified: Wed Nov 30 09:34:40 2022, max compression
+gzip compressed data, was "blockapi-0.9.0.tar", last modified: Wed Nov 30 12:36:34 2022, max compression
```

## Comparing `blockapi-0.8.1.tar` & `blockapi-0.9.0.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 09:34:40.756623 blockapi-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1071 2022-11-30 09:34:00.000000 blockapi-0.8.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (122)     5584 2022-11-30 09:34:40.756623 blockapi-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5365 2022-11-30 09:34:00.000000 blockapi-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 09:34:40.736622 blockapi-0.8.1/blockapi/
--rw-r--r--   0 runner    (1001) docker     (122)     5507 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 09:34:40.744623 blockapi-0.8.1/blockapi/api/
--rw-r--r--   0 runner    (1001) docker     (122)     1165 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12524 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/api/alethio.py
--rw-r--r--   0 runner    (1001) docker     (122)     4414 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/api/amberdata.py
--rw-r--r--   0 runner    (1001) docker     (122)     2095 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/api/binance.py
--rw-r--r--   0 runner    (1001) docker     (122)     2629 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/api/blockchaininfo.py
--rw-r--r--   0 runner    (1001) docker     (122)     3035 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/api/blockchainos.py
--rw-r--r--   0 runner    (1001) docker     (122)     5370 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/api/blockchair.py
--rw-r--r--   0 runner    (1001) docker     (122)     1305 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/api/blockcypher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2167 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/api/blockonomics.py
--rw-r--r--   0 runner    (1001) docker     (122)     2951 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/api/blockscout.py
--rw-r--r--   0 runner    (1001) docker     (122)      804 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/api/btc.py
--rw-r--r--   0 runner    (1001) docker     (122)     2564 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/api/cardanoexplorer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2056 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/api/chainso.py
--rw-r--r--   0 runner    (1001) docker     (122)    11256 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/api/cosmos.py
--rw-r--r--   0 runner    (1001) docker     (122)     1161 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/api/cryptoid.py
--rw-r--r--   0 runner    (1001) docker     (122)     7672 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/api/dcrdata.py
--rw-r--r--   0 runner    (1001) docker     (122)     1094 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/api/digonchain.py
--rw-r--r--   0 runner    (1001) docker     (122)     1764 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/api/eospark.py
--rw-r--r--   0 runner    (1001) docker     (122)     4660 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/api/etherscan.py
--rw-r--r--   0 runner    (1001) docker     (122)     1824 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/api/ethplorer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1126 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/api/greymass.py
--rw-r--r--   0 runner    (1001) docker     (122)     1796 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/api/insight.py
--rw-r--r--   0 runner    (1001) docker     (122)     6523 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/api/kyber.py
--rw-r--r--   0 runner    (1001) docker     (122)     3195 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/api/neoscan.py
--rw-r--r--   0 runner    (1001) docker     (122)     1001 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/api/ontology.py
--rw-r--r--   0 runner    (1001) docker     (122)     4695 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/api/solana.py
--rw-r--r--   0 runner    (1001) docker     (122)     1075 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/api/stellar.py
--rw-r--r--   0 runner    (1001) docker     (122)     7904 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/api/subscan.py
--rw-r--r--   0 runner    (1001) docker     (122)     4000 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/api/terra_money.py
--rw-r--r--   0 runner    (1001) docker     (122)     2472 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/api/trezor.py
--rw-r--r--   0 runner    (1001) docker     (122)     2213 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/api/tronscan.py
--rw-r--r--   0 runner    (1001) docker     (122)    12000 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/api/tzscan.py
--rw-r--r--   0 runner    (1001) docker     (122)      904 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/api/tzstats.py
--rw-r--r--   0 runner    (1001) docker     (122)      735 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/api/zchain.py
--rw-r--r--   0 runner    (1001) docker     (122)      717 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/api/zensystem.py
--rw-r--r--   0 runner    (1001) docker     (122)     6450 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/services.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 09:34:40.744623 blockapi-0.8.1/blockapi/test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 09:34:40.748623 blockapi-0.8.1/blockapi/test/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/test/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      858 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/test/api/test_amberdata.py
--rw-r--r--   0 runner    (1001) docker     (122)      889 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/test/api/test_balances.py
--rw-r--r--   0 runner    (1001) docker     (122)      675 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/test/api/test_binance.py
--rw-r--r--   0 runner    (1001) docker     (122)      610 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/test/api/test_blockchainos.py
--rw-r--r--   0 runner    (1001) docker     (122)      723 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/test/api/test_blockchair.py
--rw-r--r--   0 runner    (1001) docker     (122)      634 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/test/api/test_blockscout.py
--rw-r--r--   0 runner    (1001) docker     (122)      366 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/test/api/test_btc.py
--rw-r--r--   0 runner    (1001) docker     (122)     2029 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/test/api/test_cosmos.py
--rw-r--r--   0 runner    (1001) docker     (122)     2525 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/test/api/test_dcrdata.py
--rw-r--r--   0 runner    (1001) docker     (122)      395 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/test/api/test_digonchain.py
--rw-r--r--   0 runner    (1001) docker     (122)      394 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/test/api/test_insight.py
--rw-r--r--   0 runner    (1001) docker     (122)     2328 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/test/api/test_kyber.py
--rw-r--r--   0 runner    (1001) docker     (122)      287 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/test/api/test_ontio.py
--rw-r--r--   0 runner    (1001) docker     (122)     1039 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/test/api/test_solana.py
--rw-r--r--   0 runner    (1001) docker     (122)     1122 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/test/api/test_subscan.py
--rw-r--r--   0 runner    (1001) docker     (122)     1132 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/test/api/test_terra_money.py
--rw-r--r--   0 runner    (1001) docker     (122)      434 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/test/api/test_tronscan.py
--rw-r--r--   0 runner    (1001) docker     (122)     1191 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/test/api/test_tzscan.py
--rw-r--r--   0 runner    (1001) docker     (122)      764 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/test/api/test_tzstats.py
--rw-r--r--   0 runner    (1001) docker     (122)     5522 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/test/test_blockapi.py
--rw-r--r--   0 runner    (1001) docker     (122)      159 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/test/test_num.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 09:34:40.748623 blockapi-0.8.1/blockapi/test/v2/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/test/v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 09:34:40.748623 blockapi-0.8.1/blockapi/test/v2/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/test/v2/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      450 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/test/v2/api/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 09:34:40.748623 blockapi-0.8.1/blockapi/test/v2/api/covalenth/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/test/v2/api/covalenth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      722 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/test/v2/api/covalenth/test_ethereum.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 09:34:40.748623 blockapi-0.8.1/blockapi/test/v2/api/perpetual/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/test/v2/api/perpetual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1117 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/test/v2/api/perpetual/test_perpetual.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 09:34:40.748623 blockapi-0.8.1/blockapi/test/v2/api/synthetix/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/test/v2/api/synthetix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4005 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/test/v2/api/synthetix/test_synthetix.py
--rw-r--r--   0 runner    (1001) docker     (122)     1903 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/test/v2/api/test_blockchair_btc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1754 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/test/v2/api/test_blockchair_doge.py
--rw-r--r--   0 runner    (1001) docker     (122)      608 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/test/v2/api/test_optimistic_etherscan.py
--rw-r--r--   0 runner    (1001) docker     (122)    10865 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/test/v2/api/test_solana.py
--rw-r--r--   0 runner    (1001) docker     (122)      375 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/test/v2/test_base.py
--rw-r--r--   0 runner    (1001) docker     (122)      288 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/test/v2/test_blockchain_mapping.py
--rw-r--r--   0 runner    (1001) docker     (122)     5224 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/test/v2/test_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     2304 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/test/v2/test_enumerate_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)     2407 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/test/v2/test_generic.py
--rw-r--r--   0 runner    (1001) docker     (122)     1368 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/test/v2/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)     2578 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/test_data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 09:34:40.752623 blockapi-0.8.1/blockapi/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      523 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/utils/datetime.py
--rw-r--r--   0 runner    (1001) docker     (122)     8393 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/utils/ethereum.py
--rw-r--r--   0 runner    (1001) docker     (122)     2646 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/utils/num.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 09:34:40.752623 blockapi-0.8.1/blockapi/v2/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 09:34:40.752623 blockapi-0.8.1/blockapi/v2/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/v2/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6010 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/v2/api/blockchair.py
--rw-r--r--   0 runner    (1001) docker     (122)     5318 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/v2/api/cosmos.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 09:34:40.756623 blockapi-0.8.1/blockapi/v2/api/covalenth/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/v2/api/covalenth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      449 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/v2/api/covalenth/arbitrum.py
--rw-r--r--   0 runner    (1001) docker     (122)      441 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/v2/api/covalenth/astar.py
--rw-r--r--   0 runner    (1001) docker     (122)      453 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/v2/api/covalenth/avalanche.py
--rw-r--r--   0 runner    (1001) docker     (122)      440 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/v2/api/covalenth/axie.py
--rw-r--r--   0 runner    (1001) docker     (122)     3058 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/v2/api/covalenth/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      452 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/v2/api/covalenth/binance_smart_chain.py
--rw-r--r--   0 runner    (1001) docker     (122)      440 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/v2/api/covalenth/ethereum.py
--rw-r--r--   0 runner    (1001) docker     (122)      443 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/v2/api/covalenth/fantom.py
--rw-r--r--   0 runner    (1001) docker     (122)      437 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/v2/api/covalenth/heco.py
--rw-r--r--   0 runner    (1001) docker     (122)      444 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/v2/api/covalenth/iotex.py
--rw-r--r--   0 runner    (1001) docker     (122)      446 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/v2/api/covalenth/klaytn.py
--rw-r--r--   0 runner    (1001) docker     (122)      460 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/v2/api/covalenth/moonbeam.py
--rw-r--r--   0 runner    (1001) docker     (122)      449 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/v2/api/covalenth/palm.py
--rw-r--r--   0 runner    (1001) docker     (122)      449 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/v2/api/covalenth/polygon.py
--rw-r--r--   0 runner    (1001) docker     (122)      436 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/v2/api/covalenth/rsk.py
--rw-r--r--   0 runner    (1001) docker     (122)    15211 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/v2/api/debank.py
--rw-r--r--   0 runner    (1001) docker     (122)     1382 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/v2/api/debank_maps.py
--rw-r--r--   0 runner    (1001) docker     (122)     2984 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/v2/api/ethplorer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1798 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/v2/api/optimistic_etherscan.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 09:34:40.756623 blockapi-0.8.1/blockapi/v2/api/perpetual/
--rw-r--r--   0 runner    (1001) docker     (122)       84 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/v2/api/perpetual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8072 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/v2/api/perpetual/perp_abi.py
--rw-r--r--   0 runner    (1001) docker     (122)     7151 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/v2/api/perpetual/perpetual.py
--rw-r--r--   0 runner    (1001) docker     (122)     5069 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/v2/api/solana.py
--rw-r--r--   0 runner    (1001) docker     (122)     4850 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/v2/api/subscan.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 09:34:40.756623 blockapi-0.8.1/blockapi/v2/api/synthetix/
--rw-r--r--   0 runner    (1001) docker     (122)      182 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/v2/api/synthetix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13997 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/v2/api/synthetix/synthetix.py
--rw-r--r--   0 runner    (1001) docker     (122)   169407 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/v2/api/synthetix/synthetix_abi.py
--rw-r--r--   0 runner    (1001) docker     (122)     8174 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/v2/api/terra.py
--rw-r--r--   0 runner    (1001) docker     (122)     4931 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/v2/api/web3_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3368 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/v2/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     5691 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/v2/blockchain_mapping.py
--rw-r--r--   0 runner    (1001) docker     (122)     8512 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/v2/coins.py
--rw-r--r--   0 runner    (1001) docker     (122)    12898 2022-11-30 09:34:00.000000 blockapi-0.8.1/blockapi/v2/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 09:34:40.736622 blockapi-0.8.1/blockapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5584 2022-11-30 09:34:40.000000 blockapi-0.8.1/blockapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4053 2022-11-30 09:34:40.000000 blockapi-0.8.1/blockapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-30 09:34:40.000000 blockapi-0.8.1/blockapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      209 2022-11-30 09:34:40.000000 blockapi-0.8.1/blockapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2022-11-30 09:34:40.000000 blockapi-0.8.1/blockapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      132 2022-11-30 09:34:00.000000 blockapi-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      119 2022-11-30 09:34:40.756623 blockapi-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      828 2022-11-30 09:34:00.000000 blockapi-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:36:34.815370 blockapi-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1071 2022-11-30 12:36:02.000000 blockapi-0.9.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (122)     5584 2022-11-30 12:36:34.815370 blockapi-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5365 2022-11-30 12:36:02.000000 blockapi-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:36:34.803370 blockapi-0.9.0/blockapi/
+-rw-r--r--   0 runner    (1001) docker     (122)     5507 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:36:34.807370 blockapi-0.9.0/blockapi/api/
+-rw-r--r--   0 runner    (1001) docker     (122)     1165 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12524 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/api/alethio.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4414 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/api/amberdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2095 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/api/binance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2629 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/api/blockchaininfo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3035 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/api/blockchainos.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5370 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/api/blockchair.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1305 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/api/blockcypher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2167 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/api/blockonomics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2951 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/api/blockscout.py
+-rw-r--r--   0 runner    (1001) docker     (122)      804 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/api/btc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2564 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/api/cardanoexplorer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2056 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/api/chainso.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11256 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/api/cosmos.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1161 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/api/cryptoid.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7672 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/api/dcrdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1094 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/api/digonchain.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1764 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/api/eospark.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4660 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/api/etherscan.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1824 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/api/ethplorer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1126 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/api/greymass.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1796 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/api/insight.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6523 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/api/kyber.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3195 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/api/neoscan.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1001 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/api/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4695 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/api/solana.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1075 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/api/stellar.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7904 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/api/subscan.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4000 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/api/terra_money.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2472 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/api/trezor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2213 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/api/tronscan.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12000 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/api/tzscan.py
+-rw-r--r--   0 runner    (1001) docker     (122)      904 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/api/tzstats.py
+-rw-r--r--   0 runner    (1001) docker     (122)      735 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/api/zchain.py
+-rw-r--r--   0 runner    (1001) docker     (122)      717 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/api/zensystem.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6450 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/services.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:36:34.807370 blockapi-0.9.0/blockapi/test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:36:34.807370 blockapi-0.9.0/blockapi/test/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/test/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      858 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/test/api/test_amberdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)      889 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/test/api/test_balances.py
+-rw-r--r--   0 runner    (1001) docker     (122)      675 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/test/api/test_binance.py
+-rw-r--r--   0 runner    (1001) docker     (122)      610 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/test/api/test_blockchainos.py
+-rw-r--r--   0 runner    (1001) docker     (122)      723 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/test/api/test_blockchair.py
+-rw-r--r--   0 runner    (1001) docker     (122)      634 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/test/api/test_blockscout.py
+-rw-r--r--   0 runner    (1001) docker     (122)      366 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/test/api/test_btc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2029 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/test/api/test_cosmos.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2525 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/test/api/test_dcrdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)      395 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/test/api/test_digonchain.py
+-rw-r--r--   0 runner    (1001) docker     (122)      394 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/test/api/test_insight.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2328 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/test/api/test_kyber.py
+-rw-r--r--   0 runner    (1001) docker     (122)      287 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/test/api/test_ontio.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1039 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/test/api/test_solana.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1122 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/test/api/test_subscan.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1132 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/test/api/test_terra_money.py
+-rw-r--r--   0 runner    (1001) docker     (122)      434 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/test/api/test_tronscan.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1191 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/test/api/test_tzscan.py
+-rw-r--r--   0 runner    (1001) docker     (122)      764 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/test/api/test_tzstats.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5522 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/test/test_blockapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)      159 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/test/test_num.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:36:34.807370 blockapi-0.9.0/blockapi/test/v2/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/test/v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:36:34.807370 blockapi-0.9.0/blockapi/test/v2/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/test/v2/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      450 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/test/v2/api/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:36:34.807370 blockapi-0.9.0/blockapi/test/v2/api/covalenth/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/test/v2/api/covalenth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      722 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/test/v2/api/covalenth/test_ethereum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:36:34.811370 blockapi-0.9.0/blockapi/test/v2/api/perpetual/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/test/v2/api/perpetual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1117 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/test/v2/api/perpetual/test_perpetual.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:36:34.811370 blockapi-0.9.0/blockapi/test/v2/api/synthetix/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/test/v2/api/synthetix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4005 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/test/v2/api/synthetix/test_synthetix.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1903 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/test/v2/api/test_blockchair_btc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1754 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/test/v2/api/test_blockchair_doge.py
+-rw-r--r--   0 runner    (1001) docker     (122)      608 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/test/v2/api/test_optimistic_etherscan.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10865 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/test/v2/api/test_solana.py
+-rw-r--r--   0 runner    (1001) docker     (122)      375 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/test/v2/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      288 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/test/v2/test_blockchain_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5529 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/test/v2/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2304 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/test/v2/test_enumerate_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2407 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/test/v2/test_generic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1368 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/test/v2/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2578 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:36:34.811370 blockapi-0.9.0/blockapi/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      523 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/utils/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8393 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/utils/ethereum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2646 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/utils/num.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:36:34.811370 blockapi-0.9.0/blockapi/v2/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:36:34.811370 blockapi-0.9.0/blockapi/v2/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/v2/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6010 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/v2/api/blockchair.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5318 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/v2/api/cosmos.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:36:34.811370 blockapi-0.9.0/blockapi/v2/api/covalenth/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/v2/api/covalenth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      449 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/v2/api/covalenth/arbitrum.py
+-rw-r--r--   0 runner    (1001) docker     (122)      441 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/v2/api/covalenth/astar.py
+-rw-r--r--   0 runner    (1001) docker     (122)      453 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/v2/api/covalenth/avalanche.py
+-rw-r--r--   0 runner    (1001) docker     (122)      440 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/v2/api/covalenth/axie.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3058 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/v2/api/covalenth/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      452 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/v2/api/covalenth/binance_smart_chain.py
+-rw-r--r--   0 runner    (1001) docker     (122)      440 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/v2/api/covalenth/ethereum.py
+-rw-r--r--   0 runner    (1001) docker     (122)      443 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/v2/api/covalenth/fantom.py
+-rw-r--r--   0 runner    (1001) docker     (122)      437 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/v2/api/covalenth/heco.py
+-rw-r--r--   0 runner    (1001) docker     (122)      444 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/v2/api/covalenth/iotex.py
+-rw-r--r--   0 runner    (1001) docker     (122)      446 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/v2/api/covalenth/klaytn.py
+-rw-r--r--   0 runner    (1001) docker     (122)      460 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/v2/api/covalenth/moonbeam.py
+-rw-r--r--   0 runner    (1001) docker     (122)      449 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/v2/api/covalenth/palm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      449 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/v2/api/covalenth/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (122)      436 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/v2/api/covalenth/rsk.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15211 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/v2/api/debank.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1382 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/v2/api/debank_maps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2984 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/v2/api/ethplorer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1798 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/v2/api/optimistic_etherscan.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:36:34.811370 blockapi-0.9.0/blockapi/v2/api/perpetual/
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/v2/api/perpetual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8072 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/v2/api/perpetual/perp_abi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7151 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/v2/api/perpetual/perpetual.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5069 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/v2/api/solana.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5367 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/v2/api/subscan.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:36:34.811370 blockapi-0.9.0/blockapi/v2/api/synthetix/
+-rw-r--r--   0 runner    (1001) docker     (122)      182 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/v2/api/synthetix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13997 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/v2/api/synthetix/synthetix.py
+-rw-r--r--   0 runner    (1001) docker     (122)   169407 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/v2/api/synthetix/synthetix_abi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8174 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/v2/api/terra.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4931 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/v2/api/web3_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3368 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/v2/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5691 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/v2/blockchain_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8679 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/v2/coins.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12920 2022-11-30 12:36:02.000000 blockapi-0.9.0/blockapi/v2/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:36:34.803370 blockapi-0.9.0/blockapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5584 2022-11-30 12:36:34.000000 blockapi-0.9.0/blockapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4053 2022-11-30 12:36:34.000000 blockapi-0.9.0/blockapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-30 12:36:34.000000 blockapi-0.9.0/blockapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2022-11-30 12:36:34.000000 blockapi-0.9.0/blockapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2022-11-30 12:36:34.000000 blockapi-0.9.0/blockapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2022-11-30 12:36:02.000000 blockapi-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      119 2022-11-30 12:36:34.815370 blockapi-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      828 2022-11-30 12:36:02.000000 blockapi-0.9.0/setup.py
```

### Comparing `blockapi-0.8.1/LICENSE.md` & `blockapi-0.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/PKG-INFO` & `blockapi-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blockapi
-Version: 0.8.1
+Version: 0.9.0
 Summary: BlockAPI library
 Home-page: UNKNOWN
 Author: Devmons s.r.o.
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `blockapi-0.8.1/README.md` & `blockapi-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/__init__.py` & `blockapi-0.9.0/blockapi/__init__.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/api/__init__.py` & `blockapi-0.9.0/blockapi/api/__init__.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/api/alethio.py` & `blockapi-0.9.0/blockapi/api/alethio.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/api/amberdata.py` & `blockapi-0.9.0/blockapi/api/amberdata.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/api/binance.py` & `blockapi-0.9.0/blockapi/api/binance.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/api/blockchaininfo.py` & `blockapi-0.9.0/blockapi/api/blockchaininfo.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/api/blockchainos.py` & `blockapi-0.9.0/blockapi/api/blockchainos.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/api/blockchair.py` & `blockapi-0.9.0/blockapi/api/blockchair.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/api/blockcypher.py` & `blockapi-0.9.0/blockapi/api/blockcypher.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/api/blockonomics.py` & `blockapi-0.9.0/blockapi/api/blockonomics.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/api/blockscout.py` & `blockapi-0.9.0/blockapi/api/blockscout.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/api/btc.py` & `blockapi-0.9.0/blockapi/api/btc.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/api/cardanoexplorer.py` & `blockapi-0.9.0/blockapi/api/cardanoexplorer.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/api/chainso.py` & `blockapi-0.9.0/blockapi/api/chainso.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/api/cosmos.py` & `blockapi-0.9.0/blockapi/api/cosmos.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/api/cryptoid.py` & `blockapi-0.9.0/blockapi/api/cryptoid.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/api/dcrdata.py` & `blockapi-0.9.0/blockapi/api/dcrdata.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/api/digonchain.py` & `blockapi-0.9.0/blockapi/api/digonchain.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/api/eospark.py` & `blockapi-0.9.0/blockapi/api/eospark.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/api/etherscan.py` & `blockapi-0.9.0/blockapi/api/etherscan.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/api/ethplorer.py` & `blockapi-0.9.0/blockapi/api/ethplorer.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/api/greymass.py` & `blockapi-0.9.0/blockapi/api/greymass.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/api/insight.py` & `blockapi-0.9.0/blockapi/api/insight.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/api/kyber.py` & `blockapi-0.9.0/blockapi/api/kyber.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/api/neoscan.py` & `blockapi-0.9.0/blockapi/api/neoscan.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/api/ontology.py` & `blockapi-0.9.0/blockapi/api/ontology.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/api/solana.py` & `blockapi-0.9.0/blockapi/api/solana.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/api/stellar.py` & `blockapi-0.9.0/blockapi/api/stellar.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/api/subscan.py` & `blockapi-0.9.0/blockapi/api/subscan.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/api/terra_money.py` & `blockapi-0.9.0/blockapi/api/terra_money.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/api/trezor.py` & `blockapi-0.9.0/blockapi/api/trezor.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/api/tronscan.py` & `blockapi-0.9.0/blockapi/api/tronscan.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/api/tzscan.py` & `blockapi-0.9.0/blockapi/api/tzscan.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/api/tzstats.py` & `blockapi-0.9.0/blockapi/api/tzstats.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/api/zchain.py` & `blockapi-0.9.0/blockapi/api/zchain.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/api/zensystem.py` & `blockapi-0.9.0/blockapi/api/zensystem.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/services.py` & `blockapi-0.9.0/blockapi/services.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/test/api/test_amberdata.py` & `blockapi-0.9.0/blockapi/test/api/test_amberdata.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/test/api/test_balances.py` & `blockapi-0.9.0/blockapi/test/api/test_balances.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/test/api/test_binance.py` & `blockapi-0.9.0/blockapi/test/api/test_binance.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/test/api/test_blockchainos.py` & `blockapi-0.9.0/blockapi/test/api/test_blockchainos.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/test/api/test_blockchair.py` & `blockapi-0.9.0/blockapi/test/api/test_blockchair.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/test/api/test_blockscout.py` & `blockapi-0.9.0/blockapi/test/api/test_blockscout.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/test/api/test_cosmos.py` & `blockapi-0.9.0/blockapi/test/api/test_cosmos.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/test/api/test_dcrdata.py` & `blockapi-0.9.0/blockapi/test/api/test_dcrdata.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/test/api/test_kyber.py` & `blockapi-0.9.0/blockapi/test/api/test_kyber.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/test/api/test_solana.py` & `blockapi-0.9.0/blockapi/test/api/test_solana.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/test/api/test_subscan.py` & `blockapi-0.9.0/blockapi/test/api/test_subscan.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/test/api/test_terra_money.py` & `blockapi-0.9.0/blockapi/test/api/test_terra_money.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/test/api/test_tzscan.py` & `blockapi-0.9.0/blockapi/test/api/test_tzscan.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/test/api/test_tzstats.py` & `blockapi-0.9.0/blockapi/test/api/test_tzstats.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/test/test_blockapi.py` & `blockapi-0.9.0/blockapi/test/test_blockapi.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/test/v2/api/covalenth/test_ethereum.py` & `blockapi-0.9.0/blockapi/test/v2/api/covalenth/test_ethereum.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/test/v2/api/perpetual/test_perpetual.py` & `blockapi-0.9.0/blockapi/test/v2/api/perpetual/test_perpetual.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/test/v2/api/synthetix/test_synthetix.py` & `blockapi-0.9.0/blockapi/test/v2/api/synthetix/test_synthetix.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/test/v2/api/test_blockchair_btc.py` & `blockapi-0.9.0/blockapi/test/v2/api/test_blockchair_btc.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/test/v2/api/test_blockchair_doge.py` & `blockapi-0.9.0/blockapi/test/v2/api/test_blockchair_doge.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/test/v2/api/test_optimistic_etherscan.py` & `blockapi-0.9.0/blockapi/test/v2/api/test_optimistic_etherscan.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/test/v2/api/test_solana.py` & `blockapi-0.9.0/blockapi/test/v2/api/test_solana.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/test/v2/test_data.py` & `blockapi-0.9.0/blockapi/test/v2/test_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from blockapi.v2.api.covalenth.polygon import PolygonCovalentApi
 from blockapi.v2.api.covalenth.rsk import RskCovalentApi
 from blockapi.v2.api.debank import DebankApi
 from blockapi.v2.api.ethplorer import EthplorerApi
 from blockapi.v2.api.optimistic_etherscan import OptimismEtherscanApi
 from blockapi.v2.api.perpetual import PerpetualApi
 from blockapi.v2.api.solana import SolanaApi
-from blockapi.v2.api.subscan import PolkadotSubscanApi
+from blockapi.v2.api.subscan import KusamaSubscanApi, PolkadotSubscanApi, SubscanApi
 from blockapi.v2.api.synthetix import SynthetixApi
 from blockapi.v2.api.terra import TerraApi
 
 # TODO create method for auto loading all classes
 from blockapi.v2.base import IBalance
 from blockapi.v2.coins import (
     COIN_ATOM,
@@ -36,14 +36,15 @@
     COIN_BNB,
     COIN_DOT,
     COIN_ETH,
     COIN_FTM,
     COIN_HT,
     COIN_IOTX,
     COIN_KLAY,
+    COIN_KSM,
     COIN_MATIC,
     COIN_MOVR,
     COIN_PALM,
     COIN_RON,
     COIN_RSK,
     COIN_SDN,
     COIN_SOL,
@@ -70,14 +71,15 @@
     MoonBeamCovalentApi,
     PalmCovalentApi,
     PolygonCovalentApi,
     RskCovalentApi,
     OptimismEtherscanApi,
     DebankApi,
     PolkadotSubscanApi,
+    KusamaSubscanApi,
     CosmosApi,
     SynthetixApi,
     PerpetualApi,
     BlockchairBitcoinApi,
 ]
 
 NON_EMPTY_VALID_ADDRESSES_BY_SYMBOL = {
@@ -124,14 +126,15 @@
         '0xfc43f5f9dd45258b3aff31bdbe6561d97e8b71de',
     ],
     COIN_RSK.symbol: [
         '0xfc43f5f9dd45258b3aff31bdbe6561d97e8b71de',
     ],
     COIN_DOT.symbol: ['15j4dg5GzsL1bw2U2AWgeyAk6QTxq43V7ZPbXdAmbVLjvDCK'],
     COIN_ATOM.symbol: ['cosmos1r4v9t46zyu6df0jwtmtpn0pq864dpn7c5sha5u'],
+    COIN_KSM.symbol: ['EK8HP4biJ8FBktaREBd9Bt3E85QsVTmpYzn5aou7iiUDDgB'],
 }
 
 BAD_ADDRESSES = [
     '1',
     '10000',
     'AAAAA',
     '0x123',
@@ -158,15 +161,23 @@
 
 
 def yield_api_ibalance_classes():
     return [
         x
         for x in IBalance.__subclasses__()
         if not issubclass(
-            x, (CosmosApiBase, CovalentApiBase, DebankApi, PerpetualApi, SynthetixApi)
+            x,
+            (
+                CosmosApiBase,
+                CovalentApiBase,
+                DebankApi,
+                PerpetualApi,
+                SynthetixApi,
+                SubscanApi,
+            ),
         )
         and not inspect.isabstract(x)
     ]
 
 
 def yield_all_api_classes():
     return [x for x in IBalance.__subclasses__()]
@@ -175,14 +186,15 @@
 def get_debank_addresses():
     result = []
     for key, items in NON_EMPTY_VALID_ADDRESSES_BY_SYMBOL.items():
         if key in (
             COIN_TERRA.symbol,
             COIN_SOL.symbol,
             COIN_DOT.symbol,
+            COIN_KSM.symbol,
             COIN_ATOM.symbol,
         ):
             continue
 
         for item in items:
             result.append(pytest.param(item, id=key))
```

### Comparing `blockapi-0.8.1/blockapi/test/v2/test_enumerate_classes.py` & `blockapi-0.9.0/blockapi/test/v2/test_enumerate_classes.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/test/v2/test_generic.py` & `blockapi-0.9.0/blockapi/test/v2/test_generic.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/test/v2/test_models.py` & `blockapi-0.9.0/blockapi/test/v2/test_models.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/test_data.py` & `blockapi-0.9.0/blockapi/test_data.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/utils/datetime.py` & `blockapi-0.9.0/blockapi/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/utils/ethereum.py` & `blockapi-0.9.0/blockapi/utils/ethereum.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/utils/num.py` & `blockapi-0.9.0/blockapi/utils/num.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/v2/api/blockchair.py` & `blockapi-0.9.0/blockapi/v2/api/blockchair.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/v2/api/cosmos.py` & `blockapi-0.9.0/blockapi/v2/api/cosmos.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/v2/api/covalenth/base.py` & `blockapi-0.9.0/blockapi/v2/api/covalenth/base.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/v2/api/debank.py` & `blockapi-0.9.0/blockapi/v2/api/debank.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/v2/api/debank_maps.py` & `blockapi-0.9.0/blockapi/v2/api/debank_maps.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/v2/api/ethplorer.py` & `blockapi-0.9.0/blockapi/v2/api/ethplorer.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/v2/api/optimistic_etherscan.py` & `blockapi-0.9.0/blockapi/v2/api/optimistic_etherscan.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/v2/api/perpetual/perp_abi.py` & `blockapi-0.9.0/blockapi/v2/api/perpetual/perp_abi.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/v2/api/perpetual/perpetual.py` & `blockapi-0.9.0/blockapi/v2/api/perpetual/perpetual.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/v2/api/solana.py` & `blockapi-0.9.0/blockapi/v2/api/solana.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/v2/api/subscan.py` & `blockapi-0.9.0/blockapi/v2/api/subscan.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,34 @@
 import json
+from abc import ABC
 from decimal import Decimal
 from typing import Iterable, List, Optional
 
 from requests import Response
 
 from blockapi.utils.num import decimals_to_raw, safe_opt_decimal, to_decimal
 from blockapi.v2.base import (
     ApiException,
     ApiOptions,
     BlockchainApi,
     IBalance,
     InvalidAddressException,
 )
-from blockapi.v2.coins import COIN_DOT
+from blockapi.v2.coins import COIN_DOT, COIN_KSM
 from blockapi.v2.models import AssetType, BalanceItem, Blockchain
 
 
-class PolkadotSubscanApi(BlockchainApi, IBalance):
+class SubscanApi(BlockchainApi, IBalance, ABC):
     """
     API docs: https://docs.api.subscan.io/
     Explorer: https://www.subscan.io
     """
 
-    coin = COIN_DOT
-    api_options = ApiOptions(
-        blockchain=Blockchain.POLKADOT,
-        base_url='https://polkadot.api.subscan.io',
-        start_offset=0,
-        max_items_per_page=100,
-        page_offset_step=1,
-    )
+    coin = None
+    api_options = None
 
     supported_requests = {
         'get_balance': '/api/v2/scan/search',
         'get_rewards': '/api/v2/scan/account/reward_slash',
     }
 
     def get_balance(self, address: str) -> List[BalanceItem]:
@@ -149,7 +144,31 @@
         json_response = response.json()
         code = json_response.get('code')
 
         if code == 10004:
             raise InvalidAddressException('Invalid address format.')
         elif code:
             raise ApiException(json_response['message'])
+
+    @staticmethod
+    def _get_api_options(blockchain: Blockchain, base_url: str) -> ApiOptions:
+        return ApiOptions(
+            blockchain=blockchain,
+            base_url=base_url,
+            start_offset=0,
+            max_items_per_page=100,
+            page_offset_step=1,
+        )
+
+
+class PolkadotSubscanApi(SubscanApi):
+    coin = COIN_DOT
+    api_options = SubscanApi._get_api_options(
+        blockchain=Blockchain.POLKADOT, base_url='https://polkadot.api.subscan.io'
+    )
+
+
+class KusamaSubscanApi(SubscanApi):
+    coin = COIN_KSM
+    api_options = SubscanApi._get_api_options(
+        blockchain=Blockchain.KUSAMA, base_url='https://kusama.api.subscan.io'
+    )
```

### Comparing `blockapi-0.8.1/blockapi/v2/api/synthetix/synthetix.py` & `blockapi-0.9.0/blockapi/v2/api/synthetix/synthetix.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/v2/api/synthetix/synthetix_abi.py` & `blockapi-0.9.0/blockapi/v2/api/synthetix/synthetix_abi.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/v2/api/terra.py` & `blockapi-0.9.0/blockapi/v2/api/terra.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/v2/api/web3_utils.py` & `blockapi-0.9.0/blockapi/v2/api/web3_utils.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/v2/base.py` & `blockapi-0.9.0/blockapi/v2/base.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/v2/blockchain_mapping.py` & `blockapi-0.9.0/blockapi/v2/blockchain_mapping.py`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/blockapi/v2/coins.py` & `blockapi-0.9.0/blockapi/v2/coins.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,14 +193,22 @@
     symbol='DOT',
     name='Polkadot',
     decimals=10,
     blockchain=Blockchain.POLKADOT,
     info=CoinInfo(coingecko_id='polkadot', tags=['native']),
 )
 
+COIN_KSM = Coin(
+    symbol='KSM',
+    name='Kusama',
+    decimals=12,
+    blockchain=Blockchain.KUSAMA,
+    info=CoinInfo(coingecko_id='kusama', tags=['native']),
+)
+
 COIN_ATOM = Coin(
     symbol='ATOM',
     name='Cosmos Hub',
     decimals=6,
     blockchain=Blockchain.COSMOS,
     address='uatom',
     standards=['staking'],
```

### Comparing `blockapi-0.8.1/blockapi/v2/models.py` & `blockapi-0.9.0/blockapi/v2/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,14 +60,15 @@
     IRIS = 'iris'
     JUNO = 'juno'
     KAVA_EVM = 'kava_evm'
     KCC = 'kcc'
     KLAYTN = 'klaytn'
     KLAYTN_CYPRESS = 'klaytn_cypress'
     KU_COIN = 'ku-coin'
+    KUSAMA = 'kusama'
     LITECOIN = 'litecoin'
     METIS = 'metis'
     MILKOMEDA_C1 = 'milkomeda_c1'
     MOONBEAM = 'moonbeam'
     MOONBEAM_MOONRIVER = 'moonbeam-moonriver'
     MOONRIVER = 'moonriver'
     OASIS = 'oasis'
```

### Comparing `blockapi-0.8.1/blockapi.egg-info/PKG-INFO` & `blockapi-0.9.0/blockapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blockapi
-Version: 0.8.1
+Version: 0.9.0
 Summary: BlockAPI library
 Home-page: UNKNOWN
 Author: Devmons s.r.o.
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `blockapi-0.8.1/blockapi.egg-info/SOURCES.txt` & `blockapi-0.9.0/blockapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blockapi-0.8.1/setup.py` & `blockapi-0.9.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 PACKAGES = find_packages(where='.')
 
-__version__ = "0.8.1"
+__version__ = "0.9.0"
 
 setuptools.setup(
     name='blockapi',
     version=__version__,
     author='Devmons s.r.o.',
     description='BlockAPI library',
     license='MIT',
```

